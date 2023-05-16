# Comparing `tmp/questdb-connect-0.0.50.tar.gz` & `tmp/questdb-connect-0.0.52.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "questdb-connect-0.0.50.tar", last modified: Tue May 16 10:58:16 2023, max compression
+gzip compressed data, was "questdb-connect-0.0.52.tar", last modified: Tue May 16 13:47:46 2023, max compression
```

## Comparing `questdb-connect-0.0.50.tar` & `questdb-connect-0.0.52.tar`

### file list

```diff
@@ -1,32 +1,31 @@
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-16 10:58:16.933048 questdb-connect-0.0.50/
--rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.50/LICENSE
--rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-16 10:58:16.932884 questdb-connect-0.0.50/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)     2734 2023-05-14 12:46:11.000000 questdb-connect-0.0.50/README.md
--rw-r--r--   0 marregui   (501) staff       (20)     2568 2023-05-16 10:58:07.000000 questdb-connect-0.0.50/pyproject.toml
--rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-16 10:58:16.933087 questdb-connect-0.0.50/setup.cfg
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-16 10:58:16.923455 questdb-connect-0.0.50/src/
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-16 10:58:16.926241 questdb-connect-0.0.50/src/examples/
--rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-0.0.50/src/examples/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-08 09:22:31.000000 questdb-connect-0.0.50/src/examples/hello_world.py
--rw-r--r--   0 marregui   (501) staff       (20)     2431 2023-05-10 11:39:52.000000 questdb-connect-0.0.50/src/examples/psycopg2_connect.py
--rw-r--r--   0 marregui   (501) staff       (20)     2831 2023-05-15 10:30:22.000000 questdb-connect-0.0.50/src/examples/server_utilisation.py
--rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-08 09:20:14.000000 questdb-connect-0.0.50/src/examples/sqlalchemy_orm.py
--rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-0.0.50/src/examples/sqlalchemy_raw.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-16 10:58:16.929620 questdb-connect-0.0.50/src/questdb_connect/
--rw-r--r--   0 marregui   (501) staff       (20)     4087 2023-05-16 10:32:56.000000 questdb-connect-0.0.50/src/questdb_connect/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)    11622 2023-05-16 10:52:42.000000 questdb-connect-0.0.50/src/questdb_connect/dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-0.0.50/src/questdb_connect/function_names.py
--rw-r--r--   0 marregui   (501) staff       (20)    12581 2023-05-16 10:58:07.000000 questdb-connect-0.0.50/src/questdb_connect/superset_engine.py
--rw-r--r--   0 marregui   (501) staff       (20)     5787 2023-05-03 12:21:25.000000 questdb-connect-0.0.50/src/questdb_connect/types.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-16 10:58:16.931251 questdb-connect-0.0.50/src/questdb_connect.egg-info/
--rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-16 10:58:16.000000 questdb-connect-0.0.50/src/questdb_connect.egg-info/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)      736 2023-05-16 10:58:16.000000 questdb-connect-0.0.50/src/questdb_connect.egg-info/SOURCES.txt
--rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-16 10:58:16.000000 questdb-connect-0.0.50/src/questdb_connect.egg-info/dependency_links.txt
--rw-r--r--   0 marregui   (501) staff       (20)      148 2023-05-16 10:58:16.000000 questdb-connect-0.0.50/src/questdb_connect.egg-info/entry_points.txt
--rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-16 10:58:16.000000 questdb-connect-0.0.50/src/questdb_connect.egg-info/requires.txt
--rw-r--r--   0 marregui   (501) staff       (20)       25 2023-05-16 10:58:16.000000 questdb-connect-0.0.50/src/questdb_connect.egg-info/top_level.txt
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-16 10:58:16.932432 questdb-connect-0.0.50/tests/
--rw-r--r--   0 marregui   (501) staff       (20)     9766 2023-05-16 09:28:52.000000 questdb-connect-0.0.50/tests/test_dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     1789 2023-05-16 10:30:40.000000 questdb-connect-0.0.50/tests/test_sql_compiler.py
--rw-r--r--   0 marregui   (501) staff       (20)     8817 2023-05-16 10:51:23.000000 questdb-connect-0.0.50/tests/test_superset.py
--rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.50/tests/test_types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-16 13:47:46.407265 questdb-connect-0.0.52/
+-rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.52/LICENSE
+-rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-16 13:47:46.407136 questdb-connect-0.0.52/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)     2734 2023-05-14 12:46:11.000000 questdb-connect-0.0.52/README.md
+-rw-r--r--   0 marregui   (501) staff       (20)     2568 2023-05-16 13:46:44.000000 questdb-connect-0.0.52/pyproject.toml
+-rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-16 13:47:46.407301 questdb-connect-0.0.52/setup.cfg
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-16 13:47:46.401744 questdb-connect-0.0.52/src/
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-16 13:47:46.403913 questdb-connect-0.0.52/src/examples/
+-rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-0.0.52/src/examples/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-08 09:22:31.000000 questdb-connect-0.0.52/src/examples/hello_world.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2431 2023-05-10 11:39:52.000000 questdb-connect-0.0.52/src/examples/psycopg2_connect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2831 2023-05-15 10:30:22.000000 questdb-connect-0.0.52/src/examples/server_utilisation.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-08 09:20:14.000000 questdb-connect-0.0.52/src/examples/sqlalchemy_orm.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-0.0.52/src/examples/sqlalchemy_raw.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-16 13:47:46.405258 questdb-connect-0.0.52/src/questdb_connect/
+-rw-r--r--   0 marregui   (501) staff       (20)     3898 2023-05-16 13:44:22.000000 questdb-connect-0.0.52/src/questdb_connect/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)    11427 2023-05-16 13:44:28.000000 questdb-connect-0.0.52/src/questdb_connect/dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-0.0.52/src/questdb_connect/function_names.py
+-rw-r--r--   0 marregui   (501) staff       (20)    12445 2023-05-16 13:44:28.000000 questdb-connect-0.0.52/src/questdb_connect/superset_engine.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5787 2023-05-03 12:21:25.000000 questdb-connect-0.0.52/src/questdb_connect/types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-16 13:47:46.406166 questdb-connect-0.0.52/src/questdb_connect.egg-info/
+-rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-16 13:47:46.000000 questdb-connect-0.0.52/src/questdb_connect.egg-info/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)      709 2023-05-16 13:47:46.000000 questdb-connect-0.0.52/src/questdb_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-16 13:47:46.000000 questdb-connect-0.0.52/src/questdb_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      148 2023-05-16 13:47:46.000000 questdb-connect-0.0.52/src/questdb_connect.egg-info/entry_points.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-16 13:47:46.000000 questdb-connect-0.0.52/src/questdb_connect.egg-info/requires.txt
+-rw-r--r--   0 marregui   (501) staff       (20)       25 2023-05-16 13:47:46.000000 questdb-connect-0.0.52/src/questdb_connect.egg-info/top_level.txt
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-16 13:47:46.406879 questdb-connect-0.0.52/tests/
+-rw-r--r--   0 marregui   (501) staff       (20)     9766 2023-05-16 09:28:52.000000 questdb-connect-0.0.52/tests/test_dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     6666 2023-05-16 13:44:22.000000 questdb-connect-0.0.52/tests/test_superset.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.52/tests/test_types.py
```

### Comparing `questdb-connect-0.0.50/LICENSE` & `questdb-connect-0.0.52/LICENSE`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.50/PKG-INFO` & `questdb-connect-0.0.52/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.50
+Version: 0.0.52
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.50/README.md` & `questdb-connect-0.0.52/README.md`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.50/pyproject.toml` & `questdb-connect-0.0.52/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 # https://pip.pypa.io/en/stable/reference/build-system/pyproject-toml/
 [project]
 name = 'questdb-connect'
