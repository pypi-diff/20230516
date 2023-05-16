# Comparing `tmp/emdfile-0.0.6.tar.gz` & `tmp/emdfile-0.0.7.tar.gz`

## Comparing `emdfile-0.0.6.tar` & `emdfile-0.0.7.tar`

### file list

```diff
@@ -1,48 +1,31 @@
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 emdfile-0.0.6/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 emdfile-0.0.6/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 emdfile-0.0.6/.pytest_cache/README.md
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 emdfile-0.0.6/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 emdfile-0.0.6/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 emdfile-0.0.6/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 emdfile-0.0.6/src/emdfile/__init__.py
--rw-r--r--   0        0        0    10788 2020-02-02 00:00:00.000000 emdfile-0.0.6/src/emdfile/read.py
--rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 emdfile-0.0.6/src/emdfile/tqdmnd.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 emdfile-0.0.6/src/emdfile/version.py
--rw-r--r--   0        0        0    31055 2020-02-02 00:00:00.000000 emdfile-0.0.6/src/emdfile/write.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 emdfile-0.0.6/src/emdfile/classes/__init__.py
--rw-r--r--   0        0        0    22633 2020-02-02 00:00:00.000000 emdfile-0.0.6/src/emdfile/classes/array.py
--rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 emdfile-0.0.6/src/emdfile/classes/custom.py
--rw-r--r--   0        0        0    10249 2020-02-02 00:00:00.000000 emdfile-0.0.6/src/emdfile/classes/metadata.py
--rw-r--r--   0        0        0     6671 2020-02-02 00:00:00.000000 emdfile-0.0.6/src/emdfile/classes/pointlist.py
--rw-r--r--   0        0        0     6155 2020-02-02 00:00:00.000000 emdfile-0.0.6/src/emdfile/classes/pointlistarray.py
--rw-r--r--   0        0        0    23911 2020-02-02 00:00:00.000000 emdfile-0.0.6/src/emdfile/classes/tree.py
--rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 emdfile-0.0.6/src/emdfile/classes/utils.py
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 emdfile-0.0.6/test/clear_h5_files.py
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 emdfile-0.0.6/test/test_base_classes.py
--rw-r--r--   0        0        0     3178 2020-02-02 00:00:00.000000 emdfile-0.0.6/test/test_emd.py
--rw-r--r--   0        0        0     3083 2020-02-02 00:00:00.000000 emdfile-0.0.6/test/test_header.py
--rw-r--r--   0        0        0    28996 2020-02-02 00:00:00.000000 emdfile-0.0.6/test/test_tree.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 emdfile-0.0.6/test/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 emdfile-0.0.6/test/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 emdfile-0.0.6/test/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 emdfile-0.0.6/test/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 emdfile-0.0.6/test/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 emdfile-0.0.6/test/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0   384837 2020-02-02 00:00:00.000000 emdfile-0.0.6/tutorials/emdfile_intro_example.ipynb
--rw-r--r--   0        0        0   167826 2020-02-02 00:00:00.000000 emdfile-0.0.6/tutorials/emdfile_package_walkthrough.ipynb
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 emdfile-0.0.6/tutorials/test_custom_classes.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 emdfile-0.0.6/tutorials/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 emdfile-0.0.6/tutorials/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 emdfile-0.0.6/tutorials/.pytest_cache/README.md
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 emdfile-0.0.6/tutorials/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 emdfile-0.0.6/tutorials/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 emdfile-0.0.6/tutorials/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0    81358 2020-02-02 00:00:00.000000 emdfile-0.0.6/tutorials/pngs/node.png
--rw-r--r--   0        0        0    41590 2020-02-02 00:00:00.000000 emdfile-0.0.6/tutorials/pngs/tree.png
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 emdfile-0.0.6/tutorials/sample_custom_emd_classes/__init__.py
--rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 emdfile-0.0.6/tutorials/sample_custom_emd_classes/my_custom_classes.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 emdfile-0.0.6/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 emdfile-0.0.6/LICENSE
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 emdfile-0.0.6/README.md
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 emdfile-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 emdfile-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 emdfile-0.0.7/src/emdfile/__init__.py
+-rw-r--r--   0        0        0    10788 2020-02-02 00:00:00.000000 emdfile-0.0.7/src/emdfile/read.py
+-rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 emdfile-0.0.7/src/emdfile/tqdmnd.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 emdfile-0.0.7/src/emdfile/version.py
+-rw-r--r--   0        0        0    31055 2020-02-02 00:00:00.000000 emdfile-0.0.7/src/emdfile/write.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 emdfile-0.0.7/src/emdfile/classes/__init__.py
+-rw-r--r--   0        0        0    22633 2020-02-02 00:00:00.000000 emdfile-0.0.7/src/emdfile/classes/array.py
+-rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 emdfile-0.0.7/src/emdfile/classes/custom.py
+-rw-r--r--   0        0        0    10313 2020-02-02 00:00:00.000000 emdfile-0.0.7/src/emdfile/classes/metadata.py
+-rw-r--r--   0        0        0     6671 2020-02-02 00:00:00.000000 emdfile-0.0.7/src/emdfile/classes/pointlist.py
+-rw-r--r--   0        0        0     6155 2020-02-02 00:00:00.000000 emdfile-0.0.7/src/emdfile/classes/pointlistarray.py
+-rw-r--r--   0        0        0    23911 2020-02-02 00:00:00.000000 emdfile-0.0.7/src/emdfile/classes/tree.py
+-rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 emdfile-0.0.7/src/emdfile/classes/utils.py
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 emdfile-0.0.7/test/clear_h5_files.py
+-rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 emdfile-0.0.7/test/test_base_classes.py
+-rw-r--r--   0        0        0     3178 2020-02-02 00:00:00.000000 emdfile-0.0.7/test/test_emd.py
+-rw-r--r--   0        0        0     3083 2020-02-02 00:00:00.000000 emdfile-0.0.7/test/test_header.py
+-rw-r--r--   0        0        0    28996 2020-02-02 00:00:00.000000 emdfile-0.0.7/test/test_tree.py
+-rw-r--r--   0        0        0   384837 2020-02-02 00:00:00.000000 emdfile-0.0.7/tutorials/emdfile_intro_example.ipynb
+-rw-r--r--   0        0        0   167826 2020-02-02 00:00:00.000000 emdfile-0.0.7/tutorials/emdfile_package_walkthrough.ipynb
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 emdfile-0.0.7/tutorials/test_custom_classes.py
+-rw-r--r--   0        0        0    81358 2020-02-02 00:00:00.000000 emdfile-0.0.7/tutorials/pngs/node.png
+-rw-r--r--   0        0        0    41590 2020-02-02 00:00:00.000000 emdfile-0.0.7/tutorials/pngs/tree.png
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 emdfile-0.0.7/tutorials/sample_custom_emd_classes/__init__.py
+-rw-r--r--   0        0        0     4838 2020-02-02 00:00:00.000000 emdfile-0.0.7/tutorials/sample_custom_emd_classes/custom_class_TEMPLATE.py
+-rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 emdfile-0.0.7/tutorials/sample_custom_emd_classes/my_custom_classes.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 emdfile-0.0.7/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 emdfile-0.0.7/LICENSE
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 emdfile-0.0.7/README.md
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 emdfile-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 emdfile-0.0.7/PKG-INFO
```

