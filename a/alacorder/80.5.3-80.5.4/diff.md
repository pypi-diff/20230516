# Comparing `tmp/alacorder-80.5.3.tar.gz` & `tmp/alacorder-80.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-80.5.3.tar", max compression
+gzip compressed data, was "alacorder-80.5.4.tar", max compression
```

## Comparing `alacorder-80.5.3.tar` & `alacorder-80.5.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.5.3/LICENSE
--rw-r--r--   0        0        0     6592 2023-05-11 17:12:36.043202 alacorder-80.5.3/README.md
--rw-r--r--   0        0        0      746 2023-05-15 02:30:04.829419 alacorder-80.5.3/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-05-14 14:20:06.372148 alacorder-80.5.3/src/alacorder/.DS_Store
--rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.5.3/src/alacorder/__init__.py
--rw-r--r--   0        0        0   272869 2023-05-15 02:28:43.447468 alacorder-80.5.3/src/alacorder/__main__.py
--rw-r--r--   0        0        0   272869 2023-05-15 02:28:29.605882 alacorder-80.5.3/src/alacorder/alac.py
--rw-r--r--   0        0        0     7563 1970-01-01 00:00:00.000000 alacorder-80.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.5.4/LICENSE
+-rw-r--r--   0        0        0     6592 2023-05-11 17:12:36.043202 alacorder-80.5.4/README.md
+-rw-r--r--   0        0        0      746 2023-05-15 14:34:13.260818 alacorder-80.5.4/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-05-15 14:34:01.441216 alacorder-80.5.4/src/alacorder/.DS_Store
+-rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.5.4/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   277118 2023-05-15 14:30:40.501222 alacorder-80.5.4/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   277118 2023-05-15 14:30:44.718399 alacorder-80.5.4/src/alacorder/alac.py
+-rw-r--r--   0        0        0     7563 1970-01-01 00:00:00.000000 alacorder-80.5.4/PKG-INFO
```

### Comparing `alacorder-80.5.3/LICENSE` & `alacorder-80.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-80.5.3/README.md` & `alacorder-80.5.4/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-80.5.3/pyproject.toml` & `alacorder-80.5.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "80.5.3"
+version = "80.5.4"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-80.5.3/src/alacorder/.DS_Store` & `alacorder-80.5.4/src/alacorder/.DS_Store`

 * *Files identical despite different names*

### Comparing `alacorder-80.5.3/src/alacorder/__main__.py` & `alacorder-80.5.4/src/alacorder/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 Optional dependencies:
     pyarrow required to export summary to .xls, .xlsx,
     Google Chrome required to fetch cases from Alacourt
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.5.3"
+version = "80.5.4"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -1605,19 +1605,14 @@
             )
             .alias("CourtAction"),
             pl.col("AllPagesText")
             .str.extract(r"Court Action Date: (\d\d?/\d\d?/\d\d\d\d)")
             .str.to_date("%m/%d/%Y", strict=False)
             .alias("CourtActionDate"),
             pl.col("AllPagesText")
-            .str.extract(r"Charge: ([A-Z\.0-9\-\s]+)")
-            .str.rstrip("C")
-            .str.strip()
-            .alias("Description"),
-            pl.col("AllPagesText")
             .str.extract(r"Jury Demand: ([A-Z]+)")
             .cast(pl.Categorical)
             .alias("JuryDemand"),
             pl.col("AllPagesText")
             .str.extract(r"Inpatient Treatment Ordered: ([YES|NO]?)")
             .cast(pl.Categorical)
             .alias("InpatientTreatmentOrdered"),
