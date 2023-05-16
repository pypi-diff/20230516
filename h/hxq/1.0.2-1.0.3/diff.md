# Comparing `tmp/hxq-1.0.2.tar.gz` & `tmp/hxq-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\hxq-1.0.2.tar", last modified: Tue Apr 18 16:16:59 2023, max compression
+gzip compressed data, was "hxq-1.0.3.tar", last modified: Tue May 16 16:59:46 2023, max compression
```

## Comparing `hxq-1.0.2.tar` & `hxq-1.0.3.tar`

### file list

```diff
@@ -1,37 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 16:16:59.000000 hxq-1.0.2/
--rw-rw-rw-   0        0        0      169 2023-04-18 16:16:59.000000 hxq-1.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-18 16:16:59.000000 hxq-1.0.2/hxq/
--rw-rw-rw-   0        0        0      141 2023-04-18 16:12:01.000000 hxq-1.0.2/hxq/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 16:16:59.000000 hxq-1.0.2/hxq/interface/
--rw-rw-rw-   0        0        0      122 2023-04-18 15:01:16.000000 hxq-1.0.2/hxq/interface/__init__.py
--rw-rw-rw-   0        0        0     4230 2023-04-14 14:47:06.000000 hxq-1.0.2/hxq/interface/db_helper.py
--rw-rw-rw-   0        0        0      300 2023-04-13 13:36:38.000000 hxq-1.0.2/hxq/interface/httpx.py
--rw-rw-rw-   0        0        0      186 2023-04-13 13:11:19.000000 hxq-1.0.2/hxq/interface/win32.py
-drwxrwxrwx   0        0        0        0 2023-04-18 16:16:59.000000 hxq-1.0.2/hxq/libs/
--rw-rw-rw-   0        0        0      123 2023-04-13 13:04:22.000000 hxq-1.0.2/hxq/libs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 16:16:59.000000 hxq-1.0.2/hxq/libs/db/
--rw-rw-rw-   0        0        0      383 2023-04-13 12:57:46.000000 hxq-1.0.2/hxq/libs/db/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 16:16:59.000000 hxq-1.0.2/hxq/libs/httpx/
--rw-rw-rw-   0        0        0      127 2022-07-07 15:51:40.000000 hxq-1.0.2/hxq/libs/httpx/__init__.py
--rw-rw-rw-   0        0        0      639 2023-04-13 14:06:06.000000 hxq-1.0.2/hxq/libs/httpx/chrome_agent.py
--rw-rw-rw-   0        0        0     9254 2023-04-18 16:10:44.000000 hxq-1.0.2/hxq/libs/httpx/http.py
--rw-rw-rw-   0        0        0     3420 2023-04-18 16:09:26.000000 hxq-1.0.2/hxq/libs/httpx/session.py
-drwxrwxrwx   0        0        0        0 2023-04-18 16:16:59.000000 hxq-1.0.2/hxq/libs/win32/
--rw-rw-rw-   0        0        0     1983 2023-04-13 13:36:03.000000 hxq-1.0.2/hxq/libs/win32/__init__.py
--rw-rw-rw-   0        0        0      736 2023-04-18 16:10:11.000000 hxq-1.0.2/hxq/main.py
-drwxrwxrwx   0        0        0        0 2023-04-18 16:16:59.000000 hxq-1.0.2/hxq/utils/
--rw-rw-rw-   0        0        0      123 2023-04-10 15:30:39.000000 hxq-1.0.2/hxq/utils/__init__.py
--rw-rw-rw-   0        0        0     3596 2023-04-13 14:08:04.000000 hxq-1.0.2/hxq/utils/common.py
--rw-rw-rw-   0        0        0     1676 2023-04-10 15:34:13.000000 hxq-1.0.2/hxq/utils/decorator.py
--rw-rw-rw-   0        0        0     1576 2023-04-10 16:12:31.000000 hxq-1.0.2/hxq/utils/encipher.py
--rw-rw-rw-   0        0        0      418 2023-04-10 15:33:03.000000 hxq-1.0.2/hxq/utils/pic_code.py
--rw-rw-rw-   0        0        0      314 2023-04-09 13:39:57.000000 hxq-1.0.2/hxq/utils/ran_func.py
--rw-rw-rw-   0        0        0     3460 2023-04-18 14:38:43.000000 hxq-1.0.2/hxq/utils/threadx.py
-drwxrwxrwx   0        0        0        0 2023-04-18 16:16:59.000000 hxq-1.0.2/hxq.egg-info/
--rw-rw-rw-   0        0        0      169 2023-04-18 16:16:59.000000 hxq-1.0.2/hxq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      600 2023-04-18 16:16:59.000000 hxq-1.0.2/hxq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 16:16:59.000000 hxq-1.0.2/hxq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      110 2023-04-18 16:16:59.000000 hxq-1.0.2/hxq.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-04-18 16:16:59.000000 hxq-1.0.2/hxq.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-18 16:16:59.000000 hxq-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      788 2023-04-18 16:12:50.000000 hxq-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 16:59:46.311096 hxq-1.0.3/
+-rw-rw-rw-   0        0        0      169 2023-05-16 16:59:46.311096 hxq-1.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-16 16:59:46.264327 hxq-1.0.3/hxq/
+-rw-rw-rw-   0        0        0      141 2023-05-14 06:56:41.000000 hxq-1.0.3/hxq/__init__.py
+-rw-rw-rw-   0        0        0      187 2023-05-16 16:59:00.000000 hxq-1.0.3/hxq/db.py
+-rw-rw-rw-   0        0        0      300 2023-04-13 13:36:38.000000 hxq-1.0.3/hxq/httpx.py
+drwxrwxrwx   0        0        0        0 2023-05-16 16:59:46.279843 hxq-1.0.3/hxq/libs/
+-rw-rw-rw-   0        0        0      123 2023-04-13 13:04:22.000000 hxq-1.0.3/hxq/libs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 16:59:46.279843 hxq-1.0.3/hxq/libs/db/
+-rw-rw-rw-   0        0        0     4414 2023-05-14 06:55:27.000000 hxq-1.0.3/hxq/libs/db/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 16:59:46.295499 hxq-1.0.3/hxq/libs/httpx/
+-rw-rw-rw-   0        0        0      127 2022-07-07 15:51:40.000000 hxq-1.0.3/hxq/libs/httpx/__init__.py
+-rw-rw-rw-   0        0        0      639 2023-04-13 14:06:06.000000 hxq-1.0.3/hxq/libs/httpx/chrome_agent.py
+-rw-rw-rw-   0        0        0     9254 2023-04-18 16:10:44.000000 hxq-1.0.3/hxq/libs/httpx/http.py
+-rw-rw-rw-   0        0        0     3420 2023-04-18 16:09:26.000000 hxq-1.0.3/hxq/libs/httpx/session.py
+drwxrwxrwx   0        0        0        0 2023-05-16 16:59:46.295499 hxq-1.0.3/hxq/libs/win32/
+-rw-rw-rw-   0        0        0     1983 2023-05-14 06:38:20.000000 hxq-1.0.3/hxq/libs/win32/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 16:59:46.311096 hxq-1.0.3/hxq/utils/
+-rw-rw-rw-   0        0        0      123 2023-04-10 15:30:39.000000 hxq-1.0.3/hxq/utils/__init__.py
+-rw-rw-rw-   0        0        0     3788 2023-05-14 06:43:45.000000 hxq-1.0.3/hxq/utils/common.py
+-rw-rw-rw-   0        0        0     1676 2023-04-10 15:34:13.000000 hxq-1.0.3/hxq/utils/decorator.py
+-rw-rw-rw-   0        0        0     1518 2023-05-14 06:46:38.000000 hxq-1.0.3/hxq/utils/encipher.py
+-rw-rw-rw-   0        0        0      480 2023-05-14 06:53:55.000000 hxq-1.0.3/hxq/utils/pic_code.py
+-rw-rw-rw-   0        0        0     3460 2023-04-18 14:38:43.000000 hxq-1.0.3/hxq/utils/threadx.py
+-rw-rw-rw-   0        0        0      186 2023-04-13 13:11:19.000000 hxq-1.0.3/hxq/win32.py
+drwxrwxrwx   0        0        0        0 2023-05-16 16:59:46.279843 hxq-1.0.3/hxq.egg-info/
+-rw-rw-rw-   0        0        0      169 2023-05-16 16:59:46.000000 hxq-1.0.3/hxq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      503 2023-05-16 16:59:46.000000 hxq-1.0.3/hxq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 16:59:46.000000 hxq-1.0.3/hxq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      124 2023-05-16 16:59:46.000000 hxq-1.0.3/hxq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-05-16 16:59:46.000000 hxq-1.0.3/hxq.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-16 16:59:46.311096 hxq-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      815 2023-05-16 16:59:33.000000 hxq-1.0.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `hxq-1.0.2/hxq/interface/db_helper.py` & `hxq-1.0.3/hxq/libs/db/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 # -*- coding: utf-8 -*-
-# @Time    : 2023/4/6 23:38
+# @Time    : 2022/12/6 23:18
 # @Author  : hxq
 # @Software: PyCharm
-# @File    : db_helper.py
+# @File    : __init__.py
 import contextlib
 import re
 import json
+import datetime
 import importlib
 from typing import Union
-
-from hxq.libs.db import DateTimeEncoder
+from json import JSONEncoder
 from dbutils.pooled_db import PooledDB, PooledDedicatedDBConnection
 
-__all__ = [
-    "DBHelper",
-]
+
+class DateTimeEncoder(JSONEncoder):
+    def default(self, obj):
+        if isinstance(obj, (datetime.date, datetime.datetime)):
+            return obj.isoformat(sep=" ")
+        return super().default(obj)
 
 
 class DBHelper:
     """简单的数据库连接池助手"""
 
     def __init__(self, config):
         self.config = self.import_config(config)
```

