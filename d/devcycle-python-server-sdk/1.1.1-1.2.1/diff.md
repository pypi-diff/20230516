# Comparing `tmp/devcycle-python-server-sdk-1.1.1.tar.gz` & `tmp/devcycle-python-server-sdk-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devcycle-python-server-sdk-1.1.1.tar", last modified: Mon Nov 14 13:59:18 2022, max compression
+gzip compressed data, was "devcycle-python-server-sdk-1.2.1.tar", last modified: Mon May 15 21:03:55 2023, max compression
```

## Comparing `devcycle-python-server-sdk-1.1.1.tar` & `devcycle-python-server-sdk-1.2.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 adamwootton   (501) staff       (20)        0 2022-11-14 13:59:18.536111 devcycle-python-server-sdk-1.1.1/
--rw-r--r--   0 adamwootton   (501) staff       (20)     1071 2022-11-14 13:45:44.000000 devcycle-python-server-sdk-1.1.1/LICENSE
--rw-r--r--   0 adamwootton   (501) staff       (20)      455 2022-11-14 13:59:18.536162 devcycle-python-server-sdk-1.1.1/PKG-INFO
--rw-r--r--   0 adamwootton   (501) staff       (20)     1412 2022-11-14 13:45:44.000000 devcycle-python-server-sdk-1.1.1/README.md
-drwxr-xr-x   0 adamwootton   (501) staff       (20)        0 2022-11-14 13:59:18.532458 devcycle-python-server-sdk-1.1.1/devcycle_python_sdk/
--rw-r--r--   0 adamwootton   (501) staff       (20)        5 2022-11-14 13:59:08.000000 devcycle-python-server-sdk-1.1.1/devcycle_python_sdk/VERSION.txt
--rw-r--r--   0 adamwootton   (501) staff       (20)     1103 2022-11-14 13:45:44.000000 devcycle-python-server-sdk-1.1.1/devcycle_python_sdk/__init__.py
-drwxr-xr-x   0 adamwootton   (501) staff       (20)        0 2022-11-14 13:59:18.532802 devcycle-python-server-sdk-1.1.1/devcycle_python_sdk/api/
--rw-r--r--   0 adamwootton   (501) staff       (20)      144 2022-11-14 13:45:44.000000 devcycle-python-server-sdk-1.1.1/devcycle_python_sdk/api/__init__.py
--rw-r--r--   0 adamwootton   (501) staff       (20)    18116 2022-11-14 13:58:44.000000 devcycle-python-server-sdk-1.1.1/devcycle_python_sdk/api/dvc_client.py
--rw-r--r--   0 adamwootton   (501) staff       (20)    24815 2022-11-14 13:45:44.000000 devcycle-python-server-sdk-1.1.1/devcycle_python_sdk/api_client.py
--rw-r--r--   0 adamwootton   (501) staff       (20)     8288 2022-11-14 13:58:44.000000 devcycle-python-server-sdk-1.1.1/devcycle_python_sdk/configuration.py
--rw-r--r--   0 adamwootton   (501) staff       (20)       97 2022-11-14 13:45:44.000000 devcycle-python-server-sdk-1.1.1/devcycle_python_sdk/dvc_options.py
-drwxr-xr-x   0 adamwootton   (501) staff       (20)        0 2022-11-14 13:59:18.534107 devcycle-python-server-sdk-1.1.1/devcycle_python_sdk/models/
--rw-r--r--   0 adamwootton   (501) staff       (20)      833 2022-11-14 13:45:44.000000 devcycle-python-server-sdk-1.1.1/devcycle_python_sdk/models/__init__.py
--rw-r--r--   0 adamwootton   (501) staff       (20)     4015 2022-11-14 13:45:44.000000 devcycle-python-server-sdk-1.1.1/devcycle_python_sdk/models/error_response.py
--rw-r--r--   0 adamwootton   (501) staff       (20)     6173 2022-11-14 13:45:44.000000 devcycle-python-server-sdk-1.1.1/devcycle_python_sdk/models/event.py
--rw-r--r--   0 adamwootton   (501) staff       (20)     8501 2022-11-14 13:45:44.000000 devcycle-python-server-sdk-1.1.1/devcycle_python_sdk/models/feature.py
--rw-r--r--   0 adamwootton   (501) staff       (20)     3137 2022-11-14 13:45:44.000000 devcycle-python-server-sdk-1.1.1/devcycle_python_sdk/models/inline_response201.py
--rw-r--r--   0 adamwootton   (501) staff       (20)    15928 2022-11-14 13:45:44.000000 devcycle-python-server-sdk-1.1.1/devcycle_python_sdk/models/user_data.py
--rw-r--r--   0 adamwootton   (501) staff       (20)     3801 2022-11-14 13:45:44.000000 devcycle-python-server-sdk-1.1.1/devcycle_python_sdk/models/user_data_and_events_body.py
--rw-r--r--   0 adamwootton   (501) staff       (20)     6525 2022-11-14 13:45:44.000000 devcycle-python-server-sdk-1.1.1/devcycle_python_sdk/models/variable.py
--rw-r--r--   0 adamwootton   (501) staff       (20)    13219 2022-11-14 13:45:44.000000 devcycle-python-server-sdk-1.1.1/devcycle_python_sdk/rest.py
-drwxr-xr-x   0 adamwootton   (501) staff       (20)        0 2022-11-14 13:59:18.534622 devcycle-python-server-sdk-1.1.1/devcycle_python_server_sdk.egg-info/
--rw-r--r--   0 adamwootton   (501) staff       (20)      455 2022-11-14 13:59:18.000000 devcycle-python-server-sdk-1.1.1/devcycle_python_server_sdk.egg-info/PKG-INFO
--rw-r--r--   0 adamwootton   (501) staff       (20)     1145 2022-11-14 13:59:18.000000 devcycle-python-server-sdk-1.1.1/devcycle_python_server_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 adamwootton   (501) staff       (20)        1 2022-11-14 13:59:18.000000 devcycle-python-server-sdk-1.1.1/devcycle_python_server_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 adamwootton   (501) staff       (20)       48 2022-11-14 13:59:18.000000 devcycle-python-server-sdk-1.1.1/devcycle_python_server_sdk.egg-info/requires.txt
--rw-r--r--   0 adamwootton   (501) staff       (20)       33 2022-11-14 13:59:18.000000 devcycle-python-server-sdk-1.1.1/devcycle_python_server_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 adamwootton   (501) staff       (20)        0 2022-11-14 13:59:18.534781 devcycle-python-server-sdk-1.1.1/example/
--rw-r--r--   0 adamwootton   (501) staff       (20)        0 2022-11-14 13:45:44.000000 devcycle-python-server-sdk-1.1.1/example/__init__.py
--rw-r--r--   0 adamwootton   (501) staff       (20)     2206 2022-11-14 13:58:44.000000 devcycle-python-server-sdk-1.1.1/example/example.py
--rw-r--r--   0 adamwootton   (501) staff       (20)       79 2022-11-14 13:59:18.536339 devcycle-python-server-sdk-1.1.1/setup.cfg
--rw-r--r--   0 adamwootton   (501) staff       (20)     1320 2022-11-14 13:45:44.000000 devcycle-python-server-sdk-1.1.1/setup.py
-drwxr-xr-x   0 adamwootton   (501) staff       (20)        0 2022-11-14 13:59:18.535978 devcycle-python-server-sdk-1.1.1/test/
--rw-r--r--   0 adamwootton   (501) staff       (20)        0 2022-11-14 13:45:44.000000 devcycle-python-server-sdk-1.1.1/test/__init__.py
--rw-r--r--   0 adamwootton   (501) staff       (20)     1376 2022-11-14 13:45:44.000000 devcycle-python-server-sdk-1.1.1/test/test_devcycle_api.py
--rw-r--r--   0 adamwootton   (501) staff       (20)      965 2022-11-14 13:45:44.000000 devcycle-python-server-sdk-1.1.1/test/test_error_response.py
--rw-r--r--   0 adamwootton   (501) staff       (20)      915 2022-11-14 13:45:44.000000 devcycle-python-server-sdk-1.1.1/test/test_feature.py
--rw-r--r--   0 adamwootton   (501) staff       (20)      997 2022-11-14 13:45:44.000000 devcycle-python-server-sdk-1.1.1/test/test_inline_response200.py
--rw-r--r--   0 adamwootton   (501) staff       (20)      925 2022-11-14 13:45:44.000000 devcycle-python-server-sdk-1.1.1/test/test_user_data.py
--rw-r--r--   0 adamwootton   (501) staff       (20)     1027 2022-11-14 13:45:44.000000 devcycle-python-server-sdk-1.1.1/test/test_user_data_and_event_body.py
--rw-r--r--   0 adamwootton   (501) staff       (20)      923 2022-11-14 13:45:44.000000 devcycle-python-server-sdk-1.1.1/test/test_variable.py
+drwxr-xr-x   0 jonathannorris   (501) staff       (20)        0 2023-05-15 21:03:55.161679 devcycle-python-server-sdk-1.2.1/
+-rw-r--r--   0 jonathannorris   (501) staff       (20)     1071 2021-12-17 15:42:42.000000 devcycle-python-server-sdk-1.2.1/LICENSE
+-rw-r--r--   0 jonathannorris   (501) staff       (20)      455 2023-05-15 21:03:55.161756 devcycle-python-server-sdk-1.2.1/PKG-INFO
+-rw-r--r--   0 jonathannorris   (501) staff       (20)     1481 2023-05-15 20:59:25.000000 devcycle-python-server-sdk-1.2.1/README.md
+drwxr-xr-x   0 jonathannorris   (501) staff       (20)        0 2023-05-15 21:03:55.157518 devcycle-python-server-sdk-1.2.1/devcycle_python_sdk/
+-rw-r--r--   0 jonathannorris   (501) staff       (20)        5 2023-05-15 21:03:46.000000 devcycle-python-server-sdk-1.2.1/devcycle_python_sdk/VERSION.txt
+-rw-r--r--   0 jonathannorris   (501) staff       (20)     1103 2023-05-09 21:26:17.000000 devcycle-python-server-sdk-1.2.1/devcycle_python_sdk/__init__.py
+drwxr-xr-x   0 jonathannorris   (501) staff       (20)        0 2023-05-15 21:03:55.157966 devcycle-python-server-sdk-1.2.1/devcycle_python_sdk/api/
+-rw-r--r--   0 jonathannorris   (501) staff       (20)      144 2021-12-17 15:42:42.000000 devcycle-python-server-sdk-1.2.1/devcycle_python_sdk/api/__init__.py
+-rw-r--r--   0 jonathannorris   (501) staff       (20)    18490 2023-05-15 20:59:25.000000 devcycle-python-server-sdk-1.2.1/devcycle_python_sdk/api/dvc_client.py
+-rw-r--r--   0 jonathannorris   (501) staff       (20)    24815 2021-12-17 15:42:42.000000 devcycle-python-server-sdk-1.2.1/devcycle_python_sdk/api_client.py
+-rw-r--r--   0 jonathannorris   (501) staff       (20)     8288 2023-05-09 21:26:17.000000 devcycle-python-server-sdk-1.2.1/devcycle_python_sdk/configuration.py
+-rw-r--r--   0 jonathannorris   (501) staff       (20)       97 2023-05-09 21:26:17.000000 devcycle-python-server-sdk-1.2.1/devcycle_python_sdk/dvc_options.py
+drwxr-xr-x   0 jonathannorris   (501) staff       (20)        0 2023-05-15 21:03:55.159425 devcycle-python-server-sdk-1.2.1/devcycle_python_sdk/models/
+-rw-r--r--   0 jonathannorris   (501) staff       (20)      833 2021-12-17 15:42:42.000000 devcycle-python-server-sdk-1.2.1/devcycle_python_sdk/models/__init__.py
+-rw-r--r--   0 jonathannorris   (501) staff       (20)     4015 2021-12-17 15:42:42.000000 devcycle-python-server-sdk-1.2.1/devcycle_python_sdk/models/error_response.py
+-rw-r--r--   0 jonathannorris   (501) staff       (20)     6173 2021-12-17 15:42:42.000000 devcycle-python-server-sdk-1.2.1/devcycle_python_sdk/models/event.py
+-rw-r--r--   0 jonathannorris   (501) staff       (20)     8501 2023-05-09 21:26:17.000000 devcycle-python-server-sdk-1.2.1/devcycle_python_sdk/models/feature.py
+-rw-r--r--   0 jonathannorris   (501) staff       (20)     3137 2021-12-17 15:42:42.000000 devcycle-python-server-sdk-1.2.1/devcycle_python_sdk/models/inline_response201.py
+-rw-r--r--   0 jonathannorris   (501) staff       (20)    15928 2021-12-17 15:42:42.000000 devcycle-python-server-sdk-1.2.1/devcycle_python_sdk/models/user_data.py
+-rw-r--r--   0 jonathannorris   (501) staff       (20)     3801 2021-12-17 15:42:42.000000 devcycle-python-server-sdk-1.2.1/devcycle_python_sdk/models/user_data_and_events_body.py
+-rw-r--r--   0 jonathannorris   (501) staff       (20)     6525 2021-12-17 15:42:42.000000 devcycle-python-server-sdk-1.2.1/devcycle_python_sdk/models/variable.py
+-rw-r--r--   0 jonathannorris   (501) staff       (20)    13219 2021-12-17 15:42:42.000000 devcycle-python-server-sdk-1.2.1/devcycle_python_sdk/rest.py
+drwxr-xr-x   0 jonathannorris   (501) staff       (20)        0 2023-05-15 21:03:55.160158 devcycle-python-server-sdk-1.2.1/devcycle_python_server_sdk.egg-info/
+-rw-r--r--   0 jonathannorris   (501) staff       (20)      455 2023-05-15 21:03:55.000000 devcycle-python-server-sdk-1.2.1/devcycle_python_server_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 jonathannorris   (501) staff       (20)     1145 2023-05-15 21:03:55.000000 devcycle-python-server-sdk-1.2.1/devcycle_python_server_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathannorris   (501) staff       (20)        1 2023-05-15 21:03:55.000000 devcycle-python-server-sdk-1.2.1/devcycle_python_server_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathannorris   (501) staff       (20)       48 2023-05-15 21:03:55.000000 devcycle-python-server-sdk-1.2.1/devcycle_python_server_sdk.egg-info/requires.txt
+-rw-r--r--   0 jonathannorris   (501) staff       (20)       33 2023-05-15 21:03:55.000000 devcycle-python-server-sdk-1.2.1/devcycle_python_server_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 jonathannorris   (501) staff       (20)        0 2023-05-15 21:03:55.160392 devcycle-python-server-sdk-1.2.1/example/
+-rw-r--r--   0 jonathannorris   (501) staff       (20)        0 2021-12-17 15:42:42.000000 devcycle-python-server-sdk-1.2.1/example/__init__.py
+-rw-r--r--   0 jonathannorris   (501) staff       (20)     2505 2023-05-15 20:59:25.000000 devcycle-python-server-sdk-1.2.1/example/example.py
+-rw-r--r--   0 jonathannorris   (501) staff       (20)       79 2023-05-15 21:03:55.161974 devcycle-python-server-sdk-1.2.1/setup.cfg
+-rw-r--r--   0 jonathannorris   (501) staff       (20)     1320 2023-05-09 21:26:17.000000 devcycle-python-server-sdk-1.2.1/setup.py
+drwxr-xr-x   0 jonathannorris   (501) staff       (20)        0 2023-05-15 21:03:55.161538 devcycle-python-server-sdk-1.2.1/test/
+-rw-r--r--   0 jonathannorris   (501) staff       (20)        0 2021-12-17 15:42:42.000000 devcycle-python-server-sdk-1.2.1/test/__init__.py
+-rw-r--r--   0 jonathannorris   (501) staff       (20)     1376 2021-12-17 15:42:42.000000 devcycle-python-server-sdk-1.2.1/test/test_devcycle_api.py
+-rw-r--r--   0 jonathannorris   (501) staff       (20)      965 2021-12-17 15:42:42.000000 devcycle-python-server-sdk-1.2.1/test/test_error_response.py
+-rw-r--r--   0 jonathannorris   (501) staff       (20)      915 2021-12-17 15:42:42.000000 devcycle-python-server-sdk-1.2.1/test/test_feature.py
+-rw-r--r--   0 jonathannorris   (501) staff       (20)      997 2021-12-17 15:42:42.000000 devcycle-python-server-sdk-1.2.1/test/test_inline_response200.py
+-rw-r--r--   0 jonathannorris   (501) staff       (20)      925 2021-12-17 15:42:42.000000 devcycle-python-server-sdk-1.2.1/test/test_user_data.py
+-rw-r--r--   0 jonathannorris   (501) staff       (20)     1027 2021-12-17 15:42:42.000000 devcycle-python-server-sdk-1.2.1/test/test_user_data_and_event_body.py
+-rw-r--r--   0 jonathannorris   (501) staff       (20)      923 2021-12-17 15:42:42.000000 devcycle-python-server-sdk-1.2.1/test/test_variable.py
```

### Comparing `devcycle-python-server-sdk-1.1.1/LICENSE` & `devcycle-python-server-sdk-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-1.1.1/README.md` & `devcycle-python-server-sdk-1.2.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -32,14 +32,16 @@
      dvc = DVCClient(configuration, options)
     
      user = UserData(
         user_id='test',
         email='example@example.ca',
         country='CA'
     )
