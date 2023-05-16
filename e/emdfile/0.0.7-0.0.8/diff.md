# Comparing `tmp/emdfile-0.0.7.tar.gz` & `tmp/emdfile-0.0.8.tar.gz`

## Comparing `emdfile-0.0.7.tar` & `emdfile-0.0.8.tar`

### file list

```diff
@@ -1,31 +1,43 @@
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 emdfile-0.0.7/src/emdfile/__init__.py
--rw-r--r--   0        0        0    10788 2020-02-02 00:00:00.000000 emdfile-0.0.7/src/emdfile/read.py
--rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 emdfile-0.0.7/src/emdfile/tqdmnd.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 emdfile-0.0.7/src/emdfile/version.py
--rw-r--r--   0        0        0    31055 2020-02-02 00:00:00.000000 emdfile-0.0.7/src/emdfile/write.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 emdfile-0.0.7/src/emdfile/classes/__init__.py
--rw-r--r--   0        0        0    22633 2020-02-02 00:00:00.000000 emdfile-0.0.7/src/emdfile/classes/array.py
--rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 emdfile-0.0.7/src/emdfile/classes/custom.py
--rw-r--r--   0        0        0    10313 2020-02-02 00:00:00.000000 emdfile-0.0.7/src/emdfile/classes/metadata.py
--rw-r--r--   0        0        0     6671 2020-02-02 00:00:00.000000 emdfile-0.0.7/src/emdfile/classes/pointlist.py
--rw-r--r--   0        0        0     6155 2020-02-02 00:00:00.000000 emdfile-0.0.7/src/emdfile/classes/pointlistarray.py
--rw-r--r--   0        0        0    23911 2020-02-02 00:00:00.000000 emdfile-0.0.7/src/emdfile/classes/tree.py
--rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 emdfile-0.0.7/src/emdfile/classes/utils.py
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 emdfile-0.0.7/test/clear_h5_files.py
--rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 emdfile-0.0.7/test/test_base_classes.py
--rw-r--r--   0        0        0     3178 2020-02-02 00:00:00.000000 emdfile-0.0.7/test/test_emd.py
--rw-r--r--   0        0        0     3083 2020-02-02 00:00:00.000000 emdfile-0.0.7/test/test_header.py
--rw-r--r--   0        0        0    28996 2020-02-02 00:00:00.000000 emdfile-0.0.7/test/test_tree.py
--rw-r--r--   0        0        0   384837 2020-02-02 00:00:00.000000 emdfile-0.0.7/tutorials/emdfile_intro_example.ipynb
--rw-r--r--   0        0        0   167826 2020-02-02 00:00:00.000000 emdfile-0.0.7/tutorials/emdfile_package_walkthrough.ipynb
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 emdfile-0.0.7/tutorials/test_custom_classes.py
--rw-r--r--   0        0        0    81358 2020-02-02 00:00:00.000000 emdfile-0.0.7/tutorials/pngs/node.png
--rw-r--r--   0        0        0    41590 2020-02-02 00:00:00.000000 emdfile-0.0.7/tutorials/pngs/tree.png
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 emdfile-0.0.7/tutorials/sample_custom_emd_classes/__init__.py
--rw-r--r--   0        0        0     4838 2020-02-02 00:00:00.000000 emdfile-0.0.7/tutorials/sample_custom_emd_classes/custom_class_TEMPLATE.py
--rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 emdfile-0.0.7/tutorials/sample_custom_emd_classes/my_custom_classes.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 emdfile-0.0.7/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 emdfile-0.0.7/LICENSE
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 emdfile-0.0.7/README.md
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 emdfile-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 emdfile-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 emdfile-0.0.8/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 emdfile-0.0.8/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 emdfile-0.0.8/.pytest_cache/README.md
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 emdfile-0.0.8/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 emdfile-0.0.8/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 emdfile-0.0.8/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 emdfile-0.0.8/src/emdfile/__init__.py
+-rw-r--r--   0        0        0    10788 2020-02-02 00:00:00.000000 emdfile-0.0.8/src/emdfile/read.py
+-rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 emdfile-0.0.8/src/emdfile/tqdmnd.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 emdfile-0.0.8/src/emdfile/version.py
+-rw-r--r--   0        0        0    31055 2020-02-02 00:00:00.000000 emdfile-0.0.8/src/emdfile/write.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 emdfile-0.0.8/src/emdfile/classes/__init__.py
+-rw-r--r--   0        0        0    22633 2020-02-02 00:00:00.000000 emdfile-0.0.8/src/emdfile/classes/array.py
+-rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 emdfile-0.0.8/src/emdfile/classes/custom.py
+-rw-r--r--   0        0        0    10379 2020-02-02 00:00:00.000000 emdfile-0.0.8/src/emdfile/classes/metadata.py
+-rw-r--r--   0        0        0     6671 2020-02-02 00:00:00.000000 emdfile-0.0.8/src/emdfile/classes/pointlist.py
+-rw-r--r--   0        0        0     6155 2020-02-02 00:00:00.000000 emdfile-0.0.8/src/emdfile/classes/pointlistarray.py
+-rw-r--r--   0        0        0    23911 2020-02-02 00:00:00.000000 emdfile-0.0.8/src/emdfile/classes/tree.py
+-rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 emdfile-0.0.8/src/emdfile/classes/utils.py
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 emdfile-0.0.8/test/clear_h5_files.py
+-rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 emdfile-0.0.8/test/test_base_classes.py
+-rw-r--r--   0        0        0     3178 2020-02-02 00:00:00.000000 emdfile-0.0.8/test/test_emd.py
+-rw-r--r--   0        0        0     3083 2020-02-02 00:00:00.000000 emdfile-0.0.8/test/test_header.py
+-rw-r--r--   0        0        0    28996 2020-02-02 00:00:00.000000 emdfile-0.0.8/test/test_tree.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 emdfile-0.0.8/test/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 emdfile-0.0.8/test/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 emdfile-0.0.8/test/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 emdfile-0.0.8/test/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 emdfile-0.0.8/test/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 emdfile-0.0.8/test/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0   384837 2020-02-02 00:00:00.000000 emdfile-0.0.8/tutorials/emdfile_intro_example.ipynb
+-rw-r--r--   0        0        0   167826 2020-02-02 00:00:00.000000 emdfile-0.0.8/tutorials/emdfile_package_walkthrough.ipynb
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 emdfile-0.0.8/tutorials/test_custom_classes.py
+-rw-r--r--   0        0        0    81358 2020-02-02 00:00:00.000000 emdfile-0.0.8/tutorials/pngs/node.png
+-rw-r--r--   0        0        0    41590 2020-02-02 00:00:00.000000 emdfile-0.0.8/tutorials/pngs/tree.png
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 emdfile-0.0.8/tutorials/sample_custom_emd_classes/__init__.py
+-rw-r--r--   0        0        0     4838 2020-02-02 00:00:00.000000 emdfile-0.0.8/tutorials/sample_custom_emd_classes/custom_class_TEMPLATE.py
+-rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 emdfile-0.0.8/tutorials/sample_custom_emd_classes/my_custom_classes.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 emdfile-0.0.8/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 emdfile-0.0.8/LICENSE
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 emdfile-0.0.8/README.md
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 emdfile-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 emdfile-0.0.8/PKG-INFO
```

