# Comparing `tmp/speedtab-0.1.2.4.tar.gz` & `tmp/speedtab-0.1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speedtab-0.1.2.4.tar", max compression
+gzip compressed data, was "speedtab-0.1.3.0.tar", max compression
```

## Comparing `speedtab-0.1.2.4.tar` & `speedtab-0.1.3.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      567 2023-04-18 16:11:48.088583 speedtab-0.1.2.4/pyproject.toml
--rw-r--r--   0        0        0      352 2022-09-07 08:00:08.177672 speedtab-0.1.2.4/speedtab/__init__.py
--rw-r--r--   0        0        0    35875 2023-04-18 16:08:09.813649 speedtab-0.1.2.4/speedtab/client.py
--rw-r--r--   0        0        0     5857 2022-10-11 09:11:17.745858 speedtab-0.1.2.4/speedtab/enums.py
--rw-r--r--   0        0        0     1744 2022-08-23 18:18:16.848628 speedtab-0.1.2.4/speedtab/formats.py
--rw-r--r--   0        0        0      783 2023-04-18 16:11:56.243762 speedtab-0.1.2.4/setup.py
--rw-r--r--   0        0        0      808 2023-04-18 16:11:56.243762 speedtab-0.1.2.4/PKG-INFO
+-rw-r--r--   0        0        0      567 2023-05-16 16:02:58.325475 speedtab-0.1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      352 2022-09-07 08:00:08.177672 speedtab-0.1.3.0/speedtab/__init__.py
+-rw-r--r--   0        0        0    45758 2023-05-16 16:01:38.620493 speedtab-0.1.3.0/speedtab/client.py
+-rw-r--r--   0        0        0     5857 2022-10-11 09:11:17.745858 speedtab-0.1.3.0/speedtab/enums.py
+-rw-r--r--   0        0        0     1744 2022-08-23 18:18:16.848628 speedtab-0.1.3.0/speedtab/formats.py
+-rw-r--r--   0        0        0      783 2023-05-16 16:03:56.700500 speedtab-0.1.3.0/setup.py
+-rw-r--r--   0        0        0      808 2023-05-16 16:03:56.701500 speedtab-0.1.3.0/PKG-INFO
```

### Comparing `speedtab-0.1.2.4/pyproject.toml` & `speedtab-0.1.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "speedtab"
-version = "0.1.2.4"
+version = "0.1.3.0"
 description = "Convenient wrapper for working with Google Spreadsheets"
 authors = ["Bogdan Gergel <bogger147@gmail.com>"]
 license = "MIT"
 homepage = "https://github.com/BoggerSancho/SpeedTab-beta"
 repository = "https://github.com/BoggerSancho/SpeedTab-beta"
 
 [tool.poetry.dependencies]
```

### Comparing `speedtab-0.1.2.4/speedtab/client.py` & `speedtab-0.1.3.0/speedtab/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -92,15 +92,20 @@
     if isinstance(input_range, str):
         input_range = input_range.split(':') + [''] if len(input_range.split(':')) == 1 else input_range.split(':')
         cells = sum(tuple(sheet_cell_to_index(x) for x in input_range), ())
     else:
         cells = input_range + (None,)*4
     return cells
 
-depth = lambda l: isinstance(l, list) and max(map(depth, l)) + 1
+
+def depth(l):
+    if isinstance(l, (list, tuple)):
+        return max(map(depth, l)) + 1
+    else:
+        return 0
 
 
 class BooleanCondition:
     def __init__(self, type: BooleanConditionTypes, value):
         self.type = type.value
         self.value = value
 
@@ -111,20 +116,20 @@
                     'type': self.type,
                     'values': [
                         {'userEnteredValue': self.value}
                     ]}}}
 
 
 class Task:
-    def __init__(self, task_type, position, sheetId, task, data_cell=None):
+    def __init__(self, task_type, position, sheetId, task, work_zone):
         self.task_type = task_type
         self.position = position
         self.sheetId = sheetId
         self.task = task
-        self.data_cell = data_cell
+        self.work_zone = work_zone
 
 
 class SpreedSheet:
     def __init__(self, spreadsheet_id, token_path, credentials, connect):
         self.spreadsheet_id = spreadsheet_id
         self.token_path = token_path
         self.credentials = credentials
