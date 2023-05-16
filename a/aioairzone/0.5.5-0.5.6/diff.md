# Comparing `tmp/aioairzone-0.5.5.tar.gz` & `tmp/aioairzone-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioairzone-0.5.5.tar", last modified: Mon May  8 17:21:16 2023, max compression
+gzip compressed data, was "aioairzone-0.5.6.tar", last modified: Tue May 16 06:48:09 2023, max compression
```

## Comparing `aioairzone-0.5.5.tar` & `aioairzone-0.5.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-08 17:21:16.495659 aioairzone-0.5.5/
--rw-r--r--   0 noltari   (1000) noltari   (1000)    11357 2022-03-01 18:26:58.000000 aioairzone-0.5.5/LICENSE
--rw-r--r--   0 noltari   (1000) noltari   (1000)       87 2022-05-10 12:55:46.000000 aioairzone-0.5.5/MANIFEST.in
--rw-r--r--   0 noltari   (1000) noltari   (1000)     2218 2023-05-08 17:21:16.495659 aioairzone-0.5.5/PKG-INFO
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1488 2022-05-10 12:55:46.000000 aioairzone-0.5.5/README.md
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-08 17:21:16.495659 aioairzone-0.5.5/aioairzone/
--rw-r--r--   0 noltari   (1000) noltari   (1000)       23 2022-03-01 19:23:56.000000 aioairzone-0.5.5/aioairzone/__init__.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     4261 2023-03-08 19:43:48.000000 aioairzone-0.5.5/aioairzone/common.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     4431 2023-03-08 19:32:37.000000 aioairzone-0.5.5/aioairzone/const.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)    28296 2023-05-08 17:13:56.000000 aioairzone-0.5.5/aioairzone/device.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1396 2022-05-04 20:36:00.000000 aioairzone-0.5.5/aioairzone/exceptions.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)    13801 2023-05-08 15:42:47.000000 aioairzone-0.5.5/aioairzone/localapi.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)        0 2022-05-10 12:55:46.000000 aioairzone-0.5.5/aioairzone/py.typed
--rw-r--r--   0 noltari   (1000) noltari   (1000)     4100 2022-12-28 09:48:21.000000 aioairzone-0.5.5/aioairzone/webserver.py
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-08 17:21:16.495659 aioairzone-0.5.5/aioairzone.egg-info/
--rw-r--r--   0 noltari   (1000) noltari   (1000)     2218 2023-05-08 17:21:16.000000 aioairzone-0.5.5/aioairzone.egg-info/PKG-INFO
--rw-r--r--   0 noltari   (1000) noltari   (1000)      450 2023-05-08 17:21:16.000000 aioairzone-0.5.5/aioairzone.egg-info/SOURCES.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-05-08 17:21:16.000000 aioairzone-0.5.5/aioairzone.egg-info/dependency_links.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-05-08 17:21:16.000000 aioairzone-0.5.5/aioairzone.egg-info/not-zip-safe
--rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2023-05-08 17:21:16.000000 aioairzone-0.5.5/aioairzone.egg-info/requires.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)       11 2023-05-08 17:21:16.000000 aioairzone-0.5.5/aioairzone.egg-info/top_level.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)      909 2023-05-08 17:16:26.000000 aioairzone-0.5.5/pyproject.toml
--rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2022-03-02 19:19:23.000000 aioairzone-0.5.5/requirements.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)      303 2023-05-08 17:21:16.499659 aioairzone-0.5.5/setup.cfg
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-16 06:48:09.646561 aioairzone-0.5.6/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    11357 2022-03-01 18:26:58.000000 aioairzone-0.5.6/LICENSE
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       87 2022-05-10 12:55:46.000000 aioairzone-0.5.6/MANIFEST.in
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     2649 2023-05-16 06:48:09.646561 aioairzone-0.5.6/PKG-INFO
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1897 2023-05-10 16:25:49.000000 aioairzone-0.5.6/README.md
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-16 06:48:09.642562 aioairzone-0.5.6/aioairzone/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       23 2022-03-01 19:23:56.000000 aioairzone-0.5.6/aioairzone/__init__.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     4509 2023-05-09 19:13:01.000000 aioairzone-0.5.6/aioairzone/common.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     4721 2023-05-16 06:31:23.000000 aioairzone-0.5.6/aioairzone/const.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    31713 2023-05-16 06:43:17.000000 aioairzone-0.5.6/aioairzone/device.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1396 2022-05-04 20:36:00.000000 aioairzone-0.5.6/aioairzone/exceptions.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    14150 2023-05-12 18:16:45.000000 aioairzone-0.5.6/aioairzone/localapi.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        0 2022-05-10 12:55:46.000000 aioairzone-0.5.6/aioairzone/py.typed
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     4100 2022-12-28 09:48:21.000000 aioairzone-0.5.6/aioairzone/webserver.py
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-16 06:48:09.646561 aioairzone-0.5.6/aioairzone.egg-info/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     2649 2023-05-16 06:48:09.000000 aioairzone-0.5.6/aioairzone.egg-info/PKG-INFO
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      450 2023-05-16 06:48:09.000000 aioairzone-0.5.6/aioairzone.egg-info/SOURCES.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-05-16 06:48:09.000000 aioairzone-0.5.6/aioairzone.egg-info/dependency_links.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-05-16 06:48:09.000000 aioairzone-0.5.6/aioairzone.egg-info/not-zip-safe
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2023-05-16 06:48:09.000000 aioairzone-0.5.6/aioairzone.egg-info/requires.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       11 2023-05-16 06:48:09.000000 aioairzone-0.5.6/aioairzone.egg-info/top_level.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      930 2023-05-16 06:45:08.000000 aioairzone-0.5.6/pyproject.toml
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2022-03-02 19:19:23.000000 aioairzone-0.5.6/requirements.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      303 2023-05-16 06:48:09.646561 aioairzone-0.5.6/setup.cfg
```

### Comparing `aioairzone-0.5.5/LICENSE` & `aioairzone-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aioairzone-0.5.5/PKG-INFO` & `aioairzone-0.5.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,42 @@
 Metadata-Version: 2.1
 Name: aioairzone
