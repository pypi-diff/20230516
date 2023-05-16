# Comparing `tmp/unitrack-4.3.2.tar.gz` & `tmp/unitrack-4.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitrack-4.3.2.tar", last modified: Wed May  3 09:31:38 2023, max compression
+gzip compressed data, was "unitrack-4.5.0.tar", last modified: Tue May 16 12:16:08 2023, max compression
```

## Comparing `unitrack-4.3.2.tar` & `unitrack-4.5.0.tar`

### file list

```diff
@@ -1,44 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 09:31:38.307174 unitrack-4.3.2/
--rw-rw-rw-   0        0        0     1068 2023-03-15 15:59:33.000000 unitrack-4.3.2/LICENSE
--rw-rw-rw-   0        0        0      748 2023-05-03 09:31:38.306137 unitrack-4.3.2/PKG-INFO
--rw-rw-rw-   0        0        0       75 2023-03-15 15:59:33.000000 unitrack-4.3.2/README.md
--rw-rw-rw-   0        0        0     6351 2023-05-03 06:02:40.000000 unitrack-4.3.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-03 09:31:38.307174 unitrack-4.3.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-03 09:31:38.253302 unitrack-4.3.2/sources/
-drwxrwxrwx   0        0        0        0 2023-05-03 09:31:38.262569 unitrack-4.3.2/sources/unitrack/
--rw-rw-rw-   0        0        0      786 2023-05-03 09:30:42.000000 unitrack-4.3.2/sources/unitrack/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:31:38.289718 unitrack-4.3.2/sources/unitrack/assignment/
--rw-rw-rw-   0        0        0      253 2023-05-03 06:02:40.000000 unitrack-4.3.2/sources/unitrack/assignment/__init__.py
--rw-rw-rw-   0        0        0     2488 2023-05-03 06:02:40.000000 unitrack-4.3.2/sources/unitrack/assignment/auction.py
--rw-rw-rw-   0        0        0      718 2023-05-03 06:02:40.000000 unitrack-4.3.2/sources/unitrack/assignment/base_assignment.py
--rw-rw-rw-   0        0        0     2123 2023-05-03 06:02:40.000000 unitrack-4.3.2/sources/unitrack/assignment/greedy.py
--rw-rw-rw-   0        0        0     5521 2023-05-03 06:02:40.000000 unitrack-4.3.2/sources/unitrack/assignment/hungarian.py
--rw-rw-rw-   0        0        0     1739 2023-05-03 06:02:40.000000 unitrack-4.3.2/sources/unitrack/assignment/jonker.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:31:38.294932 unitrack-4.3.2/sources/unitrack/costs/
--rw-rw-rw-   0        0        0      203 2023-03-16 08:48:52.000000 unitrack-4.3.2/sources/unitrack/costs/__init__.py
--rw-rw-rw-   0        0        0     2453 2023-05-03 06:02:40.000000 unitrack-4.3.2/sources/unitrack/costs/base_cost.py
--rw-rw-rw-   0        0        0      711 2023-03-16 08:48:52.000000 unitrack-4.3.2/sources/unitrack/costs/category.py
--rw-rw-rw-   0        0        0     3829 2023-05-03 06:02:40.000000 unitrack-4.3.2/sources/unitrack/costs/iou.py
--rw-rw-rw-   0        0        0     3092 2023-05-03 06:02:40.000000 unitrack-4.3.2/sources/unitrack/costs/wrap.py
--rw-rw-rw-   0        0        0     2627 2023-05-03 06:02:40.000000 unitrack-4.3.2/sources/unitrack/detections.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:31:38.298211 unitrack-4.3.2/sources/unitrack/fields/
--rw-rw-rw-   0        0        0      129 2023-05-03 06:02:40.000000 unitrack-4.3.2/sources/unitrack/fields/__init__.py
--rw-rw-rw-   0        0        0     2925 2023-03-16 08:48:52.000000 unitrack-4.3.2/sources/unitrack/fields/base_field.py
--rw-rw-rw-   0        0        0      581 2023-03-16 08:48:52.000000 unitrack-4.3.2/sources/unitrack/fields/value.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:31:38.301221 unitrack-4.3.2/sources/unitrack/stages/
--rw-rw-rw-   0        0        0      128 2023-05-03 06:02:40.000000 unitrack-4.3.2/sources/unitrack/stages/__init__.py
--rw-rw-rw-   0        0        0     1325 2023-05-03 06:02:40.000000 unitrack-4.3.2/sources/unitrack/stages/association.py
--rw-rw-rw-   0        0        0     1726 2023-05-03 06:02:40.000000 unitrack-4.3.2/sources/unitrack/stages/base_stage.py
--rw-rw-rw-   0        0        0     1168 2023-05-03 06:02:40.000000 unitrack-4.3.2/sources/unitrack/stages/lost.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:31:38.305129 unitrack-4.3.2/sources/unitrack/states/
--rw-rw-rw-   0        0        0      127 2023-05-03 06:02:40.000000 unitrack-4.3.2/sources/unitrack/states/__init__.py
--rw-rw-rw-   0        0        0     1220 2023-03-16 08:48:52.000000 unitrack-4.3.2/sources/unitrack/states/base_state.py
--rw-rw-rw-   0        0        0     2015 2023-03-16 08:48:52.000000 unitrack-4.3.2/sources/unitrack/states/value.py
--rw-rw-rw-   0        0        0     4100 2023-05-03 06:02:40.000000 unitrack-4.3.2/sources/unitrack/tracker.py
--rw-rw-rw-   0        0        0     5852 2023-05-03 06:02:40.000000 unitrack-4.3.2/sources/unitrack/tracklets.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:31:38.283692 unitrack-4.3.2/sources/unitrack.egg-info/
--rw-rw-rw-   0        0        0      748 2023-05-03 09:31:38.000000 unitrack-4.3.2/sources/unitrack.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1118 2023-05-03 09:31:38.000000 unitrack-4.3.2/sources/unitrack.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 09:31:38.000000 unitrack-4.3.2/sources/unitrack.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      418 2023-05-03 09:31:38.000000 unitrack-4.3.2/sources/unitrack.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-03 09:31:38.000000 unitrack-4.3.2/sources/unitrack.egg-info/top_level.txt
+drwxrwxr-x   0 khwstolle  (1000) khwstolle  (1000)        0 2023-05-16 12:16:08.319301 unitrack-4.5.0/
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)     1068 2023-05-13 07:58:27.000000 unitrack-4.5.0/LICENSE
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)      729 2023-05-16 12:16:08.319301 unitrack-4.5.0/PKG-INFO
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)       75 2023-05-13 07:58:27.000000 unitrack-4.5.0/README.md
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)     6393 2023-05-16 12:15:34.000000 unitrack-4.5.0/pyproject.toml
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)       38 2023-05-16 12:16:08.319301 unitrack-4.5.0/setup.cfg
+drwxrwxr-x   0 khwstolle  (1000) khwstolle  (1000)        0 2023-05-16 12:16:08.309301 unitrack-4.5.0/sources/
+drwxrwxr-x   0 khwstolle  (1000) khwstolle  (1000)        0 2023-05-16 12:16:08.309301 unitrack-4.5.0/sources/unitrack/
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)      855 2023-05-16 12:15:34.000000 unitrack-4.5.0/sources/unitrack/__init__.py
+drwxrwxr-x   0 khwstolle  (1000) khwstolle  (1000)        0 2023-05-16 12:16:08.319301 unitrack-4.5.0/sources/unitrack/assignment/
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)      275 2023-05-16 12:15:34.000000 unitrack-4.5.0/sources/unitrack/assignment/__init__.py
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)     3512 2023-05-13 07:58:27.000000 unitrack-4.5.0/sources/unitrack/assignment/auction.py
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)     1470 2023-05-13 07:58:27.000000 unitrack-4.5.0/sources/unitrack/assignment/base_assignment.py
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)     2357 2023-05-13 07:58:27.000000 unitrack-4.5.0/sources/unitrack/assignment/greedy.py
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)     2254 2023-05-13 07:58:27.000000 unitrack-4.5.0/sources/unitrack/assignment/hungarian.py
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)     1349 2023-05-13 07:58:27.000000 unitrack-4.5.0/sources/unitrack/assignment/jonker.py
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)      162 2023-05-16 12:15:34.000000 unitrack-4.5.0/sources/unitrack/constants.py
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)     1926 2023-05-16 12:15:34.000000 unitrack-4.5.0/sources/unitrack/context.py
+drwxrwxr-x   0 khwstolle  (1000) khwstolle  (1000)        0 2023-05-16 12:16:08.319301 unitrack-4.5.0/sources/unitrack/costs/
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)      225 2023-05-13 07:58:27.000000 unitrack-4.5.0/sources/unitrack/costs/__init__.py
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)     1125 2023-05-16 12:15:34.000000 unitrack-4.5.0/sources/unitrack/costs/base_cost.py
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)      720 2023-05-16 12:15:34.000000 unitrack-4.5.0/sources/unitrack/costs/category.py
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)     3710 2023-05-16 12:15:34.000000 unitrack-4.5.0/sources/unitrack/costs/iou.py
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)     2224 2023-05-16 12:15:34.000000 unitrack-4.5.0/sources/unitrack/costs/reduce.py
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)     3134 2023-05-16 12:15:34.000000 unitrack-4.5.0/sources/unitrack/costs/wrap.py
+drwxrwxr-x   0 khwstolle  (1000) khwstolle  (1000)        0 2023-05-16 12:16:08.319301 unitrack-4.5.0/sources/unitrack/fields/
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)      129 2023-05-13 07:58:27.000000 unitrack-4.5.0/sources/unitrack/fields/__init__.py
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)     1274 2023-05-16 12:15:34.000000 unitrack-4.5.0/sources/unitrack/fields/base_field.py
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)      485 2023-05-16 12:15:34.000000 unitrack-4.5.0/sources/unitrack/fields/value.py
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)     4043 2023-05-16 12:15:34.000000 unitrack-4.5.0/sources/unitrack/memory.py
+drwxrwxr-x   0 khwstolle  (1000) khwstolle  (1000)        0 2023-05-16 12:16:08.319301 unitrack-4.5.0/sources/unitrack/stages/
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)      128 2023-05-13 07:58:27.000000 unitrack-4.5.0/sources/unitrack/stages/__init__.py
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)     1391 2023-05-16 12:15:34.000000 unitrack-4.5.0/sources/unitrack/stages/association.py
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)     1068 2023-05-16 12:15:34.000000 unitrack-4.5.0/sources/unitrack/stages/base_stage.py
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)     1304 2023-05-16 12:15:34.000000 unitrack-4.5.0/sources/unitrack/stages/lost.py
+drwxrwxr-x   0 khwstolle  (1000) khwstolle  (1000)        0 2023-05-16 12:16:08.319301 unitrack-4.5.0/sources/unitrack/states/
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)      127 2023-05-13 07:58:27.000000 unitrack-4.5.0/sources/unitrack/states/__init__.py
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)      992 2023-05-16 12:15:34.000000 unitrack-4.5.0/sources/unitrack/states/base_state.py
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)     2177 2023-05-16 12:15:34.000000 unitrack-4.5.0/sources/unitrack/states/value.py
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)     2774 2023-05-16 12:15:34.000000 unitrack-4.5.0/sources/unitrack/tracker.py
+drwxrwxr-x   0 khwstolle  (1000) khwstolle  (1000)        0 2023-05-16 12:16:08.309301 unitrack-4.5.0/sources/unitrack.egg-info/
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)      729 2023-05-16 12:16:08.000000 unitrack-4.5.0/sources/unitrack.egg-info/PKG-INFO
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)     1175 2023-05-16 12:16:08.000000 unitrack-4.5.0/sources/unitrack.egg-info/SOURCES.txt
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)        1 2023-05-16 12:16:08.000000 unitrack-4.5.0/sources/unitrack.egg-info/dependency_links.txt
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)      436 2023-05-16 12:16:08.000000 unitrack-4.5.0/sources/unitrack.egg-info/requires.txt
+-rw-rw-r--   0 khwstolle  (1000) khwstolle  (1000)        9 2023-05-16 12:16:08.000000 unitrack-4.5.0/sources/unitrack.egg-info/top_level.txt
```

### Comparing `unitrack-4.3.2/LICENSE` & `unitrack-4.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unitrack-4.3.2/PKG-INFO` & `unitrack-4.5.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1
-Name: unitrack
-Version: 4.3.2
-Summary: A multi-stage object tracking framework
-Author-email: Kurt Stolle <k.h.w.stolle@gmail.com>
-Keywords: perception,computer vision,deep learning,object detection,instance segmentation,semantic segmentation
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: docs
-Provides-Extra: tests
-License-File: LICENSE
-
-# Unified Tracking
-Multi-stage object tracking framework research project.
+Metadata-Version: 2.1
+Name: unitrack
+Version: 4.5.0
+Summary: A multi-stage object tracking framework
+Author-email: Kurt Stolle <k.h.w.stolle@gmail.com>
+Keywords: perception,computer vision,deep learning,object detection,instance segmentation,semantic segmentation
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+Provides-Extra: docs
+Provides-Extra: tests
+License-File: LICENSE
+
+# Unified Tracking
+Multi-stage object tracking framework research project.
```

### Comparing `unitrack-4.3.2/pyproject.toml` & `unitrack-4.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,20 @@
 classifiers = [
     "Development Status :: 4 - Beta",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
 ]
