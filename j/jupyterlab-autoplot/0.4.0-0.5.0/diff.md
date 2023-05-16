# Comparing `tmp/jupyterlab-autoplot-0.4.0.tar.gz` & `tmp/jupyterlab-autoplot-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterlab-autoplot-0.4.0.tar", last modified: Tue May  9 19:51:26 2023, max compression
+gzip compressed data, was "jupyterlab-autoplot-0.5.0.tar", last modified: Tue May 16 17:10:16 2023, max compression
```

## Comparing `jupyterlab-autoplot-0.4.0.tar` & `jupyterlab-autoplot-0.5.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 19:51:26.570782 jupyterlab-autoplot-0.4.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       44 2023-05-09 19:49:45.000000 jupyterlab-autoplot-0.4.0/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5136 2023-05-09 19:51:26.570782 jupyterlab-autoplot-0.4.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4596 2023-05-09 19:49:45.000000 jupyterlab-autoplot-0.4.0/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 19:51:26.566782 jupyterlab-autoplot-0.4.0/autoplot/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8823 2023-05-09 19:49:45.000000 jupyterlab-autoplot-0.4.0/autoplot/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 19:51:26.566782 jupyterlab-autoplot-0.4.0/autoplot/dtaler/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9125 2023-05-09 19:49:45.000000 jupyterlab-autoplot-0.4.0/autoplot/dtaler/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 19:51:26.566782 jupyterlab-autoplot-0.4.0/autoplot/extensions/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       77 2023-05-09 19:49:45.000000 jupyterlab-autoplot-0.4.0/autoplot/extensions/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1272 2023-05-09 19:49:45.000000 jupyterlab-autoplot-0.4.0/autoplot/extensions/autoplot_display.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4934 2023-05-09 19:49:45.000000 jupyterlab-autoplot-0.4.0/autoplot/extensions/toast.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 19:51:26.566782 jupyterlab-autoplot-0.4.0/autoplot/plotter/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    26256 2023-05-09 19:49:45.000000 jupyterlab-autoplot-0.4.0/autoplot/plotter/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2612 2023-05-09 19:49:45.000000 jupyterlab-autoplot-0.4.0/autoplot/plotter/range_selector_utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9665 2023-05-09 19:49:45.000000 jupyterlab-autoplot-0.4.0/autoplot/plotter/trace.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 19:51:26.566782 jupyterlab-autoplot-0.4.0/autoplot/plugins/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      836 2023-05-09 19:49:45.000000 jupyterlab-autoplot-0.4.0/autoplot/plugins/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 19:51:26.566782 jupyterlab-autoplot-0.4.0/autoplot/plugins/bundles/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5860 2023-05-09 19:51:09.000000 jupyterlab-autoplot-0.4.0/autoplot/plugins/bundles/interactiveLegend.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5885 2023-05-09 19:51:09.000000 jupyterlab-autoplot-0.4.0/autoplot/plugins/bundles/rangeSelectorButtons.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7707 2023-05-09 19:51:09.000000 jupyterlab-autoplot-0.4.0/autoplot/plugins/bundles/saveImageButtons.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11503 2023-05-09 19:51:09.000000 jupyterlab-autoplot-0.4.0/autoplot/plugins/bundles/timeSeriesTooltip.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2913 2023-05-09 19:49:45.000000 jupyterlab-autoplot-0.4.0/autoplot/plugins/interactive_legend.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1009 2023-05-09 19:49:45.000000 jupyterlab-autoplot-0.4.0/autoplot/plugins/line_utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3932 2023-05-09 19:49:45.000000 jupyterlab-autoplot-0.4.0/autoplot/plugins/range_selector_buttons.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1819 2023-05-09 19:49:45.000000 jupyterlab-autoplot-0.4.0/autoplot/plugins/save_image_buttons.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2238 2023-05-09 19:49:45.000000 jupyterlab-autoplot-0.4.0/autoplot/plugins/time_series_tooltip.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 19:51:26.566782 jupyterlab-autoplot-0.4.0/autoplot/utils/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      231 2023-05-09 19:49:45.000000 jupyterlab-autoplot-0.4.0/autoplot/utils/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      878 2023-05-09 19:49:45.000000 jupyterlab-autoplot-0.4.0/autoplot/utils/constants.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 19:51:26.570782 jupyterlab-autoplot-0.4.0/autoplot/view_manager/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12387 2023-05-09 19:49:45.000000 jupyterlab-autoplot-0.4.0/autoplot/view_manager/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1325 2023-05-09 19:49:45.000000 jupyterlab-autoplot-0.4.0/autoplot/view_manager/variable_utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 19:51:26.570782 jupyterlab-autoplot-0.4.0/jupyterlab_autoplot.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5136 2023-05-09 19:51:26.000000 jupyterlab-autoplot-0.4.0/jupyterlab_autoplot.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1041 2023-05-09 19:51:26.000000 jupyterlab-autoplot-0.4.0/jupyterlab_autoplot.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-09 19:51:26.000000 jupyterlab-autoplot-0.4.0/jupyterlab_autoplot.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       63 2023-05-09 19:51:26.000000 jupyterlab-autoplot-0.4.0/jupyterlab_autoplot.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        9 2023-05-09 19:51:26.000000 jupyterlab-autoplot-0.4.0/jupyterlab_autoplot.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       76 2023-05-09 19:49:45.000000 jupyterlab-autoplot-0.4.0/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-05-09 19:51:26.570782 jupyterlab-autoplot-0.4.0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1114 2023-05-09 19:49:45.000000 jupyterlab-autoplot-0.4.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-16 17:10:16.250717 jupyterlab-autoplot-0.5.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       44 2023-05-16 17:08:26.000000 jupyterlab-autoplot-0.5.0/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5136 2023-05-16 17:10:16.250717 jupyterlab-autoplot-0.5.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4596 2023-05-16 17:08:26.000000 jupyterlab-autoplot-0.5.0/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-16 17:10:16.246717 jupyterlab-autoplot-0.5.0/autoplot/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8823 2023-05-16 17:08:26.000000 jupyterlab-autoplot-0.5.0/autoplot/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-16 17:10:16.246717 jupyterlab-autoplot-0.5.0/autoplot/dtaler/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8898 2023-05-16 17:08:26.000000 jupyterlab-autoplot-0.5.0/autoplot/dtaler/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-16 17:10:16.246717 jupyterlab-autoplot-0.5.0/autoplot/extensions/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       77 2023-05-16 17:08:26.000000 jupyterlab-autoplot-0.5.0/autoplot/extensions/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1272 2023-05-16 17:08:26.000000 jupyterlab-autoplot-0.5.0/autoplot/extensions/autoplot_display.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4934 2023-05-16 17:08:26.000000 jupyterlab-autoplot-0.5.0/autoplot/extensions/toast.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-16 17:10:16.246717 jupyterlab-autoplot-0.5.0/autoplot/plotter/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    26256 2023-05-16 17:08:26.000000 jupyterlab-autoplot-0.5.0/autoplot/plotter/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2612 2023-05-16 17:08:26.000000 jupyterlab-autoplot-0.5.0/autoplot/plotter/range_selector_utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9665 2023-05-16 17:08:26.000000 jupyterlab-autoplot-0.5.0/autoplot/plotter/trace.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-16 17:10:16.246717 jupyterlab-autoplot-0.5.0/autoplot/plugins/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      836 2023-05-16 17:08:26.000000 jupyterlab-autoplot-0.5.0/autoplot/plugins/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-16 17:10:16.246717 jupyterlab-autoplot-0.5.0/autoplot/plugins/bundles/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5860 2023-05-16 17:09:57.000000 jupyterlab-autoplot-0.5.0/autoplot/plugins/bundles/interactiveLegend.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5885 2023-05-16 17:09:57.000000 jupyterlab-autoplot-0.5.0/autoplot/plugins/bundles/rangeSelectorButtons.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7707 2023-05-16 17:09:57.000000 jupyterlab-autoplot-0.5.0/autoplot/plugins/bundles/saveImageButtons.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11503 2023-05-16 17:09:57.000000 jupyterlab-autoplot-0.5.0/autoplot/plugins/bundles/timeSeriesTooltip.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2913 2023-05-16 17:08:26.000000 jupyterlab-autoplot-0.5.0/autoplot/plugins/interactive_legend.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1009 2023-05-16 17:08:26.000000 jupyterlab-autoplot-0.5.0/autoplot/plugins/line_utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3932 2023-05-16 17:08:26.000000 jupyterlab-autoplot-0.5.0/autoplot/plugins/range_selector_buttons.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1819 2023-05-16 17:08:26.000000 jupyterlab-autoplot-0.5.0/autoplot/plugins/save_image_buttons.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2238 2023-05-16 17:08:26.000000 jupyterlab-autoplot-0.5.0/autoplot/plugins/time_series_tooltip.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-16 17:10:16.246717 jupyterlab-autoplot-0.5.0/autoplot/utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      231 2023-05-16 17:08:26.000000 jupyterlab-autoplot-0.5.0/autoplot/utils/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      878 2023-05-16 17:08:26.000000 jupyterlab-autoplot-0.5.0/autoplot/utils/constants.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-16 17:10:16.246717 jupyterlab-autoplot-0.5.0/autoplot/view_manager/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12387 2023-05-16 17:08:26.000000 jupyterlab-autoplot-0.5.0/autoplot/view_manager/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1325 2023-05-16 17:08:26.000000 jupyterlab-autoplot-0.5.0/autoplot/view_manager/variable_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-16 17:10:16.250717 jupyterlab-autoplot-0.5.0/jupyterlab_autoplot.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5136 2023-05-16 17:10:16.000000 jupyterlab-autoplot-0.5.0/jupyterlab_autoplot.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1041 2023-05-16 17:10:16.000000 jupyterlab-autoplot-0.5.0/jupyterlab_autoplot.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-16 17:10:16.000000 jupyterlab-autoplot-0.5.0/jupyterlab_autoplot.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       63 2023-05-16 17:10:16.000000 jupyterlab-autoplot-0.5.0/jupyterlab_autoplot.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        9 2023-05-16 17:10:16.000000 jupyterlab-autoplot-0.5.0/jupyterlab_autoplot.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       76 2023-05-16 17:08:26.000000 jupyterlab-autoplot-0.5.0/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-05-16 17:10:16.250717 jupyterlab-autoplot-0.5.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1114 2023-05-16 17:08:26.000000 jupyterlab-autoplot-0.5.0/setup.py
```

### Comparing `jupyterlab-autoplot-0.4.0/PKG-INFO` & `jupyterlab-autoplot-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab-autoplot
-Version: 0.4.0
+Version: 0.5.0
 Summary: The IPython component for the Autoplot JupyterLab extension.
 Home-page: https://github.com/man-group/jupyterlab-autoplot
 Author: Man Alpha Technology
 Author-email: ManAlphaTech@man.com
 License: BSD 3-Clause
 Keywords: jupyter,jupyterlab,matplotlib,mpld3,time series
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jupyterlab-autoplot-0.4.0/README.md` & `jupyterlab-autoplot-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab-autoplot-0.4.0/autoplot/__init__.py` & `jupyterlab-autoplot-0.5.0/autoplot/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab-autoplot-0.4.0/autoplot/dtaler/__init__.py` & `jupyterlab-autoplot-0.5.0/autoplot/dtaler/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,15 +101,15 @@
         # 5. Update tracked variables which have changed
         updated_variables = _filter_updated(pandas_vars.items(), self._tracked.copy())
         for name, var in updated_variables.items():
             self._update_tracked_var(name, var)
 
     def draw(self, force: bool, output: AutoplotDisplay) -> None:
         refresh = False
