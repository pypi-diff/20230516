# Comparing `tmp/braincube-aws-core-alpha-0.0.27.tar.gz` & `tmp/braincube-aws-core-alpha-0.0.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "braincube-aws-core-alpha-0.0.27.tar", last modified: Fri May 12 21:31:14 2023, max compression
+gzip compressed data, was "braincube-aws-core-alpha-0.0.28.tar", last modified: Tue May 16 06:39:30 2023, max compression
```

## Comparing `braincube-aws-core-alpha-0.0.27.tar` & `braincube-aws-core-alpha-0.0.28.tar`

### file list

```diff
@@ -1,36 +1,35 @@
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-12 21:31:14.164129 braincube-aws-core-alpha-0.0.27/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1066 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.27/LICENSE
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     9091 2023-05-12 21:31:14.164417 braincube-aws-core-alpha-0.0.27/PKG-INFO
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     8338 2023-05-12 07:04:00.000000 braincube-aws-core-alpha-0.0.27/README.md
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      103 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.27/pyproject.toml
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      933 2023-05-12 21:31:14.166020 braincube-aws-core-alpha-0.0.27/setup.cfg
--rw-r--r--   0 evangelosboudis   (501) staff       (20)       38 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.27/setup.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-12 21:31:14.147251 braincube-aws-core-alpha-0.0.27/src/
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-12 21:31:14.153547 braincube-aws-core-alpha-0.0.27/src/braincube_aws_core_alpha.egg-info/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     9091 2023-05-12 21:31:14.000000 braincube-aws-core-alpha-0.0.27/src/braincube_aws_core_alpha.egg-info/PKG-INFO
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      769 2023-05-12 21:31:14.000000 braincube-aws-core-alpha-0.0.27/src/braincube_aws_core_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        1 2023-05-12 21:31:14.000000 braincube-aws-core-alpha-0.0.27/src/braincube_aws_core_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)       48 2023-05-12 21:31:14.000000 braincube-aws-core-alpha-0.0.27/src/braincube_aws_core_alpha.egg-info/requires.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        5 2023-05-12 21:31:14.000000 braincube-aws-core-alpha-0.0.27/src/braincube_aws_core_alpha.egg-info/top_level.txt
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-12 21:31:14.153855 braincube-aws-core-alpha-0.0.27/src/core/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.27/src/core/__init__.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-12 21:31:14.157563 braincube-aws-core-alpha-0.0.27/src/core/dal/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.27/src/core/dal/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1990 2023-05-11 11:52:40.000000 braincube-aws-core-alpha-0.0.27/src/core/dal/data.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      241 2023-05-11 10:53:14.000000 braincube-aws-core-alpha-0.0.27/src/core/dal/database_errors.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     3362 2023-05-12 12:29:46.000000 braincube-aws-core-alpha-0.0.27/src/core/dal/postgres_connection.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)    31571 2023-05-12 08:16:44.000000 braincube-aws-core-alpha-0.0.27/src/core/dal/postgres_repository.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      226 2023-05-12 11:56:51.000000 braincube-aws-core-alpha-0.0.27/src/core/dal/transaction_manager.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-12 21:31:14.159103 braincube-aws-core-alpha-0.0.27/src/core/di/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.27/src/core/di/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      561 2023-05-11 10:50:19.000000 braincube-aws-core-alpha-0.0.27/src/core/di/data.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     4122 2023-05-11 10:51:25.000000 braincube-aws-core-alpha-0.0.27/src/core/di/injector.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-12 21:31:14.161511 braincube-aws-core-alpha-0.0.27/src/core/rest/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.27/src/core/rest/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     2793 2023-05-11 10:52:14.000000 braincube-aws-core-alpha-0.0.27/src/core/rest/app_controller.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     3722 2023-05-11 10:52:31.000000 braincube-aws-core-alpha-0.0.27/src/core/rest/app_module.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     3598 2023-05-11 17:50:46.000000 braincube-aws-core-alpha-0.0.27/src/core/rest/data.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-12 21:31:14.163469 braincube-aws-core-alpha-0.0.27/src/core/utils/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.27/src/core/utils/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      738 2023-05-10 14:02:40.000000 braincube-aws-core-alpha-0.0.27/src/core/utils/convert.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1377 2023-05-11 10:53:41.000000 braincube-aws-core-alpha-0.0.27/src/core/utils/data.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-16 06:39:30.063559 braincube-aws-core-alpha-0.0.28/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1066 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.28/LICENSE
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     9091 2023-05-16 06:39:30.063844 braincube-aws-core-alpha-0.0.28/PKG-INFO
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     8338 2023-05-12 07:04:00.000000 braincube-aws-core-alpha-0.0.28/README.md
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      103 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.28/pyproject.toml
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      933 2023-05-16 06:39:30.065204 braincube-aws-core-alpha-0.0.28/setup.cfg
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)       38 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.28/setup.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-16 06:39:30.048211 braincube-aws-core-alpha-0.0.28/src/
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-16 06:39:30.052795 braincube-aws-core-alpha-0.0.28/src/braincube_aws_core_alpha.egg-info/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     9091 2023-05-16 06:39:30.000000 braincube-aws-core-alpha-0.0.28/src/braincube_aws_core_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      733 2023-05-16 06:39:30.000000 braincube-aws-core-alpha-0.0.28/src/braincube_aws_core_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        1 2023-05-16 06:39:30.000000 braincube-aws-core-alpha-0.0.28/src/braincube_aws_core_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)       48 2023-05-16 06:39:30.000000 braincube-aws-core-alpha-0.0.28/src/braincube_aws_core_alpha.egg-info/requires.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        5 2023-05-16 06:39:30.000000 braincube-aws-core-alpha-0.0.28/src/braincube_aws_core_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-16 06:39:30.053381 braincube-aws-core-alpha-0.0.28/src/core/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.28/src/core/__init__.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-16 06:39:30.055855 braincube-aws-core-alpha-0.0.28/src/core/dal/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.28/src/core/dal/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1990 2023-05-15 18:52:22.000000 braincube-aws-core-alpha-0.0.28/src/core/dal/data.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      241 2023-05-11 10:53:14.000000 braincube-aws-core-alpha-0.0.28/src/core/dal/database_errors.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     4110 2023-05-15 11:28:42.000000 braincube-aws-core-alpha-0.0.28/src/core/dal/postgres_connection.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)    33110 2023-05-15 18:42:36.000000 braincube-aws-core-alpha-0.0.28/src/core/dal/postgres_repository.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-16 06:39:30.057300 braincube-aws-core-alpha-0.0.28/src/core/di/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.28/src/core/di/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      561 2023-05-11 10:50:19.000000 braincube-aws-core-alpha-0.0.28/src/core/di/data.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     4122 2023-05-11 10:51:25.000000 braincube-aws-core-alpha-0.0.28/src/core/di/injector.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-16 06:39:30.059531 braincube-aws-core-alpha-0.0.28/src/core/rest/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.28/src/core/rest/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     2793 2023-05-11 10:52:14.000000 braincube-aws-core-alpha-0.0.28/src/core/rest/app_controller.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     3722 2023-05-11 10:52:31.000000 braincube-aws-core-alpha-0.0.28/src/core/rest/app_module.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     3598 2023-05-11 17:50:46.000000 braincube-aws-core-alpha-0.0.28/src/core/rest/data.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-16 06:39:30.062966 braincube-aws-core-alpha-0.0.28/src/core/utils/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.28/src/core/utils/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      738 2023-05-15 14:42:55.000000 braincube-aws-core-alpha-0.0.28/src/core/utils/convert.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1377 2023-05-11 10:53:41.000000 braincube-aws-core-alpha-0.0.28/src/core/utils/data.py
```

### Comparing `braincube-aws-core-alpha-0.0.27/LICENSE` & `braincube-aws-core-alpha-0.0.28/LICENSE`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.27/PKG-INFO` & `braincube-aws-core-alpha-0.0.28/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: braincube-aws-core-alpha
-Version: 0.0.27
+Version: 0.0.28
 Summary: Microframework for python aws lambdas
 Home-page: https://bitbucket.org/braincube-common/core-aws.git
 Author: Braincube
 Author-email: v.boudis@braincube.gr
 License: MIT
 Keywords: python,amazon,aws,lambda,routing,dal,injection
 Classifier: Intended Audience :: Developers
```