### Comparing `emdfile-0.0.7/src/emdfile/__init__.py` & `emdfile-0.0.8/src/emdfile/__init__.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.7/src/emdfile/read.py` & `emdfile-0.0.8/src/emdfile/read.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.7/src/emdfile/tqdmnd.py` & `emdfile-0.0.8/src/emdfile/tqdmnd.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.7/src/emdfile/write.py` & `emdfile-0.0.8/src/emdfile/write.py`

 * *Files 1% similar despite different names*

```diff
@@ -731,15 +731,15 @@
     metadata_groups = []
     if "metadatabundle" not in rootgroup.keys():
         mdbundle_group = rootgroup.create_group('metadatabundle')
     else:
         mdbundle_group = rootgroup['metadatabundle']
         for k in mdbundle_group.keys():
             if "emd_group_type" in mdbundle_group[k].attrs.keys():
-                if mdbundle_group[k].attrs["emd_group_keys"] == "metadata":
+                if mdbundle_group[k].attrs["emd_group_type"] == "metadata":
                     metadata_groups.append(k)
     # loop
     for key in root._metadata:
         # if this group already exists
         if key in metadata_groups:
             # overwrite it
             if appendover:
```

### Comparing `emdfile-0.0.7/src/emdfile/classes/array.py` & `emdfile-0.0.8/src/emdfile/classes/array.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.7/src/emdfile/classes/custom.py` & `emdfile-0.0.8/src/emdfile/classes/custom.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.7/src/emdfile/classes/metadata.py` & `emdfile-0.0.8/src/emdfile/classes/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -230,15 +230,17 @@
 
         # Get data
         data = {}
         for k,v in group.items():
 
             # get type
             try:
