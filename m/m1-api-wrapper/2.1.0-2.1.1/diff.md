# Comparing `tmp/m1_api_wrapper-2.1.0.tar.gz` & `tmp/m1_api_wrapper-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m1_api_wrapper-2.1.0.tar", last modified: Fri Jan 14 23:57:10 2022, max compression
+gzip compressed data, was "m1_api_wrapper-2.1.1.tar", last modified: Tue May 16 17:28:46 2023, max compression
```

## Comparing `m1_api_wrapper-2.1.0.tar` & `m1_api_wrapper-2.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-14 23:57:10.914155 m1_api_wrapper-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-01-14 23:56:52.000000 m1_api_wrapper-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     7551 2022-01-14 23:57:10.914155 m1_api_wrapper-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7213 2022-01-14 23:56:52.000000 m1_api_wrapper-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-14 23:57:10.914155 m1_api_wrapper-2.1.0/m1_api_wrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7551 2022-01-14 23:57:10.000000 m1_api_wrapper-2.1.0/m1_api_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      342 2022-01-14 23:57:10.000000 m1_api_wrapper-2.1.0/m1_api_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-14 23:57:10.000000 m1_api_wrapper-2.1.0/m1_api_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-01-14 23:57:10.000000 m1_api_wrapper-2.1.0/m1_api_wrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-01-14 23:57:10.000000 m1_api_wrapper-2.1.0/m1_api_wrapper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-14 23:57:10.914155 m1_api_wrapper-2.1.0/m1wrapper/
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-01-14 23:56:52.000000 m1_api_wrapper-2.1.0/m1wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      312 2022-01-14 23:56:52.000000 m1_api_wrapper-2.1.0/m1wrapper/config.py
--rw-r--r--   0 runner    (1001) docker     (121)      515 2022-01-14 23:56:52.000000 m1_api_wrapper-2.1.0/m1wrapper/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     3958 2022-01-14 23:56:52.000000 m1_api_wrapper-2.1.0/m1wrapper/m1wrapper.py
--rw-r--r--   0 runner    (1001) docker     (121)     5416 2022-01-14 23:56:52.000000 m1_api_wrapper-2.1.0/m1wrapper/search.py
--rw-r--r--   0 runner    (1001) docker     (121)     1308 2022-01-14 23:56:52.000000 m1_api_wrapper-2.1.0/m1wrapper/traverse.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-14 23:57:10.914155 m1_api_wrapper-2.1.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)      555 2022-01-14 23:56:52.000000 m1_api_wrapper-2.1.0/setup.py
+drwxrwxr-x   0 marek     (1000) marek     (1000)        0 2023-05-16 17:28:46.341235 m1_api_wrapper-2.1.1/
+-rw-rw-r--   0 marek     (1000) marek     (1000)       16 2023-03-28 15:06:30.000000 m1_api_wrapper-2.1.1/LICENSE
+-rw-rw-r--   0 marek     (1000) marek     (1000)     7531 2023-05-16 17:28:46.341235 m1_api_wrapper-2.1.1/PKG-INFO
+-rw-rw-r--   0 marek     (1000) marek     (1000)     7213 2023-03-28 15:06:30.000000 m1_api_wrapper-2.1.1/README.md
+drwxrwxr-x   0 marek     (1000) marek     (1000)        0 2023-05-16 17:28:46.341235 m1_api_wrapper-2.1.1/m1_api_wrapper.egg-info/
+-rw-rw-r--   0 marek     (1000) marek     (1000)     7531 2023-05-16 17:28:46.000000 m1_api_wrapper-2.1.1/m1_api_wrapper.egg-info/PKG-INFO
+-rw-rw-r--   0 marek     (1000) marek     (1000)      342 2023-05-16 17:28:46.000000 m1_api_wrapper-2.1.1/m1_api_wrapper.egg-info/SOURCES.txt
+-rw-rw-r--   0 marek     (1000) marek     (1000)        1 2023-05-16 17:28:46.000000 m1_api_wrapper-2.1.1/m1_api_wrapper.egg-info/dependency_links.txt
+-rw-rw-r--   0 marek     (1000) marek     (1000)        9 2023-05-16 17:28:46.000000 m1_api_wrapper-2.1.1/m1_api_wrapper.egg-info/requires.txt
+-rw-rw-r--   0 marek     (1000) marek     (1000)       10 2023-05-16 17:28:46.000000 m1_api_wrapper-2.1.1/m1_api_wrapper.egg-info/top_level.txt
+drwxrwxr-x   0 marek     (1000) marek     (1000)        0 2023-05-16 17:28:46.341235 m1_api_wrapper-2.1.1/m1wrapper/
+-rw-rw-r--   0 marek     (1000) marek     (1000)      126 2023-03-28 15:06:30.000000 m1_api_wrapper-2.1.1/m1wrapper/__init__.py
+-rw-rw-r--   0 marek     (1000) marek     (1000)      312 2023-03-28 15:06:30.000000 m1_api_wrapper-2.1.1/m1wrapper/config.py
+-rw-rw-r--   0 marek     (1000) marek     (1000)      662 2023-04-13 13:29:57.000000 m1_api_wrapper-2.1.1/m1wrapper/errors.py
+-rw-rw-r--   0 marek     (1000) marek     (1000)     4074 2023-05-16 17:22:41.000000 m1_api_wrapper-2.1.1/m1wrapper/m1wrapper.py
+-rw-rw-r--   0 marek     (1000) marek     (1000)     5625 2023-05-16 17:22:41.000000 m1_api_wrapper-2.1.1/m1wrapper/search.py
+-rw-rw-r--   0 marek     (1000) marek     (1000)     1308 2023-03-28 15:06:30.000000 m1_api_wrapper-2.1.1/m1wrapper/traverse.py
+-rw-rw-r--   0 marek     (1000) marek     (1000)       38 2023-05-16 17:28:46.341235 m1_api_wrapper-2.1.1/setup.cfg
+-rwxrwxr-x   0 marek     (1000) marek     (1000)      555 2023-05-16 17:28:33.000000 m1_api_wrapper-2.1.1/setup.py
```

### Comparing `m1_api_wrapper-2.1.0/PKG-INFO` & `m1_api_wrapper-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: m1_api_wrapper
-Version: 2.1.0
+Version: 2.1.1
 Summary: Molecule One API Wrapper
 Home-page: https://github.com/molecule-one/m1wrapper-python
 Author: Szymon Pilkowski
 Author-email: szymon.pilkowski@molecule.one
 License: # todo: license
         
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Molecule One Batch Scoring API Wrapper
 
 ## Usage:
 
