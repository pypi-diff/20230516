# Comparing `tmp/ecowitt2mqtt-2023.4.0.tar.gz` & `tmp/ecowitt2mqtt-2023.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecowitt2mqtt-2023.4.0.tar", max compression
+gzip compressed data, was "ecowitt2mqtt-2023.5.0.tar", max compression
```

## Comparing `ecowitt2mqtt-2023.4.0.tar` & `ecowitt2mqtt-2023.5.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1072 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/LICENSE
--rw-r--r--   0        0        0    31131 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/README.md
--rw-r--r--   0        0        0       39 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/__init__.py
--rw-r--r--   0        0        0    13841 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/__main__.py
--rw-r--r--   0        0        0       24 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/backports/__init__.py
--rw-r--r--   0        0        0     1735 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/backports/enum.py
--rw-r--r--   0        0        0    16656 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/config.py
--rw-r--r--   0        0        0    11058 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/const.py
--rw-r--r--   0        0        0     2308 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/core.py
--rw-r--r--   0        0        0    11872 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/data.py
--rw-r--r--   0        0        0      107 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/errors.py
--rw-r--r--   0        0        0       22 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/__init__.py
--rw-r--r--   0        0        0     6598 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/calculator/__init__.py
--rw-r--r--   0        0        0     4891 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/calculator/battery.py
--rw-r--r--   0        0        0     2301 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/calculator/humidity.py
--rw-r--r--   0        0        0     2438 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/calculator/illuminance.py
--rw-r--r--   0        0        0     1018 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/calculator/leak.py
--rw-r--r--   0        0        0     2013 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/calculator/lightning.py
--rw-r--r--   0        0        0      744 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/calculator/pollution.py
--rw-r--r--   0        0        0     2737 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/calculator/precipitation.py
--rw-r--r--   0        0        0     1364 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/calculator/pressure.py
--rw-r--r--   0        0        0    21443 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/calculator/temperature.py
--rw-r--r--   0        0        0     1333 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/calculator/time.py
--rw-r--r--   0        0        0     4610 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/calculator/uv.py
--rw-r--r--   0        0        0     9593 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/calculator/wind.py
--rw-r--r--   0        0        0     2167 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/config_validation.py
--rw-r--r--   0        0        0     1619 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/device.py
--rw-r--r--   0        0        0     1800 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/publisher/__init__.py
--rw-r--r--   0        0        0      716 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/publisher/factory.py
--rw-r--r--   0        0        0    18180 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/publisher/hass.py
--rw-r--r--   0        0        0     1114 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/publisher/topic.py
--rw-r--r--   0        0        0     4973 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/server.py
--rw-r--r--   0        0        0      348 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/typing.py
--rw-r--r--   0        0        0     7978 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/runtime.py
--rw-r--r--   0        0        0     1255 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/util/__init__.py
--rw-r--r--   0        0        0     7934 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/util/meteo.py
--rw-r--r--   0        0        0    13191 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/ecowitt2mqtt/util/unit_conversion.py
--rw-r--r--   0        0        0     4041 2023-04-14 14:49:39.283581 ecowitt2mqtt-2023.4.0/pyproject.toml
--rw-r--r--   0        0        0    32767 1970-01-01 00:00:00.000000 ecowitt2mqtt-2023.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-05-16 00:11:30.310538 ecowitt2mqtt-2023.5.0/LICENSE
+-rw-r--r--   0        0        0    31131 2023-05-16 00:11:30.310538 ecowitt2mqtt-2023.5.0/README.md
+-rw-r--r--   0        0        0       39 2023-05-16 00:11:30.310538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/__init__.py
+-rw-r--r--   0        0        0    13841 2023-05-16 00:11:30.310538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/__main__.py
+-rw-r--r--   0        0        0       24 2023-05-16 00:11:30.310538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/backports/__init__.py
+-rw-r--r--   0        0        0     1735 2023-05-16 00:11:30.310538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/backports/enum.py
+-rw-r--r--   0        0        0    16656 2023-05-16 00:11:30.310538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/config.py
+-rw-r--r--   0        0        0    11058 2023-05-16 00:11:30.310538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/const.py
+-rw-r--r--   0        0        0     2308 2023-05-16 00:11:30.310538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/core.py
+-rw-r--r--   0        0        0    11872 2023-05-16 00:11:30.310538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/data.py
+-rw-r--r--   0        0        0      107 2023-05-16 00:11:30.310538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/errors.py
+-rw-r--r--   0        0        0       22 2023-05-16 00:11:30.310538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/__init__.py
+-rw-r--r--   0        0        0     6598 2023-05-16 00:11:30.310538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/calculator/__init__.py
+-rw-r--r--   0        0        0     4891 2023-05-16 00:11:30.310538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/calculator/battery.py
+-rw-r--r--   0        0        0     2301 2023-05-16 00:11:30.310538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/calculator/humidity.py
+-rw-r--r--   0        0        0     2438 2023-05-16 00:11:30.314538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/calculator/illuminance.py
+-rw-r--r--   0        0        0     1018 2023-05-16 00:11:30.314538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/calculator/leak.py
+-rw-r--r--   0        0        0     2013 2023-05-16 00:11:30.314538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/calculator/lightning.py
+-rw-r--r--   0        0        0      744 2023-05-16 00:11:30.314538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/calculator/pollution.py
+-rw-r--r--   0        0        0     2737 2023-05-16 00:11:30.314538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/calculator/precipitation.py
+-rw-r--r--   0        0        0     1364 2023-05-16 00:11:30.314538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/calculator/pressure.py
+-rw-r--r--   0        0        0    21443 2023-05-16 00:11:30.314538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/calculator/temperature.py
+-rw-r--r--   0        0        0     1333 2023-05-16 00:11:30.314538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/calculator/time.py
+-rw-r--r--   0        0        0     4610 2023-05-16 00:11:30.314538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/calculator/uv.py
+-rw-r--r--   0        0        0     9593 2023-05-16 00:11:30.314538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/calculator/wind.py
+-rw-r--r--   0        0        0     2167 2023-05-16 00:11:30.314538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/config_validation.py
+-rw-r--r--   0        0        0     1619 2023-05-16 00:11:30.314538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/device.py
+-rw-r--r--   0        0        0     1800 2023-05-16 00:11:30.314538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/publisher/__init__.py
+-rw-r--r--   0        0        0      716 2023-05-16 00:11:30.314538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/publisher/factory.py
+-rw-r--r--   0        0        0    18180 2023-05-16 00:11:30.314538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/publisher/hass.py
+-rw-r--r--   0        0        0     1114 2023-05-16 00:11:30.314538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/publisher/topic.py
+-rw-r--r--   0        0        0     4973 2023-05-16 00:11:30.314538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/server.py
+-rw-r--r--   0        0        0      348 2023-05-16 00:11:30.314538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/typing.py
+-rw-r--r--   0        0        0     7978 2023-05-16 00:11:30.314538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/runtime.py
+-rw-r--r--   0        0        0     1255 2023-05-16 00:11:30.314538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/util/__init__.py
+-rw-r--r--   0        0        0     7934 2023-05-16 00:11:30.314538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/util/meteo.py
+-rw-r--r--   0        0        0    13191 2023-05-16 00:11:30.314538 ecowitt2mqtt-2023.5.0/ecowitt2mqtt/util/unit_conversion.py
+-rw-r--r--   0        0        0     4055 2023-05-16 00:11:30.314538 ecowitt2mqtt-2023.5.0/pyproject.toml
+-rw-r--r--   0        0        0    32763 1970-01-01 00:00:00.000000 ecowitt2mqtt-2023.5.0/PKG-INFO
```

### Comparing `ecowitt2mqtt-2023.4.0/LICENSE` & `ecowitt2mqtt-2023.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.4.0/README.md` & `ecowitt2mqtt-2023.5.0/README.md`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.4.0/ecowitt2mqtt/__main__.py` & `ecowitt2mqtt-2023.5.0/ecowitt2mqtt/__main__.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.4.0/ecowitt2mqtt/backports/enum.py` & `ecowitt2mqtt-2023.5.0/ecowitt2mqtt/backports/enum.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.4.0/ecowitt2mqtt/config.py` & `ecowitt2mqtt-2023.5.0/ecowitt2mqtt/config.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.4.0/ecowitt2mqtt/const.py` & `ecowitt2mqtt-2023.5.0/ecowitt2mqtt/const.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Define package constants."""
 import logging
 from typing import Final
 
 from ecowitt2mqtt.helpers.typing import UnitSystemType
 
-__version__ = "2023.04.0"
+__version__ = "2023.05.0"
 
 LOGGER = logging.getLogger(__package__)
 
 # Configuration keys:
 CONF_BATTERY_OVERRIDES: Final = "battery_override"
 CONF_CONFIG: Final = "config"
 CONF_DEFAULT_BATTERY_STRATEGY: Final = "default_battery_strategy"
```

