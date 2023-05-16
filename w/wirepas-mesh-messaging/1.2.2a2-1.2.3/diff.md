# Comparing `tmp/wirepas_mesh_messaging-1.2.2a2.tar.gz` & `tmp/wirepas_mesh_messaging-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wirepas_mesh_messaging-1.2.2a2.tar", last modified: Thu Sep  8 10:10:20 2022, max compression
+gzip compressed data, was "wirepas_mesh_messaging-1.2.3.tar", last modified: Tue May 16 15:59:11 2023, max compression
```

## Comparing `wirepas_mesh_messaging-1.2.2a2.tar` & `wirepas_mesh_messaging-1.2.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 10:10:20.540949 wirepas_mesh_messaging-1.2.2a2/
--rw-r--r--   0 runner    (1001) docker     (121)    11341 2022-09-08 10:10:04.000000 wirepas_mesh_messaging-1.2.2a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3560 2022-09-08 10:10:20.540949 wirepas_mesh_messaging-1.2.2a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2339 2022-09-08 10:10:04.000000 wirepas_mesh_messaging-1.2.2a2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-08 10:10:20.540949 wirepas_mesh_messaging-1.2.2a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1950 2022-09-08 10:10:04.000000 wirepas_mesh_messaging-1.2.2a2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 10:10:20.540949 wirepas_mesh_messaging-1.2.2a2/wirepas_mesh_messaging/
--rw-r--r--   0 runner    (1001) docker     (121)     1312 2022-09-08 10:10:20.000000 wirepas_mesh_messaging-1.2.2a2/wirepas_mesh_messaging/__about__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1879 2022-09-08 10:10:04.000000 wirepas_mesh_messaging-1.2.2a2/wirepas_mesh_messaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      202 2022-09-08 10:10:04.000000 wirepas_mesh_messaging-1.2.2a2/wirepas_mesh_messaging/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9102 2022-09-08 10:10:04.000000 wirepas_mesh_messaging-1.2.2a2/wirepas_mesh_messaging/config_helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     2167 2022-09-08 10:10:04.000000 wirepas_mesh_messaging-1.2.2a2/wirepas_mesh_messaging/event.py
--rw-r--r--   0 runner    (1001) docker     (121)     1980 2022-09-08 10:10:04.000000 wirepas_mesh_messaging-1.2.2a2/wirepas_mesh_messaging/gateway_result_code.py
--rw-r--r--   0 runner    (1001) docker     (121)     3349 2022-09-08 10:10:04.000000 wirepas_mesh_messaging-1.2.2a2/wirepas_mesh_messaging/get_configs.py
--rw-r--r--   0 runner    (1001) docker     (121)     4030 2022-09-08 10:10:04.000000 wirepas_mesh_messaging-1.2.2a2/wirepas_mesh_messaging/get_gw_info.py
--rw-r--r--   0 runner    (1001) docker     (121)     6470 2022-09-08 10:10:04.000000 wirepas_mesh_messaging-1.2.2a2/wirepas_mesh_messaging/get_scratchpad_status.py
--rw-r--r--   0 runner    (1001) docker     (121)     3720 2022-09-08 10:10:04.000000 wirepas_mesh_messaging-1.2.2a2/wirepas_mesh_messaging/otap_helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     2934 2022-09-08 10:10:04.000000 wirepas_mesh_messaging-1.2.2a2/wirepas_mesh_messaging/process_scratchpad.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 10:10:20.540949 wirepas_mesh_messaging-1.2.2a2/wirepas_mesh_messaging/proto/
--rw-r--r--   0 runner    (1001) docker     (121)      284 2022-09-08 10:10:04.000000 wirepas_mesh_messaging-1.2.2a2/wirepas_mesh_messaging/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    44885 2022-09-08 10:10:07.000000 wirepas_mesh_messaging-1.2.2a2/wirepas_mesh_messaging/proto/config_message_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)    14575 2022-09-08 10:10:07.000000 wirepas_mesh_messaging-1.2.2a2/wirepas_mesh_messaging/proto/data_message_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)     9031 2022-09-08 10:10:07.000000 wirepas_mesh_messaging-1.2.2a2/wirepas_mesh_messaging/proto/error_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)    17512 2022-09-08 10:10:07.000000 wirepas_mesh_messaging-1.2.2a2/wirepas_mesh_messaging/proto/generic_message_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)    32350 2022-09-08 10:10:07.000000 wirepas_mesh_messaging-1.2.2a2/wirepas_mesh_messaging/proto/otap_message_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)    12837 2022-09-08 10:10:07.000000 wirepas_mesh_messaging-1.2.2a2/wirepas_mesh_messaging/proto/wp_global_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)     5029 2022-09-08 10:10:04.000000 wirepas_mesh_messaging-1.2.2a2/wirepas_mesh_messaging/received_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     2018 2022-09-08 10:10:04.000000 wirepas_mesh_messaging-1.2.2a2/wirepas_mesh_messaging/request.py
--rw-r--r--   0 runner    (1001) docker     (121)     2441 2022-09-08 10:10:04.000000 wirepas_mesh_messaging-1.2.2a2/wirepas_mesh_messaging/response.py
--rw-r--r--   0 runner    (1001) docker     (121)     5043 2022-09-08 10:10:04.000000 wirepas_mesh_messaging-1.2.2a2/wirepas_mesh_messaging/send_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     5103 2022-09-08 10:10:04.000000 wirepas_mesh_messaging-1.2.2a2/wirepas_mesh_messaging/set_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     5099 2022-09-08 10:10:04.000000 wirepas_mesh_messaging-1.2.2a2/wirepas_mesh_messaging/set_scratchpad_target.py
--rw-r--r--   0 runner    (1001) docker     (121)     2435 2022-09-08 10:10:04.000000 wirepas_mesh_messaging-1.2.2a2/wirepas_mesh_messaging/status.py
--rw-r--r--   0 runner    (1001) docker     (121)     3370 2022-09-08 10:10:04.000000 wirepas_mesh_messaging-1.2.2a2/wirepas_mesh_messaging/upload_scratchpad.py
--rw-r--r--   0 runner    (1001) docker     (121)      299 2022-09-08 10:10:04.000000 wirepas_mesh_messaging-1.2.2a2/wirepas_mesh_messaging/wirepas_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 10:10:20.540949 wirepas_mesh_messaging-1.2.2a2/wirepas_mesh_messaging.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3560 2022-09-08 10:10:20.000000 wirepas_mesh_messaging-1.2.2a2/wirepas_mesh_messaging.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1368 2022-09-08 10:10:20.000000 wirepas_mesh_messaging-1.2.2a2/wirepas_mesh_messaging.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-08 10:10:20.000000 wirepas_mesh_messaging-1.2.2a2/wirepas_mesh_messaging.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-09-08 10:10:20.000000 wirepas_mesh_messaging-1.2.2a2/wirepas_mesh_messaging.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-09-08 10:10:20.000000 wirepas_mesh_messaging-1.2.2a2/wirepas_mesh_messaging.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:59:11.510667 wirepas_mesh_messaging-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-05-16 15:58:52.000000 wirepas_mesh_messaging-1.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-05-16 15:59:11.510667 wirepas_mesh_messaging-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-05-16 15:58:52.000000 wirepas_mesh_messaging-1.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 15:59:11.510667 wirepas_mesh_messaging-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-05-16 15:58:52.000000 wirepas_mesh_messaging-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:59:11.506667 wirepas_mesh_messaging-1.2.3/wirepas_mesh_messaging/
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-16 15:59:11.000000 wirepas_mesh_messaging-1.2.3/wirepas_mesh_messaging/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-16 15:58:52.000000 wirepas_mesh_messaging-1.2.3/wirepas_mesh_messaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-16 15:58:52.000000 wirepas_mesh_messaging-1.2.3/wirepas_mesh_messaging/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10914 2023-05-16 15:58:52.000000 wirepas_mesh_messaging-1.2.3/wirepas_mesh_messaging/config_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-16 15:58:52.000000 wirepas_mesh_messaging-1.2.3/wirepas_mesh_messaging/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-05-16 15:58:52.000000 wirepas_mesh_messaging-1.2.3/wirepas_mesh_messaging/gateway_result_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-05-16 15:58:52.000000 wirepas_mesh_messaging-1.2.3/wirepas_mesh_messaging/get_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-05-16 15:58:52.000000 wirepas_mesh_messaging-1.2.3/wirepas_mesh_messaging/get_gw_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6480 2023-05-16 15:58:52.000000 wirepas_mesh_messaging-1.2.3/wirepas_mesh_messaging/get_scratchpad_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-05-16 15:58:52.000000 wirepas_mesh_messaging-1.2.3/wirepas_mesh_messaging/otap_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-05-16 15:58:52.000000 wirepas_mesh_messaging-1.2.3/wirepas_mesh_messaging/process_scratchpad.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:59:11.510667 wirepas_mesh_messaging-1.2.3/wirepas_mesh_messaging/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-16 15:58:52.000000 wirepas_mesh_messaging-1.2.3/wirepas_mesh_messaging/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-05-16 15:58:58.000000 wirepas_mesh_messaging-1.2.3/wirepas_mesh_messaging/proto/config_message_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-05-16 15:58:58.000000 wirepas_mesh_messaging-1.2.3/wirepas_mesh_messaging/proto/data_message_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-05-16 15:58:58.000000 wirepas_mesh_messaging-1.2.3/wirepas_mesh_messaging/proto/error_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-05-16 15:58:58.000000 wirepas_mesh_messaging-1.2.3/wirepas_mesh_messaging/proto/generic_message_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-05-16 15:58:58.000000 wirepas_mesh_messaging-1.2.3/wirepas_mesh_messaging/proto/otap_message_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-05-16 15:58:58.000000 wirepas_mesh_messaging-1.2.3/wirepas_mesh_messaging/proto/wp_global_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-05-16 15:58:52.000000 wirepas_mesh_messaging-1.2.3/wirepas_mesh_messaging/received_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-16 15:58:52.000000 wirepas_mesh_messaging-1.2.3/wirepas_mesh_messaging/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-05-16 15:58:52.000000 wirepas_mesh_messaging-1.2.3/wirepas_mesh_messaging/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-05-16 15:58:52.000000 wirepas_mesh_messaging-1.2.3/wirepas_mesh_messaging/send_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-05-16 15:58:52.000000 wirepas_mesh_messaging-1.2.3/wirepas_mesh_messaging/set_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-05-16 15:58:52.000000 wirepas_mesh_messaging-1.2.3/wirepas_mesh_messaging/set_scratchpad_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-05-16 15:58:52.000000 wirepas_mesh_messaging-1.2.3/wirepas_mesh_messaging/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-05-16 15:58:52.000000 wirepas_mesh_messaging-1.2.3/wirepas_mesh_messaging/upload_scratchpad.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-16 15:58:52.000000 wirepas_mesh_messaging-1.2.3/wirepas_mesh_messaging/wirepas_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:59:11.510667 wirepas_mesh_messaging-1.2.3/wirepas_mesh_messaging.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-05-16 15:59:11.000000 wirepas_mesh_messaging-1.2.3/wirepas_mesh_messaging.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-16 15:59:11.000000 wirepas_mesh_messaging-1.2.3/wirepas_mesh_messaging.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 15:59:11.000000 wirepas_mesh_messaging-1.2.3/wirepas_mesh_messaging.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 15:59:11.000000 wirepas_mesh_messaging-1.2.3/wirepas_mesh_messaging.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-16 15:59:11.000000 wirepas_mesh_messaging-1.2.3/wirepas_mesh_messaging.egg-info/top_level.txt
```

### Comparing `wirepas_mesh_messaging-1.2.2a2/LICENSE` & `wirepas_mesh_messaging-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wirepas_mesh_messaging-1.2.2a2/PKG-INFO` & `wirepas_mesh_messaging-1.2.3/wirepas_mesh_messaging.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: wirepas_mesh_messaging
-Version: 1.2.2a2
+Name: wirepas-mesh-messaging
+Version: 1.2.3
 Summary: Wrapper interfaces to interact with Backend to/from Gateway API.
 Home-page: https://github.com/wirepas/backend-apis/tree/master/gateway_to_backend
 Author: Wirepas Ltd
 Author-email: opensource@wirepas.com
 License: Apache-2
 Description: # Wirepas Mesh Messaging