-dependencies = ["torch >= 2.0.0", "scikit-learn >= 1.2.2", "lap >= 0.4.0"]
+dependencies = [
+    "torch >= 2.0.0",
+    "scikit-learn >= 1.2.2",
+    "lap >= 0.4.0",
+    "tensordict >= 0.1.2",
+]
 
 dynamic = ["version"]
 
 [tool.setuptools.dynamic]
 version = { attr = "unitrack.__version__" }
 
 [tool.setuptools.packages.find]
```

### Comparing `unitrack-4.3.2/sources/unitrack/assignment/base_assignment.py` & `unitrack-4.5.0/sources/unitrack/assignment/base_assignment.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,55 @@
+from abc import abstractmethod
 from typing import Tuple
 
 import torch
 
 __all__ = ["Assignment"]
 
 
 class Assignment(torch.nn.Module):
     """
     Solves a linear assignment problem (LAP).
     """
 
     threshold: float
 
-    def __init__(self, threshold: float = 1.0):
+    def __init__(self, threshold: float = torch.inf):
         super().__init__()
 
         self.threshold = threshold
 
+    @torch.jit.script_if_tracing
     def forward(self, cost_matrix: torch.Tensor) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
         """
         Solve the cost matrix
 
         Parameters
         ----------
         cost_matrix
             Cost matrix (NxM) to solve
 
         Returns
         -------
             Tuple of matches (N_match x M_match), unmatched columns and
             unmatched rows
         """
+
+        if min(cost_matrix.shape) == 0:
+            return self._no_match(cost_matrix)
+
+        cost_matrix = cost_matrix * (cost_matrix < self.threshold).type_as(cost_matrix)
+
+        return self._assign(cost_matrix)
+
+    @staticmethod
+    def _no_match(cost_matrix: torch.Tensor) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
+        cs_num, ds_num = cost_matrix.shape
+        return (
+            torch.empty((0, 2), dtype=torch.long),
+            torch.arange(cs_num, dtype=torch.long),
+            torch.arange(ds_num, dtype=torch.long),
+        )
+
+    @abstractmethod
+    def _assign(self, cost_matrix: torch.Tensor) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
         raise NotImplementedError
```

### Comparing `unitrack-4.3.2/sources/unitrack/assignment/greedy.py` & `unitrack-4.5.0/sources/unitrack/assignment/greedy.py`

 * *Files 27% similar despite different names*

```diff
@@ -7,53 +7,66 @@
 
 from typing import Tuple
 
 import torch
 
 from .base_assignment import Assignment
 
+__all__ = ["Greedy", "greedy_assignment"]
 
