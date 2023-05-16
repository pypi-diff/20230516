# Comparing `tmp/unitpackage-0.7.0.tar.gz` & `tmp/unitpackage-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitpackage-0.7.0.tar", last modified: Tue May 16 14:45:28 2023, max compression
+gzip compressed data, was "unitpackage-0.7.1.tar", last modified: Tue May 16 18:12:47 2023, max compression
```

## Comparing `unitpackage-0.7.0.tar` & `unitpackage-0.7.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 14:45:28.363668 unitpackage-0.7.0/
--rw-rw-rw-   0        0        0    35823 2023-05-08 22:00:28.000000 unitpackage-0.7.0/LICENSE
--rw-rw-rw-   0        0        0     4982 2023-05-16 14:45:28.362723 unitpackage-0.7.0/PKG-INFO
--rw-rw-rw-   0        0        0     4752 2023-05-16 14:45:20.000000 unitpackage-0.7.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-16 14:45:28.363668 unitpackage-0.7.0/setup.cfg
--rw-rw-rw-   0        0        0     1724 2023-05-16 14:45:20.000000 unitpackage-0.7.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:45:28.350665 unitpackage-0.7.0/unitpackage/
--rw-rw-rw-   0        0        0        0 2023-05-16 14:21:15.000000 unitpackage-0.7.0/unitpackage/__init__.py
--rw-rw-rw-   0        0        0     8082 2023-05-16 14:21:15.000000 unitpackage-0.7.0/unitpackage/collection.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:45:28.360671 unitpackage-0.7.0/unitpackage/cv/
--rw-rw-rw-   0        0        0        0 2023-05-16 14:21:15.000000 unitpackage-0.7.0/unitpackage/cv/__init__.py
--rw-rw-rw-   0        0        0     3626 2023-05-16 14:21:15.000000 unitpackage-0.7.0/unitpackage/cv/cv_collection.py
--rw-rw-rw-   0        0        0     9399 2023-05-16 14:21:15.000000 unitpackage-0.7.0/unitpackage/cv/cv_entry.py
--rw-rw-rw-   0        0        0     7542 2023-05-16 14:21:15.000000 unitpackage-0.7.0/unitpackage/descriptor.py
--rw-rw-rw-   0        0        0    19831 2023-05-16 14:21:15.000000 unitpackage-0.7.0/unitpackage/entry.py
--rw-rw-rw-   0        0        0     2563 2023-05-16 14:21:15.000000 unitpackage-0.7.0/unitpackage/local.py
--rw-rw-rw-   0        0        0     2652 2023-05-16 14:21:15.000000 unitpackage-0.7.0/unitpackage/remote.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:45:28.356680 unitpackage-0.7.0/unitpackage.egg-info/
--rw-rw-rw-   0        0        0     4982 2023-05-16 14:45:28.000000 unitpackage-0.7.0/unitpackage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      426 2023-05-16 14:45:28.000000 unitpackage-0.7.0/unitpackage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 14:45:28.000000 unitpackage-0.7.0/unitpackage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      148 2023-05-16 14:45:28.000000 unitpackage-0.7.0/unitpackage.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-16 14:45:28.000000 unitpackage-0.7.0/unitpackage.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 18:12:47.912409 unitpackage-0.7.1/
+-rw-rw-rw-   0        0        0    35823 2023-05-08 22:00:28.000000 unitpackage-0.7.1/LICENSE
+-rw-rw-rw-   0        0        0     4982 2023-05-16 18:12:47.911409 unitpackage-0.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4752 2023-05-16 18:12:42.000000 unitpackage-0.7.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-16 18:12:47.912409 unitpackage-0.7.1/setup.cfg
+-rw-rw-rw-   0        0        0     1724 2023-05-16 18:12:42.000000 unitpackage-0.7.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 18:12:47.904890 unitpackage-0.7.1/unitpackage/
+-rw-rw-rw-   0        0        0        0 2023-05-16 17:49:24.000000 unitpackage-0.7.1/unitpackage/__init__.py
+-rw-rw-rw-   0        0        0     8082 2023-05-16 17:49:24.000000 unitpackage-0.7.1/unitpackage/collection.py
+drwxrwxrwx   0        0        0        0 2023-05-16 18:12:47.910410 unitpackage-0.7.1/unitpackage/cv/
+-rw-rw-rw-   0        0        0        0 2023-05-16 17:49:24.000000 unitpackage-0.7.1/unitpackage/cv/__init__.py
+-rw-rw-rw-   0        0        0     3626 2023-05-16 17:49:24.000000 unitpackage-0.7.1/unitpackage/cv/cv_collection.py
+-rw-rw-rw-   0        0        0     9399 2023-05-16 17:49:24.000000 unitpackage-0.7.1/unitpackage/cv/cv_entry.py
+-rw-rw-rw-   0        0        0     7542 2023-05-16 17:49:24.000000 unitpackage-0.7.1/unitpackage/descriptor.py
+-rw-rw-rw-   0        0        0    19831 2023-05-16 17:49:24.000000 unitpackage-0.7.1/unitpackage/entry.py
+-rw-rw-rw-   0        0        0     2563 2023-05-16 17:49:24.000000 unitpackage-0.7.1/unitpackage/local.py
+-rw-rw-rw-   0        0        0     2652 2023-05-16 17:49:24.000000 unitpackage-0.7.1/unitpackage/remote.py
+drwxrwxrwx   0        0        0        0 2023-05-16 18:12:47.908401 unitpackage-0.7.1/unitpackage.egg-info/
+-rw-rw-rw-   0        0        0     4982 2023-05-16 18:12:47.000000 unitpackage-0.7.1/unitpackage.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      426 2023-05-16 18:12:47.000000 unitpackage-0.7.1/unitpackage.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 18:12:47.000000 unitpackage-0.7.1/unitpackage.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      148 2023-05-16 18:12:47.000000 unitpackage-0.7.1/unitpackage.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-16 18:12:47.000000 unitpackage-0.7.1/unitpackage.egg-info/top_level.txt
```

### Comparing `unitpackage-0.7.0/LICENSE` & `unitpackage-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `unitpackage-0.7.0/PKG-INFO` & `unitpackage-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: unitpackage
-Version: 0.7.0
+Version: 0.7.1
 Summary: a Python library to work with the echemdb repository
 License: GPL 3.0+
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/echemdb/unitpackage/0.7.0?urlpath=tree%2Fdoc%2Fusage%2Fentry_interactions.md)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/echemdb/unitpackage/0.7.1?urlpath=tree%2Fdoc%2Fusage%2Fentry_interactions.md)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6502901.svg)](https://doi.org/10.5281/zenodo.6502901)
 
 This module provides a Python library to interact with a collection of
 [frictionless datapackages](https://frictionlessdata.io/). Such datapackages consist of a CSV (data) file which is annotated with a JSON file.
 This allows storing additional information such as units used in the columns of a CSV or store metadata describing the underlying data.
 Example datapackages can be found [here](https://github.com/echemdb/unitpackage/tree/main/doc/files/) and a JSON could be structured as follows
```