@@ -150,32 +155,43 @@
                     shift = []
             if shift:
                 merged_group.append(shift)
 
             groups.append(merged_group)
 
         full_groups = [sorted(sum(x, []), key=lambda x: (TYPE_ORDER[x.task_type], x.position)) for x in zip_longest(*groups, fillvalue=[])]
+
         curr_size = {}
+        new_size = {}
         for sheet in self.sheets.values():
             curr_size[sheet.get('sheetId')] = [sheet.get('max_row'), sheet.get('max_column')]
+            new_size[sheet.get('sheetId')] = [sheet.get('max_row'), sheet.get('max_column')]
 
         for group in full_groups:
             for task in group:
                 if task.task_type == 'clear' and 'updateSheetProperties' in task.task.keys():
                     vals = task.task.get('updateSheetProperties').get('properties').get('gridProperties')
-                    curr_size[task.sheetId] = [vals.get('rowCount'), vals.get('columnCount')]
+                    new_size[task.sheetId] = [vals.get('rowCount'), vals.get('columnCount')]
                 elif task.task_type == 'clear' and 'appendDimension' in task.task.keys():
                     vals = task.task.get('appendDimension')
                     if vals.get('dimension') == 'ROWS':
-                        curr_size[task.sheetId][0] += vals.get('length')
+                        new_size[task.sheetId][0] = max(curr_size[task.get('sheetId')][0] + vals.get('length'), new_size[task.sheetId][0])
                     if vals.get('dimension') == 'COLUMNS':
-                        curr_size[task.sheetId][1] += vals.get('length')
+                        new_size[task.sheetId][1] = max(curr_size[task.get('sheetId')][1] + vals.get('length'), new_size[task.sheetId][1])
                 elif task.task_type == 'data':
-                    curr_size[task.sheetId] = [max(curr_size[task.sheetId][0], task.data_cell[0] + 1),
-                                               max(curr_size[task.sheetId][1], task.data_cell[1] + 1)]
+                    new_size[task.sheetId] = [
+                        max(new_size[task.sheetId][0],
+                            task.work_zone.get('startRowIndex', 0) if task.work_zone.get('startRowIndex', 0) is not None else 0,
+                            task.work_zone.get('endRowIndex', 0) if task.work_zone.get('endRowIndex', 0) is not None else 0
+                            ),
+                        max(new_size[task.sheetId][1],
+                            task.work_zone.get('startColumnIndex', 0) if task.work_zone.get('startColumnIndex', 0) is not None else 0,
+                            task.work_zone.get('endColumnIndex', 0) if task.work_zone.get('endColumnIndex', 0) is not None else 0
+                            )
+                    ]
             for key, (rows, columns) in curr_size.items():
                 self._set_sheet_size(rows, columns, key, group)
 
         return [sorted(group, key=lambda x: (TYPE_ORDER[x.task_type], x.position)) for group in full_groups]
 
     def _set_sheet_size(self, rows: int, columns: int, sheet_id, group):
         group.append(Task('format', len(self._task_queue), sheet_id, {
@@ -184,15 +200,15 @@
                     'gridProperties': {
                         'rowCount': rows,
                         'columnCount': columns,
                     },
                     'sheetId': sheet_id,
                 },
                 'fields': 'gridProperties.rowCount, gridProperties.columnCount',
-            }}))
+            }}, None))
 
     def _get_metadata(self):
         metadata = self.connect_v4.spreadsheets().get(spreadsheetId=self.spreadsheet_id).execute()
         self.sheets = dict(
             [(prop.get('title'), {
                 'max_column': prop.get('gridProperties').get('columnCount'),
                 'max_row': prop.get('gridProperties').get('rowCount'),
@@ -212,14 +228,15 @@
             for task in group:
                 if task.task_type == 'data':
                     batch_update_data_list.append(task.task)
                 elif task.task_type == 'chart':
                     batch_update_chart_list.append(task.task)
                 else:
                     batch_update_list.append(task.task)
+
             if batch_update_list:
                 self.connect_v4.spreadsheets().batchUpdate(**{
                     'spreadsheetId': self.spreadsheet_id,
                     'body': {
                         'requests': batch_update_list
                     }}).execute()
 
@@ -243,25 +260,25 @@
             'body': {
                 'requests': [{
                     'addSheet': {
                         'properties': {
                             'title': title,
                             'gridProperties': {
                                 'rowCount': 100,
-                                'columnCount': 100,
+                                'columnCount': 26,
                             }}}} for title in sheets]
             }}).execute()
         self._get_metadata()
         return self
 
     def delete_sheets(self, sheets):
         for sheet in sheets:
             self._task_queue.append(Task('format', len(self._task_queue), self.sheets.get(sheet).get('sheetId'), {
                 'deleteSheet': {
-                    'sheetId': self.sheets.get(sheet).get('sheetId')}}))
+                    'sheetId': self.sheets.get(sheet).get('sheetId')}}, self.work_zone))
         return self
 
     def sheet(self, sheet_name):
         return Sheet(sheet_name, self.sheets.get(sheet_name).get('sheetId'), self._task_queue, self.sheets, self)
 
 
 class Range:
