# Comparing `tmp/jschemator-0.0.2.tar.gz` & `tmp/jschemator-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jschemator-0.0.2.tar", last modified: Mon May 15 06:40:38 2023, max compression
+gzip compressed data, was "jschemator-0.0.3.tar", last modified: Mon May 15 13:54:19 2023, max compression
```

## Comparing `jschemator-0.0.2.tar` & `jschemator-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 06:40:38.612392 jschemator-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-15 06:40:27.000000 jschemator-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-15 06:40:38.612392 jschemator-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-15 06:40:27.000000 jschemator-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 06:40:38.612392 jschemator-0.0.2/jschemator/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-15 06:40:27.000000 jschemator-0.0.2/jschemator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-05-15 06:40:27.000000 jschemator-0.0.2/jschemator/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 06:40:38.612392 jschemator-0.0.2/jschemator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-15 06:40:38.000000 jschemator-0.0.2/jschemator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-15 06:40:38.000000 jschemator-0.0.2/jschemator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 06:40:38.000000 jschemator-0.0.2/jschemator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-15 06:40:38.000000 jschemator-0.0.2/jschemator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-15 06:40:38.000000 jschemator-0.0.2/jschemator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 06:40:38.612392 jschemator-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-15 06:40:27.000000 jschemator-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 06:40:38.612392 jschemator-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-15 06:40:27.000000 jschemator-0.0.2/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-15 06:40:27.000000 jschemator-0.0.2/tests/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:54:19.306573 jschemator-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-15 13:54:07.000000 jschemator-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-15 13:54:19.306573 jschemator-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-15 13:54:07.000000 jschemator-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:54:19.302573 jschemator-0.0.3/jschemator/
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-15 13:54:07.000000 jschemator-0.0.3/jschemator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-05-15 13:54:07.000000 jschemator-0.0.3/jschemator/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:54:19.302573 jschemator-0.0.3/jschemator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-15 13:54:19.000000 jschemator-0.0.3/jschemator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-15 13:54:19.000000 jschemator-0.0.3/jschemator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 13:54:19.000000 jschemator-0.0.3/jschemator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-15 13:54:19.000000 jschemator-0.0.3/jschemator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-15 13:54:19.000000 jschemator-0.0.3/jschemator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 13:54:19.306573 jschemator-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-15 13:54:07.000000 jschemator-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:54:19.302573 jschemator-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-15 13:54:07.000000 jschemator-0.0.3/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-15 13:54:07.000000 jschemator-0.0.3/tests/test_schema.py
```

### Comparing `jschemator-0.0.2/LICENSE` & `jschemator-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jschemator-0.0.2/jschemator/__init__.py` & `jschemator-0.0.3/jschemator/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -26,17 +26,15 @@
     def json_schema(self):
         properties = {
             schema_field: type(self)
             .__dict__[schema_field]
             .json_schema_render()
             for schema_field in self.get_fields()
         }
-        return json.dumps(
-            {
-                "$schema": "http://json-schema.org/draft-07/schema#",
-                "type": "object",
-                "properties": properties,
-            }
-        )
+        return {
+            "$schema": "http://json-schema.org/draft-07/schema#",
+            "type": "object",
+            "properties": properties,
+        }
 
 
 __all__ = ["Schema"]
```

### Comparing `jschemator-0.0.2/jschemator/fields.py` & `jschemator-0.0.3/jschemator/fields.py`

 * *Files identical despite different names*

### Comparing `jschemator-0.0.2/tests/test_schema.py` & `jschemator-0.0.3/tests/test_schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,12 @@
 def test_to_dict():
     e = Item(**{"name": "foo"})
     assert e.to_dict() == {"name": "foo"}
 
 
 def test_json_schema():
     e = Item(**{"name": "foo"})
-    assert e.json_schema() == json.dumps(
-        {
-            "$schema": "http://json-schema.org/draft-07/schema#",
-            "type": "object",
-            "properties": {"name": {"type": "string"}},
-        }
-    )
+    assert e.json_schema() == {
+        "$schema": "http://json-schema.org/draft-07/schema#",
+        "type": "object",
+        "properties": {"name": {"type": "string"}},
+    }
```

