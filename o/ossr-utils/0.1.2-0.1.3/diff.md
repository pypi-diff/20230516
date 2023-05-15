# Comparing `tmp/ossr_utils-0.1.2.tar.gz` & `tmp/ossr_utils-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ossr_utils-0.1.2.tar", max compression
+gzip compressed data, was "ossr_utils-0.1.3.tar", max compression
```

## Comparing `ossr_utils-0.1.2.tar` & `ossr_utils-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       67 2023-05-12 16:15:06.843492 ossr_utils-0.1.2/README.md
--rw-r--r--   0        0        0      355 2023-05-12 18:44:30.526672 ossr_utils-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      112 2023-05-12 18:39:40.636726 ossr_utils-0.1.2/src/ossr_utils/__init__.py
--rw-r--r--   0        0        0      443 2023-05-12 16:08:56.032271 ossr_utils-0.1.2/src/ossr_utils/audio_utils.py
--rw-r--r--   0        0        0      981 2023-01-10 22:55:56.183254 ossr_utils-0.1.2/src/ossr_utils/fft_utils.py
--rw-r--r--   0        0        0      492 2023-05-11 15:05:58.393123 ossr_utils-0.1.2/src/ossr_utils/io_utils.py
--rw-r--r--   0        0        0     4831 2023-05-11 15:18:51.415248 ossr_utils-0.1.2/src/ossr_utils/misc_utils.py
--rw-r--r--   0        0        0      992 2023-01-27 15:44:16.196447 ossr_utils-0.1.2/src/ossr_utils/model_utils.py
--rw-r--r--   0        0        0      591 1970-01-01 00:00:00.000000 ossr_utils-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       67 2023-05-12 16:15:06.843492 ossr_utils-0.1.3/README.md
+-rw-r--r--   0        0        0      395 2023-05-15 22:58:28.914041 ossr_utils-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      116 2023-05-15 18:37:40.105429 ossr_utils-0.1.3/src/ossr_utils/__init__.py
+-rw-r--r--   0        0        0      443 2023-05-12 16:08:56.032271 ossr_utils-0.1.3/src/ossr_utils/audio_utils.py
+-rw-r--r--   0        0        0      981 2023-01-10 22:55:56.183254 ossr_utils-0.1.3/src/ossr_utils/fft_utils.py
+-rw-r--r--   0        0        0      492 2023-05-15 20:13:33.573563 ossr_utils-0.1.3/src/ossr_utils/io_utils.py
+-rw-r--r--   0        0        0     4836 2023-05-15 22:51:53.740635 ossr_utils-0.1.3/src/ossr_utils/misc_utils.py
+-rw-r--r--   0        0        0      992 2023-01-27 15:44:16.196447 ossr_utils-0.1.3/src/ossr_utils/model_utils.py
+-rw-r--r--   0        0        0      673 1970-01-01 00:00:00.000000 ossr_utils-0.1.3/PKG-INFO
```

### Comparing `ossr_utils-0.1.2/src/ossr_utils/fft_utils.py` & `ossr_utils-0.1.3/src/ossr_utils/fft_utils.py`

 * *Files identical despite different names*

### Comparing `ossr_utils-0.1.2/src/ossr_utils/misc_utils.py` & `ossr_utils-0.1.3/src/ossr_utils/misc_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 
 
 def get_seg_amp_metric(wf):
     """Calculate audio segment amplitude metric"""
-    return np.max(np.abs(wf))
+    return int(np.max(np.abs(wf)))
 
 
 def get_ts_now():
     """Get current time in UTC milliseconds"""
     return int(1e3 * time.time())
 
 def print_df_full(df: pd.DataFrame,
```

### Comparing `ossr_utils-0.1.2/src/ossr_utils/model_utils.py` & `ossr_utils-0.1.3/src/ossr_utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `ossr_utils-0.1.2/PKG-INFO` & `ossr_utils-0.1.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: ossr-utils
-Version: 0.1.2
+Version: 0.1.3
 Summary: Utils for the Open-Set Sound Recognition (OSSR) system
 License: MIT
 Author: Johannes Traa
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
+Requires-Dist: pandas (>=2.0.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # ossr_utils
 Utility methods for Open-Set Sound Recognition system
```

