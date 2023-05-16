# Comparing `tmp/banner-storedot-2.2.9.tar.gz` & `tmp/banner-storedot-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "banner-storedot-2.2.9.tar", last modified: Mon Jan 30 15:25:50 2023, max compression
+gzip compressed data, was "banner-storedot-2.3.0.tar", last modified: Tue May 16 12:13:57 2023, max compression
```

## Comparing `banner-storedot-2.2.9.tar` & `banner-storedot-2.3.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-sr-x   0 gil       (1008) developers  (1234)        0 2023-01-30 15:25:50.740200 banner-storedot-2.2.9/
--rw-rwSr--   0 gil       (1008) developers  (1234)     1073 2021-08-19 08:44:05.000000 banner-storedot-2.2.9/LICENSE
--rw-r--r--   0 gil       (1008) developers  (1234)     8235 2023-01-30 15:25:50.740200 banner-storedot-2.2.9/PKG-INFO
--rw-rwSr--   0 gil       (1008) developers  (1234)     7782 2022-07-18 10:09:00.000000 banner-storedot-2.2.9/README.md
--rw-rwSr--   0 gil       (1008) developers  (1234)      122 2021-08-19 10:21:45.000000 banner-storedot-2.2.9/pyproject.toml
--rw-r--r--   0 gil       (1008) developers  (1234)      672 2023-01-30 15:25:50.740200 banner-storedot-2.2.9/setup.cfg
-drwxr-sr-x   0 gil       (1008) developers  (1234)        0 2023-01-30 15:25:50.736199 banner-storedot-2.2.9/src/
-drwxr-sr-x   0 gil       (1008) developers  (1234)        0 2023-01-30 15:25:50.736199 banner-storedot-2.2.9/src/banner/
--rw-rwSr--   0 gil       (1008) developers  (1234)      161 2022-11-08 14:34:28.000000 banner-storedot-2.2.9/src/banner/__init__.py
--rw-r--r--   0 gil       (1008) developers  (1234)    26651 2023-01-30 15:23:16.000000 banner-storedot-2.2.9/src/banner/connection.py
--rw-rwSr--   0 gil       (1008) developers  (1234)     6049 2023-01-08 12:31:38.000000 banner-storedot-2.2.9/src/banner/pandas_decorator.py
--rw-rwSr--   0 gil       (1008) developers  (1234)     2121 2022-01-09 16:04:35.000000 banner-storedot-2.2.9/src/banner/pandas_wrap.py
--rw-rwSr--   0 gil       (1008) developers  (1234)    47841 2023-01-29 14:03:26.000000 banner-storedot-2.2.9/src/banner/queries.py
-drwxr-sr-x   0 gil       (1008) developers  (1234)        0 2023-01-30 15:25:50.740200 banner-storedot-2.2.9/src/banner/utils/
--rw-rwSr--   0 gil       (1008) developers  (1234)        0 2021-08-19 11:04:29.000000 banner-storedot-2.2.9/src/banner/utils/__init__.py
--rw-rwSr--   0 gil       (1008) developers  (1234)     3798 2022-12-22 09:12:51.000000 banner-storedot-2.2.9/src/banner/utils/const.py
--rw-rwSr--   0 gil       (1008) developers  (1234)     1739 2022-12-27 13:22:40.000000 banner-storedot-2.2.9/src/banner/utils/misc.py
--rw-rwSr--   0 gil       (1008) developers  (1234)    10084 2023-01-19 13:06:13.000000 banner-storedot-2.2.9/src/banner/utils/neware.py
--rw-rwSr--   0 gil       (1008) developers  (1234)     1952 2022-08-17 11:13:16.000000 banner-storedot-2.2.9/src/banner/utils/pandas.py
--rw-rwSr--   0 gil       (1008) developers  (1234)   166397 2023-01-12 11:46:42.000000 banner-storedot-2.2.9/src/banner/utils/web2py.py
-drwxr-sr-x   0 gil       (1008) developers  (1234)        0 2023-01-30 15:25:50.740200 banner-storedot-2.2.9/src/banner_storedot.egg-info/
--rw-rwSr--   0 gil       (1008) developers  (1234)     8235 2023-01-30 15:25:50.000000 banner-storedot-2.2.9/src/banner_storedot.egg-info/PKG-INFO
--rw-rwSr--   0 gil       (1008) developers  (1234)      544 2023-01-30 15:25:50.000000 banner-storedot-2.2.9/src/banner_storedot.egg-info/SOURCES.txt
--rw-rwSr--   0 gil       (1008) developers  (1234)        1 2023-01-30 15:25:50.000000 banner-storedot-2.2.9/src/banner_storedot.egg-info/dependency_links.txt
--rw-rwSr--   0 gil       (1008) developers  (1234)       75 2023-01-30 15:25:50.000000 banner-storedot-2.2.9/src/banner_storedot.egg-info/requires.txt
--rw-rwSr--   0 gil       (1008) developers  (1234)        7 2023-01-30 15:25:50.000000 banner-storedot-2.2.9/src/banner_storedot.egg-info/top_level.txt
+drwxr-sr-x   0 gil       (1008) developers  (1234)        0 2023-05-16 12:13:57.677067 banner-storedot-2.3.0/
+-rw-rwSr--   0 gil       (1008) developers  (1234)     1073 2021-08-19 08:44:05.000000 banner-storedot-2.3.0/LICENSE
+-rw-r--r--   0 gil       (1008) developers  (1234)     8235 2023-05-16 12:13:57.677067 banner-storedot-2.3.0/PKG-INFO
+-rw-rwSr--   0 gil       (1008) developers  (1234)     7782 2022-07-18 10:09:00.000000 banner-storedot-2.3.0/README.md
+-rw-rwSr--   0 gil       (1008) developers  (1234)      122 2021-08-19 10:21:45.000000 banner-storedot-2.3.0/pyproject.toml
+-rw-rwSr--   0 gil       (1008) developers  (1234)      672 2023-05-16 12:13:57.677067 banner-storedot-2.3.0/setup.cfg
+drwxr-sr-x   0 gil       (1008) developers  (1234)        0 2023-05-16 12:13:57.669067 banner-storedot-2.3.0/src/
+drwxr-sr-x   0 gil       (1008) developers  (1234)        0 2023-05-16 12:13:57.673067 banner-storedot-2.3.0/src/banner/
+-rw-rwSr--   0 gil       (1008) developers  (1234)      161 2022-11-08 14:34:28.000000 banner-storedot-2.3.0/src/banner/__init__.py
+-rw-rwSr--   0 gil       (1008) developers  (1234)    27556 2023-05-16 12:12:09.000000 banner-storedot-2.3.0/src/banner/connection.py
+-rw-rwSr--   0 gil       (1008) developers  (1234)     6164 2023-03-20 12:23:23.000000 banner-storedot-2.3.0/src/banner/pandas_decorator.py
+-rw-rwSr--   0 gil       (1008) developers  (1234)     2121 2022-01-09 16:04:35.000000 banner-storedot-2.3.0/src/banner/pandas_wrap.py
+-rw-rwSr--   0 gil       (1008) developers  (1234)    52211 2023-05-16 12:12:15.000000 banner-storedot-2.3.0/src/banner/queries.py
+drwxr-sr-x   0 gil       (1008) developers  (1234)        0 2023-05-16 12:13:57.673067 banner-storedot-2.3.0/src/banner/utils/
+-rw-rwSr--   0 gil       (1008) developers  (1234)        0 2021-08-19 11:04:29.000000 banner-storedot-2.3.0/src/banner/utils/__init__.py
+-rw-rwSr--   0 gil       (1008) developers  (1234)     3798 2022-12-22 09:12:51.000000 banner-storedot-2.3.0/src/banner/utils/const.py
+-rw-rwSr--   0 gil       (1008) developers  (1234)     1923 2023-03-23 08:47:01.000000 banner-storedot-2.3.0/src/banner/utils/misc.py
+-rw-rwSr--   0 gil       (1008) developers  (1234)    10202 2023-05-09 07:24:41.000000 banner-storedot-2.3.0/src/banner/utils/neware.py
+-rw-rwSr--   0 gil       (1008) developers  (1234)     1952 2022-08-17 11:13:16.000000 banner-storedot-2.3.0/src/banner/utils/pandas.py
+-rw-rwSr--   0 gil       (1008) developers  (1234)   182089 2023-05-09 12:41:23.000000 banner-storedot-2.3.0/src/banner/utils/web2py.py
+drwxr-sr-x   0 gil       (1008) developers  (1234)        0 2023-05-16 12:13:57.677067 banner-storedot-2.3.0/src/banner_storedot.egg-info/
+-rw-rwSr--   0 gil       (1008) developers  (1234)     8235 2023-05-16 12:13:57.000000 banner-storedot-2.3.0/src/banner_storedot.egg-info/PKG-INFO
+-rw-rwSr--   0 gil       (1008) developers  (1234)      544 2023-05-16 12:13:57.000000 banner-storedot-2.3.0/src/banner_storedot.egg-info/SOURCES.txt
+-rw-rwSr--   0 gil       (1008) developers  (1234)        1 2023-05-16 12:13:57.000000 banner-storedot-2.3.0/src/banner_storedot.egg-info/dependency_links.txt
+-rw-rwSr--   0 gil       (1008) developers  (1234)       75 2023-05-16 12:13:57.000000 banner-storedot-2.3.0/src/banner_storedot.egg-info/requires.txt
+-rw-rwSr--   0 gil       (1008) developers  (1234)        7 2023-05-16 12:13:57.000000 banner-storedot-2.3.0/src/banner_storedot.egg-info/top_level.txt
```

### Comparing `banner-storedot-2.2.9/LICENSE` & `banner-storedot-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `banner-storedot-2.2.9/PKG-INFO` & `banner-storedot-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: banner-storedot
-Version: 2.2.9
+Version: 2.3.0
 Summary: light dal package
 Home-page: https://https://github.com/storedot/banner
 Author: GB
 Author-email: gilb@store-dot.com
 Project-URL: Bug Tracker, https://https://github.com/storedot/banner/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `banner-storedot-2.2.9/README.md` & `banner-storedot-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `banner-storedot-2.2.9/setup.cfg` & `banner-storedot-2.3.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = banner-storedot
-version = 2.2.9
+version = 2.3.0
 author = GB
 author_email = gilb@store-dot.com
 description = light dal package
 long_description = file: README.md
 url = https://https://github.com/storedot/banner
 project_urls = 
 	Bug Tracker = https://https://github.com/storedot/banner/issues
```

### Comparing `banner-storedot-2.2.9/src/banner/connection.py` & `banner-storedot-2.3.0/src/banner/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 
 from typing import Union, Dict, Iterable
 from abc import ABC, abstractmethod
 from enum import Enum
 from itertools import chain
 from json import loads, dumps
 from inspect import getfullargspec
