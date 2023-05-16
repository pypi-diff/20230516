# Comparing `tmp/fiat_cli-0.6.6.tar.gz` & `tmp/fiat_cli-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fiat_cli-0.6.6.tar", max compression
+gzip compressed data, was "fiat_cli-0.6.8.tar", max compression
```

## Comparing `fiat_cli-0.6.6.tar` & `fiat_cli-0.6.8.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0     1067 2023-04-20 03:17:26.809646 fiat_cli-0.6.6/LICENSE
--rw-r--r--   0        0        0       68 2023-04-20 03:18:44.649085 fiat_cli-0.6.6/README.md
--rw-r--r--   0        0        0        0 2023-04-23 03:34:08.157681 fiat_cli-0.6.6/fiat/__init__.py
--rw-r--r--   0        0        0        0 2023-04-17 02:49:11.357285 fiat_cli-0.6.6/fiat/apps/__init__.py
--rw-r--r--   0        0        0     1424 2023-05-12 07:36:01.033867 fiat_cli-0.6.6/fiat/apps/computing.py
--rw-r--r--   0        0        0     2318 2023-04-26 11:36:01.175418 fiat_cli-0.6.6/fiat/apps/dashboard.py
--rw-r--r--   0        0        0     8844 2023-05-14 16:35:57.522232 fiat_cli-0.6.6/fiat/apps/envd.py
--rw-r--r--   0        0        0     5498 2023-04-26 15:24:52.709454 fiat_cli-0.6.6/fiat/apps/job.py
--rw-r--r--   0        0        0     6818 2023-05-14 07:08:04.090187 fiat_cli-0.6.6/fiat/apps/juicefs.py
--rw-r--r--   0        0        0     1458 2023-04-26 11:36:01.179870 fiat_cli-0.6.6/fiat/apps/metastore.py
--rw-r--r--   0        0        0     3153 2023-05-14 06:07:43.459755 fiat_cli-0.6.6/fiat/apps/server.py
--rw-r--r--   0        0        0     2012 2023-05-13 07:54:30.206971 fiat_cli-0.6.6/fiat/apps/templates.py
--rw-r--r--   0        0        0     4017 2023-05-13 13:26:17.158621 fiat_cli-0.6.6/fiat/apps/utils.py
--rw-r--r--   0        0        0      645 2023-05-14 05:05:45.398342 fiat_cli-0.6.6/fiat/main.py
--rw-r--r--   0        0        0      625 2023-05-16 09:46:25.314723 fiat_cli-0.6.6/pyproject.toml
--rw-r--r--   0        0        0      879 1970-01-01 00:00:00.000000 fiat_cli-0.6.6/setup.py
--rw-r--r--   0        0        0      661 1970-01-01 00:00:00.000000 fiat_cli-0.6.6/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-20 03:17:26.809646 fiat_cli-0.6.8/LICENSE
+-rw-r--r--   0        0        0       68 2023-04-20 03:18:44.649085 fiat_cli-0.6.8/README.md
+-rw-r--r--   0        0        0        0 2023-04-23 03:34:08.157681 fiat_cli-0.6.8/fiat/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-17 02:49:11.357285 fiat_cli-0.6.8/fiat/apps/__init__.py
+-rw-r--r--   0        0        0     1424 2023-05-12 07:36:01.033867 fiat_cli-0.6.8/fiat/apps/computing.py
+-rw-r--r--   0        0        0     2318 2023-04-26 11:36:01.175418 fiat_cli-0.6.8/fiat/apps/dashboard.py
+-rw-r--r--   0        0        0     1539 2023-05-16 13:40:04.322373 fiat_cli-0.6.8/fiat/apps/devs.py
+-rw-r--r--   0        0        0     8844 2023-05-14 16:35:57.522232 fiat_cli-0.6.8/fiat/apps/envd.py
+-rw-r--r--   0        0        0     5498 2023-04-26 15:24:52.709454 fiat_cli-0.6.8/fiat/apps/job.py
+-rw-r--r--   0        0        0     6818 2023-05-14 07:08:04.090187 fiat_cli-0.6.8/fiat/apps/juicefs.py
+-rw-r--r--   0        0        0     1458 2023-04-26 11:36:01.179870 fiat_cli-0.6.8/fiat/apps/metastore.py
+-rw-r--r--   0        0        0     3153 2023-05-14 06:07:43.459755 fiat_cli-0.6.8/fiat/apps/server.py
+-rw-r--r--   0        0        0     2012 2023-05-13 07:54:30.206971 fiat_cli-0.6.8/fiat/apps/templates.py
+-rw-r--r--   0        0        0     4017 2023-05-13 13:26:17.158621 fiat_cli-0.6.8/fiat/apps/utils.py
+-rw-r--r--   0        0        0      734 2023-05-16 12:23:10.412806 fiat_cli-0.6.8/fiat/main.py
+-rw-r--r--   0        0        0      625 2023-05-16 13:41:35.924331 fiat_cli-0.6.8/pyproject.toml
+-rw-r--r--   0        0        0      879 1970-01-01 00:00:00.000000 fiat_cli-0.6.8/setup.py
+-rw-r--r--   0        0        0      661 1970-01-01 00:00:00.000000 fiat_cli-0.6.8/PKG-INFO
```

### Comparing `fiat_cli-0.6.6/LICENSE` & `fiat_cli-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `fiat_cli-0.6.6/fiat/apps/computing.py` & `fiat_cli-0.6.8/fiat/apps/computing.py`

 * *Files identical despite different names*

