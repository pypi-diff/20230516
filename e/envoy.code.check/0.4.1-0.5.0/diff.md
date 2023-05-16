# Comparing `tmp/envoy.code.check-0.4.1.tar.gz` & `tmp/envoy.code.check-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "envoy.code.check-0.4.1.tar", last modified: Sun Apr  9 17:23:52 2023, max compression
+gzip compressed data, was "envoy.code.check-0.5.0.tar", last modified: Tue May 16 14:33:12 2023, max compression
```

## Comparing `envoy.code.check-0.4.1.tar` & `envoy.code.check-0.5.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:23:52.621906 envoy.code.check-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-09 17:23:52.000000 envoy.code.check-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-09 17:23:52.621906 envoy.code.check-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-09 17:23:52.000000 envoy.code.check-0.4.1/backend_shim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:23:52.617906 envoy.code.check-0.4.1/envoy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:23:52.617906 envoy.code.check-0.4.1/envoy/code/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:23:52.617906 envoy.code.check-0.4.1/envoy/code/check/
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-04-09 17:23:52.000000 envoy.code.check-0.4.1/envoy/code/check/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:23:52.621906 envoy.code.check-0.4.1/envoy/code/check/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-04-09 17:23:52.000000 envoy.code.check-0.4.1/envoy/code/check/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-04-09 17:23:52.000000 envoy.code.check-0.4.1/envoy/code/check/abstract/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-04-09 17:23:52.000000 envoy.code.check-0.4.1/envoy/code/check/abstract/changelog.py
--rw-r--r--   0 runner    (1001) docker     (123)    14358 2023-04-09 17:23:52.000000 envoy.code.check-0.4.1/envoy/code/check/abstract/checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     9647 2023-04-09 17:23:52.000000 envoy.code.check-0.4.1/envoy/code/check/abstract/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7010 2023-04-09 17:23:52.000000 envoy.code.check-0.4.1/envoy/code/check/abstract/flake8.py
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-09 17:23:52.000000 envoy.code.check-0.4.1/envoy/code/check/abstract/glint.py
--rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-04-09 17:23:52.000000 envoy.code.check-0.4.1/envoy/code/check/abstract/gofmt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-09 17:23:52.000000 envoy.code.check-0.4.1/envoy/code/check/abstract/rst.py
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-04-09 17:23:52.000000 envoy.code.check-0.4.1/envoy/code/check/abstract/runtime_guards.py
--rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-04-09 17:23:52.000000 envoy.code.check-0.4.1/envoy/code/check/abstract/shellcheck.py
--rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-04-09 17:23:52.000000 envoy.code.check-0.4.1/envoy/code/check/abstract/yamllint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-04-09 17:23:52.000000 envoy.code.check-0.4.1/envoy/code/check/abstract/yapf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-04-09 17:23:52.000000 envoy.code.check-0.4.1/envoy/code/check/checker.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-09 17:23:52.000000 envoy.code.check-0.4.1/envoy/code/check/cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-09 17:23:52.000000 envoy.code.check-0.4.1/envoy/code/check/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-04-09 17:23:52.000000 envoy.code.check-0.4.1/envoy/code/check/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:23:52.000000 envoy.code.check-0.4.1/envoy/code/check/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-04-09 17:23:52.000000 envoy.code.check-0.4.1/envoy/code/check/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:23:52.617906 envoy.code.check-0.4.1/envoy.code.check.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-09 17:23:52.000000 envoy.code.check-0.4.1/envoy.code.check.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-09 17:23:52.000000 envoy.code.check-0.4.1/envoy.code.check.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 17:23:52.000000 envoy.code.check-0.4.1/envoy.code.check.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-09 17:23:52.000000 envoy.code.check-0.4.1/envoy.code.check.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 17:23:52.000000 envoy.code.check-0.4.1/envoy.code.check.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-09 17:23:52.000000 envoy.code.check-0.4.1/envoy.code.check.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-09 17:23:52.000000 envoy.code.check-0.4.1/envoy.code.check.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 17:23:52.621906 envoy.code.check-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-04-09 17:23:52.000000 envoy.code.check-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:33:12.174984 envoy.code.check-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-16 14:33:11.000000 envoy.code.check-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-16 14:33:12.174984 envoy.code.check-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-16 14:33:11.000000 envoy.code.check-0.5.0/backend_shim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:33:12.174984 envoy.code.check-0.5.0/envoy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:33:12.174984 envoy.code.check-0.5.0/envoy/code/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:33:12.174984 envoy.code.check-0.5.0/envoy/code/check/
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-16 14:33:11.000000 envoy.code.check-0.5.0/envoy/code/check/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:33:12.174984 envoy.code.check-0.5.0/envoy/code/check/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-05-16 14:33:11.000000 envoy.code.check-0.5.0/envoy/code/check/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-16 14:33:11.000000 envoy.code.check-0.5.0/envoy/code/check/abstract/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-05-16 14:33:11.000000 envoy.code.check-0.5.0/envoy/code/check/abstract/changelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14358 2023-05-16 14:33:11.000000 envoy.code.check-0.5.0/envoy/code/check/abstract/checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9640 2023-05-16 14:33:11.000000 envoy.code.check-0.5.0/envoy/code/check/abstract/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7010 2023-05-16 14:33:11.000000 envoy.code.check-0.5.0/envoy/code/check/abstract/flake8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-16 14:33:11.000000 envoy.code.check-0.5.0/envoy/code/check/abstract/glint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-05-16 14:33:11.000000 envoy.code.check-0.5.0/envoy/code/check/abstract/gofmt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-16 14:33:11.000000 envoy.code.check-0.5.0/envoy/code/check/abstract/rst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-05-16 14:33:11.000000 envoy.code.check-0.5.0/envoy/code/check/abstract/runtime_guards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-05-16 14:33:11.000000 envoy.code.check-0.5.0/envoy/code/check/abstract/shellcheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-05-16 14:33:11.000000 envoy.code.check-0.5.0/envoy/code/check/abstract/yamllint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-05-16 14:33:11.000000 envoy.code.check-0.5.0/envoy/code/check/abstract/yapf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-05-16 14:33:11.000000 envoy.code.check-0.5.0/envoy/code/check/checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-16 14:33:11.000000 envoy.code.check-0.5.0/envoy/code/check/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-16 14:33:11.000000 envoy.code.check-0.5.0/envoy/code/check/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-05-16 14:33:11.000000 envoy.code.check-0.5.0/envoy/code/check/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 14:33:11.000000 envoy.code.check-0.5.0/envoy/code/check/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-16 14:33:11.000000 envoy.code.check-0.5.0/envoy/code/check/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:33:12.174984 envoy.code.check-0.5.0/envoy.code.check.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-16 14:33:12.000000 envoy.code.check-0.5.0/envoy.code.check.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-16 14:33:12.000000 envoy.code.check-0.5.0/envoy.code.check.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 14:33:12.000000 envoy.code.check-0.5.0/envoy.code.check.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-16 14:33:12.000000 envoy.code.check-0.5.0/envoy.code.check.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 14:33:12.000000 envoy.code.check-0.5.0/envoy.code.check.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-16 14:33:12.000000 envoy.code.check-0.5.0/envoy.code.check.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-16 14:33:12.000000 envoy.code.check-0.5.0/envoy.code.check.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 14:33:12.174984 envoy.code.check-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-16 14:33:11.000000 envoy.code.check-0.5.0/setup.py
```

### Comparing `envoy.code.check-0.4.1/backend_shim.py` & `envoy.code.check-0.5.0/backend_shim.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.4.1/envoy/code/check/__init__.py` & `envoy.code.check-0.5.0/envoy/code/check/__init__.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.4.1/envoy/code/check/abstract/__init__.py` & `envoy.code.check-0.5.0/envoy/code/check/abstract/__init__.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.4.1/envoy/code/check/abstract/base.py` & `envoy.code.check-0.5.0/envoy/code/check/abstract/base.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.4.1/envoy/code/check/abstract/changelog.py` & `envoy.code.check-0.5.0/envoy/code/check/abstract/changelog.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.4.1/envoy/code/check/abstract/checker.py` & `envoy.code.check-0.5.0/envoy/code/check/abstract/checker.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.4.1/envoy/code/check/abstract/extensions.py` & `envoy.code.check-0.5.0/envoy/code/check/abstract/extensions.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 
 from envoy.code.check import abstract, exceptions, interface, typing
 
 
 logger = logging.getLogger(__name__)
 
 