+from copy import deepcopy
 
 from MySQLdb import connect as mysql_connect, MySQLError
 from MySQLdb._exceptions import OperationalError
 from MySQLdb.cursors import DictCursor
 
 from psycopg2 import connect as postgres_sql_connect, Error as PostgresSQLError
 from psycopg2.extras import RealDictCursor
@@ -128,24 +129,25 @@
 
         controller = QUERY_TO_STORAGE_CONTROL.get(func.__name__, DefaultStorageController)
         
         return controller.store(
             self.instance, value, func, *args, ttl=ttl, nx=nx, **kwargs
         )
 
-    def retrieve_by(self, key: str):
-        return self.instance.get(
-            str(key)
-        )
+    def retrieve_by(self, keys: Union[str, list]): #TODO support json
+        if isinstance(keys, str):
+            return self.instance.get(keys)
+        
+        return self.instance.mget(keys)
         
-    def store_by(self, key: str, value, ttl=None):
+    def store_by(self, key: str, value, ttl=None, nx=True):
         ttl = ttl if ttl else self.__ttl
 
         resp = self.instance.set(
-            key, value, ex=ttl, nx=True
+            key, value, ex=ttl, nx=nx
         )
 
         if resp is True:
             return key
 
         raise KeyError(f'{key} Exists')
         
@@ -521,14 +523,15 @@
 
     @staticmethod
     def store(
         storage: redis.client.Redis, value: DataFrame, 
         func: callable, *args, 
         ttl=None, nx=True, **kwargs
     ):
+        kwargs = deepcopy(kwargs)
         condition = kwargs.get('condition', False)
         columns = kwargs.get('columns')
 
         if not columns or columns == '*':
             columns = value.columns
 
         if not NewareCacheController.__should_cache(condition, columns): # Partial value is given #TODO, should still be cached
@@ -552,14 +555,15 @@
         except (TypeError, KeyError, redis.ResponseError):
             raise
         
     @staticmethod
     def retrieve(
         storage: redis.client.Redis, func: callable, *args, **kwargs
     ):  
+        kwargs = deepcopy(kwargs)
         condition = kwargs.get('condition', False)
         columns = kwargs.get('columns') # Requested columns
 
         if not columns or columns == '*':
             columns = NW_CACHE_COLUMNS
 
         if not NewareCacheController.__should_cache(condition, columns): # Partial value is given #TODO, value should be retrieved and completed!
@@ -625,28 +629,29 @@
             if not raw and condition and condition.lower() not in ['true', 1]:
                 # Assumption!! If the given condition filters cache it will not contain partial cycle data, and is safe to use!
                 # Any exception raised here means query is meant for value and should not be cached!
                 
                 # if len(cache_data.query(condition).index) == len(cache_data.index): 
                 #     raise ValueError
                 
-                if not isinstance(cache_data.query(condition), DataFrame):
+                if not isinstance(cache_data.query(condition, engine='python'), DataFrame):
                     raise ValueError
 
         except Exception as e:
             return False
 
         return True
 
     @staticmethod
     def store(
         storage: redis.client.Redis, value: DataFrame, 
         func: callable, *args, 
         ttl=None, nx=True, **kwargs
     ):  
+        kwargs = deepcopy(kwargs)
         cache_data, condition = kwargs.get('cache_data'), parse_mysql_to_pandas_query(kwargs.get('condition', ''))
         raw = kwargs.get('raw', False)
         
         if not NewareTestController.__should_cache(cache_data, condition, raw):
             return DefaultStorageController.store(storage, value, func, *args, ttl=43200, nx=nx, **kwargs)
         
         try: 
@@ -675,23 +680,25 @@
         except (TypeError, KeyError, IndexError, UndefinedVariableError, redis.ResponseError):
             raise
 
     @staticmethod
     def retrieve(
         storage: redis.client.Redis, func: callable, *args, **kwargs
     ):  
+        kwargs = deepcopy(kwargs)
         cache_data, condition = kwargs.get('cache_data'), parse_mysql_to_pandas_query(kwargs.get('condition', ''))
-        raw = kwargs.get('raw', False)
+        raw = kwargs.get('raw', False) 
+        temperature = kwargs.get('temperature', False)
         
         if not NewareTestController.__should_cache(cache_data, condition, raw):
             return DefaultStorageController.retrieve(storage, func, *args, **kwargs)
         
         try:
             if condition and condition.lower() not in ['true', 1]:
-                cache_data = cache_data.query(condition) # Only supports query on cache
+                cache_data = cache_data.query(condition, engine='python') # Only supports query on cache
             
             cycles = set(cache_data[NewareTestController.VALUE_GROUP_KEY]) # Ordered by default
             
             partial_key = list(cache_data[NewareTestController.PRIMARY_KEY].iloc[-1]) # A single test so grab any(last) row
             
             keys = [f"{'-'.join(map(str, partial_key))}-{cycle}" for cycle in cycles]
             
@@ -704,18 +711,26 @@
             df = concat(
                 [NewareTestController.__load(cycle, value) for cycle, value in zip(cycles, values)],
                 ignore_index=True
             )
             
             columns = kwargs.get('columns')
             
-            if isinstance(columns, list):
-                df = df[columns]
+            if not isinstance(columns, list): # columns can be * (mysql all) or something invalid
+                columns = df.columns
+
+            if temperature:
+                if cache_data['t1_max'].isnull().all() or cache_data['t2_max'].isnull().all(): # If a value exists in t1/t2_max - Temperature exists for the test!
+                    assert(not df.filter(like='test_tmp').empty) # Since temperature exists, result should contain test_tmp columns
+                    
+                columns += [f'test_tmp{i+1}' for i in range(6)] # There are up to 6 temp channels
+                
+            df.loc[:,df.columns.isin(columns)]
             
-            for column in df.filter(like='test_atime').columns:
+            for column in df.filter(like='test_atime').columns: # Cast test columns to datetime
                 df[column] = df[column].astype('datetime64[ms]')
             
             return df.convert_dtypes()
             
         except (AssertionError, KeyError, IndexError, UndefinedVariableError, redis.ResponseError):
             return DataFrame()
 
@@ -763,29 +778,27 @@
         except (KeyError, AttributeError):
             table = None
 
         if not TableCacheController.__should_cache(table, condition): # Partial value is given #TODO, value should be retrieved and completed!
             return DefaultStorageController.store(storage, value, func, *args, ttl=ttl, nx=nx, **kwargs)
         
         try:
-            resp = storage.json().set(table, Path.root_path(), {},  nx=nx) # Make sure Key exists
-
-            if resp:
-                storage.expire(table, ttl)
+            storage.json().set(table, Path.root_path(), {}, nx=True) # Make sure Key exists
+            storage.expire(table, ttl)
             
             for column, series in value.items():
                 _column = LABEL_TO_COLUMN.get(column, column)
                 
-                resp = storage.json().set(
+                storage.json().set(
                     table, 
                     Path(_column), 
                     loads(series.to_json(orient='values')),
                     nx=nx
                 )
-                        
+                
             return True
 
         except (TypeError, KeyError, IndexError, UndefinedVariableError, redis.ResponseError):
             raise
         
     @staticmethod
     def retrieve(
```

### Comparing `banner-storedot-2.2.9/src/banner/pandas_decorator.py` & `banner-storedot-2.3.0/src/banner/pandas_decorator.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from pandas import DataFrame
 from MySQLdb import MySQLError
 
 from banner.connection import RelationalConnection, Storage
 from banner.queries import Queries
 
 from banner.utils.web2py import JOINS, COLUMN_TO_LABEL
+from banner.utils.misc import to_mysql_tuple
 from banner.utils.pandas import assert_required_columns
 from banner.utils.neware import (
     calculate_current, calculate_dqdv, calculate_neware_columns, 
     calculate_neware_timestamp, calculate_temperature, calculate_neware_datetime,
     calculate_voltage, group_by_auxchl, calculate_capacity, IS_CALCULATED_NEWARE_DF
 )
 
@@ -87,15 +88,15 @@
             f'{df_table}.{column}' if f'{df_table}.{column}' in _df else f'{df_table}.{COLUMN_TO_LABEL.get(column)}'
             for column in _left
         ] #Add table prefix
         
         try:
             _keys = _df[_left].dropna() # Keys cannot contain NA values
             _keys = zip(*[_keys[column].values for column in _left]) # as Iterable
-            
+            # the neware cache tables contain only numeric values
             if table == 'neware_cache':
                 table_df = Queries.neware_cache_query(
                     list(_keys), columns=columns, condition=condition, 
                     connection=connection, cache=cache, ttl=ttl,
                     **kwargs
                 )
 
@@ -110,15 +111,16 @@
                 table_df = Queries.neware_cache_anode_query(
                     list(_keys), columns=columns, condition=condition, 
                     connection=connection, ttl=ttl,
                     **kwargs
                 )
 
             else:
-                _keys = [f"({','.join([str(value) for value in values])})" for values in _keys] # as Iterable of strings
+                # keys may contain str values
+                _keys = [to_mysql_tuple(values) for values in _keys] # as Iterable of strings
                 
                 table_df = Queries.table_query(
                     table, columns=columns, condition=f"({','.join(_right)}) IN ({','.join(_keys)}) AND {condition}",
                     represent=represent, raw=raw, connection=connection, cache=cache, ttl=ttl, nx=nx, **kwargs
                 )
             
             table_df.columns = [f'{table}.{column}' for column in table_df.columns] # Prefix columns
@@ -128,15 +130,15 @@
                 for column in _right
             ] #Add table prefix
             
             tables = df._tables + [table]
             
             for left_column, right_column in zip(_left, _right):
                 table_df[right_column] = table_df[right_column].astype(_df[left_column].dtype) # Make sure right_column has same data type as left_column
-              
+            
             _df = _df.merge(
                 table_df, how=_how, 
                 left_on=_left, right_on=_right,
                 # suffixes=(f'_{df_table}', f'_{table}')
             )
             
             _df._tables = tables # Set Current Tables
```

### Comparing `banner-storedot-2.2.9/src/banner/pandas_wrap.py` & `banner-storedot-2.3.0/src/banner/pandas_wrap.py`

 * *Files identical despite different names*

### Comparing `banner-storedot-2.2.9/src/banner/queries.py` & `banner-storedot-2.3.0/src/banner/queries.py`

 * *Files 7% similar despite different names*

```diff
@@ -63,14 +63,15 @@
         if isinstance(con, Storage):
             Queries.CACHE.__CACHE_CONNECTION = con
         
         return Queries.CACHE.__CACHE_CONNECTION
 
     @staticmethod
     def __get_known_connection(connection: Union[Connection, str], typ: type = Connection):
+        ''' Basicly an assertion for a given connection'''
         # If no connection is provided, grab first available
         if not connection:
             connections = [
                 _connection for _connection in Queries.CONNECTIONS().values() if isinstance(_connection, typ)
             ]
 
             if not connections:
@@ -88,14 +89,15 @@
 
         if not isinstance(connection, typ):
             raise TypeError('Wrong Connection type', connection)
 
         return connection
 
     def __cache_query(value, cache: Storage, func: callable, args, ttl, nx, kwargs):
