# Comparing `tmp/lazi-1.7.74.tar.gz` & `tmp/lazi-1.7.80.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazi-1.7.74.tar", max compression
+gzip compressed data, was "lazi-1.7.80.tar", max compression
```

## Comparing `lazi-1.7.74.tar` & `lazi-1.7.80.tar`

### file list

```diff
@@ -1,25 +1,26 @@
--rw-r--r--   0        0        0    34523 2023-05-10 08:04:21.503726 lazi-1.7.74/LICENSE
--rw-r--r--   0        0        0     1913 2023-05-16 03:20:51.902303 lazi-1.7.74/README.md
--rw-r--r--   0        0        0      169 2023-05-16 03:17:42.603835 lazi-1.7.74/lazi/auto.py
--rw-r--r--   0        0        0      284 2023-05-12 07:30:19.063612 lazi-1.7.74/lazi/conf/auto.py
--rw-r--r--   0        0        0     1154 2023-05-16 03:26:57.047060 lazi-1.7.74/lazi/conf/base.py
--rw-r--r--   0        0        0     4738 2023-05-15 22:42:51.727662 lazi-1.7.74/lazi/conf/conf.py
--rw-r--r--   0        0        0       99 2023-05-15 22:42:51.727662 lazi-1.7.74/lazi/conf/test.py
--rw-r--r--   0        0        0      375 2023-05-16 03:17:42.603835 lazi-1.7.74/lazi/core/__init__.py
--rw-r--r--   0        0        0     3156 2023-05-16 04:58:05.546975 lazi-1.7.74/lazi/core/finder.py
--rw-r--r--   0        0        0     2988 2023-05-16 05:00:50.417144 lazi-1.7.74/lazi/core/loader.py
--rw-r--r--   0        0        0     2640 2023-05-16 04:51:11.845532 lazi-1.7.74/lazi/core/module.py
--rw-r--r--   0        0        0     1434 2023-05-16 04:58:31.383315 lazi-1.7.74/lazi/core/spec.py
--rw-r--r--   0        0        0       46 2023-05-12 00:02:04.162155 lazi-1.7.74/lazi/util/__init__.py
--rw-r--r--   0        0        0      448 2023-05-15 22:42:51.727662 lazi-1.7.74/lazi/util/debug.py
--rw-r--r--   0        0        0      146 2023-05-15 22:42:51.727662 lazi-1.7.74/lazi/util/functional.py
--rw-r--r--   0        0        0        0 2023-05-15 22:42:51.727662 lazi-1.7.74/lazi/util/util.py
--rw-r--r--   0        0        0     1555 2023-05-16 05:04:20.127915 lazi-1.7.74/pyproject.toml
--rw-r--r--   0        0        0      203 2023-05-15 22:42:51.727662 lazi-1.7.74/tests/standalone/sa_array.py
--rw-r--r--   0        0        0      273 2023-05-15 22:42:51.727662 lazi-1.7.74/tests/standalone/sa_pygments.py
--rw-r--r--   0        0        0      380 2023-05-15 22:42:51.727662 lazi-1.7.74/tests/test_array.py
--rw-r--r--   0        0        0      901 2023-05-15 22:42:51.727662 lazi-1.7.74/tests/test_django.py
--rw-r--r--   0        0        0      810 2023-05-15 22:42:51.727662 lazi-1.7.74/tests/test_pygments.py
--rw-r--r--   0        0        0      775 2023-05-15 22:42:51.727662 lazi-1.7.74/tests/test_requests.py
--rw-r--r--   0        0        0     2795 2023-05-15 22:42:51.727662 lazi-1.7.74/tests/test_rich.py
--rw-r--r--   0        0        0     3008 1970-01-01 00:00:00.000000 lazi-1.7.74/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-05-10 08:04:21.503726 lazi-1.7.80/LICENSE
+-rw-r--r--   0        0        0     1913 2023-05-16 03:20:51.902303 lazi-1.7.80/README.md
+-rw-r--r--   0        0        0      169 2023-05-16 03:17:42.603835 lazi-1.7.80/lazi/auto.py
+-rw-r--r--   0        0        0      284 2023-05-12 07:30:19.063612 lazi-1.7.80/lazi/conf/auto.py
+-rw-r--r--   0        0        0     1463 2023-05-16 07:01:30.060331 lazi-1.7.80/lazi/conf/base.py
+-rw-r--r--   0        0        0     4738 2023-05-15 22:42:51.727662 lazi-1.7.80/lazi/conf/conf.py
+-rw-r--r--   0        0        0       99 2023-05-15 22:42:51.727662 lazi-1.7.80/lazi/conf/test.py
+-rw-r--r--   0        0        0      375 2023-05-16 03:17:42.603835 lazi-1.7.80/lazi/core/__init__.py
+-rw-r--r--   0        0        0     4104 2023-05-16 06:59:12.238528 lazi-1.7.80/lazi/core/finder.py
+-rw-r--r--   0        0        0     3491 2023-05-16 06:57:18.653043 lazi-1.7.80/lazi/core/loader.py
+-rw-r--r--   0        0        0     2724 2023-05-16 07:02:30.769125 lazi-1.7.80/lazi/core/module.py
+-rw-r--r--   0        0        0     1434 2023-05-16 05:37:58.378560 lazi-1.7.80/lazi/core/spec.py
+-rw-r--r--   0        0        0       46 2023-05-12 00:02:04.162155 lazi-1.7.80/lazi/util/__init__.py
+-rw-r--r--   0        0        0      448 2023-05-15 22:42:51.727662 lazi-1.7.80/lazi/util/debug.py
+-rw-r--r--   0        0        0      146 2023-05-15 22:42:51.727662 lazi-1.7.80/lazi/util/functional.py
+-rw-r--r--   0        0        0        0 2023-05-15 22:42:51.727662 lazi-1.7.80/lazi/util/util.py
+-rw-r--r--   0        0        0     1555 2023-05-16 07:07:23.496953 lazi-1.7.80/pyproject.toml
+-rw-r--r--   0        0        0      203 2023-05-15 22:42:51.727662 lazi-1.7.80/tests/standalone/sa_array.py
+-rw-r--r--   0        0        0      273 2023-05-15 22:42:51.727662 lazi-1.7.80/tests/standalone/sa_pygments.py
+-rw-r--r--   0        0        0      380 2023-05-15 22:42:51.727662 lazi-1.7.80/tests/test_array.py
+-rw-r--r--   0        0        0      378 2023-05-16 06:33:09.290071 lazi-1.7.80/tests/test_asyncio.py
+-rw-r--r--   0        0        0     1185 2023-05-16 06:33:34.918406 lazi-1.7.80/tests/test_django.py
+-rw-r--r--   0        0        0      810 2023-05-15 22:42:51.727662 lazi-1.7.80/tests/test_pygments.py
+-rw-r--r--   0        0        0      775 2023-05-15 22:42:51.727662 lazi-1.7.80/tests/test_requests.py
+-rw-r--r--   0        0        0     2795 2023-05-16 06:12:57.710209 lazi-1.7.80/tests/test_rich.py
+-rw-r--r--   0        0        0     3008 1970-01-01 00:00:00.000000 lazi-1.7.80/PKG-INFO
```

### Comparing `lazi-1.7.74/LICENSE` & `lazi-1.7.80/LICENSE`

 * *Files identical despite different names*

### Comparing `lazi-1.7.74/README.md` & `lazi-1.7.80/README.md`

 * *Files identical despite different names*

### Comparing `lazi-1.7.74/lazi/conf/base.py` & `lazi-1.7.80/lazi/conf/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """Base project configuration.
 """
