# Comparing `tmp/tksheet-6.1.2.tar.gz` & `tmp/tksheet-6.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tksheet-6.1.2.tar", last modified: Sun May  7 09:22:39 2023, max compression
+gzip compressed data, was "tksheet-6.1.3.tar", last modified: Tue May 16 07:13:16 2023, max compression
```

## Comparing `tksheet-6.1.2.tar` & `tksheet-6.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 09:22:39.860341 tksheet-6.1.2/
--rw-rw-rw-   0        0        0     1101 2023-05-07 08:33:24.000000 tksheet-6.1.2/LICENSE.txt
--rw-rw-rw-   0        0        0     3548 2023-05-07 09:22:39.860341 tksheet-6.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2898 2023-05-07 08:33:24.000000 tksheet-6.1.2/README.md
--rw-rw-rw-   0        0        0       86 2023-05-07 09:22:39.861343 tksheet-6.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1010 2023-05-07 08:49:30.000000 tksheet-6.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-07 09:22:39.850823 tksheet-6.1.2/tksheet/
--rw-rw-rw-   0        0        0      344 2023-05-07 08:33:24.000000 tksheet-6.1.2/tksheet/__init__.py
--rw-rw-rw-   0        0        0   169752 2023-05-07 08:33:24.000000 tksheet-6.1.2/tksheet/_tksheet.py
--rw-rw-rw-   0        0        0   117473 2023-05-07 08:33:24.000000 tksheet-6.1.2/tksheet/_tksheet_column_headers.py
--rw-rw-rw-   0        0        0     8893 2023-05-07 08:33:24.000000 tksheet-6.1.2/tksheet/_tksheet_formatters.py
--rw-rw-rw-   0        0        0   348717 2023-05-07 09:18:51.000000 tksheet-6.1.2/tksheet/_tksheet_main_table.py
--rw-rw-rw-   0        0        0    12757 2023-05-07 08:33:24.000000 tksheet-6.1.2/tksheet/_tksheet_other_classes.py
--rw-rw-rw-   0        0        0   113955 2023-05-07 09:10:20.000000 tksheet-6.1.2/tksheet/_tksheet_row_index.py
--rw-rw-rw-   0        0        0     5789 2023-05-07 08:33:24.000000 tksheet-6.1.2/tksheet/_tksheet_top_left_rectangle.py
--rw-rw-rw-   0        0        0    59987 2023-05-07 08:33:24.000000 tksheet-6.1.2/tksheet/_tksheet_vars.py
-drwxrwxrwx   0        0        0        0 2023-05-07 09:22:39.859338 tksheet-6.1.2/tksheet.egg-info/
--rw-rw-rw-   0        0        0     3548 2023-05-07 09:22:39.000000 tksheet-6.1.2/tksheet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      429 2023-05-07 09:22:39.000000 tksheet-6.1.2/tksheet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 09:22:39.000000 tksheet-6.1.2/tksheet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-07 09:22:39.000000 tksheet-6.1.2/tksheet.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 07:13:16.974436 tksheet-6.1.3/
+-rw-rw-rw-   0        0        0     1101 2023-05-16 06:43:15.000000 tksheet-6.1.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     3657 2023-05-16 07:13:16.974436 tksheet-6.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3007 2023-05-16 06:43:15.000000 tksheet-6.1.3/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-16 07:13:16.974436 tksheet-6.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1010 2023-05-16 06:44:23.000000 tksheet-6.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 07:13:16.958800 tksheet-6.1.3/tksheet/
+-rw-rw-rw-   0        0        0      344 2023-05-16 06:43:15.000000 tksheet-6.1.3/tksheet/__init__.py
+-rw-rw-rw-   0        0        0   169718 2023-05-16 07:07:04.000000 tksheet-6.1.3/tksheet/_tksheet.py
+-rw-rw-rw-   0        0        0   117545 2023-05-16 06:59:56.000000 tksheet-6.1.3/tksheet/_tksheet_column_headers.py
+-rw-rw-rw-   0        0        0     8893 2023-05-16 06:43:15.000000 tksheet-6.1.3/tksheet/_tksheet_formatters.py
+-rw-rw-rw-   0        0        0   348693 2023-05-16 07:04:06.000000 tksheet-6.1.3/tksheet/_tksheet_main_table.py
+-rw-rw-rw-   0        0        0    12757 2023-05-16 06:43:15.000000 tksheet-6.1.3/tksheet/_tksheet_other_classes.py
+-rw-rw-rw-   0        0        0   114027 2023-05-16 07:00:24.000000 tksheet-6.1.3/tksheet/_tksheet_row_index.py
+-rw-rw-rw-   0        0        0     5789 2023-05-16 06:43:15.000000 tksheet-6.1.3/tksheet/_tksheet_top_left_rectangle.py
+-rw-rw-rw-   0        0        0    59987 2023-05-16 06:43:15.000000 tksheet-6.1.3/tksheet/_tksheet_vars.py
+drwxrwxrwx   0        0        0        0 2023-05-16 07:13:16.974436 tksheet-6.1.3/tksheet.egg-info/
+-rw-rw-rw-   0        0        0     3657 2023-05-16 07:13:16.000000 tksheet-6.1.3/tksheet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      429 2023-05-16 07:13:16.000000 tksheet-6.1.3/tksheet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 07:13:16.000000 tksheet-6.1.3/tksheet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-16 07:13:16.000000 tksheet-6.1.3/tksheet.egg-info/top_level.txt
```

### Comparing `tksheet-6.1.2/LICENSE.txt` & `tksheet-6.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tksheet-6.1.2/PKG-INFO` & `tksheet-6.1.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tksheet
-Version: 6.1.2
+Version: 6.1.3
 Summary: Tkinter table / sheet widget
 Home-page: https://github.com/ragardner/tksheet
