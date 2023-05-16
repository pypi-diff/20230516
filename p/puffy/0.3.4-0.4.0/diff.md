# Comparing `tmp/puffy-0.3.4.tar.gz` & `tmp/puffy-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "puffy-0.3.4.tar", last modified: Fri May 12 10:28:14 2023, max compression
+gzip compressed data, was "puffy-0.4.0.tar", last modified: Tue May 16 11:13:06 2023, max compression
```

## Comparing `puffy-0.3.4.tar` & `puffy-0.4.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-05-12 10:28:14.926266 puffy-0.3.4/
--rw-r--r--   0 nicolasdao   (501) staff       (20)     1541 2023-02-14 15:36:17.000000 puffy-0.3.4/LICENSE
--rw-r--r--   0 nicolasdao   (501) staff       (20)    19052 2023-05-12 10:28:14.926360 puffy-0.3.4/PKG-INFO
--rw-r--r--   0 nicolasdao   (501) staff       (20)    18559 2023-05-01 04:40:26.000000 puffy-0.3.4/README.md
--rw-r--r--   0 nicolasdao   (501) staff       (20)      251 2023-02-24 11:28:17.000000 puffy-0.3.4/pyproject.toml
--rw-r--r--   0 nicolasdao   (501) staff       (20)      825 2023-05-12 10:28:14.926783 puffy-0.3.4/setup.cfg
-drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-05-12 10:28:14.923500 puffy-0.3.4/src/
-drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-05-12 10:28:14.924716 puffy-0.3.4/src/puffy/
--rw-r--r--   0 nicolasdao   (501) staff       (20)        0 2023-02-27 02:26:12.000000 puffy-0.3.4/src/puffy/__init__.py
-drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-05-12 10:28:14.925542 puffy-0.3.4/src/puffy/error/
--rw-r--r--   0 nicolasdao   (501) staff       (20)     6106 2023-04-28 06:03:30.000000 puffy-0.3.4/src/puffy/error/__init__.py
-drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-05-12 10:28:14.925799 puffy-0.3.4/src/puffy/log/
--rw-r--r--   0 nicolasdao   (501) staff       (20)     4384 2023-05-12 10:26:42.000000 puffy-0.3.4/src/puffy/log/__init__.py
-drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-05-12 10:28:14.926048 puffy-0.3.4/src/puffy/object/
--rw-r--r--   0 nicolasdao   (501) staff       (20)     1278 2023-02-26 16:22:15.000000 puffy-0.3.4/src/puffy/object/__init__.py
-drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-05-12 10:28:14.925413 puffy-0.3.4/src/puffy.egg-info/
--rw-r--r--   0 nicolasdao   (501) staff       (20)    19052 2023-05-12 10:28:14.000000 puffy-0.3.4/src/puffy.egg-info/PKG-INFO
--rw-r--r--   0 nicolasdao   (501) staff       (20)      311 2023-05-12 10:28:14.000000 puffy-0.3.4/src/puffy.egg-info/SOURCES.txt
--rw-r--r--   0 nicolasdao   (501) staff       (20)        1 2023-05-12 10:28:14.000000 puffy-0.3.4/src/puffy.egg-info/dependency_links.txt
--rw-r--r--   0 nicolasdao   (501) staff       (20)       54 2023-05-12 10:28:14.000000 puffy-0.3.4/src/puffy.egg-info/requires.txt
--rw-r--r--   0 nicolasdao   (501) staff       (20)        6 2023-05-12 10:28:14.000000 puffy-0.3.4/src/puffy.egg-info/top_level.txt
+drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-05-16 11:13:06.278481 puffy-0.4.0/
+-rw-r--r--   0 nicolasdao   (501) staff       (20)     1541 2023-02-14 15:36:17.000000 puffy-0.4.0/LICENSE
+-rw-r--r--   0 nicolasdao   (501) staff       (20)    20027 2023-05-16 11:13:06.278570 puffy-0.4.0/PKG-INFO
+-rw-r--r--   0 nicolasdao   (501) staff       (20)    19534 2023-05-16 11:11:08.000000 puffy-0.4.0/README.md
+-rw-r--r--   0 nicolasdao   (501) staff       (20)      251 2023-02-24 11:28:17.000000 puffy-0.4.0/pyproject.toml
+-rw-r--r--   0 nicolasdao   (501) staff       (20)      825 2023-05-16 11:13:06.278952 puffy-0.4.0/setup.cfg
+drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-05-16 11:13:06.274414 puffy-0.4.0/src/
+drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-05-16 11:13:06.275626 puffy-0.4.0/src/puffy/
+-rw-r--r--   0 nicolasdao   (501) staff       (20)        0 2023-02-27 02:26:12.000000 puffy-0.4.0/src/puffy/__init__.py
+drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-05-16 11:13:06.276405 puffy-0.4.0/src/puffy/error/
+-rw-r--r--   0 nicolasdao   (501) staff       (20)     6106 2023-04-28 06:03:30.000000 puffy-0.4.0/src/puffy/error/__init__.py
+drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-05-16 11:13:06.277957 puffy-0.4.0/src/puffy/log/
+-rw-r--r--   0 nicolasdao   (501) staff       (20)     4919 2023-05-16 10:52:31.000000 puffy-0.4.0/src/puffy/log/__init__.py
+drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-05-16 11:13:06.278261 puffy-0.4.0/src/puffy/object/
+-rw-r--r--   0 nicolasdao   (501) staff       (20)     1278 2023-02-26 16:22:15.000000 puffy-0.4.0/src/puffy/object/__init__.py
+drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-05-16 11:13:06.276281 puffy-0.4.0/src/puffy.egg-info/
+-rw-r--r--   0 nicolasdao   (501) staff       (20)    20027 2023-05-16 11:13:06.000000 puffy-0.4.0/src/puffy.egg-info/PKG-INFO
+-rw-r--r--   0 nicolasdao   (501) staff       (20)      311 2023-05-16 11:13:06.000000 puffy-0.4.0/src/puffy.egg-info/SOURCES.txt
+-rw-r--r--   0 nicolasdao   (501) staff       (20)        1 2023-05-16 11:13:06.000000 puffy-0.4.0/src/puffy.egg-info/dependency_links.txt
+-rw-r--r--   0 nicolasdao   (501) staff       (20)       54 2023-05-16 11:13:06.000000 puffy-0.4.0/src/puffy.egg-info/requires.txt
+-rw-r--r--   0 nicolasdao   (501) staff       (20)        6 2023-05-16 11:13:06.000000 puffy-0.4.0/src/puffy.egg-info/top_level.txt
```

### Comparing `puffy-0.3.4/LICENSE` & `puffy-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `puffy-0.3.4/PKG-INFO` & `puffy-0.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: puffy
-Version: 0.3.4
+Version: 0.4.0
 Summary: A collection of modules with zero-dependencies to help manage common programming tasks.
 Home-page: https://github.com/nicolasdao/pypuffy
 Author: Nicolas Dao
 Author-email: nicolas.dao@gmail.com
 License: BSD-3-Clause
 Keywords: util
 Classifier: Programming Language :: Python :: 3
@@ -51,14 +51,15 @@
 >		- [Basic `error` APIs - Getting in control of your errors](#basic-error-apis---getting-in-control-of-your-errors)
 >		- [Nested errors and error stack](#nested-errors-and-error-stack)
 >		- [Managing errors in `async/await` corountines](#managing-errors-in-asyncawait-corountines)
 >   - [`log`](#log)
 >       - [Basic `log` APIs](#basic-log-apis)
 >       - [Logging errors](#logging-errors)
 >       - [Environment variables](#environment-variables)
+>       - [Global context](#global-context)
 >	- [`object`](#object)
 >		- [`JSON` API](#json-api)
 > * [Dev](#dev)
 >	- [Getting started](#dev---getting-started)
 >	- [CLI commands](#cli-commands)
 >	- [Install dependencies with `easypipinstall`](#install-dependencies-with-easypipinstall)
 >	- [Linting, formatting and testing](#linting-formatting-and-testing)
@@ -267,14 +268,46 @@
 from puffy.log import log
 
 os.environ["LOG_META"] = json.dumps({"api_name": "hello"})
 
 log(level="INFO", message="hello world") # '{"api_name": "hello", "level": "INFO", "message": "hello world"}'
 ```
 
