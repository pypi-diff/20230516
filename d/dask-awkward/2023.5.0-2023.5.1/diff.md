# Comparing `tmp/dask_awkward-2023.5.0.tar.gz` & `tmp/dask_awkward-2023.5.1.tar.gz`

## Comparing `dask_awkward-2023.5.0.tar` & `dask_awkward-2023.5.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 dask_awkward-2023.5.0/src/dask_awkward/__init__.py
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 dask_awkward-2023.5.0/src/dask_awkward/awkward.yaml
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 dask_awkward-2023.5.0/src/dask_awkward/config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_awkward-2023.5.0/src/dask_awkward/py.typed
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 dask_awkward-2023.5.0/src/dask_awkward/sizeof.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 dask_awkward-2023.5.0/src/dask_awkward/typing.py
--rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 dask_awkward-2023.5.0/src/dask_awkward/utils.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 dask_awkward-2023.5.0/src/dask_awkward/version.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 dask_awkward-2023.5.0/src/dask_awkward/version.pyi
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 dask_awkward-2023.5.0/src/dask_awkward/layers/__init__.py
--rw-r--r--   0        0        0     6836 2020-02-02 00:00:00.000000 dask_awkward-2023.5.0/src/dask_awkward/layers/layers.py
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 dask_awkward-2023.5.0/src/dask_awkward/lib/__init__.py
--rw-r--r--   0        0        0    61467 2020-02-02 00:00:00.000000 dask_awkward-2023.5.0/src/dask_awkward/lib/core.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 dask_awkward-2023.5.0/src/dask_awkward/lib/describe.py
--rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 dask_awkward-2023.5.0/src/dask_awkward/lib/inspect.py
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 dask_awkward-2023.5.0/src/dask_awkward/lib/operations.py
--rw-r--r--   0        0        0    15255 2020-02-02 00:00:00.000000 dask_awkward-2023.5.0/src/dask_awkward/lib/optimize.py
--rw-r--r--   0        0        0    11155 2020-02-02 00:00:00.000000 dask_awkward-2023.5.0/src/dask_awkward/lib/reducers.py
--rw-r--r--   0        0        0    27493 2020-02-02 00:00:00.000000 dask_awkward-2023.5.0/src/dask_awkward/lib/structure.py
--rw-r--r--   0        0        0     5894 2020-02-02 00:00:00.000000 dask_awkward-2023.5.0/src/dask_awkward/lib/testutils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_awkward-2023.5.0/src/dask_awkward/lib/io/__init__.py
--rw-r--r--   0        0        0    15411 2020-02-02 00:00:00.000000 dask_awkward-2023.5.0/src/dask_awkward/lib/io/io.py
--rw-r--r--   0        0        0    15172 2020-02-02 00:00:00.000000 dask_awkward-2023.5.0/src/dask_awkward/lib/io/json.py
--rw-r--r--   0        0        0    14183 2020-02-02 00:00:00.000000 dask_awkward-2023.5.0/src/dask_awkward/lib/io/parquet.py
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 dask_awkward-2023.5.0/.gitignore
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 dask_awkward-2023.5.0/LICENSE
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 dask_awkward-2023.5.0/README.md
--rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 dask_awkward-2023.5.0/pyproject.toml
--rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 dask_awkward-2023.5.0/PKG-INFO
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 dask_awkward-2023.5.1/src/dask_awkward/__init__.py
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 dask_awkward-2023.5.1/src/dask_awkward/awkward.yaml
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 dask_awkward-2023.5.1/src/dask_awkward/config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_awkward-2023.5.1/src/dask_awkward/py.typed
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 dask_awkward-2023.5.1/src/dask_awkward/sizeof.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 dask_awkward-2023.5.1/src/dask_awkward/typing.py
+-rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 dask_awkward-2023.5.1/src/dask_awkward/utils.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 dask_awkward-2023.5.1/src/dask_awkward/version.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 dask_awkward-2023.5.1/src/dask_awkward/version.pyi
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 dask_awkward-2023.5.1/src/dask_awkward/layers/__init__.py
+-rw-r--r--   0        0        0     6836 2020-02-02 00:00:00.000000 dask_awkward-2023.5.1/src/dask_awkward/layers/layers.py
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 dask_awkward-2023.5.1/src/dask_awkward/lib/__init__.py
+-rw-r--r--   0        0        0    61467 2020-02-02 00:00:00.000000 dask_awkward-2023.5.1/src/dask_awkward/lib/core.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 dask_awkward-2023.5.1/src/dask_awkward/lib/describe.py
+-rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 dask_awkward-2023.5.1/src/dask_awkward/lib/inspect.py
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 dask_awkward-2023.5.1/src/dask_awkward/lib/operations.py
+-rw-r--r--   0        0        0    15303 2020-02-02 00:00:00.000000 dask_awkward-2023.5.1/src/dask_awkward/lib/optimize.py
+-rw-r--r--   0        0        0    11155 2020-02-02 00:00:00.000000 dask_awkward-2023.5.1/src/dask_awkward/lib/reducers.py
+-rw-r--r--   0        0        0    27429 2020-02-02 00:00:00.000000 dask_awkward-2023.5.1/src/dask_awkward/lib/structure.py
+-rw-r--r--   0        0        0     5894 2020-02-02 00:00:00.000000 dask_awkward-2023.5.1/src/dask_awkward/lib/testutils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_awkward-2023.5.1/src/dask_awkward/lib/io/__init__.py
+-rw-r--r--   0        0        0    15411 2020-02-02 00:00:00.000000 dask_awkward-2023.5.1/src/dask_awkward/lib/io/io.py
+-rw-r--r--   0        0        0    15172 2020-02-02 00:00:00.000000 dask_awkward-2023.5.1/src/dask_awkward/lib/io/json.py
+-rw-r--r--   0        0        0    14183 2020-02-02 00:00:00.000000 dask_awkward-2023.5.1/src/dask_awkward/lib/io/parquet.py
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 dask_awkward-2023.5.1/.gitignore
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 dask_awkward-2023.5.1/LICENSE
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 dask_awkward-2023.5.1/README.md
+-rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 dask_awkward-2023.5.1/pyproject.toml
+-rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 dask_awkward-2023.5.1/PKG-INFO
```

### Comparing `dask_awkward-2023.5.0/src/dask_awkward/awkward.yaml` & `dask_awkward-2023.5.1/src/dask_awkward/awkward.yaml`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.5.0/src/dask_awkward/typing.py` & `dask_awkward-2023.5.1/src/dask_awkward/typing.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.5.0/src/dask_awkward/utils.py` & `dask_awkward-2023.5.1/src/dask_awkward/utils.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.5.0/src/dask_awkward/layers/layers.py` & `dask_awkward-2023.5.1/src/dask_awkward/layers/layers.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.5.0/src/dask_awkward/lib/__init__.py` & `dask_awkward-2023.5.1/src/dask_awkward/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.5.0/src/dask_awkward/lib/core.py` & `dask_awkward-2023.5.1/src/dask_awkward/lib/core.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.5.0/src/dask_awkward/lib/describe.py` & `dask_awkward-2023.5.1/src/dask_awkward/lib/describe.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.5.0/src/dask_awkward/lib/inspect.py` & `dask_awkward-2023.5.1/src/dask_awkward/lib/inspect.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.5.0/src/dask_awkward/lib/operations.py` & `dask_awkward-2023.5.1/src/dask_awkward/lib/operations.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.5.0/src/dask_awkward/lib/optimize.py` & `dask_awkward-2023.5.1/src/dask_awkward/lib/optimize.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 import copy
 import logging
 import warnings
 from collections.abc import Hashable, Mapping
 from typing import TYPE_CHECKING, Any
 
 import dask.config
-from dask.blockwise import Blockwise, fuse_roots, optimize_blockwise
+from dask.blockwise import fuse_roots, optimize_blockwise
 from dask.core import flatten
 from dask.highlevelgraph import HighLevelGraph
 from dask.local import get_sync
 
-from dask_awkward.layers import AwkwardInputLayer
+from dask_awkward.layers import AwkwardBlockwiseLayer, AwkwardInputLayer
 
 log = logging.getLogger(__name__)
 
 
 if TYPE_CHECKING:
     from awkward import Array as AwkwardArray
 
@@ -223,38 +223,38 @@
     layers = {}
     # find chains; each chain list is at least two keys long
     dependents = dsk.dependents
     all_layers = set(dsk.layers)
     while all_layers:
         lay = all_layers.pop()
         val = dsk.layers[lay]
-        if not isinstance(val, Blockwise):
+        if not isinstance(val, AwkwardBlockwiseLayer):
             # shortcut to avoid making comparisons
             layers[lay] = val  # passthrough unchanged
             continue
         children = dependents[lay]
         chain = [lay]
         lay0 = lay
         while (
             len(children) == 1
             and dsk.dependencies[list(children)[0]] == {lay}
-            and isinstance(dsk.layers[list(children)[0]], Blockwise)
+            and isinstance(dsk.layers[list(children)[0]], AwkwardBlockwiseLayer)
             and len(dsk.layers[lay]) == len(dsk.layers[list(children)[0]])
         ):
             # walk forwards
             lay = list(children)[0]
             chain.append(lay)
             all_layers.remove(lay)
             children = dependents[lay]
         lay = lay0
         parents = dsk.dependencies[lay]
         while (
             len(parents) == 1
             and dependents[list(parents)[0]] == {lay}
-            and isinstance(dsk.layers[list(parents)[0]], Blockwise)
+            and isinstance(dsk.layers[list(parents)[0]], AwkwardBlockwiseLayer)
             and len(dsk.layers[lay]) == len(dsk.layers[list(parents)[0]])
         ):
             # walk backwards
             lay = list(parents)[0]
             chain.insert(0, lay)
             all_layers.remove(lay)
             parents = dsk.dependencies[lay]
```

