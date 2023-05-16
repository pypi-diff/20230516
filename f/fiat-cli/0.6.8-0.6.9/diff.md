# Comparing `tmp/fiat_cli-0.6.8.tar.gz` & `tmp/fiat_cli-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fiat_cli-0.6.8.tar", max compression
+gzip compressed data, was "fiat_cli-0.6.9.tar", max compression
```

## Comparing `fiat_cli-0.6.8.tar` & `fiat_cli-0.6.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1067 2023-04-20 03:17:26.809646 fiat_cli-0.6.8/LICENSE
--rw-r--r--   0        0        0       68 2023-04-20 03:18:44.649085 fiat_cli-0.6.8/README.md
--rw-r--r--   0        0        0        0 2023-04-23 03:34:08.157681 fiat_cli-0.6.8/fiat/__init__.py
--rw-r--r--   0        0        0        0 2023-04-17 02:49:11.357285 fiat_cli-0.6.8/fiat/apps/__init__.py
--rw-r--r--   0        0        0     1424 2023-05-12 07:36:01.033867 fiat_cli-0.6.8/fiat/apps/computing.py
--rw-r--r--   0        0        0     2318 2023-04-26 11:36:01.175418 fiat_cli-0.6.8/fiat/apps/dashboard.py
--rw-r--r--   0        0        0     1539 2023-05-16 13:40:04.322373 fiat_cli-0.6.8/fiat/apps/devs.py
--rw-r--r--   0        0        0     8844 2023-05-14 16:35:57.522232 fiat_cli-0.6.8/fiat/apps/envd.py
--rw-r--r--   0        0        0     5498 2023-04-26 15:24:52.709454 fiat_cli-0.6.8/fiat/apps/job.py
--rw-r--r--   0        0        0     6818 2023-05-14 07:08:04.090187 fiat_cli-0.6.8/fiat/apps/juicefs.py
--rw-r--r--   0        0        0     1458 2023-04-26 11:36:01.179870 fiat_cli-0.6.8/fiat/apps/metastore.py
--rw-r--r--   0        0        0     3153 2023-05-14 06:07:43.459755 fiat_cli-0.6.8/fiat/apps/server.py
--rw-r--r--   0        0        0     2012 2023-05-13 07:54:30.206971 fiat_cli-0.6.8/fiat/apps/templates.py
--rw-r--r--   0        0        0     4017 2023-05-13 13:26:17.158621 fiat_cli-0.6.8/fiat/apps/utils.py
--rw-r--r--   0        0        0      734 2023-05-16 12:23:10.412806 fiat_cli-0.6.8/fiat/main.py
--rw-r--r--   0        0        0      625 2023-05-16 13:41:35.924331 fiat_cli-0.6.8/pyproject.toml
--rw-r--r--   0        0        0      879 1970-01-01 00:00:00.000000 fiat_cli-0.6.8/setup.py
--rw-r--r--   0        0        0      661 1970-01-01 00:00:00.000000 fiat_cli-0.6.8/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-20 03:17:26.809646 fiat_cli-0.6.9/LICENSE
+-rw-r--r--   0        0        0       68 2023-04-20 03:18:44.649085 fiat_cli-0.6.9/README.md
+-rw-r--r--   0        0        0        0 2023-04-23 03:34:08.157681 fiat_cli-0.6.9/fiat/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-17 02:49:11.357285 fiat_cli-0.6.9/fiat/apps/__init__.py
+-rw-r--r--   0        0        0     1424 2023-05-12 07:36:01.033867 fiat_cli-0.6.9/fiat/apps/computing.py
+-rw-r--r--   0        0        0     2318 2023-04-26 11:36:01.175418 fiat_cli-0.6.9/fiat/apps/dashboard.py
+-rw-r--r--   0        0        0     1539 2023-05-16 13:40:04.322373 fiat_cli-0.6.9/fiat/apps/devs.py
+-rw-r--r--   0        0        0     8844 2023-05-14 16:35:57.522232 fiat_cli-0.6.9/fiat/apps/envd.py
+-rw-r--r--   0        0        0     5498 2023-04-26 15:24:52.709454 fiat_cli-0.6.9/fiat/apps/job.py
+-rw-r--r--   0        0        0     6874 2023-05-16 16:41:30.292389 fiat_cli-0.6.9/fiat/apps/juicefs.py
+-rw-r--r--   0        0        0     1458 2023-04-26 11:36:01.179870 fiat_cli-0.6.9/fiat/apps/metastore.py
+-rw-r--r--   0        0        0     3261 2023-05-16 16:00:27.653216 fiat_cli-0.6.9/fiat/apps/server.py
+-rw-r--r--   0        0        0     2012 2023-05-13 07:54:30.206971 fiat_cli-0.6.9/fiat/apps/templates.py
+-rw-r--r--   0        0        0     4267 2023-05-16 15:53:27.211098 fiat_cli-0.6.9/fiat/apps/utils.py
+-rw-r--r--   0        0        0      734 2023-05-16 12:23:10.412806 fiat_cli-0.6.9/fiat/main.py
+-rw-r--r--   0        0        0      625 2023-05-16 16:41:49.695152 fiat_cli-0.6.9/pyproject.toml
+-rw-r--r--   0        0        0      879 1970-01-01 00:00:00.000000 fiat_cli-0.6.9/setup.py
+-rw-r--r--   0        0        0      661 1970-01-01 00:00:00.000000 fiat_cli-0.6.9/PKG-INFO
```

### Comparing `fiat_cli-0.6.8/LICENSE` & `fiat_cli-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fiat_cli-0.6.8/fiat/apps/computing.py` & `fiat_cli-0.6.9/fiat/apps/computing.py`

 * *Files identical despite different names*

### Comparing `fiat_cli-0.6.8/fiat/apps/dashboard.py` & `fiat_cli-0.6.9/fiat/apps/dashboard.py`

 * *Files identical despite different names*

### Comparing `fiat_cli-0.6.8/fiat/apps/devs.py` & `fiat_cli-0.6.9/fiat/apps/devs.py`

 * *Files identical despite different names*

### Comparing `fiat_cli-0.6.8/fiat/apps/envd.py` & `fiat_cli-0.6.9/fiat/apps/envd.py`

 * *Files identical despite different names*

### Comparing `fiat_cli-0.6.8/fiat/apps/job.py` & `fiat_cli-0.6.9/fiat/apps/job.py`

 * *Files identical despite different names*

### Comparing `fiat_cli-0.6.8/fiat/apps/juicefs.py` & `fiat_cli-0.6.9/fiat/apps/juicefs.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import typer
 import urllib3
 from rich import print
 from typer import Abort, Option, Argument
 
 from .server import send_request_to_backend, FiatBackendRequest
