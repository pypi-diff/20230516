# Comparing `tmp/lazi-1.5.59.tar.gz` & `tmp/lazi-1.6.62.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazi-1.5.59.tar", max compression
+gzip compressed data, was "lazi-1.6.62.tar", max compression
```

## Comparing `lazi-1.5.59.tar` & `lazi-1.6.62.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0    34523 2023-05-10 08:04:21.503726 lazi-1.5.59/LICENSE
--rw-r--r--   0        0        0     1917 2023-05-15 07:59:50.478074 lazi-1.5.59/README.md
--rw-r--r--   0        0        0      197 2023-05-15 07:36:15.807454 lazi-1.5.59/lazi/auto.py
--rw-r--r--   0        0        0      284 2023-05-12 07:30:19.063612 lazi-1.5.59/lazi/conf/auto.py
--rw-r--r--   0        0        0     1001 2023-05-15 19:51:29.591920 lazi-1.5.59/lazi/conf/base.py
--rw-r--r--   0        0        0     4738 2023-05-15 15:37:52.100153 lazi-1.5.59/lazi/conf/conf.py
--rw-r--r--   0        0        0       99 2023-05-15 15:35:10.790089 lazi-1.5.59/lazi/conf/test.py
--rw-r--r--   0        0        0      364 2023-05-15 07:36:15.807454 lazi-1.5.59/lazi/core/__init__.py
--rw-r--r--   0        0        0     3162 2023-05-15 19:51:00.219534 lazi-1.5.59/lazi/core/finder.py
--rw-r--r--   0        0        0     3655 2023-05-15 19:34:47.954749 lazi-1.5.59/lazi/core/loader.py
--rw-r--r--   0        0        0     3192 2023-05-15 19:48:21.985456 lazi-1.5.59/lazi/core/module.py
--rw-r--r--   0        0        0     1211 2023-05-15 19:47:25.048708 lazi-1.5.59/lazi/core/spec.py
--rw-r--r--   0        0        0       46 2023-05-12 00:02:04.162155 lazi-1.5.59/lazi/util/__init__.py
--rw-r--r--   0        0        0      448 2023-05-15 19:22:20.692875 lazi-1.5.59/lazi/util/debug.py
--rw-r--r--   0        0        0      146 2023-05-15 19:51:00.223534 lazi-1.5.59/lazi/util/functional.py
--rw-r--r--   0        0        0      618 2023-05-11 20:06:44.097623 lazi-1.5.59/lazi/util/util.py
--rw-r--r--   0        0        0     1555 2023-05-15 19:52:32.320744 lazi-1.5.59/pyproject.toml
--rw-r--r--   0        0        0      273 2023-05-15 18:29:35.039325 lazi-1.5.59/tests/standalone/sa_pygments.py
--rw-r--r--   0        0        0      380 2023-05-15 15:58:12.284137 lazi-1.5.59/tests/test_array.py
--rw-r--r--   0        0        0      901 2023-05-15 15:52:23.767715 lazi-1.5.59/tests/test_django.py
--rw-r--r--   0        0        0      810 2023-05-15 17:48:17.171059 lazi-1.5.59/tests/test_pygments.py
--rw-r--r--   0        0        0      775 2023-05-15 15:54:31.125344 lazi-1.5.59/tests/test_requests.py
--rw-r--r--   0        0        0     2795 2023-05-15 19:40:10.903002 lazi-1.5.59/tests/test_rich.py
--rw-r--r--   0        0        0     3012 1970-01-01 00:00:00.000000 lazi-1.5.59/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-05-10 08:04:21.503726 lazi-1.6.62/LICENSE
+-rw-r--r--   0        0        0     1917 2023-05-15 07:59:50.478074 lazi-1.6.62/README.md
+-rw-r--r--   0        0        0      197 2023-05-15 07:36:15.807454 lazi-1.6.62/lazi/auto.py
+-rw-r--r--   0        0        0      284 2023-05-12 07:30:19.063612 lazi-1.6.62/lazi/conf/auto.py
+-rw-r--r--   0        0        0     1001 2023-05-15 19:51:29.591920 lazi-1.6.62/lazi/conf/base.py
+-rw-r--r--   0        0        0     4738 2023-05-15 15:37:52.100153 lazi-1.6.62/lazi/conf/conf.py
+-rw-r--r--   0        0        0       99 2023-05-15 15:35:10.790089 lazi-1.6.62/lazi/conf/test.py
+-rw-r--r--   0        0        0      364 2023-05-15 07:36:15.807454 lazi-1.6.62/lazi/core/__init__.py
+-rw-r--r--   0        0        0     3225 2023-05-15 21:02:52.364570 lazi-1.6.62/lazi/core/finder.py
+-rw-r--r--   0        0        0     3838 2023-05-15 21:05:03.750327 lazi-1.6.62/lazi/core/loader.py
+-rw-r--r--   0        0        0     3358 2023-05-15 20:18:40.873359 lazi-1.6.62/lazi/core/module.py
+-rw-r--r--   0        0        0     1538 2023-05-15 21:05:03.754327 lazi-1.6.62/lazi/core/spec.py
+-rw-r--r--   0        0        0       46 2023-05-12 00:02:04.162155 lazi-1.6.62/lazi/util/__init__.py
+-rw-r--r--   0        0        0      448 2023-05-15 19:22:20.692875 lazi-1.6.62/lazi/util/debug.py
+-rw-r--r--   0        0        0      146 2023-05-15 19:51:00.223534 lazi-1.6.62/lazi/util/functional.py
+-rw-r--r--   0        0        0        0 2023-05-15 20:10:25.922835 lazi-1.6.62/lazi/util/util.py
+-rw-r--r--   0        0        0     1555 2023-05-15 21:08:09.776810 lazi-1.6.62/pyproject.toml
+-rw-r--r--   0        0        0      203 2023-05-15 20:49:57.210191 lazi-1.6.62/tests/standalone/sa_array.py
+-rw-r--r--   0        0        0      273 2023-05-15 18:29:35.039325 lazi-1.6.62/tests/standalone/sa_pygments.py
+-rw-r--r--   0        0        0      380 2023-05-15 15:58:12.284137 lazi-1.6.62/tests/test_array.py
+-rw-r--r--   0        0        0      901 2023-05-15 15:52:23.767715 lazi-1.6.62/tests/test_django.py
+-rw-r--r--   0        0        0      810 2023-05-15 17:48:17.171059 lazi-1.6.62/tests/test_pygments.py
+-rw-r--r--   0        0        0      775 2023-05-15 15:54:31.125344 lazi-1.6.62/tests/test_requests.py
+-rw-r--r--   0        0        0     2795 2023-05-15 19:40:10.903002 lazi-1.6.62/tests/test_rich.py
+-rw-r--r--   0        0        0     3012 1970-01-01 00:00:00.000000 lazi-1.6.62/PKG-INFO
```

### Comparing `lazi-1.5.59/LICENSE` & `lazi-1.6.62/LICENSE`

 * *Files identical despite different names*

### Comparing `lazi-1.5.59/README.md` & `lazi-1.6.62/README.md`

 * *Files identical despite different names*

### Comparing `lazi-1.5.59/lazi/conf/base.py` & `lazi-1.6.62/lazi/conf/base.py`

 * *Files identical despite different names*

### Comparing `lazi-1.5.59/lazi/conf/conf.py` & `lazi-1.6.62/lazi/conf/conf.py`

 * *Files identical despite different names*

### Comparing `lazi-1.5.59/lazi/core/finder.py` & `lazi-1.6.62/lazi/core/finder.py`

 * *Files 5% similar despite different names*

```diff
@@ -69,27 +69,28 @@
 
     def find_spec(self, name: str, path: list[str] | None = None, target: ModuleType | None = None) -> Spec | None:
         if self in self.__stack__:
             return None
 
         assert None is debug.traced(
             1,
-            f"<find> {name} <p:{len(path) if path else path!r}> <t:{target!r}> <f:{id(self)}>"
+            f"<find> {name} <id:{id(self)}> <p:{len(path) if path else path!r}> <t:{target!r}> "
+            f"<stack:{len(self.__stack__)}>"
         )
 
         if (spec := self.__specs__.get(name)) is not None:
             assert spec.finder is self, (spec.finder, self)
             return spec
 
         self.__stack__.append(self)
 
         try:
             if (spec := find_spec(name, path)) is not None:
                 spec = self.__specs__[name] = self.Spec(self, spec, path, target)