-Version: 0.5.5
+Version: 0.5.6
 Summary: Library to control Airzone devices
 Author-email: Álvaro Fernández Rojas <noltari@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Noltari/aioairzone
+Project-URL: Bug Tracker, https://github.com/Noltari/aioairzone/issues
 Keywords: airzone,hvac,home
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Home Automation
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # aioairzone
+[![Latest Version][mdversion-button]][md-pypi]
+[![Python Versions][pyversion-button]][md-pypi]
+[![License: Apache 2.0][apache-button]](LICENSE)
+
+[apache-button]: https://img.shields.io/badge/License-Apache%202.0-blue.svg
+[md-pypi]: https://pypi.org/project/aioairzone
+[mdversion-button]: https://img.shields.io/pypi/v/aioairzone.svg
+[pyversion-button]: https://img.shields.io/pypi/pyversions/aioairzone.svg
+
 Python library to control Airzone devices.
 
 ## Requirements
-- Python >= 3.9
+- Python >= 3.10
 
 ## Install
 ```bash
 pip install aioairzone
 ```
 
 ## Install from Source
```

### Comparing `aioairzone-0.5.5/README.md` & `aioairzone-0.5.6/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,21 @@
 # aioairzone
+[![Latest Version][mdversion-button]][md-pypi]
+[![Python Versions][pyversion-button]][md-pypi]
+[![License: Apache 2.0][apache-button]](LICENSE)
+
+[apache-button]: https://img.shields.io/badge/License-Apache%202.0-blue.svg
+[md-pypi]: https://pypi.org/project/aioairzone
+[mdversion-button]: https://img.shields.io/pypi/v/aioairzone.svg
+[pyversion-button]: https://img.shields.io/pypi/pyversions/aioairzone.svg
+
 Python library to control Airzone devices.
 
 ## Requirements
-- Python >= 3.9
+- Python >= 3.10
 
 ## Install
 ```bash
 pip install aioairzone
 ```
 
 ## Install from Source
