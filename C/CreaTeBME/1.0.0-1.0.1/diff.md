# Comparing `tmp/CreaTeBME-1.0.0.tar.gz` & `tmp/CreaTeBME-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CreaTeBME-1.0.0.tar", last modified: Wed May  3 23:41:42 2023, max compression
+gzip compressed data, was "CreaTeBME-1.0.1.tar", last modified: Tue May 16 14:24:14 2023, max compression
```

## Comparing `CreaTeBME-1.0.0.tar` & `CreaTeBME-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-05-03 23:41:42.608227 CreaTeBME-1.0.0/
--rw-r--r--   0 jonathan   (501) staff       (20)    35149 2023-03-09 12:02:38.000000 CreaTeBME-1.0.0/LICENSE
--rw-r--r--   0 jonathan   (501) staff       (20)     3212 2023-05-03 23:41:42.608115 CreaTeBME-1.0.0/PKG-INFO
--rw-r--r--   0 jonathan   (501) staff       (20)     2628 2023-05-03 23:36:29.000000 CreaTeBME-1.0.0/README.md
--rw-r--r--   0 jonathan   (501) staff       (20)       84 2023-03-09 12:02:38.000000 CreaTeBME-1.0.0/pyproject.toml
--rw-r--r--   0 jonathan   (501) staff       (20)       38 2023-05-03 23:41:42.608271 CreaTeBME-1.0.0/setup.cfg
--rw-r--r--   0 jonathan   (501) staff       (20)     1003 2023-05-03 23:36:29.000000 CreaTeBME-1.0.0/setup.py
-drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-05-03 23:41:42.605318 CreaTeBME-1.0.0/src/
-drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-05-03 23:41:42.607295 CreaTeBME-1.0.0/src/CreaTeBME/
--rw-r--r--   0 jonathan   (501) staff       (20)     5065 2023-05-03 23:36:29.000000 CreaTeBME-1.0.0/src/CreaTeBME/ImuSensor.py
--rw-r--r--   0 jonathan   (501) staff       (20)     2872 2023-05-03 23:36:29.000000 CreaTeBME-1.0.0/src/CreaTeBME/SensorEmulator.py
--rw-r--r--   0 jonathan   (501) staff       (20)     4256 2023-05-03 23:36:29.000000 CreaTeBME-1.0.0/src/CreaTeBME/SensorManager.py
--rw-r--r--   0 jonathan   (501) staff       (20)      146 2023-05-03 23:36:29.000000 CreaTeBME-1.0.0/src/CreaTeBME/__init__.py
--rw-r--r--   0 jonathan   (501) staff       (20)      962 2023-05-03 23:36:29.000000 CreaTeBME-1.0.0/src/CreaTeBME/connect.py
-drwxr-xr-x   0 jonathan   (501) staff       (20)        0 2023-05-03 23:41:42.607910 CreaTeBME-1.0.0/src/CreaTeBME.egg-info/
--rw-r--r--   0 jonathan   (501) staff       (20)     3212 2023-05-03 23:41:42.000000 CreaTeBME-1.0.0/src/CreaTeBME.egg-info/PKG-INFO
--rw-r--r--   0 jonathan   (501) staff       (20)      366 2023-05-03 23:41:42.000000 CreaTeBME-1.0.0/src/CreaTeBME.egg-info/SOURCES.txt
--rw-r--r--   0 jonathan   (501) staff       (20)        1 2023-05-03 23:41:42.000000 CreaTeBME-1.0.0/src/CreaTeBME.egg-info/dependency_links.txt
--rw-r--r--   0 jonathan   (501) staff       (20)       14 2023-05-03 23:41:42.000000 CreaTeBME-1.0.0/src/CreaTeBME.egg-info/requires.txt
--rw-r--r--   0 jonathan   (501) staff       (20)       10 2023-05-03 23:41:42.000000 CreaTeBME-1.0.0/src/CreaTeBME.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:24:14.192275 CreaTeBME-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-16 14:23:59.000000 CreaTeBME-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-05-16 14:24:14.192275 CreaTeBME-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-05-16 14:23:59.000000 CreaTeBME-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-16 14:23:59.000000 CreaTeBME-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 14:24:14.192275 CreaTeBME-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-16 14:23:59.000000 CreaTeBME-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:24:14.192275 CreaTeBME-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:24:14.192275 CreaTeBME-1.0.1/src/CreaTeBME/
+-rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-05-16 14:23:59.000000 CreaTeBME-1.0.1/src/CreaTeBME/ImuSensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-05-16 14:23:59.000000 CreaTeBME-1.0.1/src/CreaTeBME/SensorEmulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-05-16 14:23:59.000000 CreaTeBME-1.0.1/src/CreaTeBME/SensorManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-16 14:23:59.000000 CreaTeBME-1.0.1/src/CreaTeBME/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-16 14:23:59.000000 CreaTeBME-1.0.1/src/CreaTeBME/connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-16 14:23:59.000000 CreaTeBME-1.0.1/src/CreaTeBME/uuids.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:24:14.192275 CreaTeBME-1.0.1/src/CreaTeBME.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-05-16 14:24:14.000000 CreaTeBME-1.0.1/src/CreaTeBME.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-16 14:24:14.000000 CreaTeBME-1.0.1/src/CreaTeBME.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 14:24:14.000000 CreaTeBME-1.0.1/src/CreaTeBME.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-16 14:24:14.000000 CreaTeBME-1.0.1/src/CreaTeBME.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-16 14:24:14.000000 CreaTeBME-1.0.1/src/CreaTeBME.egg-info/top_level.txt
```

### Comparing `CreaTeBME-1.0.0/LICENSE` & `CreaTeBME-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `CreaTeBME-1.0.0/PKG-INFO` & `CreaTeBME-1.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: CreaTeBME
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python Package for interfacing the bluetooth IMU module for CreaTe M8 BME.
 Home-page: https://github.com/CreaTe-M8-BME/CreaTeBME
 Author: Jonathan Matarazzi
 Author-email: git@jonathanm.nl
 Project-URL: Bug Tracker, https://github.com/CreaTe-M8-BME/CreaTeBME/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CreaTeBME
+
+[![PyPI](https://img.shields.io/pypi/v/CreaTeBME)](https://pypi.org/project/CreaTeBME/)
+
 Python Package for interfacing the bluetooth IMU module for CreaTe M8 BME.
 
 # Installation
 To install the latest stable version simply run
 ```shell
 pip install CreaTeBME
 ```
@@ -33,15 +36,16 @@
 
 # Start the sensor manager
 manager.start()
 
 while True:
     measurements = manager.get_measurements()
     for sensor, data in measurements.items():
-        print(sensor, len(data))
+        if len(data) > 0:
+            print(sensor, data)
 
 # Stop the sensor manager
 manager.stop()
 ```
 
 # Usage
 
