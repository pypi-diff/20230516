# Comparing `tmp/hybridcontents-0.3.0.tar.gz` & `tmp/hybridcontents-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hybridcontents-0.3.0.tar", last modified: Wed Jan 22 20:27:10 2020, max compression
+gzip compressed data, was "hybridcontents-0.4.0.tar", last modified: Tue May 16 01:51:58 2023, max compression
```

## Comparing `hybridcontents-0.3.0.tar` & `hybridcontents-0.4.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 devstein   (501) staff       (20)        0 2020-01-22 20:27:10.000000 hybridcontents-0.3.0/
--rw-r--r--   0 devstein   (501) staff       (20)     5139 2020-01-22 20:27:10.000000 hybridcontents-0.3.0/PKG-INFO
--rw-r--r--   0 devstein   (501) staff       (20)    11324 2019-10-10 19:12:46.000000 hybridcontents-0.3.0/LICENSE
--rw-r--r--   0 devstein   (501) staff       (20)       30 2019-12-05 01:49:20.000000 hybridcontents-0.3.0/requirements.txt
--rw-r--r--   0 devstein   (501) staff       (20)      121 2019-12-07 01:04:32.000000 hybridcontents-0.3.0/MANIFEST.in
--rw-r--r--   0 devstein   (501) staff       (20)     3467 2020-01-12 17:32:59.000000 hybridcontents-0.3.0/README.md
-drwxr-xr-x   0 devstein   (501) staff       (20)        0 2020-01-22 20:27:10.000000 hybridcontents-0.3.0/hybridcontents/
-drwxr-xr-x   0 devstein   (501) staff       (20)        0 2020-01-22 20:27:10.000000 hybridcontents-0.3.0/hybridcontents/tests/
--rw-r--r--   0 devstein   (501) staff       (20)      435 2019-12-05 01:49:20.000000 hybridcontents-0.3.0/hybridcontents/tests/testing_utils.py
--rw-r--r--   0 devstein   (501) staff       (20)        0 2019-12-05 01:49:20.000000 hybridcontents-0.3.0/hybridcontents/tests/__init__.py
--rw-r--r--   0 devstein   (501) staff       (20)    12399 2020-01-22 20:19:19.000000 hybridcontents-0.3.0/hybridcontents/tests/test_hybrid_manager.py
--rw-r--r--   0 devstein   (501) staff       (20)       93 2019-12-05 01:49:20.000000 hybridcontents-0.3.0/hybridcontents/__init__.py
--rw-r--r--   0 devstein   (501) staff       (20)    10679 2020-01-22 20:19:19.000000 hybridcontents-0.3.0/hybridcontents/hybridmanager.py
--rw-r--r--   0 devstein   (501) staff       (20)     1580 2020-01-10 19:54:16.000000 hybridcontents-0.3.0/hybridcontents/api_utils.py
--rw-r--r--   0 devstein   (501) staff       (20)     1832 2020-01-22 20:22:45.000000 hybridcontents-0.3.0/setup.py
-drwxr-xr-x   0 devstein   (501) staff       (20)        0 2020-01-22 20:27:10.000000 hybridcontents-0.3.0/hybridcontents.egg-info/
--rw-r--r--   0 devstein   (501) staff       (20)     5139 2020-01-22 20:27:10.000000 hybridcontents-0.3.0/hybridcontents.egg-info/PKG-INFO
--rw-r--r--   0 devstein   (501) staff       (20)        1 2019-12-07 01:14:28.000000 hybridcontents-0.3.0/hybridcontents.egg-info/zip-safe
--rw-r--r--   0 devstein   (501) staff       (20)      511 2020-01-22 20:27:10.000000 hybridcontents-0.3.0/hybridcontents.egg-info/SOURCES.txt
--rw-r--r--   0 devstein   (501) staff       (20)       99 2020-01-22 20:27:10.000000 hybridcontents-0.3.0/hybridcontents.egg-info/requires.txt
--rw-r--r--   0 devstein   (501) staff       (20)       15 2020-01-22 20:27:10.000000 hybridcontents-0.3.0/hybridcontents.egg-info/top_level.txt
--rw-r--r--   0 devstein   (501) staff       (20)        1 2020-01-22 20:27:10.000000 hybridcontents-0.3.0/hybridcontents.egg-info/dependency_links.txt
--rw-r--r--   0 devstein   (501) staff       (20)       79 2020-01-22 20:27:10.000000 hybridcontents-0.3.0/setup.cfg
--rw-r--r--   0 devstein   (501) staff       (20)       73 2019-12-05 01:49:20.000000 hybridcontents-0.3.0/requirements_test.txt
+drwxr-xr-x   0 john       (501) staff       (20)        0 2023-05-16 01:51:58.264917 hybridcontents-0.4.0/
+-rw-r--r--   0 john       (501) staff       (20)    11324 2023-05-16 01:44:05.000000 hybridcontents-0.4.0/LICENSE
+-rw-r--r--   0 john       (501) staff       (20)      121 2023-05-16 01:44:05.000000 hybridcontents-0.4.0/MANIFEST.in
+-rw-r--r--   0 john       (501) staff       (20)     4465 2023-05-16 01:51:58.265012 hybridcontents-0.4.0/PKG-INFO
+-rw-r--r--   0 john       (501) staff       (20)     3578 2023-05-16 01:44:05.000000 hybridcontents-0.4.0/README.md
+drwxr-xr-x   0 john       (501) staff       (20)        0 2023-05-16 01:51:58.263771 hybridcontents-0.4.0/hybridcontents/
+-rw-r--r--   0 john       (501) staff       (20)       93 2023-05-16 01:44:05.000000 hybridcontents-0.4.0/hybridcontents/__init__.py
+-rw-r--r--   0 john       (501) staff       (20)     1580 2023-05-16 01:44:05.000000 hybridcontents-0.4.0/hybridcontents/api_utils.py
+-rw-r--r--   0 john       (501) staff       (20)    10041 2023-05-16 01:44:05.000000 hybridcontents-0.4.0/hybridcontents/hybridmanager.py
+drwxr-xr-x   0 john       (501) staff       (20)        0 2023-05-16 01:51:58.264815 hybridcontents-0.4.0/hybridcontents/tests/
+-rw-r--r--   0 john       (501) staff       (20)        0 2023-05-16 01:44:05.000000 hybridcontents-0.4.0/hybridcontents/tests/__init__.py
+-rw-r--r--   0 john       (501) staff       (20)    12399 2023-05-16 01:44:05.000000 hybridcontents-0.4.0/hybridcontents/tests/test_hybrid_manager.py
+-rw-r--r--   0 john       (501) staff       (20)      435 2023-05-16 01:44:05.000000 hybridcontents-0.4.0/hybridcontents/tests/testing_utils.py
+drwxr-xr-x   0 john       (501) staff       (20)        0 2023-05-16 01:51:58.264382 hybridcontents-0.4.0/hybridcontents.egg-info/
+-rw-r--r--   0 john       (501) staff       (20)     4465 2023-05-16 01:51:58.000000 hybridcontents-0.4.0/hybridcontents.egg-info/PKG-INFO
+-rw-r--r--   0 john       (501) staff       (20)      511 2023-05-16 01:51:58.000000 hybridcontents-0.4.0/hybridcontents.egg-info/SOURCES.txt
+-rw-r--r--   0 john       (501) staff       (20)        1 2023-05-16 01:51:58.000000 hybridcontents-0.4.0/hybridcontents.egg-info/dependency_links.txt
+-rw-r--r--   0 john       (501) staff       (20)      114 2023-05-16 01:51:58.000000 hybridcontents-0.4.0/hybridcontents.egg-info/requires.txt
+-rw-r--r--   0 john       (501) staff       (20)       15 2023-05-16 01:51:58.000000 hybridcontents-0.4.0/hybridcontents.egg-info/top_level.txt
+-rw-r--r--   0 john       (501) staff       (20)        1 2023-05-16 01:51:45.000000 hybridcontents-0.4.0/hybridcontents.egg-info/zip-safe
+-rw-r--r--   0 john       (501) staff       (20)       30 2023-05-16 01:44:05.000000 hybridcontents-0.4.0/requirements.txt
+-rw-r--r--   0 john       (501) staff       (20)       88 2023-05-16 01:44:05.000000 hybridcontents-0.4.0/requirements_test.txt
+-rw-r--r--   0 john       (501) staff       (20)       79 2023-05-16 01:51:58.265252 hybridcontents-0.4.0/setup.cfg
+-rw-r--r--   0 john       (501) staff       (20)     1832 2023-05-16 01:44:05.000000 hybridcontents-0.4.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `hybridcontents-0.3.0/PKG-INFO` & `hybridcontents-0.4.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,120 +1,122 @@
 Metadata-Version: 2.1
 Name: hybridcontents
-Version: 0.3.0
+Version: 0.4.0
 Summary: Hybrid Content Manager
 Home-page: https://github.com/viaduct-ai/hybridcontents
+Download-URL: https://github.com/viaduct-ai/hybridcontents/archive/v0.4.0.tar.gz
 Author: viaduct
 Author-email: engineering@viaduct.ai
 License: Apache 2.0
-Download-URL: https://github.com/viaduct-ai/hybridcontents/archive/v0.3.0.tar.gz
-Description: HybridContents
-        ======================
-        
-        The `HybridContentManager` was originally created by [Quantopian](https://www.quantopian.com/) as part of [pgcontents](https://github.com/quantopian/pgcontents); however, the usage of `HybridContentsManager` was restricted to the compatibility requirements of [pgcontents](https://github.com/quantopian/pgcontents). These restrictions included `postgres` dependencies and no support for the latest [notebook](https://pypi.org/project/notebook/) version (>6).
-        
-        At [Viaduct](https://viaduct.ai) we used [pgcontents](https://github.com/quantopian/pgcontents) exclusively for the `HybridContentsManager` and wanted to extend its functionality, so we created this fork [hybridcontents](https://github.com/viaduct-ai/hybridcontents).
-        
-        See related [pgcontents](https://github.com/quantopian/pgcontents) issues:
-        - https://github.com/quantopian/pgcontents/issues/66
-        - https://github.com/quantopian/pgcontents/issues/50
-        - https://github.com/quantopian/pgcontents/issues/28
-        
-        Getting Started
-        ---------------
-        **Prerequisites:**
-         - A Python installation with [Jupyter Notebook](https://github.com/jupyter/notebook) >= 4.0.
-        
-        **Installation:**
-        
-        #### [pip](https://pypi.org/project/hybridcontents/)
-        ```bash
-        pip install hybridcontents
-        ```
-        #### [Anaconda](https://anaconda.org/viaduct/hybridcontents)
-        ```bash
-        conda install -c viaduct hybridcontents
-        ```
-        #### [conda-forge](https://github.com/conda-forge/hybridcontents-feedstock)
-        See instructions [here](https://github.com/conda-forge/hybridcontents-feedstock#installing-hybridcontents)
-        
-        Featues
-        -----
-        - Mix and match different content managers for different directories 
-        - Easily move files between different content managers (i.e local files to s3 backed manager) 
-        - Path validation to keep consistent naming scheme and/or prevent illegal characters
-        
-        Usage
-        -----
-        For a detailed example see, [hybrid_manager_example.py](https://github.com/viaduct-ai/hybridcontents/blob/master/examples/hybrid_manager_example.py)
-        
-        The following code snippet creates a HybridContentsManager with two directories with different content managers. 
-        
-        ```python
-        c = get_config()
-        
-        c.NotebookApp.contents_manager_class = HybridContentsManager
-        
-        c.HybridContentsManager.manager_classes = {
-            "": FileContentsManager,
-            "shared": S3ContentsManager
-        }
-        
-        # Each item will be passed to the constructor of the appropriate content manager.
-        c.HybridContentsManager.manager_kwargs = {
-            # Args for root FileContentsManager
-            "": {
-                "root_dir": read_only_dir
-            },
-            # Args for the shared S3ContentsManager directory
-            "shared": {
-                "access_key_id": ...,
-                "secret_access_key": ...,
-                "endpoint_url":  ...,
-                "bucket": ...,
-                "prefix": ...
-            },
-        }
-        
-        def only_allow_notebooks(path):
-          return path.endswith('.ipynb')
-        
-        # Only allow notebook files to be stored in S3
-        c.HybridContentsManager.path_validators = {
-            "shared": only_allow_notebooks
-        }
-        ```
-        
-        
-        Testing
-        -------
-        To run unit tests, 
-        
-        ```bash
-        tox
-        ```
-        
-        This will run all unit tests for python versions 2.7, 3.6, 3.7 and jupyter notebook versions 4, 5, and 6.
-        
-        ### Publishing a Release
-        
-        1. Create a new release on Github
-        2. Update the version in `setup.py`
-        3. Run ./scripts/pip_publish.sh
-        4. Update the version `meta.yaml`
-        5. Update the [sha256 in meta.yaml](https://github.com/conda-forge/staged-recipes/wiki/Frequently-asked-questions#2-how-do-i-populate-the-hash-field)
-        6. Run ./scripts/anaconda_publish.sh
-        7. Update on Conda Forge
-        
 Keywords: jupyterhub,pgcontents,hybridcontents,content manager,hybridcontentmanager
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: IPython
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 Provides-Extra: test
+License-File: LICENSE
+
+HybridContents
+======================
+
+The `HybridContentManager` was originally created by [Quantopian](https://www.quantopian.com/) as part of [pgcontents](https://github.com/quantopian/pgcontents); however, the usage of `HybridContentsManager` was restricted to the compatibility requirements of [pgcontents](https://github.com/quantopian/pgcontents). These restrictions included `postgres` dependencies and no support for the latest [notebook](https://pypi.org/project/notebook/) version (>6).
+
+At [Viaduct](https://viaduct.ai) we used [pgcontents](https://github.com/quantopian/pgcontents) exclusively for the `HybridContentsManager` and wanted to extend its functionality, so we created this fork [hybridcontents](https://github.com/viaduct-ai/hybridcontents).
+
+See related [pgcontents](https://github.com/quantopian/pgcontents) issues:
+- https://github.com/quantopian/pgcontents/issues/66
+- https://github.com/quantopian/pgcontents/issues/50
+- https://github.com/quantopian/pgcontents/issues/28
+
+Getting Started
+---------------
+**Prerequisites:**
+ - A Python installation with [Jupyter Notebook](https://github.com/jupyter/notebook) >= 4.0.
+
+**Installation:**
+
+#### [pip](https://pypi.org/project/hybridcontents/)
+```bash
+pip install hybridcontents
+```
+#### [Anaconda](https://anaconda.org/viaduct/hybridcontents)
+```bash
+conda install -c viaduct hybridcontents
+```
+#### [conda-forge](https://github.com/conda-forge/hybridcontents-feedstock)
+See instructions [here](https://github.com/conda-forge/hybridcontents-feedstock#installing-hybridcontents)
+
+Features
+-----
+- Mix and match different content managers for different directories 
+- Easily move files between different content managers (i.e local files to s3 backed manager) 
+- Path validation to keep consistent naming scheme and/or prevent illegal characters
+
+Usage
+-----
+For a detailed example see, [hybrid_manager_example.py](https://github.com/viaduct-ai/hybridcontents/blob/master/examples/hybrid_manager_example.py)
+
+The following code snippet creates a HybridContentsManager with two directories with different content managers. 
+
+```python
+c = get_config()
+
+c.NotebookApp.contents_manager_class = HybridContentsManager
+
+c.HybridContentsManager.manager_classes = {
+    # NOTE: LargFileManager only exists in notebook > 5
+    # If using notebook < 5, use FileContentManager instead
+    "": LargeFileManager,
+    "shared": S3ContentsManager
+}
+
+# Each item will be passed to the constructor of the appropriate content manager.
+c.HybridContentsManager.manager_kwargs = {
+    # Args for root LargeFileManager
+    "": {
+        "root_dir": read_only_dir
+    },
+    # Args for the shared S3ContentsManager directory
+    "shared": {
+        "access_key_id": ...,
+        "secret_access_key": ...,
+        "endpoint_url":  ...,
+        "bucket": ...,
+        "prefix": ...
+    },
+}
+
+def only_allow_notebooks(path):
+  return path.endswith('.ipynb')
+
+# Only allow notebook files to be stored in S3
+c.HybridContentsManager.path_validators = {
+    "shared": only_allow_notebooks
+}
+```
+
+
+Testing
+-------
+To run unit tests, 
+
+```bash
+tox
+```
+
+This will run all unit tests for python versions 2.7, 3.6, 3.7 and jupyter notebook versions 4, 5, and 6.
+
+### Publishing a Release
+
+1. Create a new release on Github
+2. Update the version in `setup.py`
+3. Run ./scripts/pip_publish.sh
+4. Update the version `meta.yaml`
+5. Update the [sha256 in meta.yaml](https://github.com/conda-forge/staged-recipes/wiki/Frequently-asked-questions#2-how-do-i-populate-the-hash-field)
+6. Run ./scripts/anaconda_publish.sh
+7. Update on Conda Forge
```