### Comparing `braincube-aws-core-alpha-0.0.27/README.md` & `braincube-aws-core-alpha-0.0.28/README.md`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.27/setup.cfg` & `braincube-aws-core-alpha-0.0.28/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = braincube-aws-core-alpha
-version = 0.0.27
+version = 0.0.28
 author = Braincube
 author_email = v.boudis@braincube.gr
 description = Microframework for python aws lambdas
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://bitbucket.org/braincube-common/core-aws.git
 license = MIT
```

### Comparing `braincube-aws-core-alpha-0.0.27/src/braincube_aws_core_alpha.egg-info/PKG-INFO` & `braincube-aws-core-alpha-0.0.28/src/braincube_aws_core_alpha.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: braincube-aws-core-alpha
-Version: 0.0.27
+Version: 0.0.28
 Summary: Microframework for python aws lambdas
 Home-page: https://bitbucket.org/braincube-common/core-aws.git
 Author: Braincube
 Author-email: v.boudis@braincube.gr
 License: MIT
 Keywords: python,amazon,aws,lambda,routing,dal,injection
 Classifier: Intended Audience :: Developers
```

### Comparing `braincube-aws-core-alpha-0.0.27/src/braincube_aws_core_alpha.egg-info/SOURCES.txt` & `braincube-aws-core-alpha-0.0.28/src/braincube_aws_core_alpha.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 src/braincube_aws_core_alpha.egg-info/top_level.txt
 src/core/__init__.py
 src/core/dal/__init__.py
 src/core/dal/data.py
 src/core/dal/database_errors.py
 src/core/dal/postgres_connection.py
 src/core/dal/postgres_repository.py