-class GreedyAssignment(Assignment):
-    def forward(self, cost_matrix: torch.Tensor) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
-        """
-        Assigns detections to tracklets using a greedy algorithm. This algorithm
-        is not guaranteed to find the optimal solution, but it is fast and
-        simple to implement.
-
-        Parameters
-        ----------
-        cost_matrix
-            Cost matrix (NxM) to solve
-
-        Returns
-        -------
-            Tuple of matches (N_match x M_match), unmatched columns and
-            unmatched rows
-        """
-
-        num_rows, num_cols = cost_matrix.shape
-
-        unmatched_rows = torch.arange(num_rows, device=cost_matrix.device)
-        unmatched_cols = torch.arange(num_cols, device=cost_matrix.device)
-
-        if cost_matrix.numel() == 0:
-            return (
-                torch.zeros((0, 2), dtype=torch.long, device=cost_matrix.device),
-                unmatched_rows,
-                unmatched_cols,
-            )
-
-        # Greedy assignment
-        matches = []
-        while unmatched_rows.numel() > 0 and unmatched_cols.numel() > 0:
-            # Find minimum cost match
-            row_idx = torch.argmin(cost_matrix[unmatched_rows[:, None], unmatched_cols], dim=1)
-            col_idx = torch.arange(unmatched_cols.shape[0], device=cost_matrix.device)[row_idx]
-
-            # Add match
-            matches.append(torch.stack([unmatched_rows[row_idx], unmatched_cols[col_idx]], dim=1))
-
-            # Remove matched rows and columns
-            unmatched_rows = torch.cat([unmatched_rows[:row_idx], unmatched_rows[row_idx + 1 :]])
-            unmatched_cols = torch.cat([unmatched_cols[:col_idx], unmatched_cols[col_idx + 1 :]])
 
-        return torch.cat(matches, dim=0), unmatched_rows, unmatched_cols
+class Greedy(Assignment):
+    """
+    See :func:`.greedy_assignment` for details.
+    """
+
+    def _assign(self, cost_matrix: torch.Tensor) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
+        return greedy_assignment(cost_matrix)
+
+
+@torch.jit.script_if_tracing
+@torch.no_grad()
+def greedy_assignment(cost_matrix: torch.Tensor) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
+    """
+    Performs a greedy assignment algorithm on a cost matrix, assigning pairs of elements (rows and columns) based on
+    the minimum cost, with a threshold as the stopping condition.
+
+    Parameters
+    ----------
+    cost_matrix : torch.Tensor
+        A 2D tensor representing the cost matrix.
+    threshold : float
+        The maximum cost allowed for an assignment.
+
+    Returns
+    -------
+    matches : torch.Tensor
+        A tensor containing the indices of matched row-column pairs.
+    unmatched_rows : torch.Tensor
+        A tensor containing the indices of unmatched rows.
+    unmatched_cols : torch.Tensor
+        A tensor containing the indices of unmatched columns.
+
+    """
+    N, M = cost_matrix.shape
+    matches = torch.full((min(N, M), 2), -1, dtype=torch.long, device=cost_matrix.device)
+    unmatched_rows = torch.arange(N, dtype=torch.long, device=cost_matrix.device)
+    unmatched_cols = torch.arange(M, dtype=torch.long, device=cost_matrix.device)
+
+    match_count = 0
+    while True:
+        min_val, idx = torch.min(cost_matrix.flatten(), dim=0)
+        row, col = idx // M, idx % M
+
+        if not torch.isfinite(min_val):
+            break
+
+        matches[match_count] = torch.tensor([row, col], dtype=torch.long, device=cost_matrix.device)
+        match_count += 1
+
+        cost_matrix[row, :] = torch.inf
+        cost_matrix[:, col] = torch.inf
+
+    unmatched_rows = unmatched_rows[torch.isfinite(cost_matrix[:, 0])]
+    unmatched_cols = unmatched_cols[torch.isfinite(cost_matrix[0, :])]
+
+    return matches[:match_count], unmatched_rows, unmatched_cols
```

### Comparing `unitrack-4.3.2/sources/unitrack/assignment/jonker.py` & `unitrack-4.5.0/sources/unitrack/assignment/jonker.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,53 +2,47 @@
 
 import numpy as np
 import torch
 from lap import lapjv
 
 from .base_assignment import Assignment
 
-__all__ = ["Jonker"]
+__all__ = ["Jonker", "jonker_volgenant_assignment"]
 
 
 class Jonker(Assignment):
-    def forward(self, cost_matrix: torch.Tensor) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
-        return self.linear_assignment(cost_matrix)
+    def _assign(self, cost_matrix: torch.Tensor) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
+        return jonker_volgenant_assignment(cost_matrix)
 
-    @torch.jit.ignore
-    def linear_assignment(self, cost_matrix: torch.Tensor) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
-        """
-        Perform linear assignment. If possible, an assignment on the diagonal of the
-        matrix is preferred if this assignment has equal cost to the algorithm
-        result.
-
-        TODO: PyTorch implementation
-        """
-
-        cost_matrix = cost_matrix.detach().cpu().numpy()
-        cs_num, ds_num = cost_matrix.shape
-
-        # Skip when cost_matrix has 0-dimension
-        if cost_matrix.size == 0:
-            return (
-                torch.empty((0, 2), dtype=torch.long),
-                torch.arange(cs_num, dtype=torch.long),
-                torch.arange(ds_num, dtype=torch.long),
-            )
-        matches, unmatched_a, unmatched_b = [], [], []
-
-        # Jonker algorithm, i.e. linear sum assignment (rows) -> (cols)
-        cost, x, y = lapjv(cost_matrix, extend_cost=True, cost_limit=self.threshold)
-
-        # Create match and unassigned lists
-        for ix, mx in enumerate(x):
-            if mx >= 0:
-                matches.append([ix, mx])
-
-        unmatched_a = np.where(x < 0)[0]
-        unmatched_b = np.where(y < 0)[0]
-        matches = np.asarray(matches)
-
-        return (
-            torch.from_numpy(matches).long(),
-            torch.from_numpy(unmatched_a).long(),
-            torch.from_numpy(unmatched_b).long(),
-        )
+
+@torch.jit.ignore()
+@torch.no_grad()
+def jonker_volgenant_assignment(cost_matrix: torch.Tensor) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
+    """
+    Perform linear assignment. If possible, an assignment on the diagonal of the
+    matrix is preferred if this assignment has equal cost to the algorithm
+    result.
+
+    TODO: PyTorch implementation
+    """
+
+    cost_matrix = cost_matrix.detach().cpu().numpy()
+
+    matches, unmatched_a, unmatched_b = [], [], []
+
+    # Jonker algorithm, i.e. linear sum assignment (rows) -> (cols)
+    cost, x, y = lapjv(cost_matrix, extend_cost=True)
+
+    # Create match and unassigned lists
+    for ix, mx in enumerate(x):
+        if mx >= 0:
+            matches.append([ix, mx])
+
+    unmatched_a = np.where(x < 0)[0]
+    unmatched_b = np.where(y < 0)[0]
+    matches = np.asarray(matches)
+
+    return (
+        torch.from_numpy(matches).long(),
+        torch.from_numpy(unmatched_a).long(),
+        torch.from_numpy(unmatched_b).long(),
+    )
```

### Comparing `unitrack-4.3.2/sources/unitrack/costs/base_cost.py` & `unitrack-4.5.0/sources/unitrack/costs/reduce.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-from abc import abstractmethod
-from typing import Optional, Sequence
+import enum
+import itertools
+from enum import Enum
+from typing import Callable, Optional, Sequence
 
 import torch
-from torch import Tensor, nn
+import torch.nn as nn
+from tensordict import TensorDictBase
+from torch import Tensor
 
-from ..detections import Detections
+from .base_cost import Cost
 
-__all__ = ["Cost", "WeightedReduce"]
+__all__ = ["Reduce", "Reduction"]
 
 
-class Cost(nn.Module):
+class Weighted(Cost):
     """
-    A cost module computes an assignment cost matrix between detections and
-    tracklets.
+    A weighted cost module.
     """
 
-    def __init__(self, required_fields: tuple[str]):
-        super().__init__()
+    def __init__(self, cost: Cost, weight: float):
+        super().__init__(required_fields=cost.required_fields)
 
-        self.required_fields = required_fields
+        self.cost = cost
+        self.weight = weight
 
