# Comparing `tmp/prophecy-build-tool-test-1.0.7.tar.gz` & `tmp/prophecy-build-tool-test-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prophecy-build-tool-test-1.0.7.tar", last modified: Tue May 16 05:41:00 2023, max compression
+gzip compressed data, was "prophecy-build-tool-test-1.0.8.tar", last modified: Tue May 16 07:14:33 2023, max compression
```

## Comparing `prophecy-build-tool-test-1.0.7.tar` & `prophecy-build-tool-test-1.0.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 ankitashukla   (501) staff       (20)        0 2023-05-16 05:41:00.694392 prophecy-build-tool-test-1.0.7/
--rw-r--r--   0 ankitashukla   (501) staff       (20)    11357 2023-05-09 12:32:13.000000 prophecy-build-tool-test-1.0.7/LICENSE
--rw-r--r--   0 ankitashukla   (501) staff       (20)     5944 2023-05-16 05:41:00.694565 prophecy-build-tool-test-1.0.7/PKG-INFO
--rw-r--r--   0 ankitashukla   (501) staff       (20)     5318 2023-05-09 12:32:13.000000 prophecy-build-tool-test-1.0.7/README.md
--rw-r--r--   0 ankitashukla   (501) staff       (20)      419 2023-05-09 12:32:13.000000 prophecy-build-tool-test-1.0.7/pyproject.toml
--rw-r--r--   0 ankitashukla   (501) staff       (20)      239 2023-05-16 05:41:00.701290 prophecy-build-tool-test-1.0.7/setup.cfg
--rw-r--r--   0 ankitashukla   (501) staff       (20)     1185 2023-05-16 05:40:32.000000 prophecy-build-tool-test-1.0.7/setup.py
-drwxr-xr-x   0 ankitashukla   (501) staff       (20)        0 2023-05-16 05:41:00.664264 prophecy-build-tool-test-1.0.7/src/
-drwxr-xr-x   0 ankitashukla   (501) staff       (20)        0 2023-05-16 05:41:00.666320 prophecy-build-tool-test-1.0.7/src/pbt/
--rw-r--r--   0 ankitashukla   (501) staff       (20)     2654 2023-05-16 05:22:36.000000 prophecy-build-tool-test-1.0.7/src/pbt/__init__.py
--rw-r--r--   0 ankitashukla   (501) staff       (20)     1941 2023-05-09 12:32:13.000000 prophecy-build-tool-test-1.0.7/src/pbt/process.py
--rw-r--r--   0 ankitashukla   (501) staff       (20)    37485 2023-05-16 05:22:36.000000 prophecy-build-tool-test-1.0.7/src/pbt/prophecy_build_tool.py
-drwxr-xr-x   0 ankitashukla   (501) staff       (20)        0 2023-05-16 05:41:00.689873 prophecy-build-tool-test-1.0.7/src/prophecy_build_tool_test.egg-info/
--rw-r--r--   0 ankitashukla   (501) staff       (20)     5944 2023-05-16 05:41:00.000000 prophecy-build-tool-test-1.0.7/src/prophecy_build_tool_test.egg-info/PKG-INFO
--rw-r--r--   0 ankitashukla   (501) staff       (20)      474 2023-05-16 05:41:00.000000 prophecy-build-tool-test-1.0.7/src/prophecy_build_tool_test.egg-info/SOURCES.txt
--rw-r--r--   0 ankitashukla   (501) staff       (20)        1 2023-05-16 05:41:00.000000 prophecy-build-tool-test-1.0.7/src/prophecy_build_tool_test.egg-info/dependency_links.txt
--rw-r--r--   0 ankitashukla   (501) staff       (20)       33 2023-05-16 05:41:00.000000 prophecy-build-tool-test-1.0.7/src/prophecy_build_tool_test.egg-info/entry_points.txt
--rw-r--r--   0 ankitashukla   (501) staff       (20)       77 2023-05-16 05:41:00.000000 prophecy-build-tool-test-1.0.7/src/prophecy_build_tool_test.egg-info/requires.txt
--rw-r--r--   0 ankitashukla   (501) staff       (20)        4 2023-05-16 05:41:00.000000 prophecy-build-tool-test-1.0.7/src/prophecy_build_tool_test.egg-info/top_level.txt
-drwxr-xr-x   0 ankitashukla   (501) staff       (20)        0 2023-05-16 05:41:00.690382 prophecy-build-tool-test-1.0.7/test/
--rw-r--r--   0 ankitashukla   (501) staff       (20)     2186 2023-05-16 05:22:36.000000 prophecy-build-tool-test-1.0.7/test/test_build.py
--rw-r--r--   0 ankitashukla   (501) staff       (20)     7868 2023-05-16 05:22:36.000000 prophecy-build-tool-test-1.0.7/test/test_deploy.py
+drwxr-xr-x   0 ankitashukla   (501) staff       (20)        0 2023-05-16 07:14:33.494149 prophecy-build-tool-test-1.0.8/
+-rw-r--r--   0 ankitashukla   (501) staff       (20)    11357 2023-05-09 12:32:13.000000 prophecy-build-tool-test-1.0.8/LICENSE
+-rw-r--r--   0 ankitashukla   (501) staff       (20)     5944 2023-05-16 07:14:33.494214 prophecy-build-tool-test-1.0.8/PKG-INFO
+-rw-r--r--   0 ankitashukla   (501) staff       (20)     5318 2023-05-09 12:32:13.000000 prophecy-build-tool-test-1.0.8/README.md
+-rw-r--r--   0 ankitashukla   (501) staff       (20)      419 2023-05-09 12:32:13.000000 prophecy-build-tool-test-1.0.8/pyproject.toml
+-rw-r--r--   0 ankitashukla   (501) staff       (20)      239 2023-05-16 07:14:33.494468 prophecy-build-tool-test-1.0.8/setup.cfg
+-rw-r--r--   0 ankitashukla   (501) staff       (20)     1185 2023-05-16 07:14:27.000000 prophecy-build-tool-test-1.0.8/setup.py
+drwxr-xr-x   0 ankitashukla   (501) staff       (20)        0 2023-05-16 07:14:33.490277 prophecy-build-tool-test-1.0.8/src/
+drwxr-xr-x   0 ankitashukla   (501) staff       (20)        0 2023-05-16 07:14:33.492056 prophecy-build-tool-test-1.0.8/src/pbt/
+-rw-r--r--   0 ankitashukla   (501) staff       (20)     2659 2023-05-16 07:11:30.000000 prophecy-build-tool-test-1.0.8/src/pbt/__init__.py
+-rw-r--r--   0 ankitashukla   (501) staff       (20)     1941 2023-05-09 12:32:13.000000 prophecy-build-tool-test-1.0.8/src/pbt/process.py
+-rw-r--r--   0 ankitashukla   (501) staff       (20)    37485 2023-05-16 05:22:36.000000 prophecy-build-tool-test-1.0.8/src/pbt/prophecy_build_tool.py
+drwxr-xr-x   0 ankitashukla   (501) staff       (20)        0 2023-05-16 07:14:33.493487 prophecy-build-tool-test-1.0.8/src/prophecy_build_tool_test.egg-info/
+-rw-r--r--   0 ankitashukla   (501) staff       (20)     5944 2023-05-16 07:14:33.000000 prophecy-build-tool-test-1.0.8/src/prophecy_build_tool_test.egg-info/PKG-INFO
+-rw-r--r--   0 ankitashukla   (501) staff       (20)      474 2023-05-16 07:14:33.000000 prophecy-build-tool-test-1.0.8/src/prophecy_build_tool_test.egg-info/SOURCES.txt
+-rw-r--r--   0 ankitashukla   (501) staff       (20)        1 2023-05-16 07:14:33.000000 prophecy-build-tool-test-1.0.8/src/prophecy_build_tool_test.egg-info/dependency_links.txt
+-rw-r--r--   0 ankitashukla   (501) staff       (20)       33 2023-05-16 07:14:33.000000 prophecy-build-tool-test-1.0.8/src/prophecy_build_tool_test.egg-info/entry_points.txt
+-rw-r--r--   0 ankitashukla   (501) staff       (20)       77 2023-05-16 07:14:33.000000 prophecy-build-tool-test-1.0.8/src/prophecy_build_tool_test.egg-info/requires.txt
+-rw-r--r--   0 ankitashukla   (501) staff       (20)        4 2023-05-16 07:14:33.000000 prophecy-build-tool-test-1.0.8/src/prophecy_build_tool_test.egg-info/top_level.txt
+drwxr-xr-x   0 ankitashukla   (501) staff       (20)        0 2023-05-16 07:14:33.493855 prophecy-build-tool-test-1.0.8/test/
+-rw-r--r--   0 ankitashukla   (501) staff       (20)     2186 2023-05-16 05:22:36.000000 prophecy-build-tool-test-1.0.8/test/test_build.py
+-rw-r--r--   0 ankitashukla   (501) staff       (20)     7868 2023-05-16 05:22:36.000000 prophecy-build-tool-test-1.0.8/test/test_deploy.py
```

### Comparing `prophecy-build-tool-test-1.0.7/LICENSE` & `prophecy-build-tool-test-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `prophecy-build-tool-test-1.0.7/PKG-INFO` & `prophecy-build-tool-test-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prophecy-build-tool-test
-Version: 1.0.7
+Version: 1.0.8
 Summary: Prophecy-build-tool (PBT) provides utilities to build and distribute projects created from the Prophecy IDE.
 Home-page: https://github.com/SimpleDataLabsInc/prophecy-build-tool
 Author: Prophecy
 Author-email: maciej@prophecy.io
 Project-URL: Bug Tracker, https://github.com/SimpleDataLabsInc/prophecy-build-tool/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `prophecy-build-tool-test-1.0.7/README.md` & `prophecy-build-tool-test-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `prophecy-build-tool-test-1.0.7/setup.py` & `prophecy-build-tool-test-1.0.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as _in:
     long_description = _in.read()
 
 setuptools.setup(
     name="prophecy-build-tool-test",
-    version="1.0.7",
+    version="1.0.8",
     author="Prophecy",
     author_email="maciej@prophecy.io",
     description="Prophecy-build-tool (PBT) provides utilities to build and distribute projects created from the "
     "Prophecy IDE.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/SimpleDataLabsInc/prophecy-build-tool",
```