-src/core/dal/transaction_manager.py
 src/core/di/__init__.py
 src/core/di/data.py
 src/core/di/injector.py
 src/core/rest/__init__.py
 src/core/rest/app_controller.py
 src/core/rest/app_module.py
 src/core/rest/data.py
```

### Comparing `braincube-aws-core-alpha-0.0.27/src/core/dal/data.py` & `braincube-aws-core-alpha-0.0.28/src/core/dal/data.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.27/src/core/dal/postgres_connection.py` & `braincube-aws-core-alpha-0.0.28/src/core/dal/postgres_connection.py`

 * *Files 22% similar despite different names*

```diff
@@ -46,29 +46,49 @@
     return await create_pool(user=user, password=password, database=database, host=host, port=port,
                              min_size=min_size, max_size=max_size,
                              max_inactive_connection_lifetime=max_inactive_connection_lifetime,
                              init=__init)
 
 
 @asynccontextmanager
-async def transactional(pool: Pool = None, connection: Connection = None):
+async def create_transaction(pool: Pool = None, connection: Connection = None):
     """Create a database transaction conditionally. If connection is provided then this
     connection is returned immediately without creating any transaction, if not then a
     transaction is established using a connection acquired from provided connection pool.
     :param pool: (asyncpg) Connection pool.
     :param connection: (asyncpg) Connection.
     :raise DatabaseError: If nor connection neither connection pool are specified.
     :return: Transactional connection.
     """
 
     if connection:
         yield connection
     elif pool:
-        async with pool.acquire() as connection, connection.transaction():
-            yield connection
+        async with pool.acquire() as _connection, _connection.transaction():
+            yield _connection
+    else:
+        raise DatabaseError("nor connection neither connection pool are specified")
+
+
+@asynccontextmanager
+async def create_connection(pool: Pool = None, connection: Connection = None):
+    """Create a database connection conditionally. If connection is provided then this
+    connection is returned immediately, if not then a connection is acquired from provided
+    connection pool.
+    :param pool: (asyncpg) Connection pool.
+    :param connection: (asyncpg) Connection.
+    :raise DatabaseError: If nor connection neither connection pool are specified.
+    :return: Connection.
+    """
+
+    if connection:
+        yield connection
+    elif pool:
+        async with pool.acquire() as _connection:
+            yield _connection
     else:
         raise DatabaseError("nor connection neither connection pool are specified")
 
 
 async def __init(conn: Connection):
     await conn.set_type_codec("uuid", encoder=str, decoder=str, schema="pg_catalog")
     await conn.set_type_codec("numeric", encoder=str, decoder=float, schema="pg_catalog")
```

### Comparing `braincube-aws-core-alpha-0.0.27/src/core/dal/postgres_repository.py` & `braincube-aws-core-alpha-0.0.28/src/core/dal/postgres_repository.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from pydantic import BaseModel
 from pypika.queries import QueryBuilder
 from pypika import PostgreSQLQuery, Table, Field, Criterion, EmptyCriterion, CustomFunction, functions as fn
 
 from ..utils.data import Order, OrderType, Condition, ConditionType, Page, Pageable, Paging, Top, Metadata
 from .data import Key, Schema, SaveType, TableData, FieldData, RelatedTableData, OrderData, FieldType
 from .database_errors import DatabaseError, DeleteError, SaveError
