# Comparing `tmp/pyats-genie-command-parse-1.3.5.tar.gz` & `tmp/pyats-genie-command-parse-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyats-genie-command-parse-1.3.5.tar", last modified: Sat Mar 25 20:27:39 2023, max compression
+gzip compressed data, was "pyats-genie-command-parse-1.3.6.tar", last modified: Tue May 16 21:36:07 2023, max compression
```

## Comparing `pyats-genie-command-parse-1.3.5.tar` & `pyats-genie-command-parse-1.3.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 20:27:39.959690 pyats-genie-command-parse-1.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-03-25 20:26:39.000000 pyats-genie-command-parse-1.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-03-25 20:27:39.959690 pyats-genie-command-parse-1.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-03-25 20:26:39.000000 pyats-genie-command-parse-1.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 20:27:39.959690 pyats-genie-command-parse-1.3.5/pyats_genie_command_parse/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-03-25 20:26:39.000000 pyats-genie-command-parse-1.3.5/pyats_genie_command_parse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-03-25 20:26:39.000000 pyats-genie-command-parse-1.3.5/pyats_genie_command_parse/pyats_genie_command_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-03-25 20:26:39.000000 pyats-genie-command-parse-1.3.5/pyats_genie_command_parse/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 20:27:39.959690 pyats-genie-command-parse-1.3.5/pyats_genie_command_parse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-03-25 20:27:39.000000 pyats-genie-command-parse-1.3.5/pyats_genie_command_parse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-03-25 20:27:39.000000 pyats-genie-command-parse-1.3.5/pyats_genie_command_parse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 20:27:39.000000 pyats-genie-command-parse-1.3.5/pyats_genie_command_parse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 20:27:39.000000 pyats-genie-command-parse-1.3.5/pyats_genie_command_parse.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-25 20:27:39.000000 pyats-genie-command-parse-1.3.5/pyats_genie_command_parse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-25 20:27:39.000000 pyats-genie-command-parse-1.3.5/pyats_genie_command_parse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-03-25 20:26:39.000000 pyats-genie-command-parse-1.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-25 20:26:39.000000 pyats-genie-command-parse-1.3.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-25 20:27:39.959690 pyats-genie-command-parse-1.3.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 20:27:39.959690 pyats-genie-command-parse-1.3.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-03-25 20:26:39.000000 pyats-genie-command-parse-1.3.5/tests/test_ios_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-03-25 20:26:39.000000 pyats-genie-command-parse-1.3.5/tests/test_pyats_genie_command_parse_generic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:36:07.259076 pyats-genie-command-parse-1.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-16 21:35:15.000000 pyats-genie-command-parse-1.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-05-16 21:36:07.259076 pyats-genie-command-parse-1.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-05-16 21:35:15.000000 pyats-genie-command-parse-1.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:36:07.255076 pyats-genie-command-parse-1.3.6/pyats_genie_command_parse/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-16 21:35:15.000000 pyats-genie-command-parse-1.3.6/pyats_genie_command_parse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-05-16 21:35:15.000000 pyats-genie-command-parse-1.3.6/pyats_genie_command_parse/pyats_genie_command_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-16 21:35:15.000000 pyats-genie-command-parse-1.3.6/pyats_genie_command_parse/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:36:07.259076 pyats-genie-command-parse-1.3.6/pyats_genie_command_parse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-05-16 21:36:07.000000 pyats-genie-command-parse-1.3.6/pyats_genie_command_parse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-16 21:36:07.000000 pyats-genie-command-parse-1.3.6/pyats_genie_command_parse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 21:36:07.000000 pyats-genie-command-parse-1.3.6/pyats_genie_command_parse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 21:36:06.000000 pyats-genie-command-parse-1.3.6/pyats_genie_command_parse.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 21:36:07.000000 pyats-genie-command-parse-1.3.6/pyats_genie_command_parse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-16 21:36:07.000000 pyats-genie-command-parse-1.3.6/pyats_genie_command_parse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-05-16 21:35:15.000000 pyats-genie-command-parse-1.3.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 21:35:15.000000 pyats-genie-command-parse-1.3.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 21:36:07.259076 pyats-genie-command-parse-1.3.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:36:07.259076 pyats-genie-command-parse-1.3.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-16 21:35:15.000000 pyats-genie-command-parse-1.3.6/tests/test_ios_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-16 21:35:15.000000 pyats-genie-command-parse-1.3.6/tests/test_pyats_genie_command_parse_generic.py
```

### Comparing `pyats-genie-command-parse-1.3.5/LICENSE` & `pyats-genie-command-parse-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyats-genie-command-parse-1.3.5/PKG-INFO` & `pyats-genie-command-parse-1.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyats-genie-command-parse
-Version: 1.3.5
+Version: 1.3.6
 Summary: Run genie parsers directly.
 Author-email: "Benjamin P. Trachtenberg" <e_ben_75-python@yahoo.com>, Brett Gianpetro <e_ben_75-python@yahoo.com>
 Maintainer-email: "Benjamin P. Trachtenberg" <e_ben_75-python@yahoo.com>
 License: MIT License
         
         Copyright (c) 2020 - 2023 Benjamin Trachtenberg
```

### Comparing `pyats-genie-command-parse-1.3.5/README.md` & `pyats-genie-command-parse-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `pyats-genie-command-parse-1.3.5/pyats_genie_command_parse/pyats_genie_command_parse.py` & `pyats-genie-command-parse-1.3.6/pyats_genie_command_parse/pyats_genie_command_parse.py`

 * *Files identical despite different names*

### Comparing `pyats-genie-command-parse-1.3.5/pyats_genie_command_parse.egg-info/PKG-INFO` & `pyats-genie-command-parse-1.3.6/pyats_genie_command_parse.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyats-genie-command-parse
-Version: 1.3.5
+Version: 1.3.6
 Summary: Run genie parsers directly.
 Author-email: "Benjamin P. Trachtenberg" <e_ben_75-python@yahoo.com>, Brett Gianpetro <e_ben_75-python@yahoo.com>
 Maintainer-email: "Benjamin P. Trachtenberg" <e_ben_75-python@yahoo.com>
 License: MIT License
         
         Copyright (c) 2020 - 2023 Benjamin Trachtenberg
```

### Comparing `pyats-genie-command-parse-1.3.5/pyats_genie_command_parse.egg-info/SOURCES.txt` & `pyats-genie-command-parse-1.3.6/pyats_genie_command_parse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyats-genie-command-parse-1.3.5/pyproject.toml` & `pyats-genie-command-parse-1.3.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyats-genie-command-parse-1.3.5/tests/test_ios_parse.py` & `pyats-genie-command-parse-1.3.6/tests/test_ios_parse.py`

 * *Files identical despite different names*

### Comparing `pyats-genie-command-parse-1.3.5/tests/test_pyats_genie_command_parse_generic.py` & `pyats-genie-command-parse-1.3.6/tests/test_pyats_genie_command_parse_generic.py`

 * *Files identical despite different names*

