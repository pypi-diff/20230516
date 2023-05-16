# Comparing `tmp/convoy-python-0.1.0.tar.gz` & `tmp/convoy-python-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "convoy-python-0.1.0.tar", last modified: Mon Mar 14 16:41:44 2022, max compression
+gzip compressed data, was "convoy-python-0.2.0.tar", last modified: Tue May 16 10:14:28 2023, max compression
```

## Comparing `convoy-python-0.1.0.tar` & `convoy-python-0.2.0.tar`

### file list

```diff
@@ -1,32 +1,34 @@
-drwxr-xr-x   0 ogban      (501) staff       (20)        0 2022-03-14 16:41:44.870974 convoy-python-0.1.0/
--rw-r--r--   0 ogban      (501) staff       (20)     1075 2022-03-11 10:43:32.000000 convoy-python-0.1.0/LICENSE
--rw-r--r--   0 ogban      (501) staff       (20)     1724 2022-03-14 16:41:44.870754 convoy-python-0.1.0/PKG-INFO
--rw-r--r--   0 ogban      (501) staff       (20)     1296 2022-03-14 15:53:45.000000 convoy-python-0.1.0/README.md
-drwxr-xr-x   0 ogban      (501) staff       (20)        0 2022-03-14 16:41:44.863603 convoy-python-0.1.0/convoy/
--rw-r--r--   0 ogban      (501) staff       (20)       32 2022-03-14 13:45:47.000000 convoy-python-0.1.0/convoy/__init__.py
-drwxr-xr-x   0 ogban      (501) staff       (20)        0 2022-03-14 16:41:44.868052 convoy-python-0.1.0/convoy/api/
--rw-r--r--   0 ogban      (501) staff       (20)      214 2022-03-14 13:47:54.000000 convoy-python-0.1.0/convoy/api/__init__.py
--rw-r--r--   0 ogban      (501) staff       (20)     1513 2022-03-14 16:29:33.000000 convoy-python-0.1.0/convoy/api/application.py
--rw-r--r--   0 ogban      (501) staff       (20)      693 2022-03-14 13:38:04.000000 convoy-python-0.1.0/convoy/api/delivery_attempts.py
--rw-r--r--   0 ogban      (501) staff       (20)     1819 2022-03-14 13:38:10.000000 convoy-python-0.1.0/convoy/api/endpoint.py
--rw-r--r--   0 ogban      (501) staff       (20)      930 2022-03-14 13:38:22.000000 convoy-python-0.1.0/convoy/api/event.py
--rw-r--r--   0 ogban      (501) staff       (20)     1192 2022-03-14 13:38:15.000000 convoy-python-0.1.0/convoy/api/event_delivery.py
--rw-r--r--   0 ogban      (501) staff       (20)     2504 2022-03-14 13:38:29.000000 convoy-python-0.1.0/convoy/api/group.py
-drwxr-xr-x   0 ogban      (501) staff       (20)        0 2022-03-14 16:41:44.868604 convoy-python-0.1.0/convoy/client/
--rw-r--r--   0 ogban      (501) staff       (20)       39 2022-03-14 13:47:59.000000 convoy-python-0.1.0/convoy/client/__init__.py
--rw-r--r--   0 ogban      (501) staff       (20)     2136 2022-03-14 15:37:29.000000 convoy-python-0.1.0/convoy/client/client.py
--rw-r--r--   0 ogban      (501) staff       (20)      918 2022-03-14 13:43:25.000000 convoy-python-0.1.0/convoy/convoy.py
--rw-r--r--   0 ogban      (501) staff       (20)     1525 2022-03-14 15:35:16.000000 convoy-python-0.1.0/convoy/data.py
-drwxr-xr-x   0 ogban      (501) staff       (20)        0 2022-03-14 16:41:44.869273 convoy-python-0.1.0/convoy/utils/
--rw-r--r--   0 ogban      (501) staff       (20)       47 2022-03-14 13:48:06.000000 convoy-python-0.1.0/convoy/utils/__init__.py
--rw-r--r--   0 ogban      (501) staff       (20)      347 2022-03-13 01:57:34.000000 convoy-python-0.1.0/convoy/utils/helpers.py
-drwxr-xr-x   0 ogban      (501) staff       (20)        0 2022-03-14 16:41:44.870164 convoy-python-0.1.0/convoy_python.egg-info/
--rw-r--r--   0 ogban      (501) staff       (20)     1724 2022-03-14 16:41:44.000000 convoy-python-0.1.0/convoy_python.egg-info/PKG-INFO
--rw-r--r--   0 ogban      (501) staff       (20)      546 2022-03-14 16:41:44.000000 convoy-python-0.1.0/convoy_python.egg-info/SOURCES.txt
--rw-r--r--   0 ogban      (501) staff       (20)        1 2022-03-14 16:41:44.000000 convoy-python-0.1.0/convoy_python.egg-info/dependency_links.txt
--rw-r--r--   0 ogban      (501) staff       (20)        9 2022-03-14 16:41:44.000000 convoy-python-0.1.0/convoy_python.egg-info/requires.txt
--rw-r--r--   0 ogban      (501) staff       (20)        8 2022-03-14 16:41:44.000000 convoy-python-0.1.0/convoy_python.egg-info/top_level.txt
--rw-r--r--   0 ogban      (501) staff       (20)       38 2022-03-14 16:41:44.871035 convoy-python-0.1.0/setup.cfg
--rw-r--r--   0 ogban      (501) staff       (20)      975 2022-03-14 15:49:31.000000 convoy-python-0.1.0/setup.py
-drwxr-xr-x   0 ogban      (501) staff       (20)        0 2022-03-14 16:41:44.870279 convoy-python-0.1.0/test/
--rw-r--r--   0 ogban      (501) staff       (20)     5188 2022-03-14 16:40:38.000000 convoy-python-0.1.0/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:14:28.591794 convoy-python-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-16 10:14:17.000000 convoy-python-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-05-16 10:14:28.591794 convoy-python-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-05-16 10:14:17.000000 convoy-python-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:14:28.587794 convoy-python-0.2.0/convoy/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-16 10:14:17.000000 convoy-python-0.2.0/convoy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:14:28.587794 convoy-python-0.2.0/convoy/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-16 10:14:17.000000 convoy-python-0.2.0/convoy/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-16 10:14:17.000000 convoy-python-0.2.0/convoy/api/delivery_attempts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-05-16 10:14:17.000000 convoy-python-0.2.0/convoy/api/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-16 10:14:17.000000 convoy-python-0.2.0/convoy/api/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-16 10:14:17.000000 convoy-python-0.2.0/convoy/api/event_delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-05-16 10:14:17.000000 convoy-python-0.2.0/convoy/api/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-05-16 10:14:17.000000 convoy-python-0.2.0/convoy/api/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-05-16 10:14:17.000000 convoy-python-0.2.0/convoy/api/subscription.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:14:28.587794 convoy-python-0.2.0/convoy/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-16 10:14:17.000000 convoy-python-0.2.0/convoy/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-05-16 10:14:17.000000 convoy-python-0.2.0/convoy/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-16 10:14:17.000000 convoy-python-0.2.0/convoy/convoy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-05-16 10:14:17.000000 convoy-python-0.2.0/convoy/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:14:28.587794 convoy-python-0.2.0/convoy/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-16 10:14:17.000000 convoy-python-0.2.0/convoy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-16 10:14:17.000000 convoy-python-0.2.0/convoy/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-05-16 10:14:17.000000 convoy-python-0.2.0/convoy/utils/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:14:28.591794 convoy-python-0.2.0/convoy_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-05-16 10:14:28.000000 convoy-python-0.2.0/convoy_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-16 10:14:28.000000 convoy-python-0.2.0/convoy_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 10:14:28.000000 convoy-python-0.2.0/convoy_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-16 10:14:28.000000 convoy-python-0.2.0/convoy_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 10:14:28.000000 convoy-python-0.2.0/convoy_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 10:14:28.591794 convoy-python-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-16 10:14:17.000000 convoy-python-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:14:28.591794 convoy-python-0.2.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-05-16 10:14:17.000000 convoy-python-0.2.0/test/test.py
```

### Comparing `convoy-python-0.1.0/LICENSE` & `convoy-python-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `convoy-python-0.1.0/README.md` & `convoy-python-0.2.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -12,43 +12,78 @@
 ```
 
 ## Setup Client
 Next, import the `convoy` module and setup with your auth credentials.
 
 ```python
 from convoy import Convoy
-convoy = Convoy({"api_key":"your_api_key"})
+convoy = Convoy({"api_key":"your_api_key", "project_id": "your_project_id"})
 ```
 The SDK also supports authenticating via Basic Auth by defining your username and password.
 
