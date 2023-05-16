# Comparing `tmp/macrostrat_database-2.1.1.tar.gz` & `tmp/macrostrat_database-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrostrat_database-2.1.1.tar", max compression
+gzip compressed data, was "macrostrat_database-2.1.2.tar", max compression
```

## Comparing `macrostrat_database-2.1.1.tar` & `macrostrat_database-2.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     5975 2023-04-11 05:06:58.495410 macrostrat_database-2.1.1/macrostrat/database/__init__.py
--rw-r--r--   0        0        0     4665 2023-04-11 04:58:29.434832 macrostrat_database-2.1.1/macrostrat/database/mapper/__init__.py
--rw-r--r--   0        0        0      686 2022-05-26 00:55:15.936699 macrostrat_database-2.1.1/macrostrat/database/mapper/base.py
--rw-r--r--   0        0        0     2272 2022-05-26 05:21:07.121385 macrostrat_database-2.1.1/macrostrat/database/mapper/cache.py
--rw-r--r--   0        0        0     3271 2023-04-11 05:06:58.496060 macrostrat_database-2.1.1/macrostrat/database/mapper/utils.py
--rw-r--r--   0        0        0     1630 2022-05-26 00:55:15.936016 macrostrat_database-2.1.1/macrostrat/database/postgresql.py
--rw-r--r--   0        0        0    12662 2023-04-25 21:41:15.569926 macrostrat_database-2.1.1/macrostrat/database/utils.py
--rw-r--r--   0        0        0      598 2023-04-25 21:41:39.945703 macrostrat_database-2.1.1/pyproject.toml
--rw-r--r--   0        0        0      756 1970-01-01 00:00:00.000000 macrostrat_database-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0     5975 2023-04-11 05:06:58.495410 macrostrat_database-2.1.2/macrostrat/database/__init__.py
+-rw-r--r--   0        0        0     4665 2023-04-11 04:58:29.434832 macrostrat_database-2.1.2/macrostrat/database/mapper/__init__.py
+-rw-r--r--   0        0        0      686 2022-05-26 00:55:15.936699 macrostrat_database-2.1.2/macrostrat/database/mapper/base.py
+-rw-r--r--   0        0        0     2272 2022-05-26 05:21:07.121385 macrostrat_database-2.1.2/macrostrat/database/mapper/cache.py
+-rw-r--r--   0        0        0     3271 2023-04-11 05:06:58.496060 macrostrat_database-2.1.2/macrostrat/database/mapper/utils.py
+-rw-r--r--   0        0        0     1630 2022-05-26 00:55:15.936016 macrostrat_database-2.1.2/macrostrat/database/postgresql.py
+-rw-r--r--   0        0        0    14193 2023-05-16 20:02:34.748416 macrostrat_database-2.1.2/macrostrat/database/utils.py
+-rw-r--r--   0        0        0      598 2023-05-16 20:02:34.748658 macrostrat_database-2.1.2/pyproject.toml
+-rw-r--r--   0        0        0      756 1970-01-01 00:00:00.000000 macrostrat_database-2.1.2/PKG-INFO
```

### Comparing `macrostrat_database-2.1.1/macrostrat/database/__init__.py` & `macrostrat_database-2.1.2/macrostrat/database/__init__.py`

 * *Files identical despite different names*

### Comparing `macrostrat_database-2.1.1/macrostrat/database/mapper/__init__.py` & `macrostrat_database-2.1.2/macrostrat/database/mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `macrostrat_database-2.1.1/macrostrat/database/mapper/base.py` & `macrostrat_database-2.1.2/macrostrat/database/mapper/base.py`

 * *Files identical despite different names*

### Comparing `macrostrat_database-2.1.1/macrostrat/database/mapper/cache.py` & `macrostrat_database-2.1.2/macrostrat/database/mapper/cache.py`

 * *Files identical despite different names*

### Comparing `macrostrat_database-2.1.1/macrostrat/database/mapper/utils.py` & `macrostrat_database-2.1.2/macrostrat/database/mapper/utils.py`

 * *Files identical despite different names*

### Comparing `macrostrat_database-2.1.1/macrostrat/database/postgresql.py` & `macrostrat_database-2.1.2/macrostrat/database/postgresql.py`

 * *Files identical despite different names*

### Comparing `macrostrat_database-2.1.1/macrostrat/database/utils.py` & `macrostrat_database-2.1.2/macrostrat/database/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -109,14 +109,15 @@
     if isinstance(sql, Path):
         if echo_file_name:
             secho(sql.name, fg="cyan", bold=True)
         sql = sql.read_text()
 
     return sql
 
+
 def _get_queries(sql, interpret_as_file=None):
     if isinstance(sql, (list, tuple)):
         queries = []
         for i in sql:
             queries.extend(_get_queries(i, interpret_as_file=interpret_as_file))
         return queries
     if isinstance(sql, SQL):
@@ -130,19 +131,22 @@
         sql = canonicalize_query(sql)
 
     if isinstance(sql, Path):
         sql = sql.read_text()
 
     return split(sql)
 
+
 def _is_prebind_param(param):
     return isinstance(param, Composable)
 
+
 def _split_params(params):
-    params = params or []
+    if params is None:
+        return None, None
     new_params = []
     new_bind_params = []
     if isinstance(params, (list, tuple)):
         for i in params:
             if _is_prebind_param(i):
                 new_bind_params.append(i)
             else:
@@ -155,14 +159,15 @@
                 new_bind_params[k] = v
             else:
                 new_params[k] = v
     if len(new_bind_params) == 0:
         new_bind_params = None
     return new_params, new_bind_params
 