```

### Comparing `aioairzone-0.5.5/aioairzone/common.py` & `aioairzone-0.5.6/aioairzone/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Airzone library common code."""
 from __future__ import annotations
 
-from enum import IntEnum
+from enum import Enum, IntEnum
 from typing import Any
 
 
 class AirzoneStages(IntEnum):
     """Airzone stages."""
 
     UNKNOWN = -1
@@ -33,14 +33,28 @@
                 AirzoneStages.Combined,
             ]
         if self.value in (self.Air, self.Radiant):
             return [AirzoneStages.Off, self]
         return []
 
 
+class EcoAdapt(str, Enum):
+    """Airzone Eco-Adapt."""
+
+    OFF = "off"
+    MANUAL = "manual"
+    A = "a"
+    A_PLUS = "a_p"
+    A_PLUS_PLUS = "a_pp"
+
+    @classmethod
+    def _missing_(cls, value: Any) -> EcoAdapt:
+        return cls.OFF
+
+
 class GrilleAngle(IntEnum):
     """Airzone grille angles."""
 
     DEG_90 = 0
     DEG_50 = 1
     DEG_45 = 2
     DEG_40 = 3
```

### Comparing `aioairzone-0.5.5/aioairzone/const.py` & `aioairzone-0.5.6/aioairzone/const.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """Airzone library constants."""
 
 API_ACS_POINT = "acs_temp"
 API_AIR_DEMAND = "air_demand"
+API_ANTI_FREEZE = "antifreeze"
 API_COLD_ANGLE = "coldangle"
 API_COLD_STAGE = "coldStage"
 API_COLD_STAGES = "coldStages"
 API_COOL_MAX_TEMP = "coolmaxtemp"
 API_COOL_MIN_TEMP = "coolmintemp"
 API_COOL_SET_POINT = "coolsetpoint"
 API_DATA = "data"
 API_DEMO = "demo"
 API_DOUBLE_SET_POINT = "double_sp"
+API_ECO_ADAPT = "eco_adapt"
 API_ERROR = "error"
 API_ERRORS = "errors"
 API_FLOOR_DEMAND = "floor_demand"
 API_HEAT_ANGLE = "heatangle"
 API_HEAT_MAX_TEMP = "heatmaxtemp"
 API_HEAT_MIN_TEMP = "heatmintemp"
 API_HEAT_SET_POINT = "heatsetpoint"
@@ -22,14 +24,15 @@
 API_HEAT_STAGES = "heatStages"
 API_HUMIDITY = "humidity"
 API_HVAC = "hvac"
 API_INTEGRATION = "integration"
 API_INTERFACE = "interface"
 API_MAC = "mac"
 API_MANUFACTURER = "manufacturer"
+API_MASTER_ZONE_ID = "master_zoneID"
 API_MAX_TEMP = "maxTemp"
 API_MC_CONNECTED = "mc_connected"
 API_MIN_TEMP = "minTemp"
 API_MODE = "mode"
 API_MODES = "modes"
 API_NAME = "name"
 API_ON = "on"
@@ -91,26 +94,30 @@
     API_HEAT_STAGE,
     API_NAME,
     API_ON,
     API_SET_POINT,
     API_SLEEP,
 ]
 
+AZD_ABS_TEMP_MAX = "absolute-temp-max"
+AZD_ABS_TEMP_MIN = "absolute-temp-min"
 AZD_ACTION = "action"
 AZD_AIR_DEMAND = "air-demand"
+AZD_ANTI_FREEZE = "anti-freeze"
 AZD_BATTERY_LOW = "battery-low"
 AZD_CLAMP_METER = "clamp-meter"
 AZD_COLD_ANGLE = "cold-angle"
 AZD_COLD_STAGE = "cold-stage"
 AZD_COLD_STAGES = "cold-stages"
 AZD_COOL_TEMP_MAX = "cool-temp-max"
 AZD_COOL_TEMP_MIN = "cool-temp-min"
 AZD_COOL_TEMP_SET = "cool-temp-set"
 AZD_DEMAND = "demand"
 AZD_DOUBLE_SET_POINT = "double-set-point"
+AZD_ECO_ADAPT = "eco-adapt"
 AZD_ENERGY = "energy"
 AZD_ERRORS = "errors"
 AZD_FIRMWARE = "firmware"
 AZD_FULL_NAME = "full-name"
 AZD_FLOOR_DEMAND = "floor-demand"
 AZD_HEAT_ANGLE = "heat-angle"
 AZD_HEAT_TEMP_MAX = "heat-temp-max"
@@ -120,14 +127,15 @@
 AZD_HEAT_STAGES = "heat-stages"
 AZD_HUMIDITY = "humidity"
 AZD_ID = "id"
 AZD_INTERFACE = "interface"
 AZD_MAC = "mac"
 AZD_MANUFACTURER = "manufacturer"
 AZD_MASTER = "master"
+AZD_MASTER_ZONE = "master-zone"
 AZD_MODE = "mode"
 AZD_MODEL = "model"
 AZD_MODES = "modes"
 AZD_NAME = "name"
 AZD_NEW_ZONES = "new-zones"
 AZD_ON = "on"
 AZD_PROBLEMS = "problems"
@@ -142,14 +150,15 @@
 AZD_TEMP_MIN = "temp-min"
 AZD_TEMP_SET = "temp-set"
 AZD_TEMP_STEP = "temp-step"
 AZD_TEMP_UNIT = "temp-unit"
 AZD_THERMOSTAT_FW = "thermostat-fw"
 AZD_THERMOSTAT_MODEL = "thermostat-model"
 AZD_THERMOSTAT_RADIO = "thermostat-radio"
+AZD_VERSION = "version"
 AZD_WEBSERVER = "webserver"
 AZD_WIFI_CHANNEL = "wifi-channel"
 AZD_WIFI_QUALITY = "wifi-quality"
 AZD_WIFI_RSSI = "wifi-rssi"
 AZD_ZONES = "zones"
 AZD_ZONES_NUM = "num-zones"
```

### Comparing `aioairzone-0.5.5/aioairzone/device.py` & `aioairzone-0.5.6/aioairzone/device.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,43 +2,47 @@
 from __future__ import annotations
 
 import logging
 from typing import Any
 
 from .common import (
     AirzoneStages,
+    EcoAdapt,
     GrilleAngle,
     OperationAction,
     OperationMode,
     SleepTimeout,
     SystemType,
     TemperatureUnit,
     ThermostatType,
 )
 from .const import (
     API_AIR_DEMAND,
+    API_ANTI_FREEZE,
     API_COLD_ANGLE,
     API_COLD_STAGE,
     API_COLD_STAGES,
     API_COOL_MAX_TEMP,
     API_COOL_MIN_TEMP,
     API_COOL_SET_POINT,
     API_DOUBLE_SET_POINT,
     API_DOUBLE_SET_POINT_PARAMS,
+    API_ECO_ADAPT,
     API_ERROR_LOW_BATTERY,
     API_ERRORS,
     API_FLOOR_DEMAND,
     API_HEAT_ANGLE,
     API_HEAT_MAX_TEMP,
     API_HEAT_MIN_TEMP,
     API_HEAT_SET_POINT,
     API_HEAT_STAGE,
     API_HEAT_STAGES,
     API_HUMIDITY,
     API_MANUFACTURER,
+    API_MASTER_ZONE_ID,
     API_MAX_TEMP,
     API_MC_CONNECTED,
     API_MIN_TEMP,
     API_MODE,
     API_MODES,
     API_NAME,
     API_ON,
@@ -53,26 +57,30 @@
     API_SYSTEM_TYPE,
     API_TEMP_STEP,
     API_THERMOS_FIRMWARE,
     API_THERMOS_RADIO,
     API_THERMOS_TYPE,
     API_UNITS,
     API_ZONE_ID,
+    AZD_ABS_TEMP_MAX,
+    AZD_ABS_TEMP_MIN,
     AZD_ACTION,
     AZD_AIR_DEMAND,
+    AZD_ANTI_FREEZE,
     AZD_BATTERY_LOW,
     AZD_CLAMP_METER,
     AZD_COLD_ANGLE,
     AZD_COLD_STAGE,
     AZD_COLD_STAGES,
     AZD_COOL_TEMP_MAX,
     AZD_COOL_TEMP_MIN,
     AZD_COOL_TEMP_SET,
     AZD_DEMAND,
     AZD_DOUBLE_SET_POINT,
+    AZD_ECO_ADAPT,
     AZD_ENERGY,
     AZD_ERRORS,
     AZD_FIRMWARE,
     AZD_FLOOR_DEMAND,
     AZD_FULL_NAME,
     AZD_HEAT_ANGLE,
     AZD_HEAT_STAGE,
@@ -80,14 +88,15 @@
     AZD_HEAT_TEMP_MAX,
     AZD_HEAT_TEMP_MIN,
     AZD_HEAT_TEMP_SET,
     AZD_HUMIDITY,
     AZD_ID,
     AZD_MANUFACTURER,
     AZD_MASTER,
+    AZD_MASTER_ZONE,
     AZD_MODE,
     AZD_MODEL,
     AZD_MODES,
     AZD_NAME,
     AZD_ON,
     AZD_PROBLEMS,
     AZD_SLEEP,
@@ -116,14 +125,15 @@
 
 class System:
     """Airzone System."""
 
     def __init__(self, airzone_system: list[dict[str, Any]]):
         """System init."""
         self.clamp_meter: bool | None = None
+        self.eco_adapt: EcoAdapt | None = None
         self.energy: int | None = None
         self.errors: list[str] = []
         self.id: int | None = None
         self.firmware: str | None = None
         self.manufacturer: str | None = None
         self.mode: OperationMode | None = None
         self.modes: list[OperationMode] = []
@@ -154,14 +164,18 @@
             data[AZD_CLAMP_METER] = clamp_meter
 
             if clamp_meter:
                 energy = self.get_energy()
                 if energy is not None:
                     data[AZD_ENERGY] = energy
 
+        eco_adapt = self.get_eco_adapt()
+        if eco_adapt is not None:
+            data[AZD_ECO_ADAPT] = eco_adapt
+
         errors = self.get_errors()
         if len(errors) > 0:
             data[AZD_ERRORS] = errors
 
         firmware = self.get_firmware()
         if firmware is not None:
             data[AZD_FIRMWARE] = firmware
@@ -193,14 +207,18 @@
         if val not in self.errors:
             self.errors.append(val)
 
     def get_clamp_meter(self) -> bool | None:
         """Return system clamp meter connection."""
         return self.clamp_meter
 
+    def get_eco_adapt(self) -> EcoAdapt | None:
+        """Return system Eco Adapt."""
+        return self.eco_adapt
+
     def get_energy(self) -> int | None:
         """Return system energy consumption."""
         return self.energy
 
     def get_errors(self) -> list[str]:
         """Return system errors."""
         return self.errors
@@ -252,25 +270,31 @@
                 return zone
         raise InvalidZone(f"Zone {zone_id} not present in System {self.id}")
 
     def num_zones(self) -> int:
         """Return number of system zones."""
         return len(self.zones)
 
+    def set_eco_adapt(self, eco_adapt: EcoAdapt) -> None:
+        """Set system Eco Adapt."""
+        self.eco_adapt = eco_adapt
+
     def set_mode(self, mode: OperationMode) -> None:
         """Set system mode."""
         self.mode = mode
 
     def set_modes(self, modes: list[OperationMode]) -> None:
         """Set system modes."""
         self.modes = modes
 
     def set_param(self, key: str, value: Any) -> None:
         """Update parameters by key and value."""
-        if key == API_MODE:
+        if key == API_ECO_ADAPT:
+            self.eco_adapt = EcoAdapt(value)
+        elif key == API_MODE:
             self.mode = OperationMode(value)
 
         for zone in self.zones.values():
             zone.set_param(key, value)
 
     def update_data(self, data: dict[str, Any]) -> None:
         """Update system parameters by dict."""
@@ -337,51 +361,69 @@
 
 class Zone:
     """Airzone Zone."""
 
     def __init__(self, system: System, zone: dict[str, Any]):
         """Zone init."""
         self.air_demand: bool | None = None
+        self.anti_freeze: bool | None = None
         self.cold_angle: GrilleAngle | None = None
         self.cold_stage: AirzoneStages | None = None
         self.cold_stages: list[AirzoneStages] = []
         self.cool_temp_max: float | None = None
         self.cool_temp_min: float | None = None
         self.cool_temp_set: float | None = None
-        self.double_set_point: bool = False
+        self.double_set_point: bool | None = None
+        self.double_set_point_params: bool = zone.keys() >= API_DOUBLE_SET_POINT_PARAMS
+        self.eco_adapt: EcoAdapt | None = None
         self.errors: list[str] = []
         self.floor_demand: bool | None = None
         self.heat_angle: GrilleAngle | None = None
         self.heat_temp_max: float | None = None
         self.heat_temp_min: float | None = None
         self.heat_temp_set: float | None = None
         self.heat_stage: AirzoneStages | None = None
         self.heat_stages: list[AirzoneStages] = []
         self.humidity: int | None = None
         self.id = int(zone[API_ZONE_ID])
         self.master = bool(API_MODES in zone)
+        self.master_zone: int | None = None
         self.modes: list[OperationMode] = []
         self.on = bool(zone[API_ON])
         self.sleep: SleepTimeout | None = None
         self.speed: int | None = None
         self.speeds: list[int] = []
         self.temp = float(zone[API_ROOM_TEMP])
         self.temp_max = float(zone[API_MAX_TEMP])
         self.temp_min = float(zone[API_MIN_TEMP])
         self.temp_set = float(zone[API_SET_POINT])
         self.temp_step: float | None = None
         self.temp_unit = TemperatureUnit(zone[API_UNITS])
         self.thermostat = Thermostat(zone)
         self.system = system
 
+        if API_MASTER_ZONE_ID in zone:
+            master_zone_id = int(zone[API_MASTER_ZONE_ID])
+            if master_zone_id != self.id:
+                self.master_zone = master_zone_id
+
         if API_AIR_DEMAND in zone:
             self.air_demand = bool(zone[API_AIR_DEMAND])
         if API_FLOOR_DEMAND in zone:
             self.floor_demand = bool(zone[API_FLOOR_DEMAND])
 
+        if API_ANTI_FREEZE in zone:
+            self.anti_freeze = bool(zone[API_ANTI_FREEZE])
+
+        if API_DOUBLE_SET_POINT in zone:
+            self.double_set_point = bool(zone[API_DOUBLE_SET_POINT])
+
+        if API_ECO_ADAPT in zone:
+            self.eco_adapt = EcoAdapt(zone[API_ECO_ADAPT])
+
         if API_HUMIDITY in zone:
             self.humidity = int(zone[API_HUMIDITY])
 
         if API_COLD_ANGLE in zone:
             self.cold_angle = GrilleAngle(zone[API_COLD_ANGLE])
         if API_HEAT_ANGLE in zone:
             self.heat_angle = GrilleAngle(zone[API_HEAT_ANGLE])
@@ -404,18 +446,14 @@
 
         if API_COOL_MAX_TEMP in zone:
             self.cool_temp_max = float(zone[API_COOL_MAX_TEMP])
         if API_COOL_MIN_TEMP in zone:
             self.cool_temp_min = float(zone[API_COOL_MIN_TEMP])
         if API_COOL_SET_POINT in zone:
             self.cool_temp_set = float(zone[API_COOL_SET_POINT])
-        if API_DOUBLE_SET_POINT in zone:
-            self.double_set_point = bool(zone[API_DOUBLE_SET_POINT])
-        else:
-            self.double_set_point = zone.keys() >= API_DOUBLE_SET_POINT_PARAMS
         if API_HEAT_MAX_TEMP in zone:
             self.heat_temp_max = float(zone[API_HEAT_MAX_TEMP])
         if API_HEAT_MIN_TEMP in zone:
             self.heat_temp_min = float(zone[API_HEAT_MIN_TEMP])
         if API_HEAT_SET_POINT in zone:
             self.heat_temp_set = float(zone[API_HEAT_SET_POINT])
 
@@ -449,24 +487,31 @@
         if API_TEMP_STEP in zone:
             self.temp_step = float(zone[API_TEMP_STEP])
 
         if self.master:
             if API_MODES in zone:
                 for mode in zone[API_MODES]:
                     self.modes.append(OperationMode(mode))
+            if self.eco_adapt:
+                self.system.set_eco_adapt(self.eco_adapt)
             self.system.set_mode(self.mode)
             self.system.set_modes(self.modes)
             if OperationMode.STOP not in self.modes:
                 self.modes.append(OperationMode.STOP)
-        elif self.system.get_mode() is None:
-            self.system.set_mode(self.mode)
+        else:
+            if self.eco_adapt and self.system.get_eco_adapt() is None:
+                self.system.set_eco_adapt(self.eco_adapt)
+            if self.system.get_mode() is None:
+                self.system.set_mode(self.mode)
 
     def data(self) -> dict[str, Any]:
         """Return Airzone zone data."""
         data = {
+            AZD_ABS_TEMP_MAX: self.get_abs_temp_max(),
+            AZD_ABS_TEMP_MIN: self.get_abs_temp_min(),
             AZD_ACTION: self.get_action(),
             AZD_DEMAND: self.get_demand(),
             AZD_DOUBLE_SET_POINT: self.get_double_set_point(),
             AZD_ID: self.get_id(),
             AZD_MASTER: self.get_master(),
             AZD_MODE: self.get_mode(),
             AZD_NAME: self.get_name(),
@@ -484,41 +529,48 @@
         if air_demand is not None:
             data[AZD_AIR_DEMAND] = air_demand
 
         floor_demand = self.get_floor_demand()
         if floor_demand is not None:
             data[AZD_FLOOR_DEMAND] = floor_demand
 
+        anti_freeze = self.get_anti_freeze()
+        if anti_freeze is not None:
+            data[AZD_ANTI_FREEZE] = anti_freeze
+
+        eco_adapt = self.get_eco_adapt()
+        if eco_adapt is not None:
+            data[AZD_ECO_ADAPT] = eco_adapt
+
         full_name = self.get_full_name()
         if full_name is not None:
             data[AZD_FULL_NAME] = full_name
 
         humidity = self.get_humidity()
         if humidity is not None:
             data[AZD_HUMIDITY] = humidity
 
-        if data[AZD_DOUBLE_SET_POINT]:
-            cool_temp_max = self.get_cool_temp_max()
-            if cool_temp_max:
-                data[AZD_COOL_TEMP_MAX] = cool_temp_max
-            cool_temp_min = self.get_cool_temp_min()
-            if cool_temp_min:
-                data[AZD_COOL_TEMP_MIN] = cool_temp_min
-            cool_temp_set = self.get_cool_temp_set()
-            if cool_temp_set:
-                data[AZD_COOL_TEMP_SET] = cool_temp_set
-            heat_temp_max = self.get_heat_temp_max()
-            if heat_temp_max:
-                data[AZD_HEAT_TEMP_MAX] = heat_temp_max
-            heat_temp_min = self.get_heat_temp_min()
-            if heat_temp_min:
-                data[AZD_HEAT_TEMP_MIN] = heat_temp_min
-            heat_temp_set = self.get_heat_temp_set()
-            if heat_temp_set:
-                data[AZD_HEAT_TEMP_SET] = heat_temp_set
+        cool_temp_max = self.get_cool_temp_max()
+        if cool_temp_max:
+            data[AZD_COOL_TEMP_MAX] = cool_temp_max
+        cool_temp_min = self.get_cool_temp_min()
+        if cool_temp_min:
+            data[AZD_COOL_TEMP_MIN] = cool_temp_min
+        cool_temp_set = self.get_cool_temp_set()
+        if cool_temp_set:
+            data[AZD_COOL_TEMP_SET] = cool_temp_set
+        heat_temp_max = self.get_heat_temp_max()
+        if heat_temp_max:
+            data[AZD_HEAT_TEMP_MAX] = heat_temp_max
+        heat_temp_min = self.get_heat_temp_min()
+        if heat_temp_min:
+            data[AZD_HEAT_TEMP_MIN] = heat_temp_min
+        heat_temp_set = self.get_heat_temp_set()
+        if heat_temp_set:
+            data[AZD_HEAT_TEMP_SET] = heat_temp_set
 
         cold_angle = self.get_cold_angle()
         if cold_angle is not None:
             data[AZD_COLD_ANGLE] = cold_angle
         heat_angle = self.get_heat_angle()
         if heat_angle is not None:
             data[AZD_HEAT_ANGLE] = heat_angle
@@ -548,14 +600,18 @@
         if speeds is not None:
             data[AZD_SPEEDS] = speeds
 
         errors = self.get_errors()
         if len(errors) > 0:
             data[AZD_ERRORS] = errors
 
+        master_zone = self.get_master_zone()
+        if master_zone is not None:
+            data[AZD_MASTER_ZONE] = master_zone
+
         modes = self.get_modes()
         if modes is not None:
             data[AZD_MODES] = modes
 
         temp_step = self.get_temp_step()
         if temp_step is not None:
             data[AZD_TEMP_STEP] = temp_step
@@ -581,14 +637,32 @@
         _key = key.casefold()
         if _key == ERROR_SYSTEM:
             self.system.add_error(val)
         elif _key == ERROR_ZONE:
             if val not in self.errors:
                 self.errors.append(val)
 
+    def get_abs_temp_max(self) -> float:
+        """Return absolute max temp."""
+        temps = [
+            self.get_cool_temp_max(),
+            self.get_heat_temp_max(),
+            self.get_temp_max(),
+        ]
+        return max(list(temp for temp in temps if temp is not None))
+
+    def get_abs_temp_min(self) -> float:
+        """Return absolute min temp."""
+        temps = [
+            self.get_cool_temp_min(),
+            self.get_heat_temp_min(),
+            self.get_temp_min(),
+        ]
+        return min(list(temp for temp in temps if temp is not None))
+
     def get_action(self) -> OperationAction:
         """Return zone action."""
 
         if self.get_on():
             if self.get_demand():
                 mode = self.get_mode()
                 if mode == OperationMode.COOLING:
@@ -612,14 +686,18 @@
 
     def get_air_demand(self) -> bool | None:
         """Return zone air demand."""
         if self.air_demand is not None and self.is_stage_supported(AirzoneStages.Air):
             return self.air_demand
         return None
 
+    def get_anti_freeze(self) -> bool | None:
+        """Return zone anti freeze."""
+        return self.anti_freeze
+
     def get_auto_mode(self) -> OperationAction:
         """Return action from auto mode."""
         temp_sp = self.get_temp_set()
         temp_min = self.get_temp_min()
         temp_max = self.get_temp_max()
         cool_sp = self.get_cool_temp_set()
         cool_max = self.get_cool_temp_max()
@@ -631,15 +709,15 @@
         if (
             cool_max is not None
             and cool_min is not None
             and heat_max is not None
             and heat_min is not None
         ):
             cool_match = cool_max == temp_max and cool_min == temp_min
-            heat_match = heat_max == temp_max and cool_min == temp_min
+            heat_match = heat_max == temp_max and heat_min == temp_min
 
             if cool_match and not heat_match:
                 return OperationAction.COOLING
             if heat_match and not cool_match:
                 return OperationAction.HEATING
 
         if cool_sp is not None and heat_sp is not None:
@@ -693,15 +771,23 @@
 
     def get_demand(self) -> bool:
         """Return zone demand."""
         return bool(self.air_demand) or bool(self.floor_demand)
 
     def get_double_set_point(self) -> bool:
         """Return zone double set point."""
-        return self.double_set_point
+        if self.double_set_point_params:
+            if self.double_set_point is not None:
+                return self.double_set_point
+            return OperationMode.AUTO in self.get_modes()
+        return False
+
+    def get_eco_adapt(self) -> EcoAdapt | None:
+        """Return zone echo adapt."""
+        return self.eco_adapt
 
     def get_errors(self) -> list[str]:
         """Return zone errors."""
         return self.errors
 
     def get_floor_demand(self) -> bool | None:
         """Return zone floor demand."""
@@ -757,27 +843,45 @@
             return self.humidity
         return None
 
     def get_master(self) -> bool:
         """Return zone master/slave."""
         return self.master
 
+    def get_master_zone(self) -> int | None:
+        """Return corresponding master zone."""
+        return self.master_zone
+
     def get_mode(self) -> OperationMode:
         """Return zone mode."""
         return self.mode
 
     def get_modes(self) -> list[OperationMode]:
         """Return zone modes."""
         if self.master:
             return self.modes
-        modes = self.system.get_modes()
+
+        modes = None
+        master_zone_id = self.get_master_zone()
+        if master_zone_id is not None:
+            try:
+                master_zone = self.system.get_zone(master_zone_id)
+                modes = master_zone.get_modes()
+            except InvalidZone:
+                pass
+
+        if modes is None:
+            modes = self.system.get_modes()
+
         if modes is None:
             modes = [self.mode]
+
         if OperationMode.STOP not in modes:
             modes.append(OperationMode.STOP)
+
         return modes
 
     def get_name(self) -> str:
         """Return zone name."""
         return self.name
 
     def get_on(self) -> bool:
@@ -852,20 +956,24 @@
             if len(heat_stages) == 0:
                 return True
 
         return cold_stages is None and heat_stages is None
 
     def set_param(self, key: str, value: Any) -> None:
         """Update zone parameter by key and value."""
-        if key == API_COOL_SET_POINT:
+        if key == API_ANTI_FREEZE:
+            self.anti_freeze = bool(value)
+        elif key == API_COOL_SET_POINT:
             self.cool_temp_set = float(value)
         elif key == API_COLD_ANGLE:
             self.cold_angle = GrilleAngle(value)
         elif key == API_COLD_STAGE:
             self.cold_stage = AirzoneStages(value)
+        elif key == API_ECO_ADAPT:
+            self.eco_adapt = EcoAdapt(value)
         elif key == API_HEAT_ANGLE:
             self.heat_angle = GrilleAngle(value)
         elif key == API_HEAT_SET_POINT:
             self.heat_temp_set = float(value)
         elif key == API_HEAT_STAGE:
             self.heat_stage = AirzoneStages(value)
         elif key == API_MODE:
```

### Comparing `aioairzone-0.5.5/aioairzone/exceptions.py` & `aioairzone-0.5.6/aioairzone/exceptions.py`

 * *Files identical despite different names*

### Comparing `aioairzone-0.5.5/aioairzone/localapi.py` & `aioairzone-0.5.6/aioairzone/localapi.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     API_VERSION,
     API_WEBSERVER,
     API_ZONE_ID,
     API_ZONE_PARAMS,
     AZD_NEW_ZONES,
     AZD_SYSTEMS,
     AZD_SYSTEMS_NUM,
+    AZD_VERSION,
     AZD_WEBSERVER,
     AZD_ZONES,
     AZD_ZONES_NUM,
     DEFAULT_PORT,
     DEFAULT_SYSTEM_ID,
     HTTP_CALL_TIMEOUT,
     RAW_DEMO,
@@ -104,14 +105,15 @@
         self._first_update: bool = True
         self._new_zones: bool = False
         self.aiohttp_session = aiohttp_session
         self.api_features: int = ApiFeature.HVAC
         self.api_features_checked = False
         self.options = options
         self.systems: dict[int, System] = {}
+        self.version: str | None = None
         self.webserver: WebServer | None = None
 
     @staticmethod
     def handle_errors(errors: list[dict[str, str]]) -> None:
         """Handle API errors."""
         for error in errors:
             for key, val in error.items():
@@ -187,14 +189,21 @@
             if API_SYSTEMS in systems:
                 self.api_features |= ApiFeature.SYSTEMS
                 if update:
                     self.update_systems(systems)
         except (SystemOutOfRange, ZoneNotProvided):
             pass
 
+        try:
+            version = await self.get_version()
+            if API_VERSION in version:
+                self.version = version[API_VERSION]
+        except (InvalidHost, APIError):
+            pass
+
         self.api_features_checked = True
 
     async def update_features(self) -> None:
         """Gather Airzone features data."""
         if not self.api_features_checked:
             await self.check_features(True)
         else:
@@ -404,14 +413,17 @@
                 for zone in system.zones.values():
                     zones[zone.get_system_zone_id()] = zone.data()
             data[AZD_SYSTEMS] = systems
             if self.webserver:
                 data[AZD_WEBSERVER] = self.webserver.data()
             data[AZD_ZONES] = zones
 
+        if self.version is not None:
+            data[AZD_VERSION] = self.version
+
         return data
 
     def get_system(self, system_id: int) -> System:
         """Return Airzone system."""
         for system in self.systems.values():
             if system.get_id() == system_id:
                 return system
```

### Comparing `aioairzone-0.5.5/aioairzone/webserver.py` & `aioairzone-0.5.6/aioairzone/webserver.py`

 * *Files identical despite different names*

### Comparing `aioairzone-0.5.5/aioairzone.egg-info/PKG-INFO` & `aioairzone-0.5.6/aioairzone.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,42 @@
 Metadata-Version: 2.1
 Name: aioairzone
-Version: 0.5.5
+Version: 0.5.6
 Summary: Library to control Airzone devices
 Author-email: Álvaro Fernández Rojas <noltari@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Noltari/aioairzone
+Project-URL: Bug Tracker, https://github.com/Noltari/aioairzone/issues
 Keywords: airzone,hvac,home
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Home Automation
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # aioairzone
+[![Latest Version][mdversion-button]][md-pypi]
+[![Python Versions][pyversion-button]][md-pypi]
+[![License: Apache 2.0][apache-button]](LICENSE)
+
+[apache-button]: https://img.shields.io/badge/License-Apache%202.0-blue.svg
+[md-pypi]: https://pypi.org/project/aioairzone
+[mdversion-button]: https://img.shields.io/pypi/v/aioairzone.svg
+[pyversion-button]: https://img.shields.io/pypi/pyversions/aioairzone.svg
+
 Python library to control Airzone devices.
 
 ## Requirements
-- Python >= 3.9
+- Python >= 3.10
 
 ## Install
 ```bash
 pip install aioairzone
 ```
 
 ## Install from Source
```

### Comparing `aioairzone-0.5.5/pyproject.toml` & `aioairzone-0.5.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 [project]
 name = "aioairzone"
-version = "0.5.5"
+version = "0.5.6"
 description = "Library to control Airzone devices"
 readme = "README.md"
-requires-python = ">=3.9"
+requires-python = ">=3.10"
 license = {text = "Apache-2.0"}
 keywords = ["airzone", "hvac", "home"] 
 authors = [
   {name = "Álvaro Fernández Rojas", email = "noltari@gmail.com" }
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Intended Audience :: Developers",
   "Natural Language :: English",
   "Programming Language :: Python :: 3",
-  "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Topic :: Home Automation",
 ]
 dependencies = [
   "aiohttp"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/Noltari/aioairzone"
+"Bug Tracker" = "https://github.com/Noltari/aioairzone/issues"
 
 [tool.setuptools]
 platforms = ["any"]
 zip-safe = false
 include-package-data = true
 
 [build-system]
```