@@ -98,8 +102,8 @@
 async def connect():
     devices = await BleakScanner.discover(return_adv=True)
     sensor = ImuSensor(devices[0])
 ```
 
 # API reference
 
-For the API reference look [here](./docs/api.md)
+For the API reference look [here](https://github.com/CreaTe-M8-BME/CreaTeBME/blob/main/docs/README.md)
```

### Comparing `CreaTeBME-1.0.0/README.md` & `CreaTeBME-1.0.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 # CreaTeBME
+
+[![PyPI](https://img.shields.io/pypi/v/CreaTeBME)](https://pypi.org/project/CreaTeBME/)
+
 Python Package for interfacing the bluetooth IMU module for CreaTe M8 BME.
 
 # Installation
 To install the latest stable version simply run
 ```shell
 pip install CreaTeBME
 ```
@@ -18,15 +21,16 @@
 
 # Start the sensor manager
 manager.start()
 
 while True:
     measurements = manager.get_measurements()
     for sensor, data in measurements.items():
-        print(sensor, len(data))
+        if len(data) > 0:
+            print(sensor, data)
 
 # Stop the sensor manager
 manager.stop()
 ```
 
 # Usage
 
@@ -83,8 +87,8 @@
 async def connect():
     devices = await BleakScanner.discover(return_adv=True)
     sensor = ImuSensor(devices[0])
 ```
 
 # API reference
 
-For the API reference look [here](./docs/api.md)
+For the API reference look [here](https://github.com/CreaTe-M8-BME/CreaTeBME/blob/main/docs/README.md)
```

### Comparing `CreaTeBME-1.0.0/setup.py` & `CreaTeBME-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text('utf-8')
 
 setup(
     name='CreaTeBME',
-    version='1.0.0',
+    version='1.0.1',
     author='Jonathan Matarazzi',
     author_email='git@jonathanm.nl',
     description='Python Package for interfacing the bluetooth IMU module for CreaTe M8 BME.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/CreaTe-M8-BME/CreaTeBME',
     project_urls={
```

### Comparing `CreaTeBME-1.0.0/src/CreaTeBME/ImuSensor.py` & `CreaTeBME-1.0.1/src/CreaTeBME/ImuSensor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,14 @@
+import time
 import warnings
 import asyncio
 
 from bleak import BleakClient, BLEDevice
 from typing import Callable, List, Union
-
-_IMU_SERVICE_UUID = '0ddf5c1d-d269-4b17-bd7f-33a8658f0b89'
-_IMU_CHAR_UUID = '64b83770-6b12-4a54-b31a-e007306132bd'
-_SAMPLE_RATE_CHAR_UUID = '3003aac7-d843-4e55-9d89-3f93020cc9ee'
-_VERSION_CHAR_UUID = '2980b86f-dacb-43b9-847c-30c586224943'
+from .uuids import IMU_SERVICE_UUID, IMU_CHAR_UUID, SAMPLE_RATE_CHAR_UUID, VERSION_CHAR_UUID
 
 
 class ImuSensor:
     """
     An interface for the BLE IMU sensors.
     """
     def __init__(self, device: BLEDevice, callback: Callable[[str, List[float]], None] = None, name: str = None):
@@ -28,20 +25,22 @@
         self.__imu_service = None
         self.__sens_acc = 2048
         self.__sens_gyro = 16.4
         self.__callback = callback
         self.__reading = None
         self.__sample_rate_reserve = None
         self.__name = name if name else device.name[-4:]
+        self._is_running = False
 
         # Connect to ble device
         self.__bt_client = BleakClient(device)
 
     def __del__(self):
-        asyncio.run(self.disconnect())
+        if self.__bt_client.is_connected:
+            asyncio.run(self.disconnect())
 
     def __receive_reading(self, characteristic, inbytes):
         output = [None] * 6
         for i in range(0, 6):
             input_bytes = inbytes[i * 2:i * 2 + 2]
             num = int.from_bytes(input_bytes, "big", signed=True)
             if i < 3:
@@ -69,18 +68,18 @@
         """
         try:
             await self.__bt_client.connect()
         except Exception as e:
             raise RuntimeError('Could not connect to sensor: ', e)
 
         # Read and store services and characteristics
-        self.__imu_service = self.__bt_client.services.get_service(_IMU_SERVICE_UUID)
-        self.__imu_char = self.__imu_service.get_characteristic(_IMU_CHAR_UUID)
-        self.__sample_rate_char = self.__imu_service.get_characteristic(_SAMPLE_RATE_CHAR_UUID)
-        self.__version_char = self.__imu_service.get_characteristic(_VERSION_CHAR_UUID)
+        self.__imu_service = self.__bt_client.services.get_service(IMU_SERVICE_UUID)
+        self.__imu_char = self.__imu_service.get_characteristic(IMU_CHAR_UUID)
+        self.__sample_rate_char = self.__imu_service.get_characteristic(SAMPLE_RATE_CHAR_UUID)
+        self.__version_char = self.__imu_service.get_characteristic(VERSION_CHAR_UUID)
 
         # Register callback for notify events
         await self.__bt_client.start_notify(self.__imu_char, self.__receive_reading)
 
         # Set sample rate if reserve exists
         if self.__sample_rate_reserve:
             await self.set_sample_rate(self.__sample_rate_reserve)
```

### Comparing `CreaTeBME-1.0.0/src/CreaTeBME/SensorEmulator.py` & `CreaTeBME-1.0.1/src/CreaTeBME/SensorEmulator.py`

 * *Files 12% similar despite different names*

```diff
@@ -38,14 +38,18 @@
         """
         Stop the SensorEmulator
         """
         self._timer.cancel()
         self._is_running = False
 
     def is_running(self) -> bool:
+        """
+        Check whether the SensorEmulator is running.
+        :return: Boolean representing the running state of the SensorEmulator.
+        """
         return self._is_running
 
     def get_measurements(self) -> Dict[str, List[List[float]]]:
         """
         Get the measurements since the last time this method was called.
 
         :return: A dictionary containing a list of measurements for each sensor
```

### Comparing `CreaTeBME-1.0.0/src/CreaTeBME/SensorManager.py` & `CreaTeBME-1.0.1/src/CreaTeBME/SensorManager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from threading import Thread, Lock
+import atexit
 import asyncio
 from .connect import connect
 from typing import Callable, List, Dict
 from .ImuSensor import ImuSensor
 import copy
 import time
 import json
@@ -22,45 +23,54 @@
         self._sensors: List[ImuSensor] = []
         self._sample_rate = sample_rate
         self._thread = None
         self._loop = asyncio.new_event_loop()
         self._queue = {name: [] for name in sensor_names}
         self._lock = Lock()
         self._callback = None
+        self._is_running = False
+
+        atexit.register(self.__del__)
 
         # Connect sensors
         self._loop.run_until_complete(self._create_sensors(sensor_names))
         for sensor in self._sensors:
             sensor.set_callback(self.__receive_reading)
-        self._is_running = False
 
     def start(self) -> None:
         """
         Start the SensorManager
         :return:
         """
         if not self._loop.is_running():
             self._thread = Thread(target=self._run)
+            self._thread.daemon = True
             self._thread.start()
         self._is_running = True
 
     def stop(self) -> None:
         """
         Stop the SensorManager
         :return:
         """
+        if not self.is_running():
+            return
         if self._loop.is_running():
             self._loop.stop()
         while self._loop.is_running():
             continue
         self._loop.run_until_complete(self._disconnect_sensors())
         self._clear_queue()
         self._is_running = False
 
     def is_running(self) -> bool:
+        """
+        Check whether the SensorManager is running.
+        :return: Boolean representing the running state of the SensorManager.
+        """
         return self._is_running
 
     def _run(self) -> None:
         self._loop.create_task(self._connect_sensors())
         self._loop.run_forever()
 
     async def _connect_sensors(self) -> None:
@@ -130,7 +140,8 @@
         measurements = self.get_measurements()
         file_contents = json.dumps({'sample_rate': self._sample_rate, 'data': measurements})
         with open(filename+'.tb', 'x') as f:
             f.write(file_contents)
 
     def __del__(self):
         self.stop()
+
```

### Comparing `CreaTeBME-1.0.0/src/CreaTeBME/connect.py` & `CreaTeBME-1.0.1/src/CreaTeBME/connect.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from bleak import BleakScanner
 from typing import List
 from .ImuSensor import ImuSensor
+from .uuids import IMU_SERVICE_UUID
 
 
 async def connect(sensor_names: List[str]):
     """
     Find the specified sensors and create ImuSensor objects for them.
 
     :param sensor_names: The names of the sensors to connect to
     :return: A list of ImuSensor objects
     """
     devices = await BleakScanner.discover(return_adv=True)
-    imus = list(filter(lambda x: '0ddf5c1d-d269-4b17-bd7f-33a8658f0b89' in x[1][1].service_uuids, devices.items()))
+    imus = list(filter(lambda x: IMU_SERVICE_UUID in x[1][1].service_uuids, devices.items()))
     chosen_imus = list(filter(lambda x: x[1][1].local_name[-4:] in sensor_names, imus))
     sensors = []
     connected_names = []
     for device in chosen_imus:
         sensor = ImuSensor(device[1][0])
         sensors.append(sensor)
         connected_names.append(device[1][1].local_name[-4:])
```

### Comparing `CreaTeBME-1.0.0/src/CreaTeBME.egg-info/PKG-INFO` & `CreaTeBME-1.0.1/src/CreaTeBME.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: CreaTeBME
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python Package for interfacing the bluetooth IMU module for CreaTe M8 BME.
 Home-page: https://github.com/CreaTe-M8-BME/CreaTeBME
 Author: Jonathan Matarazzi
 Author-email: git@jonathanm.nl
 Project-URL: Bug Tracker, https://github.com/CreaTe-M8-BME/CreaTeBME/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CreaTeBME
+
+[![PyPI](https://img.shields.io/pypi/v/CreaTeBME)](https://pypi.org/project/CreaTeBME/)
+
 Python Package for interfacing the bluetooth IMU module for CreaTe M8 BME.
 
 # Installation
 To install the latest stable version simply run
 ```shell
 pip install CreaTeBME
 ```
@@ -33,15 +36,16 @@
 
 # Start the sensor manager
 manager.start()
 
 while True:
     measurements = manager.get_measurements()
     for sensor, data in measurements.items():
-        print(sensor, len(data))
+        if len(data) > 0:
+            print(sensor, data)
 
 # Stop the sensor manager
 manager.stop()
 ```
 
 # Usage
 
@@ -98,8 +102,8 @@
 async def connect():
     devices = await BleakScanner.discover(return_adv=True)
     sensor = ImuSensor(devices[0])
 ```
 
 # API reference
 
-For the API reference look [here](./docs/api.md)
+For the API reference look [here](https://github.com/CreaTe-M8-BME/CreaTeBME/blob/main/docs/README.md)
```