+In the event you're using a self-hosted convoy instance, you can define the `uri` as part of what is passed into the convoy's constructor.
+
 ```python
-convoy = Convoy({"username":"default", "password":"default"})
+convoy = Convoy({ "api_key": 'your_api_key', "uri": 'self-hosted-instance', "project_id": "your_project_id"})
 ```
 
-In the event you're using a self hosted convoy instance, you can define the url as part of what is passed into convoy's constructor.
+## Usage
+
+### Get all groups
 
 ```python
-convoy = Convoy({ "api_key": 'your_api_key', "uri": 'self-hosted-instance' })
+(response, status) = convoy.group.all({ "perPage": 10, "page": 1 })
 ```
 
-## Usage
+### Create an Endpoint
+
+An endpoint represents a target URL to receive events.
+
+```python
+endpointData = {
+    "url": "https://0d87-102-89-2-172.ngrok.io",
+    "description": "Default Endpoint",
+    "secret": "endpoint-secret",
+    "events": ["*"],
+  }
+
+(response, status) = convoy.endpoint.create({}, endpointData)
+endpoint_id = response["data"]["uid"]
+```
+
+### Sending an Event
+
+To send an event, you'll need the `uid` we created in the earlier section.
 
 ```python
-content, status = convoy.group.all({ "perPage": 10, "page": 1 })
+eventData = {
+    "endpoint_id": endpoint_id,
+    "event_type": "payment.success",
+    "data": {
+      "event": "payment.success",
+      "data": {
+        "status": "Completed",
+        "description": "Transaction Successful",
+        "userID": "test_user_id808",
+      },
+    },
+  }
+
+(response, status) = convoy.event.create({}, eventData)
 ```
 
 ## Testing
 
 ```python
 pytest ./test/test.py
 ```
 
 ## Contributing
 
