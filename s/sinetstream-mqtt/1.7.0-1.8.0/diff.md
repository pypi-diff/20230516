# Comparing `tmp/sinetstream-mqtt-1.7.0.tar.gz` & `tmp/sinetstream-mqtt-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sinetstream-mqtt-1.7.0.tar", last modified: Fri Sep 16 07:09:26 2022, max compression
+gzip compressed data, was "sinetstream-mqtt-1.8.0.tar", last modified: Tue May 16 06:40:05 2023, max compression
```

## Comparing `sinetstream-mqtt-1.7.0.tar` & `sinetstream-mqtt-1.8.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2022-09-16 07:09:26.477435 sinetstream-mqtt-1.7.0/
--rw-rw-r--   0 koie      (1004) koie      (1004)      584 2022-09-16 07:09:26.477435 sinetstream-mqtt-1.7.0/PKG-INFO
--rw-rw-r--   0 koie      (1004) koie      (1004)     1651 2022-09-16 07:09:26.477435 sinetstream-mqtt-1.7.0/setup.cfg
--rw-rw-r--   0 koie      (1004) koie      (1004)       39 2022-09-15 07:30:59.000000 sinetstream-mqtt-1.7.0/setup.py
-drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2022-09-16 07:09:26.477435 sinetstream-mqtt-1.7.0/src/
-drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2022-09-16 07:09:26.477435 sinetstream-mqtt-1.7.0/src/sinetstream_mqtt.egg-info/
--rw-rw-r--   0 koie      (1004) koie      (1004)      584 2022-09-16 07:09:26.000000 sinetstream-mqtt-1.7.0/src/sinetstream_mqtt.egg-info/PKG-INFO
--rw-rw-r--   0 koie      (1004) koie      (1004)      410 2022-09-16 07:09:26.000000 sinetstream-mqtt-1.7.0/src/sinetstream_mqtt.egg-info/SOURCES.txt
--rw-rw-r--   0 koie      (1004) koie      (1004)        1 2022-09-16 07:09:26.000000 sinetstream-mqtt-1.7.0/src/sinetstream_mqtt.egg-info/dependency_links.txt
--rw-rw-r--   0 koie      (1004) koie      (1004)      274 2022-09-16 07:09:26.000000 sinetstream-mqtt-1.7.0/src/sinetstream_mqtt.egg-info/entry_points.txt
--rw-rw-r--   0 koie      (1004) koie      (1004)       18 2022-09-16 07:09:26.000000 sinetstream-mqtt-1.7.0/src/sinetstream_mqtt.egg-info/namespace_packages.txt
--rw-rw-r--   0 koie      (1004) koie      (1004)        1 2022-09-16 07:07:28.000000 sinetstream-mqtt-1.7.0/src/sinetstream_mqtt.egg-info/not-zip-safe
--rw-rw-r--   0 koie      (1004) koie      (1004)       42 2022-09-16 07:09:26.000000 sinetstream-mqtt-1.7.0/src/sinetstream_mqtt.egg-info/requires.txt
--rw-rw-r--   0 koie      (1004) koie      (1004)       18 2022-09-16 07:09:26.000000 sinetstream-mqtt-1.7.0/src/sinetstream_mqtt.egg-info/top_level.txt
-drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2022-09-16 07:09:26.477435 sinetstream-mqtt-1.7.0/src/sinetstreamplugin/
--rw-rw-r--   0 koie      (1004) koie      (1004)    12425 2022-09-15 07:30:59.000000 sinetstream-mqtt-1.7.0/src/sinetstreamplugin/mqtt.py
+drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-05-16 06:40:05.722483 sinetstream-mqtt-1.8.0/
+-rw-rw-r--   0 koie      (1004) koie      (1004)      545 2023-05-16 06:40:05.722483 sinetstream-mqtt-1.8.0/PKG-INFO
+-rw-rw-r--   0 koie      (1004) koie      (1004)     1658 2023-05-16 06:40:05.726483 sinetstream-mqtt-1.8.0/setup.cfg
+-rw-rw-r--   0 koie      (1004) koie      (1004)       39 2023-01-12 00:12:25.000000 sinetstream-mqtt-1.8.0/setup.py
+drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-05-16 06:40:05.714484 sinetstream-mqtt-1.8.0/src/
+drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-05-16 06:40:05.722483 sinetstream-mqtt-1.8.0/src/sinetstream_mqtt.egg-info/
+-rw-rw-r--   0 koie      (1004) koie      (1004)      545 2023-05-16 06:40:05.000000 sinetstream-mqtt-1.8.0/src/sinetstream_mqtt.egg-info/PKG-INFO
+-rw-rw-r--   0 koie      (1004) koie      (1004)      410 2023-05-16 06:40:05.000000 sinetstream-mqtt-1.8.0/src/sinetstream_mqtt.egg-info/SOURCES.txt
+-rw-rw-r--   0 koie      (1004) koie      (1004)        1 2023-05-16 06:40:05.000000 sinetstream-mqtt-1.8.0/src/sinetstream_mqtt.egg-info/dependency_links.txt
+-rw-rw-r--   0 koie      (1004) koie      (1004)      273 2023-05-16 06:40:05.000000 sinetstream-mqtt-1.8.0/src/sinetstream_mqtt.egg-info/entry_points.txt
+-rw-rw-r--   0 koie      (1004) koie      (1004)       18 2023-05-16 06:40:05.000000 sinetstream-mqtt-1.8.0/src/sinetstream_mqtt.egg-info/namespace_packages.txt
+-rw-rw-r--   0 koie      (1004) koie      (1004)        1 2023-01-12 00:15:57.000000 sinetstream-mqtt-1.8.0/src/sinetstream_mqtt.egg-info/not-zip-safe
+-rw-rw-r--   0 koie      (1004) koie      (1004)       42 2023-05-16 06:40:05.000000 sinetstream-mqtt-1.8.0/src/sinetstream_mqtt.egg-info/requires.txt
+-rw-rw-r--   0 koie      (1004) koie      (1004)       18 2023-05-16 06:40:05.000000 sinetstream-mqtt-1.8.0/src/sinetstream_mqtt.egg-info/top_level.txt
+drwxrwxr-x   0 koie      (1004) koie      (1004)        0 2023-05-16 06:40:05.722483 sinetstream-mqtt-1.8.0/src/sinetstreamplugin/
+-rw-rw-r--   0 koie      (1004) koie      (1004)    14595 2023-05-16 06:28:56.000000 sinetstream-mqtt-1.8.0/src/sinetstreamplugin/mqtt.py
```

### Comparing `sinetstream-mqtt-1.7.0/PKG-INFO` & `sinetstream-mqtt-1.8.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: sinetstream-mqtt
-Version: 1.7.0
+Version: 1.8.0
 Summary: MQTT plugin for SINETStream library
 Home-page: https://github.com/nii-gakunin-cloud/sinetstream
 License: Apache License, Version 2.0
