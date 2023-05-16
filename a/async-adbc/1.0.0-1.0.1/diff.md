# Comparing `tmp/async_adbc-1.0.0.tar.gz` & `tmp/async_adbc-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_adbc-1.0.0.tar", max compression
+gzip compressed data, was "async_adbc-1.0.1.tar", max compression
```

## Comparing `async_adbc-1.0.0.tar` & `async_adbc-1.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0        0 2023-05-15 10:09:09.049083 async_adbc-1.0.0/async_adbc/__init__.py
--rw-r--r--   0        0        0     1103 2023-05-15 07:38:35.715767 async_adbc-1.0.0/async_adbc/adbclient.py
--rw-r--r--   0        0        0     2959 2023-05-16 05:06:18.477892 async_adbc-1.0.0/async_adbc/device.py
--rw-r--r--   0        0        0      595 2023-05-16 03:03:39.272909 async_adbc-1.0.0/async_adbc/plugins/__init__.py
--rw-r--r--   0        0        0      502 2023-05-16 02:17:28.058635 async_adbc-1.0.0/async_adbc/plugins/am.py
--rw-r--r--   0        0        0     2657 2023-05-16 02:32:10.948830 async_adbc-1.0.0/async_adbc/plugins/battery.py
--rw-r--r--   0        0        0    12253 2023-05-16 05:10:13.078037 async_adbc-1.0.0/async_adbc/plugins/cpu.py
--rw-r--r--   0        0        0     1236 2023-05-16 02:45:13.949373 async_adbc-1.0.0/async_adbc/plugins/forward.py
--rw-r--r--   0        0        0     3933 2023-05-16 02:51:02.455214 async_adbc-1.0.0/async_adbc/plugins/fps.py
--rw-r--r--   0        0        0      614 2023-05-15 12:07:09.349059 async_adbc-1.0.0/async_adbc/plugins/gpu.py
--rw-r--r--   0        0        0      393 2023-05-15 12:13:38.890420 async_adbc-1.0.0/async_adbc/plugins/input.py
--rw-r--r--   0        0        0      895 2023-05-16 03:18:01.857216 async_adbc-1.0.0/async_adbc/plugins/logcat.py
--rw-r--r--   0        0        0     2209 2023-05-16 03:26:42.422860 async_adbc-1.0.0/async_adbc/plugins/mem.py
--rw-r--r--   0        0        0     5591 2023-05-15 11:29:44.554984 async_adbc-1.0.0/async_adbc/plugins/pm.py
--rw-r--r--   0        0        0      510 2023-05-15 11:29:29.910308 async_adbc-1.0.0/async_adbc/plugins/prop.py
--rw-r--r--   0        0        0     4615 2023-05-16 04:20:29.957697 async_adbc-1.0.0/async_adbc/plugins/temp.py
--rw-r--r--   0        0        0     2210 2023-05-16 05:02:45.070953 async_adbc-1.0.0/async_adbc/plugins/traffic.py
--rw-r--r--   0        0        0      807 2023-05-15 11:29:32.496380 async_adbc-1.0.0/async_adbc/plugins/utils.py
--rw-r--r--   0        0        0     4509 2023-05-15 08:29:42.104875 async_adbc-1.0.0/async_adbc/protocol.py
--rw-r--r--   0        0        0      790 2023-05-15 05:22:12.341481 async_adbc-1.0.0/async_adbc/service/__init__.py
--rw-r--r--   0        0        0    10210 2023-05-16 02:45:36.884703 async_adbc-1.0.0/async_adbc/service/host.py
--rw-r--r--   0        0        0    10074 2023-05-16 02:01:45.258884 async_adbc-1.0.0/async_adbc/service/local.py
--rw-r--r--   0        0        0     1090 2023-05-16 05:23:42.403245 async_adbc-1.0.0/LICENSE
--rw-r--r--   0        0        0      482 2023-05-16 06:49:19.024526 async_adbc-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      423 2023-05-15 02:24:29.723099 async_adbc-1.0.0/README.md
--rw-r--r--   0        0        0      849 1970-01-01 00:00:00.000000 async_adbc-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0       70 2023-05-16 06:58:01.167502 async_adbc-1.0.1/async_adbc/__init__.py
+-rw-r--r--   0        0        0      998 2023-05-16 06:58:27.465793 async_adbc-1.0.1/async_adbc/adbclient.py
+-rw-r--r--   0        0        0     2983 2023-05-16 06:52:10.041298 async_adbc-1.0.1/async_adbc/device.py
+-rw-r--r--   0        0        0      601 2023-05-16 06:51:45.869292 async_adbc-1.0.1/async_adbc/plugins/__init__.py
+-rw-r--r--   0        0        0      502 2023-05-16 02:17:28.058635 async_adbc-1.0.1/async_adbc/plugins/am.py
+-rw-r--r--   0        0        0     2657 2023-05-16 02:32:10.948830 async_adbc-1.0.1/async_adbc/plugins/battery.py
+-rw-r--r--   0        0        0    12259 2023-05-16 06:51:45.908294 async_adbc-1.0.1/async_adbc/plugins/cpu.py
+-rw-r--r--   0        0        0     1242 2023-05-16 06:51:45.797292 async_adbc-1.0.1/async_adbc/plugins/forward.py
+-rw-r--r--   0        0        0     3933 2023-05-16 02:51:02.455214 async_adbc-1.0.1/async_adbc/plugins/fps.py
+-rw-r--r--   0        0        0      614 2023-05-15 12:07:09.349059 async_adbc-1.0.1/async_adbc/plugins/gpu.py
+-rw-r--r--   0        0        0      393 2023-05-15 12:13:38.890420 async_adbc-1.0.1/async_adbc/plugins/input.py
+-rw-r--r--   0        0        0      895 2023-05-16 03:18:01.857216 async_adbc-1.0.1/async_adbc/plugins/logcat.py
+-rw-r--r--   0        0        0     2209 2023-05-16 03:26:42.422860 async_adbc-1.0.1/async_adbc/plugins/mem.py
+-rw-r--r--   0        0        0     5597 2023-05-16 06:51:45.819291 async_adbc-1.0.1/async_adbc/plugins/pm.py
+-rw-r--r--   0        0        0      510 2023-05-15 11:29:29.910308 async_adbc-1.0.1/async_adbc/plugins/prop.py
+-rw-r--r--   0        0        0     4615 2023-05-16 04:20:29.957697 async_adbc-1.0.1/async_adbc/plugins/temp.py
+-rw-r--r--   0        0        0     2216 2023-05-16 06:51:45.868298 async_adbc-1.0.1/async_adbc/plugins/traffic.py
+-rw-r--r--   0        0        0      807 2023-05-15 11:29:32.496380 async_adbc-1.0.1/async_adbc/plugins/utils.py
+-rw-r--r--   0        0        0     4509 2023-05-15 08:29:42.104875 async_adbc-1.0.1/async_adbc/protocol.py
+-rw-r--r--   0        0        0      796 2023-05-16 06:51:45.874292 async_adbc-1.0.1/async_adbc/service/__init__.py
+-rw-r--r--   0        0        0    10228 2023-05-16 06:51:45.939291 async_adbc-1.0.1/async_adbc/service/host.py
+-rw-r--r--   0        0        0    10086 2023-05-16 06:51:45.937291 async_adbc-1.0.1/async_adbc/service/local.py
+-rw-r--r--   0        0        0     1090 2023-05-16 05:23:42.403245 async_adbc-1.0.1/LICENSE
+-rw-r--r--   0        0        0      482 2023-05-16 06:58:10.840881 async_adbc-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      423 2023-05-15 02:24:29.723099 async_adbc-1.0.1/README.md
+-rw-r--r--   0        0        0      849 1970-01-01 00:00:00.000000 async_adbc-1.0.1/PKG-INFO
```

### Comparing `async_adbc-1.0.0/async_adbc/adbclient.py` & `async_adbc-1.0.1/async_adbc/adbclient.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,13 @@
-import asyncio
-import functools
-from types import MethodType
-from typing import Any, AsyncGenerator, Coroutine
-from adbc.device import Device, Status
-from adbc.protocol import Connection, create_connection
+from async_adbc.device import Status
+from async_adbc.protocol import Connection, create_connection
 from dataclasses import dataclass
 from dataclasses_json import dataclass_json
 
