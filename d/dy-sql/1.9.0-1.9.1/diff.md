# Comparing `tmp/dy-sql-1.9.0.tar.gz` & `tmp/dy-sql-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dy-sql-1.9.0.tar", last modified: Wed Dec 15 20:31:03 2021, max compression
+gzip compressed data, was "dy-sql-1.9.1.tar", last modified: Wed Dec 15 21:02:33 2021, max compression
```

## Comparing `dy-sql-1.9.0.tar` & `dy-sql-1.9.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-15 20:31:03.934433 dy-sql-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1082 2021-12-15 20:31:01.000000 dy-sql-1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       42 2021-12-15 20:31:01.000000 dy-sql-1.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    23761 2021-12-15 20:31:03.934433 dy-sql-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    19340 2021-12-15 20:31:01.000000 dy-sql-1.9.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-15 20:31:03.930433 dy-sql-1.9.0/dy_sql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    23761 2021-12-15 20:31:03.000000 dy-sql-1.9.0/dy_sql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      406 2021-12-15 20:31:03.000000 dy-sql-1.9.0/dy_sql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-15 20:31:03.000000 dy-sql-1.9.0/dy_sql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-15 20:31:03.000000 dy-sql-1.9.0/dy_sql.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       47 2021-12-15 20:31:03.000000 dy-sql-1.9.0/dy_sql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-12-15 20:31:03.000000 dy-sql-1.9.0/dy_sql.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-15 20:31:03.934433 dy-sql-1.9.0/dysql/
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-12-15 20:31:01.000000 dy-sql-1.9.0/dysql/VERSION
--rw-r--r--   0 runner    (1001) docker     (121)      741 2021-12-15 20:31:01.000000 dy-sql-1.9.0/dysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8666 2021-12-15 20:31:01.000000 dy-sql-1.9.0/dysql/connections.py
--rw-r--r--   0 runner    (1001) docker     (121)     6623 2021-12-15 20:31:01.000000 dy-sql-1.9.0/dysql/databases.py
--rw-r--r--   0 runner    (1001) docker     (121)      276 2021-12-15 20:31:01.000000 dy-sql-1.9.0/dysql/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     7983 2021-12-15 20:31:01.000000 dy-sql-1.9.0/dysql/mappers.py
--rw-r--r--   0 runner    (1001) docker     (121)     5427 2021-12-15 20:31:01.000000 dy-sql-1.9.0/dysql/pydantic_mappers.py
--rw-r--r--   0 runner    (1001) docker     (121)    10973 2021-12-15 20:31:01.000000 dy-sql-1.9.0/dysql/query_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     8115 2021-12-15 20:31:01.000000 dy-sql-1.9.0/dysql/test_managers.py
--rw-r--r--   0 runner    (1001) docker     (121)      109 2021-12-15 20:31:03.934433 dy-sql-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1218 2021-12-15 20:31:01.000000 dy-sql-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-15 21:02:33.570938 dy-sql-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (121)     1082 2021-12-15 21:02:31.000000 dy-sql-1.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       42 2021-12-15 21:02:31.000000 dy-sql-1.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    25471 2021-12-15 21:02:33.570938 dy-sql-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    20834 2021-12-15 21:02:31.000000 dy-sql-1.9.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-15 21:02:33.566938 dy-sql-1.9.1/dy_sql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    25471 2021-12-15 21:02:33.000000 dy-sql-1.9.1/dy_sql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      406 2021-12-15 21:02:33.000000 dy-sql-1.9.1/dy_sql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-15 21:02:33.000000 dy-sql-1.9.1/dy_sql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-15 21:02:33.000000 dy-sql-1.9.1/dy_sql.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       47 2021-12-15 21:02:33.000000 dy-sql-1.9.1/dy_sql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2021-12-15 21:02:33.000000 dy-sql-1.9.1/dy_sql.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-15 21:02:33.570938 dy-sql-1.9.1/dysql/
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2021-12-15 21:02:31.000000 dy-sql-1.9.1/dysql/VERSION
+-rw-r--r--   0 runner    (1001) docker     (121)      741 2021-12-15 21:02:31.000000 dy-sql-1.9.1/dysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8762 2021-12-15 21:02:31.000000 dy-sql-1.9.1/dysql/connections.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6623 2021-12-15 21:02:31.000000 dy-sql-1.9.1/dysql/databases.py
+-rw-r--r--   0 runner    (1001) docker     (121)      276 2021-12-15 21:02:31.000000 dy-sql-1.9.1/dysql/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7983 2021-12-15 21:02:31.000000 dy-sql-1.9.1/dysql/mappers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5427 2021-12-15 21:02:31.000000 dy-sql-1.9.1/dysql/pydantic_mappers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10973 2021-12-15 21:02:31.000000 dy-sql-1.9.1/dysql/query_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8115 2021-12-15 21:02:31.000000 dy-sql-1.9.1/dysql/test_managers.py
+-rw-r--r--   0 runner    (1001) docker     (121)      109 2021-12-15 21:02:33.570938 dy-sql-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1218 2021-12-15 21:02:31.000000 dy-sql-1.9.1/setup.py
```

### Comparing `dy-sql-1.9.0/LICENSE` & `dy-sql-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dy-sql-1.9.0/PKG-INFO` & `dy-sql-1.9.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dy-sql
-Version: 1.9.0
+Version: 1.9.1
 Summary: Dynamically runs SQL queries and executions.
 Home-page: https://github.com/adobe/dy-sql
 Author: Adobe
 Author-email: noreply@adobe.com
 License: MIT
 Description: ######################
          Dynamic SQL (dy-sql)
