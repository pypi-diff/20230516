# Comparing `tmp/load-atoms-0.0.8.tar.gz` & `tmp/load-atoms-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "load-atoms-0.0.8.tar", last modified: Fri May 12 13:57:17 2023, max compression
+gzip compressed data, was "load-atoms-0.0.9.tar", last modified: Tue May 16 12:10:20 2023, max compression
```

## Comparing `load-atoms-0.0.8.tar` & `load-atoms-0.0.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-12 13:57:17.953891 load-atoms-0.0.8/
--rw-r--r--   0 john       (504) staff       (20)     1069 2023-04-04 12:18:14.000000 load-atoms-0.0.8/LICENSE
--rw-r--r--   0 john       (504) staff       (20)       48 2023-03-07 08:55:19.000000 load-atoms-0.0.8/MANIFEST.in
--rw-r--r--   0 john       (504) staff       (20)     2767 2023-05-12 13:57:17.953662 load-atoms-0.0.8/PKG-INFO
--rw-r--r--   0 john       (504) staff       (20)      972 2023-04-12 10:09:54.000000 load-atoms-0.0.8/README.md
--rw-r--r--   0 john       (504) staff       (20)     1376 2023-05-12 13:56:11.000000 load-atoms-0.0.8/pyproject.toml
--rw-r--r--   0 john       (504) staff       (20)       38 2023-05-12 13:57:17.953951 load-atoms-0.0.8/setup.cfg
-drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-12 13:57:17.941360 load-atoms-0.0.8/src/
-drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-12 13:57:17.944636 load-atoms-0.0.8/src/load_atoms/
--rw-r--r--   0 john       (504) staff       (20)      127 2023-05-12 13:56:11.000000 load-atoms-0.0.8/src/load_atoms/__init__.py
--rw-r--r--   0 john       (504) staff       (20)     1727 2023-04-05 06:56:03.000000 load-atoms-0.0.8/src/load_atoms/api.py
--rw-r--r--   0 john       (504) staff       (20)     4663 2023-05-12 13:55:30.000000 load-atoms-0.0.8/src/load_atoms/backend.py
--rw-r--r--   0 john       (504) staff       (20)      535 2023-04-05 08:42:48.000000 load-atoms-0.0.8/src/load_atoms/checksums.py
--rw-r--r--   0 john       (504) staff       (20)     2104 2023-05-12 13:55:30.000000 load-atoms-0.0.8/src/load_atoms/database.py
--rw-r--r--   0 john       (504) staff       (20)     3924 2023-05-12 13:55:30.000000 load-atoms-0.0.8/src/load_atoms/dataset.py
-drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-12 13:57:17.947656 load-atoms-0.0.8/src/load_atoms/datasets/
--rw-r--r--   0 john       (504) staff       (20)     1040 2023-04-06 09:55:36.000000 load-atoms-0.0.8/src/load_atoms/datasets/C-GAP-17.yaml
--rw-r--r--   0 john       (504) staff       (20)     1166 2023-04-12 12:15:55.000000 load-atoms-0.0.8/src/load_atoms/datasets/C-GAP-20.yaml
--rw-r--r--   0 john       (504) staff       (20)      760 2023-04-12 09:41:52.000000 load-atoms-0.0.8/src/load_atoms/datasets/C-SYNTH-1M.yaml
--rw-r--r--   0 john       (504) staff       (20)    24624 2023-05-12 13:55:30.000000 load-atoms-0.0.8/src/load_atoms/datasets/C-SYNTH-23M.yaml
--rw-r--r--   0 john       (504) staff       (20)     1356 2023-03-07 08:55:19.000000 load-atoms-0.0.8/src/load_atoms/datasets/QM7.yaml
--rw-r--r--   0 john       (504) staff       (20)     1222 2023-03-07 16:02:25.000000 load-atoms-0.0.8/src/load_atoms/datasets/amorphous-grahpene.yaml
--rw-r--r--   0 john       (504) staff       (20)     1279 2023-05-12 08:34:41.000000 load-atoms-0.0.8/src/load_atoms/manipulations.py
--rw-r--r--   0 john       (504) staff       (20)      946 2023-05-12 13:55:30.000000 load-atoms-0.0.8/src/load_atoms/util.py
-drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-12 13:57:17.945287 load-atoms-0.0.8/src/load_atoms.egg-info/
--rw-r--r--   0 john       (504) staff       (20)     2767 2023-05-12 13:57:17.000000 load-atoms-0.0.8/src/load_atoms.egg-info/PKG-INFO
--rw-r--r--   0 john       (504) staff       (20)      796 2023-05-12 13:57:17.000000 load-atoms-0.0.8/src/load_atoms.egg-info/SOURCES.txt
--rw-r--r--   0 john       (504) staff       (20)        1 2023-05-12 13:57:17.000000 load-atoms-0.0.8/src/load_atoms.egg-info/dependency_links.txt
--rw-r--r--   0 john       (504) staff       (20)      180 2023-05-12 13:57:17.000000 load-atoms-0.0.8/src/load_atoms.egg-info/requires.txt
--rw-r--r--   0 john       (504) staff       (20)       11 2023-05-12 13:57:17.000000 load-atoms-0.0.8/src/load_atoms.egg-info/top_level.txt
-drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-12 13:57:17.952329 load-atoms-0.0.8/tests/
--rw-r--r--   0 john       (504) staff       (20)     1706 2023-05-12 13:55:30.000000 load-atoms-0.0.8/tests/test_backend.py
--rw-r--r--   0 john       (504) staff       (20)     2141 2023-05-12 13:55:30.000000 load-atoms-0.0.8/tests/test_database.py
--rw-r--r--   0 john       (504) staff       (20)     2094 2023-04-06 09:14:52.000000 load-atoms-0.0.8/tests/test_dataset.py
--rw-r--r--   0 john       (504) staff       (20)      853 2023-05-12 08:34:41.000000 load-atoms-0.0.8/tests/test_manipulations.py
--rw-r--r--   0 john       (504) staff       (20)      441 2023-04-05 08:42:48.000000 load-atoms-0.0.8/tests/test_util.py
+drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-16 12:10:20.307698 load-atoms-0.0.9/
+-rw-r--r--   0 john       (504) staff       (20)     1069 2023-04-04 12:18:14.000000 load-atoms-0.0.9/LICENSE
+-rw-r--r--   0 john       (504) staff       (20)       48 2023-03-07 08:55:19.000000 load-atoms-0.0.9/MANIFEST.in
+-rw-r--r--   0 john       (504) staff       (20)     2767 2023-05-16 12:10:20.307136 load-atoms-0.0.9/PKG-INFO
+-rw-r--r--   0 john       (504) staff       (20)      972 2023-04-12 10:09:54.000000 load-atoms-0.0.9/README.md
+-rw-r--r--   0 john       (504) staff       (20)     1376 2023-05-16 12:10:14.000000 load-atoms-0.0.9/pyproject.toml
+-rw-r--r--   0 john       (504) staff       (20)       38 2023-05-16 12:10:20.307840 load-atoms-0.0.9/setup.cfg
+drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-16 12:10:20.297013 load-atoms-0.0.9/src/
+drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-16 12:10:20.299121 load-atoms-0.0.9/src/load_atoms/
+-rw-r--r--   0 john       (504) staff       (20)      127 2023-05-16 12:10:14.000000 load-atoms-0.0.9/src/load_atoms/__init__.py
+-rw-r--r--   0 john       (504) staff       (20)     1727 2023-04-05 06:56:03.000000 load-atoms-0.0.9/src/load_atoms/api.py
+-rw-r--r--   0 john       (504) staff       (20)     4663 2023-05-12 13:55:30.000000 load-atoms-0.0.9/src/load_atoms/backend.py
+-rw-r--r--   0 john       (504) staff       (20)      535 2023-04-05 08:42:48.000000 load-atoms-0.0.9/src/load_atoms/checksums.py
+-rw-r--r--   0 john       (504) staff       (20)     2104 2023-05-12 13:55:30.000000 load-atoms-0.0.9/src/load_atoms/database.py
+-rw-r--r--   0 john       (504) staff       (20)     4354 2023-05-16 12:10:07.000000 load-atoms-0.0.9/src/load_atoms/dataset.py
+drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-16 12:10:20.302600 load-atoms-0.0.9/src/load_atoms/datasets/
+-rw-r--r--   0 john       (504) staff       (20)     1040 2023-04-06 09:55:36.000000 load-atoms-0.0.9/src/load_atoms/datasets/C-GAP-17.yaml
+-rw-r--r--   0 john       (504) staff       (20)     1166 2023-04-12 12:15:55.000000 load-atoms-0.0.9/src/load_atoms/datasets/C-GAP-20.yaml
+-rw-r--r--   0 john       (504) staff       (20)      760 2023-04-12 09:41:52.000000 load-atoms-0.0.9/src/load_atoms/datasets/C-SYNTH-1M.yaml
+-rw-r--r--   0 john       (504) staff       (20)    24624 2023-05-12 13:55:30.000000 load-atoms-0.0.9/src/load_atoms/datasets/C-SYNTH-23M.yaml
+-rw-r--r--   0 john       (504) staff       (20)     1356 2023-03-07 08:55:19.000000 load-atoms-0.0.9/src/load_atoms/datasets/QM7.yaml
+-rw-r--r--   0 john       (504) staff       (20)     1222 2023-03-07 16:02:25.000000 load-atoms-0.0.9/src/load_atoms/datasets/amorphous-grahpene.yaml
+-rw-r--r--   0 john       (504) staff       (20)     1279 2023-05-12 08:34:41.000000 load-atoms-0.0.9/src/load_atoms/manipulations.py
+-rw-r--r--   0 john       (504) staff       (20)     1075 2023-05-16 12:10:07.000000 load-atoms-0.0.9/src/load_atoms/util.py
+drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-16 12:10:20.300126 load-atoms-0.0.9/src/load_atoms.egg-info/
+-rw-r--r--   0 john       (504) staff       (20)     2767 2023-05-16 12:10:20.000000 load-atoms-0.0.9/src/load_atoms.egg-info/PKG-INFO
+-rw-r--r--   0 john       (504) staff       (20)      796 2023-05-16 12:10:20.000000 load-atoms-0.0.9/src/load_atoms.egg-info/SOURCES.txt
+-rw-r--r--   0 john       (504) staff       (20)        1 2023-05-16 12:10:20.000000 load-atoms-0.0.9/src/load_atoms.egg-info/dependency_links.txt
+-rw-r--r--   0 john       (504) staff       (20)      180 2023-05-16 12:10:20.000000 load-atoms-0.0.9/src/load_atoms.egg-info/requires.txt
+-rw-r--r--   0 john       (504) staff       (20)       11 2023-05-16 12:10:20.000000 load-atoms-0.0.9/src/load_atoms.egg-info/top_level.txt
+drwxr-xr-x   0 john       (504) staff       (20)        0 2023-05-16 12:10:20.305129 load-atoms-0.0.9/tests/
+-rw-r--r--   0 john       (504) staff       (20)     1706 2023-05-12 13:55:30.000000 load-atoms-0.0.9/tests/test_backend.py
+-rw-r--r--   0 john       (504) staff       (20)     2141 2023-05-12 13:55:30.000000 load-atoms-0.0.9/tests/test_database.py
+-rw-r--r--   0 john       (504) staff       (20)     2872 2023-05-16 12:10:07.000000 load-atoms-0.0.9/tests/test_dataset.py
+-rw-r--r--   0 john       (504) staff       (20)      853 2023-05-12 08:34:41.000000 load-atoms-0.0.9/tests/test_manipulations.py
+-rw-r--r--   0 john       (504) staff       (20)      441 2023-04-05 08:42:48.000000 load-atoms-0.0.9/tests/test_util.py
```

### Comparing `load-atoms-0.0.8/LICENSE` & `load-atoms-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `load-atoms-0.0.8/PKG-INFO` & `load-atoms-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: load-atoms
-Version: 0.0.8
+Version: 0.0.9
 Summary: Large Open Access Datasets for Atomistic Materials Science (LOAD-AtoMS)
 Author-email: John Gardner <gardner.john97@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 John Gardner
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `load-atoms-0.0.8/README.md` & `load-atoms-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `load-atoms-0.0.8/pyproject.toml` & `load-atoms-0.0.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "load-atoms"
-version = "0.0.8"
+version = "0.0.9"
 description = "Large Open Access Datasets for Atomistic Materials Science (LOAD-AtoMS)"
 readme = "README.md"
 authors = [{ name = "John Gardner", email = "gardner.john97@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -44,15 +44,15 @@
     "twine",
 ]
 
 [project.urls]
 Homepage = "https://github.com/jla-gardner/load-atoms"
 
 [tool.bumpver]
-current_version = "0.0.8"
+current_version = "0.0.9"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `load-atoms-0.0.8/src/load_atoms/api.py` & `load-atoms-0.0.9/src/load_atoms/api.py`

 * *Files identical despite different names*

### Comparing `load-atoms-0.0.8/src/load_atoms/backend.py` & `load-atoms-0.0.9/src/load_atoms/backend.py`

 * *Files identical despite different names*

### Comparing `load-atoms-0.0.8/src/load_atoms/checksums.py` & `load-atoms-0.0.9/src/load_atoms/checksums.py`

 * *Files identical despite different names*

### Comparing `load-atoms-0.0.8/src/load_atoms/database.py` & `load-atoms-0.0.9/src/load_atoms/database.py`

 * *Files identical despite different names*

### Comparing `load-atoms-0.0.8/src/load_atoms/dataset.py` & `load-atoms-0.0.9/src/load_atoms/dataset.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,42 +1,49 @@
 from pathlib import Path
 from typing import Iterable, List
 
