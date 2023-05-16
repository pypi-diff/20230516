# Comparing `tmp/ipyautoui-0.5.2.tar.gz` & `tmp/ipyautoui-0.5.3.tar.gz`

## Comparing `ipyautoui-0.5.2.tar` & `ipyautoui-0.5.3.tar`

### file list

```diff
@@ -1,58 +1,59 @@
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/__init__.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/_dev_sys_path_append.py
--rw-r--r--   0        0        0    13120 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/_utils.py
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/_utils_debounce.py
--rw-r--r--   0        0        0    18450 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/_version.py
--rw-r--r--   0        0        0    31684 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/autodisplay.py
--rw-r--r--   0        0        0    14138 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/autodisplay_renderers.py
--rw-r--r--   0        0        0    28946 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/autoipywidget.py
--rw-r--r--   0        0        0    21441 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/automapschema.py
--rw-r--r--   0        0        0    12894 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/autoui.py
--rw-r--r--   0        0        0     4281 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/autovjsf.py
--rw-r--r--   0        0        0    14967 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/autowidgets.py
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/basemodel.py
--rw-r--r--   0        0        0     5955 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/constants.py
--rw-r--r--   0        0        0     5940 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/demo.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/env.py
--rw-r--r--   0        0        0     4693 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/mydocstring_display.py
--rw-r--r--   0        0        0     7425 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/test_schema.py
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/vjsf.vue
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/custom/__init__.py
--rw-r--r--   0        0        0    40881 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/custom/autogrid.py
--rw-r--r--   0        0        0    12640 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/custom/buttonbars.py
--rw-r--r--   0        0        0     3177 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/custom/decision_branch.py
--rw-r--r--   0        0        0    25164 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/custom/editgrid.py
--rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/custom/filechooser.py
--rw-r--r--   0        0        0     9395 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/custom/filesindir.py
--rw-r--r--   0        0        0     6680 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/custom/fileupload.py
--rw-r--r--   0        0        0    30632 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/custom/iterable.py
--rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/custom/loadproject.py
--rw-r--r--   0        0        0     5479 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/custom/markdown_widget.py
--rw-r--r--   0        0        0     5648 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/custom/modelrun.py
--rw-r--r--   0        0        0     5555 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/custom/multiselect_search.py
--rw-r--r--   0        0        0     7584 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/custom/outputlogging.py
--rw-r--r--   0        0        0     8598 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/custom/selectdir.py
--rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/custom/showhide.py
--rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/custom/showopenurl.py
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/custom/title_description.py
--rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/custom/urlimagelink.py
--rw-r--r--   0        0        0     5841 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/custom/widgetcaller_error.py
--rw-r--r--   0        0        0    12975 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/custom/workingdir.py
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/demo_schemas/__init__.py
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/demo_schemas/complex_serialization.py
--rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/demo_schemas/core_ipywidgets.py
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/demo_schemas/editable_datagrid.py
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/demo_schemas/nested.py
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/demo_schemas/nested_editable_datagrid.py
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/demo_schemas/nullable_core_ipywidgets.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/demo_schemas/override_ipywidgets.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/demo_schemas/root_array.py
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/demo_schemas/root_array_enum.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/demo_schemas/root_enum.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/demo_schemas/root_simple.py
--rw-r--r--   0        0        0     6752 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/demo_schemas/ruleset.py
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/.gitignore
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/LICENSE
--rw-r--r--   0        0        0     7477 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/README.md
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     8582 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/__init__.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/_dev_sys_path_append.py
+-rw-r--r--   0        0        0    13120 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/_utils.py
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/_utils_debounce.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/_version.py
+-rw-r--r--   0        0        0    31739 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/autodisplay.py
+-rw-r--r--   0        0        0    14138 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/autodisplay_renderers.py
+-rw-r--r--   0        0        0    28946 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/autoipywidget.py
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/automapschema-0.yaml
+-rw-r--r--   0        0        0    21750 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/automapschema.py
+-rw-r--r--   0        0        0    12894 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/autoui.py
+-rw-r--r--   0        0        0     4281 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/autovjsf.py
+-rw-r--r--   0        0        0    14967 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/autowidgets.py
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/basemodel.py
+-rw-r--r--   0        0        0     5996 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/constants.py
+-rw-r--r--   0        0        0     5940 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/demo.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/env.py
+-rw-r--r--   0        0        0     4693 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/mydocstring_display.py
+-rw-r--r--   0        0        0     7425 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/test_schema.py
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/vjsf.vue
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/custom/__init__.py
+-rw-r--r--   0        0        0    40894 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/custom/autogrid.py
+-rw-r--r--   0        0        0    12640 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/custom/buttonbars.py
+-rw-r--r--   0        0        0     3177 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/custom/decision_branch.py
+-rw-r--r--   0        0        0    25263 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/custom/editgrid.py
+-rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/custom/filechooser.py
+-rw-r--r--   0        0        0     9395 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/custom/filesindir.py
+-rw-r--r--   0        0        0     6680 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/custom/fileupload.py
+-rw-r--r--   0        0        0    30632 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/custom/iterable.py
+-rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/custom/loadproject.py
+-rw-r--r--   0        0        0     5479 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/custom/markdown_widget.py
+-rw-r--r--   0        0        0     5648 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/custom/modelrun.py
+-rw-r--r--   0        0        0     5555 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/custom/multiselect_search.py
+-rw-r--r--   0        0        0     7584 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/custom/outputlogging.py
+-rw-r--r--   0        0        0     8598 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/custom/selectdir.py
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/custom/showhide.py
+-rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/custom/showopenurl.py
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/custom/title_description.py
+-rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/custom/urlimagelink.py
+-rw-r--r--   0        0        0     5867 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/custom/widgetcaller_error.py
+-rw-r--r--   0        0        0    12975 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/custom/workingdir.py
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/demo_schemas/__init__.py
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/demo_schemas/complex_serialization.py
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/demo_schemas/core_ipywidgets.py
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/demo_schemas/editable_datagrid.py
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/demo_schemas/nested.py
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/demo_schemas/nested_editable_datagrid.py
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/demo_schemas/nullable_core_ipywidgets.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/demo_schemas/override_ipywidgets.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/demo_schemas/root_array.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/demo_schemas/root_array_enum.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/demo_schemas/root_enum.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/demo_schemas/root_simple.py
+-rw-r--r--   0        0        0     6752 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/demo_schemas/ruleset.py
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/.gitignore
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/LICENSE
+-rw-r--r--   0        0        0     7477 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/README.md
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     8582 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/PKG-INFO
```

