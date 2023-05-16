# Comparing `tmp/giant-redirect-import-0.1.0.tar.gz` & `tmp/giant_redirect_import-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "giant-redirect-import-0.1.0.tar", last modified: Tue Mar  2 13:43:50 2021, max compression
+gzip compressed data, was "giant_redirect_import-0.2.tar", max compression
```

## Comparing `giant-redirect-import-0.1.0.tar` & `giant_redirect_import-0.2.tar`

### file list

```diff
@@ -1,16 +1,14 @@
--rw-r--r--   0        0        0     1069 2021-02-24 15:29:38.453711 giant-redirect-import-0.1.0/LICENSE
--rw-r--r--   0        0        0     1069 2021-02-24 15:29:38.453711 giant-redirect-import-0.1.0/LICENSE
--rw-r--r--   0        0        0     1654 2021-02-24 15:45:49.462795 giant-redirect-import-0.1.0/README.md
--rw-r--r--   0        0        0        0 2021-02-24 15:26:36.021229 giant-redirect-import-0.1.0/giant_redirect_import/__init__.py
--rw-r--r--   0        0        0     1391 2021-02-24 15:26:36.025229 giant-redirect-import-0.1.0/giant_redirect_import/admin.py
--rw-r--r--   0        0        0     1962 2021-03-02 13:43:32.371329 giant-redirect-import-0.1.0/giant_redirect_import/forms.py
--rw-r--r--   0        0        0        0 2021-03-02 13:43:32.371329 giant-redirect-import-0.1.0/giant_redirect_import/templates/admin/base_site.html
--rw-r--r--   0        0        0      477 2021-03-02 13:43:32.371329 giant-redirect-import-0.1.0/giant_redirect_import/templates/redirects/admin/csv_import.html
--rw-r--r--   0        0        0      380 2021-03-02 13:43:32.371329 giant-redirect-import-0.1.0/giant_redirect_import/templates/redirects/admin/redirect_change_list.html
--rw-r--r--   0        0        0        0 2021-02-24 15:26:49.181547 giant-redirect-import-0.1.0/giant_redirect_import/tests/__init__.py
--rw-r--r--   0        0        0      102 2021-03-02 13:43:32.371329 giant-redirect-import-0.1.0/giant_redirect_import/tests/fixtures/test_data.csv
--rw-r--r--   0        0        0     1309 2021-03-02 13:43:32.371329 giant-redirect-import-0.1.0/giant_redirect_import/tests/test_forms.py
--rw-r--r--   0        0        0      153 2021-03-02 13:43:32.375329 giant-redirect-import-0.1.0/giant_redirect_import/tests/urls.py
--rw-r--r--   0        0        0     1117 2021-03-02 13:43:32.375329 giant-redirect-import-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2498 2021-03-02 13:43:50.480924 giant-redirect-import-0.1.0/setup.py
--rw-r--r--   0        0        0     2568 2021-03-02 13:43:50.481184 giant-redirect-import-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2021-02-24 15:29:38.453711 giant_redirect_import-0.2/LICENSE
+-rw-r--r--   0        0        0     1663 2023-05-16 09:06:38.460079 giant_redirect_import-0.2/README.md
+-rw-r--r--   0        0        0        0 2021-02-24 15:26:36.021229 giant_redirect_import-0.2/giant_redirect_import/__init__.py
+-rw-r--r--   0        0        0     1391 2021-02-24 15:26:36.025229 giant_redirect_import-0.2/giant_redirect_import/admin.py
+-rw-r--r--   0        0        0     2084 2023-05-16 09:14:13.086200 giant_redirect_import-0.2/giant_redirect_import/forms.py
+-rw-r--r--   0        0        0        0 2021-03-02 13:43:32.371329 giant_redirect_import-0.2/giant_redirect_import/templates/admin/base_site.html
+-rw-r--r--   0        0        0      477 2021-03-02 13:43:32.371329 giant_redirect_import-0.2/giant_redirect_import/templates/redirects/admin/csv_import.html
+-rw-r--r--   0        0        0      380 2021-03-02 13:43:32.371329 giant_redirect_import-0.2/giant_redirect_import/templates/redirects/admin/redirect_change_list.html
+-rw-r--r--   0        0        0        0 2021-02-24 15:26:49.181547 giant_redirect_import-0.2/giant_redirect_import/tests/__init__.py
+-rw-r--r--   0        0        0      102 2021-03-02 13:43:32.371329 giant_redirect_import-0.2/giant_redirect_import/tests/fixtures/test_data.csv
+-rw-r--r--   0        0        0     1309 2021-03-02 13:43:32.371329 giant_redirect_import-0.2/giant_redirect_import/tests/test_forms.py
+-rw-r--r--   0        0        0      153 2021-03-02 13:43:32.375329 giant_redirect_import-0.2/giant_redirect_import/tests/urls.py
+-rw-r--r--   0        0        0     1115 2023-05-16 09:14:13.086200 giant_redirect_import-0.2/pyproject.toml
+-rw-r--r--   0        0        0     2727 1970-01-01 00:00:00.000000 giant_redirect_import-0.2/PKG-INFO
```

### Comparing `giant-redirect-import-0.1.0/LICENSE` & `giant_redirect_import-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `giant-redirect-import-0.1.0/README.md` & `giant_redirect_import-0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 ## Installation
 
 To install with the package manager, run:
 
     $ poetry add giant-redirect-import
 
-You should then add `"giant-redirect-import"` to the `INSTALLED_APPS` in your settings file, this MUST be above `django.contrib.redirects`.
+You should then add `"giant_redirect_import"` to the `INSTALLED_APPS` in your settings file, this MUST be directly above `django.contrib.redirects`.
 
 In `base.py` there should also be a `REDIRECT_IMPORT_DEFAULT_SITE_ID`.
 
 
 ## Configuration
 
 This application exposes the following settings:
```