-
 __meta__ = dict(                        # Internal configuration for <root>.conf.conf (cannot override elsewhere).
     root="lazi",                        # - Root namespace package name.
 )                                       # See conf.py for more options.
-
-DEBUG_TRACING: int = 0                  # Enable debug traces.
-
+#
+DEBUG_TRACING: int = 0                  # Enable debug traces. Currently using levels 0-4.
+#
 LAZI_AUTO_INSTALL: bool = True          # Automatically install when importing lazi.auto.
 CORE_AUTO_INSTALL: bool = False         # Automatically install when importing lazi.core.
 FORCE_LOAD_MODULE: bool = False         # Immediately call exec_module() on imported modules.
 NO_STDLIB_MODULES: bool = True          # Disable loader hooking for stdlib modules.
 DISABLE_LOAD_HOOK: bool = False         # Disable all loader hooks.
-
+SOFT_INVALIDATION: bool = False         # Keep modules in sys.modules after cache invalidation.
+GARBAG_COLLECTION: bool = (             # Enable garbage collection on cache invalidation.
+    not SOFT_INVALIDATION)              # - Only makes sense if SOFT_INVALIDATION is False.
+#
 CONF_NO_CACHING: bool | None = None     # Disable caching of conf vars.
 #                                         - None: Use the default caching behavior, which will disable
 #                                                 caching if `lazi.core` is already present in sys.modules
 #                                                 when lazi.conf.conf is imported.