+
+    value = dvc.variableValue(user, 'feature-key', 'default-value')
 ```
 
 ## Usage
 
 To find usage documentation, visit our [docs](https://docs.devcycle.com/docs/sdk/server-side-sdks/python#usage).
 
 ## Development
```

### Comparing `devcycle-python-server-sdk-1.1.1/devcycle_python_sdk/__init__.py` & `devcycle-python-server-sdk-1.2.1/devcycle_python_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-1.1.1/devcycle_python_sdk/api/dvc_client.py` & `devcycle-python-server-sdk-1.2.1/devcycle_python_sdk/api/dvc_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,14 +133,25 @@
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+
+    def variableValue(self, user, key, default_value, **kwargs):
+        """Get variable value by key for user data  # noqa: E501
+
+        :param UserData user: (required)
+        :param str key: Variable key (required)
+        :param any default_value
+        :return: any variable value
+        """
+        return self.variable(user, key, default_value, **kwargs).value
+
     def variable(self, user, key, default_value, **kwargs):  # noqa: E501
         """Get variable by key for user data  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.variable(user, key, async_req=True)
         >>> result = thread.get()
```

### Comparing `devcycle-python-server-sdk-1.1.1/devcycle_python_sdk/api_client.py` & `devcycle-python-server-sdk-1.2.1/devcycle_python_sdk/api_client.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-1.1.1/devcycle_python_sdk/configuration.py` & `devcycle-python-server-sdk-1.2.1/devcycle_python_sdk/configuration.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-1.1.1/devcycle_python_sdk/models/__init__.py` & `devcycle-python-server-sdk-1.2.1/devcycle_python_sdk/models/__init__.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-1.1.1/devcycle_python_sdk/models/error_response.py` & `devcycle-python-server-sdk-1.2.1/devcycle_python_sdk/models/error_response.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-1.1.1/devcycle_python_sdk/models/event.py` & `devcycle-python-server-sdk-1.2.1/devcycle_python_sdk/models/event.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-1.1.1/devcycle_python_sdk/models/feature.py` & `devcycle-python-server-sdk-1.2.1/devcycle_python_sdk/models/feature.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-1.1.1/devcycle_python_sdk/models/inline_response201.py` & `devcycle-python-server-sdk-1.2.1/devcycle_python_sdk/models/inline_response201.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-1.1.1/devcycle_python_sdk/models/user_data.py` & `devcycle-python-server-sdk-1.2.1/devcycle_python_sdk/models/user_data.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-1.1.1/devcycle_python_sdk/models/user_data_and_events_body.py` & `devcycle-python-server-sdk-1.2.1/devcycle_python_sdk/models/user_data_and_events_body.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-1.1.1/devcycle_python_sdk/models/variable.py` & `devcycle-python-server-sdk-1.2.1/devcycle_python_sdk/models/variable.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-1.1.1/devcycle_python_sdk/rest.py` & `devcycle-python-server-sdk-1.2.1/devcycle_python_sdk/rest.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-1.1.1/devcycle_python_server_sdk.egg-info/SOURCES.txt` & `devcycle-python-server-sdk-1.2.1/devcycle_python_server_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-1.1.1/example/example.py` & `devcycle-python-server-sdk-1.2.1/example/example.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 from __future__ import print_function
 from devcycle_python_sdk import Configuration, DVCClient, DVCOptions, UserData, Event, Variable
 from devcycle_python_sdk.rest import ApiException
+
 def main():
+    """
+    Sample generic usage of the Python SDK.
+    For a Django specific sample app, please see https://github.com/DevCycleHQ/python-django-example-app/
 