-version = '0.0.50'
+version = '0.0.52'
 authors = [{ name = 'questdb.io', email = 'miguel@questdb.io' }]
 description = "SqlAlchemy/Superset libraries."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
```

### Comparing `questdb-connect-0.0.50/src/examples/__init__.py` & `questdb-connect-0.0.52/src/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.50/src/examples/hello_world.py` & `questdb-connect-0.0.52/src/examples/hello_world.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.50/src/examples/psycopg2_connect.py` & `questdb-connect-0.0.52/src/examples/psycopg2_connect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.50/src/examples/server_utilisation.py` & `questdb-connect-0.0.52/src/examples/server_utilisation.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.50/src/examples/sqlalchemy_orm.py` & `questdb-connect-0.0.52/src/examples/sqlalchemy_orm.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.50/src/examples/sqlalchemy_raw.py` & `questdb-connect-0.0.52/src/examples/sqlalchemy_raw.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.50/src/questdb_connect/__init__.py` & `questdb-connect-0.0.52/src/questdb_connect/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -80,18 +80,15 @@
 
 class Error(Exception):
     pass
 
 
 class Cursor(psycopg2.extensions.cursor):
     def execute(self, query, vars=None):
-        no_public_schema_sql = remove_public_schema(query)
-        final_sql = ts_in_group_by_removing_parse_sql(no_public_schema_sql)
-        final_sql = final_sql[0] if final_sql else no_public_schema_sql
-        return super().execute(final_sql, vars)
+        return super().execute(remove_public_schema(query), vars)
 
 
 def cursor_factory(*args, **kwargs):
     return Cursor(*args, **kwargs)
 
 
 def connect(**kwargs):