### Comparing `unitpackage-0.7.0/README.md` & `unitpackage-0.7.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 00000000: 5b21 5b42 696e 6465 725d 2868 7474 7073  [![Binder](https
 00000010: 3a2f 2f6d 7962 696e 6465 722e 6f72 672f  ://mybinder.org/
 00000020: 6261 6467 655f 6c6f 676f 2e73 7667 295d  badge_logo.svg)]
 00000030: 2868 7474 7073 3a2f 2f6d 7962 696e 6465  (https://mybinde
 00000040: 722e 6f72 672f 7632 2f67 682f 6563 6865  r.org/v2/gh/eche
 00000050: 6d64 622f 756e 6974 7061 636b 6167 652f  mdb/unitpackage/
-00000060: 302e 372e 303f 7572 6c70 6174 683d 7472  0.7.0?urlpath=tr
+00000060: 302e 372e 313f 7572 6c70 6174 683d 7472  0.7.1?urlpath=tr
 00000070: 6565 2532 4664 6f63 2532 4675 7361 6765  ee%2Fdoc%2Fusage
 00000080: 2532 4665 6e74 7279 5f69 6e74 6572 6163  %2Fentry_interac
 00000090: 7469 6f6e 732e 6d64 290d 0a5b 215b 444f  tions.md)..[![DO
 000000a0: 495d 2868 7474 7073 3a2f 2f7a 656e 6f64  I](https://zenod
 000000b0: 6f2e 6f72 672f 6261 6467 652f 444f 492f  o.org/badge/DOI/
 000000c0: 3130 2e35 3238 312f 7a65 6e6f 646f 2e36  10.5281/zenodo.6
 000000d0: 3530 3239 3031 2e73 7667 295d 2868 7474  502901.svg)](htt
```

### Comparing `unitpackage-0.7.0/setup.py` & `unitpackage-0.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 #  along with unitpackage. If not, see <https://www.gnu.org/licenses/>.
 # ********************************************************************
 
 from distutils.core import setup
 
 setup(
     name='unitpackage',
-    version="0.7.0",
+    version="0.7.1",
     packages=['unitpackage', 'unitpackage.cv'],
     license='GPL 3.0+',
     description="a Python library to work with the echemdb repository",
     long_description=open('README.md', encoding="UTF-8").read(),
     long_description_content_type="text/markdown",
     include_package_data=True,
     install_requires=[
```

### Comparing `unitpackage-0.7.0/unitpackage/collection.py` & `unitpackage-0.7.1/unitpackage/collection.py`

 * *Files identical despite different names*

### Comparing `unitpackage-0.7.0/unitpackage/cv/cv_collection.py` & `unitpackage-0.7.1/unitpackage/cv/cv_collection.py`

 * *Files identical despite different names*

### Comparing `unitpackage-0.7.0/unitpackage/cv/cv_entry.py` & `unitpackage-0.7.1/unitpackage/cv/cv_entry.py`

 * *Files identical despite different names*

### Comparing `unitpackage-0.7.0/unitpackage/descriptor.py` & `unitpackage-0.7.1/unitpackage/descriptor.py`

 * *Files identical despite different names*

### Comparing `unitpackage-0.7.0/unitpackage/entry.py` & `unitpackage-0.7.1/unitpackage/entry.py`

 * *Files identical despite different names*

### Comparing `unitpackage-0.7.0/unitpackage/local.py` & `unitpackage-0.7.1/unitpackage/local.py`

 * *Files identical despite different names*

### Comparing `unitpackage-0.7.0/unitpackage/remote.py` & `unitpackage-0.7.1/unitpackage/remote.py`

 * *Files identical despite different names*

### Comparing `unitpackage-0.7.0/unitpackage.egg-info/PKG-INFO` & `unitpackage-0.7.1/unitpackage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: unitpackage
-Version: 0.7.0
+Version: 0.7.1
 Summary: a Python library to work with the echemdb repository
 License: GPL 3.0+
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/echemdb/unitpackage/0.7.0?urlpath=tree%2Fdoc%2Fusage%2Fentry_interactions.md)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/echemdb/unitpackage/0.7.1?urlpath=tree%2Fdoc%2Fusage%2Fentry_interactions.md)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6502901.svg)](https://doi.org/10.5281/zenodo.6502901)
 
 This module provides a Python library to interact with a collection of
 [frictionless datapackages](https://frictionlessdata.io/). Such datapackages consist of a CSV (data) file which is annotated with a JSON file.
 This allows storing additional information such as units used in the columns of a CSV or store metadata describing the underlying data.
 Example datapackages can be found [here](https://github.com/echemdb/unitpackage/tree/main/doc/files/) and a JSON could be structured as follows
```

