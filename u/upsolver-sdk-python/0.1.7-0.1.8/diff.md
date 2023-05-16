# Comparing `tmp/upsolver_sdk_python-0.1.7.tar.gz` & `tmp/upsolver_sdk_python-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upsolver_sdk_python-0.1.7.tar", max compression
+gzip compressed data, was "upsolver_sdk_python-0.1.8.tar", max compression
```

## Comparing `upsolver_sdk_python-0.1.7.tar` & `upsolver_sdk_python-0.1.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     5071 2023-04-21 12:19:24.202781 upsolver_sdk_python-0.1.7/README.md
--rw-r--r--   0        0        0      651 2023-04-21 12:19:24.218782 upsolver_sdk_python-0.1.7/pyproject.toml
--rw-r--r--   0        0        0       97 2023-04-21 12:19:24.218782 upsolver_sdk_python-0.1.7/upsolver/__init__.py
--rw-r--r--   0        0        0        0 2023-04-21 12:19:24.218782 upsolver_sdk_python-0.1.7/upsolver/client/__init__.py
--rw-r--r--   0        0        0      825 2023-04-21 12:19:24.218782 upsolver_sdk_python-0.1.7/upsolver/client/auth_filler.py
--rw-r--r--   0        0        0     3673 2023-04-21 12:19:24.218782 upsolver_sdk_python-0.1.7/upsolver/client/exceptions.py
--rw-r--r--   0        0        0     4153 2023-04-21 12:19:24.218782 upsolver_sdk_python-0.1.7/upsolver/client/poller.py
--rw-r--r--   0        0        0     1185 2023-04-21 12:19:24.218782 upsolver_sdk_python-0.1.7/upsolver/client/query.py
--rw-r--r--   0        0        0     4204 2023-04-21 12:19:24.218782 upsolver_sdk_python-0.1.7/upsolver/client/requester.py
--rw-r--r--   0        0        0     1108 2023-04-21 12:19:24.218782 upsolver_sdk_python-0.1.7/upsolver/client/response.py
--rw-r--r--   0        0        0      938 2023-04-21 12:19:24.218782 upsolver_sdk_python-0.1.7/upsolver/dbapi/README.md
--rw-r--r--   0        0        0      131 2023-04-21 12:19:24.218782 upsolver_sdk_python-0.1.7/upsolver/dbapi/__init__.py
--rw-r--r--   0        0        0     2222 2023-04-21 12:19:24.218782 upsolver_sdk_python-0.1.7/upsolver/dbapi/connection.py
--rw-r--r--   0        0        0     7851 2023-04-21 12:19:24.218782 upsolver_sdk_python-0.1.7/upsolver/dbapi/cursor.py
--rw-r--r--   0        0        0     1967 2023-04-21 12:19:24.218782 upsolver_sdk_python-0.1.7/upsolver/dbapi/examples.py
--rw-r--r--   0        0        0     1423 2023-04-21 12:19:24.218782 upsolver_sdk_python-0.1.7/upsolver/dbapi/type_constructors.py
--rw-r--r--   0        0        0     1609 2023-04-21 12:19:24.218782 upsolver_sdk_python-0.1.7/upsolver/dbapi/types_definitions.py
--rw-r--r--   0        0        0     3144 2023-04-21 12:19:24.218782 upsolver_sdk_python-0.1.7/upsolver/dbapi/utils.py
--rw-r--r--   0        0        0        0 2023-04-21 12:19:24.218782 upsolver_sdk_python-0.1.7/upsolver/sdk/__init__.py
--rw-r--r--   0        0        0     1309 2023-04-21 12:19:24.218782 upsolver_sdk_python-0.1.7/upsolver/sdk/client.py
--rw-r--r--   0        0        0      454 2023-04-21 12:19:24.218782 upsolver_sdk_python-0.1.7/upsolver/sdk/utils.py
--rw-r--r--   0        0        0     2557 2023-04-21 12:19:24.218782 upsolver_sdk_python-0.1.7/upsolver/utils.py
--rw-r--r--   0        0        0     5720 1970-01-01 00:00:00.000000 upsolver_sdk_python-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     5071 2023-05-16 16:28:08.085060 upsolver_sdk_python-0.1.8/README.md
+-rw-r--r--   0        0        0      651 2023-05-16 16:28:08.097060 upsolver_sdk_python-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0       97 2023-05-16 16:28:08.097060 upsolver_sdk_python-0.1.8/upsolver/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-16 16:28:08.097060 upsolver_sdk_python-0.1.8/upsolver/client/__init__.py
+-rw-r--r--   0        0        0      825 2023-05-16 16:28:08.097060 upsolver_sdk_python-0.1.8/upsolver/client/auth_filler.py
+-rw-r--r--   0        0        0     3673 2023-05-16 16:28:08.097060 upsolver_sdk_python-0.1.8/upsolver/client/exceptions.py
+-rw-r--r--   0        0        0     4428 2023-05-16 16:28:08.097060 upsolver_sdk_python-0.1.8/upsolver/client/poller.py
+-rw-r--r--   0        0        0     1185 2023-05-16 16:28:08.097060 upsolver_sdk_python-0.1.8/upsolver/client/query.py
+-rw-r--r--   0        0        0     4204 2023-05-16 16:28:08.097060 upsolver_sdk_python-0.1.8/upsolver/client/requester.py
+-rw-r--r--   0        0        0     1108 2023-05-16 16:28:08.097060 upsolver_sdk_python-0.1.8/upsolver/client/response.py
+-rw-r--r--   0        0        0      938 2023-05-16 16:28:08.097060 upsolver_sdk_python-0.1.8/upsolver/dbapi/README.md
+-rw-r--r--   0        0        0      131 2023-05-16 16:28:08.097060 upsolver_sdk_python-0.1.8/upsolver/dbapi/__init__.py
+-rw-r--r--   0        0        0     2222 2023-05-16 16:28:08.097060 upsolver_sdk_python-0.1.8/upsolver/dbapi/connection.py
+-rw-r--r--   0        0        0     7851 2023-05-16 16:28:08.097060 upsolver_sdk_python-0.1.8/upsolver/dbapi/cursor.py
+-rw-r--r--   0        0        0     2172 2023-05-16 16:28:08.097060 upsolver_sdk_python-0.1.8/upsolver/dbapi/examples.py
+-rw-r--r--   0        0        0     1423 2023-05-16 16:28:08.097060 upsolver_sdk_python-0.1.8/upsolver/dbapi/type_constructors.py
+-rw-r--r--   0        0        0     1609 2023-05-16 16:28:08.097060 upsolver_sdk_python-0.1.8/upsolver/dbapi/types_definitions.py
+-rw-r--r--   0        0        0     3463 2023-05-16 16:28:08.097060 upsolver_sdk_python-0.1.8/upsolver/dbapi/utils.py
+-rw-r--r--   0        0        0        0 2023-05-16 16:28:08.097060 upsolver_sdk_python-0.1.8/upsolver/sdk/__init__.py
+-rw-r--r--   0        0        0     1309 2023-05-16 16:28:08.097060 upsolver_sdk_python-0.1.8/upsolver/sdk/client.py
+-rw-r--r--   0        0        0      454 2023-05-16 16:28:08.097060 upsolver_sdk_python-0.1.8/upsolver/sdk/utils.py
+-rw-r--r--   0        0        0     2557 2023-05-16 16:28:08.097060 upsolver_sdk_python-0.1.8/upsolver/utils.py
+-rw-r--r--   0        0        0     5720 1970-01-01 00:00:00.000000 upsolver_sdk_python-0.1.8/PKG-INFO
```

### Comparing `upsolver_sdk_python-0.1.7/README.md` & `upsolver_sdk_python-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `upsolver_sdk_python-0.1.7/pyproject.toml` & `upsolver_sdk_python-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "upsolver-sdk-python"
-version = "0.1.7"
+version = "0.1.8"
 description = "Python SDK for Upsolver"
 authors = ["Upsolver Team <info@upsolver.com>"]
 
 license = "MIT"
 readme = "README.md"
 packages = [
     {include = "upsolver/__init__.py"},
```