### Comparing `ecowitt2mqtt-2023.4.0/ecowitt2mqtt/core.py` & `ecowitt2mqtt-2023.5.0/ecowitt2mqtt/core.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.4.0/ecowitt2mqtt/data.py` & `ecowitt2mqtt-2023.5.0/ecowitt2mqtt/data.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/calculator/__init__.py` & `ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/calculator/__init__.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/calculator/battery.py` & `ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/calculator/battery.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/calculator/humidity.py` & `ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/calculator/humidity.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/calculator/illuminance.py` & `ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/calculator/illuminance.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/calculator/leak.py` & `ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/calculator/leak.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/calculator/lightning.py` & `ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/calculator/lightning.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/calculator/pollution.py` & `ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/calculator/pollution.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/calculator/precipitation.py` & `ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/calculator/precipitation.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/calculator/pressure.py` & `ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/calculator/pressure.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/calculator/temperature.py` & `ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/calculator/temperature.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,20 +75,20 @@
     HumidexPerceptionRating(
         perception=HumidexPerception.LITTLE_TO_NO_DISCOMFORT,
         minimum=20,
         maximum=29,
     ),
     HumidexPerceptionRating(
         perception=HumidexPerception.SOME_DISCOMFORT,
-        minimum=30,
+        minimum=29,
         maximum=39,
     ),
     HumidexPerceptionRating(
         perception=HumidexPerception.GREAT_DISCOMFORT,
-        minimum=40,
+        minimum=39,
         maximum=45,
     ),
     HumidexPerceptionRating(
         perception=HumidexPerception.DANGEROUS,
         minimum=45,
         maximum=100,
     ),