### Comparing `hxq-1.0.2/hxq/libs/httpx/chrome_agent.py` & `hxq-1.0.3/hxq/libs/httpx/chrome_agent.py`

 * *Files identical despite different names*

### Comparing `hxq-1.0.2/hxq/libs/httpx/http.py` & `hxq-1.0.3/hxq/libs/httpx/http.py`

 * *Files identical despite different names*

### Comparing `hxq-1.0.2/hxq/libs/httpx/session.py` & `hxq-1.0.3/hxq/libs/httpx/session.py`

 * *Files identical despite different names*

### Comparing `hxq-1.0.2/hxq/libs/win32/__init__.py` & `hxq-1.0.3/hxq/libs/win32/__init__.py`

 * *Files identical despite different names*

### Comparing `hxq-1.0.2/hxq/utils/common.py` & `hxq-1.0.3/hxq/utils/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # -*- coding: utf-8 -*-
 # @Time    : 2022/7/10 20:42
 # @Author  : hxq
 # @Software: PyCharm
 # @File    : common.py
 import asyncio
 import os
+import random
+import string
 import sys
 import pkgutil
 import socket
 import subprocess
 from functools import wraps
 
 from hxq.utils.decorator import except_desc, func_run_times
@@ -35,14 +37,21 @@
 def url2ip(url):
     socket_list = socket.getaddrinfo(url, None, 0, socket.SOCK_STREAM)
     ip_info = socket_list[0][4][0]
     print('【{}】 IP地址：{}'.format(url, ip_info))
     return ip_info
 
 
