# Comparing `tmp/gvmkit-build-0.2.7.tar.gz` & `tmp/gvmkit_build-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gvmkit-build-0.2.7.tar", max compression
+gzip compressed data, was "gvmkit_build-0.2.8.tar", max compression
```

## Comparing `gvmkit-build-0.2.7.tar` & `gvmkit_build-0.2.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      245 2021-07-15 08:09:51.000000 gvmkit-build-0.2.7/gvmkit_build/__init__.py
--rw-r--r--   0        0        0       65 2021-07-15 08:09:51.000000 gvmkit-build-0.2.7/gvmkit_build/__main__.py
--rw-r--r--   0        0        0     7633 2021-10-27 11:58:10.290911 gvmkit-build-0.2.7/gvmkit_build/build.py
--rw-r--r--   0        0        0      266 2021-07-15 08:09:51.000000 gvmkit-build-0.2.7/gvmkit_build/decorators.py
--rw-r--r--   0        0        0     2173 2021-07-15 08:09:51.000000 gvmkit-build-0.2.7/gvmkit_build/gvmi.py
--rw-r--r--   0        0        0     1607 2021-10-27 11:58:10.290911 gvmkit-build-0.2.7/gvmkit_build/repo.py
--rw-r--r--   0        0        0      973 2021-10-27 11:58:10.290911 gvmkit-build-0.2.7/pyproject.toml
--rw-r--r--   0        0        0      904 2021-10-27 12:02:08.085381 gvmkit-build-0.2.7/setup.py
--rw-r--r--   0        0        0      946 2021-10-27 12:02:08.085527 gvmkit-build-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0      245 2023-05-16 12:33:19.066203 gvmkit_build-0.2.8/gvmkit_build/__init__.py
+-rw-r--r--   0        0        0       65 2023-05-16 12:33:19.066203 gvmkit_build-0.2.8/gvmkit_build/__main__.py
+-rw-r--r--   0        0        0     7619 2023-05-16 12:33:19.066203 gvmkit_build-0.2.8/gvmkit_build/build.py
+-rw-r--r--   0        0        0      266 2023-05-16 12:33:19.066203 gvmkit_build-0.2.8/gvmkit_build/decorators.py
+-rw-r--r--   0        0        0     2173 2023-05-16 12:33:19.066203 gvmkit_build-0.2.8/gvmkit_build/gvmi.py
+-rw-r--r--   0        0        0     1607 2023-05-16 12:33:19.066203 gvmkit_build-0.2.8/gvmkit_build/repo.py
+-rw-r--r--   0        0        0      973 2023-05-16 12:54:27.932011 gvmkit_build-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0      912 1970-01-01 00:00:00.000000 gvmkit_build-0.2.8/setup.py
+-rw-r--r--   0        0        0     1048 1970-01-01 00:00:00.000000 gvmkit_build-0.2.8/PKG-INFO
```

### Comparing `gvmkit-build-0.2.7/gvmkit_build/build.py` & `gvmkit_build-0.2.8/gvmkit_build/build.py`

 * *Files 6% similar despite different names*

```diff
@@ -148,21 +148,19 @@
     print(f"Env          :")
     print("")
     for env in config["Env"] or []:
         print(f"     - {env}")
     print("")
 
     if config['Entrypoint']:
-        cprint("Warning: ENTRYPOINT is currently not supported.", "yellow")
-        print("You'll need to manually execute the entrypoint.")
+        cprint("ENTRYPOINT is only supported on providers with start-entrypoint capability introduced in version 0.12.0.", "yellow")
         print("")
 
     if config['Cmd']:
-        cprint("Warning: CMD is currently not supported.", "yellow")
-        print("You'll need to manually execute the command.")
+        cprint("CMD is only supported on providers with start-entrypoint capability introduced in version 0.12.0", "yellow")
         print("")
 
     for key in ["Env", "Cmd", "Entrypoint"]:
         if config[key]:
             meta[key.lower()] = config[key]
 
     upload_file_name = default_output_file(image)
```

### Comparing `gvmkit-build-0.2.7/gvmkit_build/gvmi.py` & `gvmkit_build-0.2.8/gvmkit_build/gvmi.py`

 * *Files identical despite different names*

### Comparing `gvmkit-build-0.2.7/gvmkit_build/repo.py` & `gvmkit_build-0.2.8/gvmkit_build/repo.py`

 * *Files identical despite different names*

### Comparing `gvmkit-build-0.2.7/pyproject.toml` & `gvmkit_build-0.2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gvmkit-build"
-version = "0.2.7"
+version = "0.2.8"
 description = ""
 authors = ["Przemysław K. Rekucki <prekucki@rcl.pl>"]
 classifiers = [
     'Development Status :: 2 - Pre-Alpha',
     'Environment :: Console',
     'License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)',
     'Intended Audience :: Developers'
```

### Comparing `gvmkit-build-0.2.7/setup.py` & `gvmkit_build-0.2.8/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -18,22 +18,22 @@
  'typing_extensions>=3.7.4,<4.0.0']
 
 entry_points = \
 {'console_scripts': ['gvmkit-build = gvmkit_build:build']}
 
 setup_kwargs = {
     'name': 'gvmkit-build',
-    'version': '0.2.7',
+    'version': '0.2.8',
     'description': '',
-    'long_description': None,
+    'long_description': 'None',
     'author': 'Przemysław K. Rekucki',
     'author_email': 'prekucki@rcl.pl',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
     'python_requires': '>=3.6,<4.0',
 }
```

### Comparing `gvmkit-build-0.2.7/PKG-INFO` & `gvmkit_build-0.2.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: gvmkit-build
-Version: 0.2.7
+Version: 0.2.8
 Summary: 
 Author: Przemysław K. Rekucki
 Author-email: prekucki@rcl.pl
 Requires-Python: >=3.6,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: alive-progress (>=1.5.1,<2.0.0)
 Requires-Dist: argparse (>=1.4.0,<2.0.0)
 Requires-Dist: docker (>=5.0,<6.0)
 Requires-Dist: requests (>=2.24.0,<3.0.0)
 Requires-Dist: srvlookup (>=2.0.0,<3.0.0)
 Requires-Dist: termcolor (==1.1.0)
 Requires-Dist: typing (>=3.7.4,<4.0.0)
```