```

### Comparing `questdb-connect-0.0.50/src/questdb_connect/dialect.py` & `questdb-connect-0.0.52/src/questdb_connect/dialect.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,18 +32,17 @@
     DDLCompiler,
     GenericTypeCompiler,
     IdentifierPreparer,
     SQLCompiler,
 )
 from sqlalchemy.sql.visitors import Traversible
 
-from . import remove_public_schema, ts_in_group_by_removing_parse_sql
+from . import remove_public_schema
 from .types import *
 
-
 # ===== SQLAlchemy Dialect ======
 # https://docs.sqlalchemy.org/en/14/ apache-superset requires SQLAlchemy 1.4
 
 
 def connection_uri(host: str, port: int, username: str, password: str, database: str = 'main'):
     return f'questdb://{username}:{password}@{host}:{port}/{database}'
 
@@ -173,17 +172,15 @@
 
 
 class QDBSQLCompiler(SQLCompiler, abc.ABC):
     def _is_safe_for_fast_insert_values_helper(self):
         return True
 
     def visit_textclause(self, textclause, add_to_result_map=None, **kw):
-        no_public_schema_sql = remove_public_schema(textclause.text)
-        final_sql = ts_in_group_by_removing_parse_sql(no_public_schema_sql)
-        textclause.text = final_sql[0] if final_sql else no_public_schema_sql
+        textclause.text = remove_public_schema(textclause.text)
         return super().visit_textclause(textclause, add_to_result_map, **kw)
 
 
 class QDBInspector(Inspector, abc.ABC):
     def reflecttable(
             self,
             table,
```

### Comparing `questdb-connect-0.0.50/src/questdb_connect/function_names.py` & `questdb-connect-0.0.52/src/questdb_connect/function_names.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.50/src/questdb_connect/superset_engine.py` & `questdb-connect-0.0.52/src/questdb_connect/superset_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,27 +20,28 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 import re
 from datetime import datetime
 from typing import Any, Dict, List, Optional, Tuple
 
+from flask_babel import lazy_gettext as _
 from sqlalchemy.sql import text
 from sqlalchemy.types import TypeEngine
 from superset.db_engine_specs.base import (
     BaseEngineSpec,
     BasicParametersMixin,
     BasicParametersType,
     TimeGrain,
     builtin_time_grains,
 )
 from superset.utils import core as utils
 from superset.utils.core import GenericDataType
 
-from . import remove_public_schema, ts_in_group_by_removing_parse_sql, types
+from . import remove_public_schema, types
 from .dialect import connection_uri
 from .function_names import FUNCTION_NAMES
 
 # https://superset.apache.org/docs/databases/installing-database-drivers
 # Apache Superset requires a Python DB-API database driver, and a SQLAlchemy dialect
 # https://preset.io/blog/building-database-connector/
 
@@ -78,15 +79,15 @@
         'P1Y': "date_trunc('year', {col})",
         'P3M': "date_trunc('quarter', {col})",
     }
     ret_list = []
     for duration, func in _time_grain_expressions.items():
         if duration in builtin_time_grains:
             name = builtin_time_grains[duration]