### Comparing `ipyautoui-0.5.2/src/ipyautoui/__init__.py` & `ipyautoui-0.5.3/src/ipyautoui/__init__.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.2/src/ipyautoui/_dev_sys_path_append.py` & `ipyautoui-0.5.3/src/ipyautoui/_dev_sys_path_append.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.2/src/ipyautoui/_utils.py` & `ipyautoui-0.5.3/src/ipyautoui/_utils.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.2/src/ipyautoui/_utils_debounce.py` & `ipyautoui-0.5.3/src/ipyautoui/_utils_debounce.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.2/src/ipyautoui/autodisplay.py` & `ipyautoui-0.5.3/src/ipyautoui/autodisplay.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,17 +84,19 @@
 #     from xlsxtemplater import from_excel
 # except:
 #     pass
 
 
 # %%
 def merge_default_renderers(
-    renderers: dict[str, ty.Callable],
+    renderers: ty.Optional[dict[str, ty.Callable]],
     default_renderers: frozenmap[str, ty.Callable] = DEFAULT_FILE_RENDERERS,
 ) -> dict[str, ty.Callable]:
+    if renderers is None:
+        renderers = {}
     return {**dict(default_renderers), **renderers}
 
 
 # %%
 def get_renderers(
     renderers: ty.Optional[dict[str, ty.Callable]],
     extend_default_renderers: bool = True,
@@ -205,18 +207,16 @@
             return lambda: "Error: path given is None"
 
     class Config:
         arbitrary_types_allowed = True
 
 
 def url_ok(url):
-
     # exception block
     try:
-
         # pass the url into
         # request.head
         # response = requests.head(url)
         # ^ TODO : why doens't this work?
 
         response = requests.get(url)
 
@@ -422,15 +422,14 @@
         self,
         value,
         ext,
         renderers=None,
         extend_default_renderers=True,
         **kwargs,
     ):