-from .postgres_connection import Pool, Connection
+from .postgres_connection import Pool, Connection, create_connection
 
 T = TypeVar("T", bound=BaseModel)
 
 
 class PostgresRepository:
     """SQL based repository implementation.
     :param pool: Database connection pool.
@@ -246,93 +246,80 @@
             data_[column.name] = v
 
         if not data_:
             raise SaveError("no columns provided")
 
         return data_
 
-    def __init_select_query(self, fields: list[FieldData],
-                            criterion: Criterion = None,
-                            order: list[OrderData] = None,
-                            count_query: bool = False) -> tuple[QueryBuilder, QueryBuilder | None]:
+    def _init_select_query(self, aliases: list[str] = None,
+                           conditions: list[Condition] | Criterion = None,
+                           order: list[Order] = None,
+                           set_order: bool = True,
+                           count_query: bool = False) -> tuple[QueryBuilder, QueryBuilder | None]:
+
+        fields = self._aliases_to_fields(aliases)
+
+        criterion = conditions if conditions and isinstance(conditions, Criterion) \
+            else self._conditions_to_criterion(conditions)
 
-        q = PostgreSQLQuery.from_(self._master_table.table)
+        order_by = self._order_to_fields(order) if order else (self._order_by if set_order else None)
 
         table_aliases = self._related_forced_tables_aliases.copy()
+        table_aliases.extend([t.alias for t in criterion.tables_])
 
         for field in fields:
             if field.type_ == FieldType.statement and field.relations_aliases:
                 table_aliases.extend(field.relations_aliases)
             else:
                 table_aliases.append(field.field.table.alias)
 
-        if criterion:
-            table_aliases.extend([t.alias for t in criterion.tables_])
-            q = q.where(criterion)
+        if order_by:
+            table_aliases.extend([order_.field.table.alias for order_ in order_by])
 
-        if order:
-            table_aliases.extend([order_.field.table.alias for order_ in order])
+        q = PostgreSQLQuery \
+            .from_(self._master_table.table) \
+            .where(criterion)
 
         for alias in filter(lambda ta: ta != self._master_table.table.alias, set(table_aliases)):
             related_table = self._related_tables[alias]
             q = q \
                 .join(related_table.table, related_table.join_type) \
                 .on(self._master_table.table[related_table.join_through.from_column_name] ==
                     related_table.table[related_table.join_through.to_column_name])
 
         cq = q.select(fn.Count("*")) if count_query else None
 
         for field in fields:
             q = q.select(field.field)
 
-        if order:
-            for order_ in order:
+        if order_by:
+            for order_ in order_by:
                 q = q.orderby(order_.field, order=order_.order_type)
 
         return q, cq
 
-    def _init_select_query(self, aliases: list[str] = None,
-                           criterion: Criterion = None,
-                           order: list[Order] = None,
-                           set_order: bool = True,
-                           count_query: bool = False) -> tuple[QueryBuilder, QueryBuilder | None]:
-
-        fields = self._aliases_to_fields(aliases)
-        order_ = self._order_to_fields(order) if order else (self._order_by if set_order else None)
-
-        return self.__init_select_query(fields, criterion, order_, count_query)
-
     ####################################
     # Retrieve
     ####################################
 
-    async def _find_one(self, aliases: list[str] = None,
-                        criterion: Criterion = None,
-                        order: list[Order] = None,
-                        connection: Connection = None) -> dict[str, any] | None:
-
-        q, _ = self._init_select_query(aliases, criterion, order)
-
-        return await self._fetch_one(q.limit(1), connection=connection)
-
     async def find_one(self, aliases: list[str] = None,
-                       conditions: list[Condition] = None,
+                       conditions: list[Condition] | Criterion = None,
                        order: list[Order] = None,
                        connection: Connection = None) -> dict[str, any] | None:
         """Find one record from passed filters.
         :param aliases: List of fields that will be selected by the query.
         :param conditions: List of filters that will be applied to query.
         :param order: Order that will be applied to query.
         :param connection: (asyncpg) Connection that will execute the generated query.
         :return: Record as dictionary.
         """
 
-        criterion = self._conditions_to_criterion(conditions)
+        q, _ = self._init_select_query(aliases, conditions, order)
 
-        return await self._find_one(aliases, criterion, order, connection)
+        return await self._fetch_one(q.limit(1), connection=connection)
 
     async def find_by_pk(self, key: Key,
                          aliases: list[str] = None,
                          connection: Connection = None) -> dict[str, any] | None:
         """Find the record from passed key.
         :param key: Record identifier.
         :param aliases: List of fields that will be selected by the query.
@@ -353,38 +340,29 @@
         :return: Record existence.
         """
 
         aliases = [pk.field.alias for pk in self._primary_key.values()]
 
         return await self.find_by_pk(key, aliases, connection) is not None
 
-    async def _find_all(self, aliases: list[str] = None,
-                        criterion: Criterion = None,
-                        order: list[Order] = None,
-                        connection: Connection = None) -> list[dict[str, any]]:
-
-        q, _ = self._init_select_query(aliases, criterion, order)
-
-        return await self._fetch(q, connection=connection)
-
     async def find_all(self, aliases: list[str] = None,
-                       conditions: list[Condition] = None,
+                       conditions: list[Condition] | Criterion = None,
                        order: list[Order] = None,
                        connection: Connection = None) -> list[dict[str, any]]:
         """Find all records from passed filters.
         :param aliases: List of fields that will be selected by the query.
         :param conditions: List of filters that will be applied to query.
         :param order: Order in which the records will be returned.
         :param connection: (asyncpg) Connection that will execute the generated query.
         :return: Records as dictionary list.
         """
 
-        criterion = self._conditions_to_criterion(conditions)
+        q, _ = self._init_select_query(aliases, conditions, order)
 
-        return await self._find_all(aliases, criterion, order, connection)
+        return await self._fetch(q, connection=connection)
 
     async def find_all_by_pk(self, keys: list[Key],
                              aliases: list[str] = None,
                              order: list[Order] = None,
                              connection: Connection = None) -> list[dict[str, any]]:
         """Find all records from passed keys.
         :param keys: Records identifiers.