+import numpy as np
 from ase import Atoms
 from ase.io import read
 from yaml import dump
 
 from load_atoms import backend
 from load_atoms.database import DATASETS, DatasetDescription, is_known_dataset
-from load_atoms.util import frontend_url, intersection, union
+from load_atoms.util import frontend_url, intersection, is_numpy, union
 
 
 class Dataset:
     def __init__(
         self, structures: Iterable[Atoms], description: DatasetDescription = None
     ):
         self.structures = [*structures]
         self._description = description
 
     def __len__(self):
         return len(self.structures)
 
-    def __getitem__(self, slice):
-        # if the slice can be cast to an int (e.g. is an np.int64), then
-        # return a single structure
-        try:
-            slice = int(slice)
-            return self.structures[slice]
-        except TypeError:
-            pass
-
-        # otherwise, our slice is a slice object,
-        # and we should return a new Dataset
-        sliced_structres = self.structures[slice]
-        return Dataset(sliced_structres)
+    def __getitem__(self, index):
+        # if the passed index is a slice, return a new Dataset object:
+        if isinstance(index, slice):
+            return Dataset(self.structures[index])
+
+        # if the index is iterable, return a new Dataset object:
+        if hasattr(index, "__iter__"):
+            # if the index is a np index, we want to keep the same behaviour
+            # (e.g. passing array of indices, or a boolean array)
+            if is_numpy(index):
+                to_keep = np.arange(len(self))[index]
+                return Dataset([self.structures[i] for i in to_keep])
+
+            # some other iterable, e.g. a list of indices
+            return Dataset([self.structures[i] for i in index])
+
+        # otherwise, we assume the index is an integer,
+        # and return a single structure
+        return self.structures[int(index)]
 
     def __iter__(self):
         return iter(self.structures)
 
     def __repr__(self):
         return summarise_dataset(self.structures, self._description)