```

### Comparing `ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/calculator/time.py` & `ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/calculator/time.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/calculator/uv.py` & `ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/calculator/uv.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/calculator/wind.py` & `ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/calculator/wind.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/config_validation.py` & `ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/config_validation.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/device.py` & `ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/device.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/publisher/__init__.py` & `ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/publisher/__init__.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/publisher/factory.py` & `ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/publisher/factory.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/publisher/hass.py` & `ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/publisher/hass.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/publisher/topic.py` & `ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/publisher/topic.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.4.0/ecowitt2mqtt/helpers/server.py` & `ecowitt2mqtt-2023.5.0/ecowitt2mqtt/helpers/server.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.4.0/ecowitt2mqtt/runtime.py` & `ecowitt2mqtt-2023.5.0/ecowitt2mqtt/runtime.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.4.0/ecowitt2mqtt/util/__init__.py` & `ecowitt2mqtt-2023.5.0/ecowitt2mqtt/util/__init__.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.4.0/ecowitt2mqtt/util/meteo.py` & `ecowitt2mqtt-2023.5.0/ecowitt2mqtt/util/meteo.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.4.0/ecowitt2mqtt/util/unit_conversion.py` & `ecowitt2mqtt-2023.5.0/ecowitt2mqtt/util/unit_conversion.py`

 * *Files identical despite different names*

### Comparing `ecowitt2mqtt-2023.4.0/pyproject.toml` & `ecowitt2mqtt-2023.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 warn_return_any = true
 warn_unreachable = true
 warn_unused_configs = true
 warn_unused_ignores = true
 
 [tool.poetry]
 name = "ecowitt2mqtt"