```

### Comparing `wirepas_mesh_messaging-1.2.2a2/README.md` & `wirepas_mesh_messaging-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `wirepas_mesh_messaging-1.2.2a2/setup.py` & `wirepas_mesh_messaging-1.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `wirepas_mesh_messaging-1.2.2a2/wirepas_mesh_messaging/__about__.py` & `wirepas_mesh_messaging-1.2.3/wirepas_mesh_messaging/__about__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 __copyright__ = "2020 Wirepas Ltd"
 __description__ = "Wrapper interfaces to interact with Backend to/from Gateway API."
 __keywords__ = "wirepas connectivity iot mesh gateway backend"
 __license__ = "Apache-2"
 __pkg_name__ = "wirepas_mesh_messaging"
 __title__ = "Wirepas Messaging For Mesh access"
 __url__ = "https://github.com/wirepas/backend-apis/tree/master/gateway_to_backend"
-__version__ = "1.2.2a2"
+__version__ = "1.2.3"
 __warning_msg__ = """
 ***********************************************************************
 * WARNING:
 *     You are using the pure python protobuf implementation.
 *     For better results, please consider using the cpp version.
 *     For more information please consult:
 *     https://github.com/protocolbuffers/protobuf/tree/master/python
```

### Comparing `wirepas_mesh_messaging-1.2.2a2/wirepas_mesh_messaging/__init__.py` & `wirepas_mesh_messaging-1.2.3/wirepas_mesh_messaging/__init__.py`

 * *Files identical despite different names*

### Comparing `wirepas_mesh_messaging-1.2.2a2/wirepas_mesh_messaging/config_helper.py` & `wirepas_mesh_messaging-1.2.3/wirepas_mesh_messaging/config_helper.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,14 +5,21 @@
     .. Copyright:
         Copyright 2020 Wirepas Ltd under Apache License, Version 2.0.
         See file LICENSE for full license details.
 """
 
 from .proto import ON, OFF, NodeRole
 
