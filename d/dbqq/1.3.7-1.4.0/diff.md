# Comparing `tmp/dbqq-1.3.7.tar.gz` & `tmp/dbqq-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbqq-1.3.7.tar", last modified: Thu May  4 13:05:05 2023, max compression
+gzip compressed data, was "dbqq-1.4.0.tar", last modified: Tue May 16 11:49:03 2023, max compression
```

## Comparing `dbqq-1.3.7.tar` & `dbqq-1.4.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 13:05:05.704118 dbqq-1.3.7/
--rw-rw-rw-   0        0        0    14130 2023-05-04 13:05:05.702117 dbqq-1.3.7/PKG-INFO
--rw-rw-rw-   0        0        0    13400 2023-05-04 12:58:55.000000 dbqq-1.3.7/README.md
--rw-rw-rw-   0        0        0     1083 2023-05-04 12:58:55.000000 dbqq-1.3.7/license.md
--rw-rw-rw-   0        0        0     1302 2023-05-04 13:04:37.000000 dbqq-1.3.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-04 13:05:05.705119 dbqq-1.3.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-04 13:05:05.567129 dbqq-1.3.7/src/
-drwxrwxrwx   0        0        0        0 2023-05-04 13:05:05.598117 dbqq-1.3.7/src/dbqq/
--rw-rw-rw-   0        0        0      127 2023-05-04 12:58:55.000000 dbqq-1.3.7/src/dbqq/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 13:05:05.633118 dbqq-1.3.7/src/dbqq/cli/
--rw-rw-rw-   0        0        0        0 2023-05-04 12:58:55.000000 dbqq-1.3.7/src/dbqq/cli/__init__.py
--rw-rw-rw-   0        0        0      968 2023-05-04 12:58:55.000000 dbqq-1.3.7/src/dbqq/cli/clean_connections.py
--rw-rw-rw-   0        0        0      713 2023-05-04 12:58:55.000000 dbqq-1.3.7/src/dbqq/cli/initialize_connections.py
--rw-rw-rw-   0        0        0     1295 2023-05-04 12:58:55.000000 dbqq-1.3.7/src/dbqq/cli/run_query.py
-drwxrwxrwx   0        0        0        0 2023-05-04 13:05:05.657124 dbqq-1.3.7/src/dbqq/connectors/
--rw-rw-rw-   0        0        0     1013 2023-05-04 12:58:55.000000 dbqq-1.3.7/src/dbqq/connectors/__init__.py
--rw-rw-rw-   0        0        0     7040 2023-05-04 13:00:30.000000 dbqq-1.3.7/src/dbqq/connectors/_base.py
--rw-rw-rw-   0        0        0     1778 2023-05-04 12:58:55.000000 dbqq-1.3.7/src/dbqq/connectors/_polar_connector.py
--rw-rw-rw-   0        0        0     5670 2023-05-04 12:58:55.000000 dbqq-1.3.7/src/dbqq/connectors/databricks.py
--rw-rw-rw-   0        0        0     2906 2023-05-04 12:58:55.000000 dbqq-1.3.7/src/dbqq/connectors/mssql.py
--rw-rw-rw-   0        0        0     4747 2023-05-04 12:58:55.000000 dbqq-1.3.7/src/dbqq/connectors/oracle.py
-drwxrwxrwx   0        0        0        0 2023-05-04 13:05:05.660119 dbqq-1.3.7/src/dbqq/data/
--rw-rw-rw-   0        0        0       46 2023-05-04 12:58:55.000000 dbqq-1.3.7/src/dbqq/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 13:05:05.668117 dbqq-1.3.7/src/dbqq/data/parsed/
--rw-rw-rw-   0        0        0       40 2023-05-04 12:58:55.000000 dbqq-1.3.7/src/dbqq/data/parsed/__init__.py
--rw-rw-rw-   0        0        0      822 2023-05-04 12:58:55.000000 dbqq-1.3.7/src/dbqq/data/parsed/sql.py
-drwxrwxrwx   0        0        0        0 2023-05-04 13:05:05.673120 dbqq-1.3.7/src/dbqq/security/
--rw-rw-rw-   0        0        0       86 2023-05-04 12:58:55.000000 dbqq-1.3.7/src/dbqq/security/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 13:05:05.688115 dbqq-1.3.7/src/dbqq/security/cli/
--rw-rw-rw-   0        0        0        0 2023-05-04 12:58:55.000000 dbqq-1.3.7/src/dbqq/security/cli/__init__.py
--rw-rw-rw-   0        0        0     1091 2023-05-04 12:58:55.000000 dbqq-1.3.7/src/dbqq/security/cli/decrypt_yaml.py
--rw-rw-rw-   0        0        0     1036 2023-05-04 12:58:55.000000 dbqq-1.3.7/src/dbqq/security/cli/encrypt_yaml.py
--rw-rw-rw-   0        0        0     1707 2023-05-04 12:58:55.000000 dbqq-1.3.7/src/dbqq/security/cli/write_keys.py
-drwxrwxrwx   0        0        0        0 2023-05-04 13:05:05.699118 dbqq-1.3.7/src/dbqq/security/functions/
--rw-rw-rw-   0        0        0      119 2023-05-04 12:58:55.000000 dbqq-1.3.7/src/dbqq/security/functions/__init__.py
--rw-rw-rw-   0        0        0     1006 2023-05-04 12:58:55.000000 dbqq-1.3.7/src/dbqq/security/functions/_functions.py
--rw-rw-rw-   0        0        0     4166 2023-05-04 12:58:55.000000 dbqq-1.3.7/src/dbqq/security/functions/_yaml.py
--rw-rw-rw-   0        0        0     2332 2023-05-04 12:58:55.000000 dbqq-1.3.7/src/dbqq/security/helpers.py
--rw-rw-rw-   0        0        0     5315 2023-05-04 12:58:55.000000 dbqq-1.3.7/src/dbqq/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-04 13:05:05.619120 dbqq-1.3.7/src/dbqq.egg-info/
--rw-rw-rw-   0        0        0    14130 2023-05-04 13:05:05.000000 dbqq-1.3.7/src/dbqq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      997 2023-05-04 13:05:05.000000 dbqq-1.3.7/src/dbqq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 13:05:05.000000 dbqq-1.3.7/src/dbqq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      339 2023-05-04 13:05:05.000000 dbqq-1.3.7/src/dbqq.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       96 2023-05-04 13:05:05.000000 dbqq-1.3.7/src/dbqq.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-05-04 13:05:05.000000 dbqq-1.3.7/src/dbqq.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 11:49:03.358244 dbqq-1.4.0/
+-rw-rw-rw-   0        0        0    14130 2023-05-16 11:49:03.357244 dbqq-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0    13400 2023-05-16 11:02:12.000000 dbqq-1.4.0/README.md
+-rw-rw-rw-   0        0        0     1083 2023-05-16 11:02:12.000000 dbqq-1.4.0/license.md
+-rw-rw-rw-   0        0        0     1302 2023-05-16 11:46:52.000000 dbqq-1.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-16 11:49:03.358244 dbqq-1.4.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-16 11:49:03.243243 dbqq-1.4.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-16 11:49:03.268242 dbqq-1.4.0/src/dbqq/
+-rw-rw-rw-   0        0        0      127 2023-05-16 11:02:12.000000 dbqq-1.4.0/src/dbqq/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 11:49:03.299242 dbqq-1.4.0/src/dbqq/cli/
+-rw-rw-rw-   0        0        0        0 2023-05-16 11:02:12.000000 dbqq-1.4.0/src/dbqq/cli/__init__.py
+-rw-rw-rw-   0        0        0      968 2023-05-16 11:02:12.000000 dbqq-1.4.0/src/dbqq/cli/clean_connections.py
+-rw-rw-rw-   0        0        0      713 2023-05-16 11:02:12.000000 dbqq-1.4.0/src/dbqq/cli/initialize_connections.py
+-rw-rw-rw-   0        0        0     1295 2023-05-16 11:02:12.000000 dbqq-1.4.0/src/dbqq/cli/run_query.py
+drwxrwxrwx   0        0        0        0 2023-05-16 11:49:03.317243 dbqq-1.4.0/src/dbqq/connectors/
+-rw-rw-rw-   0        0        0     1013 2023-05-16 11:02:12.000000 dbqq-1.4.0/src/dbqq/connectors/__init__.py
+-rw-rw-rw-   0        0        0     7349 2023-05-16 11:46:45.000000 dbqq-1.4.0/src/dbqq/connectors/_base.py
+-rw-rw-rw-   0        0        0     1778 2023-05-16 11:02:12.000000 dbqq-1.4.0/src/dbqq/connectors/_polar_connector.py
+-rw-rw-rw-   0        0        0     5791 2023-05-16 11:46:33.000000 dbqq-1.4.0/src/dbqq/connectors/databricks.py
+-rw-rw-rw-   0        0        0     2906 2023-05-16 11:46:33.000000 dbqq-1.4.0/src/dbqq/connectors/mssql.py
+-rw-rw-rw-   0        0        0     4747 2023-05-16 11:46:35.000000 dbqq-1.4.0/src/dbqq/connectors/oracle.py
+drwxrwxrwx   0        0        0        0 2023-05-16 11:49:03.319241 dbqq-1.4.0/src/dbqq/data/
+-rw-rw-rw-   0        0        0       46 2023-05-16 11:02:12.000000 dbqq-1.4.0/src/dbqq/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 11:49:03.326251 dbqq-1.4.0/src/dbqq/data/parsed/
+-rw-rw-rw-   0        0        0       40 2023-05-16 11:02:12.000000 dbqq-1.4.0/src/dbqq/data/parsed/__init__.py
+-rw-rw-rw-   0        0        0      822 2023-05-16 11:02:12.000000 dbqq-1.4.0/src/dbqq/data/parsed/sql.py
+drwxrwxrwx   0        0        0        0 2023-05-16 11:49:03.331256 dbqq-1.4.0/src/dbqq/security/
+-rw-rw-rw-   0        0        0       86 2023-05-16 11:02:12.000000 dbqq-1.4.0/src/dbqq/security/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 11:49:03.343243 dbqq-1.4.0/src/dbqq/security/cli/
+-rw-rw-rw-   0        0        0        0 2023-05-16 11:02:12.000000 dbqq-1.4.0/src/dbqq/security/cli/__init__.py
+-rw-rw-rw-   0        0        0     1091 2023-05-16 11:02:12.000000 dbqq-1.4.0/src/dbqq/security/cli/decrypt_yaml.py
+-rw-rw-rw-   0        0        0     1036 2023-05-16 11:02:12.000000 dbqq-1.4.0/src/dbqq/security/cli/encrypt_yaml.py
+-rw-rw-rw-   0        0        0     1707 2023-05-16 11:02:12.000000 dbqq-1.4.0/src/dbqq/security/cli/write_keys.py
+drwxrwxrwx   0        0        0        0 2023-05-16 11:49:03.353245 dbqq-1.4.0/src/dbqq/security/functions/
+-rw-rw-rw-   0        0        0      119 2023-05-16 11:02:12.000000 dbqq-1.4.0/src/dbqq/security/functions/__init__.py
+-rw-rw-rw-   0        0        0     1006 2023-05-16 11:02:12.000000 dbqq-1.4.0/src/dbqq/security/functions/_functions.py
+-rw-rw-rw-   0        0        0     4166 2023-05-16 11:02:12.000000 dbqq-1.4.0/src/dbqq/security/functions/_yaml.py
+-rw-rw-rw-   0        0        0     2332 2023-05-16 11:02:12.000000 dbqq-1.4.0/src/dbqq/security/helpers.py
+-rw-rw-rw-   0        0        0     5315 2023-05-16 11:02:12.000000 dbqq-1.4.0/src/dbqq/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-16 11:49:03.287244 dbqq-1.4.0/src/dbqq.egg-info/
+-rw-rw-rw-   0        0        0    14130 2023-05-16 11:49:03.000000 dbqq-1.4.0/src/dbqq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      997 2023-05-16 11:49:03.000000 dbqq-1.4.0/src/dbqq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 11:49:03.000000 dbqq-1.4.0/src/dbqq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      339 2023-05-16 11:49:03.000000 dbqq-1.4.0/src/dbqq.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       96 2023-05-16 11:49:03.000000 dbqq-1.4.0/src/dbqq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-05-16 11:49:03.000000 dbqq-1.4.0/src/dbqq.egg-info/top_level.txt
```

### Comparing `dbqq-1.3.7/PKG-INFO` & `dbqq-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbqq
-Version: 1.3.7
+Version: 1.4.0
 Summary: quickly connect to and query databases
 Author-email: Chris Mamon <chrisam1993@live.com>
 Project-URL: Homepage, https://github.com/Chr1sC0de/database-quick-query
 Project-URL: Bug Tracker, https://github.com/Chr1sC0de/database-quick-query/issues
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `dbqq-1.3.7/README.md` & `dbqq-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `dbqq-1.3.7/license.md` & `dbqq-1.4.0/license.md`

 * *Files identical despite different names*

### Comparing `dbqq-1.3.7/pyproject.toml` & `dbqq-1.4.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires      = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dbqq"
 description = "quickly connect to and query databases"
