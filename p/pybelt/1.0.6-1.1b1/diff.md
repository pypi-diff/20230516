# Comparing `tmp/pybelt-1.0.6.tar.gz` & `tmp/pybelt-1.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pybelt-1.0.6.tar", last modified: Mon May  8 14:04:18 2023, max compression
+gzip compressed data, was "dist\pybelt-1.1b1.tar", last modified: Tue May 16 07:31:38 2023, max compression
```

## Comparing `pybelt-1.0.6.tar` & `pybelt-1.1b1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 14:04:18.000000 pybelt-1.0.6/
--rw-rw-rw-   0        0        0     2472 2023-05-08 14:04:18.000000 pybelt-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1636 2021-01-11 09:49:47.000000 pybelt-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-08 14:04:18.000000 pybelt-1.0.6/pybelt/
--rw-rw-rw-   0        0        0      112 2020-06-22 14:06:02.000000 pybelt-1.0.6/pybelt/__init__.py
--rw-rw-rw-   0        0        0    39138 2023-05-08 13:57:43.000000 pybelt-1.0.6/pybelt/_communication_interface.py
--rw-rw-rw-   0        0        0     8833 2023-01-05 13:18:44.000000 pybelt-1.0.6/pybelt/_gatt_profile.py
--rw-rw-rw-   0        0        0    59384 2023-01-06 13:19:56.000000 pybelt-1.0.6/pybelt/belt_controller.py
--rw-rw-rw-   0        0        0     3509 2023-01-04 13:32:18.000000 pybelt-1.0.6/pybelt/belt_scanner.py
-drwxrwxrwx   0        0        0        0 2023-05-08 14:04:18.000000 pybelt-1.0.6/pybelt.egg-info/
--rw-rw-rw-   0        0        0     2472 2023-05-08 14:04:17.000000 pybelt-1.0.6/pybelt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      294 2023-05-08 14:04:18.000000 pybelt-1.0.6/pybelt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 14:04:17.000000 pybelt-1.0.6/pybelt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-08 14:04:17.000000 pybelt-1.0.6/pybelt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-08 14:04:17.000000 pybelt-1.0.6/pybelt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-08 14:04:18.000000 pybelt-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      759 2023-05-08 14:03:54.000000 pybelt-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 07:31:38.000000 pybelt-1.1b1/
+-rw-rw-rw-   0        0        0     2472 2023-05-16 07:31:38.000000 pybelt-1.1b1/PKG-INFO
+-rw-rw-rw-   0        0        0     1636 2021-01-11 09:49:47.000000 pybelt-1.1b1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-16 07:31:38.000000 pybelt-1.1b1/pybelt/
+-rw-rw-rw-   0        0        0      112 2020-06-22 14:06:02.000000 pybelt-1.1b1/pybelt/__init__.py
+-rw-rw-rw-   0        0        0    37069 2023-05-16 07:04:42.000000 pybelt-1.1b1/pybelt/_communication_interface.py
+-rw-rw-rw-   0        0        0     8833 2023-01-05 13:18:44.000000 pybelt-1.1b1/pybelt/_gatt_profile.py
+-rw-rw-rw-   0        0        0    59380 2023-05-09 09:02:51.000000 pybelt-1.1b1/pybelt/belt_controller.py
+-rw-rw-rw-   0        0        0     3980 2023-05-15 13:07:23.000000 pybelt-1.1b1/pybelt/belt_scanner.py
+drwxrwxrwx   0        0        0        0 2023-05-16 07:31:38.000000 pybelt-1.1b1/pybelt.egg-info/
+-rw-rw-rw-   0        0        0     2472 2023-05-16 07:31:38.000000 pybelt-1.1b1/pybelt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2023-05-16 07:31:38.000000 pybelt-1.1b1/pybelt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 07:31:38.000000 pybelt-1.1b1/pybelt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-16 07:31:38.000000 pybelt-1.1b1/pybelt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-16 07:31:38.000000 pybelt-1.1b1/pybelt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-16 07:31:38.000000 pybelt-1.1b1/setup.cfg
+-rw-rw-rw-   0        0        0      759 2023-05-16 07:31:01.000000 pybelt-1.1b1/setup.py
```

### Comparing `pybelt-1.0.6/PKG-INFO` & `pybelt-1.1b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybelt
-Version: 1.0.6
+Version: 1.1b1
 Summary: An Python library to control the feelSpace naviBelt from your application
 Home-page: https://github.com/feelSpace/pybelt
 Author: feelSpace GmbH
 Author-email: dev@feelspace.de
 License: UNKNOWN
 Description: # pyBelt