+### Global context
+
+puffy supports setting up a context globally. That context is a dictionary global to the current execution thread. By default, that context contains no keys (i.e., `{}`). If that context is set as follow:
+
+```python
+{ "hello": "world" }
+```
+
+Then, all logs include that keyvalue pair.
+
+This global context can be accessed as follow:
+
+```python
+from puffy.log import log, set_context, get_context, reset_context
+
+log(level="INFO", message="hello world") # '{"level": "INFO", "message": "hello world"}'
+
+print(get_context()) # {}
+
+set_context(hello="world", whatever="you want")
+
+log(level="INFO", message="hello world") # '{"hello":"world", "whatever":"you want", "level": "INFO", "message": "hello world"}'
+
+print(get_context()) # {"hello":"world", "whatever":"you want"}
+
+reset_context()
+
+log(level="INFO", message="hello world") # '{"level": "INFO", "message": "hello world"}'
+
+print(get_context()) # {}
+```
+
 ## `object`
 ### `JSON` API
 
 ```python
 from puffy.object import JSON as js
 
 obj = js({ 'hello':'world' })
```

### Comparing `puffy-0.3.4/README.md` & `puffy-0.4.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 >		- [Basic `error` APIs - Getting in control of your errors](#basic-error-apis---getting-in-control-of-your-errors)
 >		- [Nested errors and error stack](#nested-errors-and-error-stack)
 >		- [Managing errors in `async/await` corountines](#managing-errors-in-asyncawait-corountines)
 >   - [`log`](#log)
 >       - [Basic `log` APIs](#basic-log-apis)
 >       - [Logging errors](#logging-errors)
 >       - [Environment variables](#environment-variables)
+>       - [Global context](#global-context)
 >	- [`object`](#object)
 >		- [`JSON` API](#json-api)
 > * [Dev](#dev)
 >	- [Getting started](#dev---getting-started)
 >	- [CLI commands](#cli-commands)
 >	- [Install dependencies with `easypipinstall`](#install-dependencies-with-easypipinstall)
 >	- [Linting, formatting and testing](#linting-formatting-and-testing)
@@ -251,14 +252,46 @@
 from puffy.log import log
 
 os.environ["LOG_META"] = json.dumps({"api_name": "hello"})
 
 log(level="INFO", message="hello world") # '{"api_name": "hello", "level": "INFO", "message": "hello world"}'
 ```
 
+### Global context
+
+puffy supports setting up a context globally. That context is a dictionary global to the current execution thread. By default, that context contains no keys (i.e., `{}`). If that context is set as follow:
+
+```python
+{ "hello": "world" }
+```
+
+Then, all logs include that keyvalue pair.
+
+This global context can be accessed as follow:
+
+```python
+from puffy.log import log, set_context, get_context, reset_context
+
+log(level="INFO", message="hello world") # '{"level": "INFO", "message": "hello world"}'
+
+print(get_context()) # {}
+
+set_context(hello="world", whatever="you want")
+
+log(level="INFO", message="hello world") # '{"hello":"world", "whatever":"you want", "level": "INFO", "message": "hello world"}'
+
+print(get_context()) # {"hello":"world", "whatever":"you want"}
+
+reset_context()
+
+log(level="INFO", message="hello world") # '{"level": "INFO", "message": "hello world"}'
+
+print(get_context()) # {}
+```
+
 ## `object`
 ### `JSON` API
 
 ```python
 from puffy.object import JSON as js
 
 obj = js({ 'hello':'world' })
```

### Comparing `puffy-0.3.4/setup.cfg` & `puffy-0.4.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = puffy
-version = 0.3.4
+version = 0.4.0
 author = Nicolas Dao
 author_email = nicolas.dao@gmail.com
 description = A collection of modules with zero-dependencies to help manage common programming tasks.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/nicolasdao/pypuffy
 readme = README.md
```

### Comparing `puffy-0.3.4/src/puffy/error/__init__.py` & `puffy-0.4.0/src/puffy/error/__init__.py`

 * *Files identical despite different names*

### Comparing `puffy-0.3.4/src/puffy/log/__init__.py` & `puffy-0.4.0/src/puffy/log/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Copyright (c) 2019-2023, Cloudless Consulting Pty Ltd.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
 import os
+import copy
 import json
 import secrets
 import traceback
 from ..error import StackedException
 
 LEVELS = ["INFO", "WARN", "ERROR", "CRITICAL"]
 
@@ -59,14 +60,40 @@
             err_str = str(error)
             return err_str
         except:
             pass
         return ""
 
 
+global_context = {}
+
+
+def set_context(**args):
+    global global_context
+    try:
+        for key in args:
+            global_context[key] = args[key]
+    except:
+        pass
+
+
+def reset_context():
+    global global_context
+    global_context = {}
+
+
+def get_context():
+    clone = {}
+    try:
+        clone = copy.deepcopy(global_context)
+    except:
+        pass
+    return clone
+
+
 def log(
     level="INFO",
     message=None,
     code=None,
     time=None,
     op_id=None,
     test=None,
@@ -81,14 +108,21 @@
         level = str.upper(f"{level}").strip()
         if level == "WARNING":
             level = "WARN"
         if level not in LEVELS:
             level = "INFO"
 
         log_data = _getGlobalMeta()
+
+        try:
+            for key in global_context:
+                log_data[key] = global_context[key]
+        except:
+            pass
+
         log_data["level"] = level
         try:
             for key in args:
                 try:
                     log_data[key] = args[key]
                 except:
                     pass
```

### Comparing `puffy-0.3.4/src/puffy/object/__init__.py` & `puffy-0.4.0/src/puffy/object/__init__.py`

 * *Files identical despite different names*

### Comparing `puffy-0.3.4/src/puffy.egg-info/PKG-INFO` & `puffy-0.4.0/src/puffy.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: puffy
-Version: 0.3.4
+Version: 0.4.0
 Summary: A collection of modules with zero-dependencies to help manage common programming tasks.
 Home-page: https://github.com/nicolasdao/pypuffy
 Author: Nicolas Dao
 Author-email: nicolas.dao@gmail.com
 License: BSD-3-Clause
 Keywords: util
 Classifier: Programming Language :: Python :: 3
@@ -51,14 +51,15 @@
 >		- [Basic `error` APIs - Getting in control of your errors](#basic-error-apis---getting-in-control-of-your-errors)
 >		- [Nested errors and error stack](#nested-errors-and-error-stack)
 >		- [Managing errors in `async/await` corountines](#managing-errors-in-asyncawait-corountines)
 >   - [`log`](#log)
 >       - [Basic `log` APIs](#basic-log-apis)
 >       - [Logging errors](#logging-errors)
 >       - [Environment variables](#environment-variables)
+>       - [Global context](#global-context)
 >	- [`object`](#object)
 >		- [`JSON` API](#json-api)
 > * [Dev](#dev)
 >	- [Getting started](#dev---getting-started)
 >	- [CLI commands](#cli-commands)
 >	- [Install dependencies with `easypipinstall`](#install-dependencies-with-easypipinstall)
 >	- [Linting, formatting and testing](#linting-formatting-and-testing)
@@ -267,14 +268,46 @@
 from puffy.log import log
 
 os.environ["LOG_META"] = json.dumps({"api_name": "hello"})
 
 log(level="INFO", message="hello world") # '{"api_name": "hello", "level": "INFO", "message": "hello world"}'
 ```
 
+### Global context
+
+puffy supports setting up a context globally. That context is a dictionary global to the current execution thread. By default, that context contains no keys (i.e., `{}`). If that context is set as follow:
+
+```python
+{ "hello": "world" }
+```
+
+Then, all logs include that keyvalue pair.
+
+This global context can be accessed as follow:
+
+```python
+from puffy.log import log, set_context, get_context, reset_context
+
+log(level="INFO", message="hello world") # '{"level": "INFO", "message": "hello world"}'
+
+print(get_context()) # {}
+
+set_context(hello="world", whatever="you want")
+
+log(level="INFO", message="hello world") # '{"hello":"world", "whatever":"you want", "level": "INFO", "message": "hello world"}'
+
+print(get_context()) # {"hello":"world", "whatever":"you want"}
+
+reset_context()
+
+log(level="INFO", message="hello world") # '{"level": "INFO", "message": "hello world"}'
+
+print(get_context()) # {}
+```
+
 ## `object`
 ### `JSON` API
 
 ```python
 from puffy.object import JSON as js
 
 obj = js({ 'hello':'world' })
```

