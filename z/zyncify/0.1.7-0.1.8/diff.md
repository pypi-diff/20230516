# Comparing `tmp/zyncify-0.1.7-py2.py3-none-any.whl.zip` & `tmp/zyncify-0.1.8-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 17678 bytes, number of entries: 12
+Zip file size: 17693 bytes, number of entries: 12
 -rw-r--r--  2.0 unx      166 b- defN 23-May-14 22:32 zync/__init__.py
--rw-r--r--  2.0 unx     4946 b- defN 23-May-14 23:25 zync/logger.py
+-rw-r--r--  2.0 unx     5011 b- defN 23-May-16 11:11 zync/logger.py
 -rw-r--r--  2.0 unx      480 b- defN 23-May-13 13:21 zync/logging.py
--rw-r--r--  2.0 unx     1470 b- defN 23-May-14 23:27 zync/main.py
+-rw-r--r--  2.0 unx     1470 b- defN 23-May-16 11:11 zync/main.py
 -rw-r--r--  2.0 unx     1228 b- defN 23-May-14 23:19 zync/slugify.py
 -rw-r--r--  2.0 unx      966 b- defN 23-May-13 14:31 zync/zync.py
--rw-r--r--  2.0 unx    35149 b- defN 23-May-14 23:27 zyncify-0.1.7.dist-info/LICENSE
--rw-r--r--  2.0 unx     2098 b- defN 23-May-14 23:27 zyncify-0.1.7.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-May-14 23:27 zyncify-0.1.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       40 b- defN 23-May-14 23:27 zyncify-0.1.7.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        5 b- defN 23-May-14 23:27 zyncify-0.1.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      905 b- defN 23-May-14 23:27 zyncify-0.1.7.dist-info/RECORD
-12 files, 47563 bytes uncompressed, 16178 bytes compressed:  66.0%
+-rw-r--r--  2.0 unx    35149 b- defN 23-May-16 11:12 zyncify-0.1.8.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2102 b- defN 23-May-16 11:12 zyncify-0.1.8.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-May-16 11:12 zyncify-0.1.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       40 b- defN 23-May-16 11:12 zyncify-0.1.8.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        5 b- defN 23-May-16 11:12 zyncify-0.1.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      905 b- defN 23-May-16 11:12 zyncify-0.1.8.dist-info/RECORD
+12 files, 47632 bytes uncompressed, 16193 bytes compressed:  66.0%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: zync/slugify.py
 Comment: 
 
 Filename: zync/zync.py
 Comment: 
 
-Filename: zyncify-0.1.7.dist-info/LICENSE
+Filename: zyncify-0.1.8.dist-info/LICENSE
 Comment: 
 
-Filename: zyncify-0.1.7.dist-info/METADATA
+Filename: zyncify-0.1.8.dist-info/METADATA
 Comment: 
 
-Filename: zyncify-0.1.7.dist-info/WHEEL
+Filename: zyncify-0.1.8.dist-info/WHEEL
 Comment: 
 
-Filename: zyncify-0.1.7.dist-info/entry_points.txt
+Filename: zyncify-0.1.8.dist-info/entry_points.txt
 Comment: 
 
-Filename: zyncify-0.1.7.dist-info/top_level.txt
+Filename: zyncify-0.1.8.dist-info/top_level.txt
 Comment: 
 
-Filename: zyncify-0.1.7.dist-info/RECORD
+Filename: zyncify-0.1.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## zync/logger.py

```diff
@@ -136,40 +136,43 @@
 logger_base = Logger("logger")
 egger_base = Egger("egger")
 
 
 def get_relative_path(frame):
     """getting the relative path for logging position"""
     filename = inspect.getframeinfo(frame).filename
-    current_dir = os.path.dirname(os.path.abspath(__file__))
+    current_dir = os.getcwd()
     relative_path = os.path.relpath(filename, current_dir)
     return relative_path
 
 
 def bugger(log):
     """the bugger method"""
     frame = inspect.currentframe().f_back
     path = get_relative_path(frame)
     line = inspect.getframeinfo(frame).positions.lineno
     col = inspect.getframeinfo(frame).positions.col_offset
-    url = "%s:%s:%s" % (path, line, col)
+    href = "%s:%s:%s" % (path, line, col)
+    url = "file '" + href +"'"
     return bugger_base(log, line, url)
 
 
 def logger(log):
     """the logger method"""
     frame = inspect.currentframe().f_back
     path = get_relative_path(frame)
     line = inspect.getframeinfo(frame).positions.lineno
     col = inspect.getframeinfo(frame).positions.col_offset
-    url = "%s:%s:%s" % (path, line, col)
+    href = "%s:%s:%s" % (path, line, col)
+    url = "file '" + href +"'"
     return logger_base(log, line, url)
 
 
 def egger(log):
     """the egger method"""
     frame = inspect.currentframe().f_back
     path = get_relative_path(frame)
     line = inspect.getframeinfo(frame).positions.lineno
     col = inspect.getframeinfo(frame).positions.col_offset
-    url = "%s:%s:%s" % (path, line, col)
+    href = "%s:%s:%s" % (path, line, col)
+    url = "file '" + href +"'"
     return egger_base(log, line, url)
```