### Comparing `prophecy-build-tool-test-1.0.7/src/pbt/__init__.py` & `prophecy-build-tool-test-1.0.8/src/pbt/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -102,10 +102,10 @@
     pbt = ProphecyBuildTool(path)
     pbt.test(driver_library_path)
 
 
 if __name__ == "pbt":
     print(
         f"[bold purple]Prophecy-build-tool[/bold purple] [bold black]"
-        f"v{pkg_resources.require('prophecy-build-tool')[0].version}[/bold black]\n"
+        f"v{pkg_resources.require('prophecy-build-tool-test')[0].version}[/bold black]\n"
     )
     cli()
```

### Comparing `prophecy-build-tool-test-1.0.7/src/pbt/process.py` & `prophecy-build-tool-test-1.0.8/src/pbt/process.py`

 * *Files identical despite different names*

### Comparing `prophecy-build-tool-test-1.0.7/src/pbt/prophecy_build_tool.py` & `prophecy-build-tool-test-1.0.8/src/pbt/prophecy_build_tool.py`

 * *Files identical despite different names*

### Comparing `prophecy-build-tool-test-1.0.7/src/prophecy_build_tool_test.egg-info/PKG-INFO` & `prophecy-build-tool-test-1.0.8/src/prophecy_build_tool_test.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prophecy-build-tool-test
-Version: 1.0.7
+Version: 1.0.8
 Summary: Prophecy-build-tool (PBT) provides utilities to build and distribute projects created from the Prophecy IDE.
 Home-page: https://github.com/SimpleDataLabsInc/prophecy-build-tool
 Author: Prophecy
 Author-email: maciej@prophecy.io
 Project-URL: Bug Tracker, https://github.com/SimpleDataLabsInc/prophecy-build-tool/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `prophecy-build-tool-test-1.0.7/test/test_build.py` & `prophecy-build-tool-test-1.0.8/test/test_build.py`

 * *Files identical despite different names*

### Comparing `prophecy-build-tool-test-1.0.7/test/test_deploy.py` & `prophecy-build-tool-test-1.0.8/test/test_deploy.py`

 * *Files identical despite different names*