### Comparing `emdfile-0.0.6/src/emdfile/__init__.py` & `emdfile-0.0.7/src/emdfile/__init__.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.6/src/emdfile/read.py` & `emdfile-0.0.7/src/emdfile/read.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.6/src/emdfile/tqdmnd.py` & `emdfile-0.0.7/src/emdfile/tqdmnd.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.6/src/emdfile/write.py` & `emdfile-0.0.7/src/emdfile/write.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.6/src/emdfile/classes/array.py` & `emdfile-0.0.7/src/emdfile/classes/array.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.6/src/emdfile/classes/custom.py` & `emdfile-0.0.7/src/emdfile/classes/custom.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.6/src/emdfile/classes/metadata.py` & `emdfile-0.0.7/src/emdfile/classes/metadata.py`

 * *Files 6% similar despite different names*

```diff
@@ -99,110 +99,110 @@
 
         # Save data
         for k,v in self._params.items():
 
             # None
             if v is None:
                 v = "_None"
-                v = np.string_(v)  # convert to byte string
+                v = v.encode('utf-8')  # convert to byte string
                 dset = grp.create_dataset(k, data=v)
-                dset.attrs['type'] = np.string_('None')
+                dset.attrs['type'] = 'None'.encode('utf-8')
 
             # strings
             elif isinstance(v, str):
-                v = np.string_(v)  # convert to byte string
+                v = v.encode('utf-8')  # convert to byte string
                 dset = grp.create_dataset(k, data=v)
-                dset.attrs['type'] = np.string_('string')
+                dset.attrs['type'] = 'string'.encode('utf-8')
 
             # bools
             elif isinstance(v, bool):
                 dset = grp.create_dataset(k, data=v, dtype=bool)
-                dset.attrs['type'] = np.string_('bool')
+                dset.attrs['type'] = 'bool'.encode('utf-8')
 
             # numbers
             elif isinstance(v, Number):
                 dset = grp.create_dataset(k, data=v, dtype=type(v))
-                dset.attrs['type'] = np.string_('number')
+                dset.attrs['type'] = 'number'.encode('utf-8')
 
             # arrays
             elif isinstance(v, np.ndarray):
                 dset = grp.create_dataset(k, data=v, dtype=v.dtype)
-                dset.attrs['type'] = np.string_('array')
+                dset.attrs['type'] = 'array'.encode('utf-8')
 
             # tuples
             elif isinstance(v, tuple):
 
                 # of numbers
                 if isinstance(v[0], Number):
                     dset = grp.create_dataset(k, data=v)
-                    dset.attrs['type'] = np.string_('tuple')
+                    dset.attrs['type'] = 'tuple'.encode('utf-8')
 
                 # of tuples
                 elif any([isinstance(v[i], tuple) for i in range(len(v))]):
                     dset_grp = grp.create_group(k)
-                    dset_grp.attrs['type'] = np.string_('tuple_of_tuples')
+                    dset_grp.attrs['type'] = 'tuple_of_tuples'.encode('utf-8')
                     dset_grp.attrs['length'] = len(v)
                     for i,x in enumerate(v):
                         dset_grp.create_dataset(
                             str(i),
                             data=x)
 
                 # of arrays
                 elif isinstance(v[0], np.ndarray):
                     dset_grp = grp.create_group(k)
-                    dset_grp.attrs['type'] = np.string_('tuple_of_arrays')
+                    dset_grp.attrs['type'] = 'tuple_of_arrays'.encode('utf-8')
                     dset_grp.attrs['length'] = len(v)
                     for i,ar in enumerate(v):
                         dset_grp.create_dataset(
                             str(i),
                             data=ar,
                             dtype=ar.dtype)
 
                 # of strings
                 elif isinstance(v[0], str):
                     dset_grp = grp.create_group(k)
-                    dset_grp.attrs['type'] = np.string_('tuple_of_strings')
+                    dset_grp.attrs['type'] = 'tuple_of_strings'.encode('utf-8')
                     dset_grp.attrs['length'] = len(v)
                     for i,s in enumerate(v):
                         dset_grp.create_dataset(
                             str(i),
-                            data=np.string_(s))
+                            data=s.encode('utf-8'))
 
                 else:
                     er = f"Metadata only supports writing tuples with numeric and array-like arguments; found type {type(v[0])}"
                     raise Exception(er)
 
             # lists
             elif isinstance(v, list):
 
                 # of numbers
                 if isinstance(v[0], Number):
                     dset = grp.create_dataset(k, data=v)
-                    dset.attrs['type'] = np.string_('list')
+                    dset.attrs['type'] = 'list'.encode('utf-8')
 
                 # of arrays
                 elif isinstance(v[0], np.ndarray):
                     dset_grp = grp.create_group(k)
-                    dset_grp.attrs['type'] = np.string_('list_of_arrays')
+                    dset_grp.attrs['type'] = 'list_of_arrays'.encode('utf-8')
                     dset_grp.attrs['length'] = len(v)
                     for i,ar in enumerate(v):
                         dset_grp.create_dataset(
                             str(i),
                             data=ar,
                             dtype=ar.dtype)
 
                 # of strings
                 elif isinstance(v[0], str):
                     dset_grp = grp.create_group(k)
-                    dset_grp.attrs['type'] = np.string_('list_of_strings')
+                    dset_grp.attrs['type'] = 'list_of_strings'.encode('utf-8')
                     dset_grp.attrs['length'] = len(v)
                     for i,s in enumerate(v):
                         dset_grp.create_dataset(
                             str(i),
-                            data=np.string_(s))
+                            data=s.encode('utf-8'))
 
                 else:
                     er = f"Metadata only supports writing lists with numeric and array-like arguments; found type {type(v[0])}"
                     raise Exception(er)
 
             else:
                 er = f"Metadata supports writing numbers, bools, strings, arrays, tuples of numbers or arrays, and lists of numbers or arrays. Found an unsupported type {type(v[0])}"
```