-    def forward(self, cs: Detections, ds: Detections) -> Tensor:
-        for field_name in self.required_fields:
-            if field_name not in cs:
-                raise ValueError(f"Missing field '{field_name}' in trackets: {cs}!")
-            if field_name not in ds:
-                raise ValueError(f"Missing field '{field_name}' in detections: {cs}!")
+    def compute(self, cs: TensorDictBase, ds: TensorDictBase) -> torch.Tensor:
+        return self.weight * self.cost(cs, ds)
 
-        return self.compute(cs, ds)
 
-    @abstractmethod
-    def compute(self, cs: Detections, ds: Detections) -> Tensor:
-        """
-        Computes the assignment costs between :class:`.Tracklets` and
-        :class:`.Detections`.
-
-        This is an abstract method that should be overwritten be subclassses.
-
-        Parameters
-        ----------
-        ts
-            Tracklets instance.
-        ds
-            Detections instance.
+class Reduction(Enum):
+    """
+    Reduction method for :class:`.Reduce` cost module.
+    """
 
-        Returns
-        -------
-            Cost matrix
-        """
-        raise NotImplementedError
+    SUM = "sum"
+    MEAN = "mean"
+    MIN = "min"
+    MAX = "max"
+    PRODUCT = "product"
 
 
-class WeightedReduce(Cost):
+class Reduce(Cost):
     """
-    A weighted reduction module.
+    A cost reduction module.
     """
 
-    weights: Tensor
+    weights: torch.Tensor
+    method: torch.jit.Final[Reduction]
 
     def __init__(
         self,
         costs: Sequence[Cost],
+        method: Reduction,
         weights: Optional[Sequence[float]] = None,
-        reduction="sum",
     ):
-        super().__init__(required_fields=tuple(set().union(c.required_fields for c in costs)))
+        super().__init__(required_fields=itertools.chain(*(c.required_fields for c in costs)))
+
+        if isinstance(method, str):
+            method = Reduction(method)
 
-        self.reduction = reduction
+        self.method = method
         self.costs = nn.ModuleList(costs)
         if weights is None:
             weights = [1.0] * len(costs)
 
-        self.register_buffer("weights", torch.tensor(weights, dtype=torch.float))
-
-    def compute(self, cs: Detections, ds: Detections) -> Tensor:
-        costs = torch.stack([w * cost(cs, ds) for w, cost in zip(self.weights, self.costs)])
+        self.register_buffer("weights", torch.tensor(weights, dtype=torch.float32).unsqueeze_(-1).unsqueeze_(-1))
 
-        if self.reduction == "sum":
-            return costs.sum(dim=0)
-        if self.reduction == "mean":
-            return costs.mean(dim=0)
-        if self.reduction == "min":
-            return costs.min(dim=0).values
-        if self.reduction == "max":
-            return costs.max(dim=0).values
-        raise ValueError(f"Unknown reduction: {self.reduction}!")
+    def compute(self, cs: TensorDictBase, ds: TensorDictBase) -> torch.Tensor:
+        costs = torch.stack([cost(cs, ds) for cost in self.costs])
+        costs = costs * self.weights
+        costs = _reduce_stack(costs, self.method)
+
+        return costs
+
+
+@torch.jit.script_if_tracing
+def _reduce_stack(costs: Tensor, method: Reduction) -> Tensor:
+    if method == Reduction.SUM:
+        return costs.sum(dim=0)
+    if method == Reduction.MEAN:
+        return costs.mean(dim=0)
+    if method == Reduction.MIN:
+        return costs.min(dim=0).values
+    if method == Reduction.MAX:
+        return costs.max(dim=0).values
+    raise NotImplementedError(f"Reduction method '{method}' not implemented!")
```

### Comparing `unitrack-4.3.2/sources/unitrack/costs/category.py` & `unitrack-4.5.0/sources/unitrack/costs/category.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import torch
+from tensordict import TensorDictBase
 
-from ..detections import Detections
 from .base_cost import Cost
 
 __all__ = ["CategoryGate"]
 
 
 class CategoryGate(Cost):
     """
     Returns a matrix where each tracklet/detection pair that have equal
     categories are set to `True` and  that have different categories are set to
     `False`.
     """
 
+    field: torch.jit.Final[str]
+
     def __init__(self, field="categories"):
         super().__init__(required_fields=(field,))
 
-        self.field: str = field
+        self.field = field
 
-    def compute(self, cs: Detections, ds: Detections) -> torch.Tensor:
+    def compute(self, cs: TensorDictBase, ds: TensorDictBase) -> torch.Tensor:
         cs_cats = cs.get(self.field)
         ds_cats = ds.get(self.field)
 
         gate_matrix = ds_cats[None, :] - cs_cats[:, None]
 