+from .otap_helper import (
+    set_scratchpad_info,
+    parse_scratchpad_info,
+    ScratchpadStatus,
+    ScratchpadType, parse_scratchpad_target, set_scratchpad_target,
+)
+
 
 def convert_proto_role_to_wirepas(base, flags):
     """
     Maps the proto role enum to the correct Wirepas Mesh role
 
     Args:
         base (enum): protocol buffer enum
@@ -145,14 +152,37 @@
         message_obj.app_config, "app_config_data", dic, "app_config_data"
     )
     parse_optional_field(message_obj, "channel_map", dic, "channel_map")
 
     if message_obj.HasField("sink_state"):
         dic["started"] = message_obj.sink_state == ON
 
+def parse_config_otap(message_obj, dic):
+    if message_obj.HasField("stored_scratchpad"):
+        dic["stored_scratchpad"] = dict()
+        parse_scratchpad_info(message_obj.stored_scratchpad, dic["stored_scratchpad"])
+
+    if message_obj.HasField("processed_scratchpad"):
+        dic["processed_scratchpad"] = dict()
+        parse_scratchpad_info(message_obj.processed_scratchpad, dic["processed_scratchpad"])
+
+    if message_obj.HasField("stored_status"):
+        dic["stored_status"] = ScratchpadStatus(message_obj.stored_status)
+
+    if message_obj.HasField("stored_type"):
+        dic["stored_type"] = ScratchpadType(message_obj.stored_type)
+
+    if message_obj.HasField("firmware_area_id"):
+        dic["firmware_area_id"] = message_obj.firmware_area_id
+
+    if message_obj.HasField("target_and_action"):
+        dic["target_and_action"] = dict()
+        parse_scratchpad_target(message_obj.target_and_action, dic["target_and_action"])
+
+
 
 def set_config_rw(message_obj, dic):
     """
     Sets the message_obj with the read and write (rw) fields present in dic.
 
     Args:
         message_obj (proto): protocol buffer object