### Comparing `upsolver_sdk_python-0.1.7/upsolver/client/auth_filler.py` & `upsolver_sdk_python-0.1.8/upsolver/client/auth_filler.py`

 * *Files identical despite different names*

### Comparing `upsolver_sdk_python-0.1.7/upsolver/client/exceptions.py` & `upsolver_sdk_python-0.1.8/upsolver/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `upsolver_sdk_python-0.1.7/upsolver/client/poller.py` & `upsolver_sdk_python-0.1.8/upsolver/client/poller.py`

 * *Files 8% similar despite different names*

```diff
@@ -88,17 +88,22 @@
                 requester=requester,
                 resp=requester.get(path=rjson['current']),
                 start_time=start_time,
             )
 
         if 'result' in rjson:
             result = rjson['result']
-            grid = result['grid']  # columns, data, ...
-            column_names = [c['name'] for c in grid['columns']]
-            data_w_columns: ExecutionResult = [dict(zip(column_names, row)) for row in grid['data']]
+            if rjson['kind'] == 'upsolver_scalar_query_response':
+                scalar = result['scalar']
+                column_name = [scalar['valueType']]
+                data_w_columns: ExecutionResult = [dict(zip([column_name], [scalar]))]
+            else:
+                grid = result['grid']  # columns, data, ...
+                column_name = [c['name'] for c in grid['columns']]
+                data_w_columns: ExecutionResult = [dict(zip(column_name, row)) for row in grid['data']]
 
             return data_w_columns, result.get('next')
         else:
             return [rjson], None
 
     def __call__(self, requester: Requester, resp: UpsolverResponse) -> \
             tuple:
```

