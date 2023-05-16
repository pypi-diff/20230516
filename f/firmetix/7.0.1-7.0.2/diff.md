# Comparing `tmp/firmetix-7.0.1.tar.gz` & `tmp/firmetix-7.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/firmetix/firmetix/dist/.tmp-7fn_i0bh/firmetix-7.0.1.tar", last modified: Tue Apr  4 19:24:10 2023, max compression
+gzip compressed data, was "/home/runner/work/firmetix/firmetix/dist/.tmp-8khmkhko/firmetix-7.0.2.tar", last modified: Tue May 16 16:24:00 2023, max compression
```

## Comparing `firmetix-7.0.1.tar` & `firmetix-7.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:24:10.000000 firmetix-7.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-04 19:24:00.000000 firmetix-7.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-04-04 19:24:10.000000 firmetix-7.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-04-04 19:24:00.000000 firmetix-7.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:24:10.000000 firmetix-7.0.1/firmetix/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 19:24:00.000000 firmetix-7.0.1/firmetix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   102797 2023-04-04 19:24:00.000000 firmetix-7.0.1/firmetix/firmetix.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-04-04 19:24:00.000000 firmetix-7.0.1/firmetix/private_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:24:10.000000 firmetix-7.0.1/firmetix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-04-04 19:24:10.000000 firmetix-7.0.1/firmetix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-04 19:24:10.000000 firmetix-7.0.1/firmetix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 19:24:10.000000 firmetix-7.0.1/firmetix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-04 19:24:10.000000 firmetix-7.0.1/firmetix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-04 19:24:10.000000 firmetix-7.0.1/firmetix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-04-04 19:24:00.000000 firmetix-7.0.1/pypi_desc.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 19:24:10.000000 firmetix-7.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-04 19:24:00.000000 firmetix-7.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:24:00.000000 firmetix-7.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-16 16:23:48.000000 firmetix-7.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-16 16:24:00.000000 firmetix-7.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-16 16:23:48.000000 firmetix-7.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:24:00.000000 firmetix-7.0.2/firmetix/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 16:23:48.000000 firmetix-7.0.2/firmetix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   103004 2023-05-16 16:23:48.000000 firmetix-7.0.2/firmetix/firmetix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-16 16:23:48.000000 firmetix-7.0.2/firmetix/private_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:24:00.000000 firmetix-7.0.2/firmetix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-16 16:24:00.000000 firmetix-7.0.2/firmetix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-16 16:24:00.000000 firmetix-7.0.2/firmetix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 16:24:00.000000 firmetix-7.0.2/firmetix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-16 16:24:00.000000 firmetix-7.0.2/firmetix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-16 16:24:00.000000 firmetix-7.0.2/firmetix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-16 16:23:48.000000 firmetix-7.0.2/pypi_desc.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 16:24:00.000000 firmetix-7.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-16 16:23:48.000000 firmetix-7.0.2/setup.py
```

### Comparing `firmetix-7.0.1/PKG-INFO` & `firmetix-7.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firmetix
-Version: 7.0.1
+Version: 7.0.2
 Summary: Remotely Control And Monitor Arduino and Esp devices
 Home-page: https://github.com/Nilon123456789/firmetix
 Download-URL: https://github.com/Nilon123456789/firmetix
 Author: Nils Lahaye
 Author-email: nils.lahaye@icloud.com
 Keywords: firmetix,Arduino,Protocol,Python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `firmetix-7.0.1/README.md` & `firmetix-7.0.2/README.md`

 * *Files identical despite different names*

### Comparing `firmetix-7.0.1/firmetix/firmetix.py` & `firmetix-7.0.2/firmetix/firmetix.py`

 * *Files 0% similar despite different names*

```diff
@@ -355,15 +355,18 @@
                 raise RuntimeError('No Arduino Found or User Aborted Program')
         elif self.connection_type == Connection_type.TCP_IP:
             self.sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
             self.sock.connect((self.ip_address, self.ip_port))
 
             print(f'Successfully connected to: {self.ip_address}:{self.ip_port}')
         elif self.connection_type == Connection_type.BLE:
-
+            
+            if self.ble_name is None: # if no name is given, use the default
+                self.ble_name = "Firmetix4ESP_BLE_" + str(arduino_instance_id)
+                
             adapters = simplepyble.Adapter.get_adapters()
 
             if len(adapters) == 0:
                 raise RuntimeError('No Bluetooth adapters found')
             
             print(f'Found {len(adapters)} Bluetooth adapters')
             self.adapter = adapters[0] # use the first adapter
@@ -2635,15 +2638,15 @@
                     self.ble_device.write_request(PrivateConstants.SERVICE_UUID, PrivateConstants.CHARACTERISTIC_UUID_TX, command)
                 else:
                     raise RuntimeError('No serial port or ip address or ble device set.')
 
                 if not action[1]:  # sleep only if not continuous
                     time.sleep(self.send_delay)
             else:
-                pass
+                time.sleep(self.sleep_tune)
 
     def _servo_unavailable(self, report):
         """
         Message if no servos are available for use.
         :param report: pin number
         """
         if self.shutdown_on_exception:
@@ -2893,8 +2896,8 @@
             return
     
     def _ble_receiver(self, data):
         """
         Called when data is received from the BLE device.
         """
         for d in data:
-            self.the_deque.append(d)
+            self.the_deque.append(d)
```

### Comparing `firmetix-7.0.1/firmetix/private_constants.py` & `firmetix-7.0.2/firmetix/private_constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
     STEPPER_RUNNING_REPORT = 18
     STEPPER_RUN_COMPLETE_REPORT = 19
     FEATURES = 20
     NOT_IMPLEMENTED = 21
     DEBUG_PRINT = 99
     MAX_PIN_REPORT = GET_MAX_PINS
 
-    FIRMETIX_VERSION = "7.0.0"
+    FIRMETIX_VERSION = "7.0.2"
     FIRMETIX4ARDUINO_MAJOR_VERSION = 7
 
     # reporting control
     REPORTING_DISABLE_ALL = 0
     REPORTING_ANALOG_ENABLE = 1
     REPORTING_DIGITAL_ENABLE = 2
     REPORTING_ANALOG_DISABLE = 3
```

### Comparing `firmetix-7.0.1/firmetix.egg-info/PKG-INFO` & `firmetix-7.0.2/firmetix.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firmetix
-Version: 7.0.1
+Version: 7.0.2
 Summary: Remotely Control And Monitor Arduino and Esp devices
 Home-page: https://github.com/Nilon123456789/firmetix
 Download-URL: https://github.com/Nilon123456789/firmetix
 Author: Nils Lahaye
 Author-email: nils.lahaye@icloud.com
 Keywords: firmetix,Arduino,Protocol,Python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `firmetix-7.0.1/pypi_desc.md` & `firmetix-7.0.2/pypi_desc.md`

 * *Files identical despite different names*

### Comparing `firmetix-7.0.1/setup.py` & `firmetix-7.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 setup(
     name='firmetix',
     packages=['firmetix'],
     install_requires=['pyserial', 'simplepyble'],
 
-    version='7.0.1',
+    version='7.0.2',
     description="Remotely Control And Monitor Arduino and Esp devices",
     long_description=long_description,
     long_description_content_type='text/markdown',
 
     author='Nils Lahaye',
     author_email='nils.lahaye@icloud.com',
     url='https://github.com/Nilon123456789/firmetix',
@@ -28,9 +28,8 @@
         'Intended Audience :: Education',
         'License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Topic :: Software Development :: Libraries :: Python Modules'
     ],
-)
-
+)
```

