# Comparing `tmp/serviceboot-2.1.5.tar.gz` & `tmp/serviceboot-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/serviceboot-2.1.5.tar", last modified: Mon May 15 02:25:35 2023, max compression
+gzip compressed data, was "dist/serviceboot-2.1.6.tar", last modified: Tue May 16 00:56:30 2023, max compression
```

## Comparing `serviceboot-2.1.5.tar` & `serviceboot-2.1.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-15 02:25:35.000000 serviceboot-2.1.5/
--rw-rw-r--   0 hls       (1000) hls       (1000)     2726 2023-05-15 02:25:35.000000 serviceboot-2.1.5/PKG-INFO
--rw-rw-r--   0 hls       (1000) hls       (1000)     1526 2023-05-09 04:02:39.000000 serviceboot-2.1.5/README.md
-drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-15 02:25:35.000000 serviceboot-2.1.5/serviceboot/
--rw-rw-r--   0 hls       (1000) hls       (1000)        0 2022-11-15 06:17:47.000000 serviceboot-2.1.5/serviceboot/__init__.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     3283 2023-05-15 02:24:29.000000 serviceboot-2.1.5/serviceboot/build_docker.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     4542 2023-05-15 02:24:29.000000 serviceboot-2.1.5/serviceboot/build_zip.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     1376 2022-11-15 06:17:47.000000 serviceboot-2.1.5/serviceboot/command.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     4143 2022-11-15 06:17:47.000000 serviceboot-2.1.5/serviceboot/compile_python.py
--rw-rw-r--   0 hls       (1000) hls       (1000)      417 2022-11-15 06:17:47.000000 serviceboot-2.1.5/serviceboot/config_client.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     3010 2022-11-15 06:17:47.000000 serviceboot-2.1.5/serviceboot/consul_client.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     3171 2022-11-15 06:17:47.000000 serviceboot-2.1.5/serviceboot/oauth_client.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     2790 2022-11-15 06:17:47.000000 serviceboot-2.1.5/serviceboot/onboarding.py
--rw-rw-r--   0 hls       (1000) hls       (1000)      178 2022-11-15 06:17:47.000000 serviceboot-2.1.5/serviceboot/request_info.py
--rw-rw-r--   0 hls       (1000) hls       (1000)    23524 2023-05-12 02:13:11.000000 serviceboot-2.1.5/serviceboot/serviceboot.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     1144 2022-11-15 06:17:47.000000 serviceboot-2.1.5/serviceboot/token_service.py
-drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-15 02:25:35.000000 serviceboot-2.1.5/serviceboot.egg-info/
--rw-rw-r--   0 hls       (1000) hls       (1000)     2726 2023-05-15 02:25:35.000000 serviceboot-2.1.5/serviceboot.egg-info/PKG-INFO
--rw-rw-r--   0 hls       (1000) hls       (1000)      556 2023-05-15 02:25:35.000000 serviceboot-2.1.5/serviceboot.egg-info/SOURCES.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)        1 2023-05-15 02:25:35.000000 serviceboot-2.1.5/serviceboot.egg-info/dependency_links.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)       83 2023-05-15 02:25:35.000000 serviceboot-2.1.5/serviceboot.egg-info/entry_points.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)       93 2023-05-15 02:25:35.000000 serviceboot-2.1.5/serviceboot.egg-info/requires.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)       12 2023-05-15 02:25:35.000000 serviceboot-2.1.5/serviceboot.egg-info/top_level.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)       38 2023-05-15 02:25:35.000000 serviceboot-2.1.5/setup.cfg
--rw-rw-r--   0 hls       (1000) hls       (1000)     2438 2023-05-15 02:25:29.000000 serviceboot-2.1.5/setup.py
+drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-16 00:56:30.000000 serviceboot-2.1.6/
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2726 2023-05-16 00:56:30.000000 serviceboot-2.1.6/PKG-INFO
+-rw-rw-r--   0 hls       (1000) hls       (1000)     1526 2023-05-09 04:02:39.000000 serviceboot-2.1.6/README.md
+drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-16 00:56:30.000000 serviceboot-2.1.6/serviceboot/
+-rw-rw-r--   0 hls       (1000) hls       (1000)        0 2022-11-15 06:17:47.000000 serviceboot-2.1.6/serviceboot/__init__.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     3283 2023-05-15 02:27:33.000000 serviceboot-2.1.6/serviceboot/build_docker.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     4542 2023-05-15 02:27:33.000000 serviceboot-2.1.6/serviceboot/build_zip.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     1376 2022-11-15 06:17:47.000000 serviceboot-2.1.6/serviceboot/command.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     4143 2022-11-15 06:17:47.000000 serviceboot-2.1.6/serviceboot/compile_python.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)      417 2022-11-15 06:17:47.000000 serviceboot-2.1.6/serviceboot/config_client.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     3010 2022-11-15 06:17:47.000000 serviceboot-2.1.6/serviceboot/consul_client.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     3171 2022-11-15 06:17:47.000000 serviceboot-2.1.6/serviceboot/oauth_client.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2790 2022-11-15 06:17:47.000000 serviceboot-2.1.6/serviceboot/onboarding.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)      178 2022-11-15 06:17:47.000000 serviceboot-2.1.6/serviceboot/request_info.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)    23607 2023-05-16 00:56:26.000000 serviceboot-2.1.6/serviceboot/serviceboot.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     1144 2022-11-15 06:17:47.000000 serviceboot-2.1.6/serviceboot/token_service.py
+drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-16 00:56:30.000000 serviceboot-2.1.6/serviceboot.egg-info/
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2726 2023-05-16 00:56:29.000000 serviceboot-2.1.6/serviceboot.egg-info/PKG-INFO
+-rw-rw-r--   0 hls       (1000) hls       (1000)      556 2023-05-16 00:56:29.000000 serviceboot-2.1.6/serviceboot.egg-info/SOURCES.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)        1 2023-05-16 00:56:29.000000 serviceboot-2.1.6/serviceboot.egg-info/dependency_links.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)       83 2023-05-16 00:56:29.000000 serviceboot-2.1.6/serviceboot.egg-info/entry_points.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)       93 2023-05-16 00:56:29.000000 serviceboot-2.1.6/serviceboot.egg-info/requires.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)       12 2023-05-16 00:56:29.000000 serviceboot-2.1.6/serviceboot.egg-info/top_level.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)       38 2023-05-16 00:56:30.000000 serviceboot-2.1.6/setup.cfg
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2438 2023-05-16 00:56:26.000000 serviceboot-2.1.6/setup.py
```

### Comparing `serviceboot-2.1.5/PKG-INFO` & `serviceboot-2.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serviceboot
-Version: 2.1.5
+Version: 2.1.6
 Summary: ServiceBoot云原生微服务引擎
 Home-page: https://openi.pcl.ac.cn/cubepy/serviceboot
 Author: cubeai
 Author-email: cubeai@163.com
 License: Apache License 2.0
 Description: # ServiceBoot云原生微服务引擎