### Comparing `upsolver_sdk_python-0.1.7/upsolver/client/query.py` & `upsolver_sdk_python-0.1.8/upsolver/client/query.py`

 * *Files identical despite different names*

### Comparing `upsolver_sdk_python-0.1.7/upsolver/client/requester.py` & `upsolver_sdk_python-0.1.8/upsolver/client/requester.py`

 * *Files identical despite different names*

### Comparing `upsolver_sdk_python-0.1.7/upsolver/client/response.py` & `upsolver_sdk_python-0.1.8/upsolver/client/response.py`

 * *Files identical despite different names*

### Comparing `upsolver_sdk_python-0.1.7/upsolver/dbapi/README.md` & `upsolver_sdk_python-0.1.8/upsolver/dbapi/README.md`

 * *Files identical despite different names*

### Comparing `upsolver_sdk_python-0.1.7/upsolver/dbapi/connection.py` & `upsolver_sdk_python-0.1.8/upsolver/dbapi/connection.py`

 * *Files identical despite different names*

### Comparing `upsolver_sdk_python-0.1.7/upsolver/dbapi/cursor.py` & `upsolver_sdk_python-0.1.8/upsolver/dbapi/cursor.py`

 * *Files identical despite different names*

### Comparing `upsolver_sdk_python-0.1.7/upsolver/dbapi/examples.py` & `upsolver_sdk_python-0.1.8/upsolver/dbapi/examples.py`

 * *Files 16% similar despite different names*

```diff
@@ -72,7 +72,13 @@
 #%%
 conn.close()
 try:
     new_cursor = conn.cursor()
 except BaseException as e:
     print('Caught error on closed connection')
 # %%
+job_name = '' # Job name here
+print('Execute a `SHOW CREATE` statement:')
+result1 = cursor.execute(f'show create job {job_name};')
+print('create job statement:')
+result2 = cursor.fetchone()
+print(result2)
```

### Comparing `upsolver_sdk_python-0.1.7/upsolver/dbapi/type_constructors.py` & `upsolver_sdk_python-0.1.8/upsolver/dbapi/type_constructors.py`

 * *Files identical despite different names*

### Comparing `upsolver_sdk_python-0.1.7/upsolver/dbapi/types_definitions.py` & `upsolver_sdk_python-0.1.8/upsolver/dbapi/types_definitions.py`

 * *Files identical despite different names*

### Comparing `upsolver_sdk_python-0.1.7/upsolver/dbapi/utils.py` & `upsolver_sdk_python-0.1.8/upsolver/dbapi/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -79,11 +79,16 @@
                 requester=requester,
                 resp=requester.get(path=rjson['current']),
                 start_time=start_time,
             )
 
         if 'result' in rjson:
             result = rjson['result']
-            result['grid']['has_next_page'] = result.get('next') is not None
-            return result['grid'], result.get('next')
+            if rjson['kind'] == 'upsolver_scalar_query_response':
+                scalar = result['scalar']
+                columns = [{'name': scalar['valueType'], 'columnType': {'clazz': 'StringColumnType'}}]
+                return {'columns': columns, 'data': [scalar]}, result.get('next')
+            else:
+                result['grid']['has_next_page'] = result.get('next') is not None
+                return result['grid'], result.get('next')
         else:
             return rjson, None
```

### Comparing `upsolver_sdk_python-0.1.7/upsolver/sdk/client.py` & `upsolver_sdk_python-0.1.8/upsolver/sdk/client.py`

 * *Files identical despite different names*

### Comparing `upsolver_sdk_python-0.1.7/upsolver/utils.py` & `upsolver_sdk_python-0.1.8/upsolver/utils.py`

 * *Files identical despite different names*

### Comparing `upsolver_sdk_python-0.1.7/PKG-INFO` & `upsolver_sdk_python-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upsolver-sdk-python
-Version: 0.1.7
+Version: 0.1.8
 Summary: Python SDK for Upsolver
 License: MIT
 Author: Upsolver Team
 Author-email: info@upsolver.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

