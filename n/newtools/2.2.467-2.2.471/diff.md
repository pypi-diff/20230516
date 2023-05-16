# Comparing `tmp/newtools-2.2.467.tar.gz` & `tmp/newtools-2.2.471.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/newtools-2.2.467.tar", last modified: Fri Apr 21 09:46:06 2023, max compression
+gzip compressed data, was "dist/newtools-2.2.471.tar", last modified: Tue May 16 16:12:50 2023, max compression
```

## Comparing `newtools-2.2.467.tar` & `newtools-2.2.471.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 09:46:06.000000 newtools-2.2.467/
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-04-21 09:44:16.000000 newtools-2.2.467/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     1305 2023-04-21 09:46:06.000000 newtools-2.2.467/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1069 2023-04-21 09:44:16.000000 newtools-2.2.467/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 09:46:06.000000 newtools-2.2.467/newtools/
--rw-rw-rw-   0 root         (0) root         (0)      648 2023-04-21 09:44:16.000000 newtools-2.2.467/newtools/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 09:46:06.000000 newtools-2.2.467/newtools/aws/
--rw-rw-rw-   0 root         (0) root         (0)      195 2023-04-21 09:44:16.000000 newtools-2.2.467/newtools/aws/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9641 2023-04-21 09:44:16.000000 newtools-2.2.467/newtools/aws/load_partitions.py
--rw-rw-rw-   0 root         (0) root         (0)     6435 2023-04-21 09:44:16.000000 newtools-2.2.467/newtools/aws/s3_location.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 09:46:06.000000 newtools-2.2.467/newtools/db/
--rw-rw-rw-   0 root         (0) root         (0)      285 2023-04-21 09:44:16.000000 newtools-2.2.467/newtools/db/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6912 2023-04-21 09:44:16.000000 newtools-2.2.467/newtools/db/athena.py
--rw-rw-rw-   0 root         (0) root         (0)    39431 2023-04-21 09:44:16.000000 newtools-2.2.467/newtools/db/cached_query.py
--rw-rw-rw-   0 root         (0) root         (0)    12954 2023-04-21 09:44:16.000000 newtools-2.2.467/newtools/db/sql_client.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 09:46:06.000000 newtools-2.2.467/newtools/doggo/
--rw-rw-rw-   0 root         (0) root         (0)      268 2023-04-21 09:44:16.000000 newtools-2.2.467/newtools/doggo/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5576 2023-04-21 09:44:16.000000 newtools-2.2.467/newtools/doggo/csv.py
--rw-rw-rw-   0 root         (0) root         (0)    13397 2023-04-21 09:44:16.000000 newtools-2.2.467/newtools/doggo/doggo.py
--rw-rw-rw-   0 root         (0) root         (0)    19227 2023-04-21 09:44:16.000000 newtools-2.2.467/newtools/doggo/fs.py
--rw-rw-rw-   0 root         (0) root         (0)     9277 2023-04-21 09:44:16.000000 newtools-2.2.467/newtools/doggo/lock.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 09:46:06.000000 newtools-2.2.467/newtools/log/
--rw-rw-rw-   0 root         (0) root         (0)      225 2023-04-21 09:44:16.000000 newtools-2.2.467/newtools/log/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9531 2023-04-21 09:44:16.000000 newtools-2.2.467/newtools/log/json_persistent_field_logger.py
--rw-rw-rw-   0 root         (0) root         (0)     3858 2023-04-21 09:44:16.000000 newtools-2.2.467/newtools/log/log.py
--rw-rw-rw-   0 root         (0) root         (0)     2931 2023-04-21 09:44:16.000000 newtools-2.2.467/newtools/log/persistent_field_logger.py
--rw-rw-rw-   0 root         (0) root         (0)     3452 2023-04-21 09:44:16.000000 newtools-2.2.467/newtools/optional_imports.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 09:46:06.000000 newtools-2.2.467/newtools/queue/
--rw-rw-rw-   0 root         (0) root         (0)       72 2023-04-21 09:44:16.000000 newtools-2.2.467/newtools/queue/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5151 2023-04-21 09:44:16.000000 newtools-2.2.467/newtools/queue/task_queue.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-21 09:46:06.000000 newtools-2.2.467/newtools.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     1305 2023-04-21 09:46:06.000000 newtools-2.2.467/newtools.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      797 2023-04-21 09:46:06.000000 newtools-2.2.467/newtools.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-21 09:46:06.000000 newtools-2.2.467/newtools.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-21 09:46:06.000000 newtools-2.2.467/newtools.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)      119 2023-04-21 09:46:06.000000 newtools-2.2.467/newtools.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)        9 2023-04-21 09:46:06.000000 newtools-2.2.467/newtools.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       70 2023-04-21 09:44:16.000000 newtools-2.2.467/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      252 2023-04-21 09:46:06.000000 newtools-2.2.467/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2296 2023-04-21 09:44:16.000000 newtools-2.2.467/setup.py
--rw-rw-rw-   0 root         (0) root         (0)        7 2023-04-21 09:46:04.000000 newtools-2.2.467/version.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-16 16:12:50.000000 newtools-2.2.471/
+-rw-rw-rw-   0 root         (0) root         (0)       62 2023-05-16 16:10:45.000000 newtools-2.2.471/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     1305 2023-05-16 16:12:50.000000 newtools-2.2.471/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2023-05-16 16:10:45.000000 newtools-2.2.471/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-16 16:12:50.000000 newtools-2.2.471/newtools/
+-rw-rw-rw-   0 root         (0) root         (0)      648 2023-05-16 16:10:45.000000 newtools-2.2.471/newtools/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-16 16:12:50.000000 newtools-2.2.471/newtools/aws/
+-rw-rw-rw-   0 root         (0) root         (0)      195 2023-05-16 16:10:45.000000 newtools-2.2.471/newtools/aws/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9641 2023-05-16 16:10:45.000000 newtools-2.2.471/newtools/aws/load_partitions.py
+-rw-rw-rw-   0 root         (0) root         (0)     6435 2023-05-16 16:10:45.000000 newtools-2.2.471/newtools/aws/s3_location.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-16 16:12:50.000000 newtools-2.2.471/newtools/db/
+-rw-rw-rw-   0 root         (0) root         (0)      285 2023-05-16 16:10:45.000000 newtools-2.2.471/newtools/db/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6912 2023-05-16 16:10:45.000000 newtools-2.2.471/newtools/db/athena.py
+-rw-rw-rw-   0 root         (0) root         (0)    40091 2023-05-16 16:10:45.000000 newtools-2.2.471/newtools/db/cached_query.py
+-rw-rw-rw-   0 root         (0) root         (0)    12954 2023-05-16 16:10:45.000000 newtools-2.2.471/newtools/db/sql_client.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-16 16:12:50.000000 newtools-2.2.471/newtools/doggo/
+-rw-rw-rw-   0 root         (0) root         (0)      268 2023-05-16 16:10:45.000000 newtools-2.2.471/newtools/doggo/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5576 2023-05-16 16:10:45.000000 newtools-2.2.471/newtools/doggo/csv.py
+-rw-rw-rw-   0 root         (0) root         (0)    13397 2023-05-16 16:10:45.000000 newtools-2.2.471/newtools/doggo/doggo.py
+-rw-rw-rw-   0 root         (0) root         (0)    19227 2023-05-16 16:10:45.000000 newtools-2.2.471/newtools/doggo/fs.py
+-rw-rw-rw-   0 root         (0) root         (0)     9277 2023-05-16 16:10:45.000000 newtools-2.2.471/newtools/doggo/lock.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-16 16:12:50.000000 newtools-2.2.471/newtools/log/
+-rw-rw-rw-   0 root         (0) root         (0)      225 2023-05-16 16:10:45.000000 newtools-2.2.471/newtools/log/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9531 2023-05-16 16:10:45.000000 newtools-2.2.471/newtools/log/json_persistent_field_logger.py
+-rw-rw-rw-   0 root         (0) root         (0)     3858 2023-05-16 16:10:45.000000 newtools-2.2.471/newtools/log/log.py
+-rw-rw-rw-   0 root         (0) root         (0)     2931 2023-05-16 16:10:45.000000 newtools-2.2.471/newtools/log/persistent_field_logger.py
+-rw-rw-rw-   0 root         (0) root         (0)     3452 2023-05-16 16:10:45.000000 newtools-2.2.471/newtools/optional_imports.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-16 16:12:50.000000 newtools-2.2.471/newtools/queue/
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-05-16 16:10:45.000000 newtools-2.2.471/newtools/queue/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5151 2023-05-16 16:10:45.000000 newtools-2.2.471/newtools/queue/task_queue.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-16 16:12:50.000000 newtools-2.2.471/newtools.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     1305 2023-05-16 16:12:50.000000 newtools-2.2.471/newtools.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      797 2023-05-16 16:12:50.000000 newtools-2.2.471/newtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-16 16:12:50.000000 newtools-2.2.471/newtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-16 16:12:50.000000 newtools-2.2.471/newtools.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)      119 2023-05-16 16:12:50.000000 newtools-2.2.471/newtools.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)        9 2023-05-16 16:12:50.000000 newtools-2.2.471/newtools.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-05-16 16:10:45.000000 newtools-2.2.471/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      252 2023-05-16 16:12:50.000000 newtools-2.2.471/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2296 2023-05-16 16:10:45.000000 newtools-2.2.471/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)        7 2023-05-16 16:12:47.000000 newtools-2.2.471/version.txt
```

### Comparing `newtools-2.2.467/PKG-INFO` & `newtools-2.2.471/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newtools
-Version: 2.2.467
+Version: 2.2.471
 Summary: Provides useful libraries for processing large data sets.
 Home-page: https://bitbucket.org/deductive/newtools/
 Author: Deductive
 Author-email: hello@deductive.com
 License: MIT
 Project-URL: Documentation, https://newtools.readthedocs.io/en/latest/
 Project-URL: Source, https://bitbucket.org/deductive/newtools/
