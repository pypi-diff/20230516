# Comparing `tmp/PyExpUtils-andnp-4.0.1.tar.gz` & `tmp/PyExpUtils-andnp-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyExpUtils-andnp-4.0.1.tar", last modified: Mon May  8 23:10:20 2023, max compression
+gzip compressed data, was "PyExpUtils-andnp-5.0.0.tar", last modified: Tue May 16 03:43:55 2023, max compression
```

## Comparing `PyExpUtils-andnp-4.0.1.tar` & `PyExpUtils-andnp-5.0.0.tar`

### file list

```diff
@@ -1,60 +1,62 @@
--rw-r--r--   0        0        0     1011 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/FileSystemContext.py
--rw-r--r--   0        0        0      119 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/__init__.py
--rw-r--r--   0        0        0     1207 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/models/Config.py
--rw-r--r--   0        0        0     7915 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/models/ExperimentDescription.py
--rw-r--r--   0        0        0       87 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/models/__init__.py
--rw-r--r--   0        0        0        0 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/py.typed
--rw-r--r--   0        0        0     3110 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/results/Collection.py
--rw-r--r--   0        0        0        0 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/results/__init__.py
--rw-r--r--   0        0        0      510 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/results/indices.py
--rw-r--r--   0        0        0     7798 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/results/pandas.py
--rw-r--r--   0        0        0     1070 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/results/tools.py
--rw-r--r--   0        0        0     8921 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/results/voting.py
--rw-r--r--   0        0        0     5211 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/runner/Slurm.py
--rw-r--r--   0        0        0        0 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/runner/__init__.py
--rw-r--r--   0        0        0      742 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/runner/parallel.py
--rw-r--r--   0        0        0     1450 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/runner/utils.py
--rw-r--r--   0        0        0     2826 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/utils/Collector.py
--rw-r--r--   0        0        0     3030 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/utils/NestedDict.py
--rw-r--r--   0        0        0        0 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/utils/__init__.py
--rw-r--r--   0        0        0     3432 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/utils/arrays.py
--rw-r--r--   0        0        0      403 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/utils/asyncio.py
--rw-r--r--   0        0        0      595 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/utils/cache.py
--rw-r--r--   0        0        0      368 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/utils/cmdline.py
--rw-r--r--   0        0        0     1233 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/utils/csv.py
--rw-r--r--   0        0        0     3547 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/utils/dict.py
--rw-r--r--   0        0        0     1266 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/utils/fp.py
--rw-r--r--   0        0        0      921 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/utils/generator.py
--rw-r--r--   0        0        0      476 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/utils/jit.py
--rw-r--r--   0        0        0     1218 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/utils/path.py
--rw-r--r--   0        0        0     3454 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/utils/permute.py
--rw-r--r--   0        0        0      969 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/utils/random.py
--rw-r--r--   0        0        0      278 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/utils/str.py
--rw-r--r--   0        0        0      439 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/PyExpUtils/utils/types.py
--rw-r--r--   0        0        0     6884 2023-05-08 23:09:43.618942 PyExpUtils-andnp-4.0.1/README.md
--rw-r--r--   0        0        0     1018 2023-05-08 23:10:19.091060 PyExpUtils-andnp-4.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-08 23:09:43.622943 PyExpUtils-andnp-4.0.1/tests/__init__.py
--rw-r--r--   0        0        0      214 2023-05-08 23:09:43.622943 PyExpUtils-andnp-4.0.1/tests/_utils/pandas.py
--rw-r--r--   0        0        0        0 2023-05-08 23:09:43.622943 PyExpUtils-andnp-4.0.1/tests/models/__init__.py
--rw-r--r--   0        0        0     5461 2023-05-08 23:09:43.622943 PyExpUtils-andnp-4.0.1/tests/models/test_ExperimentDescription.py
--rw-r--r--   0        0        0        0 2023-05-08 23:09:43.622943 PyExpUtils-andnp-4.0.1/tests/results/__init__.py
--rw-r--r--   0        0        0      898 2023-05-08 23:09:43.622943 PyExpUtils-andnp-4.0.1/tests/results/test_indices.py
--rw-r--r--   0        0        0     9113 2023-05-08 23:09:43.622943 PyExpUtils-andnp-4.0.1/tests/results/test_pandas.py
--rw-r--r--   0        0        0     2010 2023-05-08 23:09:43.622943 PyExpUtils-andnp-4.0.1/tests/results/test_tools.py
--rw-r--r--   0        0        0     8723 2023-05-08 23:09:43.622943 PyExpUtils-andnp-4.0.1/tests/results/test_voting.py
--rw-r--r--   0        0        0        0 2023-05-08 23:09:43.622943 PyExpUtils-andnp-4.0.1/tests/runner/__init__.py
--rw-r--r--   0        0        0      385 2023-05-08 23:09:43.622943 PyExpUtils-andnp-4.0.1/tests/runner/test_parallel.py
--rw-r--r--   0        0        0      987 2023-05-08 23:09:43.622943 PyExpUtils-andnp-4.0.1/tests/runner/test_slurm.py
--rw-r--r--   0        0        0     2278 2023-05-08 23:09:43.622943 PyExpUtils-andnp-4.0.1/tests/test_FileSystemContext.py
--rw-r--r--   0        0        0        0 2023-05-08 23:09:43.622943 PyExpUtils-andnp-4.0.1/tests/utils/__init__.py
--rw-r--r--   0        0        0     3210 2023-05-08 23:09:43.622943 PyExpUtils-andnp-4.0.1/tests/utils/test_Collector.py
--rw-r--r--   0        0        0     4023 2023-05-08 23:09:43.622943 PyExpUtils-andnp-4.0.1/tests/utils/test_arrays.py
--rw-r--r--   0        0        0      881 2023-05-08 23:09:43.622943 PyExpUtils-andnp-4.0.1/tests/utils/test_cmdline.py
--rw-r--r--   0        0        0     1911 2023-05-08 23:09:43.622943 PyExpUtils-andnp-4.0.1/tests/utils/test_csv.py
--rw-r--r--   0        0        0     5882 2023-05-08 23:09:43.622943 PyExpUtils-andnp-4.0.1/tests/utils/test_dict.py
--rw-r--r--   0        0        0      586 2023-05-08 23:09:43.622943 PyExpUtils-andnp-4.0.1/tests/utils/test_generator.py
--rw-r--r--   0        0        0     1685 2023-05-08 23:09:43.622943 PyExpUtils-andnp-4.0.1/tests/utils/test_path.py
--rw-r--r--   0        0        0     3725 2023-05-08 23:09:43.622943 PyExpUtils-andnp-4.0.1/tests/utils/test_permute.py
--rw-r--r--   0        0        0     1560 2023-05-08 23:09:43.622943 PyExpUtils-andnp-4.0.1/tests/utils/test_random.py
--rw-r--r--   0        0        0      365 2023-05-08 23:09:43.622943 PyExpUtils-andnp-4.0.1/tests/utils/test_str.py
--rw-r--r--   0        0        0     7138 1970-01-01 00:00:00.000000 PyExpUtils-andnp-4.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1011 2023-05-16 03:43:17.276273 PyExpUtils-andnp-5.0.0/PyExpUtils/FileSystemContext.py
+-rw-r--r--   0        0        0      119 2023-05-16 03:43:17.276273 PyExpUtils-andnp-5.0.0/PyExpUtils/__init__.py
+-rw-r--r--   0        0        0     1207 2023-05-16 03:43:17.276273 PyExpUtils-andnp-5.0.0/PyExpUtils/models/Config.py
+-rw-r--r--   0        0        0     7915 2023-05-16 03:43:17.276273 PyExpUtils-andnp-5.0.0/PyExpUtils/models/ExperimentDescription.py
+-rw-r--r--   0        0        0       87 2023-05-16 03:43:17.276273 PyExpUtils-andnp-5.0.0/PyExpUtils/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-16 03:43:17.276273 PyExpUtils-andnp-5.0.0/PyExpUtils/py.typed
+-rw-r--r--   0        0        0     3167 2023-05-16 03:43:17.276273 PyExpUtils-andnp-5.0.0/PyExpUtils/results/Collection.py
+-rw-r--r--   0        0        0        0 2023-05-16 03:43:17.276273 PyExpUtils-andnp-5.0.0/PyExpUtils/results/__init__.py
+-rw-r--r--   0        0        0      510 2023-05-16 03:43:17.276273 PyExpUtils-andnp-5.0.0/PyExpUtils/results/indices.py
+-rw-r--r--   0        0        0     9082 2023-05-16 03:43:17.276273 PyExpUtils-andnp-5.0.0/PyExpUtils/results/pandas.py
+-rw-r--r--   0        0        0     1070 2023-05-16 03:43:17.276273 PyExpUtils-andnp-5.0.0/PyExpUtils/results/tools.py
+-rw-r--r--   0        0        0     8921 2023-05-16 03:43:17.276273 PyExpUtils-andnp-5.0.0/PyExpUtils/results/voting.py
+-rw-r--r--   0        0        0     5211 2023-05-16 03:43:17.276273 PyExpUtils-andnp-5.0.0/PyExpUtils/runner/Slurm.py
+-rw-r--r--   0        0        0        0 2023-05-16 03:43:17.276273 PyExpUtils-andnp-5.0.0/PyExpUtils/runner/__init__.py
+-rw-r--r--   0        0        0      742 2023-05-16 03:43:17.280273 PyExpUtils-andnp-5.0.0/PyExpUtils/runner/parallel.py
+-rw-r--r--   0        0        0     1450 2023-05-16 03:43:17.280273 PyExpUtils-andnp-5.0.0/PyExpUtils/runner/utils.py
+-rw-r--r--   0        0        0     6214 2023-05-16 03:43:17.280273 PyExpUtils-andnp-5.0.0/PyExpUtils/utils/Collector.py
+-rw-r--r--   0        0        0     3030 2023-05-16 03:43:17.280273 PyExpUtils-andnp-5.0.0/PyExpUtils/utils/NestedDict.py
+-rw-r--r--   0        0        0        0 2023-05-16 03:43:17.280273 PyExpUtils-andnp-5.0.0/PyExpUtils/utils/__init__.py
+-rw-r--r--   0        0        0     3432 2023-05-16 03:43:17.280273 PyExpUtils-andnp-5.0.0/PyExpUtils/utils/arrays.py
+-rw-r--r--   0        0        0      403 2023-05-16 03:43:17.280273 PyExpUtils-andnp-5.0.0/PyExpUtils/utils/asyncio.py
+-rw-r--r--   0        0        0      595 2023-05-16 03:43:17.280273 PyExpUtils-andnp-5.0.0/PyExpUtils/utils/cache.py
+-rw-r--r--   0        0        0      368 2023-05-16 03:43:17.280273 PyExpUtils-andnp-5.0.0/PyExpUtils/utils/cmdline.py
+-rw-r--r--   0        0        0     1233 2023-05-16 03:43:17.280273 PyExpUtils-andnp-5.0.0/PyExpUtils/utils/csv.py
+-rw-r--r--   0        0        0     3547 2023-05-16 03:43:17.280273 PyExpUtils-andnp-5.0.0/PyExpUtils/utils/dict.py
+-rw-r--r--   0        0        0     1266 2023-05-16 03:43:17.280273 PyExpUtils-andnp-5.0.0/PyExpUtils/utils/fp.py
+-rw-r--r--   0        0        0      921 2023-05-16 03:43:17.280273 PyExpUtils-andnp-5.0.0/PyExpUtils/utils/generator.py
+-rw-r--r--   0        0        0      197 2023-05-16 03:43:17.280273 PyExpUtils-andnp-5.0.0/PyExpUtils/utils/iterable.py
+-rw-r--r--   0        0        0      476 2023-05-16 03:43:17.280273 PyExpUtils-andnp-5.0.0/PyExpUtils/utils/jit.py
+-rw-r--r--   0        0        0      363 2023-05-16 03:43:17.280273 PyExpUtils-andnp-5.0.0/PyExpUtils/utils/pandas.py
+-rw-r--r--   0        0        0     1218 2023-05-16 03:43:17.280273 PyExpUtils-andnp-5.0.0/PyExpUtils/utils/path.py
+-rw-r--r--   0        0        0     3454 2023-05-16 03:43:17.280273 PyExpUtils-andnp-5.0.0/PyExpUtils/utils/permute.py
+-rw-r--r--   0        0        0      969 2023-05-16 03:43:17.280273 PyExpUtils-andnp-5.0.0/PyExpUtils/utils/random.py
+-rw-r--r--   0        0        0      278 2023-05-16 03:43:17.280273 PyExpUtils-andnp-5.0.0/PyExpUtils/utils/str.py
+-rw-r--r--   0        0        0      439 2023-05-16 03:43:17.280273 PyExpUtils-andnp-5.0.0/PyExpUtils/utils/types.py
+-rw-r--r--   0        0        0     6884 2023-05-16 03:43:17.280273 PyExpUtils-andnp-5.0.0/README.md
+-rw-r--r--   0        0        0     1018 2023-05-16 03:43:53.528809 PyExpUtils-andnp-5.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-16 03:43:17.280273 PyExpUtils-andnp-5.0.0/tests/__init__.py
+-rw-r--r--   0        0        0      214 2023-05-16 03:43:17.280273 PyExpUtils-andnp-5.0.0/tests/_utils/pandas.py
+-rw-r--r--   0        0        0        0 2023-05-16 03:43:17.280273 PyExpUtils-andnp-5.0.0/tests/models/__init__.py
+-rw-r--r--   0        0        0     5461 2023-05-16 03:43:17.280273 PyExpUtils-andnp-5.0.0/tests/models/test_ExperimentDescription.py
+-rw-r--r--   0        0        0        0 2023-05-16 03:43:17.280273 PyExpUtils-andnp-5.0.0/tests/results/__init__.py
+-rw-r--r--   0        0        0      898 2023-05-16 03:43:17.280273 PyExpUtils-andnp-5.0.0/tests/results/test_indices.py
+-rw-r--r--   0        0        0     9113 2023-05-16 03:43:17.280273 PyExpUtils-andnp-5.0.0/tests/results/test_pandas.py
+-rw-r--r--   0        0        0     2010 2023-05-16 03:43:17.280273 PyExpUtils-andnp-5.0.0/tests/results/test_tools.py
+-rw-r--r--   0        0        0     8723 2023-05-16 03:43:17.280273 PyExpUtils-andnp-5.0.0/tests/results/test_voting.py
+-rw-r--r--   0        0        0        0 2023-05-16 03:43:17.280273 PyExpUtils-andnp-5.0.0/tests/runner/__init__.py
+-rw-r--r--   0        0        0      385 2023-05-16 03:43:17.280273 PyExpUtils-andnp-5.0.0/tests/runner/test_parallel.py
+-rw-r--r--   0        0        0      987 2023-05-16 03:43:17.280273 PyExpUtils-andnp-5.0.0/tests/runner/test_slurm.py
+-rw-r--r--   0        0        0     2278 2023-05-16 03:43:17.280273 PyExpUtils-andnp-5.0.0/tests/test_FileSystemContext.py
+-rw-r--r--   0        0        0        0 2023-05-16 03:43:17.280273 PyExpUtils-andnp-5.0.0/tests/utils/__init__.py
+-rw-r--r--   0        0        0     4644 2023-05-16 03:43:17.280273 PyExpUtils-andnp-5.0.0/tests/utils/test_Collector.py
+-rw-r--r--   0        0        0     4023 2023-05-16 03:43:17.280273 PyExpUtils-andnp-5.0.0/tests/utils/test_arrays.py
+-rw-r--r--   0        0        0      881 2023-05-16 03:43:17.280273 PyExpUtils-andnp-5.0.0/tests/utils/test_cmdline.py
+-rw-r--r--   0        0        0     1911 2023-05-16 03:43:17.280273 PyExpUtils-andnp-5.0.0/tests/utils/test_csv.py
+-rw-r--r--   0        0        0     5882 2023-05-16 03:43:17.280273 PyExpUtils-andnp-5.0.0/tests/utils/test_dict.py
+-rw-r--r--   0        0        0      586 2023-05-16 03:43:17.280273 PyExpUtils-andnp-5.0.0/tests/utils/test_generator.py
+-rw-r--r--   0        0        0     1685 2023-05-16 03:43:17.280273 PyExpUtils-andnp-5.0.0/tests/utils/test_path.py
+-rw-r--r--   0        0        0     3725 2023-05-16 03:43:17.280273 PyExpUtils-andnp-5.0.0/tests/utils/test_permute.py
+-rw-r--r--   0        0        0     1560 2023-05-16 03:43:17.280273 PyExpUtils-andnp-5.0.0/tests/utils/test_random.py
+-rw-r--r--   0        0        0      365 2023-05-16 03:43:17.280273 PyExpUtils-andnp-5.0.0/tests/utils/test_str.py
+-rw-r--r--   0        0        0     7138 1970-01-01 00:00:00.000000 PyExpUtils-andnp-5.0.0/PKG-INFO
```

### Comparing `PyExpUtils-andnp-4.0.1/PyExpUtils/FileSystemContext.py` & `PyExpUtils-andnp-5.0.0/PyExpUtils/FileSystemContext.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.1/PyExpUtils/models/Config.py` & `PyExpUtils-andnp-5.0.0/PyExpUtils/models/Config.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.1/PyExpUtils/models/ExperimentDescription.py` & `PyExpUtils-andnp-5.0.0/PyExpUtils/models/ExperimentDescription.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.1/PyExpUtils/results/Collection.py` & `PyExpUtils-andnp-5.0.0/PyExpUtils/results/Collection.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations
 import os
 import glob
 import importlib
 import pandas as pd