-from adbc.service.host import HostService
+from async_adbc.service.host import HostService
 
 
 DEFAULT_HOST = "127.0.0.1"
 DEFAULT_PORT = 5037
 
 
 class DeviceNotFoundError(Exception):
```

### Comparing `async_adbc-1.0.0/async_adbc/device.py` & `async_adbc-1.0.1/async_adbc/device.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import asyncio
 import enum
 import re
 import typing
-from adbc.protocol import Connection
-from adbc.service.local import LocalService
+from async_adbc.protocol import Connection
+from async_adbc.service.local import LocalService
 
-from adbc.plugins import (
+from async_adbc.plugins import (
     PMPlugin,
     PropPlugin,
     CPUPlugin,
     GPUPlugin,
     BatteryPlugin,
     FpsPlugin,
     MemPlugin,
@@ -18,15 +18,15 @@
     TrafficPlugin,
     ForwardPlugin,
     ActivityManagerPlugin,
     LogcatPlugin,
 )
 
 if typing.TYPE_CHECKING:
-    from adbc.adbclient import ADBClient
+    from async_adbc.adbclient import ADBClient
 
 
 class Status(enum.Enum):
     DEVICE = "device"
     OFFLINE = "offline"
     UNKNOWN = "unknown"
```

### Comparing `async_adbc-1.0.0/async_adbc/plugins/__init__.py` & `async_adbc-1.0.1/async_adbc/plugins/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import typing
 
 if typing.TYPE_CHECKING:
-    from adbc.device import Device
+    from async_adbc.device import Device
 
 
 class Plugin:
     def __init__(self, device: "Device") -> None:
         self._device = device
```

### Comparing `async_adbc-1.0.0/async_adbc/plugins/battery.py` & `async_adbc-1.0.1/async_adbc/plugins/battery.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.0/async_adbc/plugins/cpu.py` & `async_adbc-1.0.1/async_adbc/plugins/cpu.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 from typing import Optional
 from dataclasses_json import dataclass_json
 
 from . import Plugin
 
 if typing.TYPE_CHECKING:
-    from adbc.device import Device
+    from async_adbc.device import Device
 
 CPUStatMap = dict[int, "CPUStat"]
 CPUUsageMap = dict[int, "CPUUsage"]
 
 
 @dataclass_json
 @dataclass
```

### Comparing `async_adbc-1.0.0/async_adbc/plugins/forward.py` & `async_adbc-1.0.1/async_adbc/plugins/forward.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import typing
 from . import Plugin
 
 if typing.TYPE_CHECKING:
-    from adbc.adbclient import ForwardRule
+    from async_adbc.adbclient import ForwardRule
 
 
 class ForwardPlugin(Plugin):
     """Device的forward端口映射封装
 
     与ADBClient的forward接口区别在于Device的forward接口都是作用在当前设备。
     可以理解为方法参数中serialno已经默认传入了Device的serialno。
```

### Comparing `async_adbc-1.0.0/async_adbc/plugins/fps.py` & `async_adbc-1.0.1/async_adbc/plugins/fps.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.0/async_adbc/plugins/gpu.py` & `async_adbc-1.0.1/async_adbc/plugins/gpu.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.0/async_adbc/plugins/logcat.py` & `async_adbc-1.0.1/async_adbc/plugins/logcat.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.0/async_adbc/plugins/mem.py` & `async_adbc-1.0.1/async_adbc/plugins/mem.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.0/async_adbc/plugins/pm.py` & `async_adbc-1.0.1/async_adbc/plugins/pm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import re
 from typing import Any
 
-from adbc.service.local import ProgressCallback
+from async_adbc.service.local import ProgressCallback
 from . import Plugin
 
 
 class InstallError(Exception):
     def __init__(self, src: str, msg) -> None:
         super().__init__(f"{src} 安装失败 - [{msg}]")
```

### Comparing `async_adbc-1.0.0/async_adbc/plugins/temp.py` & `async_adbc-1.0.1/async_adbc/plugins/temp.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.0/async_adbc/plugins/traffic.py` & `async_adbc-1.0.1/async_adbc/plugins/traffic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import typing
 from . import Plugin
 from typing import Optional, overload
 from dataclasses import dataclass
 from dataclasses_json import dataclass_json
 
 if typing.TYPE_CHECKING:
-    from adbc.device import Device
+    from async_adbc.device import Device
 
 
 @dataclass_json
 @dataclass
 class TrafficStat:
     """
     流量统计，单位byte
```

### Comparing `async_adbc-1.0.0/async_adbc/plugins/utils.py` & `async_adbc-1.0.1/async_adbc/plugins/utils.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.0/async_adbc/protocol.py` & `async_adbc-1.0.1/async_adbc/protocol.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.0/async_adbc/service/__init__.py` & `async_adbc-1.0.1/async_adbc/service/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 adbc是跟adb server的客户端，也就是 HOST SERVICES的封装。
 device是跟adbd守护进程的客户端，也就是LOCAL SERVICES的封装。
 """
 
 
 import abc
 
-from adbc.protocol import Connection
+from async_adbc.protocol import Connection
 
 
 class Service(abc.ABC):
     @abc.abstractmethod
     async def create_connection(self) -> Connection:
         ...
```

### Comparing `async_adbc-1.0.0/async_adbc/service/host.py` & `async_adbc-1.0.1/async_adbc/service/host.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import abc
 from dataclasses import dataclass
 from typing import Any, AsyncGenerator, Union
 
 from dataclasses_json import dataclass_json
-from adbc.service import Service
-from adbc.device import Device, Status
-from adbc.protocol import Connection
+from async_adbc.service import Service
+from async_adbc.device import Device, Status
+from async_adbc.protocol import Connection
 
 
 class DeviceNotFoundError(Exception):
     def __init__(self, serialno: str, *args: object) -> None:
         super().__init__(f"{serialno} 不存在", *args)
```

### Comparing `async_adbc-1.0.0/async_adbc/service/local.py` & `async_adbc-1.0.1/async_adbc/service/local.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from dataclasses import dataclass
 import os
 from stat import S_IFREG
 import struct
 from typing import Callable, Optional
 
 from dataclasses_json import dataclass_json
-from adbc.protocol import DATA, DONE, FAIL, RECV, SEND, Connection
-from adbc.service import Service
+from async_adbc.protocol import DATA, DONE, FAIL, RECV, SEND, Connection
+from async_adbc.service import Service
 
 ProgressCallback = Callable[[str, int, int], None]
 
 
 @dataclass_json
 @dataclass
 class ReverseRule:
```

### Comparing `async_adbc-1.0.0/LICENSE` & `async_adbc-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.0/PKG-INFO` & `async_adbc-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-adbc
-Version: 1.0.0
+Version: 1.0.1
 Summary: 
 Author: kaluluosi
 Author-email: kaluluosi@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