```

### Comparing `load-atoms-0.0.8/src/load_atoms/datasets/C-GAP-17.yaml` & `load-atoms-0.0.9/src/load_atoms/datasets/C-GAP-17.yaml`

 * *Files identical despite different names*

### Comparing `load-atoms-0.0.8/src/load_atoms/datasets/C-GAP-20.yaml` & `load-atoms-0.0.9/src/load_atoms/datasets/C-GAP-20.yaml`

 * *Files identical despite different names*

### Comparing `load-atoms-0.0.8/src/load_atoms/datasets/C-SYNTH-1M.yaml` & `load-atoms-0.0.9/src/load_atoms/datasets/C-SYNTH-1M.yaml`

 * *Files identical despite different names*

### Comparing `load-atoms-0.0.8/src/load_atoms/datasets/C-SYNTH-23M.yaml` & `load-atoms-0.0.9/src/load_atoms/datasets/C-SYNTH-23M.yaml`

 * *Files identical despite different names*

### Comparing `load-atoms-0.0.8/src/load_atoms/datasets/QM7.yaml` & `load-atoms-0.0.9/src/load_atoms/datasets/QM7.yaml`

 * *Files identical despite different names*

### Comparing `load-atoms-0.0.8/src/load_atoms/datasets/amorphous-grahpene.yaml` & `load-atoms-0.0.9/src/load_atoms/datasets/amorphous-grahpene.yaml`

 * *Files identical despite different names*

### Comparing `load-atoms-0.0.8/src/load_atoms/manipulations.py` & `load-atoms-0.0.9/src/load_atoms/manipulations.py`

 * *Files identical despite different names*

### Comparing `load-atoms-0.0.8/src/load_atoms/util.py` & `load-atoms-0.0.9/src/load_atoms/util.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from pathlib import Path
 from typing import Iterable
 
