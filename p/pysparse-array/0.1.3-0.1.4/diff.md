# Comparing `tmp/pysparse-array-0.1.3.tar.gz` & `tmp/pysparse-array-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysparse-array-0.1.3.tar", last modified: Tue May 16 11:49:38 2023, max compression
+gzip compressed data, was "pysparse-array-0.1.4.tar", last modified: Tue May 16 17:50:44 2023, max compression
```

## Comparing `pysparse-array-0.1.3.tar` & `pysparse-array-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 thomasfrost   (502) staff       (20)        0 2023-05-16 11:49:38.673487 pysparse-array-0.1.3/
--rw-r--r--   0 thomasfrost   (502) staff       (20)      834 2023-05-16 11:39:55.000000 pysparse-array-0.1.3/HISTORY.md
--rw-r--r--   0 thomasfrost   (502) staff       (20)     1060 2023-05-15 14:53:09.000000 pysparse-array-0.1.3/LICENSE.txt
--rw-r--r--   0 thomasfrost   (502) staff       (20)       19 2023-05-16 11:11:47.000000 pysparse-array-0.1.3/MANIFEST.in
--rw-r--r--   0 thomasfrost   (502) staff       (20)     2289 2023-05-16 11:49:38.667941 pysparse-array-0.1.3/PKG-INFO
--rw-r--r--   0 thomasfrost   (502) staff       (20)     1584 2023-05-15 17:35:02.000000 pysparse-array-0.1.3/README.md
--rw-r--r--   0 thomasfrost   (502) staff       (20)      779 2023-05-15 22:23:50.000000 pysparse-array-0.1.3/pyproject.toml
-drwxr-xr-x   0 thomasfrost   (502) staff       (20)        0 2023-05-16 11:49:38.626472 pysparse-array-0.1.3/pysparse_array.egg-info/
--rw-r--r--   0 thomasfrost   (502) staff       (20)     2289 2023-05-16 11:49:38.000000 pysparse-array-0.1.3/pysparse_array.egg-info/PKG-INFO
--rw-r--r--   0 thomasfrost   (502) staff       (20)      311 2023-05-16 11:49:38.000000 pysparse-array-0.1.3/pysparse_array.egg-info/SOURCES.txt
--rw-r--r--   0 thomasfrost   (502) staff       (20)        1 2023-05-16 11:49:38.000000 pysparse-array-0.1.3/pysparse_array.egg-info/dependency_links.txt
--rw-r--r--   0 thomasfrost   (502) staff       (20)       47 2023-05-16 11:49:38.000000 pysparse-array-0.1.3/pysparse_array.egg-info/requires.txt
--rw-r--r--   0 thomasfrost   (502) staff       (20)        7 2023-05-16 11:49:38.000000 pysparse-array-0.1.3/pysparse_array.egg-info/top_level.txt
--rw-r--r--   0 thomasfrost   (502) staff       (20)       38 2023-05-16 11:49:38.674045 pysparse-array-0.1.3/setup.cfg
--rw-r--r--   0 thomasfrost   (502) staff       (20)      708 2023-05-16 11:12:23.000000 pysparse-array-0.1.3/setup.py
-drwxr-xr-x   0 thomasfrost   (502) staff       (20)        0 2023-05-16 11:49:38.662705 pysparse-array-0.1.3/sparse/
--rw-r--r--   0 thomasfrost   (502) staff       (20)      113 2023-05-16 11:47:08.000000 pysparse-array-0.1.3/sparse/__init__.py
--rw-r--r--   0 thomasfrost   (502) staff       (20)     8471 2023-05-16 11:46:30.000000 pysparse-array-0.1.3/sparse/array_api.py
--rw-r--r--   0 thomasfrost   (502) staff       (20)     6846 2023-05-16 11:46:59.000000 pysparse-array-0.1.3/sparse/core.py
+drwxr-xr-x   0 thomasfrost   (502) staff       (20)        0 2023-05-16 17:50:44.864418 pysparse-array-0.1.4/
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     1497 2023-05-16 17:50:07.000000 pysparse-array-0.1.4/HISTORY.md
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     1060 2023-05-15 14:53:09.000000 pysparse-array-0.1.4/LICENSE.txt
+-rw-r--r--   0 thomasfrost   (502) staff       (20)       19 2023-05-16 11:11:47.000000 pysparse-array-0.1.4/MANIFEST.in
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     2289 2023-05-16 17:50:44.846358 pysparse-array-0.1.4/PKG-INFO
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     1584 2023-05-15 17:35:02.000000 pysparse-array-0.1.4/README.md
+-rw-r--r--   0 thomasfrost   (502) staff       (20)      779 2023-05-16 15:01:18.000000 pysparse-array-0.1.4/pyproject.toml
+drwxr-xr-x   0 thomasfrost   (502) staff       (20)        0 2023-05-16 17:50:44.777049 pysparse-array-0.1.4/pysparse_array.egg-info/
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     2289 2023-05-16 17:50:44.000000 pysparse-array-0.1.4/pysparse_array.egg-info/PKG-INFO
+-rw-r--r--   0 thomasfrost   (502) staff       (20)      311 2023-05-16 17:50:44.000000 pysparse-array-0.1.4/pysparse_array.egg-info/SOURCES.txt
+-rw-r--r--   0 thomasfrost   (502) staff       (20)        1 2023-05-16 17:50:44.000000 pysparse-array-0.1.4/pysparse_array.egg-info/dependency_links.txt
+-rw-r--r--   0 thomasfrost   (502) staff       (20)       47 2023-05-16 17:50:44.000000 pysparse-array-0.1.4/pysparse_array.egg-info/requires.txt
+-rw-r--r--   0 thomasfrost   (502) staff       (20)        7 2023-05-16 17:50:44.000000 pysparse-array-0.1.4/pysparse_array.egg-info/top_level.txt
+-rw-r--r--   0 thomasfrost   (502) staff       (20)       38 2023-05-16 17:50:44.864812 pysparse-array-0.1.4/setup.cfg
+-rw-r--r--   0 thomasfrost   (502) staff       (20)      708 2023-05-16 15:01:08.000000 pysparse-array-0.1.4/setup.py
+drwxr-xr-x   0 thomasfrost   (502) staff       (20)        0 2023-05-16 17:50:44.841362 pysparse-array-0.1.4/sparse/
+-rw-r--r--   0 thomasfrost   (502) staff       (20)      113 2023-05-16 11:47:08.000000 pysparse-array-0.1.4/sparse/__init__.py
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     9291 2023-05-16 17:35:44.000000 pysparse-array-0.1.4/sparse/array_api.py
+-rw-r--r--   0 thomasfrost   (502) staff       (20)     6821 2023-05-16 12:54:50.000000 pysparse-array-0.1.4/sparse/core.py
```

### Comparing `pysparse-array-0.1.3/LICENSE.txt` & `pysparse-array-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pysparse-array-0.1.3/PKG-INFO` & `pysparse-array-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysparse-array
-Version: 0.1.3
+Version: 0.1.4
 Summary: A package that enables on-the-fly encoding and decoding of large NumPy arrays as Sparse binaries.
 Home-page: https://github.com/tdgfrost/PySparse
 Download-URL: https://pypi.org/project/pysparse-array/
 Author: Thomas Frost
 Author-email: Thomas Frost <tdgfrost@gmail.com>
 Project-URL: Homepage, https://github.com/tdgfrost/PySparse
 Project-URL: Bug Tracker, https://github.com/tdgfrost/PySparse/issues
