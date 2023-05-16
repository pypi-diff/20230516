# Comparing `tmp/loggerv-1.0.0.tar.gz` & `tmp/loggerv-1.0.1.tar.gz`

## Comparing `loggerv-1.0.0.tar` & `loggerv-1.0.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 loggerv-1.0.0/src/loggerV/__init__.py
--rw-r--r--   0        0        0    11679 2020-02-02 00:00:00.000000 loggerv-1.0.0/src/loggerV/logger.py
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 loggerv-1.0.0/tests/main.py
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 loggerv-1.0.0/.gitignore
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 loggerv-1.0.0/LICENSE
--rw-r--r--   0        0        0     2502 2020-02-02 00:00:00.000000 loggerv-1.0.0/README.md
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 loggerv-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 loggerv-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 loggerv-1.0.1/src/loggerV/__init__.py
+-rw-r--r--   0        0        0    11679 2020-02-02 00:00:00.000000 loggerv-1.0.1/src/loggerV/logger.py
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 loggerv-1.0.1/tests/main.py
+-rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 loggerv-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 loggerv-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 loggerv-1.0.1/README.md
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 loggerv-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 loggerv-1.0.1/PKG-INFO
```

### Comparing `loggerv-1.0.0/src/loggerV/logger.py` & `loggerv-1.0.1/src/loggerV/logger.py`

 * *Files identical despite different names*

### Comparing `loggerv-1.0.0/tests/main.py` & `loggerv-1.0.1/tests/main.py`

 * *Files identical despite different names*

### Comparing `loggerv-1.0.0/.gitignore` & `loggerv-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `loggerv-1.0.0/LICENSE` & `loggerv-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `loggerv-1.0.0/README.md` & `loggerv-1.0.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# logger_v-python
-A logger class and decorator for python
+# loggerV
+A logger class, and a decorator that works with that class for python
 ## Installation
 
-Use the package manager [pip](https://pip.pypa.io/en/stable/) to install logger_v-python.
+Use the package manager [pip](https://pip.pypa.io/en/stable/) to install loggerV.
 
 ```bash
 pip install loggerV
 ```
 
 ## Basic Usage
```

### Comparing `loggerv-1.0.0/pyproject.toml` & `loggerv-1.0.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "loggerV"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Aharon Vegoda", email="aaronvegoda@gmail.com" },
 ]
 maintainers = [
   { name="Aharon Vegoda", email="aaronvegoda@gmail.com" },
 ]
-description = "A logger class and a decorator that works with that class for python"
+description = "A logger class, and a decorator that works with that class for python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `loggerv-1.0.0/PKG-INFO` & `loggerv-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: loggerV
-Version: 1.0.0
-Summary: A logger class and a decorator that works with that class for python
+Version: 1.0.1
+Summary: A logger class, and a decorator that works with that class for python
 Project-URL: Homepage, https://github.com/aaronv15/logger_v-python
 Project-URL: Bug Tracker, https://github.com/aaronv15/logger_v-python/issues
 Author-email: Aharon Vegoda <aaronvegoda@gmail.com>
 Maintainer-email: Aharon Vegoda <aaronvegoda@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
-# logger_v-python
-A logger class and decorator for python
+# loggerV
+A logger class, and a decorator that works with that class for python
 ## Installation
 
-Use the package manager [pip](https://pip.pypa.io/en/stable/) to install logger_v-python.
+Use the package manager [pip](https://pip.pypa.io/en/stable/) to install loggerV.
 
 ```bash
 pip install loggerV
 ```
 
 ## Basic Usage
```

