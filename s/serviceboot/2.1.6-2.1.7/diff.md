# Comparing `tmp/serviceboot-2.1.6.tar.gz` & `tmp/serviceboot-2.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/serviceboot-2.1.6.tar", last modified: Tue May 16 00:56:30 2023, max compression
+gzip compressed data, was "dist/serviceboot-2.1.7.tar", last modified: Tue May 16 05:22:30 2023, max compression
```

## Comparing `serviceboot-2.1.6.tar` & `serviceboot-2.1.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-16 00:56:30.000000 serviceboot-2.1.6/
--rw-rw-r--   0 hls       (1000) hls       (1000)     2726 2023-05-16 00:56:30.000000 serviceboot-2.1.6/PKG-INFO
--rw-rw-r--   0 hls       (1000) hls       (1000)     1526 2023-05-09 04:02:39.000000 serviceboot-2.1.6/README.md
-drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-16 00:56:30.000000 serviceboot-2.1.6/serviceboot/
--rw-rw-r--   0 hls       (1000) hls       (1000)        0 2022-11-15 06:17:47.000000 serviceboot-2.1.6/serviceboot/__init__.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     3283 2023-05-15 02:27:33.000000 serviceboot-2.1.6/serviceboot/build_docker.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     4542 2023-05-15 02:27:33.000000 serviceboot-2.1.6/serviceboot/build_zip.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     1376 2022-11-15 06:17:47.000000 serviceboot-2.1.6/serviceboot/command.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     4143 2022-11-15 06:17:47.000000 serviceboot-2.1.6/serviceboot/compile_python.py
--rw-rw-r--   0 hls       (1000) hls       (1000)      417 2022-11-15 06:17:47.000000 serviceboot-2.1.6/serviceboot/config_client.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     3010 2022-11-15 06:17:47.000000 serviceboot-2.1.6/serviceboot/consul_client.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     3171 2022-11-15 06:17:47.000000 serviceboot-2.1.6/serviceboot/oauth_client.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     2790 2022-11-15 06:17:47.000000 serviceboot-2.1.6/serviceboot/onboarding.py
--rw-rw-r--   0 hls       (1000) hls       (1000)      178 2022-11-15 06:17:47.000000 serviceboot-2.1.6/serviceboot/request_info.py
--rw-rw-r--   0 hls       (1000) hls       (1000)    23607 2023-05-16 00:56:26.000000 serviceboot-2.1.6/serviceboot/serviceboot.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     1144 2022-11-15 06:17:47.000000 serviceboot-2.1.6/serviceboot/token_service.py
-drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-16 00:56:30.000000 serviceboot-2.1.6/serviceboot.egg-info/
--rw-rw-r--   0 hls       (1000) hls       (1000)     2726 2023-05-16 00:56:29.000000 serviceboot-2.1.6/serviceboot.egg-info/PKG-INFO
--rw-rw-r--   0 hls       (1000) hls       (1000)      556 2023-05-16 00:56:29.000000 serviceboot-2.1.6/serviceboot.egg-info/SOURCES.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)        1 2023-05-16 00:56:29.000000 serviceboot-2.1.6/serviceboot.egg-info/dependency_links.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)       83 2023-05-16 00:56:29.000000 serviceboot-2.1.6/serviceboot.egg-info/entry_points.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)       93 2023-05-16 00:56:29.000000 serviceboot-2.1.6/serviceboot.egg-info/requires.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)       12 2023-05-16 00:56:29.000000 serviceboot-2.1.6/serviceboot.egg-info/top_level.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)       38 2023-05-16 00:56:30.000000 serviceboot-2.1.6/setup.cfg
--rw-rw-r--   0 hls       (1000) hls       (1000)     2438 2023-05-16 00:56:26.000000 serviceboot-2.1.6/setup.py
+drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-16 05:22:30.000000 serviceboot-2.1.7/
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2726 2023-05-16 05:22:30.000000 serviceboot-2.1.7/PKG-INFO
+-rw-rw-r--   0 hls       (1000) hls       (1000)     1526 2023-05-09 04:02:39.000000 serviceboot-2.1.7/README.md
+drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-16 05:22:30.000000 serviceboot-2.1.7/serviceboot/
+-rw-rw-r--   0 hls       (1000) hls       (1000)        0 2022-11-15 06:17:47.000000 serviceboot-2.1.7/serviceboot/__init__.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     3283 2023-05-15 02:27:33.000000 serviceboot-2.1.7/serviceboot/build_docker.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     4542 2023-05-15 02:27:33.000000 serviceboot-2.1.7/serviceboot/build_zip.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     1376 2022-11-15 06:17:47.000000 serviceboot-2.1.7/serviceboot/command.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     4143 2022-11-15 06:17:47.000000 serviceboot-2.1.7/serviceboot/compile_python.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)      417 2022-11-15 06:17:47.000000 serviceboot-2.1.7/serviceboot/config_client.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     3010 2022-11-15 06:17:47.000000 serviceboot-2.1.7/serviceboot/consul_client.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     3171 2022-11-15 06:17:47.000000 serviceboot-2.1.7/serviceboot/oauth_client.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2790 2022-11-15 06:17:47.000000 serviceboot-2.1.7/serviceboot/onboarding.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)      178 2022-11-15 06:17:47.000000 serviceboot-2.1.7/serviceboot/request_info.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)    24746 2023-05-16 05:22:28.000000 serviceboot-2.1.7/serviceboot/serviceboot.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     1144 2022-11-15 06:17:47.000000 serviceboot-2.1.7/serviceboot/token_service.py
+drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-16 05:22:30.000000 serviceboot-2.1.7/serviceboot.egg-info/
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2726 2023-05-16 05:22:30.000000 serviceboot-2.1.7/serviceboot.egg-info/PKG-INFO
+-rw-rw-r--   0 hls       (1000) hls       (1000)      556 2023-05-16 05:22:30.000000 serviceboot-2.1.7/serviceboot.egg-info/SOURCES.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)        1 2023-05-16 05:22:30.000000 serviceboot-2.1.7/serviceboot.egg-info/dependency_links.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)       83 2023-05-16 05:22:30.000000 serviceboot-2.1.7/serviceboot.egg-info/entry_points.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)       93 2023-05-16 05:22:30.000000 serviceboot-2.1.7/serviceboot.egg-info/requires.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)       12 2023-05-16 05:22:30.000000 serviceboot-2.1.7/serviceboot.egg-info/top_level.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)       38 2023-05-16 05:22:30.000000 serviceboot-2.1.7/setup.cfg
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2438 2023-05-16 05:22:28.000000 serviceboot-2.1.7/setup.py
```

### Comparing `serviceboot-2.1.6/PKG-INFO` & `serviceboot-2.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serviceboot
-Version: 2.1.6
+Version: 2.1.7
 Summary: ServiceBoot云原生微服务引擎
 Home-page: https://openi.pcl.ac.cn/cubepy/serviceboot
 Author: cubeai
 Author-email: cubeai@163.com
 License: Apache License 2.0
 Description: # ServiceBoot云原生微服务引擎
