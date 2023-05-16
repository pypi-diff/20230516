# Comparing `tmp/pydisadm-1.0.3.tar.gz` & `tmp/pydisadm-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydisadm-1.0.3.tar", max compression
+gzip compressed data, was "pydisadm-1.0.4.tar", max compression
```

## Comparing `pydisadm-1.0.3.tar` & `pydisadm-1.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1604 2023-05-16 12:50:44.538318 pydisadm-1.0.3/README.md
--rw-r--r--   0        0        0      111 2023-05-16 12:50:44.542318 pydisadm-1.0.3/pydisadm/__init__.py
--rw-r--r--   0        0        0     1165 2023-05-16 12:50:44.542318 pydisadm-1.0.3/pydisadm/__main__.py
--rw-r--r--   0        0        0     1120 2023-05-16 12:50:44.542318 pydisadm-1.0.3/pydisadm/bot/adm_bot.py
--rw-r--r--   0        0        0     5874 2023-05-16 12:50:44.542318 pydisadm-1.0.3/pydisadm/bot/adm_cog.py
--rw-r--r--   0        0        0      539 2023-05-16 12:50:44.542318 pydisadm-1.0.3/pydisadm/bot/utils.py
--rw-r--r--   0        0        0      649 2023-05-16 12:50:44.542318 pydisadm-1.0.3/pydisadm/configuration.py
--rw-r--r--   0        0        0     6012 2023-05-16 12:50:44.542318 pydisadm-1.0.3/pydisadm/controller/adm_controller.py
--rw-r--r--   0        0        0   368313 2023-05-16 12:50:44.542318 pydisadm-1.0.3/pydisadm/data/mapConstellations.csv
--rw-r--r--   0        0        0    34613 2023-05-16 12:50:44.542318 pydisadm-1.0.3/pydisadm/data/mapRegions.csv
--rw-r--r--   0        0        0  3277768 2023-05-16 12:50:44.558319 pydisadm-1.0.3/pydisadm/data/mapSolarSystems.csv
--rw-r--r--   0        0        0      441 2023-05-16 12:50:44.558319 pydisadm-1.0.3/pydisadm/loader/datasets.py
--rw-r--r--   0        0        0      940 2023-05-16 12:50:44.558319 pydisadm-1.0.3/pydisadm/loader/static_data.py
--rw-r--r--   0        0        0      947 2023-05-16 12:50:44.558319 pydisadm-1.0.3/pydisadm/runnable/runnable_refresh.py
--rw-r--r--   0        0        0     2976 2023-05-16 12:50:44.558319 pydisadm-1.0.3/pydisadm/services/database.py
--rw-r--r--   0        0        0     1164 2023-05-16 12:50:44.558319 pydisadm-1.0.3/pydisadm/services/esi.py
--rw-r--r--   0        0        0      372 2023-05-16 12:50:44.558319 pydisadm-1.0.3/pydisadm/utils/datetime_utils.py
--rw-r--r--   0        0        0      521 2023-05-16 12:50:44.558319 pydisadm-1.0.3/pydisadm/utils/plot_utils.py
--rw-r--r--   0        0        0      120 2023-05-16 12:50:44.558319 pydisadm-1.0.3/pydisadm/utils/thread_utils.py
--rw-r--r--   0        0        0      894 2023-05-16 12:51:19.323909 pydisadm-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     2460 1970-01-01 00:00:00.000000 pydisadm-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1901 2023-05-16 13:03:25.584071 pydisadm-1.0.4/README.md
+-rw-r--r--   0        0        0      111 2023-05-16 13:03:25.584071 pydisadm-1.0.4/pydisadm/__init__.py
+-rw-r--r--   0        0        0     1165 2023-05-16 13:03:25.584071 pydisadm-1.0.4/pydisadm/__main__.py
+-rw-r--r--   0        0        0     1120 2023-05-16 13:03:25.584071 pydisadm-1.0.4/pydisadm/bot/adm_bot.py
+-rw-r--r--   0        0        0     5874 2023-05-16 13:03:25.584071 pydisadm-1.0.4/pydisadm/bot/adm_cog.py
+-rw-r--r--   0        0        0      539 2023-05-16 13:03:25.584071 pydisadm-1.0.4/pydisadm/bot/utils.py
+-rw-r--r--   0        0        0      649 2023-05-16 13:03:25.584071 pydisadm-1.0.4/pydisadm/configuration.py
+-rw-r--r--   0        0        0     6012 2023-05-16 13:03:25.584071 pydisadm-1.0.4/pydisadm/controller/adm_controller.py
+-rw-r--r--   0        0        0   368313 2023-05-16 13:03:25.588071 pydisadm-1.0.4/pydisadm/data/mapConstellations.csv
+-rw-r--r--   0        0        0    34613 2023-05-16 13:03:25.588071 pydisadm-1.0.4/pydisadm/data/mapRegions.csv
+-rw-r--r--   0        0        0  3277768 2023-05-16 13:03:25.608073 pydisadm-1.0.4/pydisadm/data/mapSolarSystems.csv
+-rw-r--r--   0        0        0      441 2023-05-16 13:03:25.608073 pydisadm-1.0.4/pydisadm/loader/datasets.py
+-rw-r--r--   0        0        0      940 2023-05-16 13:03:25.608073 pydisadm-1.0.4/pydisadm/loader/static_data.py
+-rw-r--r--   0        0        0      947 2023-05-16 13:03:25.608073 pydisadm-1.0.4/pydisadm/runnable/runnable_refresh.py
+-rw-r--r--   0        0        0     2976 2023-05-16 13:03:25.608073 pydisadm-1.0.4/pydisadm/services/database.py
+-rw-r--r--   0        0        0     1164 2023-05-16 13:03:25.608073 pydisadm-1.0.4/pydisadm/services/esi.py
+-rw-r--r--   0        0        0      372 2023-05-16 13:03:25.608073 pydisadm-1.0.4/pydisadm/utils/datetime_utils.py
+-rw-r--r--   0        0        0      521 2023-05-16 13:03:25.608073 pydisadm-1.0.4/pydisadm/utils/plot_utils.py
+-rw-r--r--   0        0        0      120 2023-05-16 13:03:25.608073 pydisadm-1.0.4/pydisadm/utils/thread_utils.py
+-rw-r--r--   0        0        0      894 2023-05-16 13:04:00.867222 pydisadm-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2757 1970-01-01 00:00:00.000000 pydisadm-1.0.4/PKG-INFO
```

### Comparing `pydisadm-1.0.3/README.md` & `pydisadm-1.0.4/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,41 @@
 # EVE ADM Bot
 
 This is a discord bot which will collect alliance system ADM's daily and provide commands to display them in a convenient tier list.
 
 ## ⚡ Quick Start
 