-Description: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Japanese
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
```

### Comparing `sinetstream-mqtt-1.7.0/setup.cfg` & `sinetstream-mqtt-1.8.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sinetstream-mqtt
-version = 1.7.0
+version = 1.8.0
 description = MQTT plugin for SINETStream library
 license = Apache License, Version 2.0
 license_files = 
 	../../../../LICENSE
 url = https://github.com/nii-gakunin-cloud/sinetstream
 classifiers = 
 	Development Status :: 4 - Beta
@@ -16,23 +16,23 @@
 
 [options]
 package_dir = 
 	=src
 packages = find_namespace:
 zip_safe = False
 install_requires = 
-	sinetstream>=1.7.0
+	sinetstream>=1.8.0
 	paho-mqtt>=1.5
 	promise
 tests_require = 
 	pytest
 	pytest-cov
 	pytest-flake8
 	pytest-timeout
-	pytest-html
+	pytest-html==3.2.0
 	flake8>=4.0.0,<5.0.0  # workaround: https://github.com/tholo/pytest-flake8/issues/87
 setup_requires = 
 	pytest-runner
 namespace_packages = 
 	sinetstreamplugin
 python_requires = >= 3.7
```

### Comparing `sinetstream-mqtt-1.7.0/src/sinetstream_mqtt.egg-info/PKG-INFO` & `sinetstream-mqtt-1.8.0/src/sinetstream_mqtt.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: sinetstream-mqtt
-Version: 1.7.0
+Version: 1.8.0
 Summary: MQTT plugin for SINETStream library
 Home-page: https://github.com/nii-gakunin-cloud/sinetstream
 License: Apache License, Version 2.0