-from typing import Any, Callable, Dict, List, Optional, Type, overload
+from typing import Any, Callable, Dict, Iterable, List, Optional, Type, overload
 from PyExpUtils.utils.NestedDict import NestedDict
 from PyExpUtils.utils.permute import set_at_path
 from PyExpUtils.models.ExperimentDescription import ExperimentDescription, loadExperiment
-from PyExpUtils.results.pandas import loadResults
+from PyExpUtils.results.pandas import loadAllResults
 
 class ResultCollection(NestedDict[str, pd.DataFrame]):
     def __init__(self, Model: Optional[Type[ExperimentDescription]] = None):
         super().__init__(depth=2)
 
         self._data: Dict[str, Dict[str, pd.DataFrame]] = {}
         self._Model = Model
@@ -34,25 +34,25 @@
 
         for key in self:
             out[key] = f(self[key])
 
         return out
 
     @classmethod
-    def fromExperiments(cls, file: str, path: Optional[str] = None, Model: Optional[Type[ExperimentDescription]] = None) -> ResultCollection:
+    def fromExperiments(cls, metrics: Optional[Iterable[str]] = None, path: Optional[str] = None, Model: Optional[Type[ExperimentDescription]] = None) -> ResultCollection:
         exp_files = findExperiments('{domain}', path)
 
         out = cls(Model=Model)
         for domain in exp_files:
             paths = exp_files[domain]
             for p in paths:
                 alg = p.split('/')[-1].replace('.json', '')
 
                 exp = loadExperiment(p, Model)
