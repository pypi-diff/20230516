# Comparing `tmp/python-backpack-1.0.4.tar.gz` & `tmp/python-backpack-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-backpack-1.0.4.tar", last modified: Sat Apr 15 02:51:05 2023, max compression
+gzip compressed data, was "python-backpack-1.0.5.tar", last modified: Tue May 16 02:11:22 2023, max compression
```

## Comparing `python-backpack-1.0.4.tar` & `python-backpack-1.0.5.tar`

### file list

```diff
@@ -1,36 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 02:51:05.762869 python-backpack-1.0.4/
--rw-rw-rw-   0        0        0    35823 2022-07-19 16:09:57.000000 python-backpack-1.0.4/LICENSE
--rw-rw-rw-   0        0        0       19 2021-03-12 21:28:06.000000 python-backpack-1.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     2335 2023-04-15 02:51:05.761868 python-backpack-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1616 2023-04-14 23:58:08.000000 python-backpack-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-15 02:51:05.737869 python-backpack-1.0.4/backpack/
--rw-rw-rw-   0        0        0        0 2022-07-03 20:54:02.000000 python-backpack-1.0.4/backpack/__init__.py
--rw-rw-rw-   0        0        0     1275 2022-07-19 17:22:54.000000 python-backpack-1.0.4/backpack/custom_errors.py
--rw-rw-rw-   0        0        0     2483 2022-07-23 02:55:46.000000 python-backpack-1.0.4/backpack/file_utils.py
--rw-rw-rw-   0        0        0     2957 2022-07-20 01:30:36.000000 python-backpack-1.0.4/backpack/folder_utils.py
--rw-rw-rw-   0        0        0     5108 2022-07-24 17:39:20.000000 python-backpack-1.0.4/backpack/json_metadata.py
--rw-rw-rw-   0        0        0     2484 2023-04-15 02:37:12.000000 python-backpack-1.0.4/backpack/json_user_settings.py
--rw-rw-rw-   0        0        0     1227 2022-07-24 18:24:48.000000 python-backpack-1.0.4/backpack/json_utils.py
--rw-rw-rw-   0        0        0      464 2022-07-19 23:08:20.000000 python-backpack-1.0.4/backpack/logger.py
--rw-rw-rw-   0        0        0      848 2022-07-23 17:23:26.000000 python-backpack-1.0.4/backpack/patterns.py
--rw-rw-rw-   0        0        0     3289 2023-04-15 02:16:46.000000 python-backpack-1.0.4/backpack/strings.py
--rw-rw-rw-   0        0        0     1135 2022-07-20 15:08:27.000000 python-backpack-1.0.4/backpack/test_utils.py
--rw-rw-rw-   0        0        0      523 2023-04-14 23:50:49.000000 python-backpack-1.0.4/backpack/version.py
-drwxrwxrwx   0        0        0        0 2023-04-15 02:51:05.751869 python-backpack-1.0.4/python_backpack.egg-info/
--rw-rw-rw-   0        0        0     2335 2023-04-15 02:51:05.000000 python-backpack-1.0.4/python_backpack.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      708 2023-04-15 02:51:05.000000 python-backpack-1.0.4/python_backpack.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 02:51:05.000000 python-backpack-1.0.4/python_backpack.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-15 02:51:05.000000 python-backpack-1.0.4/python_backpack.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-15 02:51:05.762869 python-backpack-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1305 2023-04-15 02:50:08.000000 python-backpack-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-15 02:51:05.760869 python-backpack-1.0.4/tests/
--rw-rw-rw-   0        0        0        0 2021-01-19 15:17:59.000000 python-backpack-1.0.4/tests/__init__.py
--rw-rw-rw-   0        0        0     1580 2022-07-23 02:07:10.000000 python-backpack-1.0.4/tests/test_errors.py
--rw-rw-rw-   0        0        0     1836 2022-07-23 17:36:37.000000 python-backpack-1.0.4/tests/test_file_utils.py
--rw-rw-rw-   0        0        0     3123 2022-07-23 02:34:06.000000 python-backpack-1.0.4/tests/test_folder_utils.py
--rw-rw-rw-   0        0        0     2224 2023-04-15 02:45:26.000000 python-backpack-1.0.4/tests/test_json_user_settings.py
--rw-rw-rw-   0        0        0     1616 2022-07-24 18:25:31.000000 python-backpack-1.0.4/tests/test_json_utils.py
--rw-rw-rw-   0        0        0     2546 2022-07-24 18:14:15.000000 python-backpack-1.0.4/tests/test_jsonmd.py
--rw-rw-rw-   0        0        0     1675 2022-07-23 17:21:54.000000 python-backpack-1.0.4/tests/test_misc.py
--rw-rw-rw-   0        0        0     3704 2023-04-15 02:13:42.000000 python-backpack-1.0.4/tests/test_strings.py
--rw-rw-rw-   0        0        0     1191 2022-07-20 15:08:43.000000 python-backpack-1.0.4/tests/test_test_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-16 02:11:22.648473 python-backpack-1.0.5/
+-rw-rw-rw-   0        0        0    35823 2022-07-19 16:09:57.000000 python-backpack-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0       19 2021-03-12 21:28:06.000000 python-backpack-1.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     2511 2023-05-16 02:11:22.647473 python-backpack-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1653 2023-05-14 20:40:18.000000 python-backpack-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-16 02:11:22.628468 python-backpack-1.0.5/backpack/
+-rw-rw-rw-   0        0        0        0 2022-07-03 20:54:02.000000 python-backpack-1.0.5/backpack/__init__.py
+-rw-rw-rw-   0        0        0     2219 2023-05-14 23:51:20.000000 python-backpack-1.0.5/backpack/cache.py
+-rw-rw-rw-   0        0        0     1268 2023-05-14 20:16:03.000000 python-backpack-1.0.5/backpack/custom_errors.py
+-rw-rw-rw-   0        0        0     2519 2023-05-14 20:17:43.000000 python-backpack-1.0.5/backpack/file_utils.py
+-rw-rw-rw-   0        0        0     2975 2023-05-14 20:17:45.000000 python-backpack-1.0.5/backpack/folder_utils.py
+-rw-rw-rw-   0        0        0     4599 2023-05-14 22:32:10.000000 python-backpack-1.0.5/backpack/json_metadata.py
+-rw-rw-rw-   0        0        0     2539 2023-05-14 20:36:49.000000 python-backpack-1.0.5/backpack/json_user_settings.py
+-rw-rw-rw-   0        0        0     1301 2023-05-14 20:37:15.000000 python-backpack-1.0.5/backpack/json_utils.py
+-rw-rw-rw-   0        0        0      464 2022-07-19 23:08:20.000000 python-backpack-1.0.5/backpack/logger.py
+-rw-rw-rw-   0        0        0      848 2022-07-23 17:23:26.000000 python-backpack-1.0.5/backpack/patterns.py
+-rw-rw-rw-   0        0        0     3289 2023-04-15 02:16:46.000000 python-backpack-1.0.5/backpack/strings.py
+-rw-rw-rw-   0        0        0     1165 2023-05-14 20:38:38.000000 python-backpack-1.0.5/backpack/test_utils.py
+-rw-rw-rw-   0        0        0      607 2023-05-14 20:37:47.000000 python-backpack-1.0.5/backpack/version.py
+drwxrwxrwx   0        0        0        0 2023-05-16 02:11:22.639471 python-backpack-1.0.5/python_backpack.egg-info/
+-rw-rw-rw-   0        0        0     2511 2023-05-16 02:11:22.000000 python-backpack-1.0.5/python_backpack.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      746 2023-05-16 02:11:22.000000 python-backpack-1.0.5/python_backpack.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 02:11:22.000000 python-backpack-1.0.5/python_backpack.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-16 02:11:22.000000 python-backpack-1.0.5/python_backpack.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-16 02:11:22.648473 python-backpack-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1281 2023-05-16 02:11:19.000000 python-backpack-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 02:11:22.646472 python-backpack-1.0.5/tests/
+-rw-rw-rw-   0        0        0        0 2021-01-19 15:17:59.000000 python-backpack-1.0.5/tests/__init__.py
+-rw-rw-rw-   0        0        0      888 2023-05-14 22:36:35.000000 python-backpack-1.0.5/tests/test_cache.py
+-rw-rw-rw-   0        0        0     1580 2022-07-23 02:07:10.000000 python-backpack-1.0.5/tests/test_errors.py
+-rw-rw-rw-   0        0        0     1836 2022-07-23 17:36:37.000000 python-backpack-1.0.5/tests/test_file_utils.py
+-rw-rw-rw-   0        0        0     3123 2022-07-23 02:34:06.000000 python-backpack-1.0.5/tests/test_folder_utils.py
+-rw-rw-rw-   0        0        0     2224 2023-04-15 02:45:26.000000 python-backpack-1.0.5/tests/test_json_user_settings.py
+-rw-rw-rw-   0        0        0     1616 2022-07-24 18:25:31.000000 python-backpack-1.0.5/tests/test_json_utils.py
+-rw-rw-rw-   0        0        0     2551 2023-05-14 22:31:13.000000 python-backpack-1.0.5/tests/test_jsonmd.py
+-rw-rw-rw-   0        0        0     1675 2022-07-23 17:21:54.000000 python-backpack-1.0.5/tests/test_misc.py
+-rw-rw-rw-   0        0        0     3704 2023-04-15 02:13:42.000000 python-backpack-1.0.5/tests/test_strings.py
+-rw-rw-rw-   0        0        0     1191 2022-07-20 15:08:43.000000 python-backpack-1.0.5/tests/test_test_utils.py
```

### Comparing `python-backpack-1.0.4/LICENSE` & `python-backpack-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `python-backpack-1.0.4/PKG-INFO` & `python-backpack-1.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 Metadata-Version: 2.1
 Name: python-backpack
-Version: 1.0.4
-Summary: Python Utilities for json/files/strings/errors
+Version: 1.0.5
+Summary: Python Utilities
 Home-page: https://github.com/MaxRocamora/python-backpack
 Author: Maximiliano Rocamora
 Author-email: maxirocamora@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
+Project-URL: Source, https://github.com/MaxRocamora/python-backpack
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: Freely Distributable
+Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-
 [![PyPI Supported Python Versions](https://img.shields.io/pypi/pyversions/python-backpack.svg?style=flat-square&logo=appveyor)](https://pypi.python.org/pypi/python-backpack/)
 [![PyPI version](https://badge.fury.io/py/python-backpack.svg?style=flat-square&logo=appveyor)](https://badge.fury.io/py/python-backpack)
 [![GitHub version](https://badge.fury.io/gh/MaxRocamora%2Fpython-backpack.svg?style=flat-square&logo=appveyor)](https://badge.fury.io/gh/MaxRocamora%2Fpython-backpack)
 [![codecov](https://codecov.io/gh/MaxRocamora/python-backpack/branch/main/graph/badge.svg?token=6D1xwYdXW2)](https://codecov.io/gh/MaxRocamora/python-backpack)
 [![Message](https://img.shields.io/badge/python--backpack-python-blue?style=flat-square&logo=appveyor)](https://github.com/MaxRocamora/python-backpack)
 
 
 # Python-Backpack
-A collection of personal scripts for JSON, File/Folder Operations, String Validation, Custom Errors, and stuff.  
+A collection of personal scripts for JSON, File/Folder Operations, String Validation, Custom Errors, Cache and stuff.  
 
 
 ## Json
 + json_load()
 + json_save()
 + jsonMetaFile()
 + jsonUserSettings()
@@ -52,14 +53,17 @@
 + has_numbers()
 + camelcase_to_snakecase()
 
 ## Custom Errors
 + EnvironmentVariableNotFound()
 + ApplicationNotFound()
 
+## Cache
++ timed_lru_cache
+
 ## Test Utils
 + time_function_decorator()
 + random_string()
 
 ## Others / Patterns
 + Singleton()
```

