# Comparing `tmp/fibertools-0.2.9.tar.gz` & `tmp/fibertools-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fibertools-0.2.9.tar", last modified: Wed Nov 30 00:56:58 2022, max compression
+gzip compressed data, was "fibertools-0.3.0.tar", last modified: Tue May 16 18:15:37 2023, max compression
```

## Comparing `fibertools-0.2.9.tar` & `fibertools-0.3.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 mrvollger   (501) staff       (20)        0 2022-11-30 00:56:58.031886 fibertools-0.2.9/
--rw-r--r--   0 mrvollger   (501) staff       (20)      164 2022-05-01 17:12:39.000000 fibertools-0.2.9/AUTHORS.rst
--rw-r--r--   0 mrvollger   (501) staff       (20)     3563 2022-05-01 17:12:39.000000 fibertools-0.2.9/CONTRIBUTING.rst
--rw-r--r--   0 mrvollger   (501) staff       (20)       89 2022-05-01 17:12:39.000000 fibertools-0.2.9/HISTORY.rst
--rw-r--r--   0 mrvollger   (501) staff       (20)     1078 2022-05-01 17:12:39.000000 fibertools-0.2.9/LICENSE
--rw-r--r--   0 mrvollger   (501) staff       (20)      262 2022-05-01 17:12:39.000000 fibertools-0.2.9/MANIFEST.in
--rw-r--r--   0 mrvollger   (501) staff       (20)     1896 2022-11-30 00:56:58.032029 fibertools-0.2.9/PKG-INFO
--rw-r--r--   0 mrvollger   (501) staff       (20)     1045 2022-05-01 17:12:39.000000 fibertools-0.2.9/README.rst
-drwxr-xr-x   0 mrvollger   (501) staff       (20)        0 2022-11-30 00:56:58.014618 fibertools-0.2.9/docs/
--rw-r--r--   0 mrvollger   (501) staff       (20)      611 2022-05-01 17:12:39.000000 fibertools-0.2.9/docs/Makefile
-drwxr-xr-x   0 mrvollger   (501) staff       (20)        0 2022-11-30 00:56:58.002458 fibertools-0.2.9/docs/_build/
-drwxr-xr-x   0 mrvollger   (501) staff       (20)        0 2022-11-30 00:56:58.002566 fibertools-0.2.9/docs/_build/html/
-drwxr-xr-x   0 mrvollger   (501) staff       (20)        0 2022-11-30 00:56:58.016821 fibertools-0.2.9/docs/_build/html/_static/
--rw-r--r--   0 mrvollger   (501) staff       (20)      286 2021-09-12 10:17:28.000000 fibertools-0.2.9/docs/_build/html/_static/file.png
--rw-r--r--   0 mrvollger   (501) staff       (20)       90 2021-09-12 10:17:28.000000 fibertools-0.2.9/docs/_build/html/_static/minus.png
--rw-r--r--   0 mrvollger   (501) staff       (20)       90 2021-09-12 10:17:28.000000 fibertools-0.2.9/docs/_build/html/_static/plus.png
--rw-r--r--   0 mrvollger   (501) staff       (20)       28 2022-05-01 17:12:39.000000 fibertools-0.2.9/docs/authors.rst
--rwxr-xr-x   0 mrvollger   (501) staff       (20)     5236 2022-05-02 00:22:35.000000 fibertools-0.2.9/docs/conf.py
--rw-r--r--   0 mrvollger   (501) staff       (20)       33 2022-05-01 17:12:39.000000 fibertools-0.2.9/docs/contributing.rst
--rw-r--r--   0 mrvollger   (501) staff       (20)     1186 2022-06-04 23:44:28.000000 fibertools-0.2.9/docs/fibertools.rst
--rw-r--r--   0 mrvollger   (501) staff       (20)       28 2022-05-01 17:12:39.000000 fibertools-0.2.9/docs/history.rst
--rw-r--r--   0 mrvollger   (501) staff       (20)      307 2022-05-01 21:38:31.000000 fibertools-0.2.9/docs/index.rst
--rw-r--r--   0 mrvollger   (501) staff       (20)     1142 2022-05-01 17:12:39.000000 fibertools-0.2.9/docs/installation.rst
--rw-r--r--   0 mrvollger   (501) staff       (20)      772 2022-05-01 17:12:39.000000 fibertools-0.2.9/docs/make.bat
--rw-r--r--   0 mrvollger   (501) staff       (20)       67 2022-06-04 23:43:20.000000 fibertools-0.2.9/docs/modules.rst
--rw-r--r--   0 mrvollger   (501) staff       (20)       27 2022-05-01 17:12:39.000000 fibertools-0.2.9/docs/readme.rst
--rw-r--r--   0 mrvollger   (501) staff       (20)     1172 2022-06-04 23:15:16.000000 fibertools-0.2.9/docs/usage.rst
-drwxr-xr-x   0 mrvollger   (501) staff       (20)        0 2022-11-30 00:56:58.023810 fibertools-0.2.9/fibertools/
--rw-r--r--   0 mrvollger   (501) staff       (20)      186 2022-11-30 00:55:05.000000 fibertools-0.2.9/fibertools/__init__.py
--rwxr-xr-x   0 mrvollger   (501) staff       (20)    18328 2022-11-30 00:54:41.000000 fibertools-0.2.9/fibertools/add_nucleosomes.py
--rw-r--r--   0 mrvollger   (501) staff       (20)     6056 2022-08-22 15:39:37.000000 fibertools-0.2.9/fibertools/classify.py
--rw-r--r--   0 mrvollger   (501) staff       (20)    12696 2022-11-30 00:08:40.000000 fibertools-0.2.9/fibertools/cli.py
--rw-r--r--   0 mrvollger   (501) staff       (20)     9557 2022-08-22 15:31:48.000000 fibertools-0.2.9/fibertools/fiberdata.py
--rw-r--r--   0 mrvollger   (501) staff       (20)      130 2022-05-02 01:12:16.000000 fibertools-0.2.9/fibertools/fibertools.py
--rw-r--r--   0 mrvollger   (501) staff       (20)     4488 2022-08-19 21:09:11.000000 fibertools-0.2.9/fibertools/readutils.py
--rw-r--r--   0 mrvollger   (501) staff       (20)     4267 2022-08-18 23:46:37.000000 fibertools-0.2.9/fibertools/trackhub.py
--rw-r--r--   0 mrvollger   (501) staff       (20)     5009 2022-08-23 18:41:39.000000 fibertools-0.2.9/fibertools/unionbg.py
--rw-r--r--   0 mrvollger   (501) staff       (20)     5203 2022-08-18 17:17:32.000000 fibertools-0.2.9/fibertools/utils.py
-drwxr-xr-x   0 mrvollger   (501) staff       (20)        0 2022-11-30 00:56:58.026353 fibertools-0.2.9/fibertools.egg-info/
--rw-r--r--   0 mrvollger   (501) staff       (20)     1896 2022-11-30 00:56:57.000000 fibertools-0.2.9/fibertools.egg-info/PKG-INFO
--rw-r--r--   0 mrvollger   (501) staff       (20)      926 2022-11-30 00:56:57.000000 fibertools-0.2.9/fibertools.egg-info/SOURCES.txt
--rw-r--r--   0 mrvollger   (501) staff       (20)        1 2022-11-30 00:56:57.000000 fibertools-0.2.9/fibertools.egg-info/dependency_links.txt
--rw-r--r--   0 mrvollger   (501) staff       (20)       58 2022-11-30 00:56:57.000000 fibertools-0.2.9/fibertools.egg-info/entry_points.txt
--rw-r--r--   0 mrvollger   (501) staff       (20)        1 2022-11-30 00:56:57.000000 fibertools-0.2.9/fibertools.egg-info/not-zip-safe
--rw-r--r--   0 mrvollger   (501) staff       (20)      284 2022-11-30 00:56:57.000000 fibertools-0.2.9/fibertools.egg-info/requires.txt
--rw-r--r--   0 mrvollger   (501) staff       (20)       11 2022-11-30 00:56:57.000000 fibertools-0.2.9/fibertools.egg-info/top_level.txt
--rw-r--r--   0 mrvollger   (501) staff       (20)      382 2022-11-30 00:56:58.032544 fibertools-0.2.9/setup.cfg
--rw-r--r--   0 mrvollger   (501) staff       (20)     2243 2022-11-30 00:55:05.000000 fibertools-0.2.9/setup.py
-drwxr-xr-x   0 mrvollger   (501) staff       (20)        0 2022-11-30 00:56:58.031313 fibertools-0.2.9/tests/
--rw-r--r--   0 mrvollger   (501) staff       (20)       40 2022-05-01 17:12:39.000000 fibertools-0.2.9/tests/__init__.py
--rw-r--r--   0 mrvollger   (501) staff       (20)  1174377 2022-08-19 16:58:05.000000 fibertools-0.2.9/tests/all.tbl.gz
--rw-r--r--   0 mrvollger   (501) staff       (20)      397 2022-05-01 23:04:14.000000 fibertools-0.2.9/tests/test_fibertools.py
+drwxr-xr-x   0 mrvollger   (501) staff       (20)        0 2023-05-16 18:15:37.336285 fibertools-0.3.0/
+-rw-r--r--   0 mrvollger   (501) staff       (20)      164 2022-05-01 17:12:39.000000 fibertools-0.3.0/AUTHORS.rst
+-rw-r--r--   0 mrvollger   (501) staff       (20)     3563 2022-05-01 17:12:39.000000 fibertools-0.3.0/CONTRIBUTING.rst
+-rw-r--r--   0 mrvollger   (501) staff       (20)       89 2022-05-01 17:12:39.000000 fibertools-0.3.0/HISTORY.rst
+-rw-r--r--   0 mrvollger   (501) staff       (20)     1078 2022-05-01 17:12:39.000000 fibertools-0.3.0/LICENSE
+-rw-r--r--   0 mrvollger   (501) staff       (20)      262 2022-05-01 17:12:39.000000 fibertools-0.3.0/MANIFEST.in
+-rw-r--r--   0 mrvollger   (501) staff       (20)     3355 2023-05-16 18:15:37.336404 fibertools-0.3.0/PKG-INFO
+-rw-r--r--   0 mrvollger   (501) staff       (20)     2504 2022-11-30 01:54:01.000000 fibertools-0.3.0/README.rst
+drwxr-xr-x   0 mrvollger   (501) staff       (20)        0 2023-05-16 18:15:37.325950 fibertools-0.3.0/docs/
+-rw-r--r--   0 mrvollger   (501) staff       (20)      611 2022-05-01 17:12:39.000000 fibertools-0.3.0/docs/Makefile
+drwxr-xr-x   0 mrvollger   (501) staff       (20)        0 2023-05-16 18:15:37.314173 fibertools-0.3.0/docs/_build/
+drwxr-xr-x   0 mrvollger   (501) staff       (20)        0 2023-05-16 18:15:37.314374 fibertools-0.3.0/docs/_build/html/
+drwxr-xr-x   0 mrvollger   (501) staff       (20)        0 2023-05-16 18:15:37.326928 fibertools-0.3.0/docs/_build/html/_static/
+-rw-r--r--   0 mrvollger   (501) staff       (20)      286 2021-09-12 10:17:28.000000 fibertools-0.3.0/docs/_build/html/_static/file.png
+-rw-r--r--   0 mrvollger   (501) staff       (20)       90 2021-09-12 10:17:28.000000 fibertools-0.3.0/docs/_build/html/_static/minus.png
+-rw-r--r--   0 mrvollger   (501) staff       (20)       90 2021-09-12 10:17:28.000000 fibertools-0.3.0/docs/_build/html/_static/plus.png
+-rw-r--r--   0 mrvollger   (501) staff       (20)       28 2022-05-01 17:12:39.000000 fibertools-0.3.0/docs/authors.rst
+-rwxr-xr-x   0 mrvollger   (501) staff       (20)     5236 2022-05-02 00:22:35.000000 fibertools-0.3.0/docs/conf.py
+-rw-r--r--   0 mrvollger   (501) staff       (20)       33 2022-05-01 17:12:39.000000 fibertools-0.3.0/docs/contributing.rst
+-rw-r--r--   0 mrvollger   (501) staff       (20)     1186 2022-06-04 23:44:28.000000 fibertools-0.3.0/docs/fibertools.rst
+-rw-r--r--   0 mrvollger   (501) staff       (20)       28 2022-05-01 17:12:39.000000 fibertools-0.3.0/docs/history.rst
+-rw-r--r--   0 mrvollger   (501) staff       (20)      307 2022-05-01 21:38:31.000000 fibertools-0.3.0/docs/index.rst
+-rw-r--r--   0 mrvollger   (501) staff       (20)     1142 2022-05-01 17:12:39.000000 fibertools-0.3.0/docs/installation.rst
+-rw-r--r--   0 mrvollger   (501) staff       (20)      772 2022-05-01 17:12:39.000000 fibertools-0.3.0/docs/make.bat
+-rw-r--r--   0 mrvollger   (501) staff       (20)       67 2022-06-04 23:43:20.000000 fibertools-0.3.0/docs/modules.rst
+-rw-r--r--   0 mrvollger   (501) staff       (20)       27 2022-05-01 17:12:39.000000 fibertools-0.3.0/docs/readme.rst
+-rw-r--r--   0 mrvollger   (501) staff       (20)     1172 2022-06-04 23:15:16.000000 fibertools-0.3.0/docs/usage.rst
+drwxr-xr-x   0 mrvollger   (501) staff       (20)        0 2023-05-16 18:15:37.331155 fibertools-0.3.0/fibertools/
+-rw-r--r--   0 mrvollger   (501) staff       (20)      186 2023-05-16 18:14:55.000000 fibertools-0.3.0/fibertools/__init__.py
+-rwxr-xr-x   0 mrvollger   (501) staff       (20)    22405 2023-02-22 18:20:31.000000 fibertools-0.3.0/fibertools/add_nucleosomes.py
+-rw-r--r--   0 mrvollger   (501) staff       (20)     6761 2023-05-03 04:40:10.000000 fibertools-0.3.0/fibertools/classify.py
+-rw-r--r--   0 mrvollger   (501) staff       (20)    15745 2023-05-11 18:32:25.000000 fibertools-0.3.0/fibertools/cli.py
+-rw-r--r--   0 mrvollger   (501) staff       (20)    11405 2023-05-11 18:32:35.000000 fibertools-0.3.0/fibertools/fiberdata.py
+-rw-r--r--   0 mrvollger   (501) staff       (20)      130 2022-05-02 01:12:16.000000 fibertools-0.3.0/fibertools/fibertools.py
+-rw-r--r--   0 mrvollger   (501) staff       (20)     4488 2023-04-25 22:06:10.000000 fibertools-0.3.0/fibertools/readutils.py
+-rw-r--r--   0 mrvollger   (501) staff       (20)     5775 2023-05-16 18:02:45.000000 fibertools-0.3.0/fibertools/trackhub.py
+-rw-r--r--   0 mrvollger   (501) staff       (20)     5590 2023-04-26 04:01:02.000000 fibertools-0.3.0/fibertools/unionbg.py
+-rw-r--r--   0 mrvollger   (501) staff       (20)     5447 2023-04-25 22:08:40.000000 fibertools-0.3.0/fibertools/utils.py
+drwxr-xr-x   0 mrvollger   (501) staff       (20)        0 2023-05-16 18:15:37.333680 fibertools-0.3.0/fibertools.egg-info/
+-rw-r--r--   0 mrvollger   (501) staff       (20)     3355 2023-05-16 18:15:37.000000 fibertools-0.3.0/fibertools.egg-info/PKG-INFO
+-rw-r--r--   0 mrvollger   (501) staff       (20)      926 2023-05-16 18:15:37.000000 fibertools-0.3.0/fibertools.egg-info/SOURCES.txt
+-rw-r--r--   0 mrvollger   (501) staff       (20)        1 2023-05-16 18:15:37.000000 fibertools-0.3.0/fibertools.egg-info/dependency_links.txt
+-rw-r--r--   0 mrvollger   (501) staff       (20)       58 2023-05-16 18:15:37.000000 fibertools-0.3.0/fibertools.egg-info/entry_points.txt
+-rw-r--r--   0 mrvollger   (501) staff       (20)        1 2023-05-16 18:15:37.000000 fibertools-0.3.0/fibertools.egg-info/not-zip-safe
+-rw-r--r--   0 mrvollger   (501) staff       (20)      261 2023-05-16 18:15:37.000000 fibertools-0.3.0/fibertools.egg-info/requires.txt
+-rw-r--r--   0 mrvollger   (501) staff       (20)       11 2023-05-16 18:15:37.000000 fibertools-0.3.0/fibertools.egg-info/top_level.txt
+-rw-r--r--   0 mrvollger   (501) staff       (20)      382 2023-05-16 18:15:37.337752 fibertools-0.3.0/setup.cfg
+-rw-r--r--   0 mrvollger   (501) staff       (20)     2243 2023-05-16 18:14:55.000000 fibertools-0.3.0/setup.py
+drwxr-xr-x   0 mrvollger   (501) staff       (20)        0 2023-05-16 18:15:37.335980 fibertools-0.3.0/tests/
+-rw-r--r--   0 mrvollger   (501) staff       (20)       40 2022-05-01 17:12:39.000000 fibertools-0.3.0/tests/__init__.py
+-rw-r--r--   0 mrvollger   (501) staff       (20)  1174377 2022-08-19 16:58:05.000000 fibertools-0.3.0/tests/all.tbl.gz
+-rw-r--r--   0 mrvollger   (501) staff       (20)      397 2022-05-01 23:04:14.000000 fibertools-0.3.0/tests/test_fibertools.py
```

### Comparing `fibertools-0.2.9/CONTRIBUTING.rst` & `fibertools-0.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `fibertools-0.2.9/LICENSE` & `fibertools-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fibertools-0.2.9/docs/Makefile` & `fibertools-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fibertools-0.2.9/docs/conf.py` & `fibertools-0.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `fibertools-0.2.9/docs/fibertools.rst` & `fibertools-0.3.0/docs/fibertools.rst`

 * *Files identical despite different names*

### Comparing `fibertools-0.2.9/docs/installation.rst` & `fibertools-0.3.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `fibertools-0.2.9/docs/make.bat` & `fibertools-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `fibertools-0.2.9/docs/usage.rst` & `fibertools-0.3.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `fibertools-0.2.9/fibertools/add_nucleosomes.py` & `fibertools-0.3.0/fibertools/add_nucleosomes.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,51 @@
 #!/usr/bin/env python3
 import pysam
 import numpy as np
 import logging
 import pomegranate as pom
 import array
 import sys
+import tqdm
+from numba import njit
 
 D_TYPE = np.int64
 
 
+# @jit
+def rle_helper(ia):
+    n = ia.shape[0]
+    y = ia[1:] != ia[:-1]  # pairwise unequal (string safe)
+    i = np.append(np.where(y), n - 1)  # must include last element posi
+    z = np.diff(np.append(-1, i))  # run lengths
+    p = np.cumsum(np.append(0, z))[:-1]  # positions
+    return (z, p, ia[i])
+
+
+def rle(inarray):
+    """run length encoding. Partial credit to R rle function.
+    Multi datatype arrays catered for including non Numpy
+    returns: tuple (runlengths, startpositions, values)
+    https://stackoverflow.com/questions/1066758/
+    find-length-of-sequences-of-identical-values-in-a-numpy-array-run-length-encodi
+    """
+    ia = np.asarray(inarray, dtype=D_TYPE)  # force numpyS
+    return rle_helper(ia)
+
+
 def train_hmm(data, n_jobs=1):
     logging.info(
         f"Training HMM with {len(data)} training sequences and {n_jobs} threads"
     )
     model = pom.HiddenMarkovModel().from_samples(
         pom.DiscreteDistribution,
         n_components=2,
         X=data,
         verbose=False,
-        max_iterations=250,
+        max_iterations=100,
         n_init=10,
         n_jobs=n_jobs,
     )
     model.bake()
     return model
 
 
@@ -36,28 +59,37 @@
     else:
         actuated = 1
         nucleated = 0
 
     return actuated, nucleated
 
 
-def get_mods_from_rec(rec, mods=[("A", 0, "a"), ("T", 1, "a")], mask=True):
-    if rec.modified_bases is None:
+def get_mods_from_rec(
+    rec, mods=[("A", 0, "a"), ("T", 1, "a")], mask=True, ml_cutoff=200
+):
+    if rec.modified_bases_forward is None:
         return None, None, None
     seq = np.frombuffer(bytes(rec.query_sequence, "utf-8"), dtype="S1")
+    # Reverse the seq if reverse strand so we set the mask right later
+    if rec.is_reverse:
+        seq = seq[::-1]
+
     positions = []
     for mod in mods:
-        if mod in rec.modified_bases:
-            pos = np.array(rec.modified_bases[mod], dtype=D_TYPE)[:, 0]
+        if mod in rec.modified_bases_forward:
+            all_pos = np.array(rec.modified_bases_forward[mod], dtype=D_TYPE)
+            pos = all_pos[all_pos[:, 1] > ml_cutoff, 0]
             positions.append(pos)
     if len(positions) < 1:
         return None, None, None
     methylated_positions = np.concatenate(positions, dtype=D_TYPE)
     methylated_positions.sort(kind="mergesort")
 
+    # if on the reverse strand A become T and vice versa so the mask doenst need to be
+    # changes for rev comp
     AT_mask = (seq == b"A") | (seq == b"T")
     AT_positions = np.argwhere(AT_mask).transpose()[0]
 
     binary = np.zeros(shape=len(seq), dtype=np.uint8)
     binary[methylated_positions] = 1
 
     if mask:
@@ -70,14 +102,15 @@
     simple_starts,
     simple_sizes,
     hmm_starts,
     hmm_sizes,
     methylated_positions,
     fiber_length,
     cutoff,
+    nuc_size_cutoff,
 ):
 
     ###FILTERS TO IMPLEMENT ########
 
     #### BASELINE is simple caller
 
     # HMM calls are used to modify aspects of the simple called nucleosomes
@@ -178,80 +211,114 @@
     nucleosome_sizes = np.concatenate(nucleosome_sizes)
 
     sort_order = np.argsort(nucleosome_starts).reshape(-1)
 
     nucleosome_starts = nucleosome_starts[sort_order]
     nucleosome_sizes = nucleosome_sizes[sort_order]
 
-    min_nuc_size_mask = nucleosome_sizes >= cutoff
+    min_nuc_size_mask = nucleosome_sizes >= nuc_size_cutoff
 
     return nucleosome_starts[min_nuc_size_mask], nucleosome_sizes[min_nuc_size_mask]
     # grab valid hmm calls and bookend to be min length
     # first minmum length
     # next check that it is flanked by 0s
 
 
-def apply_hmm(bam, hmm, nuc_label, cutoff, out, min_dist=46):
-    for rec in bam.fetch(until_eof=True):
+def predict_with_hmm(hmm, binary, nuc_label, AT_positions, cutoff):
+    state_path = hmm.predict(binary)
+    # starts indicate start in AT binary array
+    # lengths indicates length in AT binary space
+    # labels is the state label
+    lengths, starts, labels = rle(state_path)
+
+    # move to genomic space instead of AT
+    hmm_nucleosome_mask = labels == nuc_label
+    hmm_nuc_ends = AT_positions[
+        np.add(starts[hmm_nucleosome_mask], lengths[hmm_nucleosome_mask] - 1)
+    ]
+    hmm_nuc_starts = AT_positions[starts[hmm_nucleosome_mask]]
+    hmm_nuc_sizes = hmm_nuc_ends - hmm_nuc_starts
+    hmm_sizing_mask = hmm_nuc_sizes >= cutoff
+    hmm_nuc_sizes = hmm_nuc_sizes[hmm_sizing_mask]
+    hmm_nuc_starts = hmm_nuc_starts[hmm_sizing_mask]
+
+    correct_sizes = hmm_nuc_starts[:-1] + hmm_nuc_sizes[:-1] <= hmm_nuc_starts[1:]
+    if not np.all(correct_sizes):
+        logging.warning(f"HMM invalid ranges.")
+    return hmm_nuc_starts, hmm_nuc_sizes
+
+
+def apply_hmm(
+    bam,
+    hmm,
+    nuc_label,
+    cutoff,
+    nuc_size_cutoff,
+    out,
+    min_dist=46,
+    ml_cutoff=200,
+    simple_only=False,
+    hmm_only=False,
+):
+    for rec in tqdm.tqdm(bam.fetch(until_eof=True)):
+        # clear previous calling methods:
+        for tag in ["ns", "nl", "as", "al"]:
+            rec.set_tag(tag, array.array("I", []), replace=True)
+
         (
             binary,
             AT_positions,
             methylated_positions,
-        ) = get_mods_from_rec(rec, mask=True)
+        ) = get_mods_from_rec(rec, mask=True, ml_cutoff=ml_cutoff)
+
+        # skip if there are no mods
         if binary is None:
             out.write(rec)
             continue
-        # binary of m6A calls in AT space, and AT positions relative to 0-based fiber start
 
-        simple_starts, simple_sizes, generated_terminal = simpleFind(
-            methylated_positions, binary, cutoff
-        )
+        fiber_length = len(rec.query_sequence)
 
+        # binary of m6A calls in AT space, and AT positions relative to 0-based fiber start
         # generated terminal is a boolean indicating if we generated a custom
         # nucleosome until tht terminal end of the fiber
+        simple_starts, simple_sizes, generated_terminal = simpleFind(
+            methylated_positions, binary, cutoff
+        )
 
-        state_path = hmm.predict(binary)
-        # print(len(binary))
-
-        lengths, starts, labels = rle(state_path)
-        # starts indicate start in AT binary array
-        # lengths indicates length in AT binary space
-        # labels is the state label
-
-        hmm_nucleosome_mask = labels == nuc_label
-
-        hmm_nuc_ends = AT_positions[
-            np.add(starts[hmm_nucleosome_mask], lengths[hmm_nucleosome_mask] - 1)
-        ]
-        hmm_nuc_starts = AT_positions[starts[hmm_nucleosome_mask]]
-
-        hmm_nuc_sizes = hmm_nuc_ends - hmm_nuc_starts
-
-        hmm_sizing_mask = hmm_nuc_sizes >= cutoff
-
-        hmm_nuc_sizes = hmm_nuc_sizes[hmm_sizing_mask]
-        hmm_nuc_starts = hmm_nuc_starts[hmm_sizing_mask]
-
-        fiber_length = len(rec.query_sequence)
-
-        all_starts, all_sizes = meshMethods(
-            simple_starts,
-            simple_sizes,
-            hmm_nuc_starts,
-            hmm_nuc_sizes,
-            methylated_positions,
-            fiber_length,
-            cutoff,
+        # apply hmm
+        hmm_nuc_starts, hmm_nuc_sizes = predict_with_hmm(
+            hmm, binary, nuc_label, AT_positions, cutoff
         )
 
+        # apply the appropriate calling method
+        if simple_only:
+            all_starts, all_sizes = mrv_simple_caller(methylated_positions, cutoff)
+            # logging.warn(
+            #    f"{np.column_stack((all_starts, all_starts+all_sizes, all_sizes))}"
+            # )
+        elif hmm_only:
+            all_starts, all_sizes = hmm_nuc_starts, hmm_nuc_sizes
+        else:
+            all_starts, all_sizes = meshMethods(
+                simple_starts,
+                simple_sizes,
+                hmm_nuc_starts,
+                hmm_nuc_sizes,
+                methylated_positions,
+                fiber_length,
+                cutoff,
+                nuc_size_cutoff,
+            )
+
         output_starts = all_starts
         output_sizes = all_sizes
 
         # no nucleosomes found, continue
         if methylated_positions.shape[0] == 0 or output_sizes.shape[0] == 0:
+            logging.info("No nucleosomes found for {}".format(rec.query_name))
             out.write(rec)
             continue
 
         # now need to bookend the fibers with the terminal nucleosomes
         # only need to bookend if hmm or simplecaller did not handle it
         # i.e. only need to book end front if there is not a 1 present in the nuc_starts
         # and only nee to book end end if there is not fib-length - 1 in
@@ -281,36 +348,42 @@
         output_starts = np.concatenate(
             [[front_terminal_nuc_start], all_starts], dtype=D_TYPE
         )
         output_sizes = np.concatenate(
             [[front_terminal_nuc_size], all_sizes], dtype=D_TYPE
         )
 
-        # check that the hmm is only making ranges that are possible.
+        # nucs always bookend the fiber, but now changing that here since we are not doing bed12
+        assert (
+            output_starts[0] == 0
+            and output_starts[-1] + output_sizes[-1] == fiber_length
+        )
+        output_starts = output_starts[1:-1]
+        output_sizes = output_sizes[1:-1]
+
+        # check that we are only making ranges that are possible.
         correct_sizes = output_starts[:-1] + output_sizes[:-1] <= output_starts[1:]
         if not np.all(correct_sizes):
             logging.warning(
-                f"HMM made invalid ranges for {rec.query_name} skipping nucelosome calling for fiber"
+                f"Made invalid ranges for {rec.query_name} skipping nucleosome calling for fiber"
             )
+            nuc_ends = output_starts[:-1] + output_sizes[:-1]
+            next_nuc_starts = output_starts[1:]
+            failed = np.column_stack([nuc_ends, next_nuc_starts, output_sizes[:-1]])[
+                ~correct_sizes
+            ]
+            logging.warning(f"Failed: {failed}\n{np.where(~correct_sizes)}")
             out.write(rec)
             continue
 
         # make the acc arrays
         acc_starts = (output_starts + output_sizes)[:-1]
         acc_ends = output_starts[1:]
         acc_sizes = acc_ends - acc_starts
 
-        # nucs always bookend the fiber, but now changing that here
-        assert (
-            output_starts[0] == 0
-            and output_starts[-1] + output_sizes[-1] == fiber_length
-        )
-        output_starts = output_starts[1:-1]
-        output_sizes = output_sizes[1:-1]
-
         # check that nucleosomes are not too close to the ends of the fiber, and have non-zero size
         cond = (
             (output_starts >= min_dist)
             & ((output_starts + output_sizes) <= (fiber_length - min_dist))
             & (output_sizes > 0)
         )
         output_starts_2 = output_starts[cond]
@@ -328,26 +401,55 @@
         n_msp = acc_starts_2.shape[0]
         n_nuc = output_starts_2.shape[0]
         assert (
             abs(n_msp - n_nuc) < 2
         ), f"Number of nucleosomes must be within 1 of the number of MSP elements: MSP({n_msp}), Nuc({n_nuc})"
 
         if output_sizes.shape[0] > 0:
-            rec.set_tag("ns", array.array("I", output_starts_2))
-            rec.set_tag("nl", array.array("I", output_sizes_2))
+            rec.set_tag("ns", array.array("I", output_starts_2), replace=True)
+            rec.set_tag("nl", array.array("I", output_sizes_2), replace=True)
+            logging.debug(f"ns nl set for fiber: {rec.query_name}")
         if acc_sizes.shape[0] > 0:
-            rec.set_tag("as", array.array("I", acc_starts_2))
-            rec.set_tag("al", array.array("I", acc_sizes_2))
+            rec.set_tag("as", array.array("I", acc_starts_2), replace=True)
+            rec.set_tag("al", array.array("I", acc_sizes_2), replace=True)
+            logging.debug(f"as al set for fiber: {rec.query_name}")
         out.write(rec)
 
 
+@njit
+def mrv_simple_caller(methylated_positions, min_nuc_size, max_m6a_in_nuc=2):
+    # previous m6a that marked a nucleosome end
+    prev_pos = -1
+    # number of m6a seen in the current attempt to make a nucleosome
+    cur_m6a_count = 0
+    # starts and lengths of nucleosomes
+    starts = []
+    sizes = []
+    for m6a_pos in methylated_positions:
+        dist = m6a_pos - prev_pos
+        # m6a is far apart or there is only a few m6a here
+        if cur_m6a_count <= max_m6a_in_nuc and dist >= min_nuc_size:
+            starts.append(prev_pos + 1)
+            sizes.append(dist - 1)
+            cur_m6a_count = 0
+            prev_pos = m6a_pos
+        ## if we get to the max m6a count then try staring a new nucleosome at this m6a
+        elif cur_m6a_count >= max_m6a_in_nuc:
+            prev_pos = m6a_pos
+            cur_m6a_count = 0
+        # we are still have few enough m6a marks to be a nuc, but not long enough yet
+        else:
+            cur_m6a_count += 1
+    return np.array(starts), np.array(sizes)
+
+
 def simpleFind(methylated_positions, binary, cutoff):
     """Using an array of methylated positions
     calculate the spacing between each methylation.
-    If the distance between two methylations > 85 then
+    If the distance between two methylations > "cutoff" then
     that is a nucleosome call. Otherwise continue."""
 
     dif = np.subtract(methylated_positions[1:], methylated_positions[:-1], dtype=D_TYPE)
     # difference between adjacent methylations
 
     index = np.argwhere(dif >= cutoff).reshape(-1)
     # indices where difference is equal or greater than 85bp
@@ -455,60 +557,67 @@
         ).astype(int)
         all_simple_sizes = np.concatenate([simple_nuc_sizes, custom_nuc_sizes]).astype(
             int
         )
 
         sort_order = np.argsort(all_simple_starts)
 
+        nuc_starts = all_simple_starts[sort_order]
+        nuc_sizes = all_simple_sizes[sort_order]
+
+        if not np.all(nuc_sizes >= 0):
+            logging.debug(f"Negative nucleosome size detected: {nuc_sizes}")
+
+        correct_sizes = nuc_starts[:-1] + nuc_sizes[:-1] <= nuc_starts[1:]
+        if not np.all(correct_sizes):
+            logging.debug(f"Simple methods made invalid ranges.")
+
         return (
             all_simple_starts[sort_order],
             all_simple_sizes[sort_order],
             terminal_nuc_generated,
         )
 
     else:
-
         return simple_nuc_starts, simple_nuc_sizes, False
 
 
-def rle(inarray):
-    """run length encoding. Partial credit to R rle function.
-    Multi datatype arrays catered for including non Numpy
-    returns: tuple (runlengths, startpositions, values)
-    https://stackoverflow.com/questions/1066758/
-    find-length-of-sequences-of-identical-values-in-a-numpy-array-run-length-encodi
-    """
-    ia = np.asarray(inarray, dtype=D_TYPE)  # force numpy
-    n = len(ia)
-    y = ia[1:] != ia[:-1]  # pairwise unequal (string safe)
-    i = np.append(np.where(y), n - 1)  # must include last element posi
-    z = np.diff(np.append(-1, i))  # run lengths
-    p = np.cumsum(np.append(0, z))[:-1]  # positions
-    return (z, p, ia[i])
-
-
 def add_nucleosomes(args):
     bam = pysam.AlignmentFile(args.input, threads=args.threads, check_sq=False)
     if args.model is None:
         logging.info("Training HMM for nucleosome calling")
         training_set = []
-        for idx, rec in enumerate(bam.fetch(until_eof=True)):
-            mods, _AT_pos, _m6a_pos = get_mods_from_rec(rec, mask=True)
-            if mods is None:
+        for rec in bam.fetch(until_eof=True):
+            mods, _AT_pos, m6a_pos = get_mods_from_rec(
+                rec, mask=True, ml_cutoff=args.ml_cutoff
+            )
+            if mods is None or m6a_pos.shape[0] < args.min_m6a_calls:
                 continue
             training_set.append(mods)
-            if idx >= args.num_train:
+            if len(training_set) >= args.num_train:
                 break
         model = train_hmm(training_set, n_jobs=args.threads)
         json_model = model.to_json()
 
         out = sys.stdout if args.out == "-" else open(args.out, "w")
         with out as handle:
             handle.write(json_model)
     else:
         logging.info("Applying HMM for nucleosome calling")
-        out = pysam.AlignmentFile(args.out, "wb", template=bam)
+        out = pysam.AlignmentFile(args.out, "wb", template=bam, threads=args.threads)
         hmm = pom.HiddenMarkovModel().from_json(args.model)
         _actuated_label, nucleated_label = assign_states(hmm)
-        apply_hmm(bam, hmm, nucleated_label, args.cutoff, out, min_dist=args.min_dist)
+        logging.warning(f"Min nucleosome size is {args.nuc_size_cutoff}")
+        apply_hmm(
+            bam,
+            hmm,
+            nucleated_label,
+            args.cutoff,
+            args.nuc_size_cutoff,
+            out,
+            min_dist=args.min_dist,
+            ml_cutoff=args.ml_cutoff,
+            simple_only=args.simple_only,
+            hmm_only=args.hmm_only,
+        )
 
     return 0
```