-                df = loadResults(exp, file)
+                df = loadAllResults(exp, metrics=metrics)
 
                 if df is not None:
                     out[domain, alg] = df
 
         return out
 
 @overload
```

### Comparing `PyExpUtils-andnp-4.0.1/PyExpUtils/results/pandas.py` & `PyExpUtils-andnp-5.0.0/PyExpUtils/results/pandas.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 from collections import defaultdict
 import os
 import glob
 import pandas as pd
+import PyExpUtils.utils.pandas as pdu
+
 from filelock import FileLock
-from typing import Any, Dict, Optional, Sequence, Union
+from typing import Any, Dict, Iterable, Optional, Sequence, Union
 from PyExpUtils.FileSystemContext import FileSystemContext
 from PyExpUtils.models.ExperimentDescription import ExperimentDescription
 from PyExpUtils.results.indices import listIndices
 from PyExpUtils.results.tools import subsetDF
 from PyExpUtils.utils.Collector import Collector
 from PyExpUtils.utils.dict import flatKeys, get
 from PyExpUtils.utils.types import NpList
 from PyExpUtils.utils.asyncio import threadMap
+from PyExpUtils.utils.iterable import filter_none
 
 class NoResultException(Exception):
     ...
 
 def saveResults(exp: ExperimentDescription, idx: int, filename: str, data: NpList, base: str = './', batch_size: Optional[int] = 20000):
     context = exp.buildSaveContext(idx, base=base)
     context.ensureExists()