-FILTER_NAMES_PATTERN = "NetworkFilterNames::get()"
+FILTER_NAMES_PATTERN = "envoy\\.filters\\.network"
 FUZZ_TEST_PATH = (
-    "test/extensions/filters/network/common/fuzz/uber_per_readfilter.cc")
+    "test/extensions/filters/network/common/fuzz/BUILD")
 METADATA_PATH = "source/extensions/extensions_metadata.yaml"
 METADATA_ONLY_EXTENSIONS = (
     "envoy.filters.network.envoy_mobile_http_connection_manager", )
 CONTRIB_METADATA_PATH = "contrib/extensions_metadata.yaml"
 EXTENSIONS_SCHEMA = "tools/extensions/extensions_schema.yaml"
 
 
@@ -104,19 +104,19 @@
 
     @property
     def fuzz_test_path(self) -> pathlib.Path:
         return self.directory.path.joinpath(FUZZ_TEST_PATH)
 
     @property
     def fuzzed_count(self) -> int:
-        # Hack-ish! We only search the first 50 lines to capture the filters
-        # in `filterNames()`.
+        # Hack-ish! We only search the first 60 lines to capture the filters
+        # in `READFILTER_FUZZ_FILTERS`.
         return len(
             self.fuzzed_filter_names_re.findall(
-                "".join(self.fuzz_test_path.read_text().splitlines()[:50])))
+                "".join(self.fuzz_test_path.read_text().splitlines()[:60])))
 
     @cached_property
     def fuzzed_filter_names_re(self) -> Pattern:
         return re.compile(FILTER_NAMES_PATTERN)
 
     @async_property(cache=True)
     async def metadata(self) -> typing.ExtensionsMetadataDict:
