# Comparing `tmp/questdb-connect-0.0.48.tar.gz` & `tmp/questdb-connect-0.0.49.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "questdb-connect-0.0.48.tar", last modified: Tue May 16 10:33:14 2023, max compression
+gzip compressed data, was "questdb-connect-0.0.49.tar", last modified: Tue May 16 10:53:43 2023, max compression
```

## Comparing `questdb-connect-0.0.48.tar` & `questdb-connect-0.0.49.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-16 10:33:14.582641 questdb-connect-0.0.48/
--rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.48/LICENSE
--rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-16 10:33:14.582439 questdb-connect-0.0.48/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)     2734 2023-05-14 12:46:11.000000 questdb-connect-0.0.48/README.md
--rw-r--r--   0 marregui   (501) staff       (20)     2568 2023-05-16 10:32:07.000000 questdb-connect-0.0.48/pyproject.toml
--rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-16 10:33:14.582681 questdb-connect-0.0.48/setup.cfg
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-16 10:33:14.572759 questdb-connect-0.0.48/src/
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-16 10:33:14.575279 questdb-connect-0.0.48/src/examples/
--rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-0.0.48/src/examples/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-08 09:22:31.000000 questdb-connect-0.0.48/src/examples/hello_world.py
--rw-r--r--   0 marregui   (501) staff       (20)     2431 2023-05-10 11:39:52.000000 questdb-connect-0.0.48/src/examples/psycopg2_connect.py
--rw-r--r--   0 marregui   (501) staff       (20)     2831 2023-05-15 10:30:22.000000 questdb-connect-0.0.48/src/examples/server_utilisation.py
--rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-08 09:20:14.000000 questdb-connect-0.0.48/src/examples/sqlalchemy_orm.py
--rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-0.0.48/src/examples/sqlalchemy_raw.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-16 10:33:14.576917 questdb-connect-0.0.48/src/questdb_connect/
--rw-r--r--   0 marregui   (501) staff       (20)     4087 2023-05-16 10:32:56.000000 questdb-connect-0.0.48/src/questdb_connect/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)    12032 2023-05-16 10:30:46.000000 questdb-connect-0.0.48/src/questdb_connect/dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-0.0.48/src/questdb_connect/function_names.py
--rw-r--r--   0 marregui   (501) staff       (20)    12620 2023-05-16 10:30:46.000000 questdb-connect-0.0.48/src/questdb_connect/superset_engine.py
--rw-r--r--   0 marregui   (501) staff       (20)     5787 2023-05-03 12:21:25.000000 questdb-connect-0.0.48/src/questdb_connect/types.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-16 10:33:14.578626 questdb-connect-0.0.48/src/questdb_connect.egg-info/
--rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-16 10:33:14.000000 questdb-connect-0.0.48/src/questdb_connect.egg-info/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)      736 2023-05-16 10:33:14.000000 questdb-connect-0.0.48/src/questdb_connect.egg-info/SOURCES.txt
--rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-16 10:33:14.000000 questdb-connect-0.0.48/src/questdb_connect.egg-info/dependency_links.txt
--rw-r--r--   0 marregui   (501) staff       (20)      148 2023-05-16 10:33:14.000000 questdb-connect-0.0.48/src/questdb_connect.egg-info/entry_points.txt
--rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-16 10:33:14.000000 questdb-connect-0.0.48/src/questdb_connect.egg-info/requires.txt
--rw-r--r--   0 marregui   (501) staff       (20)       25 2023-05-16 10:33:14.000000 questdb-connect-0.0.48/src/questdb_connect.egg-info/top_level.txt
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-16 10:33:14.581230 questdb-connect-0.0.48/tests/
--rw-r--r--   0 marregui   (501) staff       (20)     9766 2023-05-16 09:28:52.000000 questdb-connect-0.0.48/tests/test_dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     1789 2023-05-16 10:30:40.000000 questdb-connect-0.0.48/tests/test_sql_compiler.py
--rw-r--r--   0 marregui   (501) staff       (20)     6270 2023-05-15 18:36:10.000000 questdb-connect-0.0.48/tests/test_superset.py
--rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.48/tests/test_types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-16 10:53:43.466451 questdb-connect-0.0.49/
+-rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.49/LICENSE
+-rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-16 10:53:43.466321 questdb-connect-0.0.49/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)     2734 2023-05-14 12:46:11.000000 questdb-connect-0.0.49/README.md
+-rw-r--r--   0 marregui   (501) staff       (20)     2568 2023-05-16 10:53:24.000000 questdb-connect-0.0.49/pyproject.toml
+-rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-16 10:53:43.466485 questdb-connect-0.0.49/setup.cfg
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-16 10:53:43.460156 questdb-connect-0.0.49/src/
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-16 10:53:43.462492 questdb-connect-0.0.49/src/examples/
+-rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-0.0.49/src/examples/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-08 09:22:31.000000 questdb-connect-0.0.49/src/examples/hello_world.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2431 2023-05-10 11:39:52.000000 questdb-connect-0.0.49/src/examples/psycopg2_connect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2831 2023-05-15 10:30:22.000000 questdb-connect-0.0.49/src/examples/server_utilisation.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-08 09:20:14.000000 questdb-connect-0.0.49/src/examples/sqlalchemy_orm.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-0.0.49/src/examples/sqlalchemy_raw.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-16 10:53:43.463936 questdb-connect-0.0.49/src/questdb_connect/
+-rw-r--r--   0 marregui   (501) staff       (20)     4087 2023-05-16 10:32:56.000000 questdb-connect-0.0.49/src/questdb_connect/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)    11622 2023-05-16 10:52:42.000000 questdb-connect-0.0.49/src/questdb_connect/dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-0.0.49/src/questdb_connect/function_names.py
+-rw-r--r--   0 marregui   (501) staff       (20)    12569 2023-05-16 10:51:31.000000 questdb-connect-0.0.49/src/questdb_connect/superset_engine.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5787 2023-05-03 12:21:25.000000 questdb-connect-0.0.49/src/questdb_connect/types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-16 10:53:43.464954 questdb-connect-0.0.49/src/questdb_connect.egg-info/
+-rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-16 10:53:43.000000 questdb-connect-0.0.49/src/questdb_connect.egg-info/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)      736 2023-05-16 10:53:43.000000 questdb-connect-0.0.49/src/questdb_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-16 10:53:43.000000 questdb-connect-0.0.49/src/questdb_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      148 2023-05-16 10:53:43.000000 questdb-connect-0.0.49/src/questdb_connect.egg-info/entry_points.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-16 10:53:43.000000 questdb-connect-0.0.49/src/questdb_connect.egg-info/requires.txt
+-rw-r--r--   0 marregui   (501) staff       (20)       25 2023-05-16 10:53:43.000000 questdb-connect-0.0.49/src/questdb_connect.egg-info/top_level.txt
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-16 10:53:43.465952 questdb-connect-0.0.49/tests/
+-rw-r--r--   0 marregui   (501) staff       (20)     9766 2023-05-16 09:28:52.000000 questdb-connect-0.0.49/tests/test_dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     1789 2023-05-16 10:30:40.000000 questdb-connect-0.0.49/tests/test_sql_compiler.py
+-rw-r--r--   0 marregui   (501) staff       (20)     8817 2023-05-16 10:51:23.000000 questdb-connect-0.0.49/tests/test_superset.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.49/tests/test_types.py
```

### Comparing `questdb-connect-0.0.48/LICENSE` & `questdb-connect-0.0.49/LICENSE`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.48/PKG-INFO` & `questdb-connect-0.0.49/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.48
+Version: 0.0.49
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.48/README.md` & `questdb-connect-0.0.49/README.md`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.48/pyproject.toml` & `questdb-connect-0.0.49/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 # https://pip.pypa.io/en/stable/reference/build-system/pyproject-toml/
 [project]
 name = 'questdb-connect'
