# Comparing `tmp/pydisadm-1.0.2.tar.gz` & `tmp/pydisadm-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydisadm-1.0.2.tar", max compression
+gzip compressed data, was "pydisadm-1.0.3.tar", max compression
```

## Comparing `pydisadm-1.0.2.tar` & `pydisadm-1.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1604 2023-05-16 12:46:29.277105 pydisadm-1.0.2/README.md
--rw-r--r--   0        0        0      111 2023-05-16 12:46:29.281106 pydisadm-1.0.2/pydisadm/__init__.py
--rw-r--r--   0        0        0     1165 2023-05-16 12:46:29.281106 pydisadm-1.0.2/pydisadm/__main__.py
--rw-r--r--   0        0        0     1120 2023-05-16 12:46:29.281106 pydisadm-1.0.2/pydisadm/bot/adm_bot.py
--rw-r--r--   0        0        0     5874 2023-05-16 12:46:29.281106 pydisadm-1.0.2/pydisadm/bot/adm_cog.py
--rw-r--r--   0        0        0      539 2023-05-16 12:46:29.281106 pydisadm-1.0.2/pydisadm/bot/utils.py
--rw-r--r--   0        0        0      649 2023-05-16 12:46:29.281106 pydisadm-1.0.2/pydisadm/configuration.py
--rw-r--r--   0        0        0     6012 2023-05-16 12:46:29.281106 pydisadm-1.0.2/pydisadm/controller/adm_controller.py
--rw-r--r--   0        0        0   368313 2023-05-16 12:46:29.281106 pydisadm-1.0.2/pydisadm/data/mapConstellations.csv
--rw-r--r--   0        0        0    34613 2023-05-16 12:46:29.281106 pydisadm-1.0.2/pydisadm/data/mapRegions.csv
--rw-r--r--   0        0        0  3277768 2023-05-16 12:46:29.301106 pydisadm-1.0.2/pydisadm/data/mapSolarSystems.csv
--rw-r--r--   0        0        0      441 2023-05-16 12:46:29.301106 pydisadm-1.0.2/pydisadm/loader/datasets.py
--rw-r--r--   0        0        0      940 2023-05-16 12:46:29.301106 pydisadm-1.0.2/pydisadm/loader/static_data.py
--rw-r--r--   0        0        0      947 2023-05-16 12:46:29.301106 pydisadm-1.0.2/pydisadm/runnable/runnable_refresh.py
--rw-r--r--   0        0        0     2976 2023-05-16 12:46:29.301106 pydisadm-1.0.2/pydisadm/services/database.py
--rw-r--r--   0        0        0     1164 2023-05-16 12:46:29.301106 pydisadm-1.0.2/pydisadm/services/esi.py
--rw-r--r--   0        0        0      372 2023-05-16 12:46:29.301106 pydisadm-1.0.2/pydisadm/utils/datetime_utils.py
--rw-r--r--   0        0        0      521 2023-05-16 12:46:29.301106 pydisadm-1.0.2/pydisadm/utils/plot_utils.py
--rw-r--r--   0        0        0      120 2023-05-16 12:46:29.301106 pydisadm-1.0.2/pydisadm/utils/thread_utils.py
--rw-r--r--   0        0        0      844 2023-05-16 12:47:05.821468 pydisadm-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     2354 1970-01-01 00:00:00.000000 pydisadm-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1604 2023-05-16 12:50:44.538318 pydisadm-1.0.3/README.md
+-rw-r--r--   0        0        0      111 2023-05-16 12:50:44.542318 pydisadm-1.0.3/pydisadm/__init__.py
+-rw-r--r--   0        0        0     1165 2023-05-16 12:50:44.542318 pydisadm-1.0.3/pydisadm/__main__.py
+-rw-r--r--   0        0        0     1120 2023-05-16 12:50:44.542318 pydisadm-1.0.3/pydisadm/bot/adm_bot.py
+-rw-r--r--   0        0        0     5874 2023-05-16 12:50:44.542318 pydisadm-1.0.3/pydisadm/bot/adm_cog.py
+-rw-r--r--   0        0        0      539 2023-05-16 12:50:44.542318 pydisadm-1.0.3/pydisadm/bot/utils.py
+-rw-r--r--   0        0        0      649 2023-05-16 12:50:44.542318 pydisadm-1.0.3/pydisadm/configuration.py
+-rw-r--r--   0        0        0     6012 2023-05-16 12:50:44.542318 pydisadm-1.0.3/pydisadm/controller/adm_controller.py
+-rw-r--r--   0        0        0   368313 2023-05-16 12:50:44.542318 pydisadm-1.0.3/pydisadm/data/mapConstellations.csv
+-rw-r--r--   0        0        0    34613 2023-05-16 12:50:44.542318 pydisadm-1.0.3/pydisadm/data/mapRegions.csv
+-rw-r--r--   0        0        0  3277768 2023-05-16 12:50:44.558319 pydisadm-1.0.3/pydisadm/data/mapSolarSystems.csv
+-rw-r--r--   0        0        0      441 2023-05-16 12:50:44.558319 pydisadm-1.0.3/pydisadm/loader/datasets.py
+-rw-r--r--   0        0        0      940 2023-05-16 12:50:44.558319 pydisadm-1.0.3/pydisadm/loader/static_data.py
+-rw-r--r--   0        0        0      947 2023-05-16 12:50:44.558319 pydisadm-1.0.3/pydisadm/runnable/runnable_refresh.py
+-rw-r--r--   0        0        0     2976 2023-05-16 12:50:44.558319 pydisadm-1.0.3/pydisadm/services/database.py
+-rw-r--r--   0        0        0     1164 2023-05-16 12:50:44.558319 pydisadm-1.0.3/pydisadm/services/esi.py
+-rw-r--r--   0        0        0      372 2023-05-16 12:50:44.558319 pydisadm-1.0.3/pydisadm/utils/datetime_utils.py
+-rw-r--r--   0        0        0      521 2023-05-16 12:50:44.558319 pydisadm-1.0.3/pydisadm/utils/plot_utils.py
+-rw-r--r--   0        0        0      120 2023-05-16 12:50:44.558319 pydisadm-1.0.3/pydisadm/utils/thread_utils.py
+-rw-r--r--   0        0        0      894 2023-05-16 12:51:19.323909 pydisadm-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2460 1970-01-01 00:00:00.000000 pydisadm-1.0.3/PKG-INFO
```

### Comparing `pydisadm-1.0.2/README.md` & `pydisadm-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pydisadm-1.0.2/pydisadm/__main__.py` & `pydisadm-1.0.3/pydisadm/__main__.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.0.2/pydisadm/bot/adm_bot.py` & `pydisadm-1.0.3/pydisadm/bot/adm_bot.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.0.2/pydisadm/bot/adm_cog.py` & `pydisadm-1.0.3/pydisadm/bot/adm_cog.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.0.2/pydisadm/bot/utils.py` & `pydisadm-1.0.3/pydisadm/bot/utils.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.0.2/pydisadm/configuration.py` & `pydisadm-1.0.3/pydisadm/configuration.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.0.2/pydisadm/controller/adm_controller.py` & `pydisadm-1.0.3/pydisadm/controller/adm_controller.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.0.2/pydisadm/data/mapConstellations.csv` & `pydisadm-1.0.3/pydisadm/data/mapConstellations.csv`

 * *Files identical despite different names*

### Comparing `pydisadm-1.0.2/pydisadm/data/mapRegions.csv` & `pydisadm-1.0.3/pydisadm/data/mapRegions.csv`

 * *Files identical despite different names*

### Comparing `pydisadm-1.0.2/pydisadm/data/mapSolarSystems.csv` & `pydisadm-1.0.3/pydisadm/data/mapSolarSystems.csv`

 * *Files identical despite different names*

### Comparing `pydisadm-1.0.2/pydisadm/loader/static_data.py` & `pydisadm-1.0.3/pydisadm/loader/static_data.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.0.2/pydisadm/runnable/runnable_refresh.py` & `pydisadm-1.0.3/pydisadm/runnable/runnable_refresh.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.0.2/pydisadm/services/database.py` & `pydisadm-1.0.3/pydisadm/services/database.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.0.2/pydisadm/services/esi.py` & `pydisadm-1.0.3/pydisadm/services/esi.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.0.2/pydisadm/utils/plot_utils.py` & `pydisadm-1.0.3/pydisadm/utils/plot_utils.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.0.2/pyproject.toml` & `pydisadm-1.0.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 [tool.poetry]
 name = "pydisadm"
-version = "1.0.2"
+version = "1.0.3"
 description = "A Discord bot providing ADM summaries."
+repository = "https://github.com/agelito/adm-bot"
 authors = ["Axel Wettervik"]
 license = "MIT"
 readme = "README.md"
 include = ["data/*.csv"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `pydisadm-1.0.2/PKG-INFO` & `pydisadm-1.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: pydisadm
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Discord bot providing ADM summaries.
+Home-page: https://github.com/agelito/adm-bot
 License: MIT
 Author: Axel Wettervik
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -13,14 +14,15 @@
 Requires-Dist: discord (>=2.2.3,<3.0.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: pandas (>=2.0.1,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: requests (>=2.30.0,<3.0.0)
 Requires-Dist: schedule (>=1.2.0,<2.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
+Project-URL: Repository, https://github.com/agelito/adm-bot
 Description-Content-Type: text/markdown
 
 # EVE ADM Bot
 
 This is a discord bot which will collect alliance system ADM's daily and provide commands to display them in a convenient tier list.
 
 ## ⚡ Quick Start
```