@@ -395,89 +373,132 @@
         """
 
         if not keys:
             raise DatabaseError("no keys provided")
 
         criterion = Criterion.any([self._create_primary_key_criterion(key) for key in keys])
 
-        return await self._find_all(aliases, criterion, order, connection)
-
-    async def __find_many(self, connection: Connection,
-                          aliases: list[str] = None,
-                          criterion: Criterion = None,
-                          page: Pageable = Pageable(),
-                          order: list[Order] = None) -> Page | Top:
-
-        if page.top_size < 0:
-            data = await self._find_all(aliases, criterion, order, connection)
-            return Top(data, page.top_size, False)
-
-        start = time.time()
-
-        calc_top = page.top_size > 0
-        q, cq = self._init_select_query(aliases, criterion, order, count_query=not calc_top)
-
-        # top implementation
-        if calc_top:
-            records = await self._fetch(q.limit(page.top_size + 1), connection=connection)
-            has_more = len(records) > page.top_size
-            return Top(records[:-1] if has_more else records, page.top_size, has_more)
-
-        # paging implementation
-        page_no = page.page_no if page.page_no > 0 else 1
-        records = await self._fetch(q.limit(page.page_size).offset((page_no - 1) * page.page_size),
-                                    connection=connection)
-
-        # retrieve count only if we do not mention page ether we are not on
-        # first page and there are no records from first retrieve
-        count = None
-        total_pages = None
-        retrieve_pre_page = len(records) == 0 and page.page_no > 1
-
-        if retrieve_pre_page or page.page_no == 0:
-            record = await self._fetch_one(cq, connection=connection)
-            count = record["count"] if record.get("count") else 0
-            total_pages = math.ceil(count / page.page_size)
-
-        if retrieve_pre_page and total_pages > 0:
-            page_no = total_pages
-            records = await self._fetch(q.limit(page.page_size).offset((page_no - 1) * page.page_size),
-                                        connection=connection)
-
-        return Page(records, Paging(page_no, page.page_size, total_pages, count),
-                    Metadata(int((time.time() - start) * 1000)))
-
-    async def _find_many(self, aliases: list[str] = None,
-                         criterion: Criterion = None,
-                         page: Pageable = Pageable(),
-                         order: list[Order] = None,
-                         connection: Connection = None) -> Page | Top:
-
-        if connection:
-            return await self.__find_many(connection, aliases, criterion, page, order)
-        async with self._pool.acquire() as connection_:
-            return await self.__find_many(connection_, aliases, criterion, page, order)
+        return await self.find_all(aliases, criterion, order, connection)
 
     async def find_many(self, aliases: list[str] = None,
-                        conditions: list[Condition] = None,
+                        conditions: list[Condition] | Criterion = None,
                         page: Pageable = Pageable(),
                         order: list[Order] = None,
                         connection: Connection = None) -> Page | Top:
         """Find records from passed filters using paging.
         :param aliases: List of fields that will be selected by the query.
         :param conditions: List of filters that will be applied to query.
         :param page: Limit and offset of the query.
         :param order: Order in which the records will be returned.
         :param connection: (asyncpg) Connection that will execute the generated query.
         :return: Records wrapped by Page or Top dataclass.
         """
 
-        criterion = self._conditions_to_criterion(conditions)
+        async with create_connection(self._pool, connection) as _connection:
+
+            if page.top_size < 0:
+                data = await self.find_all(aliases, conditions, order, _connection)
+                return Top(data, page.top_size, False)
+
+            start = time.time()
+
+            calc_top = page.top_size > 0
+            q, cq = self._init_select_query(aliases, conditions, order, count_query=not calc_top)
+
+            # top implementation
+            if calc_top:
+                records = await self._fetch(q.limit(page.top_size + 1), connection=_connection)
+                has_more = len(records) > page.top_size
+                return Top(records[:-1] if has_more else records, page.top_size, has_more)
+
+            # paging implementation
+            page_no = page.page_no if page.page_no > 0 else 1
+            records = await self._fetch(q.limit(page.page_size).offset((page_no - 1) * page.page_size),
+                                        connection=_connection)
+
+            # retrieve count only if we do not mention page ether we are not on
+            # first page and there are no records from first retrieve
+            count = None
+            total_pages = None
+            retrieve_pre_page = len(records) == 0 and page.page_no > 1
+
+            if retrieve_pre_page or page.page_no == 0:
+                record = await self._fetch_one(cq, connection=_connection)
+                count = record["count"] if record.get("count") else 0
+                total_pages = math.ceil(count / page.page_size)
+
+            if retrieve_pre_page and total_pages > 0:
+                page_no = total_pages
+                records = await self._fetch(q.limit(page.page_size).offset((page_no - 1) * page.page_size),
+                                            connection=_connection)
+
+            return Page(records, Paging(page_no, page.page_size, total_pages, count),
+                        Metadata(int((time.time() - start) * 1000)))
+
+    async def find_one_data(self, cls: type[T],
+                            conditions: list[Condition] | Criterion = None,
+                            order: list[Order] = None,
+                            connection: Connection = None) -> T | None:
+        """Find one record from passed filters.
+        :param cls: Result type.
+        :param conditions: List of filters that will be applied to query.
+        :param order: Order that will be applied to query.
+        :param connection: (asyncpg) Connection that will execute the generated query.
+        :return: Record as returning type.
+        """
+
+        result = await self.find_one(self.__base_model_aliases(cls), conditions, order, connection)
+
+        return cls.construct(**result) if result else None
+
+    async def find_by_pk_data(self, key: Key,
+                              cls: type[T],
+                              connection: Connection = None) -> T | None:
+        """Find the record from passed key.
+        :param key: Record identifier.
+        :param cls: Result type.
+        :param connection: (asyncpg) Connection that will execute the generated query.
+        :return: Records as returning type.
+        """
+
+        result = await self.find_by_pk(key, self.__base_model_aliases(cls), connection)
+
+        return cls.construct(**result) if result else None
+
+    async def find_all_data(self, cls: type[T],
+                            conditions: list[Condition] | Criterion = None,
+                            order: list[Order] = None,
+                            connection: Connection = None) -> list[T]:
+        """Find all records from passed filters.
+        :param cls: Result type.
+        :param conditions: List of filters that will be applied to query.
+        :param order: Order in which the records will be returned.
+        :param connection: (asyncpg) Connection that will execute the generated query.
+        :return: Records as returning type.
+        """
+
+        results = await self.find_all(self.__base_model_aliases(cls), conditions, order, connection)
+
+        return [cls.construct(**r) for r in results] if results else None
+
+    async def find_all_by_pk_data(self, keys: list[Key],
+                                  cls: type[T],
+                                  order: list[Order] = None,
+                                  connection: Connection = None) -> list[T]:
+        """Find all records from passed keys.
+        :param keys: Records identifiers.
+        :param cls: Result type.
+        :param order: Order in which the records will be returned.
+        :param connection: (asyncpg) Connection that will execute the generated query.
+        :return: Records as returning type.
+        """
+
+        results = await self.find_all_by_pk(keys, self.__base_model_aliases(cls), order, connection)
 
-        return await self._find_many(aliases, criterion, page, order, connection)
+        return [cls.construct(**r) for r in results] if results else None
 
     ####################################
     # Create
     ####################################
 
     async def insert(self, data: BaseModel | dict[str, any],
                      returning_aliases: list[str] = None,
@@ -500,39 +521,28 @@
             .columns(list(data_.keys())) \
             .insert(list(data_.values()))
 
         records = await self._execute(iq, returning_aliases, connection)
 
         return records[0] if len(records) > 0 else None
 
-    async def insert_returning_master(self, data: BaseModel | dict[str, any],
-                                      connection: Connection = None):
-        """Insert one record from dictionary and return all master columns.
-        :param data: Master column aliases with values.
-        :param connection: (asyncpg) Connection that will execute the generated query.
-        :raise SaveError: When does not adjust to insert-constraints or no master column is specified.
-        :return: Execution results as dictionary.
-        """
-
-        return await self.insert(data, list(self._master_columns.keys()), connection)
-
     async def insert_data(self, data: BaseModel | dict[str, any],
                           returning: type[T],
                           connection: Connection = None) -> T:
         """Insert a record using model.
         :param data: Model which contains master table column properties.
         :param returning: Result type.
         :param connection: (asyncpg) Connection that will execute the generated query.
         :raise SaveError: When does not adjust to insert-constraints or no master column is specified.
         :return: Execution results with returning type.
         """
 
         result = await self.insert(data, self.__base_model_aliases(returning), connection)
 
-        return returning(**result) if result else None
+        return returning.construct(**result) if result else None
 
     async def insert_bulk(self, aliases: list[str],
                           data: list[list],
                           returning_aliases: list[str] = None,
                           connection: Connection = None) -> list[dict[str, any]]:
         """Insert many records at once from list.
         :param aliases: Master column aliases.
