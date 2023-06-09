# Comparing `tmp/alacorder-80.5.6.tar.gz` & `tmp/alacorder-80.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-80.5.6.tar", max compression
+gzip compressed data, was "alacorder-80.5.7.tar", max compression
```

## Comparing `alacorder-80.5.6.tar` & `alacorder-80.5.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.5.6/LICENSE
--rw-r--r--   0        0        0     6592 2023-05-11 17:12:36.043202 alacorder-80.5.6/README.md
--rw-r--r--   0        0        0      746 2023-05-16 15:19:21.562814 alacorder-80.5.6/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-05-16 15:18:37.131751 alacorder-80.5.6/src/alacorder/.DS_Store
--rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.5.6/src/alacorder/__init__.py
--rw-r--r--   0        0        0   234657 2023-05-16 15:17:38.155964 alacorder-80.5.6/src/alacorder/__main__.py
--rw-r--r--   0        0        0   234657 2023-05-16 15:17:42.868372 alacorder-80.5.6/src/alacorder/alac.py
--rw-r--r--   0        0        0     7563 1970-01-01 00:00:00.000000 alacorder-80.5.6/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.5.7/LICENSE
+-rw-r--r--   0        0        0     6592 2023-05-11 17:12:36.043202 alacorder-80.5.7/README.md
+-rw-r--r--   0        0        0      746 2023-05-16 17:24:13.355658 alacorder-80.5.7/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-05-16 17:24:09.472666 alacorder-80.5.7/src/alacorder/.DS_Store
+-rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.5.7/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   236347 2023-05-16 17:23:53.664882 alacorder-80.5.7/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   236347 2023-05-16 17:23:46.278486 alacorder-80.5.7/src/alacorder/alac.py
+-rw-r--r--   0        0        0     7563 1970-01-01 00:00:00.000000 alacorder-80.5.7/PKG-INFO
```

### Comparing `alacorder-80.5.6/LICENSE` & `alacorder-80.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-80.5.6/README.md` & `alacorder-80.5.7/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-80.5.6/pyproject.toml` & `alacorder-80.5.7/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "80.5.6"
+version = "80.5.7"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-80.5.6/src/alacorder/.DS_Store` & `alacorder-80.5.7/src/alacorder/.DS_Store`

 * *Files identical despite different names*

### Comparing `alacorder-80.5.6/src/alacorder/__main__.py` & `alacorder-80.5.7/src/alacorder/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 Optional dependencies:
     pyarrow required to export summary to .xls, .xlsx,
     Google Chrome required to fetch cases from Alacourt
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.5.6"
+version = "80.5.7"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -2282,18 +2282,26 @@
             .alias("CERV_DISQ_MATCH"),
             pl.col("Code")
             .str.contains(
                 r"(RAP1|RAP2|SOD1|SOD2|STSA|SXA1|SXA2|ECHI|SX12|CSSC|FTCS|MURD|MRDI|MURR|FMUR|PMIO|POBM|MIPR|POMA|INCE)"
             )
             .alias("PARDON_DISQ_MATCH"),
             pl.col("Charges")
-            .str.contains(r"(CM\d\d|CMUR)|(CAPITAL)")
+            .str.contains(r"(CM\d\d|CMUR|CAPITAL)")
             .alias("PERM_DISQ_MATCH"),
         ]
     )
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("A_S_C_DISQ")==None)
+            .then(True)
+            .otherwise(pl.col("A_S_C_DISQ"))
+            .alias("A_S_C_DISQ")
+        ]
+    )
     charges = charges.filter(pl.col("TypeDescription").str.contains(r"[A-Za-z]"))
     charges = charges.with_columns(
         [
             pl.when(pl.col("GUILTY_PLEA") | pl.col("CONVICTED"))
             .then(True)
             .otherwise(False)
             .alias("Conviction")
@@ -2390,14 +2398,50 @@
             .alias("Description"),
             pl.when((pl.col("Code")=="VIM1") & (pl.col("Cite").eq("")))
             .then("020-002-143(A)")
             .otherwise(pl.col("Cite"))
             .alias("Cite")
         ]
     )
