# Comparing `tmp/pyonfleet-1.3.1.tar.gz` & `tmp/pyonfleet-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyonfleet-1.3.1.tar", last modified: Wed Jul  6 17:01:10 2022, max compression
+gzip compressed data, was "pyonfleet-1.4.0.tar", last modified: Tue May 16 01:58:21 2023, max compression
```

## Comparing `pyonfleet-1.3.1.tar` & `pyonfleet-1.4.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-06 17:01:10.347860 pyonfleet-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-07-06 17:00:54.000000 pyonfleet-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-07-06 17:00:54.000000 pyonfleet-1.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     9752 2022-07-06 17:01:10.343860 pyonfleet-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     9711 2022-07-06 17:00:54.000000 pyonfleet-1.3.1/README.es.md
--rw-r--r--   0 runner    (1001) docker     (121)     9338 2022-07-06 17:00:54.000000 pyonfleet-1.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     9125 2022-07-06 17:00:54.000000 pyonfleet-1.3.1/README.zh-tw.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-06 17:01:10.343860 pyonfleet-1.3.1/onfleet/
--rw-r--r--   0 runner    (1001) docker     (121)      232 2022-07-06 17:00:54.000000 pyonfleet-1.3.1/onfleet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-07-06 17:00:54.000000 pyonfleet-1.3.1/onfleet/_meta.py
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-07-06 17:00:54.000000 pyonfleet-1.3.1/onfleet/config.py
--rw-r--r--   0 runner    (1001) docker     (121)      877 2022-07-06 17:00:54.000000 pyonfleet-1.3.1/onfleet/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)      540 2022-07-06 17:00:54.000000 pyonfleet-1.3.1/onfleet/error.py
--rw-r--r--   0 runner    (1001) docker     (121)     3689 2022-07-06 17:00:54.000000 pyonfleet-1.3.1/onfleet/onfleet.py
--rw-r--r--   0 runner    (1001) docker     (121)     5053 2022-07-06 17:00:54.000000 pyonfleet-1.3.1/onfleet/request.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-06 17:01:10.343860 pyonfleet-1.3.1/pyonfleet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9752 2022-07-06 17:01:10.000000 pyonfleet-1.3.1/pyonfleet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      399 2022-07-06 17:01:10.000000 pyonfleet-1.3.1/pyonfleet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-06 17:01:10.000000 pyonfleet-1.3.1/pyonfleet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-07-06 17:01:10.000000 pyonfleet-1.3.1/pyonfleet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-07-06 17:01:10.000000 pyonfleet-1.3.1/pyonfleet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-07-06 17:00:54.000000 pyonfleet-1.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-06 17:01:10.347860 pyonfleet-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1148 2022-07-06 17:00:54.000000 pyonfleet-1.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-06 17:01:10.343860 pyonfleet-1.3.1/test/
--rw-r--r--   0 runner    (1001) docker     (121)     5075 2022-07-06 17:00:54.000000 pyonfleet-1.3.1/test/test_onfleet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:58:21.673183 pyonfleet-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-16 01:58:10.000000 pyonfleet-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-16 01:58:10.000000 pyonfleet-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10103 2023-05-16 01:58:21.673183 pyonfleet-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9712 2023-05-16 01:58:10.000000 pyonfleet-1.4.0/README.es.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9690 2023-05-16 01:58:10.000000 pyonfleet-1.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9126 2023-05-16 01:58:10.000000 pyonfleet-1.4.0/README.zh-tw.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:58:21.669183 pyonfleet-1.4.0/onfleet/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-16 01:58:10.000000 pyonfleet-1.4.0/onfleet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-16 01:58:10.000000 pyonfleet-1.4.0/onfleet/_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-16 01:58:10.000000 pyonfleet-1.4.0/onfleet/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-16 01:58:10.000000 pyonfleet-1.4.0/onfleet/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-16 01:58:10.000000 pyonfleet-1.4.0/onfleet/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-05-16 01:58:10.000000 pyonfleet-1.4.0/onfleet/onfleet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-05-16 01:58:10.000000 pyonfleet-1.4.0/onfleet/request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:58:21.669183 pyonfleet-1.4.0/pyonfleet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10103 2023-05-16 01:58:21.000000 pyonfleet-1.4.0/pyonfleet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-16 01:58:21.000000 pyonfleet-1.4.0/pyonfleet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 01:58:21.000000 pyonfleet-1.4.0/pyonfleet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-16 01:58:21.000000 pyonfleet-1.4.0/pyonfleet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 01:58:21.000000 pyonfleet-1.4.0/pyonfleet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-16 01:58:10.000000 pyonfleet-1.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 01:58:21.673183 pyonfleet-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-16 01:58:10.000000 pyonfleet-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:58:21.673183 pyonfleet-1.4.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-05-16 01:58:10.000000 pyonfleet-1.4.0/test/test_onfleet.py
```

### Comparing `pyonfleet-1.3.1/LICENSE` & `pyonfleet-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyonfleet-1.3.1/PKG-INFO` & `pyonfleet-1.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyonfleet
-Version: 1.3.1
+Version: 1.4.0
 Summary: Onfleet's Python API Wrapper Package
 Home-page: http://docs.onfleet.com
 Author: James Li
 Author-email: support@onfleet.com
 License: LICENSE
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
@@ -77,14 +77,20 @@
 # Option 1 - Recommended
 onfleet_api = Onfleet()  # Using the .auth.json file
 
 # Option 2
 onfleet_api = Onfleet(api_key="<your_api_key>")  # Without the .auth.json file
 ```
 
+Another optional parameter for `Onfleet` is `custom_headers` where you can pass in headers to be applied to all requests. For example:
+
+```python
+onfleet_api = Onfleet(custom_headers={"<header_name>": "<header_value>"})
+```
+
 Once the `Onfleet` object is created, you will get access to all the API endpoints as documented in the [Onfleet API documentation](https://docs.onfleet.com/).
 
 ### Unit testing using Docker
 
 `docker-compose up --build`
 
 ### Throttling
@@ -95,23 +101,23 @@
 
 ### Supported CRUD operations 
 Here are the operations available for each entity:
 
 | Entity | GET | POST | PUT | DELETE |
 | :-: | :-: | :-: | :-: | :-: |
 | [Admins/Administrators](https://docs.onfleet.com/reference#administrators) | get() | create(body={})<br />matchMetadata(body={}) | update(id, body={}) | deleteOne(id) |
-| [Containers](https://docs.onfleet.com/reference#containers) | get(workers=id)<br />get(teams=id)<br />get(organizations=id) | x | update(id, body={}) | x |
-| [Destinations](https://docs.onfleet.com/reference#destinations) | get(id) | create(body={})<br />matchMetadata(body={}) | x | x |
-| [Hubs](https://docs.onfleet.com/reference#hubs) | get() | create(body={}) | update(id, body={}) | x |
-| [Organization](https://docs.onfleet.com/reference#organizations) | get()<br />get(id) | x | insertTask(id, body={}) | x |
-| [Recipients](https://docs.onfleet.com/reference#recipients) | get(id)<br />get(name='')<br />get(phone='') | create(body={})<br />matchMetadata(body={}) | update(id, body={}) | x |
-| [Tasks](https://docs.onfleet.com/reference#tasks) | get(queryParams={})<br />get(id)<br />get(shortId=id) | create(body={})<br />clone(id)<br />forceComplete(id)<br />batch(body={})<br />autoAssign(body={})<br />matchMetadata(body={}) | update(id, body={}) | deleteOne(id) |
-| [Teams](https://docs.onfleet.com/reference#teams) | get()<br />get(id)<br />getWorkerEta(id, queryParams={})<br />getTasks(id, queryParams={}) | create(body={})<br />autoDispatch(id, body={}) | update(id, body={})<br />insertTask(id, body={}) | deleteOne(id) |
-| [Webhooks](https://docs.onfleet.com/reference#webhooks) | get() | create(body={}) | x | deleteOne(id) |
-| [Workers](https://docs.onfleet.com/reference#workers) | get()<br />get(id)<br />get(queryParams={})<br />getByLocation(queryParams={})<br />getSchedule(id)<br />getTasks(id, queryParams={}) | create(body={})<br />setSchedule(id, body={})<br />matchMetadata(body={}) | update(id, body={})<br />insertTask(id, body={}) | deleteOne(id) |
+| [Containers](https://docs.onfleet.com/reference/containers) | get(workers=id)<br />get(teams=id)<br />get(organizations=id) | x | update(id, body={}) | x |
+| [Destinations](https://docs.onfleet.com/reference/destinations) | get(id) | create(body={})<br />matchMetadata(body={}) | x | x |
+| [Hubs](https://docs.onfleet.com/reference/hubs) | get() | create(body={}) | update(id, body={}) | x |
+| [Organization](https://docs.onfleet.com/reference/organizations) | get()<br />get(id) | x | insertTask(id, body={}) | x |
+| [Recipients](https://docs.onfleet.com/reference/recipients) | get(id)<br />get(name='')<br />get(phone='') | create(body={})<br />matchMetadata(body={}) | update(id, body={}) | x |
+| [Tasks](https://docs.onfleet.com/reference/tasks) | get(queryParams={})<br />get(id)<br />get(shortId=id) | create(body={})<br />clone(id)<br />forceComplete(id)<br />batch(body={})<br />autoAssign(body={})<br />matchMetadata(body={}) | update(id, body={}) | deleteOne(id) |
+| [Teams](https://docs.onfleet.com/reference/teams) | get()<br />get(id)<br />getWorkerEta(id, queryParams={})<br />getTasks(id, queryParams={}) | create(body={})<br />autoDispatch(id, body={}) | update(id, body={})<br />insertTask(id, body={}) | deleteOne(id) |
+| [Webhooks](https://docs.onfleet.com/reference/webhooks) | get() | create(body={}) | x | deleteOne(id) |
+| [Workers](https://docs.onfleet.com/reference/workers) | get()<br />get(id)<br />get(queryParams={})<br />getByLocation(queryParams={})<br />getSchedule(id)<br />getTasks(id, queryParams={}) | create(body={})<br />setSchedule(id, body={})<br />matchMetadata(body={}) | update(id, body={})<br />insertTask(id, body={}) | deleteOne(id) |
 
 #### GET Requests
 To get all the documents within an endpoint:
 ```python
 get()
 ```
 
@@ -147,14 +153,16 @@
 onfleet_api.recipients.get(name="<name>")
 
 onfleet_api.containers.get(workers="<worker_ID>")
 onfleet_api.containers.get(teams="<team_ID>")
 onfleet_api.containers.get(organizations="<organization_ID>")
 ```
 