@@ -92,16 +95,31 @@
 
     for path in to_write:
         df = pd.DataFrame(to_write[path])
 
         with FileLock(path + '.lock'):
             df.to_csv(path, mode='a+', header=False, index=False)
 
+def loadAllResults(exp: ExperimentDescription, metrics: Optional[Iterable[str]] = None, base: str = './', use_cache: bool = True) -> Union[pd.DataFrame, None]:
+    if metrics is None:
+        metrics = get_result_filenames(exp, base)
+
+    parts = (loadResults(exp, f, base, col=f, use_cache=use_cache) for f in metrics)
+    dfs: Iterable[pd.DataFrame] = filter_none(parts)
+    dfs = list(dfs)
+
+    if len(dfs) == 0:
+        return None
+
+    header = getHeader(exp) + ['run']
+    df = pdu.outer(dfs, on=header)
+
+    return df
 
-def loadResults(exp: ExperimentDescription, filename: str, base: str = './', use_cache: bool = True) -> Union[pd.DataFrame, None]:
+def loadResults(exp: ExperimentDescription, filename: str, base: str = './', col: Optional[str] = None, use_cache: bool = True) -> Union[pd.DataFrame, None]:
     context = exp.buildSaveContext(0, base=base)
 
     files = glob.glob(context.resolve(f'{filename}.*.csv'))
 
     # this could be because we did not use batching
     # try again without batching
     if len(files) == 0:
@@ -116,38 +134,48 @@
     latest = max(*times, 0, 0)
 
     cache_file = context.resolve(filename + '.pkl')
     if use_cache and os.path.exists(cache_file) and os.path.getmtime(cache_file) > latest:
         df = pd.read_pickle(cache_file)
         return _subsetDFbyExp(df, exp)
 
-    header = getHeader(exp)
-
-    if len(files) == 0:
-        raise NoResultException('No result files found')
-
     partials = threadMap(_readUnevenCsv, files)
     df = pd.concat(partials, ignore_index=True)
 
+    header = getHeader(exp)
     nparams = len(header) + 1
     new_df = df.iloc[:, :nparams]
     new_df.columns = header + ['run']
-    new_df['data'] = df.iloc[:, nparams:].values.tolist()
+
+    # figure out where to put the data
+    if col is None:
+        col = 'data'
+
+    new_df[col] = df.iloc[:, nparams:].values.tolist()
 
     if use_cache:
         new_df.to_pickle(cache_file)
 
     return _subsetDFbyExp(new_df, exp)
 
 
-def detectMissingIndices(exp: ExperimentDescription, runs: int, filename: str, base: str = './'): # noqa: C901
+def detectMissingIndices(exp: ExperimentDescription, runs: int, filename: Optional[str] = None, base: str = './'): # noqa: C901
     indices = listIndices(exp)
     nperms = exp.numPermutations()
     header = getHeader(exp)
 
