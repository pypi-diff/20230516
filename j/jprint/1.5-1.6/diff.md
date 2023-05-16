# Comparing `tmp/jprint-1.5.tar.gz` & `tmp/jprint-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jprint-1.5.tar", max compression
+gzip compressed data, was "jprint-1.6.tar", max compression
```

## Comparing `jprint-1.5.tar` & `jprint-1.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1449 2023-04-15 14:20:06.268592 jprint-1.5/README.md
--rw-r--r--   0        0        0       67 2023-04-15 13:54:50.797872 jprint-1.5/jprint/__init__.py
--rw-r--r--   0        0        0     1075 2023-05-11 11:07:57.035416 jprint-1.5/jprint/jprint.py
--rw-r--r--   0        0        0      694 2023-05-11 11:08:01.280693 jprint-1.5/pyproject.toml
--rw-r--r--   0        0        0     2226 1970-01-01 00:00:00.000000 jprint-1.5/PKG-INFO
+-rw-r--r--   0        0        0     1449 2023-04-15 14:20:06.268592 jprint-1.6/README.md
+-rw-r--r--   0        0        0       67 2023-04-15 13:54:50.797872 jprint-1.6/jprint/__init__.py
+-rw-r--r--   0        0        0     1092 2023-05-16 10:55:58.466463 jprint-1.6/jprint/jprint.py
+-rw-r--r--   0        0        0      694 2023-05-16 10:54:57.635700 jprint-1.6/pyproject.toml
+-rw-r--r--   0        0        0     2226 1970-01-01 00:00:00.000000 jprint-1.6/PKG-INFO
```

### Comparing `jprint-1.5/README.md` & `jprint-1.6/README.md`

 * *Files identical despite different names*

### Comparing `jprint-1.5/jprint/jprint.py` & `jprint-1.6/jprint/jprint.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,23 +14,23 @@
     """
     kwargs["indent"] = kwargs.get("indent", 4)
     kwargs["default"] = kwargs.get("default", str)
     kwargs["sort_keys"] = kwargs.get("sort_keys", True)
     return json.dumps(obj, **kwargs)
 
 
-def jprint(obj: Union[dict, list, tuple, str], **kwargs):
+def jprint(obj: Union[dict, list, tuple, set, str], **kwargs):
     """
     Pretty print Python dictionaries, lists, and JSON strings.
     If str is not valid json it will be printed as is.
     """
     if isinstance(obj, tuple):
         obj = list(obj)
 
-    if isinstance(obj, (dict, list)):
+    if isinstance(obj, (dict, list, tuple, set)):
         json_str = format(obj, **kwargs)
     else:
         try:
             json_str = format(json.loads(obj), **kwargs)
         except json.JSONDecodeError:
             json_str = format(obj, **kwargs)
```

### Comparing `jprint-1.5/pyproject.toml` & `jprint-1.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "jprint"
-version = "1.5"
+version = "1.6"
 authors = [ "John Furr <gnulnx@gmail.com>",]
 description = "A simple JSON and python dictionary pretty printer"
 readme = "README.md"
 license = "MIT"
 classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent",]
 
 [tool.poetry.dependencies]
```

### Comparing `jprint-1.5/PKG-INFO` & `jprint-1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jprint
-Version: 1.5
+Version: 1.6
 Summary: A simple JSON and python dictionary pretty printer
 License: MIT
 Author: John Furr
 Author-email: gnulnx@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

