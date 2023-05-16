# Comparing `tmp/pyduinocli-0.8.0.tar.gz` & `tmp/pyduinocli-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyduinocli-0.8.0.tar", last modified: Sun Apr 19 11:20:34 2020, max compression
+gzip compressed data, was "dist/pyduinocli-0.9.0.tar", last modified: Sat Jul 11 11:16:26 2020, max compression
```

## Comparing `pyduinocli-0.8.0.tar` & `pyduinocli-0.9.0.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-19 11:20:34.000000 pyduinocli-0.8.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1567 2020-04-19 11:20:34.000000 pyduinocli-0.8.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      806 2020-04-19 11:20:19.000000 pyduinocli-0.8.0/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-19 11:20:34.000000 pyduinocli-0.8.0/pyduinocli.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1567 2020-04-19 11:20:34.000000 pyduinocli-0.8.0/pyduinocli.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-04-19 11:20:34.000000 pyduinocli-0.8.0/pyduinocli.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       11 2020-04-19 11:20:34.000000 pyduinocli-0.8.0/pyduinocli.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      785 2020-04-19 11:20:34.000000 pyduinocli-0.8.0/pyduinocli.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2020-04-19 11:20:34.000000 pyduinocli-0.8.0/setup.cfg
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-19 11:20:34.000000 pyduinocli-0.8.0/pyduinocli/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-19 11:20:34.000000 pyduinocli-0.8.0/pyduinocli/errors/
--rw-rw-r--   0 travis    (2000) travis    (2000)      177 2020-04-19 11:20:19.000000 pyduinocli-0.8.0/pyduinocli/errors/arduinoerror.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       39 2020-04-19 11:20:19.000000 pyduinocli-0.8.0/pyduinocli/errors/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-19 11:20:34.000000 pyduinocli-0.8.0/pyduinocli/constants/
--rw-rw-r--   0 travis    (2000) travis    (2000)      748 2020-04-19 11:20:19.000000 pyduinocli-0.8.0/pyduinocli/constants/flags.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      172 2020-04-19 11:20:19.000000 pyduinocli-0.8.0/pyduinocli/constants/messages.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      462 2020-04-19 11:20:19.000000 pyduinocli-0.8.0/pyduinocli/constants/commands.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-19 11:20:19.000000 pyduinocli-0.8.0/pyduinocli/constants/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-19 11:20:34.000000 pyduinocli-0.8.0/pyduinocli/commands/
--rw-rw-r--   0 travis    (2000) travis    (2000)      321 2020-04-19 11:20:19.000000 pyduinocli-0.8.0/pyduinocli/commands/cache.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1533 2020-04-19 11:20:19.000000 pyduinocli-0.8.0/pyduinocli/commands/board.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1542 2020-04-19 11:20:19.000000 pyduinocli-0.8.0/pyduinocli/commands/core.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2110 2020-04-19 11:20:19.000000 pyduinocli-0.8.0/pyduinocli/commands/compile.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      559 2020-04-19 11:20:19.000000 pyduinocli-0.8.0/pyduinocli/commands/daemon.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1717 2020-04-19 11:20:19.000000 pyduinocli-0.8.0/pyduinocli/commands/lib.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      829 2020-04-19 11:20:19.000000 pyduinocli-0.8.0/pyduinocli/commands/upload.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      873 2020-04-19 11:20:19.000000 pyduinocli-0.8.0/pyduinocli/commands/debug.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      556 2020-04-19 11:20:19.000000 pyduinocli-0.8.0/pyduinocli/commands/config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      314 2020-04-19 11:20:19.000000 pyduinocli-0.8.0/pyduinocli/commands/version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      355 2020-04-19 11:20:19.000000 pyduinocli-0.8.0/pyduinocli/commands/sketch.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1815 2020-04-19 11:20:19.000000 pyduinocli-0.8.0/pyduinocli/commands/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-19 11:20:19.000000 pyduinocli-0.8.0/pyduinocli/commands/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2136 2020-04-19 11:20:19.000000 pyduinocli-0.8.0/pyduinocli/commands/arduino.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      112 2020-04-19 11:20:19.000000 pyduinocli-0.8.0/pyduinocli/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      792 2020-04-19 11:20:19.000000 pyduinocli-0.8.0/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-11 11:16:26.000000 pyduinocli-0.9.0/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1728 2020-07-11 11:16:26.000000 pyduinocli-0.9.0/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      967 2020-07-11 11:16:10.000000 pyduinocli-0.9.0/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-11 11:16:26.000000 pyduinocli-0.9.0/pyduinocli.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1728 2020-07-11 11:16:26.000000 pyduinocli-0.9.0/pyduinocli.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-07-11 11:16:26.000000 pyduinocli-0.9.0/pyduinocli.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       11 2020-07-11 11:16:26.000000 pyduinocli-0.9.0/pyduinocli.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      858 2020-07-11 11:16:26.000000 pyduinocli-0.9.0/pyduinocli.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2020-07-11 11:16:26.000000 pyduinocli-0.9.0/setup.cfg
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-11 11:16:26.000000 pyduinocli-0.9.0/pyduinocli/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-11 11:16:26.000000 pyduinocli-0.9.0/pyduinocli/errors/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      177 2020-07-11 11:16:10.000000 pyduinocli-0.9.0/pyduinocli/errors/arduinoerror.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-07-11 11:16:10.000000 pyduinocli-0.9.0/pyduinocli/errors/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-11 11:16:26.000000 pyduinocli-0.9.0/pyduinocli/constants/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      882 2020-07-11 11:16:10.000000 pyduinocli-0.9.0/pyduinocli/constants/flags.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      172 2020-07-11 11:16:10.000000 pyduinocli-0.9.0/pyduinocli/constants/messages.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      524 2020-07-11 11:16:10.000000 pyduinocli-0.9.0/pyduinocli/constants/commands.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-07-11 11:16:10.000000 pyduinocli-0.9.0/pyduinocli/constants/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-11 11:16:26.000000 pyduinocli-0.9.0/pyduinocli/commands/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      321 2020-07-11 11:16:10.000000 pyduinocli-0.9.0/pyduinocli/commands/cache.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      539 2020-07-11 11:16:10.000000 pyduinocli-0.9.0/pyduinocli/commands/completion.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1900 2020-07-11 11:16:10.000000 pyduinocli-0.9.0/pyduinocli/commands/board.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1542 2020-07-11 11:16:10.000000 pyduinocli-0.9.0/pyduinocli/commands/core.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2246 2020-07-11 11:16:10.000000 pyduinocli-0.9.0/pyduinocli/commands/compile.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      559 2020-07-11 11:16:10.000000 pyduinocli-0.9.0/pyduinocli/commands/daemon.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1717 2020-07-11 11:16:10.000000 pyduinocli-0.9.0/pyduinocli/commands/lib.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      965 2020-07-11 11:16:10.000000 pyduinocli-0.9.0/pyduinocli/commands/upload.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      889 2020-07-11 11:16:10.000000 pyduinocli-0.9.0/pyduinocli/commands/debug.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      556 2020-07-11 11:16:10.000000 pyduinocli-0.9.0/pyduinocli/commands/config.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      610 2020-07-11 11:16:10.000000 pyduinocli-0.9.0/pyduinocli/commands/version.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      355 2020-07-11 11:16:10.000000 pyduinocli-0.9.0/pyduinocli/commands/sketch.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1828 2020-07-11 11:16:10.000000 pyduinocli-0.9.0/pyduinocli/commands/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      876 2020-07-11 11:16:10.000000 pyduinocli-0.9.0/pyduinocli/commands/burn_bootloader.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-07-11 11:16:10.000000 pyduinocli-0.9.0/pyduinocli/commands/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6359 2020-07-11 11:16:10.000000 pyduinocli-0.9.0/pyduinocli/commands/arduino.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      125 2020-07-11 11:16:10.000000 pyduinocli-0.9.0/pyduinocli/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      792 2020-07-11 11:16:10.000000 pyduinocli-0.9.0/setup.py
```

### Comparing `pyduinocli-0.8.0/pyduinocli.egg-info/SOURCES.txt` & `pyduinocli-0.9.0/pyduinocli.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -5,16 +5,18 @@
 pyduinocli.egg-info/SOURCES.txt
 pyduinocli.egg-info/dependency_links.txt
 pyduinocli.egg-info/top_level.txt
 pyduinocli/commands/__init__.py
 pyduinocli/commands/arduino.py
 pyduinocli/commands/base.py
 pyduinocli/commands/board.py