+    r_files = get_result_filenames(exp, base)
+    if len(r_files) == 0:
+        for idx in indices:
+            for run in range(runs):
+                yield idx + run * nperms
+        return
+
+    filename = list(r_files)[0]
+    assert isinstance(filename, str)
     df = loadResults(exp, filename, base=base)
     # ----------------------------------
     # -- first case: no existing data --
     # ----------------------------------
     if df is None:
         for idx in indices:
             for run in range(runs):
@@ -191,14 +219,23 @@
 def getParamValues(exp: ExperimentDescription, idx: int, header: Optional[Sequence[str]] = None):
     if header is None:
         header = getHeader(exp)
 
     params = exp.getPermutation(idx)['metaParameters']
     return [get(params, k) for k in header]
 
+def get_result_filenames(exp: ExperimentDescription, base: str = './'):
+    context = exp.buildSaveContext(0, base=base)
+    files = glob.glob(context.resolve('*.*.csv')) + glob.glob(context.resolve('*.csv'))
+
+    if len(files) == 0:
+        return set[str]()
+
+    return set(map(lambda x: os.path.basename(x).split('.')[0], files))
+
 # ---------------
 # -- Utilities --
 # ---------------
 
 # makes sure the dataframe only contains the data for a given experiment description
 def _subsetDFbyExp(df: pd.DataFrame, exp: ExperimentDescription):
     params = exp._d['metaParameters']
