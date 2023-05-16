# Comparing `tmp/mkdocs_exporter-1.2.1.tar.gz` & `tmp/mkdocs_exporter-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_exporter-1.2.1.tar", max compression
+gzip compressed data, was "mkdocs_exporter-1.2.2.tar", max compression
```

## Comparing `mkdocs_exporter-1.2.1.tar` & `mkdocs_exporter-1.2.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1071 2023-05-08 13:15:16.904792 mkdocs_exporter-1.2.1/LICENSE
--rw-r--r--   0        0        0     3066 2023-05-11 19:49:17.381184 mkdocs_exporter-1.2.1/README.md
--rw-r--r--   0        0        0        0 2023-05-08 15:45:32.453553 mkdocs_exporter-1.2.1/mkdocs_exporter/__init__.py
--rw-r--r--   0        0        0     1899 2023-05-09 17:07:37.227188 mkdocs_exporter-1.2.1/mkdocs_exporter/browser.py
--rw-r--r--   0        0        0       96 2023-05-08 19:25:05.801769 mkdocs_exporter-1.2.1/mkdocs_exporter/logging.py
--rw-r--r--   0        0        0      440 2023-05-08 15:32:49.823552 mkdocs_exporter-1.2.1/mkdocs_exporter/page.py
--rw-r--r--   0        0        0      705 2023-05-08 15:33:10.113552 mkdocs_exporter-1.2.1/mkdocs_exporter/plugin.py
--rw-r--r--   0        0        0        0 2023-05-06 21:44:34.488343 mkdocs_exporter-1.2.1/mkdocs_exporter/plugins/__init__.py
--rw-r--r--   0        0        0        0 2023-05-07 17:00:48.574613 mkdocs_exporter-1.2.1/mkdocs_exporter/plugins/extras/__init__.py
--rw-r--r--   0        0        0      977 2023-05-09 09:27:33.387117 mkdocs_exporter-1.2.1/mkdocs_exporter/plugins/extras/config.py
--rw-r--r--   0        0        0      812 2023-05-09 17:07:37.227188 mkdocs_exporter-1.2.1/mkdocs_exporter/plugins/extras/plugin.py
--rw-r--r--   0        0        0        0 2023-05-07 17:48:51.834620 mkdocs_exporter-1.2.1/mkdocs_exporter/plugins/pdf/__init__.py
--rw-r--r--   0        0        0      731 2023-05-09 09:13:25.647118 mkdocs_exporter-1.2.1/mkdocs_exporter/plugins/pdf/button.py
--rw-r--r--   0        0        0     1120 2023-05-11 19:49:17.381184 mkdocs_exporter-1.2.1/mkdocs_exporter/plugins/pdf/config.py
--rw-r--r--   0        0        0     4482 2023-05-12 07:42:49.273785 mkdocs_exporter-1.2.1/mkdocs_exporter/plugins/pdf/plugin.py
--rw-r--r--   0        0        0     2330 2023-05-09 11:31:09.967140 mkdocs_exporter-1.2.1/mkdocs_exporter/plugins/pdf/renderer.py
--rw-r--r--   0        0        0     4080 2023-05-09 18:59:51.747207 mkdocs_exporter-1.2.1/mkdocs_exporter/preprocessor.py
--rw-r--r--   0        0        0      241 2023-05-07 12:23:00.605366 mkdocs_exporter-1.2.1/mkdocs_exporter/renderer.py
--rw-r--r--   0        0        0        0 2023-05-08 14:16:51.163540 mkdocs_exporter-1.2.1/mkdocs_exporter/resources/__init__.py
--rw-r--r--   0        0        0        0 2023-05-08 14:16:39.063540 mkdocs_exporter-1.2.1/mkdocs_exporter/resources/js/__init__.py
--rw-r--r--   0        0        0   499714 2023-05-08 14:10:56.413538 mkdocs_exporter-1.2.1/mkdocs_exporter/resources/js/pagedjs.min.js
--rw-r--r--   0        0        0     1525 2023-05-12 07:42:57.293783 mkdocs_exporter-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     4426 1970-01-01 00:00:00.000000 mkdocs_exporter-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-09 09:23:22.592488 mkdocs_exporter-1.2.2/LICENSE
+-rw-r--r--   0        0        0     3066 2023-05-10 11:42:02.282235 mkdocs_exporter-1.2.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-09 09:23:22.592488 mkdocs_exporter-1.2.2/mkdocs_exporter/__init__.py
+-rw-r--r--   0        0        0     1899 2023-05-09 15:43:28.836677 mkdocs_exporter-1.2.2/mkdocs_exporter/browser.py
+-rw-r--r--   0        0        0       96 2023-05-09 09:23:22.592488 mkdocs_exporter-1.2.2/mkdocs_exporter/logging.py
+-rw-r--r--   0        0        0      440 2023-05-09 09:23:22.592488 mkdocs_exporter-1.2.2/mkdocs_exporter/page.py
+-rw-r--r--   0        0        0      705 2023-05-09 17:06:53.963165 mkdocs_exporter-1.2.2/mkdocs_exporter/plugin.py
+-rw-r--r--   0        0        0        0 2023-05-09 09:23:22.592488 mkdocs_exporter-1.2.2/mkdocs_exporter/plugins/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-09 09:23:22.592488 mkdocs_exporter-1.2.2/mkdocs_exporter/plugins/extras/__init__.py
+-rw-r--r--   0        0        0      977 2023-05-09 09:28:39.475500 mkdocs_exporter-1.2.2/mkdocs_exporter/plugins/extras/config.py
+-rw-r--r--   0        0        0      812 2023-05-09 11:28:30.480215 mkdocs_exporter-1.2.2/mkdocs_exporter/plugins/extras/plugin.py
+-rw-r--r--   0        0        0        0 2023-05-09 09:23:22.592488 mkdocs_exporter-1.2.2/mkdocs_exporter/plugins/pdf/__init__.py
+-rw-r--r--   0        0        0      731 2023-05-09 09:23:22.592488 mkdocs_exporter-1.2.2/mkdocs_exporter/plugins/pdf/button.py
+-rw-r--r--   0        0        0     1120 2023-05-12 06:29:50.585343 mkdocs_exporter-1.2.2/mkdocs_exporter/plugins/pdf/config.py
+-rw-r--r--   0        0        0     4477 2023-05-16 11:51:18.093013 mkdocs_exporter-1.2.2/mkdocs_exporter/plugins/pdf/plugin.py
+-rw-r--r--   0        0        0     2330 2023-05-09 10:49:37.916810 mkdocs_exporter-1.2.2/mkdocs_exporter/plugins/pdf/renderer.py
+-rw-r--r--   0        0        0     4080 2023-05-10 11:42:02.282235 mkdocs_exporter-1.2.2/mkdocs_exporter/preprocessor.py
+-rw-r--r--   0        0        0      241 2023-05-09 09:23:22.592488 mkdocs_exporter-1.2.2/mkdocs_exporter/renderer.py
+-rw-r--r--   0        0        0        0 2023-05-09 09:23:22.592488 mkdocs_exporter-1.2.2/mkdocs_exporter/resources/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-09 09:23:22.592488 mkdocs_exporter-1.2.2/mkdocs_exporter/resources/js/__init__.py
+-rw-r--r--   0        0        0   499714 2023-05-09 09:23:22.592488 mkdocs_exporter-1.2.2/mkdocs_exporter/resources/js/pagedjs.min.js
+-rw-r--r--   0        0        0     1525 2023-05-16 11:51:18.093013 mkdocs_exporter-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     4426 1970-01-01 00:00:00.000000 mkdocs_exporter-1.2.2/PKG-INFO
```

### Comparing `mkdocs_exporter-1.2.1/LICENSE` & `mkdocs_exporter-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-1.2.1/README.md` & `mkdocs_exporter-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-1.2.1/mkdocs_exporter/browser.py` & `mkdocs_exporter-1.2.2/mkdocs_exporter/browser.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-1.2.1/mkdocs_exporter/plugin.py` & `mkdocs_exporter-1.2.2/mkdocs_exporter/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-1.2.1/mkdocs_exporter/plugins/extras/config.py` & `mkdocs_exporter-1.2.2/mkdocs_exporter/plugins/extras/config.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-1.2.1/mkdocs_exporter/plugins/extras/plugin.py` & `mkdocs_exporter-1.2.2/mkdocs_exporter/plugins/extras/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-1.2.1/mkdocs_exporter/plugins/pdf/button.py` & `mkdocs_exporter-1.2.2/mkdocs_exporter/plugins/pdf/button.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-1.2.1/mkdocs_exporter/plugins/pdf/config.py` & `mkdocs_exporter-1.2.2/mkdocs_exporter/plugins/pdf/config.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-1.2.1/mkdocs_exporter/plugins/pdf/plugin.py` & `mkdocs_exporter-1.2.2/mkdocs_exporter/plugins/pdf/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
     return server
 
 
   def on_page_markdown(self, markdown: str, page: Page, config: Config, **kwargs) -> str:
     """Invoked when the page's markdown has been loaded."""
 