```

### Comparing `lazi-1.7.74/lazi/conf/conf.py` & `lazi-1.7.80/lazi/conf/conf.py`

 * *Files identical despite different names*

### Comparing `lazi-1.7.74/lazi/core/finder.py` & `lazi-1.7.80/lazi/core/finder.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 from __future__ import annotations
 
+import gc
 import sys
 from types import ModuleType
 from importlib.util import find_spec, module_from_spec
 from importlib.abc import MetaPathFinder
 
+from lazi.conf import conf
 from lazi.util import classproperty, debug
 
 from .spec import Spec
 from .loader import Loader
 from .module import Module
 
 __all__ = "Finder", "__finder__"
 
 
 class Finder(MetaPathFinder):
     Spec: type[Spec] = Spec
     Loader: type[Loader] = Loader
     Module: type[Module] = Module
 
+    __busy__: bool = False
     __refs__: int = 0
     __specs__: dict[str, Spec]
-
     __stack__: list[Finder] = []
 
     finders = classproperty(lambda cls: (_ for _ in sys.meta_path if isinstance(_, cls)))
 
     def __init__(self):
         self.__specs__ = {}
 
@@ -33,27 +35,30 @@
         if self not in sys.meta_path:
             assert self.__refs__ == 0, self.__refs__
             assert None is debug.trace(
                 f"[{id(self)}] +{self.__class__.__name__} refs:{self.__refs__} "
                 f"inst:{len(list(self.finders))} sys:{len(sys.meta_path)} "
             )
             sys.meta_path.insert(0, self)
+            self.__stack__.append(self)
 
         self.__refs__ += 1
         return self
 
     def __exit__(self, exc_type, exc_value, traceback) -> bool:
         assert None is debug.trace(
             f"[{id(self)}] -{self.__class__.__name__} refs:{self.__refs__} "
             f"inst:{len(list(self.finders))} sys:{len(sys.meta_path)} "
         )
 
         self.__refs__ = max(self.__refs__ - 1, 0)
 
         if self.__refs__ == 0 and self in sys.meta_path:
+            pop = self.__stack__.pop()
+            assert pop is self, (pop, self)
             sys.meta_path.remove(self)
             self.invalidate_caches()
             return True
 
         return False
 
     @classmethod
@@ -61,43 +66,64 @@
         return __finder__.__enter__()
 
     @classmethod
     def uninstall(cls) -> bool:
         return __finder__.__exit__(None, None, None)
 
     def lazy(self, name: str, path: list[str] | None = None, target: ModuleType | None = None) -> ModuleType:
-        if (spec := self.find_spec(name, path, target)) is not None:
-            module = module_from_spec(spec)
-            spec.loader.exec_module(module)
-            return module
+        pop = False
+
+        if self not in self.__stack__:
+            self.__stack__.append(self)
+            pop = True
+
+        try:
+            if (spec := self.find_spec(name, path, target)) is not None:
+                module = module_from_spec(spec)
+                spec.loader.exec_module(module)
+                return module
+
+        finally:
+            if pop:
+                pop = self.__stack__.pop()
+                assert pop is self, (pop, self)
 
     def find_spec(self, name: str, path: list[str] | None = None, target: ModuleType | None = None) -> Spec | None:
-        if self in self.__stack__:
+        assert self in self.__stack__, (self, self.__stack__)
+
+        if self.__busy__ or self.__stack__[-1] != self:
             return None
 
         assert None is debug.traced(
             1,
             f"[{id(self)}] <find> {name} p:{len(path) if path else path!r} t:{target!r} "
             f"stack:{len(self.__stack__)}"
         )
 
         if (spec := self.__specs__.get(name)) is not None:
             assert spec.finder is self, (spec.finder, self)
             return spec
 
