# Comparing `tmp/homeduino-0.0.7.tar.gz` & `tmp/homeduino-0.0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "homeduino-0.0.7.tar", last modified: Sun May 14 11:35:23 2023, max compression
+gzip compressed data, was "homeduino-0.0.7.1.tar", last modified: Tue May 16 20:32:37 2023, max compression
```

## Comparing `homeduino-0.0.7.tar` & `homeduino-0.0.7.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:35:23.680281 homeduino-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    35121 2023-05-14 11:35:07.000000 homeduino-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-14 11:35:23.680281 homeduino-0.0.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:35:23.676281 homeduino-0.0.7/homeduino/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-14 11:35:07.000000 homeduino-0.0.7/homeduino/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-05-14 11:35:07.000000 homeduino-0.0.7/homeduino/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11651 2023-05-14 11:35:07.000000 homeduino-0.0.7/homeduino/homeduino.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:35:23.680281 homeduino-0.0.7/homeduino.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-14 11:35:23.000000 homeduino-0.0.7/homeduino.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-14 11:35:23.000000 homeduino-0.0.7/homeduino.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 11:35:23.000000 homeduino-0.0.7/homeduino.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-14 11:35:23.000000 homeduino-0.0.7/homeduino.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-14 11:35:23.000000 homeduino-0.0.7/homeduino.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-14 11:35:07.000000 homeduino-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 11:35:23.680281 homeduino-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:32:37.803748 homeduino-0.0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35121 2023-05-16 20:32:26.000000 homeduino-0.0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-16 20:32:37.803748 homeduino-0.0.7.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:32:37.803748 homeduino-0.0.7.1/homeduino/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-16 20:32:26.000000 homeduino-0.0.7.1/homeduino/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-05-16 20:32:26.000000 homeduino-0.0.7.1/homeduino/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11658 2023-05-16 20:32:26.000000 homeduino-0.0.7.1/homeduino/homeduino.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:32:37.803748 homeduino-0.0.7.1/homeduino.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-16 20:32:37.000000 homeduino-0.0.7.1/homeduino.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-16 20:32:37.000000 homeduino-0.0.7.1/homeduino.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 20:32:37.000000 homeduino-0.0.7.1/homeduino.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-16 20:32:37.000000 homeduino-0.0.7.1/homeduino.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-16 20:32:37.000000 homeduino-0.0.7.1/homeduino.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-16 20:32:26.000000 homeduino-0.0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 20:32:37.803748 homeduino-0.0.7.1/setup.cfg
```

### Comparing `homeduino-0.0.7/LICENSE` & `homeduino-0.0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `homeduino-0.0.7/PKG-INFO` & `homeduino-0.0.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homeduino
-Version: 0.0.7
+Version: 0.0.7.1
 Summary: Homeduino library
 Author: Rogier van Staveren
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/rrooggiieerr/homeduino.py
 Project-URL: Bug Tracker, https://github.com/rrooggiieerr/homeduino.py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
```

### Comparing `homeduino-0.0.7/homeduino/__main__.py` & `homeduino-0.0.7.1/homeduino/__main__.py`

 * *Files identical despite different names*

### Comparing `homeduino-0.0.7/homeduino/homeduino.py` & `homeduino-0.0.7.1/homeduino/homeduino.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
 
     def handle_rf_receive(self, line: str) -> None:
         logger.debug(line)
 
         # The first 8 numbers are the pulse lengths and the last string of numbers is the pulse sequence
         parts = line.split(" ")
 
-        pulse_lengths = [int(i) for i in parts[2:9]]
+        pulse_lengths = [int(i) for i in parts[2:10]]
         # logger.debug("pulse lengths: %s", pulse_lengths)
         pulse_sequence = parts[10]
 
         # Match pulse sequence to a protocol
         decoded = controller.decode_pulses(pulse_lengths, pulse_sequence)
 
         if len(decoded) == 0:
@@ -153,15 +153,15 @@
             logger.error("Not ready")
             raise NotReadyError("Homeduino is not ready")
 
         start_time = datetime.now()
         while self._tx_busy is True:
             logger.debug("Busy")
             if (datetime.now() - start_time).total_seconds() < _BUSY_TIMEOUT:
-                await asyncio.sleep(0.1)
+                await asyncio.sleep(0.01)
             else:
                 logger.error("Too busy to transmit %s", packet)
                 raise TooBusyError("Homeduino is too busy to transmit")
         self._tx_busy = True
 
         try:
             data = packet + "\n"
@@ -175,15 +175,15 @@
             logger.debug("Waiting for command response")
             start_time = datetime.now()
             while (datetime.now() - start_time).total_seconds() < _RESPONSE_TIMEOUT:
                 if len(self.str_buffer) > 0:
                     response = self.str_buffer.pop()
                     logger.debug("Command response received: %s", response)
                     return response.strip()
-                await asyncio.sleep(0)
+                await asyncio.sleep(0.01)
 
             logger.error("Timeout while waiting for command response")
             raise ResponseTimeoutError("Timeout while waiting for command response")
         finally:
             self._tx_busy = False
 
         return None
@@ -253,15 +253,15 @@
 
                         for rf_receive_callback in self.rf_receive_callbacks:
                             self.protocol.add_rf_receive_callback(rf_receive_callback)
 
                         return True
 
                     logger.debug("Waiting for Homeduino to become ready")
-                    await asyncio.sleep(0.1)
+                    await asyncio.sleep(0.01)
 
                 logger.error("Timeout while waiting for Homeduino to become ready")
                 raise ResponseTimeoutError(
                     "Timeout while waiting for Homeduino to become ready"
                 )
             except SerialException as ex:
                 logger.error(ex)
@@ -282,15 +282,15 @@
             start_time = datetime.now()
             while (datetime.now() - start_time).total_seconds() < _READY_TIMEOUT:
                 if not self.protocol.ready:
                     self.protocol = None
                     return True
 
                 logger.debug("Waiting for Homeduino to disconnect")
-                await asyncio.sleep(0.1)
+                await asyncio.sleep(0.01)
 
         return False
 
     async def ping(self) -> bool:
         if not self.connected():
             raise DisconnectedError("Homeduino is not connected")
```

### Comparing `homeduino-0.0.7/homeduino.egg-info/PKG-INFO` & `homeduino-0.0.7.1/homeduino.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homeduino
-Version: 0.0.7
+Version: 0.0.7.1
 Summary: Homeduino library
 Author: Rogier van Staveren
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/rrooggiieerr/homeduino.py
 Project-URL: Bug Tracker, https://github.com/rrooggiieerr/homeduino.py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
```

### Comparing `homeduino-0.0.7/pyproject.toml` & `homeduino-0.0.7.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "homeduino"
-version = "0.0.7"
+version = "0.0.7.1"
 license = {text = "Apache-2.0"}
 authors = [
     { name="Rogier van Staveren" }
 ]
 description = "Homeduino library"
 readme = "README.md"
 requires-python = ">=3.7"
@@ -16,15 +16,15 @@
     "Programming Language :: Python :: 3",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "pyserial-asyncio==0.6",
-    "rfcontrolpy>=0.0.3"
+    "rfcontrolpy==0.0.4"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/rrooggiieerr/homeduino.py"
 "Bug Tracker" = "https://github.com/rrooggiieerr/homeduino.py/issues"
 
 [tool.black]
```