```

### Comparing `serviceboot-2.1.5/README.md` & `serviceboot-2.1.6/README.md`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.5/serviceboot/build_docker.py` & `serviceboot-2.1.6/serviceboot/build_docker.py`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.5/serviceboot/build_zip.py` & `serviceboot-2.1.6/serviceboot/build_zip.py`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.5/serviceboot/command.py` & `serviceboot-2.1.6/serviceboot/command.py`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.5/serviceboot/compile_python.py` & `serviceboot-2.1.6/serviceboot/compile_python.py`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.5/serviceboot/consul_client.py` & `serviceboot-2.1.6/serviceboot/consul_client.py`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.5/serviceboot/oauth_client.py` & `serviceboot-2.1.6/serviceboot/oauth_client.py`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.5/serviceboot/onboarding.py` & `serviceboot-2.1.6/serviceboot/onboarding.py`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.5/serviceboot/serviceboot.py` & `serviceboot-2.1.6/serviceboot/serviceboot.py`

 * *Files 1% similar despite different names*

```diff
@@ -591,27 +591,31 @@
     kwargs = {
         'server_name': '0.0.0.0',
         'server_port': g.python_frontend_port,
     }
     python_frontend.launch(**kwargs)
 
 
-def serviceboot_client(body=None):
+def serviceboot_client(action, **args):
     url = f'http://127.0.0.1:{g.port}/api/data'
     headers = {
         'Content-Type': 'application/json;charset=UTF-8',
         'Accept': '*/*',
     }
+    body = {
+        'action': action,
+        'args': args,
+    }
 
     try:
         res = requests.post(url=url, json=body, headers=headers)
     except Exception as e:
         return {
             'status': 'err',
-            'value': '网络或服务器故障!'
+            'value': '网络或服务器故障：' + str(e)
         }
 
     if res.status_code != 200:
         return {
             'status': 'err',
             'value': res.text
         }
```

### Comparing `serviceboot-2.1.5/serviceboot/token_service.py` & `serviceboot-2.1.6/serviceboot/token_service.py`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.5/serviceboot.egg-info/PKG-INFO` & `serviceboot-2.1.6/serviceboot.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serviceboot
-Version: 2.1.5
+Version: 2.1.6
 Summary: ServiceBoot云原生微服务引擎
 Home-page: https://openi.pcl.ac.cn/cubepy/serviceboot
 Author: cubeai
 Author-email: cubeai@163.com
 License: Apache License 2.0
 Description: # ServiceBoot云原生微服务引擎
```

### Comparing `serviceboot-2.1.5/serviceboot.egg-info/SOURCES.txt` & `serviceboot-2.1.6/serviceboot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.5/setup.py` & `serviceboot-2.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 with open("README.md", "r", encoding='utf-8') as file:
     long_description = file.read()
 
 
 setup(
     name='serviceboot',
-    version='2.1.5',
+    version='2.1.6',
     author='cubeai',
     author_email='cubeai@163.com',
     description='ServiceBoot云原生微服务引擎',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='Apache License 2.0',
     packages=find_packages(),
```