@@ -189,14 +219,33 @@
             message_obj.sink_state = ON
         else:
             message_obj.sink_state = OFF
     except KeyError:
         # Field is unknown, just skip it
         pass
 
+def set_config_otap(message_obj, dic):
+    if "stored_scratchpad" in dic:
+        set_scratchpad_info(message_obj.stored_scratchpad, dic["stored_scratchpad"])
+
+    if "processed_scratchpad" in dic:
+        set_scratchpad_info(message_obj.processed_scratchpad, dic["processed_scratchpad"])
+
+    if "stored_status" in dic:
+        message_obj.stored_status = dic["stored_status"].value
+
+    if "stored_type" in dic:
+        message_obj.stored_type = dic["stored_type"].value
+
+    if "firmware_area_id" in dic:
+        message_obj.firmware_area_id = dic["firmware_area_id"]
+
+    if "target_and_action" in dic:
+        set_scratchpad_target(message_obj.target_and_action, dic["target_and_action"])
+
 
 def parse_config_keys(message_obj, dic):
     """
     Parses network keys.
 
     The keys are only available on a SinkNewConfig message.
```

### Comparing `wirepas_mesh_messaging-1.2.2a2/wirepas_mesh_messaging/event.py` & `wirepas_mesh_messaging-1.2.3/wirepas_mesh_messaging/event.py`

 * *Files identical despite different names*

### Comparing `wirepas_mesh_messaging-1.2.2a2/wirepas_mesh_messaging/gateway_result_code.py` & `wirepas_mesh_messaging-1.2.3/wirepas_mesh_messaging/gateway_result_code.py`

 * *Files identical despite different names*

### Comparing `wirepas_mesh_messaging-1.2.2a2/wirepas_mesh_messaging/get_configs.py` & `wirepas_mesh_messaging-1.2.3/wirepas_mesh_messaging/get_configs.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,27 +11,28 @@
 
 from .request import Request
 from .response import Response
 
 from .config_helper import (
     parse_config_rw,
     parse_config_ro,
+    parse_config_otap,
     set_config_ro,
     set_config_rw,
+    set_config_otap,
 )
 from .wirepas_exceptions import GatewayAPIParsingException
 
 
 class GetConfigsRequest(Request):
     """
     GetConfigsRequest: Request to obtain the configs of all sinks from a gateway
 
     Attributes:
         req_id (int): unique request id