```

### Comparing `newtools-2.2.467/README.md` & `newtools-2.2.471/README.md`

 * *Files identical despite different names*

### Comparing `newtools-2.2.467/newtools/__init__.py` & `newtools-2.2.471/newtools/__init__.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.467/newtools/aws/load_partitions.py` & `newtools-2.2.471/newtools/aws/load_partitions.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.467/newtools/aws/s3_location.py` & `newtools-2.2.471/newtools/aws/s3_location.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.467/newtools/db/athena.py` & `newtools-2.2.471/newtools/db/athena.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.467/newtools/db/cached_query.py` & `newtools-2.2.471/newtools/db/cached_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,15 @@
 from newtools.db.sql_client import SqlClient
 from newtools.doggo import DoggoLock, DoggoFileSystem, DynamoDogLock, FileDoggo, PandasDoggo
 
 # Set S3fsMixin for backwards compatibility
 S3fsMixin = DoggoFileSystem
 Path = Union[str, S3Location]
 DataFrame = Type['pd.DataFrame']
+BotoSession = Type['boto3.Session']
 
 
 class UselessLock:
     """
     Class to allow the use of a lock to be optional.
     """
     def __init__(self, *args, **kwargs):
@@ -85,17 +86,23 @@
         self.logger.info("Releasing useless lock")
 
 
 class BaseCachedClass:
     validation_mode = False
     _expiry_seconds = 0
 