@@ -225,15 +262,16 @@
 
 # if the csv contains ragged rows (i.e. rows have different numbers of columns)
 # then the native csv reader needs to know the max number of columns.
 # the resulting df will have NaNs for the shorter rows
 def _readUnevenCsv(f: str):
     with open(f, 'r') as temp_f:
         col_count = ( len(l.split(",")) for l in temp_f.readlines() )
-        names = list(map(str, range(0, max(col_count))))
+        m_cols = max(col_count)
+        names = list(map(str, range(0, m_cols)))
 
     return pd.read_csv(f, header=None, names=names)
 
 def _batchFile(context: FileSystemContext, filename: str, idx: int, batch_size: Optional[int]):
     if batch_size is None:
         return context.resolve(f'{filename}.csv')
```

### Comparing `PyExpUtils-andnp-4.0.1/PyExpUtils/results/tools.py` & `PyExpUtils-andnp-5.0.0/PyExpUtils/results/tools.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.1/PyExpUtils/results/voting.py` & `PyExpUtils-andnp-5.0.0/PyExpUtils/results/voting.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.1/PyExpUtils/runner/Slurm.py` & `PyExpUtils-andnp-5.0.0/PyExpUtils/runner/Slurm.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.1/PyExpUtils/runner/parallel.py` & `PyExpUtils-andnp-5.0.0/PyExpUtils/runner/parallel.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.1/PyExpUtils/runner/utils.py` & `PyExpUtils-andnp-5.0.0/PyExpUtils/runner/utils.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.1/PyExpUtils/utils/NestedDict.py` & `PyExpUtils-andnp-5.0.0/PyExpUtils/utils/NestedDict.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.1/PyExpUtils/utils/arrays.py` & `PyExpUtils-andnp-5.0.0/PyExpUtils/utils/arrays.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.1/PyExpUtils/utils/cache.py` & `PyExpUtils-andnp-5.0.0/PyExpUtils/utils/cache.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.1/PyExpUtils/utils/csv.py` & `PyExpUtils-andnp-5.0.0/PyExpUtils/utils/csv.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.1/PyExpUtils/utils/dict.py` & `PyExpUtils-andnp-5.0.0/PyExpUtils/utils/dict.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.1/PyExpUtils/utils/fp.py` & `PyExpUtils-andnp-5.0.0/PyExpUtils/utils/fp.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.1/PyExpUtils/utils/generator.py` & `PyExpUtils-andnp-5.0.0/PyExpUtils/utils/generator.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.1/PyExpUtils/utils/path.py` & `PyExpUtils-andnp-5.0.0/PyExpUtils/utils/path.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.1/PyExpUtils/utils/permute.py` & `PyExpUtils-andnp-5.0.0/PyExpUtils/utils/permute.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.1/PyExpUtils/utils/random.py` & `PyExpUtils-andnp-5.0.0/PyExpUtils/utils/random.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.1/README.md` & `PyExpUtils-andnp-5.0.0/README.md`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.1/pyproject.toml` & `PyExpUtils-andnp-5.0.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "4.0.1"
+version = "5.0.0"
 tag_format = "$version"
 version_files = [
     "pyproject.toml",
 ]
 
 [tool.pdm]
 source = [
     { url = "https://pypi.org/simple", verify_ssl = true, name = "pypi" },
     { url = "https://pypi.org/simple", verify_ssl = true, name = "pypi" },
 ]
 
 [tool.pdm.dev-dependencies]
 dev = [
     "mypy>=0.942",
-    "flake8>=4.0.1",
+    "flake8>=5.0.0",
     "commitizen",
     "pre-commit",
     "matplotlib",
     "types-filelock",
     "build",
     "twine",
     "vistir==0.6.1",
 ]
 
 [tool.mypy]
 mypy_path = "typings"
 
 [project]
 name = "PyExpUtils-andnp"
-version = "4.0.1"
+version = "5.0.0"
 description = "A small set of utilities for RL and ML experiments"
 authors = [
     { name = "Andy Patterson", email = "andnpatterson@gmail.com" },
 ]
 dependencies = [
     "numba>=0.57.0",
     "numpy>=1.21.5",
```