```

### Comparing `pybelt-1.0.6/README.md` & `pybelt-1.1b1/README.md`

 * *Files identical despite different names*

### Comparing `pybelt-1.0.6/pybelt/_communication_interface.py` & `pybelt-1.1b1/pybelt/_communication_interface.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 import sys
 import threading
 import time
 import logging
 
 import bleak
 import serial
-from bleak import BleakScanner, BleakClient
+from bleak import BleakScanner, BleakClient, BleakGATTCharacteristic
 from bleak.backends.device import BLEDevice
+from pybelt import belt_scanner
 
 from pybelt._gatt_profile import *
 
 SERIAL_BAUDRATE = 115200
 # Baudrate for serial connection
 
 SERIAL_READ_TIMEOUT = 0.50
@@ -475,15 +476,15 @@
 
         :param BeltCommunicationDelegate delegate:
             The delegate that handles received notifications.
         """
         threading.Thread.__init__(self, name="BleInterfaceThread")
         self._device = None
         self._delegate = delegate
-        self._gatt_client = None
+        self._gatt_client = None  # type: Optional[BleakClient]
         self._event_loop = None
         self._event_loop_ready = threading.Event()
         self._event_notifier = None
         self._is_disconnecting = False
         self._expect_disconnection = False
         # Logger
         self.logger = logging.getLogger(__name__)
@@ -507,27 +508,31 @@
         self._event_loop_ready.clear()
         self.start()
         self._event_loop_ready.wait(EVENT_LOOP_READY_TIMEOUT)
         # Retrieve device
         self._device = device
         if self._device is None:
             try:
-                future = asyncio.run_coroutine_threadsafe(self._scan(), self._event_loop)
-                self._device = future.result()
+                # Use belt scanner to find the first belt
+                belts = []
+                with belt_scanner.create() as scanner:
+                    belts = scanner.scan()
+                if not belts:
+                    self._device = belts[0]
             except:
-                self.logger.exception("BleInterface: Error when scheduling scan!")
+                self.logger.exception("BleInterface: Error when scanning!")
                 self.close()
                 raise
         if self._device is None:
             raise Exception("No belt found via BLE.")
         try:
             # Connect to device
             future = asyncio.run_coroutine_threadsafe(self._connect(), self._event_loop)
             connected = future.result()
-            if not connected:
+            if not connected or self._gatt_client is None:
                 self.close()
                 raise Exception("BLE connection failed.")
             # Retrieve profile / Service discovery (automatic)
             self._fill_gatt_profile(self._gatt_client.services)
         except:
             # Disconnect and re-raise exception
             self.logger.exception("BleInterface: Error when scheduling connection!")
@@ -547,43 +552,25 @@
         :return bleak.backends.device.BLEDevice: The connected device.
         """
         return self._device
 
     # --------------------------------------------------------------- #
     # Private methods
 
-    async def _scan(self) -> BLEDevice:
-        """Scans for a belt.
-        """
-        self.logger.debug("BleInterface: Scan for belt.")
-        try:
-            devices = await BleakScanner.discover()
-            for d in devices:
-                # Check for service UUID
-                if 'uuids' in d.metadata:
-                    for uuid in d.metadata['uuids']:
-                        if isinstance(uuid, str) and "65333333-a115-11e2-9e9a-0800200ca100" in uuid.lower():
-                            self.logger.debug("BleInterface: Belt found.")
-                            self._device = d
-                            return d
-            self.logger.debug("BleInterface: No belt found!")
-        except:
-            self.logger.exception("BleInterface: Error when scanning!")
-
     async def _connect(self) -> bool:
         """
         Connects the belt.
         :return: 'True' if successful, 'False' otherwise.
         """
         try:
             self.logger.debug("BleInterface: Connect client.")
             self._gatt_client = BleakClient(
-                self._device.address,
-                loop=self._event_loop,
-                disconnected_callback=self._on_device_disconnected)
+                self._device,
+                disconnected_callback=self._on_device_disconnected,
+                loop=self._event_loop)
             await self._gatt_client.connect()
         except:
             self.logger.exception("BleInterface: Error when connecting!")
             return False
         self.logger.debug("BleInterface: Client connected.")
         return True
 