-            ret_list.append(TimeGrain(name, name, func, duration))
+            ret_list.append(TimeGrain(name, _(name), func, duration))
     _engine_time_grains = tuple(ret_list)
     _default_column_type_mappings = (
         (re.compile("^LONG256", re.IGNORECASE), types.Long256, GenericDataType.STRING),
         (re.compile("^BOOLEAN", re.IGNORECASE), types.Boolean, GenericDataType.BOOLEAN),
         (re.compile("^BYTE", re.IGNORECASE), types.Byte, GenericDataType.BOOLEAN),
         (re.compile("^SHORT", re.IGNORECASE), types.Short, GenericDataType.NUMERIC),
         (re.compile("^INT", re.IGNORECASE), types.Int, GenericDataType.NUMERIC),
@@ -167,20 +168,20 @@
         if type_u == 'DATE':
             return f"TO_DATE('{dttm.date().isoformat()}', 'YYYY-MM-DD')"
         if type_u in ('DATETIME', 'TIMESTAMP'):
             dttm_formatted = dttm.isoformat(sep=" ", timespec="microseconds")
             return f"TO_TIMESTAMP('{dttm_formatted}', 'yyyy-MM-ddTHH:mm:ss.SSSUUUZ')"
         return None
 
-    # @classmethod
-    # def get_time_grains(cls) -> Tuple[TimeGrain, ...]:
-    #     """Generate a tuple of supported time grains.
-    #     :return: All time grains supported by the engine
-    #     """
-    #     return cls._engine_time_grains
+    @classmethod
+    def get_time_grains(cls) -> Tuple[TimeGrain, ...]:
+        """Generate a tuple of supported time grains.
+        :return: All time grains supported by the engine
+        """
+        return cls._engine_time_grains
 
     @classmethod
     def get_datatype(cls, type_code: Any) -> Optional[str]:
         """Change column type code from cursor description to string representation.
         :param type_code: Type code from cursor description
         :return: String representation of type code
         """
@@ -285,11 +286,7 @@
     def get_function_names(cls, database) -> List[str]:
         """Get a list of function names that are able to be called on the database.
         Used for SQL Lab autocomplete.
         :param database: The database to get functions for
         :return: A list of function names usable in the database
         """
         return FUNCTION_NAMES
-
-    @classmethod
-    def parse_sql(cls, sql: str) -> List[str]:
-        return ts_in_group_by_removing_parse_sql(sql, '__timestamp')
```

### Comparing `questdb-connect-0.0.50/src/questdb_connect/types.py` & `questdb-connect-0.0.52/src/questdb_connect/types.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.50/src/questdb_connect.egg-info/PKG-INFO` & `questdb-connect-0.0.52/src/questdb_connect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.50
+Version: 0.0.52
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.50/src/questdb_connect.egg-info/SOURCES.txt` & `questdb-connect-0.0.52/src/questdb_connect.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -15,10 +15,9 @@
 src/questdb_connect.egg-info/PKG-INFO
 src/questdb_connect.egg-info/SOURCES.txt
 src/questdb_connect.egg-info/dependency_links.txt
 src/questdb_connect.egg-info/entry_points.txt
 src/questdb_connect.egg-info/requires.txt
 src/questdb_connect.egg-info/top_level.txt
 tests/test_dialect.py
-tests/test_sql_compiler.py
 tests/test_superset.py
 tests/test_types.py
```

### Comparing `questdb-connect-0.0.50/tests/test_dialect.py` & `questdb-connect-0.0.52/tests/test_dialect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.50/tests/test_types.py` & `questdb-connect-0.0.52/tests/test_types.py`

 * *Files identical despite different names*