-### Using pip
+### From PyPI
 ```shell
-# Edit variables in .env
-cp .env.example .env
+# 1. Set up environment
+export DISCORD_TOKEN=your-token-here
+export DISCORD_CHANNEL=your-channel-here
+export DISCORD_APP_ID=your-app-id-here
+export ALLIANCE_ID=your-alliance-id-here
 
+# 2. Install package from PyPI
 pip install pydisadm
 
+# 3. Run Bot
 python -m pydisadm
 ```
 
-### Using poetry
+### From source
 ```shell
-# Edit variables in .env
+# 1. Clone repository
+git clone https://github.com/agelito/adm-bot
+cd adm-bot
+
+# 2. Copy and edit .env
 cp .env.example .env
 
+# 3. Install dependencies
 poetry install
+
+# 4. Run bot
 poetry run python pydisadm/__main__.py
 ```
 
 ## 📃 Commands
 
 - `/adm summary` - send a summary of ADM's
 - `/adm csv` - send a csv of ADM's
```

### Comparing `pydisadm-1.0.3/pydisadm/__main__.py` & `pydisadm-1.0.4/pydisadm/__main__.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.0.3/pydisadm/bot/adm_bot.py` & `pydisadm-1.0.4/pydisadm/bot/adm_bot.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.0.3/pydisadm/bot/adm_cog.py` & `pydisadm-1.0.4/pydisadm/bot/adm_cog.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.0.3/pydisadm/bot/utils.py` & `pydisadm-1.0.4/pydisadm/bot/utils.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.0.3/pydisadm/configuration.py` & `pydisadm-1.0.4/pydisadm/configuration.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.0.3/pydisadm/controller/adm_controller.py` & `pydisadm-1.0.4/pydisadm/controller/adm_controller.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.0.3/pydisadm/data/mapConstellations.csv` & `pydisadm-1.0.4/pydisadm/data/mapConstellations.csv`

 * *Files identical despite different names*

### Comparing `pydisadm-1.0.3/pydisadm/data/mapRegions.csv` & `pydisadm-1.0.4/pydisadm/data/mapRegions.csv`

 * *Files identical despite different names*

### Comparing `pydisadm-1.0.3/pydisadm/data/mapSolarSystems.csv` & `pydisadm-1.0.4/pydisadm/data/mapSolarSystems.csv`

 * *Files identical despite different names*

### Comparing `pydisadm-1.0.3/pydisadm/loader/static_data.py` & `pydisadm-1.0.4/pydisadm/loader/static_data.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.0.3/pydisadm/runnable/runnable_refresh.py` & `pydisadm-1.0.4/pydisadm/runnable/runnable_refresh.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.0.3/pydisadm/services/database.py` & `pydisadm-1.0.4/pydisadm/services/database.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.0.3/pydisadm/services/esi.py` & `pydisadm-1.0.4/pydisadm/services/esi.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.0.3/pydisadm/utils/plot_utils.py` & `pydisadm-1.0.4/pydisadm/utils/plot_utils.py`

 * *Files identical despite different names*

### Comparing `pydisadm-1.0.3/pyproject.toml` & `pydisadm-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydisadm"
-version = "1.0.3"
+version = "1.0.4"
 description = "A Discord bot providing ADM summaries."
 repository = "https://github.com/agelito/adm-bot"
 authors = ["Axel Wettervik"]
 license = "MIT"
 readme = "README.md"
 include = ["data/*.csv"]