@@ -591,16 +578,15 @@
         """
         Disconnects the device.
         :return: 'True' if successful, 'False' otherwise.
         """
         success = True
         try:
             if self._gatt_client is not None:
-                connected = await self._gatt_client.is_connected()
-                if connected:
+                if self._gatt_client.is_connected:
                     self.logger.debug("BleInterface: Disconnect client.")
                     success = await self._gatt_client.disconnect()
                 else:
                     self.logger.debug("BleInterface: Client already disconnected.")
         except:
             self.logger.exception("BleInterface: Error when disconnecting!")
             success = False
@@ -613,16 +599,15 @@
         :param bytes data: The data to write.
         :return: 'True' if successful, 'False' otherwise.
         """
         try:
             if self._gatt_client is None:
                 self.logger.warning("BleInterface: No connection to write char!")
                 return False
-            connected = await self._gatt_client.is_connected()
-            if not connected:
+            if not self._gatt_client.is_connected:
                 self.logger.warning("BleInterface: No connection to set notifications!")
                 return False
             await self._gatt_client.write_gatt_char(gatt_char.uuid, bytearray(data), response=True)
         except:
             self.logger.exception("BleInterface: Error when writing characteristic.")
             return False
         return True
@@ -634,16 +619,15 @@
         :param enabled: 'True' to enable notifications, 'False' to disable notifications.
         :return: 'True' if successful, 'False' otherwise.
         """
         try:
             if self._gatt_client is None:
                 self.logger.warning("BleInterface: No connection to set notifications!")
                 return False
-            connected = await self._gatt_client.is_connected()
-            if not connected:
+            if not self._gatt_client.is_connected:
                 self.logger.warning("BleInterface: No connection to set notifications!")
                 return False
             if enabled:
                 await self._gatt_client.start_notify(gatt_char.uuid, self._on_notification_received)
             else:
                 await self._gatt_client.stop_notify(gatt_char.uuid)
         except:
@@ -657,16 +641,15 @@
         :param GattCharacteristic gatt_char: The GATT characteristic to read.
         :return: 'True' if successful, 'False' otherwise.
         """
         try:
             if self._gatt_client is None:
                 self.logger.warning("BleInterface: No connection to read char!")
                 return False
-            connected = await self._gatt_client.is_connected()
-            if not connected:
+            if not self._gatt_client.is_connected:
                 self.logger.warning("BleInterface: No connection to set notifications!")
                 return False
             value = await self._gatt_client.read_gatt_char(gatt_char.uuid)
         except:
             self.logger.exception("BleInterface: Error when reading characteristic.")
             return False
         try:
@@ -675,69 +658,48 @@
             self.logger.exception("BleInterface: Error when calling delegate method 'on_gatt_char_notified'.")
         return True
 
     def _fill_gatt_profile(self, services):
         """ Fills the gatt profile with attribute handles.
         :param BleakGATTServiceCollection services: The list of services.
         """
+        self.logger.debug("BleInterface: Service discovery.")
         for gatt_char in self._gatt_profile.characteristics:
-            bleak_gatt_char = services.get_characteristic(gatt_char.uuid)
+            bleak_gatt_char: BleakGATTCharacteristic = services.get_characteristic(gatt_char.uuid)
             if bleak_gatt_char is None:
-                self.logger.error("BleInterface: Characteristic not listed for UUID {}".format(gatt_char.uuid))
-            # else: TODO Adds handles
-        # TODO
-        is_new_profile = True
-        try:
-            adv_uuids = self._device.metadata['uuids']
-            for uuid in adv_uuids:
-                if "65333333-a115-11e2-9e9a-0800200ca100" in uuid.lower() or \
-                        "65333333-a115-11e2-9e9a-0800200ca200" in uuid.lower():
-                    is_new_profile = False
-                    break
-        except:
-            pass
-        if is_new_profile:
-            self._gatt_profile.set_char_handles("0000fe01-0000-1000-8000-00805f9b34fb", 8, 9)
-            self._gatt_profile.set_char_handles("0000fe02-0000-1000-8000-00805f9b34fb", 10, 11, [12])
-            self._gatt_profile.set_char_handles("0000fe03-0000-1000-8000-00805f9b34fb", 13, 14)
-            self._gatt_profile.set_char_handles("0000fe04-0000-1000-8000-00805f9b34fb", 15, 16, [17])
-            self._gatt_profile.set_char_handles("0000fe05-0000-1000-8000-00805f9b34fb", 18, 19)
-            self._gatt_profile.set_char_handles("0000fe06-0000-1000-8000-00805f9b34fb", 20, 21, [22])
-            self._gatt_profile.set_char_handles("0000fe09-0000-1000-8000-00805f9b34fb", 28, 29, [30])
-            self._gatt_profile.set_char_handles("0000fe0a-0000-1000-8000-00805f9b34fb", 32, 33)
-            self._gatt_profile.set_char_handles("0000fe0b-0000-1000-8000-00805f9b34fb", 34, 35, [36])
-            self._gatt_profile.set_char_handles("0000fe0c-0000-1000-8000-00805f9b34fb", 37, 38, [39])
-            self._gatt_profile.set_char_handles("0000fe13-0000-1000-8000-00805f9b34fb", 41, 42)
-            self._gatt_profile.set_char_handles("0000fe14-0000-1000-8000-00805f9b34fb", 43, 44, [45])
-        else:
-            self._gatt_profile = get_usb_gatt_profile()
-        self.logger.debug("BLE interface, TBC: UUIDs should be used instead of characteristic handles!")
+                self.logger.error("BleInterface: Characteristic not listed for UUID {}.".format(gatt_char.uuid))
+            else:
+                descriptor_handles = []
+                for descriptor in bleak_gatt_char.descriptors:
+                    descriptor_handles.append(descriptor.handle)
+                self._gatt_profile.set_char_handles(gatt_char.uuid, bleak_gatt_char.handle, bleak_gatt_char.handle + 1,
+                                                    descriptor_handles)
 
     # --------------------------------------------------------------- #
     # Bleak GATT client callback methods
 
-    def _on_notification_received(self, attr_handle, data):
+    def _on_notification_received(self, characteristic, data):
         """
         Callback for notifications.
-        :param int attr_handle: The attribute handle.
+        :param BleakGATTCharacteristic characteristic: The characteristic.
         :param bytearray data: The characteristic notified value.
         """
-        gatt_char = self._gatt_profile.get_char_from_handle(attr_handle)
+        gatt_char = self._gatt_profile.get_char_from_handle(characteristic.handle)
         if gatt_char is None:
-            self.logger.debug("BleInterface: Notification on unsupported handle!")
+            self.logger.debug("BleInterface: Notification on unsupported handle ({})!".format(characteristic.handle))
             return
         try:
             self._event_notifier.notify_gatt_notification(gatt_char, bytes(data))
         except:
             self.logger.exception("BleInterface: Failed to access event notifier!")
 
     def _on_device_disconnected(self, gatt_client):
         """
         Callback on disconnection.