+def random_password(length=12):
+    """
+    随机密码生成
+    """
+    return ''.join(random.sample(string.digits + string.ascii_letters * 1, length))
+
+
 @func_run_times()
 def array_subtotal(this_list):
     """
     将数组重复数据进行分类汇总，生成一个汇总字典
     """
     data = dict()
     [data.update({item: data[item] + 1}) if item in data else data.update({item: 1}) for item in this_list].clear()
@@ -100,9 +109,8 @@
     print(sys.modules.get('subprocess').__file__)
     print(get_root_path('db'))
     # print(url2ip('z1.m1907.cn'))
     # arr = [1, 3, 5, 7, 9, 5, 1, 3, 6, 7]  # 用于在本地测试的数据，使用时需注释掉前两行
     # print(array_subtotal(arr))
     # for i in range(1, 10000):
     #     arr.append(random.randint(1, 99999))
-
     # print(run_command('ipconfig'))
```

### Comparing `hxq-1.0.2/hxq/utils/decorator.py` & `hxq-1.0.3/hxq/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `hxq-1.0.2/hxq/utils/encipher.py` & `hxq-1.0.3/hxq/utils/encipher.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,9 +59,8 @@
         """
         base64解码
         """
         return base64.b64decode(encode_bytes(string)).decode('utf-8')
 
 
 if __name__ == '__main__':
-    print(Encipher.get_file_md5('qrcode_img.png'))
-    print(Encipher.get_file_base64('qrcode_img.png'))
+    print(Encipher.get_file_md5('encipher.py'))
```

### Comparing `hxq-1.0.2/hxq/utils/threadx.py` & `hxq-1.0.3/hxq/utils/threadx.py`

 * *Files identical despite different names*

### Comparing `hxq-1.0.2/setup.py` & `hxq-1.0.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from setuptools import find_packages, setup
 
 setup(name='hxq',
       author='hxq',
-      version='1.0.2',
+      version='1.0.3',
       packages=find_packages(exclude=["*.demo", "*.demo.*", "tests", "demos"]),
       author_email='337168530@qq.com',
       description="这是一个python工具包",
       license="GPL",
       # 而 extras_require 这里仅表示该模块会依赖这些包,深度使用模块时，才会用到，这里需要你手动安装
       extras_require={
           'HTML': ["bs4>=0.0.1", "xmltodict>=1.2"],
       },
       # install_requires 在安装模块时会自动安装依赖包
       install_requires=[
-          'requests>=2.24.0',
-          'lxml>=4.9.2',
-          'pymysql~=1.0.3',
-          'DBUtils~=3.0.2',
-          'aiofiles~=23.1.0',
+          'requests==2.24.0',
+          'lxml==4.9.2',
+          'pymysql==1.0.3',
+          'DBUtils==3.0.2',
+          'aiofiles==23.1.0',
+          'winshell==0.6'
       ]
       )
```

