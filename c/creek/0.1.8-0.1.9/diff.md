# Comparing `tmp/creek-0.1.8.tar.gz` & `tmp/creek-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "creek-0.1.8.tar", last modified: Wed Sep 29 00:14:24 2021, max compression
+gzip compressed data, was "creek-0.1.9.tar", last modified: Wed Sep 29 17:54:41 2021, max compression
```

## Comparing `creek-0.1.8.tar` & `creek-0.1.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:14:24.833952 creek-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2021-09-29 00:13:51.000000 creek-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3189 2021-09-29 00:14:24.833952 creek-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2216 2021-09-29 00:13:51.000000 creek-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:14:24.829951 creek-0.1.8/creek/
--rw-r--r--   0 runner    (1001) docker     (121)      118 2021-09-29 00:13:51.000000 creek-0.1.8/creek/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4597 2021-09-29 00:13:51.000000 creek-0.1.8/creek/base.py
--rw-r--r--   0 runner    (1001) docker     (121)    25184 2021-09-29 00:13:51.000000 creek-0.1.8/creek/infinite_sequence.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:14:24.833952 creek-0.1.8/creek/scrap/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 00:13:51.000000 creek-0.1.8/creek/scrap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2577 2021-09-29 00:13:51.000000 creek-0.1.8/creek/scrap/creek_layers.py
--rw-r--r--   0 runner    (1001) docker     (121)     4088 2021-09-29 00:13:51.000000 creek-0.1.8/creek/scrap/multi_streams.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:14:24.833952 creek-0.1.8/creek/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 00:13:51.000000 creek-0.1.8/creek/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5060 2021-09-29 00:13:51.000000 creek-0.1.8/creek/tests/infinite_sequence.py
--rw-r--r--   0 runner    (1001) docker     (121)     5074 2021-09-29 00:13:51.000000 creek-0.1.8/creek/tools.py
--rw-r--r--   0 runner    (1001) docker     (121)     1505 2021-09-29 00:13:51.000000 creek-0.1.8/creek/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 00:14:24.833952 creek-0.1.8/creek.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3189 2021-09-29 00:14:24.000000 creek-0.1.8/creek.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      406 2021-09-29 00:14:24.000000 creek-0.1.8/creek.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-29 00:14:24.000000 creek-0.1.8/creek.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-29 00:14:24.000000 creek-0.1.8/creek.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-09-29 00:14:24.000000 creek-0.1.8/creek.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      498 2021-09-29 00:14:24.833952 creek-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       91 2021-09-29 00:13:51.000000 creek-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 17:54:41.246229 creek-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    11357 2021-09-29 17:54:11.000000 creek-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     3189 2021-09-29 17:54:41.246229 creek-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2216 2021-09-29 17:54:11.000000 creek-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 17:54:41.246229 creek-0.1.9/creek/
+-rw-r--r--   0 runner    (1001) docker     (121)      118 2021-09-29 17:54:11.000000 creek-0.1.9/creek/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4597 2021-09-29 17:54:11.000000 creek-0.1.9/creek/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25184 2021-09-29 17:54:11.000000 creek-0.1.9/creek/infinite_sequence.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 17:54:41.246229 creek-0.1.9/creek/scrap/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 17:54:11.000000 creek-0.1.9/creek/scrap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2577 2021-09-29 17:54:11.000000 creek-0.1.9/creek/scrap/creek_layers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4088 2021-09-29 17:54:11.000000 creek-0.1.9/creek/scrap/multi_streams.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 17:54:41.246229 creek-0.1.9/creek/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-29 17:54:11.000000 creek-0.1.9/creek/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5060 2021-09-29 17:54:11.000000 creek-0.1.9/creek/tests/infinite_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6059 2021-09-29 17:54:11.000000 creek-0.1.9/creek/tools.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1505 2021-09-29 17:54:11.000000 creek-0.1.9/creek/util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-29 17:54:41.246229 creek-0.1.9/creek.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3189 2021-09-29 17:54:41.000000 creek-0.1.9/creek.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      406 2021-09-29 17:54:41.000000 creek-0.1.9/creek.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-29 17:54:41.000000 creek-0.1.9/creek.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-29 17:54:41.000000 creek-0.1.9/creek.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2021-09-29 17:54:41.000000 creek-0.1.9/creek.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      498 2021-09-29 17:54:41.246229 creek-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)       91 2021-09-29 17:54:11.000000 creek-0.1.9/setup.py
```

### Comparing `creek-0.1.8/LICENSE` & `creek-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `creek-0.1.8/PKG-INFO` & `creek-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: creek
-Version: 0.1.8
+Version: 0.1.9
 Summary: Simple streams facade
 Home-page: https://github.com/i2mint/creek
 Author: OtoSense
 License: apache-2.0
 Description: # creek
         Simple streams facade.
```