@@ -341,20 +341,47 @@
                 return QueryData("SELECT status, name FROM table")
         
         
         @sqlupdate
         ~~~~~~~~~~
         Handles any SQL that is not a select. This is primarily, but not limited to, ``insert``, ``update``, and ``delete``.
         
+        
         .. code-block:: python
         
             @sqlupdate()
-            def insert_items(item_dict)
+            def insert_items(item_dict):
                 return QueryData("INSERT INTO", template_params={'in__item_id':item_id_list})
         
+        You can yield multiple QueryData objects. This is done in a transaction and it can be helpful for data integrity or just
+        a nice clean way to run a set of updates.
+        
+        .. code-block:: python
+        
+            @sqlupdate()
+            def insert_items(item_dict):
+                insert_values_1, insert_params_1 = TemplateGenerator.values('table1values', _get_values_for_1_from_items(item_dict))
+                insert_values_2, insert_params_2 = TemplateGenerator.values('table2values', _get_values_for_2_from_items(item_dict))
+                yield QueryData(f'INSERT INTO table_1 {insert_values_1}', query_params=insert_values_params_1)
+                yield QueryData(f'INSERT INTO table_2 {insert_values_2}', query_params=insert_values_params_2)
+        
+        if needed you can assign a callback to be ran after a query or set of queries completes successfully
+        
+        .. code-block:: python
+        
+            @sqlupdate(on_success=_handle_insert_success)
+            def insert_items_with_callback(item_dict):
+                insert_values_1, insert_params_1 = TemplateGenerator.values('table1values', _get_values_for_1_from_items(item_dict))
+                insert_values_2, insert_params_2 = TemplateGenerator.values('table2values', _get_values_for_2_from_items(item_dict))
+                yield QueryData(f'INSERT INTO table_1 {insert_values_1}', query_params=insert_values_params_1)
+                yield QueryData(f'INSERT INTO table_2 {insert_values_2}', query_params=insert_values_params_2)
+        
+            def _handle_insert_success(item_dict):
+                #  callback logic here happens after the transaction is complete
+        
         @sqlexists
         ~~~~~~~~~~
         This wraps a SQL query to determine if a row exists or not. If at least one row is returned from the query, it will
         return True, otherwise False. The query you give here can return anything you want but as good practice,
         try to always select as little as possible. For example, below we are just returning 1 because the value itself
         isn't used, we just need to know there are records available.