### Comparing `fiat_cli-0.6.6/fiat/apps/dashboard.py` & `fiat_cli-0.6.8/fiat/apps/dashboard.py`

 * *Files identical despite different names*

### Comparing `fiat_cli-0.6.6/fiat/apps/envd.py` & `fiat_cli-0.6.8/fiat/apps/envd.py`

 * *Files identical despite different names*

### Comparing `fiat_cli-0.6.6/fiat/apps/job.py` & `fiat_cli-0.6.8/fiat/apps/job.py`

 * *Files identical despite different names*

### Comparing `fiat_cli-0.6.6/fiat/apps/juicefs.py` & `fiat_cli-0.6.8/fiat/apps/juicefs.py`

 * *Files identical despite different names*

### Comparing `fiat_cli-0.6.6/fiat/apps/metastore.py` & `fiat_cli-0.6.8/fiat/apps/metastore.py`

 * *Files identical despite different names*

### Comparing `fiat_cli-0.6.6/fiat/apps/server.py` & `fiat_cli-0.6.8/fiat/apps/server.py`

 * *Files identical despite different names*

### Comparing `fiat_cli-0.6.6/fiat/apps/templates.py` & `fiat_cli-0.6.8/fiat/apps/templates.py`

 * *Files identical despite different names*

### Comparing `fiat_cli-0.6.6/fiat/apps/utils.py` & `fiat_cli-0.6.8/fiat/apps/utils.py`

 * *Files identical despite different names*

### Comparing `fiat_cli-0.6.6/fiat/main.py` & `fiat_cli-0.6.8/fiat/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import typer
 
-from .apps import dashboard, metastore, computing, job, juicefs, envd
+from .apps import dashboard, metastore, computing, job, juicefs, envd, devs
 
 app = typer.Typer()
 app.add_typer(dashboard.app, name="dash", help="🎅 Fiat Dashboard commands.")
 app.add_typer(metastore.app, name="metastore", help="👾 Fiat Metastore commands.")
 app.add_typer(computing.app, name="ray", help="🚢 Fiat Computing server commands.")
 app.add_typer(job.app, name="job", help="📦 Fiat Job Submission commands.")
 app.add_typer(juicefs.app, name="dfs", help="🗄  Fiat DFS configuration commands.")
 app.add_typer(envd.app, name="env", help="🧑‍💻 Fiat Envd management commands.")
+app.add_typer(devs.app, name="dev", help="🤹 Fiat Dagster utilities commands.")
+
 
 if __name__ == "__main__":
     app()
```

### Comparing `fiat_cli-0.6.6/pyproject.toml` & `fiat_cli-0.6.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fiat-cli"
-version = "0.6.6"
+version = "0.6.8"
 license = "MIT"
 description = "🤩 - Fiat CLI Component"
 authors = ["Jiacheng Li <cheng2029@foxmail.com>"]
 readme = "README.md"
 packages = [{include = "fiat"}]
 
 [tool.poetry.scripts]
```

### Comparing `fiat_cli-0.6.6/setup.py` & `fiat_cli-0.6.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'typer[all]>=0.7.0,<0.8.0']
 
 entry_points = \
 {'console_scripts': ['fiat = fiat.main:app']}
 
 setup_kwargs = {
     'name': 'fiat-cli',
-    'version': '0.6.6',
+    'version': '0.6.8',
     'description': '🤩 - Fiat CLI Component',
     'long_description': '# Fiat CLI\n\n#### Description\n\n🛸 - The awesome Fiat CLI component!',
     'author': 'Jiacheng Li',
     'author_email': 'cheng2029@foxmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `fiat_cli-0.6.6/PKG-INFO` & `fiat_cli-0.6.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiat-cli
-Version: 0.6.6
+Version: 0.6.8
 Summary: 🤩 - Fiat CLI Component
 License: MIT
 Author: Jiacheng Li
 Author-email: cheng2029@foxmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