@@ -568,86 +578,79 @@
 
         return await self._execute(iq, returning_aliases, connection)
 
     ####################################
     # Update
     ####################################
 
-    async def _update(self, data: BaseModel | dict[str, any],
-                      criterion: Criterion,
-                      returning_aliases: list[str] = None,
-                      connection: Connection = None) -> list[dict[str, any]] | None:
+    async def update(self, data: BaseModel | dict[str, any],
+                     conditions: list[Condition] | Criterion,
+                     returning_aliases: list[str] = None,
+                     connection: Connection = None) -> list[dict[str, any]] | None:
+        """Update records with new data according conditions.
+        :param data: Master column aliases with values.
+        :param conditions: Filters that will be applied into the query.
+        :param returning_aliases: Query returning data.
+        :param connection: (asyncpg) Connection that will execute the generated query.
+        :raise SaveError: When does not adjust to update-constraints or no master column is specified.
+        :return: Execution results as dictionary list.
+        """
+
+        if not conditions or isinstance(conditions, EmptyCriterion):
+            raise DeleteError("update without conditions is not allowed")
 
-        if isinstance(criterion, EmptyCriterion):
-            raise SaveError("update without conditions is not allowed")
+        criterion = conditions if isinstance(conditions, Criterion) \
+            else self._conditions_to_criterion(conditions, select=False)
 
         uq = PostgreSQLQuery.update(self._master_table.name)
 
         data_ = data.dict(by_alias=True, exclude_unset=True) if isinstance(data, BaseModel) else data.copy()
 
         for v, k in self._filter_save_data(data_, SaveType.update).items():
             uq = uq.set(v, k)