+import numpy as np
+
 # this file is at <root>/src/load_atoms/util.py
 # the datasets are at <root>/src/load_atoms/datasets
 DATASETS_DIR = (Path(__file__).parent / "datasets").resolve()
 DEFAULT_DOWNLOAD_DIR = Path.home() / ".load_atoms"
 BASE_REMOTE_URL = (
     "https://github.com/jla-gardner/load-atoms/raw/main/src/load_atoms/datasets/"
 )
@@ -24,7 +26,12 @@
     """Get the set intersection of a list of iterables."""
     return set.intersection(*map(set, things))
 
 
 def union(things: Iterable[Iterable]):
     """Get the set union of a list of iterables."""
     return set.union(*map(set, things))
+
+
+def is_numpy(thing):
+    """Check if a thing is a numpy array."""
+    return isinstance(thing, np.ndarray)
```

### Comparing `load-atoms-0.0.8/src/load_atoms.egg-info/PKG-INFO` & `load-atoms-0.0.9/src/load_atoms.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: load-atoms
-Version: 0.0.8
+Version: 0.0.9
 Summary: Large Open Access Datasets for Atomistic Materials Science (LOAD-AtoMS)
 Author-email: John Gardner <gardner.john97@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 John Gardner
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `load-atoms-0.0.8/src/load_atoms.egg-info/SOURCES.txt` & `load-atoms-0.0.9/src/load_atoms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `load-atoms-0.0.8/tests/test_backend.py` & `load-atoms-0.0.9/tests/test_backend.py`

 * *Files identical despite different names*

### Comparing `load-atoms-0.0.8/tests/test_database.py` & `load-atoms-0.0.9/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `load-atoms-0.0.8/tests/test_dataset.py` & `load-atoms-0.0.9/tests/test_dataset.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from pathlib import Path
 
+import numpy as np
 import pytest
 from ase import Atoms
 from ase.io import read, write
 
 from load_atoms import dataset
 from load_atoms.dataset import Dataset, summarise_dataset
 
@@ -27,27 +28,48 @@
     ds2 = dataset(read(tmp_path / "test.xyz", index=":"))
     _is_water_dataset(ds2)
 
     ds3 = dataset(tmp_path / "test.xyz")
     _is_water_dataset(ds3)
 
 
-def test_slice():
+def test_indexing():
     ds = dataset(STRUCTURES)
 
     structure = ds[0]
     assert isinstance(structure, Atoms), "Indexing should return an Atoms object"
     assert structure is STRUCTURES[0], "Indexing should return the same structure"
 
     sub_dataset = ds[1:]
     assert isinstance(sub_dataset, Dataset), "Slicing should return a dataset"
     assert (
         len(sub_dataset) == 1
     ), "Slicing should return the correct number of structures"
 
+    indices = np.array([0, 1, 0, 1])
+    sub_dataset = ds[indices]
+    assert isinstance(sub_dataset, Dataset), "Indexing should return a dataset"
+    assert (
+        len(sub_dataset) == 4
+    ), "Indexing should return the correct number of structures"
+
+    indices = np.array([True, False])
+    sub_dataset = ds[indices]
+    assert isinstance(sub_dataset, Dataset), "Indexing should return a dataset"
+    assert (
+        len(sub_dataset) == 1
+    ), "Indexing should return the correct number of structures"
+
+    indices = [0, 1, 1]
+    sub_dataset = ds[indices]
+    assert isinstance(sub_dataset, Dataset), "Indexing should return a dataset"
+    assert (
+        len(sub_dataset) == 3
+    ), "Indexing should return the correct number of structures"
+
 
 def test_can_load_from_id():
     # pass root to avoid downloading the dataset
     structures = dataset("QM7", root="src/load_atoms/datasets")
     assert len(structures) == 7165
 
     with pytest.raises(ValueError, match="is not known."):
```

### Comparing `load-atoms-0.0.8/tests/test_manipulations.py` & `load-atoms-0.0.9/tests/test_manipulations.py`

 * *Files identical despite different names*