-                assert None is debug.traced(3, f"<foun> {spec.name} <L:{spec.loader_state}>")
+                assert None is debug.traced(2, f"<foun> {spec.name} <id:{id(self)}> <L:{spec.loader_state}>")
                 return spec
 
         finally:
             pop = self.__stack__.pop()
             assert pop is self, (pop, self)
 
     def invalidate_caches(self) -> None:
```

### Comparing `lazi-1.5.59/lazi/core/loader.py` & `lazi-1.6.62/lazi/core/loader.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from __future__ import annotations
 
 import sys
+from types import ModuleType
 from typing import ForwardRef
 from enum import Enum
 from importlib.abc import Loader as _Loader
 from importlib.util import module_from_spec
+from importlib.machinery import ModuleSpec
 
 from lazi.conf import conf
 from lazi.util import debug
 
 __all__ = "Loader",
 
 Spec = ForwardRef("Spec")
@@ -25,18 +27,17 @@
         LAZY = 2
         EXEC = 3
         LOAD = 4
         DEAD = 5
 
     def __init__(self, spec: Spec):
         self.loader = spec.loader
-        spec.loader = self
         spec.loader_state = self.State.INIT
 
-    def create_module(self, spec: Spec):
+    def create_module(self, spec: Spec | ModuleSpec):
         assert spec.loader is self, (spec.loader, self)
 
         if self in self.__stack__:
             return None
 
         self.__stack__.append(self)
 
