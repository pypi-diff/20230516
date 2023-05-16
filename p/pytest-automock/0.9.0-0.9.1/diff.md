# Comparing `tmp/pytest-automock-0.9.0.tar.gz` & `tmp/pytest-automock-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-automock-0.9.0.tar", last modified: Thu Aug  4 02:39:50 2022, max compression
+gzip compressed data, was "pytest-automock-0.9.1.tar", last modified: Tue May 16 21:33:40 2023, max compression
```

## Comparing `pytest-automock-0.9.0.tar` & `pytest-automock-0.9.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-04 02:39:50.640639 pytest-automock-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)       83 2022-08-04 02:39:44.000000 pytest-automock-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     7558 2022-08-04 02:39:50.640639 pytest-automock-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7269 2022-08-04 02:39:44.000000 pytest-automock-0.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1279 2022-08-04 02:39:44.000000 pytest-automock-0.9.0/history.md
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-08-04 02:39:44.000000 pytest-automock-0.9.0/license.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-04 02:39:50.636639 pytest-automock-0.9.0/pytest_automock/
--rw-r--r--   0 runner    (1001) docker     (121)      109 2022-08-04 02:39:44.000000 pytest-automock-0.9.0/pytest_automock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7912 2022-08-04 02:39:44.000000 pytest-automock-0.9.0/pytest_automock/mock.py
--rw-r--r--   0 runner    (1001) docker     (121)     3127 2022-08-04 02:39:44.000000 pytest-automock-0.9.0/pytest_automock/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-04 02:39:50.640639 pytest-automock-0.9.0/pytest_automock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7558 2022-08-04 02:39:50.000000 pytest-automock-0.9.0/pytest_automock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      439 2022-08-04 02:39:50.000000 pytest-automock-0.9.0/pytest_automock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-04 02:39:50.000000 pytest-automock-0.9.0/pytest_automock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-08-04 02:39:50.000000 pytest-automock-0.9.0/pytest_automock.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-08-04 02:39:50.000000 pytest-automock-0.9.0/pytest_automock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-08-04 02:39:50.000000 pytest-automock-0.9.0/pytest_automock.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      518 2022-08-04 02:39:50.640639 pytest-automock-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-08-04 02:39:44.000000 pytest-automock-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-04 02:39:50.640639 pytest-automock-0.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-08-04 02:39:44.000000 pytest-automock-0.9.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     4717 2022-08-04 02:39:44.000000 pytest-automock-0.9.0/tests/test_automock.py
--rw-r--r--   0 runner    (1001) docker     (121)     2206 2022-08-04 02:39:44.000000 pytest-automock-0.9.0/tests/test_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:33:40.340360 pytest-automock-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-16 21:33:30.000000 pytest-automock-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7559 2023-05-16 21:33:40.340360 pytest-automock-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7270 2023-05-16 21:33:30.000000 pytest-automock-0.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-16 21:33:30.000000 pytest-automock-0.9.1/history.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-16 21:33:30.000000 pytest-automock-0.9.1/license.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:33:40.336360 pytest-automock-0.9.1/pytest_automock/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-16 21:33:30.000000 pytest-automock-0.9.1/pytest_automock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-05-16 21:33:30.000000 pytest-automock-0.9.1/pytest_automock/mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-05-16 21:33:30.000000 pytest-automock-0.9.1/pytest_automock/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:33:40.340360 pytest-automock-0.9.1/pytest_automock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7559 2023-05-16 21:33:40.000000 pytest-automock-0.9.1/pytest_automock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-16 21:33:40.000000 pytest-automock-0.9.1/pytest_automock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 21:33:40.000000 pytest-automock-0.9.1/pytest_automock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-16 21:33:40.000000 pytest-automock-0.9.1/pytest_automock.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-16 21:33:40.000000 pytest-automock-0.9.1/pytest_automock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-16 21:33:40.000000 pytest-automock-0.9.1/pytest_automock.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-16 21:33:40.340360 pytest-automock-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-16 21:33:30.000000 pytest-automock-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:33:40.340360 pytest-automock-0.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-16 21:33:30.000000 pytest-automock-0.9.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-05-16 21:33:30.000000 pytest-automock-0.9.1/tests/test_automock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-05-16 21:33:30.000000 pytest-automock-0.9.1/tests/test_plugin.py
```

### Comparing `pytest-automock-0.9.0/PKG-INFO` & `pytest-automock-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-automock
-Version: 0.9.0
+Version: 0.9.1
 Summary: Pytest plugin for automatical mocks creation
 Home-page: https://github.com/pohmelie/pytest-automock
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
@@ -21,15 +21,15 @@
 # Features
 * Pytest plugin
 * Autogenerate/autouse mocks for functions and objects
 * Sync and async support
 * Locked mode to be sure mocked objects stay untouched
 * Customizable serialization
 
