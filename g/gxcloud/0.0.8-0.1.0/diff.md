# Comparing `tmp/gxcloud-0.0.8.tar.gz` & `tmp/gxcloud-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gxcloud-0.0.8.tar", last modified: Tue May 16 20:57:51 2023, max compression
+gzip compressed data, was "gxcloud-0.1.0.tar", last modified: Wed Dec  7 14:24:35 2022, max compression
```

## Comparing `gxcloud-0.0.8.tar` & `gxcloud-0.1.0.tar`

### file list

```diff
@@ -1,28 +1,25 @@
-drwxr-xr-x   0 zac.thiel (1547939247) 253301862        0 2023-05-16 20:57:51.347896 gxcloud-0.0.8/
--rw-r--r--   0 zac.thiel (1547939247) 253301862     1052 2022-09-27 16:10:43.000000 gxcloud-0.0.8/LICENSE
--rw-r--r--   0 zac.thiel (1547939247) 253301862      524 2023-05-16 20:57:51.345435 gxcloud-0.0.8/PKG-INFO
--rw-r--r--   0 zac.thiel (1547939247) 253301862      137 2022-09-27 16:04:16.000000 gxcloud-0.0.8/README.md
--rw-r--r--   0 zac.thiel (1547939247) 253301862      502 2023-05-16 20:56:25.000000 gxcloud-0.0.8/pyproject.toml
--rw-r--r--   0 zac.thiel (1547939247) 253301862       38 2023-05-16 20:57:51.347993 gxcloud-0.0.8/setup.cfg
-drwxr-xr-x   0 zac.thiel (1547939247) 253301862        0 2023-05-16 20:57:51.331734 gxcloud-0.0.8/src/
--rw-r--r--   0 zac.thiel (1547939247) 253301862        0 2022-12-07 19:08:20.000000 gxcloud-0.0.8/src/__init__.py
-drwxr-xr-x   0 zac.thiel (1547939247) 253301862        0 2023-05-16 20:57:51.337328 gxcloud-0.0.8/src/govdelivery/
--rw-r--r--   0 zac.thiel (1547939247) 253301862        0 2022-11-18 16:44:15.000000 gxcloud-0.0.8/src/govdelivery/__init__.py
--rw-r--r--   0 zac.thiel (1547939247) 253301862      258 2022-11-18 16:51:55.000000 gxcloud-0.0.8/src/govdelivery/authorization.py
--rw-r--r--   0 zac.thiel (1547939247) 253301862     2536 2022-12-15 18:17:33.000000 gxcloud-0.0.8/src/govdelivery/bulletins.py
--rw-r--r--   0 zac.thiel (1547939247) 253301862     2675 2022-12-07 19:33:47.000000 gxcloud-0.0.8/src/govdelivery/categories.py
--rw-r--r--   0 zac.thiel (1547939247) 253301862     3349 2022-12-07 19:35:54.000000 gxcloud-0.0.8/src/govdelivery/subscriptions.py
--rw-r--r--   0 zac.thiel (1547939247) 253301862     1933 2022-12-07 17:29:57.000000 gxcloud-0.0.8/src/govdelivery/topics.py
-drwxr-xr-x   0 zac.thiel (1547939247) 253301862        0 2023-05-16 20:57:51.339870 gxcloud-0.0.8/src/gxcloud.egg-info/
--rw-r--r--   0 zac.thiel (1547939247) 253301862      524 2023-05-16 20:57:51.000000 gxcloud-0.0.8/src/gxcloud.egg-info/PKG-INFO
--rw-r--r--   0 zac.thiel (1547939247) 253301862      534 2023-05-16 20:57:51.000000 gxcloud-0.0.8/src/gxcloud.egg-info/SOURCES.txt
--rw-r--r--   0 zac.thiel (1547939247) 253301862        1 2023-05-16 20:57:51.000000 gxcloud-0.0.8/src/gxcloud.egg-info/dependency_links.txt
--rw-r--r--   0 zac.thiel (1547939247) 253301862       19 2023-05-16 20:57:51.000000 gxcloud-0.0.8/src/gxcloud.egg-info/requires.txt
--rw-r--r--   0 zac.thiel (1547939247) 253301862       42 2023-05-16 20:57:51.000000 gxcloud-0.0.8/src/gxcloud.egg-info/top_level.txt
-drwxr-xr-x   0 zac.thiel (1547939247) 253301862        0 2023-05-16 20:57:51.343800 gxcloud-0.0.8/src/opencities/
--rw-r--r--   0 zac.thiel (1547939247) 253301862        0 2022-10-18 20:32:50.000000 gxcloud-0.0.8/src/opencities/__init__.py
--rw-r--r--   0 zac.thiel (1547939247) 253301862     1144 2022-12-14 15:49:00.000000 gxcloud-0.0.8/src/opencities/authorization.py
--rw-r--r--   0 zac.thiel (1547939247) 253301862    15252 2023-05-16 20:42:46.000000 gxcloud-0.0.8/src/opencities/files.py
--rw-r--r--   0 zac.thiel (1547939247) 253301862     8959 2023-03-14 21:26:18.000000 gxcloud-0.0.8/src/opencities/pages.py
-drwxr-xr-x   0 zac.thiel (1547939247) 253301862        0 2023-05-16 20:57:51.345032 gxcloud-0.0.8/src/utilities/
--rw-r--r--   0 zac.thiel (1547939247) 253301862        0 2023-03-14 21:02:03.000000 gxcloud-0.0.8/src/utilities/__init__.py
+drwxr-xr-x   0 zac.thiel (1547939247) 253301862        0 2022-12-07 14:24:35.330037 gxcloud-0.1.0/
+-rw-r--r--   0 zac.thiel (1547939247) 253301862     1052 2022-09-27 16:10:43.000000 gxcloud-0.1.0/LICENSE
+-rw-r--r--   0 zac.thiel (1547939247) 253301862      524 2022-12-07 14:24:35.329852 gxcloud-0.1.0/PKG-INFO
+-rw-r--r--   0 zac.thiel (1547939247) 253301862      137 2022-09-27 16:04:16.000000 gxcloud-0.1.0/README.md
+-rw-r--r--   0 zac.thiel (1547939247) 253301862      572 2022-12-01 18:15:17.000000 gxcloud-0.1.0/pyproject.toml
+-rw-r--r--   0 zac.thiel (1547939247) 253301862       38 2022-12-07 14:24:35.330089 gxcloud-0.1.0/setup.cfg
+drwxr-xr-x   0 zac.thiel (1547939247) 253301862        0 2022-12-07 14:24:35.321900 gxcloud-0.1.0/src/
+drwxr-xr-x   0 zac.thiel (1547939247) 253301862        0 2022-12-07 14:24:35.325963 gxcloud-0.1.0/src/govdelivery/
+-rw-r--r--   0 zac.thiel (1547939247) 253301862        0 2022-11-18 16:44:15.000000 gxcloud-0.1.0/src/govdelivery/__init__.py
+-rw-r--r--   0 zac.thiel (1547939247) 253301862      258 2022-11-18 16:51:55.000000 gxcloud-0.1.0/src/govdelivery/authorization.py
+-rw-r--r--   0 zac.thiel (1547939247) 253301862     1981 2022-12-06 16:13:06.000000 gxcloud-0.1.0/src/govdelivery/bulletins.py
+-rw-r--r--   0 zac.thiel (1547939247) 253301862     2690 2022-12-06 15:28:11.000000 gxcloud-0.1.0/src/govdelivery/categories.py
+-rw-r--r--   0 zac.thiel (1547939247) 253301862     3364 2022-12-06 15:57:57.000000 gxcloud-0.1.0/src/govdelivery/subscriptions.py
+-rw-r--r--   0 zac.thiel (1547939247) 253301862     1948 2022-12-07 14:16:53.000000 gxcloud-0.1.0/src/govdelivery/topics.py
+drwxr-xr-x   0 zac.thiel (1547939247) 253301862        0 2022-12-07 14:24:35.327774 gxcloud-0.1.0/src/gxcloud.egg-info/
+-rw-r--r--   0 zac.thiel (1547939247) 253301862      524 2022-12-07 14:24:35.000000 gxcloud-0.1.0/src/gxcloud.egg-info/PKG-INFO
+-rw-r--r--   0 zac.thiel (1547939247) 253301862      492 2022-12-07 14:24:35.000000 gxcloud-0.1.0/src/gxcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 zac.thiel (1547939247) 253301862        1 2022-12-07 14:24:35.000000 gxcloud-0.1.0/src/gxcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 zac.thiel (1547939247) 253301862       65 2022-12-07 14:24:35.000000 gxcloud-0.1.0/src/gxcloud.egg-info/requires.txt
+-rw-r--r--   0 zac.thiel (1547939247) 253301862       23 2022-12-07 14:24:35.000000 gxcloud-0.1.0/src/gxcloud.egg-info/top_level.txt
+drwxr-xr-x   0 zac.thiel (1547939247) 253301862        0 2022-12-07 14:24:35.329471 gxcloud-0.1.0/src/opencities/
+-rw-r--r--   0 zac.thiel (1547939247) 253301862        0 2022-10-18 20:32:50.000000 gxcloud-0.1.0/src/opencities/__init__.py
+-rw-r--r--   0 zac.thiel (1547939247) 253301862     1144 2022-12-06 21:09:01.000000 gxcloud-0.1.0/src/opencities/authorization.py
+-rw-r--r--   0 zac.thiel (1547939247) 253301862     5240 2022-10-21 15:42:52.000000 gxcloud-0.1.0/src/opencities/files.py
+-rw-r--r--   0 zac.thiel (1547939247) 253301862     3490 2022-12-07 14:11:28.000000 gxcloud-0.1.0/src/opencities/pages.py
```

### Comparing `gxcloud-0.0.8/LICENSE` & `gxcloud-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gxcloud-0.0.8/PKG-INFO` & `gxcloud-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gxcloud
-Version: 0.0.8
+Version: 0.1.0
 Summary: A python package for using the OpenCities API
 Author-email: Zac Thiel <zac.thiel@granicus.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `gxcloud-0.0.8/src/govdelivery/bulletins.py` & `gxcloud-0.1.0/src/govdelivery/bulletins.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .authorization import basic_auth
+from src.govdelivery.authorization import basic_auth
 import requests
 import xmltodict as xd
 
 # Global variables
 base_url = 'https://api.govdelivery.com/api/account/'
 endpoint = '/bulletins'
 endpoint_send = '/send_now'
@@ -17,15 +17,15 @@
     for category in category_codes:
         payload_categories = payload_categories + '<category><code>' + category + '</code></category>'
     payload_categories = payload_categories + '</categories>'
 
     if topic_codes:
         payload_topics = '<topics type="array">'
         for topic in topic_codes:
-            payload_topics = payload_topics + '<topic><code>' + topic + '</code></topic>'
+            payload_topics = payload_topics + '<topic><code>' + topic + '</topic></code>'
         payload_topics = payload_topics + '</topics>'
         body = body + payload_topics
     else:
         payload_topics = '<topics type="array"></topics>'
         body = body + payload_topics
 
     if optional_fields:
@@ -51,27 +51,8 @@
     try:
         payload.raise_for_status()
     except requests.exceptions.HTTPError as err:
         print(err)
 
     data = xd.parse(payload.content)
 
-    return data
-
-
-def get_bulletin(username, password, account_code, bulletin_id):
-    auth = basic_auth(username, password)
-    url = base_url + account_code + endpoint + '/' + bulletin_id + '.xml'
-    headers = {'Content-Type': 'text/xml; charset: utf-8',
-               'Authorization': auth}
-
-    payload = requests.request('GET',
-                               url,
-                               headers=headers)
-    try:
-        payload.raise_for_status()
-    except requests.exceptions.HTTPError as err:
-        print(err)
-
-    data = xd.parse(payload.content)
-
     return data
```