@@ -45,31 +46,33 @@
                 module = module_from_spec(spec)
 
             spec.loader_state = self.State.CREA
             return spec.finder.Module(spec, module)
         finally:
             self.__stack__.pop()
 
-    def exec_module(self, module: Module, lazy: bool = True):
+    def exec_module(self, module: Module | ModuleType, lazy: bool = True):
         spec = module.__spec__
         assert spec.loader is self, (spec.loader, self)
         assert spec.loader_state in (self.State.CREA, self.State.LAZY), spec.loader_state
-        
+
         assert None is debug.traced(
             1,
-            f"<exec> {spec.name} <L:{spec.loader_state}> <l:{lazy}> "
-            f"<sys:{spec.name in sys.modules}> <{sys.modules.get(spec.name) is module}>"
+            f"<exec> {spec.name} <L:{spec.loader_state}> <l:{lazy}> <std:{spec.is_stdlib}> <bi:{spec.is_builtin}> "
+            f"<in:{spec.name in sys.modules}> <is-m:{sys.modules.get(spec.name) is module}> "
+            f"<is-t:{sys.modules[spec.name] is spec.target}>"
         )
 
         if spec.name not in sys.modules:
             assert None is debug.trace(
                 f"<exec> {spec.name} <L:{spec.loader_state}> <l:{lazy}> "
                 f"<missing-in-sys-modules-before>"
             )
             sys.modules[spec.name] = module
+
         elif sys.modules[spec.name] is not module:
             assert None is debug.trace(
                 f"<exec> {spec.name} <L:{spec.loader_state}> <l:{lazy}> "
                 f"<replaced-in-sys-modules-before>"
             )
             spec.target = sys.modules[spec.name]
             sys.modules[spec.name] = module