### Comparing `fibertools-0.2.9/fibertools/classify.py` & `fibertools-0.3.0/fibertools/classify.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,21 +2,31 @@
 """
 from numba import njit
 import numpy as np
 import mokapot
 import logging
 from xgboost import XGBClassifier
 from sklearn.model_selection import GridSearchCV
+import matplotlib.pyplot as plt
 
 
 @njit
 def get_msp_mid(st, msp_st, msp_size):
     return st + msp_st + msp_size // 2
 
 
+def m6a_fc_over_expected(m6a_count, AT_count, expected_frac_m6a, log=True):
+    expected = expected_frac_m6a * AT_count
+    observed = m6a_count
+    fc = np.nan_to_num(observed / expected, nan=1.0)
+    if log:
+        return np.log2(fc)
+    return fc
+
+
 @njit
 def get_bin_AT(bin_starts, is_at, bin_width=40):
     """_summary_
     Args:
         bin_starts (_type_): start sites of bins
         is_at (bool): array of AT sites
         bin_width (int, optional):  Defaults to 40.
@@ -134,29 +144,39 @@
         verbose=2,
     )
     mod = mokapot.Model(xgb_mod, train_fdr=train_fdr, subset_max_train=subset_max_train)
     mokapot_conf, models = mokapot.brew(train_psms, mod, test_fdr=test_fdr)
     return (mokapot_conf, models)
 
 