-Download-URL: https://github.com/ragardner/tksheet/archive/6.1.2.tar.gz
+Download-URL: https://github.com/ragardner/tksheet/archive/6.1.3.tar.gz
 Author: ragardner
 Author-email: github@ragardner.simplelogin.com
 License: MIT
 Keywords: tkinter,table,widget,sheet,grid,tk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -27,43 +27,49 @@
 pip install tksheet
 
 #To update using pip
 pip install tksheet --upgrade
 ```
 
 ## **Help**
+
 ----
-- [Documentation](https://github.com/ragardner/tksheet/wiki)
+
+- [Documentation](https://github.com/ragardner/tksheet/wiki/Version-6)
 - [Changelog](https://github.com/ragardner/tksheet/blob/master/CHANGELOG.md)
-- [Questions](https://github.com/ragardner/tksheet/wiki#asking-questions)
-- [Issues](https://github.com/ragardner/tksheet/wiki#issues)
-- [Suggestions](https://github.com/ragardner/tksheet/wiki#enhancements-or-suggestions)
-- This library is maintained with the help of **[others](https://github.com/ragardner/tksheet/graphs/contributors)**. If you would like to contribute please read [this help section](https://github.com/ragardner/tksheet/wiki#contributing).
+- [Questions](https://github.com/ragardner/tksheet/wiki/Version-6#asking-questions)
+- [Issues](https://github.com/ragardner/tksheet/wiki/Version-6#issues)
+- [Suggestions](https://github.com/ragardner/tksheet/wiki/Version-6#enhancements-or-suggestions)
+- This library is maintained with the help of **[others](https://github.com/ragardner/tksheet/graphs/contributors)**. If you would like to contribute please read [this help section](https://github.com/ragardner/tksheet/wiki/Version-6#contributing).
 
 ### **NOTICE:** 
 With versions `5.5.0`+ if you use `extra_bindings()` with `"edit_cell"`/`"end_edit_cell"` you must provide a return value in your bound function to set the cell value to. To disable this behavior in these versions use option `edit_cell_validation = False` in your `Sheet()` initialisation arguments or use `set_options(edit_cell_validation = False)`. [See here](https://github.com/ragardner/tksheet/issues/170#issuecomment-1522236289) for more information on this issue and if you need to *very* directly set the cell data.
 
 ## **Features**
+
 ----
+
 - Display and modify tabular data
 - Stores its display data as a Python list of lists, sublists being rows
 - Runs smoothly even with millions of rows/columns
 - Edit cells directly
-- Cell values can potentially be [any class](https://github.com/ragardner/tksheet/wiki#cell-formatting), the default is any class with a `__str__` method
+- Cell values can potentially be [any class](https://github.com/ragardner/tksheet/wiki/Version-6#cell-formatting), the default is any class with a `__str__` method
 - Drag and drop columns and rows
 - Multiple line header and index cells
 - Expand row heights and column widths
 - Change fonts and font size (not for individual cells)
 - Change any colors in the sheet
 - Create an unlimited number of high performance dropdown and check boxes
-- [Hide rows and/or columns](https://github.com/ragardner/tksheet/wiki#example-header-dropdown-boxes-and-row-filtering)
+- [Hide rows and/or columns](https://github.com/ragardner/tksheet/wiki/Version-6#example-header-dropdown-boxes-and-row-filtering)
 - Left `"w"`, Center `"center"` or Right `"e"` text alignment for any cell/row/column
 
 ### **light blue theme**
+
 ----
 
-![alt text](https://i.imgur.com/ojU3IQi.jpeg)
+![tksheet light blue theme](https://i.imgur.com/ojU3IQi.jpeg)
 
 ### **black theme**
+
 ----
 
-![alt text](https://i.imgur.com/JeF9vJe.jpeg)
+![tksheet black theme](https://i.imgur.com/JeF9vJe.jpeg)
```

