# Comparing `tmp/tksheet-6.1.3.tar.gz` & `tmp/tksheet-6.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tksheet-6.1.3.tar", last modified: Tue May 16 07:13:16 2023, max compression
+gzip compressed data, was "tksheet-6.1.4.tar", last modified: Tue May 16 17:02:20 2023, max compression
```

## Comparing `tksheet-6.1.3.tar` & `tksheet-6.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 07:13:16.974436 tksheet-6.1.3/
--rw-rw-rw-   0        0        0     1101 2023-05-16 06:43:15.000000 tksheet-6.1.3/LICENSE.txt
--rw-rw-rw-   0        0        0     3657 2023-05-16 07:13:16.974436 tksheet-6.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     3007 2023-05-16 06:43:15.000000 tksheet-6.1.3/README.md
--rw-rw-rw-   0        0        0       86 2023-05-16 07:13:16.974436 tksheet-6.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1010 2023-05-16 06:44:23.000000 tksheet-6.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-16 07:13:16.958800 tksheet-6.1.3/tksheet/
--rw-rw-rw-   0        0        0      344 2023-05-16 06:43:15.000000 tksheet-6.1.3/tksheet/__init__.py
--rw-rw-rw-   0        0        0   169718 2023-05-16 07:07:04.000000 tksheet-6.1.3/tksheet/_tksheet.py
--rw-rw-rw-   0        0        0   117545 2023-05-16 06:59:56.000000 tksheet-6.1.3/tksheet/_tksheet_column_headers.py
--rw-rw-rw-   0        0        0     8893 2023-05-16 06:43:15.000000 tksheet-6.1.3/tksheet/_tksheet_formatters.py
--rw-rw-rw-   0        0        0   348693 2023-05-16 07:04:06.000000 tksheet-6.1.3/tksheet/_tksheet_main_table.py
--rw-rw-rw-   0        0        0    12757 2023-05-16 06:43:15.000000 tksheet-6.1.3/tksheet/_tksheet_other_classes.py
--rw-rw-rw-   0        0        0   114027 2023-05-16 07:00:24.000000 tksheet-6.1.3/tksheet/_tksheet_row_index.py
--rw-rw-rw-   0        0        0     5789 2023-05-16 06:43:15.000000 tksheet-6.1.3/tksheet/_tksheet_top_left_rectangle.py
--rw-rw-rw-   0        0        0    59987 2023-05-16 06:43:15.000000 tksheet-6.1.3/tksheet/_tksheet_vars.py
-drwxrwxrwx   0        0        0        0 2023-05-16 07:13:16.974436 tksheet-6.1.3/tksheet.egg-info/
--rw-rw-rw-   0        0        0     3657 2023-05-16 07:13:16.000000 tksheet-6.1.3/tksheet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      429 2023-05-16 07:13:16.000000 tksheet-6.1.3/tksheet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 07:13:16.000000 tksheet-6.1.3/tksheet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-16 07:13:16.000000 tksheet-6.1.3/tksheet.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 17:02:20.306486 tksheet-6.1.4/
+-rw-rw-rw-   0        0        0     1101 2023-05-16 06:43:15.000000 tksheet-6.1.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     3657 2023-05-16 17:02:20.306486 tksheet-6.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3007 2023-05-16 06:43:15.000000 tksheet-6.1.4/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-16 17:02:20.307488 tksheet-6.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1010 2023-05-16 09:10:25.000000 tksheet-6.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 17:02:20.297918 tksheet-6.1.4/tksheet/
+-rw-rw-rw-   0        0        0     1901 2023-05-16 09:13:29.000000 tksheet-6.1.4/tksheet/__init__.py
+-rw-rw-rw-   0        0        0   162453 2023-05-16 10:59:08.000000 tksheet-6.1.4/tksheet/_tksheet.py
+-rw-rw-rw-   0        0        0   111539 2023-05-16 12:22:43.000000 tksheet-6.1.4/tksheet/_tksheet_column_headers.py
+-rw-rw-rw-   0        0        0     8846 2023-05-16 09:05:56.000000 tksheet-6.1.4/tksheet/_tksheet_formatters.py
+-rw-rw-rw-   0        0        0   328259 2023-05-16 13:09:52.000000 tksheet-6.1.4/tksheet/_tksheet_main_table.py
+-rw-rw-rw-   0        0        0    12695 2023-05-16 09:06:02.000000 tksheet-6.1.4/tksheet/_tksheet_other_classes.py
+-rw-rw-rw-   0        0        0   108469 2023-05-16 09:07:24.000000 tksheet-6.1.4/tksheet/_tksheet_row_index.py
+-rw-rw-rw-   0        0        0     5746 2023-05-16 09:06:07.000000 tksheet-6.1.4/tksheet/_tksheet_top_left_rectangle.py
+-rw-rw-rw-   0        0        0    59987 2023-05-16 06:43:15.000000 tksheet-6.1.4/tksheet/_tksheet_vars.py
+drwxrwxrwx   0        0        0        0 2023-05-16 17:02:20.306486 tksheet-6.1.4/tksheet.egg-info/
+-rw-rw-rw-   0        0        0     3657 2023-05-16 17:02:20.000000 tksheet-6.1.4/tksheet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      429 2023-05-16 17:02:20.000000 tksheet-6.1.4/tksheet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 17:02:20.000000 tksheet-6.1.4/tksheet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-16 17:02:20.000000 tksheet-6.1.4/tksheet.egg-info/top_level.txt
```

### Comparing `tksheet-6.1.3/LICENSE.txt` & `tksheet-6.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tksheet-6.1.3/PKG-INFO` & `tksheet-6.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tksheet
-Version: 6.1.3
+Version: 6.1.4
 Summary: Tkinter table / sheet widget
 Home-page: https://github.com/ragardner/tksheet
-Download-URL: https://github.com/ragardner/tksheet/archive/6.1.3.tar.gz
+Download-URL: https://github.com/ragardner/tksheet/archive/6.1.4.tar.gz
 Author: ragardner
 Author-email: github@ragardner.simplelogin.com
 License: MIT
 Keywords: tkinter,table,widget,sheet,grid,tk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `tksheet-6.1.3/README.md` & `tksheet-6.1.4/README.md`

 * *Files identical despite different names*

### Comparing `tksheet-6.1.3/setup.py` & `tksheet-6.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding = 'utf-8') as f:
     long_description = f.read()
 
 setup(
   name = 'tksheet',
   packages = ['tksheet'],
-  version = '6.1.3',
+  version = '6.1.4',
   python_requires = '>=3.6',
   license = 'MIT',
   description = 'Tkinter table / sheet widget',
   long_description = long_description,
   long_description_content_type = 'text/markdown',
   author = 'ragardner',
   author_email = 'github@ragardner.simplelogin.com',
   url = 'https://github.com/ragardner/tksheet',
-  download_url = 'https://github.com/ragardner/tksheet/archive/6.1.3.tar.gz',
+  download_url = 'https://github.com/ragardner/tksheet/archive/6.1.4.tar.gz',
   keywords = ['tkinter', 'table', 'widget', 'sheet', 'grid', 'tk'],
   install_requires = [],
   classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Developers',
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License'
```

### Comparing `tksheet-6.1.3/tksheet/_tksheet.py` & `tksheet-6.1.4/tksheet/_tksheet.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,39 @@
 import tkinter as tk
 from collections import deque
 from itertools import accumulate, chain, islice
 from tkinter import ttk
 import bisect
-from typing import Union
+from typing import Union, Callable
 
-from ._tksheet_column_headers import *
-from ._tksheet_formatters import *
-from ._tksheet_main_table import *
-from ._tksheet_other_classes import *
-from ._tksheet_row_index import *
-from ._tksheet_top_left_rectangle import *
-from ._tksheet_vars import *
+from ._tksheet_column_headers import ColumnHeaders
+from ._tksheet_main_table import MainTable
+from ._tksheet_other_classes import (
+    GeneratedMouseEvent,
+    SelectCellEvent,
+    dropdown_search_function,
+    get_checkbox_kwargs,
+    get_dropdown_kwargs,
+    is_iterable,
+)
+from ._tksheet_row_index import RowIndex
+from ._tksheet_top_left_rectangle import TopLeftRectangle
+from ._tksheet_vars import (
+    emitted_events,
+    get_font,
+    get_heading_font,
+    get_index_font,
+    rc_binding,
+    theme_black,
+    theme_dark,
+    theme_dark_blue,
+    theme_dark_green,
+    theme_light_blue,
+    theme_light_green,
+)
 
 
 class Sheet(tk.Frame):
     def __init__(
         self,
         parent,
         show_table: bool = True,
@@ -42,15 +60,22 @@
         paste_insert_row_limit: int = None,
         show_dropdown_borders: bool = False,
         arrow_key_down_right_scroll_page: bool = False,
         enable_edit_cell_auto_resize: bool = True,
         edit_cell_validation: bool = True,
         data_reference: list = None,
         data: list = None,
-        startup_select: tuple = None,  # either (start row, end row, "rows"), (start column, end column, "rows") or (cells start row, cells start column, cells end row, cells end column, "cells")
+        # either (start row, end row, "rows"),
+        #     or (start column, end column, "columns")
+        # or (cells start row,
+        #     cells start column,
+        #     cells end row,
+        #     cells end column,
+        #     "cells")
+        startup_select: tuple = None,
         startup_focus: bool = True,
         total_columns: int = None,
         total_rows: int = None,
         column_width: int = 120,
         header_height: str = "1",  # str or int
         max_column_width: str = "inf",  # str or int
         max_row_height: str = "inf",  # str or int
@@ -93,25 +118,21 @@
         popup_menu_bg=theme_light_blue["popup_menu_bg"],
         popup_menu_highlight_bg=theme_light_blue["popup_menu_highlight_bg"],
         popup_menu_highlight_fg=theme_light_blue["popup_menu_highlight_fg"],
         frame_bg=theme_light_blue["table_bg"],
         table_grid_fg=theme_light_blue["table_grid_fg"],
         table_bg=theme_light_blue["table_bg"],
         table_fg=theme_light_blue["table_fg"],
-        table_selected_cells_border_fg=theme_light_blue[
-            "table_selected_cells_border_fg"
-        ],
+        table_selected_cells_border_fg=theme_light_blue["table_selected_cells_border_fg"],
         table_selected_cells_bg=theme_light_blue["table_selected_cells_bg"],
         table_selected_cells_fg=theme_light_blue["table_selected_cells_fg"],
         table_selected_rows_border_fg=theme_light_blue["table_selected_rows_border_fg"],
         table_selected_rows_bg=theme_light_blue["table_selected_rows_bg"],
         table_selected_rows_fg=theme_light_blue["table_selected_rows_fg"],
-        table_selected_columns_border_fg=theme_light_blue[
-            "table_selected_columns_border_fg"
-        ],
+        table_selected_columns_border_fg=theme_light_blue["table_selected_columns_border_fg"],
         table_selected_columns_bg=theme_light_blue["table_selected_columns_bg"],
         table_selected_columns_fg=theme_light_blue["table_selected_columns_fg"],
         resizing_line_fg=theme_light_blue["resizing_line_fg"],
         drag_and_drop_bg=theme_light_blue["drag_and_drop_bg"],
         index_bg=theme_light_blue["index_bg"],
         index_border_fg=theme_light_blue["index_border_fg"],
         index_grid_fg=theme_light_blue["index_grid_fg"],
@@ -125,17 +146,15 @@
         header_border_fg=theme_light_blue["header_border_fg"],
         header_grid_fg=theme_light_blue["header_grid_fg"],
         header_fg=theme_light_blue["header_fg"],
         header_selected_cells_bg=theme_light_blue["header_selected_cells_bg"],
         header_selected_cells_fg=theme_light_blue["header_selected_cells_fg"],
         header_selected_columns_bg=theme_light_blue["header_selected_columns_bg"],
         header_selected_columns_fg=theme_light_blue["header_selected_columns_fg"],
-        header_hidden_columns_expander_bg=theme_light_blue[
-            "header_hidden_columns_expander_bg"
-        ],
+        header_hidden_columns_expander_bg=theme_light_blue["header_hidden_columns_expander_bg"],
         top_left_bg=theme_light_blue["top_left_bg"],
         top_left_fg=theme_light_blue["top_left_fg"],
         top_left_fg_highlight=theme_light_blue["top_left_fg_highlight"],
     ):
         tk.Frame.__init__(
             self,
             parent,
@@ -271,20 +290,16 @@
             main_canvas=self.MT,
             row_index_canvas=self.RI,
             header_canvas=self.CH,
             top_left_bg=top_left_bg,
             top_left_fg=top_left_fg,
             top_left_fg_highlight=top_left_fg_highlight,
         )
-        self.yscroll = ttk.Scrollbar(
-            self, command=self.MT.set_yviews, orient="vertical"
-        )
-        self.xscroll = ttk.Scrollbar(
-            self, command=self.MT.set_xviews, orient="horizontal"
-        )
+        self.yscroll = ttk.Scrollbar(self, command=self.MT.set_yviews, orient="vertical")
+        self.xscroll = ttk.Scrollbar(self, command=self.MT.set_xviews, orient="horizontal")
         if show_top_left:
             self.TL.grid(row=0, column=0)
         if show_table:
             self.MT.grid(row=1, column=1, sticky="nswe")
             self.MT["xscrollcommand"] = self.xscroll.set
             self.MT["yscrollcommand"] = self.yscroll.set
         if show_row_index:
@@ -318,58 +333,48 @@
                     self.set_options(**{k: v})
         if set_all_heights_and_widths:
             self.set_all_cell_sizes_to_text()
         if startup_select is not None:
             try:
                 if startup_select[-1] == "cells":
                     self.MT.create_selected(*startup_select)
-                    self.MT.set_currently_selected(
-                        startup_select[0], startup_select[1], type_="cell", inside=True
-                    )
+                    self.MT.set_currently_selected(startup_select[0], startup_select[1], type_="cell", inside=True)
                     self.see(startup_select[0], startup_select[1])
                 elif startup_select[-1] == "rows":
                     self.MT.create_selected(
                         startup_select[0],
                         0,
                         startup_select[1],
                         len(self.MT.col_positions) - 1,
                         "rows",
                     )
-                    self.MT.set_currently_selected(
-                        startup_select[0], 0, type_="row", inside=True
-                    )
+                    self.MT.set_currently_selected(startup_select[0], 0, type_="row", inside=True)
                     self.see(startup_select[0], 0)
                 elif startup_select[-1] in ("cols", "columns"):
                     self.MT.create_selected(
                         0,
                         startup_select[0],
                         len(self.MT.row_positions) - 1,
                         startup_select[1],
                         "columns",
                     )
-                    self.MT.set_currently_selected(
-                        0, startup_select[0], type_="column", inside=True
-                    )
+                    self.MT.set_currently_selected(0, startup_select[0], type_="column", inside=True)
                     self.see(0, startup_select[0])
             except Exception:
                 pass
         self.refresh()
         if startup_focus:
             self.MT.focus_set()
 
     def set_refresh_timer(self, redraw=True):
         if redraw and self.after_redraw_id is None:
-            self.after_redraw_id = self.after(
-                self.after_redraw_time_ms, self.after_redraw
-            )
+            self.after_redraw_id = self.after(self.after_redraw_time_ms, self.after_redraw)
 
     def after_redraw(self, redraw_header=True, redraw_row_index=True):
-        self.MT.main_table_redraw_grid_and_text(
-            redraw_header=redraw_header, redraw_row_index=redraw_row_index
-        )
+        self.MT.main_table_redraw_grid_and_text(redraw_header=redraw_header, redraw_row_index=redraw_row_index)
         self.after_redraw_id = None
 
     def show(self, canvas="all"):
         if canvas == "all":
             self.hide()
             self.TL.grid(row=0, column=0)
             self.RI.grid(row=1, column=0, sticky="nswe")
@@ -501,19 +506,15 @@
             if label in self.MT.extra_header_rc_menu_funcs:
                 del self.MT.extra_header_rc_menu_funcs[label]
             if label in self.MT.extra_empty_space_rc_menu_funcs:
                 del self.MT.extra_empty_space_rc_menu_funcs[label]
         self.MT.create_rc_menus()
 
     def extra_bindings(self, bindings, func=None):
-        if (
-            func is not None
-            and isinstance(bindings, str)
-            and bindings.lower() in emitted_events
-        ):
+        if func is not None and isinstance(bindings, str) and bindings.lower() in emitted_events:
             self.bind_event(bindings, func)
 
         if isinstance(bindings, str) and bindings.lower() in (
             "all",
             "bind_all",
             "unbind_all",
         ):
@@ -719,27 +720,27 @@
                     self.CH.ctrl_selection_binding_func = func
                 if binding == "deselect":
                     self.MT.deselection_binding_func = func
 
     def emit_event(self, event, data={}):
         self.event_generate(event, data=data)
 
-    def bind_event(self, sequence, func, add=None):
+    def bind_event(self, sequence: str, func: Callable, add: Union[str, None] = None) -> None:
         widget = self
 
-        def _substitute(*args):
-            e = lambda: None
-            e.data = eval(args[0])
+        def _substitute(*args) -> tuple[None]:
+            def e() -> None:
+                return None
+
+            e.data = args[0]
             e.widget = widget
             return (e,)
 
         funcid = widget._register(func, _substitute, needcleanup=1)
-        cmd = '{0}if {{"[{1} %d]" == "break"}} break\n'.format(
-            "+" if add else "", funcid
-        )
+        cmd = '{0}if {{"[{1} %d]" == "break"}} break\n'.format("+" if add else "", funcid)
         widget.tk.call("bind", widget._w, sequence, cmd)
 
     def bind(self, binding, func, add=None):
         if binding == "<ButtonPress-1>":
             self.MT.extra_b1_press_func = func
             self.CH.extra_b1_press_func = func
             self.RI.extra_b1_press_func = func
@@ -865,29 +866,21 @@
             else:
                 return self.MT.identify_col(x=event.x, allow_end=allow_end)
 
     def get_example_canvas_column_widths(self, total_cols=None):
         colpos = int(self.MT.default_column_width)
         if total_cols is not None:
             return list(accumulate(chain([0], (colpos for c in range(total_cols)))))
-        return list(
-            accumulate(
-                chain([0], (colpos for c in range(len(self.MT.col_positions) - 1)))
-            )
-        )
+        return list(accumulate(chain([0], (colpos for c in range(len(self.MT.col_positions) - 1)))))
 
     def get_example_canvas_row_heights(self, total_rows=None):
         rowpos = self.MT.default_row_height[1]
         if total_rows is not None:
             return list(accumulate(chain([0], (rowpos for c in range(total_rows)))))
-        return list(
-            accumulate(
-                chain([0], (rowpos for c in range(len(self.MT.row_positions) - 1)))
-            )
-        )
+        return list(accumulate(chain([0], (rowpos for c in range(len(self.MT.row_positions) - 1)))))
 
     def get_column_widths(self, canvas_positions=False):
         if canvas_positions:
             return [int(n) for n in self.MT.col_positions]
         return [
             int(b - a)
             for a, b in zip(
@@ -922,57 +915,43 @@
         self.CH.set_width_of_all_cols(
             width=width,
             only_set_if_too_small=only_set_if_too_small,
             recreate=recreate_selection_boxes,
         )
         self.set_refresh_timer(redraw)
 
-    def column_width(
-        self, column=None, width=None, only_set_if_too_small=False, redraw=True
-    ):
+    def column_width(self, column=None, width=None, only_set_if_too_small=False, redraw=True):
         if column == "all":
             if width == "default":
                 self.MT.reset_col_positions()
         elif column == "displayed":
             if width == "text":
-                sc, ec = self.MT.get_visible_columns(
-                    self.MT.canvasx(0), self.MT.canvasx(self.winfo_width())
-                )
+                sc, ec = self.MT.get_visible_columns(self.MT.canvasx(0), self.MT.canvasx(self.winfo_width()))
                 for c in range(sc, ec - 1):
                     self.CH.set_col_width(c)
         elif width == "text" and column is not None:
-            self.CH.set_col_width(
-                col=column, width=None, only_set_if_too_small=only_set_if_too_small
-            )
+            self.CH.set_col_width(col=column, width=None, only_set_if_too_small=only_set_if_too_small)
         elif width is not None and column is not None:
-            self.CH.set_col_width(
-                col=column, width=width, only_set_if_too_small=only_set_if_too_small
-            )
+            self.CH.set_col_width(col=column, width=width, only_set_if_too_small=only_set_if_too_small)
         elif column is not None:
-            return int(
-                self.MT.col_positions[column + 1] - self.MT.col_positions[column]
-            )
+            return int(self.MT.col_positions[column + 1] - self.MT.col_positions[column])
         self.set_refresh_timer(redraw)
 
-    def set_column_widths(
-        self, column_widths=None, canvas_positions=False, reset=False, verify=False
-    ):
+    def set_column_widths(self, column_widths=None, canvas_positions=False, reset=False, verify=False):
         cwx = None
         if reset:
             self.MT.reset_col_positions()
             return
         if verify:
             cwx = self.verify_column_widths(column_widths, canvas_positions)
         if is_iterable(column_widths):
             if canvas_positions and isinstance(column_widths, list):
                 self.MT.col_positions = column_widths
             else:
-                self.MT.col_positions = list(
-                    accumulate(chain([0], (width for width in column_widths)))
-                )
+                self.MT.col_positions = list(accumulate(chain([0], (width for width in column_widths))))
         return cwx
 
     def set_all_row_heights(
         self,
         height=None,
         only_set_if_too_small=False,
         redraw=True,
@@ -981,57 +960,43 @@
         self.RI.set_height_of_all_rows(
             height=height,
             only_set_if_too_small=only_set_if_too_small,
             recreate=recreate_selection_boxes,
         )
         self.set_refresh_timer(redraw)
 
-    def set_cell_size_to_text(
-        self, row, column, only_set_if_too_small=False, redraw=True
-    ):
-        self.MT.set_cell_size_to_text(
-            r=row, c=column, only_set_if_too_small=only_set_if_too_small
-        )
+    def set_cell_size_to_text(self, row, column, only_set_if_too_small=False, redraw=True):
+        self.MT.set_cell_size_to_text(r=row, c=column, only_set_if_too_small=only_set_if_too_small)
         self.set_refresh_timer(redraw)
         # backwards compatibility
 
     def set_width_of_index_to_text(self, text=None, *args, **kwargs):
         self.RI.set_width_of_index_to_text(text=text)
 
     def set_height_of_header_to_text(self, text=None):
         self.CH.set_height_of_header_to_text(text=text)
 
-    def row_height(
-        self, row=None, height=None, only_set_if_too_small=False, redraw=True
-    ):
+    def row_height(self, row=None, height=None, only_set_if_too_small=False, redraw=True):
         if row == "all":
             if height == "default":
                 self.MT.reset_row_positions()
         elif row == "displayed":
             if height == "text":
-                sr, er = self.MT.get_visible_rows(
-                    self.MT.canvasy(0), self.MT.canvasy(self.winfo_width())
-                )
+                sr, er = self.MT.get_visible_rows(self.MT.canvasy(0), self.MT.canvasy(self.winfo_width()))
                 for r in range(sr, er - 1):
                     self.RI.set_row_height(r)
         elif height == "text" and row is not None:
-            self.RI.set_row_height(
-                row=row, height=None, only_set_if_too_small=only_set_if_too_small
-            )
+            self.RI.set_row_height(row=row, height=None, only_set_if_too_small=only_set_if_too_small)
         elif height is not None and row is not None:
-            self.RI.set_row_height(
-                row=row, height=height, only_set_if_too_small=only_set_if_too_small
-            )
+            self.RI.set_row_height(row=row, height=height, only_set_if_too_small=only_set_if_too_small)
         elif row is not None:
             return int(self.MT.row_positions[row + 1] - self.MT.row_positions[row])
         self.set_refresh_timer(redraw)
 
-    def set_row_heights(
-        self, row_heights=None, canvas_positions=False, reset=False, verify=False
-    ):
+    def set_row_heights(self, row_heights=None, canvas_positions=False, reset=False, verify=False):
         if reset:
             self.MT.reset_row_positions()
             return
         if is_iterable(row_heights):
             qmin = self.MT.min_row_height
             if canvas_positions and isinstance(row_heights, list):
                 if verify:
@@ -1053,93 +1018,68 @@
                         )
                     )
                 else:
                     self.MT.row_positions = row_heights
             else:
                 if verify:
                     self.MT.row_positions = [
-                        qmin
-                        if z < qmin or not isinstance(z, int) or isinstance(z, bool)
-                        else z
-                        for z in row_heights
+                        qmin if z < qmin or not isinstance(z, int) or isinstance(z, bool) else z for z in row_heights
                     ]
                 else:
-                    self.MT.row_positions = list(
-                        accumulate(chain([0], (height for height in row_heights)))
-                    )
+                    self.MT.row_positions = list(accumulate(chain([0], (height for height in row_heights))))
 
     def verify_row_heights(self, row_heights: list, canvas_positions=False):
         if row_heights[0] != 0 or isinstance(row_heights[0], bool):
             return False
         if not isinstance(row_heights, list):
             return False
         if canvas_positions:
             if any(
-                x - z < self.MT.min_row_height
-                or not isinstance(x, int)
-                or isinstance(x, bool)
-                for z, x in zip(
-                    islice(row_heights, 0, None), islice(row_heights, 1, None)
-                )
+                x - z < self.MT.min_row_height or not isinstance(x, int) or isinstance(x, bool)
+                for z, x in zip(islice(row_heights, 0, None), islice(row_heights, 1, None))
             ):
                 return False
         elif not canvas_positions:
-            if any(
-                z < self.MT.min_row_height
-                or not isinstance(z, int)
-                or isinstance(z, bool)
-                for z in row_heights
-            ):
+            if any(z < self.MT.min_row_height or not isinstance(z, int) or isinstance(z, bool) for z in row_heights):
                 return False
         return True
 
     def verify_column_widths(self, column_widths: list, canvas_positions=False):
         if column_widths[0] != 0 or isinstance(column_widths[0], bool):
             return False
         if not isinstance(column_widths, list):
             return False
         if canvas_positions:
             if any(
-                x - z < self.MT.min_column_width
-                or not isinstance(x, int)
-                or isinstance(x, bool)
-                for z, x in zip(
-                    islice(column_widths, 0, None), islice(column_widths, 1, None)
-                )
+                x - z < self.MT.min_column_width or not isinstance(x, int) or isinstance(x, bool)
+                for z, x in zip(islice(column_widths, 0, None), islice(column_widths, 1, None))
             ):
                 return False
         elif not canvas_positions:
             if any(
-                z < self.MT.min_column_width
-                or not isinstance(z, int)
-                or isinstance(z, bool)
-                for z in column_widths
+                z < self.MT.min_column_width or not isinstance(z, int) or isinstance(z, bool) for z in column_widths
             ):
                 return False
         return True
 
     def default_row_height(self, height=None):
         if height is not None:
             self.MT.default_row_height = (
                 height if isinstance(height, str) else "pixels",
-                height
-                if isinstance(height, int)
-                else self.MT.get_lines_cell_height(int(height)),
+                height if isinstance(height, int) else self.MT.get_lines_cell_height(int(height)),
             )
         return self.MT.default_row_height[1]
 
     def default_header_height(self, height=None):
         if height is not None:
             self.MT.default_header_height = (
                 height if isinstance(height, str) else "pixels",
                 height
                 if isinstance(height, int)
-                else self.MT.get_lines_cell_height(
-                    int(height), font=self.MT.header_font
-                ),
+                else self.MT.get_lines_cell_height(int(height), font=self.MT.header_font),
             )
         return self.MT.default_header_height[1]
 
     def default_column_width(self, width=None):
         if width is not None:
             if width < self.MT.min_column_width:
                 self.MT.default_column_width = self.MT.min_column_width + 20
@@ -1184,17 +1124,15 @@
             self.set_row_heights(
                 row_heights=(
                     h
                     for r, h in enumerate(
                         int(b - a)
                         for a, b in zip(
                             self.MT.row_positions,
-                            islice(
-                                self.MT.row_positions, 1, len(self.MT.row_positions)
-                            ),
+                            islice(self.MT.row_positions, 1, len(self.MT.row_positions)),
                         )
                     )
                     if r not in to_del
                 )
             )
         else:
             dispset = set(self.MT.displayed_rows)
@@ -1203,82 +1141,62 @@
                 self.set_row_heights(
                     row_heights=(
                         h
                         for r, h in enumerate(
                             int(b - a)
                             for a, b in zip(
                                 self.MT.row_positions,
-                                islice(
-                                    self.MT.row_positions, 1, len(self.MT.row_positions)
-                                ),
+                                islice(self.MT.row_positions, 1, len(self.MT.row_positions)),
                             )
                         )
                         if r not in heights_to_del
                     )
                 )
-            self.MT.displayed_rows = [
-                r for r in self.MT.displayed_rows if r not in to_del
-            ]
+            self.MT.displayed_rows = [r for r in self.MT.displayed_rows if r not in to_del]
         self.MT.cell_options = {
             (
-                r
-                if not bisect.bisect_left(to_bis, r)
-                else r - bisect.bisect_left(to_bis, r),
+                r if not bisect.bisect_left(to_bis, r) else r - bisect.bisect_left(to_bis, r),
                 c,
             ): v
             for (r, c), v in self.MT.cell_options.items()
             if r not in to_del
         }
         self.MT.row_options = {
-            r
-            if not bisect.bisect_left(to_bis, r)
-            else r - bisect.bisect_left(to_bis, r): v
+            r if not bisect.bisect_left(to_bis, r) else r - bisect.bisect_left(to_bis, r): v
             for r, v in self.MT.row_options.items()
             if r not in to_del
         }
         self.RI.cell_options = {
-            r
-            if not bisect.bisect_left(to_bis, r)
-            else r - bisect.bisect_left(to_bis, r): v
+            r if not bisect.bisect_left(to_bis, r) else r - bisect.bisect_left(to_bis, r): v
             for r, v in self.RI.cell_options.items()
             if r not in to_del
         }
         self.set_refresh_timer(redraw)
 
-    def insert_row_position(
-        self, idx="end", height=None, deselect_all=False, redraw=False
-    ):
+    def insert_row_position(self, idx="end", height=None, deselect_all=False, redraw=False):
         self.MT.insert_row_position(idx=idx, height=height, deselect_all=deselect_all)
         self.set_refresh_timer(redraw)
 
-    def insert_row_positions(
-        self, idx="end", heights=None, deselect_all=False, redraw=False
-    ):
-        self.MT.insert_row_positions(
-            idx=idx, heights=heights, deselect_all=deselect_all
-        )
+    def insert_row_positions(self, idx="end", heights=None, deselect_all=False, redraw=False):
+        self.MT.insert_row_positions(idx=idx, heights=heights, deselect_all=deselect_all)
         self.set_refresh_timer(redraw)
 
     def total_rows(self, number=None, mod_positions=True, mod_data=True):
         if number is None:
             return int(self.MT.total_data_rows())
         if not isinstance(number, int) or number < 0:
             raise ValueError("number argument must be integer and > 0")
         if number > len(self.MT.data):
             if mod_positions:
-                height = self.MT.get_lines_cell_height(
-                    int(self.MT.default_row_height[0])
-                )
+                height = self.MT.get_lines_cell_height(int(self.MT.default_row_height[0]))
                 for r in range(number - len(self.MT.data)):
                     self.MT.insert_row_position("end", height)
         elif number < len(self.MT.data):
             if not self.MT.all_rows_displayed:
-                self.MT.display_rows(
-                    enable=False, reset_row_positions=False, deselect_all=True
-                )
+                self.MT.display_rows(enable=False, reset_row_positions=False, deselect_all=True)
             self.MT.row_positions[number + 1 :] = []
         if mod_data:
             self.MT.data_dimensions(total_rows=number)
 
     def total_columns(self, number=None, mod_positions=True, mod_data=True):
         total_cols = self.MT.total_data_cols()
         if number is None:
@@ -1288,41 +1206,31 @@
         if number > total_cols:
             if mod_positions:
                 width = self.MT.default_column_width
                 for c in range(number - total_cols):
                     self.MT.insert_col_position("end", width)
         elif number < total_cols:
             if not self.MT.all_columns_displayed:
-                self.MT.display_columns(
-                    enable=False, reset_col_positions=False, deselect_all=True
-                )
+                self.MT.display_columns(enable=False, reset_col_positions=False, deselect_all=True)
             self.MT.col_positions[number + 1 :] = []
         if mod_data:
             self.MT.data_dimensions(total_columns=number)
 
     def sheet_display_dimensions(self, total_rows=None, total_columns=None):
         if total_rows is None and total_columns is None:
             return len(self.MT.row_positions) - 1, len(self.MT.col_positions) - 1
         if total_rows is not None:
             height = self.MT.get_lines_cell_height(int(self.MT.default_row_height[0]))
-            self.MT.row_positions = list(
-                accumulate(chain([0], (height for row in range(total_rows))))
-            )
+            self.MT.row_positions = list(accumulate(chain([0], (height for row in range(total_rows)))))
         if total_columns is not None:
             width = self.MT.default_column_width
-            self.MT.col_positions = list(
-                accumulate(chain([0], (width for column in range(total_columns))))
-            )
+            self.MT.col_positions = list(accumulate(chain([0], (width for column in range(total_columns)))))
 
-    def set_sheet_data_and_display_dimensions(
-        self, total_rows=None, total_columns=None
-    ):
-        self.sheet_display_dimensions(
-            total_rows=total_rows, total_columns=total_columns
-        )
+    def set_sheet_data_and_display_dimensions(self, total_rows=None, total_columns=None):
+        self.sheet_display_dimensions(total_rows=total_rows, total_columns=total_columns)
         self.MT.data_dimensions(total_rows=total_rows, total_columns=total_columns)
 
     def move_row_position(self, row: int, moveto: int):
         self.MT.move_row_position(row, moveto)
 
     def move_row(self, row: int, moveto: int):
         self.move_rows(moveto, row, 1)
@@ -1339,29 +1247,25 @@
             self.deselect("all", redraw=False)
         if isinstance(columns, set):
             to_del = columns
         else:
             to_del = set(columns)
         if not to_del:
             return
-        self.MT.data[:] = [
-            [e for c, e in enumerate(r) if c not in to_del] for r in self.MT.data
-        ]
+        self.MT.data[:] = [[e for c, e in enumerate(r) if c not in to_del] for r in self.MT.data]
         to_bis = sorted(to_del)
         if self.MT.all_columns_displayed:
             self.set_column_widths(
                 column_widths=(
                     w
                     for c, w in enumerate(
                         int(b - a)
                         for a, b in zip(
                             self.MT.col_positions,
-                            islice(
-                                self.MT.col_positions, 1, len(self.MT.col_positions)
-                            ),
+                            islice(self.MT.col_positions, 1, len(self.MT.col_positions)),
                         )
                     )
                     if c not in to_del
                 )
             )
         else:
             dispset = set(self.MT.displayed_columns)
@@ -1370,64 +1274,50 @@
                 self.set_column_widths(
                     column_widths=(
                         w
                         for c, w in enumerate(
                             int(b - a)
                             for a, b in zip(
                                 self.MT.col_positions,
-                                islice(
-                                    self.MT.col_positions, 1, len(self.MT.col_positions)
-                                ),
+                                islice(self.MT.col_positions, 1, len(self.MT.col_positions)),
                             )
                         )
                         if c not in widths_to_del
                     )
                 )
             self.MT.displayed_columns = [
-                c
-                if not bisect.bisect_left(to_bis, c)
-                else c - bisect.bisect_left(to_bis, c)
+                c if not bisect.bisect_left(to_bis, c) else c - bisect.bisect_left(to_bis, c)
                 for c in self.MT.displayed_columns
                 if c not in to_del
             ]
         self.MT.cell_options = {
             (
                 r,
-                c
-                if not bisect.bisect_left(to_bis, c)
-                else c - bisect.bisect_left(to_bis, c),
+                c if not bisect.bisect_left(to_bis, c) else c - bisect.bisect_left(to_bis, c),
             ): v
             for (r, c), v in self.MT.cell_options.items()
             if c not in to_del
         }
         self.MT.col_options = {
-            c
-            if not bisect.bisect_left(to_bis, c)
-            else c - bisect.bisect_left(to_bis, c): v
+            c if not bisect.bisect_left(to_bis, c) else c - bisect.bisect_left(to_bis, c): v
             for c, v in self.MT.col_options.items()
             if c not in to_del
         }
         self.CH.cell_options = {
-            c
-            if not bisect.bisect_left(to_bis, c)
-            else c - bisect.bisect_left(to_bis, c): v
+            c if not bisect.bisect_left(to_bis, c) else c - bisect.bisect_left(to_bis, c): v
             for c, v in self.CH.cell_options.items()
             if c not in to_del
         }
         self.set_refresh_timer(redraw)
 
-    def insert_column_position(
-        self, idx="end", width=None, deselect_all=False, redraw=False
-    ):
+    def insert_column_position(self, idx="end", width=None, deselect_all=False, redraw=False):
         self.MT.insert_col_position(idx=idx, width=width, deselect_all=deselect_all)
         self.set_refresh_timer(redraw)
 
-    def insert_column_positions(
-        self, idx="end", widths=None, deselect_all=False, redraw=False
-    ):
+    def insert_column_positions(self, idx="end", widths=None, deselect_all=False, redraw=False):
         self.MT.insert_col_positions(idx=idx, widths=widths, deselect_all=deselect_all)
         self.set_refresh_timer(redraw)
 
     def move_column_position(self, column: int, moveto: int):
         self.MT.move_col_position(column, moveto)
 
     def move_column(self, column: int, moveto: int):
@@ -1473,27 +1363,21 @@
             index_type=index_type.lower(),
         )
         self.set_refresh_timer(redraw)
         return new_selected, dispset
 
     # works on currently selected box
     def open_cell(self, ignore_existing_editor=True):
-        self.MT.open_cell(
-            event=GeneratedMouseEvent(), ignore_existing_editor=ignore_existing_editor
-        )
+        self.MT.open_cell(event=GeneratedMouseEvent(), ignore_existing_editor=ignore_existing_editor)
 
     def open_header_cell(self, ignore_existing_editor=True):
-        self.CH.open_cell(
-            event=GeneratedMouseEvent(), ignore_existing_editor=ignore_existing_editor
-        )
+        self.CH.open_cell(event=GeneratedMouseEvent(), ignore_existing_editor=ignore_existing_editor)
 
     def open_index_cell(self, ignore_existing_editor=True):
-        self.RI.open_cell(
-            event=GeneratedMouseEvent(), ignore_existing_editor=ignore_existing_editor
-        )
+        self.RI.open_cell(event=GeneratedMouseEvent(), ignore_existing_editor=ignore_existing_editor)
 
     def set_text_editor_value(self, text="", r=None, c=None):
         if self.MT.text_editor is not None and r is None and c is None:
             self.MT.text_editor.set_text(text)
         elif self.MT.text_editor is not None and self.MT.text_editor_loc == (r, c):
             self.MT.text_editor.set_text(text)
 
@@ -1565,17 +1449,15 @@
         self.set_refresh_timer(redraw)
 
     def select_row(self, row, redraw=True):
         self.RI.select_row(int(row) if not isinstance(row, int) else row, redraw=False)
         self.set_refresh_timer(redraw)
 
     def select_column(self, column, redraw=True):
-        self.CH.select_col(
-            int(column) if not isinstance(column, int) else column, redraw=False
-        )
+        self.CH.select_col(int(column) if not isinstance(column, int) else column, redraw=False)
         self.set_refresh_timer(redraw)
 
     def select_cell(self, row, column, redraw=True):
         self.MT.select_cell(
             int(row) if not isinstance(row, int) else row,
             int(column) if not isinstance(column, int) else column,
             redraw=False,
@@ -1585,40 +1467,34 @@
     def select_all(self, redraw=True, run_binding_func=True):
         self.MT.select_all(redraw=False, run_binding_func=run_binding_func)
         self.set_refresh_timer(redraw)
 
     def move_down(self):
         self.MT.move_down()
 
-    def add_cell_selection(
-        self, row, column, redraw=True, run_binding_func=True, set_as_current=True
-    ):
+    def add_cell_selection(self, row, column, redraw=True, run_binding_func=True, set_as_current=True):
         self.MT.add_selection(
             r=row,
             c=column,
             redraw=False,
             run_binding_func=run_binding_func,
             set_as_current=set_as_current,
         )
         self.set_refresh_timer(redraw)
 
-    def add_row_selection(
-        self, row, redraw=True, run_binding_func=True, set_as_current=True
-    ):
+    def add_row_selection(self, row, redraw=True, run_binding_func=True, set_as_current=True):
         self.RI.add_selection(
             r=row,
             redraw=False,
             run_binding_func=run_binding_func,
             set_as_current=set_as_current,
         )
         self.set_refresh_timer(redraw)
 
-    def add_column_selection(
-        self, column, redraw=True, run_binding_func=True, set_as_current=True
-    ):
+    def add_column_selection(self, column, redraw=True, run_binding_func=True, set_as_current=True):
         self.CH.add_selection(
             c=column,
             redraw=False,
             run_binding_func=run_binding_func,
             set_as_current=set_as_current,
         )
         self.set_refresh_timer(redraw)
@@ -1689,45 +1565,27 @@
             c=column,
             type_=type_,
             inside=True if self.MT.cell_selected(row, column) else False,
         )
         if selection_binding and self.MT.selection_binding_func is not None:
             self.MT.selection_binding_func(SelectCellEvent("select_cell", row, column))
 
-    def get_selected_rows(
-        self, get_cells=False, get_cells_as_rows=False, return_tuple=False
-    ):
+    def get_selected_rows(self, get_cells=False, get_cells_as_rows=False, return_tuple=False):
         if return_tuple:
-            return tuple(
-                self.MT.get_selected_rows(
-                    get_cells=get_cells, get_cells_as_rows=get_cells_as_rows
-                )
-            )
+            return tuple(self.MT.get_selected_rows(get_cells=get_cells, get_cells_as_rows=get_cells_as_rows))
         else:
-            return self.MT.get_selected_rows(
-                get_cells=get_cells, get_cells_as_rows=get_cells_as_rows
-            )
+            return self.MT.get_selected_rows(get_cells=get_cells, get_cells_as_rows=get_cells_as_rows)
 
-    def get_selected_columns(
-        self, get_cells=False, get_cells_as_columns=False, return_tuple=False
-    ):
+    def get_selected_columns(self, get_cells=False, get_cells_as_columns=False, return_tuple=False):
         if return_tuple:
-            return tuple(
-                self.MT.get_selected_cols(
-                    get_cells=get_cells, get_cells_as_cols=get_cells_as_columns
-                )
-            )
+            return tuple(self.MT.get_selected_cols(get_cells=get_cells, get_cells_as_cols=get_cells_as_columns))
         else:
-            return self.MT.get_selected_cols(
-                get_cells=get_cells, get_cells_as_cols=get_cells_as_columns
-            )
+            return self.MT.get_selected_cols(get_cells=get_cells, get_cells_as_cols=get_cells_as_columns)
 
-    def get_selected_cells(
-        self, get_rows=False, get_columns=False, sort_by_row=False, sort_by_column=False
-    ):
+    def get_selected_cells(self, get_rows=False, get_columns=False, sort_by_row=False, sort_by_column=False):
         if sort_by_row and sort_by_column:
             sels = sorted(
                 self.MT.get_selected_cells(get_rows=get_rows, get_cols=get_columns),
                 key=lambda t: t[1],
             )
             return sorted(sels, key=lambda t: t[0])
         elif sort_by_row:
@@ -1746,17 +1604,15 @@
     def get_all_selection_boxes(self):
         return self.MT.get_all_selection_boxes()
 
     def get_all_selection_boxes_with_types(self):
         return self.MT.get_all_selection_boxes_with_types()
 
     def create_selection_box(self, r1, c1, r2, c2, type_="cells"):
-        return self.MT.create_selected(
-            r1=r1, c1=c1, r2=r2, c2=c2, type_="columns" if type_ == "cols" else type_
-        )
+        return self.MT.create_selected(r1=r1, c1=c1, r2=r2, c2=c2, type_="columns" if type_ == "cols" else type_)
 
     def recreate_all_selection_boxes(self):
         self.MT.recreate_all_selection_boxes()
 
     def cell_visible(self, r, c):
         return self.MT.cell_visible(r, c)
 
@@ -1768,17 +1624,15 @@
 
     def row_selected(self, r):
         return self.MT.row_selected(r)
 
     def column_selected(self, c):
         return self.MT.col_selected(c)
 
-    def anything_selected(
-        self, exclude_columns=False, exclude_rows=False, exclude_cells=False
-    ):
+    def anything_selected(self, exclude_columns=False, exclude_rows=False, exclude_cells=False):
         if self.MT.anything_selected(
             exclude_columns=exclude_columns,
             exclude_rows=exclude_rows,
             exclude_cells=exclude_cells,
         ):
             return True
         return False
@@ -1818,26 +1672,21 @@
                 self.MT.col_options[c]["readonly"] = True
         self.set_refresh_timer(redraw)
 
     def readonly_cells(self, row=0, column=0, cells=[], readonly=True, redraw=False):
         if not readonly:
             if cells:
                 for r, c in cells:
-                    if (
-                        (r, c) in self.MT.cell_options
-                        and "readonly" in self.MT.cell_options[(r, c)]
-                    ):
+                    if (r, c) in self.MT.cell_options and "readonly" in self.MT.cell_options[(r, c)]:
                         del self.MT.cell_options[(r, c)]["readonly"]
             else:
                 if (
                     row,
                     column,
-                ) in self.MT.cell_options and "readonly" in self.MT.cell_options[
-                    (row, column)
-                ]:
+                ) in self.MT.cell_options and "readonly" in self.MT.cell_options[(row, column)]:
                     del self.MT.cell_options[(row, column)]["readonly"]
         else:
             if cells:
                 for r, c in cells:
                     if (r, c) not in self.MT.cell_options:
                         self.MT.cell_options[(r, c)] = {}
                     self.MT.cell_options[(r, c)]["readonly"] = True
@@ -1970,17 +1819,15 @@
                 self.MT.col_options[c]["highlight"] = (
                     self.MT.col_options[c]["highlight"][0] if bg is None else bg,
                     self.MT.col_options[c]["highlight"][1] if fg is None else fg,
                 )
             else:
                 self.MT.col_options[c]["highlight"] = (bg, fg)
         if highlight_header:
-            self.highlight_cells(
-                cells=columns, canvas="header", bg=bg, fg=fg, redraw=False
-            )
+            self.highlight_cells(cells=columns, canvas="header", bg=bg, fg=fg, redraw=False)
         self.set_refresh_timer(redraw)
 
     def highlight_cells(
         self,
         row=0,
         column=0,
         cells=[],
@@ -1995,68 +1842,45 @@
         if canvas == "table":
             if cells:
                 for r_, c_ in cells:
                     if (r_, c_) not in self.MT.cell_options:
                         self.MT.cell_options[(r_, c_)] = {}
                     if "highlight" in self.MT.cell_options[(r_, c_)] and not overwrite:
                         self.MT.cell_options[(r_, c_)]["highlight"] = (
-                            self.MT.cell_options[(r_, c_)]["highlight"][0]
-                            if bg is None
-                            else bg,
-                            self.MT.cell_options[(r_, c_)]["highlight"][1]
-                            if fg is None
-                            else fg,
+                            self.MT.cell_options[(r_, c_)]["highlight"][0] if bg is None else bg,
+                            self.MT.cell_options[(r_, c_)]["highlight"][1] if fg is None else fg,
                         )
                     else:
                         self.MT.cell_options[(r_, c_)]["highlight"] = (bg, fg)
             else:
-                if (
-                    isinstance(row, str)
-                    and row.lower() == "all"
-                    and isinstance(column, int)
-                ):
+                if isinstance(row, str) and row.lower() == "all" and isinstance(column, int):
                     riter = range(self.MT.total_data_rows())
                     citer = (column,)
-                elif (
-                    isinstance(column, str)
-                    and column.lower() == "all"
-                    and isinstance(row, int)
-                ):
+                elif isinstance(column, str) and column.lower() == "all" and isinstance(row, int):
                     riter = (row,)
                     citer = range(self.MT.total_data_cols())
                 elif isinstance(row, int) and isinstance(column, int):
                     riter = (row,)
                     citer = (column,)
                 for r_ in riter:
                     for c_ in citer:
                         if (r_, c_) not in self.MT.cell_options:
                             self.MT.cell_options[(r_, c_)] = {}
-                        if (
-                            "highlight" in self.MT.cell_options[(r_, c_)]
-                            and not overwrite
-                        ):
+                        if "highlight" in self.MT.cell_options[(r_, c_)] and not overwrite:
                             self.MT.cell_options[(r_, c_)]["highlight"] = (
-                                self.MT.cell_options[(r_, c_)]["highlight"][0]
-                                if bg is None
-                                else bg,
-                                self.MT.cell_options[(r_, c_)]["highlight"][1]
-                                if fg is None
-                                else fg,
+                                self.MT.cell_options[(r_, c_)]["highlight"][0] if bg is None else bg,
+                                self.MT.cell_options[(r_, c_)]["highlight"][1] if fg is None else fg,
                             )
                         else:
                             self.MT.cell_options[(r_, c_)]["highlight"] = (bg, fg)
         elif canvas in ("row_index", "index"):
             if bg is None and fg is None:
                 return
             iterable = (
-                cells
-                if (cells and not isinstance(cells, int))
-                else (cells,)
-                if isinstance(cells, int)
-                else (row,)
+                cells if (cells and not isinstance(cells, int)) else (cells,) if isinstance(cells, int) else (row,)
             )
             for r_ in iterable:
                 if r_ not in self.RI.cell_options:
                     self.RI.cell_options[r_] = {}
                 if "highlight" in self.RI.cell_options[r_] and not overwrite:
                     self.RI.cell_options[r_]["highlight"] = (
                         self.RI.cell_options[r_]["highlight"][0] if bg is None else bg,
@@ -2064,35 +1888,29 @@
                     )
                 else:
                     self.RI.cell_options[r_]["highlight"] = (bg, fg)
         elif canvas == "header":
             if bg is None and fg is None:
                 return
             iterable = (
-                cells
-                if (cells and not isinstance(cells, int))
-                else (cells,)
-                if isinstance(cells, int)
-                else (column,)
+                cells if (cells and not isinstance(cells, int)) else (cells,) if isinstance(cells, int) else (column,)
             )
             for c_ in iterable:
                 if c_ not in self.CH.cell_options:
                     self.CH.cell_options[c_] = {}
                 if "highlight" in self.CH.cell_options[c_] and not overwrite:
                     self.CH.cell_options[c_]["highlight"] = (
                         self.CH.cell_options[c_]["highlight"][0] if bg is None else bg,
                         self.CH.cell_options[c_]["highlight"][1] if fg is None else fg,
                     )
                 else:
                     self.CH.cell_options[c_]["highlight"] = (bg, fg)
         self.set_refresh_timer(redraw)
 
-    def dehighlight_cells(
-        self, row=0, column=0, cells=[], canvas="table", all_=False, redraw=True
-    ):
+    def dehighlight_cells(self, row=0, column=0, cells=[], canvas="table", all_=False, redraw=True):
         if row == "all" and canvas == "table":
             for k, v in self.MT.cell_options.items():
                 if "highlight" in v:
                     del self.MT.cell_options[k]["highlight"]
         elif row == "all" and canvas == "row_index":
             for k, v in self.RI.cell_options.items():
                 if "highlight" in v:
@@ -2108,70 +1926,56 @@
                         del self.MT.cell_options[t]["highlight"]
                     except Exception:
                         pass
             elif not all_:
                 if (
                     row,
                     column,
-                ) in self.MT.cell_options and "highlight" in self.MT.cell_options[
-                    (row, column)
-                ]:
+                ) in self.MT.cell_options and "highlight" in self.MT.cell_options[(row, column)]:
                     del self.MT.cell_options[(row, column)]["highlight"]
             elif all_:
                 for k in self.MT.cell_options:
                     if "highlight" in self.MT.cell_options[k]:
                         del self.MT.cell_options[k]["highlight"]
         elif canvas == "row_index":
             if cells and not all_:
                 for r in cells:
                     try:
                         del self.RI.cell_options[r]["highlight"]
                     except Exception:
                         pass
             elif not all_:
-                if (
-                    row in self.RI.cell_options
-                    and "highlight" in self.RI.cell_options[row]
-                ):
+                if row in self.RI.cell_options and "highlight" in self.RI.cell_options[row]:
                     del self.RI.cell_options[row]["highlight"]
             elif all_:
                 for r in self.RI.cell_options:
                     if "highlight" in self.RI.cell_options[r]:
                         del self.RI.cell_options[r]["highlight"]
         elif canvas == "header":
             if cells and not all_:
                 for c in cells:
                     try:
                         del self.CH.cell_options[c]["highlight"]
                     except Exception:
                         pass
             elif not all_:
-                if (
-                    column in self.CH.cell_options
-                    and "highlight" in self.CH.cell_options[column]
-                ):
+                if column in self.CH.cell_options and "highlight" in self.CH.cell_options[column]:
                     del self.CH.cell_options[column]["highlight"]
             elif all_:
                 for c in self.CH.cell_options:
                     if "highlight" in self.CH.cell_options[c]:
                         del self.CH.cell_options[c]["highlight"]
         self.set_refresh_timer(redraw)
 
     def delete_out_of_bounds_options(self):
         maxc = self.total_columns()
         maxr = self.total_rows()
-        self.MT.cell_options = {
-            k: v for k, v in self.MT.cell_options.items() if k[0] < maxr and k[1] < maxc
-        }
-        self.RI.cell_options = {
-            k: v for k, v in self.RI.cell_options.items() if k < maxr
-        }
-        self.CH.cell_options = {
-            k: v for k, v in self.CH.cell_options.items() if k < maxc
-        }
+        self.MT.cell_options = {k: v for k, v in self.MT.cell_options.items() if k[0] < maxr and k[1] < maxc}
+        self.RI.cell_options = {k: v for k, v in self.RI.cell_options.items() if k < maxr}
+        self.CH.cell_options = {k: v for k, v in self.CH.cell_options.items() if k < maxc}
         self.MT.col_options = {k: v for k, v in self.MT.col_options.items() if k < maxc}
         self.MT.row_options = {k: v for k, v in self.MT.row_options.items() if k < maxr}
 
     def reset_all_options(self):
         self.MT.cell_options = {}
         self.RI.cell_options = {}
         self.CH.cell_options = {}
@@ -2184,31 +1988,19 @@
         elif canvas == "row_index":
             return self.RI.cell_options
         elif canvas == "header":
             return self.CH.cell_options
 
     def get_highlighted_cells(self, canvas="table"):
         if canvas == "table":
-            return {
-                k: v["highlight"]
-                for k, v in self.MT.cell_options.items()
-                if "highlight" in v
-            }
+            return {k: v["highlight"] for k, v in self.MT.cell_options.items() if "highlight" in v}
         elif canvas == "row_index":
-            return {
-                k: v["highlight"]
-                for k, v in self.RI.cell_options.items()
-                if "highlight" in v
-            }
+            return {k: v["highlight"] for k, v in self.RI.cell_options.items() if "highlight" in v}
         elif canvas == "header":
-            return {
-                k: v["highlight"]
-                for k, v in self.CH.cell_options.items()
-                if "highlight" in v
-            }
+            return {k: v["highlight"] for k, v in self.CH.cell_options.items() if "highlight" in v}
 
     def get_frame_y(self, y: int):
         return y + self.CH.current_height
 
     def get_frame_x(self, x: int):
         return x + self.RI.current_width
 
@@ -2216,34 +2008,26 @@
         a = align.lower()
         if a in ("c", "center", "centre"):
             return "center"
         elif a in ("w", "west", "left"):
             return "w"
         elif a in ("e", "east", "right"):
             return "e"
-        raise ValueError(
-            "Align must be one of the following values: c, center, w, west, left, e, east, right"
-        )
+        raise ValueError("Align must be one of the following values: c, center, w, west, left, e, east, right")
 
     def get_cell_alignments(self):
-        return {
-            (r, c): v["align"]
-            for (r, c), v in self.MT.cell_options.items()
-            if "align" in v
-        }
+        return {(r, c): v["align"] for (r, c), v in self.MT.cell_options.items() if "align" in v}
 
     def get_column_alignments(self):
         return {c: v["align"] for c, v in self.MT.col_options.items() if "align" in v}
 
     def get_row_alignments(self):
         return {r: v["align"] for r, v in self.MT.row_options.items() if "align" in v}
 
-    def align_rows(
-        self, rows=[], align="global", align_index=False, redraw=True
-    ):  # "center", "w", "e" or "global"
+    def align_rows(self, rows=[], align="global", align_index=False, redraw=True):  # "center", "w", "e" or "global"
         if align == "global" or self.convert_align(align):
             if isinstance(rows, dict):
                 for k, v in rows.items():
                     self.MT.align_rows(rows=k, align=v, align_index=align_index)
             else:
                 self.MT.align_rows(
                     rows=rows,
@@ -2263,17 +2047,15 @@
                 self.MT.align_columns(
                     columns=columns,
                     align=align if align == "global" else self.convert_align(align),
                     align_header=align_header,
                 )
         self.set_refresh_timer(redraw)
 
-    def align_cells(
-        self, row=0, column=0, cells=[], align="global", redraw=True
-    ):  # "center", "w", "e" or "global"
+    def align_cells(self, row=0, column=0, cells=[], align="global", redraw=True):  # "center", "w", "e" or "global"
         if align == "global" or self.convert_align(align):
             if isinstance(cells, dict):
                 for (r, c), v in cells.items():
                     self.MT.align_cells(row=r, column=c, cells=[], align=v)
             else:
                 self.MT.align_cells(
                     row=row,
@@ -2309,46 +2091,40 @@
 
     def align(self, align: str = None, redraw=True):
         if align is None:
             return self.MT.align
         elif self.convert_align(align):
             self.MT.align = self.convert_align(align)
         else:
-            raise ValueError(
-                "Align must be one of the following values: c, center, w, west, e, east"
-            )
+            raise ValueError("Align must be one of the following values: c, center, w, west, e, east")
         self.set_refresh_timer(redraw)
 
     def header_align(self, align: str = None, redraw=True):
         if align is None:
             return self.CH.align
         elif self.convert_align(align):
             self.CH.align = self.convert_align(align)
         else:
-            raise ValueError(
-                "Align must be one of the following values: c, center, w, west, e, east"
-            )
+            raise ValueError("Align must be one of the following values: c, center, w, west, e, east")
         self.set_refresh_timer(redraw)
 
     def row_index_align(self, align: str = None, redraw=True):
         if align is None:
             return self.RI.align
         elif self.convert_align(align):
             self.RI.align = self.convert_align(align)
         else:
-            raise ValueError(
-                "Align must be one of the following values: c, center, w, west, e, east"
-            )
+            raise ValueError("Align must be one of the following values: c, center, w, west, e, east")
         self.set_refresh_timer(redraw)
 
     def font(self, newfont=None, reset_row_positions=True):
-        self.MT.font(newfont, reset_row_positions=reset_row_positions)
+        return self.MT.set_table_font(newfont, reset_row_positions=reset_row_positions)
 
     def header_font(self, newfont=None):
-        self.MT.header_font(newfont)
+        return self.MT.set_header_font(newfont)
 
     def set_options(self, redraw=True, **kwargs):
         if "to_clipboard_delimiter" in kwargs:
             self.MT.to_clipboard_delimiter = kwargs["to_clipboard_delimiter"]
         if "to_clipboard_quotechar" in kwargs:
             self.MT.to_clipboard_quotechar = kwargs["to_clipboard_quotechar"]
         if "to_clipboard_lineterminator" in kwargs:
@@ -2356,101 +2132,73 @@
         if "from_clipboard_delimiters" in kwargs:
             self.MT.from_clipboard_delimiters = kwargs["from_clipboard_delimiters"]
         if "show_dropdown_borders" in kwargs:
             self.MT.show_dropdown_borders = kwargs["show_dropdown_borders"]
         if "edit_cell_validation" in kwargs:
             self.MT.edit_cell_validation = kwargs["edit_cell_validation"]
         if "show_default_header_for_empty" in kwargs:
-            self.CH.show_default_header_for_empty = kwargs[
-                "show_default_header_for_empty"
-            ]
+            self.CH.show_default_header_for_empty = kwargs["show_default_header_for_empty"]
         if "show_default_index_for_empty" in kwargs:
-            self.RI.show_default_index_for_empty = kwargs[
-                "show_default_index_for_empty"
-            ]
+            self.RI.show_default_index_for_empty = kwargs["show_default_index_for_empty"]
         if "selected_rows_to_end_of_window" in kwargs:
-            self.MT.selected_rows_to_end_of_window = kwargs[
-                "selected_rows_to_end_of_window"
-            ]
+            self.MT.selected_rows_to_end_of_window = kwargs["selected_rows_to_end_of_window"]
         if "horizontal_grid_to_end_of_window" in kwargs:
-            self.MT.horizontal_grid_to_end_of_window = kwargs[
-                "horizontal_grid_to_end_of_window"
-            ]
+            self.MT.horizontal_grid_to_end_of_window = kwargs["horizontal_grid_to_end_of_window"]
         if "vertical_grid_to_end_of_window" in kwargs:
-            self.MT.vertical_grid_to_end_of_window = kwargs[
-                "vertical_grid_to_end_of_window"
-            ]
+            self.MT.vertical_grid_to_end_of_window = kwargs["vertical_grid_to_end_of_window"]
         if "paste_insert_column_limit" in kwargs:
             self.MT.paste_insert_column_limit = kwargs["paste_insert_column_limit"]
         if "paste_insert_row_limit" in kwargs:
             self.MT.paste_insert_row_limit = kwargs["paste_insert_row_limit"]
         if "expand_sheet_if_paste_too_big" in kwargs:
-            self.MT.expand_sheet_if_paste_too_big = kwargs[
-                "expand_sheet_if_paste_too_big"
-            ]
+            self.MT.expand_sheet_if_paste_too_big = kwargs["expand_sheet_if_paste_too_big"]
         if "arrow_key_down_right_scroll_page" in kwargs:
-            self.MT.arrow_key_down_right_scroll_page = kwargs[
-                "arrow_key_down_right_scroll_page"
-            ]
+            self.MT.arrow_key_down_right_scroll_page = kwargs["arrow_key_down_right_scroll_page"]
         if "enable_edit_cell_auto_resize" in kwargs:
             self.MT.cell_auto_resize_enabled = kwargs["enable_edit_cell_auto_resize"]
         if "header_hidden_columns_expander_bg" in kwargs:
-            self.CH.header_hidden_columns_expander_bg = kwargs[
-                "header_hidden_columns_expander_bg"
-            ]
+            self.CH.header_hidden_columns_expander_bg = kwargs["header_hidden_columns_expander_bg"]
         if "index_hidden_rows_expander_bg" in kwargs:
-            self.RI.index_hidden_rows_expander_bg = kwargs[
-                "index_hidden_rows_expander_bg"
-            ]
+            self.RI.index_hidden_rows_expander_bg = kwargs["index_hidden_rows_expander_bg"]
         if "page_up_down_select_row" in kwargs:
             self.MT.page_up_down_select_row = kwargs["page_up_down_select_row"]
         if "display_selected_fg_over_highlights" in kwargs:
-            self.MT.display_selected_fg_over_highlights = kwargs[
-                "display_selected_fg_over_highlights"
-            ]
+            self.MT.display_selected_fg_over_highlights = kwargs["display_selected_fg_over_highlights"]
         if "show_horizontal_grid" in kwargs:
             self.MT.show_horizontal_grid = kwargs["show_horizontal_grid"]
         if "show_vertical_grid" in kwargs:
             self.MT.show_vertical_grid = kwargs["show_vertical_grid"]
         if "empty_horizontal" in kwargs:
             self.MT.empty_horizontal = kwargs["empty_horizontal"]
         if "empty_vertical" in kwargs:
             self.MT.empty_vertical = kwargs["empty_vertical"]
         if "row_height" in kwargs:
             self.MT.default_row_height = (
-                kwargs["row_height"]
-                if isinstance(kwargs["row_height"], str)
-                else "pixels",
+                kwargs["row_height"] if isinstance(kwargs["row_height"], str) else "pixels",
                 kwargs["row_height"]
                 if isinstance(kwargs["row_height"], int)
                 else self.MT.get_lines_cell_height(int(kwargs["row_height"])),
             )
         if "column_width" in kwargs:
             self.MT.default_column_width = (
                 self.MT.min_column_width + 20
                 if kwargs["column_width"] < self.MT.min_column_width
                 else int(kwargs["column_width"])
             )
         if "header_height" in kwargs:
             self.MT.default_header_height = (
-                kwargs["header_height"]
-                if isinstance(kwargs["header_height"], str)
-                else "pixels",
+                kwargs["header_height"] if isinstance(kwargs["header_height"], str) else "pixels",
                 kwargs["header_height"]
                 if isinstance(kwargs["header_height"], int)
-                else self.MT.get_lines_cell_height(
-                    int(kwargs["header_height"]), font=self.MT.header_font
-                ),
+                else self.MT.get_lines_cell_height(int(kwargs["header_height"]), font=self.MT.header_font),
             )
         if "row_drag_and_drop_perform" in kwargs:
             self.RI.row_drag_and_drop_perform = kwargs["row_drag_and_drop_perform"]
         if "column_drag_and_drop_perform" in kwargs:
-            self.CH.column_drag_and_drop_perform = kwargs[
-                "column_drag_and_drop_perform"
-            ]
+            self.CH.column_drag_and_drop_perform = kwargs["column_drag_and_drop_perform"]
         if "popup_menu_font" in kwargs:
             self.MT.popup_menu_font = kwargs["popup_menu_font"]
         if "popup_menu_fg" in kwargs:
             self.MT.popup_menu_fg = kwargs["popup_menu_fg"]
         if "popup_menu_bg" in kwargs:
             self.MT.popup_menu_bg = kwargs["popup_menu_bg"]
         if "popup_menu_highlight_bg" in kwargs:
@@ -2466,25 +2214,21 @@
         if "header_selected_columns_fg" in kwargs:
             self.CH.header_selected_columns_fg = kwargs["header_selected_columns_fg"]
         if "index_selected_rows_bg" in kwargs:
             self.RI.index_selected_rows_bg = kwargs["index_selected_rows_bg"]
         if "index_selected_rows_fg" in kwargs:
             self.RI.index_selected_rows_fg = kwargs["index_selected_rows_fg"]
         if "table_selected_rows_border_fg" in kwargs:
-            self.MT.table_selected_rows_border_fg = kwargs[
-                "table_selected_rows_border_fg"
-            ]
+            self.MT.table_selected_rows_border_fg = kwargs["table_selected_rows_border_fg"]
         if "table_selected_rows_bg" in kwargs:
             self.MT.table_selected_rows_bg = kwargs["table_selected_rows_bg"]
         if "table_selected_rows_fg" in kwargs:
             self.MT.table_selected_rows_fg = kwargs["table_selected_rows_fg"]
         if "table_selected_columns_border_fg" in kwargs:
-            self.MT.table_selected_columns_border_fg = kwargs[
-                "table_selected_columns_border_fg"
-            ]
+            self.MT.table_selected_columns_border_fg = kwargs["table_selected_columns_border_fg"]
         if "table_selected_columns_bg" in kwargs:
             self.MT.table_selected_columns_bg = kwargs["table_selected_columns_bg"]
         if "table_selected_columns_fg" in kwargs:
             self.MT.table_selected_columns_fg = kwargs["table_selected_columns_fg"]
         if "default_header" in kwargs:
             self.CH.default_header = kwargs["default_header"].lower()
         if "default_row_index" in kwargs:
@@ -2494,19 +2238,19 @@
         if "max_row_height" in kwargs:
             self.MT.max_row_height = float(kwargs["max_row_height"])
         if "max_header_height" in kwargs:
             self.MT.max_header_height = float(kwargs["max_header_height"])
         if "max_index_width" in kwargs:
             self.MT.max_index_width = float(kwargs["max_index_width"])
         if "font" in kwargs:
-            self.MT.font(kwargs["font"])
+            self.MT.set_table_font(kwargs["font"])
         if "header_font" in kwargs:
-            self.MT.header_font(kwargs["header_font"])
+            self.MT.set_header_font(kwargs["header_font"])
         if "index_font" in kwargs:
-            self.MT.index_font(kwargs["index_font"])
+            self.MT.set_index_font(kwargs["index_font"])
         if "theme" in kwargs:
             self.change_theme(kwargs["theme"])
         if "show_selected_cells_border" in kwargs:
             self.MT.show_selected_cells_border = kwargs["show_selected_cells_border"]
         if "header_bg" in kwargs:
             self.CH.config(background=kwargs["header_bg"])
             self.CH.header_bg = kwargs["header_bg"]
@@ -2545,17 +2289,15 @@
             self.MT.config(background=kwargs["table_bg"])
             self.MT.table_bg = kwargs["table_bg"]
         if "table_grid_fg" in kwargs:
             self.MT.table_grid_fg = kwargs["table_grid_fg"]
         if "table_fg" in kwargs:
             self.MT.table_fg = kwargs["table_fg"]
         if "table_selected_cells_border_fg" in kwargs:
-            self.MT.table_selected_cells_border_fg = kwargs[
-                "table_selected_cells_border_fg"
-            ]
+            self.MT.table_selected_cells_border_fg = kwargs["table_selected_cells_border_fg"]
         if "table_selected_cells_bg" in kwargs:
             self.MT.table_selected_cells_bg = kwargs["table_selected_cells_bg"]
         if "table_selected_cells_fg" in kwargs:
             self.MT.table_selected_cells_fg = kwargs["table_selected_cells_fg"]
         if "resizing_line_fg" in kwargs:
             self.CH.resizing_line_fg = kwargs["resizing_line_fg"]
             self.RI.resizing_line_fg = kwargs["resizing_line_fg"]
@@ -2611,59 +2353,38 @@
         only_columns=None,
         **kwargs,
     ):
         if only_rows is not None:
             if isinstance(only_rows, int):
                 only_rows = (only_rows,)
             elif not is_iterable(only_rows):
-                raise ValueError(
-                    f"Argument 'only_rows' must be either int or iterable or None. Not {type(only_rows)}"
-                )
+                raise ValueError(f"Argument 'only_rows' must be either int or iterable or None. Not {type(only_rows)}")
         if only_columns is not None:
             if isinstance(only_columns, int):
                 only_columns = (only_columns,)
             elif not is_iterable(only_columns):
                 raise ValueError(
                     f"Argument 'only_columns' must be either int or iterable or None. Not {type(only_columns)}"
                 )
         if get_header:
-            maxlen = (
-                len(self.MT._headers)
-                if isinstance(self.MT._headers, (list, tuple))
-                else 0
-            )
+            maxlen = len(self.MT._headers) if isinstance(self.MT._headers, (list, tuple)) else 0
             data = []
             for rn in only_rows if only_rows is not None else range(len(self.MT.data)):
-                r = self.get_row_data(
-                    rn, get_displayed=get_displayed, only_columns=only_columns
-                )
+                r = self.get_row_data(rn, get_displayed=get_displayed, only_columns=only_columns)
                 if len(r) > maxlen:
                     maxlen = len(r)
                 if get_index:
-                    data.append(
-                        [self.get_index_data(rn, get_displayed=get_index_displayed)] + r
-                    )
+                    data.append([self.get_index_data(rn, get_displayed=get_index_displayed)] + r)
                 else:
                     data.append(r)
             iterable = only_columns if only_columns is not None else range(maxlen)
             if get_index:
-                return [
-                    [""]
-                    + [
-                        self.get_header_data(cn, get_displayed=get_header_displayed)
-                        for cn in iterable
-                    ]
-                ] + data
+                return [[""] + [self.get_header_data(cn, get_displayed=get_header_displayed) for cn in iterable]] + data
             else:
-                return [
-                    [
-                        self.get_header_data(cn, get_displayed=get_header_displayed)
-                        for cn in iterable
-                    ]
-                ] + data
+                return [[self.get_header_data(cn, get_displayed=get_header_displayed) for cn in iterable]] + data
         elif not get_header:
             iterable = only_rows if only_rows is not None else range(len(self.MT.data))
             return [
                 self.get_row_data(
                     rn,
                     get_displayed=get_displayed,
                     get_index=get_index,
@@ -2693,50 +2414,40 @@
                     f"Argument 'only_columns' must be either int or iterable or None. Not {type(only_columns)}"
                 )
         if r >= self.MT.total_data_rows():
             raise IndexError(f"Row #{r} is out of range.")
         if r >= len(self.MT.data):
             total_data_cols = self.MT.total_data_cols()
             self.MT.fix_data_len(r, total_data_cols - 1)
-        iterable = (
-            only_columns if only_columns is not None else range(len(self.MT.data[r]))
-        )
+        iterable = only_columns if only_columns is not None else range(len(self.MT.data[r]))
         if get_index:
             return [self.get_index_data(r, get_displayed=get_index_displayed)] + [
-                self.MT.get_cell_data(r, c, get_displayed=get_displayed)
-                for c in iterable
+                self.MT.get_cell_data(r, c, get_displayed=get_displayed) for c in iterable
             ]
         else:
-            return [
-                self.MT.get_cell_data(r, c, get_displayed=get_displayed)
-                for c in iterable
-            ]
+            return [self.MT.get_cell_data(r, c, get_displayed=get_displayed) for c in iterable]
 
     def get_column_data(
         self,
         c,
         get_displayed=False,
         get_header=False,
         get_header_displayed=True,
         only_rows=None,
         **kwargs,
     ):
         if only_rows is not None:
             if isinstance(only_rows, int):
                 only_rows = (only_rows,)
             elif not is_iterable(only_rows):
-                raise ValueError(
-                    f"Argument 'only_rows' must be either int or iterable or None. Not {type(only_rows)}"
-                )
+                raise ValueError(f"Argument 'only_rows' must be either int or iterable or None. Not {type(only_rows)}")
         iterable = only_rows if only_rows is not None else range(len(self.MT.data))
-        return (
-            [self.get_header_data(c, get_displayed=get_header_displayed)]
-            if get_header
-            else []
-        ) + [self.MT.get_cell_data(r, c, get_displayed=get_displayed) for r in iterable]
+        return ([self.get_header_data(c, get_displayed=get_header_displayed)] if get_header else []) + [
+            self.MT.get_cell_data(r, c, get_displayed=get_displayed) for r in iterable
+        ]
 
     def yield_sheet_rows(
         self,
         get_displayed=False,
         get_header=False,
         get_index=False,
         get_index_displayed=True,
@@ -2745,30 +2456,27 @@
         only_columns=None,
         **kwargs,
     ):
         if only_rows is not None:
             if isinstance(only_rows, int):
                 only_rows = (only_rows,)
             elif not is_iterable(only_rows):
-                raise ValueError(
-                    f"Argument 'only_rows' must be either int or iterable or None. Not {type(only_rows)}"
-                )
+                raise ValueError(f"Argument 'only_rows' must be either int or iterable or None. Not {type(only_rows)}")
         if only_columns is not None:
             if isinstance(only_columns, int):
                 only_columns = (only_columns,)
             elif not is_iterable(only_columns):
                 raise ValueError(
                     f"Argument 'only_columns' must be either int or iterable or None. Not {type(only_columns)}"
                 )
         if get_header:
             maxlen = self.MT.total_data_cols()
             iterable = only_columns if only_columns is not None else range(maxlen)
             yield ([""] if get_index else []) + [
-                self.get_header_data(c, get_displayed=get_header_displayed)
-                for c in iterable
+                self.get_header_data(c, get_displayed=get_header_displayed) for c in iterable
             ]
         iterable = only_rows if only_rows is not None else range(len(self.MT.data))
         yield from (
             self.get_row_data(
                 r,
                 get_displayed=get_displayed,
                 get_index=get_index,
@@ -2790,34 +2498,28 @@
     def data_reference(
         self,
         newdataref=None,
         reset_col_positions=True,
         reset_row_positions=True,
         redraw=False,
     ):
-        return self.MT.data_reference(
-            newdataref, reset_col_positions, reset_row_positions, redraw
-        )
+        return self.MT.data_reference(newdataref, reset_col_positions, reset_row_positions, redraw)
 
     def set_sheet_data(
         self,
         data=[[]],
         reset_col_positions=True,
         reset_row_positions=True,
         redraw=True,
         verify=False,
         reset_highlights=False,
         keep_formatting=True,
     ):
-        if verify and (
-            not isinstance(data, list) or not all(isinstance(row, list) for row in data)
-        ):
-            raise ValueError(
-                "Data argument must be a list of lists, sublists being rows"
-            )
+        if verify and (not isinstance(data, list) or not all(isinstance(row, list) for row in data)):
+            raise ValueError("Data argument must be a list of lists, sublists being rows")
         if reset_highlights:
             self.dehighlight_all()
         return self.MT.data_reference(
             data,
             reset_col_positions,
             reset_row_positions,
             redraw,
@@ -2828,47 +2530,39 @@
     def set_cell_data(self, r, c, value="", redraw=False, keep_formatting=True):
         if not keep_formatting:
             self.MT.delete_cell_format(r, c, clear_values=False)
         self.MT.set_cell_data(r, c, value)
         if redraw:
             self.set_refresh_timer()
 
-    def set_row_data(
-        self, r, values=tuple(), add_columns=True, redraw=False, keep_formatting=True
-    ):
+    def set_row_data(self, r, values=tuple(), add_columns=True, redraw=False, keep_formatting=True):
         if r >= len(self.MT.data):
             raise Exception("Row number is out of range")
         if not keep_formatting:
             self.MT.delete_row_format(r, clear_values=False)
         maxidx = len(self.MT.data[r]) - 1
         if not values:
             self.MT.data[r][:] = self.MT.get_empty_row_seq(r, len(self.MT.data[r]))
         if add_columns:
             for c, v in enumerate(values):
                 if c > maxidx:
                     self.MT.data[r].append(v)
                     if self.MT.all_columns_displayed:
                         self.MT.insert_col_position("end")
                 else:
-                    self.set_cell_data(
-                        r=r, c=c, value=v, redraw=False, keep_formatting=keep_formatting
-                    )
+                    self.set_cell_data(r=r, c=c, value=v, redraw=False, keep_formatting=keep_formatting)
         else:
             for c, v in enumerate(values):
                 if c > maxidx:
                     self.MT.data[r].append(v)
                 else:
-                    self.set_cell_data(
-                        r=r, c=c, value=v, redraw=False, keep_formatting=keep_formatting
-                    )
+                    self.set_cell_data(r=r, c=c, value=v, redraw=False, keep_formatting=keep_formatting)
         self.set_refresh_timer(redraw)
 
-    def set_column_data(
-        self, c, values=tuple(), add_rows=True, redraw=False, keep_formatting=True
-    ):
+    def set_column_data(self, c, values=tuple(), add_rows=True, redraw=False, keep_formatting=True):
         if not keep_formatting:
             self.MT.delete_column_format(c, clear_values=False)
         if add_rows:
             maxidx = len(self.MT.data) - 1
             total_cols = None
             height = self.MT.default_row_height[1]
             for rn, v in enumerate(values):
@@ -2877,43 +2571,35 @@
                         total_cols = self.MT.total_data_cols()
                     self.MT.fix_data_len(rn, total_cols - 1)
                     if self.MT.all_rows_displayed:
                         self.MT.insert_row_position("end", height=height)
                     maxidx += 1
                 if c >= len(self.MT.data[rn]):
                     self.MT.fix_row_len(rn, c)
-                self.set_cell_data(
-                    r=rn, c=c, value=v, redraw=False, keep_formatting=keep_formatting
-                )
+                self.set_cell_data(r=rn, c=c, value=v, redraw=False, keep_formatting=keep_formatting)
         else:
             for rn, v in enumerate(values):
                 if c >= len(self.MT.data[rn]):
                     self.MT.fix_row_len(rn, c)
-                self.set_cell_data(
-                    r=rn, c=c, value=v, redraw=False, keep_formatting=keep_formatting
-                )
+                self.set_cell_data(r=rn, c=c, value=v, redraw=False, keep_formatting=keep_formatting)
         self.set_refresh_timer(redraw)
 
     def insert_column(
         self,
         values: Union[list, tuple, int, None] = None,
         idx: Union[str, int] = "end",
         width=None,
         deselect_all=False,
         add_rows=True,
         equalize_data_row_lengths=True,
         mod_column_positions=True,
         redraw=True,
     ):
         self.insert_columns(
-            (values,)
-            if isinstance(values, (list, tuple))
-            else 1
-            if values is None
-            else values,
+            (values,) if isinstance(values, (list, tuple)) else 1 if values is None else values,
             idx,
             (width,) if isinstance(width, int) else width,
             deselect_all,
             add_rows,
             equalize_data_row_lengths,
             mod_column_positions,
             redraw,
@@ -2936,70 +2622,56 @@
             old_total = self.MT.total_data_cols()
         if isinstance(columns, int):
             if columns < 1:
                 raise ValueError(f"columns arg must be greater than 0, not {columns}")
             total_rows = self.MT.total_data_rows()
             start = old_total if idx == "end" else idx
             data = [
-                self.MT.get_empty_row_seq(
-                    rn, end=start + columns, start=start, c_ops=idx == "end"
-                )
+                self.MT.get_empty_row_seq(rn, end=start + columns, start=start, c_ops=idx == "end")
                 for rn in range(total_rows)
             ]
             numcols = columns
         else:
             data = columns
             numcols = len(columns)
         if self.MT.all_columns_displayed:
             if mod_column_positions:
                 self.MT.insert_col_positions(
                     idx=idx,
-                    widths=columns
-                    if isinstance(columns, int) and widths is None
-                    else widths,
+                    widths=columns if isinstance(columns, int) and widths is None else widths,
                     deselect_all=deselect_all,
                 )
         elif not self.MT.all_columns_displayed:
             if idx != "end":
-                self.MT.displayed_columns = [
-                    c if c < idx else c + numcols for c in self.MT.displayed_columns
-                ]
+                self.MT.displayed_columns = [c if c < idx else c + numcols for c in self.MT.displayed_columns]
             if mod_column_positions:
                 inspos = bisect.bisect_left(self.MT.displayed_columns, idx)
-                self.MT.displayed_columns[inspos:inspos] = list(
-                    range(idx, idx + numcols)
-                )
+                self.MT.displayed_columns[inspos:inspos] = list(range(idx, idx + numcols))
                 self.MT.insert_col_positions(
                     idx=inspos,
-                    widths=columns
-                    if isinstance(columns, int) and widths is None
-                    else widths,
+                    widths=columns if isinstance(columns, int) and widths is None else widths,
                     deselect_all=deselect_all,
                 )
         maxidx = len(self.MT.data) - 1
         if add_rows:
             height = self.MT.default_row_height[1]
             if idx == "end":
                 for values in reversed(data):
                     for rn, v in enumerate(values):
                         if rn > maxidx:
-                            self.MT.data.append(
-                                self.MT.get_empty_row_seq(rn, old_total)
-                            )
+                            self.MT.data.append(self.MT.get_empty_row_seq(rn, old_total))
                             if self.MT.all_rows_displayed:
                                 self.MT.insert_row_position("end", height=height)
                             maxidx += 1
                         self.MT.data[rn].append(v)
             else:
                 for values in reversed(data):
                     for rn, v in enumerate(values):
                         if rn > maxidx:
-                            self.MT.data.append(
-                                self.MT.get_empty_row_seq(rn, old_total)
-                            )
+                            self.MT.data.append(self.MT.get_empty_row_seq(rn, old_total))
                             if self.MT.all_rows_displayed:
                                 self.MT.insert_row_position("end", height=height)
                             maxidx += 1
                         self.MT.data[rn].insert(idx, v)
         else:
             if idx == "end":
                 for values in reversed(data):
@@ -3012,25 +2684,18 @@
                     for rn, v in enumerate(values):
                         if rn > maxidx:
                             break
                         self.MT.data[rn].insert(idx, v)
         if isinstance(idx, int):
             num_add = len(data)
             self.MT.cell_options = {
-                (rn, cn if cn < idx else cn + num_add): t2
-                for (rn, cn), t2 in self.MT.cell_options.items()
-            }
-            self.MT.col_options = {
-                cn if cn < idx else cn + num_add: t
-                for cn, t in self.MT.col_options.items()
-            }
-            self.CH.cell_options = {
-                cn if cn < idx else cn + num_add: t
-                for cn, t in self.CH.cell_options.items()
+                (rn, cn if cn < idx else cn + num_add): t2 for (rn, cn), t2 in self.MT.cell_options.items()
             }
+            self.MT.col_options = {cn if cn < idx else cn + num_add: t for cn, t in self.MT.col_options.items()}
+            self.CH.cell_options = {cn if cn < idx else cn + num_add: t for cn, t in self.CH.cell_options.items()}
         self.set_refresh_timer(redraw)
 
     def insert_row(
         self,
         values: Union[list, None] = None,
         idx: Union[str, int] = "end",
         height=None,
@@ -3061,18 +2726,15 @@
     ):
         total_cols = None
         datarn = len(self.MT.data) if idx == "end" else idx
         if isinstance(rows, int):
             if rows < 1:
                 raise ValueError(f"rows arg must be greater than 0, not {rows}")
             total_cols = self.MT.total_data_cols()
-            data = [
-                self.MT.get_empty_row_seq(datarn + i, total_cols, r_ops=False)
-                for i in range(rows)
-            ]
+            data = [self.MT.get_empty_row_seq(datarn + i, total_cols, r_ops=False) for i in range(rows)]
         elif not isinstance(rows, list):
             data = list(rows)
         else:
             data = rows
         try:
             data = [r if isinstance(r, list) else list(r) for r in data]
         except Exception as msg:
@@ -3081,35 +2743,28 @@
             if total_cols is None:
                 total_cols = self.MT.total_data_cols()
             data_max_cols = len(max(data, key=len))
             if data_max_cols > total_cols:
                 self.MT.equalize_data_row_lengths(total_columns=data_max_cols)
             elif total_cols > data_max_cols:
                 data[:] = [
-                    data[i]
-                    + self.MT.get_empty_row_seq(
-                        datarn + i, end=total_cols, start=data_max_cols, r_ops=False
-                    )
+                    data[i] + self.MT.get_empty_row_seq(datarn + i, end=total_cols, start=data_max_cols, r_ops=False)
                     for i in range(len(data))
                 ]
             if self.MT.all_columns_displayed:
                 if not self.MT.col_positions:
                     self.MT.col_positions = [0]
                 if data_max_cols > len(self.MT.col_positions) - 1:
-                    self.insert_column_positions(
-                        "end", data_max_cols - (len(self.MT.col_positions) - 1)
-                    )
+                    self.insert_column_positions("end", data_max_cols - (len(self.MT.col_positions) - 1))
         if self.MT.all_rows_displayed and mod_row_positions:
             inspos = idx
         if not self.MT.all_rows_displayed:
             numrows = len(data)
             if idx != "end":
-                self.MT.displayed_rows = [
-                    r if r < idx else r + numrows for r in self.MT.displayed_rows
-                ]
+                self.MT.displayed_rows = [r if r < idx else r + numrows for r in self.MT.displayed_rows]
             if mod_row_positions:
                 inspos = bisect.bisect_left(self.MT.displayed_rows, idx)
                 self.MT.displayed_rows[inspos:inspos] = list(range(idx, idx + numrows))
         if mod_row_positions:
             self.MT.insert_row_positions(
                 idx=inspos,
                 heights=len(data) if heights is None else heights,
@@ -3117,25 +2772,18 @@
             )
         if isinstance(idx, str) and idx.lower() == "end":
             self.MT.data.extend(data)
         else:
             self.MT.data[idx:idx] = data
             num_add = len(data)
             self.MT.cell_options = {
-                (rn if rn < idx else rn + num_add, cn): t2
-                for (rn, cn), t2 in self.MT.cell_options.items()
-            }
-            self.MT.row_options = {
-                rn if rn < idx else rn + num_add: t
-                for rn, t in self.MT.row_options.items()
-            }
-            self.RI.cell_options = {
-                rn if rn < idx else rn + num_add: t
-                for rn, t in self.RI.cell_options.items()
+                (rn if rn < idx else rn + num_add, cn): t2 for (rn, cn), t2 in self.MT.cell_options.items()
             }
+            self.MT.row_options = {rn if rn < idx else rn + num_add: t for rn, t in self.MT.row_options.items()}
+            self.RI.cell_options = {rn if rn < idx else rn + num_add: t for rn, t in self.RI.cell_options.items()}
         self.set_refresh_timer(redraw)
 
     def sheet_data_dimensions(self, total_rows=None, total_columns=None):
         self.MT.data_dimensions(total_rows, total_columns)
 
     def get_total_rows(self, include_index=False):
         return self.MT.total_data_rows(include_index=include_index)
@@ -3156,17 +2804,15 @@
         deselect_all=True,
         **kwargs,
     ):
         if "all_displayed" in kwargs:
             all_rows_displayed = kwargs["all_displayed"]
         res = self.MT.display_rows(
             rows=None if isinstance(rows, str) and rows.lower() == "all" else rows,
-            all_rows_displayed=True
-            if isinstance(rows, str) and rows.lower() == "all"
-            else all_rows_displayed,
+            all_rows_displayed=True if isinstance(rows, str) and rows.lower() == "all" else all_rows_displayed,
             reset_row_positions=reset_row_positions,
             deselect_all=deselect_all,
         )
         if refresh or redraw:
             self.set_refresh_timer(redraw if redraw else refresh)
         return res
 
@@ -3179,17 +2825,15 @@
         redraw=False,
         deselect_all=True,
         **kwargs,
     ):
         if "all_displayed" in kwargs:
             all_columns_displayed = kwargs["all_displayed"]
         res = self.MT.display_columns(
-            columns=None
-            if isinstance(columns, str) and columns.lower() == "all"
-            else columns,
+            columns=None if isinstance(columns, str) and columns.lower() == "all" else columns,
             all_columns_displayed=True
             if isinstance(columns, str) and columns.lower() == "all"
             else all_columns_displayed,
             reset_col_positions=reset_col_positions,
             deselect_all=deselect_all,
         )
         if refresh or redraw:
@@ -3236,32 +2880,26 @@
         elif isinstance(columns, set):
             _columns = columns
         else:
             _columns = set(columns)
         if not _columns:
             return
         if self.MT.all_columns_displayed:
-            _columns = [
-                c for c in range(self.MT.total_data_cols()) if c not in _columns
-            ]
+            _columns = [c for c in range(self.MT.total_data_cols()) if c not in _columns]
         else:
-            _columns = [
-                e for c, e in enumerate(self.MT.displayed_columns) if c not in _columns
-            ]
+            _columns = [e for c, e in enumerate(self.MT.displayed_columns) if c not in _columns]
         self.display_columns(
             columns=_columns,
             all_columns_displayed=False,
             redraw=redraw,
             deselect_all=deselect_all,
         )
 
     def show_ctrl_outline(self, canvas="table", start_cell=(0, 0), end_cell=(1, 1)):
-        self.MT.show_ctrl_outline(
-            canvas=canvas, start_cell=start_cell, end_cell=end_cell
-        )
+        self.MT.show_ctrl_outline(canvas=canvas, start_cell=start_cell, end_cell=end_cell)
 
     def get_ctrl_x_c_boxes(self):
         return self.MT.get_ctrl_x_c_boxes()
 
     def get_selected_min_max(
         self,
     ):  # returns (min_y, min_x, max_y, max_x) of any selections including rows/columns
@@ -3301,37 +2939,28 @@
             redraw=False,
         )
 
     def reset_undos(self):
         self.MT.undo_storage = deque(maxlen=self.MT.max_undos)
 
     def redraw(self, redraw_header=True, redraw_row_index=True):
-        self.MT.main_table_redraw_grid_and_text(
-            redraw_header=redraw_header, redraw_row_index=redraw_row_index
-        )
+        self.MT.main_table_redraw_grid_and_text(redraw_header=redraw_header, redraw_row_index=redraw_row_index)
 
     def refresh(self, redraw_header=True, redraw_row_index=True):
-        self.MT.main_table_redraw_grid_and_text(
-            redraw_header=redraw_header, redraw_row_index=redraw_row_index
-        )
+        self.MT.main_table_redraw_grid_and_text(redraw_header=redraw_header, redraw_row_index=redraw_row_index)
 
     def create_checkbox(self, r=0, c=0, *args, **kwargs):
         _kwargs = get_checkbox_kwargs(*args, **kwargs)
         if isinstance(r, str) and r.lower() == "all" and isinstance(c, int):
             for r_ in range(self.MT.total_data_rows()):
                 self.MT.create_checkbox(datarn=r_, datacn=c, **_kwargs)
         elif isinstance(c, str) and c.lower() == "all" and isinstance(r, int):
             for c_ in range(self.MT.total_data_cols()):
                 self.MT.create_checkbox(datarn=r, datacn=c_, **_kwargs)
-        elif (
-            isinstance(r, str)
-            and r.lower() == "all"
-            and isinstance(c, str)
-            and c.lower() == "all"
-        ):
+        elif isinstance(r, str) and r.lower() == "all" and isinstance(c, str) and c.lower() == "all":
             totalcols = self.MT.total_data_cols()
             for r_ in range(self.MT.total_data_rows()):
                 for c_ in range(totalcols):
                     self.MT.create_checkbox(datarn=r_, datacn=c_, **_kwargs)
         elif isinstance(r, int) and isinstance(c, int):
             self.MT.create_checkbox(datarn=r, datacn=c, **_kwargs)
         self.set_refresh_timer(_kwargs["redraw"])
@@ -3399,20 +3028,15 @@
             for r_, c_ in self.MT.cell_options:
                 if "checkbox" in self.MT.cell_options[(r_, c)]:
                     self.MT.delete_cell_options_checkbox(r_, c)
         elif isinstance(c, str) and c.lower() == "all" and isinstance(r, int):
             for r_, c_ in self.MT.cell_options:
                 if "checkbox" in self.MT.cell_options[(r, c_)]:
                     self.MT.delete_cell_options_checkbox(r, c_)
-        elif (
-            isinstance(r, str)
-            and r.lower() == "all"
-            and isinstance(c, str)
-            and c.lower() == "all"
-        ):
+        elif isinstance(r, str) and r.lower() == "all" and isinstance(c, str) and c.lower() == "all":
             for r_, c_ in self.MT.cell_options:
                 if "checkbox" in self.MT.cell_options[(r_, c_)]:
                     self.MT.delete_cell_options_checkbox(r_, c_)
         elif isinstance(r, int) and isinstance(c, int):
             self.MT.delete_cell_options_checkbox(r, c)
 
     def delete_cell_checkbox(self, r=0, c=0):
@@ -3492,46 +3116,30 @@
                 else:
                     self.MT._row_index[r] = bool(checked)
             else:
                 self.MT._row_index[r] = not self.MT._row_index[r]
 
     def get_checkboxes(self):
         d = {
-            **{
-                k: v["checkbox"]
-                for k, v in self.MT.cell_options.items()
-                if "checkbox" in v
-            },
-            **{
-                k: v["checkbox"]
-                for k, v in self.MT.row_options.items()
-                if "checkbox" in v
-            },
-            **{
-                k: v["checkbox"]
-                for k, v in self.MT.col_options.items()
-                if "checkbox" in v
-            },
+            **{k: v["checkbox"] for k, v in self.MT.cell_options.items() if "checkbox" in v},
+            **{k: v["checkbox"] for k, v in self.MT.row_options.items() if "checkbox" in v},
+            **{k: v["checkbox"] for k, v in self.MT.col_options.items() if "checkbox" in v},
         }
         if "checkbox" in self.MT.options:
             return {**d, "checkbox": self.MT.options["checkbox"]}
         return d
 
     def get_header_checkboxes(self):
-        d = {
-            k: v["checkbox"] for k, v in self.CH.cell_options.items() if "checkbox" in v
-        }
+        d = {k: v["checkbox"] for k, v in self.CH.cell_options.items() if "checkbox" in v}
         if "checkbox" in self.CH.options:
             return {**d, "checkbox": self.CH.options["checkbox"]}
         return d
 
     def get_index_checkboxes(self):
-        d = {
-            k: v["checkbox"] for k, v in self.RI.cell_options.items() if "checkbox" in v
-        }
+        d = {k: v["checkbox"] for k, v in self.RI.cell_options.items() if "checkbox" in v}
         if "checkbox" in self.RI.options:
             return {**d, "checkbox": self.RI.options["checkbox"]}
         return d
 
     def checkbox(self, r, c, checked=None, state=None, check_function="", text=None):
         if type(checked) == bool:
             self.set_cell_data(r, c, checked)
@@ -3540,17 +3148,15 @@
             kwargs["check_function"] = check_function
         if state and state.lower() in ("normal", "disabled"):
             kwargs["state"] = state
         if text is not None:
             kwargs["text"] = text
         return {**kwargs, "checked": self.MT.data[r][c]}
 
-    def header_checkbox(
-        self, c, checked=None, state=None, check_function="", text=None
-    ):
+    def header_checkbox(self, c, checked=None, state=None, check_function="", text=None):
         if type(checked) == bool:
             self.headers(newheaders=checked, index=c)
         kwargs = self.CH.get_cell_kwargs(c, key="checkbox")
         if kwargs:
             if check_function != "":
                 kwargs["check_function"] = check_function
             if state and state.lower() in ("normal", "disabled"):
@@ -3576,20 +3182,15 @@
         _kwargs = get_dropdown_kwargs(*args, **kwargs)
         if isinstance(r, str) and r.lower() == "all" and isinstance(c, int):
             for r_ in range(self.MT.total_data_rows()):
                 self.MT.create_dropdown(datarn=r_, datacn=c, **_kwargs)
         elif isinstance(c, str) and c.lower() == "all" and isinstance(r, int):
             for c_ in range(self.MT.total_data_cols()):
                 self.MT.create_dropdown(datarn=r, datacn=c_, **_kwargs)
-        elif (
-            isinstance(r, str)
-            and r.lower() == "all"
-            and isinstance(c, str)
-            and c.lower() == "all"
-        ):
+        elif isinstance(r, str) and r.lower() == "all" and isinstance(c, str) and c.lower() == "all":
             totalcols = self.MT.total_data_cols()
             for r_ in range(self.MT.total_data_rows()):
                 for c_ in range(totalcols):
                     self.MT.create_dropdown(datarn=r_, datacn=c_, **_kwargs)
         elif isinstance(r, int) and isinstance(c, int):
             self.MT.create_dropdown(datarn=r, datacn=c, **_kwargs)
         self.set_refresh_timer(_kwargs["redraw"])
@@ -3659,20 +3260,15 @@
             for r_, c_ in self.MT.cell_options:
                 if "dropdown" in self.MT.cell_options[(r_, c)]:
                     self.MT.delete_cell_options_dropdown(r_, c)
         elif isinstance(c, str) and c.lower() == "all" and isinstance(r, int):
             for r_, c_ in self.MT.cell_options:
                 if "dropdown" in self.MT.cell_options[(r, c_)]:
                     self.MT.delete_cell_options_dropdown(r, c_)
-        elif (
-            isinstance(r, str)
-            and r.lower() == "all"
-            and isinstance(c, str)
-            and c.lower() == "all"
-        ):
+        elif isinstance(r, str) and r.lower() == "all" and isinstance(c, str) and c.lower() == "all":
             for r_, c_ in self.MT.cell_options:
                 if "dropdown" in self.MT.cell_options[(r_, c_)]:
                     self.MT.delete_cell_options_dropdown(r_, c_)
         elif isinstance(r, int) and isinstance(c, int):
             self.MT.delete_cell_options_dropdown(r, c)
 
     def delete_cell_dropdown(self, r=0, c=0):
@@ -3727,53 +3323,35 @@
             for r_ in r:
                 self.RI.delete_cell_options_dropdown(r_)
         elif r is None:
             self.RI.delete_options_dropdown()
 
     def get_dropdowns(self):
         d = {
-            **{
-                k: v["dropdown"]
-                for k, v in self.MT.cell_options.items()
-                if "dropdown" in v
-            },
-            **{
-                k: v["dropdown"]
-                for k, v in self.MT.row_options.items()
-                if "dropdown" in v
-            },
-            **{
-                k: v["dropdown"]
-                for k, v in self.MT.col_options.items()
-                if "dropdown" in v
-            },
+            **{k: v["dropdown"] for k, v in self.MT.cell_options.items() if "dropdown" in v},
+            **{k: v["dropdown"] for k, v in self.MT.row_options.items() if "dropdown" in v},
+            **{k: v["dropdown"] for k, v in self.MT.col_options.items() if "dropdown" in v},
         }
         if "dropdown" in self.MT.options:
             return {**d, "dropdown": self.MT.options["dropdown"]}
         return d
 
     def get_header_dropdowns(self):
-        d = {
-            k: v["dropdown"] for k, v in self.CH.cell_options.items() if "dropdown" in v
-        }
+        d = {k: v["dropdown"] for k, v in self.CH.cell_options.items() if "dropdown" in v}
         if "dropdown" in self.CH.options:
             return {**d, "dropdown": self.CH.options["dropdown"]}
         return d
 
     def get_index_dropdowns(self):
-        d = {
-            k: v["dropdown"] for k, v in self.RI.cell_options.items() if "dropdown" in v
-        }
+        d = {k: v["dropdown"] for k, v in self.RI.cell_options.items() if "dropdown" in v}
         if "dropdown" in self.RI.options:
             return {**d, "dropdown": self.RI.options["dropdown"]}
         return d
 
-    def set_dropdown_values(
-        self, r=0, c=0, set_existing_dropdown=False, values=[], set_value=None
-    ):
+    def set_dropdown_values(self, r=0, c=0, set_existing_dropdown=False, values=[], set_value=None):
         if set_existing_dropdown:
             if self.MT.existing_dropdown_window is not None:
                 r_ = self.MT.existing_dropdown_window.r
                 c_ = self.MT.existing_dropdown_window.c
             else:
                 raise Exception("No dropdown box is currently open")
         else:
@@ -3788,17 +3366,15 @@
             if (
                 kwargs["window"] != "no dropdown open"
                 and self.MT.text_editor_loc is not None
                 and self.MT.text_editor is not None
             ):
                 self.MT.text_editor.set_text(set_value)
 
-    def set_header_dropdown_values(
-        self, c=0, set_existing_dropdown=False, values=[], set_value=None
-    ):
+    def set_header_dropdown_values(self, c=0, set_existing_dropdown=False, values=[], set_value=None):
         if set_existing_dropdown:
             if self.CH.existing_dropdown_window is not None:
                 c_ = self.CH.existing_dropdown_window.c
             else:
                 raise Exception("No dropdown box is currently open")
         else:
             c_ = c
@@ -3806,17 +3382,15 @@
         if kwargs:
             kwargs["values"] = values
             if kwargs["window"] != "no dropdown open":
                 kwargs["window"].values(values)
             if set_value is not None:
                 self.MT.headers(newheaders=set_value, index=c_)
 
-    def set_index_dropdown_values(
-        self, r, set_existing_dropdown=False, values=[], set_value=None
-    ):
+    def set_index_dropdown_values(self, r, set_existing_dropdown=False, values=[], set_value=None):
         if set_existing_dropdown:
             if self.RI.existing_dropdown_window is not None:
                 r_ = self.RI.existing_dropdown_window.r
             else:
                 raise Exception("No dropdown box is currently open")
         else:
             r_ = r
@@ -3923,20 +3497,15 @@
         elif isinstance(c, str) and c.lower() == "all" and isinstance(r, int):
             for c_ in range(self.MT.total_data_cols()):
                 self.MT.format_cell(
                     datarn=r,
                     datacn=c_,
                     **{"formatter": formatter_class, **formatter_options, **kwargs},
                 )
-        elif (
-            isinstance(r, str)
-            and r.lower() == "all"
-            and isinstance(c, str)
-            and c.lower() == "all"
-        ):
+        elif isinstance(r, str) and r.lower() == "all" and isinstance(c, str) and c.lower() == "all":
             for r_ in range(self.MT.total_data_rows()):
                 for c_ in range(self.MT.total_data_cols()):
                     self.MT.format_cell(
                         datarn=r_,
                         datacn=c_,
                         **{"formatter": formatter_class, **formatter_options, **kwargs},
                     )
@@ -3958,20 +3527,15 @@
             for r_, c_ in self.MT.cell_options:
                 if "format" in self.MT.cell_options[(r_, c)]:
                     self.MT.delete_cell_format(r_, c, clear_values=clear_values)
         elif isinstance(c, str) and c.lower() == "all" and isinstance(r, int):
             for r_, c_ in self.MT.cell_options:
                 if "format" in self.MT.cell_options[(r, c_)]:
                     self.MT.delete_cell_format(r, c_, clear_values=clear_values)
-        elif (
-            isinstance(r, str)
-            and r.lower() == "all"
-            and isinstance(c, str)
-            and c.lower() == "all"
-        ):
+        elif isinstance(r, str) and r.lower() == "all" and isinstance(c, str) and c.lower() == "all":
             for r_, c_ in self.MT.cell_options:
                 if "format" in self.MT.cell_options[(r_, c_)]:
                     self.MT.delete_cell_format(r_, c_, clear_values=clear_values)
         else:
             self.MT.delete_cell_format(r, c, clear_values=clear_values)
 
     def format_row(
@@ -3980,26 +3544,20 @@
         formatter_options={},
         formatter_class=None,
         redraw=True,
         **kwargs,
     ):
         if isinstance(r, str) and r.lower() == "all":
             for r_ in range(len(self.MT.data)):
-                self.MT.format_column(
-                    r_, **{"formatter": formatter_class, **formatter_options, **kwargs}
-                )
+                self.MT.format_column(r_, **{"formatter": formatter_class, **formatter_options, **kwargs})
         elif is_iterable(r):
             for r_ in r:
-                self.MT.format_row(
-                    r_, **{"formatter": formatter_class, **formatter_options, **kwargs}
-                )
+                self.MT.format_row(r_, **{"formatter": formatter_class, **formatter_options, **kwargs})
         else:
-            self.MT.format_row(
-                r, **{"formatter": formatter_class, **formatter_options, **kwargs}
-            )
+            self.MT.format_row(r, **{"formatter": formatter_class, **formatter_options, **kwargs})
         self.set_refresh_timer(redraw)
 
     def delete_row_format(self, r="all", clear_values=False):
         if is_iterable(r):
             for r_ in r:
                 self.MT.delete_row_format(r_, clear_values=clear_values)
         else:
@@ -4011,41 +3569,31 @@
         formatter_options={},
         formatter_class=None,
         redraw=True,
         **kwargs,
     ):
         if isinstance(c, str) and c.lower() == "all":
             for c_ in range(self.MT.total_data_cols()):
-                self.MT.format_column(
-                    c_, **{"formatter": formatter_class, **formatter_options, **kwargs}
-                )
+                self.MT.format_column(c_, **{"formatter": formatter_class, **formatter_options, **kwargs})
         elif is_iterable(c):
             for c_ in c:
-                self.MT.format_column(
-                    c_, **{"formatter": formatter_class, **formatter_options, **kwargs}
-                )
+                self.MT.format_column(c_, **{"formatter": formatter_class, **formatter_options, **kwargs})
         else:
-            self.MT.format_column(
-                c, **{"formatter": formatter_class, **formatter_options, **kwargs}
-            )
+            self.MT.format_column(c, **{"formatter": formatter_class, **formatter_options, **kwargs})
         self.set_refresh_timer(redraw)
 
     def delete_column_format(self, c="all", clear_values=False):
         if is_iterable(c):
             for c_ in c:
                 self.MT.delete_column_format(c_, clear_values=clear_values)
         else:
             self.MT.delete_column_format(c, clear_values=clear_values)
 
-    def format_sheet(
-        self, formatter_options={}, formatter_class=None, redraw=True, **kwargs
-    ):
-        self.MT.format_sheet(
-            **{"formatter": formatter_class, **formatter_options, **kwargs}
-        )
+    def format_sheet(self, formatter_options={}, formatter_class=None, redraw=True, **kwargs):
+        self.MT.format_sheet(**{"formatter": formatter_class, **formatter_options, **kwargs})
         self.set_refresh_timer(redraw)
 
     def delete_sheet_format(self, clear_values=False):
         self.MT.delete_sheet_format(clear_values=clear_values)
 
 
 class Sheet_Dropdown(Sheet):
@@ -4144,17 +3692,15 @@
         self.see(self.row, 0, redraw=False)
         self.select_row(self.row)
 
     def search_and_see(self, event=None):
         if self.modified_function is not None:
             self.modified_function(event)
         if self.search_function is not None:
-            rn = self.search_function(
-                search_for=rf"{event.value}".lower(), data=self.MT.data
-            )
+            rn = self.search_function(search_for=rf"{event.value}".lower(), data=self.MT.data)
             if rn is not None:
                 self.row = rn
                 self.deselect("all")
                 self.see(self.row, 0, redraw=False)
                 self.select_row(self.row)
 
     def mouse_motion(self, event=None):
@@ -4177,17 +3723,15 @@
                 row = None
             else:
                 row = next(iter(row))
         else:
             row = self.identify_row(event, exclude_index=True, allow_end=False)
         if self.single_index:
             if row is None:
-                self.close_dropdown_window(
-                    self.r if self.single_index == "r" else self.c
-                )
+                self.close_dropdown_window(self.r if self.single_index == "r" else self.c)
             else:
                 self.close_dropdown_window(
                     self.r if self.single_index == "r" else self.c,
                     self.get_cell_data(row, 0),
                 )
         else:
             if row is None:
```

### Comparing `tksheet-6.1.3/tksheet/_tksheet_column_headers.py` & `tksheet-6.1.4/tksheet/_tksheet_column_headers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,53 @@
 import pickle
 import tkinter as tk
 import zlib
 from collections import defaultdict
 from itertools import accumulate, chain, cycle, islice
 from math import ceil, floor
 
-from ._tksheet_formatters import *
-from ._tksheet_other_classes import *
-from ._tksheet_vars import *
+from ._tksheet_formatters import (
+    is_bool_like,
+    try_to_bool,
+)
+from ._tksheet_other_classes import (
+    BeginDragDropEvent,
+    DraggedRowColumn,
+    DrawnItem,
+    DropDownModifiedEvent,
+    EditHeaderEvent,
+    EndDragDropEvent,
+    ResizeEvent,
+    SelectColumnEvent,
+    SelectionBoxEvent,
+    TextCfg,
+    TextEditor,
+    get_checkbox_dict,
+    get_dropdown_dict,
+    get_n2a,
+    get_seq_without_gaps_at_index,
+)
+from ._tksheet_vars import (
+    USER_OS,
+    Color_Map_,
+    rc_binding,
+    symbols_set,
+)
 
 
 class ColumnHeaders(tk.Canvas):
     def __init__(self, *args, **kwargs):
         tk.Canvas.__init__(
             self,
             kwargs["parentframe"],
             background=kwargs["header_bg"],
             highlightthickness=0,
         )
         self.parentframe = kwargs["parentframe"]
-        self.current_height = (
-            None  # is set from within MainTable() __init__ or from Sheet parameters
-        )
+        self.current_height = None  # is set from within MainTable() __init__ or from Sheet parameters
         self.MT = None  # is set from within MainTable() __init__
         self.RI = None  # is set from within MainTable() __init__
         self.TL = None  # is set from within TopLeftRectangle() __init__
         self.extra_begin_edit_cell_func = None
         self.extra_end_edit_cell_func = None
         self.text_editor = None
         self.text_editor_id = None
@@ -95,17 +117,15 @@
         self.header_fg = kwargs["header_fg"]
         self.header_grid_fg = kwargs["header_grid_fg"]
         self.header_border_fg = kwargs["header_border_fg"]
         self.header_selected_cells_bg = kwargs["header_selected_cells_bg"]
         self.header_selected_cells_fg = kwargs["header_selected_cells_fg"]
         self.header_selected_columns_bg = kwargs["header_selected_columns_bg"]
         self.header_selected_columns_fg = kwargs["header_selected_columns_fg"]
-        self.header_hidden_columns_expander_bg = kwargs[
-            "header_hidden_columns_expander_bg"
-        ]
+        self.header_hidden_columns_expander_bg = kwargs["header_hidden_columns_expander_bg"]
         self.show_default_header_for_empty = kwargs["show_default_header_for_empty"]
         self.drag_and_drop_bg = kwargs["drag_and_drop_bg"]
         self.resizing_line_fg = kwargs["resizing_line_fg"]
         self.align = kwargs["header_align"]
         self.basic_bindings()
 
     def basic_bindings(self, enable=True):
@@ -128,48 +148,42 @@
 
     def mousewheel(self, event=None):
         maxlines = 0
         if isinstance(self.MT._headers, int):
             if len(self.MT.data) > self.MT._headers:
                 maxlines = max(
                     len(
-                        self.MT.get_valid_cell_data_as_str(
-                            self.MT._headers, datacn, get_displayed=True
-                        )
+                        self.MT.get_valid_cell_data_as_str(self.MT._headers, datacn, get_displayed=True)
                         .rstrip()
                         .split("\n")
                     )
                     for datacn in range(len(self.MT.data[self.MT._headers]))
                 )
         elif isinstance(self.MT._headers, (list, tuple)):
             maxlines = max(
-                len(e.rstrip().split("\n"))
-                if isinstance(e, str)
-                else len(f"{e}".rstrip().split("\n"))
+                len(e.rstrip().split("\n")) if isinstance(e, str) else len(f"{e}".rstrip().split("\n"))
                 for e in self.MT._headers
             )
         if maxlines == 1:
             maxlines = 0
         if self.lines_start_at > maxlines:
             self.lines_start_at = maxlines
         if (event.delta < 0 or event.num == 5) and self.lines_start_at < maxlines:
             self.lines_start_at += 1
         elif (event.delta >= 0 or event.num == 4) and self.lines_start_at > 0:
             self.lines_start_at -= 1
-        self.MT.main_table_redraw_grid_and_text(
-            redraw_header=True, redraw_row_index=False, redraw_table=False
-        )
+        self.MT.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=False, redraw_table=False)
 
     def set_height(self, new_height, set_TL=False):
         self.current_height = new_height
         try:
             self.config(height=new_height)
         except Exception:
             return
-        if set_TL:
+        if set_TL and self.TL is not None:
             self.TL.set_dimensions(new_h=new_height)
 
     def enable_bindings(self, binding):
         if binding == "column_width_resize":
             self.width_resizing_enabled = True
         if binding == "column_height_resize":
             self.height_resizing_enabled = True
@@ -205,19 +219,15 @@
         self.mouseclick_outside_editor_or_dropdown_all_canvases()
         self.focus_set()
         popup_menu = None
         if self.MT.identify_col(x=event.x, allow_end=False) is None:
             self.MT.deselect("all")
             if self.MT.rc_popup_menus_enabled:
                 popup_menu = self.MT.empty_rc_popup_menu
-        elif (
-            self.col_selection_enabled
-            and not self.currently_resizing_width
-            and not self.currently_resizing_height
-        ):
+        elif self.col_selection_enabled and not self.currently_resizing_width and not self.currently_resizing_height:
             c = self.MT.identify_col(x=event.x)
             if c < len(self.MT.col_positions) - 1:
                 if self.MT.col_selected(c):
                     if self.MT.rc_popup_menus_enabled:
                         popup_menu = self.ch_rc_popup_menu
                 else:
                     if self.MT.single_selection_enabled and self.MT.rc_select_enabled:
@@ -240,27 +250,21 @@
             and self.rsz_w is None
         ):
             c = self.MT.identify_col(x=event.x)
             if c < len(self.MT.col_positions) - 1:
                 c_selected = self.MT.col_selected(c)
                 if not c_selected and self.col_selection_enabled:
                     self.add_selection(c, set_as_current=True)
-                    self.MT.main_table_redraw_grid_and_text(
-                        redraw_header=True, redraw_row_index=True
-                    )
+                    self.MT.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=True)
                     if self.ctrl_selection_binding_func is not None:
-                        self.ctrl_selection_binding_func(
-                            SelectionBoxEvent("ctrl_select_columns", (c, c + 1))
-                        )
+                        self.ctrl_selection_binding_func(SelectionBoxEvent("ctrl_select_columns", (c, c + 1)))
                 elif c_selected:
                     self.dragged_col = DraggedRowColumn(
                         dragged=c,
-                        to_move=get_seq_without_gaps_at_index(
-                            sorted(self.MT.get_selected_cols()), c
-                        ),
+                        to_move=get_seq_without_gaps_at_index(sorted(self.MT.get_selected_cols()), c),
                     )
         elif not self.MT.ctrl_select_enabled:
             self.b1_press(event)
 
     def ctrl_shift_b1_press(self, event):
         self.mouseclick_outside_editor_or_dropdown_all_canvases()
         x = event.x
@@ -294,40 +298,30 @@
                                 min_c + 1,
                                 "columns",
                             )
                             func_event = tuple(range(c, min_c + 1))
                     else:
                         self.add_selection(c, set_as_current=True)
                         func_event = (c,)
-                    self.MT.main_table_redraw_grid_and_text(
-                        redraw_header=True, redraw_row_index=True
-                    )
+                    self.MT.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=True)
                     if self.ctrl_selection_binding_func is not None:
-                        self.ctrl_selection_binding_func(
-                            SelectionBoxEvent("ctrl_select_columns", func_event)
-                        )
+                        self.ctrl_selection_binding_func(SelectionBoxEvent("ctrl_select_columns", func_event))
                 elif c_selected:
                     self.dragged_col = DraggedRowColumn(
                         dragged=c,
-                        to_move=get_seq_without_gaps_at_index(
-                            sorted(self.MT.get_selected_cols()), c
-                        ),
+                        to_move=get_seq_without_gaps_at_index(sorted(self.MT.get_selected_cols()), c),
                     )
         elif not self.MT.ctrl_select_enabled:
             self.shift_b1_press(event)
 
     def shift_b1_press(self, event):
         self.mouseclick_outside_editor_or_dropdown_all_canvases()
         x = event.x
         c = self.MT.identify_col(x=x)
-        if (
-            (self.drag_and_drop_enabled or self.col_selection_enabled)
-            and self.rsz_h is None
-            and self.rsz_w is None
-        ):
+        if (self.drag_and_drop_enabled or self.col_selection_enabled) and self.rsz_h is None and self.rsz_w is None:
             if c < len(self.MT.col_positions) - 1:
                 c_selected = self.MT.col_selected(c)
                 if not c_selected and self.col_selection_enabled:
                     currently_selected = self.MT.currently_selected()
                     if currently_selected and currently_selected.type_ == "column":
                         min_c = int(currently_selected[1])
                         self.MT.delete_selection_rects(delete_current=False)
@@ -348,27 +342,21 @@
                                 min_c + 1,
                                 "columns",
                             )
                             func_event = tuple(range(c, min_c + 1))
                     else:
                         self.select_col(c)
                         func_event = (c,)
-                    self.MT.main_table_redraw_grid_and_text(
-                        redraw_header=True, redraw_row_index=True
-                    )
+                    self.MT.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=True)
                     if self.shift_selection_binding_func is not None:
-                        self.shift_selection_binding_func(
-                            SelectionBoxEvent("shift_select_columns", func_event)
-                        )
+                        self.shift_selection_binding_func(SelectionBoxEvent("shift_select_columns", func_event))
                 elif c_selected:
                     self.dragged_col = DraggedRowColumn(
                         dragged=c,
-                        to_move=get_seq_without_gaps_at_index(
-                            sorted(self.MT.get_selected_cols()), c
-                        ),
+                        to_move=get_seq_without_gaps_at_index(sorted(self.MT.get_selected_cols()), c),
                     )
 
     def create_resize_line(self, x1, y1, x2, y2, width, fill, tag):
         if self.hidd_resize_lines:
             t, sh = self.hidd_resize_lines.popitem()
             self.coords(t, x1, y1, x2, y2)
             if sh:
@@ -432,36 +420,27 @@
         if (
             self.double_click_resizing_enabled
             and self.width_resizing_enabled
             and self.rsz_w is not None
             and not self.currently_resizing_width
         ):
             col = self.rsz_w - 1
-            old_width = (
-                self.MT.col_positions[self.rsz_w]
-                - self.MT.col_positions[self.rsz_w - 1]
-            )
+            old_width = self.MT.col_positions[self.rsz_w] - self.MT.col_positions[self.rsz_w - 1]
             new_width = self.set_col_width(col)
-            self.MT.main_table_redraw_grid_and_text(
-                redraw_header=True, redraw_row_index=True
-            )
+            self.MT.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=True)
             if self.column_width_resize_func is not None and old_width != new_width:
-                self.column_width_resize_func(
-                    ResizeEvent("column_width_resize", col, old_width, new_width)
-                )
+                self.column_width_resize_func(ResizeEvent("column_width_resize", col, old_width, new_width))
         elif self.col_selection_enabled and self.rsz_h is None and self.rsz_w is None:
             c = self.MT.identify_col(x=event.x)
             if c < len(self.MT.col_positions) - 1:
                 if self.MT.single_selection_enabled:
                     self.select_col(c, redraw=True)
                 elif self.MT.toggle_selection_enabled:
                     self.toggle_select_col(c, redraw=True)
-                datacn = (
-                    c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
-                )
+                datacn = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
                 if (
                     self.get_cell_kwargs(datacn, key="dropdown")
                     or self.get_cell_kwargs(datacn, key="checkbox")
                     or self.edit_cell_enabled
                 ):
                     self.open_cell(event)
         self.rsz_w = None
@@ -489,60 +468,46 @@
                 0,
                 x,
                 self.current_height,
                 width=1,
                 fill=self.resizing_line_fg,
                 tag="rwl",
             )
-            self.MT.create_resize_line(
-                x, y1, x, y2, width=1, fill=self.resizing_line_fg, tag="rwl"
-            )
+            self.MT.create_resize_line(x, y1, x, y2, width=1, fill=self.resizing_line_fg, tag="rwl")
             self.create_resize_line(
                 line2x,
                 0,
                 line2x,
                 self.current_height,
                 width=1,
                 fill=self.resizing_line_fg,
                 tag="rwl2",
             )
-            self.MT.create_resize_line(
-                line2x, y1, line2x, y2, width=1, fill=self.resizing_line_fg, tag="rwl2"
-            )
-        elif (
-            self.height_resizing_enabled
-            and self.rsz_w is None
-            and self.rsz_h is not None
-        ):
+            self.MT.create_resize_line(line2x, y1, line2x, y2, width=1, fill=self.resizing_line_fg, tag="rwl2")
+        elif self.height_resizing_enabled and self.rsz_w is None and self.rsz_h is not None:
             x1, y1, x2, y2 = self.MT.get_canvas_visible_area()
             self.currently_resizing_height = True
             y = event.y
             if y < self.MT.min_header_height:
                 y = int(self.MT.min_header_height)
             self.new_col_height = y
-            self.create_resize_line(
-                x1, y, x2, y, width=1, fill=self.resizing_line_fg, tag="rhl"
-            )
+            self.create_resize_line(x1, y, x2, y, width=1, fill=self.resizing_line_fg, tag="rhl")
         elif self.MT.identify_col(x=event.x, allow_end=False) is None:
             self.MT.deselect("all")
         elif self.col_selection_enabled and self.rsz_w is None and self.rsz_h is None:
             if c < len(self.MT.col_positions) - 1:
-                datacn = (
-                    c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
-                )
+                datacn = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
                 if (
                     self.MT.col_selected(c)
                     and not self.event_over_dropdown(c, datacn, event, x)
                     and not self.event_over_checkbox(c, datacn, event, x)
                 ):
                     self.dragged_col = DraggedRowColumn(
                         dragged=c,
-                        to_move=get_seq_without_gaps_at_index(
-                            sorted(self.MT.get_selected_cols()), c
-                        ),
+                        to_move=get_seq_without_gaps_at_index(sorted(self.MT.get_selected_cols()), c),
                     )
                 else:
                     self.being_drawn_rect = (
                         0,
                         c,
                         len(self.MT.row_positions) - 1,
                         c + 1,
@@ -553,36 +518,30 @@
                     elif self.MT.toggle_selection_enabled:
                         self.toggle_select_col(c, redraw=True)
         if self.extra_b1_press_func is not None:
             self.extra_b1_press_func(event)
 
     def b1_motion(self, event):
         x1, y1, x2, y2 = self.MT.get_canvas_visible_area()
-        if (
-            self.width_resizing_enabled
-            and self.rsz_w is not None
-            and self.currently_resizing_width
-        ):
+        if self.width_resizing_enabled and self.rsz_w is not None and self.currently_resizing_width:
             x = self.canvasx(event.x)
             size = x - self.MT.col_positions[self.rsz_w - 1]
             if size >= self.MT.min_column_width and size < self.MT.max_column_width:
                 self.delete_all_resize_and_ctrl_lines(ctrl_lines=False)
                 line2x = self.MT.col_positions[self.rsz_w - 1]
                 self.create_resize_line(
                     x,
                     0,
                     x,
                     self.current_height,
                     width=1,
                     fill=self.resizing_line_fg,
                     tag="rwl",
                 )
-                self.MT.create_resize_line(
-                    x, y1, x, y2, width=1, fill=self.resizing_line_fg, tag="rwl"
-                )
+                self.MT.create_resize_line(x, y1, x, y2, width=1, fill=self.resizing_line_fg, tag="rwl")
                 self.create_resize_line(
                     line2x,
                     0,
                     line2x,
                     self.current_height,
                     width=1,
                     fill=self.resizing_line_fg,
@@ -593,38 +552,30 @@
                     y1,
                     line2x,
                     y2,
                     width=1,
                     fill=self.resizing_line_fg,
                     tag="rwl2",
                 )
-        elif (
-            self.height_resizing_enabled
-            and self.rsz_h is not None
-            and self.currently_resizing_height
-        ):
+        elif self.height_resizing_enabled and self.rsz_h is not None and self.currently_resizing_height:
             evy = event.y
             self.delete_all_resize_and_ctrl_lines(ctrl_lines=False)
             if evy > self.current_height:
                 y = self.MT.canvasy(evy - self.current_height)
                 if evy > self.MT.max_header_height:
                     evy = int(self.MT.max_header_height)
                     y = self.MT.canvasy(evy - self.current_height)
                 self.new_col_height = evy
-                self.MT.create_resize_line(
-                    x1, y, x2, y, width=1, fill=self.resizing_line_fg, tag="rhl"
-                )
+                self.MT.create_resize_line(x1, y, x2, y, width=1, fill=self.resizing_line_fg, tag="rhl")
             else:
                 y = evy
                 if y < self.MT.min_header_height:
                     y = int(self.MT.min_header_height)
                 self.new_col_height = y
-                self.create_resize_line(
-                    x1, y, x2, y, width=1, fill=self.resizing_line_fg, tag="rhl"
-                )
+                self.create_resize_line(x1, y, x2, y, width=1, fill=self.resizing_line_fg, tag="rhl")
         elif (
             self.drag_and_drop_enabled
             and self.col_selection_enabled
             and self.MT.anything_selected(exclude_cells=True, exclude_rows=True)
             and self.rsz_h is None
             and self.rsz_w is None
             and self.dragged_col is not None
@@ -635,18 +586,15 @@
                     self.drag_and_drop_motion(event),
                     y1,
                     y2,
                     self.dragged_col.to_move[0],
                     self.dragged_col.to_move[-1],
                 )
         elif (
-            self.MT.drag_selection_enabled
-            and self.col_selection_enabled
-            and self.rsz_h is None
-            and self.rsz_w is None
+            self.MT.drag_selection_enabled and self.col_selection_enabled and self.rsz_h is None and self.rsz_w is None
         ):
             need_redraw = False
             end_col = self.MT.identify_col(x=event.x)
             currently_selected = self.MT.currently_selected()
             if end_col < len(self.MT.col_positions) - 1 and currently_selected:
                 if currently_selected.type_ == "column":
                     start_col = currently_selected[1]
@@ -670,23 +618,19 @@
                         func_event = tuple(range(end_col, start_col + 1))
                     if self.being_drawn_rect != rect:
                         need_redraw = True
                         self.MT.delete_selection_rects(delete_current=False)
                         self.MT.create_selected(*rect)
                         self.being_drawn_rect = rect
                         if self.drag_selection_binding_func is not None:
-                            self.drag_selection_binding_func(
-                                SelectionBoxEvent("drag_select_columns", func_event)
-                            )
+                            self.drag_selection_binding_func(SelectionBoxEvent("drag_select_columns", func_event))
                 if self.scroll_if_event_offscreen(event):
                     need_redraw = True
             if need_redraw:
-                self.MT.main_table_redraw_grid_and_text(
-                    redraw_header=True, redraw_row_index=False
-                )
+                self.MT.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=False)
         if self.extra_b1_motion_func is not None:
             self.extra_b1_motion_func(event)
 
     def ctrl_b1_motion(self, event):
         x1, y1, x2, y2 = self.MT.get_canvas_visible_area()
         if (
             self.drag_and_drop_enabled
@@ -739,23 +683,19 @@
                     if self.being_drawn_rect != rect:
                         need_redraw = True
                         if self.being_drawn_rect is not None:
                             self.MT.delete_selected(*self.being_drawn_rect)
                         self.MT.create_selected(*rect)
                         self.being_drawn_rect = rect
                         if self.drag_selection_binding_func is not None:
-                            self.drag_selection_binding_func(
-                                SelectionBoxEvent("drag_select_columns", func_event)
-                            )
+                            self.drag_selection_binding_func(SelectionBoxEvent("drag_select_columns", func_event))
                 if self.scroll_if_event_offscreen(event):
                     need_redraw = True
             if need_redraw:
-                self.MT.main_table_redraw_grid_and_text(
-                    redraw_header=True, redraw_row_index=False
-                )
+                self.MT.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=False)
         elif not self.MT.ctrl_select_enabled:
             self.b1_motion(event)
 
     def drag_and_drop_motion(self, event):
         x = event.x
         wend = self.winfo_width()
         xcheck = self.xview()
@@ -780,31 +720,33 @@
         col = self.MT.identify_col(x=event.x)
         if col >= self.dragged_col.to_move[0] and col <= self.dragged_col.to_move[-1]:
             xpos = self.MT.col_positions[self.dragged_col.to_move[0]]
         else:
             if col < self.dragged_col.to_move[0]:
                 xpos = self.MT.col_positions[col]
             else:
-                xpos = self.MT.col_positions[col + 1] if len(self.MT.col_positions) - 1 > col else self.MT.col_positions[col]
+                xpos = (
+                    self.MT.col_positions[col + 1]
+                    if len(self.MT.col_positions) - 1 > col
+                    else self.MT.col_positions[col]
+                )
         return xpos
 
     def show_drag_and_drop_indicators(self, xpos, y1, y2, start_col, end_col):
         self.delete_all_resize_and_ctrl_lines()
         self.create_resize_line(
             xpos,
             0,
             xpos,
             self.current_height,
             width=3,
             fill=self.drag_and_drop_bg,
             tag="dd",
         )
-        self.MT.create_resize_line(
-            xpos, y1, xpos, y2, width=3, fill=self.drag_and_drop_bg, tag="dd"
-        )
+        self.MT.create_resize_line(xpos, y1, xpos, y2, width=3, fill=self.drag_and_drop_bg, tag="dd")
         self.MT.show_ctrl_outline(
             start_cell=(start_col, 0),
             end_cell=(end_col + 1, len(self.MT.row_positions) - 1),
             dash=(),
             outline=self.drag_and_drop_bg,
             delete_on_timer=False,
         )
@@ -822,20 +764,15 @@
             try:
                 self.MT.xview_scroll(1, "units")
                 self.xview_scroll(1, "units")
             except Exception:
                 pass
             self.fix_xview()
             need_redraw = True
-        elif (
-            event.x < 0
-            and self.canvasx(self.winfo_width()) > 0
-            and xcheck
-            and xcheck[0] > 0
-        ):
+        elif event.x < 0 and self.canvasx(self.winfo_width()) > 0 and xcheck and xcheck[0] > 0:
             try:
                 self.xview_scroll(-1, "units")
                 self.MT.xview_scroll(-1, "units")
             except Exception:
                 pass
             self.fix_xview()
             need_redraw = True
@@ -870,68 +807,39 @@
     def b1_release(self, event=None):
         if self.being_drawn_rect is not None:
             self.MT.delete_selected(*self.being_drawn_rect)
             to_sel = tuple(self.being_drawn_rect)
             self.being_drawn_rect = None
             self.MT.create_selected(*to_sel)
         self.MT.bind("<MouseWheel>", self.MT.mousewheel)
-        if (
-            self.width_resizing_enabled
-            and self.rsz_w is not None
-            and self.currently_resizing_width
-        ):
+        if self.width_resizing_enabled and self.rsz_w is not None and self.currently_resizing_width:
             self.currently_resizing_width = False
             new_col_pos = int(self.coords("rwl")[0])
             self.delete_all_resize_and_ctrl_lines(ctrl_lines=False)
-            old_width = (
-                self.MT.col_positions[self.rsz_w]
-                - self.MT.col_positions[self.rsz_w - 1]
-            )
+            old_width = self.MT.col_positions[self.rsz_w] - self.MT.col_positions[self.rsz_w - 1]
             size = new_col_pos - self.MT.col_positions[self.rsz_w - 1]
             if size < self.MT.min_column_width:
-                new_col_pos = ceil(
-                    self.MT.col_positions[self.rsz_w - 1] + self.MT.min_column_width
-                )
+                new_col_pos = ceil(self.MT.col_positions[self.rsz_w - 1] + self.MT.min_column_width)
             elif size > self.MT.max_column_width:
-                new_col_pos = floor(
-                    self.MT.col_positions[self.rsz_w - 1] + self.MT.max_column_width
-                )
+                new_col_pos = floor(self.MT.col_positions[self.rsz_w - 1] + self.MT.max_column_width)
             increment = new_col_pos - self.MT.col_positions[self.rsz_w]
             self.MT.col_positions[self.rsz_w + 1 :] = [
-                e + increment
-                for e in islice(
-                    self.MT.col_positions, self.rsz_w + 1, len(self.MT.col_positions)
-                )
+                e + increment for e in islice(self.MT.col_positions, self.rsz_w + 1, len(self.MT.col_positions))
             ]
             self.MT.col_positions[self.rsz_w] = new_col_pos
-            new_width = (
-                self.MT.col_positions[self.rsz_w]
-                - self.MT.col_positions[self.rsz_w - 1]
-            )
+            new_width = self.MT.col_positions[self.rsz_w] - self.MT.col_positions[self.rsz_w - 1]
             self.MT.recreate_all_selection_boxes()
-            self.MT.main_table_redraw_grid_and_text(
-                redraw_header=True, redraw_row_index=True
-            )
+            self.MT.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=True)
             if self.column_width_resize_func is not None and old_width != new_width:
-                self.column_width_resize_func(
-                    ResizeEvent(
-                        "column_width_resize", self.rsz_w - 1, old_width, new_width
-                    )
-                )
-        elif (
-            self.height_resizing_enabled
-            and self.rsz_h is not None
-            and self.currently_resizing_height
-        ):
+                self.column_width_resize_func(ResizeEvent("column_width_resize", self.rsz_w - 1, old_width, new_width))
+        elif self.height_resizing_enabled and self.rsz_h is not None and self.currently_resizing_height:
             self.currently_resizing_height = False
             self.delete_all_resize_and_ctrl_lines(ctrl_lines=False)
             self.set_height(self.new_col_height, set_TL=True)
-            self.MT.main_table_redraw_grid_and_text(
-                redraw_header=True, redraw_row_index=True
-            )
+            self.MT.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=True)
         elif (
             self.drag_and_drop_enabled
             and self.col_selection_enabled
             and self.MT.anything_selected(exclude_cells=True, exclude_rows=True)
             and self.rsz_h is None
             and self.rsz_w is None
             and self.dragged_col is not None
@@ -939,17 +847,15 @@
             self.delete_all_resize_and_ctrl_lines()
             x = event.x
             c = self.MT.identify_col(x=x)
             orig_selected = self.dragged_col.to_move
             if (
                 c != self.dragged_col.dragged
                 and c is not None
-                and (
-                    c < self.dragged_col.to_move[0] or c > self.dragged_col.to_move[-1]
-                )
+                and (c < self.dragged_col.to_move[0] or c > self.dragged_col.to_move[-1])
                 and len(orig_selected) != len(self.MT.col_positions) - 1
             ):
                 rm1start = orig_selected[0]
                 totalcols = len(orig_selected)
                 extra_func_success = True
                 if c >= len(self.MT.col_positions) - 1:
                     c -= 1
@@ -969,50 +875,40 @@
                         c,
                         rm1start,
                         totalcols,
                         move_data=self.column_drag_and_drop_perform,
                     )
                     if self.MT.undo_enabled:
                         self.MT.undo_storage.append(
-                            zlib.compress(
-                                pickle.dumps(("move_cols", orig_selected, new_selected))
-                            )
+                            zlib.compress(pickle.dumps(("move_cols", orig_selected, new_selected)))
                         )
-                    self.MT.main_table_redraw_grid_and_text(
-                        redraw_header=True, redraw_row_index=True
-                    )
+                    self.MT.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=True)
                     if self.ch_extra_end_drag_drop_func is not None:
                         self.ch_extra_end_drag_drop_func(
                             EndDragDropEvent(
                                 "end_column_header_drag_drop",
                                 orig_selected,
                                 new_selected,
                                 int(c),
                             )
                         )
                     self.parentframe.emit_event("<<SheetModified>>")
-        elif (
-            self.b1_pressed_loc is not None
-            and self.rsz_w is None
-            and self.rsz_h is None
-        ):
+        elif self.b1_pressed_loc is not None and self.rsz_w is None and self.rsz_h is None:
             c = self.MT.identify_col(x=event.x)
             if (
                 c is not None
                 and c < len(self.MT.col_positions) - 1
                 and c == self.b1_pressed_loc
                 and self.b1_pressed_loc != self.closed_dropdown
             ):
-                datacn = (
-                    c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
-                )
+                datacn = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
                 canvasx = self.canvasx(event.x)
-                if self.event_over_dropdown(
+                if self.event_over_dropdown(c, datacn, event, canvasx) or self.event_over_checkbox(
                     c, datacn, event, canvasx
-                ) or self.event_over_checkbox(c, datacn, event, canvasx):
+                ):
                     self.open_cell(event)
             else:
                 self.mouseclick_outside_editor_or_dropdown_all_canvases()
             self.b1_pressed_loc = None
             self.closed_dropdown = None
         self.dragged_col = None
         self.currently_resizing_width = False
@@ -1063,48 +959,39 @@
                 self.select_col(column, redraw=redraw)
 
     def select_col(self, c, redraw=False):
         self.MT.delete_selection_rects()
         self.MT.create_selected(0, c, len(self.MT.row_positions) - 1, c + 1, "columns")
         self.MT.set_currently_selected(0, c, type_="column")
         if redraw:
-            self.MT.main_table_redraw_grid_and_text(
-                redraw_header=True, redraw_row_index=True
-            )
+            self.MT.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=True)
         if self.selection_binding_func is not None:
             self.selection_binding_func(SelectColumnEvent("select_column", int(c)))
 
-    def add_selection(
-        self, c, redraw=False, run_binding_func=True, set_as_current=True
-    ):
+    def add_selection(self, c, redraw=False, run_binding_func=True, set_as_current=True):
         if set_as_current:
             self.MT.set_currently_selected(0, c, type_="column")
         self.MT.create_selected(0, c, len(self.MT.row_positions) - 1, c + 1, "columns")
         if redraw:
-            self.MT.main_table_redraw_grid_and_text(
-                redraw_header=True, redraw_row_index=True
-            )
+            self.MT.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=True)
         if self.selection_binding_func is not None and run_binding_func:
             self.selection_binding_func(("select_column", c))
 
     def get_cell_dimensions(self, datacn):
         txt = self.get_valid_cell_data_as_str(datacn, fix=False)
         if txt:
-            self.MT.txt_measure_canvas.itemconfig(
-                self.MT.txt_measure_canvas_text, text=txt, font=self.MT.header_font
-            )
+            self.MT.txt_measure_canvas.itemconfig(self.MT.txt_measure_canvas_text, text=txt, font=self.MT.header_font)
             b = self.MT.txt_measure_canvas.bbox(self.MT.txt_measure_canvas_text)
             w = b[2] - b[0] + 7
             h = b[3] - b[1] + 5
         else:
             w = self.MT.min_column_width
             h = self.MT.min_header_height
         if datacn in self.cell_options and (
-            self.get_cell_kwargs(datacn, key="dropdown")
-            or self.get_cell_kwargs(datacn, key="checkbox")
+            self.get_cell_kwargs(datacn, key="dropdown") or self.get_cell_kwargs(datacn, key="checkbox")
         ):
             return w + self.MT.header_txt_h, h
         return w, h
 
     def set_height_of_header_to_text(self, text=None):
         if (
             text is None
@@ -1142,17 +1029,15 @@
                     elif h > self.MT.max_header_height:
                         h = int(self.MT.max_header_height)
                     if h > new_height:
                         new_height = h
             elif isinstance(self.MT._headers, int):
                 datarn = self.MT._headers
                 for datacn in iterable:
-                    txt = self.MT.get_valid_cell_data_as_str(
-                        datarn, datacn, get_displayed=True
-                    )
+                    txt = self.MT.get_valid_cell_data_as_str(datarn, datacn, get_displayed=True)
                     if txt:
                         qconf(qtxtm, text=txt)
                         b = qbbox(qtxtm)
                         h = b[3] - b[1] + 5
                     else:
                         h = self.MT.default_header_height
                     if h < self.MT.min_header_height:
@@ -1161,17 +1046,15 @@
                         h = int(self.MT.max_header_height)
                     if h > new_height:
                         new_height = h
         space_bot = self.MT.get_space_bot(0)
         if new_height > space_bot:
             new_height = space_bot
         self.set_height(new_height, set_TL=True)
-        self.MT.main_table_redraw_grid_and_text(
-            redraw_header=True, redraw_row_index=True
-        )
+        self.MT.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=True)
         return new_height
 
     def set_col_width(
         self,
         col,
         width=None,
         only_set_if_too_small=False,
@@ -1200,31 +1083,27 @@
             else:
                 if displayed_only:
                     x1, y1, x2, y2 = self.MT.get_canvas_visible_area()
                     start_row, end_row = self.MT.get_visible_rows(y1, y2)
                 else:
                     start_row, end_row = 0, len(self.MT.displayed_rows)
                 iterable = self.MT.displayed_rows[start_row:end_row]
-            datacn = (
-                col if self.MT.all_columns_displayed else self.MT.displayed_columns[col]
-            )
+            datacn = col if self.MT.all_columns_displayed else self.MT.displayed_columns[col]
             # header
             hw, hh_ = self.get_cell_dimensions(datacn)
             # table
             if self.MT.data:
                 for datarn in iterable:
-                    txt = self.MT.get_valid_cell_data_as_str(
-                        datarn, datacn, get_displayed=True
-                    )
+                    txt = self.MT.get_valid_cell_data_as_str(datarn, datacn, get_displayed=True)
                     if txt:
                         qconf(qtxtm, text=txt, font=qfont)
                         b = qbbox(qtxtm)
-                        if self.MT.get_cell_kwargs(
-                            datarn, datacn, key="dropdown"
-                        ) or self.MT.get_cell_kwargs(datarn, datacn, key="checkbox"):
+                        if self.MT.get_cell_kwargs(datarn, datacn, key="dropdown") or self.MT.get_cell_kwargs(
+                            datarn, datacn, key="checkbox"
+                        ):
                             tw = b[2] - b[0] + qtxth + 7
                         else:
                             tw = b[2] - b[0] + 7
                         if tw > w:
                             w = tw
             if w > hw:
                 new_width = w
@@ -1239,27 +1118,22 @@
         if only_set_if_too_small:
             if new_width <= self.MT.col_positions[col + 1] - self.MT.col_positions[col]:
                 return self.MT.col_positions[col + 1] - self.MT.col_positions[col]
         if not return_new_width:
             new_col_pos = self.MT.col_positions[col] + new_width
             increment = new_col_pos - self.MT.col_positions[col + 1]
             self.MT.col_positions[col + 2 :] = [
-                e + increment
-                for e in islice(
-                    self.MT.col_positions, col + 2, len(self.MT.col_positions)
-                )
+                e + increment for e in islice(self.MT.col_positions, col + 2, len(self.MT.col_positions))
             ]
             self.MT.col_positions[col + 1] = new_col_pos
             if recreate:
                 self.MT.recreate_all_selection_boxes()
         return new_width
 
-    def set_width_of_all_cols(
-        self, width=None, only_set_if_too_small=False, recreate=True
-    ):
+    def set_width_of_all_cols(self, width=None, only_set_if_too_small=False, recreate=True):
         if width is None:
             if self.MT.all_columns_displayed:
                 iterable = range(self.MT.total_data_cols())
             else:
                 iterable = range(len(self.MT.displayed_columns))
             self.MT.col_positions = list(
                 accumulate(
@@ -1275,26 +1149,18 @@
                             for cn in iterable
                         ),
                     )
                 )
             )
         elif width is not None:
             if self.MT.all_columns_displayed:
-                self.MT.col_positions = list(
-                    accumulate(
-                        chain([0], (width for cn in range(self.MT.total_data_cols())))
-                    )
-                )
+                self.MT.col_positions = list(accumulate(chain([0], (width for cn in range(self.MT.total_data_cols())))))
             else:
                 self.MT.col_positions = list(
-                    accumulate(
-                        chain(
-                            [0], (width for cn in range(len(self.MT.displayed_columns)))
-                        )
-                    )
+                    accumulate(chain([0], (width for cn in range(len(self.MT.displayed_columns)))))
                 )
         if recreate:
             self.MT.recreate_all_selection_boxes()
 
     def align_cells(self, columns=[], align="global"):
         if isinstance(columns, int):
             cols = [columns]
@@ -1348,16 +1214,15 @@
                 redrawn = self.redraw_highlight(
                     fc + 1,
                     0,
                     sc,
                     self.current_height - 1,
                     fill=fill,
                     outline=self.header_fg
-                    if self.get_cell_kwargs(datacn, key="dropdown")
-                    and self.MT.show_dropdown_borders
+                    if self.get_cell_kwargs(datacn, key="dropdown") and self.MT.show_dropdown_borders
                     else "",
                     tag="hi",
                 )
         elif not kwargs:
             if "columns" in selections and c in selections["columns"]:
                 tf = self.header_selected_columns_fg
             elif "cells" in selections and c in selections["cells"]:
@@ -1369,27 +1234,23 @@
     def redraw_highlight(self, x1, y1, x2, y2, fill, outline, tag):
         config = (fill, outline)
         coords = (x1 - 1 if outline else x1, y1 - 1 if outline else y1, x2, y2)
         k = None
         if config in self.hidd_high:
             k = config
             iid, showing = self.hidd_high[k].pop()
-            if all(
-                int(crd1) == int(crd2) for crd1, crd2 in zip(self.coords(iid), coords)
-            ):
+            if all(int(crd1) == int(crd2) for crd1, crd2 in zip(self.coords(iid), coords)):
                 option = 0 if showing else 2
             else:
                 option = 1 if showing else 3
 
         elif self.hidd_high:
             k = next(iter(self.hidd_high))
             iid, showing = self.hidd_high[k].pop()
-            if all(
-                int(crd1) == int(crd2) for crd1, crd2 in zip(self.coords(iid), coords)
-            ):
+            if all(int(crd1) == int(crd2) for crd1, crd2 in zip(self.coords(iid), coords)):
                 option = 2 if showing else 3
             else:
                 option = 3
 
         else:
             iid, showing, option = (
                 self.create_rectangle(coords, fill=fill, outline=outline, tag=tag),
@@ -1399,17 +1260,15 @@
 
         if option in (1, 3):
             self.coords(iid, coords)
         if option in (2, 3):
             if showing:
                 self.itemconfig(iid, fill=fill, outline=outline)
             else:
-                self.itemconfig(
-                    iid, fill=fill, outline=outline, tag=tag, state="normal"
-                )
+                self.itemconfig(iid, fill=fill, outline=outline, tag=tag, state="normal")
 
         if k is not None and not self.hidd_high[k]:
             del self.hidd_high[k]
 
         self.disp_high[config].add(DrawnItem(iid=iid, showing=1))
         return True
 
@@ -1434,17 +1293,15 @@
                     tag=tag,
                     capstyle=tk.BUTT,
                     joinstyle=tk.ROUND,
                     state="normal",
                 )
             self.disp_grid[t] = True
         else:
-            self.disp_grid[
-                self.create_line(points, fill=fill, width=width, tag=tag)
-            ] = True
+            self.disp_grid[self.create_line(points, fill=fill, width=width, tag=tag)] = True
 
     def redraw_dropdown(
         self,
         x1,
         y1,
         x2,
         y2,
@@ -1452,17 +1309,15 @@
         outline,
         tag,
         draw_outline=True,
         draw_arrow=True,
         dd_is_open=False,
     ):
         if draw_outline and self.MT.show_dropdown_borders:
-            self.redraw_highlight(
-                x1 + 1, y1 + 1, x2, y2, fill="", outline=self.header_fg, tag=tag
-            )
+            self.redraw_highlight(x1 + 1, y1 + 1, x2, y2, fill="", outline=self.header_fg, tag=tag)
         if draw_arrow:
             topysub = floor(self.MT.header_half_txt_h / 2)
             mid_y = y1 + floor(self.MT.min_header_height / 2)
             if mid_y + topysub + 1 >= y1 + self.MT.header_txt_h - 1:
                 mid_y -= 1
             if mid_y - topysub + 2 <= y1 + 4 + topysub:
                 mid_y -= 1
@@ -1507,39 +1362,33 @@
             self.coords(t, points)
             if sh:
                 self.itemconfig(t, fill=outline, outline=fill)
             else:
                 self.itemconfig(t, fill=outline, outline=fill, tag=tag, state="normal")
             self.lift(t)
         else:
-            t = self.create_polygon(
-                points, fill=outline, outline=fill, tag=tag, smooth=True
-            )
+            t = self.create_polygon(points, fill=outline, outline=fill, tag=tag, smooth=True)
         self.disp_checkbox[t] = True
         if draw_check:
             # draw filled box
             x1 = x1 + 4
             y1 = y1 + 4
             x2 = x2 - 3
             y2 = y2 - 3
             points = self.MT.get_checkbox_points(x1, y1, x2, y2, radius=4)
             if self.hidd_checkbox:
                 t, sh = self.hidd_checkbox.popitem()
                 self.coords(t, points)
                 if sh:
                     self.itemconfig(t, fill=fill, outline=outline)
                 else:
-                    self.itemconfig(
-                        t, fill=fill, outline=outline, tag=tag, state="normal"
-                    )
+                    self.itemconfig(t, fill=fill, outline=outline, tag=tag, state="normal")
                 self.lift(t)
             else:
-                t = self.create_polygon(
-                    points, fill=fill, outline=outline, tag=tag, smooth=True
-                )
+                t = self.create_polygon(points, fill=fill, outline=outline, tag=tag, smooth=True)
             self.disp_checkbox[t] = True
 
     def redraw_grid_and_text(
         self,
         last_col_line_pos,
         scrollpos_left,
         x_stop,
@@ -1582,17 +1431,15 @@
             scrollpos_left,
             self.current_height - 2,
             x_stop,
             self.current_height,
         )
         draw_x = self.MT.col_positions[start_col]
         yend = self.current_height - 5
-        if (
-            self.MT.show_vertical_grid or self.width_resizing_enabled
-        ) and col_pos_exists:
+        if (self.MT.show_vertical_grid or self.width_resizing_enabled) and col_pos_exists:
             self.grid_cyc = cycle(self.grid_cyctup)
             points = [
                 x_stop - 1,
                 self.current_height - 1,
                 scrollpos_left - 1,
                 self.current_height - 1,
                 scrollpos_left - 1,
@@ -1606,37 +1453,31 @@
                 if st_or_end == "st":
                     points.extend(
                         [
                             draw_x,
                             -1,
                             draw_x,
                             self.current_height,
-                            self.MT.col_positions[c + 1]
-                            if len(self.MT.col_positions) - 1 > c
-                            else draw_x,
+                            self.MT.col_positions[c + 1] if len(self.MT.col_positions) - 1 > c else draw_x,
                             self.current_height,
                         ]
                     )
                 elif st_or_end == "end":
                     points.extend(
                         [
                             draw_x,
                             self.current_height,
                             draw_x,
                             -1,
-                            self.MT.col_positions[c + 1]
-                            if len(self.MT.col_positions) - 1 > c
-                            else draw_x,
+                            self.MT.col_positions[c + 1] if len(self.MT.col_positions) - 1 > c else draw_x,
                             -1,
                         ]
                     )
                 if points:
-                    self.redraw_gridline(
-                        points=points, fill=self.header_grid_fg, width=1, tag="v"
-                    )
+                    self.redraw_gridline(points=points, fill=self.header_grid_fg, width=1, tag="v")
         top = self.canvasy(0)
         c_2 = (
             self.header_selected_cells_bg
             if self.header_selected_cells_bg.startswith("#")
             else Color_Map_[self.header_selected_cells_bg]
         )
         c_3 = (
@@ -1646,17 +1487,15 @@
         )
         font = self.MT.header_font
         selections = self.get_redraw_selections(start_col, end_col)
         for c in range(start_col, end_col - 1):
             draw_y = self.MT.header_fl_ins
             cleftgridln = self.MT.col_positions[c]
             crightgridln = self.MT.col_positions[c + 1]
-            datacn = (
-                c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
-            )
+            datacn = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
             fill, dd_drawn = self.redraw_highlight_get_text_fg(
                 cleftgridln, crightgridln, c, c_2, c_3, selections, datacn
             )
 
             if datacn in self.cell_options and "align" in self.cell_options[datacn]:
                 align = self.cell_options[datacn]["align"]
             else:
@@ -1702,17 +1541,15 @@
                     mw = crightgridln - cleftgridln - 1
                     draw_x = crightgridln - 3
 
             elif align == "center":
                 # stop = cleftgridln + 5
                 if kwargs:
                     mw = crightgridln - cleftgridln - self.MT.header_txt_h - 2
-                    draw_x = cleftgridln + ceil(
-                        (crightgridln - cleftgridln - self.MT.header_txt_h) / 2
-                    )
+                    draw_x = cleftgridln + ceil((crightgridln - cleftgridln - self.MT.header_txt_h) / 2)
                     self.redraw_dropdown(
                         cleftgridln,
                         0,
                         crightgridln,
                         self.current_height - 1,
                         fill=fill,
                         outline=fill,
@@ -1745,17 +1582,15 @@
                     except Exception:
                         draw_check = False
                     self.redraw_checkbox(
                         cleftgridln + 2,
                         2,
                         cleftgridln + self.MT.header_txt_h + 3,
                         self.MT.header_txt_h + 3,
-                        fill=fill
-                        if kwargs["state"] == "normal"
-                        else self.header_grid_fg,
+                        fill=fill if kwargs["state"] == "normal" else self.header_grid_fg,
                         outline="",
                         tag="cb",
                         draw_check=draw_check,
                     )
             lns = self.get_valid_cell_data_as_str(datacn, fix=False).split("\n")
             if lns == [""]:
                 if self.show_default_header_for_empty:
@@ -1765,17 +1600,15 @@
             if mw > self.MT.header_txt_w and not (
                 (align == "w" and (draw_x > x_stop))
                 or (align == "e" and (draw_x > x_stop))
                 or (align == "center" and (cleftgridln + 5 > x_stop))
             ):
                 for txt in islice(
                     lns,
-                    self.lines_start_at
-                    if self.lines_start_at < len(lns)
-                    else len(lns) - 1,
+                    self.lines_start_at if self.lines_start_at < len(lns) else len(lns) - 1,
                     None,
                 ):
                     if draw_y > top:
                         config = TextCfg(txt, fill, font, align)
                         k = None
                         if config in self.hidd_text:
                             k = config
@@ -1809,17 +1642,15 @@
                                 1,
                                 4,
                             )
                         if option in (1, 3):
                             self.coords(iid, draw_x, draw_y)
                         if option in (2, 3):
                             if showing:
-                                self.itemconfig(
-                                    iid, text=txt, fill=fill, font=font, anchor=align
-                                )
+                                self.itemconfig(iid, text=txt, fill=fill, font=font, anchor=align)
                             else:
                                 self.itemconfig(
                                     iid,
                                     text=txt,
                                     fill=fill,
                                     font=font,
                                     anchor=align,
@@ -1843,29 +1674,25 @@
                                 self.itemconfig(iid, text=txt)
                                 wd = self.bbox(iid)
                                 while wd[2] - wd[0] > mw:
                                     txt = txt[1:]
                                     self.itemconfig(iid, text=txt)
                                     wd = self.bbox(iid)
                             elif align == "center":
-                                self.c_align_cyc = cycle(
-                                    self.centre_alignment_text_mod_indexes
-                                )
+                                self.c_align_cyc = cycle(self.centre_alignment_text_mod_indexes)
                                 tmod = ceil((len(txt) - int(len(txt) * (mw / wd))) / 2)
                                 txt = txt[tmod - 1 : -tmod]
                                 self.itemconfig(iid, text=txt)
                                 wd = self.bbox(iid)
                                 while wd[2] - wd[0] > mw:
                                     txt = txt[next(self.c_align_cyc)]
                                     self.itemconfig(iid, text=txt)
                                     wd = self.bbox(iid)
                                 self.coords(iid, draw_x, draw_y)
-                            self.disp_text[config._replace(txt=txt)].add(
-                                DrawnItem(iid=iid, showing=True)
-                            )
+                            self.disp_text[config._replace(txt=txt)].add(DrawnItem(iid=iid, showing=True))
                         else:
                             self.disp_text[config].add(DrawnItem(iid=iid, showing=True))
                     draw_y += self.MT.header_xtra_lines_increment
                     if draw_y - 1 > self.current_height:
                         break
         for cfg, set_ in self.hidd_text.items():
             for namedtup in tuple(set_):
@@ -1895,44 +1722,30 @@
     def get_redraw_selections(self, startc, endc):
         d = defaultdict(list)
         for item in chain(self.find_withtag("cells"), self.find_withtag("columns")):
             tags = self.gettags(item)
             d[tags[0]].append(tuple(int(e) for e in tags[1].split("_") if e))
         d2 = {}
         if "cells" in d:
-            d2["cells"] = {
-                c
-                for c in range(startc, endc)
-                for r1, c1, r2, c2 in d["cells"]
-                if c1 <= c and c2 > c
-            }
+            d2["cells"] = {c for c in range(startc, endc) for r1, c1, r2, c2 in d["cells"] if c1 <= c and c2 > c}
         if "columns" in d:
-            d2["columns"] = {
-                c
-                for c in range(startc, endc)
-                for r1, c1, r2, c2 in d["columns"]
-                if c1 <= c and c2 > c
-            }
+            d2["columns"] = {c for c in range(startc, endc) for r1, c1, r2, c2 in d["columns"] if c1 <= c and c2 > c}
         return d2
 
     def open_cell(self, event=None, ignore_existing_editor=False):
-        if not self.MT.anything_selected() or (
-            not ignore_existing_editor and self.text_editor_id is not None
-        ):
+        if not self.MT.anything_selected() or (not ignore_existing_editor and self.text_editor_id is not None):
             return
         currently_selected = self.MT.currently_selected()
         if not currently_selected:
             return
         x1 = int(currently_selected[1])
         datacn = x1 if self.MT.all_columns_displayed else self.MT.displayed_columns[x1]
         if self.get_cell_kwargs(datacn, key="readonly"):
             return
-        elif self.get_cell_kwargs(datacn, key="dropdown") or self.get_cell_kwargs(
-            datacn, key="checkbox"
-        ):
+        elif self.get_cell_kwargs(datacn, key="dropdown") or self.get_cell_kwargs(datacn, key="checkbox"):
             if self.MT.event_opens_dropdown_or_checkbox(event):
                 if self.get_cell_kwargs(datacn, key="dropdown"):
                     self.open_dropdown_window(x1, event=event)
                 elif self.get_cell_kwargs(datacn, key="checkbox"):
                     self.click_checkbox(x1, datacn)
         elif self.edit_cell_enabled:
             self.open_text_editor(event=event, c=x1, dropdown=False)
@@ -1962,21 +1775,18 @@
         extra_func_key = "??"
         if event is None or self.MT.event_opens_dropdown_or_checkbox(event):
             if event is not None:
                 if hasattr(event, "keysym") and event.keysym == "Return":
                     extra_func_key = "Return"
                 elif hasattr(event, "keysym") and event.keysym == "F2":
                     extra_func_key = "F2"
-            datacn = (
-                c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
-            )
+            datacn = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
             text = self.get_cell_data(datacn, none_to_empty_str=True, redirect_int=True)
         elif event is not None and (
-            (hasattr(event, "keysym") and event.keysym == "BackSpace")
-            or event.keycode in (8, 855638143)
+            (hasattr(event, "keysym") and event.keysym == "BackSpace") or event.keycode in (8, 855638143)
         ):
             extra_func_key = "BackSpace"
             text = ""
         elif event is not None and (
             (hasattr(event, "char") and event.char.isalpha())
             or (hasattr(event, "char") and event.char.isdigit())
             or (hasattr(event, "char") and event.char in symbols_set)
@@ -1984,40 +1794,34 @@
             extra_func_key = event.char
             text = event.char
         else:
             return False
         self.text_editor_loc = c
         if self.extra_begin_edit_cell_func is not None:
             try:
-                text = self.extra_begin_edit_cell_func(
-                    EditHeaderEvent(c, extra_func_key, text, "begin_edit_header")
-                )
+                text = self.extra_begin_edit_cell_func(EditHeaderEvent(c, extra_func_key, text, "begin_edit_header"))
             except Exception:
                 return False
             if text is None:
                 return False
             else:
                 text = text if isinstance(text, str) else f"{text}"
         text = "" if text is None else text
         if self.MT.cell_auto_resize_enabled:
             if self.height_resizing_enabled:
                 self.set_height_of_header_to_text(text)
             self.set_col_width_run_binding(c)
 
         if c == self.text_editor_loc and self.text_editor is not None:
-            self.text_editor.set_text(
-                self.text_editor.get() + "" if not isinstance(text, str) else text
-            )
+            self.text_editor.set_text(self.text_editor.get() + "" if not isinstance(text, str) else text)
             return
         if self.text_editor is not None:
             self.destroy_text_editor()
         if see:
-            has_redrawn = self.MT.see(
-                r=0, c=c, keep_yscroll=True, check_cell_visibility=True
-            )
+            has_redrawn = self.MT.see(r=0, c=c, keep_yscroll=True, check_cell_visibility=True)
             if not has_redrawn:
                 self.MT.refresh()
         self.text_editor_loc = c
         x = self.MT.col_positions[c] + 1
         y = 0
         w = self.MT.col_positions[c + 1] - x
         h = self.current_height + 1
@@ -2043,135 +1847,97 @@
             popup_menu_highlight_fg=self.MT.popup_menu_highlight_fg,
             binding=binding,
             align=self.get_cell_align(c),
             c=c,
             newline_binding=self.text_editor_has_wrapped,
         )
         self.text_editor.update_idletasks()
-        self.text_editor_id = self.create_window(
-            (x, y), window=self.text_editor, anchor="nw"
-        )
+        self.text_editor_id = self.create_window((x, y), window=self.text_editor, anchor="nw")
         if not dropdown:
             self.text_editor.textedit.focus_set()
             self.text_editor.scroll_to_bottom()
-        self.text_editor.textedit.bind(
-            "<Alt-Return>", lambda x: self.text_editor_newline_binding(c=c)
-        )
+        self.text_editor.textedit.bind("<Alt-Return>", lambda x: self.text_editor_newline_binding(c=c))
         if USER_OS == "darwin":
-            self.text_editor.textedit.bind(
-                "<Option-Return>", lambda x: self.text_editor_newline_binding(c=c)
-            )
+            self.text_editor.textedit.bind("<Option-Return>", lambda x: self.text_editor_newline_binding(c=c))
         for key, func in self.MT.text_editor_user_bound_keys.items():
             self.text_editor.textedit.bind(key, func)
         if binding is not None:
             self.text_editor.textedit.bind("<Tab>", lambda x: binding((c, "Tab")))
             self.text_editor.textedit.bind("<Return>", lambda x: binding((c, "Return")))
-            self.text_editor.textedit.bind(
-                "<FocusOut>", lambda x: binding((c, "FocusOut"))
-            )
+            self.text_editor.textedit.bind("<FocusOut>", lambda x: binding((c, "FocusOut")))
             self.text_editor.textedit.bind("<Escape>", lambda x: binding((c, "Escape")))
         elif binding is None and set_data_on_close:
-            self.text_editor.textedit.bind(
-                "<Tab>", lambda x: self.close_text_editor((c, "Tab"))
-            )
-            self.text_editor.textedit.bind(
-                "<Return>", lambda x: self.close_text_editor((c, "Return"))
-            )
+            self.text_editor.textedit.bind("<Tab>", lambda x: self.close_text_editor((c, "Tab")))
+            self.text_editor.textedit.bind("<Return>", lambda x: self.close_text_editor((c, "Return")))
             if not dropdown:
-                self.text_editor.textedit.bind(
-                    "<FocusOut>", lambda x: self.close_text_editor((c, "FocusOut"))
-                )
-            self.text_editor.textedit.bind(
-                "<Escape>", lambda x: self.close_text_editor((c, "Escape"))
-            )
+                self.text_editor.textedit.bind("<FocusOut>", lambda x: self.close_text_editor((c, "FocusOut")))
+            self.text_editor.textedit.bind("<Escape>", lambda x: self.close_text_editor((c, "Escape")))
         else:
-            self.text_editor.textedit.bind(
-                "<Escape>", lambda x: self.destroy_text_editor("Escape")
-            )
+            self.text_editor.textedit.bind("<Escape>", lambda x: self.destroy_text_editor("Escape"))
         return True
 
     # displayed indexes                             #just here to receive text editor arg
     def text_editor_has_wrapped(self, r=0, c=0, check_lines=None):
         if self.width_resizing_enabled:
-            datacn = (
-                c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
-            )
+            datacn = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
             curr_width = self.text_editor.winfo_width()
             new_width = curr_width + (self.MT.header_txt_h * 2)
             if new_width != curr_width:
                 self.text_editor.config(width=new_width)
-                self.set_col_width_run_binding(
-                    c, width=new_width, only_set_if_too_small=False
-                )
+                self.set_col_width_run_binding(c, width=new_width, only_set_if_too_small=False)
                 kwargs = self.get_cell_kwargs(datacn, key="dropdown")
                 if kwargs:
                     self.itemconfig(kwargs["canvas_id"], width=new_width)
                     kwargs["window"].update_idletasks()
                     kwargs["window"]._reselect()
-                self.MT.main_table_redraw_grid_and_text(
-                    redraw_header=True, redraw_row_index=False, redraw_table=True
-                )
+                self.MT.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=False, redraw_table=True)
 
     # displayed indexes
     def text_editor_newline_binding(self, r=0, c=0, event=None, check_lines=True):
         if self.height_resizing_enabled:
-            datacn = (
-                c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
-            )
+            datacn = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
             curr_height = self.text_editor.winfo_height()
             if (
                 not check_lines
-                or self.MT.get_lines_cell_height(
-                    self.text_editor.get_num_lines() + 1, font=self.MT.header_font
-                )
+                or self.MT.get_lines_cell_height(self.text_editor.get_num_lines() + 1, font=self.MT.header_font)
                 > curr_height
             ):
                 new_height = curr_height + self.MT.header_xtra_lines_increment
                 space_bot = self.MT.get_space_bot(0)
                 if new_height > space_bot:
                     new_height = space_bot
                 if new_height != curr_height:
                     self.text_editor.config(height=new_height)
                     self.set_height(new_height, set_TL=True)
                     kwargs = self.get_cell_kwargs(datacn, key="dropdown")
                     if kwargs:
-                        win_h, anchor = self.get_dropdown_height_anchor(
-                            datacn, new_height
-                        )
+                        win_h, anchor = self.get_dropdown_height_anchor(datacn, new_height)
                         self.coords(
                             kwargs["canvas_id"],
                             self.MT.col_positions[c],
                             new_height - 1,
                         )
-                        self.itemconfig(
-                            kwargs["canvas_id"], anchor=anchor, height=win_h
-                        )
+                        self.itemconfig(kwargs["canvas_id"], anchor=anchor, height=win_h)
 
     def bind_cell_edit(self, enable=True):
         if enable:
             self.edit_cell_enabled = True
         else:
             self.edit_cell_enabled = False
 
     def bind_text_editor_destroy(self, binding, c):
         self.text_editor.textedit.bind("<Return>", lambda x: binding((c, "Return")))
         self.text_editor.textedit.bind("<FocusOut>", lambda x: binding((c, "FocusOut")))
         self.text_editor.textedit.bind("<Escape>", lambda x: binding((c, "Escape")))
         self.text_editor.textedit.focus_set()
 
     def destroy_text_editor(self, event=None):
-        if (
-            event is not None
-            and self.extra_end_edit_cell_func is not None
-            and self.text_editor_loc is not None
-        ):
+        if event is not None and self.extra_end_edit_cell_func is not None and self.text_editor_loc is not None:
             self.extra_end_edit_cell_func(
-                EditHeaderEvent(
-                    int(self.text_editor_loc), "Escape", None, "escape_edit_header"
-                )
+                EditHeaderEvent(int(self.text_editor_loc), "Escape", None, "escape_edit_header")
             )
         self.text_editor_loc = None
         try:
             self.delete(self.text_editor_id)
         except Exception:
             pass
         try:
@@ -2193,35 +1959,27 @@
         destroy=True,
         move_down=True,
         redraw=True,
         recreate=True,
     ):
         if self.focus_get() is None and editor_info:
             return
-        if (
-            editor_info is not None
-            and len(editor_info) >= 2
-            and editor_info[1] == "Escape"
-        ):
+        if editor_info is not None and len(editor_info) >= 2 and editor_info[1] == "Escape":
             self.destroy_text_editor("Escape")
             self.close_dropdown_window(c)
             return
         if self.text_editor is not None:
             self.text_editor_value = self.text_editor.get()
         if destroy:
             self.destroy_text_editor()
         if set_data_on_close:
             if c is None and editor_info is not None and len(editor_info) >= 2:
                 c = editor_info[0]
-            datacn = (
-                c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
-            )
-            if self.extra_end_edit_cell_func is None and self.input_valid_for_cell(
-                datacn, self.text_editor_value
-            ):
+            datacn = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
+            if self.extra_end_edit_cell_func is None and self.input_valid_for_cell(datacn, self.text_editor_value):
                 self.set_cell_data_undo(
                     c,
                     datacn=datacn,
                     value=self.text_editor_value,
                     check_input_valid=False,
                 )
             elif (
@@ -2239,18 +1997,15 @@
                     EditHeaderEvent(
                         c,
                         editor_info[1] if len(editor_info) >= 2 else "FocusOut",
                         f"{self.text_editor_value}",
                         "end_edit_header",
                     )
                 )
-            elif (
-                self.extra_end_edit_cell_func is not None
-                and self.MT.edit_cell_validation
-            ):
+            elif self.extra_end_edit_cell_func is not None and self.MT.edit_cell_validation:
                 validation = self.extra_end_edit_cell_func(
                     EditHeaderEvent(
                         c,
                         editor_info[1] if len(editor_info) >= 2 else "FocusOut",
                         f"{self.text_editor_value}",
                         "end_edit_header",
                     )
@@ -2267,19 +2022,15 @@
         if move_down:
             pass
         self.close_dropdown_window(c)
         if recreate:
             self.MT.recreate_all_selection_boxes()
         if redraw:
             self.MT.refresh()
-        if (
-            editor_info is not None
-            and len(editor_info) >= 2
-            and editor_info[1] != "FocusOut"
-        ):
+        if editor_info is not None and len(editor_info) >= 2 and editor_info[1] != "FocusOut":
             self.focus_set()
         return "break"
 
     # internal event use
     def set_cell_data_undo(
         self,
         c=0,
@@ -2287,21 +2038,17 @@
         value="",
         cell_resize=True,
         undo=True,
         redraw=True,
         check_input_valid=True,
     ):
         if datacn is None:
-            datacn = (
-                c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
-            )
+            datacn = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
         if isinstance(self.MT._headers, int):
-            self.MT.set_cell_data_undo(
-                r=self.MT._headers, c=c, datacn=datacn, value=value, undo=True
-            )
+            self.MT.set_cell_data_undo(r=self.MT._headers, c=c, datacn=datacn, value=value, undo=True)
         else:
             self.fix_header(datacn)
             if not check_input_valid or self.input_valid_for_cell(datacn, value):
                 if self.MT.undo_enabled and undo:
                     self.MT.undo_storage.append(
                         zlib.compress(
                             pickle.dumps(
@@ -2313,17 +2060,15 @@
                                 )
                             )
                         )
                     )
                 self.set_cell_data(datacn=datacn, value=value)
         if cell_resize and self.MT.cell_auto_resize_enabled:
             if self.height_resizing_enabled:
-                self.set_height_of_header_to_text(
-                    self.get_valid_cell_data_as_str(datacn, fix=False)
-                )
+                self.set_height_of_header_to_text(self.get_valid_cell_data_as_str(datacn, fix=False))
             self.set_col_width_run_binding(c)
         if redraw:
             self.MT.refresh()
         self.parentframe.emit_event("<<SheetModified>>")
 
     def set_cell_data(self, datacn=None, value=""):
         if isinstance(self.MT._headers, int):
@@ -2350,23 +2095,19 @@
     def cell_equal_to(self, datacn, value):
         self.fix_header(datacn)
         if isinstance(self.MT._headers, list):
             return self.MT._headers[datacn] == value
         elif isinstance(self.MT._headers, int):
             return self.MT.cell_equal_to(self.MT._headers, datacn, value)
 
-    def get_cell_data(
-        self, datacn, get_displayed=False, none_to_empty_str=False, redirect_int=False
-    ):
+    def get_cell_data(self, datacn, get_displayed=False, none_to_empty_str=False, redirect_int=False):
         if get_displayed:
             return self.get_valid_cell_data_as_str(datacn, fix=False)
         if redirect_int and isinstance(self.MT._headers, int):  # internal use
-            return self.MT.get_cell_data(
-                self.MT._headers, datacn, none_to_empty_str=True
-            )
+            return self.MT.get_cell_data(self.MT._headers, datacn, none_to_empty_str=True)
         if (
             isinstance(self.MT._headers, int)
             or not self.MT._headers
             or datacn >= len(self.MT._headers)
             or (self.MT._headers[datacn] is None and none_to_empty_str)
         ):
             return ""
@@ -2376,89 +2117,66 @@
         kwargs = self.get_cell_kwargs(datacn, key="dropdown")
         if kwargs and kwargs["text"] is not None:
             return f"{kwargs['text']}"
         kwargs = self.get_cell_kwargs(datacn, key="checkbox")
         if kwargs:
             return f"{kwargs['text']}"
         if isinstance(self.MT._headers, int):
-            return self.MT.get_valid_cell_data_as_str(
-                self.MT._headers, datacn, get_displayed=True
-            )
+            return self.MT.get_valid_cell_data_as_str(self.MT._headers, datacn, get_displayed=True)
         if fix:
             self.fix_header(datacn)
         try:
-            return (
-                ""
-                if self.MT._headers[datacn] is None
-                else f"{self.MT._headers[datacn]}"
-            )
+            return "" if self.MT._headers[datacn] is None else f"{self.MT._headers[datacn]}"
         except Exception:
             return ""
 
     def get_value_for_empty_cell(self, datacn, c_ops=True):
         if self.get_cell_kwargs(datacn, key="checkbox", cell=c_ops):
             return False
         kwargs = self.get_cell_kwargs(datacn, key="dropdown", cell=c_ops)
         if kwargs and kwargs["validate_input"] and kwargs["values"]:
             return kwargs["values"][0]
         return ""
 
     def get_empty_header_seq(self, end, start=0, c_ops=True):
-        return [
-            self.get_value_for_empty_cell(datacn, c_ops=c_ops)
-            for datacn in range(start, end)
-        ]
+        return [self.get_value_for_empty_cell(datacn, c_ops=c_ops) for datacn in range(start, end)]
 
     def fix_header(self, datacn=None, fix_values=tuple()):
         if isinstance(self.MT._headers, int):
             return
         if isinstance(self.MT._headers, float):
             self.MT._headers = int(self.MT._headers)
             return
         if not isinstance(self.MT._headers, list):
             try:
                 self.MT._headers = list(self.MT._headers)
             except Exception:
                 self.MT._headers = []
         if isinstance(datacn, int) and datacn >= len(self.MT._headers):
-            self.MT._headers.extend(
-                self.get_empty_header_seq(end=datacn + 1, start=len(self.MT._headers))
-            )
+            self.MT._headers.extend(self.get_empty_header_seq(end=datacn + 1, start=len(self.MT._headers)))
         if fix_values:
-            for cn, v in enumerate(
-                islice(self.MT._headers, fix_values[0], fix_values[1])
-            ):
+            for cn, v in enumerate(islice(self.MT._headers, fix_values[0], fix_values[1])):
                 if not self.input_valid_for_cell(cn, v):
                     self.MT._headers[cn] = self.get_value_for_empty_cell(cn)
 
     # displayed indexes
     def set_col_width_run_binding(self, c, width=None, only_set_if_too_small=True):
         old_width = self.MT.col_positions[c + 1] - self.MT.col_positions[c]
-        new_width = self.set_col_width(
-            c, width=width, only_set_if_too_small=only_set_if_too_small
-        )
+        new_width = self.set_col_width(c, width=width, only_set_if_too_small=only_set_if_too_small)
         if self.column_width_resize_func is not None and old_width != new_width:
-            self.column_width_resize_func(
-                ResizeEvent("column_width_resize", c, old_width, new_width)
-            )
+            self.column_width_resize_func(ResizeEvent("column_width_resize", c, old_width, new_width))
 
     # internal event use
     def click_checkbox(self, c, datacn=None, undo=True, redraw=True):
         if datacn is None:
-            datacn = (
-                c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
-            )
+            datacn = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
         kwargs = self.get_cell_kwargs(datacn, key="checkbox")
         if kwargs["state"] == "normal":
             if isinstance(self.MT._headers, list):
-                value = (
-                    not self.MT._headers[datacn]
-                    if type(self.MT._headers[datacn]) == bool
-                    else False
-                )
+                value = not self.MT._headers[datacn] if type(self.MT._headers[datacn]) == bool else False
             elif isinstance(self.MT._headers, int):
                 value = (
                     not self.MT.data[self.MT._headers][datacn]
                     if type(self.MT.data[self.MT._headers][datacn]) == bool
                     else False
                 )
             else:
@@ -2495,60 +2213,50 @@
             self.delete_options_dropdown_and_checkbox()
         if "checkbox" not in self.options:
             self.options["checkbox"] = {}
         self.options["checkbox"] = get_checkbox_dict(**kwargs)
         total_cols = self.MT.total_data_cols()
         if isinstance(self.MT._headers, int):
             for datacn in range(total_cols):
-                self.MT.set_cell_data(
-                    datarn=self.MT._headers, datacn=datacn, value=kwargs["checked"]
-                )
+                self.MT.set_cell_data(datarn=self.MT._headers, datacn=datacn, value=kwargs["checked"])
         else:
             for datacn in range(total_cols):
                 self.set_cell_data(datacn=datacn, value=kwargs["checked"])
 
     def dropdown_header(self, **kwargs):
         self.destroy_opened_dropdown_window()
         if "dropdown" in self.options or "checkbox" in self.options:
             self.delete_options_dropdown_and_checkbox()
         if "dropdown" not in self.options:
             self.options["dropdown"] = {}
         self.options["dropdown"] = get_dropdown_dict(**kwargs)
         total_cols = self.MT.total_data_cols()
         value = (
-            kwargs["set_value"]
-            if kwargs["set_value"] is not None
-            else kwargs["values"][0]
-            if kwargs["values"]
-            else ""
+            kwargs["set_value"] if kwargs["set_value"] is not None else kwargs["values"][0] if kwargs["values"] else ""
         )
         if isinstance(self.MT._headers, int):
             for datacn in range(total_cols):
-                self.MT.set_cell_data(
-                    datarn=self.MT._headers, datacn=datacn, value=value
-                )
+                self.MT.set_cell_data(datarn=self.MT._headers, datacn=datacn, value=value)
         else:
             for datacn in range(total_cols):
                 self.set_cell_data(datacn=datacn, value=value)
 
     def create_checkbox(self, datacn=0, **kwargs):
         if datacn in self.cell_options and (
-            "dropdown" in self.cell_options[datacn]
-            or "checkbox" in self.cell_options[datacn]
+            "dropdown" in self.cell_options[datacn] or "checkbox" in self.cell_options[datacn]
         ):
             self.delete_cell_options_dropdown_and_checkbox(datacn)
         if datacn not in self.cell_options:
             self.cell_options[datacn] = {}
         self.cell_options[datacn]["checkbox"] = get_checkbox_dict(**kwargs)
         self.set_cell_data(datacn=datacn, value=kwargs["checked"])
 
     def create_dropdown(self, datacn=0, **kwargs):
         if datacn in self.cell_options and (
-            "dropdown" in self.cell_options[datacn]
-            or "checkbox" in self.cell_options[datacn]
+            "dropdown" in self.cell_options[datacn] or "checkbox" in self.cell_options[datacn]
         ):
             self.delete_cell_options_dropdown_and_checkbox(datacn)
         if datacn not in self.cell_options:
             self.cell_options[datacn] = {}
         self.cell_options[datacn]["dropdown"] = get_dropdown_dict(**kwargs)
         self.set_cell_data(
             datacn=datacn,
@@ -2558,23 +2266,17 @@
             if kwargs["values"]
             else "",
         )
 
     def get_dropdown_height_anchor(self, datacn, text_editor_h=None):
         win_h = 5
         for i, v in enumerate(self.get_cell_kwargs(datacn, key="dropdown")["values"]):
-            v_numlines = len(
-                v.split("\n") if isinstance(v, str) else f"{v}".split("\n")
-            )
+            v_numlines = len(v.split("\n") if isinstance(v, str) else f"{v}".split("\n"))
             if v_numlines > 1:
-                win_h += (
-                    self.MT.header_fl_ins
-                    + (v_numlines * self.MT.header_xtra_lines_increment)
-                    + 5
-                )  # end of cell
+                win_h += self.MT.header_fl_ins + (v_numlines * self.MT.header_xtra_lines_increment) + 5  # end of cell
             else:
                 win_h += self.MT.min_header_height
             if i == 5:
                 break
         if win_h > 500:
             win_h = 500
         space_bot = self.MT.get_space_bot(0, text_editor_h)
@@ -2587,17 +2289,15 @@
             win_h = win_h2
         return win_h, "nw"
 
     def open_dropdown_window(self, c, datacn=None, event=None):
         self.destroy_text_editor("Escape")
         self.destroy_opened_dropdown_window()
         if datacn is None:
-            datacn = (
-                c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
-            )
+            datacn = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
         kwargs = self.get_cell_kwargs(datacn, key="dropdown")
         if kwargs["state"] == "normal":
             if not self.open_text_editor(event=event, c=c, dropdown=True):
                 return
         win_h, anchor = self.get_dropdown_height_anchor(datacn)
         window = self.MT.parentframe.dropdown_class(
             self.MT.winfo_toplevel(),
@@ -2618,24 +2318,20 @@
             search_function=kwargs["search_function"],
             arrowkey_RIGHT=self.MT.arrowkey_RIGHT,
             arrowkey_LEFT=self.MT.arrowkey_LEFT,
             align="w",
             single_index="c",
         )
         ypos = self.current_height - 1
-        kwargs["canvas_id"] = self.create_window(
-            (self.MT.col_positions[c], ypos), window=window, anchor=anchor
-        )
+        kwargs["canvas_id"] = self.create_window((self.MT.col_positions[c], ypos), window=window, anchor=anchor)
         if kwargs["state"] == "normal":
             self.text_editor.textedit.bind(
                 "<<TextModified>>",
                 lambda x: window.search_and_see(
-                    DropDownModifiedEvent(
-                        "HeaderComboboxModified", 0, c, self.text_editor.get()
-                    )
+                    DropDownModifiedEvent("HeaderComboboxModified", 0, c, self.text_editor.get())
                 ),
             )
             if kwargs["modified_function"] is not None:
                 window.modified_function = kwargs["modified_function"]
             self.update_idletasks()
             try:
                 self.after(1, lambda: self.text_editor.textedit.focus())
@@ -2648,61 +2344,37 @@
             self.update_idletasks()
             window.focus_set()
             redraw = True
         self.existing_dropdown_window = window
         kwargs["window"] = window
         self.existing_dropdown_canvas_id = kwargs["canvas_id"]
         if redraw:
-            self.MT.main_table_redraw_grid_and_text(
-                redraw_header=True, redraw_row_index=False, redraw_table=False
-            )
+            self.MT.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=False, redraw_table=False)
 
     def close_dropdown_window(self, c=None, selection=None, redraw=True):
         if c is not None and selection is not None:
-            datacn = (
-                c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
-            )
+            datacn = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
             kwargs = self.get_cell_kwargs(datacn, key="dropdown")
-            if (
-                kwargs["select_function"] is not None
-            ):  # user has specified a selection function
+            if kwargs["select_function"] is not None:  # user has specified a selection function
                 kwargs["select_function"](
-                    EditHeaderEvent(
-                        c, "HeaderComboboxSelected", f"{selection}", "end_edit_header"
-                    )
+                    EditHeaderEvent(c, "HeaderComboboxSelected", f"{selection}", "end_edit_header")
                 )
             if self.extra_end_edit_cell_func is None:
-                self.set_cell_data_undo(
-                    c, datacn=datacn, value=selection, redraw=not redraw
-                )
-            elif (
-                self.extra_end_edit_cell_func is not None
-                and self.MT.edit_cell_validation
-            ):
+                self.set_cell_data_undo(c, datacn=datacn, value=selection, redraw=not redraw)
+            elif self.extra_end_edit_cell_func is not None and self.MT.edit_cell_validation:
                 validation = self.extra_end_edit_cell_func(
-                    EditHeaderEvent(
-                        c, "HeaderComboboxSelected", f"{selection}", "end_edit_header"
-                    )
+                    EditHeaderEvent(c, "HeaderComboboxSelected", f"{selection}", "end_edit_header")
                 )
                 if validation is not None:
                     selection = validation
-                self.set_cell_data_undo(
-                    c, datacn=datacn, value=selection, redraw=not redraw
-                )
-            elif (
-                self.extra_end_edit_cell_func is not None
-                and not self.MT.edit_cell_validation
-            ):
-                self.set_cell_data_undo(
-                    c, datacn=datacn, value=selection, redraw=not redraw
-                )
+                self.set_cell_data_undo(c, datacn=datacn, value=selection, redraw=not redraw)
+            elif self.extra_end_edit_cell_func is not None and not self.MT.edit_cell_validation:
+                self.set_cell_data_undo(c, datacn=datacn, value=selection, redraw=not redraw)
                 self.extra_end_edit_cell_func(
-                    EditHeaderEvent(
-                        c, "HeaderComboboxSelected", f"{selection}", "end_edit_header"
-                    )
+                    EditHeaderEvent(c, "HeaderComboboxSelected", f"{selection}", "end_edit_header")
                 )
             self.focus_set()
             self.MT.recreate_all_selection_boxes()
         self.destroy_text_editor("Escape")
         self.destroy_opened_dropdown_window(c)
         if redraw:
             self.MT.refresh()
@@ -2731,17 +2403,15 @@
 
     # function can receive two None args
     def destroy_opened_dropdown_window(self, c=None, datacn=None):
         if c is None and datacn is None and self.existing_dropdown_window is not None:
             c = self.get_existing_dropdown_coords()
         if c is not None or datacn is not None:
             if datacn is None:
-                datacn_ = (
-                    c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
-                )
+                datacn_ = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
             else:
                 datacn_ = datacn
         else:
             datacn_ = None
         try:
             self.delete(self.existing_dropdown_canvas_id)
         except Exception:
```

### Comparing `tksheet-6.1.3/tksheet/_tksheet_formatters.py` & `tksheet-6.1.4/tksheet/_tksheet_formatters.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 from typing import Any, Union
 
-from ._tksheet_other_classes import *
-from ._tksheet_vars import *
+from ._tksheet_vars import (
+    falsy,
+    nonelike,
+    truthy,
+)
 
 
 def is_none_like(n: Any):
     if (isinstance(n, str) and n.lower().replace(" ", "") in nonelike) or n in nonelike:
         return True
     return False
 
@@ -287,19 +290,15 @@
         if isinstance(value, self.valid_datatypes):
             return True
         return False
 
     def format_data(self, value):
         if self.pre_format_function:
             value = self.pre_format_function(value)
-        value = (
-            None
-            if (self.nullable and is_none_like(value))
-            else self.format_function(value, **self.kwargs)
-        )
+        value = None if (self.nullable and is_none_like(value)) else self.format_function(value, **self.kwargs)
         if self.post_format_function and self.valid(value):
             value = self.post_format_function(value)
         return value
 
     def get_data_with_valid_check(self):
         if self.valid():
             return self.value
```

### Comparing `tksheet-6.1.3/tksheet/_tksheet_main_table.py` & `tksheet-6.1.4/tksheet/_tksheet_main_table.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,17 +6,50 @@
 import zlib
 from collections import defaultdict, deque
 from itertools import accumulate, chain, cycle, islice, product, repeat
 from math import ceil, floor
 from tkinter import TclError
 from typing import Any, Union
 
-from ._tksheet_formatters import *
-from ._tksheet_other_classes import *
-from ._tksheet_vars import *
+from ._tksheet_formatters import (
+    data_to_str,
+    format_data,
+    get_clipboard_data,
+    get_data_with_valid_check,
+    is_bool_like,
+    try_to_bool,
+)
+from ._tksheet_other_classes import (
+    CtrlKeyEvent,
+    CurrentlySelectedClass,
+    DeleteRowColumnEvent,
+    DeselectionEvent,
+    DrawnItem,
+    DropDownModifiedEvent,
+    EditCellEvent,
+    InsertEvent,
+    PasteEvent,
+    ResizeEvent,
+    SelectCellEvent,
+    SelectionBoxEvent,
+    TextCfg,
+    TextEditor,
+    UndoEvent,
+    get_checkbox_dict,
+    get_dropdown_dict,
+    is_iterable,
+)
+from ._tksheet_vars import (
+    USER_OS,
+    Color_Map_,
+    arrowkey_bindings_helper,
+    ctrl_key,
+    rc_binding,
+    symbols_set,
+)
 
 
 class MainTable(tk.Canvas):
     def __init__(self, *args, **kwargs):
         tk.Canvas.__init__(
             self,
             kwargs["parentframe"],
@@ -54,27 +87,14 @@
         self.hidd_checkbox = {}
 
         self.cell_options = {}
         self.col_options = {}
         self.row_options = {}
         self.options = {}
 
-        """
-        cell options dict looks like:
-        {(row int, column int): {'dropdown': {'values': values,
-                                              'window': "no dropdown open",
-                                              'select_function': selection_function,
-                                              'keypress_function': keypress_function,
-                                              'state': state},
-                                 'highlight: (bg, fg),
-                                 'align': "e",
-                                 'readonly': True,
-                                 'format': {}
-                                }
-        """
         self.arrowkey_binding_functions = {
             "tab": self.tab_key,
             "up": self.arrowkey_UP,
             "right": self.arrowkey_RIGHT,
             "down": self.arrowkey_DOWN,
             "left": self.arrowkey_LEFT,
             "prior": self.page_UP,
@@ -96,28 +116,22 @@
             if isinstance(kwargs["from_clipboard_delimiters"], str)
             else "".join(kwargs["from_clipboard_delimiters"])
         )
         self.page_up_down_select_row = kwargs["page_up_down_select_row"]
         self.expand_sheet_if_paste_too_big = kwargs["expand_sheet_if_paste_too_big"]
         self.paste_insert_column_limit = kwargs["paste_insert_column_limit"]
         self.paste_insert_row_limit = kwargs["paste_insert_row_limit"]
-        self.arrow_key_down_right_scroll_page = kwargs[
-            "arrow_key_down_right_scroll_page"
-        ]
+        self.arrow_key_down_right_scroll_page = kwargs["arrow_key_down_right_scroll_page"]
         self.cell_auto_resize_enabled = kwargs["enable_edit_cell_auto_resize"]
         self.edit_cell_validation = kwargs["edit_cell_validation"]
-        self.display_selected_fg_over_highlights = kwargs[
-            "display_selected_fg_over_highlights"
-        ]
+        self.display_selected_fg_over_highlights = kwargs["display_selected_fg_over_highlights"]
         self.show_index = kwargs["show_index"]
         self.show_header = kwargs["show_header"]
         self.selected_rows_to_end_of_window = kwargs["selected_rows_to_end_of_window"]
-        self.horizontal_grid_to_end_of_window = kwargs[
-            "horizontal_grid_to_end_of_window"
-        ]
+        self.horizontal_grid_to_end_of_window = kwargs["horizontal_grid_to_end_of_window"]
         self.vertical_grid_to_end_of_window = kwargs["vertical_grid_to_end_of_window"]
         self.empty_horizontal = kwargs["empty_horizontal"]
         self.empty_vertical = kwargs["empty_vertical"]
         self.show_vertical_grid = kwargs["show_vertical_grid"]
         self.show_horizontal_grid = kwargs["show_horizontal_grid"]
         self.min_row_height = 0
         self.min_header_height = 0
@@ -165,17 +179,16 @@
         self.deselection_binding_func = None
         self.drag_selection_binding_func = None
         self.shift_selection_binding_func = None
         self.ctrl_selection_binding_func = None
         self.select_all_binding_func = None
 
         self.single_selection_enabled = False
-        self.toggle_selection_enabled = (
-            False  # with this mode every left click adds the cell to selected cells
-        )
+        # with this mode every left click adds the cell to selected cells
+        self.toggle_selection_enabled = False
         self.show_dropdown_borders = kwargs["show_dropdown_borders"]
         self.drag_selection_enabled = False
         self.select_all_enabled = False
         self.undo_enabled = False
         self.cut_enabled = False
         self.copy_enabled = False
         self.paste_enabled = False
@@ -213,79 +226,66 @@
         self.index_font_sze = kwargs["index_font"][1]
         self.index_font_wgt = kwargs["index_font"][2]
         self.header_font = kwargs["header_font"]
         self.header_font_fam = kwargs["header_font"][0]
         self.header_font_sze = kwargs["header_font"][1]
         self.header_font_wgt = kwargs["header_font"][2]
         self.txt_measure_canvas = tk.Canvas(self)
-        self.txt_measure_canvas_text = self.txt_measure_canvas.create_text(
-            0, 0, text="", font=self.table_font
-        )
+        self.txt_measure_canvas_text = self.txt_measure_canvas.create_text(0, 0, text="", font=self.table_font)
         self.text_editor = None
         self.text_editor_id = None
 
         self.max_row_height = float(kwargs["max_row_height"])
         self.max_index_width = float(kwargs["max_index_width"])
         self.max_column_width = float(kwargs["max_column_width"])
         self.max_header_height = float(kwargs["max_header_height"])
         if kwargs["row_index_width"] is None:
             self.RI.set_width(70)
             self.default_index_width = 70
         else:
             self.RI.set_width(kwargs["row_index_width"])
             self.default_index_width = kwargs["row_index_width"]
         self.default_header_height = (
-            kwargs["header_height"]
-            if isinstance(kwargs["header_height"], str)
-            else "pixels",
+            kwargs["header_height"] if isinstance(kwargs["header_height"], str) else "pixels",
             kwargs["header_height"]
             if isinstance(kwargs["header_height"], int)
-            else self.get_lines_cell_height(
-                int(kwargs["header_height"]), font=self.header_font
-            ),
+            else self.get_lines_cell_height(int(kwargs["header_height"]), font=self.header_font),
         )
         self.default_column_width = kwargs["column_width"]
         self.default_row_height = (
             kwargs["row_height"] if isinstance(kwargs["row_height"], str) else "pixels",
             kwargs["row_height"]
             if isinstance(kwargs["row_height"], int)
             else self.get_lines_cell_height(int(kwargs["row_height"])),
         )
-        self.set_font_help()
+        self.set_table_font_help()
         self.set_header_font_help()
         self.set_index_font_help()
         self.data = kwargs["data_reference"]
         if isinstance(self.data, (list, tuple)):
             self.data = kwargs["data_reference"]
         else:
             self.data = []
         if not self.data:
             if (
                 isinstance(kwargs["total_rows"], int)
                 and isinstance(kwargs["total_cols"], int)
                 and kwargs["total_rows"] > 0
                 and kwargs["total_cols"] > 0
             ):
-                self.data = [
-                    list(repeat("", kwargs["total_cols"]))
-                    for i in range(kwargs["total_rows"])
-                ]
-        _header = (
-            kwargs["header"] if kwargs["header"] is not None else kwargs["headers"]
-        )
+                self.data = [list(repeat("", kwargs["total_cols"])) for i in range(kwargs["total_rows"])]
+        _header = kwargs["header"] if kwargs["header"] is not None else kwargs["headers"]
         if isinstance(_header, int):
             self._headers = _header
         else:
             if _header:
                 self._headers = _header
             else:
                 self._headers = []
-        _row_index = (
-            kwargs["index"] if kwargs["index"] is not None else kwargs["row_index"]
-        )
+        _row_index = kwargs["index"] if kwargs["index"] is not None else kwargs["row_index"]
         if isinstance(_row_index, int):
             self._row_index = _row_index
         else:
             if _row_index:
                 self._row_index = _row_index
             else:
                 self._row_index = []
@@ -311,17 +311,15 @@
         self.table_fg = kwargs["table_fg"]
         self.table_selected_cells_border_fg = kwargs["table_selected_cells_border_fg"]
         self.table_selected_cells_bg = kwargs["table_selected_cells_bg"]
         self.table_selected_cells_fg = kwargs["table_selected_cells_fg"]
         self.table_selected_rows_border_fg = kwargs["table_selected_rows_border_fg"]
         self.table_selected_rows_bg = kwargs["table_selected_rows_bg"]
         self.table_selected_rows_fg = kwargs["table_selected_rows_fg"]
-        self.table_selected_columns_border_fg = kwargs[
-            "table_selected_columns_border_fg"
-        ]
+        self.table_selected_columns_border_fg = kwargs["table_selected_columns_border_fg"]
         self.table_selected_columns_bg = kwargs["table_selected_columns_bg"]
         self.table_selected_columns_fg = kwargs["table_selected_columns_fg"]
         self.table_bg = kwargs["table_bg"]
         self.popup_menu_font = kwargs["popup_menu_font"]
         self.popup_menu_fg = kwargs["popup_menu_fg"]
         self.popup_menu_bg = kwargs["popup_menu_bg"]
         self.popup_menu_highlight_bg = kwargs["popup_menu_highlight_bg"]
@@ -357,20 +355,16 @@
             self.CH.bind("<Shift-MouseWheel>", self.shift_mousewheel)
             self.RI.bind("<MouseWheel>", self.mousewheel)
             self.bind(rc_binding, self.rc)
             self.bind(f"<{ctrl_key}-ButtonPress-1>", self.ctrl_b1_press)
             self.CH.bind(f"<{ctrl_key}-ButtonPress-1>", self.CH.ctrl_b1_press)
             self.RI.bind(f"<{ctrl_key}-ButtonPress-1>", self.RI.ctrl_b1_press)
             self.bind(f"<{ctrl_key}-Shift-ButtonPress-1>", self.ctrl_shift_b1_press)
-            self.CH.bind(
-                f"<{ctrl_key}-Shift-ButtonPress-1>", self.CH.ctrl_shift_b1_press
-            )
-            self.RI.bind(
-                f"<{ctrl_key}-Shift-ButtonPress-1>", self.RI.ctrl_shift_b1_press
-            )
+            self.CH.bind(f"<{ctrl_key}-Shift-ButtonPress-1>", self.CH.ctrl_shift_b1_press)
+            self.RI.bind(f"<{ctrl_key}-Shift-ButtonPress-1>", self.RI.ctrl_shift_b1_press)
             self.bind(f"<{ctrl_key}-B1-Motion>", self.ctrl_b1_motion)
             self.CH.bind(f"<{ctrl_key}-B1-Motion>", self.CH.ctrl_b1_motion)
             self.RI.bind(f"<{ctrl_key}-B1-Motion>", self.RI.ctrl_b1_motion)
         else:
             self.unbind("<Configure>")
             self.unbind("<Motion>")
             self.unbind("<ButtonPress-1>")
@@ -426,17 +420,15 @@
             self.after(1500, self.delete_ctrl_outlines)
 
     def create_ctrl_outline(self, x1, y1, x2, y2, fill, dash, width, outline, tag):
         if self.hidd_ctrl_outline:
             t, sh = self.hidd_ctrl_outline.popitem()
             self.coords(t, x1, y1, x2, y2)
             if sh:
-                self.itemconfig(
-                    t, fill=fill, dash=dash, width=width, outline=outline, tag=tag
-                )
+                self.itemconfig(t, fill=fill, dash=dash, width=width, outline=outline, tag=tag)
             else:
                 self.itemconfig(
                     t,
                     fill=fill,
                     dash=dash,
                     width=width,
                     outline=outline,
@@ -469,27 +461,23 @@
     def get_ctrl_x_c_boxes(self):
         currently_selected = self.currently_selected()
         boxes = {}
         if currently_selected.type_ in ("cell", "column"):
             for item in chain(self.find_withtag("cells"), self.find_withtag("columns")):
                 alltags = self.gettags(item)
                 boxes[tuple(int(e) for e in alltags[1].split("_") if e)] = alltags[0]
-            curr_box = self.find_last_selected_box_with_current_from_boxes(
-                currently_selected, boxes
-            )
+            curr_box = self.find_last_selected_box_with_current_from_boxes(currently_selected, boxes)
             maxrows = curr_box[2] - curr_box[0]
             for box in tuple(boxes):
                 if box[2] - box[0] != maxrows:
                     del boxes[box]
             return boxes, maxrows
         else:
             for item in self.find_withtag("rows"):
-                boxes[
-                    tuple(int(e) for e in self.gettags(item)[1].split("_") if e)
-                ] = "rows"
+                boxes[tuple(int(e) for e in self.gettags(item)[1].split("_") if e)] = "rows"
             return boxes
 
     def ctrl_c(self, event=None):
         currently_selected = self.currently_selected()
         if currently_selected:
             s = io.StringIO()
             writer = csv.writer(
@@ -500,79 +488,51 @@
                 lineterminator=self.to_clipboard_lineterminator,
             )
             rows = []
             if currently_selected.type_ in ("cell", "column"):
                 boxes, maxrows = self.get_ctrl_x_c_boxes()
                 if self.extra_begin_ctrl_c_func is not None:
                     try:
-                        self.extra_begin_ctrl_c_func(
-                            CtrlKeyEvent(
-                                "begin_ctrl_c", boxes, currently_selected, tuple()
-                            )
-                        )
+                        self.extra_begin_ctrl_c_func(CtrlKeyEvent("begin_ctrl_c", boxes, currently_selected, tuple()))
                     except Exception:
                         return
                 for rn in range(maxrows):
                     row = []
                     for r1, c1, r2, c2 in boxes:
                         if r2 - r1 < maxrows:
                             continue
-                        datarn = (
-                            (r1 + rn)
-                            if self.all_rows_displayed
-                            else self.displayed_rows[r1 + rn]
-                        )
+                        datarn = (r1 + rn) if self.all_rows_displayed else self.displayed_rows[r1 + rn]
                         for c in range(c1, c2):
-                            datacn = (
-                                c
-                                if self.all_columns_displayed
-                                else self.displayed_columns[c]
-                            )
+                            datacn = c if self.all_columns_displayed else self.displayed_columns[c]
                             row.append(self.get_cell_clipboard(datarn, datacn))
                     writer.writerow(row)
                     rows.append(row)
             else:
                 boxes = self.get_ctrl_x_c_boxes()
                 if self.extra_begin_ctrl_c_func is not None:
                     try:
-                        self.extra_begin_ctrl_c_func(
-                            CtrlKeyEvent(
-                                "begin_ctrl_c", boxes, currently_selected, tuple()
-                            )
-                        )
+                        self.extra_begin_ctrl_c_func(CtrlKeyEvent("begin_ctrl_c", boxes, currently_selected, tuple()))
                     except Exception:
                         return
                 for r1, c1, r2, c2 in boxes:
                     for rn in range(r2 - r1):
                         row = []
-                        datarn = (
-                            (r1 + rn)
-                            if self.all_rows_displayed
-                            else self.displayed_rows[r1 + rn]
-                        )
+                        datarn = (r1 + rn) if self.all_rows_displayed else self.displayed_rows[r1 + rn]
                         for c in range(c1, c2):
-                            datacn = (
-                                c
-                                if self.all_columns_displayed
-                                else self.displayed_columns[c]
-                            )
+                            datacn = c if self.all_columns_displayed else self.displayed_columns[c]
                             row.append(self.get_cell_clipboard(datarn, datacn))
                         writer.writerow(row)
                         rows.append(row)
             for r1, c1, r2, c2 in boxes:
-                self.show_ctrl_outline(
-                    canvas="table", start_cell=(c1, r1), end_cell=(c2, r2)
-                )
+                self.show_ctrl_outline(canvas="table", start_cell=(c1, r1), end_cell=(c2, r2))
             self.clipboard_clear()
             self.clipboard_append(s.getvalue())
             self.update_idletasks()
             if self.extra_end_ctrl_c_func is not None:
-                self.extra_end_ctrl_c_func(
-                    CtrlKeyEvent("end_ctrl_c", boxes, currently_selected, rows)
-                )
+                self.extra_end_ctrl_c_func(CtrlKeyEvent("end_ctrl_c", boxes, currently_selected, rows))
 
     def ctrl_x(self, event=None):
         if not self.anything_selected():
             return
         undo_storage = {}
         s = io.StringIO()
         writer = csv.writer(
@@ -585,161 +545,107 @@
         currently_selected = self.currently_selected()
         rows = []
         changes = 0
         if currently_selected.type_ in ("cell", "column"):
             boxes, maxrows = self.get_ctrl_x_c_boxes()
             if self.extra_begin_ctrl_x_func is not None:
                 try:
-                    self.extra_begin_ctrl_x_func(
-                        CtrlKeyEvent("begin_ctrl_x", boxes, currently_selected, tuple())
-                    )
+                    self.extra_begin_ctrl_x_func(CtrlKeyEvent("begin_ctrl_x", boxes, currently_selected, tuple()))
                 except Exception:
                     return
             for rn in range(maxrows):
                 row = []
                 for r1, c1, r2, c2 in boxes:
                     if r2 - r1 < maxrows:
                         continue
-                    datarn = (
-                        (r1 + rn)
-                        if self.all_rows_displayed
-                        else self.displayed_rows[r1 + rn]
-                    )
+                    datarn = (r1 + rn) if self.all_rows_displayed else self.displayed_rows[r1 + rn]
                     for c in range(c1, c2):
-                        datacn = (
-                            c
-                            if self.all_columns_displayed
-                            else self.displayed_columns[c]
-                        )
+                        datacn = c if self.all_columns_displayed else self.displayed_columns[c]
                         row.append(self.get_cell_clipboard(datarn, datacn))
                 writer.writerow(row)
                 rows.append(row)
             for rn in range(maxrows):
                 for r1, c1, r2, c2 in boxes:
                     if r2 - r1 < maxrows:
                         continue
-                    datarn = (
-                        (r1 + rn)
-                        if self.all_rows_displayed
-                        else self.displayed_rows[r1 + rn]
-                    )
+                    datarn = (r1 + rn) if self.all_rows_displayed else self.displayed_rows[r1 + rn]
                     for c in range(c1, c2):
-                        datacn = (
-                            c
-                            if self.all_columns_displayed
-                            else self.displayed_columns[c]
-                        )
+                        datacn = c if self.all_columns_displayed else self.displayed_columns[c]
                         if self.input_valid_for_cell(datarn, datacn, ""):
                             if self.undo_enabled:
-                                undo_storage[(datarn, datacn)] = self.get_cell_data(
-                                    datarn, datacn
-                                )
+                                undo_storage[(datarn, datacn)] = self.get_cell_data(datarn, datacn)
                             self.set_cell_data(datarn, datacn, "")
                             changes += 1
         else:
             boxes = self.get_ctrl_x_c_boxes()
             if self.extra_begin_ctrl_x_func is not None:
                 try:
-                    self.extra_begin_ctrl_x_func(
-                        CtrlKeyEvent("begin_ctrl_x", boxes, currently_selected, tuple())
-                    )
+                    self.extra_begin_ctrl_x_func(CtrlKeyEvent("begin_ctrl_x", boxes, currently_selected, tuple()))
                 except Exception:
                     return
             for r1, c1, r2, c2 in boxes:
                 for rn in range(r2 - r1):
                     row = []
-                    datarn = (
-                        (r1 + rn)
-                        if self.all_rows_displayed
-                        else self.displayed_rows[r1 + rn]
-                    )
+                    datarn = (r1 + rn) if self.all_rows_displayed else self.displayed_rows[r1 + rn]
                     for c in range(c1, c2):
-                        datacn = (
-                            c
-                            if self.all_columns_displayed
-                            else self.displayed_columns[c]
-                        )
+                        datacn = c if self.all_columns_displayed else self.displayed_columns[c]
                         row.append(self.get_cell_data(datarn, datacn))
                     writer.writerow(row)
                     rows.append(row)
             for r1, c1, r2, c2 in boxes:
                 for rn in range(r2 - r1):
-                    datarn = (
-                        (r1 + rn)
-                        if self.all_rows_displayed
-                        else self.displayed_rows[r1 + rn]
-                    )
+                    datarn = (r1 + rn) if self.all_rows_displayed else self.displayed_rows[r1 + rn]
                     for c in range(c1, c2):
-                        datacn = (
-                            c
-                            if self.all_columns_displayed
-                            else self.displayed_columns[c]
-                        )
+                        datacn = c if self.all_columns_displayed else self.displayed_columns[c]
                         if self.input_valid_for_cell(datarn, datacn, ""):
                             if self.undo_enabled:
-                                undo_storage[(datarn, datacn)] = self.get_cell_data(
-                                    datarn, datacn
-                                )
+                                undo_storage[(datarn, datacn)] = self.get_cell_data(datarn, datacn)
                             self.set_cell_data(datarn, datacn, "")
                             changes += 1
         if changes and self.undo_enabled:
             self.undo_storage.append(
-                zlib.compress(
-                    pickle.dumps(
-                        ("edit_cells", undo_storage, boxes, currently_selected)
-                    )
-                )
+                zlib.compress(pickle.dumps(("edit_cells", undo_storage, boxes, currently_selected)))
             )
         self.clipboard_clear()
         self.clipboard_append(s.getvalue())
         self.update_idletasks()
         self.refresh()
         for r1, c1, r2, c2 in boxes:
-            self.show_ctrl_outline(
-                canvas="table", start_cell=(c1, r1), end_cell=(c2, r2)
-            )
+            self.show_ctrl_outline(canvas="table", start_cell=(c1, r1), end_cell=(c2, r2))
         if self.extra_end_ctrl_x_func is not None:
-            self.extra_end_ctrl_x_func(
-                CtrlKeyEvent("end_ctrl_x", boxes, currently_selected, rows)
-            )
+            self.extra_end_ctrl_x_func(CtrlKeyEvent("end_ctrl_x", boxes, currently_selected, rows))
         self.parentframe.emit_event("<<SheetModified>>")
 
     def find_last_selected_box_with_current(self, currently_selected):
         if currently_selected.type_ in ("cell", "column"):
             boxes, maxrows = self.get_ctrl_x_c_boxes()
         else:
             boxes = self.get_ctrl_x_c_boxes()
-        return self.find_last_selected_box_with_current_from_boxes(
-            currently_selected, boxes
-        )
+        return self.find_last_selected_box_with_current_from_boxes(currently_selected, boxes)
 
     def find_last_selected_box_with_current_from_boxes(self, currently_selected, boxes):
         for (r1, c1, r2, c2), type_ in boxes.items():
             if (
                 type_[:2] == currently_selected.type_[:2]
                 and currently_selected.row >= r1
                 and currently_selected.row <= r2
                 and currently_selected.column >= c1
                 and currently_selected.column <= c2
             ):
-                if (
-                    self.last_selected and self.last_selected == (r1, c1, r2, c2, type_)
-                ) or not self.last_selected:
+                if (self.last_selected and self.last_selected == (r1, c1, r2, c2, type_)) or not self.last_selected:
                     return (r1, c1, r2, c2)
         return (
             currently_selected.row,
             currently_selected.column,
             currently_selected.row + 1,
             currently_selected.column + 1,
         )
 
     def ctrl_v(self, event=None):
-        if not self.expand_sheet_if_paste_too_big and (
-            len(self.col_positions) == 1 or len(self.row_positions) == 1
-        ):
+        if not self.expand_sheet_if_paste_too_big and (len(self.col_positions) == 1 or len(self.row_positions) == 1):
             return
         currently_selected = self.currently_selected()
         if currently_selected:
             selected_r = currently_selected[0]
             selected_c = currently_selected[1]
         elif not currently_selected and not self.expand_sheet_if_paste_too_big:
             return
@@ -754,22 +660,18 @@
                 elif len(self.row_positions) > 1 and len(self.col_positions) > 1:
                     selected_c, selected_r = 0, len(self.row_positions) - 1
         try:
             data = self.clipboard_get()
         except Exception:
             return
         try:
-            dialect = csv.Sniffer().sniff(
-                data, delimiters=self.from_clipboard_delimiters
-            )
+            dialect = csv.Sniffer().sniff(data, delimiters=self.from_clipboard_delimiters)
         except Exception:
             dialect = csv.excel_tab
-        data = list(
-            csv.reader(io.StringIO(data), dialect=dialect, skipinitialspace=True)
-        )
+        data = list(csv.reader(io.StringIO(data), dialect=dialect, skipinitialspace=True))
         if not data:
             return
         numcols = len(max(data, key=len))
         numrows = len(data)
         for rn, r in enumerate(data):
             if len(r) < numcols:
                 data[rn].extend(list(repeat("", numcols - len(r))))
@@ -796,79 +698,59 @@
         if self.expand_sheet_if_paste_too_big:
             added_rows = 0
             added_cols = 0
             if selected_c + numcols > len(self.col_positions) - 1:
                 added_cols = selected_c + numcols - len(self.col_positions) + 1
                 if (
                     isinstance(self.paste_insert_column_limit, int)
-                    and self.paste_insert_column_limit
-                    < len(self.col_positions) - 1 + added_cols
+                    and self.paste_insert_column_limit < len(self.col_positions) - 1 + added_cols
                 ):
-                    added_cols = (
-                        self.paste_insert_column_limit - len(self.col_positions) - 1
-                    )
+                    added_cols = self.paste_insert_column_limit - len(self.col_positions) - 1
                 if added_cols > 0:
                     self.insert_col_positions(widths=int(added_cols))
                 if not self.all_columns_displayed:
                     total_data_cols = self.total_data_cols()
-                    self.displayed_columns.extend(
-                        list(range(total_data_cols, total_data_cols + added_cols))
-                    )
+                    self.displayed_columns.extend(list(range(total_data_cols, total_data_cols + added_cols)))
             if selected_r + numrows > len(self.row_positions) - 1:
                 added_rows = selected_r + numrows - len(self.row_positions) + 1
                 if (
                     isinstance(self.paste_insert_row_limit, int)
-                    and self.paste_insert_row_limit
-                    < len(self.row_positions) - 1 + added_rows
+                    and self.paste_insert_row_limit < len(self.row_positions) - 1 + added_rows
                 ):
-                    added_rows = (
-                        self.paste_insert_row_limit - len(self.row_positions) - 1
-                    )
+                    added_rows = self.paste_insert_row_limit - len(self.row_positions) - 1
                 if added_rows > 0:
                     self.insert_row_positions(heights=int(added_rows))
                 if not self.all_rows_displayed:
                     total_data_rows = self.total_data_rows()
-                    self.displayed_rows.extend(
-                        list(range(total_data_rows, total_data_rows + added_rows))
-                    )
+                    self.displayed_rows.extend(list(range(total_data_rows, total_data_rows + added_rows)))
             added_rows_cols = (added_rows, added_cols)
         else:
             added_rows_cols = (0, 0)
         if selected_c + numcols > len(self.col_positions) - 1:
             numcols = len(self.col_positions) - 1 - selected_c
         if selected_r + numrows > len(self.row_positions) - 1:
             numrows = len(self.row_positions) - 1 - selected_r
-        if (
-            self.extra_begin_ctrl_v_func is not None
-            or self.extra_end_ctrl_v_func is not None
-        ):
+        if self.extra_begin_ctrl_v_func is not None or self.extra_end_ctrl_v_func is not None:
             rows = [
-                [
-                    data[ndr][ndc]
-                    for ndc, c in enumerate(range(selected_c, selected_c + numcols))
-                ]
+                [data[ndr][ndc] for ndc, c in enumerate(range(selected_c, selected_c + numcols))]
                 for ndr, r in enumerate(range(selected_r, selected_r + numrows))
             ]
         if self.extra_begin_ctrl_v_func is not None:
             try:
-                self.extra_begin_ctrl_v_func(
-                    PasteEvent("begin_ctrl_v", currently_selected, rows)
-                )
+                self.extra_begin_ctrl_v_func(PasteEvent("begin_ctrl_v", currently_selected, rows))
             except Exception:
                 return
         changes = 0
         for ndr, r in enumerate(range(selected_r, selected_r + numrows)):
             datarn = r if self.all_rows_displayed else self.displayed_rows[r]
             for ndc, c in enumerate(range(selected_c, selected_c + numcols)):
                 datacn = c if self.all_columns_displayed else self.displayed_columns[c]
                 if self.input_valid_for_cell(datarn, datacn, data[ndr][ndc]):
                     if self.undo_enabled:
-                        undo_storage[(datarn, datacn)] = self.get_cell_data(
-                            datarn, datacn
-                        )
+                        undo_storage[(datarn, datacn)] = self.get_cell_data(datarn, datacn)
                     self.set_cell_data(datarn, datacn, data[ndr][ndc])
                     changes += 1
         if self.expand_sheet_if_paste_too_big and self.undo_enabled:
             self.equalize_data_row_lengths()
         self.deselect("all")
         if changes and self.undo_enabled:
             self.undo_storage.append(
@@ -887,32 +769,28 @@
                             },  # boxes
                             currently_selected,
                             added_rows_cols,
                         )
                     )
                 )
             )
-        self.create_selected(
-            selected_r, selected_c, selected_r + numrows, selected_c + numcols, "cells"
-        )
+        self.create_selected(selected_r, selected_c, selected_r + numrows, selected_c + numcols, "cells")
         self.set_currently_selected(selected_r, selected_c, type_="cell")
         self.see(
             r=selected_r,
             c=selected_c,
             keep_yscroll=False,
             keep_xscroll=False,
             bottom_right_corner=False,
             check_cell_visibility=True,
             redraw=False,
         )
         self.refresh()
         if self.extra_end_ctrl_v_func is not None:
-            self.extra_end_ctrl_v_func(
-                PasteEvent("end_ctrl_v", currently_selected, rows)
-            )
+            self.extra_end_ctrl_v_func(PasteEvent("end_ctrl_v", currently_selected, rows))
         self.parentframe.emit_event("<<SheetModified>>")
 
     def delete_key(self, event=None):
         if not self.anything_selected():
             return
         currently_selected = self.currently_selected()
         undo_storage = {}
@@ -923,45 +801,33 @@
             self.find_withtag("columns"),
         ):
             alltags = self.gettags(item)
             box = tuple(int(e) for e in alltags[1].split("_") if e)
             boxes[box] = alltags[0]
         if self.extra_begin_delete_key_func is not None:
             try:
-                self.extra_begin_delete_key_func(
-                    CtrlKeyEvent("begin_delete_key", boxes, currently_selected, tuple())
-                )
+                self.extra_begin_delete_key_func(CtrlKeyEvent("begin_delete_key", boxes, currently_selected, tuple()))
             except Exception:
                 return
         changes = 0
         for r1, c1, r2, c2 in boxes:
             for r in range(r1, r2):
                 datarn = r if self.all_rows_displayed else self.displayed_rows[r]
                 for c in range(c1, c2):
-                    datacn = (
-                        c if self.all_columns_displayed else self.displayed_columns[c]
-                    )
+                    datacn = c if self.all_columns_displayed else self.displayed_columns[c]
                     if self.input_valid_for_cell(datarn, datacn, ""):
                         if self.undo_enabled:
-                            undo_storage[(datarn, datacn)] = self.get_cell_data(
-                                datarn, datacn
-                            )
+                            undo_storage[(datarn, datacn)] = self.get_cell_data(datarn, datacn)
                         self.set_cell_data(datarn, datacn, "")
                         changes += 1
         if self.extra_end_delete_key_func is not None:
-            self.extra_end_delete_key_func(
-                CtrlKeyEvent("end_delete_key", boxes, currently_selected, undo_storage)
-            )
+            self.extra_end_delete_key_func(CtrlKeyEvent("end_delete_key", boxes, currently_selected, undo_storage))
         if changes and self.undo_enabled:
             self.undo_storage.append(
-                zlib.compress(
-                    pickle.dumps(
-                        ("edit_cells", undo_storage, boxes, currently_selected)
-                    )
-                )
+                zlib.compress(pickle.dumps(("edit_cells", undo_storage, boxes, currently_selected)))
             )
         self.refresh()
         self.parentframe.emit_event("<<SheetModified>>")
 
     def move_columns_adjust_options_dict(
         self,
         col,
@@ -1006,17 +872,15 @@
                         len(self.col_positions) - 1,
                         "columns",
                     )
             else:
                 if to_move_min > c:
                     new_selected = tuple(range(c, c + num_cols))
                     if create_selections:
-                        self.create_selected(
-                            0, c, len(self.row_positions) - 1, c + num_cols, "columns"
-                        )
+                        self.create_selected(0, c, len(self.row_positions) - 1, c + num_cols, "columns")
                 else:
                     new_selected = tuple(range(c + 1 - num_cols, c + 1))
                     if create_selections:
                         self.create_selected(
                             0,
                             c + 1 - num_cols,
                             len(self.row_positions) - 1,
@@ -1040,35 +904,27 @@
                         self.data[rn][c:c] = self.data[rn][to_move_min:to_move_max]
                         self.data[rn][to_move_max:to_del] = []
                     self.CH.fix_header(extend_idx)
                     if isinstance(self._headers, list) and self._headers:
                         self._headers[c:c] = self._headers[to_move_min:to_move_max]
                         self._headers[to_move_max:to_del] = []
                 self.CH.cell_options = {
-                    newcolsdct[k]
-                    if k in newcolsdct
-                    else k + num_cols
-                    if k < to_move_min and k >= c
-                    else k: v
+                    newcolsdct[k] if k in newcolsdct else k + num_cols if k < to_move_min and k >= c else k: v
                     for k, v in self.CH.cell_options.items()
                 }
                 self.cell_options = {
                     (k[0], newcolsdct[k[1]])
                     if k[1] in newcolsdct
                     else (k[0], k[1] + num_cols)
                     if k[1] < to_move_min and k[1] >= c
                     else k: v
                     for k, v in self.cell_options.items()
                 }
                 self.col_options = {
-                    newcolsdct[k]
-                    if k in newcolsdct
-                    else k + num_cols
-                    if k < to_move_min and k >= c
-                    else k: v
+                    newcolsdct[k] if k in newcolsdct else k + num_cols if k < to_move_min and k >= c else k: v
                     for k, v in self.col_options.items()
                 }
                 if index_type != "displayed":
                     self.displayed_columns = sorted(
                         int(newcolsdct[k])
                         if k in newcolsdct
                         else k + num_cols
@@ -1086,75 +942,59 @@
                         self.data[rn][c:c] = self.data[rn][to_move_min:to_move_max]
                         self.data[rn][to_move_min:to_move_max] = []
                     self.CH.fix_header(extend_idx)
                     if isinstance(self._headers, list) and self._headers:
                         self._headers[c:c] = self._headers[to_move_min:to_move_max]
                         self._headers[to_move_min:to_move_max] = []
                 self.CH.cell_options = {
-                    newcolsdct[k]
-                    if k in newcolsdct
-                    else k - num_cols
-                    if k < c and k > to_move_min
-                    else k: v
+                    newcolsdct[k] if k in newcolsdct else k - num_cols if k < c and k > to_move_min else k: v
                     for k, v in self.CH.cell_options.items()
                 }
                 self.cell_options = {
                     (k[0], newcolsdct[k[1]])
                     if k[1] in newcolsdct
                     else (k[0], k[1] - num_cols)
                     if k[1] < c and k[1] > to_move_min
                     else k: v
                     for k, v in self.cell_options.items()
                 }
                 self.col_options = {
-                    newcolsdct[k]
-                    if k in newcolsdct
-                    else k - num_cols
-                    if k < c and k > to_move_min
-                    else k: v
+                    newcolsdct[k] if k in newcolsdct else k - num_cols if k < c and k > to_move_min else k: v
                     for k, v in self.col_options.items()
                 }
                 if index_type != "displayed":
                     self.displayed_columns = sorted(
-                        int(newcolsdct[k])
-                        if k in newcolsdct
-                        else k - num_cols
-                        if k < c and k > to_move_min
-                        else int(k)
+                        int(newcolsdct[k]) if k in newcolsdct else k - num_cols if k < c and k > to_move_min else int(k)
                         for k in self.displayed_columns
                     )
         else:
             # moves data around, not displayed columns indexes
             # which remain sorted and the same after drop and drop
             if to_move_min > c:
                 dispset = {
                     a: b
                     for a, b in zip(
                         self.displayed_columns,
                         (
                             self.displayed_columns[:c]
-                            + self.displayed_columns[
-                                to_move_min : to_move_min + num_cols
-                            ]
+                            + self.displayed_columns[to_move_min : to_move_min + num_cols]
                             + self.displayed_columns[c:to_move_min]
                             + self.displayed_columns[to_move_min + num_cols :]
                         ),
                     )
                 }
             else:
                 dispset = {
                     a: b
                     for a, b in zip(
                         self.displayed_columns,
                         (
                             self.displayed_columns[:to_move_min]
                             + self.displayed_columns[to_move_min + num_cols : c + 1]
-                            + self.displayed_columns[
-                                to_move_min : to_move_min + num_cols
-                            ]
+                            + self.displayed_columns[to_move_min : to_move_min + num_cols]
                             + self.displayed_columns[c + 1 :]
                         ),
                     )
                 }
             # has to pick up elements from all over the place in the original row
             # building an entirely new row is best due to permutations of hidden columns
             if move_data:
@@ -1188,26 +1028,19 @@
                         elif idx not in done:
                             new.append(self._headers[idx])
                             idx += 1
                         else:
                             idx += 1
                     self._headers = new
                 dispset = {b: a for a, b in dispset.items()}
-                self.CH.cell_options = {
-                    dispset[k] if k in dispset else k: v
-                    for k, v in self.CH.cell_options.items()
-                }
+                self.CH.cell_options = {dispset[k] if k in dispset else k: v for k, v in self.CH.cell_options.items()}
                 self.cell_options = {
-                    (k[0], dispset[k[1]]) if k[1] in dispset else k: v
-                    for k, v in self.cell_options.items()
-                }
-                self.col_options = {
-                    dispset[k] if k in dispset else k: v
-                    for k, v in self.col_options.items()
+                    (k[0], dispset[k[1]]) if k[1] in dispset else k: v for k, v in self.cell_options.items()
                 }
+                self.col_options = {dispset[k] if k in dispset else k: v for k, v in self.col_options.items()}
         return new_selected, {b: a for a, b in dispset.items()}
 
     def move_rows_adjust_options_dict(
         self,
         row,
         to_move_min,
         num_rows,
@@ -1230,17 +1063,15 @@
             ]
             if to_move_min > r:
                 rhs[r:r] = rhs[to_move_min:to_move_max]
                 rhs[to_move_max:to_del] = []
             else:
                 rhs[r + 1 : r + 1] = rhs[to_move_min:to_move_max]
                 rhs[to_move_min:to_move_max] = []
-            self.row_positions = list(
-                accumulate(chain([0], (height for height in rhs)))
-            )
+            self.row_positions = list(accumulate(chain([0], (height for height in rhs))))
             if r + num_rows > len(self.row_positions):
                 new_selected = tuple(
                     range(
                         len(self.row_positions) - 1 - num_rows,
                         len(self.row_positions) - 1,
                     )
                 )
@@ -1252,17 +1083,15 @@
                         len(self.col_positions) - 1,
                         "rows",
                     )
             else:
                 if to_move_min > r:
                     new_selected = tuple(range(r, r + num_rows))
                     if create_selections:
-                        self.create_selected(
-                            r, 0, r + num_rows, len(self.col_positions) - 1, "rows"
-                        )
+                        self.create_selected(r, 0, r + num_rows, len(self.col_positions) - 1, "rows")
                 else:
                     new_selected = tuple(range(r + 1 - num_rows, r + 1))
                     if create_selections:
                         self.create_selected(
                             r + 1 - num_rows,
                             0,
                             r + 1,
@@ -1285,35 +1114,27 @@
                     self.data[r:r] = self.data[to_move_min:to_move_max]
                     self.data[to_move_max:to_del] = []
                     self.RI.fix_index(extend_idx)
                     if isinstance(self._row_index, list) and self._row_index:
                         self._row_index[r:r] = self._row_index[to_move_min:to_move_max]
                         self._row_index[to_move_max:to_del] = []
                 self.RI.cell_options = {
-                    newrowsdct[k]
-                    if k in newrowsdct
-                    else k + num_rows
-                    if k < to_move_min and k >= r
-                    else k: v
+                    newrowsdct[k] if k in newrowsdct else k + num_rows if k < to_move_min and k >= r else k: v
                     for k, v in self.RI.cell_options.items()
                 }
                 self.cell_options = {
                     (newrowsdct[k[0]], k[1])
                     if k[0] in newrowsdct
                     else (k[0] + num_rows, k[1])
                     if k[0] < to_move_min and k[0] >= r
                     else k: v
                     for k, v in self.cell_options.items()
                 }
                 self.row_options = {
-                    newrowsdct[k]
-                    if k in newrowsdct
-                    else k + num_rows
-                    if k < to_move_min and k >= r
-                    else k: v
+                    newrowsdct[k] if k in newrowsdct else k + num_rows if k < to_move_min and k >= r else k: v
                     for k, v in self.row_options.items()
                 }
                 if index_type != "displayed":
                     self.displayed_rows = sorted(
                         int(newrowsdct[k])
                         if k in newrowsdct
                         else k + num_rows
@@ -1330,44 +1151,32 @@
                     self.data[r:r] = self.data[to_move_min:to_move_max]
                     self.data[to_move_min:to_move_max] = []
                     self.RI.fix_index(extend_idx)
                     if isinstance(self._row_index, list) and self._row_index:
                         self._row_index[r:r] = self._row_index[to_move_min:to_move_max]
                         self._row_index[to_move_min:to_move_max] = []
                 self.RI.cell_options = {
-                    newrowsdct[k]
-                    if k in newrowsdct
-                    else k - num_rows
-                    if k < r and k > to_move_min
-                    else k: v
+                    newrowsdct[k] if k in newrowsdct else k - num_rows if k < r and k > to_move_min else k: v
                     for k, v in self.RI.cell_options.items()
                 }
                 self.cell_options = {
                     (newrowsdct[k[0]], k[1])
                     if k[0] in newrowsdct
                     else (k[0] - num_rows, k[1])
                     if k[0] < r and k[0] > to_move_min
                     else k: v
                     for k, v in self.cell_options.items()
                 }
                 self.row_options = {
-                    newrowsdct[k]
-                    if k in newrowsdct
-                    else k - num_rows
-                    if k < r and k > to_move_min
-                    else k: v
+                    newrowsdct[k] if k in newrowsdct else k - num_rows if k < r and k > to_move_min else k: v
                     for k, v in self.row_options.items()
                 }
                 if index_type != "displayed":
                     self.displayed_rows = sorted(
-                        int(newrowsdct[k])
-                        if k in newrowsdct
-                        else k - num_rows
-                        if k < r and k > to_move_min
-                        else int(k)
+                        int(newrowsdct[k]) if k in newrowsdct else k - num_rows if k < r and k > to_move_min else int(k)
                         for k in self.displayed_rows
                     )
         else:
             # moves data around, not displayed rows indexes
             # which remain sorted and the same after drop and drop
             if to_move_min > r:
                 dispset = {
@@ -1426,41 +1235,32 @@
                         elif idx not in done:
                             new.append(self._row_index[idx])
                             idx += 1
                         else:
                             idx += 1
                     self._row_index = new
                 dispset = {b: a for a, b in dispset.items()}
-                self.RI.cell_options = {
-                    dispset[k] if k in dispset else k: v
-                    for k, v in self.RI.cell_options.items()
-                }
+                self.RI.cell_options = {dispset[k] if k in dispset else k: v for k, v in self.RI.cell_options.items()}
                 self.cell_options = {
-                    (dispset[k[0]], k[1]) if k[0] in dispset else k: v
-                    for k, v in self.cell_options.items()
-                }
-                self.row_options = {
-                    dispset[k] if k in dispset else k: v
-                    for k, v in self.row_options.items()
+                    (dispset[k[0]], k[1]) if k[0] in dispset else k: v for k, v in self.cell_options.items()
                 }
+                self.row_options = {dispset[k] if k in dispset else k: v for k, v in self.row_options.items()}
         return new_selected, {b: a for a, b in dispset.items()}
 
     def ctrl_z(self, event=None):
         if not self.undo_storage:
             return
         if not isinstance(self.undo_storage[-1], (tuple, dict)):
             undo_storage = pickle.loads(zlib.decompress(self.undo_storage[-1]))
         else:
             undo_storage = self.undo_storage[-1]
         self.deselect("all")
         if self.extra_begin_ctrl_z_func is not None:
             try:
-                self.extra_begin_ctrl_z_func(
-                    UndoEvent("begin_ctrl_z", undo_storage[0], undo_storage)
-                )
+                self.extra_begin_ctrl_z_func(UndoEvent("begin_ctrl_z", undo_storage[0], undo_storage))
             except Exception:
                 return
         self.undo_storage.pop()
         if undo_storage[0] in ("edit_header",):
             for c, v in undo_storage[1].items():
                 self._headers[c] = v
             self.reselect_from_get_boxes(undo_storage[2])
@@ -1473,55 +1273,40 @@
             self.set_currently_selected(0, undo_storage[3][1], type_="row")
 
         if undo_storage[0] in ("edit_cells", "edit_cells_paste"):
             for (datarn, datacn), v in undo_storage[1].items():
                 self.set_cell_data(datarn, datacn, v)
             start_row = float("inf")
             start_col = float("inf")
-            if (
-                undo_storage[0] == "edit_cells_paste"
-                and self.expand_sheet_if_paste_too_big
-            ):
+            if undo_storage[0] == "edit_cells_paste" and self.expand_sheet_if_paste_too_big:
                 if undo_storage[4][0] > 0:
                     self.del_row_positions(
                         len(self.row_positions) - 1 - undo_storage[4][0],
                         undo_storage[4][0],
                     )
                     self.data[:] = self.data[: -undo_storage[4][0]]
                     if not self.all_rows_displayed:
-                        self.displayed_rows[:] = self.displayed_rows[
-                            : -undo_storage[4][0]
-                        ]
+                        self.displayed_rows[:] = self.displayed_rows[: -undo_storage[4][0]]
                 if undo_storage[4][1] > 0:
                     quick_added_cols = undo_storage[4][1]
-                    self.del_col_positions(
-                        len(self.col_positions) - 1 - quick_added_cols, quick_added_cols
-                    )
+                    self.del_col_positions(len(self.col_positions) - 1 - quick_added_cols, quick_added_cols)
                     for rn in range(len(self.data)):
                         self.data[rn][:] = self.data[rn][:-quick_added_cols]
                     if not self.all_columns_displayed:
-                        self.displayed_columns[:] = self.displayed_columns[
-                            :-quick_added_cols
-                        ]
+                        self.displayed_columns[:] = self.displayed_columns[:-quick_added_cols]
             self.reselect_from_get_boxes(undo_storage[2])
             if undo_storage[3]:
                 self.set_currently_selected(
                     undo_storage[3].row,
                     undo_storage[3].column,
                     type_=undo_storage[3].type_,
                 )
-            elif (
-                start_row < len(self.row_positions) - 1
-                and start_col < len(self.col_positions) - 1
-            ):
+            elif start_row < len(self.row_positions) - 1 and start_col < len(self.col_positions) - 1:
                 self.set_currently_selected(start_row, start_col, type_="cell")
-            if (
-                start_row < len(self.row_positions) - 1
-                and start_col < len(self.col_positions) - 1
-            ):
+            if start_row < len(self.row_positions) - 1 and start_col < len(self.col_positions) - 1:
                 self.see(
                     r=start_row,
                     c=start_col,
                     keep_yscroll=False,
                     keep_xscroll=False,
                     bottom_right_corner=False,
                     check_cell_visibility=True,
@@ -1561,21 +1346,19 @@
                 check_cell_visibility=True,
                 redraw=False,
             )
 
         elif undo_storage[0] == "insert_rows":
             self.displayed_rows = undo_storage[1]["displayed_rows"]
             self.data[
-                undo_storage[1]["data_row_num"] : undo_storage[1]["data_row_num"]
-                + undo_storage[1]["numrows"]
+                undo_storage[1]["data_row_num"] : undo_storage[1]["data_row_num"] + undo_storage[1]["numrows"]
             ] = []
             try:
                 self._row_index[
-                    undo_storage[1]["data_row_num"] : undo_storage[1]["data_row_num"]
-                    + undo_storage[1]["numrows"]
+                    undo_storage[1]["data_row_num"] : undo_storage[1]["data_row_num"] + undo_storage[1]["numrows"]
                 ] = []
             except Exception:
                 pass
             self.del_row_positions(
                 undo_storage[1]["sheet_row_num"],
                 undo_storage[1]["numrows"],
                 deselect_all=False,
@@ -1590,22 +1373,18 @@
             idx = undo_storage[1]["sheet_row_num"] + undo_storage[1]["numrows"]
             self.cell_options = {
                 (rn if rn < idx else rn - numrows, cn): t2
                 for (rn, cn), t2 in self.cell_options.items()
                 if rn not in to_del
             }
             self.row_options = {
-                rn if rn < idx else rn - numrows: t
-                for rn, t in self.row_options.items()
-                if rn not in to_del
+                rn if rn < idx else rn - numrows: t for rn, t in self.row_options.items() if rn not in to_del
             }
             self.RI.cell_options = {
-                rn if rn < idx else rn - numrows: t
-                for rn, t in self.RI.cell_options.items()
-                if rn not in to_del
+                rn if rn < idx else rn - numrows: t for rn, t in self.RI.cell_options.items() if rn not in to_del
             }
             if len(self.row_positions) > 1:
                 start_row = (
                     undo_storage[1]["sheet_row_num"]
                     if undo_storage[1]["sheet_row_num"] < len(self.row_positions) - 1
                     else undo_storage[1]["sheet_row_num"] - 1
                 )
@@ -1645,22 +1424,18 @@
             idx = undo_storage[1]["sheet_col_num"] + undo_storage[1]["numcols"]
             self.cell_options = {
                 (rn, cn if cn < idx else cn - numcols): t2
                 for (rn, cn), t2 in self.cell_options.items()
                 if cn not in to_del
             }
             self.col_options = {
-                cn if cn < idx else cn - numcols: t
-                for cn, t in self.col_options.items()
-                if cn not in to_del
+                cn if cn < idx else cn - numcols: t for cn, t in self.col_options.items() if cn not in to_del
             }
             self.CH.cell_options = {
-                cn if cn < idx else cn - numcols: t
-                for cn, t in self.CH.cell_options.items()
-                if cn not in to_del
+                cn if cn < idx else cn - numcols: t for cn, t in self.CH.cell_options.items() if cn not in to_del
             }
             if len(self.col_positions) > 1:
                 start_col = (
                     undo_storage[1]["sheet_col_num"]
                     if undo_storage[1]["sheet_col_num"] < len(self.col_positions) - 1
                     else undo_storage[1]["sheet_col_num"] - 1
                 )
@@ -1700,27 +1475,23 @@
                 self.insert_col_position(idx=cn, width=w)
             for cn, rowdict in reversed(tuple(undo_storage[1]["deleted_cols"].items())):
                 for rn, v in rowdict.items():
                     try:
                         self.data[rn].insert(cn, v)
                     except Exception:
                         continue
-            for cn, v in reversed(
-                tuple(undo_storage[1]["deleted_header_values"].items())
-            ):
+            for cn, v in reversed(tuple(undo_storage[1]["deleted_header_values"].items())):
                 try:
                     self._headers.insert(cn, v)
                 except Exception:
                     continue
             self.reselect_from_get_boxes(undo_storage[1]["selection_boxes"])
         self.refresh()
         if self.extra_end_ctrl_z_func is not None:
-            self.extra_end_ctrl_z_func(
-                UndoEvent("end_ctrl_z", undo_storage[0], undo_storage)
-            )
+            self.extra_end_ctrl_z_func(UndoEvent("end_ctrl_z", undo_storage[0], undo_storage))
         self.parentframe.emit_event("<<SheetModified>>")
 
     def bind_arrowkeys(self, keys: dict = {}):
         for canvas in (self, self.parentframe, self.CH, self.RI, self.TL):
             for k, func in keys.items():
                 canvas.bind(f"<{arrowkey_bindings_helper[k.lower()]}>", func)
 
@@ -1761,16 +1532,15 @@
                     self.yview(*args)
                     self.RI.yview(*args)
                     need_redraw = True
             else:
                 if r is not None and not keep_yscroll:
                     args = (
                         "moveto",
-                        self.row_positions[r]
-                        / (self.row_positions[-1] + self.empty_vertical),
+                        self.row_positions[r] / (self.row_positions[-1] + self.empty_vertical),
                     )
                     if args[1] > 1:
                         args[1] = args[1] - 1
                     self.yview(*args)
                     self.RI.yview(*args)
                     need_redraw = True
         if not xvis:
@@ -1788,24 +1558,21 @@
                     self.xview(*args)
                     self.CH.xview(*args)
                     need_redraw = True
             else:
                 if c is not None and not keep_xscroll:
                     args = (
                         "moveto",
-                        self.col_positions[c]
-                        / (self.col_positions[-1] + self.empty_horizontal),
+                        self.col_positions[c] / (self.col_positions[-1] + self.empty_horizontal),
                     )
                     self.xview(*args)
                     self.CH.xview(*args)
                     need_redraw = True
         if redraw and need_redraw:
-            self.main_table_redraw_grid_and_text(
-                redraw_header=True, redraw_row_index=True
-            )
+            self.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=True)
             return True
         else:
             return False
 
     def get_cell_coords(self, r=None, c=None):
         return (
             0 if not c else self.col_positions[c] + 1,
@@ -1839,26 +1606,20 @@
         return False
 
     def select_all(self, redraw=True, run_binding_func=True):
         currently_selected = self.currently_selected()
         self.deselect("all")
         if len(self.row_positions) > 1 and len(self.col_positions) > 1:
             if currently_selected:
-                self.set_currently_selected(
-                    currently_selected.row, currently_selected.column, type_="cell"
-                )
+                self.set_currently_selected(currently_selected.row, currently_selected.column, type_="cell")
             else:
                 self.set_currently_selected(0, 0, type_="cell")
-            self.create_selected(
-                0, 0, len(self.row_positions) - 1, len(self.col_positions) - 1
-            )
+            self.create_selected(0, 0, len(self.row_positions) - 1, len(self.col_positions) - 1)
             if redraw:
-                self.main_table_redraw_grid_and_text(
-                    redraw_header=True, redraw_row_index=True
-                )
+                self.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=True)
             if self.select_all_binding_func is not None and run_binding_func:
                 self.select_all_binding_func(
                     SelectionBoxEvent(
                         "select_all_cells",
                         (
                             0,
                             0,
@@ -1869,30 +1630,24 @@
                 )
 
     def select_cell(self, r, c, redraw=False):
         self.delete_selection_rects()
         self.create_selected(r, c, r + 1, c + 1, state="hidden")
         self.set_currently_selected(r, c, type_="cell")
         if redraw:
-            self.main_table_redraw_grid_and_text(
-                redraw_header=True, redraw_row_index=True
-            )
+            self.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=True)
         if self.selection_binding_func is not None:
             self.selection_binding_func(SelectCellEvent("select_cell", r, c))
 
-    def add_selection(
-        self, r, c, redraw=False, run_binding_func=True, set_as_current=False
-    ):
+    def add_selection(self, r, c, redraw=False, run_binding_func=True, set_as_current=False):
         self.create_selected(r, c, r + 1, c + 1, state="hidden")
         if set_as_current:
             self.set_currently_selected(r, c, type_="cell")
         if redraw:
-            self.main_table_redraw_grid_and_text(
-                redraw_header=True, redraw_row_index=True
-            )
+            self.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=True)
         if self.selection_binding_func is not None and run_binding_func:
             self.selection_binding_func(SelectCellEvent("select_cell", r, c))
 
     def toggle_select_cell(
         self,
         row,
         column,
@@ -1914,17 +1669,15 @@
                 )
         else:
             if self.cell_selected(row, column, inc_rows=True, inc_cols=True):
                 self.deselect(r=row, c=column, redraw=redraw)
             else:
                 self.select_cell(row, column, redraw=redraw)
 
-    def align_rows(
-        self, rows=[], align="global", align_index=False
-    ):  # "center", "w", "e" or "global"
+    def align_rows(self, rows=[], align="global", align_index=False):  # "center", "w", "e" or "global"
         if isinstance(rows, str) and rows.lower() == "all" and align == "global":
             for r in self.row_options:
                 if "align" in self.row_options[r]:
                     del self.row_options[r]["align"]
             if align_index:
                 for r in self.RI.cell_options:
                     if r in self.RI.cell_options and "align" in self.RI.cell_options[r]:
@@ -1936,33 +1689,27 @@
             rows_ = (r for r in range(self.total_data_rows()))
         else:
             rows_ = rows
         if align == "global":
             for r in rows_:
                 if r in self.row_options and "align" in self.row_options[r]:
                     del self.row_options[r]["align"]
-                if (
-                    align_index
-                    and r in self.RI.cell_options
-                    and "align" in self.RI.cell_options[r]
-                ):
+                if align_index and r in self.RI.cell_options and "align" in self.RI.cell_options[r]:
                     del self.RI.cell_options[r]["align"]
         else:
             for r in rows_:
                 if r not in self.row_options:
                     self.row_options[r] = {}
                 self.row_options[r]["align"] = align
                 if align_index:
                     if r not in self.RI.cell_options:
                         self.RI.cell_options[r] = {}
                     self.RI.cell_options[r]["align"] = align
 
-    def align_columns(
-        self, columns=[], align="global", align_header=False
-    ):  # "center", "w", "e" or "global"
+    def align_columns(self, columns=[], align="global", align_header=False):  # "center", "w", "e" or "global"
         if isinstance(columns, str) and columns.lower() == "all" and align == "global":
             for c in self.col_options:
                 if "align" in self.col_options[c]:
                     del self.col_options[c]["align"]
             if align_header:
                 for c in self.CH.cell_options:
                     if c in self.CH.cell_options and "align" in self.CH.cell_options[c]:
@@ -1974,49 +1721,39 @@
             cols_ = (c for c in range(self.total_data_cols()))
         else:
             cols_ = columns
         if align == "global":
             for c in cols_:
                 if c in self.col_options and "align" in self.col_options[c]:
                     del self.col_options[c]["align"]
-                if (
-                    align_header
-                    and c in self.CH.cell_options
-                    and "align" in self.CH.cell_options[c]
-                ):
+                if align_header and c in self.CH.cell_options and "align" in self.CH.cell_options[c]:
                     del self.CH.cell_options[c]["align"]
         else:
             for c in cols_:
                 if c not in self.col_options:
                     self.col_options[c] = {}
                 self.col_options[c]["align"] = align
                 if align_header:
                     if c not in self.CH.cell_options:
                         self.CH.cell_options[c] = {}
                     self.CH.cell_options[c]["align"] = align
 
-    def align_cells(
-        self, row=0, column=0, cells=[], align="global"
-    ):  # "center", "w", "e" or "global"
+    def align_cells(self, row=0, column=0, cells=[], align="global"):  # "center", "w", "e" or "global"
         if isinstance(row, str) and row.lower() == "all" and align == "global":
             for r, c in self.cell_options:
                 if "align" in self.cell_options[(r, c)]:
                     del self.cell_options[(r, c)]["align"]
             return
         if align == "global":
             if cells:
                 for r, c in cells:
-                    if (r, c) in self.cell_options and "align" in self.cell_options[
-                        (r, c)
-                    ]:
+                    if (r, c) in self.cell_options and "align" in self.cell_options[(r, c)]:
                         del self.cell_options[(r, c)]["align"]
             else:
-                if (row, column) in self.cell_options and "align" in self.cell_options[
-                    (row, column)
-                ]:
+                if (row, column) in self.cell_options and "align" in self.cell_options[(row, column)]:
                     del self.cell_options[(row, column)]["align"]
         else:
             if cells:
                 for r, c in cells:
                     if (r, c) not in self.cell_options:
                         self.cell_options[(r, c)] = {}
                     self.cell_options[(r, c)]["align"] = align
@@ -2037,42 +1774,36 @@
                     r1, c1, r2, c2 = tuple(int(e) for e in alltags[1].split("_") if e)
                     deleted_boxes[r1, c1, r2, c2] = "rows"
                     self.delete(alltags[1])
                     self.RI.delete(alltags[1])
                     self.CH.delete(alltags[1])
             current = self.currently_selected()
             if current and current.type_ == "row":
-                deleted_boxes[
-                    tuple(int(e) for e in self.get_tags_of_current()[1].split("_") if e)
-                ] = "cell"
+                deleted_boxes[tuple(int(e) for e in self.get_tags_of_current()[1].split("_") if e)] = "cell"
                 self.delete_current()
             deselected = ("deselect_all_rows", deleted_boxes)
         elif r == "allcols":
             for item in self.find_withtag("columns"):
                 alltags = self.gettags(item)
                 if alltags:
                     r1, c1, r2, c2 = tuple(int(e) for e in alltags[1].split("_") if e)
                     deleted_boxes[r1, c1, r2, c2] = "columns"
                     self.delete(alltags[1])
                     self.RI.delete(alltags[1])
                     self.CH.delete(alltags[1])
             current = self.currently_selected()
             if current and current.type_ == "column":
-                deleted_boxes[
-                    tuple(int(e) for e in self.get_tags_of_current()[1].split("_") if e)
-                ] = "cell"
+                deleted_boxes[tuple(int(e) for e in self.get_tags_of_current()[1].split("_") if e)] = "cell"
                 self.delete_current()
             deselected = ("deselect_all_cols", deleted_boxes)
         elif r is not None and c is None and cell is None:
             current = self.find_withtag("currently")
             current_tags = self.gettags(current[0]) if current else tuple()
             if current:
-                curr_r1, curr_c1, curr_r2, curr_c2 = tuple(
-                    int(e) for e in current_tags[1].split("_") if e
-                )
+                curr_r1, curr_c1, curr_r2, curr_c2 = tuple(int(e) for e in current_tags[1].split("_") if e)
             reset_current = False
             for item in self.find_withtag("rows"):
                 alltags = self.gettags(item)
                 if alltags:
                     r1, c1, r2, c2 = tuple(int(e) for e in alltags[1].split("_") if e)
                     if r >= r1 and r < r2:
                         self.delete(f"{r1}_{c1}_{r2}_{c2}")
@@ -2086,17 +1817,15 @@
                 self.delete_current()
                 self.set_current_to_last()
             deselected = ("deselect_row", deleted_boxes)
         elif c is not None and r is None and cell is None:
             current = self.find_withtag("currently")
             current_tags = self.gettags(current[0]) if current else tuple()
             if current:
-                curr_r1, curr_c1, curr_r2, curr_c2 = tuple(
-                    int(e) for e in current_tags[1].split("_") if e
-                )
+                curr_r1, curr_c1, curr_r2, curr_c2 = tuple(int(e) for e in current_tags[1].split("_") if e)
             reset_current = False
             for item in self.find_withtag("columns"):
                 alltags = self.gettags(item)
                 if alltags:
                     r1, c1, r2, c2 = tuple(int(e) for e in alltags[1].split("_") if e)
                     if c >= c1 and c < c2:
                         self.delete(f"{r1}_{c1}_{r2}_{c2}")
@@ -2131,43 +1860,30 @@
                             and r2 - r1 == 1
                             and c2 - c1 == 1
                             and r == current[0]
                             and c == current[1]
                         ):
                             set_curr = True
                         if current and not set_curr:
-                            if (
-                                current[0] >= r1
-                                and current[0] < r2
-                                and current[1] >= c1
-                                and current[1] < c2
-                            ):
+                            if current[0] >= r1 and current[0] < r2 and current[1] >= c1 and current[1] < c2:
                                 set_curr = True
                         self.delete(f"{r1}_{c1}_{r2}_{c2}")
                         self.RI.delete(f"{r1}_{c1}_{r2}_{c2}")
                         self.CH.delete(f"{r1}_{c1}_{r2}_{c2}")
                         deleted_boxes[(r1, c1, r2, c2)] = "cells"
             if set_curr:
                 try:
-                    deleted_boxes[
-                        tuple(
-                            int(e)
-                            for e in self.get_tags_of_current()[1].split("_")
-                            if e
-                        )
-                    ] = "cells"
+                    deleted_boxes[tuple(int(e) for e in self.get_tags_of_current()[1].split("_") if e)] = "cells"
                 except Exception:
                     pass
                 self.delete_current()
                 self.set_current_to_last()
             deselected = ("deselect_cell", deleted_boxes)
         if redraw:
-            self.main_table_redraw_grid_and_text(
-                redraw_header=True, redraw_row_index=True
-            )
+            self.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=True)
         if self.deselection_binding_func is not None:
             self.deselection_binding_func(DeselectionEvent(*deselected))
 
     def page_UP(self, event=None):
         height = self.winfo_height()
         top = self.canvasy(0)
         scrollto = top - height
@@ -2177,22 +1893,21 @@
             r = bisect.bisect_left(self.row_positions, scrollto)
             current = self.currently_selected()
             if current and current[0] == r:
                 r -= 1
             if r < 0:
                 r = 0
             if self.RI.row_selection_enabled and (
-                self.anything_selected(exclude_columns=True, exclude_cells=True)
-                or not self.anything_selected()
+                self.anything_selected(exclude_columns=True, exclude_cells=True) or not self.anything_selected()
             ):
                 self.RI.select_row(r)
                 self.see(r, 0, keep_xscroll=True, check_cell_visibility=False)
-            elif (
-                self.single_selection_enabled or self.toggle_selection_enabled
-            ) and self.anything_selected(exclude_columns=True, exclude_rows=True):
+            elif (self.single_selection_enabled or self.toggle_selection_enabled) and self.anything_selected(
+                exclude_columns=True, exclude_rows=True
+            ):
                 box = self.get_all_selection_boxes_with_types()[0][0]
                 self.see(r, box[1], keep_xscroll=True, check_cell_visibility=False)
                 self.select_cell(r, box[1])
         else:
             args = ("moveto", scrollto / (self.row_positions[-1] + 100))
             self.yview(*args)
             self.RI.yview(*args)
@@ -2206,22 +1921,21 @@
             r = bisect.bisect_left(self.row_positions, scrollto) - 1
             current = self.currently_selected()
             if current and current[0] == r:
                 r += 1
             if r > len(self.row_positions) - 2:
                 r = len(self.row_positions) - 2
             if self.RI.row_selection_enabled and (
-                self.anything_selected(exclude_columns=True, exclude_cells=True)
-                or not self.anything_selected()
+                self.anything_selected(exclude_columns=True, exclude_cells=True) or not self.anything_selected()
             ):
                 self.RI.select_row(r)
                 self.see(r, 0, keep_xscroll=True, check_cell_visibility=False)
-            elif (
-                self.single_selection_enabled or self.toggle_selection_enabled
-            ) and self.anything_selected(exclude_columns=True, exclude_rows=True):
+            elif (self.single_selection_enabled or self.toggle_selection_enabled) and self.anything_selected(
+                exclude_columns=True, exclude_rows=True
+            ):
                 box = self.get_all_selection_boxes_with_types()[0][0]
                 self.see(r, box[1], keep_xscroll=True, check_cell_visibility=False)
                 self.select_cell(r, box[1])
         else:
             end = self.row_positions[-1]
             if scrollto > end + 100:
                 scrollto = end
@@ -2244,17 +1958,15 @@
                     self.see(r - 1, 0, keep_xscroll=True, check_cell_visibility=False)
         elif currently_selected.type_ in ("cell", "column"):
             r = currently_selected[0]
             c = currently_selected[1]
             if r == 0 and self.CH.col_selection_enabled:
                 if not self.cell_completely_visible(r=r, c=0):
                     self.see(r, c, keep_xscroll=True, check_cell_visibility=False)
-            elif r != 0 and (
-                self.single_selection_enabled or self.toggle_selection_enabled
-            ):
+            elif r != 0 and (self.single_selection_enabled or self.toggle_selection_enabled):
                 if self.cell_completely_visible(r=r - 1, c=c):
                     self.select_cell(r - 1, c, redraw=True)
                 else:
                     self.select_cell(r - 1, c)
                     self.see(r - 1, c, keep_xscroll=True, check_cell_visibility=False)
 
     def arrowkey_RIGHT(self, event=None):
@@ -2282,49 +1994,41 @@
                     self.CH.select_col(c + 1, redraw=True)
                 else:
                     self.CH.select_col(c + 1)
                     self.see(
                         0,
                         c + 1,
                         keep_yscroll=True,
-                        bottom_right_corner=False
-                        if self.arrow_key_down_right_scroll_page
-                        else True,
+                        bottom_right_corner=False if self.arrow_key_down_right_scroll_page else True,
                         check_cell_visibility=False,
                     )
         else:
             r = currently_selected[0]
             c = currently_selected[1]
-            if c < len(self.col_positions) - 2 and (
-                self.single_selection_enabled or self.toggle_selection_enabled
-            ):
+            if c < len(self.col_positions) - 2 and (self.single_selection_enabled or self.toggle_selection_enabled):
                 if self.cell_completely_visible(r=r, c=c + 1):
                     self.select_cell(r, c + 1, redraw=True)
                 else:
                     self.select_cell(r, c + 1)
                     self.see(
                         r,
                         c + 1,
                         keep_yscroll=True,
-                        bottom_right_corner=False
-                        if self.arrow_key_down_right_scroll_page
-                        else True,
+                        bottom_right_corner=False if self.arrow_key_down_right_scroll_page else True,
                         check_cell_visibility=False,
                     )
 
     def arrowkey_DOWN(self, event=None):
         currently_selected = self.currently_selected()
         if not currently_selected:
             return
         if currently_selected.type_ == "row":
             r = currently_selected.row
             if r < len(self.row_positions) - 2 and self.RI.row_selection_enabled:
-                if self.cell_completely_visible(
-                    r=min(r + 2, len(self.row_positions) - 2), c=0
-                ):
+                if self.cell_completely_visible(r=min(r + 2, len(self.row_positions) - 2), c=0):
                     self.RI.select_row(r + 1, redraw=True)
                 else:
                     self.RI.select_row(r + 1)
                     if (
                         r + 2 < len(self.row_positions) - 2
                         and (self.row_positions[r + 3] - self.row_positions[r + 2])
                         + (self.row_positions[r + 2] - self.row_positions[r + 1])
@@ -2339,17 +2043,15 @@
                             check_cell_visibility=False,
                         )
                     elif not self.cell_completely_visible(r=r + 1, c=0):
                         self.see(
                             r + 1,
                             0,
                             keep_xscroll=True,
-                            bottom_right_corner=False
-                            if self.arrow_key_down_right_scroll_page
-                            else True,
+                            bottom_right_corner=False if self.arrow_key_down_right_scroll_page else True,
                             check_cell_visibility=False,
                         )
         elif currently_selected.type_ == "column":
             c = currently_selected.column
             if self.single_selection_enabled or self.toggle_selection_enabled:
                 if self.cell_completely_visible(r=0, c=c):
                     self.select_cell(0, c, redraw=True)
@@ -2361,20 +2063,16 @@
                         keep_xscroll=True,
                         bottom_right_corner=True,
                         check_cell_visibility=False,
                     )
         else:
             r = currently_selected[0]
             c = currently_selected[1]
-            if r < len(self.row_positions) - 2 and (
-                self.single_selection_enabled or self.toggle_selection_enabled
-            ):
-                if self.cell_completely_visible(
-                    r=min(r + 2, len(self.row_positions) - 2), c=c
-                ):
+            if r < len(self.row_positions) - 2 and (self.single_selection_enabled or self.toggle_selection_enabled):
+                if self.cell_completely_visible(r=min(r + 2, len(self.row_positions) - 2), c=c):
                     self.select_cell(r + 1, c, redraw=True)
                 else:
                     self.select_cell(r + 1, c)
                     if (
                         r + 2 < len(self.row_positions) - 2
                         and (self.row_positions[r + 3] - self.row_positions[r + 2])
                         + (self.row_positions[r + 2] - self.row_positions[r + 1])
@@ -2389,17 +2087,15 @@
                             check_cell_visibility=False,
                         )
                     elif not self.cell_completely_visible(r=r + 1, c=c):
                         self.see(
                             r + 1,
                             c,
                             keep_xscroll=True,
-                            bottom_right_corner=False
-                            if self.arrow_key_down_right_scroll_page
-                            else True,
+                            bottom_right_corner=False if self.arrow_key_down_right_scroll_page else True,
                             check_cell_visibility=False,
                         )
 
     def arrowkey_LEFT(self, event=None):
         currently_selected = self.currently_selected()
         if not currently_selected:
             return
@@ -2419,17 +2115,15 @@
                     )
         elif currently_selected.type_ == "cell":
             r = currently_selected.row
             c = currently_selected.column
             if c == 0 and self.RI.row_selection_enabled:
                 if not self.cell_completely_visible(r=r, c=0):
                     self.see(r, c, keep_yscroll=True, check_cell_visibility=False)
-            elif c != 0 and (
-                self.single_selection_enabled or self.toggle_selection_enabled
-            ):
+            elif c != 0 and (self.single_selection_enabled or self.toggle_selection_enabled):
                 if self.cell_completely_visible(r=r, c=c - 1):
                     self.select_cell(r, c - 1, redraw=True)
                 else:
                     self.select_cell(r, c - 1)
                     self.see(r, c - 1, keep_yscroll=True, check_cell_visibility=False)
 
     def edit_bindings(self, enable=True, key=None):
@@ -2520,25 +2214,19 @@
             pass
         menu.add_command(**kwargs)
 
     def create_rc_menus(self):
         if not self.rc_popup_menu:
             self.rc_popup_menu = tk.Menu(self, tearoff=0, background=self.popup_menu_bg)
         if not self.CH.ch_rc_popup_menu:
-            self.CH.ch_rc_popup_menu = tk.Menu(
-                self.CH, tearoff=0, background=self.popup_menu_bg
-            )
+            self.CH.ch_rc_popup_menu = tk.Menu(self.CH, tearoff=0, background=self.popup_menu_bg)
         if not self.RI.ri_rc_popup_menu:
-            self.RI.ri_rc_popup_menu = tk.Menu(
-                self.RI, tearoff=0, background=self.popup_menu_bg
-            )
+            self.RI.ri_rc_popup_menu = tk.Menu(self.RI, tearoff=0, background=self.popup_menu_bg)
         if not self.empty_rc_popup_menu:
-            self.empty_rc_popup_menu = tk.Menu(
-                self, tearoff=0, background=self.popup_menu_bg
-            )
+            self.empty_rc_popup_menu = tk.Menu(self, tearoff=0, background=self.popup_menu_bg)
         for menu in (
             self.rc_popup_menu,
             self.CH.ch_rc_popup_menu,
             self.RI.ri_rc_popup_menu,
             self.empty_rc_popup_menu,
         ):
             menu.delete(0, "end")
@@ -2955,17 +2643,15 @@
         elif binding == "row_select":
             self.RI.enable_bindings("row_select")
         elif binding == "row_drag_and_drop":
             self.RI.enable_bindings("drag_and_drop")
         elif binding == "arrowkeys":
             self.bind_arrowkeys(self.arrowkey_binding_functions)
         elif binding in ("tab", "up", "right", "down", "left", "prior", "next"):
-            self.bind_arrowkeys(
-                keys={binding: self.arrowkey_binding_functions[binding]}
-            )
+            self.bind_arrowkeys(keys={binding: self.arrowkey_binding_functions[binding]})
         elif binding == "edit_bindings":
             self.edit_bindings(True)
         elif binding == "rc_delete_column":
             self.rc_delete_column_enabled = True
             self.rc_popup_menus_enabled = True
             self.rc_select_enabled = True
         elif binding == "rc_delete_row":
@@ -3061,17 +2747,15 @@
         elif binding == "row_select":
             self.RI.disable_bindings("row_select")
         elif binding == "row_drag_and_drop":
             self.RI.disable_bindings("drag_and_drop")
         elif binding == "arrowkeys":
             self.unbind_arrowkeys(self.arrowkey_binding_functions)
         elif binding in ("tab", "up", "right", "down", "left", "prior", "next"):
-            self.unbind_arrowkeys(
-                keys={binding: self.arrowkey_binding_functions[binding]}
-            )
+            self.unbind_arrowkeys(keys={binding: self.arrowkey_binding_functions[binding]})
         elif binding == "rc_delete_column":
             self.rc_delete_column_enabled = False
         elif binding == "rc_delete_row":
             self.rc_delete_row_enabled = False
         elif binding == "rc_insert_column":
             self.rc_insert_column_enabled = False
         elif binding == "rc_insert_row":
@@ -3117,38 +2801,30 @@
             and not self.RI.currently_resizing_width
             and not self.CH.currently_resizing_height
             and not self.CH.currently_resizing_width
         ):
             mouse_over_resize = False
             x = self.canvasx(event.x)
             y = self.canvasy(event.y)
-            if (
-                self.RI.width_resizing_enabled
-                and self.show_index
-                and not mouse_over_resize
-            ):
+            if self.RI.width_resizing_enabled and self.show_index and not mouse_over_resize:
                 try:
                     x1, y1, x2, y2 = (
                         self.row_width_resize_bbox[0],
                         self.row_width_resize_bbox[1],
                         self.row_width_resize_bbox[2],
                         self.row_width_resize_bbox[3],
                     )
                     if x >= x1 and y >= y1 and x <= x2 and y <= y2:
                         self.config(cursor="sb_h_double_arrow")
                         self.RI.config(cursor="sb_h_double_arrow")
                         self.RI.rsz_w = True
                         mouse_over_resize = True
                 except Exception:
                     pass
-            if (
-                self.CH.height_resizing_enabled
-                and self.show_header
-                and not mouse_over_resize
-            ):
+            if self.CH.height_resizing_enabled and self.show_header and not mouse_over_resize:
                 try:
                     x1, y1, x2, y2 = (
                         self.header_height_resize_bbox[0],
                         self.header_height_resize_bbox[1],
                         self.header_height_resize_bbox[2],
                         self.header_height_resize_bbox[3],
                     )
@@ -3165,16 +2841,15 @@
             self.extra_motion_func(event)
 
     def rc(self, event=None):
         self.mouseclick_outside_editor_or_dropdown_all_canvases()
         self.focus_set()
         popup_menu = None
         if self.single_selection_enabled and all(
-            v is None
-            for v in (self.RI.rsz_h, self.RI.rsz_w, self.CH.rsz_h, self.CH.rsz_w)
+            v is None for v in (self.RI.rsz_h, self.RI.rsz_w, self.CH.rsz_h, self.CH.rsz_w)
         ):
             r = self.identify_row(y=event.y)
             c = self.identify_col(x=event.x)
             if r < len(self.row_positions) - 1 and c < len(self.col_positions) - 1:
                 if self.col_selected(c):
                     if self.rc_popup_menus_enabled:
                         popup_menu = self.CH.ch_rc_popup_menu
@@ -3188,16 +2863,15 @@
                     if self.rc_select_enabled:
                         self.select_cell(r, c, redraw=True)
                     if self.rc_popup_menus_enabled:
                         popup_menu = self.rc_popup_menu
             else:
                 popup_menu = self.empty_rc_popup_menu
         elif self.toggle_selection_enabled and all(
-            v is None
-            for v in (self.RI.rsz_h, self.RI.rsz_w, self.CH.rsz_h, self.CH.rsz_w)
+            v is None for v in (self.RI.rsz_h, self.RI.rsz_w, self.CH.rsz_h, self.CH.rsz_w)
         ):
             r = self.identify_row(y=event.y)
             c = self.identify_col(x=event.x)
             if r < len(self.row_positions) - 1 and c < len(self.col_positions) - 1:
                 if self.col_selected(c):
                     if self.rc_popup_menus_enabled:
                         popup_menu = self.CH.ch_rc_popup_menu
@@ -3227,51 +2901,35 @@
             self.identify_col(x=event.x, allow_end=False) is None
             or self.identify_row(y=event.y, allow_end=False) is None
         ):
             self.deselect("all")
         r = self.identify_row(y=event.y)
         c = self.identify_col(x=event.x)
         if self.single_selection_enabled and all(
-            v is None
-            for v in (self.RI.rsz_h, self.RI.rsz_w, self.CH.rsz_h, self.CH.rsz_w)
+            v is None for v in (self.RI.rsz_h, self.RI.rsz_w, self.CH.rsz_h, self.CH.rsz_w)
         ):
             if r < len(self.row_positions) - 1 and c < len(self.col_positions) - 1:
                 self.select_cell(r, c, redraw=True)
         elif self.toggle_selection_enabled and all(
-            v is None
-            for v in (self.RI.rsz_h, self.RI.rsz_w, self.CH.rsz_h, self.CH.rsz_w)
+            v is None for v in (self.RI.rsz_h, self.RI.rsz_w, self.CH.rsz_h, self.CH.rsz_w)
         ):
             r = self.identify_row(y=event.y)
             c = self.identify_col(x=event.x)
             if r < len(self.row_positions) - 1 and c < len(self.col_positions) - 1:
                 self.toggle_select_cell(r, c, redraw=True)
-        elif (
-            self.RI.width_resizing_enabled
-            and self.show_index
-            and self.RI.rsz_h is None
-            and self.RI.rsz_w
-        ):
+        elif self.RI.width_resizing_enabled and self.show_index and self.RI.rsz_h is None and self.RI.rsz_w:
             self.RI.currently_resizing_width = True
             self.new_row_width = self.RI.current_width + event.x
             x = self.canvasx(event.x)
-            self.create_resize_line(
-                x, y1, x, y2, width=1, fill=self.RI.resizing_line_fg, tag="rwl"
-            )
-        elif (
-            self.CH.height_resizing_enabled
-            and self.show_header
-            and self.CH.rsz_w is None
-            and self.CH.rsz_h
-        ):
+            self.create_resize_line(x, y1, x, y2, width=1, fill=self.RI.resizing_line_fg, tag="rwl")
+        elif self.CH.height_resizing_enabled and self.show_header and self.CH.rsz_w is None and self.CH.rsz_h:
             self.CH.currently_resizing_height = True
             self.new_header_height = self.CH.current_height + event.y
             y = self.canvasy(event.y)
-            self.create_resize_line(
-                x1, y, x2, y, width=1, fill=self.RI.resizing_line_fg, tag="rhl"
-            )
+            self.create_resize_line(x1, y, x2, y, width=1, fill=self.RI.resizing_line_fg, tag="rhl")
         self.b1_pressed_loc = (r, c)
         if self.extra_b1_press_func is not None:
             self.extra_b1_press_func(event)
 
     def create_resize_line(self, x1, y1, x2, y2, width, fill, tag):
         if self.hidd_resize_lines:
             t, sh = self.hidd_resize_lines.popitem()
@@ -3293,34 +2951,24 @@
                 self.itemconfig(t, state="hidden")
                 self.hidd_resize_lines[t] = False
 
     def ctrl_b1_press(self, event=None):
         self.mouseclick_outside_editor_or_dropdown_all_canvases()
         self.focus_set()
         if self.ctrl_select_enabled and all(
-            v is None
-            for v in (self.RI.rsz_h, self.RI.rsz_w, self.CH.rsz_h, self.CH.rsz_w)
+            v is None for v in (self.RI.rsz_h, self.RI.rsz_w, self.CH.rsz_h, self.CH.rsz_w)
         ):
             self.b1_pressed_loc = None
             rowsel = int(self.identify_row(y=event.y))
             colsel = int(self.identify_col(x=event.x))
-            if (
-                rowsel < len(self.row_positions) - 1
-                and colsel < len(self.col_positions) - 1
-            ):
+            if rowsel < len(self.row_positions) - 1 and colsel < len(self.col_positions) - 1:
                 currently_selected = self.currently_selected()
-                if (
-                    not currently_selected
-                    or currently_selected.row != rowsel
-                    or currently_selected.column != colsel
-                ):
+                if not currently_selected or currently_selected.row != rowsel or currently_selected.column != colsel:
                     self.add_selection(rowsel, colsel, set_as_current=True)
-                self.main_table_redraw_grid_and_text(
-                    redraw_header=True, redraw_row_index=True, redraw_table=True
-                )
+                self.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=True, redraw_table=True)
                 if self.ctrl_selection_binding_func is not None:
                     self.ctrl_selection_binding_func(
                         SelectionBoxEvent(
                             "ctrl_select_cells",
                             (rowsel, colsel, rowsel + 1, colsel + 1),
                         )
                     )
@@ -3329,26 +2977,20 @@
 
     def ctrl_shift_b1_press(self, event=None):
         self.mouseclick_outside_editor_or_dropdown_all_canvases()
         self.focus_set()
         if (
             self.ctrl_select_enabled
             and self.drag_selection_enabled
-            and all(
-                v is None
-                for v in (self.RI.rsz_h, self.RI.rsz_w, self.CH.rsz_h, self.CH.rsz_w)
-            )
+            and all(v is None for v in (self.RI.rsz_h, self.RI.rsz_w, self.CH.rsz_h, self.CH.rsz_w))
         ):
             self.b1_pressed_loc = None
             rowsel = int(self.identify_row(y=event.y))
             colsel = int(self.identify_col(x=event.x))
-            if (
-                rowsel < len(self.row_positions) - 1
-                and colsel < len(self.col_positions) - 1
-            ):
+            if rowsel < len(self.row_positions) - 1 and colsel < len(self.col_positions) - 1:
                 currently_selected = self.currently_selected()
                 if currently_selected and currently_selected.type_ == "cell":
                     min_r = currently_selected[0]
                     min_c = currently_selected[1]
                     if rowsel >= min_r and colsel >= min_c:
                         last_selected = (min_r, min_c, rowsel + 1, colsel + 1)
                     elif rowsel >= min_r and min_c >= colsel:
@@ -3357,288 +2999,207 @@
                         last_selected = (rowsel, min_c, min_r + 1, colsel + 1)
                     elif min_r >= rowsel and min_c >= colsel:
                         last_selected = (rowsel, colsel, min_r + 1, min_c + 1)
                     self.create_selected(*last_selected)
                 else:
                     self.add_selection(rowsel, colsel, set_as_current=True)
                     last_selected = (rowsel, colsel, rowsel + 1, colsel + 1)
-                self.main_table_redraw_grid_and_text(
-                    redraw_header=True, redraw_row_index=True, redraw_table=True
-                )
+                self.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=True, redraw_table=True)
                 if self.shift_selection_binding_func is not None:
-                    self.shift_selection_binding_func(
-                        SelectionBoxEvent("shift_select_cells", last_selected)
-                    )
+                    self.shift_selection_binding_func(SelectionBoxEvent("shift_select_cells", last_selected))
         elif not self.ctrl_select_enabled:
             self.shift_b1_press(event)
 
     def shift_b1_press(self, event=None):
         self.mouseclick_outside_editor_or_dropdown_all_canvases()
         self.focus_set()
         if self.drag_selection_enabled and all(
-            v is None
-            for v in (self.RI.rsz_h, self.RI.rsz_w, self.CH.rsz_h, self.CH.rsz_w)
+            v is None for v in (self.RI.rsz_h, self.RI.rsz_w, self.CH.rsz_h, self.CH.rsz_w)
         ):
             self.b1_pressed_loc = None
             rowsel = int(self.identify_row(y=event.y))
             colsel = int(self.identify_col(x=event.x))
-            if (
-                rowsel < len(self.row_positions) - 1
-                and colsel < len(self.col_positions) - 1
-            ):
+            if rowsel < len(self.row_positions) - 1 and colsel < len(self.col_positions) - 1:
                 currently_selected = self.currently_selected()
                 if currently_selected and currently_selected.type_ == "cell":
                     min_r = currently_selected[0]
                     min_c = currently_selected[1]
                     self.delete_selection_rects(delete_current=False)
                     if rowsel >= min_r and colsel >= min_c:
                         self.create_selected(min_r, min_c, rowsel + 1, colsel + 1)
                     elif rowsel >= min_r and min_c >= colsel:
                         self.create_selected(min_r, colsel, rowsel + 1, min_c + 1)
                     elif min_r >= rowsel and colsel >= min_c:
                         self.create_selected(rowsel, min_c, min_r + 1, colsel + 1)
                     elif min_r >= rowsel and min_c >= colsel:
                         self.create_selected(rowsel, colsel, min_r + 1, min_c + 1)
-                    last_selected = tuple(
-                        int(e)
-                        for e in self.gettags(self.find_withtag("cells"))[1].split("_")
-                        if e
-                    )
+                    last_selected = tuple(int(e) for e in self.gettags(self.find_withtag("cells"))[1].split("_") if e)
                 else:
                     self.select_cell(rowsel, colsel, redraw=False)
                     last_selected = tuple(
-                        int(e)
-                        for e in self.gettags(self.find_withtag("currently"))[1].split(
-                            "_"
-                        )
-                        if e
+                        int(e) for e in self.gettags(self.find_withtag("currently"))[1].split("_") if e
                     )
-                self.main_table_redraw_grid_and_text(
-                    redraw_header=True, redraw_row_index=True, redraw_table=True
-                )
+                self.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=True, redraw_table=True)
                 if self.shift_selection_binding_func is not None:
-                    self.shift_selection_binding_func(
-                        SelectionBoxEvent("shift_select_cells", last_selected)
-                    )
+                    self.shift_selection_binding_func(SelectionBoxEvent("shift_select_cells", last_selected))
 
     def get_b1_motion_rect(self, start_row, start_col, end_row, end_col):
-        if (
-            end_row >= start_row
-            and end_col >= start_col
-            and (end_row - start_row or end_col - start_col)
-        ):
+        if end_row >= start_row and end_col >= start_col and (end_row - start_row or end_col - start_col):
             return (start_row, start_col, end_row + 1, end_col + 1, "cells")
-        elif (
-            end_row >= start_row
-            and end_col < start_col
-            and (end_row - start_row or start_col - end_col)
-        ):
+        elif end_row >= start_row and end_col < start_col and (end_row - start_row or start_col - end_col):
             return (start_row, end_col, end_row + 1, start_col + 1, "cells")
-        elif (
-            end_row < start_row
-            and end_col >= start_col
-            and (start_row - end_row or end_col - start_col)
-        ):
+        elif end_row < start_row and end_col >= start_col and (start_row - end_row or end_col - start_col):
             return (end_row, start_col, start_row + 1, end_col + 1, "cells")
-        elif (
-            end_row < start_row
-            and end_col < start_col
-            and (start_row - end_row or start_col - end_col)
-        ):
+        elif end_row < start_row and end_col < start_col and (start_row - end_row or start_col - end_col):
             return (end_row, end_col, start_row + 1, start_col + 1, "cells")
         else:
             return (start_row, start_col, start_row + 1, start_col + 1, "cells")
         return None
 
     def b1_motion(self, event):
         x1, y1, x2, y2 = self.get_canvas_visible_area()
         if self.drag_selection_enabled and all(
-            v is None
-            for v in (self.RI.rsz_h, self.RI.rsz_w, self.CH.rsz_h, self.CH.rsz_w)
+            v is None for v in (self.RI.rsz_h, self.RI.rsz_w, self.CH.rsz_h, self.CH.rsz_w)
         ):
             need_redraw = False
             end_row = self.identify_row(y=event.y)
             end_col = self.identify_col(x=event.x)
             currently_selected = self.currently_selected()
             if (
                 end_row < len(self.row_positions) - 1
                 and end_col < len(self.col_positions) - 1
                 and currently_selected
                 and currently_selected.type_ == "cell"
             ):
-                rect = self.get_b1_motion_rect(
-                    *(currently_selected[0], currently_selected[1], end_row, end_col)
-                )
+                rect = self.get_b1_motion_rect(*(currently_selected[0], currently_selected[1], end_row, end_col))
                 if rect is not None and self.being_drawn_rect != rect:
                     self.delete_selection_rects(delete_current=False)
                     if rect[2] - rect[0] == 1 and rect[3] - rect[1] == 1:
                         self.being_drawn_rect = rect
                     else:
                         self.being_drawn_rect = rect
                         self.create_selected(*rect)
                     if self.drag_selection_binding_func is not None:
-                        self.drag_selection_binding_func(
-                            SelectionBoxEvent("drag_select_cells", rect[:-1])
-                        )
+                        self.drag_selection_binding_func(SelectionBoxEvent("drag_select_cells", rect[:-1]))
                     need_redraw = True
             if self.scroll_if_event_offscreen(event):
                 need_redraw = True
             if need_redraw:
-                self.main_table_redraw_grid_and_text(
-                    redraw_header=True, redraw_row_index=True, redraw_table=True
-                )
-        elif (
-            self.RI.width_resizing_enabled
-            and self.RI.rsz_w is not None
-            and self.RI.currently_resizing_width
-        ):
+                self.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=True, redraw_table=True)
+        elif self.RI.width_resizing_enabled and self.RI.rsz_w is not None and self.RI.currently_resizing_width:
             self.RI.delete_resize_lines()
             self.delete_resize_lines()
             if event.x >= 0:
                 x = self.canvasx(event.x)
                 self.new_row_width = self.RI.current_width + event.x
-                self.create_resize_line(
-                    x, y1, x, y2, width=1, fill=self.RI.resizing_line_fg, tag="rwl"
-                )
+                self.create_resize_line(x, y1, x, y2, width=1, fill=self.RI.resizing_line_fg, tag="rwl")
             else:
                 x = self.RI.current_width + event.x
                 if x < self.min_column_width:
                     x = int(self.min_column_width)
                 self.new_row_width = x
-                self.RI.create_resize_line(
-                    x, y1, x, y2, width=1, fill=self.RI.resizing_line_fg, tag="rwl"
-                )
-        elif (
-            self.CH.height_resizing_enabled
-            and self.CH.rsz_h is not None
-            and self.CH.currently_resizing_height
-        ):
+                self.RI.create_resize_line(x, y1, x, y2, width=1, fill=self.RI.resizing_line_fg, tag="rwl")
+        elif self.CH.height_resizing_enabled and self.CH.rsz_h is not None and self.CH.currently_resizing_height:
             self.CH.delete_resize_lines()
             self.delete_resize_lines()
             if event.y >= 0:
                 y = self.canvasy(event.y)
                 self.new_header_height = self.CH.current_height + event.y
-                self.create_resize_line(
-                    x1, y, x2, y, width=1, fill=self.RI.resizing_line_fg, tag="rhl"
-                )
+                self.create_resize_line(x1, y, x2, y, width=1, fill=self.RI.resizing_line_fg, tag="rhl")
             else:
                 y = self.CH.current_height + event.y
                 if y < self.min_header_height:
                     y = int(self.min_header_height)
                 self.new_header_height = y
-                self.CH.create_resize_line(
-                    x1, y, x2, y, width=1, fill=self.RI.resizing_line_fg, tag="rhl"
-                )
+                self.CH.create_resize_line(x1, y, x2, y, width=1, fill=self.RI.resizing_line_fg, tag="rhl")
         if self.extra_b1_motion_func is not None:
             self.extra_b1_motion_func(event)
 
     def ctrl_b1_motion(self, event):
         x1, y1, x2, y2 = self.get_canvas_visible_area()
         if (
             self.ctrl_select_enabled
             and self.drag_selection_enabled
-            and all(
-                v is None
-                for v in (self.RI.rsz_h, self.RI.rsz_w, self.CH.rsz_h, self.CH.rsz_w)
-            )
+            and all(v is None for v in (self.RI.rsz_h, self.RI.rsz_w, self.CH.rsz_h, self.CH.rsz_w))
         ):
             need_redraw = False
             end_row = self.identify_row(y=event.y)
             end_col = self.identify_col(x=event.x)
             currently_selected = self.currently_selected()
             if (
                 end_row < len(self.row_positions) - 1
                 and end_col < len(self.col_positions) - 1
                 and currently_selected
                 and currently_selected.type_ == "cell"
             ):
-                rect = self.get_b1_motion_rect(
-                    *(currently_selected[0], currently_selected[1], end_row, end_col)
-                )
+                rect = self.get_b1_motion_rect(*(currently_selected[0], currently_selected[1], end_row, end_col))
                 if rect is not None and self.being_drawn_rect != rect:
                     if rect[2] - rect[0] == 1 and rect[3] - rect[1] == 1:
                         self.being_drawn_rect = rect
                     else:
                         if self.being_drawn_rect is not None:
                             self.delete_selected(*self.being_drawn_rect)
                         self.being_drawn_rect = rect
                         self.create_selected(*rect)
                     if self.drag_selection_binding_func is not None:
-                        self.drag_selection_binding_func(
-                            SelectionBoxEvent("drag_select_cells", rect[:-1])
-                        )
+                        self.drag_selection_binding_func(SelectionBoxEvent("drag_select_cells", rect[:-1]))
                     need_redraw = True
             if self.scroll_if_event_offscreen(event):
                 need_redraw = True
             if need_redraw:
-                self.main_table_redraw_grid_and_text(
-                    redraw_header=True, redraw_row_index=True, redraw_table=True
-                )
+                self.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=True, redraw_table=True)
         elif not self.ctrl_select_enabled:
             self.b1_motion(event)
 
     def b1_release(self, event=None):
         if self.being_drawn_rect is not None and (
             self.being_drawn_rect[2] - self.being_drawn_rect[0] > 1
             or self.being_drawn_rect[3] - self.being_drawn_rect[1] > 1
         ):
             self.delete_selected(*self.being_drawn_rect)
             to_sel = tuple(self.being_drawn_rect)
             self.being_drawn_rect = None
             self.create_selected(*to_sel)
         else:
             self.being_drawn_rect = None
-        if (
-            self.RI.width_resizing_enabled
-            and self.RI.rsz_w is not None
-            and self.RI.currently_resizing_width
-        ):
+        if self.RI.width_resizing_enabled and self.RI.rsz_w is not None and self.RI.currently_resizing_width:
             self.delete_resize_lines()
             self.RI.delete_resize_lines()
             self.RI.currently_resizing_width = False
             self.RI.set_width(self.new_row_width, set_TL=True)
-            self.main_table_redraw_grid_and_text(
-                redraw_header=True, redraw_row_index=True
-            )
+            self.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=True)
             self.b1_pressed_loc = None
-        elif (
-            self.CH.height_resizing_enabled
-            and self.CH.rsz_h is not None
-            and self.CH.currently_resizing_height
-        ):
+        elif self.CH.height_resizing_enabled and self.CH.rsz_h is not None and self.CH.currently_resizing_height:
             self.delete_resize_lines()
             self.CH.delete_resize_lines()
             self.CH.currently_resizing_height = False
             self.CH.set_height(self.new_header_height, set_TL=True)
-            self.main_table_redraw_grid_and_text(
-                redraw_header=True, redraw_row_index=True
-            )
+            self.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=True)
             self.b1_pressed_loc = None
         self.RI.rsz_w = None
         self.CH.rsz_h = None
         if self.b1_pressed_loc is not None:
             r = self.identify_row(y=event.y, allow_end=False)
             c = self.identify_col(x=event.x, allow_end=False)
             if r is not None and c is not None and (r, c) == self.b1_pressed_loc:
                 datarn = r if self.all_rows_displayed else self.displayed_rows[r]
                 datacn = c if self.all_columns_displayed else self.displayed_columns[c]
-                if self.get_cell_kwargs(
-                    datarn, datacn, key="dropdown"
-                ) or self.get_cell_kwargs(datarn, datacn, key="checkbox"):
+                if self.get_cell_kwargs(datarn, datacn, key="dropdown") or self.get_cell_kwargs(
+                    datarn, datacn, key="checkbox"
+                ):
                     canvasx = self.canvasx(event.x)
                     if (
                         self.closed_dropdown != self.b1_pressed_loc
                         and self.get_cell_kwargs(datarn, datacn, key="dropdown")
                         and canvasx > self.col_positions[c + 1] - self.txt_h - 4
                         and canvasx < self.col_positions[c + 1] - 1
                     ) or (
                         self.get_cell_kwargs(datarn, datacn, key="checkbox")
                         and canvasx < self.col_positions[c] + self.txt_h + 4
-                        and self.canvasy(event.y)
-                        < self.row_positions[r] + self.txt_h + 4
+                        and self.canvasy(event.y) < self.row_positions[r] + self.txt_h + 4
                     ):
                         self.open_cell(event)
             else:
                 self.mouseclick_outside_editor_or_dropdown_all_canvases()
         self.b1_pressed_loc = None
         self.closed_dropdown = None
         if self.extra_b1_release_func is not None:
@@ -3650,26 +3211,24 @@
         x1, y1, x2, y2 = self.get_canvas_visible_area()
         if (
             self.identify_col(x=event.x, allow_end=False) is None
             or self.identify_row(y=event.y, allow_end=False) is None
         ):
             self.deselect("all")
         elif self.single_selection_enabled and all(
-            v is None
-            for v in (self.RI.rsz_h, self.RI.rsz_w, self.CH.rsz_h, self.CH.rsz_w)
+            v is None for v in (self.RI.rsz_h, self.RI.rsz_w, self.CH.rsz_h, self.CH.rsz_w)
         ):
             r = self.identify_row(y=event.y)
             c = self.identify_col(x=event.x)
             if r < len(self.row_positions) - 1 and c < len(self.col_positions) - 1:
                 self.select_cell(r, c, redraw=True)
                 if self.edit_cell_enabled:
                     self.open_cell(event)
         elif self.toggle_selection_enabled and all(
-            v is None
-            for v in (self.RI.rsz_h, self.RI.rsz_w, self.CH.rsz_h, self.CH.rsz_w)
+            v is None for v in (self.RI.rsz_h, self.RI.rsz_w, self.CH.rsz_h, self.CH.rsz_w)
         ):
             r = self.identify_row(y=event.y)
             c = self.identify_col(x=event.x)
             if r < len(self.row_positions) - 1 and c < len(self.col_positions) - 1:
                 self.toggle_select_cell(r, c, redraw=True)
                 if self.edit_cell_enabled:
                     self.open_cell(event)
@@ -3758,26 +3317,22 @@
         return need_redraw
 
     def set_xviews(self, *args):
         self.xview(*args)
         if self.show_header:
             self.CH.xview(*args)
         self.fix_views()
-        self.main_table_redraw_grid_and_text(
-            redraw_header=True if self.show_header else False
-        )
+        self.main_table_redraw_grid_and_text(redraw_header=True if self.show_header else False)
 
     def set_yviews(self, *args):
         self.yview(*args)
         if self.show_index:
             self.RI.yview(*args)
         self.fix_views()
-        self.main_table_redraw_grid_and_text(
-            redraw_row_index=True if self.show_index else False
-        )
+        self.main_table_redraw_grid_and_text(redraw_row_index=True if self.show_index else False)
 
     def set_view(self, x_args, y_args):
         self.xview(*x_args)
         if self.show_header:
             self.CH.xview(*x_args)
         self.yview(*y_args)
         if self.show_index:
@@ -3849,112 +3404,120 @@
     def set_min_column_width(self):
         self.min_column_width = 5
         if self.min_column_width > self.max_column_width:
             self.max_column_width = self.min_column_width + 20
         if self.min_column_width > self.default_column_width:
             self.default_column_width = self.min_column_width + 20
 
-    def font(self, newfont=None, reset_row_positions=False):
+    def set_table_font(self, newfont=None, reset_row_positions=False):
         if newfont:
             if not isinstance(newfont, tuple):
                 raise ValueError("Argument must be tuple e.g. ('Carlito',12,'normal')")
             if len(newfont) != 3:
                 raise ValueError("Argument must be three-tuple")
-            if (
-                not isinstance(newfont[0], str)
-                or not isinstance(newfont[1], int)
-                or not isinstance(newfont[2], str)
-            ):
+            if not isinstance(newfont[0], str) or not isinstance(newfont[1], int) or not isinstance(newfont[2], str):
                 raise ValueError(
                     "Argument must be font, size and 'normal', 'bold' or 'italic' e.g. ('Carlito',12,'normal')"
                 )
             self.table_font = newfont
             self.font_fam = newfont[0]
             self.font_sze = newfont[1]
             self.font_wgt = newfont[2]
-            self.set_font_help()
+            self.set_table_font_help()
             if reset_row_positions:
                 self.reset_row_positions()
+            self.recreate_all_selection_boxes()
         else:
             return self.table_font
 
-    def set_font_help(self):
+    def set_table_font_help(self):
         self.txt_h = self.get_txt_h("|ZXjy*'^")
         self.txt_w = self.get_txt_w("|")
         self.half_txt_h = ceil(self.txt_h / 2)
         if self.half_txt_h % 2 == 0:
             self.fl_ins = self.half_txt_h + 2
         else:
             self.fl_ins = self.half_txt_h + 3
         self.xtra_lines_increment = int(self.txt_h)
         self.min_row_height = self.txt_h + 5
         if self.min_row_height < 12:
             self.min_row_height = 12
         if self.default_row_height[0] != "pixels":
             self.default_row_height = (
-                self.default_row_height[0]
-                if self.default_row_height[0] != "pixels"
-                else "pixels",
+                self.default_row_height[0] if self.default_row_height[0] != "pixels" else "pixels",
                 self.get_lines_cell_height(int(self.default_row_height[0]))
                 if self.default_row_height[0] != "pixels"
                 else self.default_row_height[1],
             )
         self.set_min_column_width()
 
-    def header_font(self, newfont=None):
+    def set_header_font(self, newfont=None):
         if newfont:
             if not isinstance(newfont, tuple):
-                raise ValueError(
-                    "Argument must be tuple e.g. ('Carlito', 12, 'normal')"
-                )
+                raise ValueError("Argument must be tuple e.g. ('Carlito', 12, 'normal')")
             if len(newfont) != 3:
                 raise ValueError("Argument must be three-tuple")
-            if (
-                not isinstance(newfont[0], str)
-                or not isinstance(newfont[1], int)
-                or not isinstance(newfont[2], str)
-            ):
+            if not isinstance(newfont[0], str) or not isinstance(newfont[1], int) or not isinstance(newfont[2], str):
                 raise ValueError(
                     "Argument must be font, size and 'normal', 'bold' or 'italic' e.g. ('Carlito', 12, 'normal')"
                 )
             self.header_font = newfont
             self.header_font_fam = newfont[0]
             self.header_font_sze = newfont[1]
             self.header_font_wgt = newfont[2]
             self.set_header_font_help()
+            self.recreate_all_selection_boxes()
         else:
             return self.header_font
 
     def set_header_font_help(self):
-        self.header_txt_w, self.header_txt_h = self.get_txt_dimensions(
-            "|", self.header_font
-        )
+        self.header_txt_w, self.header_txt_h = self.get_txt_dimensions("|", self.header_font)
         self.header_half_txt_h = ceil(self.header_txt_h / 2)
         if self.header_half_txt_h % 2 == 0:
             self.header_fl_ins = self.header_half_txt_h + 2
         else:
             self.header_fl_ins = self.header_half_txt_h + 3
         self.header_xtra_lines_increment = self.header_txt_h
         self.min_header_height = self.header_txt_h + 5
         if self.default_header_height[0] != "pixels":
             self.default_header_height = (
-                self.default_header_height[0]
-                if self.default_header_height[0] != "pixels"
-                else "pixels",
-                self.get_lines_cell_height(
-                    int(self.default_header_height[0]), font=self.header_font
-                )
+                self.default_header_height[0] if self.default_header_height[0] != "pixels" else "pixels",
+                self.get_lines_cell_height(int(self.default_header_height[0]), font=self.header_font)
                 if self.default_header_height[0] != "pixels"
                 else self.default_header_height[1],
             )
         self.set_min_column_width()
-        self.CH.set_height(self.default_header_height[1])
+        self.CH.set_height(self.default_header_height[1], set_TL=True)
+
+    def set_index_font(self, newfont: Union[tuple, None] = None) -> tuple:
+        if newfont:
+            if not isinstance(newfont, tuple):
+                raise ValueError("Argument must be tuple e.g. ('Carlito', 12, 'normal')")
+            if len(newfont) != 3:
+                raise ValueError("Argument must be three-tuple")
+            if not isinstance(newfont[0], str) or not isinstance(newfont[1], int) or not isinstance(newfont[2], str):
+                raise ValueError(
+                    "Argument must be font, size and 'normal', 'bold' or" "'italic' e.g. ('Carlito',12,'normal')"
+                )
+            self.index_font = newfont
+            self.index_font_fam = newfont[0]
+            self.index_font_sze = newfont[1]
+            self.index_font_wgt = newfont[2]
+            self.set_index_font_help()
+        return self.index_font
 
     def set_index_font_help(self):
-        pass
+        self.index_txt_width, self.index_txt_height = self.get_txt_dimensions("|", self.index_font)
+        self.index_half_txt_height = ceil(self.index_txt_height / 2)
+        if self.index_half_txt_height % 2 == 0:
+            self.index_first_ln_ins = self.index_half_txt_height + 2
+        else:
+            self.index_first_ln_ins = self.index_half_txt_height + 3
+        self.index_xtra_lines_increment = self.index_txt_height
+        self.min_index_width = 5
 
     def data_reference(
         self,
         newdataref=None,
         reset_col_positions=True,
         reset_row_positions=True,
         redraw=False,
@@ -3969,43 +3532,35 @@
                 self.delete_all_formatting(clear_values=False)
             self.undo_storage = deque(maxlen=self.max_undos)
             if reset_col_positions:
                 self.reset_col_positions()
             if reset_row_positions:
                 self.reset_row_positions()
             if redraw:
-                self.main_table_redraw_grid_and_text(
-                    redraw_header=True, redraw_row_index=True
-                )
+                self.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=True)
         if return_id:
             return id(self.data)
         else:
             return self.data
 
     def get_cell_dimensions(self, datarn, datacn):
         txt = self.get_valid_cell_data_as_str(datarn, datacn, get_displayed=True)
         if txt:
-            self.txt_measure_canvas.itemconfig(
-                self.txt_measure_canvas_text, text=txt, font=self.table_font
-            )
+            self.txt_measure_canvas.itemconfig(self.txt_measure_canvas_text, text=txt, font=self.table_font)
             b = self.txt_measure_canvas.bbox(self.txt_measure_canvas_text)
             w = b[2] - b[0] + 7
             h = b[3] - b[1] + 5
         else:
             w = self.min_column_width
             h = self.min_row_height
-        if self.get_cell_kwargs(datarn, datacn, key="dropdown") or self.get_cell_kwargs(
-            datarn, datacn, key="checkbox"
-        ):
+        if self.get_cell_kwargs(datarn, datacn, key="dropdown") or self.get_cell_kwargs(datarn, datacn, key="checkbox"):
             return w + self.txt_h, h
         return w, h
 
-    def set_cell_size_to_text(
-        self, r, c, only_set_if_too_small=False, redraw=True, run_binding=False
-    ):
+    def set_cell_size_to_text(self, r, c, only_set_if_too_small=False, redraw=True, run_binding=False):
         min_column_width = int(self.min_column_width)
         min_rh = int(self.min_row_height)
         w = min_column_width
         h = min_rh
         datacn = c if self.all_columns_displayed else self.displayed_columns[c]
         datarn = r if self.all_rows_displayed else self.displayed_rows[r]
         tw, h = self.get_cell_dimensions(datarn, datacn)
@@ -4032,45 +3587,31 @@
             if h != self.row_positions[r + 1] - self.row_positions[r]:
                 cell_needs_resize_h = True
         if cell_needs_resize_w:
             old_width = self.col_positions[c + 1] - self.col_positions[c]
             new_col_pos = self.col_positions[c] + w
             increment = new_col_pos - self.col_positions[c + 1]
             self.col_positions[c + 2 :] = [
-                e + increment
-                for e in islice(self.col_positions, c + 2, len(self.col_positions))
+                e + increment for e in islice(self.col_positions, c + 2, len(self.col_positions))
             ]
             self.col_positions[c + 1] = new_col_pos
             new_width = self.col_positions[c + 1] - self.col_positions[c]
-            if (
-                run_binding
-                and self.CH.column_width_resize_func is not None
-                and old_width != new_width
-            ):
-                self.CH.column_width_resize_func(
-                    ResizeEvent("column_width_resize", c, old_width, new_width)
-                )
+            if run_binding and self.CH.column_width_resize_func is not None and old_width != new_width:
+                self.CH.column_width_resize_func(ResizeEvent("column_width_resize", c, old_width, new_width))
         if cell_needs_resize_h:
             old_height = self.row_positions[r + 1] - self.row_positions[r]
             new_row_pos = self.row_positions[r] + h
             increment = new_row_pos - self.row_positions[r + 1]
             self.row_positions[r + 2 :] = [
-                e + increment
-                for e in islice(self.row_positions, r + 2, len(self.row_positions))
+                e + increment for e in islice(self.row_positions, r + 2, len(self.row_positions))
             ]
             self.row_positions[r + 1] = new_row_pos
             new_height = self.row_positions[r + 1] - self.row_positions[r]
-            if (
-                run_binding
-                and self.RI.row_height_resize_func is not None
-                and old_height != new_height
-            ):
-                self.RI.row_height_resize_func(
-                    ResizeEvent("row_height_resize", r, old_height, new_height)
-                )
+            if run_binding and self.RI.row_height_resize_func is not None and old_height != new_height:
+                self.RI.row_height_resize_func(ResizeEvent("row_height_resize", r, old_height, new_height))
         if cell_needs_resize_w or cell_needs_resize_h:
             self.recreate_all_selection_boxes()
             if redraw:
                 self.refresh()
                 return True
             else:
                 return False
@@ -4105,28 +3646,26 @@
                     rhs[datarn] = h
         for datacn in itercols:
             w, h_ = self.CH.get_cell_dimensions(datacn)
             if self.all_rows_displayed:
                 # refresh range generator if needed
                 iterrows = range(self.total_data_rows())
             for datarn in iterrows:
-                txt = self.get_valid_cell_data_as_str(
-                    datarn, datacn, get_displayed=True
-                )
+                txt = self.get_valid_cell_data_as_str(datarn, datacn, get_displayed=True)
                 if txt:
                     itmcon(x, text=txt)
                     b = itmbbx(x)
                     tw = b[2] - b[0] + 7
                     h = b[3] - b[1] + 5
                 else:
                     tw = min_column_width
                     h = min_rh
-                if self.get_cell_kwargs(
-                    datarn, datacn, key="dropdown"
-                ) or self.get_cell_kwargs(datarn, datacn, key="checkbox"):
+                if self.get_cell_kwargs(datarn, datacn, key="dropdown") or self.get_cell_kwargs(
+                    datarn, datacn, key="checkbox"
+                ):
                     tw += self.txt_h
                 if tw > w:
                     w = tw
                 if h < min_rh:
                     h = int(min_rh)
                 elif h > self.max_row_height:
                     h = int(self.max_row_height)
@@ -4135,110 +3674,82 @@
             if w < min_column_width:
                 w = int(min_column_width)
             elif w > self.max_column_width:
                 w = int(self.max_column_width)
             cws.append(w)
         self.txt_measure_canvas.delete(x)
         self.txt_measure_canvas.delete(x2)
-        self.row_positions = list(
-            accumulate(chain([0], (height for height in rhs.values())))
-        )
+        self.row_positions = list(accumulate(chain([0], (height for height in rhs.values()))))
         self.col_positions = list(accumulate(chain([0], (width for width in cws))))
         self.recreate_all_selection_boxes()
         return self.row_positions, self.col_positions
 
     def reset_col_positions(self, ncols=None):
         colpos = int(self.default_column_width)
         if self.all_columns_displayed:
             self.col_positions = list(
                 accumulate(
                     chain(
                         [0],
-                        (
-                            colpos
-                            for c in range(
-                                ncols if ncols is not None else self.total_data_cols()
-                            )
-                        ),
+                        (colpos for c in range(ncols if ncols is not None else self.total_data_cols())),
                     )
                 )
             )
         else:
             self.col_positions = list(
                 accumulate(
                     chain(
                         [0],
-                        (
-                            colpos
-                            for c in range(
-                                ncols
-                                if ncols is not None
-                                else len(self.displayed_columns)
-                            )
-                        ),
+                        (colpos for c in range(ncols if ncols is not None else len(self.displayed_columns))),
                     )
                 )
             )
 
     def reset_row_positions(self, nrows=None):
         rowpos = self.default_row_height[1]
         if self.all_rows_displayed:
             self.row_positions = list(
                 accumulate(
                     chain(
                         [0],
-                        (
-                            rowpos
-                            for r in range(
-                                nrows if nrows is not None else self.total_data_rows()
-                            )
-                        ),
+                        (rowpos for r in range(nrows if nrows is not None else self.total_data_rows())),
                     )
                 )
             )
         else:
             self.row_positions = list(
                 accumulate(
                     chain(
                         [0],
-                        (
-                            rowpos
-                            for r in range(
-                                nrows if nrows is not None else len(self.displayed_rows)
-                            )
-                        ),
+                        (rowpos for r in range(nrows if nrows is not None else len(self.displayed_rows))),
                     )
                 )
             )
 
     def del_col_position(self, idx, deselect_all=False):
         if deselect_all:
             self.deselect("all", redraw=False)
         if idx == "end" or len(self.col_positions) <= idx + 1:
             del self.col_positions[-1]
         else:
             w = self.col_positions[idx + 1] - self.col_positions[idx]
             idx += 1
             del self.col_positions[idx]
-            self.col_positions[idx:] = [
-                e - w for e in islice(self.col_positions, idx, len(self.col_positions))
-            ]
+            self.col_positions[idx:] = [e - w for e in islice(self.col_positions, idx, len(self.col_positions))]
 
     def del_row_position(self, idx, deselect_all=False):
         if deselect_all:
             self.deselect("all", redraw=False)
         if idx == "end" or len(self.row_positions) <= idx + 1:
             del self.row_positions[-1]
         else:
             w = self.row_positions[idx + 1] - self.row_positions[idx]
             idx += 1
             del self.row_positions[idx]
-            self.row_positions[idx:] = [
-                e - w for e in islice(self.row_positions, idx, len(self.row_positions))
-            ]
+            self.row_positions[idx:] = [e - w for e in islice(self.row_positions, idx, len(self.row_positions))]
 
     def del_col_positions(self, idx, num=1, deselect_all=False):
         if deselect_all:
             self.deselect("all", redraw=False)
         if idx == "end" or len(self.col_positions) <= idx + 1:
             del self.col_positions[-1]
         else:
@@ -4262,135 +3773,105 @@
                 int(b - a)
                 for a, b in zip(
                     self.row_positions,
                     islice(self.row_positions, 1, len(self.row_positions)),
                 )
             ]
             rhs[idx : idx + numrows] = []
-            self.row_positions = list(
-                accumulate(chain([0], (height for height in rhs)))
-            )
+            self.row_positions = list(accumulate(chain([0], (height for height in rhs))))
 
     def insert_col_position(self, idx="end", width=None, deselect_all=False):
         if deselect_all:
             self.deselect("all", redraw=False)
         if width is None:
             w = self.default_column_width
         else:
             w = width
         if idx == "end" or len(self.col_positions) == idx + 1:
             self.col_positions.append(self.col_positions[-1] + w)
         else:
             idx += 1
             self.col_positions.insert(idx, self.col_positions[idx - 1] + w)
             idx += 1
-            self.col_positions[idx:] = [
-                e + w for e in islice(self.col_positions, idx, len(self.col_positions))
-            ]
+            self.col_positions[idx:] = [e + w for e in islice(self.col_positions, idx, len(self.col_positions))]
 
     def insert_row_position(self, idx, height=None, deselect_all=False):
         if deselect_all:
             self.deselect("all", redraw=False)
         if height is None:
             h = self.default_row_height[1]
         else:
             h = height
         if idx == "end" or len(self.row_positions) == idx + 1:
             self.row_positions.append(self.row_positions[-1] + h)
         else:
             idx += 1
             self.row_positions.insert(idx, self.row_positions[idx - 1] + h)
             idx += 1
-            self.row_positions[idx:] = [
-                e + h for e in islice(self.row_positions, idx, len(self.row_positions))
-            ]
+            self.row_positions[idx:] = [e + h for e in islice(self.row_positions, idx, len(self.row_positions))]
 
     def insert_col_positions(self, idx="end", widths=None, deselect_all=False):
         if deselect_all:
             self.deselect("all", redraw=False)
         if widths is None:
             w = [self.default_column_width]
         elif isinstance(widths, int):
             w = list(repeat(self.default_column_width, widths))
         else:
             w = widths
         if idx == "end" or len(self.col_positions) == idx + 1:
             if len(w) > 1:
-                self.col_positions += list(
-                    accumulate(
-                        chain([self.col_positions[-1] + w[0]], islice(w, 1, None))
-                    )
-                )
+                self.col_positions += list(accumulate(chain([self.col_positions[-1] + w[0]], islice(w, 1, None))))
             else:
                 self.col_positions.append(self.col_positions[-1] + w[0])
         else:
             if len(w) > 1:
                 idx += 1
                 self.col_positions[idx:idx] = list(
-                    accumulate(
-                        chain([self.col_positions[idx - 1] + w[0]], islice(w, 1, None))
-                    )
+                    accumulate(chain([self.col_positions[idx - 1] + w[0]], islice(w, 1, None)))
                 )
                 idx += len(w)
                 sumw = sum(w)
-                self.col_positions[idx:] = [
-                    e + sumw
-                    for e in islice(self.col_positions, idx, len(self.col_positions))
-                ]
+                self.col_positions[idx:] = [e + sumw for e in islice(self.col_positions, idx, len(self.col_positions))]
             else:
                 w = w[0]
                 idx += 1
                 self.col_positions.insert(idx, self.col_positions[idx - 1] + w)
                 idx += 1
-                self.col_positions[idx:] = [
-                    e + w
-                    for e in islice(self.col_positions, idx, len(self.col_positions))
-                ]
+                self.col_positions[idx:] = [e + w for e in islice(self.col_positions, idx, len(self.col_positions))]
 
     def insert_row_positions(self, idx="end", heights=None, deselect_all=False):
         if deselect_all:
             self.deselect("all", redraw=False)
         if heights is None:
             h = [self.default_row_height[1]]
         elif isinstance(heights, int):
             h = list(repeat(self.default_row_height[1], heights))
         else:
             h = heights
         if idx == "end" or len(self.row_positions) == idx + 1:
             if len(h) > 1:
-                self.row_positions += list(
-                    accumulate(
-                        chain([self.row_positions[-1] + h[0]], islice(h, 1, None))
-                    )
-                )
+                self.row_positions += list(accumulate(chain([self.row_positions[-1] + h[0]], islice(h, 1, None))))
             else:
                 self.row_positions.append(self.row_positions[-1] + h[0])
         else:
             if len(h) > 1:
                 idx += 1
                 self.row_positions[idx:idx] = list(
-                    accumulate(
-                        chain([self.row_positions[idx - 1] + h[0]], islice(h, 1, None))
-                    )
+                    accumulate(chain([self.row_positions[idx - 1] + h[0]], islice(h, 1, None)))
                 )
                 idx += len(h)
                 sumh = sum(h)
-                self.row_positions[idx:] = [
-                    e + sumh
-                    for e in islice(self.row_positions, idx, len(self.row_positions))
-                ]
+                self.row_positions[idx:] = [e + sumh for e in islice(self.row_positions, idx, len(self.row_positions))]
             else:
                 h = h[0]
                 idx += 1
                 self.row_positions.insert(idx, self.row_positions[idx - 1] + h)
                 idx += 1
-                self.row_positions[idx:] = [
-                    e + h
-                    for e in islice(self.row_positions, idx, len(self.row_positions))
-                ]
+                self.row_positions[idx:] = [e + h for e in islice(self.row_positions, idx, len(self.row_positions))]
 
     def insert_cols_rc(self, event=None):
         if self.anything_selected(exclude_rows=True, exclude_cells=True):
             selcols = self.get_selected_cols()
             numcols = len(selcols)
             displayed_ins_col = min(selcols) if event == "left" else max(selcols) + 1
             if self.all_columns_displayed:
@@ -4399,34 +3880,30 @@
                 if displayed_ins_col == len(self.col_positions) - 1:
                     rowlen = len(max(self.data, key=len)) if self.data else 0
                     data_ins_col = rowlen
                 else:
                     try:
                         data_ins_col = int(self.displayed_columns[displayed_ins_col])
                     except Exception:
-                        data_ins_col = int(
-                            self.displayed_columns[displayed_ins_col - 1]
-                        )
+                        data_ins_col = int(self.displayed_columns[displayed_ins_col - 1])
         else:
             numcols = 1
             displayed_ins_col = len(self.col_positions) - 1
             data_ins_col = int(displayed_ins_col)
         if (
             isinstance(self.paste_insert_column_limit, int)
             and self.paste_insert_column_limit < displayed_ins_col + numcols
         ):
             numcols = self.paste_insert_column_limit - len(self.col_positions) - 1
             if numcols < 1:
                 return
         if self.extra_begin_insert_cols_rc_func is not None:
             try:
                 self.extra_begin_insert_cols_rc_func(
-                    InsertEvent(
-                        "begin_insert_columns", data_ins_col, displayed_ins_col, numcols
-                    )
+                    InsertEvent("begin_insert_columns", data_ins_col, displayed_ins_col, numcols)
                 )
             except Exception:
                 return
         saved_displayed_columns = list(self.displayed_columns)
         if not self.all_columns_displayed:
             if displayed_ins_col == len(self.col_positions) - 1:
                 self.displayed_columns += list(range(rowlen, rowlen + numcols))
@@ -4441,61 +3918,41 @@
                         self.displayed_columns[adj_ins],
                         self.displayed_columns[adj_ins] + numcols + 1,
                     )
                 )
                 part3 = (
                     []
                     if displayed_ins_col > len(self.displayed_columns) - 1
-                    else [
-                        cn + numcols
-                        for cn in islice(self.displayed_columns, adj_ins + 1, None)
-                    ]
+                    else [cn + numcols for cn in islice(self.displayed_columns, adj_ins + 1, None)]
                 )
                 self.displayed_columns = part1 + part2 + part3
-        self.insert_col_positions(
-            idx=displayed_ins_col, widths=numcols, deselect_all=True
-        )
+        self.insert_col_positions(idx=displayed_ins_col, widths=numcols, deselect_all=True)
         self.cell_options = {
-            (rn, cn if cn < data_ins_col else cn + numcols): t2
-            for (rn, cn), t2 in self.cell_options.items()
-        }
-        self.col_options = {
-            cn if cn < data_ins_col else cn + numcols: t
-            for cn, t in self.col_options.items()
-        }
-        self.CH.cell_options = {
-            cn if cn < data_ins_col else cn + numcols: t
-            for cn, t in self.CH.cell_options.items()
+            (rn, cn if cn < data_ins_col else cn + numcols): t2 for (rn, cn), t2 in self.cell_options.items()
         }
+        self.col_options = {cn if cn < data_ins_col else cn + numcols: t for cn, t in self.col_options.items()}
+        self.CH.cell_options = {cn if cn < data_ins_col else cn + numcols: t for cn, t in self.CH.cell_options.items()}
         self.CH.fix_header()
         if self._headers and isinstance(self._headers, list):
             if data_ins_col >= len(self._headers):
                 self.CH.fix_header(
                     datacn=data_ins_col,
                     fix_values=(data_ins_col, data_ins_col + numcols),
                 )
             else:
                 self._headers[data_ins_col:data_ins_col] = self.CH.get_empty_header_seq(
                     end=data_ins_col + numcols, start=data_ins_col, c_ops=False
                 )
         if self.row_positions == [0] and not self.data:
-            self.insert_row_position(
-                idx="end", height=int(self.min_row_height), deselect_all=False
-            )
-            self.data.append(
-                self.get_empty_row_seq(
-                    0, end=data_ins_col + numcols, start=data_ins_col, c_ops=False
-                )
-            )
+            self.insert_row_position(idx="end", height=int(self.min_row_height), deselect_all=False)
+            self.data.append(self.get_empty_row_seq(0, end=data_ins_col + numcols, start=data_ins_col, c_ops=False))
         else:
             end = data_ins_col + numcols
             for rn in range(len(self.data)):
-                self.data[rn][data_ins_col:data_ins_col] = self.get_empty_row_seq(
-                    rn, end, data_ins_col, c_ops=False
-                )
+                self.data[rn][data_ins_col:data_ins_col] = self.get_empty_row_seq(rn, end, data_ins_col, c_ops=False)
         self.create_selected(
             0,
             displayed_ins_col,
             len(self.row_positions) - 1,
             displayed_ins_col + numcols,
             "columns",
         )
@@ -4515,17 +3972,15 @@
                         )
                     )
                 )
             )
         self.refresh()
         if self.extra_end_insert_cols_rc_func is not None:
             self.extra_end_insert_cols_rc_func(
-                InsertEvent(
-                    "end_insert_columns", data_ins_col, displayed_ins_col, numcols
-                )
+                InsertEvent("end_insert_columns", data_ins_col, displayed_ins_col, numcols)
             )
         self.parentframe.emit_event("<<SheetModified>>")
 
     def insert_rows_rc(self, event=None):
         if self.anything_selected(exclude_columns=True, exclude_cells=True):
             selrows = self.get_selected_rows()
             numrows = len(selrows)
@@ -4541,27 +3996,22 @@
                         data_ins_row = int(self.displayed_rows[displayed_ins_row])
                     except Exception:
                         data_ins_row = int(self.displayed_rows[displayed_ins_row - 1])
         else:
             numrows = 1
             displayed_ins_row = len(self.row_positions) - 1
             data_ins_row = int(displayed_ins_row)
-        if (
-            isinstance(self.paste_insert_row_limit, int)
-            and self.paste_insert_row_limit < displayed_ins_row + numrows
-        ):
+        if isinstance(self.paste_insert_row_limit, int) and self.paste_insert_row_limit < displayed_ins_row + numrows:
             numrows = self.paste_insert_row_limit - len(self.row_positions) - 1
             if numrows < 1:
                 return
         if self.extra_begin_insert_rows_rc_func is not None:
             try:
                 self.extra_begin_insert_rows_rc_func(
-                    InsertEvent(
-                        "begin_insert_rows", data_ins_row, displayed_ins_row, numrows
-                    )
+                    InsertEvent("begin_insert_rows", data_ins_row, displayed_ins_row, numrows)
                 )
             except Exception:
                 return
         saved_displayed_rows = list(self.displayed_rows)
         if not self.all_rows_displayed:
             if displayed_ins_row == len(self.row_positions) - 1:
                 self.displayed_rows += list(range(datalen, datalen + numrows))
@@ -4576,55 +4026,37 @@
                         self.displayed_rows[adj_ins],
                         self.displayed_rows[adj_ins] + numrows + 1,
                     )
                 )
                 part3 = (
                     []
                     if displayed_ins_row > len(self.displayed_rows) - 1
-                    else [
-                        rn + numrows
-                        for rn in islice(self.displayed_rows, adj_ins + 1, None)
-                    ]
+                    else [rn + numrows for rn in islice(self.displayed_rows, adj_ins + 1, None)]
                 )
                 self.displayed_rows = part1 + part2 + part3
-        self.insert_row_positions(
-            idx=displayed_ins_row, heights=numrows, deselect_all=True
-        )
+        self.insert_row_positions(idx=displayed_ins_row, heights=numrows, deselect_all=True)
         self.cell_options = {
-            (rn if rn < data_ins_row else rn + numrows, cn): t2
-            for (rn, cn), t2 in self.cell_options.items()
-        }
-        self.row_options = {
-            rn if rn < data_ins_row else rn + numrows: t
-            for rn, t in self.row_options.items()
-        }
-        self.RI.cell_options = {
-            rn if rn < data_ins_row else rn + numrows: t
-            for rn, t in self.RI.cell_options.items()
+            (rn if rn < data_ins_row else rn + numrows, cn): t2 for (rn, cn), t2 in self.cell_options.items()
         }
+        self.row_options = {rn if rn < data_ins_row else rn + numrows: t for rn, t in self.row_options.items()}
+        self.RI.cell_options = {rn if rn < data_ins_row else rn + numrows: t for rn, t in self.RI.cell_options.items()}
         self.RI.fix_index()
         if self._row_index and isinstance(self._row_index, list):
             if data_ins_row >= len(self._row_index):
                 self.RI.fix_index(
                     datacn=data_ins_row,
                     fix_values=(data_ins_row, data_ins_row + numrows),
                 )
             else:
-                self._row_index[
-                    data_ins_row:data_ins_row
-                ] = self.RI.get_empty_index_seq(
+                self._row_index[data_ins_row:data_ins_row] = self.RI.get_empty_index_seq(
                     data_ins_row + numrows, data_ins_row, r_ops=False
                 )
         if self.col_positions == [0] and not self.data:
             self.insert_col_position(idx="end", width=None, deselect_all=False)
-            self.data.append(
-                self.get_empty_row_seq(
-                    0, end=data_ins_row + numrows, start=data_ins_row, r_ops=False
-                )
-            )
+            self.data.append(self.get_empty_row_seq(0, end=data_ins_row + numrows, start=data_ins_row, r_ops=False))
         else:
             total_data_cols = self.total_data_cols()
             self.data[data_ins_row:data_ins_row] = [
                 self.get_empty_row_seq(rn, total_data_cols, r_ops=False)
                 for rn in range(data_ins_row, data_ins_row + numrows)
             ]
         self.create_selected(
@@ -4649,69 +4081,53 @@
                             },
                         )
                     )
                 )
             )
         self.refresh()
         if self.extra_end_insert_rows_rc_func is not None:
-            self.extra_end_insert_rows_rc_func(
-                InsertEvent("end_insert_rows", data_ins_row, displayed_ins_row, numrows)
-            )
+            self.extra_end_insert_rows_rc_func(InsertEvent("end_insert_rows", data_ins_row, displayed_ins_row, numrows))
         self.parentframe.emit_event("<<SheetModified>>")
 
     def del_cols_rc(self, event=None):
         seld_cols = sorted(self.get_selected_cols())
         if not seld_cols:
             return
         seldmax = seld_cols[-1] if self.all_columns_displayed else self.displayed_columns[seld_cols[-1]]
         if self.extra_begin_del_cols_rc_func is not None:
             try:
-                self.extra_begin_del_cols_rc_func(
-                    DeleteRowColumnEvent("begin_delete_columns", seld_cols)
-                )
+                self.extra_begin_del_cols_rc_func(DeleteRowColumnEvent("begin_delete_columns", seld_cols))
             except Exception:
                 return
-        seldset = (
-            set(seld_cols)
-            if self.all_columns_displayed
-            else set(self.displayed_columns[c] for c in seld_cols)
-        )
+        seldset = set(seld_cols) if self.all_columns_displayed else set(self.displayed_columns[c] for c in seld_cols)
         if self.undo_enabled:
             undo_storage = {
                 "deleted_cols": {},
                 "colwidths": {},
                 "deleted_header_values": {},
                 "selection_boxes": self.get_boxes(),
                 "displayed_columns": list(self.displayed_columns)
                 if not isinstance(self.displayed_columns, int)
                 else int(self.displayed_columns),
                 "cell_options": {k: v.copy() for k, v in self.cell_options.items()},
                 "col_options": {k: v.copy() for k, v in self.col_options.items()},
-                "CH_cell_options": {
-                    k: v.copy() for k, v in self.CH.cell_options.items()
-                },
+                "CH_cell_options": {k: v.copy() for k, v in self.CH.cell_options.items()},
             }
             for c in reversed(seld_cols):
-                undo_storage["colwidths"][c] = (
-                    self.col_positions[c + 1] - self.col_positions[c]
-                )
+                undo_storage["colwidths"][c] = self.col_positions[c + 1] - self.col_positions[c]
                 datacn = c if self.all_columns_displayed else self.displayed_columns[c]
                 for rn in range(len(self.data)):
                     if datacn not in undo_storage["deleted_cols"]:
                         undo_storage["deleted_cols"][datacn] = {}
                     try:
-                        undo_storage["deleted_cols"][datacn][rn] = self.data[rn].pop(
-                            datacn
-                        )
+                        undo_storage["deleted_cols"][datacn][rn] = self.data[rn].pop(datacn)
                     except Exception:
                         continue
                 try:
-                    undo_storage["deleted_header_values"][datacn] = self._headers.pop(
-                        datacn
-                    )
+                    undo_storage["deleted_header_values"][datacn] = self._headers.pop(datacn)
                 except Exception:
                     continue
         else:
             for c in reversed(seld_cols):
                 datacn = c if self.all_columns_displayed else self.displayed_columns[c]
                 for rn in range(len(self.data)):
                     del self.data[rn][datacn]
@@ -4720,89 +4136,67 @@
                 except Exception:
                     continue
         if self.undo_enabled:
             self.undo_storage.append(("delete_cols", undo_storage))
         for c in reversed(seld_cols):
             self.del_col_position(c, deselect_all=False)
         numcols = len(seld_cols)
-        
+
         self.cell_options = {
             (rn, cn if cn < seldmax else cn - numcols): t2
             for (rn, cn), t2 in self.cell_options.items()
             if cn not in seldset
         }
         self.col_options = {
-            cn if cn < seldmax else cn - numcols: t
-            for cn, t in self.col_options.items()
-            if cn not in seldset
+            cn if cn < seldmax else cn - numcols: t for cn, t in self.col_options.items() if cn not in seldset
         }
         self.CH.cell_options = {
-            cn if cn < seldmax else cn - numcols: t
-            for cn, t in self.CH.cell_options.items()
-            if cn not in seldset
+            cn if cn < seldmax else cn - numcols: t for cn, t in self.CH.cell_options.items() if cn not in seldset
         }
         self.deselect("allcols", redraw=False)
         self.set_current_to_last()
         if not self.all_columns_displayed:
-            self.displayed_columns = [
-                c for c in self.displayed_columns if c not in seldset
-            ]
+            self.displayed_columns = [c for c in self.displayed_columns if c not in seldset]
             for c in sorted(seldset):
-                self.displayed_columns = [
-                    dc if c > dc else dc - 1 for dc in self.displayed_columns
-                ]
+                self.displayed_columns = [dc if c > dc else dc - 1 for dc in self.displayed_columns]
         self.refresh()
         if self.extra_end_del_cols_rc_func is not None:
-            self.extra_end_del_cols_rc_func(
-                DeleteRowColumnEvent("end_delete_columns", seld_cols)
-            )
+            self.extra_end_del_cols_rc_func(DeleteRowColumnEvent("end_delete_columns", seld_cols))
         self.parentframe.emit_event("<<SheetModified>>")
 
     def del_rows_rc(self, event=None):
         seld_rows = sorted(self.get_selected_rows())
         if not seld_rows:
             return
         seldmax = seld_rows[-1] if self.all_rows_displayed else self.displayed_rows[seld_rows[-1]]
         if self.extra_begin_del_rows_rc_func is not None:
             try:
-                self.extra_begin_del_rows_rc_func(
-                    DeleteRowColumnEvent("begin_delete_rows", seld_rows)
-                )
+                self.extra_begin_del_rows_rc_func(DeleteRowColumnEvent("begin_delete_rows", seld_rows))
             except Exception:
                 return
-        seldset = (
-            set(seld_rows)
-            if self.all_rows_displayed
-            else set(self.displayed_rows[r] for r in seld_rows)
-        )
+        seldset = set(seld_rows) if self.all_rows_displayed else set(self.displayed_rows[r] for r in seld_rows)
         if self.undo_enabled:
             undo_storage = {
                 "deleted_rows": [],
                 "rowheights": {},
                 "deleted_index_values": [],
                 "selection_boxes": self.get_boxes(),
                 "displayed_rows": list(self.displayed_rows)
                 if not isinstance(self.displayed_rows, int)
                 else int(self.displayed_rows),
                 "cell_options": {k: v.copy() for k, v in self.cell_options.items()},
                 "row_options": {k: v.copy() for k, v in self.row_options.items()},
-                "RI_cell_options": {
-                    k: v.copy() for k, v in self.RI.cell_options.items()
-                },
+                "RI_cell_options": {k: v.copy() for k, v in self.RI.cell_options.items()},
             }
             for r in reversed(seld_rows):
-                undo_storage["rowheights"][r] = (
-                    self.row_positions[r + 1] - self.row_positions[r]
-                )
+                undo_storage["rowheights"][r] = self.row_positions[r + 1] - self.row_positions[r]
                 datarn = r if self.all_rows_displayed else self.displayed_rows[r]
                 undo_storage["deleted_rows"].append((datarn, self.data.pop(datarn)))
                 try:
-                    undo_storage["deleted_index_values"].append(
-                        (datarn, self._row_index.pop(datarn))
-                    )
+                    undo_storage["deleted_index_values"].append((datarn, self._row_index.pop(datarn)))
                 except Exception:
                     continue
         else:
             for r in reversed(seld_rows):
                 datarn = r if self.all_rows_displayed else self.displayed_rows[r]
                 del self.data[datarn]
                 try:
@@ -4810,37 +4204,31 @@
                 except Exception:
                     continue
         if self.undo_enabled:
             self.undo_storage.append(("delete_rows", undo_storage))
         for r in reversed(seld_rows):
             self.del_row_position(r, deselect_all=False)
         numrows = len(seld_rows)
-        
+
         self.cell_options = {
             (rn if rn < seldmax else rn - numrows, cn): t2
             for (rn, cn), t2 in self.cell_options.items()
             if rn not in seldset
         }
         self.row_options = {
-            rn if rn < seldmax else rn - numrows: t
-            for rn, t in self.row_options.items()
-            if rn not in seldset
+            rn if rn < seldmax else rn - numrows: t for rn, t in self.row_options.items() if rn not in seldset
         }
         self.RI.cell_options = {
-            rn if rn < seldmax else rn - numrows: t
-            for rn, t in self.RI.cell_options.items()
-            if rn not in seldset
+            rn if rn < seldmax else rn - numrows: t for rn, t in self.RI.cell_options.items() if rn not in seldset
         }
         self.deselect("allrows", redraw=False)
         self.set_current_to_last()
         self.refresh()
         if self.extra_end_del_rows_rc_func is not None:
-            self.extra_end_del_rows_rc_func(
-                DeleteRowColumnEvent("end_delete_rows", seld_rows)
-            )
+            self.extra_end_del_rows_rc_func(DeleteRowColumnEvent("end_delete_rows", seld_rows))
         self.parentframe.emit_event("<<SheetModified>>")
 
     def move_row_position(self, idx1, idx2):
         if not len(self.row_positions) <= 2:
             if idx1 < idx2:
                 height = self.row_positions[idx1 + 1] - self.row_positions[idx1]
                 self.row_positions.insert(idx2 + 1, self.row_positions.pop(idx1 + 1))
@@ -4873,23 +4261,17 @@
         self,
         rows=None,
         all_rows_displayed=None,
         reset_row_positions=True,
         deselect_all=True,
     ):
         if rows is None and all_rows_displayed is None:
-            return (
-                list(range(self.total_data_rows()))
-                if self.all_rows_displayed
-                else self.displayed_rows
-            )
+            return list(range(self.total_data_rows())) if self.all_rows_displayed else self.displayed_rows
         total_data_rows = None
-        if (rows is not None and rows != self.displayed_rows) or (
-            all_rows_displayed and not self.all_rows_displayed
-        ):
+        if (rows is not None and rows != self.displayed_rows) or (all_rows_displayed and not self.all_rows_displayed):
             self.undo_storage = deque(maxlen=self.max_undos)
         if rows is not None and rows != self.displayed_rows:
             self.displayed_rows = sorted(rows)
         if all_rows_displayed:
             if not self.all_rows_displayed:
                 total_data_rows = self.total_data_rows()
                 self.displayed_rows = list(range(total_data_rows))
@@ -4905,19 +4287,15 @@
         self,
         columns=None,
         all_columns_displayed=None,
         reset_col_positions=True,
         deselect_all=True,
     ):
         if columns is None and all_columns_displayed is None:
-            return (
-                list(range(self.total_data_cols()))
-                if self.all_columns_displayed
-                else self.displayed_columns
-            )
+            return list(range(self.total_data_cols())) if self.all_columns_displayed else self.displayed_columns
         total_data_cols = None
         if (columns is not None and columns != self.displayed_columns) or (
             all_columns_displayed and not self.all_columns_displayed
         ):
             self.undo_storage = deque(maxlen=self.max_undos)
         if columns is not None and columns != self.displayed_columns:
             self.displayed_columns = sorted(columns)
@@ -4939,61 +4317,49 @@
         index=None,
         reset_col_positions=False,
         show_headers_if_not_sheet=True,
         redraw=False,
     ):
         if newheaders is not None:
             if isinstance(newheaders, (list, tuple)):
-                self._headers = (
-                    list(newheaders) if isinstance(newheaders, tuple) else newheaders
-                )
+                self._headers = list(newheaders) if isinstance(newheaders, tuple) else newheaders
             elif isinstance(newheaders, int):
                 self._headers = int(newheaders)
             elif isinstance(self._headers, list) and isinstance(index, int):
                 if index >= len(self._headers):
                     self.CH.fix_header(index)
                 self._headers[index] = f"{newheaders}"
             elif not isinstance(newheaders, (list, tuple, int)) and index is None:
                 try:
                     self._headers = list(newheaders)
                 except Exception:
-                    raise ValueError(
-                        "New header must be iterable or int (use int to use a row as the header"
-                    )
+                    raise ValueError("New header must be iterable or int (use int to use a row as the header")
             if reset_col_positions:
                 self.reset_col_positions()
             elif (
                 show_headers_if_not_sheet
                 and isinstance(self._headers, list)
                 and (self.col_positions == [0] or not self.col_positions)
             ):
                 colpos = int(self.default_column_width)
                 if self.all_columns_displayed:
-                    self.col_positions = list(
-                        accumulate(
-                            chain([0], (colpos for c in range(len(self._headers))))
-                        )
-                    )
+                    self.col_positions = list(accumulate(chain([0], (colpos for c in range(len(self._headers))))))
                 else:
                     self.col_positions = list(
                         accumulate(
                             chain(
                                 [0],
                                 (colpos for c in range(len(self.displayed_columns))),
                             )
                         )
                     )
             if redraw:
                 self.refresh()
         else:
-            if (
-                not isinstance(self._headers, int)
-                and index is not None
-                and isinstance(index, int)
-            ):
+            if not isinstance(self._headers, int) and index is not None and isinstance(index, int):
                 return self._headers[index]
             else:
                 return self._headers
 
     def row_index(
         self,
         newindex=None,
@@ -5002,61 +4368,43 @@
         show_index_if_not_sheet=True,
         redraw=False,
     ):
         if newindex is not None:
             if not self._row_index and not isinstance(self._row_index, int):
                 self.RI.set_width(self.default_index_width, set_TL=True)
             if isinstance(newindex, (list, tuple)):
-                self._row_index = (
-                    list(newindex) if isinstance(newindex, tuple) else newindex
-                )
+                self._row_index = list(newindex) if isinstance(newindex, tuple) else newindex
             elif isinstance(newindex, int):
                 self._row_index = int(newindex)
             elif isinstance(index, int):
                 if index >= len(self._row_index):
                     self.RI.fix_index(index)
                 self._row_index[index] = f"{newindex}"
             elif not isinstance(newindex, (list, tuple, int)) and index is None:
                 try:
                     self._row_index = list(newindex)
                 except Exception:
-                    raise ValueError(
-                        "New index must be iterable or int (use int to use a column as the index"
-                    )
+                    raise ValueError("New index must be iterable or int (use int to use a column as the index")
             if reset_row_positions:
                 self.reset_row_positions()
             elif (
                 show_index_if_not_sheet
                 and isinstance(self._row_index, list)
                 and (self.row_positions == [0] or not self.row_positions)
             ):
                 rowpos = self.default_row_height[1]
                 if self.all_rows_displayed:
-                    self.row_positions = list(
-                        accumulate(
-                            chain([0], (rowpos for r in range(len(self._row_index))))
-                        )
-                    )
+                    self.row_positions = list(accumulate(chain([0], (rowpos for r in range(len(self._row_index))))))
                 else:
-                    self.row_positions = list(
-                        accumulate(
-                            chain(
-                                [0], (rowpos for r in range(len(self.displayed_rows)))
-                            )
-                        )
-                    )
+                    self.row_positions = list(accumulate(chain([0], (rowpos for r in range(len(self.displayed_rows))))))
 
             if redraw:
                 self.refresh()
         else:
-            if (
-                not isinstance(self._row_index, int)
-                and index is not None
-                and isinstance(index, int)
-            ):
+            if not isinstance(self._row_index, int) and index is not None and isinstance(index, int):
                 return self._row_index[index]
             else:
                 return self._row_index
 
     def total_data_cols(self, include_header=True):
         h_total = 0
         d_total = 0
@@ -5079,38 +4427,28 @@
         return i_total if i_total > d_total else d_total
 
     def data_dimensions(self, total_rows=None, total_columns=None):
         if total_rows is None and total_columns is None:
             return self.total_data_rows(), self.total_data_cols()
         if total_rows is not None:
             if len(self.data) < total_rows:
-                ncols = (
-                    self.total_data_cols() if total_columns is None else total_columns
-                )
-                self.data.extend(
-                    [
-                        self.get_empty_row_seq(r, ncols)
-                        for r in range(total_rows - len(self.data))
-                    ]
-                )
+                ncols = self.total_data_cols() if total_columns is None else total_columns
+                self.data.extend([self.get_empty_row_seq(r, ncols) for r in range(total_rows - len(self.data))])
             else:
                 self.data[total_rows:] = []
         if total_columns is not None:
             self.data[:] = [
                 r[:total_columns]
                 if len(r) > total_columns
-                else r
-                + self.get_empty_row_seq(rn, end=len(r) + total_columns - len(r), start=len(r))
+                else r + self.get_empty_row_seq(rn, end=len(r) + total_columns - len(r), start=len(r))
                 for rn, r in enumerate(self.data)
             ]
 
     def equalize_data_row_lengths(self, include_header=False, total_columns=None):
-        total_columns = (
-            self.total_data_cols() if total_columns is None else total_columns
-        )
+        total_columns = self.total_data_cols() if total_columns is None else total_columns
         if include_header and total_columns > len(self._headers):
             self.CH.fix_header(total_columns)
         self.data[:] = [
             (r + self.get_empty_row_seq(rn, end=len(r) + total_columns - len(r), start=len(r)))
             if total_columns > len(r)
             else r
             for rn, r in enumerate(self.data)
@@ -5204,16 +4542,15 @@
                 redrawn = self.redraw_highlight(
                     fc + 1,
                     fr + 1,
                     sc,
                     sr,
                     fill=fill,
                     outline=self.table_fg
-                    if self.get_cell_kwargs(datarn, datacn, key="dropdown")
-                    and self.show_dropdown_borders
+                    if self.get_cell_kwargs(datarn, datacn, key="dropdown") and self.show_dropdown_borders
                     else "",
                     tag="hi",
                     can_width=can_width if (len(kwargs) > 2 and kwargs[2]) else None,
                 )
         elif not kwargs:
             if "cells" in selections and (r, c) in selections["cells"]:
                 tf = self.table_selected_cells_fg
@@ -5221,43 +4558,37 @@
                 tf = self.table_selected_rows_fg
             elif "columns" in selections and c in selections["columns"]:
                 tf = self.table_selected_columns_fg
             else:
                 tf = self.table_fg
         return tf, redrawn
 
-    def redraw_highlight(
-        self, x1, y1, x2, y2, fill, outline, tag, can_width=None, pc=None
-    ):
+    def redraw_highlight(self, x1, y1, x2, y2, fill, outline, tag, can_width=None, pc=None):
         config = (fill, outline)
         if type(pc) != int or pc >= 100 or pc <= 0:
             coords = (
                 x1 - 1 if outline else x1,
                 y1 - 1 if outline else y1,
                 x2 if can_width is None else x2 + can_width,
                 y2,
             )
         else:
             coords = (x1, y1, (x2 - x1) * (pc / 100), y2)
         k = None
         if config in self.hidd_high:
             k = config
             iid, showing = self.hidd_high[k].pop()
-            if all(
-                int(crd1) == int(crd2) for crd1, crd2 in zip(self.coords(iid), coords)
-            ):
+            if all(int(crd1) == int(crd2) for crd1, crd2 in zip(self.coords(iid), coords)):
                 option = 0 if showing else 2
             else:
                 option = 1 if showing else 3
         elif self.hidd_high:
             k = next(iter(self.hidd_high))
             iid, showing = self.hidd_high[k].pop()
-            if all(
-                int(crd1) == int(crd2) for crd1, crd2 in zip(self.coords(iid), coords)
-            ):
+            if all(int(crd1) == int(crd2) for crd1, crd2 in zip(self.coords(iid), coords)):
                 option = 2 if showing else 3
             else:
                 option = 3
         else:
             iid, showing, option = (
                 self.create_rectangle(coords, fill=fill, outline=outline, tag=tag),
                 1,
@@ -5265,17 +4596,15 @@
             )
         if option in (1, 3):
             self.coords(iid, coords)
         if option in (2, 3):
             if showing:
                 self.itemconfig(iid, fill=fill, outline=outline)
             else:
-                self.itemconfig(
-                    iid, fill=fill, outline=outline, tag=tag, state="normal"
-                )
+                self.itemconfig(iid, fill=fill, outline=outline, tag=tag, state="normal")
         if k is not None and not self.hidd_high[k]:
             del self.hidd_high[k]
         self.disp_high[config].add(DrawnItem(iid=iid, showing=1))
         return True
 
     def redraw_dropdown(
         self,
@@ -5287,17 +4616,15 @@
         outline,
         tag,
         draw_outline=True,
         draw_arrow=True,
         dd_is_open=False,
     ):
         if draw_outline and self.show_dropdown_borders:
-            self.redraw_highlight(
-                x1 + 1, y1 + 1, x2, y2, fill="", outline=self.table_fg, tag=tag
-            )
+            self.redraw_highlight(x1 + 1, y1 + 1, x2, y2, fill="", outline=self.table_fg, tag=tag)
         if draw_arrow:
             topysub = floor(self.half_txt_h / 2)
             mid_y = y1 + floor(self.min_row_height / 2)
             if mid_y + topysub + 1 >= y1 + self.txt_h - 1:
                 mid_y -= 1
             if mid_y - topysub + 2 <= y1 + 4 + topysub:
                 mid_y -= 1
@@ -5386,43 +4713,35 @@
             self.coords(t, points)
             if sh:
                 self.itemconfig(t, fill=outline, outline=fill)
             else:
                 self.itemconfig(t, fill=outline, outline=fill, tag=tag, state="normal")
             self.lift(t)
         else:
-            t = self.create_polygon(
-                points, fill=outline, outline=fill, tag=tag, smooth=True
-            )
+            t = self.create_polygon(points, fill=outline, outline=fill, tag=tag, smooth=True)
         self.disp_checkbox[t] = True
         if draw_check:
             x1 = x1 + 4
             y1 = y1 + 4
             x2 = x2 - 3
             y2 = y2 - 3
             points = self.get_checkbox_points(x1, y1, x2, y2, radius=4)
             if self.hidd_checkbox:
                 t, sh = self.hidd_checkbox.popitem()
                 self.coords(t, points)
                 if sh:
                     self.itemconfig(t, fill=fill, outline=outline)
                 else:
-                    self.itemconfig(
-                        t, fill=fill, outline=outline, tag=tag, state="normal"
-                    )
+                    self.itemconfig(t, fill=fill, outline=outline, tag=tag, state="normal")
                 self.lift(t)
             else:
-                t = self.create_polygon(
-                    points, fill=fill, outline=outline, tag=tag, smooth=True
-                )
+                t = self.create_polygon(points, fill=fill, outline=outline, tag=tag, smooth=True)
             self.disp_checkbox[t] = True
 
-    def main_table_redraw_grid_and_text(
-        self, redraw_header=False, redraw_row_index=False, redraw_table=True
-    ):
+    def main_table_redraw_grid_and_text(self, redraw_header=False, redraw_row_index=False, redraw_table=True):
         last_col_line_pos = self.col_positions[-1] + 1
         last_row_line_pos = self.row_positions[-1] + 1
         try:
             can_width = self.winfo_width()
             can_height = self.winfo_height()
             self.configure(
                 scrollregion=(
@@ -5430,32 +4749,26 @@
                     0,
                     last_col_line_pos + self.empty_horizontal,
                     last_row_line_pos + self.empty_vertical,
                 )
             )
         except Exception:
             return
-        if (
-            can_width >= last_col_line_pos + self.empty_horizontal
-            and self.parentframe.xscroll_showing
-        ):
+        if can_width >= last_col_line_pos + self.empty_horizontal and self.parentframe.xscroll_showing:
             self.parentframe.xscroll.grid_forget()
             self.parentframe.xscroll_showing = False
         elif (
             can_width < last_col_line_pos + self.empty_horizontal
             and not self.parentframe.xscroll_showing
             and not self.parentframe.xscroll_disabled
             and can_height > 45
         ):
             self.parentframe.xscroll.grid(row=2, column=0, columnspan=2, sticky="nswe")
             self.parentframe.xscroll_showing = True
-        if (
-            can_height >= last_row_line_pos + self.empty_vertical
-            and self.parentframe.yscroll_showing
-        ):
+        if can_height >= last_row_line_pos + self.empty_vertical and self.parentframe.yscroll_showing:
             self.parentframe.yscroll.grid_forget()
             self.parentframe.yscroll_showing = False
         elif (
             can_height < last_row_line_pos + self.empty_vertical
             and not self.parentframe.yscroll_showing
             and not self.parentframe.yscroll_disabled
             and can_width > 45
@@ -5533,30 +4846,26 @@
                     points.extend(
                         [
                             self.canvasx(0) - 1,
                             draw_y,
                             x_grid_stop,
                             draw_y,
                             x_grid_stop,
-                            self.row_positions[r + 1]
-                            if len(self.row_positions) - 1 > r
-                            else draw_y,
+                            self.row_positions[r + 1] if len(self.row_positions) - 1 > r else draw_y,
                         ]
                     )
                 elif st_or_end == "end":
                     points.extend(
                         [
                             x_grid_stop,
                             draw_y,
                             self.canvasx(0) - 1,
                             draw_y,
                             self.canvasx(0) - 1,
-                            self.row_positions[r + 1]
-                            if len(self.row_positions) - 1 > r
-                            else draw_y,
+                            self.row_positions[r + 1] if len(self.row_positions) - 1 > r else draw_y,
                         ]
                     )
             if points:
                 if self.hidd_grid:
                     t, sh = self.hidd_grid.popitem()
                     self.coords(t, points)
                     if sh:
@@ -5604,30 +4913,26 @@
                 if st_or_end == "st":
                     points.extend(
                         [
                             draw_x,
                             scrollpos_top - 1,
                             draw_x,
                             y_grid_stop,
-                            self.col_positions[c + 1]
-                            if len(self.col_positions) - 1 > c
-                            else draw_x,
+                            self.col_positions[c + 1] if len(self.col_positions) - 1 > c else draw_x,
                             y_grid_stop,
                         ]
                     )
                 elif st_or_end == "end":
                     points.extend(
                         [
                             draw_x,
                             y_grid_stop,
                             draw_x,
                             scrollpos_top - 1,
-                            self.col_positions[c + 1]
-                            if len(self.col_positions) - 1 > c
-                            else draw_x,
+                            self.col_positions[c + 1] if len(self.col_positions) - 1 > c else draw_x,
                             scrollpos_top - 1,
                         ]
                     )
             if points:
                 if self.hidd_grid:
                     t, sh = self.hidd_grid.popitem()
                     self.coords(t, points)
@@ -5693,17 +4998,15 @@
                     rbotgridln = self.row_positions[r + 1]
                     if rbotgridln - rtopgridln < self.txt_h:
                         continue
                     cleftgridln = self.col_positions[c]
                     crightgridln = self.col_positions[c + 1]
 
                     datarn = r if self.all_rows_displayed else self.displayed_rows[r]
-                    datacn = (
-                        c if self.all_columns_displayed else self.displayed_columns[c]
-                    )
+                    datacn = c if self.all_columns_displayed else self.displayed_columns[c]
 
                     fill, dd_drawn = self.redraw_highlight_get_text_fg(
                         r,
                         c,
                         cleftgridln,
                         rtopgridln,
                         crightgridln,
@@ -5759,34 +5062,30 @@
                         else:
                             mw = crightgridln - cleftgridln - 1
                             draw_x = crightgridln - 3
                     elif align == "center":
                         stop = cleftgridln + 5
                         if kwargs:
                             mw = crightgridln - cleftgridln - self.txt_h - 2
-                            draw_x = cleftgridln + ceil(
-                                (crightgridln - cleftgridln - self.txt_h) / 2
-                            )
+                            draw_x = cleftgridln + ceil((crightgridln - cleftgridln - self.txt_h) / 2)
                             self.redraw_dropdown(
                                 cleftgridln,
                                 rtopgridln,
                                 crightgridln,
                                 self.row_positions[r + 1],
                                 fill=fill,
                                 outline=fill,
                                 tag=f"dd_{r}_{c}",
                                 draw_outline=not dd_drawn,
                                 draw_arrow=mw >= 5,
                                 dd_is_open=kwargs["window"] != "no dropdown open",
                             )
                         else:
                             mw = crightgridln - cleftgridln - 1
-                            draw_x = cleftgridln + floor(
-                                (crightgridln - cleftgridln) / 2
-                            )
+                            draw_x = cleftgridln + floor((crightgridln - cleftgridln) / 2)
                     kwargs = self.get_cell_kwargs(datarn, datacn, key="checkbox")
                     if kwargs:
                         if mw > self.txt_h + 2:
                             box_w = self.txt_h + 1
                             mw -= box_w
                             if align == "w":
                                 draw_x += box_w + 1
@@ -5800,71 +5099,58 @@
                             except Exception:
                                 draw_check = False
                             self.redraw_checkbox(
                                 cleftgridln + 2,
                                 rtopgridln + 2,
                                 cleftgridln + self.txt_h + 3,
                                 rtopgridln + self.txt_h + 3,
-                                fill=fill
-                                if kwargs["state"] == "normal"
-                                else self.table_grid_fg,
+                                fill=fill if kwargs["state"] == "normal" else self.table_grid_fg,
                                 outline="",
                                 tag="cb",
                                 draw_check=draw_check,
                             )
-                    lns = self.get_valid_cell_data_as_str(
-                        datarn, datacn, get_displayed=True
-                    ).split("\n")
+                    lns = self.get_valid_cell_data_as_str(datarn, datacn, get_displayed=True).split("\n")
                     if (
                         lns != [""]
                         and mw > self.txt_w
                         and not (
                             (align == "w" and draw_x > scrollpos_right)
                             or (align == "e" and cleftgridln + 5 > scrollpos_right)
                             or (align == "center" and stop > scrollpos_right)
                         )
                     ):
                         draw_y = rtopgridln + self.fl_ins
-                        start_ln = int(
-                            (scrollpos_top - rtopgridln) / self.xtra_lines_increment
-                        )
+                        start_ln = int((scrollpos_top - rtopgridln) / self.xtra_lines_increment)
                         if start_ln < 0:
                             start_ln = 0
                         draw_y += start_ln * self.xtra_lines_increment
-                        if (
-                            draw_y + self.half_txt_h - 1 <= rbotgridln
-                            and len(lns) > start_ln
-                        ):
+                        if draw_y + self.half_txt_h - 1 <= rbotgridln and len(lns) > start_ln:
                             for txt in islice(lns, start_ln, None):
                                 # for performance improvements in redrawing especially when just selecting cells
                                 # option 0: text doesn't need moving or config
                                 # option 1: text needs new x, y but has same config
                                 # option 2: text needs new config but has same x, y
                                 # option 3: text needs new x, y and new config
                                 # option 4: text needs to be created
                                 config = TextCfg(txt, fill, font, align)
                                 k = None
                                 if config in self.hidd_text:
                                     k = config
                                     iid, showing = self.hidd_text[k].pop()
                                     cc1, cc2 = self.coords(iid)
-                                    if int(cc1) == int(draw_x) and int(cc2) == int(
-                                        draw_y
-                                    ):
+                                    if int(cc1) == int(draw_x) and int(cc2) == int(draw_y):
                                         option = 0 if showing else 2
                                     else:
                                         option = 1 if showing else 3
                                     self.tag_raise(iid)
                                 elif self.hidd_text:
                                     k = next(iter(self.hidd_text))
                                     iid, showing = self.hidd_text[k].pop()
                                     cc1, cc2 = self.coords(iid)
-                                    if int(cc1) == int(draw_x) and int(cc2) == int(
-                                        draw_y
-                                    ):
+                                    if int(cc1) == int(draw_x) and int(cc2) == int(draw_y):
                                         option = 2 if showing else 3
                                     else:
                                         option = 3
                                     self.tag_raise(iid)
                                 else:
                                     iid, showing, option = (
                                         self.create_text(
@@ -5909,45 +5195,35 @@
                                         self.itemconfig(iid, text=txt)
                                         wd = self.bbox(iid)
                                         while wd[2] - wd[0] > mw:
                                             txt = txt[:-1]
                                             self.itemconfig(iid, text=txt)
                                             wd = self.bbox(iid)
                                     elif align == "e":
-                                        txt = txt[
-                                            len(txt) - int(len(txt) * (mw / wd)) :
-                                        ]
+                                        txt = txt[len(txt) - int(len(txt) * (mw / wd)) :]
                                         self.itemconfig(iid, text=txt)
                                         wd = self.bbox(iid)
                                         while wd[2] - wd[0] > mw:
                                             txt = txt[1:]
                                             self.itemconfig(iid, text=txt)
                                             wd = self.bbox(iid)
                                     elif align == "center":
-                                        self.c_align_cyc = cycle(
-                                            self.centre_alignment_text_mod_indexes
-                                        )
-                                        tmod = ceil(
-                                            (len(txt) - int(len(txt) * (mw / wd))) / 2
-                                        )
+                                        self.c_align_cyc = cycle(self.centre_alignment_text_mod_indexes)
+                                        tmod = ceil((len(txt) - int(len(txt) * (mw / wd))) / 2)
                                         txt = txt[tmod - 1 : -tmod]
                                         self.itemconfig(iid, text=txt)
                                         wd = self.bbox(iid)
                                         while wd[2] - wd[0] > mw:
                                             txt = txt[next(self.c_align_cyc)]
                                             self.itemconfig(iid, text=txt)
                                             wd = self.bbox(iid)
                                         self.coords(iid, draw_x, draw_y)
-                                    self.disp_text[config._replace(txt=txt)].add(
-                                        DrawnItem(iid=iid, showing=True)
-                                    )
+                                    self.disp_text[config._replace(txt=txt)].add(DrawnItem(iid=iid, showing=True))
                                 else:
-                                    self.disp_text[config].add(
-                                        DrawnItem(iid=iid, showing=True)
-                                    )
+                                    self.disp_text[config].add(DrawnItem(iid=iid, showing=True))
                                 draw_y += self.xtra_lines_increment
                                 if draw_y + self.half_txt_h - 1 > rbotgridln:
                                     break
         if redraw_table:
             for cfg, set_ in self.hidd_text.items():
                 for namedtup in tuple(set_):
                     if namedtup.showing:
@@ -6015,17 +5291,15 @@
             if alltags[0] == "cells":
                 boxes[tuple(int(e) for e in alltags[1].split("_") if e)] = "cells"
             elif alltags[0] == "rows":
                 boxes[tuple(int(e) for e in alltags[1].split("_") if e)] = "rows"
             elif alltags[0] == "columns":
                 boxes[tuple(int(e) for e in alltags[1].split("_") if e)] = "columns"
             elif include_current and alltags[0] == "currently":
-                boxes[
-                    tuple(int(e) for e in alltags[1].split("_") if e)
-                ] = f"{alltags[2]}"
+                boxes[tuple(int(e) for e in alltags[1].split("_") if e)] = f"{alltags[2]}"
         return boxes
 
     def reselect_from_get_boxes(self, boxes):
         for (r1, c1, r2, c2), v in boxes.items():
             if r2 < len(self.row_positions) and c2 < len(self.col_positions):
                 if v == "cells":
                     self.create_selected(r1, c1, r2, c2, "cells")
@@ -6066,45 +5340,37 @@
         if type_ == "rows":
             return {"rows", "rowsbd"}
         elif type_ == "columns":
             return {"columns", "columnsbd"}
         else:
             return {"cells", "cellsbd", "rows", "rowsbd", "columns", "columnsbd"}
 
-    def delete_selection_rects(
-        self, cells=True, rows=True, cols=True, delete_current=True
-    ):
+    def delete_selection_rects(self, cells=True, rows=True, cols=True, delete_current=True):
         deleted_boxes = {}
         if cells:
             for item in self.find_withtag("cells"):
                 alltags = self.gettags(item)
                 if alltags:
-                    deleted_boxes[
-                        tuple(int(e) for e in alltags[1].split("_") if e)
-                    ] = "cells"
+                    deleted_boxes[tuple(int(e) for e in alltags[1].split("_") if e)] = "cells"
             self.delete("cells", "cellsbd")
             self.RI.delete("cells", "cellsbd")
             self.CH.delete("cells", "cellsbd")
         if rows:
             for item in self.find_withtag("rows"):
                 alltags = self.gettags(item)
                 if alltags:
-                    deleted_boxes[
-                        tuple(int(e) for e in alltags[1].split("_") if e)
-                    ] = "rows"
+                    deleted_boxes[tuple(int(e) for e in alltags[1].split("_") if e)] = "rows"
             self.delete("rows", "rowsbd")
             self.RI.delete("rows", "rowsbd")
             self.CH.delete("rows", "rowsbd")
         if cols:
             for item in self.find_withtag("columns"):
                 alltags = self.gettags(item)
                 if alltags:
-                    deleted_boxes[
-                        tuple(int(e) for e in alltags[1].split("_") if e)
-                    ] = "columns"
+                    deleted_boxes[tuple(int(e) for e in alltags[1].split("_") if e)] = "columns"
             self.delete("columns", "columnsbd")
             self.RI.delete("columns", "columnsbd")
             self.CH.delete("columns", "columnsbd")
         if delete_current:
             self.delete("currently")
             self.RI.delete("currently")
             self.CH.delete("currently")
@@ -6187,19 +5453,15 @@
         )
         self.RI.tag_lower(ri)
         self.CH.tag_lower(ch)
         return b
 
     def set_current_to_last(self):
         if not self.currently_selected():
-            items = sorted(
-                self.find_withtag("cells")
-                + self.find_withtag("rows")
-                + self.find_withtag("columns")
-            )
+            items = sorted(self.find_withtag("cells") + self.find_withtag("rows") + self.find_withtag("columns"))
             if items:
                 last = self.gettags(items[-1])
                 r1, c1, r2, c2 = tuple(int(e) for e in last[1].split("_") if e)
                 if last[0] == "cells":
                     return self.gettags(self.set_currently_selected(r1, c1, "cell"))
                 elif last[0] == "rows":
                     return self.gettags(self.set_currently_selected(r1, c1, "row"))
@@ -6242,51 +5504,41 @@
             mt_border_col = self.table_selected_columns_border_fg
         self.last_selected = (r1, c1, r2, c2, type_)
         ch_tags = tag_index_header if type_ == "rows" else tagr
         ri_tags = tag_index_header if type_ == "columns" else tagr
         r = self.create_rectangle(
             self.col_positions[c1],
             self.row_positions[r1],
-            self.canvasx(self.winfo_width())
-            if self.selected_rows_to_end_of_window
-            else self.col_positions[c2],
+            self.canvasx(self.winfo_width()) if self.selected_rows_to_end_of_window else self.col_positions[c2],
             self.row_positions[r2],
             fill=mt_bg,
             outline="",
             state=state,
             tags=tagr,
         )
         self.RI.create_rectangle(
             0,
             self.row_positions[r1],
             self.RI.current_width - 1,
             self.row_positions[r2],
-            fill=self.RI.index_selected_rows_bg
-            if type_ == "rows"
-            else self.RI.index_selected_cells_bg,
+            fill=self.RI.index_selected_rows_bg if type_ == "rows" else self.RI.index_selected_cells_bg,
             outline="",
             tags=ri_tags,
         )
         self.CH.create_rectangle(
             self.col_positions[c1],
             0,
             self.col_positions[c2],
             self.CH.current_height - 1,
-            fill=self.CH.header_selected_columns_bg
-            if type_ == "columns"
-            else self.CH.header_selected_cells_bg,
+            fill=self.CH.header_selected_columns_bg if type_ == "columns" else self.CH.header_selected_cells_bg,
             outline="",
             tags=ch_tags,
         )
         if self.show_selected_cells_border and (
-            (
-                self.being_drawn_rect is None
-                and self.RI.being_drawn_rect is None
-                and self.CH.being_drawn_rect is None
-            )
+            (self.being_drawn_rect is None and self.RI.being_drawn_rect is None and self.CH.being_drawn_rect is None)
             or len(self.anything_selected()) > 1
         ):
             b = self.create_rectangle(
                 self.col_positions[c1],
                 self.row_positions[r1],
                 self.col_positions[c2],
                 self.row_positions[r2],
@@ -6315,18 +5567,15 @@
         ):
             tags = self.gettags(item)
             if tags:
                 r1, c1, r2, c2 = tuple(int(e) for e in tags[1].split("_") if e)
                 self.delete(f"{r1}_{c1}_{r2}_{c2}")
                 self.RI.delete(f"{r1}_{c1}_{r2}_{c2}")
                 self.CH.delete(f"{r1}_{c1}_{r2}_{c2}")
-                if (
-                    r1 >= len(self.row_positions) - 1
-                    or c1 >= len(self.col_positions) - 1
-                ):
+                if r1 >= len(self.row_positions) - 1 or c1 >= len(self.col_positions) - 1:
                     continue
                 if r2 > len(self.row_positions) - 1:
                     r2 = len(self.row_positions) - 1
                 if c2 > len(self.col_positions) - 1:
                     c2 = len(self.col_positions) - 1
                 if tags[0] == "currently":
                     self.set_currently_selected(r1, c1, tags[2])
@@ -6357,83 +5606,59 @@
                 (r, c)
                 for r in range(startr, endr)
                 for c in range(startc, endc)
                 for r1, c1, r2, c2 in d["cells"]
                 if r1 <= r and c1 <= c and r2 > r and c2 > c
             }
         if "rows" in d:
-            d2["rows"] = {
-                r
-                for r in range(startr, endr)
-                for r1, c1, r2, c2 in d["rows"]
-                if r1 <= r and r2 > r
-            }
+            d2["rows"] = {r for r in range(startr, endr) for r1, c1, r2, c2 in d["rows"] if r1 <= r and r2 > r}
         if "columns" in d:
-            d2["columns"] = {
-                c
-                for c in range(startc, endc)
-                for r1, c1, r2, c2 in d["columns"]
-                if c1 <= c and c2 > c
-            }
+            d2["columns"] = {c for c in range(startc, endc) for r1, c1, r2, c2 in d["columns"] if c1 <= c and c2 > c}
         return d2
 
     def get_selected_min_max(self):
         min_x = float("inf")
         min_y = float("inf")
         max_x = 0
         max_y = 0
         for item in chain(
             self.find_withtag("cells"),
             self.find_withtag("rows"),
             self.find_withtag("columns"),
             self.find_withtag("currently"),
         ):
-            r1, c1, r2, c2 = tuple(
-                int(e) for e in self.gettags(item)[1].split("_") if e
-            )
+            r1, c1, r2, c2 = tuple(int(e) for e in self.gettags(item)[1].split("_") if e)
             if r1 < min_y:
                 min_y = r1
             if c1 < min_x:
                 min_x = c1
             if r2 > max_y:
                 max_y = r2
             if c2 > max_x:
                 max_x = c2
         if min_x != float("inf") and min_y != float("inf") and max_x > 0 and max_y > 0:
             return min_y, min_x, max_y, max_x
         else:
             return None, None, None, None
 
-    def get_selected_rows(
-        self, get_cells=False, within_range=None, get_cells_as_rows=False
-    ):
+    def get_selected_rows(self, get_cells=False, within_range=None, get_cells_as_rows=False):
         s = set()
         if within_range is not None:
             within_r1 = within_range[0]
             within_r2 = within_range[1]
         if get_cells:
             if within_range is None:
                 for item in self.find_withtag("rows"):
-                    r1, c1, r2, c2 = tuple(
-                        int(e) for e in self.gettags(item)[1].split("_") if e
-                    )
-                    s.update(
-                        set(
-                            product(
-                                range(r1, r2), range(0, len(self.col_positions) - 1)
-                            )
-                        )
-                    )
+                    r1, c1, r2, c2 = tuple(int(e) for e in self.gettags(item)[1].split("_") if e)
+                    s.update(set(product(range(r1, r2), range(0, len(self.col_positions) - 1))))
                 if get_cells_as_rows:
                     s.update(self.get_selected_cells())
             else:
                 for item in self.find_withtag("rows"):
-                    r1, c1, r2, c2 = tuple(
-                        int(e) for e in self.gettags(item)[1].split("_") if e
-                    )
+                    r1, c1, r2, c2 = tuple(int(e) for e in self.gettags(item)[1].split("_") if e)
                     if r1 >= within_r1 or r2 <= within_r2:
                         if r1 > within_r1:
                             start_row = r1
                         else:
                             start_row = within_r1
                         if r2 < within_r2:
                             end_row = r2
@@ -6457,25 +5682,21 @@
                                 len(self.col_positions) - 1,
                             )
                         )
                     )
         else:
             if within_range is None:
                 for item in self.find_withtag("rows"):
-                    r1, c1, r2, c2 = tuple(
-                        int(e) for e in self.gettags(item)[1].split("_") if e
-                    )
+                    r1, c1, r2, c2 = tuple(int(e) for e in self.gettags(item)[1].split("_") if e)
                     s.update(set(range(r1, r2)))
                 if get_cells_as_rows:
                     s.update(set(tup[0] for tup in self.get_selected_cells()))
             else:
                 for item in self.find_withtag("rows"):
-                    r1, c1, r2, c2 = tuple(
-                        int(e) for e in self.gettags(item)[1].split("_") if e
-                    )
+                    r1, c1, r2, c2 = tuple(int(e) for e in self.gettags(item)[1].split("_") if e)
                     if r1 >= within_r1 or r2 <= within_r2:
                         if r1 > within_r1:
                             start_row = r1
                         else:
                             start_row = within_r1
                         if r2 < within_r2:
                             end_row = r2
@@ -6494,41 +5715,29 @@
                                     len(self.col_positions) - 1,
                                 )
                             )
                         )
                     )
         return s
 
-    def get_selected_cols(
-        self, get_cells=False, within_range=None, get_cells_as_cols=False
-    ):
+    def get_selected_cols(self, get_cells=False, within_range=None, get_cells_as_cols=False):
         s = set()
         if within_range is not None:
             within_c1 = within_range[0]
             within_c2 = within_range[1]
         if get_cells:
             if within_range is None:
                 for item in self.find_withtag("columns"):
-                    r1, c1, r2, c2 = tuple(
-                        int(e) for e in self.gettags(item)[1].split("_") if e
-                    )
-                    s.update(
-                        set(
-                            product(
-                                range(c1, c2), range(0, len(self.row_positions) - 1)
-                            )
-                        )
-                    )
+                    r1, c1, r2, c2 = tuple(int(e) for e in self.gettags(item)[1].split("_") if e)
+                    s.update(set(product(range(c1, c2), range(0, len(self.row_positions) - 1))))
                 if get_cells_as_cols:
                     s.update(self.get_selected_cells())
             else:
                 for item in self.find_withtag("columns"):
-                    r1, c1, r2, c2 = tuple(
-                        int(e) for e in self.gettags(item)[1].split("_") if e
-                    )
+                    r1, c1, r2, c2 = tuple(int(e) for e in self.gettags(item)[1].split("_") if e)
                     if c1 >= within_c1 or c2 <= within_c2:
                         if c1 > within_c1:
                             start_col = c1
                         else:
                             start_col = within_c1
                         if c2 < within_c2:
                             end_col = c2
@@ -6552,25 +5761,21 @@
                                 within_c2,
                             )
                         )
                     )
         else:
             if within_range is None:
                 for item in self.find_withtag("columns"):
-                    r1, c1, r2, c2 = tuple(
-                        int(e) for e in self.gettags(item)[1].split("_") if e
-                    )
+                    r1, c1, r2, c2 = tuple(int(e) for e in self.gettags(item)[1].split("_") if e)
                     s.update(set(range(c1, c2)))
                 if get_cells_as_cols:
                     s.update(set(tup[1] for tup in self.get_selected_cells()))
             else:
                 for item in self.find_withtag("columns"):
-                    r1, c1, r2, c2 = tuple(
-                        int(e) for e in self.gettags(item)[1].split("_") if e
-                    )
+                    r1, c1, r2, c2 = tuple(int(e) for e in self.gettags(item)[1].split("_") if e)
                     if c1 >= within_c1 or c2 <= within_c2:
                         if c1 > within_c1:
                             start_col = c1
                         else:
                             start_col = within_c1
                         if c2 < within_c2:
                             end_col = c2
@@ -6610,29 +5815,20 @@
             iterable = chain(self.find_withtag("cells"), self.find_withtag("rows"))
         elif get_cols and not get_rows:
             iterable = chain(self.find_withtag("cells"), self.find_withtag("columns"))
         else:
             iterable = chain(self.find_withtag("cells"))
         if within_range is None:
             for item in iterable:
-                r1, c1, r2, c2 = tuple(
-                    int(e) for e in self.gettags(item)[1].split("_") if e
-                )
+                r1, c1, r2, c2 = tuple(int(e) for e in self.gettags(item)[1].split("_") if e)
                 s.update(set(product(range(r1, r2), range(c1, c2))))
         else:
             for item in iterable:
-                r1, c1, r2, c2 = tuple(
-                    int(e) for e in self.gettags(item)[1].split("_") if e
-                )
-                if (
-                    r1 >= within_r1
-                    or c1 >= within_c1
-                    or r2 <= within_r2
-                    or c2 <= within_c2
-                ):
+                r1, c1, r2, c2 = tuple(int(e) for e in self.gettags(item)[1].split("_") if e)
+                if r1 >= within_r1 or c1 >= within_c1 or r2 <= within_r2 or c2 <= within_c2:
                     if r1 > within_r1:
                         start_row = r1
                     else:
                         start_row = within_r1
                     if c1 > within_c1:
                         start_col = c1
                     else:
@@ -6641,52 +5837,37 @@
                         end_row = r2
                     else:
                         end_row = within_r2
                     if c2 < within_c2:
                         end_col = c2
                     else:
                         end_col = within_c2
-                    s.update(
-                        set(
-                            product(
-                                range(start_row, end_row), range(start_col, end_col)
-                            )
-                        )
-                    )
+                    s.update(set(product(range(start_row, end_row), range(start_col, end_col))))
         return s
 
     def get_all_selection_boxes(self):
         return tuple(
             tuple(int(e) for e in self.gettags(item)[1].split("_") if e)
             for item in chain(
                 self.find_withtag("cells"),
                 self.find_withtag("rows"),
                 self.find_withtag("columns"),
             )
         )
 
     def get_all_selection_boxes_with_types(self):
         boxes = []
-        for item in sorted(
-            self.find_withtag("cells")
-            + self.find_withtag("rows")
-            + self.find_withtag("columns")
-        ):
+        for item in sorted(self.find_withtag("cells") + self.find_withtag("rows") + self.find_withtag("columns")):
             tags = self.gettags(item)
             boxes.append((tuple(int(e) for e in tags[1].split("_") if e), tags[0]))
         return boxes
 
     def all_selected(self):
         for r1, c1, r2, c2 in self.get_all_selection_boxes():
-            if (
-                not r1
-                and not c1
-                and r2 == len(self.row_positions) - 1
-                and c2 == len(self.col_positions) - 1
-            ):
+            if not r1 and not c1 and r2 == len(self.row_positions) - 1 and c2 == len(self.col_positions) - 1:
                 return True
         return False
 
     # don't have to use "currently" because you can't have a current without a selection box
     def cell_selected(self, r, c, inc_cols=False, inc_rows=False):
         if not isinstance(r, int) or not isinstance(c, int):
             return False
@@ -6699,46 +5880,38 @@
         elif inc_cols and inc_rows:
             iterable = chain(
                 self.find_withtag("rows"),
                 self.find_withtag("columns"),
                 self.find_withtag("cells"),
             )
         for item in iterable:
-            r1, c1, r2, c2 = tuple(
-                int(e) for e in self.gettags(item)[1].split("_") if e
-            )
+            r1, c1, r2, c2 = tuple(int(e) for e in self.gettags(item)[1].split("_") if e)
             if r1 <= r and c1 <= c and r2 > r and c2 > c:
                 return True
         return False
 
     def col_selected(self, c):
         if not isinstance(c, int):
             return False
         for item in self.find_withtag("columns"):
-            r1, c1, r2, c2 = tuple(
-                int(e) for e in self.gettags(item)[1].split("_") if e
-            )
+            r1, c1, r2, c2 = tuple(int(e) for e in self.gettags(item)[1].split("_") if e)
             if c1 <= c and c2 > c:
                 return True
         return False
 
     def row_selected(self, r):
         if not isinstance(r, int):
             return False
         for item in self.find_withtag("rows"):
-            r1, c1, r2, c2 = tuple(
-                int(e) for e in self.gettags(item)[1].split("_") if e
-            )
+            r1, c1, r2, c2 = tuple(int(e) for e in self.gettags(item)[1].split("_") if e)
             if r1 <= r and r2 > r:
                 return True
         return False
 
-    def anything_selected(
-        self, exclude_columns=False, exclude_rows=False, exclude_cells=False
-    ):
+    def anything_selected(self, exclude_columns=False, exclude_rows=False, exclude_cells=False):
         if exclude_columns and exclude_rows and not exclude_cells:
             return self.find_withtag("cells")
         elif exclude_columns and exclude_cells and not exclude_rows:
             return self.find_withtag("rows")
         elif exclude_rows and exclude_cells and not exclude_columns:
             return self.find_withtag("columns")
 
@@ -6747,45 +5920,39 @@
         elif exclude_rows and not exclude_columns and not exclude_cells:
             return self.find_withtag("cells") + self.find_withtag("columns")
 
         elif exclude_cells and not exclude_columns and not exclude_rows:
             return self.find_withtag("rows") + self.find_withtag("columns")
 
         elif not exclude_columns and not exclude_rows and not exclude_cells:
-            return (
-                self.find_withtag("cells")
-                + self.find_withtag("rows")
-                + self.find_withtag("columns")
-            )
+            return self.find_withtag("cells") + self.find_withtag("rows") + self.find_withtag("columns")
         return tuple()
 
     def hide_current(self):
         for item in self.find_withtag("currently"):
             self.itemconfig(item, state="hidden")
 
     def show_current(self):
         for item in self.find_withtag("currently"):
             self.itemconfig(item, state="normal")
 
     def open_cell(self, event=None, ignore_existing_editor=False):
-        if not self.anything_selected() or (
-            not ignore_existing_editor and self.text_editor_id is not None
-        ):
+        if not self.anything_selected() or (not ignore_existing_editor and self.text_editor_id is not None):
             return
         currently_selected = self.currently_selected()
         if not currently_selected:
             return
         r, c = int(currently_selected[0]), int(currently_selected[1])
         datacn = c if self.all_columns_displayed else self.displayed_columns[c]
         datarn = r if self.all_rows_displayed else self.displayed_rows[r]
         if self.get_cell_kwargs(datarn, datacn, key="readonly"):
             return
-        elif self.get_cell_kwargs(
-            datarn, datacn, key="dropdown"
-        ) or self.get_cell_kwargs(datarn, datacn, key="checkbox"):
+        elif self.get_cell_kwargs(datarn, datacn, key="dropdown") or self.get_cell_kwargs(
+            datarn, datacn, key="checkbox"
+        ):
             if self.event_opens_dropdown_or_checkbox(event):
                 if self.get_cell_kwargs(datarn, datacn, key="dropdown"):
                     self.open_dropdown_window(r, c, event=event)
                 elif self.get_cell_kwargs(datarn, datacn, key="checkbox"):
                     self.click_checkbox(r=r, c=c, datarn=datarn, datacn=datacn)
         else:
             self.open_text_editor(event=event, r=r, c=c, dropdown=False)
@@ -6839,17 +6006,15 @@
             if event is not None:
                 if hasattr(event, "keysym") and event.keysym == "Return":
                     extra_func_key = "Return"
                 elif hasattr(event, "keysym") and event.keysym == "F2":
                     extra_func_key = "F2"
             datarn = r if self.all_rows_displayed else self.displayed_rows[r]
             datacn = c if self.all_columns_displayed else self.displayed_columns[c]
-            if event is not None and (
-                hasattr(event, "keysym") and event.keysym == "BackSpace"
-            ):
+            if event is not None and (hasattr(event, "keysym") and event.keysym == "BackSpace"):
                 extra_func_key = "BackSpace"
                 text = ""
             else:
                 text = f"{self.get_cell_data(datarn, datacn, none_to_empty_str = True)}"
         elif event is not None and (
             (hasattr(event, "char") and event.char.isalpha())
             or (hasattr(event, "char") and event.char.isdigit())
@@ -6858,33 +6023,27 @@
             extra_func_key = event.char
             text = event.char
         else:
             return False
         self.text_editor_loc = (r, c)
         if self.extra_begin_edit_cell_func is not None:
             try:
-                text = self.extra_begin_edit_cell_func(
-                    EditCellEvent(r, c, extra_func_key, text, "begin_edit_cell")
-                )
+                text = self.extra_begin_edit_cell_func(EditCellEvent(r, c, extra_func_key, text, "begin_edit_cell"))
             except Exception:
                 return False
             if text is None:
                 return False
             else:
                 text = text if isinstance(text, str) else f"{text}"
         text = "" if text is None else text
         if self.cell_auto_resize_enabled:
-            self.set_cell_size_to_text(
-                r, c, only_set_if_too_small=True, redraw=True, run_binding=True
-            )
+            self.set_cell_size_to_text(r, c, only_set_if_too_small=True, redraw=True, run_binding=True)
 
         if (r, c) == self.text_editor_loc and self.text_editor is not None:
-            self.text_editor.set_text(
-                self.text_editor.get() + "" if not isinstance(text, str) else text
-            )
+            self.text_editor.set_text(self.text_editor.get() + "" if not isinstance(text, str) else text)
             return
         if self.text_editor is not None:
             self.destroy_text_editor()
         if see:
             has_redrawn = self.see(r=r, c=c, check_cell_visibility=True)
             if not has_redrawn:
                 self.refresh()
@@ -6918,107 +6077,71 @@
             binding=binding,
             align=self.get_cell_align(r, c),
             r=r,
             c=c,
             newline_binding=self.text_editor_newline_binding,
         )
         self.text_editor.update_idletasks()
-        self.text_editor_id = self.create_window(
-            (x, y), window=self.text_editor, anchor="nw"
-        )
+        self.text_editor_id = self.create_window((x, y), window=self.text_editor, anchor="nw")
         if not dropdown:
             self.text_editor.textedit.focus_set()
             self.text_editor.scroll_to_bottom()
-        self.text_editor.textedit.bind(
-            "<Alt-Return>", lambda x: self.text_editor_newline_binding(r, c)
-        )
+        self.text_editor.textedit.bind("<Alt-Return>", lambda x: self.text_editor_newline_binding(r, c))
         if USER_OS == "darwin":
-            self.text_editor.textedit.bind(
-                "<Option-Return>", lambda x: self.text_editor_newline_binding(r, c)
-            )
+            self.text_editor.textedit.bind("<Option-Return>", lambda x: self.text_editor_newline_binding(r, c))
         for key, func in self.text_editor_user_bound_keys.items():
             self.text_editor.textedit.bind(key, func)
         if binding is not None:
             self.text_editor.textedit.bind("<Tab>", lambda x: binding((r, c, "Tab")))
-            self.text_editor.textedit.bind(
-                "<Return>", lambda x: binding((r, c, "Return"))
-            )
-            self.text_editor.textedit.bind(
-                "<FocusOut>", lambda x: binding((r, c, "FocusOut"))
-            )
-            self.text_editor.textedit.bind(
-                "<Escape>", lambda x: binding((r, c, "Escape"))
-            )
+            self.text_editor.textedit.bind("<Return>", lambda x: binding((r, c, "Return")))
+            self.text_editor.textedit.bind("<FocusOut>", lambda x: binding((r, c, "FocusOut")))
+            self.text_editor.textedit.bind("<Escape>", lambda x: binding((r, c, "Escape")))
         elif binding is None and set_data_on_close:
-            self.text_editor.textedit.bind(
-                "<Tab>", lambda x: self.close_text_editor((r, c, "Tab"))
-            )
-            self.text_editor.textedit.bind(
-                "<Return>", lambda x: self.close_text_editor((r, c, "Return"))
-            )
+            self.text_editor.textedit.bind("<Tab>", lambda x: self.close_text_editor((r, c, "Tab")))
+            self.text_editor.textedit.bind("<Return>", lambda x: self.close_text_editor((r, c, "Return")))
             if not dropdown:
-                self.text_editor.textedit.bind(
-                    "<FocusOut>", lambda x: self.close_text_editor((r, c, "FocusOut"))
-                )
-            self.text_editor.textedit.bind(
-                "<Escape>", lambda x: self.close_text_editor((r, c, "Escape"))
-            )
+                self.text_editor.textedit.bind("<FocusOut>", lambda x: self.close_text_editor((r, c, "FocusOut")))
+            self.text_editor.textedit.bind("<Escape>", lambda x: self.close_text_editor((r, c, "Escape")))
         else:
-            self.text_editor.textedit.bind(
-                "<Escape>", lambda x: self.destroy_text_editor("Escape")
-            )
+            self.text_editor.textedit.bind("<Escape>", lambda x: self.destroy_text_editor("Escape"))
         return True
 
     # displayed indexes
     def text_editor_newline_binding(self, r=0, c=0, event=None, check_lines=True):
         datarn = r if self.all_rows_displayed else self.displayed_rows[r]
         datacn = c if self.all_columns_displayed else self.displayed_columns[c]
         curr_height = self.text_editor.winfo_height()
-        if (
-            not check_lines
-            or self.get_lines_cell_height(self.text_editor.get_num_lines() + 1)
-            > curr_height
-        ):
+        if not check_lines or self.get_lines_cell_height(self.text_editor.get_num_lines() + 1) > curr_height:
             new_height = curr_height + self.xtra_lines_increment
             space_bot = self.get_space_bot(r)
             if new_height > space_bot:
                 new_height = space_bot
             if new_height != curr_height:
                 self.text_editor.config(height=new_height)
                 kwargs = self.get_cell_kwargs(datarn, datacn, key="dropdown")
                 if kwargs:
                     text_editor_h = self.text_editor.winfo_height()
-                    win_h, anchor = self.get_dropdown_height_anchor(
-                        datarn, datacn, text_editor_h
-                    )
+                    win_h, anchor = self.get_dropdown_height_anchor(datarn, datacn, text_editor_h)
                     if anchor == "nw":
                         self.coords(
                             kwargs["canvas_id"],
                             self.col_positions[c],
                             self.row_positions[r] + text_editor_h - 1,
                         )
-                        self.itemconfig(
-                            kwargs["canvas_id"], anchor=anchor, height=win_h
-                        )
+                        self.itemconfig(kwargs["canvas_id"], anchor=anchor, height=win_h)
                     elif anchor == "sw":
                         self.coords(
                             kwargs["canvas_id"],
                             self.col_positions[c],
                             self.row_positions[r],
                         )
-                        self.itemconfig(
-                            kwargs["canvas_id"], anchor=anchor, height=win_h
-                        )
+                        self.itemconfig(kwargs["canvas_id"], anchor=anchor, height=win_h)
 
     def destroy_text_editor(self, event=None):
-        if (
-            event is not None
-            and self.extra_end_edit_cell_func is not None
-            and self.text_editor_loc is not None
-        ):
+        if event is not None and self.extra_end_edit_cell_func is not None and self.text_editor_loc is not None:
             self.extra_end_edit_cell_func(
                 EditCellEvent(
                     int(self.text_editor_loc[0]),
                     int(self.text_editor_loc[1]),
                     "Escape",
                     None,
                     "escape_edit_cell",
@@ -7050,19 +6173,15 @@
         destroy=True,
         move_down=True,
         redraw=True,
         recreate=True,
     ):
         if self.focus_get() is None and editor_info:
             return "break"
-        if (
-            editor_info is not None
-            and len(editor_info) >= 3
-            and editor_info[2] == "Escape"
-        ):
+        if editor_info is not None and len(editor_info) >= 3 and editor_info[2] == "Escape":
             self.destroy_text_editor("Escape")
             self.close_dropdown_window(r, c)
             return "break"
         if self.text_editor is not None:
             self.text_editor_value = self.text_editor.get()
         if destroy:
             self.destroy_text_editor()
@@ -7102,30 +6221,26 @@
                         r,
                         c,
                         editor_info[2] if len(editor_info) >= 3 else "FocusOut",
                         f"{self.text_editor_value}",
                         "end_edit_cell",
                     )
                 )
-            elif (
-                self.extra_end_edit_cell_func is not None and self.edit_cell_validation
-            ):
+            elif self.extra_end_edit_cell_func is not None and self.edit_cell_validation:
                 validation = self.extra_end_edit_cell_func(
                     EditCellEvent(
                         r,
                         c,
                         editor_info[2] if len(editor_info) >= 3 else "FocusOut",
                         f"{self.text_editor_value}",
                         "end_edit_cell",
                     )
                 )
                 self.text_editor_value = validation
-                if validation is not None and self.input_valid_for_cell(
-                    datarn, datacn, self.text_editor_value
-                ):
+                if validation is not None and self.input_valid_for_cell(datarn, datacn, self.text_editor_value):
                     self.set_cell_data_undo(
                         r,
                         c,
                         datarn=datarn,
                         datacn=datacn,
                         value=self.text_editor_value,
                         redraw=False,
@@ -7139,104 +6254,76 @@
                 r is not None
                 and c is not None
                 and currently_selected
                 and r == currently_selected[0]
                 and c == currently_selected[1]
                 and (self.single_selection_enabled or self.toggle_selection_enabled)
             ):
-                r1, c1, r2, c2 = self.find_last_selected_box_with_current(
-                    currently_selected
-                )
+                r1, c1, r2, c2 = self.find_last_selected_box_with_current(currently_selected)
                 numcols = c2 - c1
                 numrows = r2 - r1
                 if numcols == 1 and numrows == 1:
-                    if (
-                        editor_info is not None
-                        and len(editor_info) >= 3
-                        and editor_info[2] == "Return"
-                    ):
-                        self.select_cell(
-                            r + 1 if r < len(self.row_positions) - 2 else r, c
-                        )
+                    if editor_info is not None and len(editor_info) >= 3 and editor_info[2] == "Return":
+                        self.select_cell(r + 1 if r < len(self.row_positions) - 2 else r, c)
                         self.see(
                             r + 1 if r < len(self.row_positions) - 2 else r,
                             c,
                             keep_xscroll=True,
                             bottom_right_corner=True,
                             check_cell_visibility=True,
                         )
-                    elif (
-                        editor_info is not None
-                        and len(editor_info) >= 3
-                        and editor_info[2] == "Tab"
-                    ):
-                        self.select_cell(
-                            r, c + 1 if c < len(self.col_positions) - 2 else c
-                        )
+                    elif editor_info is not None and len(editor_info) >= 3 and editor_info[2] == "Tab":
+                        self.select_cell(r, c + 1 if c < len(self.col_positions) - 2 else c)
                         self.see(
                             r,
                             c + 1 if c < len(self.col_positions) - 2 else c,
                             keep_xscroll=True,
                             bottom_right_corner=True,
                             check_cell_visibility=True,
                         )
                 else:
                     moved = False
                     new_r = r
                     new_c = c
-                    if (
-                        editor_info is not None
-                        and len(editor_info) >= 3
-                        and editor_info[2] == "Return"
-                    ):
+                    if editor_info is not None and len(editor_info) >= 3 and editor_info[2] == "Return":
                         if r + 1 == r2:
                             new_r = r1
                         elif numrows > 1:
                             new_r = r + 1
                             moved = True
                         if not moved:
                             if c + 1 == c2:
                                 new_c = c1
                             elif numcols > 1:
                                 new_c = c + 1
-                    elif (
-                        editor_info is not None
-                        and len(editor_info) >= 3
-                        and editor_info[2] == "Tab"
-                    ):
+                    elif editor_info is not None and len(editor_info) >= 3 and editor_info[2] == "Tab":
                         if c + 1 == c2:
                             new_c = c1
                         elif numcols > 1:
                             new_c = c + 1
                             moved = True
                         if not moved:
                             if r + 1 == r2:
                                 new_r = r1
                             elif numrows > 1:
                                 new_r = r + 1
-                    self.set_currently_selected(
-                        new_r, new_c, type_=currently_selected.type_
-                    )
+                    self.set_currently_selected(new_r, new_c, type_=currently_selected.type_)
                     self.see(
                         new_r,
                         new_c,
                         keep_xscroll=False,
                         bottom_right_corner=True,
                         check_cell_visibility=True,
                     )
         self.close_dropdown_window(r, c)
         if recreate:
             self.recreate_all_selection_boxes()
         if redraw:
             self.refresh()
-        if (
-            editor_info is not None
-            and len(editor_info) >= 3
-            and editor_info[2] != "FocusOut"
-        ):
+        if editor_info is not None and len(editor_info) >= 3 and editor_info[2] != "FocusOut":
             self.focus_set()
         return "break"
 
     def tab_key(self, event=None):
         currently_selected = self.currently_selected()
         if not currently_selected:
             return
@@ -7301,35 +6388,29 @@
                                 self.currently_selected(),
                             )
                         )
                     )
                 )
             self.set_cell_data(datarn, datacn, value)
         if cell_resize and self.cell_auto_resize_enabled:
-            self.set_cell_size_to_text(
-                r, c, only_set_if_too_small=True, redraw=redraw, run_binding=True
-            )
+            self.set_cell_size_to_text(r, c, only_set_if_too_small=True, redraw=redraw, run_binding=True)
         self.parentframe.emit_event("<<SheetModified>>")
         return True
 
     def set_cell_data(self, datarn, datacn, value, kwargs={}, expand_sheet=True):
         if expand_sheet:
             if datarn >= len(self.data):
                 self.fix_data_len(datarn, datacn)
             elif datacn >= len(self.data[datarn]):
                 self.fix_row_len(datarn, datacn)
-        if expand_sheet or (
-            len(self.data) > datarn and len(self.data[datarn]) > datacn
-        ):
+        if expand_sheet or (len(self.data) > datarn and len(self.data[datarn]) > datacn):
             if (
                 datarn,
                 datacn,
-            ) in self.cell_options and "checkbox" in self.cell_options[
-                (datarn, datacn)
-            ]:
+            ) in self.cell_options and "checkbox" in self.cell_options[(datarn, datacn)]:
                 self.data[datarn][datacn] = try_to_bool(value)
             else:
                 if not kwargs:
                     kwargs = self.get_cell_kwargs(datarn, datacn, key="format")
                 if kwargs:
                     if kwargs["formatter"] is None:
                         self.data[datarn][datacn] = format_data(value=value, **kwargs)
@@ -7357,102 +6438,79 @@
             column=c_ops,
         )
         if kwargs and kwargs["validate_input"] and kwargs["values"]:
             return kwargs["values"][0]
         return ""
 
     def get_empty_row_seq(self, datarn, end, start=0, r_ops=True, c_ops=True):
-        return [
-            self.get_value_for_empty_cell(datarn, datacn, r_ops=r_ops, c_ops=c_ops)
-            for datacn in range(start, end)
-        ]
+        return [self.get_value_for_empty_cell(datarn, datacn, r_ops=r_ops, c_ops=c_ops) for datacn in range(start, end)]
 
     def fix_row_len(self, datarn, datacn):
-        self.data[datarn].extend(
-            self.get_empty_row_seq(datarn, end=datacn + 1, start=len(self.data[datarn]))
-        )
+        self.data[datarn].extend(self.get_empty_row_seq(datarn, end=datacn + 1, start=len(self.data[datarn])))
 
     def fix_row_values(self, datarn, start=None, end=None):
         if datarn < len(self.data):
             for datacn, v in enumerate(islice(self.data[datarn], start, end)):
                 if not self.input_valid_for_cell(datarn, datacn, v):
-                    self.data[datarn][datacn] = self.get_value_for_empty_cell(
-                        datarn, datacn
-                    )
+                    self.data[datarn][datacn] = self.get_value_for_empty_cell(datarn, datacn)
 
     def fix_data_len(self, datarn, datacn):
         ncols = self.total_data_cols() if datacn is None else datacn + 1
-        self.data.extend(
-            [
-                self.get_empty_row_seq(rn, end=ncols, start=0)
-                for rn in range(len(self.data), datarn + 1)
-            ]
-        )
+        self.data.extend([self.get_empty_row_seq(rn, end=ncols, start=0) for rn in range(len(self.data), datarn + 1)])
 
     # internal event use
     def click_checkbox(self, r, c, datarn=None, datacn=None, undo=True, redraw=True):
         if datarn is None:
             datarn = r if self.all_rows_displayed else self.displayed_rows[r]
         if datacn is None:
             datacn = c if self.all_columns_displayed else self.displayed_columns[c]
         kwargs = self.get_cell_kwargs(datarn, datacn, key="checkbox")
         if kwargs["state"] == "normal":
             self.set_cell_data_undo(
                 r,
                 c,
-                value=not self.data[datarn][datacn]
-                if type(self.data[datarn][datacn]) == bool
-                else False,
+                value=not self.data[datarn][datacn] if type(self.data[datarn][datacn]) == bool else False,
                 undo=undo,
                 cell_resize=False,
                 check_input_valid=False,
             )
             if kwargs["check_function"] is not None:
-                kwargs["check_function"](
-                    (r, c, "CheckboxClicked", self.data[datarn][datacn])
-                )
+                kwargs["check_function"]((r, c, "CheckboxClicked", self.data[datarn][datacn]))
             if self.extra_end_edit_cell_func is not None:
-                self.extra_end_edit_cell_func(
-                    EditCellEvent(
-                        r, c, "Return", self.data[datarn][datacn], "end_edit_cell"
-                    )
-                )
+                self.extra_end_edit_cell_func(EditCellEvent(r, c, "Return", self.data[datarn][datacn], "end_edit_cell"))
         if redraw:
             self.refresh()
 
     def create_checkbox(self, datarn=0, datacn=0, **kwargs):
         self.delete_cell_format(datarn, datacn, clear_values=False)
         if (datarn, datacn) in self.cell_options and (
-            "dropdown" in self.cell_options[(datarn, datacn)]
-            or "checkbox" in self.cell_options[(datarn, datacn)]
+            "dropdown" in self.cell_options[(datarn, datacn)] or "checkbox" in self.cell_options[(datarn, datacn)]
         ):
             self.delete_cell_options_dropdown_and_checkbox(datarn, datacn)
         if (datarn, datacn) not in self.cell_options:
             self.cell_options[(datarn, datacn)] = {}
         self.cell_options[(datarn, datacn)]["checkbox"] = get_checkbox_dict(**kwargs)
         self.set_cell_data(datarn, datacn, kwargs["checked"])
 
     def checkbox_row(self, datarn=0, **kwargs):
         self.delete_row_format(datarn, clear_values=False)
         if datarn in self.row_options and (
-            "dropdown" in self.row_options[datarn]
-            or "checkbox" in self.row_options[datarn]
+            "dropdown" in self.row_options[datarn] or "checkbox" in self.row_options[datarn]
         ):
             self.delete_row_options_dropdown_and_checkbox(datarn)
         if datarn not in self.row_options:
             self.row_options[datarn] = {}
         self.row_options[datarn]["checkbox"] = get_checkbox_dict(**kwargs)
         for datacn in range(self.total_data_cols()):
             self.set_cell_data(datarn, datacn, kwargs["checked"])
 
     def checkbox_column(self, datacn=0, **kwargs):
         self.delete_column_format(datacn, clear_values=False)
         if datacn in self.col_options and (
-            "dropdown" in self.col_options[datacn]
-            or "checkbox" in self.col_options[datacn]
+            "dropdown" in self.col_options[datacn] or "checkbox" in self.col_options[datacn]
         ):
             self.delete_column_options_dropdown_and_checkbox(datacn)
         if datacn not in self.col_options:
             self.col_options[datacn] = {}
         self.col_options[datacn]["checkbox"] = get_checkbox_dict(**kwargs)
         for datarn in range(self.total_data_rows()):
             self.set_cell_data(datarn, datacn, kwargs["checked"])
@@ -7465,165 +6523,133 @@
         total_cols = self.total_data_cols()
         for datarn in range(self.total_data_rows()):
             for datacn in range(total_cols):
                 self.set_cell_data(datarn, datacn, kwargs["checked"])
 
     def create_dropdown(self, datarn=0, datacn=0, **kwargs):
         if (datarn, datacn) in self.cell_options and (
-            "dropdown" in self.cell_options[(datarn, datacn)]
-            or "checkbox" in self.cell_options[(datarn, datacn)]
+            "dropdown" in self.cell_options[(datarn, datacn)] or "checkbox" in self.cell_options[(datarn, datacn)]
         ):
             self.delete_cell_options_dropdown_and_checkbox(datarn, datacn)
         if (datarn, datacn) not in self.cell_options:
             self.cell_options[(datarn, datacn)] = {}
         self.cell_options[(datarn, datacn)]["dropdown"] = get_dropdown_dict(**kwargs)
         self.set_cell_data(
             datarn,
             datacn,
-            kwargs["set_value"]
-            if kwargs["set_value"] is not None
-            else kwargs["values"][0]
-            if kwargs["values"]
-            else "",
+            kwargs["set_value"] if kwargs["set_value"] is not None else kwargs["values"][0] if kwargs["values"] else "",
         )
 
     def dropdown_row(self, datarn=0, **kwargs):
         if datarn in self.row_options and (
-            "dropdown" in self.row_options[datarn]
-            or "checkbox" in self.row_options[datarn]
+            "dropdown" in self.row_options[datarn] or "checkbox" in self.row_options[datarn]
         ):
             self.delete_row_options_dropdown_and_checkbox(datarn)
         if datarn not in self.row_options:
             self.row_options[datarn] = {}
         self.row_options[datarn]["dropdown"] = get_dropdown_dict(**kwargs)
         value = (
-            kwargs["set_value"]
-            if kwargs["set_value"] is not None
-            else kwargs["values"][0]
-            if kwargs["values"]
-            else ""
+            kwargs["set_value"] if kwargs["set_value"] is not None else kwargs["values"][0] if kwargs["values"] else ""
         )
         for datacn in range(self.total_data_cols()):
             self.set_cell_data(datarn, datacn, value)
 
     def dropdown_column(self, datacn=0, **kwargs):
         if datacn in self.col_options and (
-            "dropdown" in self.col_options[datacn]
-            or "checkbox" in self.col_options[datacn]
+            "dropdown" in self.col_options[datacn] or "checkbox" in self.col_options[datacn]
         ):
             self.delete_column_options_dropdown_and_checkbox(datacn)
         if datacn not in self.col_options:
             self.col_options[datacn] = {}
         self.col_options[datacn]["dropdown"] = get_dropdown_dict(**kwargs)
         value = (
-            kwargs["set_value"]
-            if kwargs["set_value"] is not None
-            else kwargs["values"][0]
-            if kwargs["values"]
-            else ""
+            kwargs["set_value"] if kwargs["set_value"] is not None else kwargs["values"][0] if kwargs["values"] else ""
         )
         for datarn in range(self.total_data_rows()):
             self.set_cell_data(datarn, datacn, value)
 
     def dropdown_sheet(self, **kwargs):
         if "dropdown" in self.options or "checkbox" in self.options:
             self.delete_options_dropdown_and_checkbox()
         self.options["dropdown"] = get_dropdown_dict(**kwargs)
         value = (
-            kwargs["set_value"]
-            if kwargs["set_value"] is not None
-            else kwargs["values"][0]
-            if kwargs["values"]
-            else ""
+            kwargs["set_value"] if kwargs["set_value"] is not None else kwargs["values"][0] if kwargs["values"] else ""
         )
         total_cols = self.total_data_cols()
         for datarn in range(self.total_data_rows()):
             for datacn in range(total_cols):
                 self.set_cell_data(datarn, datacn, value)
 
     def format_cell(self, datarn, datacn, **kwargs):
-        if (datarn, datacn) in self.cell_options and "checkbox" in self.cell_options[
-            (datarn, datacn)
-        ]:
+        if (datarn, datacn) in self.cell_options and "checkbox" in self.cell_options[(datarn, datacn)]:
             return
         kwargs = self.format_fix_kwargs(kwargs)
         if (datarn, datacn) not in self.cell_options:
             self.cell_options[(datarn, datacn)] = {}
         self.cell_options[(datarn, datacn)]["format"] = kwargs
         self.set_cell_data(
             datarn,
             datacn,
-            value=kwargs["value"]
-            if "value" in kwargs
-            else self.get_cell_data(datarn, datacn),
+            value=kwargs["value"] if "value" in kwargs else self.get_cell_data(datarn, datacn),
             kwargs=kwargs,
         )
 
     def format_row(self, datarn, **kwargs):
         if datarn in self.row_options and "checkbox" in self.row_options[datarn]:
             return
         kwargs = self.format_fix_kwargs(kwargs)
         if datarn not in self.row_options:
             self.row_options[datarn] = {}
         self.row_options[datarn]["format"] = kwargs
         for datacn in range(self.total_data_cols()):
             self.set_cell_data(
                 datarn,
                 datacn,
-                value=kwargs["value"]
-                if "value" in kwargs
-                else self.get_cell_data(datarn, datacn),
+                value=kwargs["value"] if "value" in kwargs else self.get_cell_data(datarn, datacn),
                 kwargs=kwargs,
             )
 
     def format_column(self, datacn, **kwargs):
         if datacn in self.col_options and "checkbox" in self.col_options[datacn]:
             return
         kwargs = self.format_fix_kwargs(kwargs)
         if datacn not in self.col_options:
             self.col_options[datacn] = {}
         self.col_options[datacn]["format"] = kwargs
         for datarn in range(self.total_data_rows()):
             self.set_cell_data(
                 datarn,
                 datacn,
-                value=kwargs["value"]
-                if "value" in kwargs
-                else self.get_cell_data(datarn, datacn),
+                value=kwargs["value"] if "value" in kwargs else self.get_cell_data(datarn, datacn),
                 kwargs=kwargs,
             )
 
     def format_sheet(self, **kwargs):
         kwargs = self.format_fix_kwargs(kwargs)
         self.options["format"] = kwargs
         for datarn in range(self.total_data_rows()):
             for datacn in range(self.total_data_cols()):
                 self.set_cell_data(
                     datarn,
                     datacn,
-                    value=kwargs["value"]
-                    if "value" in kwargs
-                    else self.get_cell_data(datarn, datacn),
+                    value=kwargs["value"] if "value" in kwargs else self.get_cell_data(datarn, datacn),
                     kwargs=kwargs,
                 )
 
     def format_fix_kwargs(self, kwargs):
         if kwargs["formatter"] is None:
             if kwargs["nullable"]:
                 if isinstance(kwargs["datatypes"], (list, tuple)):
                     kwargs["datatypes"] = tuple(kwargs["datatypes"]) + (type(None),)
                 else:
                     kwargs["datatypes"] = (kwargs["datatypes"], type(None))
-            elif (
-                isinstance(kwargs["datatypes"], (list, tuple))
-                and type(None) in kwargs["datatypes"]
-            ) or kwargs["datatypes"] is type(None):
-                raise TypeError(
-                    "Non-nullable cells cannot have NoneType as a datatype."
-                )
+            elif (isinstance(kwargs["datatypes"], (list, tuple)) and type(None) in kwargs["datatypes"]) or kwargs[
+                "datatypes"
+            ] is type(None):
+                raise TypeError("Non-nullable cells cannot have NoneType as a datatype.")
         if not isinstance(kwargs["invalid_value"], str):
             kwargs["invalid_value"] = f"{kwargs['invalid_value']}"
         return kwargs
 
     def reapply_formatting(self):
         if "format" in self.options:
             for r in range(len(self.data)):
@@ -7643,18 +6669,15 @@
                     and "format" in self.cell_options[(r, c)]
                     or r in self.row_options
                     and "format" in self.row_options[r]
                 ):
                     self.set_cell_data(r, c, value=self.data[r][c])
         for r in self.yield_formatted_rows():
             for c in range(len(self.data[r])):
-                if not (
-                    (r, c) in self.cell_options
-                    and "format" in self.cell_options[(r, c)]
-                ):
+                if not ((r, c) in self.cell_options and "format" in self.cell_options[(r, c)]):
                     self.set_cell_data(r, c, value=self.data[r][c])
         for r, c in self.yield_formatted_cells():
             if len(self.data) > r and len(self.data[r]) > c:
                 self.set_cell_data(r, c, value=self.data[r][c])
 
     def delete_all_formatting(self, clear_values=False):
         self.delete_cell_format("all", clear_values=clear_values)
@@ -7665,17 +6688,15 @@
     def delete_cell_format(self, datarn="all", datacn=0, clear_values=False):
         if isinstance(datarn, str) and datarn.lower() == "all":
             for datarn, datacn in self.yield_formatted_cells():
                 del self.cell_options[(datarn, datacn)]["format"]
                 if clear_values:
                     self.set_cell_data(datarn, datacn, "", expand_sheet=False)
         else:
-            if (datarn, datacn) in self.cell_options and "format" in self.cell_options[
-                (datarn, datacn)
-            ]:
+            if (datarn, datacn) in self.cell_options and "format" in self.cell_options[(datarn, datacn)]:
                 del self.cell_options[(datarn, datacn)]["format"]
                 if clear_values:
                     self.set_cell_data(datarn, datacn, "", expand_sheet=False)
 
     def delete_row_format(self, datarn="all", clear_values=False):
         if isinstance(datarn, str) and datarn.lower() == "all":
             for datarn in self.yield_formatted_rows():
@@ -7713,53 +6734,43 @@
                     [self.get_value_for_empty_cell(r, c) for c in range(total_cols)]
                     for r in range(self.total_data_rows())
                 ]
 
     # deals with possibility of formatter class being in self.data cell
     # if cell is formatted - possibly returns invalid_value kwarg if cell value is not in datatypes kwarg
     # if get displayed is true then Nones are replaced by ""
-    def get_valid_cell_data_as_str(
-        self, datarn, datacn, get_displayed=False, **kwargs
-    ) -> str:
+    def get_valid_cell_data_as_str(self, datarn, datacn, get_displayed=False, **kwargs) -> str:
         if get_displayed:
             kwargs = self.get_cell_kwargs(datarn, datacn, key="dropdown")
             if kwargs and kwargs["text"] is not None:
                 return f"{kwargs['text']}"
             kwargs = self.get_cell_kwargs(datarn, datacn, key="checkbox")
             if kwargs:
                 return f"{kwargs['text']}"
-        value = (
-            self.data[datarn][datacn]
-            if len(self.data) > datarn and len(self.data[datarn]) > datacn
-            else ""
-        )
+        value = self.data[datarn][datacn] if len(self.data) > datarn and len(self.data[datarn]) > datacn else ""
         kwargs = self.get_cell_kwargs(datarn, datacn, key="format")
         if kwargs:
             if kwargs["formatter"] is None:
                 if get_displayed:
                     return data_to_str(value, **kwargs)
                 else:
                     return f"{get_data_with_valid_check(value, **kwargs)}"
             else:
                 if get_displayed:
-                    return f"{value}"  # assumed given formatter class has __str__() function
+                    # assumed given formatter class has __str__() function
+                    return f"{value}"
                 else:
-                    return f"{value.get_data_with_valid_check()}"  # assumed given formatter class has get_data_with_valid_check() function
+                    # assumed given formatter class has get_data_with_valid_check() function
+                    return f"{value.get_data_with_valid_check()}"
         return "" if value is None else f"{value}"
 
-    def get_cell_data(
-        self, datarn, datacn, get_displayed=False, none_to_empty_str=False, **kwargs
-    ) -> Any:
+    def get_cell_data(self, datarn, datacn, get_displayed=False, none_to_empty_str=False, **kwargs) -> Any:
         if get_displayed:
             return self.get_valid_cell_data_as_str(datarn, datacn, get_displayed=True)
-        value = (
-            self.data[datarn][datacn]
-            if len(self.data) > datarn and len(self.data[datarn]) > datacn
-            else ""
-        )
+        value = self.data[datarn][datacn] if len(self.data) > datarn and len(self.data[datarn]) > datacn else ""
         kwargs = self.get_cell_kwargs(datarn, datacn, key="format")
         if kwargs and kwargs["formatter"] is not None:
             value = value.value  # assumed given formatter class has value attribute
         return "" if (value is None and none_to_empty_str) else value
 
     def input_valid_for_cell(self, datarn, datacn, value):
         if self.get_cell_kwargs(datarn, datacn, key="readonly"):
@@ -7782,60 +6793,48 @@
             return v == format_data(value=value, **kwargs)
         # assumed if there is a formatter class in cell then it has a __eq__() function anyway
         # else if there is not a formatter class in cell and cell is not formatted
         # then compare value as is
         return v == value
 
     def get_cell_clipboard(self, datarn, datacn) -> Union[str, int, float, bool]:
-        value = (
-            self.data[datarn][datacn]
-            if len(self.data) > datarn and len(self.data[datarn]) > datacn
-            else ""
-        )
+        value = self.data[datarn][datacn] if len(self.data) > datarn and len(self.data[datarn]) > datacn else ""
         kwargs = self.get_cell_kwargs(datarn, datacn, key="format")
         if kwargs:
             if kwargs["formatter"] is None:
                 return get_clipboard_data(value, **kwargs)
             else:
-                return (
-                    value.get_clipboard_data()
-                )  # assumed given formatter class has get_clipboard_data() function and it returns one of above type hints
+                # assumed given formatter class has get_clipboard_data()
+                # function and it returns one of above type hints
+                return value.get_clipboard_data()
         return f"{value}"
 
     def yield_formatted_cells(self, formatter=None):
         if formatter is None:
             yield from (
                 cell
                 for cell, options in self.cell_options.items()
                 if "format" in options and options["format"]["formatter"] == formatter
             )
         else:
-            yield from (
-                cell
-                for cell, options in self.cell_options.items()
-                if "format" in options
-            )
+            yield from (cell for cell, options in self.cell_options.items() if "format" in options)
 
     def yield_formatted_rows(self, formatter=None):
         if formatter is None:
-            yield from (
-                r for r, options in self.row_options.items() if "format" in options
-            )
+            yield from (r for r, options in self.row_options.items() if "format" in options)
         else:
             yield from (
                 r
                 for r, options in self.row_options.items()
                 if "format" in options and options["format"]["formatter"] == formatter
             )
 
     def yield_formatted_columns(self, formatter=None):
         if formatter is None:
-            yield from (
-                c for c, options in self.col_options.items() if "format" in options
-            )
+            yield from (c for c, options in self.col_options.items() if "format" in options)
         else:
             yield from (
                 c
                 for c, options in self.col_options.items()
                 if "format" in options and options["format"]["formatter"] == formatter
             )
 
@@ -7845,19 +6844,15 @@
         datacn,
         key="format",
         cell=True,
         row=True,
         column=True,
         entire=True,
     ):
-        if (
-            cell
-            and (datarn, datacn) in self.cell_options
-            and key in self.cell_options[(datarn, datacn)]
-        ):
+        if cell and (datarn, datacn) in self.cell_options and key in self.cell_options[(datarn, datacn)]:
             return self.cell_options[(datarn, datacn)][key]
         if row and datarn in self.row_options and key in self.row_options[datarn]:
             return self.row_options[datarn][key]
         if column and datacn in self.col_options and key in self.col_options[datacn]:
             return self.col_options[datacn][key]
         if entire and key in self.options:
             return self.options[key]
@@ -7869,53 +6864,33 @@
                 win_h = int(self.winfo_height())
                 sheet_h = int(1 + self.empty_vertical)
             else:
                 win_h = int(self.winfo_height() - text_editor_h)
                 sheet_h = int(1 + self.empty_vertical - text_editor_h)
         else:
             if text_editor_h is None:
-                win_h = int(
-                    self.canvasy(0) + self.winfo_height() - self.row_positions[r + 1]
-                )
-                sheet_h = int(
-                    self.row_positions[-1]
-                    + 1
-                    + self.empty_vertical
-                    - self.row_positions[r + 1]
-                )
+                win_h = int(self.canvasy(0) + self.winfo_height() - self.row_positions[r + 1])
+                sheet_h = int(self.row_positions[-1] + 1 + self.empty_vertical - self.row_positions[r + 1])
             else:
-                win_h = int(
-                    self.canvasy(0)
-                    + self.winfo_height()
-                    - (self.row_positions[r] + text_editor_h)
-                )
+                win_h = int(self.canvasy(0) + self.winfo_height() - (self.row_positions[r] + text_editor_h))
                 sheet_h = int(
-                    self.row_positions[-1]
-                    + 1
-                    + self.empty_vertical
-                    - (self.row_positions[r] + text_editor_h)
+                    self.row_positions[-1] + 1 + self.empty_vertical - (self.row_positions[r] + text_editor_h)
                 )
         if win_h > 0:
             win_h -= 1
         if sheet_h > 0:
             sheet_h -= 1
         return win_h if win_h >= sheet_h else sheet_h
 
     def get_dropdown_height_anchor(self, datarn, datacn, text_editor_h=None):
         win_h = 5
-        for i, v in enumerate(
-            self.get_cell_kwargs(datarn, datacn, key="dropdown")["values"]
-        ):
-            v_numlines = len(
-                v.split("\n") if isinstance(v, str) else f"{v}".split("\n")
-            )
+        for i, v in enumerate(self.get_cell_kwargs(datarn, datacn, key="dropdown")["values"]):
+            v_numlines = len(v.split("\n") if isinstance(v, str) else f"{v}".split("\n"))
             if v_numlines > 1:
-                win_h += (
-                    self.fl_ins + (v_numlines * self.xtra_lines_increment) + 5
-                )  # end of cell
+                win_h += self.fl_ins + (v_numlines * self.xtra_lines_increment) + 5  # end of cell
             else:
                 win_h += self.min_row_height
             if i == 5:
                 break
         if win_h > 500:
             win_h = 500
         space_bot = self.get_space_bot(datarn, text_editor_h)
@@ -7969,23 +6944,19 @@
             align="w",
         )  # self.get_cell_align(r, c)
         if kwargs["state"] == "normal":
             if anchor == "nw":
                 ypos = self.row_positions[r] + self.text_editor.h_ - 1
             else:
                 ypos = self.row_positions[r]
-            kwargs["canvas_id"] = self.create_window(
-                (self.col_positions[c], ypos), window=window, anchor=anchor
-            )
+            kwargs["canvas_id"] = self.create_window((self.col_positions[c], ypos), window=window, anchor=anchor)
             self.text_editor.textedit.bind(
                 "<<TextModified>>",
                 lambda x: window.search_and_see(
-                    DropDownModifiedEvent(
-                        "ComboboxModified", r, c, self.text_editor.get()
-                    )
+                    DropDownModifiedEvent("ComboboxModified", r, c, self.text_editor.get())
                 ),
             )
             if kwargs["modified_function"] is not None:
                 window.modified_function = kwargs["modified_function"]
             self.update_idletasks()
             try:
                 self.after(1, lambda: self.text_editor.textedit.focus())
@@ -7994,86 +6965,61 @@
                 return
             redraw = False
         else:
             if anchor == "nw":
                 ypos = self.row_positions[r + 1]
             else:
                 ypos = self.row_positions[r]
-            kwargs["canvas_id"] = self.create_window(
-                (self.col_positions[c], ypos), window=window, anchor=anchor
-            )
+            kwargs["canvas_id"] = self.create_window((self.col_positions[c], ypos), window=window, anchor=anchor)
             self.update_idletasks()
             window.bind("<FocusOut>", lambda x: self.close_dropdown_window(r, c))
             window.focus()
             redraw = True
         self.existing_dropdown_window = window
         kwargs["window"] = window
         self.existing_dropdown_canvas_id = kwargs["canvas_id"]
         if redraw:
-            self.main_table_redraw_grid_and_text(
-                redraw_header=False, redraw_row_index=False
-            )
+            self.main_table_redraw_grid_and_text(redraw_header=False, redraw_row_index=False)
 
     # displayed indexes, not data
     def close_dropdown_window(self, r=None, c=None, selection=None, redraw=True):
         if r is not None and c is not None and selection is not None:
             datacn = c if self.all_columns_displayed else self.displayed_columns[c]
             datarn = r if self.all_rows_displayed else self.displayed_rows[r]
             kwargs = self.get_cell_kwargs(datarn, datacn, key="dropdown")
-            if (
-                kwargs["select_function"] is not None
-            ):  # user has specified a selection function
-                kwargs["select_function"](
-                    EditCellEvent(
-                        r, c, "ComboboxSelected", f"{selection}", "end_edit_cell"
-                    )
-                )
+            if kwargs["select_function"] is not None:  # user has specified a selection function
+                kwargs["select_function"](EditCellEvent(r, c, "ComboboxSelected", f"{selection}", "end_edit_cell"))
             if self.extra_end_edit_cell_func is None:
                 self.set_cell_data_undo(r, c, value=selection, redraw=not redraw)
-            elif (
-                self.extra_end_edit_cell_func is not None and self.edit_cell_validation
-            ):
+            elif self.extra_end_edit_cell_func is not None and self.edit_cell_validation:
                 validation = self.extra_end_edit_cell_func(
-                    EditCellEvent(
-                        r, c, "ComboboxSelected", f"{selection}", "end_edit_cell"
-                    )
+                    EditCellEvent(r, c, "ComboboxSelected", f"{selection}", "end_edit_cell")
                 )
                 if validation is not None:
                     selection = validation
                 self.set_cell_data_undo(r, c, value=selection, redraw=not redraw)
-            elif (
-                self.extra_end_edit_cell_func is not None
-                and not self.edit_cell_validation
-            ):
+            elif self.extra_end_edit_cell_func is not None and not self.edit_cell_validation:
                 self.set_cell_data_undo(r, c, value=selection, redraw=not redraw)
-                self.extra_end_edit_cell_func(
-                    EditCellEvent(
-                        r, c, "ComboboxSelected", f"{selection}", "end_edit_cell"
-                    )
-                )
+                self.extra_end_edit_cell_func(EditCellEvent(r, c, "ComboboxSelected", f"{selection}", "end_edit_cell"))
             self.focus_set()
             self.recreate_all_selection_boxes()
         self.destroy_text_editor("Escape")
         self.destroy_opened_dropdown_window(r, c)
         if redraw:
             self.refresh()
 
     def get_existing_dropdown_coords(self):
         if self.existing_dropdown_window is not None:
-            return int(self.existing_dropdown_window.r), int(
-                self.existing_dropdown_window.c
-            )
+            return int(self.existing_dropdown_window.r), int(self.existing_dropdown_window.c)
         return None
 
     def mouseclick_outside_editor_or_dropdown(self):
         closed_dd_coords = self.get_existing_dropdown_coords()
         if self.text_editor_loc is not None and self.text_editor is not None:
-            self.close_text_editor(
-                editor_info=self.text_editor_loc + ("ButtonPress-1",)
-            )
+            self.close_text_editor(editor_info=self.text_editor_loc + ("ButtonPress-1",))
         else:
             self.destroy_text_editor("Escape")
         if closed_dd_coords is not None:
             self.destroy_opened_dropdown_window(
                 closed_dd_coords[0], closed_dd_coords[1]
             )  # displayed coords not data, necessary for b1 function
         return closed_dd_coords
@@ -8081,21 +7027,15 @@
     def mouseclick_outside_editor_or_dropdown_all_canvases(self):
         self.CH.mouseclick_outside_editor_or_dropdown()
         self.RI.mouseclick_outside_editor_or_dropdown()
         return self.mouseclick_outside_editor_or_dropdown()
 
     # function can receive 4 None args
     def destroy_opened_dropdown_window(self, r=None, c=None, datarn=None, datacn=None):
-        if (
-            r is None
-            and datarn is None
-            and c is None
-            and datacn is None
-            and self.existing_dropdown_window is not None
-        ):
+        if r is None and datarn is None and c is None and datacn is None and self.existing_dropdown_window is not None:
             r, c = self.get_existing_dropdown_coords()
         if c is not None or datacn is not None:
             if datacn is None:
                 datacn_ = c if self.all_columns_displayed else self.displayed_columns[c]
             else:
                 datacn_ = datacn
         else:
@@ -8130,23 +7070,19 @@
         try:
             return self.displayed_columns.index(datacn)
         except Exception:
             return None
 
     def delete_cell_options_dropdown(self, datarn, datacn):
         self.destroy_opened_dropdown_window()
-        if (datarn, datacn) in self.cell_options and "dropdown" in self.cell_options[
-            (datarn, datacn)
-        ]:
+        if (datarn, datacn) in self.cell_options and "dropdown" in self.cell_options[(datarn, datacn)]:
             del self.cell_options[(datarn, datacn)]["dropdown"]
 
     def delete_cell_options_checkbox(self, datarn, datacn):
-        if (datarn, datacn) in self.cell_options and "checkbox" in self.cell_options[
-            (datarn, datacn)
-        ]:
+        if (datarn, datacn) in self.cell_options and "checkbox" in self.cell_options[(datarn, datacn)]:
             del self.cell_options[(datarn, datacn)]["checkbox"]
 
     def delete_cell_options_dropdown_and_checkbox(self, datarn, datacn):
         self.delete_cell_options_dropdown(datarn, datacn)
         self.delete_cell_options_checkbox(datarn, datacn)
 
     def delete_row_options_dropdown(self, datarn):
```

### Comparing `tksheet-6.1.3/tksheet/_tksheet_other_classes.py` & `tksheet-6.1.4/tksheet/_tksheet_other_classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 import bisect
 import tkinter as tk
 from collections import namedtuple
 from itertools import islice
 
-from ._tksheet_vars import *
+from ._tksheet_vars import (
+    ctrl_key,
+    get_font,
+    rc_binding,
+)
 
 CurrentlySelectedClass = namedtuple("CurrentlySelectedClass", "row column type_")
-CtrlKeyEvent = namedtuple(
-    "CtrlKeyEvent", "eventname selectionboxes currentlyselected rows"
-)
+CtrlKeyEvent = namedtuple("CtrlKeyEvent", "eventname selectionboxes currentlyselected rows")
 PasteEvent = namedtuple("PasteEvent", "eventname currentlyselected rows")
 UndoEvent = namedtuple("UndoEvent", "eventname type storeddata")
 SelectCellEvent = namedtuple("SelectCellEvent", "eventname row column")
 SelectColumnEvent = namedtuple("SelectColumnEvent", "eventname column")
 SelectRowEvent = namedtuple("SelectRowEvent", "eventname row")
 DeselectionEvent = namedtuple("DeselectionEvent", "eventname selectionboxes")
 SelectionBoxEvent = namedtuple("SelectionBoxEvent", "eventname selectionboxes")
 InsertEvent = namedtuple("InsertEvent", "eventname dataindex displayindex quantity")
 DeleteRowColumnEvent = namedtuple("DeleteRowColumnEvent", "eventname deleteindexes")
 EditCellEvent = namedtuple("EditCellEvent", "row column key text eventname")
 EditHeaderEvent = namedtuple("EditHeaderEvent", "column key text eventname")
 EditIndexEvent = namedtuple("EditIndexEvent", "row key text eventname")
 BeginDragDropEvent = namedtuple("BeginDragDropEvent", "eventname columnstomove movedto")
-EndDragDropEvent = namedtuple(
-    "EndDragDropEvent", "eventname oldindexes newindexes movedto"
-)
+EndDragDropEvent = namedtuple("EndDragDropEvent", "eventname oldindexes newindexes movedto")
 ResizeEvent = namedtuple("ResizeEvent", "eventname index oldsize newsize")
-DropDownModifiedEvent = namedtuple(
-    "DropDownModifiedEvent", "eventname row column value"
-)
+DropDownModifiedEvent = namedtuple("DropDownModifiedEvent", "eventname row column value")
 DrawnItem = namedtuple("DrawnItem", "iid showing")
 TextCfg = namedtuple("TextCfg", "txt tf font align")
 DraggedRowColumn = namedtuple("DraggedRowColumn", "dragged to_move")
 _ProgBar = namedtuple("_ProgBar", "bg fg pc name")
 
 
 class TextEditor_(tk.Text):
@@ -146,17 +144,15 @@
             return
         if command in ("insert", "delete", "replace"):
             self.tag_add("align", 1.0, "end")
             self.event_generate("<<TextModified>>")
             if args and len(args) > 1 and args[1] != "\n":
                 out_of_bounds = self.yview()
                 if out_of_bounds != (0.0, 1.0) and self.newline_bindng is not None:
-                    self.newline_bindng(
-                        r=self.parent.r, c=self.parent.c, check_lines=False
-                    )
+                    self.newline_bindng(r=self.parent.r, c=self.parent.c, check_lines=False)
         return result
 
     def rc(self, event):
         self.focus_set()
         self.rc_popup_menu.tk_popup(event.x_root, event.y_root)
 
     def select_all(self, event=None):
@@ -268,17 +264,15 @@
         dd_val = rf"{row[0]}".lower()
         st = dd_val.find(search_for)
         if st > -1:
             # priority is start index
             # if there's already a matching start
             # then compare the len difference
             len_diff = len(dd_val) - search_len
-            if st < best_match["st"] or (
-                st == best_match["st"] and len_diff < best_match["len_diff"]
-            ):
+            if st < best_match["st"] or (st == best_match["st"] and len_diff < best_match["len_diff"]):
                 best_match["rn"] = rn
                 best_match["st"] = st
                 best_match["len_diff"] = len_diff
     if best_match["rn"] != float("inf"):
         return best_match["rn"]
     return None
 
@@ -318,17 +312,15 @@
         "search_function": kwargs["search_function"],
         "validate_input": kwargs["validate_input"],
         "text": kwargs["text"],
         "state": kwargs["state"],
     }
 
 
-def get_checkbox_kwargs(
-    checked=False, state="normal", redraw=True, check_function=None, text="", **kwargs
-):
+def get_checkbox_kwargs(checked=False, state="normal", redraw=True, check_function=None, text="", **kwargs):
     return {
         "checked": checked,
         "state": state,
         "redraw": redraw,
         "check_function": check_function,
         "text": text,
     }
```

### Comparing `tksheet-6.1.3/tksheet/_tksheet_row_index.py` & `tksheet-6.1.4/tksheet/_tksheet_row_index.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,43 @@
 import pickle
 import tkinter as tk
 import zlib
 from collections import defaultdict
 from itertools import accumulate, chain, cycle, islice
 from math import ceil, floor
 
-from ._tksheet_formatters import *
-from ._tksheet_other_classes import *
-from ._tksheet_vars import *
+from ._tksheet_formatters import (
+    is_bool_like,
+    try_to_bool,
+)
+from ._tksheet_other_classes import (
+    BeginDragDropEvent,
+    DraggedRowColumn,
+    DrawnItem,
+    DropDownModifiedEvent,
+    EditHeaderEvent,
+    EditIndexEvent,
+    EndDragDropEvent,
+    ResizeEvent,
+    SelectionBoxEvent,
+    SelectRowEvent,
+    TextCfg,
+    TextEditor,
+    get_checkbox_dict,
+    get_dropdown_dict,
+    get_n2a,
+    get_seq_without_gaps_at_index,
+    num2alpha,
+)
+from ._tksheet_vars import (
+    USER_OS,
+    Color_Map_,
+    rc_binding,
+    symbols_set,
+)
 
 
 class RowIndex(tk.Canvas):
     def __init__(self, *args, **kwargs):
         tk.Canvas.__init__(
             self,
             kwargs["parentframe"],
@@ -162,19 +188,15 @@
         self.mouseclick_outside_editor_or_dropdown_all_canvases()
         self.focus_set()
         popup_menu = None
         if self.MT.identify_row(y=event.y, allow_end=False) is None:
             self.MT.deselect("all")
             if self.MT.rc_popup_menus_enabled:
                 popup_menu = self.MT.empty_rc_popup_menu
-        elif (
-            self.row_selection_enabled
-            and not self.currently_resizing_width
-            and not self.currently_resizing_height
-        ):
+        elif self.row_selection_enabled and not self.currently_resizing_width and not self.currently_resizing_height:
             r = self.MT.identify_row(y=event.y)
             if r < len(self.MT.row_positions) - 1:
                 if self.MT.row_selected(r):
                     if self.MT.rc_popup_menus_enabled:
                         popup_menu = self.ri_rc_popup_menu
                 else:
                     if self.MT.single_selection_enabled and self.MT.rc_select_enabled:
@@ -197,27 +219,21 @@
             and self.rsz_w is None
         ):
             r = self.MT.identify_row(y=event.y)
             if r < len(self.MT.row_positions) - 1:
                 r_selected = self.MT.row_selected(r)
                 if not r_selected and self.row_selection_enabled:
                     self.add_selection(r, set_as_current=True)
-                    self.MT.main_table_redraw_grid_and_text(
-                        redraw_header=True, redraw_row_index=True
-                    )
+                    self.MT.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=True)
                     if self.ctrl_selection_binding_func is not None:
-                        self.ctrl_selection_binding_func(
-                            SelectionBoxEvent("ctrl_select_rows", (r, r + 1))
-                        )
+                        self.ctrl_selection_binding_func(SelectionBoxEvent("ctrl_select_rows", (r, r + 1)))
                 elif r_selected:
                     self.dragged_row = DraggedRowColumn(
                         dragged=r,
-                        to_move=get_seq_without_gaps_at_index(
-                            sorted(self.MT.get_selected_rows()), r
-                        ),
+                        to_move=get_seq_without_gaps_at_index(sorted(self.MT.get_selected_rows()), r),
                     )
         elif not self.MT.ctrl_select_enabled:
             self.b1_press(event)
 
     def ctrl_shift_b1_press(self, event):
         self.mouseclick_outside_editor_or_dropdown_all_canvases()
         y = event.y
@@ -231,85 +247,61 @@
             if r < len(self.MT.row_positions) - 1:
                 r_selected = self.MT.row_selected(r)
                 if not r_selected and self.row_selection_enabled:
                     currently_selected = self.MT.currently_selected()
                     if currently_selected and currently_selected.type_ == "row":
                         min_r = int(currently_selected.row)
                         if r > min_r:
-                            self.MT.create_selected(
-                                min_r, 0, r + 1, len(self.MT.col_positions) - 1, "rows"
-                            )
+                            self.MT.create_selected(min_r, 0, r + 1, len(self.MT.col_positions) - 1, "rows")
                             func_event = tuple(range(min_r, r + 1))
                         elif r < min_r:
-                            self.MT.create_selected(
-                                r, 0, min_r + 1, len(self.MT.col_positions) - 1, "rows"
-                            )
+                            self.MT.create_selected(r, 0, min_r + 1, len(self.MT.col_positions) - 1, "rows")
                             func_event = tuple(range(r, min_r + 1))
                     else:
                         self.add_selection(r, set_as_current=True)
                         func_event = (r,)
-                    self.MT.main_table_redraw_grid_and_text(
-                        redraw_header=True, redraw_row_index=True
-                    )
+                    self.MT.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=True)
                     if self.ctrl_selection_binding_func is not None:
-                        self.ctrl_selection_binding_func(
-                            SelectionBoxEvent("ctrl_select_rows", func_event)
-                        )
+                        self.ctrl_selection_binding_func(SelectionBoxEvent("ctrl_select_rows", func_event))
                 elif r_selected:
                     self.dragged_row = DraggedRowColumn(
                         dragged=r,
-                        to_move=get_seq_without_gaps_at_index(
-                            sorted(self.MT.get_selected_rows()), r
-                        ),
+                        to_move=get_seq_without_gaps_at_index(sorted(self.MT.get_selected_rows()), r),
                     )
         elif not self.MT.ctrl_select_enabled:
             self.shift_b1_press(event)
 
     def shift_b1_press(self, event):
         self.mouseclick_outside_editor_or_dropdown_all_canvases()
         y = event.y
         r = self.MT.identify_row(y=y)
-        if (
-            (self.drag_and_drop_enabled or self.row_selection_enabled)
-            and self.rsz_h is None
-            and self.rsz_w is None
-        ):
+        if (self.drag_and_drop_enabled or self.row_selection_enabled) and self.rsz_h is None and self.rsz_w is None:
             if r < len(self.MT.row_positions) - 1:
                 r_selected = self.MT.row_selected(r)
                 if not r_selected and self.row_selection_enabled:
                     currently_selected = self.MT.currently_selected()
                     if currently_selected and currently_selected.type_ == "row":
                         min_r = int(currently_selected.row)
                         self.MT.delete_selection_rects(delete_current=False)
                         if r > min_r:
-                            self.MT.create_selected(
-                                min_r, 0, r + 1, len(self.MT.col_positions) - 1, "rows"
-                            )
+                            self.MT.create_selected(min_r, 0, r + 1, len(self.MT.col_positions) - 1, "rows")
                             func_event = tuple(range(min_r, r + 1))
                         elif r < min_r:
-                            self.MT.create_selected(
-                                r, 0, min_r + 1, len(self.MT.col_positions) - 1, "rows"
-                            )
+                            self.MT.create_selected(r, 0, min_r + 1, len(self.MT.col_positions) - 1, "rows")
                             func_event = tuple(range(r, min_r + 1))
                     else:
                         self.select_row(r)
                         func_event = (r,)
-                    self.MT.main_table_redraw_grid_and_text(
-                        redraw_header=True, redraw_row_index=True
-                    )
+                    self.MT.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=True)
                     if self.shift_selection_binding_func is not None:
-                        self.shift_selection_binding_func(
-                            SelectionBoxEvent("shift_select_rows", func_event)
-                        )
+                        self.shift_selection_binding_func(SelectionBoxEvent("shift_select_rows", func_event))
                 elif r_selected:
                     self.dragged_row = DraggedRowColumn(
                         dragged=r,
-                        to_move=get_seq_without_gaps_at_index(
-                            sorted(self.MT.get_selected_rows()), r
-                        ),
+                        to_move=get_seq_without_gaps_at_index(sorted(self.MT.get_selected_rows()), r),
                     )
 
     def create_resize_line(self, x1, y1, x2, y2, width, fill, tag):
         if self.hidd_resize_lines:
             t, sh = self.hidd_resize_lines.popitem()
             self.coords(t, x1, y1, x2, y2)
             if sh:
@@ -374,26 +366,19 @@
         if (
             self.double_click_resizing_enabled
             and self.height_resizing_enabled
             and self.rsz_h is not None
             and not self.currently_resizing_height
         ):
             row = self.rsz_h - 1
-            old_height = (
-                self.MT.row_positions[self.rsz_h]
-                - self.MT.row_positions[self.rsz_h - 1]
-            )
+            old_height = self.MT.row_positions[self.rsz_h] - self.MT.row_positions[self.rsz_h - 1]
             new_height = self.set_row_height(row)
-            self.MT.main_table_redraw_grid_and_text(
-                redraw_header=True, redraw_row_index=True
-            )
+            self.MT.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=True)
             if self.row_height_resize_func is not None and old_height != new_height:
-                self.row_height_resize_func(
-                    ResizeEvent("row_height_resize", row, old_height, new_height)
-                )
+                self.row_height_resize_func(ResizeEvent("row_height_resize", row, old_height, new_height))
         elif self.width_resizing_enabled and self.rsz_h is None and self.rsz_w:
             self.set_width_of_index_to_text()
         elif self.row_selection_enabled and self.rsz_h is None and self.rsz_w is None:
             r = self.MT.identify_row(y=event.y)
             if r < len(self.MT.row_positions) - 1:
                 if self.MT.single_selection_enabled:
                     self.select_row(r, redraw=True)
@@ -438,55 +423,47 @@
                 y,
                 self.current_width,
                 y,
                 width=1,
                 fill=self.resizing_line_fg,
                 tag="rhl",
             )
-            self.MT.create_resize_line(
-                x1, y, x2, y, width=1, fill=self.resizing_line_fg, tag="rhl"
-            )
+            self.MT.create_resize_line(x1, y, x2, y, width=1, fill=self.resizing_line_fg, tag="rhl")
             self.create_resize_line(
                 0,
                 line2y,
                 self.current_width,
                 line2y,
                 width=1,
                 fill=self.resizing_line_fg,
                 tag="rhl2",
             )
-            self.MT.create_resize_line(
-                x1, line2y, x2, line2y, width=1, fill=self.resizing_line_fg, tag="rhl2"
-            )
+            self.MT.create_resize_line(x1, line2y, x2, line2y, width=1, fill=self.resizing_line_fg, tag="rhl2")
         elif self.width_resizing_enabled and self.rsz_h is None and self.rsz_w:
             self.currently_resizing_width = True
             x1, y1, x2, y2 = self.MT.get_canvas_visible_area()
             x = int(event.x)
             if x < self.MT.min_column_width:
                 x = int(self.MT.min_column_width)
             self.new_row_width = x
-            self.create_resize_line(
-                x, y1, x, y2, width=1, fill=self.resizing_line_fg, tag="rwl"
-            )
+            self.create_resize_line(x, y1, x, y2, width=1, fill=self.resizing_line_fg, tag="rwl")
         elif self.MT.identify_row(y=event.y, allow_end=False) is None:
             self.MT.deselect("all")
         elif self.row_selection_enabled and self.rsz_h is None and self.rsz_w is None:
             r = self.MT.identify_row(y=event.y)
             if r < len(self.MT.row_positions) - 1:
                 datarn = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
                 if (
                     self.MT.row_selected(r)
                     and not self.event_over_dropdown(r, datarn, event, y)
                     and not self.event_over_checkbox(r, datarn, event, y)
                 ):
                     self.dragged_row = DraggedRowColumn(
                         dragged=r,
-                        to_move=get_seq_without_gaps_at_index(
-                            sorted(self.MT.get_selected_rows()), r
-                        ),
+                        to_move=get_seq_without_gaps_at_index(sorted(self.MT.get_selected_rows()), r),
                     )
                 else:
                     self.being_drawn_rect = (
                         r,
                         0,
                         r + 1,
                         len(self.MT.col_positions) - 1,
@@ -497,36 +474,30 @@
                     elif self.MT.toggle_selection_enabled:
                         self.toggle_select_row(r, redraw=True)
         if self.extra_b1_press_func is not None:
             self.extra_b1_press_func(event)
 
     def b1_motion(self, event):
         x1, y1, x2, y2 = self.MT.get_canvas_visible_area()
-        if (
-            self.height_resizing_enabled
-            and self.rsz_h is not None
-            and self.currently_resizing_height
-        ):
+        if self.height_resizing_enabled and self.rsz_h is not None and self.currently_resizing_height:
             y = self.canvasy(event.y)
             size = y - self.MT.row_positions[self.rsz_h - 1]
             if size >= self.MT.min_row_height and size < self.MT.max_row_height:
                 self.delete_all_resize_and_ctrl_lines(ctrl_lines=False)
                 line2y = self.MT.row_positions[self.rsz_h - 1]
                 self.create_resize_line(
                     0,
                     y,
                     self.current_width,
                     y,
                     width=1,
                     fill=self.resizing_line_fg,
                     tag="rhl",
                 )
-                self.MT.create_resize_line(
-                    x1, y, x2, y, width=1, fill=self.resizing_line_fg, tag="rhl"
-                )
+                self.MT.create_resize_line(x1, y, x2, y, width=1, fill=self.resizing_line_fg, tag="rhl")
                 self.create_resize_line(
                     0,
                     line2y,
                     self.current_width,
                     line2y,
                     width=1,
                     fill=self.resizing_line_fg,
@@ -537,38 +508,30 @@
                     line2y,
                     x2,
                     line2y,
                     width=1,
                     fill=self.resizing_line_fg,
                     tag="rhl2",
                 )
-        elif (
-            self.width_resizing_enabled
-            and self.rsz_w is not None
-            and self.currently_resizing_width
-        ):
+        elif self.width_resizing_enabled and self.rsz_w is not None and self.currently_resizing_width:
             evx = event.x
             self.delete_all_resize_and_ctrl_lines(ctrl_lines=False)
             if evx > self.current_width:
                 x = self.MT.canvasx(evx - self.current_width)
                 if evx > self.MT.max_index_width:
                     evx = int(self.MT.max_index_width)
                     x = self.MT.canvasx(evx - self.current_width)
                 self.new_row_width = evx
-                self.MT.create_resize_line(
-                    x, y1, x, y2, width=1, fill=self.resizing_line_fg, tag="rwl"
-                )
+                self.MT.create_resize_line(x, y1, x, y2, width=1, fill=self.resizing_line_fg, tag="rwl")
             else:
                 x = evx
                 if x < self.MT.min_column_width:
                     x = int(self.MT.min_column_width)
                 self.new_row_width = x
-                self.create_resize_line(
-                    x, y1, x, y2, width=1, fill=self.resizing_line_fg, tag="rwl"
-                )
+                self.create_resize_line(x, y1, x, y2, width=1, fill=self.resizing_line_fg, tag="rwl")
         if (
             self.drag_and_drop_enabled
             and self.row_selection_enabled
             and self.rsz_h is None
             and self.rsz_w is None
             and self.dragged_row is not None
             and self.MT.anything_selected(exclude_cells=True, exclude_columns=True)
@@ -579,18 +542,15 @@
                     self.drag_and_drop_motion(event),
                     x1,
                     x2,
                     self.dragged_row.to_move[0],
                     self.dragged_row.to_move[-1],
                 )
         elif (
-            self.MT.drag_selection_enabled
-            and self.row_selection_enabled
-            and self.rsz_h is None
-            and self.rsz_w is None
+            self.MT.drag_selection_enabled and self.row_selection_enabled and self.rsz_h is None and self.rsz_w is None
         ):
             need_redraw = False
             end_row = self.MT.identify_row(y=event.y)
             currently_selected = self.MT.currently_selected()
             if end_row < len(self.MT.row_positions) - 1 and currently_selected:
                 if currently_selected.type_ == "row":
                     start_row = currently_selected.row
@@ -614,23 +574,19 @@
                         func_event = tuple(range(end_row, start_row + 1))
                     if self.being_drawn_rect != rect:
                         need_redraw = True
                         self.MT.delete_selection_rects(delete_current=False)
                         self.MT.create_selected(*rect)
                         self.being_drawn_rect = rect
                         if self.drag_selection_binding_func is not None:
-                            self.drag_selection_binding_func(
-                                SelectionBoxEvent("drag_select_rows", func_event)
-                            )
+                            self.drag_selection_binding_func(SelectionBoxEvent("drag_select_rows", func_event))
             if self.scroll_if_event_offscreen(event):
                 need_redraw = True
             if need_redraw:
-                self.MT.main_table_redraw_grid_and_text(
-                    redraw_header=False, redraw_row_index=True
-                )
+                self.MT.main_table_redraw_grid_and_text(redraw_header=False, redraw_row_index=True)
         if self.extra_b1_motion_func is not None:
             self.extra_b1_motion_func(event)
 
     def ctrl_b1_motion(self, event):
         x1, y1, x2, y2 = self.MT.get_canvas_visible_area()
         if (
             self.drag_and_drop_enabled
@@ -683,23 +639,19 @@
                     if self.being_drawn_rect != rect:
                         need_redraw = True
                         if self.being_drawn_rect is not None:
                             self.MT.delete_selected(*self.being_drawn_rect)
                         self.MT.create_selected(*rect)
                         self.being_drawn_rect = rect
                         if self.drag_selection_binding_func is not None:
-                            self.drag_selection_binding_func(
-                                SelectionBoxEvent("drag_select_rows", func_event)
-                            )
+                            self.drag_selection_binding_func(SelectionBoxEvent("drag_select_rows", func_event))
             if self.scroll_if_event_offscreen(event):
                 need_redraw = True
             if need_redraw:
-                self.MT.main_table_redraw_grid_and_text(
-                    redraw_header=False, redraw_row_index=True
-                )
+                self.MT.main_table_redraw_grid_and_text(redraw_header=False, redraw_row_index=True)
         elif not self.MT.ctrl_select_enabled:
             self.b1_motion(event)
 
     def drag_and_drop_motion(self, event):
         y = event.y
         hend = self.winfo_height()
         ycheck = self.yview()
@@ -724,31 +676,33 @@
         row = self.MT.identify_row(y=event.y)
         if row >= self.dragged_row.to_move[0] and row <= self.dragged_row.to_move[-1]:
             ypos = self.MT.row_positions[self.dragged_row.to_move[0]]
         else:
             if row < self.dragged_row.to_move[0]:
                 ypos = self.MT.row_positions[row]
             else:
-                ypos = self.MT.row_positions[row + 1] if len(self.MT.row_positions) - 1 > row else self.MT.row_positions[row]
+                ypos = (
+                    self.MT.row_positions[row + 1]
+                    if len(self.MT.row_positions) - 1 > row
+                    else self.MT.row_positions[row]
+                )
         return ypos
 
     def show_drag_and_drop_indicators(self, ypos, x1, x2, start_row, end_row):
         self.delete_all_resize_and_ctrl_lines()
         self.create_resize_line(
             0,
             ypos,
             self.current_width,
             ypos,
             width=3,
             fill=self.drag_and_drop_bg,
             tag="dd",
         )
-        self.MT.create_resize_line(
-            x1, ypos, x2, ypos, width=3, fill=self.drag_and_drop_bg, tag="dd"
-        )
+        self.MT.create_resize_line(x1, ypos, x2, ypos, width=3, fill=self.drag_and_drop_bg, tag="dd")
         self.MT.show_ctrl_outline(
             start_cell=(0, start_row),
             end_cell=(len(self.MT.col_positions) - 1, end_row + 1),
             dash=(),
             outline=self.drag_and_drop_bg,
             delete_on_timer=False,
         )
@@ -766,20 +720,15 @@
             try:
                 self.MT.yview_scroll(1, "units")
                 self.yview_scroll(1, "units")
             except Exception:
                 pass
             self.fix_yview()
             need_redraw = True
-        elif (
-            event.y < 0
-            and self.canvasy(self.winfo_height()) > 0
-            and ycheck
-            and ycheck[0] > 0
-        ):
+        elif event.y < 0 and self.canvasy(self.winfo_height()) > 0 and ycheck and ycheck[0] > 0:
             try:
                 self.yview_scroll(-1, "units")
                 self.MT.yview_scroll(-1, "units")
             except Exception:
                 pass
             self.fix_yview()
             need_redraw = True
@@ -813,68 +762,39 @@
     def b1_release(self, event=None):
         if self.being_drawn_rect is not None:
             self.MT.delete_selected(*self.being_drawn_rect)
             to_sel = tuple(self.being_drawn_rect)
             self.being_drawn_rect = None
             self.MT.create_selected(*to_sel)
         self.MT.bind("<MouseWheel>", self.MT.mousewheel)
-        if (
-            self.height_resizing_enabled
-            and self.rsz_h is not None
-            and self.currently_resizing_height
-        ):
+        if self.height_resizing_enabled and self.rsz_h is not None and self.currently_resizing_height:
             self.currently_resizing_height = False
             new_row_pos = int(self.coords("rhl")[1])
             self.delete_all_resize_and_ctrl_lines(ctrl_lines=False)
-            old_height = (
-                self.MT.row_positions[self.rsz_h]
-                - self.MT.row_positions[self.rsz_h - 1]
-            )
+            old_height = self.MT.row_positions[self.rsz_h] - self.MT.row_positions[self.rsz_h - 1]
             size = new_row_pos - self.MT.row_positions[self.rsz_h - 1]
             if size < self.MT.min_row_height:
-                new_row_pos = ceil(
-                    self.MT.row_positions[self.rsz_h - 1] + self.MT.min_row_height
-                )
+                new_row_pos = ceil(self.MT.row_positions[self.rsz_h - 1] + self.MT.min_row_height)
             elif size > self.MT.max_row_height:
-                new_row_pos = floor(
-                    self.MT.row_positions[self.rsz_h - 1] + self.MT.max_row_height
-                )
+                new_row_pos = floor(self.MT.row_positions[self.rsz_h - 1] + self.MT.max_row_height)
             increment = new_row_pos - self.MT.row_positions[self.rsz_h]
             self.MT.row_positions[self.rsz_h + 1 :] = [
-                e + increment
-                for e in islice(
-                    self.MT.row_positions, self.rsz_h + 1, len(self.MT.row_positions)
-                )
+                e + increment for e in islice(self.MT.row_positions, self.rsz_h + 1, len(self.MT.row_positions))
             ]
             self.MT.row_positions[self.rsz_h] = new_row_pos
-            new_height = (
-                self.MT.row_positions[self.rsz_h]
-                - self.MT.row_positions[self.rsz_h - 1]
-            )
+            new_height = self.MT.row_positions[self.rsz_h] - self.MT.row_positions[self.rsz_h - 1]
             self.MT.recreate_all_selection_boxes()
-            self.MT.main_table_redraw_grid_and_text(
-                redraw_header=True, redraw_row_index=True
-            )
+            self.MT.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=True)
             if self.row_height_resize_func is not None and old_height != new_height:
-                self.row_height_resize_func(
-                    ResizeEvent(
-                        "row_height_resize", self.rsz_h - 1, old_height, new_height
-                    )
-                )
-        elif (
-            self.width_resizing_enabled
-            and self.rsz_w is not None
-            and self.currently_resizing_width
-        ):
+                self.row_height_resize_func(ResizeEvent("row_height_resize", self.rsz_h - 1, old_height, new_height))
+        elif self.width_resizing_enabled and self.rsz_w is not None and self.currently_resizing_width:
             self.currently_resizing_width = False
             self.delete_all_resize_and_ctrl_lines(ctrl_lines=False)
             self.set_width(self.new_row_width, set_TL=True)
-            self.MT.main_table_redraw_grid_and_text(
-                redraw_header=True, redraw_row_index=True
-            )
+            self.MT.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=True)
         if (
             self.drag_and_drop_enabled
             and self.MT.anything_selected(exclude_cells=True, exclude_columns=True)
             and self.row_selection_enabled
             and self.rsz_h is None
             and self.rsz_w is None
             and self.dragged_row is not None
@@ -882,17 +802,15 @@
             self.delete_all_resize_and_ctrl_lines()
             y = event.y
             r = self.MT.identify_row(y=y)
             orig_selected = self.dragged_row.to_move
             if (
                 r != self.dragged_row
                 and r is not None
-                and (
-                    r < self.dragged_row.to_move[0] or r > self.dragged_row.to_move[-1]
-                )
+                and (r < self.dragged_row.to_move[0] or r > self.dragged_row.to_move[-1])
                 and len(orig_selected) != (len(self.MT.row_positions) - 1)
             ):
                 rm1start = orig_selected[0]
                 totalrows = len(orig_selected)
                 extra_func_success = True
                 if r >= len(self.MT.row_positions) - 1:
                     r -= 1
@@ -909,48 +827,40 @@
                         extra_func_success = False
                 if extra_func_success:
                     new_selected, dispset = self.MT.move_rows_adjust_options_dict(
                         r, rm1start, totalrows, move_data=self.row_drag_and_drop_perform
                     )
                     if self.MT.undo_enabled:
                         self.MT.undo_storage.append(
-                            zlib.compress(
-                                pickle.dumps(("move_rows", orig_selected, new_selected))
-                            )
+                            zlib.compress(pickle.dumps(("move_rows", orig_selected, new_selected)))
                         )
-                    self.MT.main_table_redraw_grid_and_text(
-                        redraw_header=True, redraw_row_index=True
-                    )
+                    self.MT.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=True)
                     if self.ri_extra_end_drag_drop_func is not None:
                         self.ri_extra_end_drag_drop_func(
                             EndDragDropEvent(
                                 "end_row_index_drag_drop",
                                 orig_selected,
                                 new_selected,
                                 int(r),
                             )
                         )
                     self.parentframe.emit_event("<<SheetModified>>")
-        elif (
-            self.b1_pressed_loc is not None
-            and self.rsz_w is None
-            and self.rsz_h is None
-        ):
+        elif self.b1_pressed_loc is not None and self.rsz_w is None and self.rsz_h is None:
             r = self.MT.identify_row(y=event.y)
             if (
                 r is not None
                 and r < len(self.MT.row_positions) - 1
                 and r == self.b1_pressed_loc
                 and self.b1_pressed_loc != self.closed_dropdown
             ):
                 datarn = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
                 canvasy = self.canvasy(event.y)
-                if self.event_over_dropdown(
+                if self.event_over_dropdown(r, datarn, event, canvasy) or self.event_over_checkbox(
                     r, datarn, event, canvasy
-                ) or self.event_over_checkbox(r, datarn, event, canvasy):
+                ):
                     self.open_cell(event)
             else:
                 self.mouseclick_outside_editor_or_dropdown_all_canvases()
             self.b1_pressed_loc = None
             self.closed_dropdown = None
         self.dragged_row = None
         self.currently_resizing_width = False
@@ -1001,48 +911,38 @@
                 self.select_row(row, redraw=redraw)
 
     def select_row(self, r, redraw=False):
         self.MT.delete_selection_rects()
         self.MT.create_selected(r, 0, r + 1, len(self.MT.col_positions) - 1, "rows")
         self.MT.set_currently_selected(r, 0, type_="row")
         if redraw:
-            self.MT.main_table_redraw_grid_and_text(
-                redraw_header=True, redraw_row_index=True
-            )
+            self.MT.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=True)
         if self.selection_binding_func is not None:
             self.selection_binding_func(SelectRowEvent("select_row", int(r)))
 
-    def add_selection(
-        self, r, redraw=False, run_binding_func=True, set_as_current=True
-    ):
+    def add_selection(self, r, redraw=False, run_binding_func=True, set_as_current=True):
         if set_as_current:
             self.MT.set_currently_selected(r, 0, type_="row")
         self.MT.create_selected(r, 0, r + 1, len(self.MT.col_positions) - 1, "rows")
         if redraw:
-            self.MT.main_table_redraw_grid_and_text(
-                redraw_header=False, redraw_row_index=True
-            )
+            self.MT.main_table_redraw_grid_and_text(redraw_header=False, redraw_row_index=True)
         if self.selection_binding_func is not None and run_binding_func:
             self.selection_binding_func(("select_row", r))
 
     def get_cell_dimensions(self, datarn):
         txt = self.get_valid_cell_data_as_str(datarn, fix=False)
         if txt:
-            self.MT.txt_measure_canvas.itemconfig(
-                self.MT.txt_measure_canvas_text, text=txt, font=self.MT.index_font
-            )
+            self.MT.txt_measure_canvas.itemconfig(self.MT.txt_measure_canvas_text, text=txt, font=self.MT.index_font)
             b = self.MT.txt_measure_canvas.bbox(self.MT.txt_measure_canvas_text)
             w = b[2] - b[0] + 7
             h = b[3] - b[1] + 5
         else:
             w = self.MT.default_index_width
             h = self.MT.min_row_height
-        if self.get_cell_kwargs(datarn, key="dropdown") or self.get_cell_kwargs(
-            datarn, key="checkbox"
-        ):
+        if self.get_cell_kwargs(datarn, key="dropdown") or self.get_cell_kwargs(datarn, key="checkbox"):
             return w + self.MT.txt_h, h
         return w, h
 
     def set_row_height(
         self,
         row,
         height=None,
@@ -1079,17 +979,15 @@
                 h = int(min_rh)
             elif h > self.MT.max_row_height:
                 h = int(self.MT.max_row_height)
             if h > new_height:
                 new_height = h
             if self.MT.data:
                 for datacn in iterable:
-                    txt = self.MT.get_valid_cell_data_as_str(
-                        datarn, datacn, get_displayed=True
-                    )
+                    txt = self.MT.get_valid_cell_data_as_str(datarn, datacn, get_displayed=True)
                     if txt:
                         h = self.MT.get_txt_h(txt) + 5
                     else:
                         h = min_rh
                     if h < min_rh:
                         h = int(min_rh)
                     elif h > self.MT.max_row_height:
@@ -1098,28 +996,21 @@
                         new_height = h
         else:
             new_height = int(height)
         if new_height < min_rh:
             new_height = int(min_rh)
         elif new_height > self.MT.max_row_height:
             new_height = int(self.MT.max_row_height)
-        if (
-            only_set_if_too_small
-            and new_height
-            <= self.MT.row_positions[row + 1] - self.MT.row_positions[row]
-        ):
+        if only_set_if_too_small and new_height <= self.MT.row_positions[row + 1] - self.MT.row_positions[row]:
             return self.MT.row_positions[row + 1] - self.MT.row_positions[row]
         if not return_new_height:
             new_row_pos = self.MT.row_positions[row] + new_height
             increment = new_row_pos - self.MT.row_positions[r_norm]
             self.MT.row_positions[r_extra:] = [
-                e + increment
-                for e in islice(
-                    self.MT.row_positions, r_extra, len(self.MT.row_positions)
-                )
+                e + increment for e in islice(self.MT.row_positions, r_extra, len(self.MT.row_positions))
             ]
             self.MT.row_positions[r_norm] = new_row_pos
             if recreate:
                 self.MT.recreate_all_selection_boxes()
         return new_height
 
     def set_width_of_index_to_text(self, text=None):
@@ -1165,17 +1056,15 @@
                     elif self.get_cell_kwargs(datarn, key="dropdown"):
                         w += self.MT.txt_h + 4
                     if w > new_width:
                         new_width = w
             elif isinstance(self.MT._row_index, int):
                 datacn = self.MT._row_index
                 for datarn in iterable:
-                    txt = self.MT.get_valid_cell_data_as_str(
-                        datarn, datacn, get_displayed=True
-                    )
+                    txt = self.MT.get_valid_cell_data_as_str(datarn, datacn, get_displayed=True)
                     if txt:
                         qconf(qtxtm, text=txt)
                         b = qbbox(qtxtm)
                         w = b[2] - b[0] + 10
                     else:
                         w = self.MT.default_index_width
                     if w < self.MT.min_column_width:
@@ -1183,21 +1072,17 @@
                     elif w > self.MT.max_index_width:
                         w = int(self.MT.max_index_width)
                     if w > new_width:
                         new_width = w
         if new_width == self.MT.min_column_width:
             new_width = self.MT.min_column_width + 10
         self.set_width(new_width, set_TL=True)
-        self.MT.main_table_redraw_grid_and_text(
-            redraw_header=True, redraw_row_index=True
-        )
+        self.MT.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=True)
 
-    def set_height_of_all_rows(
-        self, height=None, only_set_if_too_small=False, recreate=True
-    ):
+    def set_height_of_all_rows(self, height=None, only_set_if_too_small=False, recreate=True):
         if height is None:
             self.MT.row_positions = list(
                 accumulate(
                     chain(
                         [0],
                         (
                             self.set_row_height(
@@ -1208,17 +1093,15 @@
                             )
                             for rn in range(len(self.MT.data))
                         ),
                     )
                 )
             )
         else:
-            self.MT.row_positions = list(
-                accumulate(chain([0], (height for r in range(len(self.MT.data)))))
-            )
+            self.MT.row_positions = list(accumulate(chain([0], (height for r in range(len(self.MT.data))))))
         if recreate:
             self.MT.recreate_all_selection_boxes()
 
     def align_cells(self, rows=[], align="global"):
         if isinstance(rows, int):
             rows = [rows]
         else:
@@ -1230,19 +1113,15 @@
         else:
             for r in rows:
                 if r not in self.cell_options:
                     self.cell_options[r] = {}
                 self.cell_options[r]["align"] = align
 
     def auto_set_index_width(self, end_row):
-        if (
-            not self.MT._row_index
-            and not isinstance(self.MT._row_index, int)
-            and self.auto_resize_width
-        ):
+        if not self.MT._row_index and not isinstance(self.MT._row_index, int) and self.auto_resize_width:
             if self.default_index == "letters":
                 new_w = self.MT.get_txt_w(f"{num2alpha(end_row)}") + 20
                 if self.current_width - new_w > 15 or new_w - self.current_width > 5:
                     self.set_width(new_w, set_TL=True)
                     return True
             elif self.default_index == "numbers":
                 new_w = self.MT.get_txt_w(f"{end_row}") + 20
@@ -1294,16 +1173,15 @@
                 redrawn = self.redraw_highlight(
                     0,
                     fr + 1,
                     self.current_width - 1,
                     sr,
                     fill=fill,
                     outline=self.index_fg
-                    if self.get_cell_kwargs(datarn, key="dropdown")
-                    and self.MT.show_dropdown_borders
+                    if self.get_cell_kwargs(datarn, key="dropdown") and self.MT.show_dropdown_borders
                     else "",
                     tag="s",
                 )
         elif not kwargs:
             if "rows" in selections and r in selections["rows"]:
                 tf = self.index_selected_rows_fg
             elif "cells" in selections and r in selections["cells"]:
@@ -1315,27 +1193,23 @@
     def redraw_highlight(self, x1, y1, x2, y2, fill, outline, tag):
         config = (fill, outline)
         coords = (x1, y1, x2, y2)
         k = None
         if config in self.hidd_high:
             k = config
             iid, showing = self.hidd_high[k].pop()
-            if all(
-                int(crd1) == int(crd2) for crd1, crd2 in zip(self.coords(iid), coords)
-            ):
+            if all(int(crd1) == int(crd2) for crd1, crd2 in zip(self.coords(iid), coords)):
                 option = 0 if showing else 2
             else:
                 option = 1 if showing else 3
 
         elif self.hidd_high:
             k = next(iter(self.hidd_high))
             iid, showing = self.hidd_high[k].pop()
-            if all(
-                int(crd1) == int(crd2) for crd1, crd2 in zip(self.coords(iid), coords)
-            ):
+            if all(int(crd1) == int(crd2) for crd1, crd2 in zip(self.coords(iid), coords)):
                 option = 2 if showing else 3
             else:
                 option = 3
 
         else:
             iid, showing, option = (
                 self.create_rectangle(coords, fill=fill, outline=outline, tag=tag),
@@ -1345,17 +1219,15 @@
 
         if option in (1, 3):
             self.coords(iid, coords)
         if option in (2, 3):
             if showing:
                 self.itemconfig(iid, fill=fill, outline=outline)
             else:
-                self.itemconfig(
-                    iid, fill=fill, outline=outline, tag=tag, state="normal"
-                )
+                self.itemconfig(iid, fill=fill, outline=outline, tag=tag, state="normal")
 
         if k is not None and not self.hidd_high[k]:
             del self.hidd_high[k]
 
         self.disp_high[config].add(DrawnItem(iid=iid, showing=1))
         return True
 
@@ -1365,17 +1237,15 @@
             self.coords(t, points)
             if sh:
                 self.itemconfig(t, fill=fill, width=width, tag=tag)
             else:
                 self.itemconfig(t, fill=fill, width=width, tag=tag, state="normal")
             self.disp_grid[t] = True
         else:
-            self.disp_grid[
-                self.create_line(points, fill=fill, width=width, tag=tag)
-            ] = True
+            self.disp_grid[self.create_line(points, fill=fill, width=width, tag=tag)] = True
 
     def redraw_dropdown(
         self,
         x1,
         y1,
         x2,
         y2,
@@ -1383,17 +1253,15 @@
         outline,
         tag,
         draw_outline=True,
         draw_arrow=True,
         dd_is_open=False,
     ):
         if draw_outline and self.MT.show_dropdown_borders:
-            self.redraw_highlight(
-                x1 + 1, y1 + 1, x2, y2, fill="", outline=self.index_fg, tag=tag
-            )
+            self.redraw_highlight(x1 + 1, y1 + 1, x2, y2, fill="", outline=self.index_fg, tag=tag)
         if draw_arrow:
             topysub = floor(self.MT.half_txt_h / 2)
             mid_y = y1 + floor(self.MT.min_row_height / 2)
             if mid_y + topysub + 1 >= y1 + self.MT.txt_h - 1:
                 mid_y -= 1
             if mid_y - topysub + 2 <= y1 + 4 + topysub:
                 mid_y -= 1
@@ -1438,39 +1306,33 @@
             self.coords(t, points)
             if sh:
                 self.itemconfig(t, fill=outline, outline=fill)
             else:
                 self.itemconfig(t, fill=outline, outline=fill, tag=tag, state="normal")
             self.lift(t)
         else:
-            t = self.create_polygon(
-                points, fill=outline, outline=fill, tag=tag, smooth=True
-            )
+            t = self.create_polygon(points, fill=outline, outline=fill, tag=tag, smooth=True)
         self.disp_checkbox[t] = True
         if draw_check:
             # draw filled box
             x1 = x1 + 4
             y1 = y1 + 4
             x2 = x2 - 3
             y2 = y2 - 3
             points = self.MT.get_checkbox_points(x1, y1, x2, y2, radius=4)
             if self.hidd_checkbox:
                 t, sh = self.hidd_checkbox.popitem()
                 self.coords(t, points)
                 if sh:
                     self.itemconfig(t, fill=fill, outline=outline)
                 else:
-                    self.itemconfig(
-                        t, fill=fill, outline=outline, tag=tag, state="normal"
-                    )
+                    self.itemconfig(t, fill=fill, outline=outline, tag=tag, state="normal")
                 self.lift(t)
             else:
-                t = self.create_polygon(
-                    points, fill=fill, outline=outline, tag=tag, smooth=True
-                )
+                t = self.create_polygon(points, fill=fill, outline=outline, tag=tag, smooth=True)
             self.disp_checkbox[t] = True
 
     def redraw_grid_and_text(
         self,
         last_row_line_pos,
         scrollpos_top,
         y_stop,
@@ -1513,17 +1375,15 @@
         xend = self.current_width - 6
         self.row_width_resize_bbox = (
             self.current_width - 2,
             scrollpos_top,
             self.current_width,
             scrollpos_bot,
         )
-        if (
-            self.MT.show_horizontal_grid or self.height_resizing_enabled
-        ) and row_pos_exists:
+        if (self.MT.show_horizontal_grid or self.height_resizing_enabled) and row_pos_exists:
             self.grid_cyc = cycle(self.grid_cyctup)
             points = [
                 self.current_width - 1,
                 y_stop - 1,
                 self.current_width - 1,
                 scrollpos_top - 1,
                 -1,
@@ -1538,36 +1398,30 @@
                     points.extend(
                         [
                             -1,
                             draw_y,
                             self.current_width,
                             draw_y,
                             self.current_width,
-                            self.MT.row_positions[r + 1]
-                            if len(self.MT.row_positions) - 1 > r
-                            else draw_y,
+                            self.MT.row_positions[r + 1] if len(self.MT.row_positions) - 1 > r else draw_y,
                         ]
                     )
                 elif st_or_end == "end":
                     points.extend(
                         [
                             self.current_width,
                             draw_y,
                             -1,
                             draw_y,
                             -1,
-                            self.MT.row_positions[r + 1]
-                            if len(self.MT.row_positions) - 1 > r
-                            else draw_y,
+                            self.MT.row_positions[r + 1] if len(self.MT.row_positions) - 1 > r else draw_y,
                         ]
                     )
                 if points:
-                    self.redraw_gridline(
-                        points=points, fill=self.index_grid_fg, width=1, tag="h"
-                    )
+                    self.redraw_gridline(points=points, fill=self.index_grid_fg, width=1, tag="h")
         c_2 = (
             self.index_selected_cells_bg
             if self.index_selected_cells_bg.startswith("#")
             else Color_Map_[self.index_selected_cells_bg]
         )
         c_3 = (
             self.index_selected_rows_bg
@@ -1578,17 +1432,15 @@
         selections = self.get_redraw_selections(start_row, end_row)
         for r in range(start_row, end_row - 1):
             rtopgridln = self.MT.row_positions[r]
             rbotgridln = self.MT.row_positions[r + 1]
             if rbotgridln - rtopgridln < self.MT.txt_h:
                 continue
             datarn = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
-            fill, dd_drawn = self.redraw_highlight_get_text_fg(
-                rtopgridln, rbotgridln, r, c_2, c_3, selections, datarn
-            )
+            fill, dd_drawn = self.redraw_highlight_get_text_fg(rtopgridln, rbotgridln, r, c_2, c_3, selections, datarn)
 
             if datarn in self.cell_options and "align" in self.cell_options[datarn]:
                 align = self.cell_options[datarn]["align"]
             else:
                 align = self.align
             dropdown_kwargs = self.get_cell_kwargs(datarn, key="dropdown")
             if align == "w":
@@ -1670,40 +1522,33 @@
                     except Exception:
                         draw_check = False
                     self.redraw_checkbox(
                         2,
                         rtopgridln + 2,
                         self.MT.txt_h + 3,
                         rtopgridln + self.MT.txt_h + 3,
-                        fill=fill
-                        if checkbox_kwargs["state"] == "normal"
-                        else self.index_grid_fg,
+                        fill=fill if checkbox_kwargs["state"] == "normal" else self.index_grid_fg,
                         outline="",
                         tag="cb",
                         draw_check=draw_check,
                     )
             lns = self.get_valid_cell_data_as_str(datarn, fix=False).split("\n")
             if lns == [""]:
                 if self.show_default_index_for_empty:
                     lns = (get_n2a(r, self.default_index),)
                 else:
                     continue
             draw_y = rtopgridln + self.MT.fl_ins
             if mw > 5:
                 draw_y = rtopgridln + self.MT.fl_ins
-                start_ln = int(
-                    (scrollpos_top - rtopgridln) / self.MT.xtra_lines_increment
-                )
+                start_ln = int((scrollpos_top - rtopgridln) / self.MT.xtra_lines_increment)
                 if start_ln < 0:
                     start_ln = 0
                 draw_y += start_ln * self.MT.xtra_lines_increment
-                if (
-                    draw_y + self.MT.half_txt_h - 1 <= rbotgridln
-                    and len(lns) > start_ln
-                ):
+                if draw_y + self.MT.half_txt_h - 1 <= rbotgridln and len(lns) > start_ln:
                     for txt in islice(lns, start_ln, None):
                         config = TextCfg(txt, fill, font, align)
                         k = None
                         if config in self.hidd_text:
                             k = config
                             iid, showing = self.hidd_text[k].pop()
                             cc1, cc2 = self.coords(iid)
@@ -1735,17 +1580,15 @@
                                 1,
                                 4,
                             )
                         if option in (1, 3):
                             self.coords(iid, draw_x, draw_y)
                         if option in (2, 3):
                             if showing:
-                                self.itemconfig(
-                                    iid, text=txt, fill=fill, font=font, anchor=align
-                                )
+                                self.itemconfig(iid, text=txt, fill=fill, font=font, anchor=align)
                             else:
                                 self.itemconfig(
                                     iid,
                                     text=txt,
                                     fill=fill,
                                     font=font,
                                     anchor=align,
@@ -1768,32 +1611,26 @@
                                 txt = txt[len(txt) - int(len(txt) * (mw / wd)) :]
                                 self.itemconfig(iid, text=txt)
                                 wd = self.bbox(iid)
                                 while wd[2] - wd[0] > mw:
                                     txt = txt[1:]
                                     self.itemconfig(iid, text=txt)
                                     wd = self.bbox(iid)
-                            elif align == "center" and (
-                                dropdown_kwargs or checkbox_kwargs
-                            ):
+                            elif align == "center" and (dropdown_kwargs or checkbox_kwargs):
                                 tmod = ceil((len(txt) - int(len(txt) * (mw / wd))) / 2)
                                 txt = txt[tmod - 1 : -tmod]
                                 self.itemconfig(iid, text=txt)
                                 wd = self.bbox(iid)
-                                self.c_align_cyc = cycle(
-                                    self.centre_alignment_text_mod_indexes
-                                )
+                                self.c_align_cyc = cycle(self.centre_alignment_text_mod_indexes)
                                 while wd[2] - wd[0] > mw:
                                     txt = txt[next(self.c_align_cyc)]
                                     self.itemconfig(iid, text=txt)
                                     wd = self.bbox(iid)
                                 self.coords(iid, draw_x, draw_y)
-                            self.disp_text[config._replace(txt=txt)].add(
-                                DrawnItem(iid=iid, showing=True)
-                            )
+                            self.disp_text[config._replace(txt=txt)].add(DrawnItem(iid=iid, showing=True))
                         else:
                             self.disp_text[config].add(DrawnItem(iid=iid, showing=True))
                         draw_y += self.MT.xtra_lines_increment
                         if draw_y + self.MT.half_txt_h - 1 > rbotgridln:
                             break
         for cfg, set_ in self.hidd_text.items():
             for namedtup in tuple(set_):
@@ -1823,44 +1660,30 @@
     def get_redraw_selections(self, startr, endr):
         d = defaultdict(list)
         for item in chain(self.find_withtag("cells"), self.find_withtag("rows")):
             tags = self.gettags(item)
             d[tags[0]].append(tuple(int(e) for e in tags[1].split("_") if e))
         d2 = {}
         if "cells" in d:
-            d2["cells"] = {
-                r
-                for r in range(startr, endr)
-                for r1, c1, r2, c2 in d["cells"]
-                if r1 <= r and r2 > r
-            }
+            d2["cells"] = {r for r in range(startr, endr) for r1, c1, r2, c2 in d["cells"] if r1 <= r and r2 > r}
         if "rows" in d:
-            d2["rows"] = {
-                r
-                for r in range(startr, endr)
-                for r1, c1, r2, c2 in d["rows"]
-                if r1 <= r and r2 > r
-            }
+            d2["rows"] = {r for r in range(startr, endr) for r1, c1, r2, c2 in d["rows"] if r1 <= r and r2 > r}
         return d2
 
     def open_cell(self, event=None, ignore_existing_editor=False):
-        if not self.MT.anything_selected() or (
-            not ignore_existing_editor and self.text_editor_id is not None
-        ):
+        if not self.MT.anything_selected() or (not ignore_existing_editor and self.text_editor_id is not None):
             return
         currently_selected = self.MT.currently_selected()
         if not currently_selected:
             return
         r = int(currently_selected[0])
         datarn = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
         if self.get_cell_kwargs(datarn, key="readonly"):
             return
-        elif self.get_cell_kwargs(datarn, key="dropdown") or self.get_cell_kwargs(
-            datarn, key="checkbox"
-        ):
+        elif self.get_cell_kwargs(datarn, key="dropdown") or self.get_cell_kwargs(datarn, key="checkbox"):
             if self.MT.event_opens_dropdown_or_checkbox(event):
                 if self.get_cell_kwargs(datarn, key="dropdown"):
                     self.open_dropdown_window(r, event=event)
                 elif self.get_cell_kwargs(datarn, key="checkbox"):
                     self.click_checkbox(r, datarn)
         elif self.edit_cell_enabled:
             self.open_text_editor(event=event, r=r, dropdown=False)
@@ -1893,16 +1716,15 @@
                 if hasattr(event, "keysym") and event.keysym == "Return":
                     extra_func_key = "Return"
                 elif hasattr(event, "keysym") and event.keysym == "F2":
                     extra_func_key = "F2"
             datarn = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
             text = self.get_cell_data(datarn, none_to_empty_str=True, redirect_int=True)
         elif event is not None and (
-            (hasattr(event, "keysym") and event.keysym == "BackSpace")
-            or event.keycode in (8, 855638143)
+            (hasattr(event, "keysym") and event.keysym == "BackSpace") or event.keycode in (8, 855638143)
         ):
             extra_func_key = "BackSpace"
             text = ""
         elif event is not None and (
             (hasattr(event, "char") and event.char.isalpha())
             or (hasattr(event, "char") and event.char.isdigit())
             or (hasattr(event, "char") and event.char in symbols_set)
@@ -1910,38 +1732,32 @@
             extra_func_key = event.char
             text = event.char
         else:
             return False
         self.text_editor_loc = r
         if self.extra_begin_edit_cell_func is not None:
             try:
-                text = self.extra_begin_edit_cell_func(
-                    EditIndexEvent(r, extra_func_key, text, "begin_edit_index")
-                )
+                text = self.extra_begin_edit_cell_func(EditIndexEvent(r, extra_func_key, text, "begin_edit_index"))
             except Exception:
                 return False
             if text is None:
                 return False
             else:
                 text = text if isinstance(text, str) else f"{text}"
         text = "" if text is None else text
         if self.MT.cell_auto_resize_enabled:
             self.set_row_height_run_binding(r)
 
         if r == self.text_editor_loc and self.text_editor is not None:
-            self.text_editor.set_text(
-                self.text_editor.get() + "" if not isinstance(text, str) else text
-            )
+            self.text_editor.set_text(self.text_editor.get() + "" if not isinstance(text, str) else text)
             return
         if self.text_editor is not None:
             self.destroy_text_editor()
         if see:
-            has_redrawn = self.MT.see(
-                r=r, c=0, keep_yscroll=True, check_cell_visibility=True
-            )
+            has_redrawn = self.MT.see(r=r, c=0, keep_yscroll=True, check_cell_visibility=True)
             if not has_redrawn:
                 self.MT.refresh()
         self.text_editor_loc = r
         x = 0
         y = self.MT.row_positions[r] + 1
         w = self.current_width + 1
         h = self.MT.row_positions[r + 1] - y
@@ -1967,122 +1783,90 @@
             popup_menu_highlight_fg=self.MT.popup_menu_highlight_fg,
             binding=binding,
             align=self.get_cell_align(r),
             r=r,
             newline_binding=self.text_editor_newline_binding,
         )
         self.text_editor.update_idletasks()
-        self.text_editor_id = self.create_window(
-            (x, y), window=self.text_editor, anchor="nw"
-        )
+        self.text_editor_id = self.create_window((x, y), window=self.text_editor, anchor="nw")
         if not dropdown:
             self.text_editor.textedit.focus_set()
             self.text_editor.scroll_to_bottom()
-        self.text_editor.textedit.bind(
-            "<Alt-Return>", lambda x: self.text_editor_newline_binding(r=r)
-        )
+        self.text_editor.textedit.bind("<Alt-Return>", lambda x: self.text_editor_newline_binding(r=r))
         if USER_OS == "darwin":
-            self.text_editor.textedit.bind(
-                "<Option-Return>", lambda x: self.text_editor_newline_binding(r=r)
-            )
+            self.text_editor.textedit.bind("<Option-Return>", lambda x: self.text_editor_newline_binding(r=r))
         for key, func in self.MT.text_editor_user_bound_keys.items():
             self.text_editor.textedit.bind(key, func)
         if binding is not None:
             self.text_editor.textedit.bind("<Tab>", lambda x: binding((r, "Tab")))
             self.text_editor.textedit.bind("<Return>", lambda x: binding((r, "Return")))
-            self.text_editor.textedit.bind(
-                "<FocusOut>", lambda x: binding((r, "FocusOut"))
-            )
+            self.text_editor.textedit.bind("<FocusOut>", lambda x: binding((r, "FocusOut")))
             self.text_editor.textedit.bind("<Escape>", lambda x: binding((r, "Escape")))
         elif binding is None and set_data_on_close:
-            self.text_editor.textedit.bind(
-                "<Tab>", lambda x: self.close_text_editor((r, "Tab"))
-            )
-            self.text_editor.textedit.bind(
-                "<Return>", lambda x: self.close_text_editor((r, "Return"))
-            )
+            self.text_editor.textedit.bind("<Tab>", lambda x: self.close_text_editor((r, "Tab")))
+            self.text_editor.textedit.bind("<Return>", lambda x: self.close_text_editor((r, "Return")))
             if not dropdown:
-                self.text_editor.textedit.bind(
-                    "<FocusOut>", lambda x: self.close_text_editor((r, "FocusOut"))
-                )
-            self.text_editor.textedit.bind(
-                "<Escape>", lambda x: self.close_text_editor((r, "Escape"))
-            )
+                self.text_editor.textedit.bind("<FocusOut>", lambda x: self.close_text_editor((r, "FocusOut")))
+            self.text_editor.textedit.bind("<Escape>", lambda x: self.close_text_editor((r, "Escape")))
         else:
-            self.text_editor.textedit.bind(
-                "<Escape>", lambda x: self.destroy_text_editor("Escape")
-            )
+            self.text_editor.textedit.bind("<Escape>", lambda x: self.destroy_text_editor("Escape"))
         return True
 
     def text_editor_newline_binding(self, r=0, c=0, event=None, check_lines=True):
         if self.height_resizing_enabled:
             datarn = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
             curr_height = self.text_editor.winfo_height()
             if (
                 not check_lines
-                or self.MT.get_lines_cell_height(
-                    self.text_editor.get_num_lines() + 1, font=self.MT.index_font
-                )
+                or self.MT.get_lines_cell_height(self.text_editor.get_num_lines() + 1, font=self.MT.index_font)
                 > curr_height
             ):
                 new_height = curr_height + self.MT.xtra_lines_increment
                 space_bot = self.MT.get_space_bot(r)
                 if new_height > space_bot:
                     new_height = space_bot
                 if new_height != curr_height:
                     self.set_row_height(datarn, new_height)
                     self.MT.refresh()
                     self.text_editor.config(height=new_height)
                     kwargs = self.get_cell_kwargs(datarn, key="dropdown")
                     if kwargs:
                         text_editor_h = self.text_editor.winfo_height()
-                        win_h, anchor = self.get_dropdown_height_anchor(
-                            datarn, text_editor_h
-                        )
+                        win_h, anchor = self.get_dropdown_height_anchor(datarn, text_editor_h)
                         if anchor == "nw":
                             self.coords(
                                 kwargs["canvas_id"],
                                 self.MT.col_positions[c],
                                 self.MT.row_positions[r] + text_editor_h - 1,
                             )
-                            self.itemconfig(
-                                kwargs["canvas_id"], anchor=anchor, height=win_h
-                            )
+                            self.itemconfig(kwargs["canvas_id"], anchor=anchor, height=win_h)
                         elif anchor == "sw":
                             self.coords(
                                 kwargs["canvas_id"],
                                 self.MT.col_positions[c],
                                 self.MT.row_positions[r],
                             )
-                            self.itemconfig(
-                                kwargs["canvas_id"], anchor=anchor, height=win_h
-                            )
+                            self.itemconfig(kwargs["canvas_id"], anchor=anchor, height=win_h)
 
     def bind_cell_edit(self, enable=True):
         if enable:
             self.edit_cell_enabled = True
         else:
             self.edit_cell_enabled = False
 
     def bind_text_editor_destroy(self, binding, r):
         self.text_editor.textedit.bind("<Return>", lambda x: binding((r, "Return")))
         self.text_editor.textedit.bind("<FocusOut>", lambda x: binding((r, "FocusOut")))
         self.text_editor.textedit.bind("<Escape>", lambda x: binding((r, "Escape")))
         self.text_editor.textedit.focus_set()
 
     def destroy_text_editor(self, event=None):
-        if (
-            event is not None
-            and self.extra_end_edit_cell_func is not None
-            and self.text_editor_loc is not None
-        ):
+        if event is not None and self.extra_end_edit_cell_func is not None and self.text_editor_loc is not None:
             self.extra_end_edit_cell_func(
-                EditHeaderEvent(
-                    int(self.text_editor_loc), "Escape", None, "escape_edit_index"
-                )
+                EditHeaderEvent(int(self.text_editor_loc), "Escape", None, "escape_edit_index")
             )
         self.text_editor_loc = None
         try:
             self.delete(self.text_editor_id)
         except Exception:
             pass
         try:
@@ -2104,33 +1888,27 @@
         destroy=True,
         move_down=True,
         redraw=True,
         recreate=True,
     ):
         if self.focus_get() is None and editor_info:
             return "break"
-        if (
-            editor_info is not None
-            and len(editor_info) >= 2
-            and editor_info[1] == "Escape"
-        ):
+        if editor_info is not None and len(editor_info) >= 2 and editor_info[1] == "Escape":
             self.destroy_text_editor("Escape")
             self.close_dropdown_window(r)
             return "break"
         if self.text_editor is not None:
             self.text_editor_value = self.text_editor.get()
         if destroy:
             self.destroy_text_editor()
         if set_data_on_close:
             if r is None and editor_info is not None and len(editor_info) >= 2:
                 r = editor_info[0]
             datarn = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
-            if self.extra_end_edit_cell_func is None and self.input_valid_for_cell(
-                datarn, self.text_editor_value
-            ):
+            if self.extra_end_edit_cell_func is None and self.input_valid_for_cell(datarn, self.text_editor_value):
                 self.set_cell_data_undo(
                     r,
                     datarn=datarn,
                     value=self.text_editor_value,
                     check_input_valid=False,
                 )
             elif (
@@ -2148,18 +1926,15 @@
                     EditIndexEvent(
                         r,
                         editor_info[1] if len(editor_info) >= 2 else "FocusOut",
                         f"{self.text_editor_value}",
                         "end_edit_index",
                     )
                 )
-            elif (
-                self.extra_end_edit_cell_func is not None
-                and self.MT.edit_cell_validation
-            ):
+            elif self.extra_end_edit_cell_func is not None and self.MT.edit_cell_validation:
                 validation = self.extra_end_edit_cell_func(
                     EditIndexEvent(
                         r,
                         editor_info[1] if len(editor_info) >= 2 else "FocusOut",
                         f"{self.text_editor_value}",
                         "end_edit_index",
                     )
@@ -2176,19 +1951,15 @@
         if move_down:
             pass
         self.close_dropdown_window(r)
         if recreate:
             self.MT.recreate_all_selection_boxes()
         if redraw:
             self.MT.refresh()
-        if (
-            editor_info is not None
-            and len(editor_info) >= 2
-            and editor_info[1] != "FocusOut"
-        ):
+        if editor_info is not None and len(editor_info) >= 2 and editor_info[1] != "FocusOut":
             self.focus_set()
         return "break"
 
     # internal event use
     def set_cell_data_undo(
         self,
         r=0,
@@ -2198,17 +1969,15 @@
         undo=True,
         redraw=True,
         check_input_valid=True,
     ):
         if datarn is None:
             datarn = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
         if isinstance(self.MT._row_index, int):
-            self.MT.set_cell_data_undo(
-                r=r, c=self.MT._row_index, datarn=datarn, value=value, undo=True
-            )
+            self.MT.set_cell_data_undo(r=r, c=self.MT._row_index, datarn=datarn, value=value, undo=True)
         else:
             self.fix_index(datarn)
             if not check_input_valid or self.input_valid_for_cell(datarn, value):
                 if self.MT.undo_enabled and undo:
                     self.MT.undo_storage.append(
                         zlib.compress(
                             pickle.dumps(
@@ -2253,23 +2022,19 @@
     def cell_equal_to(self, datarn, value):
         self.fix_index(datarn)
         if isinstance(self.MT._row_index, list):
             return self.MT._row_index[datarn] == value
         elif isinstance(self.MT._row_index, int):
             return self.MT.cell_equal_to(datarn, self.MT._row_index, value)
 
-    def get_cell_data(
-        self, datarn, get_displayed=False, none_to_empty_str=False, redirect_int=False
-    ):
+    def get_cell_data(self, datarn, get_displayed=False, none_to_empty_str=False, redirect_int=False):
         if get_displayed:
             return self.get_valid_cell_data_as_str(datarn, fix=False)
         if redirect_int and isinstance(self.MT._row_index, int):  # internal use
-            return self.MT.get_cell_data(
-                datarn, self.MT._row_index, none_to_empty_str=True
-            )
+            return self.MT.get_cell_data(datarn, self.MT._row_index, none_to_empty_str=True)
         if (
             isinstance(self.MT._row_index, int)
             or not self.MT._row_index
             or datarn >= len(self.MT._row_index)
             or (self.MT._row_index[datarn] is None and none_to_empty_str)
         ):
             return ""
@@ -2279,84 +2044,65 @@
         kwargs = self.get_cell_kwargs(datarn, key="dropdown")
         if kwargs and kwargs["text"] is not None:
             return f"{kwargs['text']}"
         kwargs = self.get_cell_kwargs(datarn, key="checkbox")
         if kwargs:
             return f"{kwargs['text']}"
         if isinstance(self.MT._row_index, int):
-            return self.MT.get_valid_cell_data_as_str(
-                datarn, self.MT._row_index, get_displayed=True
-            )
+            return self.MT.get_valid_cell_data_as_str(datarn, self.MT._row_index, get_displayed=True)
         if fix:
             self.fix_index(datarn)
         try:
-            return (
-                ""
-                if self.MT._row_index[datarn] is None
-                else f"{self.MT._row_index[datarn]}"
-            )
+            return "" if self.MT._row_index[datarn] is None else f"{self.MT._row_index[datarn]}"
         except Exception:
             return ""
 
     def get_value_for_empty_cell(self, datarn, r_ops=True):
         if self.get_cell_kwargs(datarn, key="checkbox", cell=r_ops):
             return False
         kwargs = self.get_cell_kwargs(datarn, key="dropdown", cell=r_ops)
         if kwargs and kwargs["validate_input"] and kwargs["values"]:
             return kwargs["values"][0]
         return ""
 
     def get_empty_index_seq(self, end, start=0, r_ops=True):
-        return [
-            self.get_value_for_empty_cell(datarn, r_ops=r_ops)
-            for datarn in range(start, end)
-        ]
+        return [self.get_value_for_empty_cell(datarn, r_ops=r_ops) for datarn in range(start, end)]
 
     def fix_index(self, datarn=None, fix_values=tuple()):
         if isinstance(self.MT._row_index, int):
             return
         if isinstance(self.MT._row_index, float):
             self.MT._row_index = int(self.MT._row_index)
             return
         if not isinstance(self.MT._row_index, list):
             try:
                 self.MT._row_index = list(self.MT._row_index)
             except Exception:
                 self.MT._row_index = []
         if isinstance(datarn, int) and datarn >= len(self.MT._row_index):
-            self.MT._row_index.extend(
-                self.get_empty_index_seq(end=datarn + 1, start=len(self.MT._row_index))
-            )
+            self.MT._row_index.extend(self.get_empty_index_seq(end=datarn + 1, start=len(self.MT._row_index)))
         if fix_values:
-            for rn, v in enumerate(
-                islice(self.MT._row_index, fix_values[0], fix_values[1])
-            ):
+            for rn, v in enumerate(islice(self.MT._row_index, fix_values[0], fix_values[1])):
                 if not self.input_valid_for_cell(rn, v):
                     self.MT._row_index[rn] = self.get_value_for_empty_cell(rn)
 
     def set_row_height_run_binding(self, r, only_set_if_too_small=True):
         old_height = self.MT.row_positions[r + 1] - self.MT.row_positions[r]
         new_height = self.set_row_height(r, only_set_if_too_small=only_set_if_too_small)
         if self.row_height_resize_func is not None and old_height != new_height:
-            self.row_height_resize_func(
-                ResizeEvent("row_height_resize", r, old_height, new_height)
-            )
+            self.row_height_resize_func(ResizeEvent("row_height_resize", r, old_height, new_height))
 
     # internal event use
     def click_checkbox(self, r, datarn=None, undo=True, redraw=True):
         if datarn is None:
             datarn = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
         kwargs = self.get_cell_kwargs(datarn, key="checkbox")
         if kwargs["state"] == "normal":
             if isinstance(self.MT._row_index, list):
-                value = (
-                    not self.MT._row_index[datarn]
-                    if type(self.MT._row_index[datarn]) == bool
-                    else False
-                )
+                value = not self.MT._row_index[datarn] if type(self.MT._row_index[datarn]) == bool else False
             elif isinstance(self.MT._row_index, int):
                 value = (
                     not self.MT.data[datarn][self.MT._row_index]
                     if type(self.MT.data[datarn][self.MT._row_index]) == bool
                     else False
                 )
             else:
@@ -2393,62 +2139,50 @@
             self.delete_options_dropdown_and_checkbox()
         if "checkbox" not in self.options:
             self.options["checkbox"] = {}
         self.options["checkbox"] = get_checkbox_dict(**kwargs)
         total_rows = self.MT.total_data_rows()
         if isinstance(self.MT._row_index, int):
             for datarn in range(total_rows):
-                self.MT.set_cell_data(
-                    datarn=datarn, datacn=self.MT._row_index, value=kwargs["checked"]
-                )
+                self.MT.set_cell_data(datarn=datarn, datacn=self.MT._row_index, value=kwargs["checked"])
         else:
             for datarn in range(total_rows):
                 self.set_cell_data(datarn=datarn, value=kwargs["checked"])
 
     def dropdown_index(self, **kwargs):
         self.destroy_opened_dropdown_window()
         if "dropdown" in self.options or "checkbox" in self.options:
             self.delete_options_dropdown_and_checkbox()
         if "dropdown" not in self.options:
             self.options["dropdown"] = {}
         self.options["dropdown"] = get_dropdown_dict(**kwargs)
         total_rows = self.MT.total_data_rows()
         value = (
-            kwargs["set_value"]
-            if kwargs["set_value"] is not None
-            else kwargs["values"][0]
-            if kwargs["values"]
-            else ""
+            kwargs["set_value"] if kwargs["set_value"] is not None else kwargs["values"][0] if kwargs["values"] else ""
         )
         if isinstance(self.MT._row_index, int):
             for datarn in range(total_rows):
-                self.MT.set_cell_data(
-                    datarn=datarn, datacn=self.MT._row_index, value=value
-                )
+                self.MT.set_cell_data(datarn=datarn, datacn=self.MT._row_index, value=value)
         else:
             for datarn in range(total_rows):
-                self.set_cell_data(
-                    datarn=datarn, value=value
-                )
+                self.set_cell_data(datarn=datarn, value=value)
 
     def create_checkbox(self, datarn=0, **kwargs):
         if datarn in self.cell_options and (
-            "dropdown" in self.cell_options[datarn]
-            or "checkbox" in self.cell_options[datarn]
+            "dropdown" in self.cell_options[datarn] or "checkbox" in self.cell_options[datarn]
         ):
             self.delete_cell_options_dropdown_and_checkbox(datarn)
         if datarn not in self.cell_options:
             self.cell_options[datarn] = {}
         self.cell_options[datarn]["checkbox"] = get_checkbox_dict(**kwargs)
         self.set_cell_data(datarn=datarn, value=kwargs["checked"])
 
     def create_dropdown(self, datarn, **kwargs):
         if datarn in self.cell_options and (
-            "dropdown" in self.cell_options[datarn]
-            or "checkbox" in self.cell_options[datarn]
+            "dropdown" in self.cell_options[datarn] or "checkbox" in self.cell_options[datarn]
         ):
             self.delete_cell_options_dropdown_and_checkbox(datarn)
         if datarn not in self.cell_options:
             self.cell_options[datarn] = {}
         self.cell_options[datarn]["dropdown"] = get_dropdown_dict(**kwargs)
         self.set_cell_data(
             datarn=datarn,
@@ -2458,21 +2192,17 @@
             if kwargs["values"]
             else "",
         )
 
     def get_dropdown_height_anchor(self, datarn, text_editor_h=None):
         win_h = 5
         for i, v in enumerate(self.get_cell_kwargs(datarn, key="dropdown")["values"]):
-            v_numlines = len(
-                v.split("\n") if isinstance(v, str) else f"{v}".split("\n")
-            )
+            v_numlines = len(v.split("\n") if isinstance(v, str) else f"{v}".split("\n"))
             if v_numlines > 1:
-                win_h += (
-                    self.MT.fl_ins + (v_numlines * self.MT.xtra_lines_increment) + 5
-                )  # end of cell
+                win_h += self.MT.fl_ins + (v_numlines * self.MT.xtra_lines_increment) + 5  # end of cell
             else:
                 win_h += self.MT.min_row_height
             if i == 5:
                 break
         if win_h > 500:
             win_h = 500
         space_bot = self.MT.get_space_bot(0, text_editor_h)
@@ -2515,24 +2245,20 @@
             search_function=kwargs["search_function"],
             arrowkey_RIGHT=self.MT.arrowkey_RIGHT,
             arrowkey_LEFT=self.MT.arrowkey_LEFT,
             align="w",
             single_index="r",
         )
         ypos = self.MT.row_positions[r + 1]
-        kwargs["canvas_id"] = self.create_window(
-            (0, ypos), window=window, anchor=anchor
-        )
+        kwargs["canvas_id"] = self.create_window((0, ypos), window=window, anchor=anchor)
         if kwargs["state"] == "normal":
             self.text_editor.textedit.bind(
                 "<<TextModified>>",
                 lambda x: window.search_and_see(
-                    DropDownModifiedEvent(
-                        "IndexComboboxModified", r, 0, self.text_editor.get()
-                    )
+                    DropDownModifiedEvent("IndexComboboxModified", r, 0, self.text_editor.get())
                 ),
             )
             if kwargs["modified_function"] is not None:
                 window.modified_function = kwargs["modified_function"]
             self.update_idletasks()
             try:
                 self.after(1, lambda: self.text_editor.textedit.focus())
@@ -2545,60 +2271,36 @@
             self.update_idletasks()
             window.focus_set()
             redraw = True
         self.existing_dropdown_window = window
         kwargs["window"] = window
         self.existing_dropdown_canvas_id = kwargs["canvas_id"]
         if redraw:
-            self.MT.main_table_redraw_grid_and_text(
-                redraw_header=False, redraw_row_index=True, redraw_table=False
-            )
+            self.MT.main_table_redraw_grid_and_text(redraw_header=False, redraw_row_index=True, redraw_table=False)
 
     # r is displayed row
     def close_dropdown_window(self, r=None, selection=None, redraw=True):
         if r is not None and selection is not None:
             datarn = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
             kwargs = self.get_cell_kwargs(datarn, key="dropdown")
-            if (
-                kwargs["select_function"] is not None
-            ):  # user has specified a selection function
-                kwargs["select_function"](
-                    EditIndexEvent(
-                        r, "IndexComboboxSelected", f"{selection}", "end_edit_index"
-                    )
-                )
+            if kwargs["select_function"] is not None:  # user has specified a selection function
+                kwargs["select_function"](EditIndexEvent(r, "IndexComboboxSelected", f"{selection}", "end_edit_index"))
             if self.extra_end_edit_cell_func is None:
-                self.set_cell_data_undo(
-                    r, datarn=datarn, value=selection, redraw=not redraw
-                )
-            elif (
-                self.extra_end_edit_cell_func is not None
-                and self.MT.edit_cell_validation
-            ):
+                self.set_cell_data_undo(r, datarn=datarn, value=selection, redraw=not redraw)
+            elif self.extra_end_edit_cell_func is not None and self.MT.edit_cell_validation:
                 validation = self.extra_end_edit_cell_func(
-                    EditIndexEvent(
-                        r, "IndexComboboxSelected", f"{selection}", "end_edit_index"
-                    )
+                    EditIndexEvent(r, "IndexComboboxSelected", f"{selection}", "end_edit_index")
                 )
                 if validation is not None:
                     selection = validation
-                self.set_cell_data_undo(
-                    r, datarn=datarn, value=selection, redraw=not redraw
-                )
-            elif (
-                self.extra_end_edit_cell_func is not None
-                and not self.MT.edit_cell_validation
-            ):
-                self.set_cell_data_undo(
-                    r, datarn=datarn, value=selection, redraw=not redraw
-                )
+                self.set_cell_data_undo(r, datarn=datarn, value=selection, redraw=not redraw)
+            elif self.extra_end_edit_cell_func is not None and not self.MT.edit_cell_validation:
+                self.set_cell_data_undo(r, datarn=datarn, value=selection, redraw=not redraw)
                 self.extra_end_edit_cell_func(
-                    EditIndexEvent(
-                        r, "IndexComboboxSelected", f"{selection}", "end_edit_index"
-                    )
+                    EditIndexEvent(r, "IndexComboboxSelected", f"{selection}", "end_edit_index")
                 )
             self.focus_set()
             self.MT.recreate_all_selection_boxes()
         self.destroy_text_editor("Escape")
         self.destroy_opened_dropdown_window(r)
         if redraw:
             self.MT.refresh()
```

### Comparing `tksheet-6.1.3/tksheet/_tksheet_top_left_rectangle.py` & `tksheet-6.1.4/tksheet/_tksheet_top_left_rectangle.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import tkinter as tk
 
-from ._tksheet_other_classes import *
-from ._tksheet_vars import *
+from ._tksheet_vars import (
+    rc_binding,
+)
 
 
 class TopLeftRectangle(tk.Canvas):
     def __init__(self, *args, **kwargs):
         tk.Canvas.__init__(
             self,
             kwargs["parentframe"],
@@ -132,17 +133,15 @@
                 self.MT.deselect("all")
         elif rect[0] == 1:
             if self.RI.width_resizing_enabled:
                 self.RI.set_width(self.MT.default_index_width, set_TL=True)
         elif rect[0] == 2:
             if self.CH.height_resizing_enabled:
                 self.CH.set_height(self.MT.default_header_height[1], set_TL=True)
-        self.MT.main_table_redraw_grid_and_text(
-            redraw_header=True, redraw_row_index=True
-        )
+        self.MT.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=True)
         if self.extra_b1_press_func is not None:
             self.extra_b1_press_func(event)
 
     def b1_motion(self, event=None):
         self.focus_set()
         if self.extra_b1_motion_func is not None:
             self.extra_b1_motion_func(event)
```

### Comparing `tksheet-6.1.3/tksheet/_tksheet_vars.py` & `tksheet-6.1.4/tksheet/_tksheet_vars.py`

 * *Files identical despite different names*

### Comparing `tksheet-6.1.3/tksheet.egg-info/PKG-INFO` & `tksheet-6.1.4/tksheet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tksheet
-Version: 6.1.3
+Version: 6.1.4
 Summary: Tkinter table / sheet widget
 Home-page: https://github.com/ragardner/tksheet
-Download-URL: https://github.com/ragardner/tksheet/archive/6.1.3.tar.gz
+Download-URL: https://github.com/ragardner/tksheet/archive/6.1.4.tar.gz
 Author: ragardner
 Author-email: github@ragardner.simplelogin.com
 License: MIT
 Keywords: tkinter,table,widget,sheet,grid,tk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