```

### Comparing `serviceboot-2.1.6/README.md` & `serviceboot-2.1.7/README.md`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.6/serviceboot/build_docker.py` & `serviceboot-2.1.7/serviceboot/build_docker.py`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.6/serviceboot/build_zip.py` & `serviceboot-2.1.7/serviceboot/build_zip.py`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.6/serviceboot/command.py` & `serviceboot-2.1.7/serviceboot/command.py`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.6/serviceboot/compile_python.py` & `serviceboot-2.1.7/serviceboot/compile_python.py`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.6/serviceboot/consul_client.py` & `serviceboot-2.1.7/serviceboot/consul_client.py`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.6/serviceboot/oauth_client.py` & `serviceboot-2.1.7/serviceboot/oauth_client.py`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.6/serviceboot/onboarding.py` & `serviceboot-2.1.7/serviceboot/onboarding.py`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.6/serviceboot/serviceboot.py` & `serviceboot-2.1.7/serviceboot/serviceboot.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 import json
 import yaml
 import socket
+import inspect
 import logging
 import asyncio
 import platform
 import requests
 import threading
 import tornado.web
 import tornado.ioloop
@@ -587,14 +588,15 @@
 
 
 def python_frontend_thread(event_loop, python_frontend):
     asyncio.set_event_loop(event_loop)
     kwargs = {
         'server_name': '0.0.0.0',
         'server_port': g.python_frontend_port,
+        'show_api': False,
     }
     python_frontend.launch(**kwargs)
 
 
 def serviceboot_client(action, **args):
     url = f'http://127.0.0.1:{g.port}/api/data'
     headers = {
@@ -626,14 +628,45 @@
     except:
         # 非JSON数据（二进制字节流），直接返回
         result = res.content
 
     return result
 
 
+def gen_api_docs(*api_functions):
+    api_md_text = f'---\n\n## ServiceBoot APIs\n\n'
+    for function in api_functions:
+        name = function.__name__
+        args = inspect.signature(function).parameters
+
+        api_md_text += f'### {name}\n\n'
+        api_md_text += '- HTTP方法： POST\n\n'
+        api_md_text += '- API端点： /api/data\n\n'
+        api_md_text += '- HTTP请求体：\n'
+        api_md_text += '```\n'
+        api_md_text += '{\n'
+        api_md_text += f'    "action": "{name}",\n'
+        api_md_text += '    "args": {\n'
+        for arg in args:
+            api_md_text += f'        "{arg}": <{arg}的值>,\n'
+        api_md_text += '    }\n'
+        api_md_text += '}\n'
+        api_md_text += '```\n\n'
+        api_md_text += '- HTTP响应体：\n'
+        api_md_text += '```\n'
+        api_md_text += '{\n'
+        api_md_text += '    "status": "ok" | "err",\n'
+        api_md_text += '    "value": <服务端计算返回值> | <错误描述>,\n'
+        api_md_text += '}\n'
+        api_md_text += '```\n\n'
+    api_md_text += '\n\n'
+
+    return api_md_text
+
+
 def start():
     app_profile = os.environ.get('APP_PROFILE', 'dev').lower()
     log_level = logging.DEBUG if app_profile == 'dev' else logging.ERROR
     logging.basicConfig(level=log_level, format='%(asctime)s - %(levelname)s - %(message)s')
 
     try:
         with open('./application.yml', 'rb') as f:
```

### Comparing `serviceboot-2.1.6/serviceboot/token_service.py` & `serviceboot-2.1.7/serviceboot/token_service.py`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.6/serviceboot.egg-info/PKG-INFO` & `serviceboot-2.1.7/serviceboot.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serviceboot
-Version: 2.1.6
+Version: 2.1.7
 Summary: ServiceBoot云原生微服务引擎
 Home-page: https://openi.pcl.ac.cn/cubepy/serviceboot
 Author: cubeai
 Author-email: cubeai@163.com
 License: Apache License 2.0
 Description: # ServiceBoot云原生微服务引擎
```

### Comparing `serviceboot-2.1.6/serviceboot.egg-info/SOURCES.txt` & `serviceboot-2.1.7/serviceboot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.6/setup.py` & `serviceboot-2.1.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 with open("README.md", "r", encoding='utf-8') as file:
     long_description = file.read()
 
 
 setup(
     name='serviceboot',
-    version='2.1.6',
+    version='2.1.7',
     author='cubeai',
     author_email='cubeai@163.com',
     description='ServiceBoot云原生微服务引擎',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='Apache License 2.0',
     packages=find_packages(),
```