-    def __init__(self, cache_path, logger=logging.getLogger("newtools.cached_query"), expiry_seconds=0):
+    def __init__(
+        self,
+        cache_path,
+        logger=logging.getLogger("newtools.cached_query"),
+        expiry_seconds=0,
+        boto_session: Optional[BotoSession] = None
+    ) -> None:
         self.cache_path = cache_path
-        self.dfs = DoggoFileSystem()
+        self.dfs = DoggoFileSystem(boto3_session=boto_session) if boto_session else DoggoFileSystem()
         self._logger = logger
         self._expiry_seconds = expiry_seconds
 
     def _exists(self, path):
         """
         Checks whether a path exists locally or on S3
 
@@ -185,30 +192,31 @@
 
     wait_period = 30
     time_out_seconds = 1800
     maximum_age = 3600
 
     def __init__(self, params=None, cache_path="", sql_archive_path=None, sql_paths=None, gzip=True,
                  dynamodb_lock=True, logger=logging.getLogger("newtools.cached_query"), expiry_seconds=0,
-                 use_lock: Optional[bool] = True):
+                 use_lock: Optional[bool] = True, boto_session: Optional[BotoSession] = None):
         """
         Cached query class
 
         :param params: a dictionary of parameters passed to each query
         :param cache_path: the path locally or on S3 to cache query results
         :param sql_archive_path: the path locally or on S3 to store archive SQL queries
         :param sql_paths: path or a list of paths to search for SQL queries
         :param gzip: if set, then results will be compression
         :param dynamodb_lock: defaults to True, using Dynamo DB for locking in S3
         :param logger: the logger to use for this class and any newtools classes created by this class
         :param expiry_seconds: if set, caches files we expire every expiry_seconds seconds.
         :param use_lock: whether to use a lock to prevent concurrent s3 access
             if set to False, dynamodb_lock parameter wll be ignored
+        :param boto_session: a specific boto3 session to be used
         """
-        super().__init__(cache_path, logger, expiry_seconds)
+        super().__init__(cache_path, logger, expiry_seconds, boto_session=boto_session)
 
         self._logger = logger
         self._gzip = gzip
         self._args = self._validate_args(params)
 
         self._sql_paths = ['sql', os.path.join(os.path.split(__file__)[0], 'sql')]
         if sql_paths is not None:
@@ -535,16 +543,18 @@
         df = pd.load_df(results, compression="gzip")
 
     """
     __sql = None
     _redshift_checks = True
 
     def __init__(self, pep_249_obj, params=None, cache_path="", sql_archive_path=None, sql_paths=None, gzip=True,
-                 dynamodb_lock=True, logger=logging.getLogger("newtools.cached_query"), expiry_seconds=0):
-        super().__init__(params, cache_path, sql_archive_path, sql_paths, gzip, dynamodb_lock, logger, expiry_seconds)
+                 dynamodb_lock=True, logger=logging.getLogger("newtools.cached_query"), expiry_seconds=0,
+                 boto_session: Optional[BotoSession] = None):
+        super().__init__(params, cache_path, sql_archive_path, sql_paths, gzip, dynamodb_lock, logger, expiry_seconds,
+                         boto_session=boto_session)
 
         self._sql = SqlClient(pep_249_obj,
                               logger=logger,
                               logging_level=logging.INFO)
 
     @staticmethod
     def _validate_sql(sql_file):