### Comparing `emdfile-0.0.6/src/emdfile/classes/pointlist.py` & `emdfile-0.0.7/src/emdfile/classes/pointlist.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.6/src/emdfile/classes/pointlistarray.py` & `emdfile-0.0.7/src/emdfile/classes/pointlistarray.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.6/src/emdfile/classes/tree.py` & `emdfile-0.0.7/src/emdfile/classes/tree.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.6/src/emdfile/classes/utils.py` & `emdfile-0.0.7/src/emdfile/classes/utils.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.6/test/clear_h5_files.py` & `emdfile-0.0.7/test/clear_h5_files.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.6/test/test_emd.py` & `emdfile-0.0.7/test/test_emd.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.6/test/test_header.py` & `emdfile-0.0.7/test/test_header.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.6/test/test_tree.py` & `emdfile-0.0.7/test/test_tree.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.6/tutorials/emdfile_intro_example.ipynb` & `emdfile-0.0.7/tutorials/emdfile_intro_example.ipynb`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.6/tutorials/emdfile_package_walkthrough.ipynb` & `emdfile-0.0.7/tutorials/emdfile_package_walkthrough.ipynb`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.6/tutorials/test_custom_classes.py` & `emdfile-0.0.7/tutorials/test_custom_classes.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.6/tutorials/pngs/node.png` & `emdfile-0.0.7/tutorials/pngs/node.png`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.6/tutorials/pngs/tree.png` & `emdfile-0.0.7/tutorials/pngs/tree.png`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.6/tutorials/sample_custom_emd_classes/my_custom_classes.py` & `emdfile-0.0.7/tutorials/sample_custom_emd_classes/my_custom_classes.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.6/LICENSE` & `emdfile-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.6/README.md` & `emdfile-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.6/pyproject.toml` & `emdfile-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.6/PKG-INFO` & `emdfile-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emdfile
-Version: 0.0.6
+Version: 0.0.7
 Project-URL: github, https://github.com/py4dstem/emdfile
 Project-URL: emdatasets, https://emdatasets.com/format/
 Author-email: "Benjamin H. Savitzky" <ben.savitzky@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