### Comparing `dask_awkward-2023.5.0/src/dask_awkward/lib/reducers.py` & `dask_awkward-2023.5.1/src/dask_awkward/lib/reducers.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.5.0/src/dask_awkward/lib/structure.py` & `dask_awkward-2023.5.1/src/dask_awkward/lib/structure.py`

 * *Files 0% similar despite different names*

```diff
@@ -493,25 +493,24 @@
             highlevel=highlevel,
             behavior=behavior,
         )
 
 
 @borrow_docstring(ak.mask)
 def mask(array, mask, valid_when=True, highlevel=True, behavior=None):
-    # if not compatible_partitions(array, mask):
-    #     raise IncompatiblePartitions("mask", array, mask)
-    # return map_partitions(
-    #     ak.mask,
-    #     array,
-    #     mask,
-    #     valid_when=valid_when,
-    #     highlevel=highlevel,
-    #     behavior=behavior,
-    # )
-    raise DaskAwkwardNotImplemented("TODO")
+    if not compatible_partitions(array, mask):
+        raise IncompatiblePartitions("mask", array, mask)
+    return map_partitions(
+        ak.mask,
+        array,
+        mask,
+        valid_when=valid_when,
+        highlevel=highlevel,
+        behavior=behavior,
+    )
 
 
 @borrow_docstring(ak.nan_to_num)
 def nan_to_num(
     array: Array,
     copy: bool = True,
     nan: float = 0.0,
```