+        ''' Handle caching of self(Queries) into provided cache'''
         try:
             assert(isinstance(cache, Storage))
             
             return cache.store(
                 value, 
                 func, 
                 *args,
@@ -105,48 +107,56 @@
             )
 
         except AssertionError:
             pass
         
         except Exception as e:
             exception_message = f'Failed Caching {func.__name__}:{args}{kwargs} into {cache} - {type(e).__name__}:{e}'
-            print(exception_message) #TODO add flag for print/exception
+            print(exception_message) #TODO add flag for print(to stdout, which could be a provided log path)/exception
             # raise ValueError(message) from e
     
     def __cached_query(cache: Storage, func: callable, *args, **kwargs):
+        ''' Get the cached value of Queries.func if exists inside provided cache'''
         try:
             assert(isinstance(cache, Storage))
             
             cached = cache.retrieve(
                 func, *args, **kwargs
             )
             
             return cached
 
         except AssertionError:
             return pd.DataFrame()
 
     def __cache(func):
+        ''' 
+            Decorator for handling caching interaction, 
+            A decorated Queries function will first check if its value exists in the provided cache,
+            if exists -> return value
+            if not exists -> calculate, cache and return value
+        '''
         @wraps(func)
         def inner(*args, **kwargs):
             cache = kwargs.pop(CACHE_CONNECTION_KWARG, None)
 
             if cache is None: # Specifically checking for None, If False Do not cache!
-                cache = Queries.CACHE()
+                cache = Queries.CACHE() # None cache is provided, try to get the default one
             
-            ttl = kwargs.pop(TTL_KWARG, None)
-            nx = kwargs.pop(NX_KWARG, True)
+            ttl = kwargs.pop(TTL_KWARG, None) # kwargs of the func
+            nx = kwargs.pop(NX_KWARG, True) # args of the func
             
-            value = Queries.__cached_query(cache, func, *args, **kwargs)
-            cached = True if isinstance(value, pd.DataFrame) and not value.empty else False # TODO READ TYPE HINT FROM FUNC AND CHECK IF CACHE RESULT MATCHES
+            value = Queries.__cached_query(cache, func, *args, **kwargs) # the cached value
+            # TODO READ TYPE HINT FROM FUNC AND CHECK IF CACHE RESULT MATCHES TO SUPPORT ALL TYPE OF CACHING
+            is_cached = True if isinstance(value, pd.DataFrame) and not value.empty else False
             
-            if not cached or not nx:
-                value = func(*args, **kwargs)
+            if not is_cached or not nx: # value should be cached if it is not yet cached, or if nx=False (forcing a rewrite into cache)
+                value = func(*args, **kwargs) # calculate the value
             
