# Comparing `tmp/jschemator-0.0.5.tar.gz` & `tmp/jschemator-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jschemator-0.0.5.tar", last modified: Tue May 16 04:01:28 2023, max compression
+gzip compressed data, was "jschemator-0.0.6.tar", last modified: Tue May 16 12:16:24 2023, max compression
```

## Comparing `jschemator-0.0.5.tar` & `jschemator-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:01:28.020242 jschemator-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-16 04:01:17.000000 jschemator-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-16 04:01:28.020242 jschemator-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-16 04:01:17.000000 jschemator-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:01:28.016242 jschemator-0.0.5/jschemator/
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-16 04:01:17.000000 jschemator-0.0.5/jschemator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-05-16 04:01:17.000000 jschemator-0.0.5/jschemator/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:01:28.016242 jschemator-0.0.5/jschemator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-16 04:01:28.000000 jschemator-0.0.5/jschemator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-16 04:01:28.000000 jschemator-0.0.5/jschemator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 04:01:28.000000 jschemator-0.0.5/jschemator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-16 04:01:28.000000 jschemator-0.0.5/jschemator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-16 04:01:28.000000 jschemator-0.0.5/jschemator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 04:01:28.020242 jschemator-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-16 04:01:17.000000 jschemator-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:01:28.020242 jschemator-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-16 04:01:17.000000 jschemator-0.0.5/tests/test_compose.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-16 04:01:17.000000 jschemator-0.0.5/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-16 04:01:17.000000 jschemator-0.0.5/tests/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:16:24.729602 jschemator-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-16 12:16:03.000000 jschemator-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-16 12:16:24.729602 jschemator-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-16 12:16:03.000000 jschemator-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:16:24.725602 jschemator-0.0.6/jschemator/
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-16 12:16:03.000000 jschemator-0.0.6/jschemator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-05-16 12:16:03.000000 jschemator-0.0.6/jschemator/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:16:24.729602 jschemator-0.0.6/jschemator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-16 12:16:24.000000 jschemator-0.0.6/jschemator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-16 12:16:24.000000 jschemator-0.0.6/jschemator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 12:16:24.000000 jschemator-0.0.6/jschemator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-16 12:16:24.000000 jschemator-0.0.6/jschemator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-16 12:16:24.000000 jschemator-0.0.6/jschemator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 12:16:24.729602 jschemator-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-16 12:16:03.000000 jschemator-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:16:24.729602 jschemator-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-16 12:16:03.000000 jschemator-0.0.6/tests/test_compose.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-16 12:16:03.000000 jschemator-0.0.6/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-16 12:16:03.000000 jschemator-0.0.6/tests/test_schema.py
```

### Comparing `jschemator-0.0.5/LICENSE` & `jschemator-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `jschemator-0.0.5/jschemator/__init__.py` & `jschemator-0.0.6/jschemator/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,38 +3,35 @@
 
 
 class Schema:
     def __init__(self, *__args__, **kwargs):
         for key, value in kwargs.items():
             setattr(self, key, value)
 
-    def get_fields(self):
+    @classmethod
+    def get_fields(cls):
         fields = {}
-        for attribute_name, attribute_description in type(
-            self
-        ).__dict__.items():
+        for attribute_name, attribute_description in cls.__dict__.items():
             if not attribute_name.startswith("__") and isinstance(
                 attribute_description, BaseField
             ):
-                fields[attribute_name] = getattr(self, attribute_name)
+                fields[attribute_name] = getattr(cls, attribute_name)
         return fields
 
     def to_dict(self):
         return self.get_fields()
 
-    def json_schema(self, **kwargs):
+    @classmethod
+    def json_schema(cls, **kwargs):
         properties = {
-            schema_field: type(self)
-            .__dict__[schema_field]
-            .json_schema_render()
-            for schema_field in self.get_fields()
+            schema_field: cls.__dict__[schema_field].json_schema_render()
+            for schema_field in cls.get_fields()
         }
         kwargs.update(
             {
-                "$schema": "http://json-schema.org/draft-07/schema#",
                 "type": "object",
                 "properties": properties,
             }
         )
         return kwargs
 
     def __repr__(self):
```

### Comparing `jschemator-0.0.5/tests/test_schema.py` & `jschemator-0.0.6/tests/test_schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,14 @@
     b = Item(**{"name": "baz"})
     assert b.to_dict() == {"name": "baz"}
 
 
 def test_json_schema():
     e = Item(**{"name": "foo"})
     assert e.json_schema() == {
-        "$schema": "http://json-schema.org/draft-07/schema#",
         "type": "object",
         "properties": {"name": {"type": "string"}},
     }
 
 
 def test_repr():
     e = Item(**{"name": "foo"})
```