-
         renderers = get_renderers(
             renderers=renderers, extend_default_renderers=extend_default_renderers
         )
         display_actions = DisplayFromCallable(path=value, ext=ext, renderers=renderers)
         super().__init__(display_actions=display_actions, **kwargs)
 
 
@@ -439,15 +438,14 @@
         self,
         value,
         ext,
         renderers=None,
         extend_default_renderers=True,
         **kwargs,
     ):
-
         renderers = get_renderers(
             renderers=renderers, extend_default_renderers=extend_default_renderers
         )
         display_actions = DisplayFromRequest(path=path, ext=ext, renderers=renderers)
         super().__init__(display_actions=display_actions, **kwargs)
 
 
@@ -523,14 +521,16 @@
         self.out_caller.layout.display = ""
         with self.out_caller:
             clear_output()
             self.display_actions.open_folder()
             time.sleep(5)
             clear_output()
         self.out_caller.layout.display = "none"
+
+
 # %%
 if __name__ == "__main__":
     d = DisplayFromPath(path="__init__.py")
     do = DisplayObject(d)
     display(do)
 
 # %%
@@ -552,22 +552,20 @@
     def get_catfact():
         return requests.get(path).content
 
     display(DisplayFromCallable(path=get_catfact, ext=ext).renderer())
 
 # %%
 if __name__ == "__main__":
-
     path = "https://catfact.ninja/fact"
     ext = ".json"
     display(DisplayRequest(value=path, ext=ext, order=ORDER_DEFAULT))
 
 # %%
 if __name__ == "__main__":
-
     ext = ".json"
     dobj = DisplayCallable(value=get_catfact, ext=ext)
     display(dobj)
 
 # %%
 if __name__ == "__main__":
     import json
@@ -627,18 +625,19 @@
     d.order = ORDER_DEFAULT
     display(d)
 
 
 # %%
 class AutoDisplay(tr.HasTraits):
     order = tr.Tuple(default_value=ORDER_NOTPATH, allow_none=False)
-    
+
     @tr.observe("order")
     def _observe_order(self, change):
         self._update_bx_bar(change["new"])
+
     """
     displays the contents of a file in the notebook.
     comes with the following default renderers:
     DEFAULT_FILE_RENDERERS = {
         '.csv': csv_prev,
         '.json': json_prev,
         '.plotly': plotlyjson_prev,
```

### Comparing `ipyautoui-0.5.2/src/ipyautoui/autodisplay_renderers.py` & `ipyautoui-0.5.3/src/ipyautoui/autodisplay_renderers.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.2/src/ipyautoui/autoipywidget.py` & `ipyautoui-0.5.3/src/ipyautoui/autoipywidget.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.2/src/ipyautoui/automapschema.py` & `ipyautoui-0.5.3/src/ipyautoui/automapschema.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 # %load_ext lab_black
 import typing as ty
 from pydantic import BaseModel, Field
 import ipywidgets as w
 import ipyautoui.autowidgets as auiwidgets
 from ipyautoui._utils import frozenmap, obj_from_importstr
 
+
 # +
 #  -- ATTACH DEFINITIONS TO PROPERTIES ----------------------
 def recursive_search_schema(schema: ty.Dict, li: ty.List) -> ty.Dict:
     """searches down schema tree to retrieve definitions
 
     Args:
         schema (ty.Dict): json schema made from pydantic
@@ -399,25 +400,35 @@
         return False
     if not "format" in di.keys():
         return False
     if "format" in di.keys() and di["format"] == "path":
         return True
     else:
         return False
+    
+def is_Combobox(di: dict) -> bool:
+    if "autoui" in di.keys():
+        return False
+    if "examples" not in di.keys():
+        return False
+    else:
+        return True
 
 
 def isnot_Text(di: dict) -> bool:
     if is_Date(di):
         return True
     if is_Color(di):
         return True
     if is_Markdown(di):
         return True
     if is_Path(di):
         return True
+    if is_Combobox(di):
+        return True
     return False
 
 
 def is_Text(di: dict) -> bool:
     """check if schema object is a Text
 
     Args:
@@ -590,15 +601,14 @@
     try:
         if "nullable" in caller.schema_.keys() and caller.schema_["nullable"]:
             fn = auiwidgets.nullable(caller.autoui)
         else:
             fn = caller.autoui
         wi = fn(caller.schema_, *caller.args, **caller.kwargs)
     except Exception as e:
-
         if show_errors:
             from ipyautoui.custom.widgetcaller_error import WidgetCallerError
 
             txt = f"""
 ERROR: widgetcaller
 -----
 widget:
@@ -662,14 +672,15 @@
             ),
             "Text": WidgetMapper(fn_filt=is_Text, widget=auiwidgets.Text),
             "Textarea": WidgetMapper(fn_filt=is_Textarea, widget=auiwidgets.Textarea),
             "Markdown": WidgetMapper(
                 fn_filt=is_Markdown, widget=auiwidgets.AutoMarkdown
             ),
             "Dropdown": WidgetMapper(fn_filt=is_Dropdown, widget=auiwidgets.Dropdown),
+            "Combobox": WidgetMapper(fn_filt=is_Combobox, widget=auiwidgets.Combobox),
             "SelectMultiple": WidgetMapper(
                 fn_filt=is_SelectMultiple, widget=auiwidgets.SelectMultiple
             ),
             "Color": WidgetMapper(fn_filt=is_Color, widget=auiwidgets.ColorPicker),
             "Path": WidgetMapper(fn_filt=is_Path, widget=auiwidgets.FileChooser),
             "Checkbox": WidgetMapper(fn_filt=is_Checkbox, widget=auiwidgets.Checkbox),
             "Date": WidgetMapper(fn_filt=is_Date, widget=auiwidgets.DatePickerString),
```

### Comparing `ipyautoui-0.5.2/src/ipyautoui/autoui.py` & `ipyautoui-0.5.3/src/ipyautoui/autoui.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.2/src/ipyautoui/autovjsf.py` & `ipyautoui-0.5.3/src/ipyautoui/autovjsf.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.2/src/ipyautoui/autowidgets.py` & `ipyautoui-0.5.3/src/ipyautoui/autowidgets.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.2/src/ipyautoui/basemodel.py` & `ipyautoui-0.5.3/src/ipyautoui/basemodel.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.2/src/ipyautoui/constants.py` & `ipyautoui-0.5.3/src/ipyautoui/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,46 +54,46 @@
 )
 # ---------------------------
 ADD_BUTTON_KWARGS = frozenmap(
     icon="plus",
     style={},
     button_style="success",
     tooltip="add item",
-    layout={"width": BUTTON_WIDTH_MIN}, #, "height": BUTTON_HEIGHT_MIN
+    layout={"width": BUTTON_WIDTH_MIN},  # , "height": BUTTON_HEIGHT_MIN
     disabled=False,
 )
 EDIT_BUTTON_KWARGS = frozenmap(
     icon="edit",
     style={},
     button_style="warning",
     tooltip="add item",
-    layout={"width": BUTTON_WIDTH_MIN}, #, "height": BUTTON_HEIGHT_MIN
+    layout={"width": BUTTON_WIDTH_MIN},  # , "height": BUTTON_HEIGHT_MIN
     disabled=False,
 )
 REMOVE_BUTTON_KWARGS = frozenmap(
     icon="minus",
     style={},
     button_style="danger",
     tooltip="remove item",
-    layout={"width": BUTTON_WIDTH_MIN}, #, "height": BUTTON_HEIGHT_MIN
+    layout={"width": BUTTON_WIDTH_MIN},  # , "height": BUTTON_HEIGHT_MIN
     disabled=False,
 )
 COPY_BUTTON_KWARGS = frozenmap(
     icon="copy",
     style={},
     button_style="primary",
     tooltip="copy item",
-    layout={"width": BUTTON_WIDTH_MIN}, #, "height": BUTTON_HEIGHT_MIN
+    layout={"width": BUTTON_WIDTH_MIN},  # , "height": BUTTON_HEIGHT_MIN
 )
 RELOAD_BUTTON_KWARGS = frozenmap(
     icon="sync",
     style={},
     button_style="info",
     tooltip="reload",
-    layout={"width": BUTTON_WIDTH_MIN}, #, "height": BUTTON_HEIGHT_MIN
+    layout={"width": BUTTON_WIDTH_MIN},  # , "height": BUTTON_HEIGHT_MIN
     disabled=False,
 )
 BLANK_BUTTON_KWARGS = frozenmap(
     icon="",
     style={"button_color": "white"},
     layout={"width": BUTTON_WIDTH_MIN, "height": BUTTON_HEIGHT_MIN},
     disabled=True,
@@ -182,14 +182,15 @@
 )
 
 MAP_JSONSCHEMA_TO_IPYWIDGET = frozenmap(
     **{
         "minimum": "min",
         "maximum": "max",
         "enum": "options",
+        "examples": "options",
         "default": "value",
         "description": "autoui_description",
     }
 )
 #  ^ this is how the json-schema names map to ipywidgets.