### Comparing `hybridcontents-0.3.0/LICENSE` & `hybridcontents-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hybridcontents-0.3.0/README.md` & `hybridcontents-0.4.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #### [Anaconda](https://anaconda.org/viaduct/hybridcontents)
 ```bash
 conda install -c viaduct hybridcontents
 ```
 #### [conda-forge](https://github.com/conda-forge/hybridcontents-feedstock)
 See instructions [here](https://github.com/conda-forge/hybridcontents-feedstock#installing-hybridcontents)
 
-Featues
+Features
 -----
 - Mix and match different content managers for different directories 
 - Easily move files between different content managers (i.e local files to s3 backed manager) 
 - Path validation to keep consistent naming scheme and/or prevent illegal characters
 
 Usage
 -----
@@ -42,21 +42,23 @@
 
 ```python
 c = get_config()
 
 c.NotebookApp.contents_manager_class = HybridContentsManager
 
 c.HybridContentsManager.manager_classes = {
-    "": FileContentsManager,
+    # NOTE: LargFileManager only exists in notebook > 5
+    # If using notebook < 5, use FileContentManager instead
+    "": LargeFileManager,
     "shared": S3ContentsManager
 }
 
 # Each item will be passed to the constructor of the appropriate content manager.
 c.HybridContentsManager.manager_kwargs = {
-    # Args for root FileContentsManager
+    # Args for root LargeFileManager
     "": {
         "root_dir": read_only_dir
     },
     # Args for the shared S3ContentsManager directory
     "shared": {
         "access_key_id": ...,
         "secret_access_key": ...,
```

### Comparing `hybridcontents-0.3.0/hybridcontents/tests/test_hybrid_manager.py` & `hybridcontents-0.4.0/hybridcontents/tests/test_hybrid_manager.py`

 * *Files identical despite different names*

### Comparing `hybridcontents-0.3.0/hybridcontents/hybridmanager.py` & `hybridcontents-0.4.0/hybridcontents/hybridmanager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,24 @@
 """Multi-backend ContentsManager."""
 from __future__ import unicode_literals
 
 from six import iteritems
 from tornado.web import HTTPError
 
-from notebook.services.contents.manager import ContentsManager
+# Ref. https://github.com/jupyter/nbdime/blob/c82362344e596efdc4f54c927d90338940e0fa41/nbdime/webapp/nb_server_extension.py#L16-L33
+# This allows solving conflicts between the class import from either notebook or jupyter_server
+try:
+    from notebook.services.contents.manager import ContentsManager
+except ModuleNotFoundError:
+    pass
+
+try:
+    from jupyter_server.services.contents.manager import ContentsManager
+except ModuleNotFoundError:
+    pass
 
 from traitlets import Dict
 
 from .api_utils import (
     base_directory_model,
     normalize_api_path,
     outside_root_to_404,
@@ -118,42 +128,14 @@
             return _apply_prefix(prefix, result)
         else:
             return result
 
     return _wrapper
 
 
-def path_dispatch_old_new(mname, returns_model):
-    """Decorator for methods accepting old_path and new_path."""
-    def _wrapper(self, old_path, new_path, *args, **kwargs):
-        old_prefix, old_mgr, old_mgr_path = _resolve_path(
-            old_path, self.managers)
-        new_prefix, new_mgr, new_mgr_path = _resolve_path(
-            new_path,
-            self.managers,
-        )
-        if old_mgr is not new_mgr:
-            # TODO: Consider supporting this via get+delete+save.
-            raise HTTPError(
-                400,
-                "Can't move files between backends ({old} -> {new})".format(
-                    old=old_path,
-                    new=new_path,
-                ))
-        assert new_prefix == old_prefix
-        result = getattr(new_mgr, mname)(old_mgr_path, new_mgr_path, *args,
-                                         **kwargs)
-        if returns_model and new_prefix:
-            return _apply_prefix(new_prefix, result)
-        else:
-            return result
-
-    return _wrapper
-
-
 def DEFAULT_PATH_VALIDATOR(path):
     return True
 
 
 class HybridContentsManager(ContentsManager):
     """ContentsManager subclass that delegates specific subdirectories to other
     ContentsManager/Checkpoints pairs."""
```

### Comparing `hybridcontents-0.3.0/hybridcontents/api_utils.py` & `hybridcontents-0.4.0/hybridcontents/api_utils.py`

 * *Files identical despite different names*

### Comparing `hybridcontents-0.3.0/setup.py` & `hybridcontents-0.4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 from os.path import join, dirname, abspath
 
 long_description = open('README.md').read()
 
-version = '0.3.0'
+version = '0.4.0'
 
 
 def read_requirements(basename):
     reqs_file = join(dirname(abspath(__file__)), basename)
     with open(reqs_file) as f:
         return [req.strip() for req in f.readlines()]
```

### Comparing `hybridcontents-0.3.0/hybridcontents.egg-info/PKG-INFO` & `hybridcontents-0.4.0/hybridcontents.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,120 +1,122 @@
 Metadata-Version: 2.1
 Name: hybridcontents
-Version: 0.3.0
+Version: 0.4.0
 Summary: Hybrid Content Manager
 Home-page: https://github.com/viaduct-ai/hybridcontents
+Download-URL: https://github.com/viaduct-ai/hybridcontents/archive/v0.4.0.tar.gz
 Author: viaduct
 Author-email: engineering@viaduct.ai
 License: Apache 2.0
-Download-URL: https://github.com/viaduct-ai/hybridcontents/archive/v0.3.0.tar.gz
-Description: HybridContents
-        ======================
-        
-        The `HybridContentManager` was originally created by [Quantopian](https://www.quantopian.com/) as part of [pgcontents](https://github.com/quantopian/pgcontents); however, the usage of `HybridContentsManager` was restricted to the compatibility requirements of [pgcontents](https://github.com/quantopian/pgcontents). These restrictions included `postgres` dependencies and no support for the latest [notebook](https://pypi.org/project/notebook/) version (>6).
-        
-        At [Viaduct](https://viaduct.ai) we used [pgcontents](https://github.com/quantopian/pgcontents) exclusively for the `HybridContentsManager` and wanted to extend its functionality, so we created this fork [hybridcontents](https://github.com/viaduct-ai/hybridcontents).
-        
-        See related [pgcontents](https://github.com/quantopian/pgcontents) issues:
-        - https://github.com/quantopian/pgcontents/issues/66
-        - https://github.com/quantopian/pgcontents/issues/50
-        - https://github.com/quantopian/pgcontents/issues/28
-        
-        Getting Started
-        ---------------
-        **Prerequisites:**
-         - A Python installation with [Jupyter Notebook](https://github.com/jupyter/notebook) >= 4.0.
-        
-        **Installation:**
-        
-        #### [pip](https://pypi.org/project/hybridcontents/)
-        ```bash
-        pip install hybridcontents
-        ```
-        #### [Anaconda](https://anaconda.org/viaduct/hybridcontents)
-        ```bash
-        conda install -c viaduct hybridcontents
-        ```
-        #### [conda-forge](https://github.com/conda-forge/hybridcontents-feedstock)
-        See instructions [here](https://github.com/conda-forge/hybridcontents-feedstock#installing-hybridcontents)
-        
-        Featues
-        -----
-        - Mix and match different content managers for different directories 
-        - Easily move files between different content managers (i.e local files to s3 backed manager) 
-        - Path validation to keep consistent naming scheme and/or prevent illegal characters
-        
-        Usage
-        -----
-        For a detailed example see, [hybrid_manager_example.py](https://github.com/viaduct-ai/hybridcontents/blob/master/examples/hybrid_manager_example.py)
-        
-        The following code snippet creates a HybridContentsManager with two directories with different content managers. 
-        
-        ```python
-        c = get_config()
-        
-        c.NotebookApp.contents_manager_class = HybridContentsManager
-        
-        c.HybridContentsManager.manager_classes = {
-            "": FileContentsManager,
-            "shared": S3ContentsManager
-        }
-        
-        # Each item will be passed to the constructor of the appropriate content manager.
-        c.HybridContentsManager.manager_kwargs = {
-            # Args for root FileContentsManager
-            "": {
-                "root_dir": read_only_dir
-            },
-            # Args for the shared S3ContentsManager directory
-            "shared": {
-                "access_key_id": ...,
-                "secret_access_key": ...,
-                "endpoint_url":  ...,
-                "bucket": ...,
-                "prefix": ...
-            },
-        }
-        
-        def only_allow_notebooks(path):
-          return path.endswith('.ipynb')
-        
-        # Only allow notebook files to be stored in S3
-        c.HybridContentsManager.path_validators = {
-            "shared": only_allow_notebooks
-        }
-        ```
-        
-        
-        Testing
-        -------
-        To run unit tests, 
-        
-        ```bash
-        tox
-        ```
-        
-        This will run all unit tests for python versions 2.7, 3.6, 3.7 and jupyter notebook versions 4, 5, and 6.
-        
-        ### Publishing a Release
-        
-        1. Create a new release on Github
-        2. Update the version in `setup.py`
-        3. Run ./scripts/pip_publish.sh
-        4. Update the version `meta.yaml`
-        5. Update the [sha256 in meta.yaml](https://github.com/conda-forge/staged-recipes/wiki/Frequently-asked-questions#2-how-do-i-populate-the-hash-field)
-        6. Run ./scripts/anaconda_publish.sh
-        7. Update on Conda Forge
-        
 Keywords: jupyterhub,pgcontents,hybridcontents,content manager,hybridcontentmanager
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: IPython
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 Provides-Extra: test
+License-File: LICENSE
+
+HybridContents
+======================
+
+The `HybridContentManager` was originally created by [Quantopian](https://www.quantopian.com/) as part of [pgcontents](https://github.com/quantopian/pgcontents); however, the usage of `HybridContentsManager` was restricted to the compatibility requirements of [pgcontents](https://github.com/quantopian/pgcontents). These restrictions included `postgres` dependencies and no support for the latest [notebook](https://pypi.org/project/notebook/) version (>6).
+
+At [Viaduct](https://viaduct.ai) we used [pgcontents](https://github.com/quantopian/pgcontents) exclusively for the `HybridContentsManager` and wanted to extend its functionality, so we created this fork [hybridcontents](https://github.com/viaduct-ai/hybridcontents).
+
+See related [pgcontents](https://github.com/quantopian/pgcontents) issues:
+- https://github.com/quantopian/pgcontents/issues/66
+- https://github.com/quantopian/pgcontents/issues/50
+- https://github.com/quantopian/pgcontents/issues/28
+
+Getting Started
+---------------
+**Prerequisites:**
+ - A Python installation with [Jupyter Notebook](https://github.com/jupyter/notebook) >= 4.0.
+
+**Installation:**
+
+#### [pip](https://pypi.org/project/hybridcontents/)
+```bash
+pip install hybridcontents
+```
+#### [Anaconda](https://anaconda.org/viaduct/hybridcontents)
+```bash
+conda install -c viaduct hybridcontents
+```
+#### [conda-forge](https://github.com/conda-forge/hybridcontents-feedstock)
+See instructions [here](https://github.com/conda-forge/hybridcontents-feedstock#installing-hybridcontents)
+
+Features
+-----
+- Mix and match different content managers for different directories 
+- Easily move files between different content managers (i.e local files to s3 backed manager) 
+- Path validation to keep consistent naming scheme and/or prevent illegal characters
+
+Usage
+-----
+For a detailed example see, [hybrid_manager_example.py](https://github.com/viaduct-ai/hybridcontents/blob/master/examples/hybrid_manager_example.py)
+
+The following code snippet creates a HybridContentsManager with two directories with different content managers. 
+
+```python
+c = get_config()
+
+c.NotebookApp.contents_manager_class = HybridContentsManager
+
+c.HybridContentsManager.manager_classes = {
+    # NOTE: LargFileManager only exists in notebook > 5
+    # If using notebook < 5, use FileContentManager instead
+    "": LargeFileManager,
+    "shared": S3ContentsManager
+}
+
+# Each item will be passed to the constructor of the appropriate content manager.
+c.HybridContentsManager.manager_kwargs = {
+    # Args for root LargeFileManager
+    "": {
+        "root_dir": read_only_dir
+    },
+    # Args for the shared S3ContentsManager directory
+    "shared": {
+        "access_key_id": ...,
+        "secret_access_key": ...,
+        "endpoint_url":  ...,
+        "bucket": ...,
+        "prefix": ...
+    },
+}
+
+def only_allow_notebooks(path):
+  return path.endswith('.ipynb')
+
+# Only allow notebook files to be stored in S3
+c.HybridContentsManager.path_validators = {
+    "shared": only_allow_notebooks
+}
+```
+
+
+Testing
+-------
+To run unit tests, 
+
+```bash
+tox
+```
+
+This will run all unit tests for python versions 2.7, 3.6, 3.7 and jupyter notebook versions 4, 5, and 6.
+
+### Publishing a Release
+
+1. Create a new release on Github
+2. Update the version in `setup.py`
+3. Run ./scripts/pip_publish.sh
+4. Update the version `meta.yaml`
+5. Update the [sha256 in meta.yaml](https://github.com/conda-forge/staged-recipes/wiki/Frequently-asked-questions#2-how-do-i-populate-the-hash-field)
+6. Run ./scripts/anaconda_publish.sh
+7. Update on Conda Forge
```