```

### Comparing `envoy.code.check-0.4.1/envoy/code/check/abstract/flake8.py` & `envoy.code.check-0.5.0/envoy/code/check/abstract/flake8.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.4.1/envoy/code/check/abstract/glint.py` & `envoy.code.check-0.5.0/envoy/code/check/abstract/glint.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.4.1/envoy/code/check/abstract/gofmt.py` & `envoy.code.check-0.5.0/envoy/code/check/abstract/gofmt.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.4.1/envoy/code/check/abstract/rst.py` & `envoy.code.check-0.5.0/envoy/code/check/abstract/rst.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.4.1/envoy/code/check/abstract/runtime_guards.py` & `envoy.code.check-0.5.0/envoy/code/check/abstract/runtime_guards.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.4.1/envoy/code/check/abstract/shellcheck.py` & `envoy.code.check-0.5.0/envoy/code/check/abstract/shellcheck.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.4.1/envoy/code/check/abstract/yamllint.py` & `envoy.code.check-0.5.0/envoy/code/check/abstract/yamllint.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.4.1/envoy/code/check/abstract/yapf.py` & `envoy.code.check-0.5.0/envoy/code/check/abstract/yapf.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.4.1/envoy/code/check/checker.py` & `envoy.code.check-0.5.0/envoy/code/check/checker.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.4.1/envoy/code/check/interface.py` & `envoy.code.check-0.5.0/envoy/code/check/interface.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.4.1/envoy/code/check/typing.py` & `envoy.code.check-0.5.0/envoy/code/check/typing.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.4.1/envoy.code.check.egg-info/SOURCES.txt` & `envoy.code.check-0.5.0/envoy.code.check.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.4.1/setup.py` & `envoy.code.check-0.5.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
             'envoy.code.check=envoy.code.check:run',
         ],
     },
     'install_requires': (
         'abstracts>=0.0.12',
         'aio.core>=0.10.0',
         'aio.run.checker>=0.5.7',
-        'envoy.base.utils>=0.4.1',
+        'envoy.base.utils>=0.4.7',
         'flake8>=6',
         'packaging>=23.0',
         'yamllint',
         'yapf',
     ),
     'license': 'Apache Software License 2.0',
     'long_description': """
@@ -41,10 +41,10 @@
         ),
     },
     'packages': (
         'envoy.code.check',
         'envoy.code.check.abstract',
     ),
     'python_requires': '>=3.10.0',
-    'url': 'https://github.com/envoyproxy/pytooling/tree/main/envoy.code.check',
-    'version': '0.4.1',
+    'url': 'https://github.com/envoyproxy/toolshed/tree/main/envoy.code.check',
+    'version': '0.5.0',
 })
```

