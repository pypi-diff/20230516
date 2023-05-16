# Comparing `tmp/djangocms_xliff-1.3.3.tar.gz` & `tmp/djangocms_xliff-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangocms_xliff-1.3.3.tar", max compression
+gzip compressed data, was "djangocms_xliff-1.3.4.tar", max compression
```

## Comparing `djangocms_xliff-1.3.3.tar` & `djangocms_xliff-1.3.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1073 2023-05-16 12:00:07.315426 djangocms_xliff-1.3.3/LICENSE
--rw-r--r--   0        0        0     7132 2023-05-16 12:00:07.315426 djangocms_xliff-1.3.3/README.md
--rw-r--r--   0        0        0       22 2023-05-16 12:00:07.315426 djangocms_xliff-1.3.3/djangocms_xliff/__init__.py
--rw-r--r--   0        0        0      216 2023-05-16 12:00:07.315426 djangocms_xliff-1.3.3/djangocms_xliff/apps.py
--rw-r--r--   0        0        0     2537 2023-05-16 12:00:07.315426 djangocms_xliff-1.3.3/djangocms_xliff/cms_toolbars.py
--rw-r--r--   0        0        0      186 2023-05-16 12:00:07.315426 djangocms_xliff-1.3.3/djangocms_xliff/exceptions.py
--rw-r--r--   0        0        0     1276 2023-05-16 12:00:07.315426 djangocms_xliff-1.3.3/djangocms_xliff/exports.py
--rw-r--r--   0        0        0     9424 2023-05-16 12:00:07.315426 djangocms_xliff-1.3.3/djangocms_xliff/extractors.py
--rw-r--r--   0        0        0      801 2023-05-16 12:00:07.315426 djangocms_xliff-1.3.3/djangocms_xliff/forms.py
--rw-r--r--   0        0        0     4671 2023-05-16 12:00:07.315426 djangocms_xliff-1.3.3/djangocms_xliff/imports.py
--rw-r--r--   0        0        0     4022 2023-05-16 12:00:07.315426 djangocms_xliff-1.3.3/djangocms_xliff/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     5560 2023-05-16 12:00:07.315426 djangocms_xliff-1.3.3/djangocms_xliff/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2023-05-16 12:00:07.315426 djangocms_xliff-1.3.3/djangocms_xliff/management/__init__.py
--rw-r--r--   0        0        0        0 2023-05-16 12:00:07.315426 djangocms_xliff-1.3.3/djangocms_xliff/management/commands/__init__.py
--rw-r--r--   0        0        0     1804 2023-05-16 12:00:07.315426 djangocms_xliff-1.3.3/djangocms_xliff/management/commands/xliff_export.py
--rw-r--r--   0        0        0     1704 2023-05-16 12:00:07.315426 djangocms_xliff-1.3.3/djangocms_xliff/management/commands/xliff_import.py
--rw-r--r--   0        0        0     1623 2023-05-16 12:00:07.315426 djangocms_xliff-1.3.3/djangocms_xliff/management/commands/xliff_page_plugins.py
--rw-r--r--   0        0        0     5662 2023-05-16 12:00:07.315426 djangocms_xliff-1.3.3/djangocms_xliff/parsers.py
--rw-r--r--   0        0        0     1148 2023-05-16 12:00:07.315426 djangocms_xliff-1.3.3/djangocms_xliff/renderer.py
--rw-r--r--   0        0        0     1534 2023-05-16 12:00:07.315426 djangocms_xliff-1.3.3/djangocms_xliff/settings.py
--rw-r--r--   0        0        0      193 2023-05-16 12:00:07.315426 djangocms_xliff-1.3.3/djangocms_xliff/templates/djangocms_xliff/base.html
--rw-r--r--   0        0        0      151 2023-05-16 12:00:07.315426 djangocms_xliff-1.3.3/djangocms_xliff/templates/djangocms_xliff/error.html
--rw-r--r--   0        0        0      522 2023-05-16 12:00:07.315426 djangocms_xliff-1.3.3/djangocms_xliff/templates/djangocms_xliff/export/index.html
--rw-r--r--   0        0        0     1000 2023-05-16 12:00:07.315426 djangocms_xliff-1.3.3/djangocms_xliff/templates/djangocms_xliff/export/v1.2.xliff
--rw-r--r--   0        0        0     1389 2023-05-16 12:00:07.315426 djangocms_xliff-1.3.3/djangocms_xliff/templates/djangocms_xliff/import/preview.html
--rw-r--r--   0        0        0     1116 2023-05-16 12:00:07.315426 djangocms_xliff-1.3.3/djangocms_xliff/templates/djangocms_xliff/import/success.html
--rw-r--r--   0        0        0      447 2023-05-16 12:00:07.315426 djangocms_xliff-1.3.3/djangocms_xliff/templates/djangocms_xliff/import/upload.html
--rw-r--r--   0        0        0     2328 2023-05-16 12:00:07.315426 djangocms_xliff-1.3.3/djangocms_xliff/types.py
--rw-r--r--   0        0        0      589 2023-05-16 12:00:07.315426 djangocms_xliff-1.3.3/djangocms_xliff/urls.py
--rw-r--r--   0        0        0     4155 2023-05-16 12:00:07.315426 djangocms_xliff-1.3.3/djangocms_xliff/utils.py
--rw-r--r--   0        0        0     6860 2023-05-16 12:00:07.315426 djangocms_xliff-1.3.3/djangocms_xliff/views.py
--rw-r--r--   0        0        0     1364 2023-05-16 12:00:07.319426 djangocms_xliff-1.3.3/pyproject.toml
--rw-r--r--   0        0        0     8399 1970-01-01 00:00:00.000000 djangocms_xliff-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-16 13:27:36.585963 djangocms_xliff-1.3.4/LICENSE
+-rw-r--r--   0        0        0     7132 2023-05-16 13:27:36.585963 djangocms_xliff-1.3.4/README.md
+-rw-r--r--   0        0        0       22 2023-05-16 13:27:36.585963 djangocms_xliff-1.3.4/djangocms_xliff/__init__.py
+-rw-r--r--   0        0        0      216 2023-05-16 13:27:36.585963 djangocms_xliff-1.3.4/djangocms_xliff/apps.py
+-rw-r--r--   0        0        0     2537 2023-05-16 13:27:36.585963 djangocms_xliff-1.3.4/djangocms_xliff/cms_toolbars.py
+-rw-r--r--   0        0        0      186 2023-05-16 13:27:36.585963 djangocms_xliff-1.3.4/djangocms_xliff/exceptions.py
+-rw-r--r--   0        0        0     1276 2023-05-16 13:27:36.585963 djangocms_xliff-1.3.4/djangocms_xliff/exports.py
+-rw-r--r--   0        0        0     9404 2023-05-16 13:27:36.585963 djangocms_xliff-1.3.4/djangocms_xliff/extractors.py
+-rw-r--r--   0        0        0      801 2023-05-16 13:27:36.585963 djangocms_xliff-1.3.4/djangocms_xliff/forms.py
+-rw-r--r--   0        0        0     4663 2023-05-16 13:27:36.585963 djangocms_xliff-1.3.4/djangocms_xliff/imports.py
+-rw-r--r--   0        0        0     4022 2023-05-16 13:27:36.589963 djangocms_xliff-1.3.4/djangocms_xliff/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     5560 2023-05-16 13:27:36.589963 djangocms_xliff-1.3.4/djangocms_xliff/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2023-05-16 13:27:36.589963 djangocms_xliff-1.3.4/djangocms_xliff/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-16 13:27:36.589963 djangocms_xliff-1.3.4/djangocms_xliff/management/commands/__init__.py
+-rw-r--r--   0        0        0     1804 2023-05-16 13:27:36.589963 djangocms_xliff-1.3.4/djangocms_xliff/management/commands/xliff_export.py
+-rw-r--r--   0        0        0     1704 2023-05-16 13:27:36.589963 djangocms_xliff-1.3.4/djangocms_xliff/management/commands/xliff_import.py
+-rw-r--r--   0        0        0     1623 2023-05-16 13:27:36.589963 djangocms_xliff-1.3.4/djangocms_xliff/management/commands/xliff_page_plugins.py
+-rw-r--r--   0        0        0     5662 2023-05-16 13:27:36.589963 djangocms_xliff-1.3.4/djangocms_xliff/parsers.py
+-rw-r--r--   0        0        0     1148 2023-05-16 13:27:36.589963 djangocms_xliff-1.3.4/djangocms_xliff/renderer.py
+-rw-r--r--   0        0        0     1534 2023-05-16 13:27:36.589963 djangocms_xliff-1.3.4/djangocms_xliff/settings.py
+-rw-r--r--   0        0        0      193 2023-05-16 13:27:36.589963 djangocms_xliff-1.3.4/djangocms_xliff/templates/djangocms_xliff/base.html
+-rw-r--r--   0        0        0      151 2023-05-16 13:27:36.589963 djangocms_xliff-1.3.4/djangocms_xliff/templates/djangocms_xliff/error.html
+-rw-r--r--   0        0        0      522 2023-05-16 13:27:36.589963 djangocms_xliff-1.3.4/djangocms_xliff/templates/djangocms_xliff/export/index.html
+-rw-r--r--   0        0        0     1000 2023-05-16 13:27:36.589963 djangocms_xliff-1.3.4/djangocms_xliff/templates/djangocms_xliff/export/v1.2.xliff
+-rw-r--r--   0        0        0     1389 2023-05-16 13:27:36.589963 djangocms_xliff-1.3.4/djangocms_xliff/templates/djangocms_xliff/import/preview.html
+-rw-r--r--   0        0        0     1116 2023-05-16 13:27:36.589963 djangocms_xliff-1.3.4/djangocms_xliff/templates/djangocms_xliff/import/success.html
+-rw-r--r--   0        0        0      447 2023-05-16 13:27:36.589963 djangocms_xliff-1.3.4/djangocms_xliff/templates/djangocms_xliff/import/upload.html
+-rw-r--r--   0        0        0     2328 2023-05-16 13:27:36.589963 djangocms_xliff-1.3.4/djangocms_xliff/types.py
+-rw-r--r--   0        0        0      589 2023-05-16 13:27:36.589963 djangocms_xliff-1.3.4/djangocms_xliff/urls.py
+-rw-r--r--   0        0        0     4155 2023-05-16 13:27:36.589963 djangocms_xliff-1.3.4/djangocms_xliff/utils.py
+-rw-r--r--   0        0        0     6860 2023-05-16 13:27:36.589963 djangocms_xliff-1.3.4/djangocms_xliff/views.py
+-rw-r--r--   0        0        0     1364 2023-05-16 13:27:36.593963 djangocms_xliff-1.3.4/pyproject.toml
+-rw-r--r--   0        0        0     8399 1970-01-01 00:00:00.000000 djangocms_xliff-1.3.4/PKG-INFO
```

### Comparing `djangocms_xliff-1.3.3/LICENSE` & `djangocms_xliff-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.3.3/README.md` & `djangocms_xliff-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.3.3/djangocms_xliff/cms_toolbars.py` & `djangocms_xliff-1.3.4/djangocms_xliff/cms_toolbars.py`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.3.3/djangocms_xliff/exports.py` & `djangocms_xliff-1.3.4/djangocms_xliff/exports.py`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.3.3/djangocms_xliff/extractors.py` & `djangocms_xliff-1.3.4/djangocms_xliff/extractors.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 
 from djangocms_xliff.exceptions import XliffExportError
 from djangocms_xliff.settings import (
     FIELD_EXTRACTORS,
     FIELDS,
     MODEL_METADATA_FIELDS,
     TITLE_METADATA_FIELDS,
-    UNIT_ID_METADATA_ID,
     VALIDATORS,
 )
 from djangocms_xliff.types import Unit, XliffObj
 from djangocms_xliff.utils import (
     get_plugin_id_for_extension_obj,
     get_plugin_id_for_metadata_obj,
     get_type_with_path,
@@ -255,16 +254,16 @@
     metadata_units = []
     if include_metadata:
         metadata_units.extend(
             extract_metadata_from_obj(
                 obj=obj,
                 language=language,
                 plugin_id=get_plugin_id_for_metadata_obj(obj),
-                plugin_type=UNIT_ID_METADATA_ID,
-                plugin_name=UNIT_ID_METADATA_ID,
+                plugin_type=obj._meta.object_name,
+                plugin_name=obj._meta.verbose_name,
             )
         )
 
     extension_data_units = []
     if type(obj) == Page:
         extension_data_units.extend(extract_extension_data_from_page(obj, language))
```

### Comparing `djangocms_xliff-1.3.3/djangocms_xliff/forms.py` & `djangocms_xliff-1.3.4/djangocms_xliff/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.3.3/djangocms_xliff/imports.py` & `djangocms_xliff-1.3.4/djangocms_xliff/imports.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,16 +25,16 @@
                 content_type_id, instance_id, field_name = unit.field_name.split(UNIT_ID_DELIMITER)
                 obj = get_obj(int(content_type_id), instance_id)
             except ValueError:
                 # For backwards compatibility, if there are existing xliff files
                 field_name = unit.field_name
                 obj = lazy_xliff_obj()
 
-                if type(obj) == Page:
-                    obj = obj.get_title_obj()
+            if type(obj) == Page:
+                obj = obj.get_title_obj()
 
             target = unit.target
             setattr(obj, field_name, target)
             obj.save()
 
 
 def save_xliff_units_for_extension_data(units: List[Unit], target_language: str) -> None:
```

### Comparing `djangocms_xliff-1.3.3/djangocms_xliff/locale/de/LC_MESSAGES/django.mo` & `djangocms_xliff-1.3.4/djangocms_xliff/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.3.3/djangocms_xliff/locale/de/LC_MESSAGES/django.po` & `djangocms_xliff-1.3.4/djangocms_xliff/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.3.3/djangocms_xliff/management/commands/xliff_export.py` & `djangocms_xliff-1.3.4/djangocms_xliff/management/commands/xliff_export.py`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.3.3/djangocms_xliff/management/commands/xliff_import.py` & `djangocms_xliff-1.3.4/djangocms_xliff/management/commands/xliff_import.py`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.3.3/djangocms_xliff/management/commands/xliff_page_plugins.py` & `djangocms_xliff-1.3.4/djangocms_xliff/management/commands/xliff_page_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.3.3/djangocms_xliff/parsers.py` & `djangocms_xliff-1.3.4/djangocms_xliff/parsers.py`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.3.3/djangocms_xliff/renderer.py` & `djangocms_xliff-1.3.4/djangocms_xliff/renderer.py`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.3.3/djangocms_xliff/settings.py` & `djangocms_xliff-1.3.4/djangocms_xliff/settings.py`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.3.3/djangocms_xliff/templates/djangocms_xliff/export/index.html` & `djangocms_xliff-1.3.4/djangocms_xliff/templates/djangocms_xliff/export/index.html`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.3.3/djangocms_xliff/templates/djangocms_xliff/export/v1.2.xliff` & `djangocms_xliff-1.3.4/djangocms_xliff/templates/djangocms_xliff/export/v1.2.xliff`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.3.3/djangocms_xliff/templates/djangocms_xliff/import/preview.html` & `djangocms_xliff-1.3.4/djangocms_xliff/templates/djangocms_xliff/import/preview.html`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.3.3/djangocms_xliff/templates/djangocms_xliff/import/success.html` & `djangocms_xliff-1.3.4/djangocms_xliff/templates/djangocms_xliff/import/success.html`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.3.3/djangocms_xliff/types.py` & `djangocms_xliff-1.3.4/djangocms_xliff/types.py`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.3.3/djangocms_xliff/urls.py` & `djangocms_xliff-1.3.4/djangocms_xliff/urls.py`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.3.3/djangocms_xliff/utils.py` & `djangocms_xliff-1.3.4/djangocms_xliff/utils.py`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.3.3/djangocms_xliff/views.py` & `djangocms_xliff-1.3.4/djangocms_xliff/views.py`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.3.3/pyproject.toml` & `djangocms_xliff-1.3.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "djangocms-xliff"
-version = "1.3.3"
+version = "1.3.4"
 description = "XLIFF Import and Export for the Django CMS"
 authors = ["Energie 360 <onlineservice@energie360.ch>"]
 maintainers = ["Energie 360 <onlineservice@energie360.ch>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://energie360.ch"
 repository = "https://github.com/energie360/djangocms-xliff"
```

### Comparing `djangocms_xliff-1.3.3/PKG-INFO` & `djangocms_xliff-1.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangocms-xliff
-Version: 1.3.3
+Version: 1.3.4
 Summary: XLIFF Import and Export for the Django CMS
 Home-page: https://energie360.ch
 License: MIT
 Keywords: django,django-cms,xliff,import,export
 Author: Energie 360
 Author-email: onlineservice@energie360.ch
 Maintainer: Energie 360
```