-version = '0.0.48'
+version = '0.0.49'
 authors = [{ name = 'questdb.io', email = 'miguel@questdb.io' }]
 description = "SqlAlchemy/Superset libraries."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
```

### Comparing `questdb-connect-0.0.48/src/examples/__init__.py` & `questdb-connect-0.0.49/src/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.48/src/examples/hello_world.py` & `questdb-connect-0.0.49/src/examples/hello_world.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.48/src/examples/psycopg2_connect.py` & `questdb-connect-0.0.49/src/examples/psycopg2_connect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.48/src/examples/server_utilisation.py` & `questdb-connect-0.0.49/src/examples/server_utilisation.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.48/src/examples/sqlalchemy_orm.py` & `questdb-connect-0.0.49/src/examples/sqlalchemy_orm.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.48/src/examples/sqlalchemy_raw.py` & `questdb-connect-0.0.49/src/examples/sqlalchemy_raw.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.48/src/questdb_connect/__init__.py` & `questdb-connect-0.0.49/src/questdb_connect/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.48/src/questdb_connect/dialect.py` & `questdb-connect-0.0.49/src/questdb_connect/dialect.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,26 +25,25 @@
 import sqlalchemy
 from sqlalchemy import Column, MetaData, text
 from sqlalchemy.dialects.postgresql.psycopg2 import PGDialect_psycopg2
 from sqlalchemy.engine.reflection import Inspector
 from sqlalchemy.orm.exc import NoResultFound
 from sqlalchemy.sql.base import SchemaEventTarget
 from sqlalchemy.sql.compiler import (
-    OPERATORS,
     DDLCompiler,
     GenericTypeCompiler,
     IdentifierPreparer,
     SQLCompiler,
-    operators,
 )
 from sqlalchemy.sql.visitors import Traversible
 
 from . import remove_public_schema, ts_in_group_by_removing_parse_sql
 from .types import *
 
