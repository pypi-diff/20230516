# Comparing `tmp/tinystream-0.0.8.tar.gz` & `tmp/tinystream-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinystream-0.0.8.tar", last modified: Mon May 15 09:48:22 2023, max compression
+gzip compressed data, was "tinystream-0.1.0.tar", last modified: Tue May 16 14:08:38 2023, max compression
```

## Comparing `tinystream-0.0.8.tar` & `tinystream-0.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-05-15 09:48:22.601213 tinystream-0.0.8/
--rw-r--r--   0 mikereiche   (502) staff       (20)     1068 2022-11-24 09:19:16.000000 tinystream-0.0.8/LICENSE
--rw-r--r--   0 mikereiche   (502) staff       (20)     4063 2023-05-15 09:48:22.601088 tinystream-0.0.8/PKG-INFO
--rw-r--r--   0 mikereiche   (502) staff       (20)     3829 2023-05-15 09:48:06.000000 tinystream-0.0.8/README.md
--rw-r--r--   0 mikereiche   (502) staff       (20)       38 2023-05-15 09:48:22.601256 tinystream-0.0.8/setup.cfg
--rw-r--r--   0 mikereiche   (502) staff       (20)      490 2023-05-15 09:48:16.000000 tinystream-0.0.8/setup.py
-drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-05-15 09:48:22.600928 tinystream-0.0.8/tinystream.egg-info/
--rw-r--r--   0 mikereiche   (502) staff       (20)     4063 2023-05-15 09:48:22.000000 tinystream-0.0.8/tinystream.egg-info/PKG-INFO
--rw-r--r--   0 mikereiche   (502) staff       (20)      176 2023-05-15 09:48:22.000000 tinystream-0.0.8/tinystream.egg-info/SOURCES.txt
--rw-r--r--   0 mikereiche   (502) staff       (20)        1 2023-05-15 09:48:22.000000 tinystream-0.0.8/tinystream.egg-info/dependency_links.txt
--rw-r--r--   0 mikereiche   (502) staff       (20)       11 2023-05-15 09:48:22.000000 tinystream-0.0.8/tinystream.egg-info/top_level.txt
--rw-r--r--   0 mikereiche   (502) staff       (20)     6605 2023-05-15 09:48:06.000000 tinystream-0.0.8/tinystream.py
+drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-05-16 14:08:38.090384 tinystream-0.1.0/
+-rw-r--r--   0 mikereiche   (502) staff       (20)     1068 2022-11-24 09:19:16.000000 tinystream-0.1.0/LICENSE
+-rw-r--r--   0 mikereiche   (502) staff       (20)     4152 2023-05-16 14:08:38.090253 tinystream-0.1.0/PKG-INFO
+-rw-r--r--   0 mikereiche   (502) staff       (20)     3918 2023-05-16 11:33:29.000000 tinystream-0.1.0/README.md
+-rw-r--r--   0 mikereiche   (502) staff       (20)       38 2023-05-16 14:08:38.090421 tinystream-0.1.0/setup.cfg
+-rw-r--r--   0 mikereiche   (502) staff       (20)      490 2023-05-16 14:08:26.000000 tinystream-0.1.0/setup.py
+drwxr-xr-x   0 mikereiche   (502) staff       (20)        0 2023-05-16 14:08:38.090077 tinystream-0.1.0/tinystream.egg-info/
+-rw-r--r--   0 mikereiche   (502) staff       (20)     4152 2023-05-16 14:08:38.000000 tinystream-0.1.0/tinystream.egg-info/PKG-INFO
+-rw-r--r--   0 mikereiche   (502) staff       (20)      176 2023-05-16 14:08:38.000000 tinystream-0.1.0/tinystream.egg-info/SOURCES.txt
+-rw-r--r--   0 mikereiche   (502) staff       (20)        1 2023-05-16 14:08:38.000000 tinystream-0.1.0/tinystream.egg-info/dependency_links.txt
+-rw-r--r--   0 mikereiche   (502) staff       (20)       11 2023-05-16 14:08:38.000000 tinystream-0.1.0/tinystream.egg-info/top_level.txt
+-rw-r--r--   0 mikereiche   (502) staff       (20)     6598 2023-05-16 11:27:14.000000 tinystream-0.1.0/tinystream.py
```

### Comparing `tinystream-0.0.8/LICENSE` & `tinystream-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tinystream-0.0.8/PKG-INFO` & `tinystream-0.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinystream
-Version: 0.0.8
+Version: 0.1.0
 Summary: Yet another python streams library
 Home-page: https://github.com/mreiche/python-streams
 Author: Mike Reiche
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![Tests Status](https://github.com/mreiche/python-streams/actions/workflows/tests.yml/badge.svg)
@@ -23,77 +23,84 @@
 
 stream = Stream.of([1, 2, 3, 4, 5]) # of_many(*), of_dict()
 
 stream \
     .map(lambda x: x + 1) \       # flatmap(), peek(), map_key()
     .filter(lambda x: x > 2) \    # filter_key()
     .sorted(int, reverse=True) \  # sort()
-    .reverse() \                  # collect(), count()
+    .reverse() \
     .limit(2) \
     .concat([4]) \
-    .sum()                        # reduce(), max(), min()
+    .sum()                        # reduce(), max(), min(), collect(), count()
 ```
 
+## Aggregators
+
+Aggregator methods like `sum()`, `collect()`, `count()`... will end the stream.
 
 ## Built-in Optional support
 
-Aggregator functions are *optional*:
+Some aggregator functions are *optional*:
+
 ```python
-assert Stream.of((1, 2, 3, 4, 5)).sum().is_empty == False
+assert Stream.of((1, 2, 3, 4, 5)).sum().empty is False
 ```
 
 Get next value as *optional*:
+
 ```python
-Stream.of((1, 2, 3, 4, 5)).next().is_empty = False
+assert Stream.of((1, 2, 3, 4, 5)).next().empty is False
 ```
 
 Create custom *optional*:
+
 ```python
 from tinystream import Opt
 
-assert Opt(None).is_empty is True
+assert Opt(None).empty is True
 ```
 
-Map optional:
+Map *optional*:
 ```python
 assert Opt("String").map(len).get() == 6
 ```
 
 Get default value:
 ```python
 assert Opt(None).get(6) == 6
 assert Opt(None).get(lambda: 6) == 6
 ```
 
 Filter value:
+
 ```python
-assert Opt(0).filter(lambda x: x > 0).is_empty is True
+assert Opt(0).filter(lambda x: x > 0).empty is True
 ```
 
 ## Typehinting
 
 You can typehint datatypes like:
 
 ```python
 from dataclasses import dataclass
 
 @dataclass
 class Node:
     name: str
     parent: "Node" = None
+
+parent = Node(name="B")
+child = Node(name="A", parent=parent)
 ```
 
 for lambdas:
 
 ```python
-parent = Node(name="B")
-child = Node(name="A", parent=parent)
-
 stream = Stream.of([child])
-assert stream.map(lambda x: x.parent, typehint=Node).next().get().name == "B"
+assert stream.map(lambda x: x.parent).type(Node).next().get().name == "B"
 ```
 
 This is not necessary when you pass a mapping function:
 ```python
 def map_parent(n: Node):
     return n.parent
 
@@ -113,18 +120,14 @@
 ```
 
 This is the same like (but without known types):
 ```python
 stream = Stream.of(children)
 ```
 
-## End of stream
-
-Calling methods like `sum()`, `collect()`, `count()`... will end the stream.
-
 ## More features
 
 ### Filter by existing key
 ```python
 items_with_name = Stream.of([child]).filter_key("name")
 ```
 
@@ -137,23 +140,30 @@
 ```python
 list = [
    {"node": Node(name="Node A")},
    {"node": Node(name="Node B")},
    {"node": Node(name="Node C")},
    {"node": Node(name="Node D")},
 ]
-Stream.of(list).map_keys(("node", "name"))
+Stream.of(list).map_keys("node", "name")
 ```
 
 ### Collected join
 
 ```python
 all_names = Stream.of([child]).map_key("name").join(", ")
 ```
 
+### Stream many
+
+```python
+many = Stream.of_many([1, 2, 3], (4, 5, 6))
+many = many.concat([7, 8, 9])
+```
+
 ## Comparison with other libraries
 
 There are a couple of other implementation to fulfill similar requirements.
 
 - https://github.com/alemazzo/Python-Java-Stream
 - https://github.com/ramsteak/streams
 - https://pypi.org/project/fluentpy
```

### Comparing `tinystream-0.0.8/README.md` & `tinystream-0.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -14,77 +14,84 @@
 
 stream = Stream.of([1, 2, 3, 4, 5]) # of_many(*), of_dict()
 
 stream \
     .map(lambda x: x + 1) \       # flatmap(), peek(), map_key()
     .filter(lambda x: x > 2) \    # filter_key()
     .sorted(int, reverse=True) \  # sort()
-    .reverse() \                  # collect(), count()
+    .reverse() \
     .limit(2) \
     .concat([4]) \
-    .sum()                        # reduce(), max(), min()
+    .sum()                        # reduce(), max(), min(), collect(), count()
 ```
 
+## Aggregators
+
+Aggregator methods like `sum()`, `collect()`, `count()`... will end the stream.
 
 ## Built-in Optional support
 
-Aggregator functions are *optional*:
+Some aggregator functions are *optional*:
+
 ```python
-assert Stream.of((1, 2, 3, 4, 5)).sum().is_empty == False
+assert Stream.of((1, 2, 3, 4, 5)).sum().empty is False
 ```
 
 Get next value as *optional*:
+
 ```python
-Stream.of((1, 2, 3, 4, 5)).next().is_empty = False
+assert Stream.of((1, 2, 3, 4, 5)).next().empty is False
 ```
 
 Create custom *optional*:
+
 ```python
 from tinystream import Opt
 
-assert Opt(None).is_empty is True
+assert Opt(None).empty is True
 ```
 
-Map optional:
+Map *optional*:
 ```python
 assert Opt("String").map(len).get() == 6
 ```
 
 Get default value:
 ```python
 assert Opt(None).get(6) == 6
 assert Opt(None).get(lambda: 6) == 6
 ```
 
 Filter value:
+
 ```python
-assert Opt(0).filter(lambda x: x > 0).is_empty is True
+assert Opt(0).filter(lambda x: x > 0).empty is True
 ```
 
 ## Typehinting
 
 You can typehint datatypes like:
 
 ```python
 from dataclasses import dataclass
 
 @dataclass
 class Node:
     name: str
     parent: "Node" = None
+
+parent = Node(name="B")
+child = Node(name="A", parent=parent)
 ```
 
 for lambdas:
 
 ```python
-parent = Node(name="B")
-child = Node(name="A", parent=parent)
-
 stream = Stream.of([child])
-assert stream.map(lambda x: x.parent, typehint=Node).next().get().name == "B"
+assert stream.map(lambda x: x.parent).type(Node).next().get().name == "B"
 ```
 
 This is not necessary when you pass a mapping function:
 ```python
 def map_parent(n: Node):
     return n.parent
 
@@ -104,18 +111,14 @@
 ```
 
 This is the same like (but without known types):
 ```python
 stream = Stream.of(children)
 ```
 
-## End of stream
-
-Calling methods like `sum()`, `collect()`, `count()`... will end the stream.
-
 ## More features
 
 ### Filter by existing key
 ```python
 items_with_name = Stream.of([child]).filter_key("name")
 ```
 
@@ -128,23 +131,30 @@
 ```python
 list = [
    {"node": Node(name="Node A")},
    {"node": Node(name="Node B")},
    {"node": Node(name="Node C")},
    {"node": Node(name="Node D")},
 ]
-Stream.of(list).map_keys(("node", "name"))
+Stream.of(list).map_keys("node", "name")
 ```
 
 ### Collected join
 
 ```python
 all_names = Stream.of([child]).map_key("name").join(", ")
 ```
 
+### Stream many
+
+```python
+many = Stream.of_many([1, 2, 3], (4, 5, 6))
+many = many.concat([7, 8, 9])
+```
+
 ## Comparison with other libraries
 
 There are a couple of other implementation to fulfill similar requirements.
 
 - https://github.com/alemazzo/Python-Java-Stream
 - https://github.com/ramsteak/streams
 - https://pypi.org/project/fluentpy
```

### Comparing `tinystream-0.0.8/tinystream.egg-info/PKG-INFO` & `tinystream-0.1.0/tinystream.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinystream
-Version: 0.0.8
+Version: 0.1.0
 Summary: Yet another python streams library
 Home-page: https://github.com/mreiche/python-streams
 Author: Mike Reiche
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![Tests Status](https://github.com/mreiche/python-streams/actions/workflows/tests.yml/badge.svg)
@@ -23,77 +23,84 @@
 
 stream = Stream.of([1, 2, 3, 4, 5]) # of_many(*), of_dict()
 
 stream \
     .map(lambda x: x + 1) \       # flatmap(), peek(), map_key()
     .filter(lambda x: x > 2) \    # filter_key()
     .sorted(int, reverse=True) \  # sort()
-    .reverse() \                  # collect(), count()
+    .reverse() \
     .limit(2) \
     .concat([4]) \
-    .sum()                        # reduce(), max(), min()
+    .sum()                        # reduce(), max(), min(), collect(), count()
 ```
 
+## Aggregators
+
+Aggregator methods like `sum()`, `collect()`, `count()`... will end the stream.
 
 ## Built-in Optional support
 
-Aggregator functions are *optional*:
+Some aggregator functions are *optional*:
+
 ```python
-assert Stream.of((1, 2, 3, 4, 5)).sum().is_empty == False
+assert Stream.of((1, 2, 3, 4, 5)).sum().empty is False
 ```
 
 Get next value as *optional*:
+
 ```python
-Stream.of((1, 2, 3, 4, 5)).next().is_empty = False
+assert Stream.of((1, 2, 3, 4, 5)).next().empty is False
 ```
 
 Create custom *optional*:
+
 ```python
 from tinystream import Opt
 
-assert Opt(None).is_empty is True
+assert Opt(None).empty is True
 ```
 
-Map optional:
+Map *optional*:
 ```python
 assert Opt("String").map(len).get() == 6
 ```
 
 Get default value:
 ```python
 assert Opt(None).get(6) == 6
 assert Opt(None).get(lambda: 6) == 6
 ```
 
 Filter value:
+
 ```python
-assert Opt(0).filter(lambda x: x > 0).is_empty is True
+assert Opt(0).filter(lambda x: x > 0).empty is True
 ```
 
 ## Typehinting
 
 You can typehint datatypes like:
 
 ```python
 from dataclasses import dataclass
 
 @dataclass
 class Node:
     name: str
     parent: "Node" = None
+
+parent = Node(name="B")
+child = Node(name="A", parent=parent)
 ```
 
 for lambdas:
 
 ```python
-parent = Node(name="B")
-child = Node(name="A", parent=parent)
-
 stream = Stream.of([child])
-assert stream.map(lambda x: x.parent, typehint=Node).next().get().name == "B"
+assert stream.map(lambda x: x.parent).type(Node).next().get().name == "B"
 ```
 
 This is not necessary when you pass a mapping function:
 ```python
 def map_parent(n: Node):
     return n.parent
 
@@ -113,18 +120,14 @@
 ```
 
 This is the same like (but without known types):
 ```python
 stream = Stream.of(children)
 ```
 
-## End of stream
-
-Calling methods like `sum()`, `collect()`, `count()`... will end the stream.
-
 ## More features
 
 ### Filter by existing key
 ```python
 items_with_name = Stream.of([child]).filter_key("name")
 ```
 
@@ -137,23 +140,30 @@
 ```python
 list = [
    {"node": Node(name="Node A")},
    {"node": Node(name="Node B")},
    {"node": Node(name="Node C")},
    {"node": Node(name="Node D")},
 ]
-Stream.of(list).map_keys(("node", "name"))
+Stream.of(list).map_keys("node", "name")
 ```
 
 ### Collected join
 
 ```python
 all_names = Stream.of([child]).map_key("name").join(", ")
 ```
 
+### Stream many
+
+```python
+many = Stream.of_many([1, 2, 3], (4, 5, 6))
+many = many.concat([7, 8, 9])
+```
+
 ## Comparison with other libraries
 
 There are a couple of other implementation to fulfill similar requirements.
 
 - https://github.com/alemazzo/Python-Java-Stream
 - https://github.com/ramsteak/streams
 - https://pypi.org/project/fluentpy
```

### Comparing `tinystream-0.0.8/tinystream.py` & `tinystream-0.1.0/tinystream.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import functools
 import itertools
 import sys
 import warnings
-from typing import Iterable, TypeVar, Callable, List, Dict, Tuple, Iterator, Generic
+from typing import Iterable, TypeVar, Callable, List, Dict, Tuple, Iterator, Generic, Type
 
 T = TypeVar("T")
 R = TypeVar("R")
 K = TypeVar("K")
 
 
 Mapper = Callable[[T], R]
@@ -18,34 +18,39 @@
 
 
 class Opt(Generic[T]):
     def __init__(self, value: T):
         self.__val = value
 
     @property
-    def is_empty(self):
+    def empty(self):
         return self.__val is None
 
+    @property
+    def is_empty(self):
+        warnings.warn("Use empty property instead", DeprecationWarning)
+        return self.empty
+
     def get(self, *args) -> T:
-        if self.__val:
+        if not self.empty:
             return self.__val
         elif len(args) > 0:
             if isinstance(args[0], Callable):
                 return args[0]()
             else:
                 return args[0]
         else:
             raise Exception("Cannot get value of empty Opt without default value")
 
     def if_present(self, consumer: Consumer[T]):
-        if not self.is_empty:
+        if not self.empty:
             consumer(self.get())
 
     def or_else(self, consumer: Callable):
-        if self.is_empty:
+        if self.empty:
             return consumer()
 
     def filter(self, predicate: Predicate[T]):
         if predicate(self.__val):
             return self
         else:
             return Opt(None)
@@ -61,16 +66,16 @@
         return IterableStream[T](iterable)
 
     @staticmethod
     def of_dict(source_dict: Dict[K, T]):
         return IterableStream[Tuple[K, T]](source_dict)
 
     @staticmethod
-    def of_many(typehint: T = None, *iterables):
-        return IterableStream[T]([]).concat(*iterables)
+    def of_many(*iterables):
+        return IterableStream([]).concat(*iterables)
 
 
 class IterableStream(Iterator[T]):
 
     def __next__(self) -> T | None:
         try:
             return next(self.__iterable)
@@ -102,21 +107,23 @@
             if isinstance(x, (list, dict, tuple)):
                 return x[key]
             else:
                 return getattr(x, key)
 
         return self.filter_key(key).map(__map_key, R)
 
-    def map_keys(self, keys: Iterable[str], typehint: R = None) -> "IterableStream[R]":
-        assert not isinstance(keys, (int, str))
+    def map_keys(self, *iterables) -> "IterableStream":
         inst = self
-        for key in keys:
+        for key in iterables:
             inst = inst.map_key(key)
         return inst
 
+    def type(self, typehint: R) -> "IterableStream[R]":
+        return self
+
     def filter(self, predicate: Predicate[T]):
         return IterableStream[T](filter(predicate, self.__iterable))
 
     def filter_key(self, key: str | int, invert: bool = False):
         def __filter_key(x):
             if isinstance(x, (list, tuple)):
                 size = len(x)
@@ -133,15 +140,15 @@
                 if invert:
                     return not hasattr(x, key)
                 else:
                     return hasattr(x, key)
 
         return self.filter(__filter_key)
 
-    def flatmap(self, mapper: FlatMapper[T, R] = None, typehint: R = None):
+    def flatmap(self, mapper: FlatMapper[T, R] = None, typehint: R = None) -> "IterableStream[R]":
 
         def __flatmap(f, xs):
             return (y for ys in xs for y in f(ys))
 
         def __flatten(xs):
             return (y for ys in xs for y in ys)
 
@@ -162,18 +169,14 @@
         sort = sorted(self.__iterable, key=key, reverse=reverse)
         return IterableStream[T](sort)
 
     def sorted(self, key, reverse: bool = False):
         sort = sorted(self.__iterable, key=key, reverse=reverse)
         return IterableStream[T](sort)
 
-    def each(self) -> Iterable[T]:
-        warnings.warn("Use the stream as iterator instead", DeprecationWarning)
-        return self.__iterable
-
     def next(self) -> Opt[T]:
         return Opt(self.__next__())
 
     def collect(self):
         """Collects all items to a list and ends the stream"""
         if not self.__collected:
             self.__collected = list(self.__iterable)
```

