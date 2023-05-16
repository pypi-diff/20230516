# Comparing `tmp/uwuify-1.2.1.tar.gz` & `tmp/uwuify-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uwuify-1.2.1.tar", max compression
+gzip compressed data, was "uwuify-1.3.0.tar", max compression
```

## Comparing `uwuify-1.2.1.tar` & `uwuify-1.3.0.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1065 2022-12-02 20:13:29.436187 uwuify-1.2.1/LICENSE
--rw-r--r--   0        0        0      913 2022-12-02 20:21:22.431686 uwuify-1.2.1/README.md
--rw-r--r--   0        0        0      447 2022-12-02 20:30:10.440285 uwuify-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     1264 2022-12-02 20:17:01.098820 uwuify-1.2.1/uwuify/__init__.py
--rw-r--r--   0        0        0     1190 2022-12-02 20:13:29.436187 uwuify-1.2.1/uwuify/__main__.py
--rw-r--r--   0        0        0     2034 2022-12-02 20:19:27.640468 uwuify-1.2.1/uwuify/cli.py
--rw-r--r--   0        0        0     3851 2022-12-02 20:29:52.019688 uwuify-1.2.1/uwuify/core.py
--rw-r--r--   0        0        0     1640 1970-01-01 00:00:00.000000 uwuify-1.2.1/setup.py
--rw-r--r--   0        0        0     1627 1970-01-01 00:00:00.000000 uwuify-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2022-12-02 20:13:29.436187 uwuify-1.3.0/LICENSE
+-rw-r--r--   0        0        0     1046 2023-05-16 06:25:18.470758 uwuify-1.3.0/README.md
+-rw-r--r--   0        0        0      546 2023-05-16 07:29:22.233729 uwuify-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      222 2023-05-16 07:29:33.987253 uwuify-1.3.0/uwuify/__init__.py
+-rw-r--r--   0        0        0       73 2023-05-16 07:27:24.981830 uwuify-1.3.0/uwuify/__main__.py
+-rw-r--r--   0        0        0     1040 2023-05-16 07:27:24.981830 uwuify-1.3.0/uwuify/cli.py
+-rw-r--r--   0        0        0     3066 2023-05-16 07:27:24.981830 uwuify-1.3.0/uwuify/core.py
+-rw-r--r--   0        0        0     1702 1970-01-01 00:00:00.000000 uwuify-1.3.0/PKG-INFO
```

### Comparing `uwuify-1.2.1/LICENSE` & `uwuify-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `uwuify-1.2.1/README.md` & `uwuify-1.3.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,48 @@
 # uwuify
 
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/uwuify?style=for-the-badge)
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-
 Command line uwuification
 
 # Installation
+
 ```shell
 pip install uwuify
 ```
 
 # Usage
+
 ```shell
 uwuify hello
 # outputs hewwo in console
 
 uwuify how are you? --smiley --yu
 # outputs how awe yoyu? with a random smiley
 
 uwuify how are you? --smiley --yu --stutter
 # outputs h-how awe yoyu? with a random smiley
 # --stutter stutters every 4-th word
 ```
+
 or
+
 ```python
 import uwuify
 
 print(uwuify.uwu("hello"))
 # hewwo
 
 flags = uwuify.SMILEY | uwuify.YU
 print(uwuify.uwu("how are you?", flags=flags))
 # how awe yoyu? with a random smiley
 
 flags = uwuify.SMILEY | uwuify.YU | uwuify.STUTTER
 print(uwuify.uwu("how are you?", flags=flags))
 # h-how awe yoyu? with a random smiley
-```
+
+flags = uwuify.SMILEY | uwuify.NOUWU
+print(uwuify.uwu("how are you?", flags=flags))
+# how are you? with a random smiley
+```
```

### Comparing `uwuify-1.2.1/PKG-INFO` & `uwuify-1.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: uwuify
-Version: 1.2.1
+Version: 1.3.0
 Summary: uwuifys text
 Home-page: https://github.com/StarrFox/uwuify
 License: MIT
 Author: StarrFox
 Author-email: starrfox6312@gmail.com
-Requires-Python: >=3.6,<4.0
+Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.0.1,<9.0.0)
 Project-URL: Repository, https://github.com/StarrFox/uwuify
@@ -21,42 +20,50 @@
 
 # uwuify
 
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/uwuify?style=for-the-badge)
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-
 Command line uwuification
 
 # Installation
+
 ```shell
 pip install uwuify
 ```
 
 # Usage
+
 ```shell
 uwuify hello
 # outputs hewwo in console
 
 uwuify how are you? --smiley --yu
 # outputs how awe yoyu? with a random smiley
 
 uwuify how are you? --smiley --yu --stutter
 # outputs h-how awe yoyu? with a random smiley
 # --stutter stutters every 4-th word
 ```
+
 or
+
 ```python
 import uwuify
 
 print(uwuify.uwu("hello"))
 # hewwo
 
 flags = uwuify.SMILEY | uwuify.YU
 print(uwuify.uwu("how are you?", flags=flags))
 # how awe yoyu? with a random smiley
 
 flags = uwuify.SMILEY | uwuify.YU | uwuify.STUTTER
 print(uwuify.uwu("how are you?", flags=flags))
 # h-how awe yoyu? with a random smiley
+
+flags = uwuify.SMILEY | uwuify.NOUWU
+print(uwuify.uwu("how are you?", flags=flags))
+# how are you? with a random smiley
 ```
+
```