-        self.__stack__.append(self)
-
+        self.__busy__ = True
         try:
             if (spec := find_spec(name, path)) is not None:
                 spec = self.__specs__[name] = self.Spec(self, spec, path, target)
                 assert None is debug.traced(2, f"[{id(self)}] <foun> {spec.name} L:{spec.loader_state} o:{spec.origin}")
+                if conf.FORCE_LOAD_MODULE and (module := sys.modules.get(spec.name)):
+                    spec.loader.exec_module(module, spec, True)
                 return spec
-
         finally:
-            pop = self.__stack__.pop()
-            assert pop is self, (pop, self)
+            self.__busy__ = False
 
     def invalidate_caches(self) -> None:
-        self.__specs__.clear()
+        if not conf.SOFT_INVALIDATION:
+            while self.__specs__ and (spec := self.__specs__.popitem()[1]):
+                if hasattr(spec.loader, "unload_module"):
+                    spec.loader.unload_module(spec)
+        else:
+            self.__specs__.clear()
+
+        if conf.GARBAG_COLLECTION:
+            gc.collect()
 
 
 __finder__: Finder = Finder()
```

### Comparing `lazi-1.7.74/lazi/core/loader.py` & `lazi-1.7.80/lazi/core/loader.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 from sys import modules
+from types import ModuleType
 from typing import ForwardRef
 from enum import Enum
 from importlib.abc import Loader as _Loader
 from importlib.util import module_from_spec
 
 from lazi.conf import conf
 from lazi.util import debug
@@ -22,15 +23,15 @@
     class State(Enum):
         __str__ = lambda self: self.name
         INIT = 0
         CREA = 1
         LAZY = 2
         EXEC = 3
         LOAD = 4
-        # DEAD = 5
+        DEAD = 5
 
     def __init__(self, spec: Spec):
         self.loader = spec.loader
         spec.loader_state = self.State.INIT
 
     def create_module(self, spec: Spec):
         assert spec.loader is self, (spec.loader, self)
@@ -41,25 +42,28 @@
         self.__stack__.append(self)
 
         try:
             if (module := self.loader.create_module(spec)) is None:
                 module = module_from_spec(spec)
 
             spec.loader_state = self.State.CREA
-            return spec.finder.Module(spec, module)
+            module = spec.finder.Module(spec, module)
+            return module
         finally:
             self.__stack__.pop()
 
     def exec_module(self, module: Module, spec: Spec | None = None, force: bool = False, /):
         spec = spec if spec is not None else module.__spec__
         assert spec.loader is self, (spec.loader, self)
 
         name = spec.name
         state = spec.loader_state
