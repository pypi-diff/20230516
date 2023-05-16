# Comparing `tmp/confik-1.0.7.tar.gz` & `tmp/confik-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "confik-1.0.7.tar", last modified: Mon May 15 06:28:13 2023, max compression
+gzip compressed data, was "confik-1.0.8.tar", last modified: Tue May 16 16:16:49 2023, max compression
```

## Comparing `confik-1.0.7.tar` & `confik-1.0.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-15 06:28:13.223383 confik-1.0.7/
--rw-r--r--   0 leondaz    (501) staff       (20)     1069 2023-05-13 06:57:00.000000 confik-1.0.7/LICENSE
--rw-r--r--   0 leondaz    (501) staff       (20)      219 2023-05-15 06:28:13.223272 confik-1.0.7/PKG-INFO
--rw-r--r--   0 leondaz    (501) staff       (20)     1986 2023-05-15 06:27:44.000000 confik-1.0.7/README.md
-drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-15 06:28:13.221782 confik-1.0.7/confik/
--rw-r--r--   0 leondaz    (501) staff       (20)     1090 2023-05-15 06:27:44.000000 confik-1.0.7/confik/__init__.py
--rw-r--r--   0 leondaz    (501) staff       (20)       78 2023-05-12 03:19:53.000000 confik-1.0.7/confik/exceptions.py
--rw-r--r--   0 leondaz    (501) staff       (20)     2413 2023-05-15 06:27:35.000000 confik-1.0.7/confik/parsers.py
--rw-r--r--   0 leondaz    (501) staff       (20)     1330 2023-05-15 06:17:35.000000 confik-1.0.7/confik/proxies.py
--rw-r--r--   0 leondaz    (501) staff       (20)      619 2023-05-13 04:49:37.000000 confik-1.0.7/confik/utils.py
-drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-15 06:28:13.222315 confik-1.0.7/confik.egg-info/
--rw-r--r--   0 leondaz    (501) staff       (20)      219 2023-05-15 06:28:13.000000 confik-1.0.7/confik.egg-info/PKG-INFO
--rw-r--r--   0 leondaz    (501) staff       (20)      327 2023-05-15 06:28:13.000000 confik-1.0.7/confik.egg-info/SOURCES.txt
--rw-r--r--   0 leondaz    (501) staff       (20)        1 2023-05-15 06:28:13.000000 confik-1.0.7/confik.egg-info/dependency_links.txt
--rw-r--r--   0 leondaz    (501) staff       (20)        7 2023-05-15 06:28:13.000000 confik-1.0.7/confik.egg-info/top_level.txt
--rw-r--r--   0 leondaz    (501) staff       (20)       38 2023-05-15 06:28:13.223416 confik-1.0.7/setup.cfg
--rw-r--r--   0 leondaz    (501) staff       (20)      277 2023-05-15 06:28:00.000000 confik-1.0.7/setup.py
-drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-15 06:28:13.222890 confik-1.0.7/tests/
--rw-r--r--   0 leondaz    (501) staff       (20)      308 2023-05-13 05:42:01.000000 confik-1.0.7/tests/test_confik_parser.py
--rw-r--r--   0 leondaz    (501) staff       (20)     2924 2023-05-15 05:57:52.000000 confik-1.0.7/tests/test_read_environment_variables.py
--rw-r--r--   0 leondaz    (501) staff       (20)      149 2023-05-13 04:27:37.000000 confik-1.0.7/tests/test_utils.py
+drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-16 16:16:49.881583 confik-1.0.8/
+-rw-r--r--   0 leondaz    (501) staff       (20)     1069 2023-05-13 06:57:00.000000 confik-1.0.8/LICENSE
+-rw-r--r--   0 leondaz    (501) staff       (20)      219 2023-05-16 16:16:49.881432 confik-1.0.8/PKG-INFO
+-rw-r--r--   0 leondaz    (501) staff       (20)     2272 2023-05-16 16:11:07.000000 confik-1.0.8/README.md
+drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-16 16:16:49.879823 confik-1.0.8/confik/
+-rw-r--r--   0 leondaz    (501) staff       (20)     1116 2023-05-16 16:11:07.000000 confik-1.0.8/confik/__init__.py
+-rw-r--r--   0 leondaz    (501) staff       (20)       78 2023-05-12 03:19:53.000000 confik-1.0.8/confik/exceptions.py
+-rw-r--r--   0 leondaz    (501) staff       (20)     3246 2023-05-16 16:11:07.000000 confik-1.0.8/confik/parsers.py
+-rw-r--r--   0 leondaz    (501) staff       (20)     1451 2023-05-16 15:59:45.000000 confik-1.0.8/confik/proxies.py
+-rw-r--r--   0 leondaz    (501) staff       (20)      619 2023-05-13 04:49:37.000000 confik-1.0.8/confik/utils.py
+drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-16 16:16:49.880411 confik-1.0.8/confik.egg-info/
+-rw-r--r--   0 leondaz    (501) staff       (20)      219 2023-05-16 16:16:49.000000 confik-1.0.8/confik.egg-info/PKG-INFO
+-rw-r--r--   0 leondaz    (501) staff       (20)      327 2023-05-16 16:16:49.000000 confik-1.0.8/confik.egg-info/SOURCES.txt
+-rw-r--r--   0 leondaz    (501) staff       (20)        1 2023-05-16 16:16:49.000000 confik-1.0.8/confik.egg-info/dependency_links.txt
+-rw-r--r--   0 leondaz    (501) staff       (20)        7 2023-05-16 16:16:49.000000 confik-1.0.8/confik.egg-info/top_level.txt
+-rw-r--r--   0 leondaz    (501) staff       (20)       38 2023-05-16 16:16:49.881623 confik-1.0.8/setup.cfg
+-rw-r--r--   0 leondaz    (501) staff       (20)      277 2023-05-16 16:16:27.000000 confik-1.0.8/setup.py
+drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-16 16:16:49.880975 confik-1.0.8/tests/
+-rw-r--r--   0 leondaz    (501) staff       (20)      317 2023-05-15 06:32:19.000000 confik-1.0.8/tests/test_confik_parser.py
+-rw-r--r--   0 leondaz    (501) staff       (20)     2924 2023-05-16 16:16:31.000000 confik-1.0.8/tests/test_read_environment_variables.py
+-rw-r--r--   0 leondaz    (501) staff       (20)      149 2023-05-13 04:27:37.000000 confik-1.0.8/tests/test_utils.py
```

### Comparing `confik-1.0.7/LICENSE` & `confik-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `confik-1.0.7/confik/__init__.py` & `confik-1.0.8/confik/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from pathlib import Path
 from typing import Union
 
 from .exceptions import ConfikError
-from .parsers import ConfikParser
-from .proxies import MapConfigToMappingProxy
+from .parsers import ConfikParser, EnvConfikParser
+from .proxies import MapConfiKToMappingProxy
 from .utils import boolean, csv
 
-confik = ConfikParser(path=".")
+confik = EnvConfikParser(path=".")
 
 
 def get(
     key,
     default=None,
     cast=None,
     default_factory=None,
@@ -26,10 +26,10 @@
     :param choices: A choices list to ensure that the value is in it
     :param raise_exception: Raise exceptions if the value was not found
     :return: str
     """
     return confik.get(key, default, cast, default_factory, choices, raise_exception)
 
 
-def read_env(path: Union[str, Path]) -> ConfikParser:
+def read_env(path: Union[str, Path]) -> EnvConfikParser:
     """Creates a ConfikParser, it's provided for convenience"""
-    return ConfikParser(path)
+    return EnvConfikParser(path)
```

