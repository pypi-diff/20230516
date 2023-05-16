# Comparing `tmp/pyworxcloud-3.1.4.tar.gz` & `tmp/pyworxcloud-3.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyworxcloud-3.1.4.tar", max compression
+gzip compressed data, was "pyworxcloud-3.1.5.tar", max compression
```

## Comparing `pyworxcloud-3.1.4.tar` & `pyworxcloud-3.1.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0    35149 2023-04-21 12:27:53.534131 pyworxcloud-3.1.4/LICENSE
--rw-r--r--   0        0        0      929 2023-04-21 12:27:53.534131 pyworxcloud-3.1.4/README.md
--rw-r--r--   0        0        0      609 2023-04-21 12:28:09.086120 pyworxcloud-3.1.4/pyproject.toml
--rw-r--r--   0        0        0    28713 2023-04-21 12:27:53.534131 pyworxcloud-3.1.4/pyworxcloud/__init__.py
--rw-r--r--   0        0        0     4736 2023-04-21 12:27:53.534131 pyworxcloud-3.1.4/pyworxcloud/api.py
--rw-r--r--   0        0        0     1134 2023-04-21 12:27:53.534131 pyworxcloud-3.1.4/pyworxcloud/clouds.py
--rw-r--r--   0        0        0      927 2023-04-21 12:27:53.534131 pyworxcloud-3.1.4/pyworxcloud/const.py
--rw-r--r--   0        0        0      204 2023-04-21 12:27:53.534131 pyworxcloud-3.1.4/pyworxcloud/day_map.py
--rw-r--r--   0        0        0     3647 2023-04-21 12:27:53.534131 pyworxcloud-3.1.4/pyworxcloud/events.py
--rw-r--r--   0        0        0     1918 2023-04-21 12:27:53.534131 pyworxcloud-3.1.4/pyworxcloud/exceptions.py
--rw-r--r--   0        0        0      204 2023-04-21 12:27:53.534131 pyworxcloud-3.1.4/pyworxcloud/helpers/__init__.py
--rw-r--r--   0        0        0      637 2023-04-21 12:27:53.534131 pyworxcloud-3.1.4/pyworxcloud/helpers/logger.py
--rw-r--r--   0        0        0     2794 2023-04-21 12:27:53.534131 pyworxcloud-3.1.4/pyworxcloud/helpers/time_format.py
--rw-r--r--   0        0        0      838 2023-04-21 12:27:53.538132 pyworxcloud-3.1.4/pyworxcloud/utils/__init__.py
--rw-r--r--   0        0        0     3338 2023-04-21 12:27:53.538132 pyworxcloud-3.1.4/pyworxcloud/utils/battery.py
--rw-r--r--   0        0        0     2091 2023-04-21 12:27:53.538132 pyworxcloud-3.1.4/pyworxcloud/utils/blades.py
--rw-r--r--   0        0        0     1924 2023-04-21 12:27:53.538132 pyworxcloud-3.1.4/pyworxcloud/utils/capability.py
--rw-r--r--   0        0        0     3619 2023-04-21 12:27:53.538132 pyworxcloud-3.1.4/pyworxcloud/utils/devices.py
--rw-r--r--   0        0        0      617 2023-04-21 12:27:53.538132 pyworxcloud-3.1.4/pyworxcloud/utils/firmware.py
--rw-r--r--   0        0        0      281 2023-04-21 12:27:53.538132 pyworxcloud-3.1.4/pyworxcloud/utils/landroid_class.py
--rw-r--r--   0        0        0      306 2023-04-21 12:27:53.538132 pyworxcloud-3.1.4/pyworxcloud/utils/lawn.py
--rw-r--r--   0        0        0      427 2023-04-21 12:27:53.538132 pyworxcloud-3.1.4/pyworxcloud/utils/location.py
--rw-r--r--   0        0        0     8183 2023-04-21 12:27:53.538132 pyworxcloud-3.1.4/pyworxcloud/utils/mqtt.py
--rw-r--r--   0        0        0      411 2023-04-21 12:27:53.538132 pyworxcloud-3.1.4/pyworxcloud/utils/orientation.py
--rw-r--r--   0        0        0     1348 2023-04-21 12:27:53.538132 pyworxcloud-3.1.4/pyworxcloud/utils/product.py
--rw-r--r--   0        0        0     1109 2023-04-21 12:27:53.538132 pyworxcloud-3.1.4/pyworxcloud/utils/rainsensor.py
--rw-r--r--   0        0        0     3188 2023-04-21 12:27:53.538132 pyworxcloud-3.1.4/pyworxcloud/utils/requests.py
--rw-r--r--   0        0        0     6191 2023-04-21 12:27:53.538132 pyworxcloud-3.1.4/pyworxcloud/utils/schedules.py
--rw-r--r--   0        0        0     2050 2023-04-21 12:27:53.538132 pyworxcloud-3.1.4/pyworxcloud/utils/state.py
--rw-r--r--   0        0        0      657 2023-04-21 12:27:53.538132 pyworxcloud-3.1.4/pyworxcloud/utils/statistics.py
--rw-r--r--   0        0        0      726 2023-04-21 12:27:53.538132 pyworxcloud-3.1.4/pyworxcloud/utils/warranty.py
--rw-r--r--   0        0        0     1423 2023-04-21 12:27:53.538132 pyworxcloud-3.1.4/pyworxcloud/utils/zone.py
--rw-r--r--   0        0        0     1747 1970-01-01 00:00:00.000000 pyworxcloud-3.1.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-16 12:31:04.655244 pyworxcloud-3.1.5/LICENSE
+-rw-r--r--   0        0        0      929 2023-05-16 12:31:04.655244 pyworxcloud-3.1.5/README.md
+-rw-r--r--   0        0        0      609 2023-05-16 12:31:18.587281 pyworxcloud-3.1.5/pyproject.toml
+-rw-r--r--   0        0        0    29410 2023-05-16 12:31:04.659244 pyworxcloud-3.1.5/pyworxcloud/__init__.py
+-rw-r--r--   0        0        0     4736 2023-05-16 12:31:04.659244 pyworxcloud-3.1.5/pyworxcloud/api.py
+-rw-r--r--   0        0        0     1134 2023-05-16 12:31:04.659244 pyworxcloud-3.1.5/pyworxcloud/clouds.py
+-rw-r--r--   0        0        0      927 2023-05-16 12:31:04.659244 pyworxcloud-3.1.5/pyworxcloud/const.py
+-rw-r--r--   0        0        0      204 2023-05-16 12:31:04.659244 pyworxcloud-3.1.5/pyworxcloud/day_map.py
+-rw-r--r--   0        0        0     3647 2023-05-16 12:31:04.659244 pyworxcloud-3.1.5/pyworxcloud/events.py
+-rw-r--r--   0        0        0     1918 2023-05-16 12:31:04.659244 pyworxcloud-3.1.5/pyworxcloud/exceptions.py
+-rw-r--r--   0        0        0      204 2023-05-16 12:31:04.659244 pyworxcloud-3.1.5/pyworxcloud/helpers/__init__.py
+-rw-r--r--   0        0        0      637 2023-05-16 12:31:04.659244 pyworxcloud-3.1.5/pyworxcloud/helpers/logger.py
+-rw-r--r--   0        0        0     2794 2023-05-16 12:31:04.659244 pyworxcloud-3.1.5/pyworxcloud/helpers/time_format.py
+-rw-r--r--   0        0        0      838 2023-05-16 12:31:04.659244 pyworxcloud-3.1.5/pyworxcloud/utils/__init__.py
+-rw-r--r--   0        0        0     3338 2023-05-16 12:31:04.659244 pyworxcloud-3.1.5/pyworxcloud/utils/battery.py
+-rw-r--r--   0        0        0     2091 2023-05-16 12:31:04.659244 pyworxcloud-3.1.5/pyworxcloud/utils/blades.py
+-rw-r--r--   0        0        0     1924 2023-05-16 12:31:04.659244 pyworxcloud-3.1.5/pyworxcloud/utils/capability.py
+-rw-r--r--   0        0        0     3623 2023-05-16 12:31:04.659244 pyworxcloud-3.1.5/pyworxcloud/utils/devices.py
+-rw-r--r--   0        0        0      617 2023-05-16 12:31:04.659244 pyworxcloud-3.1.5/pyworxcloud/utils/firmware.py
+-rw-r--r--   0        0        0      281 2023-05-16 12:31:04.659244 pyworxcloud-3.1.5/pyworxcloud/utils/landroid_class.py
+-rw-r--r--   0        0        0      306 2023-05-16 12:31:04.659244 pyworxcloud-3.1.5/pyworxcloud/utils/lawn.py
+-rw-r--r--   0        0        0      427 2023-05-16 12:31:04.659244 pyworxcloud-3.1.5/pyworxcloud/utils/location.py
+-rw-r--r--   0        0        0     8300 2023-05-16 12:31:04.659244 pyworxcloud-3.1.5/pyworxcloud/utils/mqtt.py
+-rw-r--r--   0        0        0      411 2023-05-16 12:31:04.659244 pyworxcloud-3.1.5/pyworxcloud/utils/orientation.py
+-rw-r--r--   0        0        0     1348 2023-05-16 12:31:04.659244 pyworxcloud-3.1.5/pyworxcloud/utils/product.py
+-rw-r--r--   0        0        0     1109 2023-05-16 12:31:04.659244 pyworxcloud-3.1.5/pyworxcloud/utils/rainsensor.py
+-rw-r--r--   0        0        0     3188 2023-05-16 12:31:04.659244 pyworxcloud-3.1.5/pyworxcloud/utils/requests.py
+-rw-r--r--   0        0        0     6191 2023-05-16 12:31:04.659244 pyworxcloud-3.1.5/pyworxcloud/utils/schedules.py
+-rw-r--r--   0        0        0     2050 2023-05-16 12:31:04.659244 pyworxcloud-3.1.5/pyworxcloud/utils/state.py
+-rw-r--r--   0        0        0      657 2023-05-16 12:31:04.659244 pyworxcloud-3.1.5/pyworxcloud/utils/statistics.py
+-rw-r--r--   0        0        0      726 2023-05-16 12:31:04.659244 pyworxcloud-3.1.5/pyworxcloud/utils/warranty.py
+-rw-r--r--   0        0        0     1763 2023-05-16 12:31:04.659244 pyworxcloud-3.1.5/pyworxcloud/utils/zone.py
+-rw-r--r--   0        0        0     1747 1970-01-01 00:00:00.000000 pyworxcloud-3.1.5/PKG-INFO
```

### Comparing `pyworxcloud-3.1.4/LICENSE` & `pyworxcloud-3.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.4/README.md` & `pyworxcloud-3.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.4/pyproject.toml` & `pyworxcloud-3.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pyworxcloud"
-version = "v3.1.4"
+version = "v3.1.5"
 description = "Landroid cloud (Positec) API library"
 authors = ["Malene Trab <malene@trab.dk>"]
 documentation = "https://github.com/mtrab/pyworxcloud"
 classifiers = [
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
```

### Comparing `pyworxcloud-3.1.4/pyworxcloud/__init__.py` & `pyworxcloud-3.1.5/pyworxcloud/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -270,52 +270,63 @@
     @property
     def auth_result(self) -> bool:
         """Return current authentication result."""
         return self._auth_result
 
     def _on_update(self, payload):  # , topic, payload, dup, qos, retain, **kwargs):
         """Triggered when a MQTT message was received."""
-        data = json.loads(payload)
         logger = self._log.getChild("MQTT_data_in")
-        logger.debug("MQTT data received")
-        # logger.debug("MQTT data received '%s' on topic '%s'", payload, topic)
-
-        for mower in self._mowers:
-            if mower["serial_number"] == data["cfg"]["sn"]:
-                break
+        try:
+            data = json.loads(payload)
+            logger.debug("MQTT data received")
+
+            # "Malformed" message, we are missing a serial number and MAC address to identify the mower.
+            if not "sn" in data["cfg"] and not "mac" in data["dat"]:
+                return
+
+            for mower in self._mowers:
+                if "sn" in data["cfg"]:
+                    if mower["serial_number"] == data["cfg"]["sn"]:
+                        break
+                else:
+                    if mower["mac_address"] == data["dat"]["mac"]:
+                        break
 
-        device: DeviceHandler = self.devices[mower["name"]]
+            device: DeviceHandler = self.devices[mower["name"]]
 
-        while not device.is_decoded:
-            pass  # Wait for last dataset to be handled
+            while not device.is_decoded:
+                pass  # Wait for last dataset to be handled
 
-        if device.raw_data == data:
-            self._log.debug("Data was already present and not changed.")
-            return  # Dataset was not changed, no update needed
+            if device.raw_data == data:
+                self._log.debug("Data was already present and not changed.")
+                return  # Dataset was not changed, no update needed
 
-        device.raw_data = payload
-        self._decode_data(device)
+            device.raw_data = payload
+            self._decode_data(device)
 
-        self._events.call(
-            LandroidEvent.DATA_RECEIVED, name=mower["name"], device=device
-        )
+            self._events.call(
+                LandroidEvent.DATA_RECEIVED, name=mower["name"], device=device
+            )
+        except json.decoder.JSONDecodeError:
+            logger.debug("Malformed MQTT message received")
+            pass
 
     def _decode_data(self, device: DeviceHandler) -> None:
         """Decode incoming JSON data."""
         device.is_decoded = False
 
         logger = self._log.getChild("decode_data")
         logger.debug("Data decoding for %s started", device.name)
 
         if device.json_data:
             logger.debug("Found JSON decoded data: %s", device.json_data)
             data = device.json_data
         elif device.raw_data:
             logger.debug("Found raw data: %s", device.raw_data)
-            data = json.loads(device.raw_data)
+            data = device.raw_data
         else:
             device.is_decoded = True
             logger.debug("No valid data was found, skipping update for %s", device.name)
             return
 
         # device.firmware["version"] = "{:.2f}".format(device.firmware["version"])
         if "dat" in data:
@@ -433,59 +444,59 @@
                     )
                     end_time = time_start + timedelta(minutes=duration)
 
                     device.schedules[TYPE_TO_STRING[sch_type]][DAY_MAP[day]][
                         "end"
                     ] = end_time.time().strftime("%H:%M")
 