-        return torch.where(gate_matrix == 0, 1.0, torch.inf)
+        return gate_matrix == 0
```

### Comparing `unitrack-4.3.2/sources/unitrack/costs/iou.py` & `unitrack-4.5.0/sources/unitrack/costs/iou.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,131 +6,126 @@
 version of that package.
 """
 
 
 from typing import Final, Tuple
 
 import torch
+from tensordict import TensorDictBase
 from torch import Tensor
 from torchvision.ops import box_iou
 
-from ..detections import Detections
 from .base_cost import Cost
 
 __all__ = ["MaskIoU", "BoxIoU"]
 
+DEFAULT_EPS: Final = 1e-8
+
 
 class MaskIoU(Cost):
     """
     Computes IoU cost matrix between two sets of bitmasks.
     """
 
-    def __init__(self, field: str):
-        super().__init__(required_fields=(field,))
-
-        self.field_name: Final = field
+    eps: torch.jit.Final[float]
+    field: torch.jit.Final[str]
 
-    def compute(self, cs: Detections, ds: Detections) -> Tensor:
-        cs_m = cs.get(self.field_name).reshape(len(cs), -1).int()
-        ds_m = ds.get(self.field_name).reshape(len(ds), -1).int()
-
-        isec = torch.mm(cs_m, ds_m.T)
-        area = cs_m.sum(dim=1)[:, None] + ds_m.sum(dim=1)[None, :]
+    def __init__(self, field: str, eps: float = DEFAULT_EPS):
+        super().__init__(required_fields=(field,))
 
-        eps = 1e-6
-        iou = (isec + eps) / (area - isec + eps)
+        self.field: Final = field
+        self.eps = eps
 
-        return 1.0 - iou
+    def compute(self, cs: TensorDictBase, ds: TensorDictBase) -> Tensor:
+        return _naive_mask_iou(cs.get(self.field), ds.get(self.field), self.eps)
 
 
 class BoxIoU(Cost):
     """
     Computes the generalized IoU cost matrix between two sets of bounding boxes.
     """
 
-    def __init__(self, field: str):
+    field: torch.jit.Final[str]
+    eps: torch.jit.Final[float]
+
+    def __init__(self, field: str, eps: float = DEFAULT_EPS):
         super().__init__(required_fields=(field,))
 
-        self.field: Final = field
+        self.field = field
+        self.eps = eps
 
-    def compute(self, cs: Detections, ds: Detections) -> Tensor:
+    def compute(self, cs: TensorDictBase, ds: TensorDictBase) -> Tensor:
         cs_field = _pad_degenerate_boxes(cs.get(self.field))
         ds_field = _pad_degenerate_boxes(ds.get(self.field))
 
-        return 1.0 - _complete_box_iou(cs_field, ds_field)
+        return 1.0 - _complete_box_iou(cs_field, ds_field, self.eps)
+
+
+def _naive_mask_iou(cs: Tensor, ds: Tensor, eps: float) -> Tensor:
+    cs_m = cs.reshape(len(cs), -1).int()
+    ds_m = ds.reshape(len(ds), -1).int()
 
+    isec = torch.mm(cs_m, ds_m.T)
+    area = cs_m.sum(dim=1)[:, None] + ds_m.sum(dim=1)[None, :]
 
-@torch.jit.script
-def _pad_degenerate_boxes(boxes: Tensor):
+    iou = (isec + eps) / (area - isec + eps)
+
+    return 1.0 - iou
+
+
+def _pad_degenerate_boxes(boxes: Tensor) -> Tensor:
     """
     Adds 1 to the far-coordinate of each box to prevent degeneracy from mask to
     box conversion.
     """
-    assert boxes.ndim == 2
-
     boxes = boxes.clone()
     boxes[:, 2] += 1
     boxes[:, 3] += 1
 
     return boxes
 
 
-@torch.jit.script
-def _upcast(t: Tensor) -> Tensor:
-    """
-    Protects from numerical overflows in multiplications by upcasting to the
-    equivalent higher type.
-    """
-
-    if t.is_floating_point():
-        return t if t.dtype in (torch.float32, torch.float64) else t.float()
-    else:
-        return t if t.dtype in (torch.int32, torch.int64) else t.int()
-
-
-@torch.jit.script
-def _box_diou_iou(boxes1: Tensor, boxes2: Tensor, eps: float = 1e-7) -> Tuple[Tensor, Tensor]:
+def _box_diou_iou(boxes1: Tensor, boxes2: Tensor, eps: float) -> Tuple[Tensor, Tensor]:
     """
     IoU with penalized center-distance
     """
 
     iou = box_iou(boxes1, boxes2)
     lti = torch.min(boxes1[:, None, :2], boxes2[:, :2])
     rbi = torch.max(boxes1[:, None, 2:], boxes2[:, 2:])
-    whi = _upcast(rbi - lti).clamp(min=0)  # [N,M,2]
-    diagonal_distance_squared = (whi[:, :, 0] ** 2) + (whi[:, :, 1] ** 2) + eps
+    whi = (rbi - lti).float().clamp(min=0)  # [N,M,2]
+    diagonal_distance_squared = (whi[:, :, 0] ** 2) + (whi[:, :, 1] ** 2)
 
     # centers of boxes
     x_p = (boxes1[:, 0] + boxes1[:, 2]) / 2
     y_p = (boxes1[:, 1] + boxes1[:, 3]) / 2
     x_g = (boxes2[:, 0] + boxes2[:, 2]) / 2
     y_g = (boxes2[:, 1] + boxes2[:, 3]) / 2
 
     # The distance between boxes' centers squared.
-    centers_distance_squared = (_upcast((x_p[:, None] - x_g[None, :])) ** 2) + (
-        _upcast((y_p[:, None] - y_g[None, :])) ** 2
+    centers_distance_squared = (((x_p[:, None] - x_g[None, :])).float() ** 2) + (
+        ((y_p[:, None] - y_g[None, :])).float() ** 2
     )
 
     # The distance IoU is the IoU penalized by a normalized
     # distance between boxes' centers squared.
-    return iou - (centers_distance_squared / diagonal_distance_squared), iou
+    return iou - ((centers_distance_squared) / diagonal_distance_squared.clamp(eps)), iou
 
 
-@torch.jit.script_if_tracing
-def _complete_box_iou(boxes1: Tensor, boxes2: Tensor, eps: float = 1e-7) -> Tensor:
-    boxes1 = _upcast(boxes1)
-    boxes2 = _upcast(boxes2)
+def _complete_box_iou(boxes1: Tensor, boxes2: Tensor, eps) -> Tensor:
+    boxes1 = boxes1.float()
+    boxes2 = boxes2.float()
 
     diou, iou = _box_diou_iou(boxes1, boxes2, eps)
 
     w_pred = boxes1[:, None, 2] - boxes1[:, None, 0]
     h_pred = boxes1[:, None, 3] - boxes1[:, None, 1]
 
     w_gt = boxes2[:, 2] - boxes2[:, 0]
     h_gt = boxes2[:, 3] - boxes2[:, 1]
 
     v = (4 / (torch.pi**2)) * torch.pow(torch.atan(w_pred / h_pred) - torch.atan(w_gt / h_gt), 2)
 
     with torch.no_grad():
-        alpha = v / (1 - iou + v + eps)
+        alpha = v / (1 - iou + v).clamp(eps)
 
     return diou - alpha * v
```

### Comparing `unitrack-4.3.2/sources/unitrack/costs/wrap.py` & `unitrack-4.5.0/sources/unitrack/costs/wrap.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from typing import List, Optional, Tuple
+from typing import Final, List, Optional, Tuple
 
 import torch
+from tensordict import TensorDictBase
 from torch import Tensor
 
-from ..detections import Detections
 from .base_cost import Cost
 
-_EPS = torch.finfo(torch.float32).eps
+__all__ = ["Distance", "Cosine"]
 
 
-__all__ = ["Distance", "Cosine"]
+DEFAULT_EPS: Final = 1e-8
 
 
 class Distance(Cost):
     """
     Cost function that wraps a distance module.
     """
 
@@ -49,48 +49,48 @@
         if select is None:
             select = []
 
         self.select = select  # type: ignore
         self.p_norm = p_norm
         self.alpha = alpha
 
-    def get_field(self, cs: Detections, ds: Detections) -> Tuple[torch.Tensor, torch.Tensor]:
+    def get_field(self, cs: TensorDictBase, ds: TensorDictBase) -> Tuple[torch.Tensor, torch.Tensor]:
         ts_field = cs.get(self.field)
         ds_field = ds.get(self.field)
 
         if len(self.select) > 0:
             assert ts_field.shape[1] >= max(self.select)
             assert ds_field.shape[1] >= max(self.select)
 
             ts_field = ts_field[:, self.select]
             ds_field = ds_field[:, self.select]
 
         return ts_field, ds_field
 
-    def compute(self, cs: Detections, ds: Detections):
+    def compute(self, cs: TensorDictBase, ds: TensorDictBase):
         ts_field, ds_field = self.get_field(cs, ds)
         return torch.cdist(ts_field, ds_field, self.p_norm) * self.alpha
 
 
 class Cosine(Distance):
     """
     Computes the distance between two fields based on a similarity measure with
     range $[0,1]$ by computing $1 - S(x,y)$.
     """
 
-    def __init__(self, *args, eps: float = _EPS, **kwargs):
+    def __init__(self, *args, eps: float = DEFAULT_EPS, **kwargs):
         super().__init__(*args, **kwargs)
         self.eps = eps
 
-    def compute(self, cs: Detections, ds: Detections):
+    def compute(self, cs: TensorDictBase, ds: TensorDictBase):
         ts_field, ds_field = self.get_field(cs, ds)
         return (1.0 - _cosine_similarity(ts_field, ds_field, eps=self.eps)) ** self.alpha
 
 
-def _cosine_similarity(a: Tensor, b: Tensor, eps=_EPS) -> Tensor:
+def _cosine_similarity(a: Tensor, b: Tensor, eps=DEFAULT_EPS) -> Tensor:
     """
     Manual computation of the cosine similarity.
 
     Based on: https://stackoverflow.com/questions/50411191/how-to-compute-the-cosine-similarity-in-pytorch-for-all-rows-in-a-matrix-with-re  # noqa: E501
 
     ```
     csim(a,b) = dot(a, b) / (norm(a) * norm(b))
@@ -102,10 +102,10 @@
     """
     a_norm = _stable_norm(a, eps=eps)
     b_norm = _stable_norm(b, eps=eps)
 
     return torch.mm(a_norm, b_norm.T)
 
 
-def _stable_norm(t: torch.Tensor, eps=_EPS):
+def _stable_norm(t: torch.Tensor, eps=DEFAULT_EPS):
     norm = torch.linalg.vector_norm(t, dim=1, keepdim=True)
     return t / norm.clamp(min=eps)
```

### Comparing `unitrack-4.3.2/sources/unitrack/detections.py` & `unitrack-4.5.0/sources/unitrack/tracker.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,82 +1,89 @@
-from typing import Any, Dict, Optional
+from typing import Dict, List, Mapping, Tuple, cast
 
 import torch
+import torch.nn as nn
+from tensordict import TensorDict, TensorDictBase
 
+from .constants import KEY_ACTIVE, KEY_FRAME, KEY_ID, KEY_INDEX, KEY_START
+from .context import Context
+from .fields import Field
+from .stages import Stage
 
-@torch.jit.script
-class Detections:
+
+class MultiStageTracker(nn.Module):
     """
-    Detections is a container class for field and state values for detections at
-    current (field values) and previous (state values) timesteps.
+    Multi-stage tracker that applies a cascade of stages to a set of detections.
     """
 
-    def __init__(
-        self,
-        fields: Dict[str, torch.Tensor],
-        indices: Optional[torch.Tensor] = None,
-        mutable: Optional[bool] = None,
-    ):
-        self._fields = fields
-
-        if mutable is None:
-            mutable = False
-        self.mutable = mutable
-
-        if indices is None:
-            indices = torch.arange(len(self), dtype=torch.long)
-        self.indices = indices
+    def __init__(self, fields: Mapping[str, Field], stages: List[Stage]):
+        super().__init__()
 