### Comparing `PyExpUtils-andnp-4.0.1/tests/models/test_ExperimentDescription.py` & `PyExpUtils-andnp-5.0.0/tests/models/test_ExperimentDescription.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.1/tests/results/test_indices.py` & `PyExpUtils-andnp-5.0.0/tests/results/test_indices.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.1/tests/results/test_pandas.py` & `PyExpUtils-andnp-5.0.0/tests/results/test_pandas.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.1/tests/results/test_tools.py` & `PyExpUtils-andnp-5.0.0/tests/results/test_tools.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.1/tests/results/test_voting.py` & `PyExpUtils-andnp-5.0.0/tests/results/test_voting.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.1/tests/runner/test_slurm.py` & `PyExpUtils-andnp-5.0.0/tests/runner/test_slurm.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.1/tests/test_FileSystemContext.py` & `PyExpUtils-andnp-5.0.0/tests/test_FileSystemContext.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.1/tests/utils/test_arrays.py` & `PyExpUtils-andnp-5.0.0/tests/utils/test_arrays.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.1/tests/utils/test_cmdline.py` & `PyExpUtils-andnp-5.0.0/tests/utils/test_cmdline.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.1/tests/utils/test_csv.py` & `PyExpUtils-andnp-5.0.0/tests/utils/test_csv.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.1/tests/utils/test_dict.py` & `PyExpUtils-andnp-5.0.0/tests/utils/test_dict.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.1/tests/utils/test_generator.py` & `PyExpUtils-andnp-5.0.0/tests/utils/test_generator.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.1/tests/utils/test_path.py` & `PyExpUtils-andnp-5.0.0/tests/utils/test_path.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.1/tests/utils/test_permute.py` & `PyExpUtils-andnp-5.0.0/tests/utils/test_permute.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.1/tests/utils/test_random.py` & `PyExpUtils-andnp-5.0.0/tests/utils/test_random.py`

 * *Files identical despite different names*

### Comparing `PyExpUtils-andnp-4.0.1/PKG-INFO` & `PyExpUtils-andnp-5.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyExpUtils-andnp
-Version: 4.0.1
+Version: 5.0.0
 Summary: A small set of utilities for RL and ML experiments
 License: MIT
 Author-email: Andy Patterson <andnpatterson@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # PyExpUtils
```