@@ -272,14 +289,146 @@
         self.start_data_cell = start_data_cell
         self.base = base
         self.data_cell = data_cell
 
     def _increment_task(self):
         return len(self._task_queue)
 
+    def add_combo_chart(self,
+                        data_start,
+                        left_columns,
+                        right_columns,
+                        chart_type_left: ChartType = ChartType.COLUMN,
+                        chart_type_right: ChartType = ChartType.LINE,
+                        index_column: int = 0,
+                        stacked_type: StackedType = StackedType.NONE,
+                        title: str = None,
+                        legend_position: LegendPosition = LegendPosition.BOTTOM_LEGEND,
+                        x_axis_name: str = None,
+                        y_axis_name_left: str = None,
+                        y_axis_name_right: str = None,
+                        y_axis_fmt_left: str = None,
+                        y_axis_fmt_right: str = None,
+                        y_axis_min_left: float = None,
+                        y_axis_min_right: float = None,
+                        y_axis_max_left: float = None,
+                        y_axis_max_right: float = None,
+                        x_scale: int = 1,
+                        y_scale: int = 1,
+                        offset_x_pixels: int = 0,
+                        offset_y_pixels: int = 0,
+                        data_sheet_name=None,
+                        header_count: int = 1,
+                        nrows: int = None
+                        ):
+
+        data_start_cell = parse_range(data_start)
+        series = [{
+            'series': {
+                'sourceRange': {
+                    'sources': [
+                        {
+                            'sheetId': self.sheet_id if not data_sheet_name else self.base.sheets.get(data_sheet_name).get('sheetId'),
+                            'startRowIndex': data_start_cell[0],
+                            'endRowIndex': data_start_cell[0] + nrows + 1 if nrows is not None else None,
+                            'startColumnIndex': data_start_cell[1] + column,
+                            'endColumnIndex': data_start_cell[1] + column + 1,
+                        }
+                    ]
+                }
+            },
+            'targetAxis': 'LEFT_AXIS',
+            'type': chart_type_left.value,
+        } for column in left_columns] + [{
+            'series': {
+                'sourceRange': {
+                    'sources': [
+                        {
+                            'sheetId': self.sheet_id if not data_sheet_name else self.base.sheets.get(data_sheet_name).get('sheetId'),
+                            'startRowIndex': data_start_cell[0],
+                            'endRowIndex': data_start_cell[0] + nrows + 1 if nrows is not None else None,
+                            'startColumnIndex': data_start_cell[1] + column,
+                            'endColumnIndex': data_start_cell[1] + column + 1,
+                        }
+                    ]
+                }
+            },
+            'targetAxis': 'RIGHT_AXIS',
+            'type': chart_type_right.value,
+        } for column in right_columns]
+
+        self._task_queue.append(Task('chart', self._increment_task(), self.sheet_id, {
+            'addChart': {
+                'chart': {
+                    'spec': {
+                        'title': title,
+                        'basicChart': {
+                            'chartType': 'COMBO',
+                            'stackedType': stacked_type.value,
+                            'legendPosition': legend_position.value,
+                            'axis': [
+                                {
+                                    'position': 'BOTTOM_AXIS',
+                                    'title': x_axis_name,
+                                },
+                                {
+                                    'position': 'LEFT_AXIS',
+                                    'title': y_axis_name_left,
+                                    'format': y_axis_fmt_left,
+                                    'viewWindowOptions': {
+                                        'viewWindowMin': y_axis_min_left,
+                                        'viewWindowMax': y_axis_max_left,
+                                    },
+                                },
+                                {
+                                    'position': 'RIGHT_AXIS',
+                                    'title': y_axis_name_right,
+                                    'format': y_axis_fmt_right,
+                                    'viewWindowOptions': {
+                                        'viewWindowMin': y_axis_min_right,
+                                        'viewWindowMax': y_axis_max_right,
+                                    },
+                                },
+                            ],
+                            'domains': [
+                                {
+                                    'domain': {
+                                        'sourceRange': {
+                                            'sources': [
+                                                {
+                                                    'sheetId': self.sheet_id if not data_sheet_name else self.base.sheets.get(data_sheet_name).get('sheetId'),
+                                                    'startRowIndex': data_start_cell[0],
+                                                    'endRowIndex': data_start_cell[0] + nrows + 1 if nrows is not None else None,
+                                                    'startColumnIndex': data_start_cell[1] + index_column,
+                                                    'endColumnIndex': data_start_cell[1] + index_column + 1,
+                                                }
+                                            ]
+                                        }
+                                    }
+                                }
+                            ],
+                            'series': [*series],
+                            'headerCount': header_count
+                        }
+                    },
+                    'position': {
+                        'overlayPosition': {
+                            'anchorCell': {
+                                'sheetId': self.sheet_id,
+                                'rowIndex': self.work_zone.get('startRowIndex'),
+                                'columnIndex': self.work_zone.get('startColumnIndex'),
+                            },
+                            'offsetXPixels': offset_x_pixels,
+                            'offsetYPixels': offset_y_pixels,
+                            'widthPixels': 800 * x_scale,
+                            'heightPixels': 400 * y_scale,
+                        }
+                    }}}}, self.work_zone))
+        return self
+
     def add_chart(self, columns,
                   target_axis: AxisPosition = AxisPosition.LEFT_AXIS,
                   index_column: int = 0,
                   chart_type: ChartType = ChartType.LINE,
                   stacked_type: StackedType = StackedType.NONE,
                   title: str = None,
                   legend_position: LegendPosition = LegendPosition.BOTTOM_LEGEND,
@@ -292,26 +441,27 @@
                   y_right_axis_max: float = None,
                   x_scale: int = 1,
                   y_scale: int = 1,
                   offset_x_pixels: int = 0,
                   offset_y_pixels: int = 0,
                   header_count: int = 1,
                   data_start: tuple = (0, 0),
-                  last_row: int = None):
+                  nrows: int = None,
+                  data_sheet_name=None,):
 
         data_start_cell = parse_range(data_start)
         target_axis = [target_axis] if not isinstance(target_axis, Iterable) else target_axis
         series = [{
             'series': {
                 'sourceRange': {
                     'sources': [
                         {
-                            'sheetId': self.sheet_id,
+                            'sheetId': self.sheet_id if not data_sheet_name else self.base.sheets.get(data_sheet_name).get('sheetId'),
                             'startRowIndex': data_start_cell[0],
-                            'endRowIndex': last_row if last_row is not None else None,
+                            'endRowIndex': data_start_cell[0] + nrows + 1 if nrows is not None else None,
                             'startColumnIndex': data_start_cell[1] + column,
                             'endColumnIndex': data_start_cell[1] + column + 1,
                         }
                     ]
                 }
             },
             'targetAxis': axis.value
@@ -352,17 +502,17 @@
                             ],
                             'domains': [
                                 {
                                     'domain': {
                                         'sourceRange': {
                                             'sources': [
                                                 {
-                                                    'sheetId': self.sheet_id,
+                                                    'sheetId': self.sheet_id if not data_sheet_name else self.base.sheets.get(data_sheet_name).get('sheetId'),
                                                     'startRowIndex': data_start_cell[0],
-                                                    'endRowIndex': last_row if last_row is not None else None,
+                                                    'endRowIndex': data_start_cell[0] + nrows + 1 if nrows is not None else None,
                                                     'startColumnIndex': data_start_cell[1] + index_column,
                                                     'endColumnIndex': data_start_cell[1] + index_column + 1,
                                                 }
                                             ]
                                         }
                                     }
                                 }
@@ -379,28 +529,28 @@
                                 'columnIndex': self.work_zone.get('startColumnIndex'),
                             },
                             'offsetXPixels': offset_x_pixels,
                             'offsetYPixels': offset_y_pixels,
                             'widthPixels': 800 * x_scale,
                             'heightPixels': 400 * y_scale,
                         }
