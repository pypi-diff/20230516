# Comparing `tmp/upy-error-0.0.2.tar.gz` & `tmp/upy-error-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upy-error-0.0.2.tar", last modified: Sat Jul 23 05:01:39 2022, max compression
+gzip compressed data, was "upy-error-0.0.3.tar", last modified: Tue May 16 00:16:45 2023, max compression
```

## Comparing `upy-error-0.0.2.tar` & `upy-error-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxr-x   0 fernandocelmer  (1000) fernandocelmer  (1000)        0 2022-07-23 05:01:39.729562 upy-error-0.0.2/
--rw-rw-r--   0 fernandocelmer  (1000) fernandocelmer  (1000)     2277 2022-07-23 05:01:39.729562 upy-error-0.0.2/PKG-INFO
--rw-rw-r--   0 fernandocelmer  (1000) fernandocelmer  (1000)     1635 2022-07-23 04:05:53.000000 upy-error-0.0.2/README.md
--rw-rw-r--   0 fernandocelmer  (1000) fernandocelmer  (1000)      138 2022-07-23 05:01:39.733562 upy-error-0.0.2/setup.cfg
--rw-rw-r--   0 fernandocelmer  (1000) fernandocelmer  (1000)     1042 2022-07-23 04:37:49.000000 upy-error-0.0.2/setup.py
-drwxrwxr-x   0 fernandocelmer  (1000) fernandocelmer  (1000)        0 2022-07-23 05:01:39.729562 upy-error-0.0.2/upy_error/
--rw-rw-r--   0 fernandocelmer  (1000) fernandocelmer  (1000)       99 2022-07-23 03:54:59.000000 upy-error-0.0.2/upy_error/__init__.py
--rw-rw-r--   0 fernandocelmer  (1000) fernandocelmer  (1000)      904 2022-07-23 03:51:04.000000 upy-error-0.0.2/upy_error/base.py
--rw-rw-r--   0 fernandocelmer  (1000) fernandocelmer  (1000)      431 2022-07-23 02:58:09.000000 upy-error-0.0.2/upy_error/config.py
-drwxrwxr-x   0 fernandocelmer  (1000) fernandocelmer  (1000)        0 2022-07-23 05:01:39.729562 upy-error-0.0.2/upy_error.egg-info/
--rw-rw-r--   0 fernandocelmer  (1000) fernandocelmer  (1000)     2277 2022-07-23 05:01:39.000000 upy-error-0.0.2/upy_error.egg-info/PKG-INFO
--rw-rw-r--   0 fernandocelmer  (1000) fernandocelmer  (1000)      252 2022-07-23 05:01:39.000000 upy-error-0.0.2/upy_error.egg-info/SOURCES.txt
--rw-rw-r--   0 fernandocelmer  (1000) fernandocelmer  (1000)        1 2022-07-23 05:01:39.000000 upy-error-0.0.2/upy_error.egg-info/dependency_links.txt
--rw-rw-r--   0 fernandocelmer  (1000) fernandocelmer  (1000)        1 2022-07-23 05:01:39.000000 upy-error-0.0.2/upy_error.egg-info/not-zip-safe
--rw-rw-r--   0 fernandocelmer  (1000) fernandocelmer  (1000)       10 2022-07-23 05:01:39.000000 upy-error-0.0.2/upy_error.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:16:45.592691 upy-error-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-05-16 00:16:45.592691 upy-error-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-05-16 00:16:25.000000 upy-error-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-16 00:16:45.596691 upy-error-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-16 00:16:25.000000 upy-error-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:16:45.592691 upy-error-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-16 00:16:25.000000 upy-error-0.0.3/tests/test_package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:16:45.592691 upy-error-0.0.3/upy_error/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-16 00:16:25.000000 upy-error-0.0.3/upy_error/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-16 00:16:25.000000 upy-error-0.0.3/upy_error/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-16 00:16:25.000000 upy-error-0.0.3/upy_error/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:16:45.592691 upy-error-0.0.3/upy_error.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-05-16 00:16:45.000000 upy-error-0.0.3/upy_error.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-16 00:16:45.000000 upy-error-0.0.3/upy_error.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 00:16:45.000000 upy-error-0.0.3/upy_error.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 00:16:45.000000 upy-error-0.0.3/upy_error.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-16 00:16:45.000000 upy-error-0.0.3/upy_error.egg-info/top_level.txt
```

### Comparing `upy-error-0.0.2/PKG-INFO` & `upy-error-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,84 +1,102 @@
 Metadata-Version: 2.1
 Name: upy-error
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python Trace Error
 Home-page: https://github.com/UpyExplorer/upy-error
 Author: Fernando Celmer
 Author-email: email@fernandocelmer.com
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # upy-error
 