@@ -2032,15 +2027,14 @@
     cases = cases.select(
         "Retrieved",
         "CaseNumber",
         "Name",
         "DOB",
         "Race",
         "Sex",
-        "Description",
         "CourtAction",
         "CourtActionDate",
         "TotalAmtDue",
         "TotalAmtPaid",
         "TotalBalance",
         "TotalAmtHold",
         "D999",
@@ -2671,20 +2665,163 @@
     # fix missing FORF
     charges = charges.with_columns(
         [
             pl.when(pl.col("Code")=="FORF")
             .then("BOND FORF-FELONY")
             .otherwise(pl.col("Description"))
             .alias("Description"),
-            pl.when(pl.col("Code")=="T012")
+            pl.when(pl.col("Code")=="FORF")
             .then("- -BOND FORT")
             .otherwise(pl.col("Cite"))
             .alias("Cite")
         ]
     )
+    # fix missing CECE
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="CECE")
+            .then("CHEM END CHILD-EXP/CTN CTR SUB")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="CECE")
+            .then("026-015-003.2(A)(1)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing UDCS
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="UDCS")
+            .then("UNLAW DISTRIB/FURN CONT SUBST")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="UDCS")
+            .then("13A-012-211")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing PRO2
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="PRO2")
+            .then("PROMOTING PROSTITUTION 2ND")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="PRO2")
+            .then("13A-012-112")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing MCS1
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="MCS1")
+            .then("UNLAW MANF CTN SUBS 1ST DEGREE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="MCS1")
+            .then("13A-012-218")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing ACHA
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="ACHA")
+            .then("AGGRAVATED CHILD ABUSE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="ACHA")
+            .then("026-015-003.1(A)(1)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing CECD
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="CECD")
+            .then("CHEM END CHILD-DEATH")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="CECD")
+            .then("026-015-003.2(A)(3)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing T627
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="T627")
+            .then("LANE CHANGE W/O PROPER SIGNAL")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="T627")
+            .then("032-05A-133")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing FTCS
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="FTCS")
+            .then("FACILITATE TRAVEL F/ CHILD SEX")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="FTCS")
+            .then("13A-006-125")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing MCS2
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="MCS2")
+            .then("UNLAW MANF CTN SUBS 2ND DEGREE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="MCS2")
+            .then("13A-012-217")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing PRO3
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="PRO3")
+            .then("PROMOTING PROSTITUTION 3RD")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="PRO3")
+            .then("13A-012-113")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing UAUM
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="UAUM")
+            .then("UNAUTHORIZED USE MOTOR VEHICLE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="UAUM")
+            .then("032-008-081")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
     # fix missing T527
     charges = charges.with_columns(
         [
             pl.when(pl.col("Code")=="T527")
             .then("DUI-CONTROLLED SUBSTANCE")
             .otherwise(pl.col("Description"))
             .alias("Description"),
```

### Comparing `alacorder-80.5.3/src/alacorder/alac.py` & `alacorder-80.5.4/src/alacorder/alac.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 Optional dependencies:
     pyarrow required to export summary to .xls, .xlsx,
     Google Chrome required to fetch cases from Alacourt
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.5.3"
+version = "80.5.4"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -1605,19 +1605,14 @@
             )
             .alias("CourtAction"),
             pl.col("AllPagesText")
             .str.extract(r"Court Action Date: (\d\d?/\d\d?/\d\d\d\d)")
             .str.to_date("%m/%d/%Y", strict=False)
             .alias("CourtActionDate"),
             pl.col("AllPagesText")
-            .str.extract(r"Charge: ([A-Z\.0-9\-\s]+)")
-            .str.rstrip("C")
-            .str.strip()
-            .alias("Description"),
-            pl.col("AllPagesText")
             .str.extract(r"Jury Demand: ([A-Z]+)")
             .cast(pl.Categorical)
             .alias("JuryDemand"),
             pl.col("AllPagesText")
             .str.extract(r"Inpatient Treatment Ordered: ([YES|NO]?)")
             .cast(pl.Categorical)
             .alias("InpatientTreatmentOrdered"),
@@ -2032,15 +2027,14 @@
     cases = cases.select(
         "Retrieved",
         "CaseNumber",
         "Name",
         "DOB",
         "Race",
         "Sex",
-        "Description",
         "CourtAction",
         "CourtActionDate",
         "TotalAmtDue",
         "TotalAmtPaid",
         "TotalBalance",
         "TotalAmtHold",
         "D999",
@@ -2671,20 +2665,163 @@
     # fix missing FORF
     charges = charges.with_columns(
         [
             pl.when(pl.col("Code")=="FORF")
             .then("BOND FORF-FELONY")
             .otherwise(pl.col("Description"))
             .alias("Description"),
-            pl.when(pl.col("Code")=="T012")
+            pl.when(pl.col("Code")=="FORF")
             .then("- -BOND FORT")
             .otherwise(pl.col("Cite"))
             .alias("Cite")
         ]
     )
+    # fix missing CECE
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="CECE")
+            .then("CHEM END CHILD-EXP/CTN CTR SUB")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="CECE")
+            .then("026-015-003.2(A)(1)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing UDCS
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="UDCS")
+            .then("UNLAW DISTRIB/FURN CONT SUBST")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="UDCS")
+            .then("13A-012-211")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing PRO2
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="PRO2")
+            .then("PROMOTING PROSTITUTION 2ND")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="PRO2")
+            .then("13A-012-112")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing MCS1
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="MCS1")
+            .then("UNLAW MANF CTN SUBS 1ST DEGREE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="MCS1")
+            .then("13A-012-218")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing ACHA
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="ACHA")
+            .then("AGGRAVATED CHILD ABUSE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="ACHA")
+            .then("026-015-003.1(A)(1)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing CECD
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="CECD")
+            .then("CHEM END CHILD-DEATH")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="CECD")
+            .then("026-015-003.2(A)(3)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing T627
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="T627")
+            .then("LANE CHANGE W/O PROPER SIGNAL")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="T627")
+            .then("032-05A-133")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing FTCS
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="FTCS")
+            .then("FACILITATE TRAVEL F/ CHILD SEX")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="FTCS")
+            .then("13A-006-125")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing MCS2
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="MCS2")
+            .then("UNLAW MANF CTN SUBS 2ND DEGREE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="MCS2")
+            .then("13A-012-217")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing PRO3
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="PRO3")
+            .then("PROMOTING PROSTITUTION 3RD")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="PRO3")
+            .then("13A-012-113")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing UAUM
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="UAUM")
+            .then("UNAUTHORIZED USE MOTOR VEHICLE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="UAUM")
+            .then("032-008-081")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
     # fix missing T527
     charges = charges.with_columns(
         [
             pl.when(pl.col("Code")=="T527")
             .then("DUI-CONTROLLED SUBSTANCE")
             .otherwise(pl.col("Description"))
             .alias("Description"),
```

### Comparing `alacorder-80.5.3/PKG-INFO` & `alacorder-80.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 80.5.3
+Version: 80.5.4
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