### Comparing `tksheet-6.1.2/README.md` & `tksheet-6.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -9,43 +9,49 @@
 pip install tksheet
 
 #To update using pip
 pip install tksheet --upgrade
 ```
 
 ## **Help**
+
 ----
-- [Documentation](https://github.com/ragardner/tksheet/wiki)
+
+- [Documentation](https://github.com/ragardner/tksheet/wiki/Version-6)
 - [Changelog](https://github.com/ragardner/tksheet/blob/master/CHANGELOG.md)
-- [Questions](https://github.com/ragardner/tksheet/wiki#asking-questions)
-- [Issues](https://github.com/ragardner/tksheet/wiki#issues)
-- [Suggestions](https://github.com/ragardner/tksheet/wiki#enhancements-or-suggestions)
-- This library is maintained with the help of **[others](https://github.com/ragardner/tksheet/graphs/contributors)**. If you would like to contribute please read [this help section](https://github.com/ragardner/tksheet/wiki#contributing).
+- [Questions](https://github.com/ragardner/tksheet/wiki/Version-6#asking-questions)
+- [Issues](https://github.com/ragardner/tksheet/wiki/Version-6#issues)
+- [Suggestions](https://github.com/ragardner/tksheet/wiki/Version-6#enhancements-or-suggestions)
+- This library is maintained with the help of **[others](https://github.com/ragardner/tksheet/graphs/contributors)**. If you would like to contribute please read [this help section](https://github.com/ragardner/tksheet/wiki/Version-6#contributing).
 
 ### **NOTICE:** 
 With versions `5.5.0`+ if you use `extra_bindings()` with `"edit_cell"`/`"end_edit_cell"` you must provide a return value in your bound function to set the cell value to. To disable this behavior in these versions use option `edit_cell_validation = False` in your `Sheet()` initialisation arguments or use `set_options(edit_cell_validation = False)`. [See here](https://github.com/ragardner/tksheet/issues/170#issuecomment-1522236289) for more information on this issue and if you need to *very* directly set the cell data.
 
 ## **Features**
+
 ----
+
 - Display and modify tabular data
 - Stores its display data as a Python list of lists, sublists being rows
 - Runs smoothly even with millions of rows/columns
 - Edit cells directly
-- Cell values can potentially be [any class](https://github.com/ragardner/tksheet/wiki#cell-formatting), the default is any class with a `__str__` method
+- Cell values can potentially be [any class](https://github.com/ragardner/tksheet/wiki/Version-6#cell-formatting), the default is any class with a `__str__` method
 - Drag and drop columns and rows
 - Multiple line header and index cells
 - Expand row heights and column widths
 - Change fonts and font size (not for individual cells)
 - Change any colors in the sheet
 - Create an unlimited number of high performance dropdown and check boxes
-- [Hide rows and/or columns](https://github.com/ragardner/tksheet/wiki#example-header-dropdown-boxes-and-row-filtering)
+- [Hide rows and/or columns](https://github.com/ragardner/tksheet/wiki/Version-6#example-header-dropdown-boxes-and-row-filtering)
 - Left `"w"`, Center `"center"` or Right `"e"` text alignment for any cell/row/column
 
 ### **light blue theme**
+
 ----
 
-![alt text](https://i.imgur.com/ojU3IQi.jpeg)
+![tksheet light blue theme](https://i.imgur.com/ojU3IQi.jpeg)
 
 ### **black theme**
+
 ----
 
-![alt text](https://i.imgur.com/JeF9vJe.jpeg)
+![tksheet black theme](https://i.imgur.com/JeF9vJe.jpeg)
```