@@ -207,9 +206,7 @@
 Parameters and returned JSON are the same as with `get_partial_results()`.
 
 ### Deleting your data:
 
 ```py
 m1wrapper.delete_batch_search(search.search_id)
 ```
-
-
```

### Comparing `m1_api_wrapper-2.1.0/README.md` & `m1_api_wrapper-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `m1_api_wrapper-2.1.0/m1_api_wrapper.egg-info/PKG-INFO` & `m1_api_wrapper-2.1.1/m1_api_wrapper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: m1-api-wrapper
-Version: 2.1.0
+Version: 2.1.1
 Summary: Molecule One API Wrapper
 Home-page: https://github.com/molecule-one/m1wrapper-python
 Author: Szymon Pilkowski
 Author-email: szymon.pilkowski@molecule.one
 License: # todo: license
         
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Molecule One Batch Scoring API Wrapper
 
 ## Usage:
 
@@ -207,9 +206,7 @@
 Parameters and returned JSON are the same as with `get_partial_results()`.
 
 ### Deleting your data:
 
 ```py
 m1wrapper.delete_batch_search(search.search_id)
 ```
-
-
```

### Comparing `m1_api_wrapper-2.1.0/m1wrapper/errors.py` & `m1_api_wrapper-2.1.1/m1wrapper/errors.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,15 +4,18 @@
     if error["message"] and error["errors"]:
         return f'{error["message"]}: {repr(error["errors"])}'
     if error["message"]:
         return f'{error["message"]}'
     else:
         return "unknown error"
 
+def is_json_response(response):
+    return response.headers.get('Content-Type', '').startswith('application/json')
+
 
 def maybe_handle_error(response):
-    if response.status_code >= 400 and response.status_code < 500:
+    if response.status_code >= 400 and response.status_code < 500 and is_json_response(response):
         error = format_error_message(response.json())
         raise requests.exceptions.HTTPError(error)
     else:
         response.raise_for_status()
```

### Comparing `m1_api_wrapper-2.1.0/m1wrapper/m1wrapper.py` & `m1_api_wrapper-2.1.1/m1wrapper/m1wrapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,36 +64,39 @@
             self,
             targets: List[str],
             parameters: Dict = None,
             detail_level = DetailLevel.SCORE,
             priority = Priority.NORMAL,
             invalid_target_strategy = InvalidTargetStrategy.REJECT ,
             starting_materials: List[str] = None,
+            preset = None,
             name = None
     ) -> BatchSearch:
         return BatchSearch(
                 self.api_base_url,
                 self.request_headers,
                 targets=targets,
                 parameters=parameters,
                 detail_level=detail_level,
                 priority=int(priority),
                 invalid_target_strategy=invalid_target_strategy,
                 starting_materials=starting_materials,
+                preset=preset,
                 name=name
             )
 
     def run_batch_search_with_metadata(
             self,
             targets_with_metadata: List[Dict[str, str]],
             parameters: Dict = None,
             detail_level = DetailLevel.SCORE,
             priority = Priority.NORMAL,
             invalid_target_strategy = InvalidTargetStrategy.REJECT ,
             starting_materials: List[str] = None,
+            preset = None,
             name = None
     ) -> BatchSearch:
         targets = []
         targets_with_metadata_copy = copy.deepcopy(targets_with_metadata)
         targets_metadata = {}
         for index, item in enumerate(targets_with_metadata_copy):
             target = item.pop('smiles', None)