```

### Comparing `dy-sql-1.9.0/README.rst` & `dy-sql-1.9.1/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -333,20 +333,47 @@
         return QueryData("SELECT status, name FROM table")
 
 
 @sqlupdate
 ~~~~~~~~~~
 Handles any SQL that is not a select. This is primarily, but not limited to, ``insert``, ``update``, and ``delete``.
 
+
 .. code-block:: python
 
     @sqlupdate()
-    def insert_items(item_dict)
+    def insert_items(item_dict):
         return QueryData("INSERT INTO", template_params={'in__item_id':item_id_list})
 
+You can yield multiple QueryData objects. This is done in a transaction and it can be helpful for data integrity or just
+a nice clean way to run a set of updates.
+
+.. code-block:: python
+
+    @sqlupdate()
+    def insert_items(item_dict):
+        insert_values_1, insert_params_1 = TemplateGenerator.values('table1values', _get_values_for_1_from_items(item_dict))
+        insert_values_2, insert_params_2 = TemplateGenerator.values('table2values', _get_values_for_2_from_items(item_dict))
+        yield QueryData(f'INSERT INTO table_1 {insert_values_1}', query_params=insert_values_params_1)
+        yield QueryData(f'INSERT INTO table_2 {insert_values_2}', query_params=insert_values_params_2)
+
+if needed you can assign a callback to be ran after a query or set of queries completes successfully
+
+.. code-block:: python
+
+    @sqlupdate(on_success=_handle_insert_success)
+    def insert_items_with_callback(item_dict):
+        insert_values_1, insert_params_1 = TemplateGenerator.values('table1values', _get_values_for_1_from_items(item_dict))
+        insert_values_2, insert_params_2 = TemplateGenerator.values('table2values', _get_values_for_2_from_items(item_dict))
+        yield QueryData(f'INSERT INTO table_1 {insert_values_1}', query_params=insert_values_params_1)
+        yield QueryData(f'INSERT INTO table_2 {insert_values_2}', query_params=insert_values_params_2)
+
+    def _handle_insert_success(item_dict):
+        #  callback logic here happens after the transaction is complete
+
 @sqlexists
 ~~~~~~~~~~
 This wraps a SQL query to determine if a row exists or not. If at least one row is returned from the query, it will
 return True, otherwise False. The query you give here can return anything you want but as good practice,
 try to always select as little as possible. For example, below we are just returning 1 because the value itself
 isn't used, we just need to know there are records available.
```

### Comparing `dy-sql-1.9.0/dy_sql.egg-info/PKG-INFO` & `dy-sql-1.9.1/dy_sql.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dy-sql
-Version: 1.9.0
+Version: 1.9.1
 Summary: Dynamically runs SQL queries and executions.
 Home-page: https://github.com/adobe/dy-sql
 Author: Adobe
 Author-email: noreply@adobe.com
 License: MIT
 Description: ######################
          Dynamic SQL (dy-sql)
@@ -341,20 +341,47 @@
                 return QueryData("SELECT status, name FROM table")
         
         
         @sqlupdate
         ~~~~~~~~~~
         Handles any SQL that is not a select. This is primarily, but not limited to, ``insert``, ``update``, and ``delete``.
         
+        
         .. code-block:: python
         
             @sqlupdate()
-            def insert_items(item_dict)
+            def insert_items(item_dict):
                 return QueryData("INSERT INTO", template_params={'in__item_id':item_id_list})
         