-                t = group[k].attrs['type'].decode('utf-8')
+                t = group[k].attrs['type']
+                if isinstance(t,bytes):
+                    t = t.decode('utf-8')
             except KeyError:
                 raise Exception(f"unrecognized Metadata value type {type(v)}")
 
             # None
             if t == 'None':
                 v = None
```

### Comparing `emdfile-0.0.7/src/emdfile/classes/pointlist.py` & `emdfile-0.0.8/src/emdfile/classes/pointlist.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.7/src/emdfile/classes/pointlistarray.py` & `emdfile-0.0.8/src/emdfile/classes/pointlistarray.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.7/src/emdfile/classes/tree.py` & `emdfile-0.0.8/src/emdfile/classes/tree.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.7/src/emdfile/classes/utils.py` & `emdfile-0.0.8/src/emdfile/classes/utils.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.7/test/clear_h5_files.py` & `emdfile-0.0.8/test/clear_h5_files.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.7/test/test_base_classes.py` & `emdfile-0.0.8/test/test_base_classes.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.7/test/test_emd.py` & `emdfile-0.0.8/test/test_emd.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.7/test/test_header.py` & `emdfile-0.0.8/test/test_header.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.7/test/test_tree.py` & `emdfile-0.0.8/test/test_tree.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.7/tutorials/emdfile_intro_example.ipynb` & `emdfile-0.0.8/tutorials/emdfile_intro_example.ipynb`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.7/tutorials/emdfile_package_walkthrough.ipynb` & `emdfile-0.0.8/tutorials/emdfile_package_walkthrough.ipynb`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.7/tutorials/test_custom_classes.py` & `emdfile-0.0.8/tutorials/test_custom_classes.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.7/tutorials/pngs/node.png` & `emdfile-0.0.8/tutorials/pngs/node.png`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.7/tutorials/pngs/tree.png` & `emdfile-0.0.8/tutorials/pngs/tree.png`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.7/tutorials/sample_custom_emd_classes/custom_class_TEMPLATE.py` & `emdfile-0.0.8/tutorials/sample_custom_emd_classes/custom_class_TEMPLATE.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.7/tutorials/sample_custom_emd_classes/my_custom_classes.py` & `emdfile-0.0.8/tutorials/sample_custom_emd_classes/my_custom_classes.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.7/LICENSE` & `emdfile-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.7/README.md` & `emdfile-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.7/pyproject.toml` & `emdfile-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.7/PKG-INFO` & `emdfile-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emdfile
-Version: 0.0.7
+Version: 0.0.8
 Project-URL: github, https://github.com/py4dstem/emdfile
 Project-URL: emdatasets, https://emdatasets.com/format/
 Author-email: "Benjamin H. Savitzky" <ben.savitzky@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

