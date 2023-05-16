# Comparing `tmp/premise_gwp-0.8.tar.gz` & `tmp/premise_gwp-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "premise_gwp-0.8.tar", last modified: Tue Apr 18 11:58:23 2023, max compression
+gzip compressed data, was "premise_gwp-0.9.tar", last modified: Tue May 16 09:34:23 2023, max compression
```

## Comparing `premise_gwp-0.8.tar` & `premise_gwp-0.9.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:58:23.861937 premise_gwp-0.8/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-18 11:58:14.000000 premise_gwp-0.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-04-18 11:58:14.000000 premise_gwp-0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-18 11:58:14.000000 premise_gwp-0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-04-18 11:58:23.861937 premise_gwp-0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-18 11:58:14.000000 premise_gwp-0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:58:23.857936 premise_gwp-0.8/premise_gwp/
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-04-18 11:58:14.000000 premise_gwp-0.8/premise_gwp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-18 11:58:14.000000 premise_gwp-0.8/premise_gwp/biosphere.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:58:23.857936 premise_gwp-0.8/premise_gwp/data/
--rw-r--r--   0 runner    (1001) docker     (123)    84350 2023-04-18 11:58:14.000000 premise_gwp-0.8/premise_gwp/data/LCIA_Implementation_3.8.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    13174 2023-04-18 11:58:14.000000 premise_gwp-0.8/premise_gwp/data/lcia_gtp_100a_w_bio.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-04-18 11:58:14.000000 premise_gwp-0.8/premise_gwp/data/lcia_gtp_20a_w_bio.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    13118 2023-04-18 11:58:14.000000 premise_gwp-0.8/premise_gwp/data/lcia_gwp_100a.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    13252 2023-04-18 11:58:14.000000 premise_gwp-0.8/premise_gwp/data/lcia_gwp_100a_w_bio.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    13217 2023-04-18 11:58:14.000000 premise_gwp-0.8/premise_gwp/data/lcia_gwp_20a.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    13286 2023-04-18 11:58:14.000000 premise_gwp-0.8/premise_gwp/data/lcia_gwp_20a_w_bio.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-18 11:58:14.000000 premise_gwp-0.8/premise_gwp/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:58:23.857936 premise_gwp-0.8/premise_gwp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-04-18 11:58:23.000000 premise_gwp-0.8/premise_gwp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-18 11:58:23.000000 premise_gwp-0.8/premise_gwp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 11:58:23.000000 premise_gwp-0.8/premise_gwp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-18 11:58:23.000000 premise_gwp-0.8/premise_gwp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-18 11:58:23.000000 premise_gwp-0.8/premise_gwp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-18 11:58:14.000000 premise_gwp-0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 11:58:23.861937 premise_gwp-0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-18 11:58:14.000000 premise_gwp-0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:58:23.861937 premise_gwp-0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-18 11:58:14.000000 premise_gwp-0.8/tests/test_implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:34:23.283338 premise_gwp-0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-16 09:34:13.000000 premise_gwp-0.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-16 09:34:13.000000 premise_gwp-0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-16 09:34:13.000000 premise_gwp-0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-16 09:34:23.283338 premise_gwp-0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-05-16 09:34:13.000000 premise_gwp-0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:34:23.283338 premise_gwp-0.9/premise_gwp/
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-05-16 09:34:13.000000 premise_gwp-0.9/premise_gwp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-16 09:34:13.000000 premise_gwp-0.9/premise_gwp/biosphere.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:34:23.283338 premise_gwp-0.9/premise_gwp/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    13833 2023-05-16 09:34:13.000000 premise_gwp-0.9/premise_gwp/data/lcia_gwp2021_100a.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    13857 2023-05-16 09:34:13.000000 premise_gwp-0.9/premise_gwp/data/lcia_gwp2021_100a_w_bio.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    13947 2023-05-16 09:34:13.000000 premise_gwp-0.9/premise_gwp/data/lcia_gwp2021_20a.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    14004 2023-05-16 09:34:13.000000 premise_gwp-0.9/premise_gwp/data/lcia_gwp2021_20a_w_bio.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    13118 2023-05-16 09:34:13.000000 premise_gwp-0.9/premise_gwp/data/lcia_gwp_100a.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    13252 2023-05-16 09:34:13.000000 premise_gwp-0.9/premise_gwp/data/lcia_gwp_100a_w_bio.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    13217 2023-05-16 09:34:13.000000 premise_gwp-0.9/premise_gwp/data/lcia_gwp_20a.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    13286 2023-05-16 09:34:13.000000 premise_gwp-0.9/premise_gwp/data/lcia_gwp_20a_w_bio.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 09:34:13.000000 premise_gwp-0.9/premise_gwp/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:34:23.283338 premise_gwp-0.9/premise_gwp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-16 09:34:23.000000 premise_gwp-0.9/premise_gwp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-16 09:34:23.000000 premise_gwp-0.9/premise_gwp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 09:34:23.000000 premise_gwp-0.9/premise_gwp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-16 09:34:23.000000 premise_gwp-0.9/premise_gwp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-16 09:34:23.000000 premise_gwp-0.9/premise_gwp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-16 09:34:13.000000 premise_gwp-0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 09:34:23.283338 premise_gwp-0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-16 09:34:13.000000 premise_gwp-0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:34:23.283338 premise_gwp-0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-16 09:34:13.000000 premise_gwp-0.9/tests/test_implementation.py
```

### Comparing `premise_gwp-0.8/LICENSE` & `premise_gwp-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `premise_gwp-0.8/PKG-INFO` & `premise_gwp-0.9/premise_gwp.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: premise_gwp
-Version: 0.8
+Name: premise-gwp
+Version: 0.9
 Summary: Import IPCC's GWP100a method, with biogenic CO2 CFs, into Brightway2
 Home-page: https://github.com/romainsacchi/premise_gwp
 Author: Romain Sacchi
 Author-email: romain.sacchi@psi.ch
 License: BSD 3-clause
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
@@ -32,33 +32,35 @@
 Without it, negative emission technologies (NET) do not yield a net negative
 carbon footprint.
 
 ## Impact category
 
 This adds:
 
-* IPCC 2013, climate change, GWP 100a, with hydrogen
+* IPCC 2013 and 2021, climate change, GWP 100a, with hydrogen
   * "Hydrogen", with a CF of 33 and 11 for GWP20 and GWP100 respectively.
   
-* IPCC 2013, climate change, GWP 100a, with hydrogen and bio CO2
+* IPCC 2013 and 2021, climate change, GWP 100a, with hydrogen and bio CO2
   * "Hydrogen", with a CF of 33 and 11 for GWP20 and GWP100 respectively.
   * "Carbon dioxide, in air", with a CF of -1
   * "Carbon dioxide, non-fossil, resource correction", with a CF of -1
   * "Carbon dioxide, non-fossil", with a CF of +1
 
 The biogenic carbon balance in the rest of the ecoinvent database should be correct.
-Hence, using this method, instead of the regular IPCC 2013 GWP100a method, should not
+Hence, using this method, instead of the regular IPCC GWP method, should not
 yield any difference, as long as BECCS are not present and solicited in the database.
 
 The characterization factors for the global warming impact GWP100a of for hydrogen 
 is taken from [Warwick et al, 2022](https://assets.publishing.service.gov.uk/government/uploads/system/uploads/attachment_data/file/1067144/atmospheric-implications-of-increased-hydrogen-use.pdf).
 
 ## Limitation
 
-Only works with ``bw2io 0.8.7`` or earlier (until ecoinvent v.3.8).
+Now works with ``bw2io 0.8.7`` and ``bw2io 0.8.8``. 
+If ``bw2io 0.8.8`` is present, IPCC 2021 methods will be
+installed, otherwise IPCC 2013 methods will be installed.
 
 ## Usage
 
 In an open Brightway2 project:
 ```python
 from premise_gwp import add_premise_gwp
 add_premise_gwp()
```

### Comparing `premise_gwp-0.8/README.md` & `premise_gwp-0.9/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -9,33 +9,35 @@
 Without it, negative emission technologies (NET) do not yield a net negative
 carbon footprint.
 
 ## Impact category
 
 This adds:
 
-* IPCC 2013, climate change, GWP 100a, with hydrogen
+* IPCC 2013 and 2021, climate change, GWP 100a, with hydrogen
   * "Hydrogen", with a CF of 33 and 11 for GWP20 and GWP100 respectively.
   
-* IPCC 2013, climate change, GWP 100a, with hydrogen and bio CO2
+* IPCC 2013 and 2021, climate change, GWP 100a, with hydrogen and bio CO2
   * "Hydrogen", with a CF of 33 and 11 for GWP20 and GWP100 respectively.
   * "Carbon dioxide, in air", with a CF of -1
   * "Carbon dioxide, non-fossil, resource correction", with a CF of -1
   * "Carbon dioxide, non-fossil", with a CF of +1
 
 The biogenic carbon balance in the rest of the ecoinvent database should be correct.
-Hence, using this method, instead of the regular IPCC 2013 GWP100a method, should not
+Hence, using this method, instead of the regular IPCC GWP method, should not
 yield any difference, as long as BECCS are not present and solicited in the database.
 
 The characterization factors for the global warming impact GWP100a of for hydrogen 
 is taken from [Warwick et al, 2022](https://assets.publishing.service.gov.uk/government/uploads/system/uploads/attachment_data/file/1067144/atmospheric-implications-of-increased-hydrogen-use.pdf).
 
 ## Limitation
 
-Only works with ``bw2io 0.8.7`` or earlier (until ecoinvent v.3.8).
+Now works with ``bw2io 0.8.7`` and ``bw2io 0.8.8``. 
+If ``bw2io 0.8.8`` is present, IPCC 2021 methods will be
+installed, otherwise IPCC 2013 methods will be installed.
 
 ## Usage
 
 In an open Brightway2 project:
 ```python
 from premise_gwp import add_premise_gwp
 add_premise_gwp()
```

### Comparing `premise_gwp-0.8/premise_gwp/__init__.py` & `premise_gwp-0.9/premise_gwp/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,23 +6,24 @@
 from pathlib import Path
 
 DATA_DIR = Path(__file__).resolve().parent / "data"
 
 import bw2io
 from bw2io import ExcelLCIAImporter
 
-from .biosphere import check_biosphere_database
+from .biosphere import check_biosphere_database, check_biosphere_version
 from .version import version as __version__
 
 
 def add_premise_gwp():
     check_biosphere_database()
+    bw2io_version = check_biosphere_version()
 
     # impact methods to create
-    categories = {
+    categories_bw2io087 = {
         (
             ("IPCC 2013", "climate change", "GWP 20a, incl. H"),
             "kg CO2-Eq",
             "IPCC 2013, with CFs for hydrogen",
             "lcia_gwp_20a.xlsx",
         ),
         (
@@ -39,28 +40,47 @@
         ),
         (
             ("IPCC 2013", "climate change", "GWP 100a, incl. H and bio CO2"),
             "kg CO2-Eq",
             "IPCC 2013, with CFs for hydrogen and biogenic CO2 flows",
             "lcia_gwp_100a_w_bio.xlsx",
         ),
+    }
+
+    categories_bw2io088 = {
+        (
+            ("IPCC 2021", "climate change", "GWP 20a, incl. H"),
+            "kg CO2-Eq",
+            "IPCC 2021, with CFs for hydrogen",
+            "lcia_gwp2021_20a.xlsx",
+        ),
         (
-            ("IPCC 2013", "climate change", "GTP 20a, incl. bio CO2"),
+            ("IPCC 2021", "climate change", "GWP 100a, incl. H"),
             "kg CO2-Eq",
-            "IPCC 2013, with CFs for biogenic CO2 flows",
-            "lcia_gtp_20a_w_bio.xlsx",
+            "IPCC 2021, with CFs for hydrogen",
+            "lcia_gwp2021_100a.xlsx",
         ),
         (
-            ("IPCC 2013", "climate change", "GTP 100a, incl. bio CO2"),
+            ("IPCC 2021", "climate change", "GWP 20a, incl. H and bio CO2"),
             "kg CO2-Eq",
-            "IPCC 2013, with CFs for biogenic CO2 flows",
-            "lcia_gtp_100a_w_bio.xlsx",
+            "IPCC 2021, with CFs for hydrogen and biogenic CO2 flows",
+            "lcia_gwp2021_20a_w_bio.xlsx",
+        ),
+        (
+            ("IPCC 2021", "climate change", "GWP 100a, incl. H and bio CO2"),
+            "kg CO2-Eq",
+            "IPCC 2021, with CFs for hydrogen and biogenic CO2 flows",
+            "lcia_gwp2021_100a_w_bio.xlsx",
         ),
     }
 
+    categories = (
+        categories_bw2io088 if bw2io_version >= (0, 8, 8) else categories_bw2io087
+    )
+
     for c in categories:
         print("Adding {}".format(c[0]))
         category = ExcelLCIAImporter(
             filepath=DATA_DIR / c[-1], name=c[0], unit=c[1], description=c[2]
         )
 
         # apply formatting strategies
```

### Comparing `premise_gwp-0.8/premise_gwp/data/lcia_gtp_100a_w_bio.xlsx` & `premise_gwp-0.9/premise_gwp/data/lcia_gwp_100a_w_bio.xlsx`

 * *Files 26% similar despite different names*

```diff
@@ -137,688 +137,693 @@
 00000880: cbb4 e480 fa84 53ec ad82 b4b7 b720 9a29  ......S...... .)
 00000890: 66e5 ffb9 43db f606 9f82 791f d1f3 1909  f...C.....y.....
 000008a0: 493c 0d79 00d1 e8d4 212b f8c1 45f6 08f2  I<.y....!+..E...
 000008b0: bcfc 664d 79ce 6bc1 a3fa 0ce5 1cab 4b1e  ..fMy.k.......K.
 000008c0: aa35 3d7c 8674 2087 c847 1f7f 2992 73e5  .5=|.t ..G..).s.
 000008d0: a299 bb55 efe1 7442 fbca 29bf dbf2 2ccb  ...U..tB..)...,.
 000008e0: f4ef 66e4 c9c7 d5df 0000 00ff ff03 0050  ..f............P
-000008f0: 4b03 0414 0006 0008 0000 0021 0037 dd59  K..........!.7.Y
-00000900: 6503 0300 0009 0700 000f 0000 0078 6c2f  e............xl/
+000008f0: 4b03 0414 0006 0008 0000 0021 0008 2fba  K..........!../.
+00000900: 2502 0300 0009 0700 000f 0000 0078 6c2f  %............xl/
 00000910: 776f 726b 626f 6f6b 2e78 6d6c ac55 db6e  workbook.xml.U.n
-00000920: e230 107d 5f69 ff21 f27b ea38 4008 5143  .0.}_i.!.{.8@.QC
-00000930: 556e bb48 ed6e d5eb 6365 1243 2c12 3b6b  Un.H.n..ce.C,.;k
-00000940: 3b85 aaea bfef 3810 28e5 a5db 6e04 be8d  ;.....8.(...n...
-00000950: 7372 66e6 8c7d 7ab6 2e72 e789 29cd a588  srf..}z..r..)...
-00000960: 1139 f190 c344 2253 2e16 31ba bb9d b821  .9...D"S..1....!
-00000970: 72b4 a122 a5b9 142c 46cf 4ca3 b3fe f76f  r.."...,F.L....o
-00000980: a72b a996 3329 970e 0008 1da3 cc98 32c2  .+..3)........2.
-00000990: 5827 192b a83e 9125 1360 994b 5550 0353  X'.+.>.%.`.KUP.S
-000009a0: b5c0 ba54 8ca6 3a63 cc14 39f6 3d2f c005  ...T..:c..9.=/..
-000009b0: e502 6d10 22f5 110c 399f f384 8d64 5215  ..m."...9....dR.
-000009c0: 4c98 0d88 6239 3540 5f67 bcd4 0d5a 917c  L...b95@_g...Z.|
-000009d0: 04ae a06a 5995 6e22 8b12 2066 3ce7 e6b9  ...jY.n".. f<...
-000009e0: 0645 4e91 44d3 8590 8ace 7270 7b4d 3ace  .EN.D.....rp{M:.
-000009f0: 5ac1 2f80 3ff1 a0f1 9b2f 81e9 e853 054f  Z./.?..../...S.O
-00000a00: 94d4 726e 4e00 1a6f 481f f94f 3c4c c841  ..rnN..oH..O<L.A
-00000a10: 08d6 c731 f818 521b 2bf6 c46d 0e77 ac54  ...1..R.+..m.w.T
-00000a20: f049 56c1 0e2b d883 11ef cb68 04a4 556b  .IV..+.....h..Uk
-00000a30: 2582 e07d 12ad b3e3 e6a3 fee9 9ce7 ec7e  %..}...........~
-00000a40: 235d 8796 e52f 5ad8 4ce5 c8c9 a936 e394  #].../Z.L....6..
-00000a50: 1b96 c6a8 0b53 b962 fb05 f04a 55e5 a0e2  .....S.b...JU...
-00000a60: 3958 89d7 223e c2fd 9d9c af94 93b2 39ad  9X..">........9.
-00000a70: 7273 0b42 6ee0 6163 10f4 fc8e dd09 c238  rs.Bn.ac.......8
-00000a80: cf0d 5382 1a36 94c2 800e b77e 7d55 7335  ..S..6.....~}Us5
-00000a90: f630 93a0 70e7 9afd a9b8 6250 58a0 2ff0  .0..p.....bPX./.
-00000aa0: 155a 9a44 74a6 afa8 c99c 4ae5 31c2 771a  .Z.Dt.....J.1.w.
-00000ab0: 9cc7 4ada 2ac2 3fb8 f959 cd30 d458 c135  ..J.*.?..Y.0.X.5
-00000ac0: 7b5c acca 8371 4a0d c56f 244b 8feb e31f  {\...qJ..o$K....
-00000ad0: 444b 131b 090c a1d8 d0dd 8cdf 8705 58ab  DK............X.
-00000ae0: a811 e695 510e 8ca7 a30b 48ce 0d7d 8254  ....Q.....H..}.T
-00000af0: 8120 d26d 254f 6d2e 5a8f 2251 1179 7c19  . .m%Om.Z."Q.y|.
-00000b00: 84c3 a0d7 f3bb eed0 9fb4 dc71 a73d 7043  ...........q.=pC
-00000b10: 6fd0 71db a349 1876 cf07 de68 3879 0567  o.q..I.v...h8y.g
-00000b20: 5410 2592 5626 dbaa c042 c7a8 0d29 3f32  T.%.V&...B...)?2
-00000b30: 5dd2 7563 215e 54f1 744f e3c5 db3e aeed  ].uc!^T.tO...>..
-00000b40: df35 8ded d53a 6ccf bb7b ce56 7aaf 173b  .5...:l..{.Vz..;
-00000b50: 75d6 0f5c a472 557b f4dc 8cbb 01f8 b7aa  u..\.rU{........
-00000b60: 0d0f 3c35 598c fc30 f476 6b3f 195f 64c0  ..<5Y..0.vk?._d.
-00000b70: 96b4 3a76 116a c2b2 8ad1 019b d186 cd04  ..:v.j..........
-00000b80: 1ed7 3607 6cf0 1b3a f5a9 0ab4 eade 1175  ..6.l..:.......u
-00000b90: 25dc d893 96c0 f16d fb3a c0a0 fcc8 7e43  %......m.:....~C
-00000ba0: 4d53 5227 b079 2da1 7902 cab7 5dbd 31f0  MSR'.y-.y...].1.
-00000bb0: 7ba4 85ea f9a5 4c21 5505 1515 85ca b23b  {.....L!U......;
-00000bc0: 7e8b 267d 1012 b636 17da d43d a892 037f  ~.&}...6...=....
-00000bd0: d2f6 cebb 5eaf ed7a e316 a42c ecf9 6ed8  ....^..z...,..n.
-00000be0: 6ef9 eeb0 3df2 c79d ee78 341e 746c f2ec  n...=....x4.tl..
-00000bf0: b511 fd8f c3b3 2e8e a8b9 8fac 1b19 55e6  ..............U.
-00000c00: 56d1 6409 b7d8 359b 0fa8 0617 361e 035f  V.d...5.....6.._
-00000c10: 106b c31a 376f f5ff 0200 00ff ff03 0050  .k..7o.........P
-00000c20: 4b03 0414 0006 0008 0000 0021 0027 96d6  K..........!.'..
-00000c30: b5ca 0200 000a 0700 000d 0000 0078 6c2f  .............xl/
-00000c40: 7374 796c 6573 2e78 6d6c b455 db6e db30  styles.xml.U.n.0
-00000c50: 0c7d 1fb0 7f10 f4ee ca76 e32c 096c 174b  .}.......v.,.l.K
-00000c60: 5303 05b6 6140 3b60 af8a 2d27 4275 3124  S...a@;`..-'Bu1$
-00000c70: 2573 36ec df47 d94e e2a2 ddad c35e 6289  %s6..G.N.....^b.
-00000c80: 120f 0f0f 2926 bd6a a540 7b66 2cd7 2ac3  ....)&.j.@{f,.*.
-00000c90: d145 8811 53a5 aeb8 da64 f8d3 7d11 cc30  .E..S....d..}..0
-00000ca0: b28e aa8a 0aad 5886 0fcc e2ab fcf5 abd4  ......X.........
-00000cb0: ba83 6077 5bc6 1c02 0865 33bc 75ae 5910  ..`w[....e3.u.Y.
-00000cc0: 62cb 2d93 d45e e886 2938 a9b5 91d4 c1d6  b.-..^..)8......
-00000cd0: 6c88 6d0c a395 f54e 5290 380c a744 52ae  l.m....NR.8..DR.
-00000ce0: 708f b090 e59f 8048 6a1e 764d 506a d950  p......Hj.vMPj.P
-00000cf0: c7d7 5c70 77e8 b030 92e5 e276 a3b4 a16b  ..\pw..0...v...k
-00000d00: 0154 db68 424b d446 5313 a3d6 1c83 74d6  .T.hBK.FS.....t.
-00000d10: 2771 242f 8db6 ba76 1780 4b74 5df3 923d  'q$/...v..Kt]..=
-00000d20: a53b 2773 42cb 3312 20bf 0c29 4a48 183f  .;'sB.3. ..)JH.?
-00000d30: cabd 352f 449a 10c3 f6dc 970f e769 ad95  ..5/D........i..
-00000d40: b3a8 d43b e532 1c03 512f c1e2 41e9 2faa  ...;.2..Q/..A./.
-00000d50: f047 50e1 e156 9eda af68 4f05 5862 4cf2  .GP..V...hO.XbL.
-00000d60: b4d4 421b e4a0 74a0 5ce4 2d8a 4ad6 dfb8  ..B...t.\.-.J...
-00000d70: a682 af0d f7c6 9a4a 2e0e bdb9 f3eb aa3d  .......J.......=
-00000d80: dc93 1cb4 f7b7 88e7 d1b3 c9d3 3518 fe7f  ............5...
-00000d90: ac2e a485 985c 8891 02bd 214f a155 1c33  .....\....!O.U.3
-00000da0: aa80 5334 acef 0f0d a4aa a0ab 7bca 70f4  ..S4........{.p.
-00000db0: dbdb 1b43 0f51 9c8c 1c48 1710 b2d4 a682  ...C.Q...H......
-00000dc0: 5774 d4de cbdc 9bf2 54b0 da81 0686 6fb6  Wt......T.....o.
-00000dd0: feeb 7403 bf6b ed1c 745a 9e56 9c6e b4a2  ..t..k..tZ.V.n..
-00000de0: c2cb 76f4 1816 904e c984 b8f3 2fed 73fd  ..v....N..../.s.
-00000df0: 08bb ad91 dac9 42ba db2a c3f0 66bd e0c7  ......B..*..f...
-00000e00: 2524 322c 7bbc 7ee3 f1c7 683d f608 3606  %$2,{.~...h=..6.
-00000e10: ca7f 0f8b dafa 84ff 33ef 08f8 3d4f eae4  ........3...=O..
-00000e20: 8d68 d388 83ef d1a1 fb3a aec0 6e24 c123  .h.......:..n$.#
-00000e30: 014e a920 dfa7 19fe e0c7 8c80 8e1f e8a0  .N. ............
-00000e40: f58e 0bc7 d533 c903 66d5 9ee5 0c7d 359d  .....3..f....}5.
-00000e50: 1f19 9dd0 a728 a06a c56a ba13 eefe 7498  .....(.j.j....t.
-00000e60: e1f3 fa3d abf8 4ec2 231b 6e7d e47b ed3a  ...=..N.#.n}.{.:
-00000e70: 880c 9fd7 ef7c d5a3 a98f c15a f7ce c2b3  .....|.....Z....
-00000e80: 802f da19 9ee1 6f37 cb37 f3d5 4d11 07b3  ./....o7.7..M...
-00000e90: 7039 0b26 972c 09e6 c972 1524 93eb e56a  p9.&.,...r.$...j
-00000ea0: 55cc c338 bcfe 3e1a 5cff 30b6 ba39 0b05  U..8..>.\.0..9..
-00000eb0: 8e26 0b2b 60b8 9921 d981 fcdd d996 e1d1  .&.+`..!........
-00000ec0: a6a7 dff5 3bd0 1e73 9fc7 d3f0 6d12 8541  ....;..s....m..A
-00000ed0: 7119 46c1 644a 67c1 6c7a 9904 4512 c5ab  q.F.dJg.lz..E...
-00000ee0: e964 7993 14c9 887b f2c2 f116 9228 ea07  .dy....{.....(..
-00000ef0: a527 9f2c 1c97 4c70 75ac d5b1 4263 2b14  .'.,..Lpu...Bc+.
-00000f00: 09b6 bf48 821c 2b41 ce7f 62f9 0f00 0000  ...H..+A..b.....
-00000f10: ffff 0300 504b 0304 1400 0600 0800 0000  ....PK..........
-00000f20: 2100 c117 10be 4e07 0000 c620 0000 1300  !.....N.... ....
-00000f30: 0000 786c 2f74 6865 6d65 2f74 6865 6d65  ..xl/theme/theme
-00000f40: 312e 786d 6cec 59cd 8b1b 3714 bf17 fa3f  1.xml.Y...7....?
-00000f50: 0c73 77fc 35e3 8f25 dee0 cf6c 93dd 2464  .sw.5..%...l..$d
-00000f60: 9d94 1cb5 b6ec 5156 3332 92bc 1b13 0225  ......QV32.....%
-00000f70: 39f5 5228 a4a5 9742 6f3d 94d2 4003 0dbd  9.R(...Bo=..@...
-00000f80: f48f 0924 b4e9 1fd1 27cd d823 ade5 249b  ...$....'..#..$.
-00000f90: 6c4a 5a76 0d8b 47fe bda7 a7f7 9e7e 7af3  lJZv..G......~z.
-00000fa0: 74f1 d2bd 987a 4798 0bc2 9296 5fbe 50f2  t....zG....._.P.
-00000fb0: 3d9c 8cd8 9824 d396 7f6b 3828 347c 4f48  =....$...k8(4|OH
-00000fc0: 948c 1165 096e f90b 2cfc 4bdb 9f7e 7211  ...e.n..,.K..~r.
-00000fd0: 6dc9 08c7 d803 f944 6ca1 961f 4939 db2a  m......Dl...I9.*
-00000fe0: 16c5 0886 91b8 c066 3881 df26 8cc7 48c2  .......f8..&..H.
-00000ff0: 239f 16c7 1c1d 83de 9816 2ba5 52ad 1823  #.........+.R..#
-00001000: 92f8 5e82 6250 7b7d 3221 23ec 0d95 4a7f  ..^.bP{}2!#...J.
-00001010: 7ba9 bc4f e131 9142 0d8c 28df 57aa b125  {..O.1.B..(.W..%
-00001020: a1b1 e3c3 b242 8885 e852 ee1d 21da f261  .....B...R..!..a
-00001030: 9e31 3b1e e27b d2f7 2812 127e 68f9 25fd  .1;..{..(..~h.%.
-00001040: e717 b72f 16d1 5626 44e5 0659 436e a0ff  .../..V&D..YCn..
-00001050: 32b9 4c60 7c58 d173 f2e9 c16a d220 0883  2.L`|X.s...j. ..
-00001060: 5a7b a55f 03a8 5cc7 f5eb fd5a bfb6 d2a7  Z{._..\....Z....
-00001070: 0168 3482 95a6 b6d8 3aeb 956e 9061 0d50  .h4.....:..n.a.P
-00001080: fad5 a1bb 57ef 55cb 16de d05f 5db3 b91d  ....W.U...._]...
-00001090: aa8f 85d7 a054 7fb0 861f 0cba e045 0baf  .....T.......E..
-000010a0: 4129 3e5c c387 9d66 a767 ebd7 a014 5f5b  A)>\...f.g...._[
-000010b0: c3d7 4bed 5e50 b7f4 6b50 4449 72b8 862e  ..K.^P..kPDIr...
-000010c0: 85b5 6a77 b9da 1564 c2e8 8e13 de0c 8341  ..jw...d.......A
-000010d0: bd92 29cf 5190 0dab ec52 534c 5822 37e5  ..).Q....RSLX"7.
-000010e0: 5a8c ee32 3e00 8002 5224 49e2 c9c5 0c4f  Z..2>...R$I....O
-000010f0: d008 b2b8 8b28 39e0 c4db 25d3 0812 6f86  .....(9...%...o.
-00001100: 1226 60b8 5429 0d4a 55f8 af3e 81fe a623  .&`.T).JU..>...#
-00001110: 8ab6 3032 a495 5d60 8958 1b52 f678 62c4  ..02..]`.X.R.xb.
-00001120: c94c b6fc 2ba0 d537 202f 9e3d 7bfe f0e9  .L..+..7 /.={...
-00001130: f387 bf3d 7ff4 e8f9 c35f b2b9 b52a 4b6e  ...=....._...*Kn
-00001140: 0725 5353 eed5 8f5f fffd fd17 de5f bffe  .%SS..._....._..
-00001150: f0ea f137 e9d4 27f1 c2c4 bffc f9cb 97bf  ...7..'.........
-00001160: fff1 3af5 b0e2 dc15 2fbe 7df2 f2e9 9317  ..:...../.}.....
-00001170: df7d f5e7 4f8f 1dda db1c 1d98 f021 89b1  .}..O........!..
-00001180: f0ae e163 ef26 8b61 810e fbf1 013f 9dc4  ...c.&.a.....?..
-00001190: 3042 c492 4011 e876 a8ee cbc8 025e 5b20  0B..@..v.....^[ 
-000011a0: eac2 75b0 edc2 db1c 58c6 05bc 3cbf 6bd9  ..u.....X...<.k.
-000011b0: ba1f f1b9 248e 99af 46b1 05dc 638c 7618  ....$...F...c.v.
-000011c0: 773a e0aa 9acb f0f0 709e 4cdd 93f3 b989  w:......p.L.....
-000011d0: bb89 d091 6bee 2e4a ac00 f7e7 33a0 57e2  ....k..J....3.W.
-000011e0: 52d9 8db0 65e6 0d8a 1289 a638 c1d2 53bf  R...e......8..S.
-000011f0: b143 8c1d abbb 4388 e5d7 3d32 e24c b089  .C....C...=2.L..
-00001200: f4ee 10af 8388 d325 4372 6025 522e b443  .......%Cr`%R..C
-00001210: 6288 cbc2 6520 84da f2cd de6d afc3 a86b  b...e .....m...k
-00001220: d53d 7c64 2361 5b20 ea30 7e88 a9e5 c6cb  .=|d#a[ .0~.....
-00001230: 682e 51ec 5239 4431 351d be8b 64e4 3272  h.Q.R9D15...d.2r
-00001240: 7fc1 4726 ae2f 2444 7a8a 29f3 fa63 2c84  ..G&./$Dz.)..c,.
-00001250: 4be6 3a87 f51a 41bf 0a0c e30e fb1e 5dc4  K.:...A.......].
-00001260: 3692 4b72 e8d2 b98b 1833 913d 76d8 8d50  6.Kr.....3.=v..P
-00001270: 3c73 da4c 92c8 c47e 260e 2145 9177 8349  <s.L...~&.!E.w.I
-00001280: 177c 8fd9 3b44 3d43 1c50 b231 dcb7 09b6  .|..;D=C.P.1....
-00001290: c2fd 6622 b805 e46a 9a94 2788 fa65 ce1d  ..f"...j..'..e..
-000012a0: b1bc 8c99 bd1f 1774 82b0 8b65 da3c b6d8  .......t...e.<..
-000012b0: b5cd 8933 3b3a f3a9 95da bb18 5374 8cc6  ...3;:......St..
-000012c0: 187b b73e 7358 d061 33cb e7b9 d157 2260  .{.>sX.a3....W"`
-000012d0: 951d ec4a ac2b c8ce 55f5 9c60 0165 92aa  ...J.+..U..`.e..
-000012e0: 6bd6 2972 9708 2b65 f7f1 946d b067 6f71  k.)r..+e...m.goq
-000012f0: 8278 1628 8911 dfa4 f91a 44dd 4a5d 38e5  .x.(......D.J]8.
-00001300: 9c54 7a9d 8e0e 4de0 3502 e51f e48b d329  .Tz...M.5......)
-00001310: d705 e830 92bb bf49 eb8d 0859 6797 7a16  ...0...I...Yg.z.
-00001320: ee7c 5d70 2b7e 6fb3 c760 5fde 3ded be04  .|]p+~o..`_.=...
-00001330: 197c 6a19 20f6 b7f6 cd10 516b 823c 6186  .|j. .....Qk.<a.
-00001340: 080a 0c17 dd82 8815 fe5c 449d ab5a 6cee  .........\D..Zl.
-00001350: 949b d89b 360f 0314 4656 bd13 93e4 8dc5  ....6...FV......
-00001360: cf89 b227 fc77 ca1e 7701 7306 058f 5bf1  ...'.w..w.s...[.
-00001370: fb94 3a9b 2865 e744 81b3 09f7 1f2c 6b7a  ..:.(e.D.....,kz
-00001380: 689e dcc0 7092 ac73 d679 5573 5ed5 f8ff  h...p..s.yUs^...
-00001390: fbaa 66d3 5e3e af65 ce6b 99f3 5ac6 f5f6  ..f.^>.e.k..Z...
-000013a0: f541 6a99 bc7c 81ca 26ef f2e8 9e4f bcb1  .Aj..|..&....O..
-000013b0: e533 2194 eecb 05c5 bb42 777d 04bc d18c  .3!......Bw}....
-000013c0: 0730 a8db 51ba 27b9 6a01 ce22 f89a 3598  .0..Q.'.j.."..5.
-000013d0: 2cdc 9423 2de3 7126 3f27 32da 8fd0 0c5a  ,..#-.q&?'2....Z
-000013e0: 4365 ddc0 9c8a 4cf5 5478 3326 a063 a487  Ce....L.Tx3&.c..
-000013f0: 752b 159f d0ad fb4e f378 8f8d d34e 67b9  u+.....N.x...Ng.
-00001400: acba 9aa9 0b05 92f9 7829 5c8d 4397 4aa6  ........x)\.C.J.
-00001410: e85a 3def dead d4eb 7ee8 5477 5997 0628  .Z=.....~.TwY..(
-00001420: d9d3 1861 4c66 1b51 7518 515f 0e42 145e  ...aLf.Qu.Q_.B.^
-00001430: 6784 5ed9 9958 d174 58d1 50ea 97a1 5a46  g.^..X.tX.P...ZF
-00001440: 71e5 0a30 6d15 1578 e5f6 e045 bde5 8741  q..0m..x...E...A
-00001450: da41 8666 1c94 e763 15a7 b499 bc8c ae0a  .A.f...c........
-00001460: ce99 467a 9333 a999 0150 622f 3320 8f74  ..Fz.3...Pb/3 .t
-00001470: 53d9 ba71 796a 7569 aabd 45a4 2d23 8c74  S..qyjui..E.-#.t
-00001480: b38d 30d2 3082 17e1 2c3b cd96 fb59 c6ba  ..0.0...,;...Y..
-00001490: 9987 d432 4fb9 62b9 1b72 33ea 8d0f 116b  ...2O.b..r3....k
-000014a0: 4522 27b8 8126 2653 d0c4 3b6e f9b5 6a08  E"'..&&S..;n..j.
-000014b0: b72a 2334 6bf9 13e8 18c3 d778 06b9 23d4  .*#4k......x..#.
-000014c0: 5b17 a253 b876 1949 9e6e f877 6196 1917  [..S.v.I.n.wa...
-000014d0: b287 4494 3a5c 934e ca06 3191 987b 94c4  ..D.:\.N..1..{..
-000014e0: 2d5f 2d7f 950d 34d1 1ca2 6d2b 5780 103e  -_-...4...m+W..>
-000014f0: 5ae3 9a40 2b1f 9b71 1074 3bc8 7832 c123  Z..@+..q.t;.x2.#
-00001500: 6986 dd18 519e 4e1f 81e1 53ae 70fe aac5  i...Q.N...S.p...
-00001510: df1d ac24 d91c c2bd 1f8d 8fbd 033a e737  ...$.........:.7
-00001520: 11a4 5858 2f2b 078e 8980 8b83 72ea cd31  ..XX/+......r..1
-00001530: 819b b015 91e5 f977 e260 ca68 d7bc 8ad2  .......w.`.h....
-00001540: 3994 8e23 3a8b 5076 a298 649e c235 89ae  9..#:.Pv..d..5..
-00001550: ccd1 4f2b 1f18 4fd9 9ac1 a1eb 2e3c 98aa  ..O+..O......<..
-00001560: 03f6 bd4f dd37 1fd5 ca73 0669 e667 a6c5  ...O.7...s.i.g..
-00001570: 2aea d474 93e9 873b e40d abf2 43d4 b22a  *..t...;....C..*
-00001580: a56e fd4e 2d72 ae6b 2eb9 0e12 d579 4abc  .n.N-r.k.....yJ.
-00001590: e1d4 7d8b 03c1 302d 9fcc 324d 59bc 4ec3  ..}...0-..2MY.N.
-000015a0: 8ab3 b351 dbb4 332c 080c 4fd4 36f8 6d75  ...Q..3,..O.6.mu
-000015b0: 4638 3df1 ae27 3fc8 9dcc 5a75 402c eb4a  F8=..'?...Zu@,.J
-000015c0: 9df8 faca dcbc d566 0777 813c 7a70 7f38  .......f.w.<zp.8
-000015d0: a752 e850 426f 9723 28fa d21b c894 3660  .R.PBo.#(.....6`
-000015e0: 8bdc 9359 8d08 dfbc 3927 2dff 7e29 6c07  ...Y....9'-.~)l.
-000015f0: dd4a d82d 941a 61bf 1054 8352 a111 b6ab  .J.-..a..T.R....
-00001600: 8576 1856 cbfd b05c ea75 2a0f e060 9151  .v.V...\.u*..`.Q
-00001610: 5c0e d3eb fa01 5c61 d045 7669 afc7 d72e  \.....\a.Evi....
-00001620: eee3 e52d cd85 118b 8b4c 5fcc 17b5 e1fa  ...-.....L_.....
-00001630: e2be 5cd9 7c71 ef11 209d fbb5 caa0 596d  ..\.|q.. .....Ym
-00001640: 766a 8566 b53d 2804 bd4e a3d0 ecd6 3a85  vj.f.=(..N....:.
-00001650: 5ead 5bef 0d7a ddb0 d11c 3cf0 bd23 0d0e  ^.[..z....<..#..
-00001660: dad5 6e50 eb37 0ab5 72b7 5b08 6a25 657e  ..nP.7..r.[.j%e~
-00001670: a359 a807 954a 3ba8 b71b fda0 fd20 2b63  .Y...J;...... +c
-00001680: 60e5 297d 64be 00f7 6abb b6ff 0100 00ff  `.)}d...j.......
-00001690: ff03 0050 4b03 0414 0006 0008 0000 0021  ...PK..........!
-000016a0: 004f 821b e147 1100 0074 8400 0018 0000  .O...G...t......
-000016b0: 0078 6c2f 776f 726b 7368 6565 7473 2f73  .xl/worksheets/s
-000016c0: 6865 6574 312e 786d 6c9c 93db 8e9b 3010  heet1.xml.....0.
-000016d0: 86ef 2bf5 1d2c df07 0361 d95d 14b2 6ab3  ..+..,...a.]..j.
-000016e0: 8aba 522f aa1e af8d 1982 151b 53db 39ac  ..R/........S.9.
-000016f0: aabe 7bc7 9093 948b 468b c036 b6e7 fbff  ..{.....F..6....
-00001700: c1c3 ec69 af15 d982 75d2 7425 4da2 9812  ...i....u.t%M...
-00001710: e884 a965 b72a e98f efcb c903 25ce f3ae  ...e.*......%...
-00001720: e6ca 7450 d257 70f4 69fe fedd 6c67 ecda  ..tP.Wp.i...lg..
-00001730: b500 9e20 a173 256d bdef 0bc6 9c68 4173  ... .s%m.....hAs
-00001740: 1799 1e3a 5c69 8cd5 dce3 ab5d 31d7 5be0  ...:\i.....]1.[.
-00001750: f510 a415 4be3 3867 9acb 8e8e 84c2 dec2  ....K.8g........
-00001760: 304d 2305 3c1b b1d1 d0f9 1162 4171 8ffe  0M#.<......bAq..
-00001770: 5d2b 7b77 a469 710b 4e73 bbde f413 6174  ]+{w.iq.Ns....at
-00001780: 8f88 4a2a e95f 0728 255a 142f abce 585e  ..J*._.(%Z./..X^
-00001790: 29cc 7b9f 645c 90bd c53b c567 7a94 19e6  ).{.d\...;.gz...
-000017a0: af94 b414 d638 d3f8 08c9 6cf4 7c9d fe23  .....8....l.|..#
-000017b0: 7b64 5c9c 48d7 f9df 8449 3266 612b c301  {d\.H....I2fa+..
-000017c0: 9e51 e9db 2c25 7727 567a 864d df08 cb4f  .Q..,%w'Vz.M...O
-000017d0: b0f0 b96c b191 7549 ffc4 876b 827d 129a  ...l..uI...k.}..
-000017e0: f8dc 1cd7 fed2 f9ac 9678 c221 2b62 a129  .........x.!+b.)
-000017f0: e987 a458 a4c9 0365 f3d9 5041 3f25 ecdc  ...X...e..PA?%..
-00001800: c598 785e 7d03 05c2 03aa 2494 78d3 7f86  ..x^}.....$.x...
-00001810: c62f 40a9 109d 6794 849a ad8c 5987 d817  ./@...g.....Y...
-00001820: dc15 a38c 1b62 820c 175e 6e61 dcff 31b9  .....b...^na..1.
-00001830: 0f85 ff7b 901e 5e50 979d 842f c747 13cb  ...{..^P.../.G..
-00001840: a1d2 bf58 5271 070b a37e c9da b7e8 04ff  ...XRq...~......
-00001850: a81a 1abe 51fe 6212 fd1d 26bf 9add 2790  ....Q.b...&...'.
-00001860: abd6 e3d6 1c3f 53a8 b3a2 7e7d 0627 b0c0  .....?S...~}.'..
-00001870: d163 9486 9c85 5128 842d d132 fca8 589f  .c....Q(.-.2..X.
-00001880: 7c3f f4bb 5127 cba2 3b4a 2a70 7e29 038b  |?..Q'..;J*p~)..
-00001890: 12b1 71de e8a3 8d03 640c c7c3 1dc2 b13f  ..q.....d......?
-000018a0: 844f efa3 3ccf e23c fd2f 840d 56fe 0100  .O..<..<./..V...
-000018b0: 00ff ff00 0000 ffff 949d eb8e dd36 1284  .............6..
-000018c0: 5fc5 f0ff c8e2 45b7 c019 6067 fc22 03ef  _.....E...`g."..
-000018d0: 00f9 955d 6406 dedd b7df a686 e748 c5a6  ...]d........H..
-000018e0: fa74 3940 10b8 d9f6 171d b28a 1255 67be  .t9@.........Ug.
-000018f0: bfff f9f6 f6f1 e3f5 e3f5 e9fb dfff facf  ................
-00001900: 97bf fff8 1abe 7e79 fff7 eb5f eff2 5fbf  ......~y..._.._.
-00001910: a7af 5ffe 1bf2 ebcf dfff f9bf 1f6f ef3f  .._..........o.?
-00001920: dffe faf8 e3eb 38c4 af4f df7f 96a1 ff28  ......8..O.....(
-00001930: 63f7 0ef9 fd77 f9dd 5f4f e3f7 6fbf 9ebe  c....w.._O..o...
-00001940: 7ffb 5947 3ceb 1101 47bc e811 f13e e29b  ..YG<...G....>..
-00001950: 30dd c122 0126 63ef 48a9 413a d7a6 86f7  0..".&c.H.A:....
-00001960: a5fc bffd 7afa ed80 0404 b91e ee6b 2363  ....z........k#c
-00001970: ef08 73f3 3ffd 7c2e 2a86 6432 6482 41c6  ..s.?.|.*.d2d.A.
-00001980: de19 7273 19ce b5a9 fd50 f28e 7071 1526  ..rs.....P..pq.&
-00001990: 8240 c65e 129c 6bd3 f1a1 ef53 eb65 b208  .@.^..k....S.e..
-000019a0: 6682 40c6 5e12 9c6b 5333 4f5e 668b 6021  f.@.^..kS3O^f.`!
-000019b0: 0864 ec25 c1b9 3635 1fd1 cb62 11ac 0481  .d.%..65...b....
-000019c0: 8cbd 134c cd3c 805a 537c 592d 828d 2090  ...L.<.ZS|Y-.. .
-000019d0: b197 0450 6b67 e266 1184 9111 2b19 7cc9  ...Pkg.f....+.|.
-000019e0: 50fe a4a3 d84e 46a9 1659 b858 0f81 924c  P....NF..Y.X...L
-000019f0: 197c 4d01 c576 42ca df63 5130 fa18 4004  .|M..vB..cQ0..@.
-00001a00: 5bcd 8662 3b29 a5d5 a260 2432 8046 b614  [..b;)...`$2.F..
-00001a10: a091 73eb 1a9f 2279 f589 3022 19ce 4ad8  ..s..."y..0"..J.
-00001a20: fc3d cf50 9cda e521 55eb 5a30 4219 ce6a  .=.P...!U.Z0B..j
-00001a30: a828 402a 9583 9a5a 1918 b12c 830f d76a  .(@*...Z...,...j
-00001a40: 3f11 904b b546 4cbd 0c8c 6096 c1d7 1420  ?..K.FL...`.... 
-00001a50: 996a 8d98 9a19 18d1 2c83 af29 4036 d51a  .j......,..)@6..
-00001a60: 3175 3330 c259 06df 2996 f613 01e9 6caa  1u30.Y..).....l.
-00001a70: 2fd2 6a6d 6622 239e 65f0 2506 14a7 b559  /.jmf"#.e.%....Y
-00001a80: aa52 3531 18f5 8c67 816c af06 14a7 adc5  .R51...g.l......
-00001a90: f854 cfab ad5d a4b6 9767 8554 18e7 e2ac  .T...]...g.T....
-00001aa0: 3698 f60e 3332 fa59 06df 3f94 e6b2 3f43  6...32.Y..?...?C
-00001ab0: 5129 9754 77e5 1ab6 6939 3a71 bfcd 8868  Q).Tw...i9:q...h
-00001ac0: 3c8b a842 31f7 9ad2 fa10 8551 d278 164b  <..B1......Q.x.K
-00001ad0: 8562 6e3a a5f5 210a 23a7 f1ac 980a c5dc  .bn:..!.#.......
-00001ae0: 7d4a eb43 1446 53e3 5936 158a b90d 95d6  }J.C.FS.Y6......
-00001af0: 8728 8cb0 c6b3 7636 cbf4 198a 536b fb52  .(....v6....Sk.R
-00001b00: 7d88 c2a8 6b3c 0ba8 4201 756d bd5f 5a1f  }...k<..B.um._Z.
-00001b10: a124 4661 cbe0 fb62 6e51 a0a8 eed6 a4fa  .$Fa...bnQ......
-00001b20: 1085 51d9 7456 5985 027b d476 1720 ad0f  ..Q.tVY..{.v. ..
-00001b30: 5118 a54d 6731 5528 b051 6db7 02d2 fa10  Q..Mg1U(.Qm.....
-00001b40: 85ba a13f abad 4281 dd6a bb1f 488f d536  ...?..B..j..H..6
-00001b50: 316a 5b06 dfe7 4a68 9fb9 4055 29bf 54cb  1j[...Jh..@U).T.
-00001b60: 6519 87b4 ce79 3cfd ba78 ec92 18ed 2d83  e....y<..x....-.
-00001b70: 0d30 731b 2bbd 1c18 a3c4 e92c b6fa 8a99  .0s.+......,....
-00001b80: 3b5b e9e5 c018 5d4e 67e9 d560 e666 577a  ;[....]Ng..`.fWz
-00001b90: 3930 46a5 d359 a535 98b9 ff95 5e0e 8cd1  90F..Y.5....^...
-00001ba0: ec74 96e5 a09e ac99 a22d bd05 2c0e 711e  .t.......-..,.q.
-00001bb0: b72d 8c87 66c0 d627 33c2 5d06 1f73 bee5  .-..f..'3.]..s..
-00001bc0: 81aa 7ece f6a9 dc0f 7918 f5ce 6781 56d7  ..~.....y...g.V.
-00001bd0: 07aa eaa9 9b54 5dd7 8791 f07c 5669 cd63  .....T]....|Vi.c
-00001be0: 6ab8 f4ba 7818 1dcf 67a9 d63c a690 4baf  j...x...g..<..K.
-00001bf0: 8b87 7a48 0b62 de18 ea73 86bd 73bb 0991  ..zH.b...s..s...
-00001c00: eace 93f2 7021 df99 91ef 32f8 98ca 0ac5  ....p!....2.....
-00001c10: 946f e97d 84c2 0876 06c1 5628 a660 4bef  .o.}...v..V(.`K.
-00001c20: 2314 46a2 3348 b442 3125 5a7a 1fa1 30a2  #.F.3H.B1%Zz..0.
-00001c30: 9c41 9415 8a29 cad2 fb08 8591 e10c 32dc  .A...)........2.
-00001c40: 1eb2 4055 ed41 a4ba a38c e3b0 e435 8e63  ..@U.A.......5.c
-00001c50: 1435 2ebf fa27 3f13 23c7 65f0 3187 5b2e  .5...'?.#.e.1.[.
-00001c60: a82a 3996 2ac5 c5c8 f204 b2ac b8cc 5db5  .*9.*.........].
-00001c70: f452 5c8c 3c4f 20cf 8acb 9467 e9a5 b818  .R\.<O ....g....
-00001c80: 999e 40a6 1597 29d3 d24b 7131 723d 815c  ..@...)..Kq1r=.\
-00001c90: b7a7 6a50 55f3 5eaa 3b57 1c52 da52 98e7  ..jPU.^.;W.R.R..
-00001ca0: ab09 4f1d b181 682b 2053 b4a7 2ada 0f81  ..O...h+ S..*...
-00001cb0: 18e9 9e40 ba15 9029 ddd2 ebbb 428c 804f  ...@...)....B..O
-00001cc0: 20e0 0ac8 1470 e9f5 0131 323e 818c 2b20   ....p...12>..+ 
-00001cd0: 53c6 a5d7 07c4 88f9 0462 de1e 1142 554f  S........b...BUO
-00001ce0: ea2a e6d3 9887 2987 b084 3994 dbca 8b0d  .*....)...9.....
-00001cf0: c9cc 8879 197c 8879 cb05 5525 e652 dd2f  ...y.|.y..U%.R./
-00001d00: 9497 8b11 f319 c45c 7199 622e bd14 1723  .......\q.b....#
-00001d10: e633 88b9 e232 c55c 7a29 2e46 cc67 1073  .3...2.\z).F.g.s
-00001d20: c565 8ab9 f452 5c8c 98cf 20e6 edb1 1b54  .e...R\... ....T
-00001d30: d5bc 976a e1ca 7949 c31c d79c d3b2 cffb  ...j..yI........
-00001d40: 8b7b ca99 d1f4 32f8 98f7 8acb d474 e9a5  .{....2......t..
-00001d50: b818 699f 41da 1597 29ed d24b 7131 0a3f  ..i.A...)..Kq1.?
-00001d60: 83c2 2b2e 53e1 a597 e262 847e 06a1 575c  ..+.S....b.~..W\
-00001d70: a6d0 4b2f c5c5 e8fd 0c7a df9e 6041 55cf  ..K/.....z..`AU.
-00001d80: fbfa e03b 8421 cdeb 3a8f f142 e917 46e9  ...;.!..:..B..F.
-00001d90: cbe0 63c6 b744 5055 4a2f d572 a5c2 6322  ..c..DPUJ/.r..c"
-00001da0: 46e3 17d0 7845 646a bcf4 3a89 1875 5f40  F...xEdj..:..u_@
-00001db0: dd15 91a9 eed2 eb24 6274 7d01 5d57 44a6  .......$bt}.]WD.
-00001dc0: ae4b af93 8851 f405 14bd 3de8 82aa 9ad9  .K...Q....=.....
-00001dd0: 52dd 89b6 610c 53ca 7232 faf9 78fc e22d  R...a.S.r2..x..-
-00001de0: 9385 51f4 32f8 98df 8acb 5474 e9a5 b818  ..Q.2.....Tt....
-00001df0: 455f 40d1 1597 a9e8 d24b 7131 8abe 80a2  E_@......Kq1....
-00001e00: 2b2e 53d1 a597 e262 147d 0145 575c a6a2  +.S....b.}.EW\..
-00001e10: 4b2f c5c5 28fa 028a de1e 4f41 55cf fb4f  K/..(.....OAU..O
-00001e20: 451f 8710 d332 c936 a6ff 1866 65f4 bc0c  E....2.6...fe...
-00001e30: 3ee6 7bcb 0355 a5e7 522d d7e9 210f a3e6  >.{..U..R-..!...
-00001e40: 2ba8 b9e2 31d5 5c7a 5d3c 8c96 afa0 e58a  +...1.\z]<......
-00001e50: c7d4 72e9 75f1 304a be82 922b 1e53 c9a5  ..r.u.0J...+.S..
-00001e60: d7c5 c3e8 f87a d6f1 d81e 7142 55cd 67a9  .....z....qBU.g.
-00001e70: 169e 759a d210 d669 967f 26e3 8e74 6574  ..u....i..&..tet
-00001e80: bc0c becf 6bcd 65ea b8f4 525c 8c8e af67  ....k.e...R\...g
-00001e90: a5d6 5ca6 8e4b 2fc5 c5e8 f87a 566a cd65  ..\..K/....zVj.e
-00001ea0: eab8 f452 5c8c 8eaf 67a5 d65c a68e 4b2f  ...R\...g..\..K/
-00001eb0: c5c5 e8f8 7ad6 f1d8 9e26 4255 cffb 4f1d  ....z....&BU..O.
-00001ec0: 4fd3 342c e336 e638 07eb b1fa c6e8 7919  O.4,.6.8......y.
-00001ed0: 7ccc fb96 0baa 4acf a55a ae97 9b8b d1f5  |.....J..Z......
-00001ee0: edac dcea 7a41 559d 764a 95e2 62f4 7d3b  ....zAU.vJ..b.};
-00001ef0: 2bb8 e632 f55d 7a29 2e46 e7b7 b392 6b2e  +..2.]z).F....k.
-00001f00: 53e7 a597 e262 f47e 03bd 6f4f b6a0 aae6  S....b.~..oO....
-00001f10: bd54 f77d d538 6ca2 f453 588f 1b6d 38d6  .T.}.8l..SX..m8.
-00001f20: df18 a12f 838f 09af 804c a197 5e1f 10a3  .../.....L..^...
-00001f30: f01b 28bc 0232 155e 7a7d 408c b46f 20ed  ..(..2.^z}@..o .
-00001f40: 0ac8 9476 e9f5 0131 9abe 81a6 2b20 53d3  ...v...1....+ S.
-00001f50: a5d7 07c4 88f9 0662 de9e 6141 554f ea4f  .......b..aAUO.O
-00001f60: 312f 0f17 971c c3bc e64f 2dbf 78bc 288f  1/.......O-.x.(.
-00001f70: 1ea9 2c0c c879 4bb6 ff61 f7c9 aff4 bc94  ..,..yK..a......
-00001f80: cbc5 f2b3 318a 1e46 9074 cd66 eed5 4b37  ....1..F.t.f..K7
-00001f90: c7c6 a87a 1841 d635 9ba9 eba5 9b63 6394  ...z.A.5.....cc.
-00001fa0: 5dde 663a 2b96 6633 b5bd 7473 6c8c ba87  ].f:+.f3..tsl...
-00001fb0: 11e4 bd3d f1c2 b28e d948 f7be e1da 9645  ...=.....H.....E
-00001fc0: 1ecd e479 5e97 5436 f497 6b81 11fa 3082  ...y^.T6..k...0.
-00001fd0: d26b 3653 ea4b 37c7 c668 7e18 41f4 359b  .k6S.K7..h~.A.5.
-00001fe0: a9fa a59b 6363 e43f 8ca0 ff9a cd34 80d2  ....cc.?.....4..
-00001ff0: cdb1 314e 1046 b002 cd66 7a41 e9e6 d818  ..1N.F...fzA....
-00002000: 5308 23b8 427b 1886 e5ce 5aa8 8fdf e5f9  S.#.B{....Z.....
-00002010: e434 cc29 aef2 c0e6 6a1d 70f9 48c8 4046  .4.)....j.p.H.@F
-00002020: c585 1149 1542 bb65 245d 5c94 1f94 7ce5  ...I.B.e$]\...|.
-00002030: b113 d35c b61f dc52 932e 2eca 0b20 44d9  ...\...R..... D.
-00002040: b95e b617 dc72 942e 2eca 0720 56d9 e1b2  .^...r..... V...
-00002050: 7d40 baf7 8d90 8b8b f200 c852 4695 717c  }@.........RF.q|
-00002060: 10b5 ac59 cb6d 5e86 3cca 2b06 cbbc 3fd3  ...Y.m^.<.+...?.
-00002070: 198f f900 7bfd 5002 95fe 2f32 80f8 6587  ....{.P.../2..e.
-00002080: cdf6 00e9 2ed7 cccf 4679 0084 323b 6cb6  ........Fy..2;l.
-00002090: 0748 37c7 4679 0044 353b 6cb6 0748 37c7  .H7.Fy.D5;l..H7.
-000020a0: 4679 0004 383b 6cb6 0748 37c7 4679 00c4  Fy..8;l..H7.Fy..
-000020b0: 3aa3 ca75 4259 7d2f 40a8 c94e d1ff cf7b  :..uBY}/@..N...{
-000020c0: 82db bfaf 7c80 8a7a 0688 73c6 f688 03cb  ....|..z..s.....
-000020d0: da9f 6adc 53f2 2531 afdb 1c0f c4fe a942  ..j.S.%1.......B
-000020e0: 28b1 4dff 4285 9067 070e cc40 9994 7497  (.M.B..g...@..t.
-000020f0: 0f95 80a3 1ca1 8448 0fa7 d257 0e1c 4105  .......H...W..A.
-00002100: a8a5 9b84 a36c 0102 a19d 2b07 b6d0 dc3d  .....l....+....=
-00002110: bcc8 c910 0b47 7903 e447 3b70 f016 bcfe  .....Gy..G;p....
-00002120: 4a82 7ba6 c93b e728 7380 4469 6ccf 4602  J.{..;.(s.Dil.F.
-00002130: 943b 0ba2 be63 b9cd c33a cb7a 5897 d57a  .;...c...:.zX..z
-00002140: 2a1b 4a68 9458 0f70 83a0 d9c0 1cf4 7aa8  *.Jh.X.p......z.
-00002150: af5b bad9 2873 80cc 69e7 ba81 39e8 e550  .[..(s..i...9..P
-00002160: dfbc 74b3 51e6 0039 d30e 1b98 835e 0df5  ..t.Q..9.....^..
-00002170: 254c 371b 650e 904a edb0 9def 1fb4 39d4  %L7.e..J......9.
-00002180: 606a f4b2 5129 d500 49d4 a4be ee09 83aa  `j..Q)..I.......
-00002190: eafb 326a 5235 07d9 c54d 611b c7bc ecfe  ..2jR5...Ma.....
-000021a0: 7011 410f 2589 ea5f 0b90 5bed b0d9 de50  p.A.%.._..[....P
-000021b0: a3ab 7e36 ca1a 20c8 da61 b3ad a166 59fd  ..~6.. ..a...fY.
-000021c0: 6c94 3348 3cf5 b0ad 0e9b ed0c 35dc ea67  l.3H<.......5..g
-000021d0: a38c 01c2 ac1d 36db 186a d8d5 cf46 f902  ......6..j...F..
-000021e0: a45d 537b 2616 a0ac 7da1 e65d e590 4e4e  .]S{&...}..]..NN
-000021f0: ebe6 18f3 b2ec af1b 5d7d a74d 89b0 126b  ........]}.M...k
-00002200: e12c fc1d 36db 176a e4d5 cf46 f902 645e  .,..6..j...F..d^
-00002210: 3b6c b62f d4d4 ab9f 8df2 0588 bd76 d86c  ;l./.........v.l
-00002220: 5fa8 c157 3f1b e50b 907c edb0 d9be 70cb  _..W?....|....p.
-00002230: be7a e71b 1582 0d90 734d edd9 0b96 f55a  .z......sM.....Z
-00002240: 90ee fda1 c3b4 c538 ac61 9ad7 edf2 a156  .......8.a.....V
-00002250: 49b0 fad7 01e4 5d3b 5cb6 27d4 3c6c 7071  I.....];\.'.<lpq
-00002260: 517e 00a9 d80e 97ed 0735 17eb e3a2 bc00  Q~.......5......
-00002270: d2b1 1d2e db0b 6a3e d6c7 45f9 00e4 603b  ......j>..E...`;
-00002280: 5cb6 0fd4 9cac 8f8b f200 88cc 2675 e802  \...........&u..
-00002290: e5ce bcbf 7de1 4c8c eb16 96ab 00a4 1c79  ....}.L........y
-000022a0: 5073 1eb4 5f33 d9da 5fd3 b361 78c4 4469  Ps.._3.._..ax.Di
-000022b0: 3e84 683b d7c9 d6fc 1aa3 7dcc 4469 3da4  >.h;......}.Di=.
-000022c0: 693b 4cb6 d6d7 3ced 6326 4ae3 2138 db61  i;L...<.c&J.!8.a
-000022d0: b235 be06 6b1f 3251 89da 00a1 d9a4 0e53  .5..k.2Q.......S
-000022e0: 3053 abf6 fc35 542b 0199 7548 5348 7207  0S...5T+..uHSHr.
-000022f0: bca7 7d2f 5ed2 0825 28eb d777 88d5 76d8  ..}/^..%(..w..v.
-00002300: 6c7d afc1 5a3f 1ba5 f110 aded b0d9 1a5f  l}..Z?........._
-00002310: c3b5 7e36 4ae7 215e db61 b375 be06 6cfd  ..~6J.!^.a.u..l.
-00002320: 6c94 d643 88b6 c366 6b7d 0dd9 fad9 28bd  l..C...fk}....(.
-00002330: 97c4 ece9 5e49 1d46 4159 ebfd 2d6f 3b0e  ....^I.FAY..-o;.
-00002340: 39ca 8e7f 8c9f 6718 5759 49d9 0851 6b01  9.....g.WYI..Qk.
-00002350: 745f b3d9 ba7f 8bde bad9 28fd 870c 6ed2  t_........(...n.
-00002360: 6cb6 fedf 52b8 6e36 ca07 208e db61 b37d  l...R.n6.. ..a.}
-00002370: e016 c875 b351 7e00 d9db 0e9b ed07 d25d  ...u.Q~........]
-00002380: f6d5 d1cb 4685 7303 e46f 933a d0c3 78ae  ....F.s..o.:..x.
-00002390: f285 9acf ddf2 90b7 24af 74e4 fa1d 1057  ........$.t....W
-000023a0: cf82 4ae6 d6ef 0b90 d0ed b0d9 be50 33ba  ..J..........P3.
-000023b0: 7e36 ca17 20a5 db61 b37d a1e6 74fd 6c94  ~6.. ..a.}..t.l.
-000023c0: 2f40 52b7 c366 fb42 cdea fad9 285f 803c  /@R..f.B....(_.<
-000023d0: 6e87 cdf6 859a d7f5 b351 be00 89dd a40e  n........Q......
-000023e0: f4a0 ac7d a166 76dd 077a 2587 4bac 05f0  ...}.fv..z%.K...
-000023f0: 05cd 66fb 42cd edfa d928 5f80 e46e e7ba  ..f.B....(_..n..
-00002400: d9be 50b3 bb7e 36ca 1720 bddb 61b3 7da1  ..P..~6.. ..a.}.
-00002410: e677 fd6c 942f 4046 b7c3 66fb 8274 175f  .w.l./@F..f..t._
-00002420: 70b3 5151 de00 69dd a48e 4131 ccab bed9  p.QQ..i...A1....
-00002430: bba6 79fd 6c94 2f40 aab7 c306 bea0 3cab  ..y.l./@......<.
-00002440: e67a fd6c 942f 40be b7c3 06be a0ce f26a  .z.l./@........j
-00002450: c2d7 cf46 f902 247d 3b6c e00b ea2c af66  ...F..$};l...,.f
-00002460: 7dfd 6c94 2f40 aab7 c306 bea0 cef2 6aea  }.l./@........j.
-00002470: d7cf 46f9 02e4 7e3b 6cf0 6291 3ad8 aec9  ..F...~;l.b.:...
-00002480: 5f3f 1be5 0b90 fd4d eaec 18ca dab3 6ee9  _?.....M......n.
-00002490: df61 5e83 bc98 bbd4 f7d3 2f9f 6195 44af  .a^......./.a.D.
-000024a0: dfb3 20ff db61 035f d06b e1f6 95c5 5e36  .. ..a._.k....^6
-000024b0: ca17 2003 dc61 035f d06b e1f6 1dc6 5e36  .. ..a._.k....^6
-000024c0: ca17 20e9 db61 035f d06b e1f6 a5c6 4e36  .. ..a._.k....N6
-000024d0: 2a12 1c20 f5ab d930 14ac bf53 fff6 2dc7  *.. ...0...S..-.
-000024e0: 5e36 ca17 201f 9cd5 b936 94f5 5aa8 0961  ^6.. ....6..Z..a
-000024f0: f73a 2de9 5fff 5a80 ac70 87cd f685 9a16  .:-._.Z..p......
-00002500: f6b3 51be 00b9 e10e 9bed 0b35 39ec 67a3  ..Q........59.g.
-00002510: 7c01 52c2 1d36 db17 6a8a d8cf 46f9 02e4  |.R..6..j...F...
-00002520: 883b 6cb6 2fd4 24b1 9f8d f205 c812 6775  .;l./.$.......gu
-00002530: ae0d e5ce 5aa8 dff3 b36c 83bc 8d35 c92b  ....Z....l...5.+
-00002540: ea72 ae21 bfae eeeb 4b42 9858 0b67 e1ef  .r.!....KB.X.g..
-00002550: b0d9 be50 13c5 d9cd 46f9 0264 8a3b 6cb6  ...P....F..d.;l.
-00002560: 2fd4 54b1 9f8d f205 480e 77d8 6c5f 90ee  /.T.....H.w.l_..
-00002570: 72bf e066 a3a2 c5f2 1ed0 e999 aa66 c370  r..f.........f.p
-00002580: b1f2 859a 2ef6 b351 be00 09e2 acce b531  .......Q.......1
-00002590: 60ac ee17 6ac2 781d d32a 6fad a725 861c  `...j.x..*o..%..
-000025a0: cb5a 38ee c1f1 a5f5 921a f6af 05c8 1877  .Z8............w
-000025b0: d86c 5fa8 2963 3f1b e50b 9033 eeb0 d9be  .l_.)c?....3....
-000025c0: 5093 c67e 36ca 1720 4ddc 61b3 7da1 a68d  P..~6.. M.a.}...
-000025d0: fd6c 942f 40ec b8c3 66fb 420d 1efb d928  .l./@...f.B....(
-000025e0: 5f80 0472 56e7 ca50 d6be 5033 c831 a569  _..rV..P..P3.1.i
-000025f0: 089b 84b4 e54b 7fcb 0b4f 57ef 3b95 7831  .....K...OW.;.x1
-00002600: b116 c017 349b ed0b 358e ec67 a37c 0172  ....4...5..g.|.r
-00002610: c99d eb66 fb42 4d26 fbd9 285f 8010 7287  ...f.BM&..(_..r.
-00002620: cdf6 05e9 decf 179c 9fa9 7cd3 33f1 99ee  ..........|.3...
-00002630: a3ef afd3 2b36 2cab f760 4b99 6363 7c21  ....+6,..`K.cc|!
-00002640: 4248 39b7 67e2 5856 6ba1 94f7 f79d e232  BH9.g.XVk......2
-00002650: ae83 ec91 4639 18bf 0832 c512 3976 af83  ....F9...2..9v..
-00002660: 7df4 71cd 3497 e909 a5db cfc5 f841 8470  }.q.4........A.p
-00002670: 72e7 7a99 7e50 bafd 5c8c 1744 0826 77b8  r.z.~P..\..D.&w.
-00002680: 4c2f 28dd 7e2e c607 2284 923b 5ca6 0f94  L/(.~..."..;\...
-00002690: 6e3f 17e3 0111 02c9 b93d c7c5 b2fa 91aa  n?.......=......
-000026a0: a55c b87e 9397 fc2e 7ec8 6f09 1513 b31d  .\.~....~.o.....
-000026b0: 54bf 3d81 8c90 50ee acc2 fa94 680d 611d  T.=...P.....h.a.
-000026c0: 1609 d2ca c6ac 6433 2ed9 18d5 8f10 41ce  ......d3......A.
-000026d0: 9a0d 54bf 7d82 55ba f74f d0cd c6a8 be38  ..T.}.U..O.....8
-000026e0: ef79 c7ad d940 f5db 2758 a59b 62a3 62c8  .y...@..'X..b.b.
-000026f0: 1172 c6fa ba61 0cb9 7d82 55ba 3936 4af5  .r...a..}.U.96J.
-00002700: 218a dc61 83d3 83f6 4e25 dea2 c8de cfb4  !..a....N%......
-00002710: 048c fd6b 01e2 c859 ff70 4450 7e7d ddaa  ...k...Y.pDP~}..
-00002720: f28f f24d c643 5ce5 599d 7c83 f7f5 8f64  ...M.C\.Y.|....d
-00002730: 8825 644c b09d e53d ab1f 3f07 8965 bd4e  .%dL...=..?..e.N
-00002740: 6b24 39ae 72fb 34c8 cb63 698c 8bac d5ab  k$9.r.4..ci.....
-00002750: 27cd 328a 623b 4b7c 870d 1c40 add3 1a4b  '.2.b;K|...@...K
-00002760: f6b3 512e 00b1 e40e 1bb8 805a a735 96ec  ..Q........Z.5..
-00002770: 67a3 9c00 62c9 1d36 3855 d6f3 ad26 cfdc  g...b..68U...&..
-00002780: 9f29 e50b 104b eeb0 c1dd 805e a735 79e6  .)...K.....^.5y.
-00002790: 66a3 7c01 62c9 59fd d041 286b 07ad b1e4  f.|.b.Y..A(k....
-000027a0: 7198 dbf7 27bf bdff f9f6 f6f1 e3f5 e3f5  q...'...........
-000027b0: e9ff 0000 00ff ff00 0000 ffff b229 484c  .............)HL
-000027c0: 4ff5 4d2c 4acf cc2b 56c8 494d 2bb1 5532  O.M,J..+V.IM+.U2
-000027d0: d033 5752 28ca 4ccf 80b1 4bf2 0bc0 a2a6  .3WR(.L...K.....
-000027e0: 4a0a 49f9 2525 f9b9 305e 466a 624a 6a11  J.I.%%..0^FjbJj.
-000027f0: 8867 aca4 9096 9f5f 02e3 e8db d9e8 97e7  .g....._........
-00002800: 1765 1767 a4a6 96d8 0100 0000 ffff 0300  .e.g............
-00002810: 504b 0304 1400 0600 0800 0000 2100 d38b  PK..........!...
-00002820: a087 3d03 0000 5a0b 0000 1400 0000 786c  ..=...Z.......xl
-00002830: 2f73 6861 7265 6453 7472 696e 6773 2e78  /sharedStrings.x
-00002840: 6d6c 9456 4d73 9b30 10bd 77a6 ff41 c3b5  ml.VMs.0..w..A..
-00002850: 100c 76dc 8ec7 760e 6e33 b9f4 63d2 8fbb  ..v...v.n3..c...
-00002860: 0c6b d004 242a 8934 f9f7 5d49 0e60 3038  .k..$*.4..]I.`08
-00002870: 194e 48bb 6fdf ae56 abb7 be79 2a0b f208  .NH.o..V...y*...
-00002880: 5231 c137 5e74 35f3 08f0 44a4 8c67 1bef  R1.7^t5...D..g..
-00002890: f7af dbe0 9347 94a6 3ca5 85e0 b0f1 9e41  .....G..<......A
-000028a0: 7937 dbf7 efd6 4a69 82be 5c6d bc5c eb6a  y7....Ji..\m.\.j
-000028b0: 1586 2ac9 a1a4 ea4a 54c0 71e7 2064 4935  ..*....JT.q. dI5
-000028c0: feca 2c54 9504 9aaa 1c40 9745 18cf 66cb  ..,T.....@.E..f.
-000028d0: b0a4 8c7b 2411 35d7 1b6f 31ff e891 9ab3  ...{$.5..o1.....
-000028e0: bf35 ecdc ca32 f6b6 6bc5 b66b bde5 b484  .5...2..k..k....
-000028f0: 75a8 b7eb d0fc bbb5 846a c884 64a0 fa3b  u........j..d..;
-00002900: b434 00fd d51d 957b c149 cac4 134b c127  .4.....{.I...K.'
-00002910: 8c13 cae4 252b 2e78 7010 4ab1 e292 e52b  ....%+.xp.J....+
-00002920: ada4 2889 12ac 2042 923d 1358 2d85 d515  ..(... B.=.X-...
-00002930: c9c3 257c 2dde e457 0a7e 4c74 9258 c7ec  ..%|-..W.~Lt.X..
-00002940: adcc 5ad7 8922 e585 90c2 f441 3fbd cf8c  ..Z..".....A?...
-00002950: 332d 4506 9cbc 00f5 4dbe e89c 723c a9c8  3-E.....M...r<..
-00002960: 375f 1c68 d092 1e8a 1a11 039f dcdd ee82  7_.h............
-00002970: 68be a093 5e81 962c b11c 8cc7 ceb8 2c66  h...^..,......,f
-00002980: 173d 4e63 2ce6 9331 9057 1303 591a 9e92  .=Nc,..1.W..Y...
-00002990: 3508 3664 349f 0819 a42f 0ca3 a00d eca8  5.6d4..../......
-000029a0: 46fb 69c7 53a2 d7f1 04d1 b88d 338e d931  F.i.S.......3..1
-000029b0: b225 1f14 dda5 b318 4508 8ec5 466f 8cd7  .%......E...Fo..
-000029c0: 4f27 1e4d c794 adad 8339 ef93 2aba 938b  O'.M.....9..*...
-000029d0: 47cb 1877 e29e 6b15 4b3b 1ea5 ed48 e3cc  G..w..k.K;...H..
-000029e0: d26d 7bb9 4caf c732 cde1 a9d7 8ad1 72cc  .m{.L..2......r.
-000029f0: f614 d8f6 6d3c 00fe 0ab6 dbfb 18c7 659f  ....m<........e.
-00002a00: ecf1 7ada b637 5398 44b3 5934 6dea 72ea  ..z..7S.D.Y4m.r.
-00002a10: 9e81 738c a30b 8edd eebd 733e f389 60c3  ..s.......s>..`.
-00002a20: 38a6 7271 3cca ce39 0cee c8e0 6c9b cc9b  8.rq<..9....l...
-00002a30: be30 3778 17cc 07f7 7760 d9c9 da9d fc28  .07x....w`.....(
-00002a40: 9917 ecd3 4e8d c74b d42d 28e6 391f cff3  ....N..K.-(.9...
-00002a50: fcd8 6db8 1e5e 3d6e 1b17 3327 9b61 761f  ..m..^=n..3'.av.
-00002a60: 0c07 5963 393e 901b 133b 4c3b 68d1 7859  ..Yc9>...;L;h.xY
-00002a70: 4fe7 ee3d 8ed0 d17a 36a3 b037 00a7 1c4e  O..=...z6..7...N
-00002a80: 86d8 f08e 7fc3 6782 25c4 3e66 7d18 b367  ......g.%.>f}..g
-00002a90: 9f10 8b81 cf7a dfe0 0748 076f ef20 1fec  .....z...H.o. ..
-00002aa0: ffac 8b43 2d49 739b cf40 fcf9 bef3 c9a3  ...C-Is..@......
-00002ab0: 28a8 6605 e0ab 9d51 8e74 1251 56a8 3252  (.f....Q.t.QV.2R
-00002ac0: e5a3 6851 1524 ecc0 20c5 6d96 31de 67c1  ..hQ.$.. .m.1.g.
-00002ad0: a9ae 252d 8804 256a 99c0 6a75 5e7c a01e  ..%-..%j..ju^|..
-00002ae0: 59ad 0af1 0f24 4a02 49b5 5055 0e12 c807  Y....$J.I.PU....
-00002af0: 5257 152e 62b2 d571 ad1f c2ba 9a63 afe5  RW..b..q.....c..
-00002b00: 9e5a 6563 0486 6db2 9c65 b911 70c9 c350  .Zec..m..e..p..P
-00002b10: 2999 801d fe67 515b c4a4 100a 080a 914c  )....gQ[.......L
-00002b20: 9adc cf5a 237d 5289 aa36 f532 720b b862  ...Z#}R..6.2r..b
-00002b30: fad9 2738 b532 7cc1 8742 c032 673c 1562  ..'8.2|..B.2g<.b
-00002b40: 20c6 8c4e 5aad 6886 e75f 17b6 84fd 90ce   ..NZ.h.._......
-00002b50: 02f5 0560 c19e cfef 2276 8dbb 8c0e 249c  ...`...."v....$.
-00002b60: f39e c8bf af19 db7b e537 8789 ad20 2524  .......{.7... %$
-00002b70: 26db 367e 88da 78fb 1f00 00ff ff03 0050  &.6~..x........P
-00002b80: 4b03 0414 0006 0008 0000 0021 00d5 5d15  K..........!..].
-00002b90: d059 0100 0071 0200 0011 0008 0164 6f63  .Y...q.......doc
-00002ba0: 5072 6f70 732f 636f 7265 2e78 6d6c 20a2  Props/core.xml .
-00002bb0: 0401 28a0 0001 0000 0000 0000 0000 0000  ..(.............
-00002bc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002bd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002be0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002bf0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002c00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000920: a330 107d 5f69 ff01 f99d 1a13 2009 2aa9  .0.}_i...... .*.
+00000930: 9a4b 772b b5bb 55af 8f95 034e b002 366b  .Kw+..U....N..6k
+00000940: 9b26 55d5 7fdf 3109 49d3 bc74 db45 896f  .&U...1.I..t.E.o
+00000950: 630e 6766 ced8 c727 abb2 709e 98d2 5c8a  c.gf...'..p...\.
+00000960: 0491 230f 394c a432 e362 9ea0 bbdb 33b7  ..#.9L.2.b....3.
+00000970: 871c 6da8 c868 2105 4bd0 33d3 e864 f0fd  ..m..h!.K.3..d..
+00000980: dbf1 52aa c554 ca85 0300 4227 2837 a68a  ..R..T....B'(7..
+00000990: 31d6 69ce 4aaa 8f64 c504 5866 5295 d4c0  1.i.J..d..XfR...
+000009a0: 54cd b1ae 14a3 99ce 1933 6581 7dcf 8b70  T........3e.}..p
+000009b0: 49b9 406b 8458 7d04 43ce 663c 6563 99d6  I.@k.X}.C.f<ec..
+000009c0: 2513 660d a258 410d d0d7 39af 748b 56a6  %.f..XA...9.t.V.
+000009d0: 1f81 2ba9 5ad4 959b cab2 0288 292f b879  ..+.Z.......)/.y
+000009e0: 6e40 9153 a6f1 f95c 4845 a705 b8bd 22a1  n@.S...\HE....".
+000009f0: b352 f08b e04f 3c68 fcf6 4b60 3af8 54c9  .R...O<h..K`:.T.
+00000a00: 5325 b59c 9923 80c6 6bd2 07fe 130f 13b2  S%...#..k.......
+00000a10: 1782 d561 0c3e 8614 60c5 9eb8 cde1 9695  ...a.>..`.......
+00000a20: 8a3e c92a da62 453b 30e2 7d19 8d80 b41a  .>.*.bE;0.}.....
+00000a30: adc4 10bc 4fa2 855b 6e3e 1a1c cf78 c1ee  ....O..[n>...x..
+00000a40: d7d2 7568 55fd a2a5 cd54 819c 826a 33c9  ..uhU....T...j3.
+00000a50: b861 5982 ba30 954b b65b 00af 545d 0d6b  .aY..0.K.[..T].k
+00000a60: 5e80 9578 1de2 233c d8ca f94a 3919 9bd1  ^..x..#<...J9...
+00000a70: ba30 b720 e416 1e36 4651 df0f ed4e 10c6  .0. ...6FQ...N..
+00000a80: 6961 9812 d4b0 9114 0674 b8f1 ebab 9a6b  ia.......t.....k
+00000a90: b047 b904 853b d7ec 4fcd 1583 c202 7d81  .G...;..O.....}.
+00000aa0: afd0 d234 a653 7d45 4dee d4aa 4810 bed3  ...4.S}EM...H...
+00000ab0: e03c 56d2 5611 fec1 cdcf 7a8a a1c6 4aae  .<V.V.....z...J.
+00000ac0: d9e3 7c59 ed8d 336a 287e 2359 7a58 1fff  ..|Y..3j(~#YzX..
+00000ad0: 205a 9ada 4860 08c5 9aee 7afc 3e2c c05a   Z..H`....z.>,.Z
+00000ae0: c5ad 30af 8c72 607c 3ebe 80e4 dcd0 2748  ..0..r`|>.....'H
+00000af0: 1508 22db 54f2 b9cd 45e7 51a4 2a26 8f2f  ..".T...E.Q.*&./
+00000b00: 91df 0fba c40f dc51 8f9c ba63 2f18 bac3  .......Q...c/...
+00000b10: dec4 77bd 200c 4723 6fdc 0dba c12b 38a3  ..w. .G#o....+8.
+00000b20: a238 95b4 36f9 4605 163a 4101 a4fc c074  .8..6.F..:A....t
+00000b30: 4957 ad85 7871 cdb3 1d8d 176f f3b8 b67f  IW..xq.....o....
+00000b40: d7b4 b657 ebb0 3def ee39 5bea 9d5e ecd4  ...W..=..9[..^..
+00000b50: 593d 7091 c965 e3d1 733b ee46 e0df b231  Y=p..e..s;.F...1
+00000b60: 3cf0 cce4 09f2 7b3d 6fbb f693 f179 0e6c  <.....{=o....y.l
+00000b70: 4927 b48b 5013 9655 82f6 d88c d76c cee0  I'..P..U.....l..
+00000b80: 716d b3c7 06bf a1d3 9caa 40ab e91d d154  qm........@....T
+00000b90: c28d 3d69 091c dfb6 6f02 0cca 8fed 37d4  ..=i....o.....7.
+00000ba0: 7946 9a04 b6af a5b4 4841 f9b6 6b36 4202  yF......HA..k6B.
+00000bb0: 4807 35f3 4b99 41aa 4a2a 6a0a 9565 77fc  H.5.K.A.J*j..ew.
+00000bc0: 166d fa20 246c 652e b469 7a50 2507 fe24  .m. $le..izP%..$
+00000bd0: f04e bb5e 3f70 bd49 2774 835e df77 7b41  .N.^?p.I't.^.w{A
+00000be0: c777 47c1 d89f 84dd c978 320c 6df2 ecb5  .wG......x2.m...
+00000bf0: 11ff 8fc3 b329 8eb8 bd8f ac1b 3955 e656  .....)......9U.V
+00000c00: d174 01b7 d835 9b0d a906 17d6 1e03 5f10  .t...5........_.
+00000c10: 6bcb 1ab7 6f0d fe02 0000 ffff 0300 504b  k...o.........PK
+00000c20: 0304 1400 0600 0800 0000 2100 2796 d6b5  ..........!.'...
+00000c30: ca02 0000 0a07 0000 0d00 0000 786c 2f73  ............xl/s
+00000c40: 7479 6c65 732e 786d 6cb4 55db 6edb 300c  tyles.xml.U.n.0.
+00000c50: 7d1f b07f 10f4 eeca 76e3 2c09 6c17 4b53  }.......v.,.l.KS
+00000c60: 0305 b661 403b 60af 8a2d 2742 7531 2425  ...a@;`..-'Bu1$%
+00000c70: 7336 ecdf 47d9 4ee2 a2dd adc3 5e62 8912  s6..G.N.....^b..
+00000c80: 0f0f 0f29 26bd 6aa5 407b 662c d72a c3d1  ...)&.j.@{f,.*..
+00000c90: 4588 1153 a5ae b8da 64f8 d37d 11cc 30b2  E..S....d..}..0.
+00000ca0: 8eaa 8a0a ad58 860f cce2 abfc f5ab d4ba  .....X..........
+00000cb0: 8360 775b c61c 0208 6533 bc75 ae59 1062  .`w[....e3.u.Y.b
+00000cc0: cb2d 93d4 5ee8 8629 38a9 b591 d4c1 d66c  .-..^..)8......l
+00000cd0: 886d 0ca3 95f5 4e52 9038 0ca7 4452 ae70  .m....NR.8..DR.p
+00000ce0: 8fb0 90e5 9f80 486a 1e76 4d50 6ad9 50c7  ......Hj.vMPj.P.
+00000cf0: d75c 7077 e8b0 3092 e5e2 76a3 b4a1 6b01  .\pw..0...v...k.
+00000d00: 54db 6842 4bd4 4653 13a3 d61c 8374 d627  T.hBK.FS.....t.'
+00000d10: 7124 2f8d b6ba 7617 804b 745d f392 3da5  q$/...v..Kt]..=.
+00000d20: 3b27 7342 cb33 1220 bf0c 294a 4818 3fca  ;'sB.3. ..)JH.?.
+00000d30: bd35 2f44 9a10 c3f6 dc97 0fe7 69ad 95b3  .5/D........i...
+00000d40: a8d4 3be5 321c 0351 2fc1 e241 e92f aaf0  ..;.2..Q/..A./..
+00000d50: 4750 e1e1 569e daaf 684f 0558 624c f2b4  GP..V...hO.XbL..
+00000d60: d442 1be4 a074 a05c e42d 8a4a d6df b8a6  .B...t.\.-.J....
+00000d70: 82af 0df7 c69a 4a2e 0ebd b9f3 ebaa 3ddc  ......J.......=.
+00000d80: 931c b4f7 b788 e7d1 b3c9 d335 18fe 7fac  ...........5....
+00000d90: 2ea4 8598 5c88 9102 bd21 4fa1 551c 33aa  ....\....!O.U.3.
+00000da0: 8053 34ac ef0f 0da4 aaa0 ab7b ca70 f4db  .S4........{.p..
+00000db0: db1b 430f 519c 8c1c 4817 10b2 d4a6 8257  ..C.Q...H......W
+00000dc0: 74d4 decb dc9b f254 b0da 8106 866f b6fe  t......T.....o..
+00000dd0: eb74 03bf 6bed 1c74 5a9e 569c 6eb4 a2c2  .t..k..tZ.V.n...
+00000de0: cb76 f418 1690 4ec9 84b8 f32f ed73 fd08  .v....N..../.s..
+00000df0: bbad 91da c942 badb 2ac3 f066 bde0 c725  .....B..*..f...%
+00000e00: 2432 2c7b bc7e e3f1 c768 3df6 0836 06ca  $2,{.~...h=..6..
+00000e10: 7f0f 8bda fa84 ff33 ef08 f83d 4fea e48d  .......3...=O...
+00000e20: 68d3 8883 efd1 a1fb 3aae c06e 24c1 2301  h.......:..n$.#.
+00000e30: 4ea9 20df a719 fee0 c78c 808e 1fe8 a0f5  N. .............
+00000e40: 8e0b c7d5 33c9 0366 d59e e50c 7d35 9d1f  ....3..f....}5..
+00000e50: 199d d0a7 28a0 6ac5 6aba 13ee fe74 98e1  ....(.j.j....t..
+00000e60: f3fa 3dab f84e c223 1b6e 7de4 7bed 3a88  ..=..N.#.n}.{.:.
+00000e70: 0c9f d7ef 7cd5 a3a9 8fc1 5af7 cec2 b380  ....|.....Z.....
+00000e80: 2fda 199e e16f 37cb 37f3 d54d 1107 b370  /....o7.7..M...p
+00000e90: 390b 2697 2c09 e6c9 7215 2493 ebe5 6a55  9.&.,...r.$...jU
+00000ea0: ccc3 38bc fe3e 1a5c ff30 b6ba 390b 058e  ..8..>.\.0..9...
+00000eb0: 260b 2b60 b899 21d9 81fc ddd9 96e1 d1a6  &.+`..!.........
+00000ec0: a7df f53b d01e 739f c7d3 f06d 1285 4171  ...;..s....m..Aq
+00000ed0: 1946 c164 4a67 c16c 7a99 0445 12c5 abe9  .F.dJg.lz..E....
+00000ee0: 6479 9314 c988 7bf2 c2f1 1692 28ea 07a5  dy....{.....(...
+00000ef0: 279f 2c1c 974c 7075 acd5 b142 632b 1409  '.,..Lpu...Bc+..
+00000f00: b6bf 4882 1c2b 41ce 7f62 f90f 0000 00ff  ..H..+A..b......
+00000f10: ff03 0050 4b03 0414 0006 0008 0000 0021  ...PK..........!
+00000f20: 00c1 1710 be4e 0700 00c6 2000 0013 0000  .....N.... .....
+00000f30: 0078 6c2f 7468 656d 652f 7468 656d 6531  .xl/theme/theme1
+00000f40: 2e78 6d6c ec59 cd8b 1b37 14bf 17fa 3f0c  .xml.Y...7....?.
+00000f50: 7377 fc35 e38f 25de e0cf 6c93 dd24 649d  sw.5..%...l..$d.
+00000f60: 941c b5b6 ec51 5633 3292 bc1b 1302 2539  .....QV32.....%9
+00000f70: f552 28a4 a597 426f 3d94 d240 030d bdf4  .R(...Bo=..@....
+00000f80: 8f09 24b4 e91f d127 cdd8 23ad e524 9b6c  ..$....'..#..$.l
+00000f90: 4a5a 760d 8b47 febd a7a7 f79e 7e7a f374  JZv..G......~z.t
+00000fa0: f1d2 bd98 7a47 980b c292 965f be50 f23d  ....zG....._.P.=
+00000fb0: 9c8c d898 24d3 967f 6b38 2834 7c4f 4894  ....$...k8(4|OH.
+00000fc0: 8c11 6509 6ef9 0b2c fc4b db9f 7e72 116d  ..e.n..,.K..~r.m
+00000fd0: c908 c7d8 03f9 446c a196 1f49 39db 2a16  ......Dl...I9.*.
+00000fe0: c508 8691 b8c0 6638 81df 268c c748 c223  ......f8..&..H.#
+00000ff0: 9f16 c71c 1d83 de98 162b a552 ad18 2392  .........+.R..#.
+00001000: f85e 8262 507b 7d32 2123 ec0d 954a 7f7b  .^.bP{}2!#...J.{
+00001010: a9bc 4fe1 3191 420d 8c28 df57 aab1 25a1  ..O.1.B..(.W..%.
+00001020: b1e3 c3b2 4288 85e8 52ee 1d21 daf2 619e  ....B...R..!..a.
+00001030: 313b 1ee2 7bd2 f728 1212 7e68 f925 fde7  1;..{..(..~h.%..
+00001040: 17b7 2f16 d156 2644 e506 5943 6ea0 ff32  ../..V&D..YCn..2
+00001050: b94c 607c 58d1 73f2 e9c1 6ad2 2008 835a  .L`|X.s...j. ..Z
+00001060: 7ba5 5f03 a85c c7f5 ebfd 5abf b6d2 a701  {._..\....Z.....
+00001070: 6834 8295 a6b6 d83a eb95 6e90 610d 50fa  h4.....:..n.a.P.
+00001080: d5a1 bb57 ef55 cb16 ded0 5f5d b3b9 1daa  ...W.U...._]....
+00001090: 8f85 d7a0 547f b086 1f0c bae0 450b af41  ....T.......E..A
+000010a0: 293e 5cc3 879d 66a7 67eb d7a0 145f 5bc3  )>\...f.g...._[.
+000010b0: d74b ed5e 50b7 f46b 5044 4972 b886 2e85  .K.^P..kPDIr....
+000010c0: b56a 77b9 da15 64c2 e88e 13de 0c83 41bd  .jw...d.......A.
+000010d0: 9229 cf51 900d abec 5253 4c58 2237 e55a  .).Q....RSLX"7.Z
+000010e0: 8cee 323e 0080 0252 2449 e2c9 c50c 4fd0  ..2>...R$I....O.
+000010f0: 08b2 b88b 2839 e0c4 db25 d308 126f 8612  ....(9...%...o..
+00001100: 2660 b854 290d 4a55 f8af 3e81 fea6 238a  &`.T).JU..>...#.
+00001110: b630 32a4 955d 6089 581b 52f6 7862 c4c9  .02..]`.X.R.xb..
+00001120: 4cb6 fc2b a0d5 3720 2f9e 3d7b fef0 e9f3  L..+..7 /.={....
+00001130: 87bf 3d7f f4e8 f9c3 5fb2 b9b5 2a4b 6e07  ..=....._...*Kn.
+00001140: 2553 53ee d58f 5fff fdfd 17de 5fbf fef0  %SS..._....._...
+00001150: eaf1 37e9 d427 f1c2 c4bf fcf9 cb97 bfff  ..7..'..........
+00001160: f13a f5b0 e2dc 152f be7d f2f2 e993 17df  .:...../.}......
+00001170: 7df5 e74f 8f1d dadb 1c1d 98f0 2189 b1f0  }..O........!...
+00001180: aee1 63ef 268b 6181 0efb f101 3f9d c430  ..c.&.a.....?..0
+00001190: 42c4 9240 11e8 76a8 eecb c802 5e5b 20ea  B..@..v.....^[ .
+000011a0: c275 b0ed c2db 1c58 c605 bc3c bf6b d9ba  .u.....X...<.k..
+000011b0: 1ff1 b924 8e99 af46 b105 dc63 8c76 1877  ...$...F...c.v.w
+000011c0: 3ae0 aa9a cbf0 f070 9e4c dd93 f3b9 89bb  :......p.L......
+000011d0: 89d0 916b ee2e 4aac 00f7 e733 a057 e252  ...k..J....3.W.R
+000011e0: d98d b065 e60d 8a12 89a6 38c1 d253 bfb1  ...e......8..S..
+000011f0: 438c 1dab bb43 88e5 d73d 32e2 4cb0 89f4  C....C...=2.L...
+00001200: ee10 af83 88d3 2543 7260 2552 2eb4 4362  ......%Cr`%R..Cb
+00001210: 88cb c265 2084 daf2 cdde 6daf c3a8 6bd5  ...e .....m...k.
+00001220: 3d7c 6423 615b 20ea 307e 88a9 e5c6 cb68  =|d#a[ .0~.....h
+00001230: 2e51 ec52 3944 3135 1dbe 8b64 e432 727f  .Q.R9D15...d.2r.
+00001240: c147 26ae 2f24 447a 8a29 f3fa 632c 844b  .G&./$Dz.)..c,.K
+00001250: e63a 87f5 1a41 bf0a 0ce3 0efb 1e5d c436  .:...A.......].6
+00001260: 924b 72e8 d2b9 8b18 3391 3d76 d88d 503c  .Kr.....3.=v..P<
+00001270: 73da 4c92 c8c4 7e26 0e21 4591 7783 4917  s.L...~&.!E.w.I.
+00001280: 7c8f d93b 443d 431c 50b2 31dc b709 b6c2  |..;D=C.P.1.....
+00001290: fd66 22b8 05e4 6a9a 9427 88fa 65ce 1db1  .f"...j..'..e...
+000012a0: bc8c 99bd 1f17 7482 b08b 65da 3cb6 d8b5  ......t...e.<...
+000012b0: cd89 333b 3af3 a995 dabb 1853 748c c618  ..3;:......St...
+000012c0: 7bb7 3e73 58d0 6133 cbe7 b9d1 5722 6095  {.>sX.a3....W"`.
+000012d0: 1dec 4aac 2bc8 ce55 f59c 6001 6592 aa6b  ..J.+..U..`.e..k
+000012e0: d629 7297 082b 65f7 f194 6db0 676f 7182  .)r..+e...m.goq.
+000012f0: 7816 2889 11df a4f9 1a44 dd4a 5d38 e59c  x.(......D.J]8..
+00001300: 547a 9d8e 0e4d e035 02e5 1fe4 8bd3 29d7  Tz...M.5......).
+00001310: 05e8 3092 bbbf 49eb 8d08 5967 977a 16ee  ..0...I...Yg.z..
+00001320: 7c5d 702b 7e6f b3c7 605f de3d edbe 0419  |]p+~o..`_.=....
+00001330: 7c6a 1920 f6b7 f6cd 1051 6b82 3c61 8608  |j. .....Qk.<a..
+00001340: 0a0c 17dd 8288 15fe 5c44 9dab 5a6c ee94  ........\D..Zl..
+00001350: 9bd8 9b36 0f03 1446 56bd 1393 e48d c5cf  ...6...FV.......
+00001360: 89b2 27fc 77ca 1e77 0173 0605 8f5b f1fb  ..'.w..w.s...[..
+00001370: 943a 9b28 65e7 4481 b309 f71f 2c6b 7a68  .:.(e.D.....,kzh
+00001380: 9edc c070 92ac 73d6 7955 735e d5f8 fffb  ...p..s.yUs^....
+00001390: aa66 d35e 3eaf 65ce 6b99 f35a c6f5 f6f5  .f.^>.e.k..Z....
+000013a0: 416a 99bc 7c81 ca26 eff2 e89e 4fbc b1e5  Aj..|..&....O...
+000013b0: 3321 94ee cb05 c5bb 4277 7d04 bcd1 8c07  3!......Bw}.....
+000013c0: 30a8 db51 ba27 b96a 01ce 22f8 9a35 982c  0..Q.'.j.."..5.,
+000013d0: dc94 232d e371 263f 2732 da8f d00c 5a43  ..#-.q&?'2....ZC
+000013e0: 65dd c09c 8a4c f554 7833 26a0 63a4 8775  e....L.Tx3&.c..u
+000013f0: 2b15 9fd0 adfb 4ef3 788f 8dd3 4e67 b9ac  +.....N.x...Ng..
+00001400: ba9a a90b 0592 f978 295c 8d43 974a a6e8  .......x)\.C.J..
+00001410: 5a3d efde add4 eb7e e854 7759 9706 28d9  Z=.....~.TwY..(.
+00001420: d318 614c 661b 5175 1851 5f0e 4214 5e67  ..aLf.Qu.Q_.B.^g
+00001430: 845e d999 58d1 7458 d150 ea97 a15a 4671  .^..X.tX.P...ZFq
+00001440: e50a 306d 1515 78e5 f6e0 45bd e587 41da  ..0m..x...E...A.
+00001450: 4186 661c 94e7 6315 a7b4 99bc 8cae 0ace  A.f...c.........
+00001460: 9946 7a93 33a9 9901 5062 2f33 208f 7453  .Fz.3...Pb/3 .tS
+00001470: d9ba 7179 6a75 69aa bd45 a42d 238c 74b3  ..qyjui..E.-#.t.
+00001480: 8d30 d230 8217 e12c 3bcd 96fb 59c6 ba99  .0.0...,;...Y...
+00001490: 87d4 324f b962 b91b 7233 ea8d 0f11 6b45  ..2O.b..r3....kE
+000014a0: 2227 b881 2626 53d0 c43b 6ef9 b56a 08b7  "'..&&S..;n..j..
+000014b0: 2a23 346b f913 e818 c3d7 7806 b923 d45b  *#4k......x..#.[
+000014c0: 17a2 53b8 7619 499e 6ef8 7761 9619 17b2  ..S.v.I.n.wa....
+000014d0: 8744 943a 5c93 4eca 0631 9198 7b94 c42d  .D.:\.N..1..{..-
+000014e0: 5f2d 7f95 0d34 d11c a26d 2b57 8010 3e5a  _-...4...m+W..>Z
+000014f0: e39a 402b 1f9b 7110 743b c878 32c1 2369  ..@+..q.t;.x2.#i
+00001500: 86dd 1851 9e4e 1f81 e153 ae70 feaa c5df  ...Q.N...S.p....
+00001510: 1dac 24d9 1cc2 bd1f 8d8f bd03 3ae7 3711  ..$.........:.7.
+00001520: a458 582f 2b07 8e89 808b 8372 eacd 3181  .XX/+......r..1.
+00001530: 9bb0 1591 e5f9 77e2 60ca 68d7 bc8a d239  ......w.`.h....9
+00001540: 948e 233a 8b50 76a2 9864 9ec2 3589 aecc  ..#:.Pv..d..5...
+00001550: d14f 2b1f 184f d99a c1a1 eb2e 3c98 aa03  .O+..O......<...
+00001560: f6bd 4fdd 371f d5ca 7306 69e6 67a6 c52a  ..O.7...s.i.g..*
+00001570: ead4 7493 e987 3be4 0dab f243 d4b2 2aa5  ..t...;....C..*.
+00001580: 6efd 4e2d 72ae 6b2e b90e 12d5 794a bce1  n.N-r.k.....yJ..
+00001590: d47d 8b03 c130 2d9f cc32 4d59 bc4e c38a  .}...0-..2MY.N..
+000015a0: b3b3 51db b433 2c08 0c4f d436 f86d 7546  ..Q..3,..O.6.muF
+000015b0: 383d f1ae 273f c89d cc5a 7540 2ceb 4a9d  8=..'?...Zu@,.J.
+000015c0: f8fa cadc bcd5 6607 7781 3c7a 707f 38a7  ......f.w.<zp.8.
+000015d0: 52e8 5042 6f97 2328 fad2 1bc8 9436 608b  R.PBo.#(.....6`.
+000015e0: dc93 598d 08df bc39 272d ff7e 296c 07dd  ..Y....9'-.~)l..
+000015f0: 4ad8 2d94 1a61 bf10 5483 52a1 11b6 ab85  J.-..a..T.R.....
+00001600: 7618 56cb fdb0 5cea 752a 0fe0 6091 515c  v.V...\.u*..`.Q\
+00001610: 0ed3 ebfa 015c 61d0 4576 69af c7d7 2eee  .....\a.Evi.....
+00001620: e3e5 2dcd 8511 8b8b 4c5f cc17 b5e1 fae2  ..-.....L_......
+00001630: be5c d97c 71ef 1120 9dfb b5ca a059 6d76  .\.|q.. .....Ymv
+00001640: 6a85 66b5 3d28 04bd 4ea3 d0ec d63a 855e  j.f.=(..N....:.^
+00001650: ad5b ef0d 7add b0d1 1c3c f0bd 230d 0eda  .[..z....<..#...
+00001660: d56e 50eb 370a b572 b75b 086a 2565 7ea3  .nP.7..r.[.j%e~.
+00001670: 59a8 0795 4a3b a8b7 1bfd a0fd 202b 6360  Y...J;...... +c`
+00001680: e529 7d64 be00 f76a bbb6 ff01 0000 ffff  .)}d...j........
+00001690: 0300 504b 0304 1400 0600 0800 0000 2100  ..PK..........!.
+000016a0: 678c 4f02 8e11 0000 8b86 0000 1800 0000  g.O.............
+000016b0: 786c 2f77 6f72 6b73 6865 6574 732f 7368  xl/worksheets/sh
+000016c0: 6565 7431 2e78 6d6c 9c93 c96e db30 1086  eet1.xml...n.0..
+000016d0: ef05 fa0e 04ef 3625 d971 12c1 72d0 3a30  ......6%.q..r.:0
+000016e0: 1aa0 87a2 4b72 a6a8 9145 9814 5592 de50  ....Kr...E..U..P
+000016f0: f4dd 33a4 bc01 be18 1124 eefc fe7f c8d1  ..3......$......
+00001700: f469 a715 d980 75d2 b405 4d87 0925 d00a  .i....u...M..%..
+00001710: 53c9 7659 d03f bf17 8307 4a9c e76d c595  S.vY.?....J..m..
+00001720: 69a1 a07b 70f4 69f6 f9d3 746b ecca 3500  i..{p.i...tk..5.
+00001730: 9e20 a175 056d bcef 72c6 9c68 4073 3734  . .u.m..r..h@s74
+00001740: 1db4 3853 1bab b9c7 ae5d 32d7 59e0 55dc  ..8S.....]2.Y.U.
+00001750: a415 cb92 64c2 3497 2ded 09b9 bd85 61ea  ....d.4.-.....a.
+00001760: 5a0a 7836 62ad a1f5 3dc4 82e2 1efd bb46  Z.x6b...=......F
+00001770: 76ee 48d3 e216 9ce6 76b5 ee06 c2e8 0e11  v.H.....v.......
+00001780: a554 d2ef 2394 122d f297 656b 2c2f 15c6  .T..#..-..ek,/..
+00001790: bd4b c75c 909d c537 c36f 7494 89e3 574a  .K.\...7.ot...WJ
+000017a0: 5a0a 6b9c a9fd 10c9 acf7 7c1d fe23 7b64  Z.k.......|..#{d
+000017b0: 5c9c 48d7 f1df 8449 c7cc c246 860b 3ca3  \.H....I...F..<.
+000017c0: b28f 594a ef4e acec 0c1b 7d10 3639 c1c2  ..YJ.N....}.69..
+000017d0: 71d9 7c2d ab82 fe4b 0ecf 00eb 3414 c9b9  q.|-...K....4...
+000017e0: 38ce fda7 b369 25f1 8643 54c4 425d d02f  8....i%..CT.B]./
+000017f0: 693e cfb2 1165 b369 cca0 5709 5b77 d126  i>...e.i..W.[w.&
+00001800: 9e97 bf40 81f0 802a 2925 de74 dfa1 f673  ...@...*)%.t...s
+00001810: 502a ecbe c7cc 0e39 5b1a b30a 7b5f 7055  P*.....9[...{_pU
+00001820: 8232 2eee 0932 5c78 b981 7efd d7f4 0111  .2...2\x..~.....
+00001830: ee6f 948e 1dd4 6527 e1cb f6d1 c422 66fa  .o....e'....."f.
+00001840: 0f4b 4aee 606e d49b ac7c 834e 50b7 829a  .KJ.`n...|.NP...
+00001850: af95 bf18 44f8 61f0 a7d9 7e03 b96c 3c2e  ....D.a...~..l<.
+00001860: 9de0 3185 3ccb abfd 3338 8109 8e1e 8759  ..1.<...38.....Y
+00001870: 8859 1885 4258 122d c38f 8af9 c977 b1de  .Y..BX.-.....w..
+00001880: f63a e3f1 309d 8c93 4976 4749 09ce 2f64  .:..0...IvGI../d
+00001890: 2052 22d6 ce1b 7d34 7340 f510 bce2 08c1   R"...}4s@......
+000018a0: fa00 49ef 6f85 b068 e81d 0000 ffff 0000  ..I.o..h........
+000018b0: 00ff ff94 9ded 6edc 3812 455f 25c8 ff51  ......n.8.E_%..Q
+000018c0: 448a fa1a 640c ac9d 1731 b206 e6d7 ec62  D...d....1.....b
+000018d0: 6c64 77df 7e8b 6a76 8b97 4595 eb06 c860  ldw.~.jv..E....`
+000018e0: 9012 e313 3575 8a2d f655 7f7f fff3 eded  ....5u.-.U......
+000018f0: e3c7 ebc7 ebd3 f7bf fff5 9f2f 7fff f135  .........../...5
+00001900: 7cfd f2fe efd7 bfde e5ff 7e9f be7e f96f  |.........~..~.o
+00001910: 48af 3f7f ffe7 ff7e bcbd ff7c fbeb e38f  H.?....~...|....
+00001920: afe3 10bf 3e7d ff99 0ffd 473e f618 217f  ....>}....G>..!.
+00001930: fe2e 7ffa eb69 fcfe edd7 d3f7 6f3f cb11  .....i......o?..
+00001940: cffa 8880 47bc e823 e2e3 886f c2f4 008b  ....G..#...o....
+00001950: 0498 1cfb 409a 1aa4 ba36 37bc 2ff9 dff6  ....@....67./...
+00001960: ebe9 b713 1210 e47c b8cf 8d1c fb40 589a  .......|.....@X.
+00001970: 7ff4 735d 540c 93c9 9008 0639 f6c1 909a  ..s]T......9....
+00001980: d350 d7e6 f645 4907 c2c5 5998 0902 39f6  .P...EI...Y...9.
+00001990: 92a0 aecd e78b 7e4c ad97 d922 5808 0239  ......~L..."X..9
+000019a0: f692 a0ae cdcd 3c79 592c 8295 2090 632f  ......<yY,.. .c/
+000019b0: 09ea dadc bc44 2fab 45b0 1104 72ec 8360  .....D/.E...r..`
+000019c0: 6ee6 01d4 9ae2 cb66 11ec 0481 1c7b 4900  n......f.....{I.
+000019d0: b576 26ee 1641 1819 59c9 c197 0cf9 6f3a  .v&..A..Y.....o:
+000019e0: 8bed 6494 6ad6 c2c5 f510 2865 cac1 d714  ..d.j.....(e....
+000019f0: 506c 27a4 fc1c 8b82 f163 0009 b6ce 8662  Pl'......c.....b
+00001a00: 3b29 65a8 45c1 2832 8023 5b0a 70e4 d276  ;)e.E.(2.#[.p..v
+00001a10: 8d9b 24af 5e11 4692 a136 61f3 739e a138  ..$.^.F..6a.s..8
+00001a20: b797 8754 ad73 c188 32d4 3654 14a0 4ad5  ...T.s..2.6T..J.
+00001a30: 414d 5706 4696 f9e0 b36b b5af 08e8 525d  AMW.F....k....R]
+00001a40: 23a6 2f03 23cc 7cf0 3505 2853 5d23 a633  #./.#.|.5.(S]#.3
+00001a50: 0323 cd7c f035 0568 535d 23a6 3703 23ce  .#.|.5.hS]#.7.#.
+00001a60: 7cf0 8362 6d5f 1150 6753 7d91 a1d6 6226  |..bm_.PgS}...b&
+00001a70: 32f2 cc07 5f62 4071 de9a 4b55 aa26 0663  2..._b@q..KU.&.c
+00001a80: cf58 0bb2 3d1b 509c f716 e366 cfab a55d  .X..=.P....f...]
+00001a90: a496 97b5 2115 465d 5cd4 02d3 5e61 46c6  ....!.F]\...^aF.
+00001aa0: 9ff9 e0c7 8bd2 9cf6 6728 2a73 4935 bf28  ........g(*sI5.(
+00001ab0: 6918 9798 c6f3 d7d5 da9b 116a ac85 aab0  i..........j....
+00001ac0: cc75 a70c a5b0 18c3 c65a a20a cb5c 8cca  .u.......Z...\..
+00001ad0: 500a 8b51 6eac adaa b0cc 15aa 0ca5 b018  P..Qn...........
+00001ae0: 07c7 5ab3 0acb 5cb6 ca50 0a8b 9172 acbd  ..Z...\..P...r..
+00001af0: db5c e2cf 509c db25 8354 292c c6d2 b116  .\..P..%.T),....
+00001b00: b1c2 024b b76b 0819 ca60 4d8c b5f3 c10f  ...K.k...`M.....
+00001b10: 41b4 5850 54ef 00a5 4a61 3116 9f6a 8b2b  A.XPT...Ja1..j.+
+00001b20: 2c58 03b7 ab0c 194a 6131 569f 6a71 2b2c  ,X.....Ja1V.jq+,
+00001b30: 5814 b7cb 0e19 4a61 5137 126a cb2b 2c58  X.....JaQ7.j.+,X
+00001b40: 25b7 eb90 89b3 fcc4 583e 1ffc 985b a1bd  %.......X>...[..
+00001b50: ef03 55d5 7da4 9a4f 571c d21e aae6 335e  ..U.}..OW.....3^
+00001b60: dd76 6134 3fd5 26d7 5ce6 4a5a c652 5c8c  .va4?.&.\.JZ.R\.
+00001b70: e7a7 5ae5 9acb 5c5b cb58 8a8b 11fd 54bb  ..Z...\[.X....T.
+00001b80: 5c73 99ab 6d19 4b71 31a6 9f6a d36b 2e73  \s..m.Kq1..j.k.s
+00001b90: fd2d 6329 2e46 f553 6df3 a06e ec99 ae97  .-c).F.Sm..n....
+00001ba0: b199 2b2c 431a c336 6efb d9a3 e03e 6362  ..+,C..6n....>cb
+00001bb0: 249f 0f3e 2fc4 1608 aafa 3e5f b9b1 f129  $..>/.....>_...)
+00001bc0: 10a3 f754 1b5c 9d21 a8aa db7e 52f5 9d21  ...T.\.!...~R..!
+00001bd0: 46ec a976 b706 32cd 2e63 7d40 8cd2 536d  F..v..2..c}@..Sm
+00001be0: 6d0d 643a 5dc6 fa80 a81b c520 f3a6 e93e  m.d:]...... ...>
+00001bf0: 2758 b3b7 0b18 a91e 17db 9286 739d 88d3  'X..........s...
+00001c00: 99f1 7702 7f2b 14d3 df32 f633 1446 d909  ..w..+...2.3.F..
+00001c10: 94ad 504c 65cb d8cf 5018 4b27 b0b4 4231  ..PLe...P.K'..B1
+00001c20: 2d2d 633f 4361 c49c 40cc 0ac5 14b3 8cfd  --c?Ca..@.......
+00001c30: 0c85 7171 0217 b71b 3d50 556b 10a9 1ed7  ..qq....=PUk....
+00001c40: d134 8621 ae63 d8f7 7d96 dffb b9c2 8239  .4.!.c..}......9
+00001c50: 3c33 4ace 079f 4a6e b9a0 aa94 2c55 8a8b  <3J...Jn....,U..
+00001c60: 31f3 0c66 565c e6ca 5bc6 525c 8ca0 6710  1..fV\..[.R\..g.
+00001c70: b4e2 3205 2d63 292e c6d3 3378 5a71 999e  ..2.-c)...3xZq..
+00001c80: 96b1 1417 a3eb 1974 ddee ec41 55cd 7ba9  .......t...AU.{.
+00001c90: defa c738 8cfb b64c e3e5 8ca7 f6f9 c0da  ...8...L........
+00001ca0: 8ac8 b4f6 5cee 5f2f 9f12 31f2 9e41 de8a  ....\._/..1..A..
+00001cb0: c894 b78c 759e 23c6 e133 385c 1199 0e97  ....u.#..38\....
+00001cc0: b14e 2246 e533 a85c 1199 2a97 b14e 22c6  .N"F.3.\..*..N".
+00001cd0: e833 18bd ddab 84aa 9ed9 e54e ca36 a621  .3.........N.6.!
+00001ce0: 4dfb b8ca affe 4709 1646 e6f9 e053 e62d  M.....G..F...S.-
+00001cf0: 1254 95cc a59a 4f52 7220 311e 5fc0 e30a  .T....ORr 1._...
+00001d00: c9f4 b88c f522 310a 5f40 e10a c954 b88c  ....."1._@...T..
+00001d10: f522 31f6 5ec0 de0a c9b4 b78c f522 31e2  ."1.^........"1.
+00001d20: 5e40 dced 361f 54d5 f496 6a46 9ab7 380d  ^@..6.T...jF..8.
+00001d30: 6b5c c226 8b96 7cf3 e4e2 a6c9 c2e8 3b1f  k\.&..|.......;.
+00001d40: 7cce 71c5 65ea 5bc6 525c 8cc4 1790 b8e2  |.q.e.[.R\......
+00001d50: 3225 2e63 292e 46e5 0ba8 5c71 992a 97b1  2%.c).F...\q.*..
+00001d60: 1417 23f4 0584 aeb8 4ca1 cb58 8a8b d1fa  ..#.....L..X....
+00001d70: 025a 6f77 cca0 aae7 fd4d ebeb 1687 715a  .Zow.....M....qZ
+00001d80: e3bc 6fb7 75fa 7941 c342 7d65 dc9e 0f3e  ..o.u.yA.B}e...>
+00001d90: e77d cb05 55e5 76a9 e6f3 e5e6 6204 bf82  .}..U.v.....b...
+00001da0: e015 9729 7819 4b71 3196 5fc1 f28a cbb4  ...)x.Kq1._.....
+00001db0: bc8c a5b8 18d5 afa0 7ac5 65aa 5ec6 525c  ........z.e.^.R\
+00001dc0: 8cef 57f0 7dbb 8d06 5535 efa5 7a2c b0a6  ..W.}...U5..z,..
+00001dd0: 7598 9731 8ed3 7ebe 01c1 19cf 987e 05d3  u..1..~......~..
+00001de0: 2b22 d3f4 32d6 49c4 387e 05c7 2b22 d3f1  +"..2.I.8~..+"..
+00001df0: 32d6 49c4 d87d 05bb 2b22 d3ee 32d6 49c4  2.I..}..+"..2.I.
+00001e00: 787d 05af 2b22 d3eb 32d6 49c4 187d 05a3  x}..+"..2.I..}..
+00001e10: b7db 5250 d533 fb66 f471 d8f6 2d2e 312c  ..RP.3.f.q..-.1,
+00001e20: c77d 17f9 cfc5 727d 6394 9e0f 3e95 de82  .}....r}c...>...
+00001e30: 4155 295d aaf9 54f9 c118 a76f e074 0566  AU)]..T....o.t.f
+00001e40: 3a5d c672 608c d437 90ba 0233 a52e 6339  :].r`..7...3..c9
+00001e50: 30c6 ea1b 585d 8199 5697 b11c 18a3 f5ad  0...X]..V.......
+00001e60: d67a 6cf7 3ea1 aa26 bf54 3398 2c62 e210  .zl.>..&.T3.,b..
+00001e70: 45eb 5b4a 5b9e ff17 f7ce 3746 eef9 e0c7  E.[J[.....7F....
+00001e80: dcd7 5ca6 dc65 2cc5 c528 7eab 25ae b94c  ..\..e,..(~.%..L
+00001e90: c5cb 588a 8b11 fd56 ab5c 7399 a297 b114  ..X....V.\s.....
+00001ea0: 17a3 fbad 16ba e632 752f 6329 2e46 fa5b  .......2u/c).F.[
+00001eb0: 2dfd d86e 3542 55cf fb72 bf5d 942f ebf8  -..n5BU..r.]./..
+00001ec0: 392d 71b1 eeb7 ef8c f3f3 c1e7 bc6f b9a0  9-q..........o..
+00001ed0: aa9c 2fd5 a33d 7ab9 18e5 efb5 d4d5 f982  ../..=z.........
+00001ee0: aada 0995 2ac5 c518 7faf 9dae b94c e3cb  ....*........L..
+00001ef0: 588a 8b11 fe5e 2b5d 7399 c297 b114 17e3  X....^+]s.......
+00001f00: fb1d 7cdf 6e79 4155 cd7b a966 ae75 1fa6  ..|.nyAU.{.f.u..
+00001f10: 650d ebb2 a6b2 dae9 df9a dc19 dfe7 83cf  e...............
+00001f20: 79af b84c dfcb 588a 8bf1 fd0e be57 5ca6  y..L..X......W\.
+00001f30: ef65 2cc5 c5f8 7e07 df2b 2ed3 f732 96e2  .e,...~..+...2..
+00001f40: 627c bf83 ef15 97e9 7b19 4b71 31be dfc1  b|......{.Kq1...
+00001f50: f7ed fe17 54f5 bcbf f97e 8ecb 3027 b913  ....T....~..0'..
+00001f60: bf94 8f7a 9dbb 0cf0 2656 6e65 5259 1e30  ...z....&VneRY.0
+00001f70: 7e4b 76fc 658f 0b43 293f 97f3 39f3 b331  ~Kv.e..C)?..9..1
+00001f80: d20f 2358 5fb3 992b fd3c 9a63 63c4 1f46  ..#X_..+.<.cc..F
+00001f90: 30bf 6633 d59f 4773 6c8c fcc3 08f6 d76c  0.f3..Gsl......l
+00001fa0: a6fe f368 8e8d 6900 6184 0ed0 ee94 6159  ...h..i.a.....aY
+00001fb0: c784 64f4 718d 2ecb 2c5d 204c 61a9 3e9d  ..d.q...,] La.>.
+00001fc0: dc5c 068c ffc3 080d 4063 991d 208f 7663  .\......@c.. .vc
+00001fd0: 31fa 0f23 f85f 6399 0d20 8f76 6331 f60f  1..#._c.. .vc1..
+00001fe0: 23e8 5f63 99fe cfa3 dd58 8cfc c308 f6d7  #._c.....X......
+00001ff0: 58a6 fef3 6837 16e3 fe30 82fc dbed 332c  X...h7...0....3,
+00002000: 77a6 7c59 ee87 20db 5569 9f76 f980 cd45  w.|Y.. .Ui.v...E
+00002010: b824 7031 4e88 6a46 c585 494e 9595 bb47  .$p1N.jF..IN...G
+00002020: 395d 5c94 f673 0cf4 5c8c 692e 5bfb f770  9]\..s..\.i.[..p
+00002030: a78b 8b52 3e64 3d3b e7cb 56fe 3dee e9e2  ...R>d=;..V.=...
+00002040: a274 0fe9 cf0e 97ad 7b19 7d2c f75d 5c94  .t......{.},.]\.
+00002050: ea21 f219 5514 f393 4468 8984 8ae2 f721  .!..U...Dh.....!
+00002060: ceb3 2cf8 6334 7669 43ce 7dfa 9fb7 0029  ..,.c4viC.}....)
+00002070: d10e 9bed 7b19 9dcf 999f 8d92 3e64 473b  ....{.......>dG;
+00002080: 6cb6 f465 34c7 4699 1f12 a51d 36db fc32  l..e4.F.....6..2
+00002090: 9a63 a3f4 0f39 d30e 9bad 7f19 cdb1 513d  .c...9........Q=
+000020a0: 00d2 a74b fbc6 2440 59f7 8012 40ad 3ee0  ...K..$@Y...@.>.
+000020b0: 8c6b 1d2a 811a 2065 aa59 3084 aabc 5f52  .k.*.. e.Y0..._R
+000020c0: a8d7 2c94 eb21 6ada 61b1 5d2f a36f eeea  ..,..!j.a.]/.o..
+000020d0: df02 0854 16f5 38fa d177 3a2c b6df e567  ...T..8..w:,...g
+000020e0: d92c 94d3 2174 da61 b19d 5e42 a9d7 af11  .,..!t.a..^B....
+000020f0: e571 88a1 4615 9d86 b27a f446 2849 d4b8  .q..F....z.F(I..
+00002100: 0f17 9b52 21e7 49fd e686 f469 6c77 f08e  ...R!.I....ilw..
+00002110: bfec 7cc3 aa9e 3350 02a8 7190 1ba7 72eb  ..|...3P..q...r.
+00002120: 74be 87a6 ae9e 7f90 43a5 041b 2cd7 351b  t.......C...,.5.
+00002130: 985b 5f59 f770 9297 8d32 37e4 503b e70d  .[_Y.p...27.P;..
+00002140: ccad 9e49 50a2 a8fe f346 991b f2a6 1d36  ...IP....F.....6
+00002150: 30b7 7a52 41c9 a3fa d928 7343 22b5 c356  0.zRA....(sC"..V
+00002160: 2fee 3bb3 ffb6 7a77 b351 a9d4 00c9 d3d8  /.;...zw.Q......
+00002170: eeeb 6159 7795 924c 0d6b 92d4 d216 f6fc  ..aYw..L.k......
+00002180: 39b8 0b91 e6a0 a9ff 3280 586a 070b a4ae  9.......2.Xj....
+00002190: 2e83 924c 7561 51eb 7788 a576 b0c0 efea  ...LuaQ.w..v....
+000021a0: 0a28 c954 1716 a57a c996 566f 77f4 8b08  .(.T...z..Vow...
+000021b0: aa57 93bf 2453 5d58 94f5 2178 da39 5b10  .W..$S]X..!x.9[.
+000021c0: 6552 cfed 28c1 5417 16a5 7f48 a54e ea29  eR..(.T....H.N.)
+000021d0: 6950 ee4c f9db c27d 897b 18e4 3ff3 3aef  iP.L...}.{..?.:.
+000021e0: b75d 84ab 794f e91f 92a9 1d36 5bff 259b  .]..yO.....6[.%.
+000021f0: ea67 a3f4 0fe9 d40e 9bad ff92 4ff5 b351  .g..........O..Q
+00002200: fa87 846a 87cd d67f c9a8 fad9 28fd 434a  ...j........(.CJ
+00002210: b5c3 66eb bfe4 54dd 6c54 5e35 4024 756a  ..f...T.lT^5@$uj
+00002220: 776b b1ac af05 197d 2c58 57c9 1be6 6b61  wk.....},XW...ka
+00002230: dc36 eb63 d021 e74d fd3d 00d2 a91d 36bb  .6.c.!.M.=....6.
+00002240: 07dc d3ab 6e36 aa11 408c b5c3 6637 827b  ....n6..@...f7.{
+00002250: 90d5 cd46 7503 48b4 76d8 ec6e 70cf b4ba  ...Fu.H.v..np...
+00002260: d9a8 9600 f1d5 0e9b dd12 4abc 556e e438  ..........J.Un.8
+00002270: e71b d517 20ed 3aa9 37d8 50ee 5c0b f70f  .... .:.7.P.\...
+00002280: 646e fb24 6f0d e222 8980 abfd b51c 6625  dn.$o.."......f%
+00002290: ae83 5afa 1d2e bb27 94f0 6b98 3c5c 543f  ..Z....'..k.<\T?
+000022a0: 801c 6c87 cbee 0725 09eb e3a2 7a01 8462  ..l....%....z..b
+000022b0: 3b5c 762f 28b1 581f 17d5 0720 03db e1b2  ;\v/(.X.... ....
+000022c0: fbc0 2323 eb78 1da9 806c 800c eca4 f6fa  ..##.x...l......
+000022d0: 3022 abde 0e97 8cec 36ec 610e 7bba 7d8e  0"......6.a.{.}.
+000022e0: 2807 782f d643 39f7 ea9f fb90 92ed b0d9  (.x/.C9.........
+000022f0: 3da0 e464 fd6c 540f 80a4 6c87 cdee 0125  =..d.lT...l....%
+00002300: 2beb 67a3 7a00 a465 3b6c 760f 2879 593f  +.g.z..e;lv.(yY?
+00002310: 1bd5 0320 13db 61b3 7b40 c9cc fad9 a81e  ... ..a.{@......
+00002320: 20f9 d7f3 9dd4 a4f6 ffa0 ac7b c03d 3d3b   ..........{.==;
+00002330: c649 761c a67c 3184 f53a c71e 722e 96b8  .Iv..|1..:..r...
+00002340: 16a0 0f68 36bb 0fdc 73b4 6e36 aa17 409e  ...h6...s.n6..@.
+00002350: b673 deec 5e70 4fd4 bad9 a87e 00c9 da0e  .s..^pO....~....
+00002360: 9bdd 0fee d95a 371b d513 2045 db61 b37b  .....Z7... E.a.{
+00002370: 828c 3ed6 df5e 362a 6b1b 204e 3ba9 4d54  ..>..^6*k. N;.MT
+00002380: 4cdb aabe 50e2 b621 adc3 22fb 6e69 9687  L...P..!..".ni..
+00002390: ec58 9b6f 3947 ebbf 1620 75db 61b3 fb42  .X.o9G... u.a..B
+000023a0: c9dd fad9 a8be 00f1 db0e 9bdd 174a 00d7  .............J..
+000023b0: cf46 f505 c8e1 76d8 ecbe 5092 b87e 36aa  .F....v...P..~6.
+000023c0: 2f40 e4b6 c366 f785 12c9 f5b3 517d 0142  /@...f......Q}.B
+000023d0: b993 da88 86b2 ee0b 2596 bbac cbb0 4914  ........%.....I.
+000023e0: 7e4b d543 e871 1b2e 876c 89ab 003a 82a6  ~K.C.q...l...:..
+000023f0: b23b 4209 e57a a8a8 5e00 81dc ceb9 b27b  .;B..z..^......{
+00002400: 4189 e47a a8a8 2e00 71dc 0e95 dd05 4a20  A..z....q.....J 
+00002410: d743 45f9 1fe2 b61d 2adb ff32 3afb df41  .CE.....*..2:..A
+00002420: 4525 7103 846d 27b5 5d87 595c 65fe 12c6  E%q..m'.].Y\e...
+00002430: 35b6 eb72 a4d6 3fcb 2180 dba1 b15d 5f22  5..r..?.!....]_"
+00002440: b816 0d65 7788 dd76 686c bb97 e0ad 4543  ...ew..vhl....EC
+00002450: f91c c2b6 1d1a dbe7 256e 6bd1 5006 8710  ........%nk.P...
+00002460: 6d87 c636 7809 d95a 3494 b321 5e3b a9ad  m..6x..Z4..!^;..
+00002470: 5428 ab27 d486 12b0 b568 2857 43b4 b643  T(.'.....h(WC..C
+00002480: 03ae d6d7 54d9 d8bd de02 cf41 59e2 9aaa  ....T......AY...
+00002490: 25dc a101 47ab fdb5 12ac b5ce 0de5 6688  %...G.........f.
+000024a0: d476 68c0 cd6a 5bad 846a 2d1a cac9 1098  .vh..j[..j-.....
+000024b0: edd0 8093 f543 efcb 76ed f52b 4545 6865  .....C..v..+EEhe
+000024c0: d55c bf23 55b3 1843 b46a 13ad a468 8d73  .\.#U..C.j...h.s
+000024d0: 93a3 b0fe 7903 c1d9 49ed 3442 59af 834a  ....y...I.4BY..J
+000024e0: 7436 c421 6c53 8c72 1bf7 e226 518e c112  t6.!lS.r...&Q...
+000024f0: 50b5 733b 50a0 6435 994b 6cd6 0145 9919  P.s;P.d5.Kl..E..
+00002500: 02b3 1d28 30b3 9ad3 2532 eb80 a204 0d71  ...(0...%2.....q
+00002510: d80e 1408 5a4d ed12 9775 4051 9e86 a46c  ....ZM...u@Q...l
+00002520: 070a 3e48 a967 78b9 effe f99c a274 0d31  ..>H.gx......t.1
+00002530: d9a4 3689 a1dc 99e8 9fea 3ac7 5d89 195e  ..6.......:.]..^
+00002540: fbb8 4363 ebba c463 2d09 50ba 8648 6c87  ..Cc...c-.P..Hl.
+00002550: c6d6 7509 c55a 3494 ae21 eada a1b1 752d  ..u..Z4..!....u-
+00002560: a3f3 12da a0a1 d2af 0102 ae9a 06f3 af6a  ...............j
+00002570: 3297 00ac 4543 e91a 62ad 496d ef62 ea55  2...EC..b.Im.b.U
+00002580: 2d3a eeb1 d735 6e43 5ac7 650b d547 62f1  -:...5nCZ.e..Gb.
+00002590: 7d6b 4eb1 faa7 3364 5e3b 58b6 b0ef a957  }kN...3d^;X....W
+000025a0: 0f16 a56c 88bc 76b0 6c65 df43 af1e 2c4a  ...l..v.le.C..,J
+000025b0: da90 69ed 60d9 d22e 99d7 e0c1 a2b4 0d81  ..i.`...........
+000025c0: d70e 96ad ed12 7975 6151 e286 bc6b 52bb  ......yuaQ...kR.
+000025d0: b850 d6e2 2e89 57b9 6339 0fab 3c29 30ca  .P....W.c9..<)0.
+000025e0: ed1a ebae 654e b112 f31e 34ae d96c 8d97  ....eN....4..l..
+000025f0: d4ab 9f8d 923a e45e 3be7 cd96 7a49 befa  .....:.^;...zI..
+00002600: d928 c543 bab5 c366 2b5e 461f 7749 9caf  .(.C...f+^F.wI..
+00002610: a944 4488 d7f4 38fa f169 61c5 8665 f5e1  .DD...8..ia..e..
+00002620: ce5c e6d8 18fd 4748 bfa6 7667 17cb ea5a  .\....GH..vg...Z
+00002630: c8e5 cc96 e445 1df6 491e 0c94 a6e3 16fe  .....E..I.......
+00002640: 4574 4c1e a042 9db7 5af2 1d36 b307 e49f  EtL..B..Z..6....
+00002650: c5b1 318d 409e ef55 bde7 eab0 998d 208f  ..1.@..U...... .
+00002660: e6d8 986e 1021 fdda 6133 bb41 1ecd b131  ...n.!..a3.A...1
+00002670: 2d21 4204 b6c3 66b6 843c 9a63 63fa 4284  -!B...f..<.cc.B.
+00002680: 1c6c 6a77 4fb1 dcb9 16ca c3cd 6463 57f6  .ljwO.......dcW.
+00002690: b3c6 492e 8574 1146 9096 415d 07d0 1334  ..I..t.F..A]...4
+000026a0: 97d9 13f2 cf3a 7600 5d5c 4c3f 9087 21d5  .....:v.]\L?..!.
+000026b0: d780 e632 fb41 1eed e762 7a41 8428 6ce7  ...2.A...bzA.(l.
+000026c0: 7534 7b41 1eed e6a2 a2b0 11b2 ae9a 0ba3  u4{A............
+000026d0: b0ed c23f 8ff6 7351 3d00 a2b0 a9dd c58d  ...?..sQ=.......
+000026e0: 5056 dfbb 9bcb 99eb b720 cf61 ebdf ab89  PV....... .a....
+000026f0: 39d3 ea5e 021d 479f edb2 ddb2 c2b2 be0c  9..^..G.........
+00002700: ef09 d865 9448 a73c a36e 99e4 cb5b aeb8  ...e.H.<.n...[..
+00002710: 28e5 4302 3669 2e50 7e7b 0f29 de13 b02e  (.C.6i.P~{.)....
+00002720: 2e4a f710 71ed 7081 eedb db48 f1fe a5a8  .J..q.p....H....
+00002730: 2e2e 4af5 907e ed70 81ea db3b 49b1 a45f  ..J..~.p...;I.._
+00002740: e523 068e d791 d23c 245f 3b5c 709b 5d5f  .#.....<$_;\p.]_
+00002750: 868f 87cd 3bb8 28cd 43ea b56a 1dc7 376c  ....;.(.C..j..7l
+00002760: 3f47 2877 2ec3 fb03 ce24 67b3 8e69 9ee4  ?G(w.....$g..i..
+00002770: 77fe 5cd1 550b a2be 5c35 42ea 35a9 2f18  w.\.U...\5B.5./.
+00002780: 8472 e79a 2cdf 2332 cda3 6c6f e7ef ee98  .r..,.#2..lo....
+00002790: c201 7775 5d52 ba87 586b 870d 74af afcb  ..wu]R..Xk..t...
+000027a0: 7277 c7cb c67d 0f2b c45c 351b a660 d5b5  rw...}.+.\5..`..
+000027b0: 5952 b0d1 cd46 691f 52b1 1d36 d834 55d7  YR...Fi.R..6.4U.
+000027c0: 6749 c5fa d9a8 1e90 33b5 670f 50f3 0dca  gI......3.g.P...
+000027d0: fa2d 5349 c9fa d9a8 3e00 a9d9 a4be 3e12  .-SI....>.....>.
+000027e0: bfc9 559f b7fb 97fc b59f 7efd f6fe e7db  ..U.......~.....
+000027f0: dbc7 8fd7 8fd7 a7ff 0300 00ff ff00 0000  ................
+00002800: ffff b229 484c 4ff5 4d2c 4acf cc2b 56c8  ...)HLO.M,J..+V.
+00002810: 494d 2bb1 5532 d033 5752 28ca 4ccf 80b1  IM+.U2.3WR(.L...
+00002820: 4bf2 0bc0 a2a6 4a0a 49f9 2525 f9b9 305e  K.....J.I.%%..0^
+00002830: 466a 624a 6a11 8867 aca4 9096 9f5f 02e3  FjbJj..g....._..
+00002840: e8db d9e8 97e7 1765 1767 a4a6 96d8 0100  .......e.g......
+00002850: 0000 ffff 0300 504b 0304 1400 0600 0800  ......PK........
+00002860: 0000 2100 91d7 54d3 4403 0000 720b 0000  ..!...T.D...r...
+00002870: 1400 0000 786c 2f73 6861 7265 6453 7472  ....xl/sharedStr
+00002880: 696e 6773 2e78 6d6c 9456 4d73 9b30 10bd  ings.xml.VMs.0..
+00002890: 77a6 ff41 c3b5 100c 76d2 8ec7 760e 6e33  w..A....v...v.n3
+000028a0: b9f4 63d2 8fbb 0c6b d004 242a 8934 fef7  ..c....k..$*.4..
+000028b0: 5d09 07b0 3038 194e 48bb 6fdf ae56 abb7  ]...08.NH.o..V..
+000028c0: ba7d 2e0b f204 5231 c1d7 5e74 35f3 08f0  .}....R1..^t5...
+000028d0: 44a4 8c67 6bef f7af bbe0 9347 94a6 3ca5  D..gk......G..<.
+000028e0: 85e0 b0f6 0ea0 bcdb cdfb 772b a534 415f  ..........w+.4A_
+000028f0: aed6 5eae 75b5 0c43 95e4 5052 7525 2ae0  ..^.u..C..PRu%*.
+00002900: b8b3 17b2 a41a 7f65 16aa 4a02 4d55 0ea0  .......e..J.MU..
+00002910: cb22 8c67 b39b b0a4 8c7b 2411 35d7 6b6f  .".g.....{$.5.ko
+00002920: b1f8 e891 9ab3 bf35 6c9b 959b b9b7 5929  .......5l.....Y)
+00002930: b659 e90d a725 ac42 bd59 85e6 bf59 4ba8  .Y...%.B.Y...YK.
+00002940: 864c 4806 cadd a1a5 0170 57b7 54ee 0427  .LH......pW.T..'
+00002950: 2913 cf2c 059f 304e 2893 97ac b8e0 c15e  )..,..0N(......^
+00002960: 28c5 8a4b 96af b492 a224 4ab0 8208 4976  (..K.....$J...Iv
+00002970: 4c60 b514 5657 248f 97f0 b578 935f 29f8  L`..VW$....x._).
+00002980: 31d1 4962 3db3 b732 eb5c 278a 9417 420a  1.Ib=..2.\'...B.
+00002990: d307 6e7a 9f19 675a 8a0c 3879 0172 4dbe  ..nz..gZ..8y.rM.
+000029a0: e89c 723c a9c8 375f 1c68 d092 ee8b 1a11  ..r<..7_.h......
+000029b0: 039f dcdf 6d83 68be a093 5e81 962c b11c  ....m.h...^..,..
+000029c0: 8cc7 d6b8 2c66 173d 4e63 2ce6 9331 9057  ....,f.=Nc,..1.W
+000029d0: 1b03 591a 9e92 b508 3664 349f 0819 a42f  ..Y.....6d4..../
+000029e0: 0ca3 a00b dc50 8d76 d38e a744 afe3 09a2  .....P.v...D....
+000029f0: 7117 671c b367 644b 3e28 7a93 ce62 1421  q.g..gdK>(z..b.!
+00002a00: 3816 1bbd 319e 9b4e 3c9a 8e29 5b57 0773  8...1..N<..)[W.s
+00002a10: de27 556c 4e2e 1e2d 63dc 8b7b ae55 2ced  .'UlN..-c..{.U,.
+00002a20: 7894 7643 1a67 96ee daab c9f4 7a2c d31c  x.vC.g......z,..
+00002a30: 9e9d 568c 6ec6 6c4f 816d dfc6 03e0 af60  ..V.n.lO.m.....`
+00002a40: bbdd c538 2efb 6487 d7d3 b6bd 99c2 249a  ...8..d.......$.
+00002a50: cda2 69d3 26a7 fe19 348e 7174 c1b1 dfbd  ..i.&...4.qt....
+00002a60: f78d cf7c 22d8 308e a95c 1c8f b26b 1c06  ...|".0..\...k..
+00002a70: 7764 70b6 6de6 6d5f 981b bc0d e683 fb3b  wdp.m.m_.......;
+00002a80: b0ec 65dd 9cfc 2899 17ec d34e 8dc7 4bd4  ..e...(....N..K.
+00002a90: 2f28 e639 1fcf f3fc d86d b9ee 5f3d 6e5b  /(.9.....m.._=n[
+00002aa0: 1733 27db 61f6 100c 0759 6b39 3e90 5b13  .3'.a....Yk9>.[.
+00002ab0: 3b4c 7b68 d178 594f e7ee 038e d0d1 7ab6  ;L{h.xYO......z.
+00002ac0: a3d0 1980 530e 2743 6c78 c7bf e133 c112  ....S.'Clx...3..
+00002ad0: 621f 3317 c6ec d927 c462 e0b3 ee1a fc00  b.3....'.b......
+00002ae0: d9c0 db3b c807 fb3f eb62 5f4b d2de e633  ...;...?.b_K...3
+00002af0: 107f be6f 7df2 240a aa59 01f8 6a67 9423  ...o}.$..Y..jg.#
+00002b00: 9d44 9415 aa8c 54f9 285a 5405 09db 3348  .D....T.(ZT...3H
+00002b10: 719b 658c bb2c 38d5 b5a4 0591 a044 2d13  q.e..,8......D-.
+00002b20: 582e cf8b 0fd4 23cb 6521 fe81 4449 20a9  X.....#.e!..DI .
+00002b30: 16aa ca41 02f9 40ea aac2 454c b63a aeb9  ...A..@...EL.:..
+00002b40: 21ac ab39 f65a eea8 5536 4660 d826 cb59  !..9.Z..U6F`.&.Y
+00002b50: 961b 0197 3c0e 9592 09d8 e37f 16b5 434c  ....<.........CL
+00002b60: 0aa1 80a0 10c9 a4c9 fdac 35d2 2795 a86a  ..........5.'..j
+00002b70: 532f 23b7 802b a60f 3ec1 a995 e10b 3e14  S/#..+..>.....>.
+00002b80: 0296 39e3 a910 0331 6674 d272 4933 3cff  ..9....1ft.rI3<.
+00002b90: bab0 2574 4336 16a8 2f00 0b76 38bf 8bd8  ..%tC6../..v8...
+00002ba0: 35ee 323a 9070 8df7 44fe ae66 ecee 95df  5.2:.p..D..f....
+00002bb0: 1e26 b682 9490 986c ddf8 f787 d4b6 67b7  .&.....l......g.
+00002bc0: 1ea2 66de fc07 0000 ffff 0300 504b 0304  ..f.........PK..
+00002bd0: 1400 0600 0800 0000 2100 5333 c060 5a01  ........!.S3.`Z.
+00002be0: 0000 7102 0000 1100 0801 646f 6350 726f  ..q.......docPro
+00002bf0: 7073 2f63 6f72 652e 786d 6c20 a204 0128  ps/core.xml ...(
+00002c00: a000 0100 0000 0000 0000 0000 0000 0000  ................
 00002c10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002c20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002c30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002c40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002c50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002c60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002c70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002c80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002c90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002ca0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002cb0: 0000 0000 0000 7c92 514b c330 1485 df05  ......|.QK.0....
-00002cc0: ff43 c97b 9ba6 7532 4bdb 8193 3d59 14dc  .C.{..u2K...=Y..
-00002cd0: 507c 0bc9 ed16 6c93 9064 cefd 7bd3 76ab  P|....l..d..{.v.
-00002ce0: 1d8a 8fb9 e7e4 cb39 97e4 8baf b609 3ec1  .......9......>.
-00002cf0: 58a1 6481 4814 a300 2453 5cc8 6d81 36eb  X.d.H...$S\.m.6.
-00002d00: 5538 4781 7554 72da 2809 053a 8245 8bf2  U8G.uTr.(..:.E..
-00002d10: fa2a 673a 63ca c0b3 511a 8c13 6003 4f92  .*g:c...Q...`.O.
-00002d20: 3663 ba40 3be7 7486 b165 3b68 a98d bc43  6c.@;.t..e;h...C
-00002d30: 7ab1 56a6 a5ce 1fcd 166b ca3e e816 7012  z.V......k.>..p.
-00002d40: c7b7 b805 4739 7514 77c0 508f 4474 4272  ....G9u.w.P.DtBr
-00002d50: 3622 f5de 343d 8033 0c0d b420 9dc5 2422  6"..4=.3... ..$"
-00002d60: f8c7 ebc0 b4f6 cf0b bd32 71b6 c21d b5ef  .........2q.....
-00002d70: 748a 3b65 7336 88a3 fbcb 8ad1 7838 1ca2  t.;es6......x8..
-00002d80: 43da c7f0 f909 7eab 1e5f faaa a190 ddae  C.....~.._......
-00002d90: 18a0 32e7 2c63 06a8 53a6 5cee 8cb0 41b5  ..2.,c..S.\...A.
-00002da0: 77d0 e478 32ef 76d8 50eb 2abf ee5a 00bf  w..x2.v.P.*..Z..
-00002db0: 3f96 9560 4659 55bb e0a9 ae05 8360 63c1  ?..`FYU......`c.
-00002dc0: e4f8 b7d1 f3fb 3ac3 23c0 031f 301b ea9c  ......:.#...0...
-00002dd0: 95d7 74f9 b05e a132 8913 12c6 4998 24eb  ..t..^.2....I.$.
-00002de0: 789e cd48 36bb 7bef 725c dcef 020f 83f6  x..H6.{.r\......
-00002df0: 94e6 7f62 1ac6 3721 9977 4412 67e9 9478  ...b..7!.wD.g..x
-00002e00: 0694 7dee cb4f 527e 0300 00ff ff03 0050  ..}..OR~.......P
-00002e10: 4b03 0414 0006 0008 0000 0021 00e4 ee61  K..........!...a
-00002e20: 559b 0100 0033 0300 0010 0008 0164 6f63  U....3.......doc
-00002e30: 5072 6f70 732f 6170 702e 786d 6c20 a204  Props/app.xml ..
-00002e40: 0128 a000 0100 0000 0000 0000 0000 0000  .(..............
-00002e50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002e60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002e70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002e80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002e90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002cb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002cc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002cd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002ce0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002cf0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002d00: 0000 007c 9251 4bc3 3014 85df 05ff 43c8  ...|.QK.0.....C.
+00002d10: 7b9b a673 324b db81 933d 5914 dc50 7c0b  {..s2K...=Y..P|.
+00002d20: c9ed 166c 9392 64d6 fd7b d376 ab1d 8a8f  ...l..d..{.v....
+00002d30: b9e7 e4cb 3997 a4cb afba 429f 60ac d42a  ....9.....B.`..*
+00002d40: c334 8c30 02c5 b590 6a97 e1ed 661d 2c30  .4.0....j...f.,0
+00002d50: b28e 29c1 2aad 20c3 47b0 7899 5f5f a5bc  ..).*. .G.x.__..
+00002d60: 49b8 36f0 6c74 03c6 49b0 c893 944d 7893  I.6.lt..I....Mx.
+00002d70: e1bd 734d 4288 e57b a899 0dbd 4379 b1d4  ..sMB..{....Cy..
+00002d80: a666 ce1f cd8e 348c 7fb0 1d90 388a 6e49  .f....4.....8.nI
+00002d90: 0d8e 09e6 18e9 8041 3312 f109 29f8 886c  .......A3...)..l
+00002da0: 0ea6 ea01 8213 a8a0 06e5 2ca1 2125 3f5e  ..........,.!%?^
+00002db0: 07a6 b67f 5ee8 9589 b396 eed8 f84e a7b8  ....^........N..
+00002dc0: 53b6 e083 38ba bfac 1c8d 6ddb 86ed ac8f  S...8.....m.....
+00002dd0: e1f3 53f2 563c bef4 5503 a9ba 5d71 c079  ..S.V<..U...]q.y
+00002de0: 2a78 c20d 30a7 4dbe da1b 6951 7170 50a5  *x..0.M...iQqpP.
+00002df0: 6432 ef76 5831 eb0a bfee 5282 b83f e685  d2.vX1....R..?..
+00002e00: e446 5b5d 3af4 5496 9203 da5a 3029 f96d  .F[]:.T....Z0).m
+00002e10: f4fc bece f008 08e4 0326 439d b3f2 3a5b  .........&C...:[
+00002e20: 3d6c d638 8fa3 9806 511c c4f1 265a 2473  =l.8....Q...&Z$s
+00002e30: 9acc efde bb1c 17f7 bbc0 c3a0 3ea5 f99f  ............>...
+00002e40: 380b a29b 802e 3a22 a549 3c9f 10cf 80bc  8.....:".I<.....
+00002e50: cf7d f949 f26f 0000 00ff ff03 0050 4b03  .}.I.o.......PK.
+00002e60: 0414 0006 0008 0000 0021 00e4 ee61 559b  .........!...aU.
+00002e70: 0100 0033 0300 0010 0008 0164 6f63 5072  ...3.......docPr
+00002e80: 6f70 732f 6170 702e 786d 6c20 a204 0128  ops/app.xml ...(
+00002e90: a000 0100 0000 0000 0000 0000 0000 0000  ................
 00002ea0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002eb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002ec0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002ed0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002ee0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002ef0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002f00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002f10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002f20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002f30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002f40: 0000 0000 009c 934d 6fdb 300c 86ef 03f6  .......Mo.0.....
-00002f50: 1f0c dd1b 395d 510c 81ac a248 5bf4 b0a2  ....9]Q....H[...
-00002f60: 01e2 7667 4ea6 63a1 b264 88ac 91ec d757  ..vgN.c..d.....W
-00002f70: b6d1 c4d9 76da 8d1f 2f5e 3ea2 2475 b36f  ....v.../^>.$u.o
-00002f80: 5dd6 6324 1b7c 2196 8b5c 64e8 4da8 acdf  ].c$.|!..\d.M...
-00002f90: 15e2 a57c b8f8 2e32 62f0 15b8 e0b1 1007  ...|...2b.......
-00002fa0: 2471 a3bf 7e51 9b18 3a8c 6c91 b264 e1a9  $q..~Q..:.l..d..
-00002fb0: 100d 73b7 9292 4c83 2dd0 22b5 7dea d421  ..s...L.-.".}..!
-00002fc0: b6c0 298d 3b19 eada 1abc 0be6 bd45 cff2  ..).;........E..
-00002fd0: 32cf af25 ee19 7d85 d545 7734 1493 e3aa  2..%..}..Ew4....
-00002fe0: e7ff 35ad 8219 f8e8 b53c 7409 58ab 3230  ..5......<t.X.20
-00002ff0: b8d2 b6a8 7325 4f89 baed 3a67 0d70 3abd  ....s%O...:g.p:.
-00003000: 7eb2 2606 0a35 674f 60ac e740 4d76 bf37  ~.&..5gO`..@Mv.7
-00003010: e894 9ccb 54e2 dfa2 798f 960f 83db 3c55  ....T...y.....<U
-00003020: 5b03 0ed7 69b4 aec1 112a 792a a847 8461  [...i....*y*.G.a
-00003030: ad1b b091 b4ea 79d5 a3e1 1033 b2bf d362  ......y....3...b
-00003040: 2f45 f60b 0807 e042 f410 2d78 4ee0 836c  /E.....B..-xN..l
-00003050: 4ac6 d875 c451 ff0c f18d 1a44 2625 9360  J..u.Q.....D&%.`
-00003060: 2a8e e15c 3b8f ed95 5e8e 8214 9c0b 0783  *..\;...^.......
-00003070: 0924 35ce 114b cb0e e9b9 de40 e47f 102f  .$5..K.....@.../
-00003080: e7c4 23c3 c43b e16c 07be 69e6 9c6f 3c72  ..#..;.l..i..o<r
-00003090: 9af4 87f7 3ab4 1df8 436a 1ca3 1fd6 bfd1  ....:...Cj......
-000030a0: 4b57 863b 60fc 5ce7 7951 6d1b 8858 a51b  KW.;`.\.yQm..X..
-000030b0: 38ae fb58 508f 6993 d10d 26eb 06fc 0eab  8..XP.i...&.....
-000030c0: 4fcd df8d e119 bc4e 7f40 2faf 17f9 b73c  O......N.@/....<
-000030d0: ddeb aca6 e4e9 b5eb 0f00 0000 ffff 0300  ................
-000030e0: 504b 0102 2d00 1400 0600 0800 0000 2100  PK..-.........!.
-000030f0: 62ee 9d68 5e01 0000 9004 0000 1300 0000  b..h^...........
-00003100: 0000 0000 0000 0000 0000 0000 0000 5b43  ..............[C
-00003110: 6f6e 7465 6e74 5f54 7970 6573 5d2e 786d  ontent_Types].xm
-00003120: 6c50 4b01 022d 0014 0006 0008 0000 0021  lPK..-.........!
-00003130: 00b5 5530 23f4 0000 004c 0200 000b 0000  ..U0#....L......
-00003140: 0000 0000 0000 0000 0000 0097 0300 005f  ..............._
-00003150: 7265 6c73 2f2e 7265 6c73 504b 0102 2d00  rels/.relsPK..-.
-00003160: 1400 0600 0800 0000 2100 813e 9497 f300  ........!..>....
-00003170: 0000 ba02 0000 1a00 0000 0000 0000 0000  ................
-00003180: 0000 0000 bc06 0000 786c 2f5f 7265 6c73  ........xl/_rels
-00003190: 2f77 6f72 6b62 6f6f 6b2e 786d 6c2e 7265  /workbook.xml.re
-000031a0: 6c73 504b 0102 2d00 1400 0600 0800 0000  lsPK..-.........
-000031b0: 2100 37dd 5965 0303 0000 0907 0000 0f00  !.7.Ye..........
-000031c0: 0000 0000 0000 0000 0000 0000 ef08 0000  ................
-000031d0: 786c 2f77 6f72 6b62 6f6f 6b2e 786d 6c50  xl/workbook.xmlP
-000031e0: 4b01 022d 0014 0006 0008 0000 0021 0027  K..-.........!.'
-000031f0: 96d6 b5ca 0200 000a 0700 000d 0000 0000  ................
-00003200: 0000 0000 0000 0000 001f 0c00 0078 6c2f  .............xl/
-00003210: 7374 796c 6573 2e78 6d6c 504b 0102 2d00  styles.xmlPK..-.
-00003220: 1400 0600 0800 0000 2100 c117 10be 4e07  ........!.....N.
-00003230: 0000 c620 0000 1300 0000 0000 0000 0000  ... ............
-00003240: 0000 0000 140f 0000 786c 2f74 6865 6d65  ........xl/theme
-00003250: 2f74 6865 6d65 312e 786d 6c50 4b01 022d  /theme1.xmlPK..-
-00003260: 0014 0006 0008 0000 0021 004f 821b e147  .........!.O...G
-00003270: 1100 0074 8400 0018 0000 0000 0000 0000  ...t............
-00003280: 0000 0000 0093 1600 0078 6c2f 776f 726b  .........xl/work
-00003290: 7368 6565 7473 2f73 6865 6574 312e 786d  sheets/sheet1.xm
-000032a0: 6c50 4b01 022d 0014 0006 0008 0000 0021  lPK..-.........!
-000032b0: 00d3 8ba0 873d 0300 005a 0b00 0014 0000  .....=...Z......
-000032c0: 0000 0000 0000 0000 0000 0010 2800 0078  ............(..x
-000032d0: 6c2f 7368 6172 6564 5374 7269 6e67 732e  l/sharedStrings.
-000032e0: 786d 6c50 4b01 022d 0014 0006 0008 0000  xmlPK..-........
-000032f0: 0021 00d5 5d15 d059 0100 0071 0200 0011  .!..]..Y...q....
-00003300: 0000 0000 0000 0000 0000 0000 007f 2b00  ..............+.
-00003310: 0064 6f63 5072 6f70 732f 636f 7265 2e78  .docProps/core.x
-00003320: 6d6c 504b 0102 2d00 1400 0600 0800 0000  mlPK..-.........
-00003330: 2100 e4ee 6155 9b01 0000 3303 0000 1000  !...aU....3.....
-00003340: 0000 0000 0000 0000 0000 0000 0f2e 0000  ................
-00003350: 646f 6350 726f 7073 2f61 7070 2e78 6d6c  docProps/app.xml
-00003360: 504b 0506 0000 0000 0a00 0a00 8002 0000  PK..............
-00003370: e030 0000 0000                           .0....
+00002f40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002f50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002f60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002f70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002f80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002f90: 0000 009c 934d 6fdb 300c 86ef 03f6 1f0c  .....Mo.0.......
+00002fa0: dd1b 395d 510c 81ac a248 5bf4 b0a2 01e2  ..9]Q....H[.....
+00002fb0: 7667 4ea6 63a1 b264 88ac 91ec d757 b6d1  vgN.c..d.....W..
+00002fc0: c4d9 76da 8d1f 2f5e 3ea2 2475 b36f 5dd6  ..v.../^>.$u.o].
+00002fd0: 6324 1b7c 2196 8b5c 64e8 4da8 acdf 15e2  c$.|!..\d.M.....
+00002fe0: a57c b8f8 2e32 62f0 15b8 e0b1 1007 2471  .|...2b.......$q
+00002ff0: a3bf 7e51 9b18 3a8c 6c91 b264 e1a9 100d  ..~Q..:.l..d....
+00003000: 73b7 9292 4c83 2dd0 22b5 7dea d421 b6c0  s...L.-.".}..!..
+00003010: 298d 3b19 eada 1abc 0be6 bd45 cff2 32cf  ).;........E..2.
+00003020: af25 ee19 7d85 d545 7734 1493 e3aa e7ff  .%..}..Ew4......
+00003030: 35ad 8219 f8e8 b53c 7409 58ab 3230 b8d2  5......<t.X.20..
+00003040: b6a8 7325 4f89 baed 3a67 0d70 3abd 7eb2  ..s%O...:g.p:.~.
+00003050: 2606 0a35 674f 60ac e740 4d76 bf37 e894  &..5gO`..@Mv.7..
+00003060: 9ccb 54e2 dfa2 798f 960f 83db 3c55 5b03  ..T...y.....<U[.
+00003070: 0ed7 69b4 aec1 112a 792a a847 8461 ad1b  ..i....*y*.G.a..
+00003080: b091 b4ea 79d5 a3e1 1033 b2bf d362 2f45  ....y....3...b/E
+00003090: f60b 0807 e042 f410 2d78 4ee0 836c 4ac6  .....B..-xN..lJ.
+000030a0: d875 c451 ff0c f18d 1a44 2625 9360 2a8e  .u.Q.....D&%.`*.
+000030b0: e15c 3b8f ed95 5e8e 8214 9c0b 0783 0924  .\;...^........$
+000030c0: 35ce 114b cb0e e9b9 de40 e47f 102f e7c4  5..K.....@.../..
+000030d0: 23c3 c43b e16c 07be 69e6 9c6f 3c72 9af4  #..;.l..i..o<r..
+000030e0: 87f7 3ab4 1df8 436a 1ca3 1fd6 bfd1 4b57  ..:...Cj......KW
+000030f0: 863b 60fc 5ce7 7951 6d1b 8858 a51b 38ae  .;`.\.yQm..X..8.
+00003100: fb58 508f 6993 d10d 26eb 06fc 0eab 4fcd  .XP.i...&.....O.
+00003110: df8d e119 bc4e 7f40 2faf 17f9 b73c ddeb  .....N.@/....<..
+00003120: aca6 e4e9 b5eb 0f00 0000 ffff 0300 504b  ..............PK
+00003130: 0102 2d00 1400 0600 0800 0000 2100 62ee  ..-.........!.b.
+00003140: 9d68 5e01 0000 9004 0000 1300 0000 0000  .h^.............
+00003150: 0000 0000 0000 0000 0000 0000 5b43 6f6e  ............[Con
+00003160: 7465 6e74 5f54 7970 6573 5d2e 786d 6c50  tent_Types].xmlP
+00003170: 4b01 022d 0014 0006 0008 0000 0021 00b5  K..-.........!..
+00003180: 5530 23f4 0000 004c 0200 000b 0000 0000  U0#....L........
+00003190: 0000 0000 0000 0000 0097 0300 005f 7265  ............._re
+000031a0: 6c73 2f2e 7265 6c73 504b 0102 2d00 1400  ls/.relsPK..-...
+000031b0: 0600 0800 0000 2100 813e 9497 f300 0000  ......!..>......
+000031c0: ba02 0000 1a00 0000 0000 0000 0000 0000  ................
+000031d0: 0000 bc06 0000 786c 2f5f 7265 6c73 2f77  ......xl/_rels/w
+000031e0: 6f72 6b62 6f6f 6b2e 786d 6c2e 7265 6c73  orkbook.xml.rels
+000031f0: 504b 0102 2d00 1400 0600 0800 0000 2100  PK..-.........!.
+00003200: 082f ba25 0203 0000 0907 0000 0f00 0000  ./.%............
+00003210: 0000 0000 0000 0000 0000 ef08 0000 786c  ..............xl
+00003220: 2f77 6f72 6b62 6f6f 6b2e 786d 6c50 4b01  /workbook.xmlPK.
+00003230: 022d 0014 0006 0008 0000 0021 0027 96d6  .-.........!.'..
+00003240: b5ca 0200 000a 0700 000d 0000 0000 0000  ................
+00003250: 0000 0000 0000 001e 0c00 0078 6c2f 7374  ...........xl/st
+00003260: 796c 6573 2e78 6d6c 504b 0102 2d00 1400  yles.xmlPK..-...
+00003270: 0600 0800 0000 2100 c117 10be 4e07 0000  ......!.....N...
+00003280: c620 0000 1300 0000 0000 0000 0000 0000  . ..............
+00003290: 0000 130f 0000 786c 2f74 6865 6d65 2f74  ......xl/theme/t
+000032a0: 6865 6d65 312e 786d 6c50 4b01 022d 0014  heme1.xmlPK..-..
+000032b0: 0006 0008 0000 0021 0067 8c4f 028e 1100  .......!.g.O....
+000032c0: 008b 8600 0018 0000 0000 0000 0000 0000  ................
+000032d0: 0000 0092 1600 0078 6c2f 776f 726b 7368  .......xl/worksh
+000032e0: 6565 7473 2f73 6865 6574 312e 786d 6c50  eets/sheet1.xmlP
+000032f0: 4b01 022d 0014 0006 0008 0000 0021 0091  K..-.........!..
+00003300: d754 d344 0300 0072 0b00 0014 0000 0000  .T.D...r........
+00003310: 0000 0000 0000 0000 0056 2800 0078 6c2f  .........V(..xl/
+00003320: 7368 6172 6564 5374 7269 6e67 732e 786d  sharedStrings.xm
+00003330: 6c50 4b01 022d 0014 0006 0008 0000 0021  lPK..-.........!
+00003340: 0053 33c0 605a 0100 0071 0200 0011 0000  .S3.`Z...q......
+00003350: 0000 0000 0000 0000 0000 00cc 2b00 0064  ............+..d
+00003360: 6f63 5072 6f70 732f 636f 7265 2e78 6d6c  ocProps/core.xml
+00003370: 504b 0102 2d00 1400 0600 0800 0000 2100  PK..-.........!.
+00003380: e4ee 6155 9b01 0000 3303 0000 1000 0000  ..aU....3.......
+00003390: 0000 0000 0000 0000 0000 5d2e 0000 646f  ..........]...do
+000033a0: 6350 726f 7073 2f61 7070 2e78 6d6c 504b  cProps/app.xmlPK
+000033b0: 0506 0000 0000 0a00 0a00 8002 0000 2e31  ...............1
+000033c0: 0000 0000                                ....
```

### Comparing `premise_gwp-0.8/premise_gwp/data/lcia_gwp_100a.xlsx` & `premise_gwp-0.9/premise_gwp/data/lcia_gwp_100a.xlsx`

 * *Files identical despite different names*

### Comparing `premise_gwp-0.8/premise_gwp/data/lcia_gwp_100a_w_bio.xlsx` & `premise_gwp-0.9/premise_gwp/data/lcia_gwp_20a_w_bio.xlsx`

 * *Files 22% similar despite different names*

```diff
@@ -137,65 +137,65 @@
 00000880: cbb4 e480 fa84 53ec ad82 b4b7 b720 9a29  ......S...... .)
 00000890: 66e5 ffb9 43db f606 9f82 791f d1f3 1909  f...C.....y.....
 000008a0: 493c 0d79 00d1 e8d4 212b f8c1 45f6 08f2  I<.y....!+..E...
 000008b0: bcfc 664d 79ce 6bc1 a3fa 0ce5 1cab 4b1e  ..fMy.k.......K.
 000008c0: aa35 3d7c 8674 2087 c847 1f7f 2992 73e5  .5=|.t ..G..).s.
 000008d0: a299 bb55 efe1 7442 fbca 29bf dbf2 2ccb  ...U..tB..)...,.
 000008e0: f4ef 66e4 c9c7 d5df 0000 00ff ff03 0050  ..f............P
-000008f0: 4b03 0414 0006 0008 0000 0021 0008 2fba  K..........!../.
-00000900: 2502 0300 0009 0700 000f 0000 0078 6c2f  %............xl/
+000008f0: 4b03 0414 0006 0008 0000 0021 00d4 8db4  K..........!....
+00000900: 0e02 0300 0009 0700 000f 0000 0078 6c2f  .............xl/
 00000910: 776f 726b 626f 6f6b 2e78 6d6c ac55 db6e  workbook.xml.U.n
-00000920: a330 107d 5f69 ff01 f99d 1a13 2009 2aa9  .0.}_i...... .*.
-00000930: 9a4b 772b b5bb 55af 8f95 034e b002 366b  .Kw+..U....N..6k
-00000940: 9b26 55d5 7fdf 3109 49d3 bc74 db45 896f  .&U...1.I..t.E.o
-00000950: 630e 6766 ced8 c727 abb2 709e 98d2 5c8a  c.gf...'..p...\.
-00000960: 0491 230f 394c a432 e362 9ea0 bbdb 33b7  ..#.9L.2.b....3.
-00000970: 871c 6da8 c868 2105 4bd0 33d3 e864 f0fd  ..m..h!.K.3..d..
-00000980: dbf1 52aa c554 ca85 0300 4227 2837 a68a  ..R..T....B'(7..
-00000990: 31d6 69ce 4aaa 8f64 c504 5866 5295 d4c0  1.i.J..d..XfR...
-000009a0: 54cd b1ae 14a3 99ce 1933 6581 7dcf 8b70  T........3e.}..p
-000009b0: 49b9 406b 8458 7d04 43ce 663c 6563 99d6  I.@k.X}.C.f<ec..
-000009c0: 2513 660d a258 410d d0d7 39af 748b 56a6  %.f..XA...9.t.V.
-000009d0: 1f81 2ba9 5ad4 959b cab2 0288 292f b879  ..+.Z.......)/.y
-000009e0: 6e40 9153 a6f1 f95c 4845 a705 b8bd 22a1  n@.S...\HE....".
-000009f0: b352 f08b e04f 3c68 fcf6 4b60 3af8 54c9  .R...O<h..K`:.T.
-00000a00: 5325 b59c 9923 80c6 6bd2 07fe 130f 13b2  S%...#..k.......
-00000a10: 1782 d561 0c3e 8614 60c5 9eb8 cde1 9695  ...a.>..`.......
-00000a20: 8a3e c92a da62 453b 30e2 7d19 8d80 b41a  .>.*.bE;0.}.....
-00000a30: adc4 10bc 4fa2 855b 6e3e 1a1c cf78 c1ee  ....O..[n>...x..
-00000a40: d7d2 7568 55fd a2a5 cd54 819c 826a 33c9  ..uhU....T...j3.
-00000a50: b861 5982 ba30 954b b65b 00af 545d 0d6b  .aY..0.K.[..T].k
-00000a60: 5e80 9578 1de2 233c d8ca f94a 3919 9bd1  ^..x..#<...J9...
-00000a70: ba30 b720 e416 1e36 4651 df0f ed4e 10c6  .0. ...6FQ...N..
-00000a80: 6961 9812 d4b0 9114 0674 b8f1 ebab 9a6b  ia.......t.....k
-00000a90: b047 b904 853b d7ec 4fcd 1583 c202 7d81  .G...;..O.....}.
-00000aa0: afd0 d234 a653 7d45 4dee d4aa 4810 bed3  ...4.S}EM...H...
-00000ab0: e03c 56d2 5611 fec1 cdcf 7a8a a1c6 4aae  .<V.V.....z...J.
-00000ac0: d9e3 7c59 ed8d 336a 287e 2359 7a58 1fff  ..|Y..3j(~#YzX..
-00000ad0: 205a 9ada 4860 08c5 9aee 7afc 3e2c c05a   Z..H`....z.>,.Z
-00000ae0: c5ad 30af 8c72 607c 3ebe 80e4 dcd0 2748  ..0..r`|>.....'H
-00000af0: 1508 22db 54f2 b9cd 45e7 51a4 2a26 8f2f  ..".T...E.Q.*&./
-00000b00: 91df 0fba c40f dc51 8f9c ba63 2f18 bac3  .......Q...c/...
-00000b10: dec4 77bd 200c 4723 6fdc 0dba c12b 38a3  ..w. .G#o....+8.
-00000b20: a238 95b4 36f9 4605 163a 4101 a4fc c074  .8..6.F..:A....t
-00000b30: 4957 ad85 7871 cdb3 1d8d 176f f3b8 b67f  IW..xq.....o....
-00000b40: d7b4 b657 ebb0 3def ee39 5bea 9d5e ecd4  ...W..=..9[..^..
-00000b50: 593d 7091 c965 e3d1 733b ee46 e0df b231  Y=p..e..s;.F...1
-00000b60: 3cf0 cce4 09f2 7b3d 6fbb f693 f179 0e6c  <.....{=o....y.l
-00000b70: 4927 b48b 5013 9655 82f6 d88c d76c cee0  I'..P..U.....l..
-00000b80: 716d b3c7 06bf a1d3 9caa 40ab e91d d154  qm........@....T
-00000b90: c28d 3d69 091c dfb6 6f02 0cca 8fed 37d4  ..=i....o.....7.
-00000ba0: 7946 9a04 b6af a5b4 4841 f9b6 6b36 4202  yF......HA..k6B.
-00000bb0: 4807 35f3 4b99 41aa 4a2a 6a0a 9565 77fc  H.5.K.A.J*j..ew.
-00000bc0: 166d fa20 246c 652e b469 7a50 2507 fe24  .m. $le..izP%..$
-00000bd0: f04e bb5e 3f70 bd49 2774 835e df77 7b41  .N.^?p.I't.^.w{A
-00000be0: c777 47c1 d89f 84dd c978 320c 6df2 ecb5  .wG......x2.m...
-00000bf0: 11ff 8fc3 b329 8eb8 bd8f ac1b 3955 e656  .....)......9U.V
-00000c00: d174 01b7 d835 9b0d a906 17d6 1e03 5f10  .t...5........_.
-00000c10: 6bcb 1ab7 6f0d fe02 0000 ffff 0300 504b  k...o.........PK
+00000920: e230 107d 5f69 ff21 f27b ea38 8400 5143  .0.}_i.!.{.8..QC
+00000930: 556e bb48 ed6e d5eb 6365 1243 2c12 3b6b  Un.H.n..ce.C,.;k
+00000940: 3b85 aaea bfef 3810 28e5 a5db 6e04 be8d  ;.....8.(...n...
+00000950: 7372 66e6 8c7d 7ab6 2e72 e789 29cd a588  srf..}z..r..)...
+00000960: 1139 f190 c344 2253 2e16 31ba bb9d b85d  .9...D"S..1....]
+00000970: e468 4345 4a73 2958 8c9e 9946 67fd efdf  .hCEJs)X...Fg...
+00000980: 4e57 522d 6752 2e1d 0010 3a46 9931 6584  NWR-gR....:F.1e.
+00000990: b14e 3256 507d 224b 26c0 3297 aaa0 06a6  .N2VP}"K&.2.....
+000009a0: 6a81 75a9 184d 75c6 9829 72ec 7b5e 880b  j.u..Mu..)r.{^..
+000009b0: ca05 da20 44ea 2318 723e e709 1bc9 a42a  ... D.#.r>.....*
+000009c0: 9830 1b10 c572 6a80 bece 78a9 1bb4 22f9  .0...rj...x...".
+000009d0: 085c 41d5 b22a dd44 1625 40cc 78ce cd73  .\A..*.D.%@.x..s
+000009e0: 0d8a 9c22 89a6 0b21 159d e5e0 f69a b49d  ..."...!........
+000009f0: b582 5f08 7fe2 41e3 375f 02d3 d1a7 0a9e  .._...A.7_......
+00000a00: 28a9 e5dc 9c00 34de 903e f29f 7898 9083  (.....4..>..x...
+00000a10: 10ac 8f63 f031 a400 2bf6 c46d 0e77 ac54  ...c.1..+..m.w.T
+00000a20: f849 56e1 0e2b dc83 11ef cb68 04a4 556b  .IV..+.....h..Uk
+00000a30: 2582 e07d 12ad bde3 e6a3 fee9 9ce7 ec7e  %..}...........~
+00000a40: 235d 8796 e52f 5ad8 4ce5 c8c9 a936 e394  #].../Z.L....6..
+00000a50: 1b96 c6a8 0353 b962 fb05 f04a 55e5 a0e2  .....S.b...JU...
+00000a60: 3958 89d7 223e c2fd 9d9c af94 93b2 39ad  9X..">........9.
+00000a70: 7273 0b42 6ee0 6163 18f6 fcb6 dd09 c238  rs.Bn.ac.......8
+00000a80: cf0d 5382 1a36 94c2 800e b77e 7d55 7335  ..S..6.....~}Us5
+00000a90: f630 93a0 70e7 9afd a9b8 6250 58a0 2ff0  .0..p.....bPX./.
+00000aa0: 155a 9a44 74a6 afa8 c99c 4ae5 31c2 771a  .Z.Dt.....J.1.w.
+00000ab0: 9cc7 4ada 2ac2 3fb8 f959 cd30 d458 c135  ..J.*.?..Y.0.X.5
+00000ac0: 7b5c acca 8371 4a0d c56f 244b 8feb e31f  {\...qJ..o$K....
+00000ad0: 444b 131b 090c a1d8 d0dd 8cdf 8705 58ab  DK............X.
+00000ae0: a811 e695 510e 8ca7 a30b 48ce 0d7d 8254  ....Q.....H..}.T
+00000af0: 8120 d26d 254f 6d2e 5a8f 2251 1179 7c99  . .m%Om.Z."Q.y|.
+00000b00: 0cc9 8010 3276 8349 77e2 8ebd 2070 07a4  ....2v.Iw... p..
+00000b10: d572 bdc9 30ec b547 0121 93f0 159c 5161  .r..0..G.!....Qa
+00000b20: 9448 5a99 6cab 020b 1da3 0052 7e64 baa4  .HZ.l......R~d..
+00000b30: ebc6 42bc a8e2 e99e c68b b77d 5cdb bf6b  ..B........}\..k
+00000b40: 1adb ab75 d89e 77f7 9cad f45e 2f76 eaac  ...u..w....^/v..
+00000b50: 1fb8 48e5 aaf6 e8b9 1977 42f0 6f55 1b1e  ..H......wB.oU..
+00000b60: 786a b218 f9dd aeb7 5bfb c9f8 2203 b6a4  xj......[..."...
+00000b70: d5b6 8b50 1396 558c 0ed8 8c36 6c26 f0b8  ...P..U....6l&..
+00000b80: b639 6083 dfd0 a94f 55a0 55f7 8ea8 2be1  .9`....OU.U...+.
+00000b90: c69e b404 8e6f dbd7 0106 e547 f61b 6a9a  .....o.....G..j.
+00000ba0: 923a 81cd 6b09 cd13 50be edea 8da1 df23  .:..k...P......#
+00000bb0: 2d54 cf2f 650a a92a a8a8 2854 96dd f15b  -T./e..*..(T...[
+00000bc0: 34e9 8390 b0b5 b9d0 a6ee 4195 1cf8 93c0  4.........A.....
+00000bd0: 3bef 78bd c0f5 c6ad b61b 747b bedb 0d5a  ;.x.......t{...Z
+00000be0: be3b 0c46 feb8 dd19 8fc6 83b6 4d9e bd36  .;.F........M..6
+00000bf0: a2ff 7178 d6c5 1135 f791 7523 a3ca dc2a  ..qx...5..u#...*
+00000c00: 9a2c e116 bb66 f301 d5e0 c2c6 63e0 0b62  .,...f......c..b
+00000c10: 6d58 e3e6 adfe 5f00 0000 ffff 0300 504b  mX...._.......PK
 00000c20: 0304 1400 0600 0800 0000 2100 2796 d6b5  ..........!.'...
 00000c30: ca02 0000 0a07 0000 0d00 0000 786c 2f73  ............xl/s
 00000c40: 7479 6c65 732e 786d 6cb4 55db 6edb 300c  tyles.xml.U.n.0.
 00000c50: 7d1f b07f 10f4 eeca 76e3 2c09 6c17 4b53  }.......v.,.l.KS
 00000c60: 0305 b661 403b 60af 8a2d 2742 7531 2425  ...a@;`..-'Bu1$%
 00000c70: 7336 ecdf 47d9 4ee2 a2dd adc3 5e62 8912  s6..G.N.....^b..
 00000c80: 0f0f 0f29 26bd 6aa5 407b 662c d72a c3d1  ...)&.j.@{f,.*..
@@ -356,474 +356,476 @@
 00001630: be5c d97c 71ef 1120 9dfb b5ca a059 6d76  .\.|q.. .....Ymv
 00001640: 6a85 66b5 3d28 04bd 4ea3 d0ec d63a 855e  j.f.=(..N....:.^
 00001650: ad5b ef0d 7add b0d1 1c3c f0bd 230d 0eda  .[..z....<..#...
 00001660: d56e 50eb 370a b572 b75b 086a 2565 7ea3  .nP.7..r.[.j%e~.
 00001670: 59a8 0795 4a3b a8b7 1bfd a0fd 202b 6360  Y...J;...... +c`
 00001680: e529 7d64 be00 f76a bbb6 ff01 0000 ffff  .)}d...j........
 00001690: 0300 504b 0304 1400 0600 0800 0000 2100  ..PK..........!.
-000016a0: 678c 4f02 8e11 0000 8b86 0000 1800 0000  g.O.............
+000016a0: 0b04 22b9 b011 0000 e087 0000 1800 0000  ..".............
 000016b0: 786c 2f77 6f72 6b73 6865 6574 732f 7368  xl/worksheets/sh
-000016c0: 6565 7431 2e78 6d6c 9c93 c96e db30 1086  eet1.xml...n.0..
-000016d0: ef05 fa0e 04ef 3625 d971 12c1 72d0 3a30  ......6%.q..r.:0
-000016e0: 1aa0 87a2 4b72 a6a8 9145 9814 5592 de50  ....Kr...E..U..P
-000016f0: f4dd 33a4 bc01 be18 1124 eefc fe7f c8d1  ..3......$......
-00001700: f469 a715 d980 75d2 b405 4d87 0925 d00a  .i....u...M..%..
-00001710: 53c9 7659 d03f bf17 8307 4a9c e76d c595  S.vY.?....J..m..
-00001720: 69a1 a07b 70f4 69f6 f9d3 746b ecca 3500  i..{p.i...tk..5.
-00001730: 9e20 a175 056d bcef 72c6 9c68 4073 3734  . .u.m..r..h@s74
-00001740: 1db4 3853 1bab b9c7 ae5d 32d7 59e0 55dc  ..8S.....]2.Y.U.
-00001750: a415 cb92 64c2 3497 2ded 09b9 bd85 61ea  ....d.4.-.....a.
-00001760: 5a0a 7836 62ad a1f5 3dc4 82e2 1efd bb46  Z.x6b...=......F
-00001770: 76ee 48d3 e216 9ce6 76b5 ee06 c2e8 0e11  v.H.....v.......
-00001780: a554 d2ef 2394 122d f297 656b 2c2f 15c6  .T..#..-..ek,/..
-00001790: bd4b c75c 909d c537 c36f 7494 89e3 574a  .K.\...7.ot...WJ
-000017a0: 5a0a 6b9c a9fd 10c9 acf7 7c1d fe23 7b64  Z.k.......|..#{d
-000017b0: 5c9c 48d7 f1df 8449 c7cc c246 860b 3ca3  \.H....I...F..<.
-000017c0: b28f 594a ef4e acec 0c1b 7d10 3639 c1c2  ..YJ.N....}.69..
-000017d0: 71d9 7c2d ab82 fe4b 0ecf 00eb 3414 c9b9  q.|-...K....4...
-000017e0: 38ce fda7 b369 25f1 8643 54c4 425d d02f  8....i%..CT.B]./
-000017f0: 693e cfb2 1165 b369 cca0 5709 5b77 d126  i>...e.i..W.[w.&
-00001800: 9e97 bf40 81f0 802a 2925 de74 dfa1 f673  ...@...*)%.t...s
-00001810: 502a ecbe c7cc 0e39 5b1a b30a 7b5f 7055  P*.....9[...{_pU
-00001820: 8232 2eee 0932 5c78 b981 7efd d7f4 0111  .2...2\x..~.....
-00001830: ee6f 948e 1dd4 6527 e1cb f6d1 c422 66fa  .o....e'....."f.
-00001840: 0f4b 4aee 606e d49b ac7c 834e 50b7 829a  .KJ.`n...|.NP...
-00001850: af95 bf18 44f8 61f0 a7d9 7e03 b96c 3c2e  ....D.a...~..l<.
-00001860: 9de0 3185 3ccb abfd 3338 8109 8e1e 8759  ..1.<...38.....Y
-00001870: 8859 1885 4258 122d c38f 8af9 c977 b1de  .Y..BX.-.....w..
-00001880: f63a e3f1 309d 8c93 4976 4749 09ce 2f64  .:..0...IvGI../d
-00001890: 2052 22d6 ce1b 7d34 7340 f510 bce2 08c1   R"...}4s@......
-000018a0: fa00 49ef 6f85 b068 e81d 0000 ffff 0000  ..I.o..h........
-000018b0: 00ff ff94 9ded 6edc 3812 455f 25c8 ff51  ......n.8.E_%..Q
-000018c0: 448a fa1a 640c ac9d 1731 b206 e6d7 ec62  D...d....1.....b
-000018d0: 6c64 77df 7e8b 6a76 8b97 4595 eb06 c860  ldw.~.jv..E....`
-000018e0: 9012 e313 3575 8a2d f655 7f7f fff3 eded  ....5u.-.U......
-000018f0: e3c7 ebc7 ebd3 f7bf fff5 9f2f 7fff f135  .........../...5
-00001900: 7cfd f2fe efd7 bfde e5ff 7e9f be7e f96f  |.........~..~.o
-00001910: 48af 3f7f ffe7 ff7e bcbd ff7c fbeb e38f  H.?....~...|....
-00001920: afe3 10bf 3e7d ff99 0ffd 473e f618 217f  ....>}....G>..!.
-00001930: fe2e 7ffa eb69 fcfe edd7 d3f7 6f3f cb11  .....i......o?..
-00001940: cffa 8880 47bc e823 e2e3 886f c2f4 008b  ....G..#...o....
-00001950: 0498 1cfb 409a 1aa4 ba36 37bc 2ff9 dff6  ....@....67./...
-00001960: ebe9 b713 1210 e47c b8cf 8d1c fb40 589a  .......|.....@X.
-00001970: 7ff4 735d 540c 93c9 9008 0639 f6c1 909a  ..s]T......9....
-00001980: d350 d7e6 f645 4907 c2c5 5998 0902 39f6  .P...EI...Y...9.
-00001990: 92a0 aecd e78b 7e4c ad97 d922 5808 0239  ......~L..."X..9
-000019a0: f692 a0ae cdcd 3c79 592c 8295 2090 632f  ......<yY,.. .c/
-000019b0: 09ea dadc bc44 2fab 45b0 1104 72ec 8360  .....D/.E...r..`
-000019c0: 6ee6 01d4 9ae2 cb66 11ec 0481 1c7b 4900  n......f.....{I.
-000019d0: b576 26ee 1641 1819 59c9 c197 0cf9 6f3a  .v&..A..Y.....o:
-000019e0: 8bed 6494 6ad6 c2c5 f510 2865 cac1 d714  ..d.j.....(e....
-000019f0: 506c 27a4 fc1c 8b82 f163 0009 b6ce 8662  Pl'......c.....b
-00001a00: 3b29 65a8 45c1 2832 8023 5b0a 70e4 d276  ;)e.E.(2.#[.p..v
-00001a10: 8d9b 24af 5e11 4692 a136 61f3 739e a138  ..$.^.F..6a.s..8
-00001a20: b797 8754 ad73 c188 32d4 3654 14a0 4ad5  ...T.s..2.6T..J.
-00001a30: 414d 5706 4696 f9e0 b36b b5af 08e8 525d  AMW.F....k....R]
-00001a40: 23a6 2f03 23cc 7cf0 3505 2853 5d23 a633  #./.#.|.5.(S]#.3
-00001a50: 0323 cd7c f035 0568 535d 23a6 3703 23ce  .#.|.5.hS]#.7.#.
-00001a60: 7cf0 8362 6d5f 1150 6753 7d91 a1d6 6226  |..bm_.PgS}...b&
-00001a70: 32f2 cc07 5f62 4071 de9a 4b55 aa26 0663  2..._b@q..KU.&.c
-00001a80: cf58 0bb2 3d1b 509c f716 e366 cfab a55d  .X..=.P....f...]
-00001a90: a496 97b5 2115 465d 5cd4 02d3 5e61 46c6  ....!.F]\...^aF.
-00001aa0: 9ff9 e0c7 8bd2 9cf6 6728 2a73 4935 bf28  ........g(*sI5.(
-00001ab0: 6918 9798 c6f3 d7d5 da9b 116a ac85 aab0  i..........j....
-00001ac0: cc75 a70c a5b0 18c3 c65a a20a cb5c 8cca  .u.......Z...\..
-00001ad0: 500a 8b51 6eac adaa b0cc 15aa 0ca5 b018  P..Qn...........
-00001ae0: 07c7 5ab3 0acb 5cb6 ca50 0a8b 9172 acbd  ..Z...\..P...r..
-00001af0: db5c e2cf 509c db25 8354 292c c6d2 b116  .\..P..%.T),....
-00001b00: b1c2 024b b76b 0819 ca60 4d8c b5f3 c10f  ...K.k...`M.....
-00001b10: 41b4 5850 54ef 00a5 4a61 3116 9f6a 8b2b  A.XPT...Ja1..j.+
-00001b20: 2c58 03b7 ab0c 194a 6131 569f 6a71 2b2c  ,X.....Ja1V.jq+,
-00001b30: 5814 b7cb 0e19 4a61 5137 126a cb2b 2c58  X.....JaQ7.j.+,X
-00001b40: 25b7 eb90 89b3 fcc4 583e 1ffc 985b a1bd  %.......X>...[..
-00001b50: ef03 55d5 7da4 9a4f 571c d21e aae6 335e  ..U.}..OW.....3^
-00001b60: dd76 6134 3fd5 26d7 5ce6 4a5a c652 5c8c  .va4?.&.\.JZ.R\.
-00001b70: e7a7 5ae5 9acb 5c5b cb58 8a8b 11fd 54bb  ..Z...\[.X....T.
-00001b80: 5c73 99ab 6d19 4b71 31a6 9f6a d36b 2e73  \s..m.Kq1..j.k.s
-00001b90: fd2d 6329 2e46 f553 6df3 a06e ec99 ae97  .-c).F.Sm..n....
-00001ba0: b199 2b2c 431a c336 6efb d9a3 e03e 6362  ..+,C..6n....>cb
-00001bb0: 249f 0f3e 2fc4 1608 aafa 3e5f b9b1 f129  $..>/.....>_...)
-00001bc0: 10a3 f754 1b5c 9d21 a8aa db7e 52f5 9d21  ...T.\.!...~R..!
-00001bd0: 46ec a976 b706 32cd 2e63 7d40 8cd2 536d  F..v..2..c}@..Sm
-00001be0: 6d0d 643a 5dc6 fa80 a81b c520 f3a6 e93e  m.d:]...... ...>
-00001bf0: 2758 b3b7 0b18 a91e 17db 9286 739d 88d3  'X..........s...
-00001c00: 99f1 7702 7f2b 14d3 df32 f633 1446 d909  ..w..+...2.3.F..
-00001c10: 94ad 504c 65cb d8cf 5018 4b27 b0b4 4231  ..PLe...P.K'..B1
-00001c20: 2d2d 633f 4361 c49c 40cc 0ac5 14b3 8cfd  --c?Ca..@.......
-00001c30: 0c85 7171 0217 b71b 3d50 556b 10a9 1ed7  ..qq....=PUk....
-00001c40: d134 8621 ae63 d8f7 7d96 dffb b9c2 8239  .4.!.c..}......9
-00001c50: 3c33 4ace 079f 4a6e b9a0 aa94 2c55 8a8b  <3J...Jn....,U..
-00001c60: 31f3 0c66 565c e6ca 5bc6 525c 8ca0 6710  1..fV\..[.R\..g.
-00001c70: b4e2 3205 2d63 292e c6d3 3378 5a71 999e  ..2.-c)...3xZq..
-00001c80: 96b1 1417 a3eb 1974 ddee ec41 55cd 7ba9  .......t...AU.{.
-00001c90: defa c738 8cfb b64c e3e5 8ca7 f6f9 c0da  ...8...L........
-00001ca0: 8ac8 b4f6 5cee 5f2f 9f12 31f2 9e41 de8a  ....\._/..1..A..
-00001cb0: c894 b78c 759e 23c6 e133 385c 1199 0e97  ....u.#..38\....
-00001cc0: b14e 2246 e533 a85c 1199 2a97 b14e 22c6  .N"F.3.\..*..N".
-00001cd0: e833 18bd ddab 84aa 9ed9 e54e ca36 a621  .3.........N.6.!
-00001ce0: 4dfb b8ca affe 4709 1646 e6f9 e053 e62d  M.....G..F...S.-
-00001cf0: 1254 95cc a59a 4f52 7220 311e 5fc0 e30a  .T....ORr 1._...
-00001d00: c9f4 b88c f522 310a 5f40 e10a c954 b88c  ....."1._@...T..
-00001d10: f522 31f6 5ec0 de0a c9b4 b78c f522 31e2  ."1.^........"1.
-00001d20: 5e40 dced 361f 54d5 f496 6a46 9ab7 380d  ^@..6.T...jF..8.
-00001d30: 6b5c c226 8b96 7cf3 e4e2 a6c9 c2e8 3b1f  k\.&..|.......;.
-00001d40: 7cce 71c5 65ea 5bc6 525c 8cc4 1790 b8e2  |.q.e.[.R\......
-00001d50: 3225 2e63 292e 46e5 0ba8 5c71 992a 97b1  2%.c).F...\q.*..
-00001d60: 1417 23f4 0584 aeb8 4ca1 cb58 8a8b d1fa  ..#.....L..X....
-00001d70: 025a 6f77 cca0 aae7 fd4d ebeb 1687 715a  .Zow.....M....qZ
-00001d80: e3bc 6fb7 75fa 7941 c342 7d65 dc9e 0f3e  ..o.u.yA.B}e...>
-00001d90: e77d cb05 55e5 76a9 e6f3 e5e6 6204 bf82  .}..U.v.....b...
-00001da0: e015 9729 7819 4b71 3196 5fc1 f28a cbb4  ...)x.Kq1._.....
-00001db0: bc8c a5b8 18d5 afa0 7ac5 65aa 5ec6 525c  ........z.e.^.R\
-00001dc0: 8cef 57f0 7dbb 8d06 5535 efa5 7a2c b0a6  ..W.}...U5..z,..
-00001dd0: 7598 9731 8ed3 7ebe 01c1 19cf 987e 05d3  u..1..~......~..
-00001de0: 2b22 d3f4 32d6 49c4 387e 05c7 2b22 d3f1  +"..2.I.8~..+"..
-00001df0: 32d6 49c4 d87d 05bb 2b22 d3ee 32d6 49c4  2.I..}..+"..2.I.
-00001e00: 787d 05af 2b22 d3eb 32d6 49c4 187d 05a3  x}..+"..2.I..}..
-00001e10: b7db 5250 d533 fb66 f471 d8f6 2d2e 312c  ..RP.3.f.q..-.1,
-00001e20: c77d 17f9 cfc5 727d 6394 9e0f 3e95 de82  .}....r}c...>...
-00001e30: 4155 295d aaf9 54f9 c118 a76f e074 0566  AU)]..T....o.t.f
-00001e40: 3a5d c672 608c d437 90ba 0233 a52e 6339  :].r`..7...3..c9
-00001e50: 30c6 ea1b 585d 8199 5697 b11c 18a3 f5ad  0...X]..V.......
-00001e60: d67a 6cf7 3ea1 aa26 bf54 3398 2c62 e210  .zl.>..&.T3.,b..
-00001e70: 45eb 5b4a 5b9e ff17 f7ce 3746 eef9 e0c7  E.[J[.....7F....
-00001e80: dcd7 5ca6 dc65 2cc5 c528 7eab 25ae b94c  ..\..e,..(~.%..L
-00001e90: c5cb 588a 8b11 fd56 ab5c 7399 a297 b114  ..X....V.\s.....
-00001ea0: 17a3 fbad 16ba e632 752f 6329 2e46 fa5b  .......2u/c).F.[
-00001eb0: 2dfd d86e 3542 55cf fb72 bf5d 942f ebf8  -..n5BU..r.]./..
-00001ec0: 392d 71b1 eeb7 ef8c f3f3 c1e7 bc6f b9a0  9-q..........o..
-00001ed0: aa9c 2fd5 a33d 7ab9 18e5 efb5 d4d5 f982  ../..=z.........
-00001ee0: aada 0995 2ac5 c518 7faf 9dae b94c e3cb  ....*........L..
-00001ef0: 588a 8b11 fe5e 2b5d 7399 c297 b114 17e3  X....^+]s.......
-00001f00: fb1d 7cdf 6e79 4155 cd7b a966 ae75 1fa6  ..|.nyAU.{.f.u..
-00001f10: 650d ebb2 a6b2 dae9 df9a dc19 dfe7 83cf  e...............
-00001f20: 79af b84c dfcb 588a 8bf1 fd0e be57 5ca6  y..L..X......W\.
-00001f30: ef65 2cc5 c5f8 7e07 df2b 2ed3 f732 96e2  .e,...~..+...2..
-00001f40: 627c bf83 ef15 97e9 7b19 4b71 31be dfc1  b|......{.Kq1...
-00001f50: f7ed fe17 54f5 bcbf f97e 8ecb 3027 b913  ....T....~..0'..
-00001f60: bf94 8f7a 9dbb 0cf0 2656 6e65 5259 1e30  ...z....&VneRY.0
-00001f70: 7e4b 76fc 658f 0b43 293f 97f3 39f3 b331  ~Kv.e..C)?..9..1
-00001f80: d20f 2358 5fb3 992b fd3c 9a63 63c4 1f46  ..#X_..+.<.cc..F
-00001f90: 30bf 6633 d59f 4773 6c8c fcc3 08f6 d76c  0.f3..Gsl......l
-00001fa0: a6fe f368 8e8d 6900 6184 0ed0 ee94 6159  ...h..i.a.....aY
-00001fb0: c784 64f4 718d 2ecb 2c5d 204c 61a9 3e9d  ..d.q...,] La.>.
-00001fc0: dc5c 068c ffc3 080d 4063 991d 208f 7663  .\......@c.. .vc
-00001fd0: 31fa 0f23 f85f 6399 0d20 8f76 6331 f60f  1..#._c.. .vc1..
-00001fe0: 23e8 5f63 99fe cfa3 dd58 8cfc c308 f6d7  #._c.....X......
-00001ff0: 58a6 fef3 6837 16e3 fe30 82fc dbed 332c  X...h7...0....3,
-00002000: 77a6 7c59 ee87 20db 5569 9f76 f980 cd45  w.|Y.. .Ui.v...E
-00002010: b824 7031 4e88 6a46 c585 494e 9595 bb47  .$p1N.jF..IN...G
-00002020: 395d 5c94 f673 0cf4 5c8c 692e 5bfb f770  9]\..s..\.i.[..p
-00002030: a78b 8b52 3e64 3d3b e7cb 56fe 3dee e9e2  ...R>d=;..V.=...
-00002040: a274 0fe9 cf0e 97ad 7b19 7d2c f75d 5c94  .t......{.},.]\.
-00002050: ea21 f219 5514 f393 4468 8984 8ae2 f721  .!..U...Dh.....!
-00002060: ceb3 2cf8 6334 7669 43ce 7dfa 9fb7 0029  ..,.c4viC.}....)
-00002070: d10e 9bed 7b19 9dcf 999f 8d92 3e64 473b  ....{.......>dG;
-00002080: 6cb6 f465 34c7 4699 1f12 a51d 36db fc32  l..e4.F.....6..2
-00002090: 9a63 a3f4 0f39 d30e 9bad 7f19 cdb1 513d  .c...9........Q=
-000020a0: 00d2 a74b fbc6 2440 59f7 8012 40ad 3ee0  ...K..$@Y...@.>.
-000020b0: 8c6b 1d2a 811a 2065 aa59 3084 aabc 5f52  .k.*.. e.Y0..._R
-000020c0: a8d7 2c94 eb21 6ada 61b1 5d2f a36f eeea  ..,..!j.a.]/.o..
-000020d0: df02 0854 16f5 38fa d177 3a2c b6df e567  ...T..8..w:,...g
-000020e0: d92c 94d3 2174 da61 b19d 5e42 a9d7 af11  .,..!t.a..^B....
-000020f0: e571 88a1 4615 9d86 b27a f446 2849 d4b8  .q..F....z.F(I..
-00002100: 0f17 9b52 21e7 49fd e686 f469 6c77 f08e  ...R!.I....ilw..
-00002110: bfec 7cc3 aa9e 3350 02a8 7190 1ba7 72eb  ..|...3P..q...r.
-00002120: 74be 87a6 ae9e 7f90 43a5 041b 2cd7 351b  t.......C...,.5.
-00002130: 985b 5f59 f770 9297 8d32 37e4 503b e70d  .[_Y.p...27.P;..
-00002140: ccad 9e49 50a2 a8fe f346 991b f2a6 1d36  ...IP....F.....6
-00002150: 30b7 7a52 41c9 a3fa d928 7343 22b5 c356  0.zRA....(sC"..V
-00002160: 2fee 3bb3 ffb6 7a77 b351 a9d4 00c9 d3d8  /.;...zw.Q......
-00002170: eeeb 6159 7795 924c 0d6b 92d4 d216 f6fc  ..aYw..L.k......
-00002180: 39b8 0b91 e6a0 a9ff 3280 586a 070b a4ae  9.......2.Xj....
-00002190: 2e83 924c 7561 51eb 7788 a576 b0c0 efea  ...LuaQ.w..v....
-000021a0: 0a28 c954 1716 a57a c996 566f 77f4 8b08  .(.T...z..Vow...
-000021b0: aa57 93bf 2453 5d58 94f5 2178 da39 5b10  .W..$S]X..!x.9[.
-000021c0: 6552 cfed 28c1 5417 16a5 7f48 a54e ea29  eR..(.T....H.N.)
-000021d0: 6950 ee4c f9db c27d 897b 18e4 3ff3 3aef  iP.L...}.{..?.:.
-000021e0: b75d 84ab 794f e91f 92a9 1d36 5bff 259b  .]..yO.....6[.%.
-000021f0: ea67 a3f4 0fe9 d40e 9bad ff92 4ff5 b351  .g..........O..Q
-00002200: fa87 846a 87cd d67f c9a8 fad9 28fd 434a  ...j........(.CJ
-00002210: b5c3 66eb bfe4 54dd 6c54 5e35 4024 756a  ..f...T.lT^5@$uj
-00002220: 776b b1ac af05 197d 2c58 57c9 1be6 6b61  wk.....},XW...ka
-00002230: dc36 eb63 d021 e74d fd3d 00d2 a91d 36bb  .6.c.!.M.=....6.
-00002240: 07dc d3ab 6e36 aa11 408c b5c3 6637 827b  ....n6..@...f7.{
-00002250: 90d5 cd46 7503 48b4 76d8 ec6e 70cf b4ba  ...Fu.H.v..np...
-00002260: d9a8 9600 f1d5 0e9b dd12 4abc 556e e438  ..........J.Un.8
-00002270: e71b d517 20ed 3aa9 37d8 50ee 5c0b f70f  .... .:.7.P.\...
-00002280: 646e fb24 6f0d e222 8980 abfd b51c 6625  dn.$o.."......f%
-00002290: ae83 5afa 1d2e bb27 94f0 6b98 3c5c 543f  ..Z....'..k.<\T?
-000022a0: 801c 6c87 cbee 0725 09eb e3a2 7a01 8462  ..l....%....z..b
-000022b0: 3b5c 762f 28b1 581f 17d5 0720 03db e1b2  ;\v/(.X.... ....
-000022c0: fbc0 2323 eb78 1da9 806c 800c eca4 f6fa  ..##.x...l......
-000022d0: 3022 abde 0e97 8cec 36ec 610e 7bba 7d8e  0"......6.a.{.}.
-000022e0: 2807 782f d643 39f7 ea9f fb90 92ed b0d9  (.x/.C9.........
-000022f0: 3da0 e464 fd6c 540f 80a4 6c87 cdee 0125  =..d.lT...l....%
-00002300: 2beb 67a3 7a00 a465 3b6c 760f 2879 593f  +.g.z..e;lv.(yY?
-00002310: 1bd5 0320 13db 61b3 7b40 c9cc fad9 a81e  ... ..a.{@......
-00002320: 20f9 d7f3 9dd4 a4f6 ffa0 ac7b c03d 3d3b   ..........{.==;
-00002330: c649 761c a67c 3184 f53a c71e 722e 96b8  .Iv..|1..:..r...
-00002340: 16a0 0f68 36bb 0fdc 73b4 6e36 aa17 409e  ...h6...s.n6..@.
-00002350: b673 deec 5e70 4fd4 bad9 a87e 00c9 da0e  .s..^pO....~....
-00002360: 9bdd 0fee d95a 371b d513 2045 db61 b37b  .....Z7... E.a.{
-00002370: 828c 3ed6 df5e 362a 6b1b 204e 3ba9 4d54  ..>..^6*k. N;.MT
-00002380: 4cdb aabe 50e2 b621 adc3 22fb 6e69 9687  L...P..!..".ni..
-00002390: ec58 9b6f 3947 ebbf 1620 75db 61b3 fb42  .X.o9G... u.a..B
-000023a0: c9dd fad9 a8be 00f1 db0e 9bdd 174a 00d7  .............J..
-000023b0: cf46 f505 c8e1 76d8 ecbe 5092 b87e 36aa  .F....v...P..~6.
-000023c0: 2f40 e4b6 c366 f785 12c9 f5b3 517d 0142  /@...f......Q}.B
-000023d0: b993 da88 86b2 ee0b 2596 bbac cbb0 4914  ........%.....I.
-000023e0: 7e4b d543 e871 1b2e 876c 89ab 003a 82a6  ~K.C.q...l...:..
-000023f0: b23b 4209 e57a a8a8 5e00 81dc ceb9 b27b  .;B..z..^......{
-00002400: 4189 e47a a8a8 2e00 71dc 0e95 dd05 4a20  A..z....q.....J 
-00002410: d743 45f9 1fe2 b61d 2adb ff32 3afb df41  .CE.....*..2:..A
-00002420: 4525 7103 846d 27b5 5d87 595c 65fe 12c6  E%q..m'.].Y\e...
-00002430: 35b6 eb72 a4d6 3fcb 2180 dba1 b15d 5f22  5..r..?.!....]_"
-00002440: b816 0d65 7788 dd76 686c bb97 e0ad 4543  ...ew..vhl....EC
-00002450: f91c c2b6 1d1a dbe7 256e 6bd1 5006 8710  ........%nk.P...
-00002460: 6d87 c636 7809 d95a 3494 b321 5e3b a9ad  m..6x..Z4..!^;..
-00002470: 5428 ab27 d486 12b0 b568 2857 43b4 b643  T(.'.....h(WC..C
-00002480: 03ae d6d7 54d9 d8bd de02 cf41 59e2 9aaa  ....T......AY...
-00002490: 25dc a101 47ab fdb5 12ac b5ce 0de5 6688  %...G.........f.
-000024a0: d476 68c0 cd6a 5bad 846a 2d1a cac9 1098  .vh..j[..j-.....
-000024b0: edd0 8093 f543 efcb 76ed f52b 4545 6865  .....C..v..+EEhe
-000024c0: d55c bf23 55b3 1843 b46a 13ad a468 8d73  .\.#U..C.j...h.s
-000024d0: 93a3 b0fe 7903 c1d9 49ed 3442 59af 834a  ....y...I.4BY..J
-000024e0: 7436 c421 6c53 8c72 1bf7 e226 518e c112  t6.!lS.r...&Q...
-000024f0: 50b5 733b 50a0 6435 994b 6cd6 0145 9919  P.s;P.d5.Kl..E..
-00002500: 02b3 1d28 30b3 9ad3 2532 eb80 a204 0d71  ...(0...%2.....q
-00002510: d80e 1408 5a4d ed12 9775 4051 9e86 a46c  ....ZM...u@Q...l
-00002520: 070a 3e48 a967 78b9 effe f99c a274 0d31  ..>H.gx......t.1
-00002530: d9a4 3689 a1dc 99e8 9fea 3ac7 5d89 195e  ..6.......:.]..^
-00002540: fbb8 4363 ebba c463 2d09 50ba 8648 6c87  ..Cc...c-.P..Hl.
-00002550: c6d6 7509 c55a 3494 ae21 eada a1b1 752d  ..u..Z4..!....u-
-00002560: a3f3 12da a0a1 d2af 0102 ae9a 06f3 af6a  ...............j
-00002570: 3297 00ac 4543 e91a 62ad 496d ef62 ea55  2...EC..b.Im.b.U
-00002580: 2d3a eeb1 d735 6e43 5ac7 650b d547 62f1  -:...5nCZ.e..Gb.
-00002590: 7d6b 4eb1 faa7 3364 5e3b 58b6 b0ef a957  }kN...3d^;X....W
-000025a0: 0f16 a56c 88bc 76b0 6c65 df43 af1e 2c4a  ...l..v.le.C..,J
-000025b0: da90 69ed 60d9 d22e 99d7 e0c1 a2b4 0d81  ..i.`...........
-000025c0: d70e 96ad ed12 7975 6151 e286 bc6b 52bb  ......yuaQ...kR.
-000025d0: b850 d6e2 2e89 57b9 6339 0fab 3c29 30ca  .P....W.c9..<)0.
-000025e0: ed1a ebae 654e b112 f31e 34ae d96c 8d97  ....eN....4..l..
-000025f0: d4ab 9f8d 923a e45e 3be7 cd96 7a49 befa  .....:.^;...zI..
-00002600: d928 c543 bab5 c366 2b5e 461f 7749 9caf  .(.C...f+^F.wI..
-00002610: a944 4488 d7f4 38fa f169 61c5 8665 f5e1  .DD...8..ia..e..
-00002620: ce5c e6d8 18fd 4748 bfa6 7667 17cb ea5a  .\....GH..vg...Z
-00002630: c8e5 cc96 e445 1df6 491e 0c94 a6e3 16fe  .....E..I.......
-00002640: 4574 4c1e a042 9db7 5af2 1d36 b307 e49f  EtL..B..Z..6....
-00002650: c5b1 318d 409e ef55 bde7 eab0 998d 208f  ..1.@..U...... .
-00002660: e6d8 986e 1021 fdda 6133 bb41 1ecd b131  ...n.!..a3.A...1
-00002670: 2d21 4204 b6c3 66b6 843c 9a63 63fa 4284  -!B...f..<.cc.B.
-00002680: 1c6c 6a77 4fb1 dcb9 16ca c3cd 6463 57f6  .ljwO.......dcW.
-00002690: b3c6 492e 8574 1146 9096 415d 07d0 1334  ..I..t.F..A]...4
-000026a0: 97d9 13f2 cf3a 7600 5d5c 4c3f 9087 21d5  .....:v.]\L?..!.
-000026b0: d780 e632 fb41 1eed e762 7a41 8428 6ce7  ...2.A...bzA.(l.
-000026c0: 7534 7b41 1eed e6a2 a2b0 11b2 ae9a 0ba3  u4{A............
-000026d0: b0ed c23f 8ff6 7351 3d00 a2b0 a9dd c58d  ...?..sQ=.......
-000026e0: 5056 dfbb 9bcb 99eb b720 cf61 ebdf ab89  PV....... .a....
-000026f0: 39d3 ea5e 021d 479f edb2 ddb2 c2b2 be0c  9..^..G.........
-00002700: ef09 d865 9448 a73c a36e 99e4 cb5b aeb8  ...e.H.<.n...[..
-00002710: 28e5 4302 3669 2e50 7e7b 0f29 de13 b02e  (.C.6i.P~{.)....
-00002720: 2e4a f710 71ed 7081 eedb db48 f1fe a5a8  .J..q.p....H....
-00002730: 2e2e 4af5 907e ed70 81ea db3b 49b1 a45f  ..J..~.p...;I.._
-00002740: e523 068e d791 d23c 245f 3b5c 709b 5d5f  .#.....<$_;\p.]_
-00002750: 868f 87cd 3bb8 28cd 43ea b56a 1dc7 376c  ....;.(.C..j..7l
-00002760: 3f47 2877 2ec3 fb03 ce24 67b3 8e69 9ee4  ?G(w.....$g..i..
-00002770: 77fe 5cd1 550b a2be 5c35 42ea 35a9 2f18  w.\.U...\5B.5./.
-00002780: 8472 e79a 2cdf 2332 cda3 6c6f e7ef ee98  .r..,.#2..lo....
-00002790: c201 7775 5d52 ba87 586b 870d 74af afcb  ..wu]R..Xk..t...
-000027a0: 7277 c7cb c67d 0f2b c45c 351b a660 d5b5  rw...}.+.\5..`..
-000027b0: 5952 b0d1 cd46 691f 52b1 1d36 d834 55d7  YR...Fi.R..6.4U.
-000027c0: 6749 c5fa d9a8 1e90 33b5 670f 50f3 0dca  gI......3.g.P...
-000027d0: fa2d 5349 c9fa d9a8 3e00 a9d9 a4be 3e12  .-SI....>.....>.
-000027e0: bfc9 559f b7fb 97fc b59f 7efd f6fe e7db  ..U.......~.....
-000027f0: dbc7 8fd7 8fd7 a7ff 0300 00ff ff00 0000  ................
-00002800: ffff b229 484c 4ff5 4d2c 4acf cc2b 56c8  ...)HLO.M,J..+V.
-00002810: 494d 2bb1 5532 d033 5752 28ca 4ccf 80b1  IM+.U2.3WR(.L...
-00002820: 4bf2 0bc0 a2a6 4a0a 49f9 2525 f9b9 305e  K.....J.I.%%..0^
-00002830: 466a 624a 6a11 8867 aca4 9096 9f5f 02e3  FjbJj..g....._..
-00002840: e8db d9e8 97e7 1765 1767 a4a6 96d8 0100  .......e.g......
-00002850: 0000 ffff 0300 504b 0304 1400 0600 0800  ......PK........
-00002860: 0000 2100 91d7 54d3 4403 0000 720b 0000  ..!...T.D...r...
-00002870: 1400 0000 786c 2f73 6861 7265 6453 7472  ....xl/sharedStr
-00002880: 696e 6773 2e78 6d6c 9456 4d73 9b30 10bd  ings.xml.VMs.0..
-00002890: 77a6 ff41 c3b5 100c 76d2 8ec7 760e 6e33  w..A....v...v.n3
-000028a0: b9f4 63d2 8fbb 0c6b d004 242a 8934 fef7  ..c....k..$*.4..
-000028b0: 5d09 07b0 3038 194e 48bb 6fdf ae56 abb7  ]...08.NH.o..V..
-000028c0: ba7d 2e0b f204 5231 c1d7 5e74 35f3 08f0  .}....R1..^t5...
-000028d0: 44a4 8c67 6bef f7af bbe0 9347 94a6 3ca5  D..gk......G..<.
-000028e0: 85e0 b0f6 0ea0 bcdb cdfb 772b a534 415f  ..........w+.4A_
-000028f0: aed6 5eae 75b5 0c43 95e4 5052 7525 2ae0  ..^.u..C..PRu%*.
-00002900: b8b3 17b2 a41a 7f65 16aa 4a02 4d55 0ea0  .......e..J.MU..
-00002910: cb22 8c67 b39b b0a4 8c7b 2411 35d7 6b6f  .".g.....{$.5.ko
-00002920: b1f8 e891 9ab3 bf35 6c9b 959b b9b7 5929  .......5l.....Y)
-00002930: b659 e90d a725 ac42 bd59 85e6 bf59 4ba8  .Y...%.B.Y...YK.
-00002940: 864c 4806 cadd a1a5 0170 57b7 54ee 0427  .LH......pW.T..'
-00002950: 2913 cf2c 059f 304e 2893 97ac b8e0 c15e  )..,..0N(......^
-00002960: 28c5 8a4b 96af b492 a224 4ab0 8208 4976  (..K.....$J...Iv
-00002970: 4c60 b514 5657 248f 97f0 b578 935f 29f8  L`..VW$....x._).
-00002980: 31d1 4962 3db3 b732 eb5c 278a 9417 420a  1.Ib=..2.\'...B.
-00002990: d307 6e7a 9f19 675a 8a0c 3879 0172 4dbe  ..nz..gZ..8y.rM.
-000029a0: e89c 723c a9c8 375f 1c68 d092 ee8b 1a11  ..r<..7_.h......
-000029b0: 039f dcdf 6d83 68be a093 5e81 962c b11c  ....m.h...^..,..
-000029c0: 8cc7 d6b8 2c66 173d 4e63 2ce6 9331 9057  ....,f.=Nc,..1.W
-000029d0: 1b03 591a 9e92 b508 3664 349f 0819 a42f  ..Y.....6d4..../
-000029e0: 0ca3 a00b dc50 8d76 d38e a744 afe3 09a2  .....P.v...D....
-000029f0: 7117 671c b367 644b 3e28 7a93 ce62 1421  q.g..gdK>(z..b.!
-00002a00: 3816 1bbd 319e 9b4e 3c9a 8e29 5b57 0773  8...1..N<..)[W.s
-00002a10: de27 556c 4e2e 1e2d 63dc 8b7b ae55 2ced  .'UlN..-c..{.U,.
-00002a20: 7894 7643 1a67 96ee daab c9f4 7a2c d31c  x.vC.g......z,..
-00002a30: 9e9d 568c 6ec6 6c4f 816d dfc6 03e0 af60  ..V.n.lO.m.....`
-00002a40: bbdd c538 2efb 6487 d7d3 b6bd 99c2 249a  ...8..d.......$.
-00002a50: cda2 69d3 26a7 fe19 348e 7174 c1b1 dfbd  ..i.&...4.qt....
-00002a60: f78d cf7c 22d8 308e a95c 1c8f b26b 1c06  ...|".0..\...k..
-00002a70: 7764 70b6 6de6 6d5f 981b bc0d e683 fb3b  wdp.m.m_.......;
-00002a80: b0ec 65dd 9cfc 2899 17ec d34e 8dc7 4bd4  ..e...(....N..K.
-00002a90: 2f28 e639 1fcf f3fc d86d b9ee 5f3d 6e5b  /(.9.....m.._=n[
-00002aa0: 1733 27db 61f6 100c 0759 6b39 3e90 5b13  .3'.a....Yk9>.[.
-00002ab0: 3b4c 7b68 d178 594f e7ee 038e d0d1 7ab6  ;L{h.xYO......z.
-00002ac0: a3d0 1980 530e 2743 6c78 c7bf e133 c112  ....S.'Clx...3..
-00002ad0: 621f 3317 c6ec d927 c462 e0b3 ee1a fc00  b.3....'.b......
-00002ae0: d9c0 db3b c807 fb3f eb62 5f4b d2de e633  ...;...?.b_K...3
-00002af0: 107f be6f 7df2 240a aa59 01f8 6a67 9423  ...o}.$..Y..jg.#
-00002b00: 9d44 9415 aa8c 54f9 285a 5405 09db 3348  .D....T.(ZT...3H
-00002b10: 719b 658c bb2c 38d5 b5a4 0591 a044 2d13  q.e..,8......D-.
-00002b20: 582e cf8b 0fd4 23cb 6521 fe81 4449 20a9  X.....#.e!..DI .
-00002b30: 16aa ca41 02f9 40ea aac2 454c b63a aeb9  ...A..@...EL.:..
-00002b40: 21ac ab39 f65a eea8 5536 4660 d826 cb59  !..9.Z..U6F`.&.Y
-00002b50: 961b 0197 3c0e 9592 09d8 e37f 16b5 434c  ....<.........CL
-00002b60: 0aa1 80a0 10c9 a4c9 fdac 35d2 2795 a86a  ..........5.'..j
-00002b70: 532f 23b7 802b a60f 3ec1 a995 e10b 3e14  S/#..+..>.....>.
-00002b80: 0296 39e3 a910 0331 6674 d272 4933 3cff  ..9....1ft.rI3<.
-00002b90: bab0 2574 4336 16a8 2f00 0b76 38bf 8bd8  ..%tC6../..v8...
-00002ba0: 35ee 323a 9070 8df7 44fe ae66 ecee 95df  5.2:.p..D..f....
-00002bb0: 1e26 b682 9490 986c ddf8 f787 d4b6 67b7  .&.....l......g.
-00002bc0: 1ea2 66de fc07 0000 ffff 0300 504b 0304  ..f.........PK..
-00002bd0: 1400 0600 0800 0000 2100 5333 c060 5a01  ........!.S3.`Z.
-00002be0: 0000 7102 0000 1100 0801 646f 6350 726f  ..q.......docPro
-00002bf0: 7073 2f63 6f72 652e 786d 6c20 a204 0128  ps/core.xml ...(
-00002c00: a000 0100 0000 0000 0000 0000 0000 0000  ................
-00002c10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002c20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000016c0: 6565 7431 2e78 6d6c 9c93 cb8e db20 1486  eet1.xml..... ..
+000016d0: f795 fa0e 887d 82ed 64dc 192b cea8 cd28  .....}..d..+...(
+000016e0: ea48 5d54 bdae 313e 8e51 c0b8 406e aafa  .H]T..1>.Q..@n..
+000016f0: ee3d e0dc a46c a2b1 6cc0 5cbe ff3f 7098  .=...l..l.\..?p.
+00001700: 3def b522 5bb0 4e9a aea4 e938 a104 3a61  =.."[.N....8..:a
+00001710: 6ad9 ad4a faf3 c772 f448 89f3 bcab b932  j..J...r.H.....2
+00001720: 1d94 f400 8e3e cfdf bf9b ed8c 5dbb 16c0  .....>......]...
+00001730: 1324 74ae a4ad f77d c198 132d 68ee c6a6  .$t....}...-h...
+00001740: 870e 471a 6335 f7f8 6b57 ccf5 1678 1d17  ..G.c5..kW...x..
+00001750: 69c5 b224 c999 e6b2 a303 a1b0 f730 4cd3  i..$.........0L.
+00001760: 4801 2f46 6c34 747e 8058 50dc a37f d7ca  H./Fl4t~.XP.....
+00001770: de9d 685a dc83 d3dc ae37 fd48 18dd 23a2  ..hZ.....7.H..#.
+00001780: 924a fa43 8452 a245 f1ba ea8c e595 c2b8  .J.C.R.E........
+00001790: f7e9 940b b2b7 f866 f84d 4e32 b1ff 4649  .......f.MN2..FI
+000017a0: 4b61 8d33 8d1f 2399 0d9e 6fc3 7f62 4f8c  Ka.3..#...o..bO.
+000017b0: 8b33 e936 febb 30e9 9459 d8ca 7080 1754  .3.6..0..Y..p..T
+000017c0: f636 4be9 c399 955d 6093 37c2 f233 2c6c  .6K....]`.7..3,l
+000017d0: 972d 36b2 2ee9 dfe4 f88c b04e 4391 5c8a  .-6........NC.\.
+000017e0: d3d8 3f3a 9fd5 124f 3844 452c 3425 fd98  ..?:...O8DE,4%..
+000017f0: 168b 2c9b 5036 9fc5 0cfa 2561 e7ae dac4  ..,.P6....%a....
+00001800: f3ea 3b28 101e 5025 a5c4 9bfe 0b34 7e01  ..;(..P%.....4~.
+00001810: 4a85 d579 4e49 c8d9 ca98 7558 fb8a b312  J..yNI....uX....
+00001820: 9471 714d 90e1 c2cb 2d0c f33f a58f b801  .qqM....-..?....
+00001830: ee4f 948e 3fa8 cbce c2d7 ed93 8965 ccf4  .O..?........e..
+00001840: af96 54dc c1c2 a8df b2f6 2d3a c11b 5543  ..T.......-:..UC
+00001850: c337 ca5f 75a2 bf63 e737 b3fb 0c72 d57a  .7._u..c.7...r.z
+00001860: 9c8a 1663 3e15 f5e1 059c c004 478f e32c  ...c>.......G..,
+00001870: c42c 8c42 212c 8996 e1a2 627e f27d ac77  .,.B!,....b~.}.w
+00001880: 83ce 743a 4ef3 6992 670f 9454 e0fc 5206  ..t:N.i.g..T..R.
+00001890: 2225 62e3 bcd1 2733 47d4 00c1 0823 04eb  "%b...'3G....#..
+000018a0: 2324 fd70 2f84 4543 ff01 0000 ffff 0000  #$.p/.EC........
+000018b0: 00ff ff94 9ddd 8e1c b711 855f 45d0 7d5a  ..........._E.}Z
+000018c0: cd9f fe33 e405 b2ab 1759 2802 7ce5 045e  ...3.....Y(.|..^
+000018d0: 414e de3e c519 ee34 0f8b 5d5b 4717 41e0  AN.>...4..][G.A.
+000018e0: 6259 9f7b c873 38cd 3e3d 5fdf fef8 f1e3  bY.{.s8.>=_.....
+000018f0: e7b7 d79f af4f 5fff faf7 df9f fefa fd73  .....O_........s
+00001900: f8fc e9ed 3faf 7fbe c9ff fb2d 7dfe f4df  ....?......-}...
+00001910: 905f bfff f6af ff7d fbf1 f6fd c79f 3f7f  ._.....}......?.
+00001920: ff3c 4ff1 f3d3 d7ef 65e8 3fcb d85b 87fc  .<O.....e.?..[..
+00001930: f337 f9a7 bf9e e6af 5f7e 3d7d fdf2 bd8e  .7......_~=}....
+00001940: 78d6 2302 8e78 d123 e263 c417 617a 8045  x.#..x.#.c..az.E
+00001950: 024c c63e 9052 87d4 d696 8ef7 a5fc b7fd  .L.>.R..........
+00001960: 7afa c709 0908 723d dcd7 46c6 3e10 d6ee  z.....r=..F.>...
+00001970: 3ffa b92d 2a86 6432 6482 41c6 3e18 7277  ?..-*.d2d.A.>.rw
+00001980: 19da dad2 7f28 f986 7071 1516 8240 c65e  .....(..pq...@.^
+00001990: 12b4 b5e5 fcd0 6f53 eb65 b108 5682 40c6  ......oS.e..V.@.
+000019a0: 5e12 b4b5 a59b 272f ab45 b011 0432 f692  ^.....'/.E...2..
+000019b0: a0ad 2ddd 47f4 b259 043b 4120 631f 044b  ..-.G..Y.;A c..K
+000019c0: 370f a0d6 155f 768b e020 0864 ec25 01d4  7...._v.. .d.%..
+000019d0: fa99 7858 0461 66c4 4a06 5f32 947f d359  ..xX.af.J._2...Y
+000019e0: ec27 a354 8b2c 5cac 8740 49a6 0cbe a680  .'.T.,\..@I.....
+000019f0: 623f 21e5 efb1 2818 7d0c 2082 bd66 43b1  b?!...(.}. ..fC.
+00001a00: 9f94 d26a 5130 1219 4023 7b0a d0c8 b577  ...jQ0..@#{....w
+00001a10: 8dbb 485e 7d22 8c48 8656 09bb bfe7 198a  ..H^}".H.V......
+00001a20: 4bbf 3ca4 6a5d 0b46 2843 ab86 8a02 a452  K.<.j].F(C.....R
+00001a30: 39a8 a995 8111 cb32 f874 adfe 1301 b954  9......2.t.....T
+00001a40: 6bc4 d4cb c008 6619 7c4d 0192 a9d6 88a9  k.....f.|M......
+00001a50: 9981 11cd 32f8 9a02 6453 ad11 5337 0323  ....2...dS..S7.#
+00001a60: 9c65 f083 62eb 3f11 90ce aefa 22ad d666  .e..b.?....."..f
+00001a70: 2632 e259 065f 6240 71d9 bba5 2a55 1383  &2.Y._b@q...*U..
+00001a80: 51cf d80a 647f 35a0 b81c 3dc6 5d3d afb6  Q...d.5...=.]=..
+00001a90: 7691 da5e b60a a930 dae2 aa36 98f6 0e33  v..^...0...6...3
+00001aa0: 32fa 5906 3f3e 94ee b23f 4351 2997 54cb  2.Y.?>...?CQ).T.
+00001ab0: 8772 4c31 863c 9f7f ceab 867b 6f46 5063  .rL1.<.....{oFPc
+00001ac0: 2ba8 0acb dc77 4a2b 85c5 286c 6c45 5461  +....wJ+..(llETa
+00001ad0: 999b 5169 a5b0 18c9 8dad aa2a 2c73 872a  ..Qi.......*,s.*
+00001ae0: ad14 16a3 c1b1 9559 8565 6e5b a595 c262  .......Y.en[...b
+00001af0: 4439 b6ba db2d f167 282e fd96 41aa 1416  D9...-.g(...A...
+00001b00: a3d2 b115 6285 052a ddef 21a4 95c1 4a8c  ....b..*..!...J.
+00001b10: 6a97 c10f 81e8 b1a0 a8be 014a 95c2 6254  j..........J..bT
+00001b20: 3cb5 2aae b060 0fdc ef32 a495 c262 543d  <.*..`...2...bT=
+00001b30: b5c2 adb0 6053 dc6f 3ba4 95c2 a26e 24b4  ....`S.o;....n$.
+00001b40: 2aaf b060 97dc ef43 12a7 f289 51f9 32f8  *..`...C....Q.2.
+00001b50: 31b7 427f df07 aaca 7da4 5a2e d736 ade7  1.B.....}.Z..6..
+00001b60: 6ac0 1b2d 8cb0 a756 bb35 89b9 7796 de0f  j..-...V.5..w...
+00001b70: 4818 2d4f ad5c 6b12 73ff 2cbd 1f90 30f2  H.-O.\k.s.,...0.
+00001b80: 9d5a 85d6 24e6 1e5a 7a3f 2061 143b b58a  .Z..$..Zz? a.;..
+00001b90: ad49 cc7d b4f4 7e40 c288 746a 7538 a85b  .I.}..~@..tju8.[
+00001ba0: 72a6 4a4b 6f21 59e5 eee7 b1e6 2ded f1be  r.JKo!Y.....-...
+00001bb0: 673a 8500 e66f 6654 ba0c 3e57 52cf 0555  g:...ofT..>WR..U
+00001bc0: 7da3 ee2e d36e 2e46 a673 abc4 ea7a 4155  }....n.F.s...zAU
+00001bd0: ddbe 932a 75bd 189d cead 146b 2e53 a8a5  ...*u......k.S..
+00001be0: 97e2 6284 3ab7 5aac b94c a596 5e8a 8bba  ..b.:.Z..L..^...
+00001bf0: 0b0c 4add 39ea 7386 0d79 bf3b 916a e18a  ..J.9.s..y.;.j..
+00001c00: 6b9a ceef 3938 d519 a9ce 20d5 0ac5 946a  k...98.... ....j
+00001c10: e9fd 0885 d1ea 0c5a ad50 4cad 96de 8f50  .......Z.PL....P
+00001c20: 18b1 ce20 d60a c514 6be9 fd08 8551 eb0c  ... ....k....Q..
+00001c30: 6aad 504c b596 de8f 5018 b9ce 20d7 fd29  j.PL....P... ..)
+00001c40: 0e54 d506 43aa 0525 6d61 9ef2 b6ef e138  .T..C..%ma.....8
+00001c50: bf0d c0ec 5d18 a12e 834f a1ee 89a0 aa84  ....]....O......
+00001c60: 5aaa 4e22 46a2 1790 6845 646e a5a5 d749  Z.N"F...hEdn...I
+00001c70: c488 f302 e2ac 884c 7196 5e27 1123 cb0b  .......Lq.^'.#..
+00001c80: c8b2 2232 6559 7a9d 448c 202f 20c8 fdc1  .."2eYz.D. / ...
+00001c90: 1c54 d5cc 966a 215a b66d dab6 3586 18d3  .T...j!Z.m..5...
+00001ca0: 51fe 5c6c a417 eab0 0ed4 5971 99ea 2c7f  Q.\l......Yq..,.
+00001cb0: 11c5 c548 f502 52ad b84c a996 5e8a 8bd1  ...H..R..L..^...
+00001cc0: ed05 745b 7199 ba2d bd14 1723 e20b 88b8  ..t[q..-...#....
+00001cd0: e232 455c 7a29 2e46 d117 50f4 fe20 12aa  .2E\z).F..P.. ..
+00001ce0: 7ade d70d f891 c394 f31e 53ba 9af2 2b23  z.........S...+#
+00001cf0: e965 f029 e93d 1254 95a4 4bf5 b667 7320  .e.).=.T..K..gs 
+00001d00: 319a be82 a62b 2453 d3a5 d78b c488 fa0a  1....+$S........
+00001d10: a2ae 904c 5197 5e2f 12a3 ea2b a8ba 4232  ...LQ.^/...+..B2
+00001d20: 555d 7abd 488c acaf 20eb fd19 1e54 d5f4  U]z.H... ....T..
+00001d30: 96ea 0d29 efc7 746c fbbc c6b4 1759 bfd8  ...)..tl.....Y..
+00001d40: b6ac 8cac 97c1 e71c 575c a6ac 4b2f c5c5  ........W\..K/..
+00001d50: c8fa 0ab2 aeb8 4c59 975e 8a8b 91f5 1564  ......LY.^.....d
+00001d60: 5d71 99b2 2ebd 1417 23eb 2bc8 bae2 3265  ]q......#.+...2e
+00001d70: 5d7a 292e 46d6 5790 f5fe 380c aa7a dedf  ]z).F.W...8..z..
+00001d80: 653d 2e79 9fe6 f9d8 9663 ddca 9d95 8b67  e=.y.....c.....g
+00001d90: c036 46db cbe0 73de f75c 5055 da2e d572  .6F...s..\PU...r
+00001da0: bddc 5c8c c06f 20f0 8acb 1478 e9a5 b818  ..\..o ....x....
+00001db0: 95df 40e5 1597 a9f2 d24b 7131 52bf 81d4  ..@......Kq1R...
+00001dc0: 2b2e 53ea a597 e262 f47e 03bd efcf c8a0  +.S....b.~......
+00001dd0: aae6 bd54 6fdb ac79 99d6 e388 f376 dc4f  ...To..y.....v.O
+00001de0: 612f 1e68 d918 bd2f 83cf 79af b84c bd97  a/.h.../..y..L..
+00001df0: 5e8a 8bd1 fb0d f45e 7199 7a2f bd14 17a3  ^......^q.z/....
+00001e00: f71b e8bd e232 f55e 7a29 2e46 ef37 d07b  .....2.^z).F.7.{
+00001e10: c565 eabd f452 5c8c de6f a0f7 fd89 1454  .e...R\..o.....T
+00001e20: f5bc af37 66a6 34c7 2013 ffe2 a6e2 cee8  ...7f.4. .......
+00001e30: 7c19 7cce f79e 07aa 4ae7 a55a ae53 fa88  |.|.....J..Z.S..
+00001e40: 87d1 f71d f45d f198 fa2e bd2e 1e46 d777  .....].......F.w
+00001e50: d075 c563 eaba f4ba 7818 3ddf 41cf 158f  .u.c....x.=.A...
+00001e60: a9e7 d2eb e261 747c 6f75 3cf6 2799 5055  .....at|ou<.'.PU
+00001e70: f359 aa85 67db 4298 8e25 8779 4da2 e7f2  .Y..g.B..%.yM...
+00001e80: 67fc 0cfb cee8 7819 fc98 d79a cbd4 71e9  g.....x.......q.
+00001e90: a5b8 181d df5b a5d6 5ca6 8e4b 2fc5 c5e8  .....[..\..K/...
+00001ea0: f8de 2ab5 e632 755c 7a29 2e46 c7f7 56a9  ..*..2u\z).F..V.
+00001eb0: 3597 a9e3 d24b 7131 3abe b73a 1efb 7347  5....Kq1:..:..sG
+00001ec0: a8ea 797f d7f1 658e 695a d6b0 a71c a2f1  ..y...e.iZ......
+00001ed0: 7df5 60f4 bc0c 3ee7 7dcf 0555 a5e7 52bd  }.`...>.}..U..R.
+00001ee0: fb9e 938b d1f5 a355 6e75 bda0 aace 43a5  .......Unu....C.
+00001ef0: 4a71 31fa 7eb4 0aae b94c 7d97 5e8a 8bd1  Jq1.~....L}.^...
+00001f00: f9a3 5572 cd65 eabc f452 5c8c de1f a0f7  ..Ur.e...R\.....
+00001f10: fd19 1754 d5bc 976a e18a 4790 dbef 73cc  ...T...j..G...s.
+00001f20: c79e 6e0f 025c ecdb 0f46 efcb e073 de2b  ..n..\...F...s.+
+00001f30: 2e53 efa5 97e2 62f4 fe00 bd57 5ca6 de4b  .S....b....W\..K
+00001f40: 2fc5 c5e8 fd01 7aaf b84c bd97 5e8a 8bd1  /.....z..L..^...
+00001f50: fb03 f45e 7199 7a2f bd14 17a3 f707 e87d  ...^q.z/.......}
+00001f60: 7f10 0655 3def 6b0e 67df e440 35c9 ff86  ...U=.k.g..@5...
+00001f70: e6f9 4a38 510d 33a3 f5b7 d1e7 a4ef a1b0  ..J8Q.3.........
+00001f80: acd4 be94 cbe5 0a1e 2c46 eac3 0c5a afb1  ........,F...Z..
+00001f90: cc4d 7ce9 7663 314a 1f66 907a 8d65 6a7d  .M|.vc1J.f.z.ej}
+00001fa0: e976 6331 421f 6650 7a8d 654a 7de9 7663  .vc1B.fPz.eJ}.vc
+00001fb0: 313a 1f66 10fa fe1c 0ccb 3adb 23dd 370b  1:.f......:.#.7.
+00001fc0: da97 639a b36c f0c3 b695 2dce f945 bc9b  ..c..l....-..E..
+00001fd0: f78c d687 19c4 5eb3 996a 5fba 3936 46ef  ......^..j_.96F.
+00001fe0: e54b 4c6b 449a cd54 fcd2 cdb1 319a 1f66  .KLkD..T....1..f
+00001ff0: 107d cd66 aa7e e9e6 d818 dd0f 3308 bf66  .}.f.~......3..f
+00002000: 3395 bf74 736c 8cf6 8719 c4bf 3f2f c3f2  3..tsl......?/..
+00002010: 602d dce5 7f8f f235 37ce 695d 43b8 3f76  `-.....57.i]C.?v
+00002020: 30fe 9a1b b860 2684 2fa3 62c3 6ca6 4abf  0....`&./.b.l.J.
+00002030: d570 a69f 8d32 8212 ee3c fd49 b3d9 4650  .p...2...<.I..FP
+00002040: 239b 7e36 ca0d 20c5 39b8 6eb6 1bd4 20a7  #.~6.. .9.n... .
+00002050: 9f8d b204 c876 0ed8 6c4b 90ee b216 fc6c  .....v..lK.....l
+00002060: 942f 40a8 33aa b0e5 0799 cf1a fa5c e723  ./@.3........\.#
+00002070: 4f65 296c fb76 5b0b 57be 5092 9dfe 372a  Oe)l.v[.W.P...7*
+00002080: 400e 74c0 66fb 8274 97eb e667 a37c 01d2  @.t.f..t...g.|..
+00002090: a103 36db 17a4 9b63 a37c 0132 a303 36db  ..6....c.|.2..6.
+000020a0: 17a4 9b63 a37c 0192 a403 36db 17a4 9b63  ...c.|....6....c
+000020b0: a37c 01f2 a56b ff65 2540 59fb 428d 98a6  .|...k.e%@Y.B...
+000020c0: 8bc7 e003 9531 bd8d 7e68 ad66 c198 a9f2  .....1..~h.f....
+000020d0: 819a 33bd 66a1 741f c2a4 0316 5bf7 a5bb  ..3.f.t.....[...
+000020e0: 7c66 d72c 94ce 976c aa75 5d6c 9d97 6e9b  |f.,...l.u]l..n.
+000020f0: 85d2 7588 950e ae8b adeb 3576 7a7d 5d28  ..u.......5vz}](
+00002100: 1d87 a069 7394 747b 83c8 7380 b27a b946  ...is.t{..s..z.F
+00002110: 29df 3c26 4f6b 1380 9587 102e f634 253f  ).<&Ok.......4%?
+00002120: ead7 7148 9bc6 fef0 2e40 59af ab1a 38dd  ..qH.....@Y...8.
+00002130: 2520 b5ec b33c ef56 092f 9ef2 0c25 444a  % ...<.V./...%DJ
+00002140: b0c1 fe5e b381 8eeb 7576 d771 3f1b a5e3  ...^....uv.q?...
+00002150: 903b 1d5c 37d0 71f5 0e82 1a3d f5b3 513a  .;.\7.q....=..Q:
+00002160: 0ef9 d201 1be8 b87a 3341 cd9f fad9 281d  .......z3A....(.
+00002170: 8704 ea80 addd fe0f d642 dddf 7be7 1b95  .........B..{...
+00002180: 420d 9034 8dfd 811f 96f5 5aa8 49d4 bcc8  B..4......Z.I...
+00002190: a371 fbbc 8718 96c3 7844 2894 74a9 7f2d  .q......xD(.t..-
+000021a0: 4016 75c0 063a afd6 428d a3fa d928 dd87  @.u..:..B....(..
+000021b0: 40ea 800d 745f ad85 9a49 f5b3 513e 20d1  @...t_...I..Q> .
+000021c0: d2e6 7b91 fe4c c107 d45a a8c1 543f 1be5  ..{..L...Z..T?..
+000021d0: 0b10 3e1d 5c37 483c a977 77d4 70aa 9f8d  ..>.\7H<.ww.p...
+000021e0: f205 08ab 26f5 ba34 280f d642 3dd6 153f  ....&..4(..B=..?
+000021f0: 90e3 e635 1cf7 af1e 97f7 a44a 2095 580b  ...5.......J .X.
+00002200: adf0 0fd8 6c5f 780f b0ba d928 5f80 40eb  ....l_x....(_.@.
+00002210: 80cd f685 f748 ab9b 8df2 0588 b80e d86c  .....H.........l
+00002220: 5f78 0fb9 bad9 285f 80d0 eb80 cdf6 851a  _x....(_........
+00002230: 7b95 0792 7df3 8dca bdca 8b47 1a0d 49fd  {...}......G..I.
+00002240: 412f 96f5 5a90 eedb fdb2 b8cf 93dc d89b  A/..Z...........
+00002250: f3b2 c813 45c7 71f1 4851 2881 55ff 5a80  ....E.q.HQ(.U.Z.
+00002260: 78eb 80cd f685 1a7f 5ddc 6c94 2f40 0076  x.......].l./@.v
+00002270: c066 fb42 8dc0 fad9 285f 8010 ec80 cdf6  .f.B....(_......
+00002280: 851a 83f5 b351 be00 51d7 019b ed0b 350a  .....Q..Q.....5.
+00002290: eb67 a37c 0192 b149 7d0f 87f2 602d d457  .g.|...I}...`-.W
+000022a0: 80cd bb04 75c3 362f 6b0a a7b1 e139 4509  ....u.6/k....9E.
+000022b0: be12 eb00 3c41 73d9 9e50 83b2 726f dbc1  ....<As..P..ro..
+000022c0: 45f9 0164 6607 d7cb f683 9a9a f571 515e  E..df........qQ^
+000022d0: 0001 da01 97ed 0535 42eb e3a2 7c00 f2b2  .......5B...|...
+000022e0: 032e db07 6a9e d6c5 4545 6a03 a466 9bfb  ....j...EEj..f..
+000022f0: 02f5 3b3c 866a d5fb f7de 53b5 519e c6c8  ..;<.j....S.Q...
+00002300: 21ac f9f6 ecdd f519 5dc9 cbfa e73e a46b  !.......]....>.k
+00002310: 076c b607 bce7 6bdd 6c94 0740 ce76 c066  .l....k.l..@.v.f
+00002320: 7bc0 7bd2 d6cd 4679 0024 6e07 6cb6 07bc  {.{...Fy.$n.l...
+00002330: 676e dd6c 9407 40ba 76c0 667b 404d df26  gn.l..@.v.f{@M.&
+00002340: 371b e501 25ac fbb8 cf97 d4f9 2194 b507  7...%.......!...
+00002350: d404 ae6c 85e4 6022 a645 363c fbd5 bdac  ...l..`".E6<....
+00002360: 92a8 25d6 0178 80e6 b23d a026 707d 5c94  ..%..x...=.&p}\.
+00002370: 0740 fe76 70bd 6c0f a809 5c1f 17e5 0190  .@.vp.l...\.....
+00002380: bf1d 70d9 1e50 13b8 3e2e ca03 2061 3be0  ..p..P..>... a;.
+00002390: b23d 40ba 6f8f 6978 e617 95c1 0d10 b34d  .=@.o.ix.......M
+000023a0: ea8c 1553 b8ca 036a 0c77 c971 da53 9ac3  ...S...j.w.q.S..
+000023b0: 91ef 519a abfd 4fc9 d7fa e73e a471 076c  ..Q...O....>.q.l
+000023c0: b607 d43c ae9f 8df2 0088 e50e d86c 0fa8  ...<.........l..
+000023d0: c15c 3f1b e501 90cf 1db0 d91e 5013 ba7e  .\?.........P..~
+000023e0: 36ca 0320 8a3b 60b3 3da0 4675 fd6c 9407  6.. .;`.=.Fu.l..
+000023f0: 4058 37a9 b369 286b 0fa8 71dd 9853 9e8e  @X7..i(k..q..S..
+00002400: b4ca a34b d97c 66a9 4470 89b5 003e a0d9  ...K.|f.Dp...>..
+00002410: 6c1f a891 5d3f 1be5 0510 da1d 5c37 db0b  l...]?......\7..
+00002420: 6a6c d7cf 46f9 0104 7707 6cb6 1fd4 e8ae  jl..F...w.l.....
+00002430: 9f8d f204 88e7 0ed8 6c4f 90ee e209 6e36  ........lO....n6
+00002440: 2abf 2bdf 63db fd90 7af9 3126 7895 2fd4  *.+.c...z.1&x./.
+00002450: 08ef ee3d df2b b15c ff5a 8010 6fd2 6cb6  ...=.+.\.Z..o.l.
+00002460: 2fd4 18af 9f8d f205 08f2 0ed8 6c5f a851  /...........l_.Q
+00002470: 5e3f 1be5 0b10 e61d b0d9 be50 e3bc 7e36  ^?.........P..~6
+00002480: ca17 20b2 3b60 b37d a146 7afd 6c94 2f40  .. .;`.}.Fz.l./@
+00002490: a837 a933 5b28 ab57 df86 1aeb f5b3 51be  .7.3[(.W......Q.
+000024a0: 00c1 de01 1bf8 825e a7f5 3cd9 bd4e 295f  .......^..<..N)_
+000024b0: 8070 ef80 0d7c 419d efd5 78af ffba 51be  .p...|A...x...Q.
+000024c0: 0001 df01 1bf8 823a dfab 115f 3f1b e50b  .......:..._?...
+000024d0: 10e3 1db0 812f e8b7 f0d7 f364 ef67 4ae5  ...../.....d.gJ.
+000024e0: 7d03 447a 351b 267e d5f9 5e8d fcba af5b  }.Dz5.&~..^....[
+000024f0: 89f3 fa7d 01c2 bf49 9d8b 4259 efdf 6afc  ...}...I..BY..j.
+00002500: 37e7 495e 5a37 cb7b ebe6 fb0d adab 338d  7.I^Z7.{......3.
+00002510: 12ed 25d8 5ae1 1fb0 812f a8b5 50a3 c07e  ..%.Z..../..P..~
+00002520: 36ca 1720 143c 6003 5f50 6ba1 c682 fd6c  6.. .<`._Pk....l
+00002530: 942f 4004 78c0 06be a0d6 428d 08fb d928  ./@.x.....B....(
+00002540: 5f80 90f0 800d 9e17 d56b e17e 6ee0 67a3  _........k.~n.g.
+00002550: 7c01 82c2 599d 7543 79b0 1648 5f28 f15f  |...Y.uCy..H_(._
+00002560: 622d b4c2 3f60 b37d a1c6 85fd 1a42 f902  b-..?`.}.....B..
+00002570: 0486 076c b62f d4c8 b09f 8df2 0588 050f  ...l./..........
+00002580: d86c 5f90 6eea 993b 2a37 1c20 1aac d930  .l_.n..;*7. ...0
+00002590: 39ac d642 8d0e bbaf 5b09 fcfa e71b c483  9..B....[.......
+000025a0: b33a ebc6 f4b0 da23 d5f8 70ca 4227 39eb  .:.....#..p.B'9.
+000025b0: 286f 7ebc bd1e ecea fe6e 8904 136c adf0  (o~......n...l..
+000025c0: 0fd8 6c5f a811 623f 1be5 0b10 221e b0d9  ..l_..b?...."...
+000025d0: be50 63c4 7e36 ca17 202a 3c60 b37d a146  .Pc.~6.. *<`.}.F
+000025e0: 89fd 6c94 2f40 9878 c066 fb42 8d13 fbd9  ..l./@.x.f.B....
+000025f0: 285f 8040 7156 67ca 50d6 be50 23c5 79df  (_.@qVg.P..P#.y.
+00002600: 96f2 26c8 1c37 79f8 43fe 5cdd ef2d 3161  ..&..7y.C.\..-1a
+00002610: 622d 802f 6836 db17 6aac d8cf 46f9 0204  b-./h6..j...F...
+00002620: 8b07 d7cd f685 1a2d f6b3 51be 00f1 e101  .......-..Q.....
+00002630: 9bed 0bd2 5d7c c1cb 262f df27 3ed3 dbe8  ....]|..&/.'>...
+00002640: c7b9 9a62 c3b2 7a36 b694 3936 c617 2204  ...b..z6..96..".
+00002650: 8d73 1f9d c5b2 5a0b a57c cb86 ecc7 3ee5  .s....Z..|....>.
+00002660: 78c8 7b23 f3ed f533 17df 1762 c90f bbd7  x.{#...3...b....
+00002670: c26d f479 dd34 9be9 0ba5 9b63 637c 4142  .m.y.4.....cc|AB
+00002680: 88cd bdc1 c175 337d a174 736c 8c2f 44c8  .....u3}.tsl./D.
+00002690: 1d0f d84c 5f28 dd1c 1be3 0b11 72c7 0336  ...L_(......r..6
+000026a0: d317 4a37 c7c6 f842 84dc 71ee cf99 b13c  ..J7...B..q....<
+000026b0: 580b f507 08e7 3dae f2a0 f8b1 1d71 59c4  X.....=......qY.
+000026c0: 172e 5ecd 21ef dca3 d602 f882 6633 7da1  ..^.!.......f3}.
+000026d0: fc5d f7b3 532f 1be3 0b11 72c7 83eb 66fa  .]..S/....r...f.
+000026e0: 42e9 e6d8 185f 8890 3b1e b099 be50 ba29  B...._..;....P.)
+000026f0: 362a 771c 2158 acd9 3077 dc7f 5f28 dd1c  6*w.!X..0w.._(..
+00002700: 1be5 0b90 3bce fd99 b8e4 b01b f953 3f5d  ....;........S?]
+00002710: 5cca 37b6 f5ea 573b e4c5 f1cc ec87 a471  \.7...W;.......q
+00002720: ee4f fe6e ffb2 8751 e895 f9fe 93b1 71db  .O.n...Q......q.
+00002730: f6e9 c872 e5e6 b564 aeae 5666 c90e fb5d  ...r...d..Vf...]
+00002740: 0a92 c603 3670 82fe ae56 ac49 e3e0 66a3  ....6p...V.I..f.
+00002750: 9c00 a2c4 0336 7082 feae 96fc 32e3 fd53  .....6p.....2..S
+00002760: 74b3 514e 0049 e301 1b38 417f 574b 4238  t.QN.I...8A.WKB8
+00002770: 241b e504 9034 1eb0 c189 825e 99d5 09dc  $....4.....^....
+00002780: d78d 7202 481a 67fd 23a4 e004 faba d5a4  ..r.H.g.#.......
+00002790: 71ca cb94 f291 e497 a4ac 1706 46ea 276b  q...........F.'k
+000027a0: 6fa3 cf1d 9bfa d946 0822 0fd6 6975 824d  o......F."..iu.M
+000027b0: 1ea3 9c8e 597e 5f22 2fb2 56af d729 e504  ....Y~_"/.V..)..
+000027c0: 1025 ce9a 0d9c 40af d3ea 045e 36ee d76d  .%....@....^6..m
+000027d0: 215a acd9 3079 acd6 694d 1e07 371b e504  !Z..0y..iM..7...
+000027e0: 9044 1eb0 d94e 5093 c87e 36ca 1720 993c  .D...NP..~6.. .<
+000027f0: 6083 6f08 6a9d d664 b29f 8df2 0548 2ae7  `.o.j..d.....H*.
+00002800: fe24 467e 37c5 74d0 9a54 564f d17f 79fb  .$F~7.t..TVO..y.
+00002810: e3c7 8f9f df5e 7fbe 3efd 1f00 00ff ff00  .....^..>.......
+00002820: 0000 ffff b229 484c 4ff5 4d2c 4acf cc2b  .....)HLO.M,J..+
+00002830: 56c8 494d 2bb1 5532 d033 5752 28ca 4ccf  V.IM+.U2.3WR(.L.
+00002840: 80b1 4bf2 0bc0 a2a6 4a0a 49f9 2525 f9b9  ..K.....J.I.%%..
+00002850: 305e 466a 624a 6a11 8867 aca4 9096 9f5f  0^FjbJj..g....._
+00002860: 02e3 e8db d9e8 97e7 1765 1767 a4a6 96d8  .........e.g....
+00002870: 0100 0000 ffff 0300 504b 0304 1400 0600  ........PK......
+00002880: 0800 0000 2100 91d7 54d3 4403 0000 720b  ....!...T.D...r.
+00002890: 0000 1400 0000 786c 2f73 6861 7265 6453  ......xl/sharedS
+000028a0: 7472 696e 6773 2e78 6d6c 9456 4d73 9b30  trings.xml.VMs.0
+000028b0: 10bd 77a6 ff41 c3b5 100c 76d2 8ec7 760e  ..w..A....v...v.
+000028c0: 6e33 b9f4 63d2 8fbb 0c6b d004 242a 8934  n3..c....k..$*.4
+000028d0: fef7 5d09 07b0 3038 194e 48bb 6fdf ae56  ..]...08.NH.o..V
+000028e0: abb7 ba7d 2e0b f204 5231 c1d7 5e74 35f3  ...}....R1..^t5.
+000028f0: 08f0 44a4 8c67 6bef f7af bbe0 9347 94a6  ..D..gk......G..
+00002900: 3ca5 85e0 b0f6 0ea0 bcdb cdfb 772b a534  <...........w+.4
+00002910: 415f aed6 5eae 75b5 0c43 95e4 5052 7525  A_..^.u..C..PRu%
+00002920: 2ae0 b8b3 17b2 a41a 7f65 16aa 4a02 4d55  *........e..J.MU
+00002930: 0ea0 cb22 8c67 b39b b0a4 8c7b 2411 35d7  ...".g.....{$.5.
+00002940: 6b6f b1f8 e891 9ab3 bf35 6c9b 959b b9b7  ko.......5l.....
+00002950: 5929 b659 e90d a725 ac42 bd59 85e6 bf59  Y).Y...%.B.Y...Y
+00002960: 4ba8 864c 4806 cadd a1a5 0170 57b7 54ee  K..LH......pW.T.
+00002970: 0427 2913 cf2c 059f 304e 2893 97ac b8e0  .')..,..0N(.....
+00002980: c15e 28c5 8a4b 96af b492 a224 4ab0 8208  .^(..K.....$J...
+00002990: 4976 4c60 b514 5657 248f 97f0 b578 935f  IvL`..VW$....x._
+000029a0: 29f8 31d1 4962 3db3 b732 eb5c 278a 9417  ).1.Ib=..2.\'...
+000029b0: 420a d307 6e7a 9f19 675a 8a0c 3879 0172  B...nz..gZ..8y.r
+000029c0: 4dbe e89c 723c a9c8 375f 1c68 d092 ee8b  M...r<..7_.h....
+000029d0: 1a11 039f dcdf 6d83 68be a093 5e81 962c  ......m.h...^..,
+000029e0: b11c 8cc7 d6b8 2c66 173d 4e63 2ce6 9331  ......,f.=Nc,..1
+000029f0: 9057 1b03 591a 9e92 b508 3664 349f 0819  .W..Y.....6d4...
+00002a00: a42f 0ca3 a00b dc50 8d76 d38e a744 afe3  ./.....P.v...D..
+00002a10: 09a2 7117 671c b367 644b 3e28 7a93 ce62  ..q.g..gdK>(z..b
+00002a20: 1421 3816 1bbd 319e 9b4e 3c9a 8e29 5b57  .!8...1..N<..)[W
+00002a30: 0773 de27 556c 4e2e 1e2d 63dc 8b7b ae55  .s.'UlN..-c..{.U
+00002a40: 2ced 7894 7643 1a67 96ee daab c9f4 7a2c  ,.x.vC.g......z,
+00002a50: d31c 9e9d 568c 6ec6 6c4f 816d dfc6 03e0  ....V.n.lO.m....
+00002a60: af60 bbdd c538 2efb 6487 d7d3 b6bd 99c2  .`...8..d.......
+00002a70: 249a cda2 69d3 26a7 fe19 348e 7174 c1b1  $...i.&...4.qt..
+00002a80: dfbd f78d cf7c 22d8 308e a95c 1c8f b26b  .....|".0..\...k
+00002a90: 1c06 7764 70b6 6de6 6d5f 981b bc0d e683  ..wdp.m.m_......
+00002aa0: fb3b b0ec 65dd 9cfc 2899 17ec d34e 8dc7  .;..e...(....N..
+00002ab0: 4bd4 2f28 e639 1fcf f3fc d86d b9ee 5f3d  K./(.9.....m.._=
+00002ac0: 6e5b 1733 27db 61f6 100c 0759 6b39 3e90  n[.3'.a....Yk9>.
+00002ad0: 5b13 3b4c 7b68 d178 594f e7ee 038e d0d1  [.;L{h.xYO......
+00002ae0: 7ab6 a3d0 1980 530e 2743 6c78 c7bf e133  z.....S.'Clx...3
+00002af0: c112 621f 3317 c6ec d927 c462 e0b3 ee1a  ..b.3....'.b....
+00002b00: fc00 d9c0 db3b c807 fb3f eb62 5f4b d2de  .....;...?.b_K..
+00002b10: e633 107f be6f 7df2 240a aa59 01f8 6a67  .3...o}.$..Y..jg
+00002b20: 9423 9d44 9415 aa8c 54f9 285a 5405 09db  .#.D....T.(ZT...
+00002b30: 3348 719b 658c bb2c 38d5 b5a4 0591 a044  3Hq.e..,8......D
+00002b40: 2d13 582e cf8b 0fd4 23cb 6521 fe81 4449  -.X.....#.e!..DI
+00002b50: 20a9 16aa ca41 02f9 40ea aac2 454c b63a   ....A..@...EL.:
+00002b60: aeb9 21ac ab39 f65a eea8 5536 4660 d826  ..!..9.Z..U6F`.&
+00002b70: cb59 961b 0197 3c0e 9592 09d8 e37f 16b5  .Y....<.........
+00002b80: 434c 0aa1 80a0 10c9 a4c9 fdac 35d2 2795  CL..........5.'.
+00002b90: a86a 532f 23b7 802b a60f 3ec1 a995 e10b  .jS/#..+..>.....
+00002ba0: 3e14 0296 39e3 a910 0331 6674 d272 4933  >...9....1ft.rI3
+00002bb0: 3cff bab0 2574 4336 16a8 2f00 0b76 38bf  <...%tC6../..v8.
+00002bc0: 8bd8 35ee 323a 9070 8df7 44fe ae66 ecee  ..5.2:.p..D..f..
+00002bd0: 95df 1e26 b682 9490 986c ddf8 f787 d4b6  ...&.....l......
+00002be0: 67b7 1ea2 66de fc07 0000 ffff 0300 504b  g...f.........PK
+00002bf0: 0304 1400 0600 0800 0000 2100 3abe f890  ..........!.:...
+00002c00: 5a01 0000 7102 0000 1100 0801 646f 6350  Z...q.......docP
+00002c10: 726f 7073 2f63 6f72 652e 786d 6c20 a204  rops/core.xml ..
+00002c20: 0128 a000 0100 0000 0000 0000 0000 0000  .(..............
 00002c30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002c40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002c50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002c60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002c70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002c80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002c90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002ca0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002cb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002cc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002cd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002ce0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002cf0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002d00: 0000 007c 9251 4bc3 3014 85df 05ff 43c8  ...|.QK.0.....C.
-00002d10: 7b9b a673 324b db81 933d 5914 dc50 7c0b  {..s2K...=Y..P|.
-00002d20: c9ed 166c 9392 64d6 fd7b d376 ab1d 8a8f  ...l..d..{.v....
-00002d30: b9e7 e4cb 3997 a4cb afba 429f 60ac d42a  ....9.....B.`..*
-00002d40: c334 8c30 02c5 b590 6a97 e1ed 661d 2c30  .4.0....j...f.,0
-00002d50: b28e 29c1 2aad 20c3 47b0 7899 5f5f a5bc  ..).*. .G.x.__..
-00002d60: 49b8 36f0 6c74 03c6 49b0 c893 944d 7893  I.6.lt..I....Mx.
-00002d70: e1bd 734d 4288 e57b a899 0dbd 4379 b1d4  ..sMB..{....Cy..
-00002d80: a666 ce1f cd8e 348c 7fb0 1d90 388a 6e49  .f....4.....8.nI
-00002d90: 0d8e 09e6 18e9 8041 3312 f109 29f8 886c  .......A3...)..l
-00002da0: 0ea6 ea01 8213 a8a0 06e5 2ca1 2125 3f5e  ..........,.!%?^
-00002db0: 07a6 b67f 5ee8 9589 b396 eed8 f84e a7b8  ....^........N..
-00002dc0: 53b6 e083 38ba bfac 1c8d 6ddb 86ed ac8f  S...8.....m.....
-00002dd0: e1f3 53f2 563c bef4 5503 a9ba 5d71 c079  ..S.V<..U...]q.y
-00002de0: 2a78 c20d 30a7 4dbe da1b 6951 7170 50a5  *x..0.M...iQqpP.
-00002df0: 6432 ef76 5831 eb0a bfee 5282 b83f e685  d2.vX1....R..?..
-00002e00: e446 5b5d 3af4 5496 9203 da5a 3029 f96d  .F[]:.T....Z0).m
-00002e10: f4fc bece f008 08e4 0326 439d b3f2 3a5b  .........&C...:[
-00002e20: 3d6c d638 8fa3 9806 511c c4f1 265a 2473  =l.8....Q...&Z$s
-00002e30: 9acc efde bb1c 17f7 bbc0 c3a0 3ea5 f99f  ............>...
-00002e40: 380b a29b 802e 3a22 a549 3c9f 10cf 80bc  8.....:".I<.....
-00002e50: cf7d f949 f26f 0000 00ff ff03 0050 4b03  .}.I.o.......PK.
-00002e60: 0414 0006 0008 0000 0021 00e4 ee61 559b  .........!...aU.
-00002e70: 0100 0033 0300 0010 0008 0164 6f63 5072  ...3.......docPr
-00002e80: 6f70 732f 6170 702e 786d 6c20 a204 0128  ops/app.xml ...(
-00002e90: a000 0100 0000 0000 0000 0000 0000 0000  ................
-00002ea0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002eb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002d00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002d10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002d20: 0000 0000 007c 9251 4fc3 2014 85df 4dfc  .....|.QO. ...M.
+00002d30: 0f0d ef2d a573 3a49 db25 ceec c946 13b7  ...-.s:I.%...F..
+00002d40: 687c 2370 bb11 5b68 80d9 eddf 4bbb ad76  h|#p..[h....K..v
+00002d50: d1f8 c83d 878f 736e 48e7 fbba 0abe c058  ...=..snH......X
+00002d60: a955 8648 14a3 0014 d742 aa4d 86d6 ab65  .U.H.....B.M...e
+00002d70: 3843 8175 4c09 5669 0519 3a80 45f3 fcfa  8C.uL.Vi..:.E...
+00002d80: 2ae5 0de5 dac0 8bd1 0d18 27c1 069e a42c  *.........'....,
+00002d90: e54d 86b6 ce35 1463 cbb7 5033 1b79 87f2  .M...5.c..P3.y..
+00002da0: 62a9 4dcd 9c3f 9a0d 6e18 ff64 1bc0 491c  b.M..?..n..d..I.
+00002db0: dfe2 1a1c 13cc 31dc 01c3 6620 a213 52f0  ......1...f ..R.
+00002dc0: 01d9 ec4c d503 04c7 5041 0dca 594c 2282  ...L....PA..YL".
+00002dd0: 7fbc 0e4c 6dff bcd0 2b23 672d dda1 f19d  ...Lm...+#g-....
+00002de0: 4e71 c76c c18f e2e0 de5b 3918 dbb6 8dda  Nq.l.....[9.....
+00002df0: 491f c3e7 27f8 bd78 7aed ab86 5275 bbe2  I...'..xz...Ru..
+00002e00: 80f2 5470 ca0d 30a7 4dbe d81a 6983 62e7  ..Tp..0.M...i.b.
+00002e10: a04a f168 deed b062 d615 7edd a504 f170  .J.h...b..~....p
+00002e20: c80b c98d b6ba 74c1 7359 4a0e c1da 8249  ......t.sYJ....I
+00002e30: f16f a3e7 f775 8e8f 8008 7c40 7aac 7356  .o...u....|@z.sV
+00002e40: de26 8bc7 d512 e549 9c90 304e c224 59c5  .&.....I..0N.$Y.
+00002e50: 333a 2574 7aff d1e5 b8b8 df05 3e0e ea53  3:%tz.......>..S
+00002e60: 9aff 8993 30be 09c9 ac23 9298 4eef 46c4  ....0....#..N.F.
+00002e70: 3320 ef73 5f7e 92fc 1b00 00ff ff03 0050  3 .s_~.........P
+00002e80: 4b03 0414 0006 0008 0000 0021 00e4 ee61  K..........!...a
+00002e90: 559b 0100 0033 0300 0010 0008 0164 6f63  U....3.......doc
+00002ea0: 5072 6f70 732f 6170 702e 786d 6c20 a204  Props/app.xml ..
+00002eb0: 0128 a000 0100 0000 0000 0000 0000 0000  .(..............
 00002ec0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002ed0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002ee0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002ef0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002f00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002f10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002f20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002f30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002f40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002f50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002f60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002f70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002f80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002f90: 0000 009c 934d 6fdb 300c 86ef 03f6 1f0c  .....Mo.0.......
-00002fa0: dd1b 395d 510c 81ac a248 5bf4 b0a2 01e2  ..9]Q....H[.....
-00002fb0: 7667 4ea6 63a1 b264 88ac 91ec d757 b6d1  vgN.c..d.....W..
-00002fc0: c4d9 76da 8d1f 2f5e 3ea2 2475 b36f 5dd6  ..v.../^>.$u.o].
-00002fd0: 6324 1b7c 2196 8b5c 64e8 4da8 acdf 15e2  c$.|!..\d.M.....
-00002fe0: a57c b8f8 2e32 62f0 15b8 e0b1 1007 2471  .|...2b.......$q
-00002ff0: a3bf 7e51 9b18 3a8c 6c91 b264 e1a9 100d  ..~Q..:.l..d....
-00003000: 73b7 9292 4c83 2dd0 22b5 7dea d421 b6c0  s...L.-.".}..!..
-00003010: 298d 3b19 eada 1abc 0be6 bd45 cff2 32cf  ).;........E..2.
-00003020: af25 ee19 7d85 d545 7734 1493 e3aa e7ff  .%..}..Ew4......
-00003030: 35ad 8219 f8e8 b53c 7409 58ab 3230 b8d2  5......<t.X.20..
-00003040: b6a8 7325 4f89 baed 3a67 0d70 3abd 7eb2  ..s%O...:g.p:.~.
-00003050: 2606 0a35 674f 60ac e740 4d76 bf37 e894  &..5gO`..@Mv.7..
-00003060: 9ccb 54e2 dfa2 798f 960f 83db 3c55 5b03  ..T...y.....<U[.
-00003070: 0ed7 69b4 aec1 112a 792a a847 8461 ad1b  ..i....*y*.G.a..
-00003080: b091 b4ea 79d5 a3e1 1033 b2bf d362 2f45  ....y....3...b/E
-00003090: f60b 0807 e042 f410 2d78 4ee0 836c 4ac6  .....B..-xN..lJ.
-000030a0: d875 c451 ff0c f18d 1a44 2625 9360 2a8e  .u.Q.....D&%.`*.
-000030b0: e15c 3b8f ed95 5e8e 8214 9c0b 0783 0924  .\;...^........$
-000030c0: 35ce 114b cb0e e9b9 de40 e47f 102f e7c4  5..K.....@.../..
-000030d0: 23c3 c43b e16c 07be 69e6 9c6f 3c72 9af4  #..;.l..i..o<r..
-000030e0: 87f7 3ab4 1df8 436a 1ca3 1fd6 bfd1 4b57  ..:...Cj......KW
-000030f0: 863b 60fc 5ce7 7951 6d1b 8858 a51b 38ae  .;`.\.yQm..X..8.
-00003100: fb58 508f 6993 d10d 26eb 06fc 0eab 4fcd  .XP.i...&.....O.
-00003110: df8d e119 bc4e 7f40 2faf 17f9 b73c ddeb  .....N.@/....<..
-00003120: aca6 e4e9 b5eb 0f00 0000 ffff 0300 504b  ..............PK
-00003130: 0102 2d00 1400 0600 0800 0000 2100 62ee  ..-.........!.b.
-00003140: 9d68 5e01 0000 9004 0000 1300 0000 0000  .h^.............
-00003150: 0000 0000 0000 0000 0000 0000 5b43 6f6e  ............[Con
-00003160: 7465 6e74 5f54 7970 6573 5d2e 786d 6c50  tent_Types].xmlP
-00003170: 4b01 022d 0014 0006 0008 0000 0021 00b5  K..-.........!..
-00003180: 5530 23f4 0000 004c 0200 000b 0000 0000  U0#....L........
-00003190: 0000 0000 0000 0000 0097 0300 005f 7265  ............._re
-000031a0: 6c73 2f2e 7265 6c73 504b 0102 2d00 1400  ls/.relsPK..-...
-000031b0: 0600 0800 0000 2100 813e 9497 f300 0000  ......!..>......
-000031c0: ba02 0000 1a00 0000 0000 0000 0000 0000  ................
-000031d0: 0000 bc06 0000 786c 2f5f 7265 6c73 2f77  ......xl/_rels/w
-000031e0: 6f72 6b62 6f6f 6b2e 786d 6c2e 7265 6c73  orkbook.xml.rels
-000031f0: 504b 0102 2d00 1400 0600 0800 0000 2100  PK..-.........!.
-00003200: 082f ba25 0203 0000 0907 0000 0f00 0000  ./.%............
-00003210: 0000 0000 0000 0000 0000 ef08 0000 786c  ..............xl
-00003220: 2f77 6f72 6b62 6f6f 6b2e 786d 6c50 4b01  /workbook.xmlPK.
-00003230: 022d 0014 0006 0008 0000 0021 0027 96d6  .-.........!.'..
-00003240: b5ca 0200 000a 0700 000d 0000 0000 0000  ................
-00003250: 0000 0000 0000 001e 0c00 0078 6c2f 7374  ...........xl/st
-00003260: 796c 6573 2e78 6d6c 504b 0102 2d00 1400  yles.xmlPK..-...
-00003270: 0600 0800 0000 2100 c117 10be 4e07 0000  ......!.....N...
-00003280: c620 0000 1300 0000 0000 0000 0000 0000  . ..............
-00003290: 0000 130f 0000 786c 2f74 6865 6d65 2f74  ......xl/theme/t
-000032a0: 6865 6d65 312e 786d 6c50 4b01 022d 0014  heme1.xmlPK..-..
-000032b0: 0006 0008 0000 0021 0067 8c4f 028e 1100  .......!.g.O....
-000032c0: 008b 8600 0018 0000 0000 0000 0000 0000  ................
-000032d0: 0000 0092 1600 0078 6c2f 776f 726b 7368  .......xl/worksh
-000032e0: 6565 7473 2f73 6865 6574 312e 786d 6c50  eets/sheet1.xmlP
-000032f0: 4b01 022d 0014 0006 0008 0000 0021 0091  K..-.........!..
-00003300: d754 d344 0300 0072 0b00 0014 0000 0000  .T.D...r........
-00003310: 0000 0000 0000 0000 0056 2800 0078 6c2f  .........V(..xl/
-00003320: 7368 6172 6564 5374 7269 6e67 732e 786d  sharedStrings.xm
-00003330: 6c50 4b01 022d 0014 0006 0008 0000 0021  lPK..-.........!
-00003340: 0053 33c0 605a 0100 0071 0200 0011 0000  .S3.`Z...q......
-00003350: 0000 0000 0000 0000 0000 00cc 2b00 0064  ............+..d
-00003360: 6f63 5072 6f70 732f 636f 7265 2e78 6d6c  ocProps/core.xml
-00003370: 504b 0102 2d00 1400 0600 0800 0000 2100  PK..-.........!.
-00003380: e4ee 6155 9b01 0000 3303 0000 1000 0000  ..aU....3.......
-00003390: 0000 0000 0000 0000 0000 5d2e 0000 646f  ..........]...do
-000033a0: 6350 726f 7073 2f61 7070 2e78 6d6c 504b  cProps/app.xmlPK
-000033b0: 0506 0000 0000 0a00 0a00 8002 0000 2e31  ...............1
-000033c0: 0000 0000                                ....
+00002f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002fb0: 0000 0000 009c 934d 6fdb 300c 86ef 03f6  .......Mo.0.....
+00002fc0: 1f0c dd1b 395d 510c 81ac a248 5bf4 b0a2  ....9]Q....H[...
+00002fd0: 01e2 7667 4ea6 63a1 b264 88ac 91ec d757  ..vgN.c..d.....W
+00002fe0: b6d1 c4d9 76da 8d1f 2f5e 3ea2 2475 b36f  ....v.../^>.$u.o
+00002ff0: 5dd6 6324 1b7c 2196 8b5c 64e8 4da8 acdf  ].c$.|!..\d.M...
+00003000: 15e2 a57c b8f8 2e32 62f0 15b8 e0b1 1007  ...|...2b.......
+00003010: 2471 a3bf 7e51 9b18 3a8c 6c91 b264 e1a9  $q..~Q..:.l..d..
+00003020: 100d 73b7 9292 4c83 2dd0 22b5 7dea d421  ..s...L.-.".}..!
+00003030: b6c0 298d 3b19 eada 1abc 0be6 bd45 cff2  ..).;........E..
+00003040: 32cf af25 ee19 7d85 d545 7734 1493 e3aa  2..%..}..Ew4....
+00003050: e7ff 35ad 8219 f8e8 b53c 7409 58ab 3230  ..5......<t.X.20
+00003060: b8d2 b6a8 7325 4f89 baed 3a67 0d70 3abd  ....s%O...:g.p:.
+00003070: 7eb2 2606 0a35 674f 60ac e740 4d76 bf37  ~.&..5gO`..@Mv.7
+00003080: e894 9ccb 54e2 dfa2 798f 960f 83db 3c55  ....T...y.....<U
+00003090: 5b03 0ed7 69b4 aec1 112a 792a a847 8461  [...i....*y*.G.a
+000030a0: ad1b b091 b4ea 79d5 a3e1 1033 b2bf d362  ......y....3...b
+000030b0: 2f45 f60b 0807 e042 f410 2d78 4ee0 836c  /E.....B..-xN..l
+000030c0: 4ac6 d875 c451 ff0c f18d 1a44 2625 9360  J..u.Q.....D&%.`
+000030d0: 2a8e e15c 3b8f ed95 5e8e 8214 9c0b 0783  *..\;...^.......
+000030e0: 0924 35ce 114b cb0e e9b9 de40 e47f 102f  .$5..K.....@.../
+000030f0: e7c4 23c3 c43b e16c 07be 69e6 9c6f 3c72  ..#..;.l..i..o<r
+00003100: 9af4 87f7 3ab4 1df8 436a 1ca3 1fd6 bfd1  ....:...Cj......
+00003110: 4b57 863b 60fc 5ce7 7951 6d1b 8858 a51b  KW.;`.\.yQm..X..
+00003120: 38ae fb58 508f 6993 d10d 26eb 06fc 0eab  8..XP.i...&.....
+00003130: 4fcd df8d e119 bc4e 7f40 2faf 17f9 b73c  O......N.@/....<
+00003140: ddeb aca6 e4e9 b5eb 0f00 0000 ffff 0300  ................
+00003150: 504b 0102 2d00 1400 0600 0800 0000 2100  PK..-.........!.
+00003160: 62ee 9d68 5e01 0000 9004 0000 1300 0000  b..h^...........
+00003170: 0000 0000 0000 0000 0000 0000 0000 5b43  ..............[C
+00003180: 6f6e 7465 6e74 5f54 7970 6573 5d2e 786d  ontent_Types].xm
+00003190: 6c50 4b01 022d 0014 0006 0008 0000 0021  lPK..-.........!
+000031a0: 00b5 5530 23f4 0000 004c 0200 000b 0000  ..U0#....L......
+000031b0: 0000 0000 0000 0000 0000 0097 0300 005f  ..............._
+000031c0: 7265 6c73 2f2e 7265 6c73 504b 0102 2d00  rels/.relsPK..-.
+000031d0: 1400 0600 0800 0000 2100 813e 9497 f300  ........!..>....
+000031e0: 0000 ba02 0000 1a00 0000 0000 0000 0000  ................
+000031f0: 0000 0000 bc06 0000 786c 2f5f 7265 6c73  ........xl/_rels
+00003200: 2f77 6f72 6b62 6f6f 6b2e 786d 6c2e 7265  /workbook.xml.re
+00003210: 6c73 504b 0102 2d00 1400 0600 0800 0000  lsPK..-.........
+00003220: 2100 d48d b40e 0203 0000 0907 0000 0f00  !...............
+00003230: 0000 0000 0000 0000 0000 0000 ef08 0000  ................
+00003240: 786c 2f77 6f72 6b62 6f6f 6b2e 786d 6c50  xl/workbook.xmlP
+00003250: 4b01 022d 0014 0006 0008 0000 0021 0027  K..-.........!.'
+00003260: 96d6 b5ca 0200 000a 0700 000d 0000 0000  ................
+00003270: 0000 0000 0000 0000 001e 0c00 0078 6c2f  .............xl/
+00003280: 7374 796c 6573 2e78 6d6c 504b 0102 2d00  styles.xmlPK..-.
+00003290: 1400 0600 0800 0000 2100 c117 10be 4e07  ........!.....N.
+000032a0: 0000 c620 0000 1300 0000 0000 0000 0000  ... ............
+000032b0: 0000 0000 130f 0000 786c 2f74 6865 6d65  ........xl/theme
+000032c0: 2f74 6865 6d65 312e 786d 6c50 4b01 022d  /theme1.xmlPK..-
+000032d0: 0014 0006 0008 0000 0021 000b 0422 b9b0  .........!..."..
+000032e0: 1100 00e0 8700 0018 0000 0000 0000 0000  ................
+000032f0: 0000 0000 0092 1600 0078 6c2f 776f 726b  .........xl/work
+00003300: 7368 6565 7473 2f73 6865 6574 312e 786d  sheets/sheet1.xm
+00003310: 6c50 4b01 022d 0014 0006 0008 0000 0021  lPK..-.........!
+00003320: 0091 d754 d344 0300 0072 0b00 0014 0000  ...T.D...r......
+00003330: 0000 0000 0000 0000 0000 0078 2800 0078  ...........x(..x
+00003340: 6c2f 7368 6172 6564 5374 7269 6e67 732e  l/sharedStrings.
+00003350: 786d 6c50 4b01 022d 0014 0006 0008 0000  xmlPK..-........
+00003360: 0021 003a bef8 905a 0100 0071 0200 0011  .!.:...Z...q....
+00003370: 0000 0000 0000 0000 0000 0000 00ee 2b00  ..............+.
+00003380: 0064 6f63 5072 6f70 732f 636f 7265 2e78  .docProps/core.x
+00003390: 6d6c 504b 0102 2d00 1400 0600 0800 0000  mlPK..-.........
+000033a0: 2100 e4ee 6155 9b01 0000 3303 0000 1000  !...aU....3.....
+000033b0: 0000 0000 0000 0000 0000 0000 7f2e 0000  ................
+000033c0: 646f 6350 726f 7073 2f61 7070 2e78 6d6c  docProps/app.xml
+000033d0: 504b 0506 0000 0000 0a00 0a00 8002 0000  PK..............
+000033e0: 5031 0000 0000                           P1....
```

### Comparing `premise_gwp-0.8/premise_gwp/data/lcia_gwp_20a.xlsx` & `premise_gwp-0.9/premise_gwp/data/lcia_gwp_20a.xlsx`

 * *Files identical despite different names*

### Comparing `premise_gwp-0.8/premise_gwp/data/lcia_gwp_20a_w_bio.xlsx` & `premise_gwp-0.9/premise_gwp/data/lcia_gwp2021_100a_w_bio.xlsx`

 * *Files 25% similar despite different names*

```diff
@@ -137,695 +137,731 @@
 00000880: cbb4 e480 fa84 53ec ad82 b4b7 b720 9a29  ......S...... .)
 00000890: 66e5 ffb9 43db f606 9f82 791f d1f3 1909  f...C.....y.....
 000008a0: 493c 0d79 00d1 e8d4 212b f8c1 45f6 08f2  I<.y....!+..E...
 000008b0: bcfc 664d 79ce 6bc1 a3fa 0ce5 1cab 4b1e  ..fMy.k.......K.
 000008c0: aa35 3d7c 8674 2087 c847 1f7f 2992 73e5  .5=|.t ..G..).s.
 000008d0: a299 bb55 efe1 7442 fbca 29bf dbf2 2ccb  ...U..tB..)...,.
 000008e0: f4ef 66e4 c9c7 d5df 0000 00ff ff03 0050  ..f............P
-000008f0: 4b03 0414 0006 0008 0000 0021 00d4 8db4  K..........!....
-00000900: 0e02 0300 0009 0700 000f 0000 0078 6c2f  .............xl/
-00000910: 776f 726b 626f 6f6b 2e78 6d6c ac55 db6e  workbook.xml.U.n
-00000920: e230 107d 5f69 ff21 f27b ea38 8400 5143  .0.}_i.!.{.8..QC
-00000930: 556e bb48 ed6e d5eb 6365 1243 2c12 3b6b  Un.H.n..ce.C,.;k
-00000940: 3b85 aaea bfef 3810 28e5 a5db 6e04 be8d  ;.....8.(...n...
-00000950: 7372 66e6 8c7d 7ab6 2e72 e789 29cd a588  srf..}z..r..)...
-00000960: 1139 f190 c344 2253 2e16 31ba bb9d b85d  .9...D"S..1....]
-00000970: e468 4345 4a73 2958 8c9e 9946 67fd efdf  .hCEJs)X...Fg...
-00000980: 4e57 522d 6752 2e1d 0010 3a46 9931 6584  NWR-gR....:F.1e.
-00000990: b14e 3256 507d 224b 26c0 3297 aaa0 06a6  .N2VP}"K&.2.....
-000009a0: 6a81 75a9 184d 75c6 9829 72ec 7b5e 880b  j.u..Mu..)r.{^..
-000009b0: ca05 da20 44ea 2318 723e e709 1bc9 a42a  ... D.#.r>.....*
-000009c0: 9830 1b10 c572 6a80 bece 78a9 1bb4 22f9  .0...rj...x...".
-000009d0: 085c 41d5 b22a dd44 1625 40cc 78ce cd73  .\A..*.D.%@.x..s
-000009e0: 0d8a 9c22 89a6 0b21 159d e5e0 f69a b49d  ..."...!........
-000009f0: b582 5f08 7fe2 41e3 375f 02d3 d1a7 0a9e  .._...A.7_......
-00000a00: 28a9 e5dc 9c00 34de 903e f29f 7898 9083  (.....4..>..x...
-00000a10: 10ac 8f63 f031 a400 2bf6 c46d 0e77 ac54  ...c.1..+..m.w.T
-00000a20: f849 56e1 0e2b dc83 11ef cb68 04a4 556b  .IV..+.....h..Uk
-00000a30: 2582 e07d 12ad bde3 e6a3 fee9 9ce7 ec7e  %..}...........~
-00000a40: 235d 8796 e52f 5ad8 4ce5 c8c9 a936 e394  #].../Z.L....6..
-00000a50: 1b96 c6a8 0353 b962 fb05 f04a 55e5 a0e2  .....S.b...JU...
-00000a60: 3958 89d7 223e c2fd 9d9c af94 93b2 39ad  9X..">........9.
-00000a70: 7273 0b42 6ee0 6163 18f6 fcb6 dd09 c238  rs.Bn.ac.......8
-00000a80: cf0d 5382 1a36 94c2 800e b77e 7d55 7335  ..S..6.....~}Us5
-00000a90: f630 93a0 70e7 9afd a9b8 6250 58a0 2ff0  .0..p.....bPX./.
-00000aa0: 155a 9a44 74a6 afa8 c99c 4ae5 31c2 771a  .Z.Dt.....J.1.w.
-00000ab0: 9cc7 4ada 2ac2 3fb8 f959 cd30 d458 c135  ..J.*.?..Y.0.X.5
-00000ac0: 7b5c acca 8371 4a0d c56f 244b 8feb e31f  {\...qJ..o$K....
-00000ad0: 444b 131b 090c a1d8 d0dd 8cdf 8705 58ab  DK............X.
-00000ae0: a811 e695 510e 8ca7 a30b 48ce 0d7d 8254  ....Q.....H..}.T
-00000af0: 8120 d26d 254f 6d2e 5a8f 2251 1179 7c99  . .m%Om.Z."Q.y|.
-00000b00: 0cc9 8010 3276 8349 77e2 8ebd 2070 07a4  ....2v.Iw... p..
-00000b10: d572 bdc9 30ec b547 0121 93f0 159c 5161  .r..0..G.!....Qa
-00000b20: 9448 5a99 6cab 020b 1da3 0052 7e64 baa4  .HZ.l......R~d..
-00000b30: ebc6 42bc a8e2 e99e c68b b77d 5cdb bf6b  ..B........}\..k
-00000b40: 1adb ab75 d89e 77f7 9cad f45e 2f76 eaac  ...u..w....^/v..
-00000b50: 1fb8 48e5 aaf6 e8b9 1977 42f0 6f55 1b1e  ..H......wB.oU..
-00000b60: 786a b218 f9dd aeb7 5bfb c9f8 2203 b6a4  xj......[..."...
-00000b70: d5b6 8b50 1396 558c 0ed8 8c36 6c26 f0b8  ...P..U....6l&..
-00000b80: b639 6083 dfd0 a94f 55a0 55f7 8ea8 2be1  .9`....OU.U...+.
-00000b90: c69e b404 8e6f dbd7 0106 e547 f61b 6a9a  .....o.....G..j.
-00000ba0: 923a 81cd 6b09 cd13 50be edea 8da1 df23  .:..k...P......#
-00000bb0: 2d54 cf2f 650a a92a a8a8 2854 96dd f15b  -T./e..*..(T...[
-00000bc0: 34e9 8390 b0b5 b9d0 a6ee 4195 1cf8 93c0  4.........A.....
-00000bd0: 3bef 78bd c0f5 c6ad b61b 747b bedb 0d5a  ;.x.......t{...Z
-00000be0: be3b 0c46 feb8 dd19 8fc6 83b6 4d9e bd36  .;.F........M..6
-00000bf0: a2ff 7178 d6c5 1135 f791 7523 a3ca dc2a  ..qx...5..u#...*
-00000c00: 9a2c e116 bb66 f301 d5e0 c2c6 63e0 0b62  .,...f......c..b
-00000c10: 6d58 e3e6 adfe 5f00 0000 ffff 0300 504b  mX...._.......PK
-00000c20: 0304 1400 0600 0800 0000 2100 2796 d6b5  ..........!.'...
-00000c30: ca02 0000 0a07 0000 0d00 0000 786c 2f73  ............xl/s
-00000c40: 7479 6c65 732e 786d 6cb4 55db 6edb 300c  tyles.xml.U.n.0.
-00000c50: 7d1f b07f 10f4 eeca 76e3 2c09 6c17 4b53  }.......v.,.l.KS
-00000c60: 0305 b661 403b 60af 8a2d 2742 7531 2425  ...a@;`..-'Bu1$%
-00000c70: 7336 ecdf 47d9 4ee2 a2dd adc3 5e62 8912  s6..G.N.....^b..
-00000c80: 0f0f 0f29 26bd 6aa5 407b 662c d72a c3d1  ...)&.j.@{f,.*..
-00000c90: 4588 1153 a5ae b8da 64f8 d37d 11cc 30b2  E..S....d..}..0.
-00000ca0: 8eaa 8a0a ad58 860f cce2 abfc f5ab d4ba  .....X..........
-00000cb0: 8360 775b c61c 0208 6533 bc75 ae59 1062  .`w[....e3.u.Y.b
-00000cc0: cb2d 93d4 5ee8 8629 38a9 b591 d4c1 d66c  .-..^..)8......l
-00000cd0: 886d 0ca3 95f5 4e52 9038 0ca7 4452 ae70  .m....NR.8..DR.p
-00000ce0: 8fb0 90e5 9f80 486a 1e76 4d50 6ad9 50c7  ......Hj.vMPj.P.
-00000cf0: d75c 7077 e8b0 3092 e5e2 76a3 b4a1 6b01  .\pw..0...v...k.
-00000d00: 54db 6842 4bd4 4653 13a3 d61c 8374 d627  T.hBK.FS.....t.'
-00000d10: 7124 2f8d b6ba 7617 804b 745d f392 3da5  q$/...v..Kt]..=.
-00000d20: 3b27 7342 cb33 1220 bf0c 294a 4818 3fca  ;'sB.3. ..)JH.?.
-00000d30: bd35 2f44 9a10 c3f6 dc97 0fe7 69ad 95b3  .5/D........i...
-00000d40: a8d4 3be5 321c 0351 2fc1 e241 e92f aaf0  ..;.2..Q/..A./..
-00000d50: 4750 e1e1 569e daaf 684f 0558 624c f2b4  GP..V...hO.XbL..
-00000d60: d442 1be4 a074 a05c e42d 8a4a d6df b8a6  .B...t.\.-.J....
-00000d70: 82af 0df7 c69a 4a2e 0ebd b9f3 ebaa 3ddc  ......J.......=.
-00000d80: 931c b4f7 b788 e7d1 b3c9 d335 18fe 7fac  ...........5....
-00000d90: 2ea4 8598 5c88 9102 bd21 4fa1 551c 33aa  ....\....!O.U.3.
-00000da0: 8053 34ac ef0f 0da4 aaa0 ab7b ca70 f4db  .S4........{.p..
-00000db0: db1b 430f 519c 8c1c 4817 10b2 d4a6 8257  ..C.Q...H......W
-00000dc0: 74d4 decb dc9b f254 b0da 8106 866f b6fe  t......T.....o..
-00000dd0: eb74 03bf 6bed 1c74 5a9e 569c 6eb4 a2c2  .t..k..tZ.V.n...
-00000de0: cb76 f418 1690 4ec9 84b8 f32f ed73 fd08  .v....N..../.s..
-00000df0: bbad 91da c942 badb 2ac3 f066 bde0 c725  .....B..*..f...%
-00000e00: 2432 2c7b bc7e e3f1 c768 3df6 0836 06ca  $2,{.~...h=..6..
-00000e10: 7f0f 8bda fa84 ff33 ef08 f83d 4fea e48d  .......3...=O...
-00000e20: 68d3 8883 efd1 a1fb 3aae c06e 24c1 2301  h.......:..n$.#.
-00000e30: 4ea9 20df a719 fee0 c78c 808e 1fe8 a0f5  N. .............
-00000e40: 8e0b c7d5 33c9 0366 d59e e50c 7d35 9d1f  ....3..f....}5..
-00000e50: 199d d0a7 28a0 6ac5 6aba 13ee fe74 98e1  ....(.j.j....t..
-00000e60: f3fa 3dab f84e c223 1b6e 7de4 7bed 3a88  ..=..N.#.n}.{.:.
-00000e70: 0c9f d7ef 7cd5 a3a9 8fc1 5af7 cec2 b380  ....|.....Z.....
-00000e80: 2fda 199e e16f 37cb 37f3 d54d 1107 b370  /....o7.7..M...p
-00000e90: 390b 2697 2c09 e6c9 7215 2493 ebe5 6a55  9.&.,...r.$...jU
-00000ea0: ccc3 38bc fe3e 1a5c ff30 b6ba 390b 058e  ..8..>.\.0..9...
-00000eb0: 260b 2b60 b899 21d9 81fc ddd9 96e1 d1a6  &.+`..!.........
-00000ec0: a7df f53b d01e 739f c7d3 f06d 1285 4171  ...;..s....m..Aq
-00000ed0: 1946 c164 4a67 c16c 7a99 0445 12c5 abe9  .F.dJg.lz..E....
-00000ee0: 6479 9314 c988 7bf2 c2f1 1692 28ea 07a5  dy....{.....(...
-00000ef0: 279f 2c1c 974c 7075 acd5 b142 632b 1409  '.,..Lpu...Bc+..
-00000f00: b6bf 4882 1c2b 41ce 7f62 f90f 0000 00ff  ..H..+A..b......
-00000f10: ff03 0050 4b03 0414 0006 0008 0000 0021  ...PK..........!
-00000f20: 00c1 1710 be4e 0700 00c6 2000 0013 0000  .....N.... .....
-00000f30: 0078 6c2f 7468 656d 652f 7468 656d 6531  .xl/theme/theme1
-00000f40: 2e78 6d6c ec59 cd8b 1b37 14bf 17fa 3f0c  .xml.Y...7....?.
-00000f50: 7377 fc35 e38f 25de e0cf 6c93 dd24 649d  sw.5..%...l..$d.
-00000f60: 941c b5b6 ec51 5633 3292 bc1b 1302 2539  .....QV32.....%9
-00000f70: f552 28a4 a597 426f 3d94 d240 030d bdf4  .R(...Bo=..@....
-00000f80: 8f09 24b4 e91f d127 cdd8 23ad e524 9b6c  ..$....'..#..$.l
-00000f90: 4a5a 760d 8b47 febd a7a7 f79e 7e7a f374  JZv..G......~z.t
-00000fa0: f1d2 bd98 7a47 980b c292 965f be50 f23d  ....zG....._.P.=
-00000fb0: 9c8c d898 24d3 967f 6b38 2834 7c4f 4894  ....$...k8(4|OH.
-00000fc0: 8c11 6509 6ef9 0b2c fc4b db9f 7e72 116d  ..e.n..,.K..~r.m
-00000fd0: c908 c7d8 03f9 446c a196 1f49 39db 2a16  ......Dl...I9.*.
-00000fe0: c508 8691 b8c0 6638 81df 268c c748 c223  ......f8..&..H.#
-00000ff0: 9f16 c71c 1d83 de98 162b a552 ad18 2392  .........+.R..#.
-00001000: f85e 8262 507b 7d32 2123 ec0d 954a 7f7b  .^.bP{}2!#...J.{
-00001010: a9bc 4fe1 3191 420d 8c28 df57 aab1 25a1  ..O.1.B..(.W..%.
-00001020: b1e3 c3b2 4288 85e8 52ee 1d21 daf2 619e  ....B...R..!..a.
-00001030: 313b 1ee2 7bd2 f728 1212 7e68 f925 fde7  1;..{..(..~h.%..
-00001040: 17b7 2f16 d156 2644 e506 5943 6ea0 ff32  ../..V&D..YCn..2
-00001050: b94c 607c 58d1 73f2 e9c1 6ad2 2008 835a  .L`|X.s...j. ..Z
-00001060: 7ba5 5f03 a85c c7f5 ebfd 5abf b6d2 a701  {._..\....Z.....
-00001070: 6834 8295 a6b6 d83a eb95 6e90 610d 50fa  h4.....:..n.a.P.
-00001080: d5a1 bb57 ef55 cb16 ded0 5f5d b3b9 1daa  ...W.U...._]....
-00001090: 8f85 d7a0 547f b086 1f0c bae0 450b af41  ....T.......E..A
-000010a0: 293e 5cc3 879d 66a7 67eb d7a0 145f 5bc3  )>\...f.g...._[.
-000010b0: d74b ed5e 50b7 f46b 5044 4972 b886 2e85  .K.^P..kPDIr....
-000010c0: b56a 77b9 da15 64c2 e88e 13de 0c83 41bd  .jw...d.......A.
-000010d0: 9229 cf51 900d abec 5253 4c58 2237 e55a  .).Q....RSLX"7.Z
-000010e0: 8cee 323e 0080 0252 2449 e2c9 c50c 4fd0  ..2>...R$I....O.
-000010f0: 08b2 b88b 2839 e0c4 db25 d308 126f 8612  ....(9...%...o..
-00001100: 2660 b854 290d 4a55 f8af 3e81 fea6 238a  &`.T).JU..>...#.
-00001110: b630 32a4 955d 6089 581b 52f6 7862 c4c9  .02..]`.X.R.xb..
-00001120: 4cb6 fc2b a0d5 3720 2f9e 3d7b fef0 e9f3  L..+..7 /.={....
-00001130: 87bf 3d7f f4e8 f9c3 5fb2 b9b5 2a4b 6e07  ..=....._...*Kn.
-00001140: 2553 53ee d58f 5fff fdfd 17de 5fbf fef0  %SS..._....._...
-00001150: eaf1 37e9 d427 f1c2 c4bf fcf9 cb97 bfff  ..7..'..........
-00001160: f13a f5b0 e2dc 152f be7d f2f2 e993 17df  .:...../.}......
-00001170: 7df5 e74f 8f1d dadb 1c1d 98f0 2189 b1f0  }..O........!...
-00001180: aee1 63ef 268b 6181 0efb f101 3f9d c430  ..c.&.a.....?..0
-00001190: 42c4 9240 11e8 76a8 eecb c802 5e5b 20ea  B..@..v.....^[ .
-000011a0: c275 b0ed c2db 1c58 c605 bc3c bf6b d9ba  .u.....X...<.k..
-000011b0: 1ff1 b924 8e99 af46 b105 dc63 8c76 1877  ...$...F...c.v.w
-000011c0: 3ae0 aa9a cbf0 f070 9e4c dd93 f3b9 89bb  :......p.L......
-000011d0: 89d0 916b ee2e 4aac 00f7 e733 a057 e252  ...k..J....3.W.R
-000011e0: d98d b065 e60d 8a12 89a6 38c1 d253 bfb1  ...e......8..S..
-000011f0: 438c 1dab bb43 88e5 d73d 32e2 4cb0 89f4  C....C...=2.L...
-00001200: ee10 af83 88d3 2543 7260 2552 2eb4 4362  ......%Cr`%R..Cb
-00001210: 88cb c265 2084 daf2 cdde 6daf c3a8 6bd5  ...e .....m...k.
-00001220: 3d7c 6423 615b 20ea 307e 88a9 e5c6 cb68  =|d#a[ .0~.....h
-00001230: 2e51 ec52 3944 3135 1dbe 8b64 e432 727f  .Q.R9D15...d.2r.
-00001240: c147 26ae 2f24 447a 8a29 f3fa 632c 844b  .G&./$Dz.)..c,.K
-00001250: e63a 87f5 1a41 bf0a 0ce3 0efb 1e5d c436  .:...A.......].6
-00001260: 924b 72e8 d2b9 8b18 3391 3d76 d88d 503c  .Kr.....3.=v..P<
-00001270: 73da 4c92 c8c4 7e26 0e21 4591 7783 4917  s.L...~&.!E.w.I.
-00001280: 7c8f d93b 443d 431c 50b2 31dc b709 b6c2  |..;D=C.P.1.....
-00001290: fd66 22b8 05e4 6a9a 9427 88fa 65ce 1db1  .f"...j..'..e...
-000012a0: bc8c 99bd 1f17 7482 b08b 65da 3cb6 d8b5  ......t...e.<...
-000012b0: cd89 333b 3af3 a995 dabb 1853 748c c618  ..3;:......St...
-000012c0: 7bb7 3e73 58d0 6133 cbe7 b9d1 5722 6095  {.>sX.a3....W"`.
-000012d0: 1dec 4aac 2bc8 ce55 f59c 6001 6592 aa6b  ..J.+..U..`.e..k
-000012e0: d629 7297 082b 65f7 f194 6db0 676f 7182  .)r..+e...m.goq.
-000012f0: 7816 2889 11df a4f9 1a44 dd4a 5d38 e59c  x.(......D.J]8..
-00001300: 547a 9d8e 0e4d e035 02e5 1fe4 8bd3 29d7  Tz...M.5......).
-00001310: 05e8 3092 bbbf 49eb 8d08 5967 977a 16ee  ..0...I...Yg.z..
-00001320: 7c5d 702b 7e6f b3c7 605f de3d edbe 0419  |]p+~o..`_.=....
-00001330: 7c6a 1920 f6b7 f6cd 1051 6b82 3c61 8608  |j. .....Qk.<a..
-00001340: 0a0c 17dd 8288 15fe 5c44 9dab 5a6c ee94  ........\D..Zl..
-00001350: 9bd8 9b36 0f03 1446 56bd 1393 e48d c5cf  ...6...FV.......
-00001360: 89b2 27fc 77ca 1e77 0173 0605 8f5b f1fb  ..'.w..w.s...[..
-00001370: 943a 9b28 65e7 4481 b309 f71f 2c6b 7a68  .:.(e.D.....,kzh
-00001380: 9edc c070 92ac 73d6 7955 735e d5f8 fffb  ...p..s.yUs^....
-00001390: aa66 d35e 3eaf 65ce 6b99 f35a c6f5 f6f5  .f.^>.e.k..Z....
-000013a0: 416a 99bc 7c81 ca26 eff2 e89e 4fbc b1e5  Aj..|..&....O...
-000013b0: 3321 94ee cb05 c5bb 4277 7d04 bcd1 8c07  3!......Bw}.....
-000013c0: 30a8 db51 ba27 b96a 01ce 22f8 9a35 982c  0..Q.'.j.."..5.,
-000013d0: dc94 232d e371 263f 2732 da8f d00c 5a43  ..#-.q&?'2....ZC
-000013e0: 65dd c09c 8a4c f554 7833 26a0 63a4 8775  e....L.Tx3&.c..u
-000013f0: 2b15 9fd0 adfb 4ef3 788f 8dd3 4e67 b9ac  +.....N.x...Ng..
-00001400: ba9a a90b 0592 f978 295c 8d43 974a a6e8  .......x)\.C.J..
-00001410: 5a3d efde add4 eb7e e854 7759 9706 28d9  Z=.....~.TwY..(.
-00001420: d318 614c 661b 5175 1851 5f0e 4214 5e67  ..aLf.Qu.Q_.B.^g
-00001430: 845e d999 58d1 7458 d150 ea97 a15a 4671  .^..X.tX.P...ZFq
-00001440: e50a 306d 1515 78e5 f6e0 45bd e587 41da  ..0m..x...E...A.
-00001450: 4186 661c 94e7 6315 a7b4 99bc 8cae 0ace  A.f...c.........
-00001460: 9946 7a93 33a9 9901 5062 2f33 208f 7453  .Fz.3...Pb/3 .tS
-00001470: d9ba 7179 6a75 69aa bd45 a42d 238c 74b3  ..qyjui..E.-#.t.
-00001480: 8d30 d230 8217 e12c 3bcd 96fb 59c6 ba99  .0.0...,;...Y...
-00001490: 87d4 324f b962 b91b 7233 ea8d 0f11 6b45  ..2O.b..r3....kE
-000014a0: 2227 b881 2626 53d0 c43b 6ef9 b56a 08b7  "'..&&S..;n..j..
-000014b0: 2a23 346b f913 e818 c3d7 7806 b923 d45b  *#4k......x..#.[
-000014c0: 17a2 53b8 7619 499e 6ef8 7761 9619 17b2  ..S.v.I.n.wa....
-000014d0: 8744 943a 5c93 4eca 0631 9198 7b94 c42d  .D.:\.N..1..{..-
-000014e0: 5f2d 7f95 0d34 d11c a26d 2b57 8010 3e5a  _-...4...m+W..>Z
-000014f0: e39a 402b 1f9b 7110 743b c878 32c1 2369  ..@+..q.t;.x2.#i
-00001500: 86dd 1851 9e4e 1f81 e153 ae70 feaa c5df  ...Q.N...S.p....
-00001510: 1dac 24d9 1cc2 bd1f 8d8f bd03 3ae7 3711  ..$.........:.7.
-00001520: a458 582f 2b07 8e89 808b 8372 eacd 3181  .XX/+......r..1.
-00001530: 9bb0 1591 e5f9 77e2 60ca 68d7 bc8a d239  ......w.`.h....9
-00001540: 948e 233a 8b50 76a2 9864 9ec2 3589 aecc  ..#:.Pv..d..5...
-00001550: d14f 2b1f 184f d99a c1a1 eb2e 3c98 aa03  .O+..O......<...
-00001560: f6bd 4fdd 371f d5ca 7306 69e6 67a6 c52a  ..O.7...s.i.g..*
-00001570: ead4 7493 e987 3be4 0dab f243 d4b2 2aa5  ..t...;....C..*.
-00001580: 6efd 4e2d 72ae 6b2e b90e 12d5 794a bce1  n.N-r.k.....yJ..
-00001590: d47d 8b03 c130 2d9f cc32 4d59 bc4e c38a  .}...0-..2MY.N..
-000015a0: b3b3 51db b433 2c08 0c4f d436 f86d 7546  ..Q..3,..O.6.muF
-000015b0: 383d f1ae 273f c89d cc5a 7540 2ceb 4a9d  8=..'?...Zu@,.J.
-000015c0: f8fa cadc bcd5 6607 7781 3c7a 707f 38a7  ......f.w.<zp.8.
-000015d0: 52e8 5042 6f97 2328 fad2 1bc8 9436 608b  R.PBo.#(.....6`.
-000015e0: dc93 598d 08df bc39 272d ff7e 296c 07dd  ..Y....9'-.~)l..
-000015f0: 4ad8 2d94 1a61 bf10 5483 52a1 11b6 ab85  J.-..a..T.R.....
-00001600: 7618 56cb fdb0 5cea 752a 0fe0 6091 515c  v.V...\.u*..`.Q\
-00001610: 0ed3 ebfa 015c 61d0 4576 69af c7d7 2eee  .....\a.Evi.....
-00001620: e3e5 2dcd 8511 8b8b 4c5f cc17 b5e1 fae2  ..-.....L_......
-00001630: be5c d97c 71ef 1120 9dfb b5ca a059 6d76  .\.|q.. .....Ymv
-00001640: 6a85 66b5 3d28 04bd 4ea3 d0ec d63a 855e  j.f.=(..N....:.^
-00001650: ad5b ef0d 7add b0d1 1c3c f0bd 230d 0eda  .[..z....<..#...
-00001660: d56e 50eb 370a b572 b75b 086a 2565 7ea3  .nP.7..r.[.j%e~.
-00001670: 59a8 0795 4a3b a8b7 1bfd a0fd 202b 6360  Y...J;...... +c`
-00001680: e529 7d64 be00 f76a bbb6 ff01 0000 ffff  .)}d...j........
-00001690: 0300 504b 0304 1400 0600 0800 0000 2100  ..PK..........!.
-000016a0: 0b04 22b9 b011 0000 e087 0000 1800 0000  ..".............
-000016b0: 786c 2f77 6f72 6b73 6865 6574 732f 7368  xl/worksheets/sh
-000016c0: 6565 7431 2e78 6d6c 9c93 cb8e db20 1486  eet1.xml..... ..
-000016d0: f795 fa0e 887d 82ed 64dc 192b cea8 cd28  .....}..d..+...(
-000016e0: ea48 5d54 bdae 313e 8e51 c0b8 406e aafa  .H]T..1>.Q..@n..
-000016f0: ee3d e0dc a46c a2b1 6cc0 5cbe ff3f 7098  .=...l..l.\..?p.
-00001700: 3def b522 5bb0 4e9a aea4 e938 a104 3a61  =.."[.N....8..:a
-00001710: 6ad9 ad4a faf3 c772 f448 89f3 bcab b932  j..J...r.H.....2
-00001720: 1d94 f400 8e3e cfdf bf9b ed8c 5dbb 16c0  .....>......]...
-00001730: 1324 74ae a4ad f77d c198 132d 68ee c6a6  .$t....}...-h...
-00001740: 870e 471a 6335 f7f8 6b57 ccf5 1678 1d17  ..G.c5..kW...x..
-00001750: 69c5 b224 c999 e6b2 a303 a1b0 f730 4cd3  i..$.........0L.
-00001760: 4801 2f46 6c34 747e 8058 50dc a37f d7ca  H./Fl4t~.XP.....
-00001770: de9d 685a dc83 d3dc ae37 fd48 18dd 23a2  ..hZ.....7.H..#.
-00001780: 924a fa43 8452 a245 f1ba ea8c e595 c2b8  .J.C.R.E........
-00001790: f7e9 940b b2b7 f866 f84d 4e32 b1ff 4649  .......f.MN2..FI
-000017a0: 4b61 8d33 8d1f 2399 0d9e 6fc3 7f62 4f8c  Ka.3..#...o..bO.
-000017b0: 8b33 e936 febb 30e9 9459 d8ca 7080 1754  .3.6..0..Y..p..T
-000017c0: f636 4be9 c399 955d 6093 37c2 f233 2c6c  .6K....]`.7..3,l
-000017d0: 972d 36b2 2ee9 dfe4 f88c b04e 4391 5c8a  .-6........NC.\.
-000017e0: d3d8 3f3a 9fd5 124f 3844 452c 3425 fd98  ..?:...O8DE,4%..
-000017f0: 168b 2c9b 5036 9fc5 0cfa 2561 e7ae dac4  ..,.P6....%a....
-00001800: f3ea 3b28 101e 5025 a5c4 9bfe 0b34 7e01  ..;(..P%.....4~.
-00001810: 4a85 d579 4e49 c8d9 ca98 7558 fb8a b312  J..yNI....uX....
-00001820: 9471 714d 90e1 c2cb 2d0c f33f a58f b801  .qqM....-..?....
-00001830: ee4f 948e 3fa8 cbce c2d7 ed93 8965 ccf4  .O..?........e..
-00001840: af96 54dc c1c2 a8df b2f6 2d3a c11b 5543  ..T.......-:..UC
-00001850: c337 ca5f 75a2 bf63 e737 b3fb 0c72 d57a  .7._u..c.7...r.z
-00001860: 9c8a 1663 3e15 f5e1 059c c004 478f e32c  ...c>.......G..,
-00001870: c42c 8c42 212c 8996 e1a2 627e f27d ac77  .,.B!,....b~.}.w
-00001880: 83ce 743a 4ef3 6992 670f 9454 e0fc 5206  ..t:N.i.g..T..R.
-00001890: 2225 62e3 bcd1 2733 47d4 00c1 0823 04eb  "%b...'3G....#..
-000018a0: 2324 fd70 2f84 4543 ff01 0000 ffff 0000  #$.p/.EC........
-000018b0: 00ff ff94 9ddd 8e1c b711 855f 45d0 7d5a  ..........._E.}Z
-000018c0: cd9f fe33 e405 b2ab 1759 2802 7ce5 045e  ...3.....Y(.|..^
-000018d0: 414e de3e c519 ee34 0f8b 5d5b 4717 41e0  AN.>...4..][G.A.
-000018e0: 6259 9f7b c873 38cd 3e3d 5fdf fef8 f1e3  bY.{.s8.>=_.....
-000018f0: e7b7 d79f af4f 5fff faf7 df9f fefa fd73  .....O_........s
-00001900: f8fc e9ed 3faf 7fbe c9ff fb2d 7dfe f4df  ....?......-}...
-00001910: 905f bfff f6af ff7d fbf1 f6fd c79f 3f7f  ._.....}......?.
-00001920: ff3c 4ff1 f3d3 d7ef 65e8 3fcb d85b 87fc  .<O.....e.?..[..
-00001930: f337 f9a7 bf9e e6af 5f7e 3d7d fdf2 bd8e  .7......_~=}....
-00001940: 78d6 2302 8e78 d123 e263 c417 617a 8045  x.#..x.#.c..az.E
-00001950: 024c c63e 9052 87d4 d696 8ef7 a5fc b7fd  .L.>.R..........
-00001960: 7afa c709 0908 723d dcd7 46c6 3e10 d6ee  z.....r=..F.>...
-00001970: 3ffa b92d 2a86 6432 6482 41c6 3e18 7277  ?..-*.d2d.A.>.rw
-00001980: 19da dad2 7f28 f986 7071 1516 8240 c65e  .....(..pq...@.^
-00001990: 12b4 b5e5 fcd0 6f53 eb65 b108 5682 40c6  ......oS.e..V.@.
-000019a0: 5e12 b4b5 a59b 272f ab45 b011 0432 f692  ^.....'/.E...2..
-000019b0: a0ad 2ddd 47f4 b259 043b 4120 631f 044b  ..-.G..Y.;A c..K
-000019c0: 370f a0d6 155f 768b e020 0864 ec25 01d4  7...._v.. .d.%..
-000019d0: fa99 7858 0461 66c4 4a06 5f32 947f d359  ..xX.af.J._2...Y
-000019e0: ec27 a354 8b2c 5cac 8740 49a6 0cbe a680  .'.T.,\..@I.....
-000019f0: 623f 21e5 efb1 2818 7d0c 2082 bd66 43b1  b?!...(.}. ..fC.
-00001a00: 9f94 d26a 5130 1219 4023 7b0a d0c8 b577  ...jQ0..@#{....w
-00001a10: 8dbb 485e 7d22 8c48 8656 09bb bfe7 198a  ..H^}".H.V......
-00001a20: 4bbf 3ca4 6a5d 0b46 2843 ab86 8a02 a452  K.<.j].F(C.....R
-00001a30: 39a8 a995 8111 cb32 f874 adfe 1301 b954  9......2.t.....T
-00001a40: 6bc4 d4cb c008 6619 7c4d 0192 a9d6 88a9  k.....f.|M......
-00001a50: 9981 11cd 32f8 9a02 6453 ad11 5337 0323  ....2...dS..S7.#
-00001a60: 9c65 f083 62eb 3f11 90ce aefa 22ad d666  .e..b.?....."..f
-00001a70: 2632 e259 065f 6240 71d9 bba5 2a55 1383  &2.Y._b@q...*U..
-00001a80: 51cf d80a 647f 35a0 b81c 3dc6 5d3d afb6  Q...d.5...=.]=..
-00001a90: 7691 da5e b60a a930 dae2 aa36 98f6 0e33  v..^...0...6...3
-00001aa0: 32fa 5906 3f3e 94ee b23f 4351 2997 54cb  2.Y.?>...?CQ).T.
-00001ab0: 8772 4c31 863c 9f7f ceab 867b 6f46 5063  .rL1.<.....{oFPc
-00001ac0: 2ba8 0acb dc77 4a2b 85c5 286c 6c45 5461  +....wJ+..(llETa
-00001ad0: 999b 5169 a5b0 18c9 8dad aa2a 2c73 872a  ..Qi.......*,s.*
-00001ae0: ad14 16a3 c1b1 9559 8565 6e5b a595 c262  .......Y.en[...b
-00001af0: 4439 b6ba db2d f167 282e fd96 41aa 1416  D9...-.g(...A...
-00001b00: a3d2 b115 6285 052a ddef 21a4 95c1 4a8c  ....b..*..!...J.
-00001b10: 6a97 c10f 81e8 b1a0 a8be 014a 95c2 6254  j..........J..bT
-00001b20: 3cb5 2aae b060 0fdc ef32 a495 c262 543d  <.*..`...2...bT=
-00001b30: b5c2 adb0 6053 dc6f 3ba4 95c2 a26e 24b4  ....`S.o;....n$.
-00001b40: 2aaf b060 97dc ef43 12a7 f289 51f9 32f8  *..`...C....Q.2.
-00001b50: 31b7 427f df07 aaca 7da4 5a2e d736 ade7  1.B.....}.Z..6..
-00001b60: 6ac0 1b2d 8cb0 a756 bb35 89b9 7796 de0f  j..-...V.5..w...
-00001b70: 4818 2d4f ad5c 6b12 73ff 2cbd 1f90 30f2  H.-O.\k.s.,...0.
-00001b80: 9d5a 85d6 24e6 1e5a 7a3f 2061 143b b58a  .Z..$..Zz? a.;..
-00001b90: ad49 cc7d b4f4 7e40 c288 746a 7538 a85b  .I.}..~@..tju8.[
-00001ba0: 72a6 4a4b 6f21 59e5 eee7 b1e6 2ded f1be  r.JKo!Y.....-...
-00001bb0: 673a 8500 e66f 6654 ba0c 3e57 52cf 0555  g:...ofT..>WR..U
-00001bc0: 7da3 ee2e d36e 2e46 a673 abc4 ea7a 4155  }....n.F.s...zAU
-00001bd0: ddbe 932a 75bd 189d cead 146b 2e53 a8a5  ...*u......k.S..
-00001be0: 97e2 6284 3ab7 5aac b94c a596 5e8a 8bba  ..b.:.Z..L..^...
-00001bf0: 0b0c 4add 39ea 7386 0d79 bf3b 916a e18a  ..J.9.s..y.;.j..
-00001c00: 6b9a ceef 3938 d519 a9ce 20d5 0ac5 946a  k...98.... ....j
-00001c10: e9fd 0885 d1ea 0c5a ad50 4cad 96de 8f50  .......Z.PL....P
-00001c20: 18b1 ce20 d60a c514 6be9 fd08 8551 eb0c  ... ....k....Q..
-00001c30: 6aad 504c b596 de8f 5018 b9ce 20d7 fd29  j.PL....P... ..)
-00001c40: 0e54 d506 43aa 0525 6d61 9ef2 b6ef e138  .T..C..%ma.....8
-00001c50: bf0d c0ec 5d18 a12e 834f a1ee 89a0 aa84  ....]....O......
-00001c60: 5aaa 4e22 46a2 1790 6845 646e a5a5 d749  Z.N"F...hEdn...I
-00001c70: c488 f302 e2ac 884c 7196 5e27 1123 cb0b  .......Lq.^'.#..
-00001c80: c8b2 2232 6559 7a9d 448c 202f 20c8 fdc1  .."2eYz.D. / ...
-00001c90: 1c54 d5cc 966a 215a b66d dab6 3586 18d3  .T...j!Z.m..5...
-00001ca0: 51fe 5c6c a417 eab0 0ed4 5971 99ea 2c7f  Q.\l......Yq..,.
-00001cb0: 11c5 c548 f502 52ad b84c a996 5e8a 8bd1  ...H..R..L..^...
-00001cc0: ed05 745b 7199 ba2d bd14 1723 e20b 88b8  ..t[q..-...#....
-00001cd0: e232 455c 7a29 2e46 d117 50f4 fe20 12aa  .2E\z).F..P.. ..
-00001ce0: 7ade d70d f891 c394 f31e 53ba 9af2 2b23  z.........S...+#
-00001cf0: e965 f029 e93d 1254 95a4 4bf5 b667 7320  .e.).=.T..K..gs 
-00001d00: 319a be82 a62b 2453 d3a5 d78b c488 fa0a  1....+$S........
-00001d10: a2ae 904c 5197 5e2f 12a3 ea2b a8ba 4232  ...LQ.^/...+..B2
-00001d20: 555d 7abd 488c acaf 20eb fd19 1e54 d5f4  U]z.H... ....T..
-00001d30: 96ea 0d29 efc7 746c fbbc c6b4 1759 bfd8  ...)..tl.....Y..
-00001d40: b6ac 8cac 97c1 e71c 575c a6ac 4b2f c5c5  ........W\..K/..
-00001d50: c8fa 0ab2 aeb8 4c59 975e 8a8b 91f5 1564  ......LY.^.....d
-00001d60: 5d71 99b2 2ebd 1417 23eb 2bc8 bae2 3265  ]q......#.+...2e
-00001d70: 5d7a 292e 46d6 5790 f5fe 380c aa7a dedf  ]z).F.W...8..z..
-00001d80: 653d 2e79 9fe6 f9d8 9663 ddca 9d95 8b67  e=.y.....c.....g
-00001d90: c036 46db cbe0 73de f75c 5055 da2e d572  .6F...s..\PU...r
-00001da0: bddc 5c8c c06f 20f0 8acb 1478 e9a5 b818  ..\..o ....x....
-00001db0: 95df 40e5 1597 a9f2 d24b 7131 52bf 81d4  ..@......Kq1R...
-00001dc0: 2b2e 53ea a597 e262 f47e 03bd efcf c8a0  +.S....b.~......
-00001dd0: aae6 bd54 6fdb ac79 99d6 e388 f376 dc4f  ...To..y.....v.O
-00001de0: 612f 1e68 d918 bd2f 83cf 79af b84c bd97  a/.h.../..y..L..
-00001df0: 5e8a 8bd1 fb0d f45e 7199 7a2f bd14 17a3  ^......^q.z/....
-00001e00: f71b e8bd e232 f55e 7a29 2e46 ef37 d07b  .....2.^z).F.7.{
-00001e10: c565 eabd f452 5c8c de6f a0f7 fd89 1454  .e...R\..o.....T
-00001e20: f5bc af37 66a6 34c7 2013 ffe2 a6e2 cee8  ...7f.4. .......
-00001e30: 7c19 7cce f79e 07aa 4ae7 a55a ae53 fa88  |.|.....J..Z.S..
-00001e40: 87d1 f71d f45d f198 fa2e bd2e 1e46 d777  .....].......F.w
-00001e50: d075 c563 eaba f4ba 7818 3ddf 41cf 158f  .u.c....x.=.A...
-00001e60: a9e7 d2eb e261 747c 6f75 3cf6 2799 5055  .....at|ou<.'.PU
-00001e70: f359 aa85 67db 4298 8e25 8779 4da2 e7f2  .Y..g.B..%.yM...
-00001e80: 67fc 0cfb cee8 7819 fc98 d79a cbd4 71e9  g.....x.......q.
-00001e90: a5b8 181d df5b a5d6 5ca6 8e4b 2fc5 c5e8  .....[..\..K/...
-00001ea0: f8de 2ab5 e632 755c 7a29 2e46 c7f7 56a9  ..*..2u\z).F..V.
-00001eb0: 3597 a9e3 d24b 7131 3abe b73a 1efb 7347  5....Kq1:..:..sG
-00001ec0: a8ea 797f d7f1 658e 695a d6b0 a71c a2f1  ..y...e.iZ......
-00001ed0: 7df5 60f4 bc0c 3ee7 7dcf 0555 a5e7 52bd  }.`...>.}..U..R.
-00001ee0: fb9e 938b d1f5 a355 6e75 bda0 aace 43a5  .......Unu....C.
-00001ef0: 4a71 31fa 7eb4 0aae b94c 7d97 5e8a 8bd1  Jq1.~....L}.^...
-00001f00: f9a3 5572 cd65 eabc f452 5c8c de1f a0f7  ..Ur.e...R\.....
-00001f10: fd19 1754 d5bc 976a e18a 4790 dbef 73cc  ...T...j..G...s.
-00001f20: c79e 6e0f 025c ecdb 0f46 efcb e073 de2b  ..n..\...F...s.+
-00001f30: 2e53 efa5 97e2 62f4 fe00 bd57 5ca6 de4b  .S....b....W\..K
-00001f40: 2fc5 c5e8 fd01 7aaf b84c bd97 5e8a 8bd1  /.....z..L..^...
-00001f50: fb03 f45e 7199 7a2f bd14 17a3 f707 e87d  ...^q.z/.......}
-00001f60: 7f10 0655 3def 6b0e 67df e440 35c9 ff86  ...U=.k.g..@5...
-00001f70: e6f9 4a38 510d 33a3 f5b7 d1e7 a4ef a1b0  ..J8Q.3.........
-00001f80: acd4 be94 cbe5 0a1e 2c46 eac3 0c5a afb1  ........,F...Z..
-00001f90: cc4d 7ce9 7663 314a 1f66 907a 8d65 6a7d  .M|.vc1J.f.z.ej}
-00001fa0: e976 6331 421f 6650 7a8d 654a 7de9 7663  .vc1B.fPz.eJ}.vc
-00001fb0: 313a 1f66 10fa fe1c 0ccb 3adb 23dd 370b  1:.f......:.#.7.
-00001fc0: da97 639a b36c f0c3 b695 2dce f945 bc9b  ..c..l....-..E..
-00001fd0: f78c d687 19c4 5eb3 996a 5fba 3936 46ef  ......^..j_.96F.
-00001fe0: e54b 4c6b 449a cd54 fcd2 cdb1 319a 1f66  .KLkD..T....1..f
-00001ff0: 107d cd66 aa7e e9e6 d818 dd0f 3308 bf66  .}.f.~......3..f
-00002000: 3395 bf74 736c 8cf6 8719 c4bf 3f2f c3f2  3..tsl......?/..
-00002010: 602d dce5 7f8f f235 37ce 695d 43b8 3f76  `-.....57.i]C.?v
-00002020: 30fe 9a1b b860 2684 2fa3 62c3 6ca6 4abf  0....`&./.b.l.J.
-00002030: d570 a69f 8d32 8212 ee3c fd49 b3d9 4650  .p...2...<.I..FP
-00002040: 239b 7e36 ca0d 20c5 39b8 6eb6 1bd4 20a7  #.~6.. .9.n... .
-00002050: 9f8d b204 c876 0ed8 6c4b 90ee b216 fc6c  .....v..lK.....l
-00002060: 942f 40a8 33aa b0e5 0799 cf1a fa5c e723  ./@.3........\.#
-00002070: 4f65 296c fb76 5b0b 57be 5092 9dfe 372a  Oe)l.v[.W.P...7*
-00002080: 400e 74c0 66fb 8274 97eb e667 a37c 01d2  @.t.f..t...g.|..
-00002090: a103 36db 17a4 9b63 a37c 0132 a303 36db  ..6....c.|.2..6.
-000020a0: 17a4 9b63 a37c 0192 a403 36db 17a4 9b63  ...c.|....6....c
-000020b0: a37c 01f2 a56b ff65 2540 59fb 428d 98a6  .|...k.e%@Y.B...
-000020c0: 8bc7 e003 9531 bd8d 7e68 ad66 c198 a9f2  .....1..~h.f....
-000020d0: 819a 33bd 66a1 741f c2a4 0316 5bf7 a5bb  ..3.f.t.....[...
-000020e0: 7c66 d72c 94ce 976c aa75 5d6c 9d97 6e9b  |f.,...l.u]l..n.
-000020f0: 85d2 7588 950e ae8b adeb 3576 7a7d 5d28  ..u.......5vz}](
-00002100: 1d87 a069 7394 747b 83c8 7380 b27a b946  ...is.t{..s..z.F
-00002110: 29df 3c26 4f6b 1380 9587 102e f634 253f  ).<&Ok.......4%?
-00002120: ead7 7148 9bc6 fef0 2e40 59af ab1a 38dd  ..qH.....@Y...8.
-00002130: 2520 b5ec b33c ef56 092f 9ef2 0c25 444a  % ...<.V./...%DJ
-00002140: b0c1 fe5e b381 8eeb 7576 d771 3f1b a5e3  ...^....uv.q?...
-00002150: 903b 1d5c 37d0 71f5 0e82 1a3d f5b3 513a  .;.\7.q....=..Q:
-00002160: 0ef9 d201 1be8 b87a 3341 cd9f fad9 281d  .......z3A....(.
-00002170: 8704 ea80 addd fe0f d642 dddf 7be7 1b95  .........B..{...
-00002180: 420d 9034 8dfd 811f 96f5 5aa8 49d4 bcc8  B..4......Z.I...
-00002190: a371 fbbc 8718 96c3 7844 2894 74a9 7f2d  .q......xD(.t..-
-000021a0: 4016 75c0 063a afd6 428d a3fa d928 dd87  @.u..:..B....(..
-000021b0: 40ea 800d 745f ad85 9a49 f5b3 513e 20d1  @...t_...I..Q> .
-000021c0: d2e6 7b91 fe4c c107 d45a a8c1 543f 1be5  ..{..L...Z..T?..
-000021d0: 0b10 3e1d 5c37 483c a977 77d4 70aa 9f8d  ..>.\7H<.ww.p...
-000021e0: f205 08ab 26f5 ba34 280f d642 3dd6 153f  ....&..4(..B=..?
-000021f0: 90e3 e635 1cf7 af1e 97f7 a44a 2095 580b  ...5.......J .X.
-00002200: adf0 0fd8 6c5f 780f b0ba d928 5f80 40eb  ....l_x....(_.@.
-00002210: 80cd f685 f748 ab9b 8df2 0588 b80e d86c  .....H.........l
-00002220: 5f78 0fb9 bad9 285f 80d0 eb80 cdf6 851a  _x....(_........
-00002230: 7b95 0792 7df3 8dca bdca 8b47 1a0d 49fd  {...}......G..I.
-00002240: 412f 96f5 5a90 eedb fdb2 b8cf 93dc d89b  A/..Z...........
-00002250: f3b2 c813 45c7 71f1 4851 2881 55ff 5a80  ....E.q.HQ(.U.Z.
-00002260: 78eb 80cd f685 1a7f 5ddc 6c94 2f40 0076  x.......].l./@.v
-00002270: c066 fb42 8dc0 fad9 285f 8010 ec80 cdf6  .f.B....(_......
-00002280: 851a 83f5 b351 be00 51d7 019b ed0b 350a  .....Q..Q.....5.
-00002290: eb67 a37c 0192 b149 7d0f 87f2 602d d457  .g.|...I}...`-.W
-000022a0: 80cd bb04 75c3 362f 6b0a a7b1 e139 4509  ....u.6/k....9E.
-000022b0: be12 eb00 3c41 73d9 9e50 83b2 726f dbc1  ....<As..P..ro..
-000022c0: 45f9 0164 6607 d7cb f683 9a9a f571 515e  E..df........qQ^
-000022d0: 0001 da01 97ed 0535 42eb e3a2 7c00 f2b2  .......5B...|...
-000022e0: 032e db07 6a9e d6c5 4545 6a03 a466 9bfb  ....j...EEj..f..
-000022f0: 02f5 3b3c 866a d5fb f7de 53b5 519e c6c8  ..;<.j....S.Q...
-00002300: 21ac f9f6 ecdd f519 5dc9 cbfa e73e a46b  !.......]....>.k
-00002310: 076c b607 bce7 6bdd 6c94 0740 ce76 c066  .l....k.l..@.v.f
-00002320: 7bc0 7bd2 d6cd 4679 0024 6e07 6cb6 07bc  {.{...Fy.$n.l...
-00002330: 676e dd6c 9407 40ba 76c0 667b 404d df26  gn.l..@.v.f{@M.&
-00002340: 371b e501 25ac fbb8 cf97 d4f9 2194 b507  7...%.......!...
-00002350: d404 ae6c 85e4 6022 a645 363c fbd5 bdac  ...l..`".E6<....
-00002360: 92a8 25d6 0178 80e6 b23d a026 707d 5c94  ..%..x...=.&p}\.
-00002370: 0740 fe76 70bd 6c0f a809 5c1f 17e5 0190  .@.vp.l...\.....
-00002380: bf1d 70d9 1e50 13b8 3e2e ca03 2061 3be0  ..p..P..>... a;.
-00002390: b23d 40ba 6f8f 6978 e617 95c1 0d10 b34d  .=@.o.ix.......M
-000023a0: ea8c 1553 b8ca 036a 0c77 c971 da53 9ac3  ...S...j.w.q.S..
-000023b0: 91ef 519a abfd 4fc9 d7fa e73e a471 076c  ..Q...O....>.q.l
-000023c0: b607 d43c ae9f 8df2 0088 e50e d86c 0fa8  ...<.........l..
-000023d0: c15c 3f1b e501 90cf 1db0 d91e 5013 ba7e  .\?.........P..~
-000023e0: 36ca 0320 8a3b 60b3 3da0 4675 fd6c 9407  6.. .;`.=.Fu.l..
-000023f0: 4058 37a9 b369 286b 0fa8 71dd 9853 9e8e  @X7..i(k..q..S..
-00002400: b4ca a34b d97c 66a9 4470 89b5 003e a0d9  ...K.|f.Dp...>..
-00002410: 6c1f a891 5d3f 1be5 0510 da1d 5c37 db0b  l...]?......\7..
-00002420: 6a6c d7cf 46f9 0104 7707 6cb6 1fd4 e8ae  jl..F...w.l.....
-00002430: 9f8d f204 88e7 0ed8 6c4f 90ee e209 6e36  ........lO....n6
-00002440: 2abf 2bdf 63db fd90 7af9 3126 7895 2fd4  *.+.c...z.1&x./.
-00002450: 08ef ee3d df2b b15c ff5a 8010 6fd2 6cb6  ...=.+.\.Z..o.l.
-00002460: 2fd4 18af 9f8d f205 08f2 0ed8 6c5f a851  /...........l_.Q
-00002470: 5e3f 1be5 0b10 e61d b0d9 be50 e3bc 7e36  ^?.........P..~6
-00002480: ca17 20b2 3b60 b37d a146 7afd 6c94 2f40  .. .;`.}.Fz.l./@
-00002490: a837 a933 5b28 ab57 df86 1aeb f5b3 51be  .7.3[(.W......Q.
-000024a0: 00c1 de01 1bf8 825e a7f5 3cd9 bd4e 295f  .......^..<..N)_
-000024b0: 8070 ef80 0d7c 419d efd5 78af ffba 51be  .p...|A...x...Q.
-000024c0: 0001 df01 1bf8 823a dfab 115f 3f1b e50b  .......:..._?...
-000024d0: 10e3 1db0 812f e8b7 f0d7 f364 ef67 4ae5  ...../.....d.gJ.
-000024e0: 7d03 447a 351b 267e d5f9 5e8d fcba af5b  }.Dz5.&~..^....[
-000024f0: 89f3 fa7d 01c2 bf49 9d8b 4259 efdf 6afc  ...}...I..BY..j.
-00002500: 37e7 495e 5a37 cb7b ebe6 fb0d adab 338d  7.I^Z7.{......3.
-00002510: 12ed 25d8 5ae1 1fb0 812f a8b5 50a3 c07e  ..%.Z..../..P..~
-00002520: 36ca 1720 143c 6003 5f50 6ba1 c682 fd6c  6.. .<`._Pk....l
-00002530: 942f 4004 78c0 06be a0d6 428d 08fb d928  ./@.x.....B....(
-00002540: 5f80 90f0 800d 9e17 d56b e17e 6ee0 67a3  _........k.~n.g.
-00002550: 7c01 82c2 599d 7543 79b0 1648 5f28 f15f  |...Y.uCy..H_(._
-00002560: 622d b4c2 3f60 b37d a1c6 85fd 1a42 f902  b-..?`.}.....B..
-00002570: 0486 076c b62f d4c8 b09f 8df2 0588 050f  ...l./..........
-00002580: d86c 5f90 6eea 993b 2a37 1c20 1aac d930  .l_.n..;*7. ...0
-00002590: 39ac d642 8d0e bbaf 5b09 fcfa e71b c483  9..B....[.......
-000025a0: b33a ebc6 f4b0 da23 d5f8 70ca 4227 39eb  .:.....#..p.B'9.
-000025b0: 286f 7ebc bd1e ecea fe6e 8904 136c adf0  (o~......n...l..
-000025c0: 0fd8 6c5f a811 623f 1be5 0b10 221e b0d9  ..l_..b?...."...
-000025d0: be50 63c4 7e36 ca17 202a 3c60 b37d a146  .Pc.~6.. *<`.}.F
-000025e0: 89fd 6c94 2f40 9878 c066 fb42 8d13 fbd9  ..l./@.x.f.B....
-000025f0: 285f 8040 7156 67ca 50d6 be50 23c5 79df  (_.@qVg.P..P#.y.
-00002600: 96f2 26c8 1c37 79f8 43fe 5cdd ef2d 3161  ..&..7y.C.\..-1a
-00002610: 622d 802f 6836 db17 6aac d8cf 46f9 0204  b-./h6..j...F...
-00002620: 8b07 d7cd f685 1a2d f6b3 51be 00f1 e101  .......-..Q.....
-00002630: 9bed 0bd2 5d7c c1cb 262f df27 3ed3 dbe8  ....]|..&/.'>...
-00002640: c7b9 9a62 c3b2 7a36 b694 3936 c617 2204  ...b..z6..96..".
-00002650: 8d73 1f9d c5b2 5a0b a57c cb86 ecc7 3ee5  .s....Z..|....>.
-00002660: 78c8 7b23 f3ed f533 17df 1762 c90f bbd7  x.{#...3...b....
-00002670: c26d f479 dd34 9be9 0ba5 9b63 637c 4142  .m.y.4.....cc|AB
-00002680: 88cd bdc1 c175 337d a174 736c 8c2f 44c8  .....u3}.tsl./D.
-00002690: 1d0f d84c 5f28 dd1c 1be3 0b11 72c7 0336  ...L_(......r..6
-000026a0: d317 4a37 c7c6 f842 84dc 71ee cf99 b13c  ..J7...B..q....<
-000026b0: 580b f507 08e7 3dae f2a0 f8b1 1d71 59c4  X.....=......qY.
-000026c0: 172e 5ecd 21ef dca3 d602 f882 6633 7da1  ..^.!.......f3}.
-000026d0: fc5d f7b3 532f 1be3 0b11 72c7 83eb 66fa  .]..S/....r...f.
-000026e0: 42e9 e6d8 185f 8890 3b1e b099 be50 ba29  B...._..;....P.)
-000026f0: 362a 771c 2158 acd9 3077 dc7f 5f28 dd1c  6*w.!X..0w.._(..
-00002700: 1be5 0b90 3bce fd99 b8e4 b01b f953 3f5d  ....;........S?]
-00002710: 5cca 37b6 f5ea 573b e4c5 f1cc ec87 a471  \.7...W;.......q
-00002720: ee4f fe6e ffb2 8751 e895 f9fe 93b1 71db  .O.n...Q......q.
-00002730: f6e9 c872 e5e6 b564 aeae 5666 c90e fb5d  ...r...d..Vf...]
-00002740: 0a92 c603 3670 82fe ae56 ac49 e3e0 66a3  ....6p...V.I..f.
-00002750: 9c00 a2c4 0336 7082 feae 96fc 32e3 fd53  .....6p.....2..S
-00002760: 74b3 514e 0049 e301 1b38 417f 574b 4238  t.QN.I...8A.WKB8
-00002770: 241b e504 9034 1eb0 c189 825e 99d5 09dc  $....4.....^....
-00002780: d78d 7202 481a 67fd 23a4 e004 faba d5a4  ..r.H.g.#.......
-00002790: 71ca cb94 f291 e497 a4ac 1706 46ea 276b  q...........F.'k
-000027a0: 6fa3 cf1d 9bfa d946 0822 0fd6 6975 824d  o......F."..iu.M
-000027b0: 1ea3 9c8e 597e 5f22 2fb2 56af d729 e504  ....Y~_"/.V..)..
-000027c0: 1025 ce9a 0d9c 40af d3ea 045e 36ee d76d  .%....@....^6..m
-000027d0: 215a acd9 3079 acd6 694d 1e07 371b e504  !Z..0y..iM..7...
-000027e0: 9044 1eb0 d94e 5093 c87e 36ca 1720 993c  .D...NP..~6.. .<
-000027f0: 6083 6f08 6a9d d664 b29f 8df2 0548 2ae7  `.o.j..d.....H*.
-00002800: fe24 467e 37c5 74d0 9a54 564f d17f 79fb  .$F~7.t..TVO..y.
-00002810: e3c7 8f9f df5e 7fbe 3efd 1f00 00ff ff00  .....^..>.......
-00002820: 0000 ffff b229 484c 4ff5 4d2c 4acf cc2b  .....)HLO.M,J..+
-00002830: 56c8 494d 2bb1 5532 d033 5752 28ca 4ccf  V.IM+.U2.3WR(.L.
-00002840: 80b1 4bf2 0bc0 a2a6 4a0a 49f9 2525 f9b9  ..K.....J.I.%%..
-00002850: 305e 466a 624a 6a11 8867 aca4 9096 9f5f  0^FjbJj..g....._
-00002860: 02e3 e8db d9e8 97e7 1765 1767 a4a6 96d8  .........e.g....
-00002870: 0100 0000 ffff 0300 504b 0304 1400 0600  ........PK......
-00002880: 0800 0000 2100 91d7 54d3 4403 0000 720b  ....!...T.D...r.
-00002890: 0000 1400 0000 786c 2f73 6861 7265 6453  ......xl/sharedS
-000028a0: 7472 696e 6773 2e78 6d6c 9456 4d73 9b30  trings.xml.VMs.0
-000028b0: 10bd 77a6 ff41 c3b5 100c 76d2 8ec7 760e  ..w..A....v...v.
-000028c0: 6e33 b9f4 63d2 8fbb 0c6b d004 242a 8934  n3..c....k..$*.4
-000028d0: fef7 5d09 07b0 3038 194e 48bb 6fdf ae56  ..]...08.NH.o..V
-000028e0: abb7 ba7d 2e0b f204 5231 c1d7 5e74 35f3  ...}....R1..^t5.
-000028f0: 08f0 44a4 8c67 6bef f7af bbe0 9347 94a6  ..D..gk......G..
-00002900: 3ca5 85e0 b0f6 0ea0 bcdb cdfb 772b a534  <...........w+.4
-00002910: 415f aed6 5eae 75b5 0c43 95e4 5052 7525  A_..^.u..C..PRu%
-00002920: 2ae0 b8b3 17b2 a41a 7f65 16aa 4a02 4d55  *........e..J.MU
-00002930: 0ea0 cb22 8c67 b39b b0a4 8c7b 2411 35d7  ...".g.....{$.5.
-00002940: 6b6f b1f8 e891 9ab3 bf35 6c9b 959b b9b7  ko.......5l.....
-00002950: 5929 b659 e90d a725 ac42 bd59 85e6 bf59  Y).Y...%.B.Y...Y
-00002960: 4ba8 864c 4806 cadd a1a5 0170 57b7 54ee  K..LH......pW.T.
-00002970: 0427 2913 cf2c 059f 304e 2893 97ac b8e0  .')..,..0N(.....
-00002980: c15e 28c5 8a4b 96af b492 a224 4ab0 8208  .^(..K.....$J...
-00002990: 4976 4c60 b514 5657 248f 97f0 b578 935f  IvL`..VW$....x._
-000029a0: 29f8 31d1 4962 3db3 b732 eb5c 278a 9417  ).1.Ib=..2.\'...
-000029b0: 420a d307 6e7a 9f19 675a 8a0c 3879 0172  B...nz..gZ..8y.r
-000029c0: 4dbe e89c 723c a9c8 375f 1c68 d092 ee8b  M...r<..7_.h....
-000029d0: 1a11 039f dcdf 6d83 68be a093 5e81 962c  ......m.h...^..,
-000029e0: b11c 8cc7 d6b8 2c66 173d 4e63 2ce6 9331  ......,f.=Nc,..1
-000029f0: 9057 1b03 591a 9e92 b508 3664 349f 0819  .W..Y.....6d4...
-00002a00: a42f 0ca3 a00b dc50 8d76 d38e a744 afe3  ./.....P.v...D..
-00002a10: 09a2 7117 671c b367 644b 3e28 7a93 ce62  ..q.g..gdK>(z..b
-00002a20: 1421 3816 1bbd 319e 9b4e 3c9a 8e29 5b57  .!8...1..N<..)[W
-00002a30: 0773 de27 556c 4e2e 1e2d 63dc 8b7b ae55  .s.'UlN..-c..{.U
-00002a40: 2ced 7894 7643 1a67 96ee daab c9f4 7a2c  ,.x.vC.g......z,
-00002a50: d31c 9e9d 568c 6ec6 6c4f 816d dfc6 03e0  ....V.n.lO.m....
-00002a60: af60 bbdd c538 2efb 6487 d7d3 b6bd 99c2  .`...8..d.......
-00002a70: 249a cda2 69d3 26a7 fe19 348e 7174 c1b1  $...i.&...4.qt..
-00002a80: dfbd f78d cf7c 22d8 308e a95c 1c8f b26b  .....|".0..\...k
-00002a90: 1c06 7764 70b6 6de6 6d5f 981b bc0d e683  ..wdp.m.m_......
-00002aa0: fb3b b0ec 65dd 9cfc 2899 17ec d34e 8dc7  .;..e...(....N..
-00002ab0: 4bd4 2f28 e639 1fcf f3fc d86d b9ee 5f3d  K./(.9.....m.._=
-00002ac0: 6e5b 1733 27db 61f6 100c 0759 6b39 3e90  n[.3'.a....Yk9>.
-00002ad0: 5b13 3b4c 7b68 d178 594f e7ee 038e d0d1  [.;L{h.xYO......
-00002ae0: 7ab6 a3d0 1980 530e 2743 6c78 c7bf e133  z.....S.'Clx...3
-00002af0: c112 621f 3317 c6ec d927 c462 e0b3 ee1a  ..b.3....'.b....
-00002b00: fc00 d9c0 db3b c807 fb3f eb62 5f4b d2de  .....;...?.b_K..
-00002b10: e633 107f be6f 7df2 240a aa59 01f8 6a67  .3...o}.$..Y..jg
-00002b20: 9423 9d44 9415 aa8c 54f9 285a 5405 09db  .#.D....T.(ZT...
-00002b30: 3348 719b 658c bb2c 38d5 b5a4 0591 a044  3Hq.e..,8......D
-00002b40: 2d13 582e cf8b 0fd4 23cb 6521 fe81 4449  -.X.....#.e!..DI
-00002b50: 20a9 16aa ca41 02f9 40ea aac2 454c b63a   ....A..@...EL.:
-00002b60: aeb9 21ac ab39 f65a eea8 5536 4660 d826  ..!..9.Z..U6F`.&
-00002b70: cb59 961b 0197 3c0e 9592 09d8 e37f 16b5  .Y....<.........
-00002b80: 434c 0aa1 80a0 10c9 a4c9 fdac 35d2 2795  CL..........5.'.
-00002b90: a86a 532f 23b7 802b a60f 3ec1 a995 e10b  .jS/#..+..>.....
-00002ba0: 3e14 0296 39e3 a910 0331 6674 d272 4933  >...9....1ft.rI3
-00002bb0: 3cff bab0 2574 4336 16a8 2f00 0b76 38bf  <...%tC6../..v8.
-00002bc0: 8bd8 35ee 323a 9070 8df7 44fe ae66 ecee  ..5.2:.p..D..f..
-00002bd0: 95df 1e26 b682 9490 986c ddf8 f787 d4b6  ...&.....l......
-00002be0: 67b7 1ea2 66de fc07 0000 ffff 0300 504b  g...f.........PK
-00002bf0: 0304 1400 0600 0800 0000 2100 3abe f890  ..........!.:...
-00002c00: 5a01 0000 7102 0000 1100 0801 646f 6350  Z...q.......docP
-00002c10: 726f 7073 2f63 6f72 652e 786d 6c20 a204  rops/core.xml ..
-00002c20: 0128 a000 0100 0000 0000 0000 0000 0000  .(..............
-00002c30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002c40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002c50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002c60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002c70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002c80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002c90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002ca0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002cb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002cc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002cd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002ce0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002cf0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002d00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002d10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002d20: 0000 0000 007c 9251 4fc3 2014 85df 4dfc  .....|.QO. ...M.
-00002d30: 0f0d ef2d a573 3a49 db25 ceec c946 13b7  ...-.s:I.%...F..
-00002d40: 687c 2370 bb11 5b68 80d9 eddf 4bbb ad76  h|#p..[h....K..v
-00002d50: d1f8 c83d 878f 736e 48e7 fbba 0abe c058  ...=..snH......X
-00002d60: a955 8648 14a3 0014 d742 aa4d 86d6 ab65  .U.H.....B.M...e
-00002d70: 3843 8175 4c09 5669 0519 3a80 45f3 fcfa  8C.uL.Vi..:.E...
-00002d80: 2ae5 0de5 dac0 8bd1 0d18 27c1 069e a42c  *.........'....,
-00002d90: e54d 86b6 ce35 1463 cbb7 5033 1b79 87f2  .M...5.c..P3.y..
-00002da0: 62a9 4dcd 9c3f 9a0d 6e18 ff64 1bc0 491c  b.M..?..n..d..I.
-00002db0: dfe2 1a1c 13cc 31dc 01c3 6620 a213 52f0  ......1...f ..R.
-00002dc0: 01d9 ec4c d503 04c7 5041 0dca 594c 2282  ...L....PA..YL".
-00002dd0: 7fbc 0e4c 6dff bcd0 2b23 672d dda1 f19d  ...Lm...+#g-....
-00002de0: 4e71 c76c c18f e2e0 de5b 3918 dbb6 8dda  Nq.l.....[9.....
-00002df0: 491f c3e7 27f8 bd78 7aed ab86 5275 bbe2  I...'..xz...Ru..
-00002e00: 80f2 5470 ca0d 30a7 4dbe d81a 6983 62e7  ..Tp..0.M...i.b.
-00002e10: a04a f168 deed b062 d615 7edd a504 f170  .J.h...b..~....p
-00002e20: c80b c98d b6ba 74c1 7359 4a0e c1da 8249  ......t.sYJ....I
-00002e30: f16f a3e7 f775 8e8f 8008 7c40 7aac 7356  .o...u....|@z.sV
-00002e40: de26 8bc7 d512 e549 9c90 304e c224 59c5  .&.....I..0N.$Y.
-00002e50: 333a 2574 7aff d1e5 b8b8 df05 3e0e ea53  3:%tz.......>..S
-00002e60: 9aff 8993 30be 09c9 ac23 9298 4eef 46c4  ....0....#..N.F.
-00002e70: 3320 ef73 5f7e 92fc 1b00 00ff ff03 0050  3 .s_~.........P
-00002e80: 4b03 0414 0006 0008 0000 0021 00e4 ee61  K..........!...a
-00002e90: 559b 0100 0033 0300 0010 0008 0164 6f63  U....3.......doc
-00002ea0: 5072 6f70 732f 6170 702e 786d 6c20 a204  Props/app.xml ..
-00002eb0: 0128 a000 0100 0000 0000 0000 0000 0000  .(..............
+000008f0: 4b03 0414 0006 0008 0000 0021 002e b1ce  K..........!....
+00000900: 08bd 0300 006e 0900 000f 0000 0078 6c2f  .....n.......xl/
+00000910: 776f 726b 626f 6f6b 2e78 6d6c ac55 5b6f  workbook.xml.U[o
+00000920: a338 147e 5f69 ff03 8bfa 4a8d 0997 0435  .8.~_i....J....5
+00000930: 1991 1076 2a35 a32a cdb4 bb4f 9103 4eb0  ...v*5.*...O..N.
+00000940: 0a98 35a6 4935 9aff bec7 1072 99ac 56d9  ..5.I5.....r..V.
+00000950: cea2 c4c6 173e 7fe7 9cef 1cdf 7dda e599  .....>......}...
+00000960: f646 45c5 7831 d4f1 ada9 6bb4 8879 c28a  .FE.x1....k..y..
+00000970: cd50 ffba 888c beae 5592 1409 c978 4187  .P......U....xA.
+00000980: fa3b adf4 4fa3 5f7f b9db 72f1 bae2 fc55  .;..O._...r....U
+00000990: 0380 a21a eaa9 94a5 8f50 15a7 3427 d52d  .........P..4'.-
+000009a0: 2f69 012b 6b2e 7222 6128 36a8 2a05 2549  /i.+k.r"a(6.*.%I
+000009b0: 9552 2af3 0c59 a6e9 a29c b042 6f11 7c71  .R*..Y.....Bo.|q
+000009c0: 0d06 5faf 594c 431e d739 2d64 0b22 6846  .._.YLC..9-d."hF
+000009d0: 24d0 af52 5656 1d5a 1e5f 0397 13f1 5a97  $..RVV.Z._....Z.
+000009e0: 46cc f312 2056 2c63 f2bd 01d5 b53c f6ef  F... V,c.....<..
+000009f0: 3705 1764 9581 d93b ec68 3b01 3f17 fed8  7..d...;.h;.?...
+00000a00: 84c6 ea4e 82a5 8ba3 7216 0b5e f1b5 bc05  ...N....r..^....
+00000a10: 68d4 92be b01f 9b08 e333 17ec 2e7d 701d  h........3...}p.
+00000a20: 928d 047d 632a 8607 56c2 fd20 2bf7 80e5  ...}c*..V.. +...
+00000a30: 1ec1 b0f9 d368 18a4 d568 c507 e77d 10cd  .....h...h...}..
+00000a40: 3970 b3f4 d1dd 9a65 f4b9 95ae 46ca f20b  9p.....e....F...
+00000a50: c955 a432 5dcb 4825 a709 9334 19ea 1e0c  .U.2].H%...4....
+00000a60: f996 1e27 c02a 5197 e39a 65b0 8a4d db1c  ...'.*Q...e..M..
+00000a70: e868 7490 f3a3 d012 ba26 7526 1720 e40e  .ht......&u&. ..
+00000a80: 1e36 baee c072 d44e 1046 9049 2a0a 22e9  .6...r.N.F.I*.".
+00000a90: 8417 1274 b8b7 eb67 35d7 604f 520e 0ad7  ...t...g5.`OR...
+00000aa0: e6f4 af9a 090a 8905 fa02 5ba1 25b1 4f56  ..........[.%.OV
+00000ab0: d523 91a9 568b 6ca8 a3af 1518 8f04 5759  .#..V.l.......WY
+00000ac0: 847e 67f2 73bd 4290 6339 abe8 72b3 2dcf  .~g.s.B.c9..r.-.
+00000ad0: de13 2209 3a91 2cb9 cc8f ff20 5a12 2b4f  ..".:.,.... Z.+O
+00000ae0: 2070 454b b77d ffd1 2dc0 5af8 9d30 1fa5   pEK.}..-.Z..0..
+00000af0: d0e0 fd3e 7c80 e03c 9137 0815 0822 d967  ...>|..<.7...".g
+00000b00: f2bd 8a45 6f59 c4c2 c7cb 6f53 3bf0 9cc0  ...EoY....oS;...
+00000b10: b50d cf8e 5cc3 9bd8 d818 8713 d7c0 5ecf  ....\.........^.
+00000b20: b23d 33e8 f5ad fe77 3046 b87e cc49 2dd3  .=3....w0F.~.I-.
+00000b30: bd0a 14f4 50b7 21e4 174b 33b2 eb56 b0e9  ....P.!..K3..V..
+00000b40: d72c 39d2 f866 ee1f 43f5 3f34 ddda 7765  .,9..f..C.?4..we
+00000b50: b0aa 77cf 8c6e aba3 5ed4 50db bdb0 22e1  ..w..n..^.P...".
+00000b60: dbc6 a2f7 eedd 73c1 be6d b3f0 c212 990e  ......s..m......
+00000b70: 75ab df37 0f73 9f29 dba4 c016 f71c 3509  u..7.s.)......5.
+00000b80: 39a1 580d f533 3661 cb26 82c7 50cd 191b  9.X..36a.&..P...
+00000b90: 7442 a7a9 aa40 abe9 b5a2 c984 2755 6931  tB...@......'Ui1
+00000ba0: 946f d537 0e06 e5fb ea0c 719f e026 80dd  .o.7......q..&..
+00000bb0: 6720 7956 d044 6510 809c 8cf6 50cb 5d56  g yV.De.....P.]V
+00000bc0: e4b7 cb88 29e1 8720 a515 a9a8 4aac 9864  ....).. ....J..d
+00000bd0: cd31 0a1e ac48 5992 5075 8fe8 a3f6 f4df  .1...HY.Pu......
+00000be0: 6e82 1bec df4c 6e2c c7b9 4327 c0a0 98f3  n....Ln,..C'....
+00000bf0: 4301 2986 e453 5dc3 7580 4d6b a037 e319  C.)..S].u.Mk.7..
+00000c00: 4f40 2d39 296a 9229 da74 271f 2ad9 f490  O@-9)j.).t'.*...
+00000c10: 090c 7c86 6d33 f0cc 816d 98d3 9e63 d8fd  ..|.m3...m...c..
+00000c20: 8165 f4ed 9e65 4cec d09a 3ade 349c 8e1d  .e...eL...:.4...
+00000c30: 2518 7555 f9ff 47c1 6e12 d2ef ee40 c53b  %.uU..G.n....@.;
+00000c40: 2542 2e04 895f e1e6 9cd3 f518 1ca4 fca0  %B..._..........
+00000c50: d204 f89e 921d 3bfd b1d9 038a 7684 23c3  ......;.....v.#.
+00000c60: c603 d318 8f41 ec4e 18f5 1c0f 8793 a913  .....A.N........
+00000c70: 1dc9 2a87 ac3f 582e fba8 f99a 1259 4329  ..*..?X......YC)
+00000c80: 5155 a419 fbaa 8df6 b387 c975 3bb1 8ff8  QU.........u;...
+00000c90: 5931 f0e7 a132 64ff f5bf 6d7c 02eb 337a  Y1...2d...m|..3z
+00000ca0: e5e6 e8f9 ca8d 932f b3c5 ecca bd0f d3c5  ......./........
+00000cb0: f225 ba76 7330 1b87 c1f5 fb83 f93c f873  .%.vs0.......<.s
+00000cc0: 31fd a33b 02fd a343 db80 abb6 9129 ea64  1..;...C.....).d
+00000cd0: 32fa 1b00 00ff ff03 0050 4b03 0414 0006  2........PK.....
+00000ce0: 0008 0000 0021 0027 96d6 b5ca 0200 000a  .....!.'........
+00000cf0: 0700 000d 0000 0078 6c2f 7374 796c 6573  .......xl/styles
+00000d00: 2e78 6d6c b455 db6e db30 0c7d 1fb0 7f10  .xml.U.n.0.}....
+00000d10: f4ee ca76 e32c 096c 174b 5303 05b6 6140  ...v.,.l.KS...a@
+00000d20: 3b60 af8a 2d27 4275 3124 2573 36ec df47  ;`..-'Bu1$%s6..G
+00000d30: d94e e2a2 ddad c35e 6289 120f 0f0f 2926  .N.....^b.....)&
+00000d40: bd6a a540 7b66 2cd7 2ac3 d145 8811 53a5  .j.@{f,.*..E..S.
+00000d50: aeb8 da64 f8d3 7d11 cc30 b28e aa8a 0aad  ...d..}..0......
+00000d60: 5886 0fcc e2ab fcf5 abd4 ba83 6077 5bc6  X...........`w[.
+00000d70: 1c02 0865 33bc 75ae 5910 62cb 2d93 d45e  ...e3.u.Y.b.-..^
+00000d80: e886 2938 a9b5 91d4 c1d6 6c88 6d0c a395  ..)8......l.m...
+00000d90: f54e 5290 380c a744 52ae 708f b090 e59f  .NR.8..DR.p.....
+00000da0: 8048 6a1e 764d 506a d950 c7d7 5c70 77e8  .Hj.vMPj.P..\pw.
+00000db0: b030 92e5 e276 a3b4 a16b 0154 db68 424b  .0...v...k.T.hBK
+00000dc0: d446 5313 a3d6 1c83 74d6 2771 242f 8db6  .FS.....t.'q$/..
+00000dd0: ba76 1780 4b74 5df3 923d a53b 2773 42cb  .v..Kt]..=.;'sB.
+00000de0: 3312 20bf 0c29 4a48 183f cabd 352f 449a  3. ..)JH.?..5/D.
+00000df0: 10c3 f6dc 970f e769 ad95 b3a8 d43b e532  .......i.....;.2
+00000e00: 1c03 512f c1e2 41e9 2faa f047 50e1 e156  ..Q/..A./..GP..V
+00000e10: 9eda af68 4f05 5862 4cf2 b4d4 421b e4a0  ...hO.XbL...B...
+00000e20: 74a0 5ce4 2d8a 4ad6 dfb8 a682 af0d f7c6  t.\.-.J.........
+00000e30: 9a4a 2e0e bdb9 f3eb aa3d dc93 1cb4 f7b7  .J.......=......
+00000e40: 88e7 d1b3 c9d3 3518 fe7f ac2e a485 985c  ......5........\
+00000e50: 8891 02bd 214f a155 1c33 aa80 5334 acef  ....!O.U.3..S4..
+00000e60: 0f0d a4aa a0ab 7bca 70f4 dbdb 1b43 0f51  ......{.p....C.Q
+00000e70: 9c8c 1c48 1710 b2d4 a682 5774 d4de cbdc  ...H......Wt....
+00000e80: 9bf2 54b0 da81 0686 6fb6 feeb 7403 bf6b  ..T.....o...t..k
+00000e90: ed1c 745a 9e56 9c6e b4a2 c2cb 76f4 1816  ..tZ.V.n....v...
+00000ea0: 904e c984 b8f3 2fed 73fd 08bb ad91 dac9  .N..../.s.......
+00000eb0: 42ba db2a c3f0 66bd e0c7 2524 322c 7bbc  B..*..f...%$2,{.
+00000ec0: 7ee3 f1c7 683d f608 3606 ca7f 0f8b dafa  ~...h=..6.......
+00000ed0: 84ff 33ef 08f8 3d4f eae4 8d68 d388 83ef  ..3...=O...h....
+00000ee0: d1a1 fb3a aec0 6e24 c123 014e a920 dfa7  ...:..n$.#.N. ..
+00000ef0: 19fe e0c7 8c80 8e1f e8a0 f58e 0bc7 d533  ...............3
+00000f00: c903 66d5 9ee5 0c7d 359d 1f19 9dd0 a728  ..f....}5......(
+00000f10: a06a c56a ba13 eefe 7498 e1f3 fa3d abf8  .j.j....t....=..
+00000f20: 4ec2 231b 6e7d e47b ed3a 880c 9fd7 ef7c  N.#.n}.{.:.....|
+00000f30: d5a3 a98f c15a f7ce c2b3 802f da19 9ee1  .....Z...../....
+00000f40: 6f37 cb37 f3d5 4d11 07b3 7039 0b26 972c  o7.7..M...p9.&.,
+00000f50: 09e6 c972 1524 93eb e56a 55cc c338 bcfe  ...r.$...jU..8..
+00000f60: 3e1a 5cff 30b6 ba39 0b05 8e26 0b2b 60b8  >.\.0..9...&.+`.
+00000f70: 9921 d981 fcdd d996 e1d1 a6a7 dff5 3bd0  .!............;.
+00000f80: 1e73 9fc7 d3f0 6d12 8541 7119 46c1 644a  .s....m..Aq.F.dJ
+00000f90: 67c1 6c7a 9904 4512 c5ab e964 7993 14c9  g.lz..E....dy...
+00000fa0: 887b f2c2 f116 9228 ea07 a527 9f2c 1c97  .{.....(...'.,..
+00000fb0: 4c70 75ac d5b1 4263 2b14 09b6 bf48 821c  Lpu...Bc+....H..
+00000fc0: 2b41 ce7f 62f9 0f00 0000 ffff 0300 504b  +A..b.........PK
+00000fd0: 0304 1400 0600 0800 0000 2100 c117 10be  ..........!.....
+00000fe0: 4e07 0000 c620 0000 1300 0000 786c 2f74  N.... ......xl/t
+00000ff0: 6865 6d65 2f74 6865 6d65 312e 786d 6cec  heme/theme1.xml.
+00001000: 59cd 8b1b 3714 bf17 fa3f 0c73 77fc 35e3  Y...7....?.sw.5.
+00001010: 8f25 dee0 cf6c 93dd 2464 9d94 1cb5 b6ec  .%...l..$d......
+00001020: 5156 3332 92bc 1b13 0225 39f5 5228 a4a5  QV32.....%9.R(..
+00001030: 9742 6f3d 94d2 4003 0dbd f48f 0924 b4e9  .Bo=..@......$..
+00001040: 1fd1 27cd d823 ade5 249b 6c4a 5a76 0d8b  ..'..#..$.lJZv..
+00001050: 47fe bda7 a7f7 9e7e 7af3 74f1 d2bd 987a  G......~z.t....z
+00001060: 4798 0bc2 9296 5fbe 50f2 3d9c 8cd8 9824  G....._.P.=....$
+00001070: d396 7f6b 3828 347c 4f48 948c 1165 096e  ...k8(4|OH...e.n
+00001080: f90b 2cfc 4bdb 9f7e 7211 6dc9 08c7 d803  ..,.K..~r.m.....
+00001090: f944 6ca1 961f 4939 db2a 16c5 0886 91b8  .Dl...I9.*......
+000010a0: c066 3881 df26 8cc7 48c2 239f 16c7 1c1d  .f8..&..H.#.....
+000010b0: 83de 9816 2ba5 52ad 1823 92f8 5e82 6250  ....+.R..#..^.bP
+000010c0: 7b7d 3221 23ec 0d95 4a7f 7ba9 bc4f e131  {}2!#...J.{..O.1
+000010d0: 9142 0d8c 28df 57aa b125 a1b1 e3c3 b242  .B..(.W..%.....B
+000010e0: 8885 e852 ee1d 21da f261 9e31 3b1e e27b  ...R..!..a.1;..{
+000010f0: d2f7 2812 127e 68f9 25fd e717 b72f 16d1  ..(..~h.%..../..
+00001100: 5626 44e5 0659 436e a0ff 32b9 4c60 7c58  V&D..YCn..2.L`|X
+00001110: d173 f2e9 c16a d220 0883 5a7b a55f 03a8  .s...j. ..Z{._..
+00001120: 5cc7 f5eb fd5a bfb6 d2a7 0168 3482 95a6  \....Z.....h4...
+00001130: b6d8 3aeb 956e 9061 0d50 fad5 a1bb 57ef  ..:..n.a.P....W.
+00001140: 55cb 16de d05f 5db3 b91d aa8f 85d7 a054  U...._]........T
+00001150: 7fb0 861f 0cba e045 0baf 4129 3e5c c387  .......E..A)>\..
+00001160: 9d66 a767 ebd7 a014 5f5b c3d7 4bed 5e50  .f.g...._[..K.^P
+00001170: b7f4 6b50 4449 72b8 862e 85b5 6a77 b9da  ..kPDIr.....jw..
+00001180: 1564 c2e8 8e13 de0c 8341 bd92 29cf 5190  .d.......A..).Q.
+00001190: 0dab ec52 534c 5822 37e5 5a8c ee32 3e00  ...RSLX"7.Z..2>.
+000011a0: 8002 5224 49e2 c9c5 0c4f d008 b2b8 8b28  ..R$I....O.....(
+000011b0: 39e0 c4db 25d3 0812 6f86 1226 60b8 5429  9...%...o..&`.T)
+000011c0: 0d4a 55f8 af3e 81fe a623 8ab6 3032 a495  .JU..>...#..02..
+000011d0: 5d60 8958 1b52 f678 62c4 c94c b6fc 2ba0  ]`.X.R.xb..L..+.
+000011e0: d537 202f 9e3d 7bfe f0e9 f387 bf3d 7ff4  .7 /.={......=..
+000011f0: e8f9 c35f b2b9 b52a 4b6e 0725 5353 eed5  ..._...*Kn.%SS..
+00001200: 8f5f fffd fd17 de5f bffe f0ea f137 e9d4  ._....._.....7..
+00001210: 27f1 c2c4 bffc f9cb 97bf fff1 3af5 b0e2  '...........:...
+00001220: dc15 2fbe 7df2 f2e9 9317 df7d f5e7 4f8f  ../.}......}..O.
+00001230: 1dda db1c 1d98 f021 89b1 f0ae e163 ef26  .......!.....c.&
+00001240: 8b61 810e fbf1 013f 9dc4 3042 c492 4011  .a.....?..0B..@.
+00001250: e876 a8ee cbc8 025e 5b20 eac2 75b0 edc2  .v.....^[ ..u...
+00001260: db1c 58c6 05bc 3cbf 6bd9 ba1f f1b9 248e  ..X...<.k.....$.
+00001270: 99af 46b1 05dc 638c 7618 773a e0aa 9acb  ..F...c.v.w:....
+00001280: f0f0 709e 4cdd 93f3 b989 bb89 d091 6bee  ..p.L.........k.
+00001290: 2e4a ac00 f7e7 33a0 57e2 52d9 8db0 65e6  .J....3.W.R...e.
+000012a0: 0d8a 1289 a638 c1d2 53bf b143 8c1d abbb  .....8..S..C....
+000012b0: 4388 e5d7 3d32 e24c b089 f4ee 10af 8388  C...=2.L........
+000012c0: d325 4372 6025 522e b443 6288 cbc2 6520  .%Cr`%R..Cb...e 
+000012d0: 84da f2cd de6d afc3 a86b d53d 7c64 2361  .....m...k.=|d#a
+000012e0: 5b20 ea30 7e88 a9e5 c6cb 682e 51ec 5239  [ .0~.....h.Q.R9
+000012f0: 4431 351d be8b 64e4 3272 7fc1 4726 ae2f  D15...d.2r..G&./
+00001300: 2444 7a8a 29f3 fa63 2c84 4be6 3a87 f51a  $Dz.)..c,.K.:...
+00001310: 41bf 0a0c e30e fb1e 5dc4 3692 4b72 e8d2  A.......].6.Kr..
+00001320: b98b 1833 913d 76d8 8d50 3c73 da4c 92c8  ...3.=v..P<s.L..
+00001330: c47e 260e 2145 9177 8349 177c 8fd9 3b44  .~&.!E.w.I.|..;D
+00001340: 3d43 1c50 b231 dcb7 09b6 c2fd 6622 b805  =C.P.1......f"..
+00001350: e46a 9a94 2788 fa65 ce1d b1bc 8c99 bd1f  .j..'..e........
+00001360: 1774 82b0 8b65 da3c b6d8 b5cd 8933 3b3a  .t...e.<.....3;:
+00001370: f3a9 95da bb18 5374 8cc6 187b b73e 7358  ......St...{.>sX
+00001380: d061 33cb e7b9 d157 2260 951d ec4a ac2b  .a3....W"`...J.+
+00001390: c8ce 55f5 9c60 0165 92aa 6bd6 2972 9708  ..U..`.e..k.)r..
+000013a0: 2b65 f7f1 946d b067 6f71 8278 1628 8911  +e...m.goq.x.(..
+000013b0: dfa4 f91a 44dd 4a5d 38e5 9c54 7a9d 8e0e  ....D.J]8..Tz...
+000013c0: 4de0 3502 e51f e48b d329 d705 e830 92bb  M.5......)...0..
+000013d0: bf49 eb8d 0859 6797 7a16 ee7c 5d70 2b7e  .I...Yg.z..|]p+~
+000013e0: 6fb3 c760 5fde 3ded be04 197c 6a19 20f6  o..`_.=....|j. .
+000013f0: b7f6 cd10 516b 823c 6186 080a 0c17 dd82  ....Qk.<a.......
+00001400: 8815 fe5c 449d ab5a 6cee 949b d89b 360f  ...\D..Zl.....6.
+00001410: 0314 4656 bd13 93e4 8dc5 cf89 b227 fc77  ..FV.........'.w
+00001420: ca1e 7701 7306 058f 5bf1 fb94 3a9b 2865  ..w.s...[...:.(e
+00001430: e744 81b3 09f7 1f2c 6b7a 689e dcc0 7092  .D.....,kzh...p.
+00001440: ac73 d679 5573 5ed5 f8ff fbaa 66d3 5e3e  .s.yUs^.....f.^>
+00001450: af65 ce6b 99f3 5ac6 f5f6 f541 6a99 bc7c  .e.k..Z....Aj..|
+00001460: 81ca 26ef f2e8 9e4f bcb1 e533 2194 eecb  ..&....O...3!...
+00001470: 05c5 bb42 777d 04bc d18c 0730 a8db 51ba  ...Bw}.....0..Q.
+00001480: 27b9 6a01 ce22 f89a 3598 2cdc 9423 2de3  '.j.."..5.,..#-.
+00001490: 7126 3f27 32da 8fd0 0c5a 4365 ddc0 9c8a  q&?'2....ZCe....
+000014a0: 4cf5 5478 3326 a063 a487 752b 159f d0ad  L.Tx3&.c..u+....
+000014b0: fb4e f378 8f8d d34e 67b9 acba 9aa9 0b05  .N.x...Ng.......
+000014c0: 92f9 7829 5c8d 4397 4aa6 e85a 3def dead  ..x)\.C.J..Z=...
+000014d0: d4eb 7ee8 5477 5997 0628 d9d3 1861 4c66  ..~.TwY..(...aLf
+000014e0: 1b51 7518 515f 0e42 145e 6784 5ed9 9958  .Qu.Q_.B.^g.^..X
+000014f0: d174 58d1 50ea 97a1 5a46 71e5 0a30 6d15  .tX.P...ZFq..0m.
+00001500: 1578 e5f6 e045 bde5 8741 da41 8666 1c94  .x...E...A.A.f..
+00001510: e763 15a7 b499 bc8c ae0a ce99 467a 9333  .c..........Fz.3
+00001520: a999 0150 622f 3320 8f74 53d9 ba71 796a  ...Pb/3 .tS..qyj
+00001530: 7569 aabd 45a4 2d23 8c74 b38d 30d2 3082  ui..E.-#.t..0.0.
+00001540: 17e1 2c3b cd96 fb59 c6ba 9987 d432 4fb9  ..,;...Y.....2O.
+00001550: 62b9 1b72 33ea 8d0f 116b 4522 27b8 8126  b..r3....kE"'..&
+00001560: 2653 d0c4 3b6e f9b5 6a08 b72a 2334 6bf9  &S..;n..j..*#4k.
+00001570: 13e8 18c3 d778 06b9 23d4 5b17 a253 b876  .....x..#.[..S.v
+00001580: 1949 9e6e f877 6196 1917 b287 4494 3a5c  .I.n.wa.....D.:\
+00001590: 934e ca06 3191 987b 94c4 2d5f 2d7f 950d  .N..1..{..-_-...
+000015a0: 34d1 1ca2 6d2b 5780 103e 5ae3 9a40 2b1f  4...m+W..>Z..@+.
+000015b0: 9b71 1074 3bc8 7832 c123 6986 dd18 519e  .q.t;.x2.#i...Q.
+000015c0: 4e1f 81e1 53ae 70fe aac5 df1d ac24 d91c  N...S.p......$..
+000015d0: c2bd 1f8d 8fbd 033a e737 11a4 5858 2f2b  .......:.7..XX/+
+000015e0: 078e 8980 8b83 72ea cd31 819b b015 91e5  ......r..1......
+000015f0: f977 e260 ca68 d7bc 8ad2 3994 8e23 3a8b  .w.`.h....9..#:.
+00001600: 5076 a298 649e c235 89ae ccd1 4f2b 1f18  Pv..d..5....O+..
+00001610: 4fd9 9ac1 a1eb 2e3c 98aa 03f6 bd4f dd37  O......<.....O.7
+00001620: 1fd5 ca73 0669 e667 a6c5 2aea d474 93e9  ...s.i.g..*..t..
+00001630: 873b e40d abf2 43d4 b22a a56e fd4e 2d72  .;....C..*.n.N-r
+00001640: ae6b 2eb9 0e12 d579 4abc e1d4 7d8b 03c1  .k.....yJ...}...
+00001650: 302d 9fcc 324d 59bc 4ec3 8ab3 b351 dbb4  0-..2MY.N....Q..
+00001660: 332c 080c 4fd4 36f8 6d75 4638 3df1 ae27  3,..O.6.muF8=..'
+00001670: 3fc8 9dcc 5a75 402c eb4a 9df8 faca dcbc  ?...Zu@,.J......
+00001680: d566 0777 813c 7a70 7f38 a752 e850 426f  .f.w.<zp.8.R.PBo
+00001690: 9723 28fa d21b c894 3660 8bdc 9359 8d08  .#(.....6`...Y..
+000016a0: dfbc 3927 2dff 7e29 6c07 dd4a d82d 941a  ..9'-.~)l..J.-..
+000016b0: 61bf 1054 8352 a111 b6ab 8576 1856 cbfd  a..T.R.....v.V..
+000016c0: b05c ea75 2a0f e060 9151 5c0e d3eb fa01  .\.u*..`.Q\.....
+000016d0: 5c61 d045 7669 afc7 d72e eee3 e52d cd85  \a.Evi.......-..
+000016e0: 118b 8b4c 5fcc 17b5 e1fa e2be 5cd9 7c71  ...L_.......\.|q
+000016f0: ef11 209d fbb5 caa0 596d 766a 8566 b53d  .. .....Ymvj.f.=
+00001700: 2804 bd4e a3d0 ecd6 3a85 5ead 5bef 0d7a  (..N....:.^.[..z
+00001710: ddb0 d11c 3cf0 bd23 0d0e dad5 6e50 eb37  ....<..#....nP.7
+00001720: 0ab5 72b7 5b08 6a25 657e a359 a807 954a  ..r.[.j%e~.Y...J
+00001730: 3ba8 b71b fda0 fd20 2b63 60e5 297d 64be  ;...... +c`.)}d.
+00001740: 00f7 6abb b6ff 0100 00ff ff03 0050 4b03  ..j..........PK.
+00001750: 0414 0006 0008 0000 0021 00ae 18fb 4a10  .........!....J.
+00001760: 1300 0062 9300 0018 0000 0078 6c2f 776f  ...b.......xl/wo
+00001770: 726b 7368 6565 7473 2f73 6865 6574 312e  rksheets/sheet1.
+00001780: 786d 6c9c 934d 8f9b 3010 86ef 95f6 3f58  xml..M..0.....?X
+00001790: be07 034b d22e 0a59 adb2 8aba b7aa ddb6  ...K...Y........
+000017a0: 6763 8660 c5c6 d436 f950 d5ff de31 e44b  gc.`...6.P...1.K
+000017b0: ca25 5a04 368c cdf3 be63 8fe7 cf7b adc8  .%Z.6....c...{..
+000017c0: 16ac 93a6 2d68 12c5 9440 2b4c 25db 7541  ....-h...@+L%.uA
+000017d0: 7fbe af26 5f28 719e b715 57a6 8582 1ec0  ...&_(q...W.....
+000017e0: d1e7 c5c3 a7f9 ced8 8d6b 003c 4142 eb0a  .........k.<AB..
+000017f0: da78 dfe5 8c39 d180 e62e 321d b438 521b  .x...9....2..8R.
+00001800: abb9 c74f bb66 aeb3 c0ab e127 ad58 1ac7  ...O.f.....'.X..
+00001810: 33a6 b96c e948 c8ed 3d0c 53d7 52c0 ab11  3..l.H..=.S.R...
+00001820: bd86 d68f 100b 8a7b f4ef 1ad9 b913 4d8b  .......{......M.
+00001830: 7b70 9adb 4ddf 4d84 d11d 224a a9a4 3f0c  {p..M.M..."J..?.
+00001840: 504a b4c8 dfd6 adb1 bc54 98f7 3ec9 b820  PJ.......T..>.. 
+00001850: 7b8b 778a cfe3 4966 88df 2869 29ac 71a6  {.w...If..(i).q.
+00001860: f611 92d9 e8f9 36fd 27f6 c4b8 3893 6ef3  ......6.'...8.n.
+00001870: bf0b 9364 ccc2 5686 0dbc a0d2 8f59 4aa6  ...d..V......YJ.
+00001880: 6756 7a81 3d7e 1036 3bc3 c272 d9bc 9755  gVz.=~.6;..r...U
+00001890: 41ff c6c7 6b82 7d12 9af8 d29c c6fe d1c5  A...k.}.........
+000018a0: bc92 b8c3 212b 62a1 2ee8 4b92 2fd3 e994  ....!+b...K./...
+000018b0: b2c5 7ca8 a05f 1276 eeea 9d78 5efe 0005  ..|.._.v...x^...
+000018c0: c203 aa24 9484 022d 8dd9 8489 6f18 8a91  ...$...-....o...
+000018d0: e986 0981 c985 975b 5882 5201 9d61 91ff  .......[X.R..a..
+000018e0: 39ca 6441 829d 35ae df4f 7aab a1a8 bf59  9.dA..5..Oz....Y
+000018f0: 5272 074b a37e cbca 3728 8a87 a782 9af7  Rr.K.~..7(......
+00001900: ca5f 05d1 ca31 f8dd ecbe 825c 371e a7ce  ._...1.....\7...
+00001910: 7045 4249 e5d5 e115 9cc0 5a46 8751 1ab4  pEBI......ZF.Q..
+00001920: 8551 2884 2dd1 329c 492c 45be 1f53 1a75  .Q(.-.2.I,E..S.u
+00001930: b22c 4a66 593c 4ba7 9494 e0fc 4a06 2225  .,JfY<K.....J."%
+00001940: a277 dee8 9399 236a 84e0 6e0e 10ec 7747  .w....#j..n...wG
+00001950: b39f ef85 b0c1 d07f 0000 00ff ff00 0000  ................
+00001960: ffff 949d dfee db36 1285 5fa5 c87d 1c93  .......6.._..}..
+00001970: fa63 bb48 03ec 2fed 8304 d900 bdea 2e9a  .c.H../.........
+00001980: 20bb fbf6 3b94 c716 0f87 3cf2 e955 d1d1   ...;.....<..U..
+00001990: 245f 69ea 3345 e958 1fbf fff9 eddb 8fdf  $_i.3E.X........
+000019a0: bffc f8f2 e9e3 dfff facf 2f7f fff6 2ebd  ........../.....
+000019b0: fbe5 fbbf bffc f5dd feed d7e9 dd2f ff4d  ............./.M
+000019c0: f397 afbf fef3 7fbf 7ffb fef5 db5f 3f7e  ............._?~
+000019d0: 7b77 3ee5 779f 3e7e 2d87 fea3 1cbb 75d8  {w>.w.>~-.....u.
+000019e0: 7fff 6eff f5e7 a7f3 c70f 3f3f 7dfc f0d5  ..n.......??}...
+000019f0: 8f78 8b47 243c e273 3c22 3f8f f860 4c4f  .x.G$<.s<"?..`LO
+00001a00: b02c 80d9 b14f a475 6a98 eae2 7c6d 70ca  .,...O.uj...|mp.
+00001a10: ffdc cf4f cb29 dde0 9feb 1fef 0758 3646  ...O.).......X6F
+00001a20: 2f8f 971d fbc4 5ad6 06ab 2ece b706 6bda  /.....Z.......k.
+00001a30: b0d6 d319 ff49 7fbc dfff ef60 b466 01cb  .....I.....`.f..
+00001a40: 8e1d 63d5 c5f9 d260 cd2a d622 60d9 b163  ..c....`.*."`..c
+00001a50: 2c28 36b3 eef3 a262 ad02 961d 3bc6 aa8b  ,(6....b....;...
+00001a60: 73f3 097f 5e55 ac8b 8065 c78e b1ea 6298  s...^U...e....b.
+00001a70: f217 15eb 2a60 d9b1 fb99 b834 531e 8aed  ....*`.....4S...
+00001a80: 685d 37ac f7bb 2f60 7edf 0406 3b76 6768  h]7.../`~...;vgh
+00001a90: a6f0 1b14 5b86 1b65 4867 c595 76f0 93a2  ....[..eHg..v...
+00001aa0: 5552 f993 9ec5 70f2 5bb5 4869 3012 4932  UR....p.[.Hi0.I2
+00001ab0: b61d 3ca6 a88b e15c b7bf 8751 287a 4eb5  ..<....\...Q(zN.
+00001ac0: 82c3 58d4 c5a5 3db5 ad95 5128 364e b571  ..X...=...Q(6N.q
+00001ad0: 0305 e8b8 9d17 d6ca 2814 f9a6 5ab0 8102  ........(...Z...
+00001ae0: ecdb 7e57 592b a350 5c9b 6a9f ceed 9738  ..~WY+.P\.j....8
+00001af0: 1403 c5dd b6a3 d9a9 a835 813e 5b0a 106f  .........5.>[..o
+00001b00: 9817 77b9 8e28 1493 26b0 654b 01c5 302f  ..w..(..&.eK..0/
+00001b10: ee2e 1d51 28e2 4cb5 1cc3 2702 c5f6 5bd9  ...Q(.L...'...[.
+00001b20: 5ad9 bc50 d499 6a3d 060a 28b6 4b16 6b25  Z..P..j=..(.K.k%
+00001b30: 1459 7167 3978 ff72 6b97 7350 6c18 3f5b  .Yqg9x.rk.sPl.?[
+00001b40: 6ba1 187d 8d64 459e e5e0 3106 14db 55ae  k..}.dE...1...U.
+00001b50: b552 0c69 710b 826c 4703 8a8d 4f3e e7bb  .R.iq..lG...O>..
+00001b60: 3d87 a3a1 e833 c36a b6c5 80e2 be74 deae  =....3.j.....t..
+00001b70: 1b3e 5b2b 1d0d c59f b956 64bb a686 62f8  .>[+.....Vd...b.
+00001b80: 5eb5 6ac1 984f e735 cfd5 c27a 7401 a208  ^.j..O.5...zt...
+00001b90: 35d7 ce0c 5820 d4f6 f4b5 5609 4b31 6cae  5...X ....V.K1l.
+00001ba0: 251a b0a8 61ad 55c2 5294 9b6b ab06 2caa  %...a.U.R..k..,.
+00001bb0: 5c6b 95b0 1407 6758 a0b6 531c 1c1c ae23  \k....gX..S....#
+00001bc0: ef0e 7e79 6e29 52ce b577 dbf5 2c14 c3f2  ..~yn)R..w..,...
+00001bd0: c9aa ca68 4d8a a5cb c14f 3db6 5850 0c97  ...hM....O=.XP..
+00001be0: 2056 95b0 146b 4fb5 9803 162c 79c3 55f7   V...kO....,y.U.
+00001bf0: ddda af7e 8893 62f1 72f0 78b4 608f a215  ...~..b.r.x.`...
+00001c00: 84b5 4aa3 256d 51d4 e20e a345 17c5 d3dd  ..J.%mQ....E....
+00001c10: ea2f 8f96 62f9 a9b6 7c73 aebd 4131 6e9d  ./..b...|s..A1n.
+00001c20: dc2d 9f4f f32d d5bb 2783 45da a458 be1c  .-.O.-..'.E..X..
+00001c30: fcfc 1003 16b5 bcb5 960f f165 2cc5 f253  ...........e,..S
+00001c40: 2df2 8045 2d6f ad12 9662 f9a9 1679 c0a2  -..E-o...b...y..
+00001c50: 96b7 5609 4bb1 fc54 8b3c 6051 cb5b ab84  ..V.K..T.<`Q.[..
+00001c60: a558 7eaa 2ddf 98e9 0d8a 71ca df2d 9fcf  .X~.-.....q..-..
+00001c70: a7fd bb14 7707 15af cfb5 d75b 1028 c6fd  ....w......[.(..
+00001c80: c1bb d709 8862 f2b9 9675 0081 f577 7b79  .....b...u...w{y
+00001c90: 68ad db07 351e 11c5 dd73 ade7 0002 ee6e  h...5....s.....n
+00001ca0: af10 adf5 0044 b1f5 5c0b 3980 80ad db05  .....D..\.9.....
+00001cb0: 8ab5 1e80 485b c8b5 9f53 7b17 6086 6d8c  ....H[...S{.`.m.
+00001cc0: f65b d6aa 1bc9 65b4 95ad 1879 aea5 1b41  .[....e....y...A
+00001cd0: a892 ad97 8328 0e9e 6bcd 4610 2a61 ebe5  .....(..k.F.*a..
+00001ce0: 208a 75e7 5aac 1184 6ad7 7a39 88e2 d9b9   .u.Z...j.z9....
+00001cf0: 5669 04a1 a2b5 5e0e a298 75ae cdba b48b  Vi....^...u.....
+00001d00: 1ca8 06b5 5ab5 809c 4ff3 b437 825b 17c5  ....Z...O..7.[..
+00001d10: ade5 e07d 4ba1 4581 6a90 ab55 8f50 14bb  ...}K.E.j..U.P..
+00001d20: 2e20 d080 42f5 6abd 4728 8a5f 17d8 c408  . ..B.j.G(._....
+00001d30: 2854 b0d6 7b84 a218 7681 8d8c 8042 156b  (T..{...v....B.k
+00001d40: bd47 288a 6317 706c 6b7b a886 696b d5ed  .G(.c.plk{..ik..
+00001d50: fc99 cebb 9b71 d64a 77e6 40b2 8184 4a76  .....q.Jw.@...Jv
+00001d60: 71c9 8e49 14cb 2e60 d940 422d 6bbd 0763  q..I...`.@B-k..c
+00001d70: a268 7601 cd06 12aa 59eb 3d20 513c bb80  .hv.....Y.= Q<..
+00001d80: 6703 09f5 acf5 1e90 28a2 5d6a d1a6 f6ee  g.......(.]j....
+00001d90: 1f54 e38c bd8b f6ba 0e26 ecaa 68b6 1cfc  .T.......&..h...
+00001da0: d46c 0081 6ad0 ac55 cb90 8c41 14c9 aeb5  .l..j..U...A....
+00001db0: 4623 0895 acf5 7210 45b1 6b2d d108 4215  F#....r.E.k-..B.
+00001dc0: 6bbd 1c44 11ec 5a2b 3482 50c1 5a2f 0751  k..D..Z+4.P.Z/.Q
+00001dd0: f4ba 825e db4d 48a8 86c9 6ad5 0292 d6fd  ...^.MH...j.....
+00001de0: f603 d875 55ec 5a0e de27 6b00 a176 b55e  ...uU.Z..'k..v.^
+00001df0: 0ea2 c875 05b9 0610 2a57 ebe5 208a 5b57  ...u....*W.. .[W
+00001e00: 706b 00a1 6eb5 5e0e a2a8 7505 b506 10aa  pk..n.^...u.....
+00001e10: 56eb e520 8a59 5730 6b73 7fe5 0daa 71b2  V.. .YW0ks....q.
+00001e20: fa8d b975 b003 7651 cc5a 0ede 276b 0b02  ...u..vQ.Z..'k..
+00001e30: d560 56ab de47 6404 a298 f502 660d 20d4  .`V..Gd.....f. .
+00001e40: acd6 cb41 14b3 5ec0 ac01 849a d57a 3988  ...A..^......z9.
+00001e50: 62d6 0b98 3580 50b3 5a2f 0751 cc7a 01b3  b...5.P.Z/.Q.z..
+00001e60: b6cf 3840 354c 56ab 1690 e55a 5d30 825a  ..8@5LV....Z]0.Z
+00001e70: 2f8a 5acb c1fb 6c0d 2454 add6 7b40 a2b8  /.Z...l.$T..{@..
+00001e80: f502 6e0d 24d4 add6 7b40 a2c8 f502 720d  ..n.$...{@....r.
+00001e90: 2454 aed6 7b40 a2d8 f502 760d 24d4 aed6  $T..{@....v.$...
+00001ea0: 7b40 a2e8 f502 7a6d 6ee6 bf41 35ce 58d7  {@....zmn..A5.X.
+00001eb0: eb32 0d56 ae57 c5af e5e0 7dc6 b624 500d  .2.V.W....}..$P.
+00001ec0: 7eb5 ea76 128f 4914 c15e 41b0 8184 0ad6  ~..v..I..^A.....
+00001ed0: 7a0f 4814 c35e c1b0 8184 1ad6 7a0f 4814  z.H..^......z.H.
+00001ee0: c55e 41b1 8184 2ad6 7a0f 4814 c75e c1b1  .^A...*.z.H..^..
+00001ef0: ed93 3a50 0d37 85ad 5a48 d625 8f66 ace2  ..:P.7..ZH.%.f..
+00001f00: d82b 3836 9080 63db 4d69 eb3d 2051 1c7b  .+86..c.Mi.= Q.{
+00001f10: 05c7 0692 ba1a 9ed5 b5de 0312 c5b1 5770  ..............Wp
+00001f20: 6c20 01c7 b677 7bad f780 4471 ec15 1c1b  l ...w{...Dq....
+00001f30: 48c0 b1ed 46bd f51e 9028 8ebd 8263 db9d  H...F....(...c..
+00001f40: 35a8 06c7 5a75 3b77 4e83 5b06 3745 b1e5  5...Zu;wN.[.7E..
+00001f50: e05d b1e1 f9e0 ba1a 146b bd1c 4431 ec0d  .].......k..D1..
+00001f60: 0c1b 40a8 61ad 9783 2882 bd81 6003 0815  ..@.a...(...`...
+00001f70: acf5 7210 c5af 37f0 6b00 a17e b55e 0ea2  ..r...7.k..~.^..
+00001f80: e8f5 067a 6d6f 1243 353c dc62 d502 729b  ...zmo.C5<.b..r.
+00001f90: 470b 829b a2d7 72f0 3e5b 0309 e835 3cce  G.....r.>[...5<.
+00001fa0: 7ed7 2b21 51f4 7a03 bd06 12ba 84b5 de83  ~.+!Q.z.........
+00001fb0: 3151 f47a 03bd 0612 aa57 eb3d 2051 f47a  1Q.z.....W.= Q.z
+00001fc0: 03bd 0612 aa57 eb3d 2051 f47a abf5 9adb  .....W.= Q.z....
+00001fd0: a509 5483 5ead 5a48 96db e016 973d 4723  ..T.^.ZH.....=G#
+00001fe0: 251f 6a85 0694 ed0f dbc3 0fed d75f 291f  %.j.........._).
+00001ff0: c028 8e4d e75a a31d 186a d9d2 7d00 a378  .(.M.Z...j..}..x
+00002000: 369d 6b95 7660 a869 4bf7 018c e2da 74ae  6.k.v`.iK.....t.
+00002010: 75da 81a1 b62d dd07 308a 6fd3 b916 6eb5  u....-..0.o...n.
+00002020: 2edd 1e20 7ec3 7227 30e3 cab5 dbb4 fd30  ... ~.r'0......0
+00002030: 613a 2bce dd8e 7e4e d10e 0ddd 3828 dddb  a:+...~N....8(..
+00002040: 894d 6814 efa6 73ad d60e 0d35 6fe9 3ea2  .Mh...s....5o.>.
+00002050: 51dc 9bce b55e 3b34 7403 a174 1fd1 28fe  Q....^;4t..t..(.
+00002060: 4de7 5ab1 1d1a ba89 50ba 8f68 1407 a733  M.Z.....P..h...3
+00002070: 48b8 dd82 c372 6716 df35 7c5b 4737 6d93  H....rg..5|[G7m.
+00002080: 9640 8394 590e 3418 420b 1ef6 141a a391  .@..Y.4.B.......
+00002090: 445c 726b fb39 1569 b888 3d8d c668 2413  D\rk.9.i..=..h$.
+000020a0: 4324 ad33 36dc c49e 4a63 3492 8a21 9ad6  C$.36...Jc4..!..
+000020b0: a1e1 2af6 741a a391 5c0c 11b5 1c32 6a50  ..*.t...\....2jP
+000020c0: 8eb3 f891 522b 118b 818c 4bfa ecf5 d039  ....R+....K....9
+000020d0: 64d5 3a38 5cc6 d6bd 5d16 301c c9c6 105a  d.:8\...].0....Z
+000020e0: ebe0 701b 5bf7 218e a463 48af 7570 b88e  ..p.[.!..cH.up..
+000020f0: adfb 1047 f231 c4d8 3a38 dcc7 8f24 1bfb  ...G.1..:8...$..
+00002100: b024 2143 9e2d 8740 1bc6 dd42 a2cd 236d  .$!C.-.@...B..#m
+00002110: d365 1ecd 6429 d696 20d7 1669 a01c f3b8  .e..d).. ..i....
+00002120: 1e6d 6334 9290 21de d6a1 e142 f684 1ba3  .mc4..!....B....
+00002130: 9184 6c51 b5ea eb21 7c52 500e bb77 c983  ..lQ...!|RP..w..
+00002140: 6e8c 4612 3284 dd3a 63c3 85ec 7937 4623  n.F.2..:c...y7F#
+00002150: 0919 626d 4bfb 5c4d c272 4c50 fbc3 0aa3  ..bmK.\M.rLP....
+00002160: 946a 89ae bd6e 6308 ba75 58e8 8644 f2ac  .j...nc..uX..D..
+00002170: 5b1a b248 2a86 745b 8705 767c c302 c703  [..H*.t[..v|....
+00002180: 6e63 16c9 c310 69eb b080 8743 a6da 536d  nc....i....C..Sm
+00002190: 6316 49c2 9063 ebb0 d06d 8964 dddb 77c2  c.I..c...m.d..w.
+000021a0: f033 920c 0cf9 b41c e76e bd62 8e8b 09cf  .3.......n.b....
+000021b0: af59 6ac6 9e1f 3c8e 6c26 29c0 b61d bd2f  .Yj...<.l&)..../
+000021c0: 4903 1b66 d8c2 fcf1 10db eb6c 929d 21c6  I..f.......l..!.
+000021d0: 16c7 0dca f157 13ac 5c3e c3d7 d924 5743  .....W..\>...$WC
+000021e0: 96ad c3c6 17cf 1e67 7b9d 4d32 b7a5 d2aa  .......g{.M2....
+000021f0: ef91 f899 7273 7ba6 ed75 36c9 e310 5ccb  ....rs{..u6...\.
+00002200: ede3 4489 e7da 4a79 3b2f 6fa3 7de5 2465  ..D...Jy;/o.}.$e
+00002210: d9b6 a3f7 d91f 69f8 bada f36c 89d0 482e  ......i....l..H.
+00002220: 870c 5b67 6cf8 b2da 636c 8c46 b239 44d7  ..[gl...cl.F.9D.
+00002230: 3a34 7c55 ede9 3546 23f9 1c12 6b1d 1abe  :4|U..5F#...k...
+00002240: a8f6 d01a a391 8c0e 59b4 dcde a449 3caa  ........Y....I<.
+00002250: 56ca 6516 5ff2 f0ea b044 cc5e 5f8f 4020  V.e._....D.^_.@ 
+00002260: 2dd2 f0bc 5ab2 f211 8d64 6d88 ac75 68f8  -...Z....dm..uh.
+00002270: 9ada 536b 6c6c 244f 436e ad43 c33d edd1  ..Skll$OCn.C.=..
+00002280: 3546 2399 19c2 6b1d 1a6e 66cf af31 1ac9  5F#...k..nf..1..
+00002290: c590 51ab 1e3a f70d 671e 614b 9e61 bbdc  ..Q..:..g.aK.a..
+000022a0: 4ef5 0f49 9ccf 83fc 652a 3135 614e d7ea  N..I....e*15aN..
+000022b0: edb0 7133 7bac ed75 36c9 d390 73eb b071  ..q3{..u6...s..q
+000022c0: 4f7b d2ed 7536 c9da 107d ebb0 716b 7bf8  O{..u6...}..qk{.
+000022d0: ed75 36c9 e190 86eb b071 877b 1eee 7536  .u6......q.{..u6
+000022e0: c9e8 1081 cbed 5dcc c413 72a5 7c5f 978c  ......]...r.|_..
+000022f0: a21b 498a c86d 47ef eb92 40c3 4372 a5fb  ..I..mG...@.Cr..
+00002300: 8846 323a c4e4 e2d8 608a 2e5c 7b7b 502e  .F2:....`..\{{P.
+00002310: d9de ec60 2fb4 64df 5e37 0324 e53a 34dc  ...`/.d.^7.$.:4.
+00002320: e89e 9563 3492 d121 2cd7 a1e1 46f7 b81c  ...c4..!,...F...
+00002330: a391 8c0e 89b8 dce6 a012 0fcc 95f2 366f  ..............6o
+00002340: d6f1 c2c4 a26c ca47 555b ba83 c325 eeb1  .....l.GU[...%..
+00002350: b9c4 7024 6f43 72ae 83c3 bded d939 8a23  ..p$oCr......9.#
+00002360: a91a e273 1d1c ae6a 0fd0 511c c9ce 90a1  ...s...j..Q.....
+00002370: ebe0 703b 7b8a 8ee2 4842 86a8 5c75 b9e7  ..p;{...HB..\u..
+00002380: 8b13 9ea4 4b56 be6f e09c 06bf 6c95 a430  ....KV.o....l..0
+00002390: dd76 f453 c891 86c7 e94a f711 8d24 6488  .v.S.....J...$d.
+000023a0: d475 68f8 12db 4375 298d c746 1232 e4ea  .uh...Cu)..F.2..
+000023b0: 3a34 5cc8 9eac 6334 9290 215c d7a1 e142  :4\...c4..!\...B
+000023c0: f678 1da3 9184 0c19 baa9 7d24 c9c2 73d5  .x........}$..s.
+000023d0: 4e4d dcfa 7b64 ecf2 32bc 5294 6276 0972  NM..{d..2.R.bv.r
+000023e0: 761d 1c2e e447 d28e e148 4286 b45d 0787  v....G...HB..]..
+000023f0: 0bf9 91b7 6338 9290 2173 d7c1 e142 7ea4  ....c8..!s...B~.
+00002400: ee18 8e24 6448 de75 70b8 901f d93b 8623  ...$dH.up....;.#
+00002410: 0919 1276 5378 7881 07f0 9295 ef6b 8bd1  ...vSxx......k..
+00002420: 2250 8ae0 2548 d945 181e c22b dd07 3092  "P..%H.E...+..0.
+00002430: 8e21 87d7 81e1 3a7e 26f1 8623 23d9 18b2  .!....:~&..##...
+00002440: 781d 186e e367 1a6f 0823 c918 f278 1d18  x..n.g.o.#...x..
+00002450: 2ee3 6722 6f08 23b9 1852 7753 78a6 8387  ..g"o.#..RwSx...
+00002460: f292 a7f2 2e97 e1ef ed4a 4b63 88e5 7560  .........JKc..u`
+00002470: b889 3d98 4760 240f 4332 af03 c33d ecd9  ..=.G`$.C2...=..
+00002480: 3c02 2359 18c2 791d 186e 618f e711 18c9  <.#Y..y..na.....
+00002490: c190 cfeb c070 077b 428f c048 0686 10de  .....p.{B..H....
+000024a0: 149e 0fe0 19bd 64e5 ed7e d8ed b4ef 2740  ......d..~....'@
+000024b0: ac34 4929 bded e87d 491c 7fae 9986 484a  .4I)...}I.....HJ
+000024c0: f711 8de4 6088 eac5 b181 72bc 57e8 61bd  ....`.....r.W.a.
+000024d0: 4cc6 4692 30c4 f53a 345c c21e d863 3492  L.F.0..:4\...c4.
+000024e0: 8521 b2d7 a1e1 16f6 d01e a391 340c c1bc  .!..........4...
+000024f0: 29dc 9d84 727c 02c8 837b 8c46 f230 44f7  )...r|...{.F.0D.
+00002500: 3a34 b587 3bf3 c67f d987 cc1b 49c4 10df  :4..;.......I...
+00002510: ebd0 c0d3 1ce1 97d8 3dc0 c7c6 4632 3144  ........=...F21D
+00002520: f83a 34fc 790e 0ff1 311a 49c5 10e3 ebd0  .:4.y...1.I.....
+00002530: f027 3a3c c8c7 6824 1743 586f 0a77 8e79  .':<..h$.CXo.w.y
+00002540: 962f 7998 6f39 2da3 87f5 a538 5f82 3c5f  ./y.o9-....8_.<_
+00002550: a481 723c a73c d1c7 6824 1743 a8af 43c3  ..r<.<..h$.C..C.
+00002560: d7c3 1eeb 6334 928b 21d9 d7a1 e12e f66c  ....c4..!......l
+00002570: 1fa3 915c 0cf1 be0e 0d77 b107 fc18 8de4  ...\.....w......
+00002580: 6248 f155 bfee e79b 6c18 f28b 6f3b 78fc  bH.U....l...o;x.
+00002590: 8ae5 605f 5f0a f925 48f9 7558 f88a d8ba  ..`__..%H.uX....
+000025a0: 0fd6 1325 bbf7 fa5d 0648 fa75 68f8 92d8  ...%...].H.uh...
+000025b0: b37e c436 25bf 27d0 d4aa edd0 f035 b1e7  .~.6%.'......5..
+000025c0: fd18 8d64 6248 fc75 68f8 a2d8 337f 8c46  ...dbH.uh...3..F
+000025d0: 3231 e4fa 3a34 f074 5d78 82cd 737f d5bd  21..:4.t]x..s...
+000025e0: 787c 039b 14fb b3fb 26d5 7e5e 60c1 72fc  x|......&.~^`.r.
+000025f0: a17a 8ffd 8d59 140b 6748 fd75 586a 0b87  .z...Y..gH.uXj..
+00002600: a789 4bf7 763e 0de2 90b9 c4f8 5e9e bfdb  ..K.v>......^...
+00002610: d1fb b542 fbbc 0c96 e3fb e93c f437 1e17  ...B.......<.7..
+00002620: c5c0 1932 7f53 7b6f 15cb 614b b694 b771  ...2.S{o..aK...q
+00002630: 19de 22cb 25c6 278c 4cbd 03dc a181 0de2  ..".%.'.L.......
+00002640: 76f6 96bf eb88 4659 0de7 1211 dc3f a738  v.....FY.....?.8
+00002650: 3674 355c ba8f 6814 0767 08fd 75c6 86ae  6t5\..h..g..u...
+00002660: 864b f711 8de2 e00c a1bf 0e0d 5d0d 97ee  .K..........]...
+00002670: 231a c5c1 1942 7f53 7ba7 17cb 9d59 7c7f  #....B.S{....Y|.
+00002680: bef9 325d 075b 6bb9 c4f8 8459 5c4b b643  ..2].[k....Y\K.C
+00002690: 431d 5cfe ae32 3684 460a fd65 48f5 451a  C.\..26.F..eH.E.
+000026a0: 2847 0b7b e88f d148 1e86 d05f 8786 7bd8  (G.{...H..._..{.
+000026b0: 437f 8c46 3231 be87 2ecc 1b28 4713 7be8  C..F21.....(G.{.
+000026c0: 8fd1 482e 86d0 5f95 30ba af3f 3396 dbf5  ..H..._.0..?3...
+000026d0: 6729 9779 b3e6 d1d3 c0b9 e4f4 5e9f c598  g).y........^...
+000026e0: ea6b 7fd1 7dfb c3c6 a1fd 523e a291 5c8c  .k..}.....R>..\.
+000026f0: efa7 8b34 dcc5 9ef9 6363 23b9 18df 5317  ...4....cc#...S.
+00002700: 69b8 8b3d f2c7 6824 17e3 fbea 220d 77b1  i..=..h$....".w.
+00002710: 27fe 188d e462 7c6f 5d7b 9337 6339 ce62  '....b|o]{.7c9.b
+00002720: cf9a ccc3 cc73 2e19 3d61 1a83 6d23 0e97  .....s..=a..m#..
+00002730: f1e3 1d76 0447 7b91 1d46 fa02 0ebe e8ae  ...v.G{..F......
+00002740: 7d7a 2c7b e22f 311c 49c7 10f9 9b23 0ed7  }z,{./1.I....#..
+00002750: b147 fe28 8ee4 630c f545 1cd8 9d68 3353  .G.(..c..E...h3S
+00002760: d933 7f14 4712 3284 feaa 5f4b 7521 4339  .3..G.2..._Ku!C9
+00002770: 2e2b 3cf4 673f fa70 3de3 bba4 fb3b 04b9  .+<.g?.p=....;..
+00002780: c4f6 5e9f d8f8 debb 3856 7cad ecaf be13  ..^.....8V|.....
+00002790: e024 5de3 dbef 221c d7b5 8702 0538 c9de  .$]..."......8..
+000027a0: f80e bc08 c7ed ed29 4101 4e92 39be 092f  .......)A.N.9../
+000027b0: c271 997b 6c50 8093 dc0e 39c2 b97d ea21  .q.{lP....9..}.!
+000027c0: 6339 9e9f 8f37 3a9f 4737 dd72 0907 0aa7  c9...7:.G7.r....
+000027d0: 00c8 3bbc e61d 9286 9df3 d31f c2b0 30f7  ..;...........0.
+000027e0: 68dd 2fa5 076d e155 3fbf 1470 787a b074  h./..m.U?..pxz.t
+000027f0: 6f8f 6130 1cc9 ed90 089c 230e dd78 ce1e  o.a0......#..x..
+00002800: 18b4 3bfd e3d1 91dc 0e19 c10e 0edd 79ce  ..;...........y.
+00002810: 9e11 a438 92db 2116 d8c1 a15b cfd9 6381  ...8..!....[..c.
+00002820: 1447 b239 46fd dafb c719 cbe1 ccf2 24e0  .G.9F.........$.
+00002830: cd16 0883 ef16 2909 98e1 b576 6b38 cfa1  ......)....vk8..
+00002840: 1c4f 2c4f 029e 4fe7 d18b 544b b6ef f5d3  .O,O..O...TK....
+00002850: 1c92 801d 1af0 75d8 15f2 2420 a391 040d  ......u...$ ....
+00002860: 49c0 0e4d 2de8 783d ed49 4046 2319 1992  I..M-.x=.I@F#...
+00002870: 801d 1ad8 7d6e ef91 664f 0232 1a49 c810  ....}n..fO.2.I..
+00002880: f5eb d080 afe3 2c7e bc5a 6938 6fa4 24a0  ......,~.Zi8o.$.
+00002890: fd66 48ed e3f6 de7a 530e 5722 9e04 ccf6  .fH....zS.W"....
+000028a0: a3b8 a393 aa84 fb5e 9fc6 1005 9c23 0eac  .......^.....#..
+000028b0: b5c3 347e bcc0 8ee1 483e 862c 6007 a7f6  ..4~....H>.,`...
+000028c0: 719c c78f d7d8 311c c9c7 1006 ece0 808f  q.....1.........
+000028d0: c344 7ebc cc8e e148 3ec6 b85f fcb0 6075  .D~....H>.._..`u
+000028e0: 1d66 f2e3 8d76 0c47 5a4f c35b ed96 b015  .f...v.GZO.[....
+000028f0: 0de5 2864 0f00 aea7 ea71 17bc b153 427c  ..(d.....q...SB|
+00002900: c24c 86fb 7d91 860b d923 7f8c 4612 3284  .L..}....#..F.2.
+00002910: fc3a 63c3 85ec 213f 4623 0919 627d 1d1a  .:c...!?F#..b}..
+00002920: 2e64 8ff5 311a 49c8 f8a6 bbf8 4971 217b  .d..1.I.....Iq!{
+00002930: 908f d048 413e 7bf8 ba7e d95d d86e c520  ...HA>{..~.].n. 
+00002940: 5f10 b207 f9e6 d304 57d3 b7cb 1fef 872f  _.......W....../
+00002950: 6c97 048d d1bd 88c7 05ed c93e 094f 1236  l..........>.O.6
+00002960: be14 2fe2 7161 7bd4 4fc2 9304 8e2f ca8b  ../.qa{.O..../..
+00002970: 785c e09e fd93 f024 a143 da6f 8978 5ce8  x\.....$.C.o.x\.
+00002980: 1e06 94f0 24c1 9728 e173 3bbd 7a8b 946f  ....$..(.s;.z..o
+00002990: 3541 39de 89f0 70e0 7cda bfa8 ee7e fff0  5A9...p.|....~..
+000029a0: fdcf 6fdf 7efc fee5 c797 4fff 0700 00ff  ..o.~.....O.....
+000029b0: ff00 0000 ffff 4450 c16a c330 0cfd 15e3  ......DP.j.0....
+000029c0: fbe2 246b 5716 9240 29f4 b6d3 bec0 b3e5  ..$kW..@).......
+000029d0: d834 8e82 acb2 c2d8 bfcf e992 5607 e93d  .4..........V..=
+000029e0: 09a4 f7d4 ea2b e339 8c0c 2408 5c27 8f55  .....+.9..$.\'.U
+000029f0: 73aa f77b 296e d45c 83ed e44f b9c6 4bae  s..{)n.\...O..K.
+00002a00: d592 ca67 da66 bfb2 6f13 127f b266 5817  ...g.f..o....fX.
+00002a10: d5db a238 4ea9 b98d 64eb 4e7a e6b9 512a  ...8N...d.Nz..Q*
+00002a20: 190f 51a7 2206 4398 d071 6130 2a74 2e18  ..Q.".C..qa0*t..
+00002a30: 5069 26d0 3679 008e a3aa cbea a028 186f  Pi&.6y.......(.o
+00002a40: 35eb 7abd 73c2 c906 0e38 3d44 1fdf 776f  5.z.s....8=D..wo
+00002a50: 52f5 ad7a c8c8 f869 ae6f 673d c087 a621  R..z...i.og=...!
+00002a60: 4c49 8ce0 b893 6571 9082 c2e0 37cc 38df  LI....eq....7.8.
+00002a70: bbd9 fd17 3263 dc98 cf7a 8016 f62a 8543  ....2c...z...*.C
+00002a80: ccdf fa27 cbc1 6fa4 cb5d 6cff 0700 00ff  ...'..o..]l.....
+00002a90: ff03 0050 4b03 0414 0006 0008 0000 0021  ...PK..........!
+00002aa0: 0014 d607 8a62 0300 00f5 0b00 0014 0000  .....b..........
+00002ab0: 0078 6c2f 7368 6172 6564 5374 7269 6e67  .xl/sharedString
+00002ac0: 732e 786d 6c94 565b 6fda 3014 7e9f b4ff  s.xml.V[o.0.~...
+00002ad0: 60e5 75a4 9040 ab0a 0195 ca56 f565 1775  `.u..@.....V.e.u
+00002ae0: ddde 4d62 12ab 899d d9ce 56fe fd8e 63c8  ..Mb......V...c.
+00002af0: c5c6 a115 4fc4 e7f2 9ddb 77ce eaee b52c  ....O.....w....,
+00002b00: d05f 2224 e56c 1d44 57b3 0011 96f0 94b2  ._"$.l.DW.......
+00002b10: 6c1d fc7a 7e08 6f03 2415 6629 2e38 23eb  l..z~.o.$.f).8#.
+00002b20: e040 6470 b7f9 f861 25a5 42a0 cbe4 3ac8  .@dp...a%.B...:.
+00002b30: 95aa 96d3 a94c 7252 6279 c52b c2e0 65cf  .....LrRby.+..e.
+00002b40: 4589 15fc 15d9 5456 82e0 54e6 84a8 b298  E.....TV..T.....
+00002b50: c6b3 d9cd b4c4 9405 28e1 3553 ebe0 3a8a  ........(.5S..:.
+00002b60: 0254 33fa a726 5bf3 e5e6 36d8 ac24 ddac  .T3..&[...6..$..
+00002b70: d486 e192 aca6 6ab3 9aea ffe6 5b82 15c9  ......j.....[...
+00002b80: b8a0 44da 2fb8 d406 ecaf 5b2c 769c a194  ..D./.....[,v...
+00002b90: f257 9a92 09da 7329 6971 514a f012 494e  .W....s)iqQJ..IN
+00002ba0: 0bc4 05da 510e d149 c806 4f5e 2e69 2afe  ....Q..I..O^.i*.
+00002bb0: 2ebd 92b3 b700 eb89 bd17 59a7 ca38 0b3d  ..........Y..8.=
+00002bc0: e1e7 0517 5cd7 cd0e ef33 6554 099e 1186  ....\....3eT....
+00002bd0: 4e86 6c91 2f2a c70c 321b 4df4 2f0e 1551  N.l./*..2.M./..Q
+00002be0: 02ef 8b1a 2c86 13f4 f8b0 0da3 f902 8f6a  ....,..........j
+00002bf0: 854a d0a4 c1a0 35b6 5a65 31bb a831 f4b1  .J....5.Ze1..1..
+00002c00: 988f fa00 5cad 0f40 a971 0ada 5a68 5c46  ....\..@.q..Zh\F
+00002c10: f311 9761 7a42 1885 9d63 0335 da8d 2b0e  ...azB...c.5..+.
+00002c20: 815e c723 40e3 ce8f df66 4fa8 49b9 9374  .^.#@....fO.I..t
+00002c30: 13ce c26b 213c 261b b4c1 9f1d 4eec 0d47  ...k!<&.....N..G
+00002c40: a7ad cb83 aef7 208b a672 b137 8d71 cfef  ...... ..r.7.q..
+00002c50: b956 6960 c75e d806 3470 8cea dacb 447a  .Vi`.^..4p....Dz
+00002c60: ed8b 3427 af56 2b46 373e d9a1 e1a6 6f63  ..4'.V+F7>....oc
+00002c70: c7f0 5772 ecf6 1dcc 61d3 df9a 1e51 349b  ..Wr....a....Q4.
+00002c80: 45b6 dda1 a801 df4f b651 8ca3 0b8a fd36  E......O.Q.....6
+00002c90: 7d34 3af3 1167 ae1f 9da2 38f6 a233 0ace  }4:..g....8..3..
+00002ca0: 3038 456c c369 1b40 8fea 369c 3b83 ea48  08El.i.@..6.;..H
+00002cb0: f6a2 3625 f682 39d9 1eb6 64ec 4f51 3fa1  ..6%..9...d.OQ?.
+00002cc0: 10e7 dc1f e779 e66b b1ee dfcc abad 8a26  .....y.k.......&
+00002cd0: c496 b59e 4297 b15a 493f f3b6 220d 6bf6  ....B..ZI?..".k.
+00002ce0: ac45 feb4 0e09 f609 b8d2 9bcf 96f3 2ca6  .E............,.
+00002cf0: 1b53 18b0 953b ccdf 601f d004 355b cb36  .S...;..`...5[.6
+00002d00: a3df 9a5d d1d8 807d 6b0b fc20 c298 6f86  ...]...}k.. ..o.
+00002d10: 8d39 ef3f eb62 5f0b d48e ed19 1398 8ae5  .9.?.b_.........
+00002d20: b2e0 ff88 8085 2cb0 e2b2 ca89 20e8 13aa  ......,..... ...
+00002d30: ab0a 3e02 82ea f8cd f6de a8ea 5ad4 6287  ..>.........Z.b.
+00002d40: 1982 bf7a bd37 95cf 6996 eb73 2779 71ef  ...z.7..i..s'yq.
+00002d50: 0aed b066 b222 09dd 5392 9eb5 da59 4c0a  ...f."..S....YL.
+00002d60: 2e09 8233 2013 708f 9c97 06f8 a8e2 555d  ...3 .p.......U]
+00002d70: 6005 d717 4a09 9354 1d26 08a8 2483 fde9  `...J..T.&..$...
+00002d80: ae61 7d8a 2c97 3883 ccd7 85aa 0576 2e18  .a}.,.8......v..
+00002d90: 2301 2b9c 4056 0e36 46f3 4a59 5ac3 2bf5  #.+.@V.6F.JYZ.+.
+00002da0: 698f 04f9 7848 9bca da86 ef6b 3811 9d32  i...xH.....k8..2
+00002db0: 9a93 c096 7dd6 8781 6971 60d1 4341 5cc5  ....}...iq`.CA\.
+00002dc0: e7d3 8ef6 09b4 f372 1c95 2151 cc5d a268  .......r..!Q.].h
+00002dd0: 67d4 10b7 d390 d02d 6702 b8d7 ec5e 9d7f  g......-g....^..
+00002de0: fbfd 7d3b 417f b9ae 5d41 a081 32cc 601e  ..};A...]A..2.`.
+00002df0: 125e 56ba de4e fbd8 0728 6d1a cfc6 c170  .^V..N...(m....p
+00002e00: 5355 04e5 e3b5 48c8 7279 5ece b6d6 31cb  SU....H.ry^...1.
+00002e10: a4d5 052c 4290 44b7 56e7 660a 67fb e63f  ...,B.D.V.f.g..?
+00002e20: 0000 00ff ff03 0050 4b03 0414 0006 0008  .......PK.......
+00002e30: 0000 0021 0040 a709 045c 0100 0071 0200  ...!.@...\...q..
+00002e40: 0011 0008 0164 6f63 5072 6f70 732f 636f  .....docProps/co
+00002e50: 7265 2e78 6d6c 20a2 0401 28a0 0001 0000  re.xml ...(.....
+00002e60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002e70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002e80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002e90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002ea0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002eb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002ec0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002ed0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002ee0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002ef0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002f00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002f10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002f20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002f30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002f40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002f50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002f60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002f70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002f80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002fb0: 0000 0000 009c 934d 6fdb 300c 86ef 03f6  .......Mo.0.....
-00002fc0: 1f0c dd1b 395d 510c 81ac a248 5bf4 b0a2  ....9]Q....H[...
-00002fd0: 01e2 7667 4ea6 63a1 b264 88ac 91ec d757  ..vgN.c..d.....W
-00002fe0: b6d1 c4d9 76da 8d1f 2f5e 3ea2 2475 b36f  ....v.../^>.$u.o
-00002ff0: 5dd6 6324 1b7c 2196 8b5c 64e8 4da8 acdf  ].c$.|!..\d.M...
-00003000: 15e2 a57c b8f8 2e32 62f0 15b8 e0b1 1007  ...|...2b.......
-00003010: 2471 a3bf 7e51 9b18 3a8c 6c91 b264 e1a9  $q..~Q..:.l..d..
-00003020: 100d 73b7 9292 4c83 2dd0 22b5 7dea d421  ..s...L.-.".}..!
-00003030: b6c0 298d 3b19 eada 1abc 0be6 bd45 cff2  ..).;........E..
-00003040: 32cf af25 ee19 7d85 d545 7734 1493 e3aa  2..%..}..Ew4....
-00003050: e7ff 35ad 8219 f8e8 b53c 7409 58ab 3230  ..5......<t.X.20
-00003060: b8d2 b6a8 7325 4f89 baed 3a67 0d70 3abd  ....s%O...:g.p:.
-00003070: 7eb2 2606 0a35 674f 60ac e740 4d76 bf37  ~.&..5gO`..@Mv.7
-00003080: e894 9ccb 54e2 dfa2 798f 960f 83db 3c55  ....T...y.....<U
-00003090: 5b03 0ed7 69b4 aec1 112a 792a a847 8461  [...i....*y*.G.a
-000030a0: ad1b b091 b4ea 79d5 a3e1 1033 b2bf d362  ......y....3...b
-000030b0: 2f45 f60b 0807 e042 f410 2d78 4ee0 836c  /E.....B..-xN..l
-000030c0: 4ac6 d875 c451 ff0c f18d 1a44 2625 9360  J..u.Q.....D&%.`
-000030d0: 2a8e e15c 3b8f ed95 5e8e 8214 9c0b 0783  *..\;...^.......
-000030e0: 0924 35ce 114b cb0e e9b9 de40 e47f 102f  .$5..K.....@.../
-000030f0: e7c4 23c3 c43b e16c 07be 69e6 9c6f 3c72  ..#..;.l..i..o<r
-00003100: 9af4 87f7 3ab4 1df8 436a 1ca3 1fd6 bfd1  ....:...Cj......
-00003110: 4b57 863b 60fc 5ce7 7951 6d1b 8858 a51b  KW.;`.\.yQm..X..
-00003120: 38ae fb58 508f 6993 d10d 26eb 06fc 0eab  8..XP.i...&.....
-00003130: 4fcd df8d e119 bc4e 7f40 2faf 17f9 b73c  O......N.@/....<
-00003140: ddeb aca6 e4e9 b5eb 0f00 0000 ffff 0300  ................
-00003150: 504b 0102 2d00 1400 0600 0800 0000 2100  PK..-.........!.
-00003160: 62ee 9d68 5e01 0000 9004 0000 1300 0000  b..h^...........
-00003170: 0000 0000 0000 0000 0000 0000 0000 5b43  ..............[C
-00003180: 6f6e 7465 6e74 5f54 7970 6573 5d2e 786d  ontent_Types].xm
-00003190: 6c50 4b01 022d 0014 0006 0008 0000 0021  lPK..-.........!
-000031a0: 00b5 5530 23f4 0000 004c 0200 000b 0000  ..U0#....L......
-000031b0: 0000 0000 0000 0000 0000 0097 0300 005f  ..............._
-000031c0: 7265 6c73 2f2e 7265 6c73 504b 0102 2d00  rels/.relsPK..-.
-000031d0: 1400 0600 0800 0000 2100 813e 9497 f300  ........!..>....
-000031e0: 0000 ba02 0000 1a00 0000 0000 0000 0000  ................
-000031f0: 0000 0000 bc06 0000 786c 2f5f 7265 6c73  ........xl/_rels
-00003200: 2f77 6f72 6b62 6f6f 6b2e 786d 6c2e 7265  /workbook.xml.re
-00003210: 6c73 504b 0102 2d00 1400 0600 0800 0000  lsPK..-.........
-00003220: 2100 d48d b40e 0203 0000 0907 0000 0f00  !...............
-00003230: 0000 0000 0000 0000 0000 0000 ef08 0000  ................
-00003240: 786c 2f77 6f72 6b62 6f6f 6b2e 786d 6c50  xl/workbook.xmlP
-00003250: 4b01 022d 0014 0006 0008 0000 0021 0027  K..-.........!.'
-00003260: 96d6 b5ca 0200 000a 0700 000d 0000 0000  ................
-00003270: 0000 0000 0000 0000 001e 0c00 0078 6c2f  .............xl/
-00003280: 7374 796c 6573 2e78 6d6c 504b 0102 2d00  styles.xmlPK..-.
-00003290: 1400 0600 0800 0000 2100 c117 10be 4e07  ........!.....N.
-000032a0: 0000 c620 0000 1300 0000 0000 0000 0000  ... ............
-000032b0: 0000 0000 130f 0000 786c 2f74 6865 6d65  ........xl/theme
-000032c0: 2f74 6865 6d65 312e 786d 6c50 4b01 022d  /theme1.xmlPK..-
-000032d0: 0014 0006 0008 0000 0021 000b 0422 b9b0  .........!..."..
-000032e0: 1100 00e0 8700 0018 0000 0000 0000 0000  ................
-000032f0: 0000 0000 0092 1600 0078 6c2f 776f 726b  .........xl/work
-00003300: 7368 6565 7473 2f73 6865 6574 312e 786d  sheets/sheet1.xm
-00003310: 6c50 4b01 022d 0014 0006 0008 0000 0021  lPK..-.........!
-00003320: 0091 d754 d344 0300 0072 0b00 0014 0000  ...T.D...r......
-00003330: 0000 0000 0000 0000 0000 0078 2800 0078  ...........x(..x
-00003340: 6c2f 7368 6172 6564 5374 7269 6e67 732e  l/sharedStrings.
-00003350: 786d 6c50 4b01 022d 0014 0006 0008 0000  xmlPK..-........
-00003360: 0021 003a bef8 905a 0100 0071 0200 0011  .!.:...Z...q....
-00003370: 0000 0000 0000 0000 0000 0000 00ee 2b00  ..............+.
-00003380: 0064 6f63 5072 6f70 732f 636f 7265 2e78  .docProps/core.x
-00003390: 6d6c 504b 0102 2d00 1400 0600 0800 0000  mlPK..-.........
-000033a0: 2100 e4ee 6155 9b01 0000 3303 0000 1000  !...aU....3.....
-000033b0: 0000 0000 0000 0000 0000 0000 7f2e 0000  ................
-000033c0: 646f 6350 726f 7073 2f61 7070 2e78 6d6c  docProps/app.xml
-000033d0: 504b 0506 0000 0000 0a00 0a00 8002 0000  PK..............
-000033e0: 5031 0000 0000                           P1....
+00002f50: 0000 0000 0000 0000 0000 0000 0000 7c92  ..............|.
+00002f60: 514b c330 1485 df05 ff43 c97b 9ba6 63d3  QK.0.....C.{..c.
+00002f70: 85b6 0327 7b72 28d8 a1f8 1692 db2d d826  ...'{r(......-.&
+00002f80: 25c9 dcf6 ef4d dbad 7628 3ee6 9e93 2fe7  %....M..v(>.../.
+00002f90: 5c92 2e8e 7515 7c81 b152 ab0c 9128 4601  \...u.|..R...(F.
+00002fa0: 28ae 8554 db0c 6d8a 5578 8f02 eb98 12ac  (..T..m.Ux......
+00002fb0: d20a 3274 028b 16f9 ed4d ca1b cab5 8117  ..2t.....M......
+00002fc0: a31b 304e 820d 3c49 59ca 9b0c ed9c 6b28  ..0N..<IY.....k(
+00002fd0: c696 efa0 6636 f20e e5c5 529b 9a39 7f34  ....f6....R..9.4
+00002fe0: 5bdc 30fe c9b6 8093 389e e11a 1c13 cc31  [.0.....8......1
+00002ff0: dc02 c366 20a2 3352 f001 d9ec 4dd5 0104  ...f .3R....M...
+00003000: c750 410d ca59 4c22 827f bc0e 4c6d ffbc  .PA..YL"....Lm..
+00003010: d029 2367 2ddd a9f1 9dce 71c7 6cc1 7b71  .)#g-.....q.l.{q
+00003020: 701f ad1c 8c87 c321 3a4c ba18 3e3f c1ef  p......!:L..>?..
+00003030: eba7 d7ae 6a28 55bb 2b0e 284f 05a7 dc00  ....j(U.+.(O....
+00003040: 73da e4cb 9d91 3658 ef1d 5429 1ecd db1d  s.....6X..T)....
+00003050: 56cc bab5 5f77 2941 3c9c f2b5 e446 5b5d  V..._w)A<....F[]
+00003060: bae0 b92c 2587 6063 c1a4 f8b7 d1f3 bb3a  ...,%.`c.......:
+00003070: fd23 2002 1f90 f675 2eca db64 f958 ac50  .# ....u...d.X.P
+00003080: 9ec4 0909 e324 4c92 22be a753 42a7 f38f  .....$L."..SB...
+00003090: 36c7 d5fd 3670 3fa8 cf69 fe27 4ec2 781a  6...6p?..i.'N.x.
+000030a0: 9259 11cf 29b9 a364 3622 5e00 7997 fbfa  .Y..)..d6"^.y...
+000030b0: 93e4 df00 0000 ffff 0300 504b 0304 1400  ..........PK....
+000030c0: 0600 0800 0000 2100 e4ee 6155 9b01 0000  ......!...aU....
+000030d0: 3303 0000 1000 0801 646f 6350 726f 7073  3.......docProps
+000030e0: 2f61 7070 2e78 6d6c 20a2 0401 28a0 0001  /app.xml ...(...
+000030f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003100: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003110: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003120: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003130: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003140: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003150: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003160: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003170: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003180: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003190: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000031a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000031b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000031c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000031d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000031e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000031f0: 9c93 4d6f db30 0c86 ef03 f61f 0cdd 1b39  ..Mo.0.........9
+00003200: 5d51 0c81 aca2 485b f4b0 a201 e276 674e  ]Q....H[.....vgN
+00003210: a663 a1b2 6488 ac91 ecd7 57b6 d1c4 d976  .c..d.....W....v
+00003220: da8d 1f2f 5e3e a224 75b3 6f5d d663 241b  .../^>.$u.o].c$.
+00003230: 7c21 968b 5c64 e84d a8ac df15 e2a5 7cb8  |!..\d.M......|.
+00003240: f82e 3262 f015 b8e0 b110 0724 71a3 bf7e  ..2b.......$q..~
+00003250: 519b 183a 8c6c 91b2 64e1 a910 0d73 b792  Q..:.l..d....s..
+00003260: 924c 832d d022 b57d ead4 21b6 c029 8d3b  .L.-.".}..!..).;
+00003270: 19ea da1a bc0b e6bd 45cf f232 cfaf 25ee  ........E..2..%.
+00003280: 197d 85d5 4577 3414 93e3 aae7 ff35 ad82  .}..Ew4......5..
+00003290: 19f8 e8b5 3c74 0958 ab32 30b8 d2b6 a873  ....<t.X.20....s
+000032a0: 254f 89ba ed3a 670d 703a bd7e b226 060a  %O...:g.p:.~.&..
+000032b0: 3567 4f60 ace7 404d 76bf 37e8 949c cb54  5gO`..@Mv.7....T
+000032c0: e2df a279 8f96 0f83 db3c 555b 030e d769  ...y.....<U[...i
+000032d0: b4ae c111 2a79 2aa8 4784 61ad 1bb0 91b4  ....*y*.G.a.....
+000032e0: ea79 d5a3 e110 33b2 bfd3 622f 45f6 0b08  .y....3...b/E...
+000032f0: 07e0 42f4 102d 784e e083 6c4a c6d8 75c4  ..B..-xN..lJ..u.
+00003300: 51ff 0cf1 8d1a 4426 2593 602a 8ee1 5c3b  Q.....D&%.`*..\;
+00003310: 8fed 955e 8e82 149c 0b07 8309 2435 ce11  ...^........$5..
+00003320: 4bcb 0ee9 b9de 40e4 7f10 2fe7 c423 c3c4  K.....@.../..#..
+00003330: 3be1 6c07 be69 e69c 6f3c 729a f487 f73a  ;.l..i..o<r....:
+00003340: b41d f843 6a1c a31f d6bf d14b 5786 3b60  ...Cj......KW.;`
+00003350: fc5c e779 516d 1b88 58a5 1b38 aefb 5850  .\.yQm..X..8..XP
+00003360: 8f69 93d1 0d26 eb06 fc0e ab4f cddf 8de1  .i...&.....O....
+00003370: 19bc 4e7f 402f af17 f9b7 3cdd ebac a6e4  ..N.@/....<.....
+00003380: e9b5 eb0f 0000 00ff ff03 0050 4b01 022d  ...........PK..-
+00003390: 0014 0006 0008 0000 0021 0062 ee9d 685e  .........!.b..h^
+000033a0: 0100 0090 0400 0013 0000 0000 0000 0000  ................
+000033b0: 0000 0000 0000 0000 005b 436f 6e74 656e  .........[Conten
+000033c0: 745f 5479 7065 735d 2e78 6d6c 504b 0102  t_Types].xmlPK..
+000033d0: 2d00 1400 0600 0800 0000 2100 b555 3023  -.........!..U0#
+000033e0: f400 0000 4c02 0000 0b00 0000 0000 0000  ....L...........
+000033f0: 0000 0000 0000 9703 0000 5f72 656c 732f  .........._rels/
+00003400: 2e72 656c 7350 4b01 022d 0014 0006 0008  .relsPK..-......
+00003410: 0000 0021 0081 3e94 97f3 0000 00ba 0200  ...!..>.........
+00003420: 001a 0000 0000 0000 0000 0000 0000 00bc  ................
+00003430: 0600 0078 6c2f 5f72 656c 732f 776f 726b  ...xl/_rels/work
+00003440: 626f 6f6b 2e78 6d6c 2e72 656c 7350 4b01  book.xml.relsPK.
+00003450: 022d 0014 0006 0008 0000 0021 002e b1ce  .-.........!....
+00003460: 08bd 0300 006e 0900 000f 0000 0000 0000  .....n..........
+00003470: 0000 0000 0000 00ef 0800 0078 6c2f 776f  ...........xl/wo
+00003480: 726b 626f 6f6b 2e78 6d6c 504b 0102 2d00  rkbook.xmlPK..-.
+00003490: 1400 0600 0800 0000 2100 2796 d6b5 ca02  ........!.'.....
+000034a0: 0000 0a07 0000 0d00 0000 0000 0000 0000  ................
+000034b0: 0000 0000 d90c 0000 786c 2f73 7479 6c65  ........xl/style
+000034c0: 732e 786d 6c50 4b01 022d 0014 0006 0008  s.xmlPK..-......
+000034d0: 0000 0021 00c1 1710 be4e 0700 00c6 2000  ...!.....N.... .
+000034e0: 0013 0000 0000 0000 0000 0000 0000 00ce  ................
+000034f0: 0f00 0078 6c2f 7468 656d 652f 7468 656d  ...xl/theme/them
+00003500: 6531 2e78 6d6c 504b 0102 2d00 1400 0600  e1.xmlPK..-.....
+00003510: 0800 0000 2100 ae18 fb4a 1013 0000 6293  ....!....J....b.
+00003520: 0000 1800 0000 0000 0000 0000 0000 0000  ................
+00003530: 4d17 0000 786c 2f77 6f72 6b73 6865 6574  M...xl/worksheet
+00003540: 732f 7368 6565 7431 2e78 6d6c 504b 0102  s/sheet1.xmlPK..
+00003550: 2d00 1400 0600 0800 0000 2100 14d6 078a  -.........!.....
+00003560: 6203 0000 f50b 0000 1400 0000 0000 0000  b...............
+00003570: 0000 0000 0000 932a 0000 786c 2f73 6861  .......*..xl/sha
+00003580: 7265 6453 7472 696e 6773 2e78 6d6c 504b  redStrings.xmlPK
+00003590: 0102 2d00 1400 0600 0800 0000 2100 40a7  ..-.........!.@.
+000035a0: 0904 5c01 0000 7102 0000 1100 0000 0000  ..\...q.........
+000035b0: 0000 0000 0000 0000 272e 0000 646f 6350  ........'...docP
+000035c0: 726f 7073 2f63 6f72 652e 786d 6c50 4b01  rops/core.xmlPK.
+000035d0: 022d 0014 0006 0008 0000 0021 00e4 ee61  .-.........!...a
+000035e0: 559b 0100 0033 0300 0010 0000 0000 0000  U....3..........
+000035f0: 0000 0000 0000 00ba 3000 0064 6f63 5072  ........0..docPr
+00003600: 6f70 732f 6170 702e 786d 6c50 4b05 0600  ops/app.xmlPK...
+00003610: 0000 000a 000a 0080 0200 008b 3300 0000  ............3...
+00003620: 00                                       .
```

### Comparing `premise_gwp-0.8/premise_gwp.egg-info/PKG-INFO` & `premise_gwp-0.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: premise-gwp
-Version: 0.8
+Name: premise_gwp
+Version: 0.9
 Summary: Import IPCC's GWP100a method, with biogenic CO2 CFs, into Brightway2
 Home-page: https://github.com/romainsacchi/premise_gwp
 Author: Romain Sacchi
 Author-email: romain.sacchi@psi.ch
 License: BSD 3-clause
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
@@ -32,33 +32,35 @@
 Without it, negative emission technologies (NET) do not yield a net negative
 carbon footprint.
 
 ## Impact category
 
 This adds:
 
-* IPCC 2013, climate change, GWP 100a, with hydrogen
+* IPCC 2013 and 2021, climate change, GWP 100a, with hydrogen
   * "Hydrogen", with a CF of 33 and 11 for GWP20 and GWP100 respectively.
   
-* IPCC 2013, climate change, GWP 100a, with hydrogen and bio CO2
+* IPCC 2013 and 2021, climate change, GWP 100a, with hydrogen and bio CO2
   * "Hydrogen", with a CF of 33 and 11 for GWP20 and GWP100 respectively.
   * "Carbon dioxide, in air", with a CF of -1
   * "Carbon dioxide, non-fossil, resource correction", with a CF of -1
   * "Carbon dioxide, non-fossil", with a CF of +1
 
 The biogenic carbon balance in the rest of the ecoinvent database should be correct.
-Hence, using this method, instead of the regular IPCC 2013 GWP100a method, should not
+Hence, using this method, instead of the regular IPCC GWP method, should not
 yield any difference, as long as BECCS are not present and solicited in the database.
 
 The characterization factors for the global warming impact GWP100a of for hydrogen 
 is taken from [Warwick et al, 2022](https://assets.publishing.service.gov.uk/government/uploads/system/uploads/attachment_data/file/1067144/atmospheric-implications-of-increased-hydrogen-use.pdf).
 
 ## Limitation
 
-Only works with ``bw2io 0.8.7`` or earlier (until ecoinvent v.3.8).
+Now works with ``bw2io 0.8.7`` and ``bw2io 0.8.8``. 
+If ``bw2io 0.8.8`` is present, IPCC 2021 methods will be
+installed, otherwise IPCC 2013 methods will be installed.
 
 ## Usage
 
 In an open Brightway2 project:
 ```python
 from premise_gwp import add_premise_gwp
 add_premise_gwp()
```

### Comparing `premise_gwp-0.8/premise_gwp.egg-info/SOURCES.txt` & `premise_gwp-0.9/premise_gwp.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 premise_gwp/biosphere.py
 premise_gwp/version.py
 premise_gwp.egg-info/PKG-INFO
 premise_gwp.egg-info/SOURCES.txt
 premise_gwp.egg-info/dependency_links.txt
 premise_gwp.egg-info/requires.txt
 premise_gwp.egg-info/top_level.txt
-premise_gwp/data/LCIA_Implementation_3.8.xlsx
-premise_gwp/data/lcia_gtp_100a_w_bio.xlsx
-premise_gwp/data/lcia_gtp_20a_w_bio.xlsx
+premise_gwp/data/lcia_gwp2021_100a.xlsx
+premise_gwp/data/lcia_gwp2021_100a_w_bio.xlsx
+premise_gwp/data/lcia_gwp2021_20a.xlsx
+premise_gwp/data/lcia_gwp2021_20a_w_bio.xlsx
 premise_gwp/data/lcia_gwp_100a.xlsx
 premise_gwp/data/lcia_gwp_100a_w_bio.xlsx
 premise_gwp/data/lcia_gwp_20a.xlsx
 premise_gwp/data/lcia_gwp_20a_w_bio.xlsx
 tests/test_implementation.py
```

### Comparing `premise_gwp-0.8/setup.py` & `premise_gwp-0.9/setup.py`

 * *Files identical despite different names*

### Comparing `premise_gwp-0.8/tests/test_implementation.py` & `premise_gwp-0.9/tests/test_implementation.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     bw2data.projects.set_current("test")
     bw2io.create_default_biosphere3()
 
     add_premise_gwp()
 
     # check that the new method exists
-    new_method = ("IPCC 2013", "climate change", "GWP 20a, incl. H and bio CO2")
+    new_method = ("IPCC 2013", "climate change", "GWP 100a, incl. H and bio CO2")
     assert new_method in bw2data.methods
 
     # check that "Carbon dioxide, in air" has now a CF of -1
 
     co2_in_air = [
         f
         for f in bw2data.Database("biosphere3")
```