-            # Fetch secondary schedule
-            if "dd" in data["cfg"]["sc"]:
-                sch_type = ScheduleType.SECONDARY
-                device.schedules.update({TYPE_TO_STRING[sch_type]: Weekdays()})
-
-                for day in range(0, len(data["cfg"]["sc"]["d"])):
-                    device.schedules[TYPE_TO_STRING[sch_type]][DAY_MAP[day]][
-                        "start"
-                    ] = data["cfg"]["sc"]["dd"][day][0]
-                    device.schedules[TYPE_TO_STRING[sch_type]][DAY_MAP[day]][
-                        "duration"
-                    ] = data["cfg"]["sc"]["dd"][day][1]
-                    device.schedules[TYPE_TO_STRING[sch_type]][DAY_MAP[day]][
-                        "boundary"
-                    ] = bool(data["cfg"]["sc"]["dd"][day][2])
-
-                    time_start = datetime.strptime(
-                        data["cfg"]["sc"]["dd"][day][0],
-                        "%H:%M",
-                    )
+                # Fetch secondary schedule
+                if "dd" in data["cfg"]["sc"]:
+                    sch_type = ScheduleType.SECONDARY
+                    device.schedules.update({TYPE_TO_STRING[sch_type]: Weekdays()})
 
-                    if isinstance(
+                    for day in range(0, len(data["cfg"]["sc"]["dd"])):
                         device.schedules[TYPE_TO_STRING[sch_type]][DAY_MAP[day]][
-                            "duration"
-                        ],
-                        type(None),
-                    ):
+                            "start"
+                        ] = data["cfg"]["sc"]["dd"][day][0]
                         device.schedules[TYPE_TO_STRING[sch_type]][DAY_MAP[day]][
                             "duration"
-                        ] = "0"
-
-                    duration = int(
+                        ] = data["cfg"]["sc"]["dd"][day][1]
                         device.schedules[TYPE_TO_STRING[sch_type]][DAY_MAP[day]][
-                            "duration"
-                        ]
-                    )
+                            "boundary"
+                        ] = bool(data["cfg"]["sc"]["dd"][day][2])
 