### Comparing `creek-0.1.8/README.md` & `creek-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `creek-0.1.8/creek/base.py` & `creek-0.1.9/creek/base.py`

 * *Files identical despite different names*

### Comparing `creek-0.1.8/creek/infinite_sequence.py` & `creek-0.1.9/creek/infinite_sequence.py`

 * *Files identical despite different names*

### Comparing `creek-0.1.8/creek/scrap/creek_layers.py` & `creek-0.1.9/creek/scrap/creek_layers.py`

 * *Files identical despite different names*

### Comparing `creek-0.1.8/creek/scrap/multi_streams.py` & `creek-0.1.9/creek/scrap/multi_streams.py`

 * *Files identical despite different names*

### Comparing `creek-0.1.8/creek/tests/infinite_sequence.py` & `creek-0.1.9/creek/tests/infinite_sequence.py`

 * *Files identical despite different names*

### Comparing `creek-0.1.8/creek/tools.py` & `creek-0.1.9/creek/tools.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,51 @@
 """Tools to work with creek objects"""
 
-from typing import Union, Any, Callable
+from typing import Union, Any, Callable, Tuple, TypeVar, Iterable
 from dataclasses import dataclass
 
 
 Number = Union[int, float]
 Index = Number
-DataItem = Any
+DataItem = TypeVar('DataItem')
 IndexUpdater = Callable[[Index, DataItem], Index]
+Indexer = Callable[[DataItem], Tuple[Index, DataItem]]
+
+
+def filter_and_index_stream(
+    stream: Iterable, data_item_filt, timestamper: Indexer = enumerate
+):
+    """Index a stream and filter it (based only on the data items).
+
+    >>> assert (
+    ... list(filter_and_index_stream('this  is   a   stream', data_item_filt=' ')) == [
+    ... (0, 't'),
+    ... (1, 'h'),
+    ... (2, 'i'),
+    ... (3, 's'),
+    ... (6, 'i'),
+    ... (7, 's'),
+    ... (11, 'a'),
+    ... (15, 's'),
+    ... (16, 't'),
+    ... (17, 'r'),
+    ... (18, 'e'),
+    ... (19, 'a'),
+    ... (20, 'm')
+    ... ])
+
+    >>> list(filter_and_index_stream(
+    ...     [1, 2, 3, 4, 5, 6, 7, 8],
+    ...     data_item_filt=lambda x: x % 2))
+    [(0, 1), (2, 3), (4, 5), (6, 7)]
+    """
+    if not callable(data_item_filt):
+        sentinel = data_item_filt
+        data_item_filt = lambda x: x != sentinel
+    return filter(lambda x: data_item_filt(x[1]), timestamper(stream))
 
 
 def count_increments(current_idx, obj, step=1):
     return current_idx + step
 
 
 def size_increments(current_idx, obj, size_func=len):
```

### Comparing `creek-0.1.8/creek/util.py` & `creek-0.1.9/creek/util.py`

 * *Files identical despite different names*

### Comparing `creek-0.1.8/creek.egg-info/PKG-INFO` & `creek-0.1.9/creek.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: creek
-Version: 0.1.8
+Version: 0.1.9
 Summary: Simple streams facade
 Home-page: https://github.com/i2mint/creek
 Author: OtoSense
 License: apache-2.0
 Description: # creek
         Simple streams facade.
```