-version = "1.3.7"
+version = "1.4.0"
 readme = "README.md"
 dependencies = [
   "tabulate",
   "rsa",
   "pyaml",
   "polars",
   "databricks-sql-connector",
```

### Comparing `dbqq-1.3.7/src/dbqq/cli/clean_connections.py` & `dbqq-1.4.0/src/dbqq/cli/clean_connections.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.3.7/src/dbqq/cli/initialize_connections.py` & `dbqq-1.4.0/src/dbqq/cli/initialize_connections.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.3.7/src/dbqq/cli/run_query.py` & `dbqq-1.4.0/src/dbqq/cli/run_query.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.3.7/src/dbqq/connectors/__init__.py` & `dbqq-1.4.0/src/dbqq/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.3.7/src/dbqq/connectors/_base.py` & `dbqq-1.4.0/src/dbqq/connectors/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,17 @@
 
         query = environment.from_string(query).render(*args, **kwargs)
         return Base.RenderedTemplateLoader(query, self)
 
     def execute(
         self, *args, scan_parquet_kwargs=None, **run_query_kwargs
     ) -> pl.LazyFrame:
-        return self(*args, scan_parquet_kwargs=None, **run_query_kwargs)
+        return self(
+            *args, scan_parquet_kwargs=scan_parquet_kwargs, **run_query_kwargs
+        )
 
     def __call__(
         self, query: str, *args, scan_parquet_kwargs=None, **run_query_kwargs
     ) -> pl.LazyFrame:
         self.query_info = self.QueryInfo(None, None)
 
         if self.to_cache:
@@ -216,7 +218,16 @@
     @abstractmethod
     def _run_query(self):
         ...
 
     @abstractmethod
     def close(self):
         ...
+
+    def get_database(self) -> str:
+        return self.__module__.split(".")[-1]
+
+    def get_name(self) -> str:
+        return self.__class__.__name__.split(".")[-1]
+
+    def get_db_name(self) -> str:
+        return f"{self.get_database()}-{self.get_name()}"
```

### Comparing `dbqq-1.3.7/src/dbqq/connectors/_polar_connector.py` & `dbqq-1.4.0/src/dbqq/connectors/_polar_connector.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.3.7/src/dbqq/connectors/databricks.py` & `dbqq-1.4.0/src/dbqq/connectors/databricks.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,35 +50,38 @@
             conn = super().__new__(Cluster, *args, **kwargs)
             conn.__init__()
             return conn
 
         return super().__new__(cls, *args, **kwargs)
 
     def __init__(self, hostname: str, http_path: str, access_token: str):
-        self.connection = databricks_sql.connect(
+        self.connection_kwargs = dict(
             server_hostname=hostname,
             http_path=http_path,
             access_token=access_token,
         )
-        self.cursor = self.connection.cursor()
 
     def __call__(self, query: str, scan_parquet_kwargs=None) -> pl.LazyFrame:
         """
         scan_parquet_kwargs are arguments which will be passed to
         https://pola-rs.github.io/polars/py-polars/html/reference/api/polars.scan_parquet.html#polars-scan-parquet
         """
         return super().__call__(query, scan_parquet_kwargs=scan_parquet_kwargs)
 
     def _run_query(self, query, *args, **kwargs) -> pl.LazyFrame:
+        self.connection = databricks_sql.connect(**self.connection_kwargs)
+        self.cursor = self.connection.cursor()
         self.cursor.execute(query)
-        return pl.from_arrow(self.cursor.fetchall_arrow()).lazy()
+        results = pl.from_arrow(self.cursor.fetchall_arrow()).lazy()
+        self.cursor.close()
+        self.connection.close()
+        return results
 
     def close(self):
-        self.connection.close()
-        self.cursor.close()
+        ...
 
     def describe_columns(self, table_name: str) -> pl.LazyFrame:
         query = f"describe {table_name}"
 
         description: pl.LazyFrame = self(query)
 
         self.description_query = (
@@ -141,15 +144,15 @@
         args = [connector_config[key] for key in self.targets]
         super().__init__(*args)
 
 
 class Cluster(_DatabricksBase):
     def __init__(self, *args, **kwargs):
         try:
-            from pyspark.sql import SparkSession
+            from pyspark.sql import SparkSession  # type: ignore
 
             self.spark = SparkSession.builder.getOrCreate()
         except ImportError:
             self.spark = None
 
     def _load_from_cache(*args, **kwargs) -> pl.LazyFrame:
         return
```

### Comparing `dbqq-1.3.7/src/dbqq/connectors/mssql.py` & `dbqq-1.4.0/src/dbqq/connectors/mssql.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.3.7/src/dbqq/connectors/oracle.py` & `dbqq-1.4.0/src/dbqq/connectors/oracle.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.3.7/src/dbqq/data/parsed/sql.py` & `dbqq-1.4.0/src/dbqq/data/parsed/sql.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.3.7/src/dbqq/security/cli/decrypt_yaml.py` & `dbqq-1.4.0/src/dbqq/security/cli/decrypt_yaml.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.3.7/src/dbqq/security/cli/encrypt_yaml.py` & `dbqq-1.4.0/src/dbqq/security/cli/encrypt_yaml.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.3.7/src/dbqq/security/cli/write_keys.py` & `dbqq-1.4.0/src/dbqq/security/cli/write_keys.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.3.7/src/dbqq/security/functions/_functions.py` & `dbqq-1.4.0/src/dbqq/security/functions/_functions.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.3.7/src/dbqq/security/functions/_yaml.py` & `dbqq-1.4.0/src/dbqq/security/functions/_yaml.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.3.7/src/dbqq/security/helpers.py` & `dbqq-1.4.0/src/dbqq/security/helpers.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.3.7/src/dbqq/utils.py` & `dbqq-1.4.0/src/dbqq/utils.py`

 * *Files identical despite different names*

### Comparing `dbqq-1.3.7/src/dbqq.egg-info/PKG-INFO` & `dbqq-1.4.0/src/dbqq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbqq
-Version: 1.3.7
+Version: 1.4.0
 Summary: quickly connect to and query databases
 Author-email: Chris Mamon <chrisam1993@live.com>
 Project-URL: Homepage, https://github.com/Chr1sC0de/database-quick-query
 Project-URL: Bug Tracker, https://github.com/Chr1sC0de/database-quick-query/issues
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `dbqq-1.3.7/src/dbqq.egg-info/SOURCES.txt` & `dbqq-1.4.0/src/dbqq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