-version = "2023.04.0"
+version = "2023.05.0"
 description = "A small web server to send data from Ecowitt devices to an MQTT Broker"
 readme = "README.md"
 authors = ["Aaron Bach <bachya1208@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/bachya/ecowitt2mqtt"
 classifiers = [
     "License :: OSI Approved :: MIT License",
@@ -63,15 +63,15 @@
 aiohttp = "^3.8.1"
 asyncio-mqtt = ">=0.12.1"
 colorlog = "^6.6.0"
 fastapi = ">=0.89.1,<0.96.0"
 meteocalc = "^1.1.0"
 python = "^3.9.0"
 python-multipart = ">=0.0.5,<0.0.7"
-rapidfuzz = "^2.13.0"
+rapidfuzz = ">=2.13,<4.0"
 uvicorn = ">=0.19.0"
 uvloop = "^0.17.0"
 voluptuous = "^0.13.1"
 
 [tool.poetry.group.dev.dependencies]
 aresponses = "^2.1.6"
 bandit = "^1.7.4"
@@ -86,15 +86,15 @@
 pre-commit-hooks = "^4.3.0"
 pylint = "^2.15.5"
 pytest = "^7.2.0"
 pytest-aiohttp = "^1.0.0"
 pytest-asyncio = ">=0.20.1,<0.22.0"
 pytest-cov = "^4.0.0"
 pyupgrade = "^3.1.0"
-ruff = "^0.0.261"
+ruff = ">=0.0.261,<0.0.268"
 safety = "^2.3.1"
 typing-extensions = "^4.4.0"
 vulture = "^2.6"
 yamllint = "^1.28.0"
 
 [tool.poetry.scripts]
 ecowitt2mqtt = "ecowitt2mqtt.__main__:main"
```

### Comparing `ecowitt2mqtt-2023.4.0/PKG-INFO` & `ecowitt2mqtt-2023.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecowitt2mqtt
-Version: 2023.4.0
+Version: 2023.5.0
 Summary: A small web server to send data from Ecowitt devices to an MQTT Broker
 Home-page: https://github.com/bachya/ecowitt2mqtt
 License: MIT
 Author: Aaron Bach
 Author-email: bachya1208@gmail.com
 Requires-Python: >=3.9.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: aiohttp (>=3.8.1,<4.0.0)
 Requires-Dist: asyncio-mqtt (>=0.12.1)
 Requires-Dist: colorlog (>=6.6.0,<7.0.0)
 Requires-Dist: fastapi (>=0.89.1,<0.96.0)
 Requires-Dist: meteocalc (>=1.1.0,<2.0.0)
 Requires-Dist: python-multipart (>=0.0.5,<0.0.7)
-Requires-Dist: rapidfuzz (>=2.13.0,<3.0.0)
+Requires-Dist: rapidfuzz (>=2.13,<4.0)
 Requires-Dist: ruamel.yaml (>=0.17.21,<0.18.0)
 Requires-Dist: uvicorn (>=0.19.0)
 Requires-Dist: uvloop (>=0.17.0,<0.18.0)
 Requires-Dist: voluptuous (>=0.13.1,<0.14.0)
 Project-URL: Bug Tracker, https://github.com/bachya/ecowitt2mqtt/issues
 Project-URL: Changelog, https://github.com/bachya/ecowitt2mqtt/releases
 Project-URL: Repository, https://github.com/bachya/ecowitt2mqtt
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: ecowitt2mqtt Version: 2023.4.0 Summary: A small web
+Metadata-Version: 2.1 Name: ecowitt2mqtt Version: 2023.5.0 Summary: A small web
 server to send data from Ecowitt devices to an MQTT Broker Home-page: https://
 github.com/bachya/ecowitt2mqtt License: MIT Author: Aaron Bach Author-email:
 bachya1208@gmail.com Requires-Python: >=3.9.0,<4.0.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: Implementation ::
 CPython Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: aiohttp (>=3.8.1,<4.0.0) Requires-Dist: asyncio-mqtt (>=0.12.1)
 Requires-Dist: colorlog (>=6.6.0,<7.0.0) Requires-Dist: fastapi
 (>=0.89.1,<0.96.0) Requires-Dist: meteocalc (>=1.1.0,<2.0.0) Requires-Dist:
-python-multipart (>=0.0.5,<0.0.7) Requires-Dist: rapidfuzz (>=2.13.0,<3.0.0)
+python-multipart (>=0.0.5,<0.0.7) Requires-Dist: rapidfuzz (>=2.13,<4.0)
 Requires-Dist: ruamel.yaml (>=0.17.21,<0.18.0) Requires-Dist: uvicorn
 (>=0.19.0) Requires-Dist: uvloop (>=0.17.0,<0.18.0) Requires-Dist: voluptuous
 (>=0.13.1,<0.14.0) Project-URL: Bug Tracker, https://github.com/bachya/
 ecowitt2mqtt/issues Project-URL: Changelog, https://github.com/bachya/
 ecowitt2mqtt/releases Project-URL: Repository, https://github.com/bachya/
 ecowitt2mqtt Description-Content-Type: text/markdown ![ecowitt2mqtt][logo] [!
 [CI][ci-badge]][ci] [![PyPI][pypi-badge]][pypi] [![Docker Hub][docker-hub-
```