+    """
+    charges = charges.with_columns(
+        [
+            pl.when(
+                pl.col("Description").str.contains("CAPITAL") 
+                & pl.col("Description").str.contains(r'(A ATT|ATTEMPT|S SOLICIT|CONSP|SOLICITATION)').is_not()
+            )
+            .then(True)
+            .otherwise(pl.col("PermanentDisqCharge"))
+            .alias("PermanentDisqCharge"),
+            pl.when(
+                pl.col("Description").str.contains("CAPITAL") 
+                & pl.col("Description").str.contains(r'(A ATT|ATTEMPT|S SOLICIT|CONSP|SOLICITATION)').is_not()
+                & pl.col("Conviction")
+            )
+            .then(True)
+            .otherwise(pl.col("PermanentDisqConviction"))
+            .alias("PermanentDisqConviction"),
+            pl.when(
+                pl.col("Description").str.contains("CAPITAL") 
+                & pl.col("Description").str.contains(r'(A ATT|ATTEMPT|S SOLICIT|CONSP|SOLICITATION)').is_not()
+            )
+            .then(False)
+            .otherwise(pl.col("PardonDisqCharge"))
+            .alias("PardonDisqCharge"),
+            pl.when(
+                pl.col("Description").str.contains("CAPITAL") 
+                & pl.col("Description").str.contains(r'(A ATT|ATTEMPT|S SOLICIT|CONSP|SOLICITATION)').is_not()
+                & pl.col("Conviction")
+            )
+            .then(False)
+            .otherwise(pl.col("PardonDisqConviction"))
+            .alias("PardonDisqConviction")
+        ]
+    )
+    """
     charges = charges.with_columns(
         [
             pl.concat_str(
                 [
                     pl.col("CaseNumber"),
                     pl.lit(" - "),
                     pl.col("Num"),
@@ -2447,15 +2491,15 @@
         "CERVDisqConviction",
         "PardonDisqCharge",
         "PardonDisqConviction",
         "PermanentDisqCharge",
         "PermanentDisqConviction",
         "Filing",
         "Disposition",
-        "ChargesSummary",
+        "ChargesSummary"
     )
     dlog(charges.columns, charges.shape, cf=debug)
     return charges
 
 
 def _split_fees(df, debug=False):
     df = df.with_columns(
```

### Comparing `alacorder-80.5.6/src/alacorder/alac.py` & `alacorder-80.5.7/src/alacorder/alac.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 Optional dependencies:
     pyarrow required to export summary to .xls, .xlsx,
     Google Chrome required to fetch cases from Alacourt
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.5.6"
+version = "80.5.7"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -2282,18 +2282,26 @@
             .alias("CERV_DISQ_MATCH"),
             pl.col("Code")
             .str.contains(
                 r"(RAP1|RAP2|SOD1|SOD2|STSA|SXA1|SXA2|ECHI|SX12|CSSC|FTCS|MURD|MRDI|MURR|FMUR|PMIO|POBM|MIPR|POMA|INCE)"
             )
             .alias("PARDON_DISQ_MATCH"),
             pl.col("Charges")
-            .str.contains(r"(CM\d\d|CMUR)|(CAPITAL)")
+            .str.contains(r"(CM\d\d|CMUR|CAPITAL)")
             .alias("PERM_DISQ_MATCH"),
         ]
     )
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("A_S_C_DISQ")==None)
+            .then(True)
+            .otherwise(pl.col("A_S_C_DISQ"))
+            .alias("A_S_C_DISQ")
+        ]
+    )
     charges = charges.filter(pl.col("TypeDescription").str.contains(r"[A-Za-z]"))
     charges = charges.with_columns(
         [
             pl.when(pl.col("GUILTY_PLEA") | pl.col("CONVICTED"))
             .then(True)
             .otherwise(False)
             .alias("Conviction")
@@ -2390,14 +2398,50 @@
             .alias("Description"),
             pl.when((pl.col("Code")=="VIM1") & (pl.col("Cite").eq("")))
             .then("020-002-143(A)")
             .otherwise(pl.col("Cite"))
             .alias("Cite")
         ]
     )
+    """
+    charges = charges.with_columns(
+        [
+            pl.when(
+                pl.col("Description").str.contains("CAPITAL") 
+                & pl.col("Description").str.contains(r'(A ATT|ATTEMPT|S SOLICIT|CONSP|SOLICITATION)').is_not()
+            )
+            .then(True)
+            .otherwise(pl.col("PermanentDisqCharge"))
+            .alias("PermanentDisqCharge"),
+            pl.when(
+                pl.col("Description").str.contains("CAPITAL") 
+                & pl.col("Description").str.contains(r'(A ATT|ATTEMPT|S SOLICIT|CONSP|SOLICITATION)').is_not()
+                & pl.col("Conviction")
+            )
+            .then(True)
+            .otherwise(pl.col("PermanentDisqConviction"))
+            .alias("PermanentDisqConviction"),
+            pl.when(
+                pl.col("Description").str.contains("CAPITAL") 
+                & pl.col("Description").str.contains(r'(A ATT|ATTEMPT|S SOLICIT|CONSP|SOLICITATION)').is_not()
+            )
+            .then(False)
+            .otherwise(pl.col("PardonDisqCharge"))
+            .alias("PardonDisqCharge"),
+            pl.when(
+                pl.col("Description").str.contains("CAPITAL") 
+                & pl.col("Description").str.contains(r'(A ATT|ATTEMPT|S SOLICIT|CONSP|SOLICITATION)').is_not()
+                & pl.col("Conviction")
+            )
+            .then(False)
+            .otherwise(pl.col("PardonDisqConviction"))
+            .alias("PardonDisqConviction")
+        ]
+    )
+    """
     charges = charges.with_columns(
         [
             pl.concat_str(
                 [
                     pl.col("CaseNumber"),
                     pl.lit(" - "),
                     pl.col("Num"),
@@ -2447,15 +2491,15 @@
         "CERVDisqConviction",
         "PardonDisqCharge",
         "PardonDisqConviction",
         "PermanentDisqCharge",
         "PermanentDisqConviction",
         "Filing",
         "Disposition",
-        "ChargesSummary",
+        "ChargesSummary"
     )
     dlog(charges.columns, charges.shape, cf=debug)
     return charges
 
 
 def _split_fees(df, debug=False):
     df = df.with_columns(
```

### Comparing `alacorder-80.5.6/PKG-INFO` & `alacorder-80.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 80.5.6
+Version: 80.5.7
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

