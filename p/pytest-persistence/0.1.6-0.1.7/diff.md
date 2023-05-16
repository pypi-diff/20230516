# Comparing `tmp/pytest-persistence-0.1.6.tar.gz` & `tmp/pytest-persistence-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-persistence-0.1.6.tar", last modified: Tue Mar 28 20:17:13 2023, max compression
+gzip compressed data, was "pytest-persistence-0.1.7.tar", last modified: Tue May 16 11:16:38 2023, max compression
```

## Comparing `pytest-persistence-0.1.6.tar` & `pytest-persistence-0.1.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 jaurban   (1000) jaurban   (1000)        0 2023-03-28 20:17:13.082402 pytest-persistence-0.1.6/
--rw-r--r--   0 jaurban   (1000) jaurban   (1000)     1077 2021-12-07 17:34:12.000000 pytest-persistence-0.1.6/LICENSE
--rw-r--r--   0 jaurban   (1000) jaurban   (1000)      835 2023-03-28 20:17:13.081402 pytest-persistence-0.1.6/PKG-INFO
--rw-r--r--   0 jaurban   (1000) jaurban   (1000)      372 2021-12-07 17:34:12.000000 pytest-persistence-0.1.6/README.md
-drwxr-xr-x   0 jaurban   (1000) jaurban   (1000)        0 2023-03-28 20:17:13.080402 pytest-persistence-0.1.6/pytest_persistence/
--rw-r--r--   0 jaurban   (1000) jaurban   (1000)     1428 2023-03-28 16:41:44.000000 pytest-persistence-0.1.6/pytest_persistence/XDistScheduling.py
--rw-r--r--   0 jaurban   (1000) jaurban   (1000)       22 2023-03-28 20:12:05.000000 pytest-persistence-0.1.6/pytest_persistence/__init__.py
--rw-r--r--   0 jaurban   (1000) jaurban   (1000)     6339 2023-03-28 15:49:52.000000 pytest-persistence-0.1.6/pytest_persistence/plugin.py
-drwxr-xr-x   0 jaurban   (1000) jaurban   (1000)        0 2023-03-28 20:17:13.081402 pytest-persistence-0.1.6/pytest_persistence.egg-info/
--rw-r--r--   0 jaurban   (1000) jaurban   (1000)      835 2023-03-28 20:17:13.000000 pytest-persistence-0.1.6/pytest_persistence.egg-info/PKG-INFO
--rw-r--r--   0 jaurban   (1000) jaurban   (1000)      396 2023-03-28 20:17:13.000000 pytest-persistence-0.1.6/pytest_persistence.egg-info/SOURCES.txt
--rw-r--r--   0 jaurban   (1000) jaurban   (1000)        1 2023-03-28 20:17:13.000000 pytest-persistence-0.1.6/pytest_persistence.egg-info/dependency_links.txt
--rw-r--r--   0 jaurban   (1000) jaurban   (1000)       51 2023-03-28 20:17:13.000000 pytest-persistence-0.1.6/pytest_persistence.egg-info/entry_points.txt
--rw-r--r--   0 jaurban   (1000) jaurban   (1000)       19 2023-03-28 20:17:13.000000 pytest-persistence-0.1.6/pytest_persistence.egg-info/top_level.txt
--rw-r--r--   0 jaurban   (1000) jaurban   (1000)       38 2023-03-28 20:17:13.082402 pytest-persistence-0.1.6/setup.cfg
--rw-r--r--   0 jaurban   (1000) jaurban   (1000)      969 2021-12-07 17:34:12.000000 pytest-persistence-0.1.6/setup.py
-drwxr-xr-x   0 jaurban   (1000) jaurban   (1000)        0 2023-03-28 20:17:13.081402 pytest-persistence-0.1.6/tests/
--rw-r--r--   0 jaurban   (1000) jaurban   (1000)      111 2022-03-14 13:20:28.000000 pytest-persistence-0.1.6/tests/test_mock.py
--rw-r--r--   0 jaurban   (1000) jaurban   (1000)     1980 2022-06-27 12:07:26.000000 pytest-persistence-0.1.6/tests/test_plugin.py
--rw-r--r--   0 jaurban   (1000) jaurban   (1000)     1367 2022-06-27 12:28:20.000000 pytest-persistence-0.1.6/tests/test_unit.py
+drwxr-xr-x   0 jaurban   (1000) jaurban   (1000)        0 2023-05-16 11:16:38.813660 pytest-persistence-0.1.7/
+-rw-r--r--   0 jaurban   (1000) jaurban   (1000)     1077 2021-12-07 17:34:12.000000 pytest-persistence-0.1.7/LICENSE
+-rw-r--r--   0 jaurban   (1000) jaurban   (1000)      835 2023-05-16 11:16:38.813660 pytest-persistence-0.1.7/PKG-INFO
+-rw-r--r--   0 jaurban   (1000) jaurban   (1000)      372 2021-12-07 17:34:12.000000 pytest-persistence-0.1.7/README.md
+drwxr-xr-x   0 jaurban   (1000) jaurban   (1000)        0 2023-05-16 11:16:38.812660 pytest-persistence-0.1.7/pytest_persistence/
+-rw-r--r--   0 jaurban   (1000) jaurban   (1000)     1428 2023-03-28 16:41:44.000000 pytest-persistence-0.1.7/pytest_persistence/XDistScheduling.py
+-rw-r--r--   0 jaurban   (1000) jaurban   (1000)       22 2023-05-16 11:15:44.000000 pytest-persistence-0.1.7/pytest_persistence/__init__.py
+-rw-r--r--   0 jaurban   (1000) jaurban   (1000)     6547 2023-05-16 10:48:26.000000 pytest-persistence-0.1.7/pytest_persistence/plugin.py
+drwxr-xr-x   0 jaurban   (1000) jaurban   (1000)        0 2023-05-16 11:16:38.812660 pytest-persistence-0.1.7/pytest_persistence.egg-info/
+-rw-r--r--   0 jaurban   (1000) jaurban   (1000)      835 2023-05-16 11:16:38.000000 pytest-persistence-0.1.7/pytest_persistence.egg-info/PKG-INFO
+-rw-r--r--   0 jaurban   (1000) jaurban   (1000)      396 2023-05-16 11:16:38.000000 pytest-persistence-0.1.7/pytest_persistence.egg-info/SOURCES.txt
+-rw-r--r--   0 jaurban   (1000) jaurban   (1000)        1 2023-05-16 11:16:38.000000 pytest-persistence-0.1.7/pytest_persistence.egg-info/dependency_links.txt
+-rw-r--r--   0 jaurban   (1000) jaurban   (1000)       51 2023-05-16 11:16:38.000000 pytest-persistence-0.1.7/pytest_persistence.egg-info/entry_points.txt
+-rw-r--r--   0 jaurban   (1000) jaurban   (1000)       19 2023-05-16 11:16:38.000000 pytest-persistence-0.1.7/pytest_persistence.egg-info/top_level.txt
+-rw-r--r--   0 jaurban   (1000) jaurban   (1000)       38 2023-05-16 11:16:38.813660 pytest-persistence-0.1.7/setup.cfg
+-rw-r--r--   0 jaurban   (1000) jaurban   (1000)      969 2021-12-07 17:34:12.000000 pytest-persistence-0.1.7/setup.py
+drwxr-xr-x   0 jaurban   (1000) jaurban   (1000)        0 2023-05-16 11:16:38.813660 pytest-persistence-0.1.7/tests/
+-rw-r--r--   0 jaurban   (1000) jaurban   (1000)      111 2023-05-16 08:13:42.000000 pytest-persistence-0.1.7/tests/test_mock.py
+-rw-r--r--   0 jaurban   (1000) jaurban   (1000)     1980 2022-06-27 12:07:26.000000 pytest-persistence-0.1.7/tests/test_plugin.py
+-rw-r--r--   0 jaurban   (1000) jaurban   (1000)     1367 2022-06-27 12:28:20.000000 pytest-persistence-0.1.7/tests/test_unit.py
```

### Comparing `pytest-persistence-0.1.6/LICENSE` & `pytest-persistence-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-persistence-0.1.6/PKG-INFO` & `pytest-persistence-0.1.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-persistence
-Version: 0.1.6
+Version: 0.1.7
 Summary: Pytest tool for persistent objects
 Home-page: https://github.com/JaurbanRH/pytest-persistence
 Author: Jakub Urban
 Author-email: kubo.urban@gmail.com
 Maintainer: Jakub Urban
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pytest-persistence-0.1.6/pytest_persistence/XDistScheduling.py` & `pytest-persistence-0.1.7/pytest_persistence/XDistScheduling.py`

 * *Files identical despite different names*

### Comparing `pytest-persistence-0.1.6/pytest_persistence/plugin.py` & `pytest-persistence-0.1.7/pytest_persistence/plugin.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         "--load", action="store", default=False, help="Load config")
 
 
 class Plugin:
     """
     Pytest persistence plugin
     """
