# Comparing `tmp/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.3.tar.gz` & `tmp/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.3.tar", last modified: Tue May 16 06:20:13 2023, max compression
+gzip compressed data, was "dist/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.4.tar", last modified: Tue May 16 06:52:43 2023, max compression
```

## Comparing `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.3.tar` & `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 06:20:13.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.3/
--rw-r--r--   0 root         (0) root         (0)      600 2023-05-16 06:20:12.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-16 06:20:12.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2354 2023-05-16 06:20:13.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      900 2023-05-16 06:20:12.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.3/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1086 2023-05-16 06:20:12.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 06:20:13.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.3/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2354 2023-05-16 06:20:12.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.3/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      579 2023-05-16 06:20:12.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.3/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 06:20:12.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.3/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-05-16 06:20:12.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.3/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-05-16 06:20:12.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.3/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 06:20:13.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.3/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-16 06:20:12.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.3/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35756 2023-05-16 06:20:12.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.3/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/client.py
--rw-r--r--   0 root         (0) root         (0)    41149 2023-05-16 06:20:12.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.3/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-16 06:20:13.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2650 2023-05-16 06:20:12.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 06:52:43.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.4/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-05-16 06:52:42.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-16 06:52:42.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-05-16 06:52:43.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      900 2023-05-16 06:52:42.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.4/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1086 2023-05-16 06:52:42.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 06:52:43.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.4/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-05-16 06:52:42.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.4/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      579 2023-05-16 06:52:42.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.4/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 06:52:42.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.4/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-05-16 06:52:42.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.4/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-05-16 06:52:42.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.4/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 06:52:43.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.4/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-16 06:52:42.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.4/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22004 2023-05-16 06:52:42.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.4/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/client.py
+-rw-r--r--   0 root         (0) root         (0)    15216 2023-05-16 06:52:42.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.4/antchain_sdk_ak_c3cc551641bc4a1e948f7b80bb2180f4/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-16 06:52:43.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2650 2023-05-16 06:52:42.000000 antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.4/setup.py
```

### Comparing `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.3/LICENSE` & `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.3/PKG-INFO` & `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.4/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4
-Version: 1.0.3
+Name: antchain-ak-c3cc551641bc4a1e948f7b80bb2180f4
+Version: 1.0.4
 Summary: Ant Chain Ak_c3cc551641bc4a1e948f7b80bb2180f4 SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.3/README-CN.md` & `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.4/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.3/README.md` & `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.3/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/PKG-INFO` & `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: antchain-ak-c3cc551641bc4a1e948f7b80bb2180f4
-Version: 1.0.3
+Name: antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4
+Version: 1.0.4
 Summary: Ant Chain Ak_c3cc551641bc4a1e948f7b80bb2180f4 SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.3/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/SOURCES.txt` & `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.4/antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.3/setup.py` & `antchain_ak_c3cc551641bc4a1e948f7b80bb2180f4-1.0.4/setup.py`

 * *Files identical despite different names*