+pyduinocli/commands/burn_bootloader.py
 pyduinocli/commands/cache.py
 pyduinocli/commands/compile.py
+pyduinocli/commands/completion.py
 pyduinocli/commands/config.py
 pyduinocli/commands/core.py
 pyduinocli/commands/daemon.py
 pyduinocli/commands/debug.py
 pyduinocli/commands/lib.py
 pyduinocli/commands/sketch.py
 pyduinocli/commands/upload.py
```

### Comparing `pyduinocli-0.8.0/pyduinocli/constants/flags.py` & `pyduinocli-0.9.0/pyduinocli/constants/flags.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,7 +23,12 @@
 NAMES = '--names'
 ALL = '--all'
 DAEMONIZE = '--daemonize'
 LIBRARIES = '--libraries'
 OPTIMIZE_FOR_DEBUG = '--optimize-for-debug'
 DRY_RUN = '--dry-run'
 INTERPRETER = '--interpreter'
+FULL = '--full'
+PROGRAMMER = '--programmer'
+OUTPUT_DIR = '--output-dir'
+NO_DESCRIPTION = '--no-description'
+INPUT_DIR = '--input-dir'
```

### Comparing `pyduinocli-0.8.0/pyduinocli/commands/board.py` & `pyduinocli-0.9.0/pyduinocli/commands/board.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,33 @@
 from pyduinocli.commands.base import CommandBase
 from pyduinocli.constants import commands
 from pyduinocli.constants import messages
 from pyduinocli.constants import flags