-        time_ms_epoch(int): timestamp in ms of request generation
     """
 
     def __init__(self, req_id=None, **kwargs):
         super(GetConfigsRequest, self).__init__(req_id=req_id, **kwargs)
 
     @classmethod
     def from_payload(cls, payload):
@@ -88,14 +89,15 @@
         for conf in response.configs:
             config = {}
 
             config["sink_id"] = conf.sink_id
 
             parse_config_rw(conf, config)
             parse_config_ro(conf, config)
+            parse_config_otap(conf, config)
 
             configs.append(config)
 
         return cls(d["req_id"], d["gw_id"], d["res"], configs, time_ms_epoch=d["time_ms_epoch"])
 
     @property
     def payload(self):
@@ -106,9 +108,10 @@
 
         for config in self.configs:
             conf = response.configs.add()
             conf.sink_id = config["sink_id"]
 
             set_config_rw(conf, config)
             set_config_ro(conf, config)
+            set_config_otap(conf, config)
 
         return message.SerializeToString()
```

### Comparing `wirepas_mesh_messaging-1.2.2a2/wirepas_mesh_messaging/get_gw_info.py` & `wirepas_mesh_messaging-1.2.3/wirepas_mesh_messaging/get_gw_info.py`

 * *Files identical despite different names*

### Comparing `wirepas_mesh_messaging-1.2.2a2/wirepas_mesh_messaging/get_scratchpad_status.py` & `wirepas_mesh_messaging-1.2.3/wirepas_mesh_messaging/get_scratchpad_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         stored_status=None,
         stored_type=None,
         processed_scratchpad=None,
         firmware_area_id=None,
         target_scratchpad_and_action=None,
         **kwargs
     ):
-        super(GetScratchpadStatusResponse, self).__init__(req_id, gw_id, res, sink_id)
+        super(GetScratchpadStatusResponse, self).__init__(req_id, gw_id, res, sink_id, **kwargs)
         self.stored_scratchpad = stored_scratchpad
         self.stored_status = stored_status
         self.stored_type = stored_type
         self.processed_scratchpad = processed_scratchpad
         self.firmware_area_id = firmware_area_id
         self.target_scratchpad_and_action = target_scratchpad_and_action
```

### Comparing `wirepas_mesh_messaging-1.2.2a2/wirepas_mesh_messaging/otap_helper.py` & `wirepas_mesh_messaging-1.2.3/wirepas_mesh_messaging/otap_helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 
     .. Copyright:
         Copyright 2019 Wirepas Ltd under Apache License, Version 2.0.
         See file LICENSE for full license details.
 """
 
 # flake8: noqa