-                    }}}}))
+                    }}}}, self.work_zone))
 
         return self
 
     def auto_size(self, axis: Union[str, int] = 1):
         axis = axis.upper() if isinstance(axis, str) else DIMENSION.get(axis)
         self._task_queue.append(Task('format', self._increment_task(), self.sheet_id, {
                 'autoResizeDimensions': {
                     'dimensions': {
                         'sheetId': self.sheet_id,
                         'dimension': axis,
                         'startIndex': self.work_zone.get('startRowIndex') if axis == 'ROWS' else self.work_zone.get('startColumnIndex'),
                         'endIndex': self.work_zone.get('endRowIndex') if axis == 'ROWS' else self.work_zone.get('endColumnIndex')
-                    }}}))
+                    }}}, self.work_zone))
         return self
 
     def clear(self, values=True, formats=True):
         field = None
         if values and formats:
             field = '*'
         elif formats:
@@ -408,143 +558,172 @@
         elif values:
             field = 'userEnteredValue'
 
         self._task_queue.append(Task('clear', self._increment_task(), self.sheet_id, {
                 'updateCells': {
                     'range': self.work_zone,
                     'fields': field,
-                }}))
+                }}, self.work_zone))
 
         return self
 
     def delete_axis(self, axis: Union[str, int] = 1):
         axis = axis.upper() if isinstance(axis, str) else DIMENSION.get(axis)
         self._task_queue.append(Task('clear', self._increment_task(), self.sheet_id, {
                 'deleteDimension': {
                     'range': {
                         'sheetId': self.sheet_id,
                         'dimension': axis,
                         'startIndex': self.work_zone.get('startRowIndex') if axis == 'ROWS' else self.work_zone.get('startColumnIndex'),
                         'endIndex': self.work_zone.get('endRowIndex') if axis == 'ROWS' else self.work_zone.get('endColumnIndex')
-                    }}}))
+                    }}}, self.work_zone))
 
         return self
 
     def extend_sheet(self, rows: int = None, cols: int = None):
         if cols:
-            self._task_queue.append(Task('clear', self._increment_task(), self.sheet_id, {
+            self._task_queue.append(Task('format', self._increment_task(), self.sheet_id, {
                 'appendDimension': {
                     'sheetId': self.sheet_id,
                     'dimension': 'COLUMNS',
                     'length': cols,
-                }}))
+                }}, self.work_zone))
         if rows:
-            self._task_queue.append(Task('clear', self._increment_task(), self.sheet_id, {
+            self._task_queue.append(Task('format', self._increment_task(), self.sheet_id, {
                 'appendDimension': {
                     'sheetId': self.sheet_id,
                     'dimension': 'ROWS',
                     'length': rows,
-                }}))
+                }}, self.work_zone))
 
         return self
 
     def hide_grid_lines(self, hide_grid=True):
         self._task_queue.append(Task('format', self._increment_task(), self.sheet_id, {
             'updateSheetProperties': {
                 'properties': {
                     'sheetId': self.sheet_id,
                     'gridProperties': {
                         'hideGridlines': hide_grid,
                     },
                 },
                 'fields': 'gridProperties.hideGridlines',
             }
-        }))
+        }, self.work_zone))
         return self
 
     def merge_cells(self, merge_type: MergeType = MergeType.MERGE_ALL):
         self._task_queue.append(Task('format', self._increment_task(), self.sheet_id, {
                 'mergeCells': {
                     'mergeType': merge_type.value,
                     'range': self.work_zone
-                }}))
+                }}, self.work_zone))
         return self
 