+**Note:** don't use Python-style `True` and `False` for boolean values - supply these as strings like `"true"` or `"false"`.
+
 To get a driver by location, use the `getByLocation` function:
 ```python
 getByLocation(queryParams="<location_params>")
 ```
 
 ##### Examples of `getByLocation`
 ```python
```

### Comparing `pyonfleet-1.3.1/README.es.md` & `pyonfleet-1.4.0/README.es.md`

 * *Files 0% similar despite different names*

```diff
@@ -81,24 +81,24 @@
 Las respuestas de esta librería son instancias de [Response](https://2.python-requests.org//en/master/api/#requests.Response) de la librería `requests`.
 
 ### Operaciones CRUD soportadas
 Estas son las operaciones disponibles para cada endpoint:
 
 | Entity | GET | POST | PUT | DELETE |
 | :-: | :-: | :-: | :-: | :-: |
-| [Admins/Administrators](https://docs.onfleet.com/reference#administrators) | get() | create(body={})<br />matchMetadata(body={}) | update(id, body={}) | deleteOne(id) |
-| [Containers](https://docs.onfleet.com/reference#containers) | get(workers=id)<br />get(teams=id)<br />get(organizations=id) | x | update(id, body={}) | x |
-| [Destinations](https://docs.onfleet.com/reference#destinations) | get(id) | create(body={})<br />matchMetadata(body={}) | x | x |
-| [Hubs](https://docs.onfleet.com/reference#hubs) | get() | create(body={}) | update(id, body={}) | x |
-| [Organization](https://docs.onfleet.com/reference#organizations) | get()<br />get(id) | x | insertTask(id, body={}) | x |
-| [Recipients](https://docs.onfleet.com/reference#recipients) | get(id)<br />get(name='')<br />get(phone='') | create(body={})<br />matchMetadata(body={}) | update(id, body={}) | x |
-| [Tasks](https://docs.onfleet.com/reference#tasks) | get(queryParams={})<br />get(id)<br />get(shortId=id) | create(body={})<br />clone(id)<br />forceComplete(id)<br />batch(body={})<br />autoAssign(body={})<br />matchMetadata(body={}) | update(id, body={}) | deleteOne(id) |
-| [Teams](https://docs.onfleet.com/reference#teams) | get()<br />get(id)<br />getWorkerEta(id, queryParams={})<br />getTasks(id, queryParams={}) | create(body={})<br />autoDispatch(id, body={}) | update(id, body={})<br />insertTask(id, body={}) | deleteOne(id) |
-| [Webhooks](https://docs.onfleet.com/reference#webhooks) | get() | create(body={}) | x | deleteOne(id) |
-| [Workers](https://docs.onfleet.com/reference#workers) | get()<br />get(id)<br />get(queryParams={})<br />getByLocation(queryParams={})<br />getSchedule(id)<br />getTasks(id, queryParams={}) | create(body={})<br />setSchedule(id, body={})<br />matchMetadata(body={}) | update(id, body={})<br />insertTask(id, body={}) | deleteOne(id) |
+| [Admins/Administrators](https://docs.onfleet.com/reference/administrators) | get() | create(body={})<br />matchMetadata(body={}) | update(id, body={}) | deleteOne(id) |
+| [Containers](https://docs.onfleet.com/reference/containers) | get(workers=id)<br />get(teams=id)<br />get(organizations=id) | x | update(id, body={}) | x |
+| [Destinations](https://docs.onfleet.com/reference/destinations) | get(id) | create(body={})<br />matchMetadata(body={}) | x | x |
+| [Hubs](https://docs.onfleet.com/reference/hubs) | get() | create(body={}) | update(id, body={}) | x |
+| [Organization](https://docs.onfleet.com/reference/organizations) | get()<br />get(id) | x | insertTask(id, body={}) | x |
+| [Recipients](https://docs.onfleet.com/reference/recipients) | get(id)<br />get(name='')<br />get(phone='') | create(body={})<br />matchMetadata(body={}) | update(id, body={}) | x |
+| [Tasks](https://docs.onfleet.com/reference/tasks) | get(queryParams={})<br />get(id)<br />get(shortId=id) | create(body={})<br />clone(id)<br />forceComplete(id)<br />batch(body={})<br />autoAssign(body={})<br />matchMetadata(body={}) | update(id, body={}) | deleteOne(id) |
+| [Teams](https://docs.onfleet.com/reference/teams) | get()<br />get(id)<br />getWorkerEta(id, queryParams={})<br />getTasks(id, queryParams={}) | create(body={})<br />autoDispatch(id, body={}) | update(id, body={})<br />insertTask(id, body={}) | deleteOne(id) |
+| [Webhooks](https://docs.onfleet.com/reference/webhooks) | get() | create(body={}) | x | deleteOne(id) |
+| [Workers](https://docs.onfleet.com/reference/workers) | get()<br />get(id)<br />get(queryParams={})<br />getByLocation(queryParams={})<br />getSchedule(id)<br />getTasks(id, queryParams={}) | create(body={})<br />setSchedule(id, body={})<br />matchMetadata(body={}) | update(id, body={})<br />insertTask(id, body={}) | deleteOne(id) |
 
 #### Peticiones GET
 Para obtener todos los elementos disponibles en un recurso:
 ```python
 get()
 ```
 
@@ -222,8 +222,8 @@
 ```
 
 ##### Ejemplos de `deleteOne()`
 ```python
 onfleet_api.workers.deleteOne(id="<24_digit_ID>")
 ```
 