-                    duration = duration * (
-                        1 + (int(device.schedules["time_extension"]) / 100)
-                    )
-                    end_time = time_start + timedelta(minutes=duration)
+                        time_start = datetime.strptime(
+                            data["cfg"]["sc"]["dd"][day][0],
+                            "%H:%M",
+                        )
+
+                        if isinstance(
+                            device.schedules[TYPE_TO_STRING[sch_type]][DAY_MAP[day]][
+                                "duration"
+                            ],
+                            type(None),
+                        ):
+                            device.schedules[TYPE_TO_STRING[sch_type]][DAY_MAP[day]][
+                                "duration"
+                            ] = "0"
+
+                        duration = int(
+                            device.schedules[TYPE_TO_STRING[sch_type]][DAY_MAP[day]][
+                                "duration"
+                            ]
+                        )
+
+                        duration = duration * (
+                            1 + (int(device.schedules["time_extension"]) / 100)
+                        )
+                        end_time = time_start + timedelta(minutes=duration)
 
-                    device.schedules[TYPE_TO_STRING[sch_type]][DAY_MAP[day]][
-                        "end"
-                    ] = end_time.time().strftime("%H:%M")
+                        device.schedules[TYPE_TO_STRING[sch_type]][DAY_MAP[day]][
+                            "end"
+                        ] = end_time.time().strftime("%H:%M")
 
             device.schedules.update_progress_and_next(
                 tz=self._tz
                 if not isinstance(self._tz, type(None))
                 else device.time_zone
             )
 