-        self._validate()
+        assert len(stages) > 0
 
-    def __getitem__(self, index):
-        select: Dict[str, torch.Tensor] = {}
-        for key, values in self._fields.items():
-            if isinstance(values, torch.Tensor):
-                select[key] = values[index]
-            else:
-                raise TypeError(f"Unsupported field type at key '{key}'!")
-        return Detections(fields=select, indices=self.indices[index], mutable=False)
-
-    def __len__(self):
-        for item in self._fields.values():
-            return len(item)
-        raise NotImplementedError(f"Empty detections class!")
+        self.stages = cast(List[Stage], nn.ModuleList(stages))
+        self.fields = cast(Dict[str, Field], nn.ModuleDict({**fields}))
 
-    def __contains__(self, key: str) -> bool:
-        return key in self._fields.keys()
+        self._validate()
 
-    def get(
+    def _validate(self):
+        for i, stage in enumerate(self.stages):
+            for id in stage.required_fields:
+                if id not in self.fields:
+                    raise ValueError(f"Field with ID '{id}' missing for {stage}!")
+
+    def get_required_fields(self) -> List[str]:
+        field_keys: List[str] = []
+        for f in self.fields.values():
+            field_keys += f.required_keys
+        return field_keys
+
+    def get_required_data(self) -> List[str]:
+        data_keys: List[str] = []
+        for f in self.stages:
+            data_keys += f.required_data
+        return data_keys
+
+    def forward(
         self,
-        key: str,
-    ) -> torch.Tensor:
-        return self._fields[key]
-
-    def set(self, key: str, value: torch.Tensor) -> None:
-        if not self.mutable:
-            raise RuntimeError("Not a mutable collection!")
-        if key not in self:
-            raise ValueError(f"Key '{key}' not in {self}")
-
-        self._fields[key] = value
-
-    def __getattr__(self, key: str) -> Any:
-        if key == "indices":
-            return self.indices
-        if key == "mutable":
-            return self.mutable
-        return self._fields[key]
-
-    def _validate(self) -> None:
-        len_self = len(self)
-        if len(self.indices) != len(self):
-            raise ValueError(f"Indices length {len(self.indices)} not equal to fields " f"length {len_self}!")
-
-        for key, value in self._fields.items():
-            len_value = len(value)
-            if len_self != len_value:
-                raise ValueError(f"Excepted fields of length {len_self} but found '{key}' " f"with length {len_value}!")
-
-    def __repr__(self) -> str:
-        indices: list[int] = self.indices.tolist()
-        field_names: list[str] = list(self._fields.keys())
-        return f"Detections({len(self)}, " f"fields={field_names}, " f"indices={indices}, mutable={self.mutable})"
+        ctx: Context,
+        obs: TensorDictBase,
+    ) -> Tuple[TensorDictBase, TensorDictBase]:
+        """
+        Perform tracking, returns a tuple of updated observations and the field-values of new tracklets.
+
+        Parameters
+        ----------
+        ctx
+            Context object
+        obs
+            Observations
+        det
+            Detections
+
+        Returns
+        -------
+        Tuple[TensorDict, TensorDict]
+            Updated observations and field-values of new tracklets.
+        """
+
+        new = self._apply_fields(ctx)
+        obs, new = self._apply_stages(ctx, obs, new)
+
+        return obs, new
+
+    def _apply_fields(self, ctx: Context) -> TensorDictBase:
+        items = {key: field(ctx) for key, field in self.fields.items()}
+        items[KEY_INDEX] = torch.arange(len(ctx.ids), device=ctx.ids.device)
+        return TensorDict(items, batch_size=ctx.ids.shape, device=ctx.ids.device)  # type: ignore
+
+    def _apply_stages(
+        self, ctx: Context, obs: TensorDictBase, new: TensorDictBase
+    ) -> Tuple[TensorDictBase, TensorDictBase]:
+        obs_candidates = obs.get_sub_tensordict(obs.get(KEY_ACTIVE))
+        for stage in self.stages:
+            obs_candidates, new = stage(ctx, obs_candidates, new)
+
+        if len(obs_candidates) > 0 and obs_candidates.batch_size[0] > 0:
+            obs_candidates.fill_(KEY_ACTIVE, False)
+
+        return obs, new
```

### Comparing `unitrack-4.3.2/sources/unitrack/stages/association.py` & `unitrack-4.5.0/sources/unitrack/stages/association.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,52 @@
 from typing import Tuple
 
-from ..assignment import Jonker
-from ..costs import CategoryGate, Cost
-from ..detections import Detections
-from .base_stage import Stage, StageContext
+from tensordict import TensorDictBase
+
+from ..assignment import Assignment
+from ..context import Context
+from ..costs import Cost
+from .base_stage import Stage
 
 __all__ = ["Association"]
 
 
 class Association(Stage):
     """
     An association stage assigns new track IDs using a cost matrix computed via
     a :class:`.Cost` module.
     """
 
     def __init__(
         self,
         cost: Cost,
-        threshold: float,
+        assignment: Assignment,
     ) -> None:
         super().__init__([], [])
 
         self.cost = cost
-        self.category_gate = CategoryGate()
-        self.assignment = Jonker(threshold=threshold)
+        self.assignment = assignment
 
-        self._extend_required_fields(self.cost, self.category_gate)
+        self._extend_required_fields(self.cost)
 
     def _extend_required_fields(self, *costs: Cost) -> None:
         for cost in costs:
             self.required_fields += cost.required_fields
 
-    def forward(self, ctx: StageContext, cs: Detections, ds: Detections) -> Tuple[Detections, Detections]:
+    def forward(self, ctx: Context, cs: TensorDictBase, ds: TensorDictBase) -> Tuple[TensorDictBase, TensorDictBase]:
         if len(cs) == 0 or len(ds) == 0:
             return cs, ds
 
         cost_matrix = self.cost(cs, ds)
-        cost_matrix *= self.category_gate(cs, ds)
 
-        matches, cs_fail, ds_fail = self.assignment(cost_matrix)
+        matches, cs_fail_idx, ds_fail_idx = self.assignment(cost_matrix)
 
         if len(matches) > 0:
-            # idx_t, idx_d = matches.T
-            ctx.match(cs[matches[:, 0]], ds[matches[:, 1]])
+            cs_match = cs.get_sub_tensordict(matches[:, 0])
+            ds_match = ds.get_sub_tensordict(matches[:, 1])
+
+            ctx.match(cs_match, ds_match)
+
+        cs_fail = cs.get_sub_tensordict(cs_fail_idx)
+        ds_fail = ds.get_sub_tensordict(ds_fail_idx)
 
-        return cs[cs_fail], ds[ds_fail]
+        return cs_fail, ds_fail
```

### Comparing `unitrack-4.3.2/sources/unitrack/stages/base_stage.py` & `unitrack-4.5.0/sources/unitrack/fields/base_field.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,74 +1,56 @@
 from abc import abstractmethod
-from typing import List, NamedTuple, Optional, Sequence, Tuple
+from typing import Dict, List
 
 import torch
 
-from ..detections import Detections
+from ..context import Context
 
-__all__ = ["Stage", "StageContext"]
+from tensordict import TensorDict
 
+__all__ = ["Field"]
 
-@torch.jit.script
-class StageContext:
-    def __init__(
-        self,
-        frame: int,
-        num_tracks: int,
-        device: torch.device,
-        data: dict[str, torch.Tensor],
-    ):
-        self.frame = frame
-        self.matches = torch.full((num_tracks,), -1, dtype=torch.long, device=device)
-        self.dt = 1
-
-        if data is None:
-            data = {}
-        self.data = data
 
-    def match(self, cs: Detections, ds: Detections) -> None:
-        """
-        Match candidates to detections.
+class Field(torch.nn.Module):
+    """
+    A field is a module that transforms data into state items of a tracked
+    object.
+    """
 
+    def __init__(self, required_keys: List[str], required_data: List[str]):
+        """
         Parameters
         ----------