+
 def _get_cursor(connectable):
     if isinstance(connectable, Engine):
         conn = connectable.connect()
 
     # Find a connection or cursor object for the connectable
     conn = connectable
     if hasattr(conn, "raw_connection"):
@@ -173,45 +178,57 @@
         else:
             conn = conn.connection
     if hasattr(conn, "cursor"):
         conn = conn.cursor()
 
     return conn
 
+
 def _get_connection(connectable):
     if isinstance(connectable, Engine):
         return connectable.connect()
     if isinstance(connectable, Connection):
         return connectable
     if not hasattr(connectable, "connection"):
         return connectable
     conn = connectable.connection
     if callable(conn):
         return conn()
     return conn
-    
+
 
 def _render_query(query: Union[SQL, Composed], connectable: Union[Engine, Connection]):
     """Render a query to a SQL string."""
     if not isinstance(query, (Composed, SQL)):
         return query
     # Find a connection or cursor object for the connectable
     conn = _get_cursor(connectable)
     return query.as_string(conn)
 
-            
+
+def infer_has_server_binds(sql):
+    return "%s" in sql or search(r"%\(\w+\)s", sql)
+
+
 def _run_sql(connectable, sql, **kwargs):
+    """
+    Internal function for running a query on a SQLAlchemy connectable,
+    which always returns an iterator. The wrapper function adds the option
+    to return a list of results.
+    """
     if isinstance(connectable, Engine):
         with connectable.connect() as conn:
             yield from _run_sql(conn, sql, **kwargs)
             return
 
     params = kwargs.pop("params", None)
     stop_on_error = kwargs.pop("stop_on_error", False)
     raise_errors = kwargs.pop("raise_errors", False)
+    has_server_binds = kwargs.pop("has_server_binds", None)
+
     if stop_on_error:
         raise_errors = True
         warn(DeprecationWarning("stop_on_error is deprecated, use raise_errors"))
 
     interpret_as_file = kwargs.pop("interpret_as_file", None)
 
     queries = _get_queries(sql, interpret_as_file=interpret_as_file)
@@ -238,22 +255,22 @@
                 # Pre-bind the parameters using PsycoPG2
                 query = query.format(**pre_bind_params)
 
             if isinstance(query, (SQL, Composed)):
                 query = _render_query(query, connectable)
 
             sql_text = query
-            has_server_binds = False
             if isinstance(query, str):
                 sql_text = format(query, strip_comments=True).strip()
                 if sql_text == "":
                     continue
                 # Check for server-bound parameters in sql native style. If there are none, use
                 # the SQLAlchemy text() function, otherwise use the raw query string
-                has_server_binds = "%s" in sql_text or search(r'%\(\w+\)s', sql_text)
+                if has_server_binds is None:
+                    has_server_binds = infer_has_server_binds(sql_text)
 
             log.debug("Executing SQL: \n %s", query)
             if has_server_binds:
                 conn = _get_connection(connectable)
                 res = conn.exec_driver_sql(query, params)
             else:
                 res = connectable.execute(text(query), params=params)
@@ -280,14 +297,41 @@
 
 
 def run_sql_file(connectable, filename, **kwargs):
     return run_sql(connectable, filename, interpret_as_file=True, **kwargs)
 
 
 def run_sql(*args, **kwargs):
+    """
+    Run a query on a SQLAlchemy connectable.
+
+    Parameters
+    ----------
+    connectable : Union[Engine, Connection]
+        A SQLAlchemy engine or connection object.
+    sql : Union[str, Path, IO, SQL, Composed]
+        A SQL query, or a file containing a SQL query.
+    params : Union[dict, list, tuple]
+        Parameters to bind to the query. If a list or tuple, the parameters
+        will be bound to the query in order. If a dict, the parameters will
+        be bound to the query by name.
+    stop_on_error : bool
+        If True, stop running queries if an error is encountered.
+    raise_errors : bool
+        If True, raise errors encountered while running queries.
+    has_server_binds : bool
+        Interpret the query to have server-side bind parameters (requiring execution
+        with the backend driver). By default, this is inferred from the query string,
+        but inference is not always reliable.
+    interpret_as_file : bool
+        If True, force interpreting the query as a file path.
+    yield_results : bool
+        If True, yield the results of the query as they are executed, rather than
+        returning a list after completion.
+    """
     res = _run_sql(*args, **kwargs)
     if kwargs.pop("yield_results", False):
         return res
     return list(res)
 
 
 def execute(connectable, sql, params=None, stop_on_error=False):
```

### Comparing `macrostrat_database-2.1.1/pyproject.toml` & `macrostrat_database-2.1.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 authors = ["Daven Quinn <dev@davenquinn.com>"]
 description = "A SQLAlchemy-based database toolkit."
 name = "macrostrat.database"
 packages = [
   {include = "macrostrat"},
 ]
-version = "2.1.1"
+version = "2.1.2"
 
 [tool.poetry.dependencies]
 GeoAlchemy2 = "^0.9.4"
 SQLAlchemy = "^1.4.26"
 SQLAlchemy-Utils = "^0.37.0"
 click = "^8.1.3"
 "macrostrat.utils" = "^1.0.0"
```

### Comparing `macrostrat_database-2.1.1/PKG-INFO` & `macrostrat_database-2.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrostrat-database
-Version: 2.1.1
+Version: 2.1.2
 Summary: A SQLAlchemy-based database toolkit.
 Author: Daven Quinn
 Author-email: dev@davenquinn.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