@@ -501,14 +512,15 @@
         self._mowers = self._api.get_mowers()
 
         for mower in self._mowers:
             device = DeviceHandler(self._api, mower)
             _LOGGER.debug("Mower '%s' data: %s", mower["name"], mower)
             self.devices.update({mower["name"]: device})
 
+            device.raw_data = mower["last_status"]["payload"]
             self._decode_data(device)
 
     def get_mower(self, serial_number: str) -> dict:
         """Get a specific mower."""
         for mower in self._mowers:
             if mower["serial_number"] == serial_number:
                 return mower
@@ -659,15 +671,15 @@
                     else {"sc": {"m": 1, "distm": 0}},
                 )
             elif not device.capabilities.check(DeviceCapability.PARTY_MODE):
                 raise NoPartymodeError("This device does not support Partymode")
         elif not mower["online"]:
             raise OfflineError("The device is currently offline, no action was sent.")
 
-    def setzone(self, serial_number: str, zone: str) -> None:
+    def setzone(self, serial_number: str, zone: str | int) -> None:
         """Set zone to be mowed when next mowing task is started.
 
         Args:
             zone (str | int): Zone to mow, valid possibilities are a number from 1 to 4.
 
         Raises:
             OfflineError: Raised if the device is offline.
```

### Comparing `pyworxcloud-3.1.4/pyworxcloud/api.py` & `pyworxcloud-3.1.5/pyworxcloud/api.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.4/pyworxcloud/clouds.py` & `pyworxcloud-3.1.5/pyworxcloud/clouds.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.4/pyworxcloud/const.py` & `pyworxcloud-3.1.5/pyworxcloud/const.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.4/pyworxcloud/events.py` & `pyworxcloud-3.1.5/pyworxcloud/events.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.4/pyworxcloud/exceptions.py` & `pyworxcloud-3.1.5/pyworxcloud/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.4/pyworxcloud/helpers/logger.py` & `pyworxcloud-3.1.5/pyworxcloud/helpers/logger.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.4/pyworxcloud/helpers/time_format.py` & `pyworxcloud-3.1.5/pyworxcloud/helpers/time_format.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.4/pyworxcloud/utils/__init__.py` & `pyworxcloud-3.1.5/pyworxcloud/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.4/pyworxcloud/utils/battery.py` & `pyworxcloud-3.1.5/pyworxcloud/utils/battery.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.4/pyworxcloud/utils/blades.py` & `pyworxcloud-3.1.5/pyworxcloud/utils/blades.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.4/pyworxcloud/utils/capability.py` & `pyworxcloud-3.1.5/pyworxcloud/utils/capability.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.4/pyworxcloud/utils/devices.py` & `pyworxcloud-3.1.5/pyworxcloud/utils/devices.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         self.blades = Blades(data)
         self.chassis = ProductInfo(InfoType.MOWER, api, data["product_id"])
         self.error = States(StateType.ERROR)
         self.orientation = Orientation([0, 0, 0])
         self.capabilities = Capability(data)
         self.rainsensor = Rainsensor()
         self.status = States()
-        self.zone = Zone()
+        self.zone = Zone(data)
         self.warranty = Warranty(data)
         self.firmware = Firmware(data)
         self.schedules = Schedule(data)
         self.in_topic = data["mqtt_topics"]["command_in"]
         self.out_topic = data["mqtt_topics"]["command_out"]
 
         if data in ["lawn_perimeter", "lawn_size"]:
```

### Comparing `pyworxcloud-3.1.4/pyworxcloud/utils/firmware.py` & `pyworxcloud-3.1.5/pyworxcloud/utils/firmware.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.4/pyworxcloud/utils/mqtt.py` & `pyworxcloud-3.1.5/pyworxcloud/utils/mqtt.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,16 +214,19 @@
                 )
                 self.client.reconnect()
 
     def disconnect(
         self, reasoncode=None, properties=None  # pylint: disable=unused-argument
     ):
         """Disconnect from AWSIoT MQTT server."""
+        logger = self._log.getChild("MQTT_Disconnect")
         for topic in self._topic:
-            self.client.unsubscribe(self._topic.pop(topic))
+            logger.debug("Unsubscribing '%s'", topic)
+            self.client.unsubscribe(topic)
+        self._topic = []
         self._disconnected = True
         self.client.loop_stop()
         self.client.disconnect()
 
     def ping(self, serial_number: str, topic: str) -> None:
         """Ping (update) the mower."""
         cmd = self.format_message(serial_number, {"cmd": Command.FORCE_REFRESH})
```

### Comparing `pyworxcloud-3.1.4/pyworxcloud/utils/product.py` & `pyworxcloud-3.1.5/pyworxcloud/utils/product.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.4/pyworxcloud/utils/rainsensor.py` & `pyworxcloud-3.1.5/pyworxcloud/utils/rainsensor.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.4/pyworxcloud/utils/requests.py` & `pyworxcloud-3.1.5/pyworxcloud/utils/requests.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.4/pyworxcloud/utils/schedules.py` & `pyworxcloud-3.1.5/pyworxcloud/utils/schedules.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.4/pyworxcloud/utils/state.py` & `pyworxcloud-3.1.5/pyworxcloud/utils/state.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.4/pyworxcloud/utils/statistics.py` & `pyworxcloud-3.1.5/pyworxcloud/utils/statistics.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.4/pyworxcloud/utils/warranty.py` & `pyworxcloud-3.1.5/pyworxcloud/utils/warranty.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.4/pyworxcloud/utils/zone.py` & `pyworxcloud-3.1.5/pyworxcloud/utils/zone.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,23 +3,31 @@
 
 from .landroid_class import LDict
 
 
 class Zone(LDict):
     """Class for handling zone data."""
 
-    def __init__(self) -> dict:
+    def __init__(self, data) -> dict:
         """Initialize zone object."""
         super().__init__()
 
         self["current"] = None
         self["index"] = None
         self["indicies"] = [0, 0, 0, 0, 0, 0, 0, 0, 0, 0]
         self["starting_point"] = [0, 0, 0, 0]
 
+        if not "last_status" in data:
+            return
+
+        self["index"] = data["last_status"]["payload"]["dat"]["lz"]
+        self["indicies"] = data["last_status"]["payload"]["cfg"]["mzv"]
+        self["starting_point"] = data["last_status"]["payload"]["cfg"]["mz"]
+        self["current"] = self["indicies"][self["index"]]
+
     @property
     def current(self) -> int:
         """Get current zone."""
         return self["current"]
 
     @current.setter
     def current(self, value: int) -> None:
```

### Comparing `pyworxcloud-3.1.4/PKG-INFO` & `pyworxcloud-3.1.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyworxcloud
-Version: 3.1.4
+Version: 3.1.5
 Summary: Landroid cloud (Positec) API library
 License: MIT
 Author: Malene Trab
 Author-email: malene@trab.dk
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyworxcloud Version: 3.1.4 Summary: Landroid cloud
+Metadata-Version: 2.1 Name: pyworxcloud Version: 3.1.5 Summary: Landroid cloud
 (Positec) API library License: MIT Author: Malene Trab Author-email:
 malene@trab.dk Requires-Python: >=3.9,<4.0 Classifier: License :: OSI Approved
 :: MIT License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Topic :: Software Development :: Libraries :: Python Modules Requires-Dist:
 paho-mqtt (>=1.6.1,<2.0.0) Requires-Dist: requests (>=2.26.0,<3.0.0) Requires-
```