### Comparing `tksheet-6.1.2/setup.py` & `tksheet-6.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding = 'utf-8') as f:
     long_description = f.read()
 
 setup(
   name = 'tksheet',
   packages = ['tksheet'],
-  version = '6.1.2',
+  version = '6.1.3',
   python_requires = '>=3.6',
   license = 'MIT',
   description = 'Tkinter table / sheet widget',
   long_description = long_description,
   long_description_content_type = 'text/markdown',
   author = 'ragardner',
   author_email = 'github@ragardner.simplelogin.com',
   url = 'https://github.com/ragardner/tksheet',
-  download_url = 'https://github.com/ragardner/tksheet/archive/6.1.2.tar.gz',
+  download_url = 'https://github.com/ragardner/tksheet/archive/6.1.3.tar.gz',
   keywords = ['tkinter', 'table', 'widget', 'sheet', 'grid', 'tk'],
   install_requires = [],
   classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Developers',
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License'
```

### Comparing `tksheet-6.1.2/tksheet/_tksheet.py` & `tksheet-6.1.3/tksheet/_tksheet.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import tkinter as tk
 from collections import deque
 from itertools import accumulate, chain, islice
 from tkinter import ttk
+import bisect
+from typing import Union
 
 from ._tksheet_column_headers import *
 from ._tksheet_formatters import *
 from ._tksheet_main_table import *
 from ._tksheet_other_classes import *
 from ._tksheet_row_index import *
 from ._tksheet_top_left_rectangle import *
@@ -1173,14 +1175,15 @@
         if isinstance(rows, set):
             to_del = rows
         else:
             to_del = set(rows)
         if not to_del:
             return
         self.MT.data[:] = [row for r, row in enumerate(self.MT.data) if r not in to_del]
+        to_bis = sorted(to_del)
         if self.MT.all_rows_displayed:
             self.set_row_heights(
                 row_heights=(
                     h
                     for r, h in enumerate(
                         int(b - a)
                         for a, b in zip(
@@ -1211,15 +1214,14 @@
                         )
                         if r not in heights_to_del
                     )
                 )
             self.MT.displayed_rows = [
                 r for r in self.MT.displayed_rows if r not in to_del
             ]
-        to_bis = sorted(to_del)
         self.MT.cell_options = {
             (
                 r
                 if not bisect.bisect_left(to_bis, r)
                 else r - bisect.bisect_left(to_bis, r),
                 c,
             ): v
@@ -3895,17 +3897,14 @@
 
     def close_index_dropdown(self, r):
         self.RI.close_dropdown_window(r)
 
     def reapply_formatting(self):
         self.MT.reapply_formatting()
 
-    def reapply_formatting(self):
-        self.MT.reapply_formatting()
-
     def delete_all_formatting(self, clear_values=False):
         self.MT.delete_all_formatting(clear_values=clear_values)
 
     def format_cell(
         self,
         r,
         c,
```

### Comparing `tksheet-6.1.2/tksheet/_tksheet_column_headers.py` & `tksheet-6.1.3/tksheet/_tksheet_column_headers.py`

 * *Files 0% similar despite different names*

```diff
@@ -780,15 +780,15 @@
         col = self.MT.identify_col(x=event.x)
         if col >= self.dragged_col.to_move[0] and col <= self.dragged_col.to_move[-1]:
             xpos = self.MT.col_positions[self.dragged_col.to_move[0]]
         else:
             if col < self.dragged_col.to_move[0]:
                 xpos = self.MT.col_positions[col]
             else:
-                xpos = self.MT.col_positions[col + 1]
+                xpos = self.MT.col_positions[col + 1] if len(self.MT.col_positions) - 1 > col else self.MT.col_positions[col]
         return xpos
 
     def show_drag_and_drop_indicators(self, xpos, y1, y2, start_col, end_col):
         self.delete_all_resize_and_ctrl_lines()
         self.create_resize_line(
             xpos,
             0,
```

### Comparing `tksheet-6.1.2/tksheet/_tksheet_formatters.py` & `tksheet-6.1.3/tksheet/_tksheet_formatters.py`

 * *Files identical despite different names*

### Comparing `tksheet-6.1.2/tksheet/_tksheet_main_table.py` & `tksheet-6.1.3/tksheet/_tksheet_main_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -469,23 +469,20 @@
     def get_ctrl_x_c_boxes(self):
         currently_selected = self.currently_selected()
         boxes = {}
         if currently_selected.type_ in ("cell", "column"):
             for item in chain(self.find_withtag("cells"), self.find_withtag("columns")):
                 alltags = self.gettags(item)
                 boxes[tuple(int(e) for e in alltags[1].split("_") if e)] = alltags[0]
-            maxrows = 0
-            for r1, c1, r2, c2 in boxes:
-                if r2 - r1 > maxrows:
-                    maxrows = r2 - r1
             curr_box = self.find_last_selected_box_with_current_from_boxes(
                 currently_selected, boxes
             )
+            maxrows = curr_box[2] - curr_box[0]
             for box in tuple(boxes):
-                if box[2] - box[0] < maxrows and box != curr_box:
+                if box[2] - box[0] != maxrows:
                     del boxes[box]
             return boxes, maxrows
         else:
             for item in self.find_withtag("rows"):
                 boxes[
                     tuple(int(e) for e in self.gettags(item)[1].split("_") if e)
                 ] = "rows"
@@ -4661,14 +4658,15 @@
             )
         self.parentframe.emit_event("<<SheetModified>>")
 
     def del_cols_rc(self, event=None):
         seld_cols = sorted(self.get_selected_cols())
         if not seld_cols:
             return
+        seldmax = seld_cols[-1] if self.all_columns_displayed else self.displayed_columns[seld_cols[-1]]
         if self.extra_begin_del_cols_rc_func is not None:
             try:
                 self.extra_begin_del_cols_rc_func(
                     DeleteRowColumnEvent("begin_delete_columns", seld_cols)
                 )
             except Exception:
                 return
@@ -4722,27 +4720,27 @@
                 except Exception:
                     continue
         if self.undo_enabled:
             self.undo_storage.append(("delete_cols", undo_storage))
         for c in reversed(seld_cols):
             self.del_col_position(c, deselect_all=False)
         numcols = len(seld_cols)
-        idx = seld_cols[-1]
+        
         self.cell_options = {
-            (rn, cn if cn < idx else cn - numcols): t2
+            (rn, cn if cn < seldmax else cn - numcols): t2
             for (rn, cn), t2 in self.cell_options.items()
             if cn not in seldset
         }
         self.col_options = {
-            cn if cn < idx else cn - numcols: t
+            cn if cn < seldmax else cn - numcols: t
             for cn, t in self.col_options.items()
             if cn not in seldset
         }
         self.CH.cell_options = {
-            cn if cn < idx else cn - numcols: t
+            cn if cn < seldmax else cn - numcols: t
             for cn, t in self.CH.cell_options.items()
             if cn not in seldset
         }
         self.deselect("allcols", redraw=False)
         self.set_current_to_last()
         if not self.all_columns_displayed:
             self.displayed_columns = [
@@ -4759,14 +4757,15 @@
             )
         self.parentframe.emit_event("<<SheetModified>>")
 
     def del_rows_rc(self, event=None):
         seld_rows = sorted(self.get_selected_rows())
         if not seld_rows:
             return
+        seldmax = seld_rows[-1] if self.all_rows_displayed else self.displayed_rows[seld_rows[-1]]
         if self.extra_begin_del_rows_rc_func is not None:
             try:
                 self.extra_begin_del_rows_rc_func(
                     DeleteRowColumnEvent("begin_delete_rows", seld_rows)
                 )
             except Exception:
                 return
@@ -4811,31 +4810,27 @@
                 except Exception:
                     continue
         if self.undo_enabled:
             self.undo_storage.append(("delete_rows", undo_storage))
         for r in reversed(seld_rows):
             self.del_row_position(r, deselect_all=False)
         numrows = len(seld_rows)
-        idx = (
-            seld_rows[-1]
-            if self.all_rows_displayed
-            else self.displayed_rows[seld_rows[-1]]
-        )
+        
         self.cell_options = {
-            (rn if rn < idx else rn - numrows, cn): t2
+            (rn if rn < seldmax else rn - numrows, cn): t2
             for (rn, cn), t2 in self.cell_options.items()
             if rn not in seldset
         }
         self.row_options = {
-            rn if rn < idx else rn - numrows: t
+            rn if rn < seldmax else rn - numrows: t
             for rn, t in self.row_options.items()
             if rn not in seldset
         }
         self.RI.cell_options = {
-            rn if rn < idx else rn - numrows: t
+            rn if rn < seldmax else rn - numrows: t
             for rn, t in self.RI.cell_options.items()
             if rn not in seldset
         }
         self.deselect("allrows", redraw=False)
         self.set_current_to_last()
         self.refresh()
         if self.extra_end_del_rows_rc_func is not None:
@@ -5100,26 +5095,26 @@
             else:
                 self.data[total_rows:] = []
         if total_columns is not None:
             self.data[:] = [
                 r[:total_columns]
                 if len(r) > total_columns
                 else r
-                + self.get_empty_row_seq(rn, end=len(r) + total_columns, start=len(r))
+                + self.get_empty_row_seq(rn, end=len(r) + total_columns - len(r), start=len(r))
                 for rn, r in enumerate(self.data)
             ]
 
     def equalize_data_row_lengths(self, include_header=False, total_columns=None):
         total_columns = (
             self.total_data_cols() if total_columns is None else total_columns
         )
         if include_header and total_columns > len(self._headers):
             self.CH.fix_header(total_columns)
         self.data[:] = [
-            (r + self.get_empty_row_seq(rn, end=len(r) + total_columns, start=len(r)))
+            (r + self.get_empty_row_seq(rn, end=len(r) + total_columns - len(r), start=len(r)))
             if total_columns > len(r)
             else r
             for rn, r in enumerate(self.data)
         ]
         return total_columns
 
     def get_canvas_visible_area(self):
```

### Comparing `tksheet-6.1.2/tksheet/_tksheet_other_classes.py` & `tksheet-6.1.3/tksheet/_tksheet_other_classes.py`

 * *Files identical despite different names*

### Comparing `tksheet-6.1.2/tksheet/_tksheet_row_index.py` & `tksheet-6.1.3/tksheet/_tksheet_row_index.py`

 * *Files 0% similar despite different names*

```diff
@@ -724,15 +724,15 @@
         row = self.MT.identify_row(y=event.y)
         if row >= self.dragged_row.to_move[0] and row <= self.dragged_row.to_move[-1]:
             ypos = self.MT.row_positions[self.dragged_row.to_move[0]]
         else:
             if row < self.dragged_row.to_move[0]:
                 ypos = self.MT.row_positions[row]
             else:
-                ypos = self.MT.row_positions[row + 1]
+                ypos = self.MT.row_positions[row + 1] if len(self.MT.row_positions) - 1 > row else self.MT.row_positions[row]
         return ypos
 
     def show_drag_and_drop_indicators(self, ypos, x1, x2, start_row, end_row):
         self.delete_all_resize_and_ctrl_lines()
         self.create_resize_line(
             0,
             ypos,
```

### Comparing `tksheet-6.1.2/tksheet/_tksheet_top_left_rectangle.py` & `tksheet-6.1.3/tksheet/_tksheet_top_left_rectangle.py`

 * *Files identical despite different names*

### Comparing `tksheet-6.1.2/tksheet/_tksheet_vars.py` & `tksheet-6.1.3/tksheet/_tksheet_vars.py`

 * *Files identical despite different names*

### Comparing `tksheet-6.1.2/tksheet.egg-info/PKG-INFO` & `tksheet-6.1.3/tksheet.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tksheet
-Version: 6.1.2
+Version: 6.1.3
 Summary: Tkinter table / sheet widget
 Home-page: https://github.com/ragardner/tksheet
-Download-URL: https://github.com/ragardner/tksheet/archive/6.1.2.tar.gz
+Download-URL: https://github.com/ragardner/tksheet/archive/6.1.3.tar.gz
 Author: ragardner
 Author-email: github@ragardner.simplelogin.com
 License: MIT
 Keywords: tkinter,table,widget,sheet,grid,tk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -27,43 +27,49 @@
 pip install tksheet
 
 #To update using pip
 pip install tksheet --upgrade
 ```
 
 ## **Help**
+
 ----
-- [Documentation](https://github.com/ragardner/tksheet/wiki)
+
+- [Documentation](https://github.com/ragardner/tksheet/wiki/Version-6)
 - [Changelog](https://github.com/ragardner/tksheet/blob/master/CHANGELOG.md)
-- [Questions](https://github.com/ragardner/tksheet/wiki#asking-questions)
-- [Issues](https://github.com/ragardner/tksheet/wiki#issues)
-- [Suggestions](https://github.com/ragardner/tksheet/wiki#enhancements-or-suggestions)
-- This library is maintained with the help of **[others](https://github.com/ragardner/tksheet/graphs/contributors)**. If you would like to contribute please read [this help section](https://github.com/ragardner/tksheet/wiki#contributing).
+- [Questions](https://github.com/ragardner/tksheet/wiki/Version-6#asking-questions)
+- [Issues](https://github.com/ragardner/tksheet/wiki/Version-6#issues)
+- [Suggestions](https://github.com/ragardner/tksheet/wiki/Version-6#enhancements-or-suggestions)
+- This library is maintained with the help of **[others](https://github.com/ragardner/tksheet/graphs/contributors)**. If you would like to contribute please read [this help section](https://github.com/ragardner/tksheet/wiki/Version-6#contributing).
 
 ### **NOTICE:** 
 With versions `5.5.0`+ if you use `extra_bindings()` with `"edit_cell"`/`"end_edit_cell"` you must provide a return value in your bound function to set the cell value to. To disable this behavior in these versions use option `edit_cell_validation = False` in your `Sheet()` initialisation arguments or use `set_options(edit_cell_validation = False)`. [See here](https://github.com/ragardner/tksheet/issues/170#issuecomment-1522236289) for more information on this issue and if you need to *very* directly set the cell data.
 
 ## **Features**
+
 ----
+
 - Display and modify tabular data
 - Stores its display data as a Python list of lists, sublists being rows
 - Runs smoothly even with millions of rows/columns
 - Edit cells directly
-- Cell values can potentially be [any class](https://github.com/ragardner/tksheet/wiki#cell-formatting), the default is any class with a `__str__` method
+- Cell values can potentially be [any class](https://github.com/ragardner/tksheet/wiki/Version-6#cell-formatting), the default is any class with a `__str__` method
 - Drag and drop columns and rows
 - Multiple line header and index cells
 - Expand row heights and column widths
 - Change fonts and font size (not for individual cells)
 - Change any colors in the sheet
 - Create an unlimited number of high performance dropdown and check boxes
-- [Hide rows and/or columns](https://github.com/ragardner/tksheet/wiki#example-header-dropdown-boxes-and-row-filtering)
+- [Hide rows and/or columns](https://github.com/ragardner/tksheet/wiki/Version-6#example-header-dropdown-boxes-and-row-filtering)
 - Left `"w"`, Center `"center"` or Right `"e"` text alignment for any cell/row/column
 
 ### **light blue theme**
+
 ----
 
-![alt text](https://i.imgur.com/ojU3IQi.jpeg)
+![tksheet light blue theme](https://i.imgur.com/ojU3IQi.jpeg)
 
 ### **black theme**
+
 ----
 
-![alt text](https://i.imgur.com/JeF9vJe.jpeg)
+![tksheet black theme](https://i.imgur.com/JeF9vJe.jpeg)
```