```

### Comparing `ipyautoui-0.5.2/src/ipyautoui/demo.py` & `ipyautoui-0.5.3/src/ipyautoui/demo.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.2/src/ipyautoui/env.py` & `ipyautoui-0.5.3/src/ipyautoui/env.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.2/src/ipyautoui/mydocstring_display.py` & `ipyautoui-0.5.3/src/ipyautoui/mydocstring_display.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.2/src/ipyautoui/test_schema.py` & `ipyautoui-0.5.3/src/ipyautoui/test_schema.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.2/src/ipyautoui/vjsf.vue` & `ipyautoui-0.5.3/src/ipyautoui/vjsf.vue`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.2/src/ipyautoui/custom/autogrid.py` & `ipyautoui-0.5.3/src/ipyautoui/custom/autogrid.py`

 * *Files 0% similar despite different names*

```diff
@@ -1042,24 +1042,25 @@
             return self.data.T.loc[self.selected_col_indexes].to_dict("index")
         else:
             return self.data.loc[self.selected_row_indexes].to_dict("index")
 
     # ----------------
 
 
-# +
+# -
+
 if __name__ == "__main__":
 
     class DataFrameCols(BaseModel):
         string: str = Field(
             "string",
             title="Important String",
             column_width=120,
         )
-        integer: int = Field(40, title="Integer of somesort", column_width=150)
+        integer: int = Field(40, title="Integer of somesort", column_width=400)
         floater: float = Field(
             1.3398234, title="Floater", column_width=70  # , renderer={"format": ".2f"}
         )
 
     class TestDataFrame(BaseModel):
         # dataframe: ty.List[DataFrameCols] = Field(..., format="dataframe")
         __root__: ty.List[DataFrameCols] = Field(
@@ -1067,15 +1068,14 @@
             format="dataframe",
             global_decimal_places=2,
         )
 
     grid = AutoGrid(schema=TestDataFrame, by_title=True)
     display(grid)
 
-
 if __name__ == "__main__":
     # ORDER OVERRIDE
     class DataFrameCols(BaseModel):
         string: str = Field(
             "string",
             title="Important String",
             column_width=120,
@@ -1130,15 +1130,15 @@
 if __name__ == "__main__":
 
     class DataFrameCols(BaseModel):
         string: str = Field(
             title="Important String",
             column_width=120,
         )
-        integer: int = Field(title="Integer of somesort", column_width=150)
+        integer: int = Field(title="Integer of somesort", column_width=400)
         floater: float = Field(
             title="Floater", column_width=70  # , renderer={"format": ".2f"}
         )
 
     class TestDataFrame(BaseModel):
         __root__: ty.List[DataFrameCols] = Field(
             [
@@ -1149,14 +1149,24 @@
             format="dataframe",
             global_decimal_places=2,
         )
 
     grid = AutoGrid(schema=TestDataFrame, by_title=True)
     display(grid)
 
+# +
+
+
+
+
+
+
+
+
+
 if __name__ == "__main__":
     grid.data = pd.DataFrame(grid.data.to_dict(orient="records") * 4)  # .T
 
 if __name__ == "__main__":
     print(grid.is_transposed)
 
 if __name__ == "__main__":
```

### Comparing `ipyautoui-0.5.2/src/ipyautoui/custom/buttonbars.py` & `ipyautoui-0.5.3/src/ipyautoui/custom/buttonbars.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.2/src/ipyautoui/custom/decision_branch.py` & `ipyautoui-0.5.3/src/ipyautoui/custom/decision_branch.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.2/src/ipyautoui/custom/editgrid.py` & `ipyautoui-0.5.3/src/ipyautoui/custom/editgrid.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #   jupytext:
 #     cell_metadata_filter: -all
 #     formats: py:light
 #     text_representation:
 #       extension: .py
 #       format_name: light
 #       format_version: '1.5'