+        You can yield multiple QueryData objects. This is done in a transaction and it can be helpful for data integrity or just
+        a nice clean way to run a set of updates.
+        
+        .. code-block:: python
+        
+            @sqlupdate()
+            def insert_items(item_dict):
+                insert_values_1, insert_params_1 = TemplateGenerator.values('table1values', _get_values_for_1_from_items(item_dict))
+                insert_values_2, insert_params_2 = TemplateGenerator.values('table2values', _get_values_for_2_from_items(item_dict))
+                yield QueryData(f'INSERT INTO table_1 {insert_values_1}', query_params=insert_values_params_1)
+                yield QueryData(f'INSERT INTO table_2 {insert_values_2}', query_params=insert_values_params_2)
+        
+        if needed you can assign a callback to be ran after a query or set of queries completes successfully
+        
+        .. code-block:: python
+        
+            @sqlupdate(on_success=_handle_insert_success)
+            def insert_items_with_callback(item_dict):
+                insert_values_1, insert_params_1 = TemplateGenerator.values('table1values', _get_values_for_1_from_items(item_dict))
+                insert_values_2, insert_params_2 = TemplateGenerator.values('table2values', _get_values_for_2_from_items(item_dict))
+                yield QueryData(f'INSERT INTO table_1 {insert_values_1}', query_params=insert_values_params_1)
+                yield QueryData(f'INSERT INTO table_2 {insert_values_2}', query_params=insert_values_params_2)
+        
+            def _handle_insert_success(item_dict):
+                #  callback logic here happens after the transaction is complete
+        
         @sqlexists
         ~~~~~~~~~~
         This wraps a SQL query to determine if a row exists or not. If at least one row is returned from the query, it will
         return True, otherwise False. The query you give here can return anything you want but as good practice,
         try to always select as little as possible. For example, below we are just returning 1 because the value itself
         isn't used, we just need to know there are records available.
```

### Comparing `dy-sql-1.9.0/dysql/__init__.py` & `dy-sql-1.9.1/dysql/__init__.py`

 * *Files identical despite different names*

### Comparing `dy-sql-1.9.0/dysql/connections.py` & `dy-sql-1.9.1/dysql/connections.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,15 +166,15 @@
                 return result == 1
 
         return handle_query
 
     return decorator
 
 
-def sqlupdate(isolation_level='READ_COMMITTED', disable_foreign_key_checks=False):
+def sqlupdate(isolation_level='READ_COMMITTED', disable_foreign_key_checks=False, on_success=None):
     """
     :param isolation_level should specify whether we can read data from transactions that are not
         yet committed defaults to READ_COMMITTED
     :param disable_foreign_key_checks Should be used with caution. Only use this if you have
         confidence the data you are inserting is going to have everything it needs to satisfy
         foreign_key_checks once all the data is applied. Foreign key checks are there to provide
         our database with integrety
@@ -227,11 +227,13 @@
                     query, params = get_query_data(data)
                     if isinstance(params, list):
                         raise Exception('Params must not be a list')
                     conn_manager.execute_query(query, params)
 
                 if disable_foreign_key_checks:
                     conn_manager.execute_query("SET FOREIGN_KEY_CHECKS=1")
+                if on_success:
+                    on_success(*args, **kwargs)
 
         return handle_query
 
     return update_wrapper
```

### Comparing `dy-sql-1.9.0/dysql/databases.py` & `dy-sql-1.9.1/dysql/databases.py`

 * *Files identical despite different names*

### Comparing `dy-sql-1.9.0/dysql/mappers.py` & `dy-sql-1.9.1/dysql/mappers.py`

 * *Files identical despite different names*

### Comparing `dy-sql-1.9.0/dysql/pydantic_mappers.py` & `dy-sql-1.9.1/dysql/pydantic_mappers.py`

 * *Files identical despite different names*

### Comparing `dy-sql-1.9.0/dysql/query_utils.py` & `dy-sql-1.9.1/dysql/query_utils.py`

 * *Files identical despite different names*

### Comparing `dy-sql-1.9.0/dysql/test_managers.py` & `dy-sql-1.9.1/dysql/test_managers.py`

 * *Files identical despite different names*

### Comparing `dy-sql-1.9.0/setup.py` & `dy-sql-1.9.1/setup.py`

 * *Files identical despite different names*