### Comparing `python-backpack-1.0.4/README.md` & `python-backpack-1.0.5/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [![PyPI version](https://badge.fury.io/py/python-backpack.svg?style=flat-square&logo=appveyor)](https://badge.fury.io/py/python-backpack)
 [![GitHub version](https://badge.fury.io/gh/MaxRocamora%2Fpython-backpack.svg?style=flat-square&logo=appveyor)](https://badge.fury.io/gh/MaxRocamora%2Fpython-backpack)
 [![codecov](https://codecov.io/gh/MaxRocamora/python-backpack/branch/main/graph/badge.svg?token=6D1xwYdXW2)](https://codecov.io/gh/MaxRocamora/python-backpack)
 [![Message](https://img.shields.io/badge/python--backpack-python-blue?style=flat-square&logo=appveyor)](https://github.com/MaxRocamora/python-backpack)
 
 
 # Python-Backpack
-A collection of personal scripts for JSON, File/Folder Operations, String Validation, Custom Errors, and stuff.  
+A collection of personal scripts for JSON, File/Folder Operations, String Validation, Custom Errors, Cache and stuff.  
 
 
 ## Json
 + json_load()
 + json_save()
 + jsonMetaFile()
 + jsonUserSettings()
@@ -32,14 +32,17 @@
 + has_numbers()
 + camelcase_to_snakecase()
 
 ## Custom Errors
 + EnvironmentVariableNotFound()
 + ApplicationNotFound()
 
+## Cache
++ timed_lru_cache
+
 ## Test Utils
 + time_function_decorator()
 + random_string()
 
 ## Others / Patterns
 + Singleton()
```

### Comparing `python-backpack-1.0.4/backpack/custom_errors.py` & `python-backpack-1.0.5/backpack/custom_errors.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     def __init__(self, var_name: str) -> None:
         '''Error Raised when a required environment variable is missing from os.
 
         Args:
             var_name (str): name of the required variable missing
         '''
         self.var_name = var_name
-        self.message = f'System required ({var_name}) Environment Variable not found.'
+        self.message = f'Required Environment Variable [{var_name}] not found.'
         super().__init__(self.message)
 
     def __str__(self):
         return self.message
 
 
 class ApplicationNotFound(Exception):
```

### Comparing `python-backpack-1.0.4/backpack/file_utils.py` & `python-backpack-1.0.5/backpack/file_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 # https://github.com/MaxRocamora/python-backpack
 # ----------------------------------------------------------------------------------------
 
 import contextlib
 
 from backpack.logger import get_logger
 
-log = get_logger('FileUtils')
+log = get_logger('Python Backpack - FileUtils')
 
 
-def replace_strings_in_file(ascii_file: str, strings: list, new_string: str):
+def replace_strings_in_file(ascii_file: str, strings: list, new_string: str) -> None:
     ''' Opens ascii file and replaces all occurrences from strings into new_string.
     In this class we use a full path to avoid use of os.dirname, which
     causes string encode problems.
     Args:
         ascii_file (fullpath) file to open
         strings (list) strings to replace
         new_string (string) new string or path to set
@@ -36,15 +36,15 @@
 
     with open(ascii_file, 'w') as f:
         f.write(file_data)
         f.close()
         log.info(f"Closing File: {ascii_file}")
 
 
-def remove_line_from_file(ascii_file: str, strings: str):
+def remove_line_from_file(ascii_file: str, strings: str) -> None:
     ''' removes given lines from ascii file.
     Args:
         ascii_file (path) ASCII file to process
         strings (list) match lines to remove
     '''
 
     with open(ascii_file) as f:
@@ -70,8 +70,9 @@
     '''
     try:
         with open(filepath, 'r+') as _:
             return True
     except OSError as x:
         log.warning(f'{filepath} is locked ')
         log.info(x.strerror)
+
     return False
```

### Comparing `python-backpack-1.0.4/backpack/folder_utils.py` & `python-backpack-1.0.5/backpack/folder_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import os
 import shutil
 import subprocess
 
 from backpack.logger import get_logger
 
-log = get_logger('FolderUtils')
+log = get_logger('Python Backpack - FolderUtils')
 
 
 def browse_folder(folder: str) -> bool:
     ''' Open windows explorer on folder
     Args:
         folder (path) folder to open
     '''
```

### Comparing `python-backpack-1.0.4/backpack/json_metadata.py` & `python-backpack-1.0.5/backpack/json_metadata.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,146 +5,126 @@
 # ----------------------------------------------------------------------------------------
 import sys
 import os
 import time
 import inspect
 from datetime import datetime
 import platform
+from typing import Any
 
 from backpack.json_utils import json_load, json_save
 from backpack.version import version
 
 
 class JsonMetaFile():
 
-    def __init__(self, name: str, path: str):
+    PREFIX = "MD_"
+
+    def __init__(self, name: str, path: str) -> None:
         '''saves/load a class/dict as a json metadata file
 
         Args:
             name (str): name of the file/class
             path (str, optional): filepath. Defaults to None.
         '''
         self._name = name
         self._path = path
-        self._data = {}
-        self._data["_about"] = {'package': 'python-backpack',
-                                'version': self.version}
-
-    # ------------------------------------------------------------------------------------
-    # PROPERTIES
-    # ------------------------------------------------------------------------------------
+        self._data = {
+            "_about": {'package': 'python-backpack', 'version': self.version}
+        }
 
     @property
-    def name(self):
+    def name(self) -> str:
         ''' name of this metadata class'''
         return self._name
 
     @property
-    def version(self):
+    def version(self) -> str:
         ''' version of this metadata class'''
         return version
 
     @property
-    def data(self):
-        ''' stored metadata dict '''
-        return self._data
-
-    @data.setter
-    def data(self, val):
-        self._data = val
-
-    @property
-    def prefix(self):
-        ''' file prefix, is auto-included on the filename '''
-        return "MD_"
-
-    @property
-    def filename(self):
+    def filename(self) -> str:
         ''' Returns default filename with prefix and extension '''
-        return self.prefix + self.name + '.json'
+        return self.PREFIX + self.name + '.json'
 
     @property
-    def filepath(self):
+    def filepath(self) -> str:
         ''' full json metadata filepath '''
         return os.path.join(self.path, self.filename)
 
     @property
-    def path(self):
+    def path(self) -> str:
         ''' base path location of metadata json file '''
         return self._path
 
-    def has_file(self):
+    def has_file(self) -> bool:
+        ''' returns true if file exists '''
         return os.path.exists(self.filepath)
 
     # ------------------------------------------------------------------------------------
     # LOAD/INSERT/REMOVE/SAVE
     # ------------------------------------------------------------------------------------
 
-    def load(self):
+    def load(self) -> None:
         ''' loads metadata from disk '''
         self._data = json_load(self.filepath) if self.has_file() else {}
 
-    def insert(self, key, value):
+    def insert(self, key: str, value: Any) -> None:
         ''' inserts value into metadata '''
         self._data[key] = value
 
-    def remove(self, key):
+    def remove(self, key: str) -> None:
         ''' remove key from metadata '''
         if key in self._data.keys():
             del self._data[key]
 
-    def save(self, path: str = None):
-        ''' Save current metadata into json file.
-        Args:
-            path (str) sets target path for json file. Optional. Defaults to None
-        '''
+    def save(self) -> None:
+        ''' Save current metadata into json file. '''
         if not os.path.exists(self.path):
             os.makedirs(self.path)
 
-        self.data['system'] = self._system_data()
-        json_save(self.data, self.filepath)
+        self._data['system'] = self._system_data()
+        json_save(self._data, self.filepath)
 
     # ------------------------------------------------------------------------------------
     # CLASS MODE METHODS
     # ------------------------------------------------------------------------------------
 
-    def load_as_class(self):
+    def load_as_class(self) -> type:
         ''' returns the metadata dict as a class obj '''
         metadataClass = type(self.name, (), self._data)
         return metadataClass
 
-    def insert_class(self, _class):
-        ''' set class dict to data, data is cleared '''
-        self.data = self._attributes_from_class(_class)
-
-    def _attributes_from_class(self, _class):
+    def insert_class(self, _class: type) -> None:
+        ''' load all attributes from  a  given class into this class metadata '''
         attributes = {}
         for name in dir(_class):
             value = getattr(_class, name)
             if not name.startswith('__') and not inspect.ismethod(value):
                 attributes[name] = value
-        return attributes
+
+        self._data = attributes
 
     # ------------------------------------------------------------------------------------
     # SYSTEM METADATA OS/USER/TIME
     # ------------------------------------------------------------------------------------
 
-    def _system_data(self):
+    def _system_data(self) -> dict:
         ''' add system metadata to the default data before save '''
         return {
             'name': self.name,
             'app': os.path.basename(sys.executable),
             'PC': str(platform.node()),
             'python_version': sys.version,
             'User': str(os.getenv('username')),
-            'time': self._get_time_metadata,
+            'time': self._current_time_metadata(),
         }
 
-    @property
-    def _get_time_metadata(self):
+    def _current_time_metadata(self) -> dict:
         ''' Get export time info. '''
         ftime = time.strftime("%Y,%b,%d,%j,%H:%M", time.localtime())
         times = ftime.split(",")
         td = {
             "year": times[0],
             "month": times[1],
             "day": times[2],
```

### Comparing `python-backpack-1.0.4/backpack/json_user_settings.py` & `python-backpack-1.0.5/backpack/json_user_settings.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,79 +1,79 @@
-# -*- coding: utf-8 -*-
-# --------------------------------------------------------------------------------------------
+# ----------------------------------------------------------------------------------------
 # Json Settings Class
 # This class handle load/save json files on win/linux local user folder
 ''' Usage:
 us = JsonUserSettings('my_app')
 us.save(someDict)
 data = us.load()
 
 '''
-# --------------------------------------------------------------------------------------------
+# ----------------------------------------------------------------------------------------
 import os
 
 from backpack.logger import get_logger
 from backpack.json_utils import json_save, json_load
 
-log = get_logger('UserSettings')
+log = get_logger('Python Backpack - UserSettings')
 
 
 class JsonUserSettings():
-    def __init__(self, folder: str, name: str):
+    def __init__(self, folder: str, name: str) -> None:
         '''Manages saving/loading json file on local user folder
 
         Args:
             folder (str): name of sub folder inside user path. Defaults to 'json_settings'.
             filename (str): name used for the json file. Defaults to 'user_data'.
         '''
         self.name = name
         self.folder = folder
         self._user_data = {}
         self._verify_path()
 
     @property
-    def filepath(self):
+    def filepath(self) -> str:
         ''' Returns user filepath '''
-        path = os.path.join(self.os_user_folder, self.folder, self.name + '.json')
+        path = os.path.join(self.os_user_folder, self.folder, f'{self.name}.json')
         return os.path.abspath(path)
 
     @property
-    def os_user_folder(self):
+    def os_user_folder(self) -> str:
         ''' returns os users home directory '''
         return os.path.expanduser('~')
 
     @property
-    def user_data(self):
+    def user_data(self) -> dict:
         ''' override this property to modify saving dict '''
         return self._user_data
 
     @user_data.setter
-    def user_data(self, v):
+    def user_data(self, v: dict) -> None:
         self._user_data = v
 
-    def _verify_path(self):
+    def _verify_path(self) -> bool:
         ''' Checks for target directory or make it '''
         path = os.path.dirname(self.filepath)
         if not os.path.exists(path):
             os.makedirs(path)
+
         return True
 
-    def save_settings(self, data=False):
+    def save_settings(self, data=False) -> bool:
         ''' Saves a dictionary into a json file (os user path)
         Args:
             data (dictionary) : info dictionary to save, if set to False,
                 saves instead local self.user_data property
         '''
         if not data:
             data = self.user_data
 
         r = json_save(data, self.filepath)
         if r:
             log.info('json settings file saved! [%s]', self.filepath)
         return r
 
-    def load_settings(self):
+    def load_settings(self) -> dict:
         ''' Load json file from path and returns its contents '''
         try:
             return json_load(self.filepath)
         except OSError:
             return False
```

### Comparing `python-backpack-1.0.4/backpack/json_utils.py` & `python-backpack-1.0.5/backpack/json_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import json
 
 from backpack.logger import get_logger
 
-log = get_logger('JsonUtils')
+log = get_logger('Python Backpack - JsonUtils')
 
 
 def json_load(json_file: str) -> dict:
     ''' Reads a json file
     Args:
         json_file (filepath) json file to read data.
     Returns:
@@ -18,22 +18,25 @@
 
     with open(json_file) as json_file_opened:
         try:
             value = json.load(json_file_opened)
         except ValueError as e:
             json_file_opened.close()
             raise OSError(f"{json_file} \n JSON File issue: {str(e)}") from e
+
     return value
 
 
-def json_save(data: dict, json_file: str):
+def json_save(data: dict, json_file: str) -> bool:
     ''' Saves a dictionary into a json file
     Args:
         data (dict) : dictionary to save
         json_file (filepath) json file to save data.
+    Returns:
+        bool (True if success)
     '''
 
     if not os.path.exists(os.path.dirname(json_file)):
         os.makedirs(os.path.dirname(json_file))
 
     try:
         with open(json_file, 'w') as f:
```

### Comparing `python-backpack-1.0.4/backpack/patterns.py` & `python-backpack-1.0.5/backpack/patterns.py`

 * *Files identical despite different names*

### Comparing `python-backpack-1.0.4/backpack/strings.py` & `python-backpack-1.0.5/backpack/strings.py`

 * *Files identical despite different names*

### Comparing `python-backpack-1.0.4/backpack/test_utils.py` & `python-backpack-1.0.5/backpack/test_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # ----------------------------------------------------------------------------------------
 import time
 import random
 import string
 
 from backpack.logger import get_logger
 
-log = get_logger('TestUtils')
+log = get_logger('Python Backpack - TestUtils')
 
 
 def random_string(length: str = 10) -> str:
     '''Generates a random string of fixed length
 
     Args:
         length (int, optional): max string length. Defaults to 10.
@@ -22,18 +22,21 @@
         str: random string
     '''
 
     letters = string.ascii_lowercase
     return ''.join(random.choice(letters) for _ in range(length))
 
 
-def time_function_decorator(method):
+def time_function_decorator(method: type):
     ''' decorator to measure methods execution time '''
+
     def timed(*args, **kw):
         ts = time.time()
         result = method(*args, **kw)
         te = time.time()
 
         message = f'{method.__name__!r}  {(te - ts) * 1000:2.2f} ms'
         log.info(message)
+
         return result
+
     return timed
```

### Comparing `python-backpack-1.0.4/backpack/version.py` & `python-backpack-1.0.5/backpack/version.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # ----------------------------------------------------------------------------------------
 # 1.0.0 07/2022 - Initial Release
 # 1.0.2 07/2022 - More Methods and tests
 # 1.0.3 07/2022 - JsonMetaFile, JsonUserSettings
 # 1.0.4 04/2023 - Added camelcase_to_snakecase function
+# 1.0.5 05/2023 - Refactor JsonMetaFile, Added Cache, Some type hints / docstrings
 # ----------------------------------------------------------------------------------------
 
 VERSION_MAJOR = 1
 VERSION_MINOR = 0
-VERSION_PATCH = 4
+VERSION_PATCH = 5
 
 version = f'{VERSION_MAJOR}.{VERSION_MINOR}.{VERSION_PATCH}'
 
 app_name = 'python-backpack'
```

### Comparing `python-backpack-1.0.4/python_backpack.egg-info/PKG-INFO` & `python-backpack-1.0.5/python_backpack.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 Metadata-Version: 2.1
 Name: python-backpack
-Version: 1.0.4
-Summary: Python Utilities for json/files/strings/errors
+Version: 1.0.5
+Summary: Python Utilities
 Home-page: https://github.com/MaxRocamora/python-backpack
 Author: Maximiliano Rocamora
 Author-email: maxirocamora@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
+Project-URL: Source, https://github.com/MaxRocamora/python-backpack
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: Freely Distributable
+Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-
 [![PyPI Supported Python Versions](https://img.shields.io/pypi/pyversions/python-backpack.svg?style=flat-square&logo=appveyor)](https://pypi.python.org/pypi/python-backpack/)
 [![PyPI version](https://badge.fury.io/py/python-backpack.svg?style=flat-square&logo=appveyor)](https://badge.fury.io/py/python-backpack)
 [![GitHub version](https://badge.fury.io/gh/MaxRocamora%2Fpython-backpack.svg?style=flat-square&logo=appveyor)](https://badge.fury.io/gh/MaxRocamora%2Fpython-backpack)
 [![codecov](https://codecov.io/gh/MaxRocamora/python-backpack/branch/main/graph/badge.svg?token=6D1xwYdXW2)](https://codecov.io/gh/MaxRocamora/python-backpack)
 [![Message](https://img.shields.io/badge/python--backpack-python-blue?style=flat-square&logo=appveyor)](https://github.com/MaxRocamora/python-backpack)
 
 
 # Python-Backpack
-A collection of personal scripts for JSON, File/Folder Operations, String Validation, Custom Errors, and stuff.  
+A collection of personal scripts for JSON, File/Folder Operations, String Validation, Custom Errors, Cache and stuff.  
 
 
 ## Json
 + json_load()
 + json_save()
 + jsonMetaFile()
 + jsonUserSettings()
@@ -52,14 +53,17 @@
 + has_numbers()
 + camelcase_to_snakecase()
 
 ## Custom Errors
 + EnvironmentVariableNotFound()
 + ApplicationNotFound()
 
+## Cache
++ timed_lru_cache
+
 ## Test Utils
 + time_function_decorator()
 + random_string()
 
 ## Others / Patterns
 + Singleton()
```

### Comparing `python-backpack-1.0.4/python_backpack.egg-info/SOURCES.txt` & `python-backpack-1.0.5/python_backpack.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 backpack/__init__.py
+backpack/cache.py
 backpack/custom_errors.py
 backpack/file_utils.py
 backpack/folder_utils.py
 backpack/json_metadata.py
 backpack/json_user_settings.py
 backpack/json_utils.py
 backpack/logger.py
@@ -15,14 +16,15 @@
 backpack/test_utils.py
 backpack/version.py
 python_backpack.egg-info/PKG-INFO
 python_backpack.egg-info/SOURCES.txt
 python_backpack.egg-info/dependency_links.txt
 python_backpack.egg-info/top_level.txt
 tests/__init__.py
+tests/test_cache.py
 tests/test_errors.py
 tests/test_file_utils.py
 tests/test_folder_utils.py
 tests/test_json_user_settings.py
 tests/test_json_utils.py
 tests/test_jsonmd.py
 tests/test_misc.py
```

### Comparing `python-backpack-1.0.4/tests/test_errors.py` & `python-backpack-1.0.5/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `python-backpack-1.0.4/tests/test_file_utils.py` & `python-backpack-1.0.5/tests/test_file_utils.py`

 * *Files identical despite different names*

### Comparing `python-backpack-1.0.4/tests/test_folder_utils.py` & `python-backpack-1.0.5/tests/test_folder_utils.py`

 * *Files identical despite different names*

### Comparing `python-backpack-1.0.4/tests/test_json_user_settings.py` & `python-backpack-1.0.5/tests/test_json_user_settings.py`

 * *Files identical despite different names*

### Comparing `python-backpack-1.0.4/tests/test_json_utils.py` & `python-backpack-1.0.5/tests/test_json_utils.py`

 * *Files identical despite different names*

### Comparing `python-backpack-1.0.4/tests/test_jsonmd.py` & `python-backpack-1.0.5/tests/test_jsonmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,31 +39,31 @@
 
         # test properties
         self.assertEqual(meta.name, NAME)
 
         meta.insert(key='coins', value=12)
 
         # check if data have coins and value 12
-        self.assertEqual(meta.data['coins'], 12)
+        self.assertEqual(meta._data['coins'], 12)
 
         meta.save()
 
         # file was created
         self.assertEqual(meta.has_file(), True)
 
         # check if file exists
         self.assertEqual(os.path.exists(meta.filepath), True)
 
         meta.insert('coins', 7)
 
         # check if data have coins and value 7
-        self.assertEqual(meta.data['coins'], 7)
+        self.assertEqual(meta._data['coins'], 7)
 
         meta.remove('coins')
-        self.assertEqual(meta.data.get('coins', None), None)
+        self.assertEqual(meta._data.get('coins', None), None)
 
         meta.insert(key='items', value=ATTRIBUTES)
         meta.save()
 
         # load
         metaObj = meta.load_as_class()
         self.assertEqual(type(metaObj), type)
@@ -77,14 +77,14 @@
     def test_create_from_class(self):
         ''' save_from_a_class '''
         meta = JsonMetaFile(NAME, TEST_PATH)
         self.assertEqual(meta.name, NAME)
 
         proxyClass = type('Proxy', (), {'foo': 12, 'items': ATTRIBUTES})
         meta.insert_class(proxyClass)
-        self.assertEqual(meta.data['foo'], 12)
-        self.assertEqual(meta.data['items'], ATTRIBUTES)
+        self.assertEqual(meta._data['foo'], 12)
+        self.assertEqual(meta._data['items'], ATTRIBUTES)
         meta.save()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `python-backpack-1.0.4/tests/test_misc.py` & `python-backpack-1.0.5/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `python-backpack-1.0.4/tests/test_strings.py` & `python-backpack-1.0.5/tests/test_strings.py`

 * *Files identical despite different names*

### Comparing `python-backpack-1.0.4/tests/test_test_utils.py` & `python-backpack-1.0.5/tests/test_test_utils.py`

 * *Files identical despite different names*