-from .proto.otap_message_pb2 import BLANK, PRESENT, PROCESS, SUCCESS, NEW, ERROR
-from .proto.otap_message_pb2 import NO_OTAP, PROPAGATE_ONLY, PROPAGATE_AND_PROCESS, PROPAGATE_AND_PROCESS_WITH_DELAY, LEGACY_OTAP
-from .proto.otap_message_pb2 import UNKNOWN_DELAY, TEN_MINUTES, THIRTY_MINUTES, ONE_HOUR, SIX_HOURS, ONE_DAY, TWO_DAYS, FIVE_DAYS
+from .proto.wp_global_pb2 import BLANK, PRESENT, PROCESS, SUCCESS, NEW, ERROR
+from .proto.wp_global_pb2 import NO_OTAP, PROPAGATE_ONLY, PROPAGATE_AND_PROCESS, PROPAGATE_AND_PROCESS_WITH_DELAY, LEGACY_OTAP
+from .proto.wp_global_pb2 import UNKNOWN_DELAY, TEN_MINUTES, THIRTY_MINUTES, ONE_HOUR, SIX_HOURS, ONE_DAY, TWO_DAYS, FIVE_DAYS
 
 import enum
 
 
 def parse_optional_field(message_obj, field, dic, key):
     """
     Copies attribute into dic if it exists in the proto message
```

### Comparing `wirepas_mesh_messaging-1.2.2a2/wirepas_mesh_messaging/process_scratchpad.py` & `wirepas_mesh_messaging-1.2.3/wirepas_mesh_messaging/process_scratchpad.py`

 * *Files identical despite different names*

### Comparing `wirepas_mesh_messaging-1.2.2a2/wirepas_mesh_messaging/received_data.py` & `wirepas_mesh_messaging-1.2.3/wirepas_mesh_messaging/received_data.py`

 * *Files identical despite different names*

### Comparing `wirepas_mesh_messaging-1.2.2a2/wirepas_mesh_messaging/request.py` & `wirepas_mesh_messaging-1.2.3/wirepas_mesh_messaging/request.py`

 * *Files identical despite different names*

### Comparing `wirepas_mesh_messaging-1.2.2a2/wirepas_mesh_messaging/response.py` & `wirepas_mesh_messaging-1.2.3/wirepas_mesh_messaging/response.py`

 * *Files identical despite different names*

### Comparing `wirepas_mesh_messaging-1.2.2a2/wirepas_mesh_messaging/send_data.py` & `wirepas_mesh_messaging-1.2.3/wirepas_mesh_messaging/send_data.py`

 * *Files identical despite different names*

### Comparing `wirepas_mesh_messaging-1.2.2a2/wirepas_mesh_messaging/set_config.py` & `wirepas_mesh_messaging-1.2.3/wirepas_mesh_messaging/set_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,20 +42,19 @@
                     cipher_key (bytearray)
                     authentication_key (bytearray)
                     started (bool)
 
                 Note: app_config_data/app_config_seq/app_config_data must all be defined to change one of them
                       only relevant keys for new config has to be defined
         req_id (int): unique request id
-        time_ms_epoch(int): timestamp in ms of request generation
 
     """
 