-#       jupytext_version: 1.14.5
+#       jupytext_version: 1.14.0
 #   kernelspec:
 #     display_name: Python 3 (ipykernel)
 #     language: python
 #     name: python3
 # ---
 
 # +
@@ -442,21 +442,22 @@
                 "you must select an index (row if transposed==True, col if"
                 " transposed==True)"
             )
         self._check_one_row_selected()
 
     def _save_edit_to_grid(self):
         selections = self.grid.selections  # Store current selection
+        selected_index = self.grid.selected_index
         self.grid.selections = []
         # ^ HOTFIX: Have to set empty to reselect later on
 
         if self.datahandler is not None:
             self._reload_all_data()
         else:
-            self.grid.set_item_value(self.grid.selected_index, self.ui_edit.value)
+            self.grid.set_item_value(selected_index, self.ui_edit.value)
 
         if self.close_crud_dialogue_on_action:
             self.buttonbar_grid.edit.value = False
         else:
             # Reselect previous selection after reload.
             self.grid.selections = selections
 
@@ -624,19 +625,17 @@
             "integer": 1,
             "floater": 3.14,
         },
     ]
     AUTO_GRID_DEFAULT_VALUE = AUTO_GRID_DEFAULT_VALUE * 4
 
     class DataFrameCols(BaseModel):
-        string: str = Field("string", column_width=100, section="a")
+        string: str = Field("string", column_width=400, section="a")
         integer: int = Field(1, column_width=80, section="a")
-        floater: float = Field(
-            None, column_width=70, global_decimal_places=3, section="b"
-        )
+        floater: float = Field(None, column_width=70, section="b")
 
     class TestDataFrame(BaseModel):
         """a description of TestDataFrame"""
 
         __root__: ty.List[DataFrameCols] = Field(
             default=AUTO_GRID_DEFAULT_VALUE,
             format="dataframe",
@@ -650,14 +649,16 @@
         title=title,
         description=description,
         ui_add=None,
         ui_edit=None,
         warn_on_delete=True,
         show_copy_dialogue=False,
         close_crud_dialogue_on_action=False,
+        global_decimal_places=1,
+        column_width={"String": 400},
     )
     editgrid.observe(lambda c: print("_value changed"), "_value")
     display(editgrid)
 
 
 if __name__ == "__main__":
     editgrid.grid.order = ("floater", "string")
@@ -688,34 +689,32 @@
 # editgrid._reload_datahandler()
 # -
 
 if __name__ == "__main__":
     from ipyautoui.demo_schemas import CoreIpywidgets
     from ipyautoui.autoipywidget import AutoObject
 