### Comparing `confik-1.0.7/confik/parsers.py` & `confik-1.0.8/confik/parsers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from collections.abc import Callable, Iterable
 
 from confik.exceptions import ConfikError
-from confik.proxies import EnvMappingProxy
+from confik.proxies import EnvMappingProxy, MapConfiKToMappingProxy
 from confik.utils import boolean
 
 
 class ConfikParser:
-    proxy_class = EnvMappingProxy
+    proxy_class = None
 
     def __init__(self, *args, **kwargs):
-        self.source = self.proxy_class(*args, **kwargs)
+        self.source: MapConfiKToMappingProxy = self.proxy_class(*args, **kwargs)
 
     def validate_params(
         self,
         key,
         cast,
         default,
         default_factory,
@@ -33,29 +33,23 @@
         assert isinstance(raise_exception, bool), "raise_exception must be a boolean"
 
         if default and choices:
             assert (
                 default in choices
             ), "default value is not in the list of provided choices"
 
-    def get(
+    def process_env(
         self,
+        env,
         key,
-        default=None,
-        cast=None,
-        default_factory=None,
-        choices=tuple(),
-        raise_exception=True,
+        cast,
+        default_factory,
+        choices,
+        raise_exception,
     ):
-        self.validate_params(
-            key, cast, default, default_factory, choices, raise_exception
-        )
-
-        env = self.source.get(key, default)
-
         if env is None:
             if default_factory:
                 return default_factory(key)
             elif raise_exception:
                 raise ConfikError(
                     "{key} variable can't be of type None".format(key=key)
                 )
@@ -74,7 +68,46 @@
                 return cast(env)
             except ValueError:
                 raise ConfikError(
                     "value {v} can't be casted into {c}".format(v=env, c=cast.__name__)
                 )
 
         return env
+
+    def get(
+        self,
+        key,
+        default=None,
+        cast=None,
+        default_factory=None,
+        choices=tuple(),
+        raise_exception=True,
+    ):
+        self.validate_params(
+            key, cast, default, default_factory, choices, raise_exception
+        )
+
+        env = self.source.get(key, default)
+        return self.process_env(
+            env, key, cast, default_factory, choices, raise_exception
+        )
+
+    async def aget(
+        self,
+        key,
+        default=None,
+        cast=None,
+        default_factory=None,
+        choices=tuple(),
+        raise_exception=True,
+    ):
+        self.validate_params(
+            key, cast, default, default_factory, choices, raise_exception
+        )
+        env = await self.source.aget(key, default)
+        return self.process_env(
+            env, key, cast, default_factory, choices, raise_exception
+        )
+
+
+class EnvConfikParser(ConfikParser):
+    proxy_class = EnvMappingProxy
```

### Comparing `confik-1.0.7/confik/utils.py` & `confik-1.0.8/confik/utils.py`

 * *Files identical despite different names*

### Comparing `confik-1.0.7/tests/test_read_environment_variables.py` & `confik-1.0.8/tests/test_read_environment_variables.py`

 * *Files identical despite different names*

