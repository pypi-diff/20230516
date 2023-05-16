# Comparing `tmp/async_adbc-1.0.1.tar.gz` & `tmp/async_adbc-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_adbc-1.0.1.tar", max compression
+gzip compressed data, was "async_adbc-1.0.2.tar", max compression
```

## Comparing `async_adbc-1.0.1.tar` & `async_adbc-1.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0       70 2023-05-16 06:58:01.167502 async_adbc-1.0.1/async_adbc/__init__.py
--rw-r--r--   0        0        0      998 2023-05-16 06:58:27.465793 async_adbc-1.0.1/async_adbc/adbclient.py
--rw-r--r--   0        0        0     2983 2023-05-16 06:52:10.041298 async_adbc-1.0.1/async_adbc/device.py
--rw-r--r--   0        0        0      601 2023-05-16 06:51:45.869292 async_adbc-1.0.1/async_adbc/plugins/__init__.py
--rw-r--r--   0        0        0      502 2023-05-16 02:17:28.058635 async_adbc-1.0.1/async_adbc/plugins/am.py
--rw-r--r--   0        0        0     2657 2023-05-16 02:32:10.948830 async_adbc-1.0.1/async_adbc/plugins/battery.py
--rw-r--r--   0        0        0    12259 2023-05-16 06:51:45.908294 async_adbc-1.0.1/async_adbc/plugins/cpu.py
--rw-r--r--   0        0        0     1242 2023-05-16 06:51:45.797292 async_adbc-1.0.1/async_adbc/plugins/forward.py
--rw-r--r--   0        0        0     3933 2023-05-16 02:51:02.455214 async_adbc-1.0.1/async_adbc/plugins/fps.py
--rw-r--r--   0        0        0      614 2023-05-15 12:07:09.349059 async_adbc-1.0.1/async_adbc/plugins/gpu.py
--rw-r--r--   0        0        0      393 2023-05-15 12:13:38.890420 async_adbc-1.0.1/async_adbc/plugins/input.py
--rw-r--r--   0        0        0      895 2023-05-16 03:18:01.857216 async_adbc-1.0.1/async_adbc/plugins/logcat.py
--rw-r--r--   0        0        0     2209 2023-05-16 03:26:42.422860 async_adbc-1.0.1/async_adbc/plugins/mem.py
--rw-r--r--   0        0        0     5597 2023-05-16 06:51:45.819291 async_adbc-1.0.1/async_adbc/plugins/pm.py
--rw-r--r--   0        0        0      510 2023-05-15 11:29:29.910308 async_adbc-1.0.1/async_adbc/plugins/prop.py
--rw-r--r--   0        0        0     4615 2023-05-16 04:20:29.957697 async_adbc-1.0.1/async_adbc/plugins/temp.py
--rw-r--r--   0        0        0     2216 2023-05-16 06:51:45.868298 async_adbc-1.0.1/async_adbc/plugins/traffic.py
--rw-r--r--   0        0        0      807 2023-05-15 11:29:32.496380 async_adbc-1.0.1/async_adbc/plugins/utils.py
--rw-r--r--   0        0        0     4509 2023-05-15 08:29:42.104875 async_adbc-1.0.1/async_adbc/protocol.py
--rw-r--r--   0        0        0      796 2023-05-16 06:51:45.874292 async_adbc-1.0.1/async_adbc/service/__init__.py
--rw-r--r--   0        0        0    10228 2023-05-16 06:51:45.939291 async_adbc-1.0.1/async_adbc/service/host.py
--rw-r--r--   0        0        0    10086 2023-05-16 06:51:45.937291 async_adbc-1.0.1/async_adbc/service/local.py
--rw-r--r--   0        0        0     1090 2023-05-16 05:23:42.403245 async_adbc-1.0.1/LICENSE
--rw-r--r--   0        0        0      482 2023-05-16 06:58:10.840881 async_adbc-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      423 2023-05-15 02:24:29.723099 async_adbc-1.0.1/README.md
--rw-r--r--   0        0        0      849 1970-01-01 00:00:00.000000 async_adbc-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0       70 2023-05-16 06:58:01.167502 async_adbc-1.0.2/async_adbc/__init__.py
+-rw-r--r--   0        0        0      998 2023-05-16 06:58:27.465793 async_adbc-1.0.2/async_adbc/adbclient.py
+-rw-r--r--   0        0        0     2983 2023-05-16 06:52:10.041298 async_adbc-1.0.2/async_adbc/device.py
+-rw-r--r--   0        0        0      601 2023-05-16 06:51:45.869292 async_adbc-1.0.2/async_adbc/plugins/__init__.py
+-rw-r--r--   0        0        0      502 2023-05-16 02:17:28.058635 async_adbc-1.0.2/async_adbc/plugins/am.py
+-rw-r--r--   0        0        0     2657 2023-05-16 02:32:10.948830 async_adbc-1.0.2/async_adbc/plugins/battery.py
+-rw-r--r--   0        0        0    12259 2023-05-16 06:51:45.908294 async_adbc-1.0.2/async_adbc/plugins/cpu.py
+-rw-r--r--   0        0        0     1242 2023-05-16 06:51:45.797292 async_adbc-1.0.2/async_adbc/plugins/forward.py
+-rw-r--r--   0        0        0     3933 2023-05-16 02:51:02.455214 async_adbc-1.0.2/async_adbc/plugins/fps.py
+-rw-r--r--   0        0        0      614 2023-05-15 12:07:09.349059 async_adbc-1.0.2/async_adbc/plugins/gpu.py
+-rw-r--r--   0        0        0      393 2023-05-15 12:13:38.890420 async_adbc-1.0.2/async_adbc/plugins/input.py
+-rw-r--r--   0        0        0      895 2023-05-16 03:18:01.857216 async_adbc-1.0.2/async_adbc/plugins/logcat.py
+-rw-r--r--   0        0        0     2209 2023-05-16 03:26:42.422860 async_adbc-1.0.2/async_adbc/plugins/mem.py
+-rw-r--r--   0        0        0     5597 2023-05-16 06:51:45.819291 async_adbc-1.0.2/async_adbc/plugins/pm.py
+-rw-r--r--   0        0        0      510 2023-05-15 11:29:29.910308 async_adbc-1.0.2/async_adbc/plugins/prop.py
+-rw-r--r--   0        0        0     4615 2023-05-16 04:20:29.957697 async_adbc-1.0.2/async_adbc/plugins/temp.py
+-rw-r--r--   0        0        0     2216 2023-05-16 06:51:45.868298 async_adbc-1.0.2/async_adbc/plugins/traffic.py
+-rw-r--r--   0        0        0      807 2023-05-15 11:29:32.496380 async_adbc-1.0.2/async_adbc/plugins/utils.py
+-rw-r--r--   0        0        0     4481 2023-05-16 07:19:17.701385 async_adbc-1.0.2/async_adbc/protocol.py
+-rw-r--r--   0        0        0      796 2023-05-16 06:51:45.874292 async_adbc-1.0.2/async_adbc/service/__init__.py
+-rw-r--r--   0        0        0    10228 2023-05-16 06:51:45.939291 async_adbc-1.0.2/async_adbc/service/host.py
+-rw-r--r--   0        0        0    10086 2023-05-16 06:51:45.937291 async_adbc-1.0.2/async_adbc/service/local.py
+-rw-r--r--   0        0        0     1090 2023-05-16 05:23:42.403245 async_adbc-1.0.2/LICENSE
+-rw-r--r--   0        0        0      482 2023-05-16 07:19:30.857945 async_adbc-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      423 2023-05-15 02:24:29.723099 async_adbc-1.0.2/README.md
+-rw-r--r--   0        0        0      849 1970-01-01 00:00:00.000000 async_adbc-1.0.2/PKG-INFO
```

### Comparing `async_adbc-1.0.1/async_adbc/adbclient.py` & `async_adbc-1.0.2/async_adbc/adbclient.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.1/async_adbc/device.py` & `async_adbc-1.0.2/async_adbc/device.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.1/async_adbc/plugins/__init__.py` & `async_adbc-1.0.2/async_adbc/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.1/async_adbc/plugins/battery.py` & `async_adbc-1.0.2/async_adbc/plugins/battery.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.1/async_adbc/plugins/cpu.py` & `async_adbc-1.0.2/async_adbc/plugins/cpu.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.1/async_adbc/plugins/forward.py` & `async_adbc-1.0.2/async_adbc/plugins/forward.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.1/async_adbc/plugins/fps.py` & `async_adbc-1.0.2/async_adbc/plugins/fps.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.1/async_adbc/plugins/gpu.py` & `async_adbc-1.0.2/async_adbc/plugins/gpu.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.1/async_adbc/plugins/logcat.py` & `async_adbc-1.0.2/async_adbc/plugins/logcat.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.1/async_adbc/plugins/mem.py` & `async_adbc-1.0.2/async_adbc/plugins/mem.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.1/async_adbc/plugins/pm.py` & `async_adbc-1.0.2/async_adbc/plugins/pm.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.1/async_adbc/plugins/temp.py` & `async_adbc-1.0.2/async_adbc/plugins/temp.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.1/async_adbc/plugins/traffic.py` & `async_adbc-1.0.2/async_adbc/plugins/traffic.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.1/async_adbc/plugins/utils.py` & `async_adbc-1.0.2/async_adbc/plugins/utils.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.1/async_adbc/protocol.py` & `async_adbc-1.0.2/async_adbc/protocol.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,14 @@
             msg (str): _description_
 
         Returns:
             _type_: _description_
         """
 
         msg = ":".join([str(arg) for arg in args])
-        print("req:", msg)
         data = pack(msg)
         self.writer.write(data)
         await self.writer.drain()
         await self._check_status()
         return Response(self.reader)
 
     async def message(self, MSG: str, length: int | None = None, data: bytes = b""):
```

### Comparing `async_adbc-1.0.1/async_adbc/service/__init__.py` & `async_adbc-1.0.2/async_adbc/service/__init__.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.1/async_adbc/service/host.py` & `async_adbc-1.0.2/async_adbc/service/host.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.1/async_adbc/service/local.py` & `async_adbc-1.0.2/async_adbc/service/local.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.1/LICENSE` & `async_adbc-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.1/PKG-INFO` & `async_adbc-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-adbc
-Version: 1.0.1
+Version: 1.0.2
 Summary: 
 Author: kaluluosi
 Author-email: kaluluosi@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