-# Limitaions
+# Limitations
 * No support for dunder methods (can be partly solved in future)
 * No support for sync/async generators/contexts
 * Races can break tests, since order counts
 * Non-determenistic representation will break tests, since representation is a part of call snapshot key
 
 # License
 `pytest-automock` is offered under MIT license.
```

### Comparing `pytest-automock-0.9.0/README.md` & `pytest-automock-0.9.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # Features
 * Pytest plugin
 * Autogenerate/autouse mocks for functions and objects
 * Sync and async support
 * Locked mode to be sure mocked objects stay untouched
 * Customizable serialization
 
-# Limitaions
+# Limitations
 * No support for dunder methods (can be partly solved in future)
 * No support for sync/async generators/contexts
 * Races can break tests, since order counts
 * Non-determenistic representation will break tests, since representation is a part of call snapshot key
 
 # License
 `pytest-automock` is offered under MIT license.
```

### Comparing `pytest-automock-0.9.0/history.md` & `pytest-automock-0.9.1/history.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# 0.9.1 (2023-05-17)
+* add `mtime=0` to `gzip.compress` call for reproducible builds
+
 # 0.9.0 (2022-08-04)
 * use gzip to compress pickle artifacts
 
 # 0.8.0 (2022-02-02)
 * use common exception class `AutoMockException`
 
 # 0.7.0 (2020-04-22)
```

### Comparing `pytest-automock-0.9.0/license.txt` & `pytest-automock-0.9.1/license.txt`

 * *Files identical despite different names*

### Comparing `pytest-automock-0.9.0/pytest_automock/mock.py` & `pytest-automock-0.9.1/pytest_automock/mock.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 class _CallType(Enum):
     sync = "sync"
     async_ = "async"
 
 
 def default_encode(v: Any) -> bytes:
-    return gzip.compress(pickle.dumps(v))
+    return gzip.compress(pickle.dumps(v), mtime=0)
 
 
 def default_decode(b: bytes) -> Any:
     return pickle.loads(gzip.decompress(b))
 
 
 class Call:
```

### Comparing `pytest-automock-0.9.0/pytest_automock/plugin.py` & `pytest-automock-0.9.1/pytest_automock/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-automock-0.9.0/pytest_automock.egg-info/PKG-INFO` & `pytest-automock-0.9.1/pytest_automock.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-automock
-Version: 0.9.0
+Version: 0.9.1
 Summary: Pytest plugin for automatical mocks creation
 Home-page: https://github.com/pohmelie/pytest-automock
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
@@ -21,15 +21,15 @@
 # Features
 * Pytest plugin
 * Autogenerate/autouse mocks for functions and objects
 * Sync and async support
 * Locked mode to be sure mocked objects stay untouched
 * Customizable serialization
 
-# Limitaions
+# Limitations
 * No support for dunder methods (can be partly solved in future)
 * No support for sync/async generators/contexts
 * Races can break tests, since order counts
 * Non-determenistic representation will break tests, since representation is a part of call snapshot key
 
 # License
 `pytest-automock` is offered under MIT license.
```

### Comparing `pytest-automock-0.9.0/setup.cfg` & `pytest-automock-0.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pytest-automock-0.9.0/tests/test_automock.py` & `pytest-automock-0.9.1/tests/test_automock.py`

 * *Files identical despite different names*

### Comparing `pytest-automock-0.9.0/tests/test_plugin.py` & `pytest-automock-0.9.1/tests/test_plugin.py`

 * *Files identical despite different names*