-    def __init__(self, sink_id, new_config, req_id=None, time_ms_epoch=None, **kwargs):
-        super(SetConfigRequest, self).__init__(req_id=req_id, time_ms_epoch=time_ms_epoch, **kwargs)
+    def __init__(self, sink_id, new_config, req_id=None, **kwargs):
+        super(SetConfigRequest, self).__init__(req_id=req_id, **kwargs)
         self.sink_id = sink_id
         self.new_config = new_config
 
     @classmethod
     def from_payload(cls, payload):
         message = GenericMessage()
         try:
```

### Comparing `wirepas_mesh_messaging-1.2.2a2/wirepas_mesh_messaging/set_scratchpad_target.py` & `wirepas_mesh_messaging-1.2.3/wirepas_mesh_messaging/set_scratchpad_target.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,24 +31,22 @@
             Dict keys are:
                 action (ScratchpadAction): target action for network
                 target_sequence (int): target sequence
                 target_crc (int): target crc
                 param(int): raw parameter for action
                 delay(ProcessingDelay): delay for WITH_DELAY action
         req_id (int): unique request id
-        time_ms_epoch(int): timestamp in ms of request generation
     """
 
     def __init__(self,
                  sink_id,
                  target,
                  req_id=None,
-                 time_ms_epoch=None,
                  **kwargs):
-        super(SetScratchpadTargetAndActionRequest, self).__init__(sink_id, req_id, time_ms_epoch=time_ms_epoch, **kwargs)
+        super(SetScratchpadTargetAndActionRequest, self).__init__(sink_id, req_id, **kwargs)
 
         if target["action"].value > 255:
             raise ValueError("Wrong Target action")
 
         try:
             seq = target["target_sequence"]
             if seq is not None and seq > 255:
```

### Comparing `wirepas_mesh_messaging-1.2.2a2/wirepas_mesh_messaging/upload_scratchpad.py` & `wirepas_mesh_messaging-1.2.3/wirepas_mesh_messaging/upload_scratchpad.py`

 * *Files identical despite different names*

### Comparing `wirepas_mesh_messaging-1.2.2a2/wirepas_mesh_messaging.egg-info/PKG-INFO` & `wirepas_mesh_messaging-1.2.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: wirepas-mesh-messaging
-Version: 1.2.2a2
+Name: wirepas_mesh_messaging
+Version: 1.2.3
 Summary: Wrapper interfaces to interact with Backend to/from Gateway API.
 Home-page: https://github.com/wirepas/backend-apis/tree/master/gateway_to_backend
 Author: Wirepas Ltd
 Author-email: opensource@wirepas.com
 License: Apache-2
 Description: # Wirepas Mesh Messaging
```

### Comparing `wirepas_mesh_messaging-1.2.2a2/wirepas_mesh_messaging.egg-info/SOURCES.txt` & `wirepas_mesh_messaging-1.2.3/wirepas_mesh_messaging.egg-info/SOURCES.txt`

 * *Files identical despite different names*

