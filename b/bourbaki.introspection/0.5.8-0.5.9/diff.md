# Comparing `tmp/bourbaki.introspection-0.5.8.tar.gz` & `tmp/bourbaki.introspection-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bourbaki.introspection-0.5.8.tar", last modified: Sun Apr 12 02:07:24 2020, max compression
+gzip compressed data, was "dist/bourbaki.introspection-0.5.9.tar", last modified: Sun May 24 16:20:23 2020, max compression
```

## Comparing `bourbaki.introspection-0.5.8.tar` & `bourbaki.introspection-0.5.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2020-04-12 02:07:24.000000 bourbaki.introspection-0.5.8/
--rw-r--r--   0 matt      (1000) matt      (1000)     1127 2020-04-12 02:07:24.000000 bourbaki.introspection-0.5.8/PKG-INFO
--rw-r--r--   0 matt      (1000) matt      (1000)      308 2020-02-20 08:18:10.000000 bourbaki.introspection-0.5.8/README.md
-drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2020-04-12 02:07:24.000000 bourbaki.introspection-0.5.8/bourbaki/
--rw-r--r--   0 matt      (1000) matt      (1000)       56 2020-04-02 05:15:43.000000 bourbaki.introspection-0.5.8/bourbaki/__init__.py
-drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2020-04-12 02:07:24.000000 bourbaki.introspection-0.5.8/bourbaki/introspection/
--rw-r--r--   0 matt      (1000) matt      (1000)      774 2020-04-12 02:07:06.000000 bourbaki.introspection-0.5.8/bourbaki/introspection/__init__.py
--rw-r--r--   0 matt      (1000) matt      (1000)     4206 2020-04-11 22:55:29.000000 bourbaki.introspection-0.5.8/bourbaki/introspection/builtin_signatures.py
--rw-r--r--   0 matt      (1000) matt      (1000)    19065 2020-04-11 23:29:28.000000 bourbaki.introspection-0.5.8/bourbaki/introspection/callables.py
--rw-r--r--   0 matt      (1000) matt      (1000)     3762 2020-04-02 05:15:43.000000 bourbaki.introspection-0.5.8/bourbaki/introspection/classes.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1115 2020-02-16 07:31:06.000000 bourbaki.introspection-0.5.8/bourbaki/introspection/debug.py
--rw-r--r--   0 matt      (1000) matt      (1000)    14275 2019-12-30 04:08:16.000000 bourbaki.introspection-0.5.8/bourbaki/introspection/docstrings.py
--rw-r--r--   0 matt      (1000) matt      (1000)    11889 2020-04-12 01:40:32.000000 bourbaki.introspection-0.5.8/bourbaki/introspection/generic_dispatch.py
--rw-r--r--   0 matt      (1000) matt      (1000)     6868 2020-03-23 04:04:44.000000 bourbaki.introspection-0.5.8/bourbaki/introspection/generic_dispatch_helpers.py
--rw-r--r--   0 matt      (1000) matt      (1000)    17742 2020-04-02 05:15:44.000000 bourbaki.introspection-0.5.8/bourbaki/introspection/imports.py
-drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2020-04-12 02:07:24.000000 bourbaki.introspection-0.5.8/bourbaki/introspection/object_models/
--rw-r--r--   0 matt      (1000) matt      (1000)       46 2019-12-30 04:08:16.000000 bourbaki.introspection-0.5.8/bourbaki/introspection/object_models/__init__.py
--rw-r--r--   0 matt      (1000) matt      (1000)     8962 2019-12-30 04:08:16.000000 bourbaki.introspection-0.5.8/bourbaki/introspection/object_models/scala.py
--rw-r--r--   0 matt      (1000) matt      (1000)     3509 2020-04-05 18:27:37.000000 bourbaki.introspection-0.5.8/bourbaki/introspection/polymorphism.py
--rw-r--r--   0 matt      (1000) matt      (1000)     5761 2020-03-28 03:29:33.000000 bourbaki.introspection-0.5.8/bourbaki/introspection/prettyprint.py
--rw-r--r--   0 matt      (1000) matt      (1000)     4570 2020-04-12 00:09:35.000000 bourbaki.introspection-0.5.8/bourbaki/introspection/references.py
--rw-r--r--   0 matt      (1000) matt      (1000)     7099 2020-04-02 05:15:43.000000 bourbaki.introspection-0.5.8/bourbaki/introspection/simple_repr.py
--rw-r--r--   0 matt      (1000) matt      (1000)     9442 2019-12-30 04:08:17.000000 bourbaki.introspection-0.5.8/bourbaki/introspection/subclassing.py
--rw-r--r--   0 matt      (1000) matt      (1000)    10508 2020-04-05 20:14:13.000000 bourbaki.introspection-0.5.8/bourbaki/introspection/typechecking.py
-drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2020-04-12 02:07:24.000000 bourbaki.introspection-0.5.8/bourbaki/introspection/types/
--rw-r--r--   0 matt      (1000) matt      (1000)     1196 2019-12-30 04:08:17.000000 bourbaki.introspection-0.5.8/bourbaki/introspection/types/__init__.py
--rw-r--r--   0 matt      (1000) matt      (1000)     5041 2020-04-02 05:15:43.000000 bourbaki.introspection-0.5.8/bourbaki/introspection/types/abcs.py
--rw-r--r--   0 matt      (1000) matt      (1000)     9548 2020-04-05 20:27:24.000000 bourbaki.introspection-0.5.8/bourbaki/introspection/types/compat.py
--rw-r--r--   0 matt      (1000) matt      (1000)     9005 2020-04-05 20:23:48.000000 bourbaki.introspection-0.5.8/bourbaki/introspection/types/evaluation.py
--rw-r--r--   0 matt      (1000) matt      (1000)     4851 2019-12-30 04:08:17.000000 bourbaki.introspection-0.5.8/bourbaki/introspection/types/inspection.py
--rw-r--r--   0 matt      (1000) matt      (1000)    11156 2020-04-02 05:15:44.000000 bourbaki.introspection-0.5.8/bourbaki/introspection/types/issubclass_generic_.py
--rw-r--r--   0 matt      (1000) matt      (1000)      718 2020-04-11 23:29:07.000000 bourbaki.introspection-0.5.8/bourbaki/introspection/utils.py
--rw-r--r--   0 matt      (1000) matt      (1000)      999 2020-02-09 17:22:31.000000 bourbaki.introspection-0.5.8/bourbaki/introspection/wrappers.py
-drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2020-04-12 02:07:24.000000 bourbaki.introspection-0.5.8/bourbaki.introspection.egg-info/
--rw-r--r--   0 matt      (1000) matt      (1000)     1127 2020-04-12 02:07:24.000000 bourbaki.introspection-0.5.8/bourbaki.introspection.egg-info/PKG-INFO
--rw-r--r--   0 matt      (1000) matt      (1000)     1312 2020-04-12 02:07:24.000000 bourbaki.introspection-0.5.8/bourbaki.introspection.egg-info/SOURCES.txt
--rw-r--r--   0 matt      (1000) matt      (1000)        1 2020-04-12 02:07:24.000000 bourbaki.introspection-0.5.8/bourbaki.introspection.egg-info/dependency_links.txt
--rw-r--r--   0 matt      (1000) matt      (1000)       69 2020-04-12 02:07:24.000000 bourbaki.introspection-0.5.8/bourbaki.introspection.egg-info/requires.txt
--rw-r--r--   0 matt      (1000) matt      (1000)        9 2020-04-12 02:07:24.000000 bourbaki.introspection-0.5.8/bourbaki.introspection.egg-info/top_level.txt
--rw-r--r--   0 matt      (1000) matt      (1000)        1 2020-02-16 03:30:37.000000 bourbaki.introspection-0.5.8/bourbaki.introspection.egg-info/zip-safe
--rw-r--r--   0 matt      (1000) matt      (1000)     1306 2020-04-12 02:07:24.000000 bourbaki.introspection-0.5.8/setup.cfg
--rw-r--r--   0 matt      (1000) matt      (1000)       59 2019-07-21 02:03:19.000000 bourbaki.introspection-0.5.8/setup.py
+drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2020-05-24 16:20:23.000000 bourbaki.introspection-0.5.9/
+-rw-r--r--   0 matt      (1000) matt      (1000)     1127 2020-05-24 16:20:23.000000 bourbaki.introspection-0.5.9/PKG-INFO
+-rw-r--r--   0 matt      (1000) matt      (1000)      308 2020-02-20 08:18:10.000000 bourbaki.introspection-0.5.9/README.md
+drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2020-05-24 16:20:23.000000 bourbaki.introspection-0.5.9/bourbaki/
+-rw-r--r--   0 matt      (1000) matt      (1000)       56 2020-04-02 05:15:43.000000 bourbaki.introspection-0.5.9/bourbaki/__init__.py
+drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2020-05-24 16:20:23.000000 bourbaki.introspection-0.5.9/bourbaki/introspection/
+-rw-r--r--   0 matt      (1000) matt      (1000)      774 2020-05-24 16:20:05.000000 bourbaki.introspection-0.5.9/bourbaki/introspection/__init__.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     4206 2020-04-11 22:55:29.000000 bourbaki.introspection-0.5.9/bourbaki/introspection/builtin_signatures.py
+-rw-r--r--   0 matt      (1000) matt      (1000)    19065 2020-04-11 23:29:28.000000 bourbaki.introspection-0.5.9/bourbaki/introspection/callables.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     3772 2020-05-24 16:16:26.000000 bourbaki.introspection-0.5.9/bourbaki/introspection/classes.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     1115 2020-02-16 07:31:06.000000 bourbaki.introspection-0.5.9/bourbaki/introspection/debug.py
+-rw-r--r--   0 matt      (1000) matt      (1000)    14275 2019-12-30 04:08:16.000000 bourbaki.introspection-0.5.9/bourbaki/introspection/docstrings.py
+-rw-r--r--   0 matt      (1000) matt      (1000)    11889 2020-04-12 01:40:32.000000 bourbaki.introspection-0.5.9/bourbaki/introspection/generic_dispatch.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     6768 2020-05-24 16:13:06.000000 bourbaki.introspection-0.5.9/bourbaki/introspection/generic_dispatch_helpers.py
+-rw-r--r--   0 matt      (1000) matt      (1000)    17742 2020-04-02 05:15:44.000000 bourbaki.introspection-0.5.9/bourbaki/introspection/imports.py
+drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2020-05-24 16:20:23.000000 bourbaki.introspection-0.5.9/bourbaki/introspection/object_models/
+-rw-r--r--   0 matt      (1000) matt      (1000)       46 2019-12-30 04:08:16.000000 bourbaki.introspection-0.5.9/bourbaki/introspection/object_models/__init__.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     8962 2019-12-30 04:08:16.000000 bourbaki.introspection-0.5.9/bourbaki/introspection/object_models/scala.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     3509 2020-04-05 18:27:37.000000 bourbaki.introspection-0.5.9/bourbaki/introspection/polymorphism.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     5761 2020-03-28 03:29:33.000000 bourbaki.introspection-0.5.9/bourbaki/introspection/prettyprint.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     4570 2020-04-12 00:09:35.000000 bourbaki.introspection-0.5.9/bourbaki/introspection/references.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     7099 2020-04-02 05:15:43.000000 bourbaki.introspection-0.5.9/bourbaki/introspection/simple_repr.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     9442 2019-12-30 04:08:17.000000 bourbaki.introspection-0.5.9/bourbaki/introspection/subclassing.py
+-rw-r--r--   0 matt      (1000) matt      (1000)    10193 2020-05-24 16:12:29.000000 bourbaki.introspection-0.5.9/bourbaki/introspection/typechecking.py
+drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2020-05-24 16:20:23.000000 bourbaki.introspection-0.5.9/bourbaki/introspection/types/
+-rw-r--r--   0 matt      (1000) matt      (1000)     1196 2019-12-30 04:08:17.000000 bourbaki.introspection-0.5.9/bourbaki/introspection/types/__init__.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     5041 2020-04-02 05:15:43.000000 bourbaki.introspection-0.5.9/bourbaki/introspection/types/abcs.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     9548 2020-04-05 20:27:24.000000 bourbaki.introspection-0.5.9/bourbaki/introspection/types/compat.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     9005 2020-04-05 20:23:48.000000 bourbaki.introspection-0.5.9/bourbaki/introspection/types/evaluation.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     4851 2019-12-30 04:08:17.000000 bourbaki.introspection-0.5.9/bourbaki/introspection/types/inspection.py
+-rw-r--r--   0 matt      (1000) matt      (1000)    11156 2020-04-02 05:15:44.000000 bourbaki.introspection-0.5.9/bourbaki/introspection/types/issubclass_generic_.py
+-rw-r--r--   0 matt      (1000) matt      (1000)      718 2020-04-11 23:29:07.000000 bourbaki.introspection-0.5.9/bourbaki/introspection/utils.py
+-rw-r--r--   0 matt      (1000) matt      (1000)      999 2020-02-09 17:22:31.000000 bourbaki.introspection-0.5.9/bourbaki/introspection/wrappers.py
+drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2020-05-24 16:20:23.000000 bourbaki.introspection-0.5.9/bourbaki.introspection.egg-info/
+-rw-r--r--   0 matt      (1000) matt      (1000)     1127 2020-05-24 16:20:23.000000 bourbaki.introspection-0.5.9/bourbaki.introspection.egg-info/PKG-INFO
+-rw-r--r--   0 matt      (1000) matt      (1000)     1312 2020-05-24 16:20:23.000000 bourbaki.introspection-0.5.9/bourbaki.introspection.egg-info/SOURCES.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)        1 2020-05-24 16:20:23.000000 bourbaki.introspection-0.5.9/bourbaki.introspection.egg-info/dependency_links.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)       69 2020-05-24 16:20:23.000000 bourbaki.introspection-0.5.9/bourbaki.introspection.egg-info/requires.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)        9 2020-05-24 16:20:23.000000 bourbaki.introspection-0.5.9/bourbaki.introspection.egg-info/top_level.txt
+-rw-r--r--   0 matt      (1000) matt      (1000)        1 2020-02-16 03:30:37.000000 bourbaki.introspection-0.5.9/bourbaki.introspection.egg-info/zip-safe
+-rw-r--r--   0 matt      (1000) matt      (1000)     1306 2020-05-24 16:20:23.000000 bourbaki.introspection-0.5.9/setup.cfg
+-rw-r--r--   0 matt      (1000) matt      (1000)       59 2019-07-21 02:03:19.000000 bourbaki.introspection-0.5.9/setup.py
```

### Comparing `bourbaki.introspection-0.5.8/PKG-INFO` & `bourbaki.introspection-0.5.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bourbaki.introspection
-Version: 0.5.8
+Version: 0.5.9
 Summary: UNKNOWN
 Home-page: https://github.com/bourbaki-py
 Author: Matthew Hawthorn
 Author-email: hawthorn.matthew@gmail.com
 License: Apache License 2.0
 Description: [![Build Status](https://travis-ci.org/bourbaki-py/introspection.svg?branch=master)](https://travis-ci.org/bourbaki-py/introspection)
         [![Coverage Status](https://coveralls.io/repos/github/bourbaki-py/introspection/badge.svg?branch=master)](https://coveralls.io/github/bourbaki-py/introspection?branch=master)
```

### Comparing `bourbaki.introspection-0.5.8/bourbaki/introspection/__init__.py` & `bourbaki.introspection-0.5.9/bourbaki/introspection/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 from .references import find_refs, find_refs_by_type, find_refs_by_id, find_refs_by_size
 from .simple_repr import with_simple_repr
 from .subclassing import subclass_method, subclass_mutator_method
 from .typechecking import type_checker
 from .types import issubclass_generic
 from .wrappers import cached_getter, lru_cache_sig_preserving
 
-__version__ = "0.5.8"
+__version__ = "0.5.9"
```

### Comparing `bourbaki.introspection-0.5.8/bourbaki/introspection/builtin_signatures.py` & `bourbaki.introspection-0.5.9/bourbaki/introspection/builtin_signatures.py`

 * *Files identical despite different names*

### Comparing `bourbaki.introspection-0.5.8/bourbaki/introspection/callables.py` & `bourbaki.introspection-0.5.9/bourbaki/introspection/callables.py`

 * *Files identical despite different names*

### Comparing `bourbaki.introspection-0.5.8/bourbaki/introspection/classes.py` & `bourbaki.introspection-0.5.9/bourbaki/introspection/classes.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,18 +8,17 @@
 from .types import get_generic_origin, get_generic_args, LazyType, ForwardRef
 
 
 def classpath(t: type):
     org = get_generic_origin(t)
     if org is Union:
         return "Union"
-    if org is Any:
+    elif org is Any:
         return "Any"
-
-    if issubclass(org, LazyType):
+    elif org is LazyType:
         a = get_generic_args(t)[0]
         if isinstance(a, str):
             return a
         elif isinstance(a, ForwardRef):
             return a.__forward_arg__
         else:
             t = a
@@ -33,42 +32,43 @@
 
     # python3.7 new typing module
     classpath = singledispatch(classpath)
 
     def get_qualname(t: type):
         if t.__module__ == "typing" and isinstance(t, _GenericAlias):
             return t._name
-        return getattr(t, "__qualname__", get_generic_origin(t).__qualname__)
+        return getattr(t, "__qualname__", getattr(t, "__name__"))
 
     @classpath.register(_GenericAlias)
     def classpath_generic_alias(t: _GenericAlias):
         if t.__module__ == "typing":
             return t._name
         return "{}.{}".format(t.__module__, get_qualname(t))
 
 
 else:
-
     def get_qualname(t: type):
-        return getattr(t, "__qualname__", get_generic_origin(t).__qualname__)
+        return getattr(t, "__qualname__", gettr(t, "__name__"))
 
 
 def parameterized_classpath(t: type):
     def _inner(t):
         if t is Ellipsis:
             return "..."
         if isinstance(t, list):
             # for callables
             return "[{}]".format(",".join(map(_inner, t)))
         return parameterized_classpath(t)
 
     args = get_generic_args(t, evaluate=True)
     origin = get_generic_origin(t)
+    print("PARAM CLSS")
     if not args:
-        return classpath(origin)
+        print("NO ARGS")
+        return classpath(t)
     return "{}[{}]".format(classpath(origin), ",".join(map(_inner, args)))
 
 
 def most_specific_constructor(t: type, return_class=False):
     # first class in mro, preferring __new__ over __init__
     # note that this is different than getattr(t, "__new__", getattr(t, "__init__)),
     # since t.__new__ is usually higher up in the mro, e.g. object.__new__
```

### Comparing `bourbaki.introspection-0.5.8/bourbaki/introspection/debug.py` & `bourbaki.introspection-0.5.9/bourbaki/introspection/debug.py`

 * *Files identical despite different names*

### Comparing `bourbaki.introspection-0.5.8/bourbaki/introspection/docstrings.py` & `bourbaki.introspection-0.5.9/bourbaki/introspection/docstrings.py`

 * *Files identical despite different names*

### Comparing `bourbaki.introspection-0.5.8/bourbaki/introspection/generic_dispatch.py` & `bourbaki.introspection-0.5.9/bourbaki/introspection/generic_dispatch.py`

 * *Files identical despite different names*

### Comparing `bourbaki.introspection-0.5.8/bourbaki/introspection/generic_dispatch_helpers.py` & `bourbaki.introspection-0.5.9/bourbaki/introspection/generic_dispatch_helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # coding:utf-8
 from typing import Generic
 import collections
 from functools import partial
 from inspect import Parameter
+from itertools import repeat
 from .wrappers import cached_getter
 from .imports import import_type
 from .utils import identity
 from .types.evaluation import deconstruct_generic, reconstruct_generic
 from .types.inspection import is_named_tuple_class, get_named_tuple_arg_types
 from .types.compat import get_constructor_for
 
@@ -81,39 +82,38 @@
         self.val_func = self.getter(val_type)
 
     def call_iter(self, arg):
         return (self.val_func(a) for a in arg)
 
 
 class TupleWrapper(ReducingGenericWrapper):
-    _collection_cls = CollectionWrapper
     require_same_len = True
 
-    def __new__(cls, tup_type, *types):
+    def __init__(self, tup_type, *types):
+        super().__init__(tup_type, *types)
         if is_named_tuple_class(tup_type) and not types:
             types = get_named_tuple_arg_types(tup_type)
+
         if not types:
-            cls = cls._collection_cls
+            self.require_same_len = False
+            self.funcs = (self.getter(object),)
         elif types[-1] is Ellipsis:
             # variable-length, uniformly-typed tuple
-            cls = cls._collection_cls
-            types = types[:1]
-
-        new = object.__new__(cls)
-        cls.__init__(new, tup_type, *types)
-        return new
-
-    def __init__(self, tup_type, *types):
-        super().__init__(tup_type, *types)
-        if not getattr(self, "funcs", None):
-            # somehow this is being called twice in some instances - haven't identified the source
+            self.require_same_len = False
+            self.funcs = (self.getter(types[0]),)
+        else:
+            self.require_same_len = True
             self.funcs = tuple(self.getter(t) for t in types)
 
     def call_iter(self, arg):
-        return (d(v) for d, v in zip(self.funcs, arg))
+        if not self.require_same_len:
+            f = self.funcs[0]
+            return map(f, arg)
+        else:
+            return (d(v) for d, v in zip(self.funcs, arg))
 
     def __call__(self, value):
         if self.require_same_len and len(value) != len(self.funcs):
             raise ValueError(
                 "{} expected a collection of {} values for type {} but received {}".format(
                     self, len(self.funcs), self.type_, value
                 )
@@ -123,16 +123,15 @@
 
 class NamedTupleWrapper(TupleWrapper):
     reduce_named = None
     get_named_reducer = staticmethod(identity)
 
     def __init__(self, tup_type, *types):
         super().__init__(tup_type, *types)
-        if not getattr(self, "named_funcs", None):
-            self.named_funcs = dict(zip(tup_type._fields, self.funcs))
+        self.named_funcs = dict(zip(tup_type._fields, self.funcs))
         if self.reduce_named is None:
             self.reduce_named = self.get_named_reducer(tup_type)
 
     def __call__(self, value):
         if isinstance(value, collections.Mapping):
             kwargs = ((name, self.named_funcs[name](v)) for name, v in value.items())
             return self.reduce_named(kwargs)
```

### Comparing `bourbaki.introspection-0.5.8/bourbaki/introspection/imports.py` & `bourbaki.introspection-0.5.9/bourbaki/introspection/imports.py`

 * *Files identical despite different names*

### Comparing `bourbaki.introspection-0.5.8/bourbaki/introspection/object_models/scala.py` & `bourbaki.introspection-0.5.9/bourbaki/introspection/object_models/scala.py`

 * *Files identical despite different names*

### Comparing `bourbaki.introspection-0.5.8/bourbaki/introspection/polymorphism.py` & `bourbaki.introspection-0.5.9/bourbaki/introspection/polymorphism.py`

 * *Files identical despite different names*

### Comparing `bourbaki.introspection-0.5.8/bourbaki/introspection/prettyprint.py` & `bourbaki.introspection-0.5.9/bourbaki/introspection/prettyprint.py`

 * *Files identical despite different names*

### Comparing `bourbaki.introspection-0.5.8/bourbaki/introspection/references.py` & `bourbaki.introspection-0.5.9/bourbaki/introspection/references.py`

 * *Files identical despite different names*

### Comparing `bourbaki.introspection-0.5.8/bourbaki/introspection/simple_repr.py` & `bourbaki.introspection-0.5.9/bourbaki/introspection/simple_repr.py`

 * *Files identical despite different names*

### Comparing `bourbaki.introspection-0.5.8/bourbaki/introspection/subclassing.py` & `bourbaki.introspection-0.5.9/bourbaki/introspection/subclassing.py`

 * *Files identical despite different names*

### Comparing `bourbaki.introspection-0.5.8/bourbaki/introspection/typechecking.py` & `bourbaki.introspection-0.5.9/bourbaki/introspection/typechecking.py`

 * *Files 2% similar despite different names*

```diff
@@ -266,30 +266,20 @@
 class MappingTypeChecker(_GenericContainerTypeCheckerMixin, MappingWrapper):
     helper_cls = MappingWrapper
     keyval_op = staticmethod(operator.and_)
 
 
 @type_checker.register(typing.Tuple)
 class TupleTypeChecker(_GenericContainerTypeCheckerMixin, TupleWrapper):
-    _collection_cls = CollectionTypeChecker
-    require_same_len = False
     helper_cls = TupleWrapper
 
-    def __new__(cls, tup_type, *args):
-        if not args:
-            return isinstance_of(tup_type)
-        return TupleWrapper.__new__(cls, tup_type, *args)
-
     def __call__(self, value):
-        try:
-            len_ = len(value)
-        except TypeError:
-            return super().__call__(value)
-        else:
-            return len(self.funcs) == len_ and super().__call__(value)
+        if not isinstance(value, self.generic_type):
+            return False
+        return super().__call__(value)
 
 
 @type_checker.register(typing.Union)
 class UnionTypeChecker(_GenericUnionTypeCheckerMixin, UnionWrapper):
     pass
```

### Comparing `bourbaki.introspection-0.5.8/bourbaki/introspection/types/__init__.py` & `bourbaki.introspection-0.5.9/bourbaki/introspection/types/__init__.py`

 * *Files identical despite different names*

### Comparing `bourbaki.introspection-0.5.8/bourbaki/introspection/types/abcs.py` & `bourbaki.introspection-0.5.9/bourbaki/introspection/types/abcs.py`

 * *Files identical despite different names*

### Comparing `bourbaki.introspection-0.5.8/bourbaki/introspection/types/compat.py` & `bourbaki.introspection-0.5.9/bourbaki/introspection/types/compat.py`

 * *Files identical despite different names*

### Comparing `bourbaki.introspection-0.5.8/bourbaki/introspection/types/evaluation.py` & `bourbaki.introspection-0.5.9/bourbaki/introspection/types/evaluation.py`

 * *Files identical despite different names*

### Comparing `bourbaki.introspection-0.5.8/bourbaki/introspection/types/inspection.py` & `bourbaki.introspection-0.5.9/bourbaki/introspection/types/inspection.py`

 * *Files identical despite different names*

### Comparing `bourbaki.introspection-0.5.8/bourbaki/introspection/types/issubclass_generic_.py` & `bourbaki.introspection-0.5.9/bourbaki/introspection/types/issubclass_generic_.py`

 * *Files identical despite different names*

### Comparing `bourbaki.introspection-0.5.8/bourbaki/introspection/utils.py` & `bourbaki.introspection-0.5.9/bourbaki/introspection/utils.py`

 * *Files identical despite different names*

### Comparing `bourbaki.introspection-0.5.8/bourbaki/introspection/wrappers.py` & `bourbaki.introspection-0.5.9/bourbaki/introspection/wrappers.py`

 * *Files identical despite different names*

### Comparing `bourbaki.introspection-0.5.8/bourbaki.introspection.egg-info/PKG-INFO` & `bourbaki.introspection-0.5.9/bourbaki.introspection.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bourbaki.introspection
-Version: 0.5.8
+Version: 0.5.9
 Summary: UNKNOWN
 Home-page: https://github.com/bourbaki-py
 Author: Matthew Hawthorn
 Author-email: hawthorn.matthew@gmail.com
 License: Apache License 2.0
 Description: [![Build Status](https://travis-ci.org/bourbaki-py/introspection.svg?branch=master)](https://travis-ci.org/bourbaki-py/introspection)
         [![Coverage Status](https://coveralls.io/repos/github/bourbaki-py/introspection/badge.svg?branch=master)](https://coveralls.io/github/bourbaki-py/introspection?branch=master)
```

### Comparing `bourbaki.introspection-0.5.8/bourbaki.introspection.egg-info/SOURCES.txt` & `bourbaki.introspection-0.5.9/bourbaki.introspection.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bourbaki.introspection-0.5.8/setup.cfg` & `bourbaki.introspection-0.5.9/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.5.8
+current_version = 0.5.9
 tag = True
 commit = True
 
 [bumpversion:file:bourbaki/introspection/__init__.py]
 
 [bumpversion:file:version.txt]
```