-Description: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Japanese
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
```

### Comparing `sinetstream-mqtt-1.7.0/src/sinetstreamplugin/mqtt.py` & `sinetstream-mqtt-1.8.0/src/sinetstreamplugin/mqtt.py`

 * *Files 15% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 from sys import exc_info
 from threading import Condition, Lock
 
 from paho.mqtt.client import (
     Client, MQTT_ERR_QUEUE_SIZE, MQTT_ERR_NO_CONN,
     connack_string, MQTTv31, MQTTv311, MQTTv5, WebsocketConnectionError,
     MQTT_ERR_SUCCESS)
+from paho.mqtt.properties import (Properties, MQTTException)
+from paho.mqtt.packettypes import PacketTypes
 from promise import Promise
 
 from sinetstream import (
     AT_MOST_ONCE, AT_LEAST_ONCE, EXACTLY_ONCE,
     InvalidArgumentError, ConnectionError,
     SinetError)
 
@@ -140,17 +142,18 @@
         raise InvalidArgumentError(f'transport: invalid value: {transport}')
     return transport
 
 
 def _create_mqtt_client(params):
     mqttc = Client(
         client_id=params.get("client_id", ''),
-        clean_session=params.get('clean_session'),
+        clean_session=params.get('clean_session'),  # NOTE: MUST be None in MQTTv5, USE clean_start
         protocol=_to_protocol(params.get('protocol')),
         transport=_get_transport(params),
+        # reconnect_on_failure=params.get("reconnect_on_failure", True),
     )
 
     for name in _MQTT_NESTED_PARAMETER:
         if name not in params:
             continue
         logger.debug(f'invoke: {name}({params[name]})')
         getattr(mqttc, name)(**params[name])
@@ -193,41 +196,90 @@
                      isinstance(value, str) and hasattr(ssl, value))
              else getattr(ssl, value))
         )
         for key, value in params['tls_set'].items()
     ])
 
 
+def _replace_will_params(params):
+    if 'will_set' not in params:
+        return
+    will_params = params['will_set']
+    if 'delay_interval' in will_params:
+        props = Properties(PacketTypes.WILLMESSAGE)
+        props.WillDelayInterval = will_params.pop('delay_interval')
+        will_params['properties'] = props
+
+
 class MqttClient(object):
     def __init__(self, params):
         self._params = _translate_tls_params(params)
         self._params.update(params)
         _replace_ssl_params(self._params)
+        _replace_will_params(self._params)
         logger.debug(self._params)
 
         try:
             self._mqttc = _create_mqtt_client(self._params)
         except ValueError as ex:
             raise InvalidArgumentError(ex)
 
         self._mqttc.on_connect = self._on_connect
         self.qos = _to_qos(self._params)
         self.connection_timeout = self._params.get('connection_timeout', 10)
         self.keepalive = self._params.get('keepalive', 60)
         self.host, self.port = _get_broker(self._params)
         logger.debug(f'broker={self.host} port={self.port}')
-        self.protocol = _to_protocol(self._params.get('protocol')),
+        self.protocol = _to_protocol(self._params.get('protocol'))
         self._connection_result = None
         self._conn_cond = Condition()
 
+    def _make_properties(self):
+        def name2(s):
+            name = s.replace(" ", "")
+            name_ = (s.replace("Information", "Info")
+                      .replace("Authentication", "Auth")
+                      .replace(" ", "_")
+                      .lower())
+            return (name, name_)
+        properties = Properties(PacketTypes.CONNECT)
+        n = 0
+        for (name, name_) in [name2(k) for k in properties.names.keys()]:
+            # print(f"name={name} name_={name_}")
+            # ptype = PacketTypes.CONNECT
+            # if ptype not in properties.properties[properties.getIdentFromName(name)][1]:
+            #     continue
+            if name_ in self._params:
+                n += 1
+                val = self._params[name_]
+                if name_ == "user_property":
+                    val = [(k, v) for k, v in val.items()]
+                try:
+                    properties.__setattr__(name, val)
+                except MQTTException as ex:
+                    # ok, maybe packet type mismatch.
+                    logger.warning(f"{name_}: {ex}")
+        logger.debug(f"properties={properties}")
+        return properties if n > 0 else None
+
     def open(self, timeout=None):
         logger.debug("open")
         try:
-            self._mqttc.connect(self.host, self.port, self.keepalive)
-        except (socket.error, OSError, WebsocketConnectionError):
+            kwargs = {
+                "host": self.host,
+                "port": self.port,
+                "keepalive": self.keepalive,
+            }
+            if "clean_start" in self._params:
+                kwargs["clean_start"] = self._params["clean_start"]
+            properties = self._make_properties()
+            if properties is not None:
+                kwargs["properties"] = properties
+            self._mqttc.connect(**kwargs)
+        except (socket.error, OSError, WebsocketConnectionError, ValueError):
             logger.error(f"cannot connect broker: {self.host}:{self.port}")
             self.close()
             raise ConnectionError(
                 f"cannot connect broker: {self.host}:{self.port}")
 
         self._mqttc.loop_start()
```