### Comparing `giant-redirect-import-0.1.0/giant_redirect_import/admin.py` & `giant_redirect_import-0.2/giant_redirect_import/admin.py`

 * *Files identical despite different names*

### Comparing `giant-redirect-import-0.1.0/giant_redirect_import/forms.py` & `giant_redirect_import-0.2/giant_redirect_import/forms.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from csv import DictReader
 from io import StringIO
 from urllib.parse import urlparse
 
 from django import forms
 from django.conf import settings
-from django.contrib.sites.models import Site
 from django.contrib.redirects.models import Redirect
-from django.utils.translation import ugettext
 
 
 class RedirectImportForm(forms.Form):
 
     """
     Form to handle csv file import from redirect admin.
     List the rows to be imported in the "rows" list
@@ -33,35 +31,42 @@
 
         if hasattr(settings, "REDIRECT_IMPORT_DEFAULT_SITE_ID"):
             site_id = settings.REDIRECT_IMPORT_DEFAULT_SITE_ID
 
         created, updated = 0, 0
 
         for row in csv_data:
-            old_slug = row["Original URL"]
-            new_slug = row["Redirect To"]
+            try:
+                old_slug = row["Original URL"]
+                new_slug = row["Redirect To"]
+            except:
+                return {
+                    "message": "Import failed. Check the spelling of your column names.",
+                    "error": True,
+                }
 
             # Will catch urls with no schema, such as 'example.com/career/'
             if schema not in new_slug:
                 new_slug = schema + new_slug
 
-            # Ensuring new path ends with a trailing slash
+            # Ensuring paths end with a trailing slash
             if not new_slug.endswith("/"):
                 new_slug += "/"
 
+            if not old_slug.endswith("/"):
+                old_slug += "/"
+
             _, status = Redirect.objects.update_or_create(
                 site_id=site_id,
                 old_path=old_slug,
                 defaults={"new_path": urlparse(new_slug).path},
             )
             if status:
                 created += 1
             else:
                 updated += 1
-        message = ugettext(
-            "{created} new redirects were imported, {updated} redirects were updated."
-        ).format(created=created, updated=updated)
+        message = f"{created} new redirects were imported, {updated} redirects were updated."
 
         return {
             "message": message,
             "error": False,
         }
```

### Comparing `giant-redirect-import-0.1.0/giant_redirect_import/tests/test_forms.py` & `giant_redirect_import-0.2/giant_redirect_import/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `giant-redirect-import-0.1.0/pyproject.toml` & `giant_redirect_import-0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "giant-redirect-import"
-version = "0.1.0"
+version = "0.2"
 description = "Reusable package which adds an option to bulk import redirects from a csv file"
 authors = ["Will-Hoey <will.hoey@hotmail.co.uk>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/giantmade/giant-redirect-import"
 repository = "https://github.com/giantmade/giant-redirect-import"
 keywords = ["import", "app"]
```

### Comparing `giant-redirect-import-0.1.0/PKG-INFO` & `giant_redirect_import-0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: giant-redirect-import
-Version: 0.1.0
+Version: 0.2
 Summary: Reusable package which adds an option to bulk import redirects from a csv file
 Home-page: https://github.com/giantmade/giant-redirect-import
 License: MIT
 Keywords: import,app
 Author: Will-Hoey
 Author-email: will.hoey@hotmail.co.uk
 Requires-Python: >=3.6,<4.0
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Project-URL: Repository, https://github.com/giantmade/giant-redirect-import
 Description-Content-Type: text/markdown
 
 # Giant Redirect Import
 
@@ -28,15 +31,15 @@
 
 ## Installation
 
 To install with the package manager, run:
 
     $ poetry add giant-redirect-import
 
-You should then add `"giant-redirect-import"` to the `INSTALLED_APPS` in your settings file, this MUST be above `django.contrib.redirects`.
+You should then add `"giant_redirect_import"` to the `INSTALLED_APPS` in your settings file, this MUST be directly above `django.contrib.redirects`.
 
 In `base.py` there should also be a `REDIRECT_IMPORT_DEFAULT_SITE_ID`.
 
 
 ## Configuration
 
 This application exposes the following settings:
```