+    def read_cell_details(self):
+        return (self.base.connect_v4.spreadsheets()
+        .get(spreadsheetId=self.base.spreadsheet_id,
+             ranges=[self.data_cell],
+             includeGridData=True
+             )
+            .execute()['sheets'][0]['data'][0].get('rowData', [])
+        )
+
     def read_dataframe(self):
-        rows = self.read_range()
+        rows = self.read_values()
         return pd.DataFrame(data=rows[1:], columns=rows[0])
 
-    def read_range(self):
-        return (self.base._connect().spreadsheets().values()
-                .get(spreadsheetId=self.sheet_id,
+    def read_values(self, formated_values: bool = True):
+        print(self.data_cell)
+        return (self.base.connect_v4.spreadsheets().values()
+                .get(spreadsheetId=self.base.spreadsheet_id,
                      range=self.data_cell,
-                     valueRenderOption='UNFORMATTED_VALUE').execute()
+                     valueRenderOption='FORMATTED_VALUE' if formated_values else 'UNFORMATTED_VALUE').execute()
                 .get('values', []))
 
+    def put_copied_cells(self, copied_data):
+        '''
+        This function puts data from other cells into the current
+        :param copied_data: use method read_cell_details to collect date
+        '''
+        self._task_queue.append(Task('format', self._increment_task(), self.sheet_id, {
+                'updateCells': {
+                    'range': {
+                        'sheetId': self.sheet_id,
+                        'startRowIndex': self.work_zone.get('startRowIndex'),
+                        'endRowIndex': self.work_zone.get('endRowIndex'),
+                        'startColumnIndex': self.work_zone.get('startColumnIndex'),
+                        'endColumnIndex': self.work_zone.get('endColumnIndex')
+                    },
+                    'fields': 'userEnteredFormat, userEnteredValue',
+                    'rows': copied_data
+                }}, self.work_zone))
+        return self
+
     def set_background_color(self, color: Color = Color((255, 255, 255))):
         color = color.value if isinstance(color, Enum) else color
         self._task_queue.append(Task('format', self._increment_task(), self.sheet_id, {
                 'repeatCell': {
                     'range': self.work_zone,
                     'cell': {
                         'userEnteredFormat': {
                             'backgroundColor': color.color
                         }},
                     'fields': 'userEnteredFormat(backgroundColor)',
-                }}))
+                }}, self.work_zone))
         return self
 
     def set_borders(self, border_style: BorderStyle = BorderStyle.SOLID,
                     border_width: int = 1,
                     color: Color = Color((0, 0, 0)),
                     border_sides: list = BORDER_SIDES,
                     ):
         color = color.value if isinstance(color, Enum) else color
         self._task_queue.append(Task('format', self._increment_task(), self.sheet_id, {
                 'updateBorders': {
                     'range': self.work_zone,
                     **dict((x, Border(border_style, border_width, color).__dict__) for x in border_sides),
-                }}))
+                }}, self.work_zone))
         return self
 
     def set_freeze_cell(self):
         self._task_queue.append(Task('format', self._increment_task(), self.sheet_id, {
             'updateSheetProperties': {
                 'properties': {
                     'gridProperties': {
                         'frozenRowCount': self.work_zone.get('startRowIndex'),
                         'frozenColumnCount': self.work_zone.get('startColumnIndex')},
                     'sheetId': self.sheet_id
                 },
                 'fields': 'gridProperties.frozenRowCount, gridProperties.frozenColumnCount'
             }
-        }))
+        }, self.work_zone))
         return self
 
     def set_num_format(self, default_format: BaseNumberFormat = Number):
         default_format = default_format.value if isinstance(default_format, Enum) else default_format
         self._task_queue.append(Task('format', self._increment_task(), self.sheet_id, {
                 'repeatCell': {
                     'range': self.work_zone,
                     **default_format.__dict__,
-                }}))
+                }}, self.work_zone))
         return self
 
     def set_sheet_size(self, rows: int, columns: int):
         self._task_queue.append(Task('clear', self._increment_task(), self.sheet_id, {
                 'updateSheetProperties': {
                     'properties': {
                         'gridProperties': {
                             'rowCount': rows,
                             'columnCount': columns,
                         },
                         'sheetId': self.sheet_id,
                     },
                     'fields': 'gridProperties.rowCount, gridProperties.columnCount',
-                }}))
+                }}, self.work_zone))
 
         return self
 
     def set_size(self, size: int = None, axis: Union[str, int] = 1):
         axis = axis.upper() if isinstance(axis, str) else DIMENSION.get(axis)
         self._task_queue.append(Task('format', self._increment_task(), self.sheet_id, {
                 'updateDimensionProperties': {
@@ -554,15 +733,15 @@
                         'startIndex': self.work_zone.get('startRowIndex') if axis == 'ROWS' else self.work_zone.get('startColumnIndex'),
                         'endIndex': self.work_zone.get('endRowIndex') if axis == 'ROWS' else self.work_zone.get('endColumnIndex'),
                     },
                     'properties': {
                         'pixelSize': size,
                     },
                     'fields': 'pixelSize',
-                }}))
+                }}, self.work_zone))
         return self
 
     def set_text_format(self, horizontal_alignment: HorizontalAlignment = None,
                         vertical_alignment: VerticalAlignment = None,
                         wrap_strategy: WrapStrategy = None,
                         font_size: int = None,
                         bold: bool = None,
@@ -594,22 +773,22 @@
                                 'fontSize': font_size if font_size is not None or False else None,
                                 'bold': bold if bold is not None or False else None,
                                 'italic': italic if italic is not None or False else None,
                                 'strikethrough': strikethrough if strikethrough is not None or False else None,
                                 'underline': underline if underline is not None or False else None,
                             }}},
                     'fields': f'userEnteredFormat({list_of_inputs})',