@@ -87,15 +90,15 @@
             f"<in:{spec.name in sys.modules}> <is-m:{sys.modules[spec.name] is module}> "
             f"<is-t:{sys.modules[spec.name] is spec.target}>"
         )
 
         if spec.name not in sys.modules:
             assert None is debug.trace(
                 f"<exec> {spec.name} <L:{spec.loader_state}> <l:{lazy}> "
-                f"<deleted-from-sys-modules>"
+                f"<deleted-from-sys-modules-after>"
             )
 
         elif sys.modules[spec.name] is not spec.target and sys.modules[spec.name] is not module:
             assert None is debug.trace(
                 f"<exec> {spec.name} <L:{spec.loader_state}> <l:{lazy}> "
                 f"<replaced-in-sys-modules-after>"
             )
```

### Comparing `lazi-1.5.59/lazi/core/module.py` & `lazi-1.6.62/lazi/core/module.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import ForwardRef
 
 from lazi.util import debug
 
 __all__ = "Module",
 
 Spec = ForwardRef("Spec")
+Loader = ForwardRef("Loader")
 
 # See https://peps.python.org/pep-0451/#attributes
 MODULE_SPEC_ATTR_MAP = dict(
     __name__="name",
     __loader__="loader",
     __package__="parent",
     __file__="origin",
@@ -18,14 +19,17 @@
 )
 
 GETATTR_PASS = ("__spec__", "__dict__", "__class__")
 SETATTR_PASS = GETATTR_PASS + tuple(MODULE_SPEC_ATTR_MAP)
 
 
 class Module:
+    __name__: str
+    __loader__: Loader
+    __package__: str
     __spec__: Spec
 
     def __init__(self, spec: Spec, module: ModuleType | None = None):
         super().__setattr__("__spec__", spec)
         spec.target = module if module is not None else self
 
     def __getattribute__(self, attr):
@@ -46,15 +50,15 @@
                         return spec.cached
                 case "__path__":
                     if spec.submodule_search_locations is not None:
                         return spec.submodule_search_locations
                 case _:
                     return getattr(spec, MODULE_SPEC_ATTR_MAP[attr])
 
-            raise AttributeError(attr)
+            return super().__getattribute__(attr) if spec.target is self else spec.target.__getattribute__(attr)
 
         self_dict = super().__getattribute__("__dict__")
 
         if attr in self_dict:
             return super().__getattribute__(attr)
 
         if spec.target is not self and attr in (module_dict := spec.target.__getattribute__("__dict__")):
```

### Comparing `lazi-1.5.59/pyproject.toml` & `lazi-1.6.62/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lazi"
-version = "1.5.59"
+version = "1.6.62"
 description = "A lightweight and extensible way to implement lazy imports globally."
 authors = ["Phillip Sitbon <phillip.sitbon@gmail.com>"]
 readme = "README.md"
 license = "AGPLv3"
 repository = "https://github.com/sitbon/lazi"
 classifiers= [
     "Environment :: Web Environment",
```

### Comparing `lazi-1.5.59/tests/test_django.py` & `lazi-1.6.62/tests/test_django.py`

 * *Files identical despite different names*

### Comparing `lazi-1.5.59/tests/test_pygments.py` & `lazi-1.6.62/tests/test_pygments.py`

 * *Files identical despite different names*

### Comparing `lazi-1.5.59/tests/test_requests.py` & `lazi-1.6.62/tests/test_requests.py`

 * *Files identical despite different names*

### Comparing `lazi-1.5.59/tests/test_rich.py` & `lazi-1.6.62/tests/test_rich.py`

 * *Files identical despite different names*

### Comparing `lazi-1.5.59/PKG-INFO` & `lazi-1.6.62/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazi
-Version: 1.5.59
+Version: 1.6.62
 Summary: A lightweight and extensible way to implement lazy imports globally.
 Home-page: https://github.com/sitbon/lazi
 License: AGPLv3
 Author: Phillip Sitbon
 Author-email: phillip.sitbon@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Environment :: Web Environment
```