+
 # ===== SQLAlchemy Dialect ======
 # https://docs.sqlalchemy.org/en/14/ apache-superset requires SQLAlchemy 1.4
 
 
 def connection_uri(host: str, port: int, username: str, password: str, database: str = 'main'):
     return f'questdb://{username}:{password}@{host}:{port}/{database}'
 
@@ -179,26 +178,14 @@
 
     def visit_textclause(self, textclause, add_to_result_map=None, **kw):
         no_public_schema_sql = remove_public_schema(textclause.text)
         final_sql = ts_in_group_by_removing_parse_sql(no_public_schema_sql)
         textclause.text = final_sql[0] if final_sql else no_public_schema_sql
         return super().visit_textclause(textclause, add_to_result_map, **kw)
 
-    def group_by_clause(self, select, **kw):
-        """allow dialects to customize how GROUP BY is rendered."""
-        group_by = self._generate_delimited_list(
-            select._group_by_clauses,
-            OPERATORS[operators.comma_op],
-            **kw
-        )
-        if group_by:
-            return " FUCK OFF GROUP BY " + group_by
-        else:
-            return ""
-
 
 class QDBInspector(Inspector, abc.ABC):
     def reflecttable(
             self,
             table,
             include_columns,
             exclude_columns=(),
```

### Comparing `questdb-connect-0.0.48/src/questdb_connect/function_names.py` & `questdb-connect-0.0.49/src/questdb_connect/function_names.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.48/src/questdb_connect/superset_engine.py` & `questdb-connect-0.0.49/src/questdb_connect/superset_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 import re
 from datetime import datetime
 from typing import Any, Dict, List, Optional, Tuple
 
-from flask_babel import lazy_gettext
 from sqlalchemy.sql import text
 from sqlalchemy.types import TypeEngine
 from superset.db_engine_specs.base import (
     BaseEngineSpec,
     BasicParametersMixin,
     BasicParametersType,
     TimeGrain,
@@ -79,15 +78,15 @@
         'P1Y': "date_trunc('year', {col})",
         'P3M': "date_trunc('quarter', {col})",
     }
     ret_list = []
     for duration, func in _time_grain_expressions.items():
         if duration in builtin_time_grains:
             name = builtin_time_grains[duration]
-            ret_list.append(TimeGrain(name, lazy_gettext(name), func, duration))
+            ret_list.append(TimeGrain(name, name, func, duration))
     _engine_time_grains = tuple(ret_list)
     _default_column_type_mappings = (
         (re.compile("^LONG256", re.IGNORECASE), types.Long256, GenericDataType.STRING),
         (re.compile("^BOOLEAN", re.IGNORECASE), types.Boolean, GenericDataType.BOOLEAN),
         (re.compile("^BYTE", re.IGNORECASE), types.Byte, GenericDataType.BOOLEAN),
         (re.compile("^SHORT", re.IGNORECASE), types.Short, GenericDataType.NUMERIC),
         (re.compile("^INT", re.IGNORECASE), types.Int, GenericDataType.NUMERIC),
```

### Comparing `questdb-connect-0.0.48/src/questdb_connect/types.py` & `questdb-connect-0.0.49/src/questdb_connect/types.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.48/src/questdb_connect.egg-info/PKG-INFO` & `questdb-connect-0.0.49/src/questdb_connect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.48
+Version: 0.0.49
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.48/src/questdb_connect.egg-info/SOURCES.txt` & `questdb-connect-0.0.49/src/questdb_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.48/tests/test_dialect.py` & `questdb-connect-0.0.49/tests/test_dialect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.48/tests/test_sql_compiler.py` & `questdb-connect-0.0.49/tests/test_sql_compiler.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.48/tests/test_types.py` & `questdb-connect-0.0.49/tests/test_types.py`

 * *Files identical despite different names*