-                }}))
+                }}, self.work_zone))
         return self
 
     def unmerge_cells(self):
         self._task_queue.append(Task('format', self._increment_task(), self.sheet_id, {
                 'unmergeCells': {
                     'range': self.work_zone,
-                }}))
+                }}, self.work_zone))
         return self
 
     def write_dataframe(self, df: pd.DataFrame, header=True, index=True):
         df = df.copy()
 
         for column, column_type in zip(df.dtypes.index, df.dtypes.values):
             if isinstance(column_type, pd.CategoricalDtype):
@@ -621,59 +800,60 @@
             if isinstance(df.index, pd.CategoricalIndex) or any(isinstance(x, pd.Interval) for x in df.index.values):
                 df.index = df.index.astype(str)
             try:
                 df = df.reset_index(col_level=-1)
             except:
                 df = pd.merge(df.index.to_frame(index=False), df.reset_index(drop=True), left_index=True, right_index=True)
 
-        df = df.applymap(datetime_to_xls).replace([np.inf, -np.inf], None).where(pd.notnull(df), None)
+        df = df.applymap(datetime_to_xls).replace([np.inf, -np.inf, np.NaN], None)
 
         if header:
             if isinstance(df.columns, pd.MultiIndex):
                 values = [[str(elem) for elem in level] for level in list(zip(*df.columns.to_list()))] + df.values.tolist()
             else:
                 values = [[str(elem) for elem in df.columns.to_list()]] + df.values.tolist()
         else:
             values = df.values.tolist()
 
         self._task_queue.append(Task('data', self._increment_task(), self.sheet_id, {
                 'range': self.start_data_cell,
                 'values': values,
                 'majorDimension': 'ROWS',
-        }, [self.work_zone.get('startRowIndex'), self.work_zone.get('startColumnIndex')]))
+        }, self.work_zone))
         return self
 
     def write_formula(self, value):
         self._task_queue.append(Task('format', self._increment_task(), self.sheet_id, {
             'repeatCell': {
                 'range': self.work_zone,
                 'cell': {
                     'userEnteredValue': {
                         'formulaValue': value
                     }
                 },
                 'fields': 'userEnteredValue'
-            }}, [self.work_zone.get('startRowIndex'), self.work_zone.get('startColumnIndex')]))
+            }}, self.work_zone))
 
         return self
 
     def write_range(self, values, axis: Union[str, int] = 0):
         values = list(values) if not isinstance(values, list) else values
         while depth(values) < 2:
             values = [values]
         values = apply(values, datetime_to_xls)
         self._task_queue.append(Task('data', self._increment_task(), self.sheet_id, {
                 'range': self.start_data_cell,
                 'values': values,
                 'majorDimension': DIMENSION.get(axis.upper() if isinstance(axis, str) else axis),
-              }, [self.work_zone.get('startRowIndex'), self.work_zone.get('startColumnIndex')]))
+              }, self.work_zone))
 
         return self
 
 