-        cs
-            Candidates
-        ds
-            Detections
+        id
+            Unique ID for this field.
+        required_data
+            List of required keys in the input data.
         """
-        self.matches[ds.indices] = cs.indices
-
-
-class Stage(torch.nn.Module):
-    """
-    Base class for stages in a ::class::`..Tracker`.
-
-    Inputs to a stage are in the context data, or as fields of the detections.
-    """
 
-    required_fields: List[str]
-    required_data: List[str]
-
-    def __init__(
-        self,
-        required_fields: List[str],
-        required_data: List[str],
-    ):
         super().__init__()
 
-        self.required_fields: List[str] = required_fields
-        self.required_data: List[str] = required_data
+        self.required_keys = required_keys
+        self.required_data = required_data
+
+    def forward(self, ctx: Context):
+        return self.extract(ctx)
 
     @torch.jit.unused
     def __repr__(self) -> str:
-        req = ", ".join(self.required_fields)
-        return f"{type(self).__name__}(fields=[{req}])"
+        req = ", ".join(self.required_keys)
+        return f"{type(self).__name__}({self.id}, " f"data=[{req}])"
+
+    @abstractmethod
+    def extract(self, ctx: Context) -> torch.Tensor | TensorDict:
+        """
+        Extract field values from data.
 
-    def forward(
-        self,
-        ctx: StageContext,
-        cs: Detections,
-        ds: Detections,
-    ) -> Tuple[Detections, Detections]:
+        Parameters
+        ----------
+        data
+            Mapping of data keys to tensors.
+
+        Returns
+        -------
+            Mapping of field names to values.
+        """
         raise NotImplementedError
-        return self.run(ctx, cs, ds)
```

### Comparing `unitrack-4.3.2/sources/unitrack/stages/lost.py` & `unitrack-4.5.0/sources/unitrack/stages/lost.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 from typing import Tuple
 
-from ..detections import Detections
-from .base_stage import Stage, StageContext
+import torch
+from tensordict import TensorDictBase
+
+from ..constants import KEY_FRAME
+from ..context import Context
+from .base_stage import Stage
 
 __all__ = ["Lost"]
 
 
 class Lost(Stage):
     """
     Stage that filters out candidates that have been lost for less than a
@@ -15,28 +19,30 @@
     The time lost is computed via $$ T_l = t - T_c - dt $$ where $t$ is the
     current time (i.e. frame) and $T_c$ are the candidate time states.
     The value is corrected with time-step $dt$ to account for candidates not yet
     being updated to the current time, as the state update is performed
     *after* all stages have been ran.
     """
 
+    max_lost: torch.jit.Final[int]
+
     def __init__(self, max_lost: int):
         """
         Parameters
         ----------
         max_lost
             Maximum amount of time a candidate may remain lost.
         """
 
         super().__init__([], [])
 
         assert max_lost > 0, max_lost
 
         self.max_lost = max_lost
 
-    def forward(self, ctx: StageContext, cs: Detections, ds: Detections) -> Tuple[Detections, Detections]:
+    def forward(self, ctx: Context, cs: TensorDictBase, ds: TensorDictBase) -> Tuple[TensorDictBase, TensorDictBase]:
         if len(cs) == 0:
             return cs, ds
 
-        time_lost = ctx.frame - cs.get("_frame") - ctx.dt
+        time_lost = ctx.frame - cs.get(KEY_FRAME) - ctx.delta
 
-        return cs[time_lost > self.max_lost], ds
+        return cs.get_sub_tensordict(time_lost > self.max_lost), ds
```

### Comparing `unitrack-4.3.2/sources/unitrack/states/value.py` & `unitrack-4.5.0/sources/unitrack/states/value.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,25 +7,23 @@
     """
     A :class:`.State` that holds values as-is without any updating logic
     implemented.
     """
 
     values: torch.Tensor
 
-    def __init__(self, id: str, dtype: torch.dtype | str):
-        super().__init__(id)
+    def __init__(self, dtype: torch.dtype | str):
+        super().__init__()
 
         if isinstance(dtype, str):
             dtype = getattr(torch, dtype)
         if not isinstance(dtype, torch.dtype):
             raise ValueError(f"No a valid data type: {dtype}!")
 
-        self.register_buffer(
-            "values", torch.empty(0, dtype=dtype), persistent=False
-        )
+        self.register_buffer("values", torch.empty(0, dtype=dtype), persistent=False)
 
     @torch.jit.export
     def update(self, values: torch.Tensor) -> None:
         self.values = values
 
     @torch.jit.export
     def extend(self, values: torch.Tensor) -> None:
@@ -45,21 +43,24 @@
     """
     A :class:`.State` that computes the mean of its values over a given window
     size.
     """
 
     values_history: torch.Tensor
 
-    def __init__(self, id: str, window: int):
-        super().__init__(id)
+    def __init__(self, window: int, dtype: torch.dtype | str):
+        super().__init__()
+
+        if isinstance(dtype, str):
+            dtype = getattr(torch, dtype)
+        if not isinstance(dtype, torch.dtype):
+            raise ValueError(f"No a valid data type: {dtype}!")
 
         self.window = window
-        self.register_buffer(
-            "values_history", torch.zeros((0,)), persistent=False
-        )
+        self.register_buffer("values_history", torch.zeros((0,), dtype=dtype), persistent=False)
 
     @torch.jit.export
     def update(self, values: torch.Tensor) -> None:
         raise NotImplementedError
 
     @torch.jit.export
     def extend(self, values: torch.Tensor) -> None:
```

### Comparing `unitrack-4.3.2/sources/unitrack/tracklets.py` & `unitrack-4.5.0/sources/unitrack/memory.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,176 +1,122 @@
-from typing import Dict, Final, List, Optional
+from typing import Mapping
 
 import torch
+from tensordict import TensorDict, TensorDictBase
 
-from .detections import Detections
+from .constants import KEY_ACTIVE, KEY_FRAME, KEY_ID, KEY_INDEX, KEY_START
+from .context import Context
 from .states import State
 from .states import Value as ValueState
-from .tracker import TrackerResult
 
-__all__ = ["Tracklets"]
+__all__ = ["TrackletMemory"]
 
 
-class Tracklets(torch.nn.Module):
+class TrackletMemory(torch.nn.Module):
     """
     Container module for tracking predictions/paths, canonically called
     "tracklets" in literature.
 
     A tracklet is a generic representation of any tracked collection of states,
     e.g. objects in a scene. States of the tracklets are implemented in
     subclasses of :class:`Field`, which may be used to compute a distance
     matrix between tracklets at different frames.
     """
 
-    state_frame: Final = "_frame"
-    state_id: Final = "_id"
-    state_start: Final = "_start"
-    state_active: Final = "_active"
-
-    frame: int
-    count: int
-    sequence_id: Optional[str]
-    max_id: int
+    frame: torch.Tensor
+    count: torch.Tensor
+    max_id: torch.jit.Final[int]
+    states: Mapping[str, State]
 
-    def __init__(self, states: List[State], max_id=1000):
+    def __init__(self, states: Mapping[str, State], max_id=1000):
         super().__init__()
 
         assert max_id > 0, max_id
         assert len(states) > 0, len(states)
 
         self.max_id = max_id
-        self.states = torch.nn.ModuleDict(
-            {
-                state.id: state
-                for state in (
-                    ValueState(id=self.state_frame, dtype=torch.int),
-                    ValueState(id=self.state_start, dtype=torch.int),
-                    ValueState(id=self.state_id, dtype=torch.int),
-                    ValueState(id=self.state_active, dtype=torch.bool),
-                    *states,
-                )
-            }
-        )
+        self.states = torch.nn.ModuleDict()  # type: ignore
+        self.states[KEY_FRAME] = ValueState(torch.int)
+        self.states[KEY_START] = ValueState(torch.int)
+        self.states[KEY_ID] = ValueState(torch.int)
+        self.states[KEY_ACTIVE] = ValueState(torch.bool)
+        self.states.update(states)
 
-        self.frame = -1
-        self.count = 0
-        self.sequence_id = None
+        self.register_buffer("frame", torch.tensor(-1, dtype=torch.int, requires_grad=False))
+        self.register_buffer("count", torch.tensor(0, dtype=torch.int, requires_grad=False))
 
     def __len__(self) -> int:
-        return self.count
-
-    def forward(self, sequence_id: str, frame: int, res: TrackerResult) -> torch.Tensor:
-        """
-        Update the ``Tracklets`` at a given frame with new state data from
-        detections.
+        return int(self.count.detach().cpu().item())
 