@@ -628,25 +638,27 @@
         df = pd.load_df(results, compression="gzip")
 
     """
     __ac = None
 
     def __init__(self, params=None, cache_path="", sql_archive_path=None, sql_paths=None, gzip=True,
                  dynamodb_lock=True, logger=logging.getLogger("newtools.cached_query"),
-                 queue_queries=False, expiry_seconds=0, use_lock: Optional[bool] = True):
+                 queue_queries=False, expiry_seconds=0, use_lock: Optional[bool] = True,
+                 boto_session: Optional[BotoSession] = None):
         super().__init__(
             params=params,
             cache_path=cache_path,
             sql_archive_path=sql_archive_path,
             sql_paths=sql_paths,
             gzip=gzip,
             dynamodb_lock=dynamodb_lock,
             logger=logger,
             expiry_seconds=expiry_seconds,
-            use_lock=use_lock
+            use_lock=use_lock,
+            boto_session=boto_session
         )
 
         self._results = dict()
         self.queue_queries = queue_queries
 
     @property
     def _ac(self):
@@ -753,15 +765,16 @@
         sql_archive_path: Optional[str] = None,
         sql_paths: Optional[Union[str, List[str]]] = None,
         dynamodb_lock: Optional[bool] = True,
         use_lock: Optional[bool] = True,
         logger: Optional[logging.Logger] = logging.getLogger(__name__),
         expiry_seconds: Optional[int] = 0,
         queue_queries: Optional[bool] = False,
-        return_meta: Optional[bool] = False
+        return_meta: Optional[bool] = False,
+        boto_session: Optional[BotoSession] = None
     ) -> None:
         """
         :param use_lock: whether to use a lock to prevent concurrent s3 access
             if set to False, dynamodb_lock parameter wll be ignored
         :param return_meta: whether to return the metadata of the query (e.g. count(1) of the results)
             this functionality will only work if queue_queries is set to False
         """
@@ -780,15 +793,15 @@
             expiry_seconds=expiry_seconds,
             use_lock=use_lock
         )
 
         self.return_meta = return_meta
         self.queue_queries = queue_queries
 
-        self.doggo = PandasDoggo()
+        self.doggo = PandasDoggo(boto_session=boto_session) if boto_session else PandasDoggo()
 
     @classmethod
     def get_query_header(
         cls,
         database: str,
         table_name: str,
         external_location: Path,
```

### Comparing `newtools-2.2.467/newtools/db/sql_client.py` & `newtools-2.2.471/newtools/db/sql_client.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.467/newtools/doggo/csv.py` & `newtools-2.2.471/newtools/doggo/csv.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.467/newtools/doggo/doggo.py` & `newtools-2.2.471/newtools/doggo/doggo.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.467/newtools/doggo/fs.py` & `newtools-2.2.471/newtools/doggo/fs.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.467/newtools/doggo/lock.py` & `newtools-2.2.471/newtools/doggo/lock.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.467/newtools/log/json_persistent_field_logger.py` & `newtools-2.2.471/newtools/log/json_persistent_field_logger.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.467/newtools/log/log.py` & `newtools-2.2.471/newtools/log/log.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.467/newtools/log/persistent_field_logger.py` & `newtools-2.2.471/newtools/log/persistent_field_logger.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.467/newtools/optional_imports.py` & `newtools-2.2.471/newtools/optional_imports.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.467/newtools/queue/task_queue.py` & `newtools-2.2.471/newtools/queue/task_queue.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.467/newtools.egg-info/PKG-INFO` & `newtools-2.2.471/newtools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newtools
-Version: 2.2.467
+Version: 2.2.471
 Summary: Provides useful libraries for processing large data sets.
 Home-page: https://bitbucket.org/deductive/newtools/
 Author: Deductive
 Author-email: hello@deductive.com
 License: MIT
 Project-URL: Documentation, https://newtools.readthedocs.io/en/latest/
 Project-URL: Source, https://bitbucket.org/deductive/newtools/
```

### Comparing `newtools-2.2.467/newtools.egg-info/SOURCES.txt` & `newtools-2.2.471/newtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `newtools-2.2.467/setup.py` & `newtools-2.2.471/setup.py`

 * *Files identical despite different names*