+
         uq = uq.where(criterion)
 
         return await self._execute(uq, returning_aliases, connection)
 
-    async def update(self, data: BaseModel | dict[str, any],
-                     conditions: list[Condition],
-                     returning_aliases: list[str] = None,
-                     connection: Connection = None) -> list[dict[str, any]] | None:
-        """Update records with new data according conditions.
+    async def update_by_pk(self, key: Key,
+                           data: BaseModel | dict[str, any],
+                           returning_aliases: list[str] = None,
+                           connection: Connection = None) -> dict[str, any] | None:
+        """Update record with new data according to passed key.
+        :param key: Record identifier.
         :param data: Master column aliases with values.
-        :param conditions: List of filters that will be applied into the query.
         :param returning_aliases: Query returning data.
         :param connection: (asyncpg) Connection that will execute the generated query.
         :raise SaveError: When does not adjust to update-constraints or no master column is specified.
-        :return: Execution results as dictionary list.
+        :return: Execution result as dictionary.
         """
 
-        criterion = self._conditions_to_criterion(conditions, select=False)
+        criterion = self._create_primary_key_criterion(key, select=False)
 
-        return await self._update(data, criterion, returning_aliases, connection)
+        records = await self.update(data, criterion, returning_aliases, connection)
 
-    # _update_data: criterion: Criterion
+        return records[0] if len(records) > 0 else None
 
     async def update_data(self, data: BaseModel | dict[str, any],
-                          conditions: list[Condition],
+                          conditions: list[Condition] | Criterion,
                           returning: type[T],
                           connection: Connection = None) -> list[T] | None:
         """Update records with new data according conditions using model.
         :param data: Model which contains master table column properties.
         :param conditions: List of filters that will be applied into the query.
         :param returning: Result type.
         :param connection: (asyncpg) Connection that will execute the generated query.
         :raise SaveError: When does not adjust to update-constraints or no master column is specified.
         :return: Execution results with returning type.
         """
 
         results = await self.update(data, conditions, self.__base_model_aliases(returning), connection)
 
-        return [returning(**r) for r in results] if results else None
-
-    async def update_by_pk(self, key: Key,
-                           data: BaseModel | dict[str, any],
-                           returning_aliases: list[str] = None,
-                           connection: Connection = None) -> dict[str, any] | None:
-        """Update record with new data according to passed key.
-        :param key: Record identifier.
-        :param data: Master column aliases with values.
-        :param returning_aliases: Query returning data.
-        :param connection: (asyncpg) Connection that will execute the generated query.
-        :raise SaveError: When does not adjust to update-constraints or no master column is specified.
-        :return: Execution result as dictionary.
-        """
-
-        criterion = self._create_primary_key_criterion(key, select=False)
-
-        records = await self._update(data, criterion, returning_aliases, connection)
-
-        return records[0] if len(records) > 0 else None
+        return [returning.construct(**r) for r in results] if results else None
 
     async def update_data_by_pk(self, key: Key,
                                 data: BaseModel | dict[str, any],
                                 returning: type[T],
                                 connection: Connection = None) -> T | None:
         """Update record with new data according to passed key using model.
         :param key: Record identifier.