-        nexts = spec.loader_state = self.State.EXEC if force or conf.FORCE_LOAD_MODULE else self.State.LAZY
+        nexts = spec.loader_state = self.State.EXEC if force else self.State.LAZY
+
+        assert state in (self.State.INIT, self.State.CREA, self.State.LAZY), state
 
         if name not in modules:
             assert None is debug.trace(f"[{id(module)}] <exec> {state} {name}:{nexts} missing-in-sys-modules-before")
             modules[name] = module
 
         elif modules[name] is not module:
             assert None is debug.trace(
@@ -70,19 +74,29 @@
             modules[name] = module
 
         assert None is debug.traced(1, f"[{id(module)}] <exec> {state} {name}:{nexts} std:{int(spec.stdlib)} bi:{int(spec.builtin)}")
 
         if spec.loader_state is self.State.EXEC:
             self.loader.exec_module(module, spec, force) if isinstance(self.loader, type(self)) else \
                 self.loader.exec_module(module)
-            spec.loader_state = self.State.LOAD
-            assert None is debug.traced(3, f"[{id(module)}] <EXEC> {state} {name}:{nexts}")
+            state = nexts
+            nexts = spec.loader_state = self.State.LOAD
+            assert None is debug.traced(2, f"[{id(module)}] <load> {state} {name}:{nexts}")
 
         if name not in modules:
             assert None is debug.trace(f"[{id(module)}] <exec> {state} {name}:{nexts} deleted-from-sys-modules-after")
 
         elif modules[name] is not spec.target and modules[name] is not module:
             assert None is debug.trace(
                 f"[{id(module)}] <exec> {state} {name}:{nexts} replaced-in-sys-modules-after "
                 f" by:{id(modules[name])}"
             )
             spec.target = modules[name]
+
+    def unload_module(self, spec: Spec) -> ModuleType | None:
+        module = modules.pop(spec.name, None)
+        assert None is debug.traced(
+            2,
+            f"[{id(module) if module else None}] <dead> {spec.loader_state} {spec.name}:DEAD t:{id(spec.target)}"
+        )
+        spec.loader_state = self.State.DEAD
+        return spec.target
```

### Comparing `lazi-1.7.74/lazi/core/module.py` & `lazi-1.7.80/lazi/core/module.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from types import ModuleType
 from typing import ForwardRef
 
-from lazi.conf import conf
 from lazi.util import debug
 
 __all__ = "Module",
 
 Spec = ForwardRef("Spec")
 Loader = ForwardRef("Loader")
 
@@ -30,36 +29,37 @@
     __spec__: Spec
 
     def __init__(self, spec: Spec, module: ModuleType):
         super().__init__(spec.name)
         self.__spec__ = module.__spec__ = spec
         spec.target = module
 
-    def __getattribute__(self, attr):
-        spec = super().__getattribute__("__spec__")
-
-        assert None is debug.traced(3, f"[{id(self)}] <GET> {spec.loader_state} {spec.name}[.{attr}]")
-
-        if attr in GETATTR_PASS and (index := GETATTR_PASS.index(attr)) >= 0:
-            return spec if not index else spec.target.__getattribute__(attr)
-
-        if name := MODULE_SPEC_ATTR_MAP.get(attr):
+        for module_attr, attr in MODULE_SPEC_ATTR_MAP.items():
             match attr:
                 case "__file__":
                     if spec.has_location:
-                        return spec.origin
+                        module.__file__ = spec.origin
                 case "__cached__":
                     if spec.has_location and spec.cached is not None:
-                        return spec.cached
+                        module.__cached__ = spec.cached
                 case "__path__":
                     if spec.submodule_search_locations is not None:
-                        return spec.submodule_search_locations
+                        module.__path__ = spec.submodule_search_locations
                 case _:
-                    return getattr(spec, name)
+                    setattr(module, module_attr, getattr(spec, attr))
+
+    def __getattribute__(self, attr):
+        spec = super().__getattribute__("__spec__")
+
+        assert None is debug.traced(3, f"[{id(self)}] <GET> {spec.loader_state} {spec.name}[.{attr}]")
+
+        if attr in GETATTR_PASS and (index := GETATTR_PASS.index(attr)) >= 0:
+            return spec if not index else spec.target.__getattribute__(attr)
 
+        if attr in MODULE_SPEC_ATTR_MAP:
             return spec.target.__getattribute__(attr)
 
         if spec.loader_state.value <= spec.loader.State.LAZY.value:
             assert None is debug.trace(f"[{id(self)}] <get> {spec.loader_state} {spec.name}[.{attr}]")
             spec.loader.exec_module(self, spec, True)
 
         return spec.target.__getattribute__(attr)
```

### Comparing `lazi-1.7.74/lazi/core/spec.py` & `lazi-1.7.80/lazi/core/spec.py`

 * *Files identical despite different names*

### Comparing `lazi-1.7.74/pyproject.toml` & `lazi-1.7.80/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lazi"
-version = "1.7.74"
+version = "1.7.80"
 description = "A lightweight and extensible way to implement lazy imports globally."
 authors = ["Phillip Sitbon <phillip.sitbon@gmail.com>"]
 readme = "README.md"
 license = "AGPLv3"
 repository = "https://github.com/sitbon/lazi"
 classifiers= [
     "Environment :: Web Environment",
```

### Comparing `lazi-1.7.74/tests/test_pygments.py` & `lazi-1.7.80/tests/test_pygments.py`

 * *Files identical despite different names*

### Comparing `lazi-1.7.74/tests/test_requests.py` & `lazi-1.7.80/tests/test_requests.py`

 * *Files identical despite different names*

### Comparing `lazi-1.7.74/tests/test_rich.py` & `lazi-1.7.80/tests/test_rich.py`

 * *Files identical despite different names*

### Comparing `lazi-1.7.74/PKG-INFO` & `lazi-1.7.80/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazi
-Version: 1.7.74
+Version: 1.7.80
 Summary: A lightweight and extensible way to implement lazy imports globally.
 Home-page: https://github.com/sitbon/lazi
 License: AGPLv3
 Author: Phillip Sitbon
 Author-email: phillip.sitbon@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Environment :: Web Environment
```