-Please see [CONTRIBUTING](CONTRIBUTING.md) for details.
+Please see [CONTRIBUTING](CONTRIBUTING.MD) for details.
 
 
 ## Credits
 
 - [Frain](https://github.com/frain-dev)
 
 ## License
```

### Comparing `convoy-python-0.1.0/convoy/api/delivery_attempts.py` & `convoy-python-0.2.0/convoy/api/delivery_attempts.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     Parameters
     ----------
     config : dict of config values
     """
     def __init__(self, config):
         self.client = Client(config)
 
-    def all(self, eventdeliveryId, query):
-        response = self.client.httpGet("/eventdeliveries/%s/deliveryattempts" %  eventdeliveryId, query)
+    def all(self, event_delivery_id, query):
+        response = self.client.http_get("/eventdeliveries/%s/deliveryattempts" %  event_delivery_id, query)
         return response
 
-    def find(self, eventdeliveryId, deliveryAttemptId, query):
-        response = self.client.httpGet("/eventdeliveries/%s/deliveryattempts/%s" %  (eventdeliveryId, deliveryAttemptId), query)
+    def find(self, event_delivery_id, delivery_attempt_id, query):
+        response = self.client.http_get("/eventdeliveries/%s/deliveryattempts/%s" %  (event_delivery_id, delivery_attempt_id), query)
         return response
```

### Comparing `convoy-python-0.1.0/convoy/api/endpoint.py` & `convoy-python-0.2.0/convoy/api/endpoint.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,58 +6,58 @@
     Parameters
     ----------
     config : dict of config values
     """
     def __init__(self, config):
         self.client = Client(config)
 
-    def all(self, appId, query):
-        '''
-        Get all endpoints for an application.
-        '''
-        response = self.client.httpGet("/applications/%s/endpoints" % appId, query)
+    def all(self, query):
+        """
+        Get all endpoints for a project.
+        """
+        response = self.client.http_get("/endpoints", query)
         return response
 
-    def create(self, appId, query, data):
-        '''
+    def create(self, query, data):
+        """
         Create a new endpoint.
         Parameters
         ----------
         data = {
                 "url": "",
                 "description": "",
                 "secret": "",
                 "events": [],
                 }
-        '''
-        response = self.client.httpPost("/applications/%s/endpoints" % appId, query, data)
+        """
+        response = self.client.http_post("/endpoints", query, data)
         return response
 
-    def find(self, appId, endpointId, query):
-        '''
-        Find a particular application.
-        '''
-        response = self.client.httpGet("/applications/%s/endpoints/%s" % (appId, endpointId), query)
+    def find(self, endpoint_id, query):
+        """
+        Find a particular endpoint.
+        """
+        response = self.client.http_get("endpoints/%s" % endpoint_id, query)
         return response
 
-    def update(self, appId, endpointId, query, data):
-        '''
-        Update an application.
+    def update(self, endpoint_id, query, data):
+        """
+        Update an endpoint.
         Parameters
         ---------- 
         data = {
                 "url": "",
                 "description": "",
                 "secret": "",
                 "events": [],
                 }
-        '''
-        response = self.client.httpPut("/applications/%s/endpoints/%s" % (appId, endpointId), query, data)
+        """
+        response = self.client.http_put("/endpoints/%s" % endpoint_id, query, data)
         return response
 
-    def delete(self, appId, endpointId, query, data):
-        '''
-        Delete an application.
-        '''
-        response = self.client.httpDelete("/applications/%s/endpoints/%s" % (appId, endpointId), query, data)
+    def delete(self, endpoint_id, query, data):
+        """
+        Delete an endpoint.
+        """
+        response = self.client.http_delete("/endpoints/%s" % endpoint_id, query, data)
         return response
```

### Comparing `convoy-python-0.1.0/convoy/api/event_delivery.py` & `convoy-python-0.2.0/convoy/api/event_delivery.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,39 +7,39 @@
     ----------
     config : dict of config values
     """
     def __init__(self, config):
         self.client = Client(config)
 
     def all(self, query):
-        '''
+        """
         Get all eventdeliveries.
-        '''
-        response = self.client.httpGet("/eventdeliveries", query)
+        """
+        response = self.client.http_get("/eventdeliveries", query)
         return response
 
     def find(self, id, query):
-        '''
+        """
         Find a particular eventdelivery.    
-        '''
-        response = self.client.httpGet("/eventdeliveries/%s" % id, query)
+        """
+        response = self.client.http_get("/eventdeliveries/%s" % id, query)
         return response
 
     def resend(self, id, query):
-        '''
+        """
         Resend an eventdelivery.    
-        '''
-        response = self.client.httpPut("/eventdeliveries/%s/resend" % id, query, {})
+        """
+        response = self.client.http_put("/eventdeliveries/%s/resend" % id, query, {})
         return response
 
     def batchresend(self, id, query, data):
-        '''
+        """
         Batch resend eventdeliveries.
         Parameters
         ----------
         data = {
                 ids: []
                 }
-        '''
-        response = self.client.httpPut("/eventdeliveries/batchretry" % id, query, data)
+        """
+        response = self.client.http_put("/eventdeliveries/batchretry" % id, query, data)
         return response
```

### Comparing `convoy-python-0.1.0/convoy/api/group.py` & `convoy-python-0.2.0/convoy/api/group.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,22 +7,22 @@
     ----------
     config : dict of config values
     """
     def __init__(self, config):
         self.client = Client(config)
 
     def all(self, query):
-        '''
+        """
         Get all groups.
-        '''
-        response = self.client.httpGet("/groups", query)
+        """
+        response = self.client.http_get("/groups", query)
         return response
 
     def create(self, query, data):
-        '''
+        """
         Create a new group.
         Parameters
         ----------
         data = {
             "name": "",
             "logo_url": "",
             "config": {
@@ -36,27 +36,27 @@
                                 "default": {
                                     "intervalSeconds": int,
                                     "retryLimit": int
                             }
                         },
                     },
                 }
-        '''
-        response = self.client.httpPost("/groups", query, data)
+        """
+        response = self.client.http_post("/groups", query, data)
         return response
 
     def find(self, id, query):
-        '''
+        """
         Find a particular group.    
-        '''
-        response = self.client.httpGet("/groups/%s" % id, query)
+        """
+        response = self.client.http_get("/groups/%s" % id, query)
         return response
 
     def update(self, id, query, data):
-        '''
+        """
         Update a group.
         Parameters
         ---------- 
         data = {
             "name": "",
             "logo_url": "",
             "config": {
@@ -70,18 +70,18 @@
                                 "default": {
                                     "intervalSeconds": int,
                                     "retryLimit": int
                             }
                         },
                     },
                 }