-*Ir al [inicio](#onfleet-python-wrapper)*.
+*Ir al [inicio](#onfleet-python-wrapper)*.
```

### Comparing `pyonfleet-1.3.1/README.md` & `pyonfleet-1.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -63,14 +63,20 @@
 # Option 1 - Recommended
 onfleet_api = Onfleet()  # Using the .auth.json file
 
 # Option 2
 onfleet_api = Onfleet(api_key="<your_api_key>")  # Without the .auth.json file
 ```
 
+Another optional parameter for `Onfleet` is `custom_headers` where you can pass in headers to be applied to all requests. For example:
+
+```python
+onfleet_api = Onfleet(custom_headers={"<header_name>": "<header_value>"})
+```
+
 Once the `Onfleet` object is created, you will get access to all the API endpoints as documented in the [Onfleet API documentation](https://docs.onfleet.com/).
 
 ### Unit testing using Docker
 
 `docker-compose up --build`
 
 ### Throttling
@@ -81,23 +87,23 @@
 
 ### Supported CRUD operations 
 Here are the operations available for each entity:
 
 | Entity | GET | POST | PUT | DELETE |
 | :-: | :-: | :-: | :-: | :-: |
 | [Admins/Administrators](https://docs.onfleet.com/reference#administrators) | get() | create(body={})<br />matchMetadata(body={}) | update(id, body={}) | deleteOne(id) |
-| [Containers](https://docs.onfleet.com/reference#containers) | get(workers=id)<br />get(teams=id)<br />get(organizations=id) | x | update(id, body={}) | x |
-| [Destinations](https://docs.onfleet.com/reference#destinations) | get(id) | create(body={})<br />matchMetadata(body={}) | x | x |
-| [Hubs](https://docs.onfleet.com/reference#hubs) | get() | create(body={}) | update(id, body={}) | x |
-| [Organization](https://docs.onfleet.com/reference#organizations) | get()<br />get(id) | x | insertTask(id, body={}) | x |
-| [Recipients](https://docs.onfleet.com/reference#recipients) | get(id)<br />get(name='')<br />get(phone='') | create(body={})<br />matchMetadata(body={}) | update(id, body={}) | x |
-| [Tasks](https://docs.onfleet.com/reference#tasks) | get(queryParams={})<br />get(id)<br />get(shortId=id) | create(body={})<br />clone(id)<br />forceComplete(id)<br />batch(body={})<br />autoAssign(body={})<br />matchMetadata(body={}) | update(id, body={}) | deleteOne(id) |
-| [Teams](https://docs.onfleet.com/reference#teams) | get()<br />get(id)<br />getWorkerEta(id, queryParams={})<br />getTasks(id, queryParams={}) | create(body={})<br />autoDispatch(id, body={}) | update(id, body={})<br />insertTask(id, body={}) | deleteOne(id) |
-| [Webhooks](https://docs.onfleet.com/reference#webhooks) | get() | create(body={}) | x | deleteOne(id) |
-| [Workers](https://docs.onfleet.com/reference#workers) | get()<br />get(id)<br />get(queryParams={})<br />getByLocation(queryParams={})<br />getSchedule(id)<br />getTasks(id, queryParams={}) | create(body={})<br />setSchedule(id, body={})<br />matchMetadata(body={}) | update(id, body={})<br />insertTask(id, body={}) | deleteOne(id) |
+| [Containers](https://docs.onfleet.com/reference/containers) | get(workers=id)<br />get(teams=id)<br />get(organizations=id) | x | update(id, body={}) | x |
+| [Destinations](https://docs.onfleet.com/reference/destinations) | get(id) | create(body={})<br />matchMetadata(body={}) | x | x |
+| [Hubs](https://docs.onfleet.com/reference/hubs) | get() | create(body={}) | update(id, body={}) | x |
+| [Organization](https://docs.onfleet.com/reference/organizations) | get()<br />get(id) | x | insertTask(id, body={}) | x |
+| [Recipients](https://docs.onfleet.com/reference/recipients) | get(id)<br />get(name='')<br />get(phone='') | create(body={})<br />matchMetadata(body={}) | update(id, body={}) | x |
+| [Tasks](https://docs.onfleet.com/reference/tasks) | get(queryParams={})<br />get(id)<br />get(shortId=id) | create(body={})<br />clone(id)<br />forceComplete(id)<br />batch(body={})<br />autoAssign(body={})<br />matchMetadata(body={}) | update(id, body={}) | deleteOne(id) |
+| [Teams](https://docs.onfleet.com/reference/teams) | get()<br />get(id)<br />getWorkerEta(id, queryParams={})<br />getTasks(id, queryParams={}) | create(body={})<br />autoDispatch(id, body={}) | update(id, body={})<br />insertTask(id, body={}) | deleteOne(id) |
+| [Webhooks](https://docs.onfleet.com/reference/webhooks) | get() | create(body={}) | x | deleteOne(id) |
+| [Workers](https://docs.onfleet.com/reference/workers) | get()<br />get(id)<br />get(queryParams={})<br />getByLocation(queryParams={})<br />getSchedule(id)<br />getTasks(id, queryParams={}) | create(body={})<br />setSchedule(id, body={})<br />matchMetadata(body={}) | update(id, body={})<br />insertTask(id, body={}) | deleteOne(id) |
 
 #### GET Requests
 To get all the documents within an endpoint:
 ```python
 get()
 ```
 
@@ -133,14 +139,16 @@
 onfleet_api.recipients.get(name="<name>")
 
 onfleet_api.containers.get(workers="<worker_ID>")
 onfleet_api.containers.get(teams="<team_ID>")
 onfleet_api.containers.get(organizations="<organization_ID>")
 ```
 
+**Note:** don't use Python-style `True` and `False` for boolean values - supply these as strings like `"true"` or `"false"`.
+
 To get a driver by location, use the `getByLocation` function:
 ```python
 getByLocation(queryParams="<location_params>")
 ```
 
 ##### Examples of `getByLocation`
 ```python
@@ -221,8 +229,8 @@
 ```
 
 ##### Examples of `deleteOne()`
 ```python
 onfleet_api.workers.deleteOne(id="<24_digit_ID>")
 ```
 
-*Go to [top](#onfleet-python-wrapper)*.
+*Go to [top](#onfleet-python-wrapper)*.
```

### Comparing `pyonfleet-1.3.1/README.zh-tw.md` & `pyonfleet-1.4.0/README.zh-tw.md`

 * *Files 1% similar despite different names*

```diff
@@ -79,22 +79,22 @@
 ### 支援的CRUD操作
 下面為各entity所支援的函式列表：
 
 | Entity | GET | POST | PUT | DELETE |
 | :-: | :-: | :-: | :-: | :-: |
 | [Admins/Administrators](https://docs.onfleet.com/reference#administrators) | get() | create(body={})<br />matchMetadata(body={}) | update(id, body={}) | deleteOne(id) |
 | [Containers](https://docs.onfleet.com/reference#containers) | get(workers=id)<br />get(teams=id)<br />get(organizations=id) | x | update(id, body={}) | x |
-| [Destinations](https://docs.onfleet.com/reference#destinations) | get(id) | create(body={})<br />matchMetadata(body={}) | x | x |
-| [Hubs](https://docs.onfleet.com/reference#hubs) | get() | create(body={}) | update(id, body={}) | x |
-| [Organization](https://docs.onfleet.com/reference#organizations) | get()<br />get(id) | x | insertTask(id, body={}) | x |
-| [Recipients](https://docs.onfleet.com/reference#recipients) | get(id)<br />get(name='')<br />get(phone='') | create(body={})<br />matchMetadata(body={}) | update(id, body={}) | x |
-| [Tasks](https://docs.onfleet.com/reference#tasks) | get(queryParams={})<br />get(id)<br />get(shortId=id) | create(body={})<br />clone(id)<br />forceComplete(id)<br />batch(body={})<br />autoAssign(body={})<br />matchMetadata(body={}) | update(id, body={}) | deleteOne(id) |
-| [Teams](https://docs.onfleet.com/reference#teams) | get()<br />get(id)<br />getWorkerEta(id, queryParams={})<br />getTasks(id, queryParams={}) | create(body={})<br />autoDispatch(id, body={}) | update(id, body={})<br />insertTask(id, body={}) | deleteOne(id) |
-| [Webhooks](https://docs.onfleet.com/reference#webhooks) | get() | create(body={}) | x | deleteOne(id) |
-| [Workers](https://docs.onfleet.com/reference#workers) | get()<br />get(id)<br />get(queryParams={})<br />getByLocation(queryParams={})<br />getSchedule(id)<br />getTasks(id, queryParams={}) | create(body={})<br />setSchedule(id, body={})<br />matchMetadata(body={}) | update(id, body={})<br />insertTask(id, body={}) | deleteOne(id) |
+| [Destinations](https://docs.onfleet.com/reference/destinations) | get(id) | create(body={})<br />matchMetadata(body={}) | x | x |
+| [Hubs](https://docs.onfleet.com/reference/hubs) | get() | create(body={}) | update(id, body={}) | x |
+| [Organization](https://docs.onfleet.com/reference/organizations) | get()<br />get(id) | x | insertTask(id, body={}) | x |
+| [Recipients](https://docs.onfleet.com/reference/recipients) | get(id)<br />get(name='')<br />get(phone='') | create(body={})<br />matchMetadata(body={}) | update(id, body={}) | x |
+| [Tasks](https://docs.onfleet.com/reference/tasks) | get(queryParams={})<br />get(id)<br />get(shortId=id) | create(body={})<br />clone(id)<br />forceComplete(id)<br />batch(body={})<br />autoAssign(body={})<br />matchMetadata(body={}) | update(id, body={}) | deleteOne(id) |
+| [Teams](https://docs.onfleet.com/reference/teams) | get()<br />get(id)<br />getWorkerEta(id, queryParams={})<br />getTasks(id, queryParams={}) | create(body={})<br />autoDispatch(id, body={}) | update(id, body={})<br />insertTask(id, body={}) | deleteOne(id) |
+| [Webhooks](https://docs.onfleet.com/reference/webhooks) | get() | create(body={}) | x | deleteOne(id) |
+| [Workers](https://docs.onfleet.com/reference/workers) | get()<br />get(id)<br />get(queryParams={})<br />getByLocation(queryParams={})<br />getSchedule(id)<br />getTasks(id, queryParams={}) | create(body={})<br />setSchedule(id, body={})<br />matchMetadata(body={}) | update(id, body={})<br />insertTask(id, body={}) | deleteOne(id) |
 
 #### GET 請求
 展示所有資源的指令如下：
 ```python
 get()
 ```
 
@@ -199,8 +199,8 @@
 ```
 
 ##### 使用`deleteOne`刪除指定資源的範例
 ```python
 onfleet_api.workers.deleteOne(id="<24_digit_ID>")
 ```
 
-*返回[頂端](#onfleet-python-wrapper)*。
+*返回[頂端](#onfleet-python-wrapper)*。
```

### Comparing `pyonfleet-1.3.1/onfleet/endpoint.py` & `pyonfleet-1.4.0/onfleet/endpoint.py`

 * *Files identical despite different names*

### Comparing `pyonfleet-1.3.1/onfleet/error.py` & `pyonfleet-1.4.0/onfleet/error.py`

 * *Files identical despite different names*

### Comparing `pyonfleet-1.3.1/onfleet/onfleet.py` & `pyonfleet-1.4.0/onfleet/onfleet.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,19 +61,22 @@
     workers.getTasks = Request('GET', '/workers/:workerId/tasks', _session)
     workers.setSchedule = Request('POST', '/workers/:workerId/schedule', _session)
     workers.matchMetadata = Request('POST', '/workers/metadata', _session)
     workers.insertTask = Request('PUT', '/containers/workers/:taskId', _session)
 
     webhooks = Endpoint('webhooks', ('GET', 'POST', 'DELETE'), _session)
 
-    def __init__(self, api_key=None):
+    def __init__(self, api_key=None, custom_headers={}):
         # Looking up local authentication JSON if no api_key was passed
         if not api_key:
             if os.path.isfile(".auth.json"):
                 with open(".auth.json") as json_secret_file:
                     local_secret = json.load(json_secret_file)
                     api_key = local_secret.get('API_KEY')
         self._session.auth = (api_key, '')  # Username, password
+        # Apply custom headers to all requests if given
+        if bool(custom_headers):
+            self._session.headers.update(custom_headers)
 
     def auth_test(self):
         response = self._session.get(f'{API_BASE_URL}/auth/test')
         return response.json()
```

### Comparing `pyonfleet-1.3.1/onfleet/request.py` & `pyonfleet-1.4.0/onfleet/request.py`

 * *Files identical despite different names*

### Comparing `pyonfleet-1.3.1/pyonfleet.egg-info/PKG-INFO` & `pyonfleet-1.4.0/pyonfleet.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyonfleet
-Version: 1.3.1
+Version: 1.4.0
 Summary: Onfleet's Python API Wrapper Package
 Home-page: http://docs.onfleet.com
 Author: James Li
 Author-email: support@onfleet.com
 License: LICENSE
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
@@ -77,14 +77,20 @@
 # Option 1 - Recommended
 onfleet_api = Onfleet()  # Using the .auth.json file
 
 # Option 2
 onfleet_api = Onfleet(api_key="<your_api_key>")  # Without the .auth.json file
 ```
 
+Another optional parameter for `Onfleet` is `custom_headers` where you can pass in headers to be applied to all requests. For example:
+
+```python
+onfleet_api = Onfleet(custom_headers={"<header_name>": "<header_value>"})
+```
+
 Once the `Onfleet` object is created, you will get access to all the API endpoints as documented in the [Onfleet API documentation](https://docs.onfleet.com/).
 
 ### Unit testing using Docker
 
 `docker-compose up --build`
 
 ### Throttling
@@ -95,23 +101,23 @@
 
 ### Supported CRUD operations 
 Here are the operations available for each entity:
 
 | Entity | GET | POST | PUT | DELETE |
 | :-: | :-: | :-: | :-: | :-: |
 | [Admins/Administrators](https://docs.onfleet.com/reference#administrators) | get() | create(body={})<br />matchMetadata(body={}) | update(id, body={}) | deleteOne(id) |
-| [Containers](https://docs.onfleet.com/reference#containers) | get(workers=id)<br />get(teams=id)<br />get(organizations=id) | x | update(id, body={}) | x |
-| [Destinations](https://docs.onfleet.com/reference#destinations) | get(id) | create(body={})<br />matchMetadata(body={}) | x | x |
-| [Hubs](https://docs.onfleet.com/reference#hubs) | get() | create(body={}) | update(id, body={}) | x |
-| [Organization](https://docs.onfleet.com/reference#organizations) | get()<br />get(id) | x | insertTask(id, body={}) | x |
-| [Recipients](https://docs.onfleet.com/reference#recipients) | get(id)<br />get(name='')<br />get(phone='') | create(body={})<br />matchMetadata(body={}) | update(id, body={}) | x |
-| [Tasks](https://docs.onfleet.com/reference#tasks) | get(queryParams={})<br />get(id)<br />get(shortId=id) | create(body={})<br />clone(id)<br />forceComplete(id)<br />batch(body={})<br />autoAssign(body={})<br />matchMetadata(body={}) | update(id, body={}) | deleteOne(id) |
-| [Teams](https://docs.onfleet.com/reference#teams) | get()<br />get(id)<br />getWorkerEta(id, queryParams={})<br />getTasks(id, queryParams={}) | create(body={})<br />autoDispatch(id, body={}) | update(id, body={})<br />insertTask(id, body={}) | deleteOne(id) |
-| [Webhooks](https://docs.onfleet.com/reference#webhooks) | get() | create(body={}) | x | deleteOne(id) |
-| [Workers](https://docs.onfleet.com/reference#workers) | get()<br />get(id)<br />get(queryParams={})<br />getByLocation(queryParams={})<br />getSchedule(id)<br />getTasks(id, queryParams={}) | create(body={})<br />setSchedule(id, body={})<br />matchMetadata(body={}) | update(id, body={})<br />insertTask(id, body={}) | deleteOne(id) |
+| [Containers](https://docs.onfleet.com/reference/containers) | get(workers=id)<br />get(teams=id)<br />get(organizations=id) | x | update(id, body={}) | x |
+| [Destinations](https://docs.onfleet.com/reference/destinations) | get(id) | create(body={})<br />matchMetadata(body={}) | x | x |
+| [Hubs](https://docs.onfleet.com/reference/hubs) | get() | create(body={}) | update(id, body={}) | x |
+| [Organization](https://docs.onfleet.com/reference/organizations) | get()<br />get(id) | x | insertTask(id, body={}) | x |
+| [Recipients](https://docs.onfleet.com/reference/recipients) | get(id)<br />get(name='')<br />get(phone='') | create(body={})<br />matchMetadata(body={}) | update(id, body={}) | x |
+| [Tasks](https://docs.onfleet.com/reference/tasks) | get(queryParams={})<br />get(id)<br />get(shortId=id) | create(body={})<br />clone(id)<br />forceComplete(id)<br />batch(body={})<br />autoAssign(body={})<br />matchMetadata(body={}) | update(id, body={}) | deleteOne(id) |
+| [Teams](https://docs.onfleet.com/reference/teams) | get()<br />get(id)<br />getWorkerEta(id, queryParams={})<br />getTasks(id, queryParams={}) | create(body={})<br />autoDispatch(id, body={}) | update(id, body={})<br />insertTask(id, body={}) | deleteOne(id) |
+| [Webhooks](https://docs.onfleet.com/reference/webhooks) | get() | create(body={}) | x | deleteOne(id) |
+| [Workers](https://docs.onfleet.com/reference/workers) | get()<br />get(id)<br />get(queryParams={})<br />getByLocation(queryParams={})<br />getSchedule(id)<br />getTasks(id, queryParams={}) | create(body={})<br />setSchedule(id, body={})<br />matchMetadata(body={}) | update(id, body={})<br />insertTask(id, body={}) | deleteOne(id) |
 
 #### GET Requests
 To get all the documents within an endpoint:
 ```python
 get()
 ```
 
@@ -147,14 +153,16 @@
 onfleet_api.recipients.get(name="<name>")
 
 onfleet_api.containers.get(workers="<worker_ID>")
 onfleet_api.containers.get(teams="<team_ID>")
 onfleet_api.containers.get(organizations="<organization_ID>")
 ```
 
+**Note:** don't use Python-style `True` and `False` for boolean values - supply these as strings like `"true"` or `"false"`.
+
 To get a driver by location, use the `getByLocation` function:
 ```python
 getByLocation(queryParams="<location_params>")
 ```
 
 ##### Examples of `getByLocation`
 ```python
```

### Comparing `pyonfleet-1.3.1/setup.py` & `pyonfleet-1.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `pyonfleet-1.3.1/test/test_onfleet.py` & `pyonfleet-1.4.0/test/test_onfleet.py`

 * *Files identical despite different names*

