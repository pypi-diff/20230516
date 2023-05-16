# Comparing `tmp/prelude-sdk-1.1.1.tar.gz` & `tmp/prelude-sdk-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prelude-sdk-1.1.1.tar", last modified: Sat May 13 20:30:41 2023, max compression
+gzip compressed data, was "prelude-sdk-1.1.2.tar", last modified: Tue May 16 20:31:57 2023, max compression
```

## Comparing `prelude-sdk-1.1.1.tar` & `prelude-sdk-1.1.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-13 20:30:41.680450 prelude-sdk-1.1.1/
--rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-sdk-1.1.1/LICENSE
--rw-r--r--   0 pack       (501) staff       (20)     1139 2023-05-13 20:30:41.680502 prelude-sdk-1.1.1/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      697 2023-04-11 22:16:02.000000 prelude-sdk-1.1.1/README.md
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-13 20:30:41.676136 prelude-sdk-1.1.1/prelude_sdk/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.1.1/prelude_sdk/__init__.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-13 20:30:41.678264 prelude-sdk-1.1.1/prelude_sdk/controllers/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.1.1/prelude_sdk/controllers/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     2230 2023-05-07 12:16:47.000000 prelude-sdk-1.1.1/prelude_sdk/controllers/build_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     4115 2023-05-12 13:56:19.000000 prelude-sdk-1.1.1/prelude_sdk/controllers/detect_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     3266 2023-05-12 13:56:19.000000 prelude-sdk-1.1.1/prelude_sdk/controllers/iam_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     2046 2023-05-03 13:30:52.000000 prelude-sdk-1.1.1/prelude_sdk/controllers/partner_controller.py
--rw-r--r--   0 pack       (501) staff       (20)      443 2023-05-03 13:30:52.000000 prelude-sdk-1.1.1/prelude_sdk/controllers/probe_controller.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-13 20:30:41.678822 prelude-sdk-1.1.1/prelude_sdk/models/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.1.1/prelude_sdk/models/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     2816 2023-04-07 19:23:14.000000 prelude-sdk-1.1.1/prelude_sdk/models/account.py
--rw-r--r--   0 pack       (501) staff       (20)     2698 2023-05-09 16:39:45.000000 prelude-sdk-1.1.1/prelude_sdk/models/codes.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-13 20:30:41.676729 prelude-sdk-1.1.1/prelude_sdk.egg-info/
--rw-r--r--   0 pack       (501) staff       (20)     1139 2023-05-13 20:30:41.000000 prelude-sdk-1.1.1/prelude_sdk.egg-info/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      806 2023-05-13 20:30:41.000000 prelude-sdk-1.1.1/prelude_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 pack       (501) staff       (20)        1 2023-05-13 20:30:41.000000 prelude-sdk-1.1.1/prelude_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 pack       (501) staff       (20)        9 2023-05-13 20:30:41.000000 prelude-sdk-1.1.1/prelude_sdk.egg-info/requires.txt
--rw-r--r--   0 pack       (501) staff       (20)       18 2023-05-13 20:30:41.000000 prelude-sdk-1.1.1/prelude_sdk.egg-info/top_level.txt
--rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-sdk-1.1.1/pyproject.toml
--rw-r--r--   0 pack       (501) staff       (20)      532 2023-05-13 20:30:41.680703 prelude-sdk-1.1.1/setup.cfg
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-13 20:30:41.680099 prelude-sdk-1.1.1/tests/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-04-07 19:23:14.000000 prelude-sdk-1.1.1/tests/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     1101 2023-04-11 22:16:02.000000 prelude-sdk-1.1.1/tests/conftest.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-13 20:30:41.680359 prelude-sdk-1.1.1/tests/templates/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-04-07 19:23:14.000000 prelude-sdk-1.1.1/tests/templates/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     2188 2023-05-07 12:16:47.000000 prelude-sdk-1.1.1/tests/test_build_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     3734 2023-05-03 13:30:52.000000 prelude-sdk-1.1.1/tests/test_detect_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     3359 2023-05-12 13:56:19.000000 prelude-sdk-1.1.1/tests/test_iam_controller.py
--rw-r--r--   0 pack       (501) staff       (20)      785 2023-05-02 14:19:17.000000 prelude-sdk-1.1.1/tests/test_partner_controller.py
--rw-r--r--   0 pack       (501) staff       (20)      682 2023-04-07 19:23:14.000000 prelude-sdk-1.1.1/tests/test_probe_controller.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-16 20:31:57.516418 prelude-sdk-1.1.2/
+-rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-sdk-1.1.2/LICENSE
+-rw-r--r--   0 pack       (501) staff       (20)     1139 2023-05-16 20:31:57.516488 prelude-sdk-1.1.2/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      697 2023-04-11 22:16:02.000000 prelude-sdk-1.1.2/README.md
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-16 20:31:57.512205 prelude-sdk-1.1.2/prelude_sdk/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.1.2/prelude_sdk/__init__.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-16 20:31:57.514202 prelude-sdk-1.1.2/prelude_sdk/controllers/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.1.2/prelude_sdk/controllers/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     2230 2023-05-07 12:16:47.000000 prelude-sdk-1.1.2/prelude_sdk/controllers/build_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     4115 2023-05-12 13:56:19.000000 prelude-sdk-1.1.2/prelude_sdk/controllers/detect_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     3266 2023-05-12 13:56:19.000000 prelude-sdk-1.1.2/prelude_sdk/controllers/iam_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     2046 2023-05-03 13:30:52.000000 prelude-sdk-1.1.2/prelude_sdk/controllers/partner_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)      443 2023-05-03 13:30:52.000000 prelude-sdk-1.1.2/prelude_sdk/controllers/probe_controller.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-16 20:31:57.514735 prelude-sdk-1.1.2/prelude_sdk/models/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.1.2/prelude_sdk/models/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     2816 2023-04-07 19:23:14.000000 prelude-sdk-1.1.2/prelude_sdk/models/account.py
+-rw-r--r--   0 pack       (501) staff       (20)     2698 2023-05-09 16:39:45.000000 prelude-sdk-1.1.2/prelude_sdk/models/codes.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-16 20:31:57.512780 prelude-sdk-1.1.2/prelude_sdk.egg-info/
+-rw-r--r--   0 pack       (501) staff       (20)     1139 2023-05-16 20:31:57.000000 prelude-sdk-1.1.2/prelude_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      806 2023-05-16 20:31:57.000000 prelude-sdk-1.1.2/prelude_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 pack       (501) staff       (20)        1 2023-05-16 20:31:57.000000 prelude-sdk-1.1.2/prelude_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 pack       (501) staff       (20)        9 2023-05-16 20:31:57.000000 prelude-sdk-1.1.2/prelude_sdk.egg-info/requires.txt
+-rw-r--r--   0 pack       (501) staff       (20)       18 2023-05-16 20:31:57.000000 prelude-sdk-1.1.2/prelude_sdk.egg-info/top_level.txt
+-rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-sdk-1.1.2/pyproject.toml
+-rw-r--r--   0 pack       (501) staff       (20)      532 2023-05-16 20:31:57.516719 prelude-sdk-1.1.2/setup.cfg
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-16 20:31:57.516105 prelude-sdk-1.1.2/tests/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-04-07 19:23:14.000000 prelude-sdk-1.1.2/tests/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     1101 2023-04-11 22:16:02.000000 prelude-sdk-1.1.2/tests/conftest.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-16 20:31:57.516317 prelude-sdk-1.1.2/tests/templates/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-04-07 19:23:14.000000 prelude-sdk-1.1.2/tests/templates/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     2188 2023-05-07 12:16:47.000000 prelude-sdk-1.1.2/tests/test_build_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     3734 2023-05-03 13:30:52.000000 prelude-sdk-1.1.2/tests/test_detect_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     3359 2023-05-12 13:56:19.000000 prelude-sdk-1.1.2/tests/test_iam_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)      785 2023-05-02 14:19:17.000000 prelude-sdk-1.1.2/tests/test_partner_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)      682 2023-04-07 19:23:14.000000 prelude-sdk-1.1.2/tests/test_probe_controller.py
```

### Comparing `prelude-sdk-1.1.1/LICENSE` & `prelude-sdk-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.1.1/PKG-INFO` & `prelude-sdk-1.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-sdk
-Version: 1.1.1
+Version: 1.1.2
 Summary: For interacting with the Prelude API
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prelude-sdk-1.1.1/README.md` & `prelude-sdk-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.1.1/prelude_sdk/controllers/build_controller.py` & `prelude-sdk-1.1.2/prelude_sdk/controllers/build_controller.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.1.1/prelude_sdk/controllers/detect_controller.py` & `prelude-sdk-1.1.2/prelude_sdk/controllers/detect_controller.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.1.1/prelude_sdk/controllers/iam_controller.py` & `prelude-sdk-1.1.2/prelude_sdk/controllers/iam_controller.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.1.1/prelude_sdk/controllers/partner_controller.py` & `prelude-sdk-1.1.2/prelude_sdk/controllers/partner_controller.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.1.1/prelude_sdk/models/account.py` & `prelude-sdk-1.1.2/prelude_sdk/models/account.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.1.1/prelude_sdk/models/codes.py` & `prelude-sdk-1.1.2/prelude_sdk/models/codes.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.1.1/prelude_sdk.egg-info/PKG-INFO` & `prelude-sdk-1.1.2/prelude_sdk.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-sdk
-Version: 1.1.1
+Version: 1.1.2
 Summary: For interacting with the Prelude API
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prelude-sdk-1.1.1/prelude_sdk.egg-info/SOURCES.txt` & `prelude-sdk-1.1.2/prelude_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.1.1/setup.cfg` & `prelude-sdk-1.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = prelude-sdk
-version = 1.1.1
+version = 1.1.2
 author = Prelude Research
 author_email = support@preludesecurity.com
 description = For interacting with the Prelude API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/preludeorg
 classifiers =
```

### Comparing `prelude-sdk-1.1.1/tests/conftest.py` & `prelude-sdk-1.1.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.1.1/tests/test_build_controller.py` & `prelude-sdk-1.1.2/tests/test_build_controller.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.1.1/tests/test_detect_controller.py` & `prelude-sdk-1.1.2/tests/test_detect_controller.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.1.1/tests/test_iam_controller.py` & `prelude-sdk-1.1.2/tests/test_iam_controller.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.1.1/tests/test_partner_controller.py` & `prelude-sdk-1.1.2/tests/test_partner_controller.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.1.1/tests/test_probe_controller.py` & `prelude-sdk-1.1.2/tests/test_probe_controller.py`

 * *Files identical despite different names*