-        '''
-        response = self.client.httpPut("/groups/%s" % id, query, data)
+        """
+        response = self.client.http_put("/groups/%s" % id, query, data)
         return response
 
     def delete(self, id, query, data):
-        '''
+        """
         Delete a group.
-        '''
-        response = self.client.httpDelete("/groups/%s" % id, query, data)
+        """
+        response = self.client.http_delete("/groups/%s" % id, query, data)
         return response
```

### Comparing `convoy-python-0.1.0/convoy/convoy.py` & `convoy-python-0.2.0/convoy/convoy.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from convoy.api import application, delivery_attempts, endpoint, event, event_delivery, group
+from re import sub
+from convoy.api import delivery_attempts, endpoint, event, event_delivery, group, source, subscription
+from convoy.utils import webhook
 
 class Convoy():
     """Initializes the main Convoy Object.
        
     Parameters
     ----------
     config : dict of config values, see example config below;
@@ -15,13 +17,15 @@
         #API Key used for bearer token authentication
         "api_key": "",
         #Convoy self hosted uri
         "uri": ""
     }
     """
     def __init__(self, config):
-        self.applications = application.Application(config)
-        self.deliveryAttempts = delivery_attempts.DeliveryAttempt(config)
+        self.delivery_attempt = delivery_attempts.DeliveryAttempt(config)
         self.endpoint = endpoint.Endpoint(config)