+def plot_classifier(mokapot_conf, out):
+    _fig, ax = plt.subplots(1, 1, figsize=(6, 4))
+    colors = ("#343131", "#24B8A0")
+    # Plot the performance:
+    mokapot_conf.plot_qvalues(c=colors[1], ax=ax, label="mokapot")
+    ax.legend(frameon=False)
+    plt.tight_layout()
+    plt.savefig(f"{out}.pdf")
+
+
 def assign_classifier_fdr(pin_data, models, mokapot_conf):
     psms = mokapot.read_pin(pin_data)
     all_scores = [model.predict(pin_data) for model in models]
     scores = np.mean(np.array(all_scores), axis=0)
     # scores = np.amin(np.array(all_scores), axis=0)
     # scores = np.amax(np.array(all_scores), axis=0)
 
     q_values = find_nearest_q_values(
         mokapot_conf.psms["mokapot score"], mokapot_conf.psms["mokapot q-value"], scores
     )
     return q_values
 
 
 def make_accessibility_model(
-    pin, train_fdr=0.10, test_fdr=0.05, subset_max_train=2_000_000
+    pin, train_fdr=0.10, test_fdr=0.05, subset_max_train=2_000_000, out_file=None
 ):
     logging.debug(f"dataset size: {pin.shape}")
     logging.debug(f"dataset label counts: {pin.Label.value_counts()}")
     train = pin[(pin.Label != 0)].copy()
     logging.debug(f"train size: {train.shape}")
     min_size = 1
 