-        current = dtale.get_instance(int(output.data_id))
+        current = dtale.get_instance(output.data_id)
         if current is None:
             current = Image(data=resource_filename(__name__, "assets/imgs/dtale.png"))
         # The conditionals below encode precedence. Whatever the user wants to show takes is the preferred value to
         # display, followed by new values and so on.
         if set(self._force_show) & set(self._tracked.keys()):
             for key in reversed(self._force_show):
                 if key in self._tracked:
@@ -169,37 +169,32 @@
         return result
 
     def _remove_tracked_var(self, var_name: str):
         vardata = self._tracked.pop(var_name, None)
         if vardata:
             data_id = vardata.dd._data_id
             dtale.global_state.cleanup(data_id)
-            try:
-                # this will be fixed in newer version of D-Tale
-                del dtale.global_state._default_store._data_names[var_name]
-            except KeyError:
-                pass
-            self._deleted.append(str(vardata.dd._data_id))
+            self._deleted.append(vardata.dd._data_id)
 
     def _add_tracked_var(self, name, var):
         dd = self._dtale_show(data=var, ignore_duplicate=True, reaper_on=False, name=name, hide_shutdown=True)
         self._tracked[name] = VarData(pdf=var, dd=dd)
         self._new.append(name)
 
     def _update_tracked_var(self, name, var):
         vardata = self._tracked[name]
         vardata.dd.data = var
         self._tracked[name] = VarData(pdf=var, dd=vardata.dd)