-        self.eventDelivery = event_delivery.EventDelivery(config)
+        self.event_delivery = event_delivery.EventDelivery(config)
         self.event = event.Event(config)
-        self.group = group.Group(config)
+        self.group = group.Group(config)
+        self.source = source.Source(config)
+        self.subscription = subscription.Subscription(config)
+        self.webhook = webhook.Webhook()
```

### Comparing `convoy-python-0.1.0/convoy/data.py` & `convoy-python-0.2.0/convoy/data.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,24 @@
-'''
+"""
 You can use these dict objects to create your own data.
-'''
+"""
 
 Config = {
         #Username used for basic authentication
         "username": "",
         #Password used for basic authentication
         "password": "",
         #API Key used for bearer token authentication
         "api_key": "",
         #Convoy self hosted uri
         "uri": ""
     }
 
-NewApplication = {
-                "name": "",
-                "support_email": "",
-                "secret": ""
-                }
-
-
 NewEvent = {
-            "app_id": "",
+            "endpoint_id": "",
             "event_type": "",
             "data": {
                     "event": "",
                     "data": {},
                 }
             }
```

### Comparing `convoy-python-0.1.0/convoy_python.egg-info/SOURCES.txt` & `convoy-python-0.2.0/convoy_python.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 LICENSE
 README.md
 setup.py
 convoy/__init__.py
 convoy/convoy.py
 convoy/data.py
 convoy/api/__init__.py
-convoy/api/application.py
 convoy/api/delivery_attempts.py
 convoy/api/endpoint.py
 convoy/api/event.py
 convoy/api/event_delivery.py
 convoy/api/group.py
+convoy/api/source.py
+convoy/api/subscription.py
 convoy/client/__init__.py
 convoy/client/client.py
 convoy/utils/__init__.py
 convoy/utils/helpers.py
+convoy/utils/webhook.py
 convoy_python.egg-info/PKG-INFO
 convoy_python.egg-info/SOURCES.txt
 convoy_python.egg-info/dependency_links.txt
 convoy_python.egg-info/requires.txt
 convoy_python.egg-info/top_level.txt
 test/test.py
```

### Comparing `convoy-python-0.1.0/setup.py` & `convoy-python-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 # The text of the README file is used as a description
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="convoy-python",
-    version="0.1.0",
+    version="0.2.0",
     description="Python SDK for Convoy",
     url="https://github.com/frain-dev/convoy-python",
     long_description=README,
     long_description_content_type="text/markdown",
     author="Frain Inc.",
     author_email="info@frain.dev",
     license="MIT",
```

### Comparing `convoy-python-0.1.0/test/test.py` & `convoy-python-0.2.0/test/test.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,26 +2,14 @@
 from convoy.data import *
 from convoy.client import Client
 
 Config["api_key"] = "your-api-key"
 
 cnv = Convoy(Config)
 
-#Application
-def test_application():
-    NewApplication["name"] = "pythonsdktestapp"
-    NewApplication["support_email"] = "testsdk@frain.dev"
-    _, status = cnv.applications.create({"groupID":"449f4d86-e70b-40eb-a733-dadd89d8d3b6"}, NewApplication)
-    assert(status == 201)
-    # response = cnv.applications.all("groupID=449f4d86-e70b-40eb-a733-dadd89d8d3b6")
-    # response = cnv.applications.find("fb05c3c7-2d9c-4e07-95b4-e859c1415385", "groupID=449f4d86-e70b-40eb-a733-dadd89d8d3b6")
-    # UpdateApplication = NewApplication
-    # UpdateApplication["name"] = "sdktest_app"
-    # response = cnv.applications.update("9a3cc2b9-ce09-4dbd-9ea9-594def3dd347", "groupID=449f4d86-e70b-40eb-a733-dadd89d8d3b6", UpdateApplication)
-
 #Endpoint
 def test_endpoint():
     NewEndpoint["url"] = "http://ed0b-102-219-153-85.ngrok.io"
     NewEndpoint["description"] = "testendpoint"
     _, status = cnv.endpoint.create("9a3cc2b9-ce09-4dbd-9ea9-594def3dd347", {"groupID":"449f4d86-e70b-40eb-a733-dadd89d8d3b6"}, NewEndpoint)
     assert(status == 201)
     # response = cnv.endpoint.all("fb05c3c7-2d9c-4e07-95b4-e859c1415385", {"groupID":"449f4d86-e70b-40eb-a733-dadd89d8d3b6"})
@@ -91,10 +79,10 @@
     # response = cnv.group.find("96d04e60-854c-4f7e-9257-be88c15474fd", {"groupID":"449f4d86-e70b-40eb-a733-dadd89d8d3b6"})
     # UpdateGroup = NewGroup
     # UpdateGroup["name"] = "convoypythonsdk"
     # response  = cnv.group.update("f46f780a-4216-4306-b1ba-1c5e0a30086e", {"groupID":"449f4d86-e70b-40eb-a733-dadd89d8d3b6"}, UpdateGroup)
 
 #DeliveryAttempts
 def test_deliverattempts():
-    content, status = cnv.deliveryAttempts.all("6bb26fe3-a3d8-4ea8-aa7c-55bd61caa8be", {"groupID":"449f4d86-e70b-40eb-a733-dadd89d8d3b6"})
+    content, status = cnv.delivery_attempt.all("6bb26fe3-a3d8-4ea8-aa7c-55bd61caa8be", {"groupID":"449f4d86-e70b-40eb-a733-dadd89d8d3b6"})
     assert(status == 404)
     # response  = cnv.deliveryAttempts.find("dfa306bd-ef49-4528-8175-a363e01c4623", "1d1e3b81-3a33-472b-9380-a8c8afa06252", {})
```