@@ -172,10 +192,16 @@
     xgb_mod = GridSearchCV(
         XGBClassifier(use_label_encoder=False, eval_metric="auc"),
         param_grid=grid,
         cv=3,
         scoring="roc_auc",
         verbose=2,
     )
-    mod = mokapot.Model(xgb_mod, train_fdr=train_fdr, subset_max_train=subset_max_train)
+    mod = mokapot.Model(
+        xgb_mod,
+        train_fdr=train_fdr,
+        subset_max_train=subset_max_train,
+        direction="msp_fc",
+    )
     moka_conf, models = mokapot.brew(train_psms, mod, test_fdr=test_fdr)
+    plot_classifier(moka_conf, out_file)
     return (moka_conf, models)
```

### Comparing `fibertools-0.2.9/fibertools/cli.py` & `fibertools-0.3.0/fibertools/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,21 +3,22 @@
 import argparse
 from cgi import test
 from email.policy import default
 import sys
 import logging
 from typing_extensions import Required
 from fibertools.readutils import read_in_bed_file
-from fibertools.trackhub import generate_trackhub
+from fibertools.trackhub import generate_trackhub, make_bins
 from fibertools.unionbg import bed2d4, make_q_values
 from fibertools.add_nucleosomes import add_nucleosomes
 import fibertools as ft
 import numpy as np
 import gzip
 import pandas as pd