```

### Comparing `pysparse-array-0.1.3/README.md` & `pysparse-array-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pysparse-array-0.1.3/pyproject.toml` & `pysparse-array-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "pysparse-array"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
 	{ name="Thomas Frost", email="tdgfrost@gmail.com" },
 ]
 description = "A package that enables on-the-fly encoding and decoding of large NumPy arrays as Sparse binaries."
 readme = "README.md"
 requires-python = ">=3.8.0"
 classifiers = [
```

### Comparing `pysparse-array-0.1.3/pysparse_array.egg-info/PKG-INFO` & `pysparse-array-0.1.4/pysparse_array.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysparse-array
-Version: 0.1.3
+Version: 0.1.4
 Summary: A package that enables on-the-fly encoding and decoding of large NumPy arrays as Sparse binaries.
 Home-page: https://github.com/tdgfrost/PySparse
 Download-URL: https://pypi.org/project/pysparse-array/
 Author: Thomas Frost
 Author-email: Thomas Frost <tdgfrost@gmail.com>
 Project-URL: Homepage, https://github.com/tdgfrost/PySparse
 Project-URL: Bug Tracker, https://github.com/tdgfrost/PySparse/issues
```

### Comparing `pysparse-array-0.1.3/setup.py` & `pysparse-array-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme_file.read()
 
 with open('HISTORY.md') as history_file:
     HISTORY = history_file.read()
 
 setup_args = dict(
     name='pysparse-array',
-    version='0.1.3',
+    version='0.1.4',
     description='Package to encode and decode large OOM numpy arrays as Sparse binaries',
     long_description_content_type="text/markdown",
     long_description=README + '\n\n' + HISTORY,
     packages=find_packages(),
     author='Thomas Frost',
     author_email='tdgfrost@gmail.com',
     url='https://github.com/tdgfrost/PySparse',
```

### Comparing `pysparse-array-0.1.3/sparse/array_api.py` & `pysparse-array-0.1.4/sparse/array_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,43 @@
 import numpy as np
 from numba import njit, types
 from .core import find_indices
+import os
 
 
-def load_sparse(data_path: str, coords_path: str, shape: str or tuple, mode='r'):
+def load_sparse(data_path: str, coords_path='', shape='', mode='r'):
     """
     Load a (memory-mapped) sparse array from disk
-    :param data_path: path to sparse data array
+    :param data_path: path to sparse data array OR parent directory containing 'sparse_data.npy', 'sparse_coords.npy', and 'dense_shape.npy' arrays
     :param coords_path: path to sparse coordinates array
     :param shape: shape of the dense array, as either tuple or path to numpy array containing shape
     :param mode: mode to open the sparse arrays in (e.g., read-only, read-write, etc.) - r/r+/w
     :return: SparseArray object
     """
+    if os.path.isdir(data_path):
+        coords_path = os.path.join(data_path, 'sparse_coords.npy')
+        shape = os.path.join(data_path, 'dense_shape.npy')
+        data_path = os.path.join(data_path, 'sparse_data.npy')
+
     return SparseArray(data_path, coords_path, shape, mode)
 
 
 class SparseArray:
     def __init__(self, data_path: str, coords_path: str, shape: str or tuple, mode='r'):
         self.data = np.load(data_path, mmap_mode=mode)
+        self.data_dtype = self.data.dtype
+
         self.coords = np.load(coords_path, mmap_mode=mode)
+        self.coords_shape = self.coords.shape
 
         if shape is tuple:
             self.dense_shape = shape
         else:
             self.dense_shape = tuple(np.load(shape))
 
-        self.coords_shape = self.coords.shape
-
     def __getitem__(self, items):
         """"
         Get the values of the dense array at the given indices
         """
         if isinstance(items, int):
             return self.__get_row(items)
 
@@ -113,15 +120,23 @@
         find_coords, coords_present = search_function[type(row_idx)](self.coords, row_idx,
                                                                      maxlen=self.coords_shape[0])
 
         # Assuming the row indices have non-zero data...
         if coords_present:
             # Locate the coordinates of the non-zero data in the original dense array
             target_coords = self.coords[find_coords]
-            target_coords[:, 0] -= target_coords[:, 0].min()
+
+            # Some slightly complex indexing to identify the non-zero cells of the (indexed) target array
+            nonzero_row_indices_unique = np.where(np.isin(row_idx, np.unique(target_coords[:, 0])))[0]
+            nonzero_row_indices_unique_idx = np.unique(target_coords[:, 0], return_index=True)[1]
+
+            target_coords[:, 0] = -1
+            target_coords[nonzero_row_indices_unique_idx, 0] = nonzero_row_indices_unique
+
+            target_coords[:, 0] = np.maximum.accumulate(target_coords[:, 0], axis=0)
 
             # Re-create the dense array (of the shape requested) with all zeros
             target_data = np.zeros((1,) + self.dense_shape[1:]) if isinstance(row_idx, int) else np.zeros(
                 (len(row_idx),) + self.dense_shape[1:])
 
             # Fill the dense array with the non-zero data at the target coordinates
             target_data[tuple(target_coords.T)] = self.data[find_coords]
@@ -182,12 +197,12 @@
         """
 
         # Start by getting the values of the dense array at the given row indices,
         # with the dense array fully in memory
         target_data = self.__get_row(items[0])
 
         # Then index the dense array with the remaining indices as usual
-        items[0] = slice(None)
+        items[0] = Ellipsis
         target_data = target_data[tuple(items)]
 
         return target_data
```

### Comparing `pysparse-array-0.1.3/sparse/core.py` & `pysparse-array-0.1.4/sparse/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     :return: tuple of shape
     """
 
     data_shape = 0
     shape = array.shape
     announce_progress('Identifying sparse shape...') if verbose else None
 
-    if chunksize is None:
+    if (chunksize is None) or (type(array) is np.ndarray):
         data_shape = np.count_nonzero(array)
 
     else:
         for i in tqdm(range(0, shape[0], chunksize)) if verbose else range(0, shape[0], chunksize):
             data_shape += np.count_nonzero(array[i:i + chunksize])
 
     return (data_shape,)
@@ -59,15 +59,15 @@
     sparse_coords = list(sparse_coords)
     sparse_coords[0] += iteration
     sparse_coords = np.stack(sparse_coords, axis=1)
 
     return sparse_coords, sparse_values
 
 
-def __write_sparse_arrays(array: np.ndarray, path: 'str', chunksize: int, verbose: bool) -> None:
+def __write_sparse_arrays(array: np.ndarray or np.memmap, path: 'str', chunksize: int, verbose: bool) -> None:
     """
     Simultaneously convert and write a dense array to sparse arrays
     :param array: dense numpy array to be converted
     :param path: path to write sparse arrays to
     :param chunksize: chunksize to use for conversion - if None, will convert the whole array in memory
     :param verbose: whether to print progress statements
     :return:
@@ -91,40 +91,38 @@
 
     np.save(os.path.join(path, 'dense_shape.npy'), dense_shape)
 
     # Convert the dense array to sparse arrays
     announce_progress('Writing sparse arrays...') if verbose else None
     sparse_index = 0
 
-    if chunksize is None:
+    if (chunksize is None) or (type(array) is np.ndarray):
         sparse_coords, sparse_values = __convert_to_sparse_data(array, 0)
 
-        memmap_sparse_coords[sparse_index:sparse_index + sparse_coords.shape[0]] = sparse_coords
-        memmap_sparse_data[sparse_index:sparse_index + sparse_coords.shape[0]] = sparse_values
-
-        sparse_index += sparse_coords.shape[0]
+        memmap_sparse_coords[:] = sparse_coords
+        memmap_sparse_data[:] = sparse_values
 
     else:
         for chunk_idx in tqdm(range(0, dense_shape[0], chunksize)) if verbose else range(0, dense_shape[0], chunksize):
             sparse_coords, sparse_values = __convert_to_sparse_data(array[chunk_idx:chunk_idx + chunksize], chunk_idx)
 
             memmap_sparse_coords[sparse_index:sparse_index + sparse_coords.shape[0]] = sparse_coords
             memmap_sparse_data[sparse_index:sparse_index + sparse_coords.shape[0]] = sparse_values
 
             sparse_index += sparse_coords.shape[0]
 
     return
 
 
-def to_sparse(array: np.ndarray, savepath: 'str', chunksize=1000, verbose=True) -> None:
+def to_sparse(array: np.ndarray or np.memmap, savepath: 'str', chunksize=1000, verbose=True) -> None:
     """
     Convert and write a dense array to a sparse array
     :param array: numpy array to be converted
     :param savepath: filepath to write sparse array to
-    :param chunksize: number of rows to process at a time - if None, will process the whole array in memory
+    :param chunksize: number of memmap rows to process at a time if array is np.memmap - if None, will convert the whole array in memory
     :param verbose: whether to print progress statements
     :return: None
     """
     if not os.path.isdir(savepath):
         os.makedirs(savepath)
 
     __write_sparse_arrays(array, savepath, chunksize, verbose)
```

