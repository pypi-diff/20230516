# Comparing `tmp/test-teste-21479813-1.0.0.tar.gz` & `tmp/test-teste-21479813-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test-teste-21479813-1.0.0.tar", last modified: Tue May 16 15:40:03 2023, max compression
+gzip compressed data, was "test-teste-21479813-1.1.0.tar", last modified: Tue May 16 15:57:25 2023, max compression
```

## Comparing `test-teste-21479813-1.0.0.tar` & `test-teste-21479813-1.1.0.tar`

### file list

```diff
@@ -1,22 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 15:40:03.919345 test-teste-21479813-1.0.0/
--rw-rw-rw-   0        0        0     1089 2023-05-16 15:23:17.000000 test-teste-21479813-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      527 2023-05-16 15:40:03.921346 test-teste-21479813-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       21 2023-05-16 15:23:17.000000 test-teste-21479813-1.0.0/README.md
--rw-rw-rw-   0        0        0       86 2023-05-16 15:31:05.000000 test-teste-21479813-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0      638 2023-05-16 15:40:03.933342 test-teste-21479813-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-16 15:40:03.750340 test-teste-21479813-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-16 15:40:03.801338 test-teste-21479813-1.0.0/src/fundamentus_extractor/
--rw-rw-rw-   0        0        0      168 2023-05-16 15:23:17.000000 test-teste-21479813-1.0.0/src/fundamentus_extractor/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 15:40:03.822347 test-teste-21479813-1.0.0/src/fundamentus_extractor/data/
--rw-rw-rw-   0        0        0      183 2023-05-16 15:23:17.000000 test-teste-21479813-1.0.0/src/fundamentus_extractor/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 15:40:03.860337 test-teste-21479813-1.0.0/src/fundamentus_extractor/data/extract/
--rw-rw-rw-   0        0        0      572 2023-05-16 15:23:17.000000 test-teste-21479813-1.0.0/src/fundamentus_extractor/data/extract/Title.py
--rw-rw-rw-   0        0        0       90 2023-05-16 15:23:17.000000 test-teste-21479813-1.0.0/src/fundamentus_extractor/data/extract/__init__.py
--rw-rw-rw-   0        0        0     3816 2023-05-16 15:23:17.000000 test-teste-21479813-1.0.0/src/fundamentus_extractor/data/extract/core.py
--rw-rw-rw-   0        0        0      963 2023-05-16 15:23:17.000000 test-teste-21479813-1.0.0/src/fundamentus_extractor/data/extract/helpers.py
--rw-rw-rw-   0        0        0     2204 2023-05-16 15:23:17.000000 test-teste-21479813-1.0.0/src/fundamentus_extractor/data/tranforms.py
-drwxrwxrwx   0        0        0        0 2023-05-16 15:40:03.911344 test-teste-21479813-1.0.0/src/test_teste_21479813.egg-info/
--rw-rw-rw-   0        0        0      527 2023-05-16 15:40:02.000000 test-teste-21479813-1.0.0/src/test_teste_21479813.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      551 2023-05-16 15:40:03.000000 test-teste-21479813-1.0.0/src/test_teste_21479813.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 15:40:02.000000 test-teste-21479813-1.0.0/src/test_teste_21479813.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-05-16 15:40:02.000000 test-teste-21479813-1.0.0/src/test_teste_21479813.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 15:57:25.220748 test-teste-21479813-1.1.0/
+-rw-rw-rw-   0        0        0     1089 2023-05-16 15:23:17.000000 test-teste-21479813-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0      527 2023-05-16 15:57:25.222746 test-teste-21479813-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       21 2023-05-16 15:23:17.000000 test-teste-21479813-1.1.0/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-16 15:31:05.000000 test-teste-21479813-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0      638 2023-05-16 15:57:25.235746 test-teste-21479813-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-16 15:57:25.032975 test-teste-21479813-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-16 15:57:25.079746 test-teste-21479813-1.1.0/src/fundamentus_extractor/
+-rw-rw-rw-   0        0        0      156 2023-05-16 15:56:46.000000 test-teste-21479813-1.1.0/src/fundamentus_extractor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:57:25.100742 test-teste-21479813-1.1.0/src/fundamentus_extractor/data/
+-rw-rw-rw-   0        0        0      183 2023-05-16 15:23:17.000000 test-teste-21479813-1.1.0/src/fundamentus_extractor/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:57:25.143749 test-teste-21479813-1.1.0/src/fundamentus_extractor/data/extract/
+-rw-rw-rw-   0        0        0      572 2023-05-16 15:23:17.000000 test-teste-21479813-1.1.0/src/fundamentus_extractor/data/extract/Title.py
+-rw-rw-rw-   0        0        0       90 2023-05-16 15:23:17.000000 test-teste-21479813-1.1.0/src/fundamentus_extractor/data/extract/__init__.py
+-rw-rw-rw-   0        0        0     3816 2023-05-16 15:23:17.000000 test-teste-21479813-1.1.0/src/fundamentus_extractor/data/extract/core.py
+-rw-rw-rw-   0        0        0      963 2023-05-16 15:23:17.000000 test-teste-21479813-1.1.0/src/fundamentus_extractor/data/extract/helpers.py
+-rw-rw-rw-   0        0        0     2204 2023-05-16 15:23:17.000000 test-teste-21479813-1.1.0/src/fundamentus_extractor/data/tranforms.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:57:25.167746 test-teste-21479813-1.1.0/src/fundamentus_extractor/main/
+-rw-rw-rw-   0        0        0      164 2023-05-16 15:53:31.000000 test-teste-21479813-1.1.0/src/fundamentus_extractor/main/__init__.py
+-rw-rw-rw-   0        0        0      613 2023-05-16 15:23:17.000000 test-teste-21479813-1.1.0/src/fundamentus_extractor/main/fundamentus.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:57:25.214741 test-teste-21479813-1.1.0/src/test_teste_21479813.egg-info/
+-rw-rw-rw-   0        0        0      527 2023-05-16 15:57:23.000000 test-teste-21479813-1.1.0/src/test_teste_21479813.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      640 2023-05-16 15:57:24.000000 test-teste-21479813-1.1.0/src/test_teste_21479813.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 15:57:23.000000 test-teste-21479813-1.1.0/src/test_teste_21479813.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-05-16 15:57:23.000000 test-teste-21479813-1.1.0/src/test_teste_21479813.egg-info/top_level.txt
```

### Comparing `test-teste-21479813-1.0.0/LICENSE` & `test-teste-21479813-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `test-teste-21479813-1.0.0/PKG-INFO` & `test-teste-21479813-1.1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test-teste-21479813
-Version: 1.0.0
+Version: 1.1.0
 Summary: A simple Python package test
 Home-page: https://google.com.br/
 Author: test@test.com
 Author-email: test@test.com
 Project-URL: Bug Tracker, https://google.com.br/
 Project-URL: repository, https://google.com.br/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `test-teste-21479813-1.0.0/setup.cfg` & `test-teste-21479813-1.1.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2074 6573 742d 7465 7374 652d 3231   = test-teste-21
 00000020: 3437 3938 3133 0d0a 7665 7273 696f 6e20  479813..version 