### Comparing `gxcloud-0.0.8/src/govdelivery/categories.py` & `gxcloud-0.1.0/src/govdelivery/categories.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .authorization import basic_auth
+from src.govdelivery.authorization import basic_auth
 import requests
 import xmltodict as xd
 
 # Global API variables
 base_url = 'https://api.govdelivery.com/api/account/'
 endpoint = '/categories.xml'
 xml_attributes = {'default-open': ' type="boolean"'}
```

### Comparing `gxcloud-0.0.8/src/govdelivery/subscriptions.py` & `gxcloud-0.1.0/src/govdelivery/subscriptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .authorization import basic_auth
+from src.govdelivery.authorization import basic_auth
 import requests
 import xmltodict as xd
 import base64
 
 # Global variables
 base_url = 'https://api.govdelivery.com/api/account/'
 endpoint_subscriber = '/subscribers.xml'
```

### Comparing `gxcloud-0.0.8/src/govdelivery/topics.py` & `gxcloud-0.1.0/src/govdelivery/topics.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .authorization import basic_auth
+from src.govdelivery.authorization import basic_auth
 import requests
 import xmltodict as xd
 
 # Global API variables
 base_url = 'https://api.govdelivery.com/api/account/'
 topics_endpoint = '/topics.xml'
 base_header = {'Content-Type': 'text/xml; charset: utf-8'}
```

### Comparing `gxcloud-0.0.8/src/gxcloud.egg-info/PKG-INFO` & `gxcloud-0.1.0/src/gxcloud.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gxcloud
-Version: 0.0.8
+Version: 0.1.0
 Summary: A python package for using the OpenCities API
 Author-email: Zac Thiel <zac.thiel@granicus.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `gxcloud-0.0.8/src/opencities/authorization.py` & `gxcloud-0.1.0/src/opencities/authorization.py`

 * *Files 19% similar despite different names*

```diff
@@ -26,12 +26,12 @@
 
     auth = 'hmac ' + app_id + ':' + signature + ':' + nonce + ':' + timestamp
 
     return auth
 
 
 def basic_auth(api_key, app_id):
-    ascii_bytes = (app_id + ':' + api_key).encode('ascii', 'replace')
+    ascii_bytes = (api_key + ':' + app_id).encode('ascii', 'replace')
     basic_base64 = base64.b64encode(ascii_bytes).decode()
     auth = 'Basic ' + basic_base64
 
     return auth
```