-        self._updated.append(str(vardata.dd._data_id))
+        self._updated.append(vardata.dd._data_id)
 
 
 def _removed_in_dtale(tracked: Iterable) -> Set[str]:
     removed: Set[str] = set()
     for name, vardata in tracked:
-        if dtale.get_instance(int(vardata.dd._data_id)) is None:
+        if dtale.get_instance(vardata.dd._data_id) is None:
             removed.add(name)
     return removed
 
 
 def _filter_updated(pandas_vars: Iterable, tracked: Dict[str, VarData]) -> Dict[str, Union[pd.Series, pd.DataFrame]]:
     result: Dict[str, Union[pd.Series, pd.DataFrame]] = {}
```

### Comparing `jupyterlab-autoplot-0.4.0/autoplot/extensions/autoplot_display.py` & `jupyterlab-autoplot-0.5.0/autoplot/extensions/autoplot_display.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import uuid
 
 from ipywidgets import Output
 from traitlets import Unicode
 
 # these values must mach those in autoplot-display/version.ts
 EXTENSION_TITLE = "Autoplot Display"
-EXTENSION_VERSION = "0.4.0"
+EXTENSION_VERSION = "0.5.0"
 MODULE_NAME = "@jupyter-widgets/autoplot-display"
 
 MODEL_NAME = "AutoplotDisplayModel"
 VIEW_NAME = "AutoplotDisplayView"
 
 
 class AutoplotDisplay(Output):