-    if not self._enabled(page) and 'covers' not in page.meta.get('hide', []):
+    if not self._enabled(page) or 'covers' in page.meta.get('hide', []):
       return
 
     content = markdown
     covers = {**self.config.covers, **{k: os.path.join(os.path.dirname(config['config_file_path']), v) for k, v in page.meta.get('covers', {}).items()}}
 
     if covers.get('front'):
       with open(covers['front'], 'r') as file:
```

### Comparing `mkdocs_exporter-1.2.1/mkdocs_exporter/plugins/pdf/renderer.py` & `mkdocs_exporter-1.2.2/mkdocs_exporter/plugins/pdf/renderer.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-1.2.1/mkdocs_exporter/preprocessor.py` & `mkdocs_exporter-1.2.2/mkdocs_exporter/preprocessor.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-1.2.1/mkdocs_exporter/resources/js/pagedjs.min.js` & `mkdocs_exporter-1.2.2/mkdocs_exporter/resources/js/pagedjs.min.js`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-1.2.1/pyproject.toml` & `mkdocs_exporter-1.2.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "mkdocs-exporter"
-version = "1.2.1"
+version = "1.2.2"
 repository = "https://github.com/adrienbrignon/mkdocs-exporter"
 keywords = ["mkdocs", "pdf", "exporter"]
 description = "A highly-configurable plugin for MkDocs that exports your pages to PDF files."
 authors = ["Adrien Brignon <adrien@brignon.dev>"]
 readme = "README.md"
 classifiers = [
   "License :: OSI Approved :: MIT License",
```

### Comparing `mkdocs_exporter-1.2.1/PKG-INFO` & `mkdocs_exporter-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-exporter
-Version: 1.2.1
+Version: 1.2.2
 Summary: A highly-configurable plugin for MkDocs that exports your pages to PDF files.
 Home-page: https://github.com/adrienbrignon/mkdocs-exporter
 Keywords: mkdocs,pdf,exporter
 Author: Adrien Brignon
 Author-email: adrien@brignon.dev
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
```