### Comparing `dask_awkward-2023.5.0/src/dask_awkward/lib/testutils.py` & `dask_awkward-2023.5.1/src/dask_awkward/lib/testutils.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.5.0/src/dask_awkward/lib/io/io.py` & `dask_awkward-2023.5.1/src/dask_awkward/lib/io/io.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.5.0/src/dask_awkward/lib/io/json.py` & `dask_awkward-2023.5.1/src/dask_awkward/lib/io/json.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.5.0/src/dask_awkward/lib/io/parquet.py` & `dask_awkward-2023.5.1/src/dask_awkward/lib/io/parquet.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.5.0/.gitignore` & `dask_awkward-2023.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.5.0/LICENSE` & `dask_awkward-2023.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.5.0/README.md` & `dask_awkward-2023.5.1/README.md`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.5.0/pyproject.toml` & `dask_awkward-2023.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.5.0/PKG-INFO` & `dask_awkward-2023.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-awkward
-Version: 2023.5.0
+Version: 2023.5.1
 Summary: Awkward Array meets Dask
 Project-URL: Homepage, https://github.com/dask-contrib/dask-awkward
 Project-URL: Bug Tracker, https://github.com/dask-contrib/dask-awkward/issues
 Author-email: Doug Davis <ddavis@ddavis.io>, Martin Durant <mdurant@anaconda.com>
 Maintainer-email: Doug Davis <ddavis@ddavis.io>, Martin Durant <mdurant@anaconda.com>
 License: BSD-3-Clause
 License-File: LICENSE
```

