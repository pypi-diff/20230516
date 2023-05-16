# Comparing `tmp/partis_basis-0.0.1.tar.gz` & `tmp/partis_basis-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Tue May 16 16:14:11 2023, max compression
+gzip compressed data, last modified: Tue May 16 17:44:18 2023, max compression
```

## Comparing `partis_basis-0.0.1.tar` & `partis_basis-0.0.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     7984 1970-01-01 00:00:00.000000 partis_basis-0.0.1/src/partis-basis/__main__.py
--rw-r--r--   0        0        0     2417 1970-01-01 00:00:00.000000 partis_basis-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0     1537 1970-01-01 00:00:00.000000 partis_basis-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1606 1970-01-01 00:00:00.000000 partis_basis-0.0.1/README.md
--rw-r--r--   0        0        0     1971 1970-01-01 00:00:00.000000 partis_basis-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     8008 1970-01-01 00:00:00.000000 partis_basis-0.0.2/src/partis-basis/__main__.py
+-rw-r--r--   0        0        0     2417 1970-01-01 00:00:00.000000 partis_basis-0.0.2/LICENSE.txt
+-rw-r--r--   0        0        0     1472 1970-01-01 00:00:00.000000 partis_basis-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1606 1970-01-01 00:00:00.000000 partis_basis-0.0.2/README.md
+-rw-r--r--   0        0        0     1892 1970-01-01 00:00:00.000000 partis_basis-0.0.2/PKG-INFO
```

### Comparing `partis_basis-0.0.1/src/partis-basis/__main__.py` & `partis_basis-0.0.2/src/partis-basis/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 import re
 from tempfile import TemporaryDirectory
 from shlex import quote
 import shutil
 import webbrowser
 import asks
 import errno
+import shlex
 from timeit import default_timer as timer
 import json
 
 venv = Path(os.environ['HOME'])/'.basis'
 APPS = ['bash', 'fish', 'jupyter', 'code']
 
 MPI_ENV_REC = re.compile('|'.join([
@@ -46,15 +47,15 @@
   # MVAPICH2:
   '(MV2_*\w+)',
   '(MPIR_*\w+)',
   '(PMI_*\w+)',
   '(PMIX_*\w+)',
   '(HYDRA_*\w+)']))
 
-CONTAINER = "library://kcdodd/basis/ubuntu-22.04-basis:0.0.1"
+CONTAINER = "library://kcdodd/basis/ubuntu-22.04-basis:0.0.2"
 
 #+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 def set_win_size(fd):
   if fd == -1:
     return
 
   # Get the window size of the real terminal
@@ -224,30 +225,32 @@
     tmp = Path(tmp)
     env_file = tmp/'env_file.txt'
 
     env_file.write_text('\n'.join([
       f"{k}='{quote(str(v))}'"
       for k,v in env.items()]))
 
+    cmd_singularity = [
+      'singularity',
+      'run',
+      '--app',
+      app,
+      '--cleanenv',
+      '--no-home',
+      '--env-file', str(env_file),
+      '--pwd', str(pwd),
+      '--bind', f"{basis}:/basis",
+      '--bind', f"{work}:/work",
+      str(image),
+      *cmd]
+
     try:
       pid, host_fd = pty.fork()
       if pid == 0:
-        os.execvp('singularity', [
-          'singularity',
-          'run',
-          '--app',
-          app,
-          '--cleanenv',
-          '--no-home',
-          '--env-file', str(env_file),
-          '--pwd', str(pwd),
-          '--bind', f"{basis}:/basis",
-          '--bind', f"{work}:/work",
-          str(image),
-          *cmd])
+        os.execvp(cmd_singularity[0], cmd_singularity)
 
         # should not return
         assert False
 
       fcntl.fcntl(host_fd, fcntl.F_SETFL, fcntl.fcntl(host_fd, fcntl.F_GETFL)|os.O_NONBLOCK)
 
       if isatty:
@@ -311,15 +314,15 @@
   '-i', '--image',
   help = "",
   type = str,
   default = CONTAINER)
 @click.option(
   '-a', '--app',
   help = f"{{{', '.join(APPS)}}}",
-  type = str,
+  type = click.Choice(APPS),
   default = 'fish')
 @click.option(
   '-b', '--basis',
   help = "",
   type = Path,
   default = None)
 @click.option(
```

### Comparing `partis_basis-0.0.1/LICENSE.txt` & `partis_basis-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `partis_basis-0.0.1/pyproject.toml` & `partis_basis-0.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -9,26 +9,24 @@
 
 #+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 # Package meta-data
 [project]
 name = "partis-basis"
 description = ""
 readme = "README.md"
-version = "0.0.1"
+version = "0.0.2"
 license = { file = "LICENSE.txt" }
 
 #+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 # Package dependencies
 requires-python = ">= 3.7.2"
 
 dependencies = [
-  "partis-pyproj ~= 0.1.1",
-  "partis-utils ~= 0.1.0",
   "click >= 8.1.3",
-  "Jinja2 >= 3.1.2",
+  "anyio",
   "asks >= 3.0.0",
   "uvloop >= 0.17.0" ]
 
 [[project.authors]]
 name = "Nanohmics Inc"
 email = ""
```

### Comparing `partis_basis-0.0.1/README.md` & `partis_basis-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `partis_basis-0.0.1/PKG-INFO` & `partis_basis-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: partis-basis
-Version: 0.0.1
+Version: 0.0.2
 Requires-Python: >=3.7.2
 Author: Nanohmics Inc
 Summary: 
 License-File: LICENSE.txt
-Requires-Dist: click>=8.1.3
-Requires-Dist: partis-utils~=0.1.0
-Requires-Dist: Jinja2>=3.1.2
-Requires-Dist: partis-pyproj~=0.1.1
-Requires-Dist: uvloop>=0.17.0
 Requires-Dist: asks>=3.0.0
+Requires-Dist: uvloop>=0.17.0
+Requires-Dist: anyio
+Requires-Dist: click>=8.1.3
 Description-Content-Type: text/markdown
 
 CLI utility for using Singularity container as virtual environment (requires singularity to already be installed).
 
 ```
 $ basis --help
 Usage: basis [OPTIONS] [CMD]...
```