-        Parameters
-        ----------
-        frame
-            Current frame.
-        put
-            Detections that are put into the current state.
-        new
-            Detections that are newly added to the state.
+    def forward(self) -> None:
+        raise NotImplementedError("TrackletMemory does not implement forward()!")
 
-        Returns
-        -------
-            New states.
+    @torch.jit.export
+    def update(self, ctx: Context, obs: TensorDictBase, new: TensorDictBase) -> torch.Tensor:
         """
+        Apply the updated observations and new detections to the tracklets states.
 
-        assert res.update.indices.dtype == torch.int64, res.update.indices.dtype
-        assert res.extend.indices.dtype == torch.int64, res.extend.indices.dtype
-        assert res.matches.dtype == torch.int64, res.matches.dtype
-
-        device = res.matches.device
-
-        if not torch.allclose(
-            res.update.indices,
-            torch.arange(len(res.update), device=device, dtype=res.update.indices.dtype),
-        ):
-            raise ValueError("Updated detections are not in the correct ordering!")
-        if not res.update.mutable:
-            raise ValueError("Updated observations must be a mutable detections collection!")
-        if res.extend.mutable:
-            raise ValueError("Updated additions should not be a mutable collection!")
+        Returns the complete set of IDs of the context (which is also updated in-place).
+        """
 
-        self.frame = frame
+        self.frame.fill_(ctx.frame)
         self.count += 1
-        self.sequence_id = sequence_id
 
-        # Pull IDs from update for each detection in the tracker result
-        detection_ids = torch.zeros_like(res.matches, dtype=torch.int)
+        extend_num = new.batch_size[0]
+        extend_ids = torch.arange(extend_num, dtype=torch.long, device=self.frame.device, requires_grad=False)
+        extend_ids += 1
+        if len(obs.get(KEY_ID)) > 0:
+            extend_ids += obs.get(KEY_ID).max()
+
+        ctx.ids[new.get(KEY_INDEX)] = extend_ids
+
+        extend_frame = torch.full(
+            (extend_num,),
+            ctx.frame,
+            dtype=torch.int,
+            device=self.frame.device,
+        )
 
-        match_mask = (res.matches >= 0).to(torch.bool)
-        match_update_indices = res.matches[match_mask]
+        assert extend_ids.max() < self.max_id, (extend_ids.max().cpu().item(), self.max_id)
 
-        detection_ids[match_mask] = res.update.get(self.state_id)[res.update.indices[match_update_indices]]
-
-        # Put new measurements into state
-        update_num = len(res.update)
-        if update_num > 0:
-            for id, state in self.states.items():
-                state.update(res.update.get(id))  # type: ignore
-
-        # Add new measurements into states
-        extend_num = len(res.extend)
-        extend_ids = torch.arange(extend_num, dtype=torch.int, device=device) + 1
-        if update_num > 0:
-            extend_ids += res.update.get(self.state_id).max()
-        if extend_num > 0:
-            for id, state in self.states.items():
-                if id == self.state_active:
-                    state.extend(torch.as_tensor([True] * extend_num, dtype=torch.bool, device=device))  # type: ignore
-                elif id == self.state_frame:
-                    state.extend(  # type: ignore
-                        torch.as_tensor(
-                            [frame] * extend_num,
-                            dtype=torch.int,
-                            device=device,
-                        )
-                    )
-                elif id == self.state_start:
-                    state.extend(  # type: ignore
-                        torch.as_tensor(
-                            [frame] * extend_num,
-                            dtype=torch.int,
-                            device=device,
-                        )
-                    )
-                elif id == self.state_id:
-                    state.extend(extend_ids)  # type: ignore
-                elif id in res.extend:
-                    state.extend(res.extend.get(id))  # type: ignore
-                else:
-                    raise ValueError(f"State '{id}' does not match a field in {res.extend}!")
+        for id, state in self.states.items():
+            state.update(obs.get(id))
 
-        detection_ids[~match_mask] = extend_ids
+            if id == KEY_ACTIVE:
+                state.extend(torch.ones((extend_num,), dtype=torch.bool, device=self.frame.device, requires_grad=False))  # type: ignore
+            elif id == KEY_FRAME or id == KEY_START:
+                state.extend(extend_frame)
+            elif id == KEY_ID:
+                state.extend(extend_ids)  # type: ignore
+            elif id in new.keys():
+                state.extend(new.get(id))  # type: ignore
+            else:
+                raise ValueError(f"State '{id}' does not match a field in {new.keys()}!")
 
-        return detection_ids
+        return ctx.ids
 
     @torch.jit.export
     def reset(self) -> None:
         """
         Reset the states of this ``Tracklets`` module.
         """
-        self.frame = -1
-        self.count = 0
-        self.sequence_id = None
+        self.frame.fill_(-1)
+        self.count.fill_(0)
 
         for state in self.states.values():
             state.reset()  # type: ignore
 
     @torch.jit.export
-    def observe(self) -> Detections:
+    def observe(self) -> TensorDictBase:
         """
         Observe the current state of tracklets.
 
         Returns
         -------
-            A ``Detections`` object will all observed states.
+            A ``TensorDict`` object will all observed states.
         """
 
-        field_values = {}
+        obs = {}
         for id, state in self.states.items():
-            field_values[id] = state.observe()  # type: ignore
+            obs[id] = state.observe()  # type: ignore
 
-        return Detections(field_values, mutable=True)
+        return TensorDict.from_dict(obs, device=self.frame.device)
```

### Comparing `unitrack-4.3.2/sources/unitrack.egg-info/PKG-INFO` & `unitrack-4.5.0/sources/unitrack.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1
-Name: unitrack
-Version: 4.3.2
-Summary: A multi-stage object tracking framework
-Author-email: Kurt Stolle <k.h.w.stolle@gmail.com>
-Keywords: perception,computer vision,deep learning,object detection,instance segmentation,semantic segmentation
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: docs
-Provides-Extra: tests
-License-File: LICENSE
-
-# Unified Tracking
-Multi-stage object tracking framework research project.
+Metadata-Version: 2.1
+Name: unitrack
+Version: 4.5.0
+Summary: A multi-stage object tracking framework
+Author-email: Kurt Stolle <k.h.w.stolle@gmail.com>
+Keywords: perception,computer vision,deep learning,object detection,instance segmentation,semantic segmentation
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+Provides-Extra: docs
+Provides-Extra: tests
+License-File: LICENSE
+
+# Unified Tracking
+Multi-stage object tracking framework research project.
```

### Comparing `unitrack-4.3.2/sources/unitrack.egg-info/SOURCES.txt` & `unitrack-4.5.0/sources/unitrack.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.md
 pyproject.toml
 sources/unitrack/__init__.py
-sources/unitrack/detections.py
+sources/unitrack/constants.py
+sources/unitrack/context.py
+sources/unitrack/memory.py
 sources/unitrack/tracker.py
-sources/unitrack/tracklets.py
 sources/unitrack.egg-info/PKG-INFO
 sources/unitrack.egg-info/SOURCES.txt
 sources/unitrack.egg-info/dependency_links.txt
 sources/unitrack.egg-info/requires.txt
 sources/unitrack.egg-info/top_level.txt
 sources/unitrack/assignment/__init__.py
 sources/unitrack/assignment/auction.py
@@ -16,14 +17,15 @@
 sources/unitrack/assignment/greedy.py
 sources/unitrack/assignment/hungarian.py
 sources/unitrack/assignment/jonker.py
 sources/unitrack/costs/__init__.py
 sources/unitrack/costs/base_cost.py
 sources/unitrack/costs/category.py
 sources/unitrack/costs/iou.py
+sources/unitrack/costs/reduce.py
 sources/unitrack/costs/wrap.py
 sources/unitrack/fields/__init__.py
 sources/unitrack/fields/base_field.py
 sources/unitrack/fields/value.py
 sources/unitrack/stages/__init__.py
 sources/unitrack/stages/association.py
 sources/unitrack/stages/base_stage.py
```