-    #     class TestDataFrame(BaseModel):
-    #         """a description of TestDataFrame"""
-
-    #         __root__: ty.List[CoreIpywidgets] = Field(
-    #             [CoreIpywidgets().dict()], format="dataframe"
-    #         )
-    # TODO: ^ fix this
+    class DataFrameCols(BaseModel):
+        string: str = Field("string", column_width=400, section="a")
+        integer: int = Field(1, column_width=80, section="b")
+        floater: float = Field(None, column_width=70, section="b")
 
     class TestDataFrame(BaseModel):
         """a description of TestDataFrame"""
 
         __root__: ty.List[DataFrameCols] = Field(
             [
                 DataFrameCols(
                     string="String",
                     integer=1,
                     floater=2.5,
                 ).dict()
             ],
             format="dataframe",
+            #datagrid_index_name=("section", "title"),
         )
 
     description = markdown(
         "<b>The Wonderful Edit Grid Application</b><br>Useful for all editing purposes"
         " whatever they may be 👍"
     )
     editgrid = EditGrid(
```

### Comparing `ipyautoui-0.5.2/src/ipyautoui/custom/filechooser.py` & `ipyautoui-0.5.3/src/ipyautoui/custom/filechooser.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.2/src/ipyautoui/custom/filesindir.py` & `ipyautoui-0.5.3/src/ipyautoui/custom/filesindir.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.2/src/ipyautoui/custom/fileupload.py` & `ipyautoui-0.5.3/src/ipyautoui/custom/fileupload.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.2/src/ipyautoui/custom/iterable.py` & `ipyautoui-0.5.3/src/ipyautoui/custom/iterable.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.2/src/ipyautoui/custom/loadproject.py` & `ipyautoui-0.5.3/src/ipyautoui/custom/loadproject.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.2/src/ipyautoui/custom/markdown_widget.py` & `ipyautoui-0.5.3/src/ipyautoui/custom/markdown_widget.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.2/src/ipyautoui/custom/modelrun.py` & `ipyautoui-0.5.3/src/ipyautoui/custom/modelrun.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.2/src/ipyautoui/custom/multiselect_search.py` & `ipyautoui-0.5.3/src/ipyautoui/custom/multiselect_search.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.2/src/ipyautoui/custom/outputlogging.py` & `ipyautoui-0.5.3/src/ipyautoui/custom/outputlogging.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.2/src/ipyautoui/custom/selectdir.py` & `ipyautoui-0.5.3/src/ipyautoui/custom/selectdir.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.2/src/ipyautoui/custom/showhide.py` & `ipyautoui-0.5.3/src/ipyautoui/custom/showhide.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.2/src/ipyautoui/custom/showopenurl.py` & `ipyautoui-0.5.3/src/ipyautoui/custom/showopenurl.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.2/src/ipyautoui/custom/title_description.py` & `ipyautoui-0.5.3/src/ipyautoui/custom/title_description.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.2/src/ipyautoui/custom/urlimagelink.py` & `ipyautoui-0.5.3/src/ipyautoui/custom/urlimagelink.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.2/src/ipyautoui/custom/widgetcaller_error.py` & `ipyautoui-0.5.3/src/ipyautoui/custom/widgetcaller_error.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,50 +22,48 @@
 # %run ../_dev_sys_path_append.py
 # %run __init__.py
 # %run ../__init__.py
 
 # %%
 import ipywidgets as w
 import traitlets as tr
-from IPython.display import clear_output
-from IPython.display import JSON
+from IPython.display import clear_output, JSON, display
 from ipyautoui._utils import display_python_string
 
 
 # %%
 class WidgetCallerError(w.VBox):
     widget = tr.Unicode(default_value="")
     error = tr.Unicode(default_value="")
     schema = tr.Dict(default_value={})
+    value = tr.Unicode(default_value="error")
 
     @tr.observe("widget")
     def _observe_widget(self, change):
         with self.out_widget:
             clear_output()
             display_python_string(change["new"])
         return change["new"]
 
     @tr.observe("error")
     def _observe_error(self, change):
-
         with self.out_error:
             clear_output()
             display_python_string(change["new"])
         return change["new"]
 
     @tr.observe("schema")
     def _observe_schema(self, change):
         with self.out_schema:
             clear_output()
             display(JSON(change["new"]))
 
         return change["new"]
 
     def __init__(self, **kwargs):
-
         self.html_widget_title = w.HTML("<b>Widget Name:</b>")
         self.html_error_title = w.HTML("<b>Error:</b>")
         self.html_schema_title = w.HTML("<b>JsonSchema that generates UI:</b>")
         self.out_widget = w.Output()
         self.out_error = w.Output()
         self.out_schema = w.Output()
         super().__init__(**kwargs)
```

### Comparing `ipyautoui-0.5.2/src/ipyautoui/custom/workingdir.py` & `ipyautoui-0.5.3/src/ipyautoui/custom/workingdir.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.2/src/ipyautoui/demo_schemas/__init__.py` & `ipyautoui-0.5.3/src/ipyautoui/demo_schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.2/src/ipyautoui/demo_schemas/complex_serialization.py` & `ipyautoui-0.5.3/src/ipyautoui/demo_schemas/complex_serialization.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.2/src/ipyautoui/demo_schemas/core_ipywidgets.py` & `ipyautoui-0.5.3/src/ipyautoui/demo_schemas/core_ipywidgets.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,21 +24,24 @@
     """
 
     int_slider_req: conint(ge=1, le=3)
     int_slider_nullable: conint(ge=1, le=3) = None
     int_slider: conint(ge=1, le=3) = 2
     int_text: int = 1
     int_range_slider: tuple[int, int] = Field(default=(0, 3), ge=0, le=4)
-    int_range_slider_disabled: tuple[int, int] = Field(default=(0, 3), ge=0, le=4, disabled=True)
+    int_range_slider_disabled: tuple[int, int] = Field(
+        default=(0, 3), ge=0, le=4, disabled=True
+    )
     float_slider: float = Field(default=2.2, ge=1, le=3)
     float_text: float = 2.2
     float_text_locked: float = Field(default=2.2, disabled=True)
     float_range_slider: tuple[float, float] = Field(default=(0, 2.2), ge=0, le=3.5)
     checkbox: bool = True
     dropdown: FruitEnum = None
+    combobox: str = Field("apple", examples=FruitEnum._member_names_)
     dropdown_edge_case: FruitEnum = Field(
         title="FruitEnum with metadata",
         default=FruitEnum.apple,
         description="updated description",
     )
     dropdown_simple: str = Field(default="asd", enum=["asd", "asdf"])
     text: str = Field(default="adsf", description="a description about my string")
```

### Comparing `ipyautoui-0.5.2/src/ipyautoui/demo_schemas/editable_datagrid.py` & `ipyautoui-0.5.3/src/ipyautoui/demo_schemas/editable_datagrid.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.2/src/ipyautoui/demo_schemas/nested.py` & `ipyautoui-0.5.3/src/ipyautoui/demo_schemas/nested.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.2/src/ipyautoui/demo_schemas/nested_editable_datagrid.py` & `ipyautoui-0.5.3/src/ipyautoui/demo_schemas/nested_editable_datagrid.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.2/src/ipyautoui/demo_schemas/nullable_core_ipywidgets.py` & `ipyautoui-0.5.3/src/ipyautoui/demo_schemas/nullable_core_ipywidgets.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.2/src/ipyautoui/demo_schemas/root_array_enum.py` & `ipyautoui-0.5.3/src/ipyautoui/demo_schemas/root_array_enum.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.2/src/ipyautoui/demo_schemas/root_enum.py` & `ipyautoui-0.5.3/src/ipyautoui/demo_schemas/root_enum.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.2/src/ipyautoui/demo_schemas/ruleset.py` & `ipyautoui-0.5.3/src/ipyautoui/demo_schemas/ruleset.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.2/.gitignore` & `ipyautoui-0.5.3/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -69,14 +69,15 @@
 /ipyautoui/__pycache__
 /docs/autoui_mapping.xlsx
 /src/ipyautoui/custom/.ipynb_checkpoints
 /src/ipyautoui/custom/__pycache__
 /src/ipyautoui/autoui.ipynb
 /src/ipyautoui/displayfile.ipynb
 /src/ipyautoui/.ipynb_checkpoints
+/src/ipyautoui/_version.py
 /src/ipyautoui/demo_schemas/.ipynb_checkpoints/
 /src/ipyautoui/demo_schemas/.__pycache__/
 /tests/.ipynb_checkpoints
 /tests/__pycache__
 /tests/testdata/.ipynb_checkpoints
 /tests/filetypes/.ipynb_checkpoints
 /examples/.ipynb_checkpoints
```

### Comparing `ipyautoui-0.5.2/LICENSE` & `ipyautoui-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.2/README.md` & `ipyautoui-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.2/pyproject.toml` & `ipyautoui-0.5.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -35,15 +35,17 @@
 ]
 
 [project.urls]
 Homepage = "https://github.com/maxfordham/ipyautoui"
 
 [tool.hatch.version]
 source = "vcs"
-version-file = "_version.py"
+
+[tool.hatch.build.hooks.vcs]
+version-file = "src/ipyautoui/_version.py"
 
 [tool.hatch.build.targets.sdist]
 include = ["/src/ipyautoui"]
 
 # [tool.hatch.envs.ipyautoui-dev]
 # type = "conda"
 # command = "mamba"
```

### Comparing `ipyautoui-0.5.2/PKG-INFO` & `ipyautoui-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyautoui
-Version: 0.5.2
+Version: 0.5.3
 Summary: wrapper that sits on top of ipywidgets and other ipy widget libraries to template / automate the creation of widget forms. Uses pydantic to create defined data-container and serialisation to JSON. Includes example patterns for adding new custom widgets.
 Project-URL: Homepage, https://github.com/maxfordham/ipyautoui
 Author-email: John Gunstone <gunstone.john@gmail.com>
 License-File: LICENSE
 Keywords: ipyautoui
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