-00000030: 3d20 312e 302e 300d 0a61 7574 686f 7220  = 1.0.0..author 
+00000030: 3d20 312e 312e 300d 0a61 7574 686f 7220  = 1.1.0..author 
 00000040: 3d20 7465 7374 4074 6573 742e 636f 6d0d  = test@test.com.
 00000050: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
 00000060: 7465 7374 4074 6573 742e 636f 6d0d 0a64  test@test.com..d
 00000070: 6573 6372 6970 7469 6f6e 203d 2041 2073  escription = A s
 00000080: 696d 706c 6520 5079 7468 6f6e 2070 6163  imple Python pac
 00000090: 6b61 6765 2074 6573 740d 0a6c 6f6e 675f  kage test..long_
 000000a0: 6465 7363 7269 7074 696f 6e20 3d20 7465  description = te
```

### Comparing `test-teste-21479813-1.0.0/src/fundamentus_extractor/data/extract/Title.py` & `test-teste-21479813-1.1.0/src/fundamentus_extractor/data/extract/Title.py`

 * *Files identical despite different names*

### Comparing `test-teste-21479813-1.0.0/src/fundamentus_extractor/data/extract/core.py` & `test-teste-21479813-1.1.0/src/fundamentus_extractor/data/extract/core.py`

 * *Files identical despite different names*

### Comparing `test-teste-21479813-1.0.0/src/fundamentus_extractor/data/extract/helpers.py` & `test-teste-21479813-1.1.0/src/fundamentus_extractor/data/extract/helpers.py`

 * *Files identical despite different names*

### Comparing `test-teste-21479813-1.0.0/src/fundamentus_extractor/data/tranforms.py` & `test-teste-21479813-1.1.0/src/fundamentus_extractor/data/tranforms.py`

 * *Files identical despite different names*

### Comparing `test-teste-21479813-1.0.0/src/test_teste_21479813.egg-info/PKG-INFO` & `test-teste-21479813-1.1.0/src/test_teste_21479813.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test-teste-21479813
-Version: 1.0.0
+Version: 1.1.0
 Summary: A simple Python package test
 Home-page: https://google.com.br/
 Author: test@test.com
 Author-email: test@test.com
 Project-URL: Bug Tracker, https://google.com.br/
 Project-URL: repository, https://google.com.br/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `test-teste-21479813-1.0.0/src/test_teste_21479813.egg-info/SOURCES.txt` & `test-teste-21479813-1.1.0/src/test_teste_21479813.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -5,11 +5,13 @@
 src/fundamentus_extractor/__init__.py
 src/fundamentus_extractor/data/__init__.py
 src/fundamentus_extractor/data/tranforms.py
 src/fundamentus_extractor/data/extract/Title.py
 src/fundamentus_extractor/data/extract/__init__.py
 src/fundamentus_extractor/data/extract/core.py
 src/fundamentus_extractor/data/extract/helpers.py
+src/fundamentus_extractor/main/__init__.py
+src/fundamentus_extractor/main/fundamentus.py
 src/test_teste_21479813.egg-info/PKG-INFO
 src/test_teste_21479813.egg-info/SOURCES.txt
 src/test_teste_21479813.egg-info/dependency_links.txt
 src/test_teste_21479813.egg-info/top_level.txt
```