-                # Cache TODO USE CELERY
+                # TODO Caching should be done using a suitable pkg (ex. CELERY)
                 Thread(
                     target=Queries.__cache_query, 
                     kwargs=dict(
                         value=value,
                         cache=cache,
                         func=func,
                         args=args,
@@ -158,14 +168,15 @@
             
             return value
         
         return inner
 
     @staticmethod
     def __query(query: str, connection=None, cache=None, ttl=None, w2p_parse=True) -> pd.DataFrame:
+        ''' direct str sql query without caching '''
         if not isinstance(query, str):
             return pd.DataFrame()
 
         connection = Queries.__get_known_connection(connection)
         
         if w2p_parse:
             query = parse_w2p_to_mysql_query(query)
@@ -248,15 +259,15 @@
         if not isinstance(table, str):
             return pd.DataFrame()
 
         connection = Queries.__get_known_connection(connection, RelationalConnection)
         
         data = connection.describe(table)
         
-        data.insert(0, "Label", data['Field'].map(W2P_COLUMN_TO_LABEL))
+        data.insert(0, "Label", data['Field'].map(W2P_COLUMN_TO_LABEL)) # TODO W2P_COLUMN_TO_LABEL per table
 
         return data
 
     @staticmethod
     def describe(connection: Union[RelationalConnection, str] = None) -> pd.DataFrame:
         '''
             Describe Table names in connection
@@ -277,29 +288,29 @@
             Queries a given connection for 'SELECT {columns} FROM {table} WHERE {condition}'
             Accepts both column values and labels
             raw=True - column names as in db
             Queries a given Connection(ip)/str of a known connection (or first known) return result as DataFrame
             Cache if cache or first known with ttl or default ttl for cache
             Raises OperationalError and KeyError(Failed to find a connection for given key) 
         '''
-        if isinstance(columns, str):
+        if isinstance(columns, str): # Handle columns as str
             columns = list(
                 map(
                     str.strip,
                     filter(
                         None, 
                         split(
                             ' , |, | ,|,',
                             columns
                         )
                     )
                 )
             )
         
-        _columns = [W2P_LABEL_TO_COLUMN.get(column, column) for column in columns]
+        _columns = [W2P_LABEL_TO_COLUMN.get(column, column) for column in columns] # Get the actual column name (support Labels)
         
         data = Queries.__query(
             f"SELECT {', '.join(_columns)} FROM {table} WHERE {condition}",
             connection=connection,
             cache=cache,
             ttl=ttl
         )
@@ -310,27 +321,27 @@
                 data.columns = columns 
 
             except ValueError:
                 # Case columns contain *
                 data.columns = [W2P_COLUMN_TO_LABEL.get(column, column) for column in data.columns]
                 pass
             
-        data._tables = [table]
+        data._tables = [table] # add _tables METADATA, indicating this dataframe represents a web2py table, allowing future joins
         
         if represent:
-            data = w2p_repr(data)
+            data = w2p_repr(data) # Add column representation as they appear in web2py
 
         return data
 
     @staticmethod
     @__cache
     def neware_query(
         device: int, unit: int, channel: int, test: int, connection: Union[MySqlConnection, str] = None, 
         columns: Union[list, str] = [NW_UNIT, NW_CHANNEL, NW_TEST, NW_CYCLE, NW_SEQ, NW_STEP, NW_STEP_TYPE, NW_TIMESTAMP, NW_VOLTAGE, NW_CURRENT], 
-        condition: str = 'TRUE', raw: bool = False, dqdv: bool = False, temperature: bool = False,
+        condition: str = 'TRUE', neware_condition: str = 'TRUE', raw: bool = False, dqdv: bool = False, temperature: bool = False,
         cache_data: pd.DataFrame = pd.DataFrame(), cache: Storage = None, ttl: int = None,
     ) -> pd.DataFrame:
         '''
             Queries a given Connection(ip)/str of a known connection (or first known) return result as DataFrame
             Cache if cache or first known with ttl or default ttl for cache
             If dqdv -> neware.calc_dq_dv
             Raises KeyError and OperationalError
@@ -386,41 +397,43 @@
         required_columns = set([
             NW_SEQ, NW_TIMESTAMP, NW_STEP_RANGE, NW_VOLTAGE, NW_CURRENT, *nw_columns
         ]) # The actually needed columns (requested + required) 
         
         required_columns = ', '.join(required_columns) # to string
         
         first_data = Queries.__query(
-            f'SELECT {required_columns} FROM {first_main_table} WHERE unit_id = {unit} AND chl_id = {channel} AND test_id = {test} AND {condition}', 
+            f'SELECT {required_columns} FROM {first_main_table} WHERE unit_id = {unit} AND chl_id = {channel} AND test_id = {test} AND ({condition} AND {neware_condition})', 
             connection=connection
         )
 
         second_data = Queries.__query(
-            f'SELECT {required_columns} FROM {second_main_table} WHERE unit_id = {unit} AND chl_id = {channel} AND test_id = {test} AND {condition}', 
+            f'SELECT {required_columns} FROM {second_main_table} WHERE unit_id = {unit} AND chl_id = {channel} AND test_id = {test} AND ({condition} AND {neware_condition})', 
             connection=connection
         ) if second_main_table else pd.DataFrame() # There is a second main table for the test
 
         if temperature: # Temperature requested
             nw_aux_columns = ', '.join(NW_AUX_SIGNIFICANT_COLUMNS)
 
             if not first_data.empty: # If we have data in first_data then we will have from first_aux_table
                 first_aux_data = Queries.__query(
-                    f'SELECT {nw_aux_columns} FROM {first_aux_table} WHERE unit_id = {unit} AND chl_id = {channel} AND test_id = {test} AND {condition}', 
+                    f'SELECT {nw_aux_columns} FROM {first_aux_table} WHERE unit_id = {unit} AND chl_id = {channel} AND test_id = {test} AND ({condition} AND {neware_condition})', 
                     connection=connection
                 )
 
                 if not first_aux_data.empty:
                     first_data = pd.merge(first_data, first_aux_data, on=NW_SEQ) # Merge Aux from first_aux_table
 
             if second_aux_table and not second_data.empty: # There is a second aux table for the test and we have data in second_data then we will have from second_aux_table
                 second_aux_data = Queries.__query(
-                    f'SELECT {nw_aux_columns} FROM {second_aux_table} WHERE unit_id = {unit} AND chl_id = {channel} AND test_id = {test} AND {condition}', 
+                    f'SELECT {nw_aux_columns} FROM {second_aux_table} WHERE unit_id = {unit} AND chl_id = {channel} AND test_id = {test} AND ({condition} AND {neware_condition})', 
                     connection=connection
                 )
-                second_data = pd.merge(second_data, second_aux_data, on=NW_SEQ) # Merge Aux from second_aux_table
+
+                if not second_aux_data.empty:
+                    second_data = pd.merge(second_data, second_aux_data, on=NW_SEQ) # Merge Aux from second_aux_table
 
         # Into a single Dataframe
         data = pd.concat([first_data, second_data], ignore_index=True)
 
         try:
             data = data.group_by_auxchl() # Banner method, neware.group_by_auxchl
             nw_columns.extend([column for column in data.columns if column.startswith(NW_TEMP)]) # nw_columns add temp columns
@@ -444,18 +457,19 @@
         data = data[[*nw_columns, *nw_cache_columns]] # Keep requested columns
             
         return data
         
     @staticmethod
     def __neware_queries(
         devices: list, units: list, channels: list, tests: list, connection: Union[MySqlConnection, str] = None, 
-        columns: Union[list, str] = [NW_UNIT, NW_CHANNEL, NW_TEST, NW_CYCLE, NW_SEQ, NW_STEP, NW_STEP_TYPE, NW_TIMESTAMP, NW_VOLTAGE, NW_CURRENT], condition: str = 'TRUE',  
-        temperature: bool = False, dqdv: bool = False, cache_data: pd.DataFrame = pd.DataFrame(),
+        columns: Union[list, str] = [NW_UNIT, NW_CHANNEL, NW_TEST, NW_CYCLE, NW_SEQ, NW_STEP, NW_STEP_TYPE, NW_TIMESTAMP, NW_VOLTAGE, NW_CURRENT], 
+        condition: str = 'TRUE', neware_condition: str = 'TRUE', temperature: bool = False, dqdv: bool = False, cache_data: pd.DataFrame = pd.DataFrame(),
         cache: Storage = None, ttl: int = None, raw: bool = False, 
     ):  
+        ''' This function gets multiple neware pks and their cache_data(df) calls neware_query per requested test with its relevant cache'''
         _connection_key = connection
 
         if isinstance(connection, Connection):
             _connection_key = str(_connection_key.name)
 
         data = dict()
         
@@ -466,48 +480,54 @@
                         device, unit, channel, test,
                         connection=connection,
                         cache=cache,
                         ttl=ttl,
                         raw=raw, 
                         dqdv=dqdv, 
                         condition=condition,
+                        neware_condition=neware_condition,
                         columns=columns,
                         temperature=temperature, 
                         cache_data=cache_data[
                             (cache_data.dev_uid == int(device)) &
                             (cache_data.unit_id == int(unit)) & 
                             (cache_data.chl_id == int(channel)) & 
                             (cache_data.test_id == int(test))
                         ]
                     )
                 })
 
             except (TypeError, KeyError, ValueError):
-                pass
+                pass #TODO ADD LOGGING
         
         return data
 
     @staticmethod
     def neware_cache_query(
         keys: Iterable, columns: Union[list, str] = '*', pulse: bool = False, anode: bool = False, condition: str = 'TRUE', 
         connection: Union[MySqlConnection, str] = None, cache: Storage = None, ttl: int = None
     ) -> pd.DataFrame:
+        ''' 
+            Query neware cache tables by iterable of keys, looking at neware_cache
+            pulse flag on will look at neware_pulses_cache switching (removing the neware_cache entries) any pks found in the table into the result
+            anode does the same as pulse with neware_cache_anode table
+        '''
         neware_cache = Queries._neware_cache_query(
             keys, columns=columns, condition=condition, connection=connection, cache=cache, ttl=ttl
-        )
+        ) # fetch neware_cache data
        
         neware_cache_pulse = Queries.neware_cache_pulse_query(
             keys, columns=columns, condition=condition, connection=connection, cache=cache, ttl=ttl
-        ) if pulse else pd.DataFrame()
+        ) if pulse else pd.DataFrame() # fetch neware_pulses_cache data
 
         neware_cache_pulse['pulse'] = 1 # It is a pulse
 
         neware_cache_anode = Queries.neware_cache_anode_query(
             keys, columns=columns, condition=condition, connection=connection, cache=cache, ttl=ttl
-        ) if anode else pd.DataFrame()
+        ) if anode else pd.DataFrame() # fetch neware_cache_anode data
         
         neware_cache_anode['anode'] = 1 # It is an anode
         
         neware_cache = pd.concat(
             [neware_cache, neware_cache_pulse, neware_cache_anode], 
             ignore_index=True
         ) # Concat data
@@ -538,14 +558,15 @@
         
     @staticmethod
     @__cache
     def _neware_cache_query(
         keys: Iterable, columns: Union[list, str] = '*', condition: str = 'TRUE', connection: Union[MySqlConnection, str] = None,
         cache: Storage = None, ttl: int = None
     ) -> pd.DataFrame:
+        ''' cache decorated __neware_cache_query for neware_cache table'''
         return Queries.__neware_cache_query(
             'neware_cache', keys, columns=columns, condition=condition, connection=connection, cache=cache, ttl=ttl
         )
 
     @staticmethod
     def neware_cache_anode_query(
         keys: Iterable, columns: Union[list, str] = '*', condition: str = 'TRUE', connection: Union[MySqlConnection, str] = None,
@@ -585,15 +606,15 @@
                 _keys = [tuple(key) for key in keys] # Make sure each key(collection) is a tuple
                 
             else:
                 _keys = [tuple(keys)] # Single entry was given
             
             _keys = [
                 f'({ip},{device},{unit},{channel},{test})' for ip, device, unit, channel, test in _keys
-            ]
+            ] # mysql entries
 
         except (TypeError, ValueError):
             raise ValueError(f'Bad Input, Expected List(Tuple)')
         
         _keys = f'(ip,dev_uid,unit_id,chl_id,test_id) IN ({",".join(_keys)})'
         
         if not isinstance(columns, str):
@@ -612,15 +633,15 @@
 
         return cache_data
 
     @staticmethod
     def __neware_tests_query(
         table: str, experiments: str = '', templates: str = '', tests: str = '', cells: str = '', 
         columns: Union[list, str] = [NW_UNIT, NW_CHANNEL, NW_TEST, NW_CYCLE, NW_SEQ, NW_STEP, NW_STEP_TYPE, NW_TIMESTAMP, NW_VOLTAGE, NW_CURRENT],
-        condition: str = 'TRUE', raw: bool = False, dqdv: bool = False, temperature: bool = False, 
+        condition: str = 'TRUE', neware_condition: str = 'TRUE', raw: bool = False, dqdv: bool = False, temperature: bool = False, 
         connection: Union[MySqlConnection, str] = None, cache: Storage = None, ttl: int = None
     ):  
         if not any([experiments, templates, tests, cells]):
             raise ValueError('A combination of experiments, templates, tests, cells is Required')
         
         connection = Queries.__get_known_connection(connection, MySqlConnection)
 
@@ -669,41 +690,41 @@
         
         __tests_by_ip = __tests.groupby('ip')
         
         data = Parallel(n_jobs=__tests_by_ip.ngroups, require='sharedmem', verbose=0)(
             delayed(Queries.__neware_queries)(
                 df['device'].values, df['unit'].values, df['channel'].values, df['test_id'].values,
                 connection=name, cache=cache, ttl=ttl, raw=raw, columns=columns,
-                dqdv=dqdv, condition=condition, temperature=temperature,
+                dqdv=dqdv, condition=condition, neware_condition=neware_condition, temperature=temperature,
                 cache_data=__cached_data[__cached_data.ip == int(name)]
             )
             for name, df in __tests_by_ip
         )
         
         return dict(ChainMap(*data))
 
     @staticmethod
     def neware_tests_query(
         table: str, experiments: Union[list, Number, str] = [], templates: Union[list, Number, str] = [], 
         tests: Union[list, Number, str] = [], cells: Union[list, Number, str] = [], 
         columns: Union[list, str] = [NW_UNIT, NW_CHANNEL, NW_TEST, NW_CYCLE, NW_SEQ, NW_STEP, NW_STEP_TYPE, NW_TIMESTAMP, NW_VOLTAGE, NW_CURRENT], 
-        condition: str = 'cycle < 2', raw: bool = False, dqdv: bool = False, temperature: bool = False,
+        condition: str = 'cycle < 2', neware_condition: str = 'TRUE', raw: bool = False, dqdv: bool = False, temperature: bool = False,
         connection: Union[MySqlConnection, str] = None, cache: Storage = None, ttl: int = None
     ):
         if not any([experiments, templates, tests, cells]):
             raise ValueError('A combination of experiments, templates, tests, cells is Required')
         
         experiments = experiments_to_sql(table, experiments)
         templates = templates_to_sql(f'{table}_test_template', templates)
         cells = cells_to_sql(table, cells)
         tests = tests_to_sql(f'{table}_test', tests)
          
         return Queries.__neware_tests_query(
             table, experiments, templates, 
-            tests, cells, columns, condition, raw, 
+            tests, cells, columns, condition, neware_condition, raw, 
             dqdv, temperature, connection, cache, ttl
         )
     
     @staticmethod
     @__cache
     def test_tables_query(
         table: str, experiments: Union[list, Number, str] = [], templates: Union[list, Number, str] = [], 
@@ -755,86 +776,105 @@
             h_test = Queries.__query(
                 f"""
                     SELECT {neware_keys_as_str}, {FIRST_NEWARE_DATA_TABLE}, {SECOND_NEWARE_DATA_TABLE}, {FIRST_NEWARE_AUX_TABLE}, {SECOND_NEWARE_AUX_TABLE}
                     FROM h_test WHERE {condition}
                 """,
                 connection=group.name
             ) # Select relevant data from h_test of neware (group.name)
-            
-            if not h_test.empty:
-                group = group.merge(
-                    h_test,
-                    left_on=keys,
-                    right_on=neware_keys
-                ) # Merge h_test into group
 
-            return group
+            if not h_test.empty:
+                h_test['ip'] = group.name
 
+            return h_test
+        
         __data = __data.apply(pd.to_numeric) # Ensure all columns are numeric, device column might be string
-        __data = __data.groupby('ip').apply(__query_h_test) # Add neware tables
-
+        __h_test_data = __data.groupby('ip').apply(__query_h_test).reset_index(drop=True) # Add neware tables
+        
         keys.insert(0 , 'ip')
         neware_keys.insert(0 , 'ip')
+        
+        if not __h_test_data.empty:
+            __data = __data.merge(
+                __h_test_data,
+                left_on=keys,
+                right_on=neware_keys
+            ) # Merge h_test into group
+            
         values = [tpl for tpl in __data[keys].itertuples(index=False, name=None)]
 
         # Set cache tables to False
         __data.assign(
             neware_cache=False, neware_pulses_cache=False, neware_cache_anode=False
         )
-
+        
         neware_cache = Queries.neware_cache_query(values, columns=neware_keys, condition='cycle <= 1') # Only single row per test
 
         if not neware_cache.empty:
             neware_cache['neware_cache'] = True
 
             __data = __data.merge(
                 neware_cache,
                 left_on=keys,
-                right_on=neware_keys
+                right_on=neware_keys,
+                how='left'
             ) # Merge neware_cache
-            
+
+            __data['neware_cache'].replace(to_replace=np.nan, value=False, inplace=True)
+        
         neware_cache_pulse = Queries.neware_cache_pulse_query(values, columns=neware_keys, condition='cycle <= 1') # Only single row per test
 
         if not neware_cache_pulse.empty:
             neware_cache_pulse['neware_pulses_cache'] = True
 
             __data = __data.merge(
                 neware_cache_pulse,
                 left_on=keys,
-                right_on=neware_keys
+                right_on=neware_keys,
+                how='left'
             ) # Merge neware_cache_pulse
-            
+
+            __data['neware_pulses_cache'].replace(to_replace=np.nan, value=False, inplace=True)
+        
         neware_cache_anode = Queries.neware_cache_anode_query(values, columns=neware_keys, condition='cycle <= 1') # Only single row per test
 
         if not neware_cache_anode.empty:
             neware_cache_anode['neware_cache_anode'] = True
 
             __data = __data.merge(
                 neware_cache_anode,
                 left_on=keys,
-                right_on=neware_keys
+                right_on=neware_keys,
+                how='left'
             ) # Merge neware_cache_anode
+
+            __data['neware_cache_anode'].replace(to_replace=np.nan, value=False, inplace=True)
         
         return __data[__data.columns.intersection([
             'id', *keys, 'neware_cache', 'neware_pulses_cache', 'neware_cache_anode',
             FIRST_NEWARE_DATA_TABLE, SECOND_NEWARE_DATA_TABLE, FIRST_NEWARE_AUX_TABLE, SECOND_NEWARE_AUX_TABLE
         ])]
 
 
 class AugmentQueries(object):
+    # available table keys
     PER_CYCLE_TABLE = 'augm_per_cycle'
+    PER_CYCLE_SNAPPER_TABLE = 'augm_per_cycle_snapper'
     PER_CELL_TABLE = 'augm_per_cell'
     PER_TEST_TABLE = 'augm_per_test'
     PER_PULSE_TABLE = 'augm_per_pulse'
     PER_ANODE_TABLE = 'augm_per_anode'
 
-    TIMESTAMP_FORMAT = "%Y-%m-%d %H:%M:%S"
+    TIMESTAMP_FORMAT = "%Y-%m-%d %H:%M:%S" # web2py timestamp format
 
-    COLUMN_DESCRIPTION_INDEX = '_description'
-    COLUMN_UPDATED_ON_INDEX = '_updated_on'
+    COLUMN_DESCRIPTION_INDEX = '_description' # description column suffix
+    COLUMN_UPDATED_ON_INDEX = '_updated_on' # index column suffix
+
+    PER_CELL_UNIQUE_COLUMNS = ['cell_table', 'cell_id'] # Unique columns (pk) per cell table
+    PER_TEST_UNIQUE_COLUMNS = ['augm_per_cell', 'test_id'] # Unique columns (pk) per test table
+    PER_CYCLE_UNIQUE_COLUMNS = ['augm_per_test', 'ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id', 'cycle'] # Unique columns (pk) per cycle table
 
     def __init__(self, connection: RelationalConnection):
         self._connection = connection
 
         self.prefix = 'augm'
 
         self.per_cycle_table = AugmentQueries.PER_CYCLE_TABLE
@@ -854,27 +894,27 @@
         self.associated_cache_tables = {
             self.per_cycle_table: 'neware_cache',
             self.per_pulse_table: 'neware_pulses_cache',
             self.per_anode_table: 'neware_cache_anode',
         }
         
         self.required_columns_for_table = {
-            self.per_cycle_table: ['augm_per_test', 'ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id', 'cycle'],
-            self.per_pulse_table: ['augm_per_test', 'ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id', 'cycle'],
-            self.per_anode_table: ['augm_per_test', 'ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id', 'cycle'],
-            self.per_cell_table: ['cell_table', 'cell_id'],
-            self.per_test_table: ['augm_per_cell', 'test_id'],
+            self.per_cycle_table: AugmentQueries.PER_CYCLE_UNIQUE_COLUMNS,
+            self.per_pulse_table: AugmentQueries.PER_CYCLE_UNIQUE_COLUMNS,
+            self.per_anode_table: AugmentQueries.PER_CYCLE_UNIQUE_COLUMNS,
+            self.per_cell_table: AugmentQueries.PER_CELL_UNIQUE_COLUMNS,
+            self.per_test_table: AugmentQueries.PER_TEST_UNIQUE_COLUMNS,
         }
 
         self.primary_columns = ['cell_table', 'cell_id', 'test_id', 'cycle']
 
 
     def __assert_table(self, table: str):
         if table not in self.tables:
-            raise ValueError(f'Available Augment Tables: {self.tables}')
+            raise ValueError(f'Available {self.__class__.__name__} Tables: {self.tables}')
     
     def get_keys_per_table(self, data: pd.DataFrame, table: str):
         columns = self.required_columns_for_table.get(table)
         
         return [str(tuple(row)) for _, row in data[columns].iterrows()]
  
     def set_features(self, table: str, features: pd.DataFrame, columns: list, validate=True): # TABLE, CELL, TEST_ID, CYCLE 
@@ -884,43 +924,39 @@
         _columns = self.primary_columns + columns
         
         features = features[features.columns.intersection(set(_columns))]
         
         if validate:
             features = self.__filter_non_existant(table, features)
         
-        try:
-            keys = self.get_keys_per_table(features, self.per_cell_table)
+        keys = self.get_keys_per_table(features, self.per_cell_table)
+        
+        self.__create_rows_per_table(keys, self.per_cell_table) # Create Per Cell Rows!
+        
+        features = features.merge(
+            self.__get_per_table_rows(keys, self.per_cell_table), # Relevant Rows
+            how='left', on=self.required_columns_for_table.get(self.per_cell_table)
+        ) # Add params
+        
+        if table != self.per_cell_table: # Tests/Cycles/Pulses/Anode
+            keys = self.get_keys_per_table(features, self.per_test_table)
             
-            self.__create_rows_per_table(keys, self.per_cell_table) # Create Per Cell Rows!
+            self.__create_rows_per_table(keys, self.per_test_table) # Create Per Test Rows!
             
             features = features.merge(
-                self.__get_per_table_rows(keys, self.per_cell_table), # Relevant Rows
-                how='left', on=self.required_columns_for_table.get(self.per_cell_table)
+                self.__get_per_table_rows(keys, self.per_test_table), # Relevant Rows
+                how='left', 
+                on=self.required_columns_for_table.get(self.per_test_table)
             ) # Add params
             
-            if table != self.per_cell_table: # Tests/Cycles/Pulses/Anode
-                keys = self.get_keys_per_table(features, self.per_test_table)
-                
-                self.__create_rows_per_table(keys, self.per_test_table) # Create Per Test Rows!
+            if table != self.per_test_table: # Cycles/Pulses/Anode
+                features = self.__create_and_get_rows_per_cycle_pulse_or_anode(features, table)
                 
-                features = features.merge(
-                    self.__get_per_table_rows(keys, self.per_test_table), # Relevant Rows
-                    how='left', 
-                    on=self.required_columns_for_table.get(self.per_test_table)
-                ) # Add params
-                
-                if table != self.per_test_table: # Cycles/Pulses/Anode
-                    features = self.__create_and_get_rows_per_cycle_pulse_or_anode(features, table)
-                    
-            for part in features.split(): # Banner function 
-                self.__set_feature(table, part, columns) # Set feature into table
-        
-        except KeyError:
-            pass
+        for part in features.split(): # Banner function 
+            self.__set_feature(table, part, columns) # Set feature into table
         
     def add_feature(self, table: str, name: str, dtype: str, index=False, description=False, updated_on=False):
         self.__assert_table(table)
         
         self.__add_column(table, name, dtype)
 
         if index:
@@ -1008,27 +1044,29 @@
         
         Queries.simple_edit(
             query, values, connection=self._connection
         )
 
     def __create_and_get_rows_per_cycle_pulse_or_anode(self, data: pd.DataFrame, table: str):
         cache_table = self.associated_cache_tables[table]
+        cache_kwargs = dict(anode=True, pulse=True) if cache_table == 'neware_cache' else {}
         columns = ['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id', 'cycle']
         cache_columns = {f'{cache_table}.{column}': column for column in columns}
         
         def __create_augm_per_pk(group):
             test_table = f'{group.name}_test'
             
             try:
                 data = Queries.table_query(
                     test_table, raw=True,
                     columns=['id', 'ip', 'device', 'unit', 'channel', 'test_id'], 
                     condition=f"id IN ({', '.join(group['test_id'].astype(str))})"
                 ).join_table(
-                    cache_table, columns=columns
+                    cache_table, columns=columns,
+                    **cache_kwargs
                 )
                 
                 joined_group = group.merge(data, how='inner', left_on=['test_id', 'cycle'], right_on=[f'{test_table}.id', f'{cache_table}.cycle'])
                 joined_group[f'{cache_table}.dev_uid'] = pd.to_numeric(joined_group[f'{cache_table}.dev_uid']) # device is originally a string
                 joined_group.drop(columns, inplace=True, axis=1, errors='ignore')
                 joined_group.rename(columns=cache_columns, inplace=True)
                 
@@ -1103,15 +1141,19 @@
     PER_CYCLE_REGRESSORS_TABLE = 'prediction_per_cycle_regressors'
     PER_CYCLE_CLASSIFIERS_TABLE = 'prediction_per_cycle_classifiers'
     PER_CELL_TABLE = 'prediction_per_cell'
     PER_TEST_TABLE = 'prediction_per_test'
     PER_PULSE_TABLE = 'prediction_per_pulse'
     PER_ANODE_TABLE = 'prediction_per_anode'
     PREDICTOR_TABLE = 'predictor'
-    
+
+    PER_CELL_UNIQUE_COLUMNS = ['cell_table', 'cell_id', 'predictor'] # Unique columns (pk) per cell table
+    PER_TEST_UNIQUE_COLUMNS = ['prediction_per_cell', 'test_id', 'predictor'] # Unique columns (pk) per test table
+    PER_CYCLE_UNIQUE_COLUMNS = ['prediction_per_test', 'ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id', 'cycle', 'predictor'] # Unique columns (pk) per cycle table
+
     def __init__(self, connection: RelationalConnection):
         self._connection = connection
 
         self.prefix = 'prediction'
 
         self.per_cycle_regressors_table = PredictionQueries.PER_CYCLE_REGRESSORS_TABLE
         self.per_cycle_classifiers_table = PredictionQueries.PER_CYCLE_CLASSIFIERS_TABLE
@@ -1124,59 +1166,77 @@
 
         self.tables = (
             self.per_cycle_regressors_table,
             self.per_cycle_classifiers_table,
             self.per_cell_table,
             self.per_test_table,
             self.per_pulse_table,
-            self.per_anode_table
+            self.per_anode_table,
+            self.predictor_table
         )
 
         self.associated_cache_tables = {
             self.per_cycle_regressors_table: 'neware_cache',
             self.per_cycle_classifiers_table: 'neware_cache',
             self.per_pulse_table: 'neware_pulses_cache',
             self.per_anode_table: 'neware_cache_anode',
         }
 
         self.required_columns_for_table = {
-            self.per_cycle_regressors_table: ['prediction_per_test', 'ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id', 'cycle', 'predictor'],
-            self.per_cycle_classifiers_table: ['prediction_per_test', 'ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id', 'cycle', 'predictor'],
-            self.per_pulse_table: ['prediction_per_test', 'ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id', 'cycle', 'predictor'],
-            self.per_anode_table: ['prediction_per_test', 'ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id', 'cycle', 'predictor'],
-            self.per_cell_table: ['cell_table', 'cell_id', 'predictor'],
-            self.per_test_table: ['prediction_per_cell', 'test_id', 'predictor'],
+            self.per_cycle_regressors_table: PredictionQueries.PER_CYCLE_UNIQUE_COLUMNS,
+            self.per_cycle_classifiers_table: PredictionQueries.PER_CYCLE_UNIQUE_COLUMNS,
+            self.per_pulse_table: PredictionQueries.PER_CYCLE_UNIQUE_COLUMNS,
+            self.per_anode_table: PredictionQueries.PER_CYCLE_UNIQUE_COLUMNS,
+            self.per_cell_table: PredictionQueries.PER_CELL_UNIQUE_COLUMNS,
+            self.per_test_table: PredictionQueries.PER_TEST_UNIQUE_COLUMNS,
         }
 
         self.primary_columns = ['cell_table', 'cell_id', 'test_id', 'cycle', 'predictor']
 
         self.unique_columns = ['name', 'version']
-        self.nullable_columns = ['create_date', 'blob_type', 'features', 'cycling_application_point', 'target']
-    
+
         self.model_column = 'model'
 
     def set_update_predictors(self, predictors: pd.DataFrame):
-        _predictors = predictors[predictors.columns.intersection(set(self.unique_columns + self.nullable_columns))]
+        predictor_columns = Queries.describe_table('predictor', connection=self._connection)['Field'].values
+
+        _predictors = predictors[predictors.columns.intersection(set(predictor_columns))] # Intersection of given columns with available columns
         
-        on_duplicate = [f'{column}=VALUES({column})' for column in _predictors.columns]
+        _predictors = _predictors.loc[:,~_predictors.columns.str.endswith('updated_on')] # updated_on columns should not be set manually
+        
+        updated_on_columns = list() # list of updated_on columns
+
+        # Find if a column has an updated_on column
+        for column in _predictors.columns:
+            if (column_updated_on_index := f'{column}{PredictionQueries.COLUMN_UPDATED_ON_INDEX}') in predictor_columns:
+                updated_on_columns.append(column_updated_on_index)
+                
+        _predictors = _predictors.assign(**{
+            column: datetime.now().strftime(AugmentQueries.TIMESTAMP_FORMAT) for column in updated_on_columns
+        }) # Add updated_on column
         
-        keys = [str(tuple(row)) for _, row in _predictors.iterrows()]
+        if self.model_column in predictors:
+            _predictors.drop(self.model_column, inplace=True, axis=1) # model is a glob(binary) column, it is handled by itself
 
+        on_duplicate = [f'{column}=VALUES({column})' for column in _predictors.columns] # How to handle duplicate
+        
+        keys = [str(tuple(row)) for _, row in _predictors.iterrows()] # as mysql tuples
+        
         Queries.simple_edit(
             f"""
                 INSERT INTO {self.predictor_table} ({",".join(_predictors.columns)}) 
                 VALUES {",".join(keys)}
                 ON DUPLICATE KEY
                 UPDATE {",".join(on_duplicate)};
             """,
             connection=self._connection
-        )
+        ) # Insert/Update
         
-        if self.model_column in predictors:
+        if self.model_column in predictors: # handle model column
             for _, row in predictors[[*self.unique_columns, self.model_column]].iterrows():
                 name, version = row[self.unique_columns]
                 model = row[self.model_column]
-
+                
                 Queries.simple_edit(
                     """UPDATE predictor SET model=%s WHERE name=%s AND version=%s""" , (model, name, version),
                     connection=self._connection
-                )
+                ) # Update since rows should exist by now
```

### Comparing `banner-storedot-2.2.9/src/banner/utils/const.py` & `banner-storedot-2.3.0/src/banner/utils/const.py`

 * *Files identical despite different names*

### Comparing `banner-storedot-2.2.9/src/banner/utils/misc.py` & `banner-storedot-2.3.0/src/banner/utils/misc.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,8 +52,15 @@
             )
         )
     )
 
 def query_df_by_dict(df: DataFrame, query: dict):
     _query = ' & '.join([f'{key}=={value}' for key, value in query.items()])
 
-    return df.query(_query)
+    return df.query(_query, engine='python')
+
+def to_mysql_tuple(tpl: tuple):
+    _tpl = tuple(
+        f'"{val}"' if isinstance(val, str) else str(val) for val in tpl
+    )
+    
+    return f"({','.join(_tpl)})"
```

### Comparing `banner-storedot-2.2.9/src/banner/utils/neware.py` & `banner-storedot-2.3.0/src/banner/utils/neware.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,26 +64,29 @@
     
     return df
 
 def group_by_auxchl(df: pd.DataFrame):
     ''' 
         Group by auxchl_id set test_temp to auxchl_num
     '''
-    merge_columns = [column for column in list(df.columns) if column not in [NW_TEMP, NW_AUX_CHANNEL]]
-    
     assert_required_columns(df, NW_TEMP, NW_AUX_CHANNEL)
-    
-    def _by_aux_channel(group):
-        group = group.rename(
-            columns={NW_TEMP: f'{NW_TEMP}{group.name}'}
-        ).drop(NW_AUX_CHANNEL, axis=1, errors='ignore')
-        
-        return group
 
-    return df.groupby([NW_AUX_CHANNEL]).apply(_by_aux_channel)
+    merge_columns = [column for column in list(df.columns) if column not in [NW_TEMP, NW_AUX_CHANNEL]]
+    # TODO perhaps use pivot for faster calculation
+    group_as_list = [
+        _df.loc[
+            :, _df.columns != NW_AUX_CHANNEL
+        ].rename(columns={NW_TEMP: f'{NW_TEMP}{name}'})
+        for name, _df in df.groupby(NW_AUX_CHANNEL)
+    ]
+
+    return reduce(
+        lambda left,right: pd.merge(left, right, on=merge_columns, how='left'),
+        group_as_list
+    )
 
 def calculate_temperature(df: pd.DataFrame):
     ''' 
         Calculate temp from test_temp
     '''
     assert_required_columns(df, NW_TEMP)
     
@@ -246,15 +249,15 @@
 
 def query_cache(df: pd.DataFrame, query: str):
     ''' 
         Query df and returnes seq_id ranges
     '''
     try:
         df_by_query = df.query(
-            parse_mysql_to_pandas_query(query)
+            parse_mysql_to_pandas_query(query), engine='python'
         )
         
         ranges = [__query_cache_by_group(df, group_by_query) for index, group_by_query in df_by_query.groupby(df_by_query.index.to_series().diff().ne(1).cumsum())]
         
         assert(ranges)
 
         return f'({" OR ".join(ranges)})'
```

### Comparing `banner-storedot-2.2.9/src/banner/utils/pandas.py` & `banner-storedot-2.3.0/src/banner/utils/pandas.py`

 * *Files identical despite different names*

### Comparing `banner-storedot-2.2.9/src/banner/utils/web2py.py` & `banner-storedot-2.3.0/src/banner/utils/web2py.py`

 * *Files 16% similar despite different names*

```diff
@@ -212,132 +212,228 @@
 
 # Merge dict
 JOINS = dict(
     neware_cache=dict(
         pilot_pouch_test=dict(left=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], right=['ip', 'device', 'unit', 'channel', 'test_id'], how='left'),
         pouch_test=dict(left=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], right=['ip', 'device', 'unit', 'channel', 'test_id'], how='left'),
         augm_per_cycle=dict(left=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id', 'cycle'], right=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id', 'cycle'], how='inner'),
+        ext_pouch_test=dict(left=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], right=['ip', 'device', 'unit', 'channel', 'test_id'], how='left'),
+        jellyroll_test=dict(left=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], right=['ip', 'device', 'unit', 'channel', 'test_id'], how='left'),
+        coin_anode_test=dict(left=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], right=['ip', 'device', 'unit', 'channel', 'test_id'], how='left'),
+        coin_cathode_test=dict(left=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], right=['ip', 'device', 'unit', 'channel', 'test_id'], how='left'),
+        coin_fc_test=dict(left=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], right=['ip', 'device', 'unit', 'channel', 'test_id'], how='left'),
+        ct_coin_test=dict(left=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], right=['ip', 'device', 'unit', 'channel', 'test_id'], how='left'),
+        bia_cell_test=dict(left=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], right=['ip', 'device', 'unit', 'channel', 'test_id'], how='left'),
+        bic_cell_test=dict(left=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], right=['ip', 'device', 'unit', 'channel', 'test_id'], how='left'),
+        mi_cell_test=dict(left=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], right=['ip', 'device', 'unit', 'channel', 'test_id'], how='left'),
+    ),
+    neware_pulses_cache=dict(
+        pouch_test=dict(right=['ip', 'device', 'unit', 'channel', 'test_id'], left=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], how='inner'),
+        pilot_pouch_test=dict(right=['ip', 'device', 'unit', 'channel', 'test_id'], left=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], how='inner'),
+        ext_pouch_test=dict(right=['ip', 'device', 'unit', 'channel', 'test_id'], left=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], how='inner'),
+        jellyroll_test=dict(right=['ip', 'device', 'unit', 'channel', 'test_id'], left=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], how='inner'),
+        coin_anode_test=dict(right=['ip', 'device', 'unit', 'channel', 'test_id'], left=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], how='inner'),
+        coin_cathode_test=dict(right=['ip', 'device', 'unit', 'channel', 'test_id'], left=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], how='inner'),
+        coin_fc_test=dict(right=['ip', 'device', 'unit', 'channel', 'test_id'], left=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], how='inner'),
+        ct_coin_test=dict(right=['ip', 'device', 'unit', 'channel', 'test_id'], left=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], how='inner'),
+        bia_cell_test=dict(right=['ip', 'device', 'unit', 'channel', 'test_id'], left=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], how='inner'),
+        bic_cell_test=dict(right=['ip', 'device', 'unit', 'channel', 'test_id'], left=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], how='inner'),
+        mi_cell_test=dict(right=['ip', 'device', 'unit', 'channel', 'test_id'], left=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], how='inner'),
+    ),
+    neware_cache_anode=dict(
+        pouch_test=dict(right=['ip', 'device', 'unit', 'channel', 'test_id'], left=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], how='inner'),
+        pilot_pouch_test=dict(right=['ip', 'device', 'unit', 'channel', 'test_id'], left=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], how='inner'),
+        ext_pouch_test=dict(right=['ip', 'device', 'unit', 'channel', 'test_id'], left=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], how='inner'),
+        jellyroll_test=dict(right=['ip', 'device', 'unit', 'channel', 'test_id'], left=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], how='inner'),
+        coin_anode_test=dict(right=['ip', 'device', 'unit', 'channel', 'test_id'], left=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], how='inner'),
+        coin_cathode_test=dict(right=['ip', 'device', 'unit', 'channel', 'test_id'], left=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], how='inner'),
+        coin_fc_test=dict(right=['ip', 'device', 'unit', 'channel', 'test_id'], left=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], how='inner'),
+        ct_coin_test=dict(right=['ip', 'device', 'unit', 'channel', 'test_id'], left=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], how='inner'),
+        bia_cell_test=dict(right=['ip', 'device', 'unit', 'channel', 'test_id'], left=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], how='inner'),
+        bic_cell_test=dict(right=['ip', 'device', 'unit', 'channel', 'test_id'], left=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], how='inner'),
+        mi_cell_test=dict(right=['ip', 'device', 'unit', 'channel', 'test_id'], left=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], how='inner'),
     ),
     pouch=dict(
         pouch_test=dict(left='id', right='pouch_id', how='inner'),
         anode_batch=dict(left='anode_batch_id', right='id', how='left'),
         sd_a_batch=dict(left='sd_a_batch_id', right='id', how='left'),
+        sd_c_batch=dict(left='sd_c_batch_id', right='id', how='left'),
         pouch_anode=dict(left='anode_id', right='id', how='left'),
         cathode_batch=dict(left='cathode_batch_id', right='id', how='left'),
-        sd_c_batch=dict(left='sd_c_batch', right='id', how='left'),
         pouch_cathode=dict(left='cathode_id', right='id', how='left'),
         el_batch=dict(left='electrolyte_ct', right='id', how='left'),
+        fa_analysis=dict(left='id', right='pouch_id', how='left'),
+        storage_analysis=dict(left='id', right='cell_id', how='left'),
+        electrolyte_batch=dict(left='electrolyte', right='id', how='left'),
+        el=dict(left='electrolyte_type', right='id', how='left'),
+        track_locations=dict(left='location', right='barcode', how='left'),
     ),
     pouch_test=dict(
         pouch=dict(left='pouch_id', right='id', how='left'),
         pouch_test_template=dict(left='test_type_id', right='id', how='left'),
         neware_cache=dict(left=['ip', 'device', 'unit', 'channel', 'test_id'], right=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], how='inner'),
         neware_pulses_cache=dict(left=['ip', 'device', 'unit', 'channel', 'test_id'], right=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], how='inner'),
         neware_cache_anode=dict(left=['ip', 'device', 'unit', 'channel', 'test_id'], right=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], how='inner'),
     ),
+    pouch_test_template=dict(
+        pouch_test=dict(right='test_type_id', left='id', how='left'),
+    ),
     pilot_pouch=dict(
         pilot_pouch_test=dict(left='id', right='pilot_pouch_id', how='left'),
         pilot_c_batch=dict(left='p_cathode_batch_id', right='id', how='left'),
         pilot_a_batch=dict(left='p_anode_batch_id', right='id', how='left'),
         anode_el_batch=dict(left='anode_el_batch_id', right='id', how='left'),
         cathode_el_batch=dict(left='cathode_el_batch_id', right='id', how='left'),
         pouch_anode=dict(left='anode_id', right='id', how='left'),
         pouch_cathode=dict(left='cathode_id', right='id', how='left'),
         el_batch=dict(left='electrolyte_ct', right='id', how='left'),
+        fa_analysis=dict(left='id', right='pilot_pouch_id', how='left'),
+        storage_analysis=dict(left='id', right='cell_id', how='left'),
+        electrolyte_batch=dict(left='electrolyte', right='id', how='left'),
+        el=dict(left='electrolyte_type', right='id', how='left'),
+        sd_a_batch=dict(left='sd_a_batch_id', right='id', how='left'),
+        sd_c_batch=dict(left='sd_c_batch_id', right='id', how='left'),
+        track_locations=dict(left='location', right='barcode', how='left'),
     ),
     pilot_pouch_test=dict(
         pilot_pouch_test_template=dict(left='test_type_id', right='id', how='left'),
+        pilot_pouch=dict(left='pilot_pouch_id', right='id', how='left'),
         neware_cache=dict(left=['ip', 'device', 'unit', 'channel', 'test_id'], right=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], how='inner'),
         neware_pulses_cache=dict(left=['ip', 'device', 'unit', 'channel', 'test_id'], right=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], how='inner'),
         neware_cache_anode=dict(left=['ip', 'device', 'unit', 'channel', 'test_id'], right=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], how='inner'),
     ),
     ext_pouch=dict(
         ext_pouch_test=dict(left='id', right='ext_pouch_id', how='left'),
         pilot_c_batch=dict(left='p_cathode_batch_id', right='id', how='left'),
         pilot_a_batch=dict(left='p_anode_batch_id', right='id', how='left'),
         anode_el_batch=dict(left='anode_el_batch_id', right='id', how='left'),
         cathode_el_batch=dict(left='cathode_el_batch_id', right='id', how='left'),
         pouch_anode=dict(left='anode_id', right='id', how='left'),
         pouch_cathode=dict(left='cathode_id', right='id', how='left'),
         el_batch=dict(left='electrolyte_ct', right='id', how='left'),
+        fa_analysis=dict(left='id', right='ext_pouch_id', how='left'),
+        storage_analysis=dict(left='id', right='cell_id', how='left'),
+        electrolyte_batch=dict(left='electrolyte', right='id', how='left'),
+        el=dict(left='electrolyte_type', right='id', how='left'),
+        sd_a_batch=dict(left='sd_a_batch_id', right='id', how='left'),
+        sd_c_batch=dict(left='sd_c_batch_id', right='id', how='left'),
+        ext_a_batch=dict(left='anode_batch_id', right='id', how='left'),
+        ext_c_batch=dict(left='cathode_batch_id', right='id', how='left'),
     ),
     ext_pouch_test=dict(
         ext_pouch_test_template=dict(left='test_type_id', right='id', how='left'),
+        ext_pouch=dict(left='ext_pouch_id', right='id', how='left'),
         neware_cache=dict(left=['ip', 'device', 'unit', 'channel', 'test_id'], right=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], how='inner'),
         neware_pulses_cache=dict(left=['ip', 'device', 'unit', 'channel', 'test_id'], right=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], how='inner'),
         neware_cache_anode=dict(left=['ip', 'device', 'unit', 'channel', 'test_id'], right=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], how='inner'),
     ),
     jellyroll=dict(
         jellyroll_test=dict(left='id', right='jellyroll_id', how='left'),
+        fa_analysis=dict(left='id', right='pouch_id', how='left'),
+        pilot_c_batch=dict(left='p_cathode_batch_id', right='id', how='left'),
+        pilot_a_batch=dict(left='p_anode_batch_id', right='id', how='left'),
+        jellyroll_anode=dict(left='anode_id', right='id', how='left'),
+        jellyroll_cathode=dict(left='cathode_id', right='id', how='left'),
+        el_batch=dict(left='electrolyte_ct', right='id', how='left'),
+        electrolyte_batch=dict(left='electrolyte', right='id', how='left'),
+        el=dict(left='electrolyte_type', right='id', how='left'),
+        sd_a_batch=dict(left='sd_a_batch_id', right='id', how='left'),
+        sd_c_batch=dict(left='sd_c_batch_id', right='id', how='left'),
     ),
     jellyroll_test=dict(
         jellyroll_test_template=dict(left='test_type_id', right='id', how='left'),
+        jellyroll=dict(left='jellyroll_id', right='id', how='left'),
         neware_cache=dict(left=['ip', 'device', 'unit', 'channel', 'test_id'], right=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], how='inner'),
         neware_pulses_cache=dict(left=['ip', 'device', 'unit', 'channel', 'test_id'], right=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], how='inner'),
         neware_cache_anode=dict(left=['ip', 'device', 'unit', 'channel', 'test_id'], right=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], how='inner'),
     ),
     coin_anode=dict(
         coin_anode_test=dict(left='id', right='coin_anode_id', how='left'),
+        anode_batch=dict(left='batch_id', right='id', how='left'),
+        anode_el_batch=dict(left='el_batch_id', right='id', how='left'),
+        electrolyte_batch=dict(left='electrolyte', right='id', how='left'),
+        el=dict(left='electrolyte_type', right='id', how='left'),
+        sd_a_batch=dict(left='sd_a_batch_id', right='id', how='left'),
     ),
     coin_anode_test=dict(
         coin_anode_test_template=dict(left='test_type_id', right='id', how='left'),
+        coin_anode=dict(left='coin_anode_id', right='id', how='left'),
         neware_cache=dict(left=['ip', 'device', 'unit', 'channel', 'test_id'], right=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], how='inner'),
         neware_pulses_cache=dict(left=['ip', 'device', 'unit', 'channel', 'test_id'], right=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], how='inner'),
         neware_cache_anode=dict(left=['ip', 'device', 'unit', 'channel', 'test_id'], right=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], how='inner'),
     ),
     coin_cathode=dict(
         coin_cathode_test=dict(left='id', right='coin_cathode_id', how='left'),
+        cathode_batch=dict(left='batch_id', right='id', how='left'),
+        cathode_el_batch=dict(left='el_batch_id', right='id', how='left'),
+        electrolyte_batch=dict(left='electrolyte', right='id', how='left'),
+        el=dict(left='electrolyte_type', right='id', how='left'),
+        sd_c_batch=dict(left='sd_c_batch_id', right='id', how='left'),
     ),
     coin_cathode_test=dict(
         coin_cathode_test_template=dict(left='test_type_id', right='id', how='left'),
+        coin_cathode=dict(left='coin_cathode_id', right='id', how='left'),
         neware_cache=dict(left=['ip', 'device', 'unit', 'channel', 'test_id'], right=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], how='inner'),
         neware_pulses_cache=dict(left=['ip', 'device', 'unit', 'channel', 'test_id'], right=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], how='inner'),
         neware_cache_anode=dict(left=['ip', 'device', 'unit', 'channel', 'test_id'], right=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], how='inner'),
     ),
     coin_fc=dict(
         coin_fc_test=dict(left='id', right='coin_fc_id', how='left'),
+        anode_batch=dict(left='anode_batch_id', right='id', how='left'),
+        anode_el_batch=dict(left='anode_el_batch_id', right='id', how='left'),
+        cathode_batch=dict(left='cathode_batch_id', right='id', how='left'),
+        cathode_el_batch=dict(left='cathode_el_batch_id', right='id', how='left'),
+        electrolyte_batch=dict(left='electrolyte', right='id', how='left'),
+        el=dict(left='electrolyte_type', right='id', how='left'),
+        sd_a_batch=dict(left='sd_a_batch_id', right='id', how='left'),
+        sd_c_batch=dict(left='sd_c_batch_id', right='id', how='left'),
     ),
     coin_fc_test=dict(
         coin_fc_test_template=dict(left='test_type_id', right='id', how='left'),
+        coin_fc=dict(left='coin_fc_id', right='id', how='left'),
         neware_cache=dict(left=['ip', 'device', 'unit', 'channel', 'test_id'], right=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], how='inner'),
         neware_pulses_cache=dict(left=['ip', 'device', 'unit', 'channel', 'test_id'], right=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], how='inner'),
         neware_cache_anode=dict(left=['ip', 'device', 'unit', 'channel', 'test_id'], right=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], how='inner'),
     ),
     ct_coin=dict(
         ct_coin_test=dict(left='id', right='ct_coin_id', how='left'),
     ),
     ct_coin_test=dict(
         ct_coin_test_template=dict(left='test_type_id', right='id', how='left'),
+        ct_coin=dict(left='ct_coin_id', right='id', how='left'),
         neware_cache=dict(left=['ip', 'device', 'unit', 'channel', 'test_id'], right=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], how='inner'),
         neware_pulses_cache=dict(left=['ip', 'device', 'unit', 'channel', 'test_id'], right=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], how='inner'),
         neware_cache_anode=dict(left=['ip', 'device', 'unit', 'channel', 'test_id'], right=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], how='inner'),
     ),
     bia_cell=dict(
         bia_cell_test=dict(left='id', right='bia_cell_id', how='left'),
     ),
     bia_cell_test=dict(
         bia_cell_test_template=dict(left='test_type_id', right='id', how='left'),
+        bia_cell=dict(left='bia_cell_id', right='id', how='left'),
         neware_cache=dict(left=['ip', 'device', 'unit', 'channel', 'test_id'], right=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], how='inner'),
         neware_pulses_cache=dict(left=['ip', 'device', 'unit', 'channel', 'test_id'], right=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], how='inner'),
         neware_cache_anode=dict(left=['ip', 'device', 'unit', 'channel', 'test_id'], right=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], how='inner'),
     ),
     bic_cell=dict(
         bic_cell_test=dict(left='id', right='bic_cell_id', how='left'),
     ),
     bic_cell_test=dict(
         bic_cell_test_template=dict(left='test_type_id', right='id', how='left'),
+        bic_cell=dict(left='bic_cell_id', right='id', how='left'),
         neware_cache=dict(left=['ip', 'device', 'unit', 'channel', 'test_id'], right=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], how='inner'),
         neware_pulses_cache=dict(left=['ip', 'device', 'unit', 'channel', 'test_id'], right=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], how='inner'),
         neware_cache_anode=dict(left=['ip', 'device', 'unit', 'channel', 'test_id'], right=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], how='inner'),
     ),
     mi_cell=dict(
         mi_cell_test=dict(left='id', right='mi_cell_id', how='left'),
     ),
     mi_cell_test=dict(
         mi_cell_test_template=dict(left='test_type_id', right='id', how='left'),
+        mi_cell=dict(left='mi_cell_id', right='id', how='left'),
         neware_cache=dict(left=['ip', 'device', 'unit', 'channel', 'test_id'], right=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], how='inner'),
         neware_pulses_cache=dict(left=['ip', 'device', 'unit', 'channel', 'test_id'], right=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], how='inner'),
         neware_cache_anode=dict(left=['ip', 'device', 'unit', 'channel', 'test_id'], right=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'], how='inner'),
     ),
     augm_per_cell=dict(
         augm_per_test=dict(left='id', right='augm_per_cell', how='left'),
     ),
@@ -345,14 +441,156 @@
         augm_per_cycle=dict(left='id', right='augm_per_test', how='left'),
         augm_per_cell=dict(left='augm_per_cell', right='id', how='left'),
     ),
     augm_per_cycle=dict(
         augm_per_test=dict(left='augm_per_test', right='id', how='left'),
         neware_cache=dict(left=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id', 'cycle'], right=['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id', 'cycle'], how='inner'),
     ),
+    anode_batch=dict(
+        pouch=dict(right='anode_batch_id', left='id', how='left'),
+        coin_anode=dict(right='batch_id', left='id', how='left'),
+        coin_fc=dict(right='anode_batch_id', left='id', how='left'),
+    ),  
+    sd_a_batch=dict(
+        pouch=dict(right='sd_a_batch_id', left='id', how='left'),
+        pilot_pouch=dict(right='sd_a_batch_id', left='id', how='left'),
+        ext_pouch=dict(right='sd_a_batch_id', left='id', how='left'),
+        jellyroll=dict(right='sd_a_batch_id', left='id', how='left'),
+        coin_anode=dict(right='sd_a_batch_id', left='id', how='left'),
+        coin_fc=dict(right='sd_a_batch_id', left='id', how='left'),
+    ),
+    pouch_anode=dict(
+        pouch=dict(right='anode_id', left='id', how='left'),
+        pilot_pouch=dict(right='anode_id', left='id', how='left'),
+        ext_pouch=dict(right='anode_id', left='id', how='left'),
+    ),
+    cathode_batch=dict(
+        pouch=dict(right='cathode_batch_id', left='id', how='left'),
+        coin_cathode=dict(right='batch_id', left='id', how='left'),
+        coin_fc=dict(right='cathode_batch_id', left='id', how='left'),
+    ),
+    sd_c_batch=dict(
+        pouch=dict(right='sd_c_batch_id', left='id', how='left'),
+        pilot_pouch=dict(right='sd_c_batch_id', left='id', how='left'),
+        ext_pouch=dict(right='sd_c_batch_id', left='id', how='left'),
+        jellyroll=dict(right='sd_c_batch_id', left='id', how='left'),
+        coin_cathode=dict(right='sd_c_batch_id', left='id', how='left'),
+        coin_fc=dict(right='sd_c_batch_id', left='id', how='left'),
+    ),
+    pouch_cathode=dict(
+        pouch=dict(right='cathode_id', left='id', how='left'),
+        pilot_pouch=dict(right='cathode_id', left='id', how='left'),
+        ext_pouch=dict(right='cathode_id', left='id', how='left'),
+    ),
+    el_batch=dict(
+        pouch=dict(right='electrolyte_ct', left='id', how='left'),
+        pilot_pouch=dict(right='electrolyte_ct', left='id', how='left'),
+        ext_pouch=dict(right='electrolyte_ct', left='id', how='left'),
+        jellyroll=dict(right='electrolyte_ct', left='id', how='left'),
+    ),
+    fa_analysis=dict(
+        pouch=dict(right='id', left='pouch_id', how='left'),
+        pilot_pouch=dict(right='id', left='pilot_pouch_id', how='left'),
+        ext_pouch=dict(right='id', left='ext_pouch_id', how='left'),
+        jellyroll=dict(right='id', left='pouch_id', how='left'),
+    ),
+    storage_analysis=dict(
+        pouch=dict(right='id', left='cell_id', how='left'),
+        pilot_pouch=dict(right='id', left='cell_id', how='left'),
+        ext_pouch=dict(right='id', left='cell_id', how='left'),
+    ),
+    electrolyte_batch=dict(
+        pouch=dict(right='electrolyte', left='id', how='left'),
+        pilot_pouch=dict(right='electrolyte', left='id', how='left'),
+        ext_pouch=dict(right='electrolyte', left='id', how='left'),
+        jellyroll=dict(right='electrolyte', left='id', how='left'),
+        coin_anode=dict(right='electrolyte', left='id', how='left'),
+        coin_cathode=dict(right='electrolyte', left='id', how='left'),
+        coin_fc=dict(right='electrolyte', left='id', how='left'),
+    ),
+    pilot_c_batch=dict(
+        pilot_pouch=dict(right='p_cathode_batch_id', left='id', how='left'),
+        ext_pouch=dict(right='p_cathode_batch_id', left='id', how='left'),
+        jellyroll=dict(right='p_cathode_batch_id', left='id', how='left'),
+    ),
+    pilot_a_batch=dict(
+        pilot_pouch=dict(right='p_anode_batch_id', left='id', how='left'),
+        ext_pouch=dict(right='p_anode_batch_id', left='id', how='left'),
+        jellyroll=dict(right='p_anode_batch_id', left='id', how='left'),
+    ),
+    anode_el_batch=dict(
+        pilot_pouch=dict(right='anode_el_batch_id', left='id', how='left'),
+        ext_pouch=dict(right='anode_el_batch_id', left='id', how='left'),
+        coin_anode=dict(right='el_batch_id', left='id', how='left'),
+        coin_fc=dict(right='anode_el_batch_id', left='id', how='left'),
+    ),
+    cathode_el_batch=dict(
+        pilot_pouch=dict(right='cathode_el_batch_id', left='id', how='left'),
+        ext_pouch=dict(right='cathode_el_batch_id', left='id', how='left'),
+        coin_cathode=dict(right='el_batch_id', left='id', how='left'),
+        coin_fc=dict(right='cathode_el_batch_id', left='id', how='left'),
+    ),
+    pilot_pouch_test_template=dict(
+        pilot_pouch_test=dict(right='test_type_id', left='id', how='left'),
+    ),
+    ext_pouch_test_template=dict(
+        ext_pouch_test=dict(right='test_type_id', left='id', how='left'),
+    ),
+    jellyroll_anode=dict(
+        jellyroll=dict(right='anode_id', left='id', how='left'),
+    ),
+    jellyroll_cathode=dict(
+        jellyroll=dict(right='cathode_id', left='id', how='left'),
+    ),
+    jellyroll_test_template=dict(
+        jellyroll_test=dict(right='test_type_id', left='id', how='left'),
+    ),
+    coin_anode_test_template=dict(
+        coin_anode_test=dict(right='test_type_id', left='id', how='left'),
+    ),
+    coin_cathode_test_template=dict(
+        coin_cathode_test=dict(right='test_type_id', left='id', how='left'),
+    ),
+    coin_fc_test_template=dict(
+        coin_fc_test=dict(right='test_type_id', left='id', how='left'),
+    ),
+    ct_coin_test_template=dict(
+        ct_coin_test=dict(right='test_type_id', left='id', how='left'),
+    ),
+    bia_cell_test_template=dict(
+        bia_cell_test=dict(right='test_type_id', left='id', how='left'),
+    ),
+    bic_cell_test_template=dict(
+        bic_cell_test=dict(right='test_type_id', left='id', how='left'),
+    ),
+    mi_cell_test_template=dict(
+        mi_cell_test=dict(right='test_type_id', left='id', how='left'),
+    ),
+    el=dict(
+        pouch=dict(right='electrolyte_type', left='id', how='left'),
+        pilot_pouch=dict(right='electrolyte_type', left='id', how='left'),
+        ext_pouch=dict(right='electrolyte_type', left='id', how='left'),
+        jellyroll=dict(right='electrolyte_type', left='id', how='left'),
+        coin_anode=dict(right='electrolyte_type', left='id', how='left'),
+        coin_cathode=dict(right='electrolyte_type', left='id', how='left'),
+        coin_fc=dict(right='electrolyte_type', left='id', how='left'),
+    ),
+    us_cell=dict(
+        us_cell_test=dict(left='id', right='us_cell_id', how='inner'),
+    ),
+    us_cell_test=dict(
+        us_cell=dict(left='us_cell_id', right='id', how='left'),
+        us_cell_test_template=dict(left='test_type_id', right='id', how='left'),
+    ),
+    us_cell_test_template=dict(
+        us_cell_test=dict(left='id', right='test_type_id', how='left'),
+    ),
+    material=dict(
+        material_type=dict(left='type', right='id', how='left'),
+    ),
 )
 
 COLUMN_TO_LABEL = {
     'a_batch_id': 'Anode batch',
     'a_chg': 'A Chg',
     'a_dchg': 'A Dchg',
     'a_el_batch': 'resulting batch (A)',
```

### Comparing `banner-storedot-2.2.9/src/banner_storedot.egg-info/PKG-INFO` & `banner-storedot-2.3.0/src/banner_storedot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: banner-storedot
-Version: 2.2.9
+Version: 2.3.0
 Summary: light dal package
 Home-page: https://https://github.com/storedot/banner
 Author: GB
 Author-email: gilb@store-dot.com
 Project-URL: Bug Tracker, https://https://github.com/storedot/banner/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `banner-storedot-2.2.9/src/banner_storedot.egg-info/SOURCES.txt` & `banner-storedot-2.3.0/src/banner_storedot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