+    """
     configuration = Configuration()
-    configuration.api_key['Authorization'] = 'YOUR SERVER KEY HERE'
+    configuration.api_key['Authorization'] = '<DVC_SERVER_SDK_KEY>'
     options = DVCOptions(enableEdgeDB=True)
 
     # create an instance of the API class
     dvc = DVCClient(configuration, options)
 
     user = UserData(
         user_id='test',
         email='yo@yo.ca',
         country='CA'
     )
-    variable = Variable(value='test', is_defaulted=True, key='test')
-    print('test varia')
-    print(variable)
     event = Event(
         type="customEvent",
         target="somevariable.key"
     )
 
     try:
         # Get all features by key for user data
@@ -29,14 +31,21 @@
         print(api_response)
     except ApiException as e:
         print("Exception when calling DevcycleApi->all_features: %s\n" % e)
 
     key = 'elliot-test' # str | Variable key
 
     try:
+        # Get variable value by key for user data
+        value = dvc.variableValue(user, key, 'default-value')
+        print(value)
+    except ApiException as e:
+        print("Exception when calling DevcycleApi->varaible: %s\n" % e)
+
+    try:
         # Get variable by key for user data
         api_response = dvc.variable(user, key, 'default-value')
         print(api_response)
         if not api_response.is_defaulted:
             print('NOT DEFAULTED')
     except ApiException as e:
         print("Exception when calling DevcycleApi->varaible: %s\n" % e)
```

### Comparing `devcycle-python-server-sdk-1.1.1/setup.py` & `devcycle-python-server-sdk-1.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-1.1.1/test/test_devcycle_api.py` & `devcycle-python-server-sdk-1.2.1/test/test_devcycle_api.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-1.1.1/test/test_error_response.py` & `devcycle-python-server-sdk-1.2.1/test/test_error_response.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-1.1.1/test/test_feature.py` & `devcycle-python-server-sdk-1.2.1/test/test_feature.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-1.1.1/test/test_inline_response200.py` & `devcycle-python-server-sdk-1.2.1/test/test_inline_response200.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-1.1.1/test/test_user_data.py` & `devcycle-python-server-sdk-1.2.1/test/test_user_data.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-1.1.1/test/test_user_data_and_event_body.py` & `devcycle-python-server-sdk-1.2.1/test/test_user_data_and_event_body.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-1.1.1/test/test_variable.py` & `devcycle-python-server-sdk-1.2.1/test/test_variable.py`

 * *Files identical despite different names*