@@ -656,58 +659,82 @@
         :param connection: (asyncpg) Connection that will execute the generated query.
         :raise SaveError: When does not adjust to update-constraints or no master column is specified.
         :return: Execution result with returning type.
         """
 
         result = await self.update_by_pk(key, data, self.__base_model_aliases(returning), connection)
 
-        return returning(**result) if result else None
+        return returning.construct(**result) if result else None
 
     ####################################
     # Delete
     ####################################
 
-    async def _delete(self, criterion: Criterion,
-                      returning_aliases: list[str] = None,
-                      connection: Connection = None) -> list[dict[str, any]] | None:
-
-        if isinstance(criterion, EmptyCriterion):
-            raise DeleteError("delete without conditions is not allowed")
-
-        dq = PostgreSQLQuery \
-            .from_(self._master_table.name) \
-            .delete() \
-            .where(criterion)
-
-        return await self._execute(dq, returning_aliases, connection)
-
-    async def delete(self, conditions: list[Condition],
+    async def delete(self, conditions: list[Condition] | Criterion,
                      returning_aliases: list[str] = None,
                      connection: Connection = None) -> list[dict[str, any]] | None:
         """Delete records according conditions.
-        :param conditions: List of filters that will be applied into the query.
+        :param conditions: Filters that will be applied into the query.
         :param returning_aliases: Query returning data.
         :param connection: (asyncpg) Connection that will execute the generated query.
-        :raise SaveError: When conditions are empty.
+        :raise DeleteError: When conditions are empty.
         :return: Execution results as dictionary list.
         """
 
-        criterion = self._conditions_to_criterion(conditions, select=False)
+        if not conditions or isinstance(conditions, EmptyCriterion):
+            raise DeleteError("delete without conditions is not allowed")
+
+        criterion = conditions if isinstance(conditions, Criterion) \
+            else self._conditions_to_criterion(conditions, select=False)
+
+        dq = PostgreSQLQuery \
+            .from_(self._master_table.name) \
+            .delete() \
+            .where(criterion)
 
-        return await self._delete(criterion, returning_aliases, connection)
+        return await self._execute(dq, returning_aliases, connection)
 
     async def delete_by_pk(self, key: Key,
                            returning_aliases: list[str] = None,
                            connection: Connection = None) -> dict[str, any] | None:
         """Delete records according to passed key.
         :param key: Record identifier.
         :param returning_aliases: Query returning data.
         :param connection: (asyncpg) Connection that will execute the generated query.
-        :raise SaveError: When conditions are empty.
+        :raise DeleteError: When conditions are empty.
         :return: Execution results as dictionary.
         """
 
         criterion = self._create_primary_key_criterion(key, select=False)
 
-        records = await self._delete(criterion, returning_aliases, connection)
+        records = await self.delete(criterion, returning_aliases, connection)
 
         return records[0] if len(records) > 0 else None
+
+    async def delete_data(self, conditions: list[Condition] | Criterion,
+                          returning: type[T],
+                          connection: Connection = None) -> list[T] | None:
+        """Delete records according conditions.
+        :param conditions: Filters that will be applied into the query.
+        :param returning: Result type.
+        :param connection: (asyncpg) Connection that will execute the generated query.
+        :raise DeleteError: When conditions are empty.
+        :return: Execution results with returning type.
+        """
+
+        results = await self.delete(conditions, self.__base_model_aliases(returning), connection)
+
+        return [returning.construct(**r) for r in results] if results else None
+
+    async def delete_data_by_pk(self, key: Key,
+                                returning: type[T],
+                                connection: Connection = None) -> T | None:
+        """Delete record according to passed key.
+        :param key: Record identifier.
+        :param returning: Result type.
+        :param connection: (asyncpg) Connection that will execute the generated query.
+        :return: Execution result with returning type.
+        """
+
+        result = await self.delete_by_pk(key, self.__base_model_aliases(returning), connection)
+
+        return returning.construct(**result) if result else None
```

### Comparing `braincube-aws-core-alpha-0.0.27/src/core/di/data.py` & `braincube-aws-core-alpha-0.0.28/src/core/di/data.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.27/src/core/di/injector.py` & `braincube-aws-core-alpha-0.0.28/src/core/di/injector.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.27/src/core/rest/app_controller.py` & `braincube-aws-core-alpha-0.0.28/src/core/rest/app_controller.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.27/src/core/rest/app_module.py` & `braincube-aws-core-alpha-0.0.28/src/core/rest/app_module.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.27/src/core/rest/data.py` & `braincube-aws-core-alpha-0.0.28/src/core/rest/data.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.27/src/core/utils/convert.py` & `braincube-aws-core-alpha-0.0.28/src/core/utils/convert.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.27/src/core/utils/data.py` & `braincube-aws-core-alpha-0.0.28/src/core/utils/data.py`

 * *Files identical despite different names*