+![GitHub Org's stars](https://img.shields.io/github/stars/UpyExplorer?label=LinuxProfile&style=flat-square)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/upy-error)
 ![PyPI](https://img.shields.io/pypi/v/upy-error)
 ![GitHub last commit](https://img.shields.io/github/last-commit/UpyExplorer/upy-error)
-![GitHub followers](https://img.shields.io/github/followers/UpyExplorer?label=UpyExplorer&style=social)
-<br>
+
+---
+
+- **Documentation**: [https://github.com/UpyExplorer/upy-error](https://github.com/UpyExplorer/upy-error)
+- **Source Code**: [https://github.com/UpyExplorer/upy-error](https://github.com/UpyExplorer/upy-error)
+
+---
 
 ## How to install?
-```python
 
+```python
 pip install upy-error
 
 ```
 ## How to use?
+
 ```python
 # Import the package
 from upy_error import format_exception
 ```
+
 ### Exception example with (log)
+
 ```python
 try:
     print(x)
 except Exception as error:
     # Using the function to process the error with the 'logging' package.
     format_exception(error=error, log=True)
 ```
+
 **Output:**
+
 ```shell
 ==========================================
 2022-07-23 00:13:37,577 ERROR 
 UpyError: 
   File "test_upy_error.py", line 4, in <module>
     print(x)
 NameError: name 'x' is not defined
 ==========================================
 ```
 
 ### Exception example with (print)
+
 ```python
 try:
     1 / 0
 except Exception as error:
     # Using the function to return the error in string format.
     print(format_exception(error=error))
 ```
+
 **Output:**
 ```shell
 UpyError: 
   File "test_upy_error.py", line 11, in <module>
     1 / 0
 ZeroDivisionError: division by zero
 ```
 
-<!-- LICENSE -->
-## License
-
-Distributed under the MIT License. See `LICENSE` for more information.
+## Commit Style
 
-<!-- CONTACT -->
-## Contact
+- ⚙️ FEATURE
+- 📝 PEP8
+- 📌 ISSUE
+- 🪲 BUG
+- 📘 DOCS
+- 📦 PyPI
+- ❤️️ TEST
+- ⬆️ CI/CD
+- ⚠️ SECURITY
 
-Fernando Celmer - email@fernandocelmer.com
+## License
 
-- Project Github: [https://github.com/UpyExplorer/upy-error](https://github.com/UpyExplorer/upy-error)
-- Project Pypi: [https://pypi.org/project/upy-error/](https://pypi.org/project/upy-error/)
+Distributed under the MIT License. See `LICENSE` for more information.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `upy-error-0.0.2/README.md` & `upy-error-0.0.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,66 +1,82 @@
 # upy-error
 
+![GitHub Org's stars](https://img.shields.io/github/stars/UpyExplorer?label=LinuxProfile&style=flat-square)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/upy-error)
 ![PyPI](https://img.shields.io/pypi/v/upy-error)
 ![GitHub last commit](https://img.shields.io/github/last-commit/UpyExplorer/upy-error)
-![GitHub followers](https://img.shields.io/github/followers/UpyExplorer?label=UpyExplorer&style=social)
-<br>
+
+---
+
+- **Documentation**: [https://github.com/UpyExplorer/upy-error](https://github.com/UpyExplorer/upy-error)
+- **Source Code**: [https://github.com/UpyExplorer/upy-error](https://github.com/UpyExplorer/upy-error)
+
+---
 
 ## How to install?
-```python
 
+```python
 pip install upy-error
 
 ```
 ## How to use?
+
 ```python
 # Import the package
 from upy_error import format_exception
 ```
+
 ### Exception example with (log)
+
 ```python
 try:
     print(x)
 except Exception as error:
     # Using the function to process the error with the 'logging' package.
     format_exception(error=error, log=True)
 ```
+
 **Output:**
+
 ```shell
 ==========================================
 2022-07-23 00:13:37,577 ERROR 
 UpyError: 
   File "test_upy_error.py", line 4, in <module>
     print(x)
 NameError: name 'x' is not defined
 ==========================================
 ```
 
 ### Exception example with (print)
+
 ```python
 try:
     1 / 0
 except Exception as error:
     # Using the function to return the error in string format.
     print(format_exception(error=error))
 ```
+
 **Output:**
 ```shell
 UpyError: 
   File "test_upy_error.py", line 11, in <module>
     1 / 0
 ZeroDivisionError: division by zero
 ```
 
-<!-- LICENSE -->
-## License
-
-Distributed under the MIT License. See `LICENSE` for more information.
+## Commit Style
 
-<!-- CONTACT -->
-## Contact
+- ⚙️ FEATURE
+- 📝 PEP8
+- 📌 ISSUE
+- 🪲 BUG
+- 📘 DOCS
+- 📦 PyPI
+- ❤️️ TEST
+- ⬆️ CI/CD
+- ⚠️ SECURITY
 
-Fernando Celmer - email@fernandocelmer.com
+## License
 
-- Project Github: [https://github.com/UpyExplorer/upy-error](https://github.com/UpyExplorer/upy-error)
-- Project Pypi: [https://pypi.org/project/upy-error/](https://pypi.org/project/upy-error/)
+Distributed under the MIT License. See `LICENSE` for more information.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `upy-error-0.0.2/setup.py` & `upy-error-0.0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-import setuptools
+from setuptools import setup
 import upy_error
 
 version = upy_error.__version__
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
-setuptools.setup(
+
+setup(
     name="upy-error",
     version=version,
     author="Fernando Celmer",
     author_email="email@fernandocelmer.com",
     description="Python Trace Error",
     long_description=long_description,
     long_description_content_type="text/markdown",
@@ -27,11 +28,13 @@
         "License :: OSI Approved :: MIT License",
         'Intended Audience :: Developers',
         'Natural Language :: English',
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     python_requires=">=3.6",
     zip_safe=False
 )
```

### Comparing `upy-error-0.0.2/upy_error/base.py` & `upy-error-0.0.3/upy_error/base.py`

 * *Files identical despite different names*

### Comparing `upy-error-0.0.2/upy_error.egg-info/PKG-INFO` & `upy-error-0.0.3/upy_error.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,84 +1,102 @@
 Metadata-Version: 2.1
 Name: upy-error
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python Trace Error
 Home-page: https://github.com/UpyExplorer/upy-error
 Author: Fernando Celmer
 Author-email: email@fernandocelmer.com
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # upy-error
 
+![GitHub Org's stars](https://img.shields.io/github/stars/UpyExplorer?label=LinuxProfile&style=flat-square)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/upy-error)
 ![PyPI](https://img.shields.io/pypi/v/upy-error)
 ![GitHub last commit](https://img.shields.io/github/last-commit/UpyExplorer/upy-error)
-![GitHub followers](https://img.shields.io/github/followers/UpyExplorer?label=UpyExplorer&style=social)
-<br>
+
+---
+
+- **Documentation**: [https://github.com/UpyExplorer/upy-error](https://github.com/UpyExplorer/upy-error)
+- **Source Code**: [https://github.com/UpyExplorer/upy-error](https://github.com/UpyExplorer/upy-error)
+
+---
 
 ## How to install?
-```python
 
+```python
 pip install upy-error
 
 ```
 ## How to use?
+
 ```python
 # Import the package
 from upy_error import format_exception
 ```
+
 ### Exception example with (log)
+
 ```python
 try:
     print(x)
 except Exception as error:
     # Using the function to process the error with the 'logging' package.
     format_exception(error=error, log=True)
 ```
+
 **Output:**
+
 ```shell
 ==========================================
 2022-07-23 00:13:37,577 ERROR 
 UpyError: 
   File "test_upy_error.py", line 4, in <module>
     print(x)
 NameError: name 'x' is not defined
 ==========================================
 ```
 
 ### Exception example with (print)
+
 ```python
 try:
     1 / 0
 except Exception as error:
     # Using the function to return the error in string format.
     print(format_exception(error=error))
 ```
+
 **Output:**
 ```shell
 UpyError: 
   File "test_upy_error.py", line 11, in <module>
     1 / 0
 ZeroDivisionError: division by zero
 ```
 
-<!-- LICENSE -->
-## License
-
-Distributed under the MIT License. See `LICENSE` for more information.
+## Commit Style
 
-<!-- CONTACT -->
-## Contact
+- ⚙️ FEATURE
+- 📝 PEP8
+- 📌 ISSUE
+- 🪲 BUG
+- 📘 DOCS
+- 📦 PyPI
+- ❤️️ TEST
+- ⬆️ CI/CD
+- ⚠️ SECURITY
 
-Fernando Celmer - email@fernandocelmer.com
+## License
 
-- Project Github: [https://github.com/UpyExplorer/upy-error](https://github.com/UpyExplorer/upy-error)
-- Project Pypi: [https://pypi.org/project/upy-error/](https://pypi.org/project/upy-error/)
+Distributed under the MIT License. See `LICENSE` for more information.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