+import polars as pl
 
 
 def make_bam2bed_parser(subparsers):
     parser = subparsers.add_parser(
         "bam2bed",
         help="Extract m6a calls from bam and output bed12.",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
@@ -73,15 +74,40 @@
         "-d",
         "--min-dist",
         help="Minimum distance from the start or end of a fiber for a accessible or nucelosome call.",
         type=int,
         default=46,
     )
     parser.add_argument(
-        "-c", "--cutoff", type=int, default=65, help="hmm nucleosome size cutoff"
+        "--ml-cutoff",
+        type=int,
+        default=200,
+        help="Min value in the ML tag to consider basemod for HMM.",
+    )
+    parser.add_argument(
+        "--min-m6a-calls",
+        type=int,
+        default=200,
+        help="Minimum number of m6A calls in a fiber to use a fiber for training the HMM.",
+    )
+    parser.add_argument(
+        "-c", "--cutoff", type=int, default=65, help="Internal nucleosome size cutoff"
+    )
+    parser.add_argument(
+        "--nuc-size-cutoff", type=int, default=85, help="Final nucleosome size cutoff"
+    )
+    parser.add_argument(
+        "--simple-only",
+        help="Use only the simple model for nucleosome calling.",
+        action="store_true",
+    )
+    parser.add_argument(
+        "--hmm-only",
+        help="Use only the HMM for nucleosome calling.",
+        action="store_true",
     )
 
 
 def make_bed_split_parser(subparsers):
     parser = subparsers.add_parser(
         "split",
         help="Split a bed over many output files.",
@@ -101,28 +127,71 @@
 
 def make_trackhub_parser(subparsers):
     parser = subparsers.add_parser(
         "trackhub",
         help="Make a trackhub from a bed file.",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
-    parser.add_argument("bed", help="A bed file")
     parser.add_argument(
         "genome_file", help="A file with chromosome sizes for the genome."
     )
     parser.add_argument("-r", "--ref", default="hg38")
+    parser.add_argument(
+        "--sample", default="Sample", help="Sample name to add to the trackhub."
+    )
     parser.add_argument("-t", "--trackhub-dir", default="trackHub")
     parser.add_argument("--bw", nargs="+", help="bw files to include", default=None)
     parser.add_argument(
+        "--max-bins",
+        help="Max number of dijoint bins to plot.",
+        type=int,
+        default=75,
+    )
+    parser.add_argument(
+        "-c",
+        "--average-coverage",
+        help="bam coverage.",
+        type=float,
+        default=60.0,
+    )
+    parser.add_argument(
+        "-n",
+        "--n-rows",
+        help="For debugging only reads in n rows.",
+        type=int,
+        default=None,
+    )
+
+
+def make_bin_parser(subparsers):
+    parser = subparsers.add_parser(
+        "bin",
+        help="Make a binned version of the bed file (add an extra column).",
+        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
+    )
+    parser.add_argument("bed", help="A bed file")
+    parser.add_argument(
+        "--outs",
+        "-o",
+        help="Output bed files",
+        nargs="+",
+    )
+    parser.add_argument(
         "--spacer-size",
         help="adjust minimum distance between fibers for them to be in the same bin.",
         type=int,
         default=100,
     )
     parser.add_argument(
+        "--max-bins",
+        help="Max number of dijoint bins to plot.",
+        type=int,
+        default=75,
+    )
+    parser.add_argument(
         "-n",
         "--n-rows",
         help="For debugging only reads in n rows.",
         type=int,
         default=None,
     )
 
@@ -149,14 +218,19 @@
     )
     parser.add_argument(
         "-c",
         "--column",
         help="Name of the column to split the bed file on to make bed graphs.",
         default="name",
     )
+    parser.add_argument(
+        "--chromosome",
+        help="Only do this chromosome.",
+        default=None,
+    )
 
 
 def make_accessibility_model_parser(subparsers):
     parser = subparsers.add_parser(
         "model",
         help="Make MSP features",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
@@ -181,17 +255,17 @@
         "--bin-num",
         help="Number of feature bins to work. Must be an odd number.",
         type=int,
         default=9,
     )
     parser.add_argument(
         "--min-tp-msp-len",
-        help="min msp length to be in the DHS positive training set.",
+        help="Minimum MSP length to be in the DHS positive training set for Mokapot.",
         type=int,
-        default=40,
+        default=85,
     )
     parser.add_argument(
         "--spacer-size",
         help="adjust minimum distance between fibers for them to be in the same bin.",
         type=int,
         default=100,
     )
@@ -202,14 +276,20 @@
         "--test-fdr", help="Testing FDR used by mokapot.", type=float, default=0.05
     )
     parser.add_argument("-m", "--model", default=None)
     parser.add_argument(
         "-o", "--out", help="Write the accessibility model to this file."
     )
     parser.add_argument(
+        "--haps",
+        help="Write the three accessibility results these files per haplotype.",
+        nargs=3,
+        default=None,
+    )
+    parser.add_argument(
         "-n",
         "--n-rows",
         help="For debugging only reads in n rows.",
         type=int,
         default=None,
     )
 