```

### Comparing `pydisadm-1.0.3/PKG-INFO` & `pydisadm-1.0.4/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydisadm
-Version: 1.0.3
+Version: 1.0.4
 Summary: A Discord bot providing ADM summaries.
 Home-page: https://github.com/agelito/adm-bot
 License: MIT
 Author: Axel Wettervik
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -23,30 +23,42 @@
 
 # EVE ADM Bot
 
 This is a discord bot which will collect alliance system ADM's daily and provide commands to display them in a convenient tier list.
 
 ## ⚡ Quick Start
 
-### Using pip
+### From PyPI
 ```shell
-# Edit variables in .env
-cp .env.example .env
+# 1. Set up environment
+export DISCORD_TOKEN=your-token-here
+export DISCORD_CHANNEL=your-channel-here
+export DISCORD_APP_ID=your-app-id-here
+export ALLIANCE_ID=your-alliance-id-here
 
+# 2. Install package from PyPI
 pip install pydisadm
 
+# 3. Run Bot
 python -m pydisadm
 ```
 
-### Using poetry
+### From source
 ```shell
-# Edit variables in .env
+# 1. Clone repository
+git clone https://github.com/agelito/adm-bot
+cd adm-bot
+
+# 2. Copy and edit .env
 cp .env.example .env
 
+# 3. Install dependencies
 poetry install
+
+# 4. Run bot
 poetry run python pydisadm/__main__.py
 ```
 
 ## 📃 Commands
 
 - `/adm summary` - send a summary of ADM's
 - `/adm csv` - send a csv of ADM's
```