-from .utils import get_logger, app_conf_dir, progress_execution_with_subproc
+from .utils import get_logger, app_conf_dir, progress_execution_with_subproc, simple_execution_with_system
 
 app = typer.Typer()
 logger = get_logger()
 
 
 class StorageType(Enum):
     S3 = "s3"
@@ -185,15 +185,18 @@
             "--force", "-f",
             help="Forcebly unmount a mounted DFS."
         )
 ):
     """
     🛁 Unmount a pre-configured DFS from your computer or development environment.
     """
-    command = f"juicefs {'--force' if force else ''} umount {mounting_path}"
+    command = f"juicefs umount "
+    if force:
+        command += "--force "
+    command += mounting_path
     logger.debug(f"Unmounting Command: {command}")
 
     print(":wrench: Unmounting DFS.")
 
     progress_execution_with_subproc(
         cmd=command,
         error_msg="Unmounting DFS failed! Aborting."
@@ -225,15 +228,15 @@
     """
     🤯 !!!DANGER!!! - Destroy an existing DFS with Metaengine URL and its UUID
     """
     command = f"juicefs destroy {metastore} {fs_uuid}"
     logger.debug(f"Unmounting Command: {command}")
 
     print(":hammer_and_wrench: Destroying DFS.")
-    progress_execution_with_subproc(
+    simple_execution_with_system(
         cmd=command,
         error_msg="Destroying DFS failed! Aborting."
     )
     print(":two-hump_camel: Delete DFS Metadata from Fiat Metastore.")
     send_request_to_backend(
         api=FiatBackendRequest.DFSDelete,
         query={
```

### Comparing `fiat_cli-0.6.8/fiat/apps/metastore.py` & `fiat_cli-0.6.9/fiat/apps/metastore.py`

 * *Files identical despite different names*

### Comparing `fiat_cli-0.6.8/fiat/apps/server.py` & `fiat_cli-0.6.9/fiat/apps/server.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,18 +93,20 @@
         with open(f"{current_path}/auth.json", "r+") as file_obj:
             auth_data = json.load(file_obj)
 
     auth_header = {
         "Authorization": f"Bearer {auth_data['access_token']}"
     }
     server_host = server_conf['host']
+    logger.debug(f"Request payload: {payload}")
     if api is FiatBackendRequest.EnvdCreate or api is FiatBackendRequest.DFSCreate:
+        serialized_payload = json.dumps(payload)
         resp = requests.post(
             f"{server_host}{api.value}",
-            data=payload,
+            data=serialized_payload,
             headers=auth_header
         )
     else:
         resp = requests.delete(
             f"{server_host}{api.value}",
             params=query,
             headers=auth_header
```

### Comparing `fiat_cli-0.6.8/fiat/apps/templates.py` & `fiat_cli-0.6.9/fiat/apps/templates.py`

 * *Files identical despite different names*

### Comparing `fiat_cli-0.6.8/fiat/apps/utils.py` & `fiat_cli-0.6.9/fiat/apps/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 import logging
 import os
 import subprocess
 from pathlib import Path
 
 import click
 from click import Abort
@@ -10,19 +11,27 @@
 
 import docker
 from rich.progress import Progress, SpinnerColumn, TextColumn
 
 home_path = Path(os.environ['HOME'])
 app_conf_dir = home_path / ".fiat"
 docker_scripts_path = app_conf_dir / "docker"
+current_path = os.getcwd()
 
 
 def get_logger():
+    with open(f"{current_path}/fiat.json", "r+") as file_obj:
+        conf = json.load(file_obj)
+    if "log_level" in conf.keys():
+        log_level = conf['log_level']
+    else:
+        log_level = "INFO"
+
     logging.basicConfig(
-        level="INFO",
+        level=log_level,
         format="%(message)s",
         datefmt="[%Y-%m-%d %H:%M:%S]",
         handlers=[RichHandler(rich_tracebacks=True, tracebacks_suppress=[click])]
     )
     log = logging.getLogger("rich")
 
     return log
```

### Comparing `fiat_cli-0.6.8/fiat/main.py` & `fiat_cli-0.6.9/fiat/main.py`

 * *Files identical despite different names*

### Comparing `fiat_cli-0.6.8/pyproject.toml` & `fiat_cli-0.6.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fiat-cli"
-version = "0.6.8"
+version = "0.6.9"
 license = "MIT"
 description = "🤩 - Fiat CLI Component"
 authors = ["Jiacheng Li <cheng2029@foxmail.com>"]
 readme = "README.md"
 packages = [{include = "fiat"}]
 
 [tool.poetry.scripts]
```

### Comparing `fiat_cli-0.6.8/setup.py` & `fiat_cli-0.6.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'typer[all]>=0.7.0,<0.8.0']
 
 entry_points = \
 {'console_scripts': ['fiat = fiat.main:app']}
 
 setup_kwargs = {
     'name': 'fiat-cli',
-    'version': '0.6.8',
+    'version': '0.6.9',
     'description': '🤩 - Fiat CLI Component',
     'long_description': '# Fiat CLI\n\n#### Description\n\n🛸 - The awesome Fiat CLI component!',
     'author': 'Jiacheng Li',
     'author_email': 'cheng2029@foxmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `fiat_cli-0.6.8/PKG-INFO` & `fiat_cli-0.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiat-cli
-Version: 0.6.8
+Version: 0.6.9
 Summary: 🤩 - Fiat CLI Component
 License: MIT
 Author: Jiacheng Li
 Author-email: cheng2029@foxmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