-    output = {"session": {}, "package": {}, "module": {}, "class": {}, "function": {}, "workers": {}}
+    output = {"session": {}, "package": {}, "module": {}, "class": {}, "function": {}, "workers": {}, "tests": {}}
     input = {}
     unable_to_pickle = set()
     pickled_fixtures = set()
 
     def pytest_sessionstart(self, session):
         """
         Called after the ``Session`` object has been created and before performing collection
@@ -152,17 +152,22 @@
                 self.output["workers"].update({node_id: worker_id})
                 self.store_fixture(result, fixture_id, node_id, worker_id)
             except Exception:
                 self.unable_to_pickle.add(fixture_id)
 
         return result
 
+    def pytest_runtest_setup(self, item):
+        worker_id = os.getenv("PYTEST_XDIST_WORKER")
+        node_id = item._pyfuncitem._nodeid
+        self.output["tests"].update({node_id: worker_id})
+
     @pytest.hookimpl(trylast=True)
     def pytest_xdist_make_scheduler(self, config, log):
-        if (test_order := self.input.get("workers")) is not None:
+        if (test_order := self.input.get("tests")) is not None:
             return XDistScheduling(config, log, test_order)
 
 
 def pytest_configure(config):
     """
     Hook ensures that plugin works only when the --load or --store option is present.
     """
```

### Comparing `pytest-persistence-0.1.6/pytest_persistence.egg-info/PKG-INFO` & `pytest-persistence-0.1.7/pytest_persistence.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-persistence
-Version: 0.1.6
+Version: 0.1.7
 Summary: Pytest tool for persistent objects
 Home-page: https://github.com/JaurbanRH/pytest-persistence
 Author: Jakub Urban
 Author-email: kubo.urban@gmail.com
 Maintainer: Jakub Urban
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pytest-persistence-0.1.6/setup.py` & `pytest-persistence-0.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `pytest-persistence-0.1.6/tests/test_plugin.py` & `pytest-persistence-0.1.7/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-persistence-0.1.6/tests/test_unit.py` & `pytest-persistence-0.1.7/tests/test_unit.py`

 * *Files identical despite different names*