+
 class Sheet(Range):
     def __init__(self, sheet_name, sheet_id, task_query, sheets, base, cells=(0, 0, None, None)):
         self.base = base
         self.sheet_name = sheet_name
         self.sheet_id = sheet_id
         self._task_queue = task_query
         self.sheets = sheets
@@ -705,25 +885,34 @@
 
     def __enter__(self):
         return self
 
     def __exit__(self, *args):
         self.exec()
 
-    def create_spreadsheet(self, title, sheets: list = ['Sheet1']):
+    def create_spreadsheet(self, title, sheets: list = ['Sheet1'], hide_grid_lines: Union[list, bool] = False):
+        if isinstance(hide_grid_lines, bool):
+            hide_grid_lines = [hide_grid_lines] * len(sheets)
+
+        if len(hide_grid_lines) != len(sheets):
+            raise NameError(f'Wrong list lenghts. Number of tabs: {len(sheets)}, number of grid options: {len(hide_grid_lines)}')
+
         ss = SpreedSheet(self.connect_v4.spreadsheets()
                          .create(fields='spreadsheetId',
                                  body={
                                      'properties': {'title': title},
-                                     'sheets': [{'properties': {'title': sheet_name}} for sheet_name in sheets]})
+                                     'sheets': [{'properties': {'title': sheet_name,
+                                                                'gridProperties': {'hideGridlines': grid}}}
+                                                for sheet_name, grid in zip(sheets, hide_grid_lines)]})
                          .execute().get('spreadsheetId'), token_path=self.token_path,
                          credentials=self.credentials, connect=self.connect_v4)
         self.list_of_spreadsheets.append(ss)
         return ss
 
+
     def create_folder(self, folderName, parentID=None):
         return self.connect_v3.files().create(body={
             'name': folderName,
             'mimeType': "application/vnd.google-apps.folder",
             'parents': [parentID] if parentID else None,
         }, supportsAllDrives=True).execute()['id']
```

### Comparing `speedtab-0.1.2.4/speedtab/enums.py` & `speedtab-0.1.3.0/speedtab/enums.py`

 * *Files identical despite different names*

### Comparing `speedtab-0.1.2.4/speedtab/formats.py` & `speedtab-0.1.3.0/speedtab/formats.py`

 * *Files identical despite different names*

### Comparing `speedtab-0.1.2.4/setup.py` & `speedtab-0.1.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 install_requires = \
 ['google-api-python-client>=2.58.0,<3.0.0',
  'google-auth-httplib2>=0.1.0,<0.2.0',
  'google-auth-oauthlib>=0.5.2,<0.6.0']
 
 setup_kwargs = {
     'name': 'speedtab',
-    'version': '0.1.2.4',
+    'version': '0.1.3.0',
     'description': 'Convenient wrapper for working with Google Spreadsheets',
     'long_description': None,
     'author': 'Bogdan Gergel',
     'author_email': 'bogger147@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/BoggerSancho/SpeedTab-beta',
```

### Comparing `speedtab-0.1.2.4/PKG-INFO` & `speedtab-0.1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speedtab
-Version: 0.1.2.4
+Version: 0.1.3.0
 Summary: Convenient wrapper for working with Google Spreadsheets
 Home-page: https://github.com/BoggerSancho/SpeedTab-beta
 License: MIT
 Author: Bogdan Gergel
 Author-email: bogger147@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

