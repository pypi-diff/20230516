# Comparing `tmp/prophecy-build-tool-1.1.0.0.tar.gz` & `tmp/prophecy-build-tool-1.1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prophecy-build-tool-1.1.0.0.tar", last modified: Mon May 15 11:22:34 2023, max compression
+gzip compressed data, was "prophecy-build-tool-1.1.0.1.tar", last modified: Tue May 16 14:13:31 2023, max compression
```

## Comparing `prophecy-build-tool-1.1.0.0.tar` & `prophecy-build-tool-1.1.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 ashishpatel   (501) staff       (20)        0 2023-05-15 11:22:34.908846 prophecy-build-tool-1.1.0.0/
--rw-r--r--   0 ashishpatel   (501) staff       (20)    11357 2023-02-21 12:57:27.000000 prophecy-build-tool-1.1.0.0/LICENSE
--rw-r--r--   0 ashishpatel   (501) staff       (20)     5941 2023-05-15 11:22:34.908913 prophecy-build-tool-1.1.0.0/PKG-INFO
--rw-r--r--   0 ashishpatel   (501) staff       (20)     5318 2023-04-26 12:33:20.000000 prophecy-build-tool-1.1.0.0/README.md
--rw-r--r--   0 ashishpatel   (501) staff       (20)      419 2023-04-26 12:33:20.000000 prophecy-build-tool-1.1.0.0/pyproject.toml
--rw-r--r--   0 ashishpatel   (501) staff       (20)      239 2023-05-15 11:22:34.909161 prophecy-build-tool-1.1.0.0/setup.cfg
--rw-r--r--   0 ashishpatel   (501) staff       (20)     1182 2023-05-15 11:21:47.000000 prophecy-build-tool-1.1.0.0/setup.py
-drwxr-xr-x   0 ashishpatel   (501) staff       (20)        0 2023-05-15 11:22:34.905246 prophecy-build-tool-1.1.0.0/src/
-drwxr-xr-x   0 ashishpatel   (501) staff       (20)        0 2023-05-15 11:22:34.906833 prophecy-build-tool-1.1.0.0/src/pbt/
--rw-r--r--   0 ashishpatel   (501) staff       (20)     2471 2023-05-15 11:21:47.000000 prophecy-build-tool-1.1.0.0/src/pbt/__init__.py
--rw-r--r--   0 ashishpatel   (501) staff       (20)     1941 2023-04-26 12:33:20.000000 prophecy-build-tool-1.1.0.0/src/pbt/process.py
--rw-r--r--   0 ashishpatel   (501) staff       (20)    36939 2023-05-15 11:21:47.000000 prophecy-build-tool-1.1.0.0/src/pbt/prophecy_build_tool.py
-drwxr-xr-x   0 ashishpatel   (501) staff       (20)        0 2023-05-15 11:22:34.908221 prophecy-build-tool-1.1.0.0/src/prophecy_build_tool.egg-info/
--rw-r--r--   0 ashishpatel   (501) staff       (20)     5941 2023-05-15 11:22:34.000000 prophecy-build-tool-1.1.0.0/src/prophecy_build_tool.egg-info/PKG-INFO
--rw-r--r--   0 ashishpatel   (501) staff       (20)      444 2023-05-15 11:22:34.000000 prophecy-build-tool-1.1.0.0/src/prophecy_build_tool.egg-info/SOURCES.txt
--rw-r--r--   0 ashishpatel   (501) staff       (20)        1 2023-05-15 11:22:34.000000 prophecy-build-tool-1.1.0.0/src/prophecy_build_tool.egg-info/dependency_links.txt
--rw-r--r--   0 ashishpatel   (501) staff       (20)       33 2023-05-15 11:22:34.000000 prophecy-build-tool-1.1.0.0/src/prophecy_build_tool.egg-info/entry_points.txt
--rw-r--r--   0 ashishpatel   (501) staff       (20)       77 2023-05-15 11:22:34.000000 prophecy-build-tool-1.1.0.0/src/prophecy_build_tool.egg-info/requires.txt
--rw-r--r--   0 ashishpatel   (501) staff       (20)        4 2023-05-15 11:22:34.000000 prophecy-build-tool-1.1.0.0/src/prophecy_build_tool.egg-info/top_level.txt
-drwxr-xr-x   0 ashishpatel   (501) staff       (20)        0 2023-05-15 11:22:34.908608 prophecy-build-tool-1.1.0.0/test/
--rw-r--r--   0 ashishpatel   (501) staff       (20)     2186 2023-05-15 11:21:47.000000 prophecy-build-tool-1.1.0.0/test/test_build.py
--rw-r--r--   0 ashishpatel   (501) staff       (20)     7868 2023-05-15 11:21:47.000000 prophecy-build-tool-1.1.0.0/test/test_deploy.py
+drwxr-xr-x   0 ankitashukla   (501) staff       (20)        0 2023-05-16 14:13:31.983000 prophecy-build-tool-1.1.0.1/
+-rw-r--r--   0 ankitashukla   (501) staff       (20)    11357 2023-05-09 12:32:13.000000 prophecy-build-tool-1.1.0.1/LICENSE
+-rw-r--r--   0 ankitashukla   (501) staff       (20)     5941 2023-05-16 14:13:31.983095 prophecy-build-tool-1.1.0.1/PKG-INFO
+-rw-r--r--   0 ankitashukla   (501) staff       (20)     5318 2023-05-09 12:32:13.000000 prophecy-build-tool-1.1.0.1/README.md
+-rw-r--r--   0 ankitashukla   (501) staff       (20)      419 2023-05-09 12:32:13.000000 prophecy-build-tool-1.1.0.1/pyproject.toml
+-rw-r--r--   0 ankitashukla   (501) staff       (20)      239 2023-05-16 14:13:31.983394 prophecy-build-tool-1.1.0.1/setup.cfg
+-rw-r--r--   0 ankitashukla   (501) staff       (20)     1182 2023-05-16 14:12:33.000000 prophecy-build-tool-1.1.0.1/setup.py
+drwxr-xr-x   0 ankitashukla   (501) staff       (20)        0 2023-05-16 14:13:31.956556 prophecy-build-tool-1.1.0.1/src/
+drwxr-xr-x   0 ankitashukla   (501) staff       (20)        0 2023-05-16 14:13:31.979872 prophecy-build-tool-1.1.0.1/src/pbt/
+-rw-r--r--   0 ankitashukla   (501) staff       (20)     2654 2023-05-16 14:11:17.000000 prophecy-build-tool-1.1.0.1/src/pbt/__init__.py
+-rw-r--r--   0 ankitashukla   (501) staff       (20)     1941 2023-05-09 12:32:13.000000 prophecy-build-tool-1.1.0.1/src/pbt/process.py
+-rw-r--r--   0 ankitashukla   (501) staff       (20)    37485 2023-05-16 05:22:36.000000 prophecy-build-tool-1.1.0.1/src/pbt/prophecy_build_tool.py
+drwxr-xr-x   0 ankitashukla   (501) staff       (20)        0 2023-05-16 14:13:31.982058 prophecy-build-tool-1.1.0.1/src/prophecy_build_tool.egg-info/
+-rw-r--r--   0 ankitashukla   (501) staff       (20)     5941 2023-05-16 14:13:31.000000 prophecy-build-tool-1.1.0.1/src/prophecy_build_tool.egg-info/PKG-INFO
+-rw-r--r--   0 ankitashukla   (501) staff       (20)      444 2023-05-16 14:13:31.000000 prophecy-build-tool-1.1.0.1/src/prophecy_build_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 ankitashukla   (501) staff       (20)        1 2023-05-16 14:13:31.000000 prophecy-build-tool-1.1.0.1/src/prophecy_build_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 ankitashukla   (501) staff       (20)       33 2023-05-16 14:13:31.000000 prophecy-build-tool-1.1.0.1/src/prophecy_build_tool.egg-info/entry_points.txt
+-rw-r--r--   0 ankitashukla   (501) staff       (20)       77 2023-05-16 14:13:31.000000 prophecy-build-tool-1.1.0.1/src/prophecy_build_tool.egg-info/requires.txt
+-rw-r--r--   0 ankitashukla   (501) staff       (20)        4 2023-05-16 14:13:31.000000 prophecy-build-tool-1.1.0.1/src/prophecy_build_tool.egg-info/top_level.txt
+drwxr-xr-x   0 ankitashukla   (501) staff       (20)        0 2023-05-16 14:13:31.982633 prophecy-build-tool-1.1.0.1/test/
+-rw-r--r--   0 ankitashukla   (501) staff       (20)     2186 2023-05-16 05:22:36.000000 prophecy-build-tool-1.1.0.1/test/test_build.py
+-rw-r--r--   0 ankitashukla   (501) staff       (20)     7868 2023-05-16 05:22:36.000000 prophecy-build-tool-1.1.0.1/test/test_deploy.py
```

### Comparing `prophecy-build-tool-1.1.0.0/LICENSE` & `prophecy-build-tool-1.1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prophecy-build-tool-1.1.0.0/PKG-INFO` & `prophecy-build-tool-1.1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prophecy-build-tool
-Version: 1.1.0.0
+Version: 1.1.0.1
 Summary: Prophecy-build-tool (PBT) provides utilities to build and distribute projects created from the Prophecy IDE.
 Home-page: https://github.com/SimpleDataLabsInc/prophecy-build-tool
 Author: Prophecy
 Author-email: maciej@prophecy.io
 Project-URL: Bug Tracker, https://github.com/SimpleDataLabsInc/prophecy-build-tool/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `prophecy-build-tool-1.1.0.0/README.md` & `prophecy-build-tool-1.1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `prophecy-build-tool-1.1.0.0/setup.py` & `prophecy-build-tool-1.1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as _in:
     long_description = _in.read()
 
 setuptools.setup(
     name="prophecy-build-tool",
-    version="1.1.0.0",
+    version="1.1.0.1",
     author="Prophecy",
     author_email="maciej@prophecy.io",
     description="Prophecy-build-tool (PBT) provides utilities to build and distribute projects created from the "
     "Prophecy IDE.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/SimpleDataLabsInc/prophecy-build-tool",
```

### Comparing `prophecy-build-tool-1.1.0.0/src/pbt/__init__.py` & `prophecy-build-tool-1.1.0.1/src/pbt/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -89,17 +89,22 @@
 
 @cli.command()
 @click.option(
     "--path",
     help="Path to the directory containing the pbt_project.yml file",
     required=True,
 )
-def test(path):
+@click.option(
+    "--driver-library-path",
+    help="Jar path of prophecy-python-libs and other required dependencies",
+    required=False,
+)
+def test(path, driver_library_path):
     pbt = ProphecyBuildTool(path)
-    pbt.test()
+    pbt.test(driver_library_path)
 
 
 if __name__ == "pbt":
     print(
         f"[bold purple]Prophecy-build-tool[/bold purple] [bold black]"
         f"v{pkg_resources.require('prophecy-build-tool')[0].version}[/bold black]\n"
     )
```

### Comparing `prophecy-build-tool-1.1.0.0/src/pbt/process.py` & `prophecy-build-tool-1.1.0.1/src/pbt/process.py`

 * *Files identical despite different names*

### Comparing `prophecy-build-tool-1.1.0.0/src/pbt/prophecy_build_tool.py` & `prophecy-build-tool-1.1.0.1/src/pbt/prophecy_build_tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -517,25 +517,28 @@
             print("\n[bold red] Deployment failed![/bold red]")
             if len(pipelines_upload_failures) > 0:
                 print("   Pipeline failures: %s" % (" ,".join(pipelines_upload_failures.keys())))
             if len(job_update_failures) > 0:
                 print("   Create/Update failed for jobs: %s" % (" ,".join(job_update_failures.keys())))
             sys.exit(1)
 
-    def test(self):
+    def test(self, build_jars: str = ""):
         if self._verify_unit_test_env():
             unit_test_results = {}
 
             for pipeline_i, (path_pipeline, pipeline) in enumerate(self.pipelines.items()):
                 print("\n  Unit Testing pipeline %s [%s/%s]" % (path_pipeline, pipeline_i + 1, self.pipelines_count))
 
                 path_pipeline_absolute = os.path.join(os.path.join(self.path_root, path_pipeline), "code")
                 if self.project_language == "python":
                     if os.path.isfile(os.path.join(path_pipeline_absolute, f"test{os.sep}TestSuite.py")):
+                        # unique_key_for_jars = \
+                        self._setJarsNeededForUT(build_jars)
                         unit_test_results[path_pipeline] = self.test_python(path_pipeline_absolute, path_pipeline)
+                        self.removeJarsKeyFromEnv()
                 elif self.project_language == "scala":
                     unit_test_results[path_pipeline] = self.test_scala(path_pipeline_absolute)
             is_any_ut_failed = False
             for path_pipeline, return_code in unit_test_results.items():
                 if return_code not in (0, 5):
                     is_any_ut_failed = True
                     print(
@@ -786,7 +789,17 @@
                 "Current path [u]%s[/u]" % self.path_root
             )
 
     @classmethod
     def _error(cls, message: str):
         print("[bold red]ERROR[/bold red]:", message)
         sys.exit(1)
+
+    def _setJarsNeededForUT(self, build_jars):
+        import random
+        uniqueKey = random.random()
+        jars_unique_key: str = f"driver_library_path_{uniqueKey}"
+        os.environ["SPARK_JARS_CONFIG"] = build_jars if build_jars else ""
+        # return jars_unique_key
+
+    def removeJarsKeyFromEnv(self):
+        del os.environ["SPARK_JARS_CONFIG"]
```

### Comparing `prophecy-build-tool-1.1.0.0/src/prophecy_build_tool.egg-info/PKG-INFO` & `prophecy-build-tool-1.1.0.1/src/prophecy_build_tool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prophecy-build-tool
-Version: 1.1.0.0
+Version: 1.1.0.1
 Summary: Prophecy-build-tool (PBT) provides utilities to build and distribute projects created from the Prophecy IDE.
 Home-page: https://github.com/SimpleDataLabsInc/prophecy-build-tool
 Author: Prophecy
 Author-email: maciej@prophecy.io
 Project-URL: Bug Tracker, https://github.com/SimpleDataLabsInc/prophecy-build-tool/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `prophecy-build-tool-1.1.0.0/test/test_build.py` & `prophecy-build-tool-1.1.0.1/test/test_build.py`

 * *Files identical despite different names*

### Comparing `prophecy-build-tool-1.1.0.0/test/test_deploy.py` & `prophecy-build-tool-1.1.0.1/test/test_deploy.py`

 * *Files identical despite different names*