## zync/main.py

```diff
@@ -5,15 +5,15 @@
 import argparse
 from .__init__ import __all__ as methods
 
 NAME = "zyncify"
 DISPLAY_NAME = "zync"
 DESCRIPTION = "zync is a utility tool for python operations"
 URL = "https://github.com/tjbredemeyer/zync"
-VERSION = "0.1.7"
+VERSION = "0.1.8"
 AUTHOR = "TJ Bredemeyer"
 AUTHOR_EMAIL = "tj@teicor.com"
 LICENSE = "GNU Public License v3"
 
 info_string = (
     "\n"
     f"name: {DISPLAY_NAME}\n"
```

## Comparing `zyncify-0.1.7.dist-info/LICENSE` & `zyncify-0.1.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `zyncify-0.1.7.dist-info/METADATA` & `zyncify-0.1.8.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zyncify
-Version: 0.1.7
+Version: 0.1.8
 Summary: zync is a utility tool for python operations
 Home-page: https://github.com/tjbredemeyer/zync
 Author: TJ Bredemeyer
 Author-email: tj@teicor.com
 License: GNU Public License v3
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -30,14 +30,15 @@
 ```
 
 ### 2. FUNCTIONS
 
 #### logger
 
 logger takes in a string and logs it with an INFO level.  
+```
 
 ```python
 from zync import logger
 
 # logging a string INFO
 logger("info message")
```

## Comparing `zyncify-0.1.7.dist-info/RECORD` & `zyncify-0.1.8.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 zync/__init__.py,sha256=EHQzuPUyj4YgW7mibWngIWgUz5cLTUwUkACuulUmvxk,166
-zync/logger.py,sha256=eTfQJZR1g3NTIhnPGjX1QrWauC-eUY3oxGwRMv8KuQA,4946
+zync/logger.py,sha256=Juw99pIN9C-eBYsNLbfzaAkbaumdgT65Ge-7mrT-5hs,5011
 zync/logging.py,sha256=m5_OZAfXkLTDfUD-rTyPJMt9H64VQKnZELGUeRExvdA,480
-zync/main.py,sha256=zrtXrdHLzNMp3jCFTVDDiCgPwck9132pN5-If4nyIz0,1470
+zync/main.py,sha256=UV0MZlvs472ROwcU_VQvBMDVKey_SLSXtXeWHz7fBz4,1470
 zync/slugify.py,sha256=OwfO44VxBVkfqor6P7JXOVQZw8KoUFFdDvhyTGMoaqE,1228
 zync/zync.py,sha256=8v_UuFXkqXBWJoWMVPXrYaTjm44A-ebqma6aWz7C08o,966
-zyncify-0.1.7.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-zyncify-0.1.7.dist-info/METADATA,sha256=kDDRIrWBjItQFc2Bep137gzucipuHCTx1GiYWhyoFCs,2098
-zyncify-0.1.7.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-zyncify-0.1.7.dist-info/entry_points.txt,sha256=0QVFF5WXT78tlcVIjqC1XaJQCoKLt3Ift4yf5XKvang,40
-zyncify-0.1.7.dist-info/top_level.txt,sha256=mlXSVhjVoe_juOKGaECAEy2FR1Bt94xpiQhAcXNu5w0,5
-zyncify-0.1.7.dist-info/RECORD,,
+zyncify-0.1.8.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+zyncify-0.1.8.dist-info/METADATA,sha256=tlfXAztSG3zRtpTTFZM-vJokh_kunqej_fcUHwuHsEA,2102
+zyncify-0.1.8.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+zyncify-0.1.8.dist-info/entry_points.txt,sha256=0QVFF5WXT78tlcVIjqC1XaJQCoKLt3Ift4yf5XKvang,40
+zyncify-0.1.8.dist-info/top_level.txt,sha256=mlXSVhjVoe_juOKGaECAEy2FR1Bt94xpiQhAcXNu5w0,5
+zyncify-0.1.8.dist-info/RECORD,,
```