```

### Comparing `jupyterlab-autoplot-0.4.0/autoplot/extensions/toast.py` & `jupyterlab-autoplot-0.5.0/autoplot/extensions/toast.py`

 * *Files identical despite different names*

### Comparing `jupyterlab-autoplot-0.4.0/autoplot/plotter/__init__.py` & `jupyterlab-autoplot-0.5.0/autoplot/plotter/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab-autoplot-0.4.0/autoplot/plotter/range_selector_utils.py` & `jupyterlab-autoplot-0.5.0/autoplot/plotter/range_selector_utils.py`

 * *Files identical despite different names*

### Comparing `jupyterlab-autoplot-0.4.0/autoplot/plotter/trace.py` & `jupyterlab-autoplot-0.5.0/autoplot/plotter/trace.py`

 * *Files identical despite different names*

### Comparing `jupyterlab-autoplot-0.4.0/autoplot/plugins/__init__.py` & `jupyterlab-autoplot-0.5.0/autoplot/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab-autoplot-0.4.0/autoplot/plugins/bundles/interactiveLegend.js` & `jupyterlab-autoplot-0.5.0/autoplot/plugins/bundles/interactiveLegend.js`

 * *Files identical despite different names*

### Comparing `jupyterlab-autoplot-0.4.0/autoplot/plugins/bundles/rangeSelectorButtons.js` & `jupyterlab-autoplot-0.5.0/autoplot/plugins/bundles/rangeSelectorButtons.js`

 * *Files identical despite different names*

### Comparing `jupyterlab-autoplot-0.4.0/autoplot/plugins/bundles/saveImageButtons.js` & `jupyterlab-autoplot-0.5.0/autoplot/plugins/bundles/saveImageButtons.js`

 * *Files identical despite different names*

### Comparing `jupyterlab-autoplot-0.4.0/autoplot/plugins/bundles/timeSeriesTooltip.js` & `jupyterlab-autoplot-0.5.0/autoplot/plugins/bundles/timeSeriesTooltip.js`

 * *Files identical despite different names*

### Comparing `jupyterlab-autoplot-0.4.0/autoplot/plugins/interactive_legend.py` & `jupyterlab-autoplot-0.5.0/autoplot/plugins/interactive_legend.py`

 * *Files identical despite different names*

### Comparing `jupyterlab-autoplot-0.4.0/autoplot/plugins/line_utils.py` & `jupyterlab-autoplot-0.5.0/autoplot/plugins/line_utils.py`

 * *Files identical despite different names*

### Comparing `jupyterlab-autoplot-0.4.0/autoplot/plugins/range_selector_buttons.py` & `jupyterlab-autoplot-0.5.0/autoplot/plugins/range_selector_buttons.py`

 * *Files identical despite different names*

### Comparing `jupyterlab-autoplot-0.4.0/autoplot/plugins/save_image_buttons.py` & `jupyterlab-autoplot-0.5.0/autoplot/plugins/save_image_buttons.py`

 * *Files identical despite different names*

### Comparing `jupyterlab-autoplot-0.4.0/autoplot/plugins/time_series_tooltip.py` & `jupyterlab-autoplot-0.5.0/autoplot/plugins/time_series_tooltip.py`

 * *Files identical despite different names*

### Comparing `jupyterlab-autoplot-0.4.0/autoplot/utils/constants.py` & `jupyterlab-autoplot-0.5.0/autoplot/utils/constants.py`

 * *Files identical despite different names*

### Comparing `jupyterlab-autoplot-0.4.0/autoplot/view_manager/__init__.py` & `jupyterlab-autoplot-0.5.0/autoplot/view_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab-autoplot-0.4.0/autoplot/view_manager/variable_utils.py` & `jupyterlab-autoplot-0.5.0/autoplot/view_manager/variable_utils.py`

 * *Files identical despite different names*

### Comparing `jupyterlab-autoplot-0.4.0/jupyterlab_autoplot.egg-info/PKG-INFO` & `jupyterlab-autoplot-0.5.0/jupyterlab_autoplot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab-autoplot
-Version: 0.4.0
+Version: 0.5.0
 Summary: The IPython component for the Autoplot JupyterLab extension.
 Home-page: https://github.com/man-group/jupyterlab-autoplot
 Author: Man Alpha Technology
 Author-email: ManAlphaTech@man.com
 License: BSD 3-Clause
 Keywords: jupyter,jupyterlab,matplotlib,mpld3,time series
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jupyterlab-autoplot-0.4.0/jupyterlab_autoplot.egg-info/SOURCES.txt` & `jupyterlab-autoplot-0.5.0/jupyterlab_autoplot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab-autoplot-0.4.0/setup.py` & `jupyterlab-autoplot-0.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,25 +5,25 @@
     with open("README.md", "r", encoding="utf-8") as f:
         desc = f.read()
     return desc
 
 
 setup(
     name="jupyterlab-autoplot",
-    version="0.4.0",
+    version="0.5.0",
     author="Man Alpha Technology",
     author_email="ManAlphaTech@man.com",
     license="BSD 3-Clause",
     description="The IPython component for the Autoplot JupyterLab extension.",
     long_description=get_long_description(),
     url="https://github.com/man-group/jupyterlab-autoplot",
     keywords=["jupyter", "jupyterlab", "matplotlib", "mpld3", "time series"],
     packages=find_packages(include=["autoplot", "autoplot.*"], exclude=["tests", "tests.*"]),
     include_package_data=True,
-    install_requires=["ipywidgets", "ipython", "numpy", "pandas", "matplotlib", "mpld3", "dtale>=2.15.2"],
+    install_requires=["ipywidgets", "ipython", "numpy", "pandas", "matplotlib", "mpld3", "dtale>=2.16.0"],
     tests_require=["pytest", "pytest-cov", "mock"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
         "Framework :: Jupyter",
     ],
```