@@ -108,14 +111,15 @@
                 targets=targets,
                 parameters=parameters,
                 detail_level=detail_level,
                 priority=int(priority),
                 invalid_target_strategy=invalid_target_strategy,
                 starting_materials=starting_materials,
                 name=name,
+                preset=preset,
                 targets_metadata=targets_metadata
             )
 
     def get_batch_search(self, search_id: str) -> BatchSearch:
         search = BatchSearch.from_id(
                 self.api_base_url,
                 self.request_headers,
```

### Comparing `m1_api_wrapper-2.1.0/m1wrapper/search.py` & `m1_api_wrapper-2.1.1/m1wrapper/search.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,14 +32,15 @@
         search_id=None,
         targets=None,
         parameters=None,
         detail_level=None,
         priority=None,
         invalid_target_strategy=None,
         starting_materials=None,
+        preset=None,
         name=None,
         targets_metadata=None,
     ):
         self.search_id = search_id
         self.base_url = base_url
         self.headers = headers
         self.http = self.__prepare_http()
@@ -47,29 +48,32 @@
             new_search = self.__run(
                     targets=targets,
                     parameters=parameters,
                     detail_level=detail_level,
                     priority=priority,
                     invalid_target_strategy=invalid_target_strategy,
                     starting_materials=starting_materials,
+                    preset=preset,
                     name=name,
                     targets_metadata=targets_metadata
             )
             self.search_id = new_search['id']
 
-    def __prepare_payload(self, targets, parameters, detail_level, priority, invalid_target_strategy, starting_materials, name, targets_metadata) -> dict:
+    def __prepare_payload(self, targets, parameters, detail_level, priority, invalid_target_strategy, starting_materials, preset, name, targets_metadata) -> dict:
         payload = {
             'targets': targets,
             'parameters': parameters or {},
             'detail_level': detail_level,
             'priority': priority,
             'invalid_target_strategy': invalid_target_strategy
         }
         if starting_materials is not None:
             payload["starting_materials"] = starting_materials
+        if preset is not None:
+            payload["preset"] = preset 
         if name is not None:
             payload["name"] = name
         if targets_metadata is not None:
             payload['targets_metadata'] = targets_metadata
 
         return payload
 
@@ -83,16 +87,16 @@
         )
         adapter = HTTPAdapter(max_retries=retry_strategy)
         http = requests.Session()
         http.mount("https://", adapter)
         http.mount("http://", adapter)
         return http
 
-    def __run(self, targets, parameters, detail_level, priority, invalid_target_strategy, starting_materials, name, targets_metadata):
-        payload = self.__prepare_payload(targets, parameters, detail_level, priority, invalid_target_strategy, starting_materials, name, targets_metadata)
+    def __run(self, targets, parameters, detail_level, priority, invalid_target_strategy, starting_materials, preset, name, targets_metadata):
+        payload = self.__prepare_payload(targets, parameters, detail_level, priority, invalid_target_strategy, starting_materials, preset, name, targets_metadata)
         response = self.http.post(
             urljoin(self.base_url, api_search_endpoint),
             data=json.dumps(payload),
             headers=self.headers,
         )
         maybe_handle_error(response)
         return response.json()
@@ -143,14 +147,17 @@
                 'precision': precision,
                 'only': only
             }
         )
         maybe_handle_error(response)
         results = response.json()
 
+        if precision is None:
+            return results
+
         precision_str = '.' + str(precision) + 'f'
         results = traverse_modify(results, '[].result', lambda el: format(float(el), precision_str) if el else el)
         results = traverse_modify(results, '[].certainty', lambda el: format(float(el), precision_str) if el else el)
         results = traverse_modify(results, '[].price', lambda el: format(float(el), precision_str) if el else el)
         return results
 
     def delete(self):
```

### Comparing `m1_api_wrapper-2.1.0/m1wrapper/traverse.py` & `m1_api_wrapper-2.1.1/m1wrapper/traverse.py`

 * *Files identical despite different names*

### Comparing `m1_api_wrapper-2.1.0/setup.py` & `m1_api_wrapper-2.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     readme = f.read()
 
 with open('LICENSE') as f:
     license = f.read()
 
 setup(
     name='m1_api_wrapper',
-    version='2.1.0',
+    version='2.1.1',
     description='Molecule One API Wrapper',
     long_description=readme,
     long_description_content_type='text/markdown',
     author='Szymon Pilkowski',
     author_email='szymon.pilkowski@molecule.one',
     url='https://github.com/molecule-one/m1wrapper-python',
     license=license,
```