-        :param gatt_client: The GATT client disconnected.
+        :param BleakClient gatt_client: The GATT client disconnected.
         """
         self.logger.debug("BleInterface: Client {} disconnected.".format(gatt_client.address))
         if self._gatt_client is None:
             # Connection already closed
             return
         if self._is_disconnecting:
             # Ignore callback when properly disconnecting from 'close()' call
```

### Comparing `pybelt-1.0.6/pybelt/_gatt_profile.py` & `pybelt-1.1b1/pybelt/_gatt_profile.py`

 * *Files identical despite different names*

### Comparing `pybelt-1.0.6/pybelt/belt_controller.py` & `pybelt-1.1b1/pybelt/belt_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -950,27 +950,27 @@
         sensor_id = int.from_bytes(
             bytes(packet[0:1]),
             byteorder='little',
             signed=False)
         belt_heading = int.from_bytes(
             bytes(packet[1:3]),
             byteorder='little',
-            signed=False)
+            signed=True)
         box_heading = int.from_bytes(
             bytes(packet[3:5]),
             byteorder='little',
-            signed=False)
+            signed=True)
         box_roll = int.from_bytes(
             bytes(packet[5:7]),
             byteorder='little',
-            signed=False)
+            signed=True)
         box_pitch = int.from_bytes(
             bytes(packet[7:9]),
             byteorder='little',
-            signed=False)
+            signed=True)
         accuracy = int.from_bytes(
             bytes(packet[9:11]),
             byteorder='little',
             signed=False)
         mag_stat = int.from_bytes(
             bytes(packet[11:12]),
             byteorder='little',
```

### Comparing `pybelt-1.0.6/pybelt/belt_scanner.py` & `pybelt-1.1b1/pybelt/belt_scanner.py`

 * *Files 16% similar despite different names*

```diff
@@ -65,24 +65,32 @@
         return future.result()
 
     async def _scan(self) -> List[BLEDevice]:
         """Scans for advertising belts (asynchronous).
         """
         self._logger.debug("BeltScanner: Start async scan.")
         belts = []
-        devices = await BleakScanner.discover()
-        for d in devices:
+        devices = await BleakScanner.discover(return_adv=True)
+        for d in devices.values():
             self._logger.debug("BeltScanner: Device found.")
             # Check for service UUID
-            if 'uuids' in d.metadata:
-                for uuid in d.metadata['uuids']:
-                    self._logger.debug("BeltScanner: Advertised UUID {}.".format(uuid))
-                    if isinstance(uuid, str) and ("65333333-a115-11e2-9e9a-0800200ca100" in uuid.lower()
-                                                  or "0000fe51-0000-1000-8000-00805f9b34fb" in uuid.lower()):
-                        belts.append(d)
+            adv_data = d[1]
+            for uuid in adv_data.service_uuids:
+                self._logger.debug("BeltScanner: Advertised UUID {}.".format(uuid))
+                if isinstance(uuid, str) and ("65333333-a115-11e2-9e9a-0800200ca100" in uuid.lower()
+                                              or "0000fe51-0000-1000-8000-00805f9b34fb" in uuid.lower()):
+                    # Check if belt not yet discovered
+                    belt_already_discovered = False
+                    for b in belts:
+                        if isinstance(b.address, str) and isinstance(d[0].address, str) and \
+                                (b.address.lower() == d[0].address.lower()):
+                            belt_already_discovered = True
+                            break
+                    if not belt_already_discovered:
+                        belts.append(d[0])
         self._logger.debug("BeltScanner: End async scan.")
         return belts
 
 
 class _EventLoopThread(threading.Thread):
     """Thread for the event loop.
     """
```

### Comparing `pybelt-1.0.6/pybelt.egg-info/PKG-INFO` & `pybelt-1.1b1/pybelt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybelt
-Version: 1.0.6
+Version: 1.1b1
 Summary: An Python library to control the feelSpace naviBelt from your application
 Home-page: https://github.com/feelSpace/pybelt
 Author: feelSpace GmbH
 Author-email: dev@feelspace.de
 License: UNKNOWN
 Description: # pyBelt
```

### Comparing `pybelt-1.0.6/setup.py` & `pybelt-1.1b1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pybelt",
-    version="1.0.6",
+    version="1.1b1",
     author="feelSpace GmbH",
     author_email="dev@feelspace.de",
     description="An Python library to control the feelSpace naviBelt from your application",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/feelSpace/pybelt",
     packages=setuptools.find_packages(),
```

