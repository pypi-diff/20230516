# Comparing `tmp/aiosow-0.1.5.tar.gz` & `tmp/aiosow-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiosow-0.1.5.tar", last modified: Fri May 12 10:57:49 2023, max compression
+gzip compressed data, was "aiosow-0.1.6.tar", last modified: Tue May 16 12:04:04 2023, max compression
```

## Comparing `aiosow-0.1.5.tar` & `aiosow-0.1.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:57:49.321510 aiosow-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-12 10:57:49.321510 aiosow-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-05-12 10:57:36.000000 aiosow-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:57:49.321510 aiosow-0.1.5/aiosow/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-12 10:57:36.000000 aiosow-0.1.5/aiosow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-05-12 10:57:36.000000 aiosow-0.1.5/aiosow/autofill.py
--rw-r--r--   0 runner    (1001) docker     (123)    13566 2023-05-12 10:57:36.000000 aiosow-0.1.5/aiosow/bindings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-05-12 10:57:36.000000 aiosow-0.1.5/aiosow/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-12 10:57:36.000000 aiosow-0.1.5/aiosow/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-05-12 10:57:36.000000 aiosow-0.1.5/aiosow/perpetuate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-05-12 10:57:36.000000 aiosow-0.1.5/aiosow/routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-12 10:57:36.000000 aiosow-0.1.5/aiosow/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:57:49.321510 aiosow-0.1.5/aiosow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-12 10:57:49.000000 aiosow-0.1.5/aiosow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-12 10:57:49.000000 aiosow-0.1.5/aiosow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 10:57:49.000000 aiosow-0.1.5/aiosow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-12 10:57:49.000000 aiosow-0.1.5/aiosow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-12 10:57:49.000000 aiosow-0.1.5/aiosow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-12 10:57:49.000000 aiosow-0.1.5/aiosow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 10:57:49.321510 aiosow-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-12 10:57:36.000000 aiosow-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:57:49.321510 aiosow-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-05-12 10:57:36.000000 aiosow-0.1.5/tests/test_autofill.py
--rw-r--r--   0 runner    (1001) docker     (123)     7836 2023-05-12 10:57:36.000000 aiosow-0.1.5/tests/test_bindings.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 10:57:36.000000 aiosow-0.1.5/tests/test_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-12 10:57:36.000000 aiosow-0.1.5/tests/test_perpetuate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-12 10:57:36.000000 aiosow-0.1.5/tests/test_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-12 10:57:36.000000 aiosow-0.1.5/tests/test_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:03.998016 aiosow-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-16 12:04:03.998016 aiosow-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-05-16 12:03:52.000000 aiosow-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:03.994016 aiosow-0.1.6/aiosow/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-16 12:03:52.000000 aiosow-0.1.6/aiosow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-05-16 12:03:52.000000 aiosow-0.1.6/aiosow/autofill.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13566 2023-05-16 12:03:52.000000 aiosow-0.1.6/aiosow/bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-05-16 12:03:52.000000 aiosow-0.1.6/aiosow/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-16 12:03:52.000000 aiosow-0.1.6/aiosow/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-05-16 12:03:52.000000 aiosow-0.1.6/aiosow/perpetuate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-05-16 12:03:52.000000 aiosow-0.1.6/aiosow/routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-16 12:03:52.000000 aiosow-0.1.6/aiosow/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:03.998016 aiosow-0.1.6/aiosow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-16 12:04:03.000000 aiosow-0.1.6/aiosow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-16 12:04:03.000000 aiosow-0.1.6/aiosow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 12:04:03.000000 aiosow-0.1.6/aiosow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-16 12:04:03.000000 aiosow-0.1.6/aiosow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-16 12:04:03.000000 aiosow-0.1.6/aiosow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-16 12:04:03.000000 aiosow-0.1.6/aiosow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 12:04:03.998016 aiosow-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-16 12:03:52.000000 aiosow-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:04:03.998016 aiosow-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-05-16 12:03:52.000000 aiosow-0.1.6/tests/test_autofill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7836 2023-05-16 12:03:52.000000 aiosow-0.1.6/tests/test_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:03:52.000000 aiosow-0.1.6/tests/test_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-16 12:03:52.000000 aiosow-0.1.6/tests/test_perpetuate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-16 12:03:52.000000 aiosow-0.1.6/tests/test_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-16 12:03:52.000000 aiosow-0.1.6/tests/test_setup.py
```

### Comparing `aiosow-0.1.5/PKG-INFO` & `aiosow-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiosow
-Version: 0.1.5
+Version: 0.1.6
 Summary: An event-based framework
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: doc
 
 [![Pypi](https://img.shields.io/pypi/v/aiosow?color=white&style=for-the-badge&logo=pypi&logoColor=white)](https://pypi.org/project/aiosow/)
```

### Comparing `aiosow-0.1.5/README.md` & `aiosow-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `aiosow-0.1.5/aiosow/autofill.py` & `aiosow-0.1.6/aiosow/autofill.py`

 * *Files 6% similar despite different names*

```diff
@@ -71,24 +71,34 @@
     """
     memory = kwargs.get("memory", {})
 
     def prototype(function: Callable) -> List:
         return [
             (
                 param_name,
-                None if param.default is inspect.Parameter.empty else param.default,
+                None
+                if param.default is inspect.Parameter.empty
+                else param.default,
             )
-            for param_name, param in inspect.signature(function).parameters.items()
+            for param_name, param in inspect.signature(
+                function
+            ).parameters.items()
             if param.kind != inspect.Parameter.VAR_KEYWORD
             and param.kind != inspect.Parameter.VAR_POSITIONAL
         ]
 
     class Sentinel:
         """Used to represent element to be deleted"""
 
+    def none_to_empty(el):  # pragma: no cover
+        if el == None:
+            return []
+        else:
+            return el
+
     argscopy = list(args)
     if hasattr(function, "__wrapped__"):
         given_args = args
         kws = kwargs
         name = function.__wrapped__.__name__
     else:
         name = getattr(function, "__name__", None) or str(function)
@@ -99,25 +109,28 @@
             if name == "memory"
             else await autofill(ALIASES[name], args=[], memory=memory)
             if name in ALIASES
             else argscopy.pop(0)
             if len(argscopy) > 0
             else (
                 memory.get(name, value)
-                if not inspect.getfullargspec(function).varkw
+                if not name
+                in none_to_empty(inspect.getfullargspec(function).varkw)
                 else Sentinel
             )
             for (name, value) in prot
         ]
         given_args = [arg for arg in given_args if arg != Sentinel]
         has_varargs = any(
             param.kind == inspect.Parameter.VAR_POSITIONAL
             for param in inspect.signature(function).parameters.values()
         )
-        given_args = given_args if not has_varargs else given_args + list(argscopy)
+        given_args = (
+            given_args if not has_varargs else given_args + list(argscopy)
+        )
     return (name, given_args, kws)
 
 
 def get_function_representation(function):
     name = function.__name__
     if name == "<lambda>":
         name = (
@@ -128,15 +141,17 @@
         )
     return name
 
 
 async def autofill(function: Callable, args: Any = [], **kwargs) -> Any:
     name, given_args, kws = await fill_prototype(function, args=args, **kwargs)
     try:
-        if kwargs.get("memory", {}).get("log_autofill", False):  # pragma: no cover
+        if kwargs.get("memory", {}).get(
+            "log_autofill", False
+        ):  # pragma: no cover
             function_representation = get_function_representation(function)
             logging.info(f" -> {function_representation}")
         result = function(*given_args, **kws)
         return await result if inspect.iscoroutine(result) else result
     except Exception as err:  # pragma: no cover
         logging.error(f"{name} : {err}")
         logging.debug(f" > error generated by calling {name}({given_args})")
@@ -153,14 +168,16 @@
 
     **returns**:
     - Async Callable
     """
 
     async def wrapper(*args, **kwargs):
         loop = asyncio.get_event_loop()
-        __name__, given_args, kws = await fill_prototype(function, args=args, **kwargs)
+        __name__, given_args, kws = await fill_prototype(
+            function, args=args, **kwargs
+        )
         return await loop.run_in_executor(None, function, *given_args, **kws)
 
     return wrapper
 
 
 __all__ = ["alias", "autofill", "make_async", "fill_prototype"]
```

### Comparing `aiosow-0.1.5/aiosow/bindings.py` & `aiosow-0.1.6/aiosow/bindings.py`

 * *Files identical despite different names*

### Comparing `aiosow-0.1.5/aiosow/command.py` & `aiosow-0.1.6/aiosow/command.py`

 * *Files identical despite different names*

### Comparing `aiosow-0.1.5/aiosow/options.py` & `aiosow-0.1.6/aiosow/options.py`

 * *Files identical despite different names*

### Comparing `aiosow-0.1.5/aiosow/perpetuate.py` & `aiosow-0.1.6/aiosow/perpetuate.py`

 * *Files identical despite different names*

### Comparing `aiosow-0.1.5/aiosow/routines.py` & `aiosow-0.1.6/aiosow/routines.py`

 * *Files identical despite different names*

### Comparing `aiosow-0.1.5/aiosow/setup.py` & `aiosow-0.1.6/aiosow/setup.py`

 * *Files identical despite different names*

### Comparing `aiosow-0.1.5/aiosow.egg-info/PKG-INFO` & `aiosow-0.1.6/aiosow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiosow
-Version: 0.1.5
+Version: 0.1.6
 Summary: An event-based framework
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: doc
 
 [![Pypi](https://img.shields.io/pypi/v/aiosow?color=white&style=for-the-badge&logo=pypi&logoColor=white)](https://pypi.org/project/aiosow/)
```

### Comparing `aiosow-0.1.5/setup.py` & `aiosow-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="aiosow",
-    version="0.1.5",
+    version="0.1.6",
     packages=find_packages(include=["aiosow"]),
     description="An event-based framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     entry_points={
         "console_scripts": [
```

### Comparing `aiosow-0.1.5/tests/test_autofill.py` & `aiosow-0.1.6/tests/test_autofill.py`

 * *Files identical despite different names*

### Comparing `aiosow-0.1.5/tests/test_bindings.py` & `aiosow-0.1.6/tests/test_bindings.py`

 * *Files identical despite different names*

### Comparing `aiosow-0.1.5/tests/test_perpetuate.py` & `aiosow-0.1.6/tests/test_perpetuate.py`

 * *Files identical despite different names*

### Comparing `aiosow-0.1.5/tests/test_routines.py` & `aiosow-0.1.6/tests/test_routines.py`

 * *Files identical despite different names*

### Comparing `aiosow-0.1.5/tests/test_setup.py` & `aiosow-0.1.6/tests/test_setup.py`

 * *Files identical despite different names*