@@ -284,14 +364,15 @@
     )
     make_bam2bed_parser(subparsers)
     make_add_m6a_parser(subparsers)
     make_add_nucleosome_parser(subparsers)
     make_accessibility_model_parser(subparsers)
     make_bed_split_parser(subparsers)
     make_trackhub_parser(subparsers)
+    make_bin_parser(subparsers)
     make_bed2d4_parser(subparsers)
     # shared arguments
     parser.add_argument("-t", "--threads", help="n threads to use", type=int, default=1)
     parser.add_argument(
         "-v", "--verbose", help="increase logging verbosity", action="store_true"
     )
     parser.add_argument(
@@ -317,16 +398,20 @@
         # check if we have data
         if fiberdata.all.shape[0] == 0:
             if args.model is None:
                 logging.warning("No MSPs found in training set.")
                 sys.exit(1)
             else:
                 logging.warning("No MSPs found in MSP bed file.")
-                with open(args.out, "w") as f:
-                    f.write("")
+                outs = [args.out]
+                if args.haps is not None:
+                    outs += args.haps
+                for out in outs:
+                    with open(out, "w") as f:
+                        f.write("")
                 sys.exit(0)
         fiberdata.make_msp_features(bin_num=args.bin_num, bin_width=args.bin_width)
         # else:
         # fiberdata = ft.Fiberdata(
         #     args.msp_bed12,
         #     args.m6a_bed12,
         #     n_rows=args.n_rows,
@@ -349,27 +434,45 @@
         else:
             logging.debug("Loading model from file and predicting.")
             logging.debug(
                 f"Max FDR allowed for an accessibility call: {args.train_fdr}"
             )
             fiberdata.predict_accessibility(args.model, max_fdr=args.train_fdr)
             fiberdata.accessibility.to_csv(args.out, sep="\t", index=False)
+            if args.haps is not None:
+                for o_hap_file, hap in zip(args.haps, ["H1", "H2", "UNK"]):
+                    hap_df = fiberdata.accessibility[fiberdata.accessibility.HP == hap]
+                    hap_df.to_csv(o_hap_file, sep="\t", index=False)
+
     elif args.command == "split":
         split_bed_over_files(args)
     elif args.command == "trackhub":
-        df = pd.read_csv(args.bed, sep="\t", nrows=args.n_rows)
         generate_trackhub(
-            df,
             trackhub_dir=args.trackhub_dir,
             ref=args.ref,
-            genome_file=args.genome_file,
-            spacer_size=args.spacer_size,
             bw=args.bw,
+            sample=args.sample,
+            max_bins=args.max_bins,
+            ave_coverage=args.average_coverage,
+        )
+    elif args.command == "bin":
+        logging.info("Reading bed.")
+        df = ft.utils.read_bed_with_header(args.bed, n_rows=args.n_rows)
+        logging.info("Done reading bed.")
+        if args.outs is None:
+            outs = [f"bin.{i}.bed" for i in range(args.n_bins)]
+        else:
+            outs = args.outs
+        make_bins(
+            df,
+            outs,
+            spacer_size=args.spacer_size,
         )
+        logging.info("done making bins")
     elif args.command == "bed2d4":
         if args.fdr:
             logging.debug("Making fdr peaks.")
-            make_q_values(args.bed, args.d4)
+            make_q_values(args.bed, args.d4, chromosome=args.chromosome)
         else:
             bed2d4(args)
 
     return 0
```

### Comparing `fibertools-0.2.9/fibertools/fiberdata.py` & `fibertools-0.3.0/fibertools/fiberdata.py`

 * *Files 14% similar despite different names*

```diff
@@ -30,58 +30,93 @@
             ft_all (str): Path to a `ft extract --all` table.
             n_rows (int, optional): Only read a subset of the data for testing. Defaults to None.
         """
         self.all = ft.read_fibertools_rs_all_file(all_file, n_rows=n_rows)
         logging.debug("Finished reading ft-extract --all table")
 
     def get_msp_features(self, row, bin_width=40, bin_num=5):
-        # is_at = AT_genome[row["ct"]][row["st"] : row["en"]]
+        # fiber_wide_features
         seq = np.frombuffer(bytes(row["fiber_sequence"], "utf-8"), dtype="S1")
         is_at = (seq == b"T") | (seq == b"A")
 
-        typed_bst_m6a = row["msp_starts"]
+        # typed_bst_m6a = row["msp_starts"]
+        typed_bst_m6a = row["m6a"]
         rtn = []
         mids = ft.classify.get_msp_mid(0, row["msp_starts"], row["msp_lengths"])
         all_bin_starts = ft.classify.make_bin_starts(
             mids, bin_width=bin_width, bin_num=bin_num
         )
         fiber_AT_count = is_at.sum()
         fiber_m6a_count = row["m6a"].shape[0]
+        fiber_frac_m6a = fiber_m6a_count / fiber_AT_count
 
+        # figure out average msp density
+        all_msp_m6a_count = 0.0
+        all_msp_AT_count = 0.0
+        all_msp_count = 0.0
+        for msp_st, msp_size in zip(row["msp_starts"], row["msp_lengths"]):
+            msp_en = msp_st + msp_size
+            if msp_en <= msp_st:
+                continue
+            all_msp_AT_count += is_at[msp_st:msp_en].sum()
+            all_msp_m6a_count += (
+                (typed_bst_m6a >= msp_st) & (typed_bst_m6a < msp_en)
+            ).sum()
+            all_msp_count += 1
+        all_msp_bp = row["msp_lengths"].sum()
+        all_frac_AT = all_msp_AT_count / all_msp_bp
+        expected_m6a_per_msp = np.nan_to_num(
+            all_msp_m6a_count / (all_msp_count * all_frac_AT), nan=1.0
+        )
+
+        # make the features
         for msp_st, msp_size, bin_starts, ref_msp_st, ref_msp_size in zip(
             row["msp_starts"],
             row["msp_lengths"],
             all_bin_starts,
             row["ref_msp_starts"],
             row["ref_msp_lengths"],
         ):
             msp_en = msp_st + msp_size
             if msp_en <= msp_st:
                 continue
             m6a_counts = ft.classify.get_bin_m6a(
                 bin_starts, typed_bst_m6a, bin_width=bin_width
             )
             AT_count = ft.classify.get_bin_AT(bin_starts, is_at, bin_width=bin_width)
+            m6a_fc = ft.classify.m6a_fc_over_expected(
+                m6a_counts, AT_count, fiber_frac_m6a
+            )
+            # msp features
             msp_AT = is_at[msp_st:msp_en].sum()
             msp_m6a = ((typed_bst_m6a >= msp_st) & (typed_bst_m6a < msp_en)).sum()
+            msp_fc = np.log2(
+                np.nan_to_num(
+                    msp_m6a / (msp_AT / msp_size) * 1.0 / expected_m6a_per_msp,
+                    nan=1.0,
+                )
+            )
             rtn.append(
                 {
                     "ct": row["ct"],
                     "st": ref_msp_st,
                     "en": ref_msp_st + ref_msp_size,
                     "fiber": row["fiber"],
                     "score": row["score"],
+                    "HP": row["HP"],
                     "msp_len": msp_size,
                     "fiber_m6a_count": fiber_m6a_count,
                     "fiber_AT_count": fiber_AT_count,
-                    "fiber_m6a_frac": fiber_m6a_count / fiber_AT_count,
+                    "fiber_m6a_frac": fiber_frac_m6a,
                     "msp_m6a": msp_m6a,
                     "msp_AT": msp_AT,
+                    "msp_fc": msp_fc,
                     "m6a_count": m6a_counts,
                     "AT_count": AT_count,
+                    "m6a_fc": m6a_fc,
                 }
             )
         return rtn
 
     def make_msp_features(self, bin_width=40, bin_num=9):
         msp_stuff = []
         rows = self.all.to_dicts()
@@ -114,47 +149,55 @@
             z["m6a_count"].tolist(),
             columns=[f"m6a_count_{i}" for i in range(bin_num)],
         )
         AT_counts = pd.DataFrame(
             z["AT_count"].tolist(),
             columns=[f"AT_count_{i}" for i in range(bin_num)],
         )
+        m6a_fold_changes = pd.DataFrame(
+            z["m6a_fc"].tolist(),
+            columns=[f"m6a_fc_{i}" for i in range(bin_num)],
+        )
+        # for x in [m6a_fold_changes, z["msp_fc"]]:
+        #    logging.debug(f"\n{x}")
         out = (
-            pd.concat([z, m6a_fracs, m6a_counts, AT_counts], axis=1)
-            .drop(["bin_m6a_frac", "m6a_count", "AT_count"], axis=1)
+            pd.concat([z, m6a_fracs, m6a_counts, AT_counts, m6a_fold_changes], axis=1)
+            .drop(["bin_m6a_frac", "m6a_count", "AT_count", "m6a_fc"], axis=1)
             .replace([np.inf, -np.inf], np.nan)
             .fillna(0)
         )
+        logging.debug("Finished expanding bed12s into individual MSPs.")
+        logging.debug(f"\n{out}")
+        t = out.msp_fc.describe()
+        logging.debug(f"\n{t}")
         self.features = out
 
-    def make_percolator_input(self, dhs_df=None, sort=False, min_tp_msp_len=40):
+    def make_percolator_input(self, dhs_df=None, sort=False, min_tp_msp_len=85):
         """write a input file that works with percolator.
 
         Args:
             msp_features_df (_type_): _description_
             out_file (_type_): _description_
 
         return None
         """
         # need to add the following columns: SpecId	Label Peptide Proteins
         # and need to remove the following columns:
-        to_remove = ["ct", "st", "en", "fiber"]
+        to_remove = ["ct", "st", "en", "fiber", "HP"]
 
         out_df = self.features.copy()
         out_df.insert(1, "Label", 0)
         if dhs_df is not None:
             dhs_null = ft.utils.n_overlaps(self.features, dhs_df[dhs_df.name != "DHS"])
             dhs_true = ft.utils.n_overlaps(self.features, dhs_df[dhs_df.name == "DHS"])
             out_df.loc[dhs_true > 0, "Label"] = 1
             out_df.loc[dhs_null > 0, "Label"] = -1
 
-            # if the msp is short make it null
-            out_df.loc[
-                (dhs_true > 0) & (out_df.msp_len <= min_tp_msp_len), "Label"
-            ] = -1
+            # if the msp is short make it a non informative label
+            out_df.loc[(dhs_true > 0) & (out_df.msp_len <= min_tp_msp_len), "Label"] = 0
         else:
             # has no effect, percolator just needs some items to have positive labels
             out_df.loc[out_df.msp_len >= min_tp_msp_len, "Label"] = 1
 
         # add and drop columns needed for mokapot
         out_df.drop(to_remove, axis=1, inplace=True)
         if "SpecId" in out_df.columns:
@@ -170,38 +213,40 @@
         self.pin = out_df
 
     def train_accessibility_model(self, out_file: str, train_fdr=0.1, test_fdr=0.05):
         logging.debug(
             f"Using {train_fdr} fdr for training and {test_fdr} fdr for testing."
         )
         moka_conf, models = ft.classify.make_accessibility_model(
-            self.pin, train_fdr=train_fdr, test_fdr=test_fdr
+            self.pin, train_fdr=train_fdr, test_fdr=test_fdr, out_file=out_file
         )
         with open(out_file, "wb") as f:
             pickle.dump(moka_conf.psms, f)
             pickle.dump(models, f)
 
     def make_nucleosome_accessibility_df(self):
         df = pd.DataFrame(
-            self.all[["ct", "fiber", "ref_nuc_starts", "ref_nuc_lengths"]].to_dicts()
+            self.all[
+                ["ct", "fiber", "HP", "ref_nuc_starts", "ref_nuc_lengths"]
+            ].to_dicts()
         )
         logging.debug(f"Expanding into individual nucleosomes. {df.shape[0]}")
         df = df.explode(["ref_nuc_starts", "ref_nuc_lengths"])
         df["st"] = df.ref_nuc_starts
         df["en"] = df.ref_nuc_starts + df.ref_nuc_lengths
         df["score"] = 1
         df["strand"] = "+"
         df["tst"] = df["st"]
-        df["ten"] = df["en"]
+        df["ten"] = df["st"]
         df["color"] = "230,230,230"
         df["qValue"] = 1
         logging.debug(f"Finished expanding into individual nucleosomes. {df.shape[0]}")
         return df
 
-    def predict_accessibility(self, model_file: str, max_fdr=0.30):
+    def predict_accessibility(self, model_file: str, max_fdr=0.10):
         moka_conf_psms, models = list(ft.utils.load_all(model_file))
 
         test_psms = mokapot.read_pin(self.pin)
         all_scores = [model.predict(test_psms) for model in models]
         # scores = np.mean(np.array(all_scores), axis=0)
         # scores = np.amin(np.array(all_scores), axis=0)
         scores = np.amax(np.array(all_scores), axis=0)
@@ -225,25 +270,27 @@
         out.loc[out.qValue >= max_fdr, "qValue"] = 1
 
         # out.loc[out.qValue <= 0.10, "color"] = "255,255,0"
         out.loc[out.qValue <= 0.10, "color"] = "255,140,0"
         out.loc[out.qValue <= 0.05, "color"] = "255,0,0"
         out.loc[out.qValue <= 0.01, "color"] = "139,0,0"
 
+        logging.debug(f"Writing accessibility\n{out.head(5)}")
         out_cols = [
             "ct",
             "st",
             "en",
             "fiber",
             "score",
             "strand",
             "tst",
             "ten",
             "color",
             "qValue",
+            "HP",
             # "bin",
         ]
         final_out = (
             pd.concat(
                 [out[out_cols], self.make_nucleosome_accessibility_df()[out_cols]]
             )
             .sort_values(["ct", "st"])
```

### Comparing `fibertools-0.2.9/fibertools/readutils.py` & `fibertools-0.3.0/fibertools/readutils.py`

 * *Files identical despite different names*

### Comparing `fibertools-0.2.9/fibertools/unionbg.py` & `fibertools-0.3.0/fibertools/unionbg.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import pyd4
 import tempfile
-from joblib import Parallel
 import numpy as np
 from numba import njit
 import logging
 import fibertools as ft
 import polars as pl
 import sys
+import os
 
 
 @njit
 def chrom_bg(sts, ens, chrom_len):
     chrom = np.zeros(chrom_len, dtype=np.int32)
     to_add = np.int32(1)
     for st, en in zip(sts, ens):
@@ -51,15 +51,15 @@
     for idx, g in enumerate(df.groupby([group_col])):
         g_n = g[group_col][0]
         logging.debug(f"Making d4 for group: {g_n}")
         out_files.append((g_n, make_temp_d4_from_df(g, genome)))
 
     merged = pyd4.D4Merger(d4_f)
     for tag, d4 in sorted(out_files):
-        logging.debug(f"{tag} sum: {pyd4.D4File(d4.name)['chr11'].sum()}")
+        # logging.debug(f"{tag} sum: {pyd4.D4File(d4.name)[tag].sum()}")
         merged.add_tagged_track("q_" + str(tag), d4.name)
     merged.merge()
     # close files
     [d4.close() for _tag, d4 in out_files]
 
 
 def bed2d4(args):
@@ -79,30 +79,37 @@
             .otherwise(pl.col("column_5"))
             .alias(args.column)
         )
     genome = {line.split()[0]: int(line.split()[1]) for line in open(args.genome)}
     make_union_d4_from_df(df, genome, args.column, args.d4)
 
 
-@njit(parallel=True)
-def make_summary_stats(matrix, log_q_values=None, adjust_for_coverage=True):
+# @njit(parallel=True)
+def make_summary_stats(matrix, log_q_values=None):
     y = matrix.T
     log_q_vals = (y[:, :-2] * log_q_values).sum(axis=1)
     acc_cov = y[:, :-2].sum(axis=1)
     link_cov = y[:, -2]
     nuc_cov = y[:, -1]
     cov = acc_cov + link_cov + nuc_cov
     # adjust for expected amount of coverage
-    if adjust_for_coverage:
-        log_q_vals = log_q_vals - cov / 10 * (-10 * np.log10(0.1))
+    if True:
+        average_log_q_value = np.nanmean(log_q_vals / cov)
+        if np.isnan(average_log_q_value):
+            average_log_q_value = 0
+        print("Average log q value:")
+        print(average_log_q_value)
+        print("")
+        log_q_vals = log_q_vals - cov * average_log_q_value
     # assert nuc_cov.sum() == link_cov.sum()
     return (log_q_vals, acc_cov, link_cov, nuc_cov)
 
 
-def make_q_values(in_d4, out_d4):
+def make_q_values(in_d4, out_d4, chromosome=None):
+    logging.info(f"Reading in d4 file: {in_d4}")
     file = pyd4.D4File(in_d4)
     chroms = file.chroms()
     matrix = file.open_all_tracks()
     track_names = matrix.track_names
     # these are the q values
     q_values = np.array([max(int(x.strip("q_")) / 100, 0.01) for x in track_names])
     log_q_values = -10 * np.log10(q_values[:-2])
@@ -122,25 +129,34 @@
             .for_sparse_data()
             .generate_index()
             .get_writer()
         )
         out_temp_files.append((temp, w))
 
     for ct, ct_len in chroms:
+        if chromosome is not None and ct != chromosome:
+            logging.debug(f"Skipping {ct} due to cli argument")
+            continue
         logging.debug(f"Processing q-values for chrom: {ct}")
         bin_size = 5_000_000
         cur_st = 0
         cur_en = bin_size
         while True:  # cur_en < ct_len and cur_st < ct_len:
             if cur_en > ct_len:
                 cur_en = ct_len
-
+            if cur_en <= cur_st:
+                break
+            logging.info(f"Processing {ct} {cur_st} {cur_en}")
+            logging.info(os.path.exists(in_d4))
             cur_mat = matrix[ct, cur_st, cur_en]
             idx = 0
-            for data in make_summary_stats(cur_mat, log_q_values=log_q_values):
+            for data in make_summary_stats(
+                cur_mat,
+                log_q_values=log_q_values,
+            ):
                 logging.debug(
                     f"Writing {ct} {cur_st} {cur_en} with index {idx} to d4. Mean is {data.mean()}"
                 )
                 w = out_temp_files[idx][1]
                 w.write_np_array(ct, cur_st, data)
                 idx += 1
```

### Comparing `fibertools-0.2.9/fibertools/utils.py` & `fibertools-0.3.0/fibertools/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,19 +2,29 @@
 import pandas as pd
 import polars as pl
 import numpy as np
 import logging
 import fibertools as ft
 import pyranges as pr
 import pickle
+import io
+import sys
 
 numba_logger = logging.getLogger("numba")
 numba_logger.setLevel(logging.WARNING)
 
 
+def read_bed_with_header(bed, n_rows=None):
+    input = bed
+    if bed == "-":
+        input = io.StringIO(sys.stdin.read())
+    df = pl.read_csv(input, sep="\t", stop_after_n_rows=n_rows, comment_char="$")
+    return df
+
+
 def split_to_ints(df, col, sep=",", trim=True):
     """Split a columns with list of ints separated by
     "sep" into a numpy array quickly.
 
     Args:
         df (dataframe): dataframe that is like a bed12 file.
         col (str): column name within the dataframe to split up.
```

### Comparing `fibertools-0.2.9/fibertools.egg-info/SOURCES.txt` & `fibertools-0.3.0/fibertools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fibertools-0.2.9/setup.py` & `fibertools-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,10 +67,10 @@
     include_package_data=True,
     keywords="fibertools",
     name="fibertools",
     packages=find_packages(include=["fibertools", "fibertools.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/mrvollger/fibertools",
-    version="0.2.9",
+    version="0.3.0",
     zip_safe=False,
 )
```

### Comparing `fibertools-0.2.9/tests/all.tbl.gz` & `fibertools-0.3.0/tests/all.tbl.gz`

 * *Files identical despite different names*

