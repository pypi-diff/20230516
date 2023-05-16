# Comparing `tmp/jschemator-0.0.4.tar.gz` & `tmp/jschemator-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jschemator-0.0.4.tar", last modified: Tue May 16 00:56:26 2023, max compression
+gzip compressed data, was "jschemator-0.0.5.tar", last modified: Tue May 16 04:01:28 2023, max compression
```

## Comparing `jschemator-0.0.4.tar` & `jschemator-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:56:26.731200 jschemator-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-16 00:56:15.000000 jschemator-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-16 00:56:26.731200 jschemator-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-16 00:56:15.000000 jschemator-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:56:26.731200 jschemator-0.0.4/jschemator/
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-16 00:56:15.000000 jschemator-0.0.4/jschemator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-05-16 00:56:15.000000 jschemator-0.0.4/jschemator/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:56:26.731200 jschemator-0.0.4/jschemator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-16 00:56:26.000000 jschemator-0.0.4/jschemator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-16 00:56:26.000000 jschemator-0.0.4/jschemator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 00:56:26.000000 jschemator-0.0.4/jschemator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-16 00:56:26.000000 jschemator-0.0.4/jschemator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-16 00:56:26.000000 jschemator-0.0.4/jschemator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 00:56:26.731200 jschemator-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-16 00:56:15.000000 jschemator-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:56:26.731200 jschemator-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-16 00:56:15.000000 jschemator-0.0.4/tests/test_compose.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-16 00:56:15.000000 jschemator-0.0.4/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-16 00:56:15.000000 jschemator-0.0.4/tests/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:01:28.020242 jschemator-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-16 04:01:17.000000 jschemator-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-16 04:01:28.020242 jschemator-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-16 04:01:17.000000 jschemator-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:01:28.016242 jschemator-0.0.5/jschemator/
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-16 04:01:17.000000 jschemator-0.0.5/jschemator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-05-16 04:01:17.000000 jschemator-0.0.5/jschemator/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:01:28.016242 jschemator-0.0.5/jschemator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-16 04:01:28.000000 jschemator-0.0.5/jschemator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-16 04:01:28.000000 jschemator-0.0.5/jschemator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 04:01:28.000000 jschemator-0.0.5/jschemator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-16 04:01:28.000000 jschemator-0.0.5/jschemator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-16 04:01:28.000000 jschemator-0.0.5/jschemator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 04:01:28.020242 jschemator-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-16 04:01:17.000000 jschemator-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:01:28.020242 jschemator-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-16 04:01:17.000000 jschemator-0.0.5/tests/test_compose.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-16 04:01:17.000000 jschemator-0.0.5/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-16 04:01:17.000000 jschemator-0.0.5/tests/test_schema.py
```

### Comparing `jschemator-0.0.4/LICENSE` & `jschemator-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jschemator-0.0.4/jschemator/fields.py` & `jschemator-0.0.5/jschemator/fields.py`

 * *Files identical despite different names*

### Comparing `jschemator-0.0.4/tests/test_schema.py` & `jschemator-0.0.5/tests/test_schema.py`

 * *Files 27% similar despite different names*

```diff
@@ -19,18 +19,26 @@
 
 def test_from_dict():
     e = Item(**{"name": "foo"})
     assert e.name == "foo"
 
 
 def test_to_dict():
-    e = Item(**{"name": "foo"})
-    assert e.to_dict() == {"name": "foo"}
+    a = Item(**{"name": "foo"})
+    assert a.to_dict() == {"name": "foo"}
+
+    b = Item(**{"name": "baz"})
+    assert b.to_dict() == {"name": "baz"}
 
 
 def test_json_schema():
     e = Item(**{"name": "foo"})
     assert e.json_schema() == {
         "$schema": "http://json-schema.org/draft-07/schema#",
         "type": "object",
         "properties": {"name": {"type": "string"}},
     }
+
+
+def test_repr():
+    e = Item(**{"name": "foo"})
+    assert str(e) == '{"name": "foo"}'
```