-from pyduinocli.errors import ArduinoError
+from pyduinocli.errors.arduinoerror import ArduinoError
 
 
 class BoardCommand(CommandBase):
+    """
+    This class wraps the call to the :code:`board` command of :code:`arduino-cli`
+    """
 
     def __init__(self, base_args):
         CommandBase.__init__(self, base_args)
         self._base_args.append(commands.BOARD)
 
     def attach(self, port=None, fqbn=None, sketch_path=None, timeout=None):
+        """
+        Calls the :code:`board attach` command.
+
+        :param port:
+        :param fqbn:
+        :param sketch_path:
+        :param timeout:
+        :return:
+        """
         args = [commands.ATTACH]
         if port and fqbn:
             raise ArduinoError(messages.ERROR_PORT_FQBN_SET)
         if not port and not fqbn:
             raise ArduinoError(messages.ERROR_PORT_FQBN_NOT_SET)
         if port:
             args.append(CommandBase._strip_arg(port))
@@ -23,16 +35,18 @@
             args.append(CommandBase._strip_arg(fqbn))
         if sketch_path:
             args.append(CommandBase._strip_arg(sketch_path))
         if timeout:
             args.extend([flags.TIMEOUT, CommandBase._strip_arg(timeout)])
         return self._exec(args)
 
-    def details(self, fqbn):
+    def details(self, fqbn, full=None):
         args = [commands.DETAILS, CommandBase._strip_arg(fqbn)]
+        if full is True:
+            args.append(flags.FULL)
         return self._exec(args)
 
     def list(self, timeout=None):
         args = [commands.LIST]
         if timeout:
             args.extend([flags.TIMEOUT, CommandBase._strip_arg(timeout)])
         return self._exec(args)
```

### Comparing `pyduinocli-0.8.0/pyduinocli/commands/core.py` & `pyduinocli-0.9.0/pyduinocli/commands/core.py`

 * *Files identical despite different names*

### Comparing `pyduinocli-0.8.0/pyduinocli/commands/compile.py` & `pyduinocli-0.9.0/pyduinocli/commands/compile.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 class CompileCommand(CommandBase):
 
     def __init__(self, base_args):
         CommandBase.__init__(self, base_args)
         self._base_args.append(commands.COMPILE)
 
     def __call__(self,
-                 sketch, build_cache_path=None, build_path=None, build_properties=None, fqbn=None, output=None,
+                 sketch, build_cache_path=None, build_path=None, build_properties=None, fqbn=None, output_dir=None,
                  port=None, preprocess=None, show_properties=None, upload=None, verify=None, vid_pid=None,
-                 warnings=None, libraries=None, optimize_for_debug=None, dry_run=None):
+                 warnings=None, libraries=None, optimize_for_debug=None, dry_run=None, programmer=None):
         args = []
         if build_cache_path:
             args.extend([flags.BUILD_CACHE_PATH, CommandBase._strip_arg(build_cache_path)])
         if build_path:
             args.extend([flags.BUILD_PATH, CommandBase._strip_arg(build_path)])
         if build_properties:
             args.extend([flags.BUILD_PROPERTIES, CommandBase._strip_arg(build_properties)])
         if fqbn:
             args.extend([flags.FQBN, CommandBase._strip_arg(fqbn)])
-        if output:
-            args.extend([flags.OUTPUT, CommandBase._strip_arg(output)])
+        if output_dir:
+            args.extend([flags.OUTPUT_DIR, CommandBase._strip_arg(output_dir)])
         if port:
             args.extend([flags.PORT, CommandBase._strip_arg(port)])
         if preprocess is True:
             args.append(flags.PREPROCESS)
         if show_properties is True:
             args.append(flags.SHOW_PROPERTIES)
         if upload is True:
@@ -41,9 +41,11 @@
         if libraries:
             for library in libraries:
                 args.extend([flags.LIBRARIES, CommandBase._strip_arg(library)])
         if optimize_for_debug is True:
             args.append(flags.OPTIMIZE_FOR_DEBUG)
         if dry_run is True:
             args.append(flags.DRY_RUN)
+        if programmer:
+            args.extend([flags.PROGRAMMER, CommandBase._strip_arg(programmer)])
         args.append(CommandBase._strip_arg(sketch))
         return self._exec(args)
```

### Comparing `pyduinocli-0.8.0/pyduinocli/commands/daemon.py` & `pyduinocli-0.9.0/pyduinocli/commands/daemon.py`

 * *Files identical despite different names*

### Comparing `pyduinocli-0.8.0/pyduinocli/commands/lib.py` & `pyduinocli-0.9.0/pyduinocli/commands/lib.py`

 * *Files identical despite different names*

### Comparing `pyduinocli-0.8.0/pyduinocli/commands/upload.py` & `pyduinocli-0.9.0/pyduinocli/commands/upload.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,20 +5,22 @@
 
 class UploadCommand(CommandBase):
 
     def __init__(self, base_args):
         CommandBase.__init__(self, base_args)
         self._base_args.append(commands.UPLOAD)
 
-    def __call__(self, sketch=None, fqbn=None, input=None, port=None, verify=None):
+    def __call__(self, sketch=None, fqbn=None, input_dir=None, port=None, verify=None, programmer=None):
         args = []
         if fqbn:
             args.extend([flags.FQBN, CommandBase._strip_arg(fqbn)])
-        if input:
-            args.extend([flags.INPUT, CommandBase._strip_arg(input)])
+        if input_dir:
+            args.extend([flags.INPUT_DIR, CommandBase._strip_arg(input_dir)])
         if port:
             args.extend([flags.PORT, CommandBase._strip_arg(port)])
         if verify is True:
             args.append(flags.VERIFY)
         if sketch:
             args.append(CommandBase._strip_arg(sketch))
+        if programmer:
+            args.extend([flags.PROGRAMMER, CommandBase._strip_arg(programmer)])
         return self._exec(args)
```

### Comparing `pyduinocli-0.8.0/pyduinocli/commands/debug.py` & `pyduinocli-0.9.0/pyduinocli/commands/debug.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 
 class DebugCommand(CommandBase):
 
     def __init__(self, base_args):
         CommandBase.__init__(self, base_args)
         self._base_args.append(commands.DEBUG)
 
-    def __call__(self, fqbn=None, input=None, port=None, interpreter=None, sketch=None):
+    def __call__(self, fqbn=None, input_dir=None, port=None, interpreter=None, sketch=None):
         args = []
         if fqbn:
             args.extend([flags.FQBN, CommandBase._strip_arg(fqbn)])
-        if input:
-            args.extend([flags.INPUT, CommandBase._strip_arg(input)])
+        if input_dir:
+            args.extend([flags.INPUT_DIR, CommandBase._strip_arg(input_dir)])
         if port:
             args.extend([flags.PORT, CommandBase._strip_arg(port)])
         if interpreter:
             args.extend([flags.INTERPRETER, CommandBase._strip_arg(interpreter)])
         if sketch:
             args.append(CommandBase._strip_arg(sketch))
         return self._exec(args)
```

### Comparing `pyduinocli-0.8.0/pyduinocli/commands/config.py` & `pyduinocli-0.9.0/pyduinocli/commands/config.py`

 * *Files identical despite different names*

### Comparing `pyduinocli-0.8.0/pyduinocli/commands/base.py` & `pyduinocli-0.9.0/pyduinocli/commands/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import re
 import json
 from subprocess import Popen, PIPE
-from pyduinocli.errors import ArduinoError
+from pyduinocli.errors.arduinoerror import ArduinoError
 from pyduinocli.constants import messages
 
 
 class CommandBase:
     __ERROR_MESSAGE = "Message"
     __ERROR_CAUSE = "Cause"
```

### Comparing `pyduinocli-0.8.0/setup.py` & `pyduinocli-0.9.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def get_long_description():
     with open("README.md", "r") as readme:
         return readme.read()
 
 
 setuptools.setup(
     name="pyduinocli",
-    version="0.8.0",
+    version="0.9.0",
     author="Renaud Gaspard",
     author_email="gaspardrenaud@hotmail.com",
     description="Wrapper library around arduino-cli",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     url="https://github.com/Renaud11232/pyduinocli",
     packages=setuptools.find_packages(exclude=("tests",)),
```

