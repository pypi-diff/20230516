# Comparing `tmp/questdb-connect-0.0.47.tar.gz` & `tmp/questdb-connect-0.0.48.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "questdb-connect-0.0.47.tar", last modified: Mon May 15 19:51:04 2023, max compression
+gzip compressed data, was "questdb-connect-0.0.48.tar", last modified: Tue May 16 10:33:14 2023, max compression
```

## Comparing `questdb-connect-0.0.47.tar` & `questdb-connect-0.0.48.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-15 19:51:04.843435 questdb-connect-0.0.47/
--rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.47/LICENSE
--rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-15 19:51:04.843309 questdb-connect-0.0.47/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)     2734 2023-05-14 12:46:11.000000 questdb-connect-0.0.47/README.md
--rw-r--r--   0 marregui   (501) staff       (20)     2568 2023-05-15 19:47:06.000000 questdb-connect-0.0.47/pyproject.toml
--rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-15 19:51:04.843469 questdb-connect-0.0.47/setup.cfg
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-15 19:51:04.836915 questdb-connect-0.0.47/src/
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-15 19:51:04.839354 questdb-connect-0.0.47/src/examples/
--rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-0.0.47/src/examples/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-08 09:22:31.000000 questdb-connect-0.0.47/src/examples/hello_world.py
--rw-r--r--   0 marregui   (501) staff       (20)     2431 2023-05-10 11:39:52.000000 questdb-connect-0.0.47/src/examples/psycopg2_connect.py
--rw-r--r--   0 marregui   (501) staff       (20)     2831 2023-05-15 10:30:22.000000 questdb-connect-0.0.47/src/examples/server_utilisation.py
--rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-08 09:20:14.000000 questdb-connect-0.0.47/src/examples/sqlalchemy_orm.py
--rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-0.0.47/src/examples/sqlalchemy_raw.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-15 19:51:04.841010 questdb-connect-0.0.47/src/questdb_connect/
--rw-r--r--   0 marregui   (501) staff       (20)     1937 2023-05-14 09:35:51.000000 questdb-connect-0.0.47/src/questdb_connect/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)    13534 2023-05-15 19:46:46.000000 questdb-connect-0.0.47/src/questdb_connect/dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-0.0.47/src/questdb_connect/function_names.py
--rw-r--r--   0 marregui   (501) staff       (20)    11956 2023-05-15 19:46:46.000000 questdb-connect-0.0.47/src/questdb_connect/superset_engine.py
--rw-r--r--   0 marregui   (501) staff       (20)     5787 2023-05-03 12:21:25.000000 questdb-connect-0.0.47/src/questdb_connect/types.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-15 19:51:04.842124 questdb-connect-0.0.47/src/questdb_connect.egg-info/
--rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-15 19:51:04.000000 questdb-connect-0.0.47/src/questdb_connect.egg-info/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)      709 2023-05-15 19:51:04.000000 questdb-connect-0.0.47/src/questdb_connect.egg-info/SOURCES.txt
--rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-15 19:51:04.000000 questdb-connect-0.0.47/src/questdb_connect.egg-info/dependency_links.txt
--rw-r--r--   0 marregui   (501) staff       (20)      148 2023-05-15 19:51:04.000000 questdb-connect-0.0.47/src/questdb_connect.egg-info/entry_points.txt
--rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-15 19:51:04.000000 questdb-connect-0.0.47/src/questdb_connect.egg-info/requires.txt
--rw-r--r--   0 marregui   (501) staff       (20)       25 2023-05-15 19:51:04.000000 questdb-connect-0.0.47/src/questdb_connect.egg-info/top_level.txt
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-15 19:51:04.842921 questdb-connect-0.0.47/tests/
--rw-r--r--   0 marregui   (501) staff       (20)     9751 2023-05-15 13:49:03.000000 questdb-connect-0.0.47/tests/test_dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     6270 2023-05-15 18:36:10.000000 questdb-connect-0.0.47/tests/test_superset.py
--rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.47/tests/test_types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-16 10:33:14.582641 questdb-connect-0.0.48/
+-rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.48/LICENSE
+-rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-16 10:33:14.582439 questdb-connect-0.0.48/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)     2734 2023-05-14 12:46:11.000000 questdb-connect-0.0.48/README.md
+-rw-r--r--   0 marregui   (501) staff       (20)     2568 2023-05-16 10:32:07.000000 questdb-connect-0.0.48/pyproject.toml
+-rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-16 10:33:14.582681 questdb-connect-0.0.48/setup.cfg
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-16 10:33:14.572759 questdb-connect-0.0.48/src/
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-16 10:33:14.575279 questdb-connect-0.0.48/src/examples/
+-rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-0.0.48/src/examples/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-08 09:22:31.000000 questdb-connect-0.0.48/src/examples/hello_world.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2431 2023-05-10 11:39:52.000000 questdb-connect-0.0.48/src/examples/psycopg2_connect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2831 2023-05-15 10:30:22.000000 questdb-connect-0.0.48/src/examples/server_utilisation.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-08 09:20:14.000000 questdb-connect-0.0.48/src/examples/sqlalchemy_orm.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-0.0.48/src/examples/sqlalchemy_raw.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-16 10:33:14.576917 questdb-connect-0.0.48/src/questdb_connect/
+-rw-r--r--   0 marregui   (501) staff       (20)     4087 2023-05-16 10:32:56.000000 questdb-connect-0.0.48/src/questdb_connect/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)    12032 2023-05-16 10:30:46.000000 questdb-connect-0.0.48/src/questdb_connect/dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-0.0.48/src/questdb_connect/function_names.py
+-rw-r--r--   0 marregui   (501) staff       (20)    12620 2023-05-16 10:30:46.000000 questdb-connect-0.0.48/src/questdb_connect/superset_engine.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5787 2023-05-03 12:21:25.000000 questdb-connect-0.0.48/src/questdb_connect/types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-16 10:33:14.578626 questdb-connect-0.0.48/src/questdb_connect.egg-info/
+-rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-16 10:33:14.000000 questdb-connect-0.0.48/src/questdb_connect.egg-info/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)      736 2023-05-16 10:33:14.000000 questdb-connect-0.0.48/src/questdb_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-16 10:33:14.000000 questdb-connect-0.0.48/src/questdb_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      148 2023-05-16 10:33:14.000000 questdb-connect-0.0.48/src/questdb_connect.egg-info/entry_points.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-16 10:33:14.000000 questdb-connect-0.0.48/src/questdb_connect.egg-info/requires.txt
+-rw-r--r--   0 marregui   (501) staff       (20)       25 2023-05-16 10:33:14.000000 questdb-connect-0.0.48/src/questdb_connect.egg-info/top_level.txt
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-16 10:33:14.581230 questdb-connect-0.0.48/tests/
+-rw-r--r--   0 marregui   (501) staff       (20)     9766 2023-05-16 09:28:52.000000 questdb-connect-0.0.48/tests/test_dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     1789 2023-05-16 10:30:40.000000 questdb-connect-0.0.48/tests/test_sql_compiler.py
+-rw-r--r--   0 marregui   (501) staff       (20)     6270 2023-05-15 18:36:10.000000 questdb-connect-0.0.48/tests/test_superset.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.48/tests/test_types.py
```

### Comparing `questdb-connect-0.0.47/LICENSE` & `questdb-connect-0.0.48/LICENSE`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.47/PKG-INFO` & `questdb-connect-0.0.48/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.47
+Version: 0.0.48
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.47/README.md` & `questdb-connect-0.0.48/README.md`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.47/pyproject.toml` & `questdb-connect-0.0.48/pyproject.toml`

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
-version = '0.0.47'
+version = '0.0.48'
 authors = [{ name = 'questdb.io', email = 'miguel@questdb.io' }]
 description = "SqlAlchemy/Superset libraries."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
```

### Comparing `questdb-connect-0.0.47/src/examples/__init__.py` & `questdb-connect-0.0.48/src/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.47/src/examples/hello_world.py` & `questdb-connect-0.0.48/src/examples/hello_world.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.47/src/examples/psycopg2_connect.py` & `questdb-connect-0.0.48/src/examples/psycopg2_connect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.47/src/examples/server_utilisation.py` & `questdb-connect-0.0.48/src/examples/server_utilisation.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.47/src/examples/sqlalchemy_orm.py` & `questdb-connect-0.0.48/src/examples/sqlalchemy_orm.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.47/src/examples/sqlalchemy_raw.py` & `questdb-connect-0.0.48/src/examples/sqlalchemy_raw.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.47/src/questdb_connect/dialect.py` & `questdb-connect-0.0.48/src/questdb_connect/dialect.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,33 +17,32 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 import abc
-from typing import List
 
 import sqlalchemy
-import sqlparse
 from sqlalchemy import Column, MetaData, text
 from sqlalchemy.dialects.postgresql.psycopg2 import PGDialect_psycopg2
 from sqlalchemy.engine.reflection import Inspector
 from sqlalchemy.orm.exc import NoResultFound
 from sqlalchemy.sql.base import SchemaEventTarget
 from sqlalchemy.sql.compiler import (
+    OPERATORS,
     DDLCompiler,
     GenericTypeCompiler,
     IdentifierPreparer,
     SQLCompiler,
+    operators,
 )
 from sqlalchemy.sql.visitors import Traversible
-from sqlparse import tokens as T
 
-from . import remove_public_schema
+from . import remove_public_schema, ts_in_group_by_removing_parse_sql
 from .types import *
 
 # ===== SQLAlchemy Dialect ======
 # https://docs.sqlalchemy.org/en/14/ apache-superset requires SQLAlchemy 1.4
 
 
 def connection_uri(host: str, port: int, username: str, password: str, database: str = 'main'):
@@ -116,52 +115,14 @@
 def _has_special_char(_value):
     for candidate in _value:
         if candidate in _special_chars:
             return True
     return False
 
 
-def parse_sql(sql: str, timestamp_alias: str = '__timestamp') -> List[str]:
-    parsed_sql_text = []
-    for parsed_sql in sqlparse.parse(sql):
-        if parsed_sql.get_type().lower() == 'select':
-            # remove timestamp column from any group by
-            ts_col_name = None
-            has_group_by = False
-            for tok in parsed_sql.tokens:
-                if not ts_col_name and isinstance(tok, sqlparse.sql.IdentifierList):
-                    for select_tok in tok.tokens:
-                        if timestamp_alias in select_tok.value:
-                            ts_col_name = select_tok.normalized
-                            break
-                elif ts_col_name and tok.value.lower() == 'group by':
-                    has_group_by = True
-                elif ts_col_name and has_group_by and isinstance(tok, sqlparse.sql.IdentifierList):
-                    remove_idx = None
-                    comma_idxs = []
-                    for idx, group_tok in enumerate(tok.tokens):
-                        if group_tok.match(T.Punctuation, ','):
-                            comma_idxs.append(idx)
-                        elif group_tok.normalized == ts_col_name:
-                            remove_idx = idx
-                    if remove_idx is not None:
-                        tok.tokens.pop(remove_idx)
-                        if remove_idx == 0:
-                            tok.tokens.pop(comma_idxs[0] - 1)
-                        else:
-                            remove_comma_idx = -1
-                            for i, c_i in enumerate(comma_idxs):
-                                if c_i > remove_idx:
-                                    remove_comma_idx = i - 1
-                                    break
-                            tok.tokens.pop(comma_idxs[remove_comma_idx])
-        parsed_sql_text.append(str(parsed_sql).strip(' ;'))
-    return parsed_sql_text
-
-
 class QDBIdentifierPreparer(IdentifierPreparer, abc.ABC):
     schema_for_object = staticmethod(_none)
 
     def __init__(
             self,
             dialect,
             initial_quote='"',
@@ -214,18 +175,30 @@
 
 class QDBSQLCompiler(SQLCompiler, abc.ABC):
     def _is_safe_for_fast_insert_values_helper(self):
         return True
 
     def visit_textclause(self, textclause, add_to_result_map=None, **kw):
         no_public_schema_sql = remove_public_schema(textclause.text)
-        final_sql = parse_sql(no_public_schema_sql)
+        final_sql = ts_in_group_by_removing_parse_sql(no_public_schema_sql)
         textclause.text = final_sql[0] if final_sql else no_public_schema_sql
         return super().visit_textclause(textclause, add_to_result_map, **kw)
 
+    def group_by_clause(self, select, **kw):
+        """allow dialects to customize how GROUP BY is rendered."""
+        group_by = self._generate_delimited_list(
+            select._group_by_clauses,
+            OPERATORS[operators.comma_op],
+            **kw
+        )
+        if group_by:
+            return " FUCK OFF GROUP BY " + group_by
+        else:
+            return ""
+
 
 class QDBInspector(Inspector, abc.ABC):
     def reflecttable(
             self,
             table,
             include_columns,
             exclude_columns=(),
```

### Comparing `questdb-connect-0.0.47/src/questdb_connect/function_names.py` & `questdb-connect-0.0.48/src/questdb_connect/function_names.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.47/src/questdb_connect/superset_engine.py` & `questdb-connect-0.0.48/src/questdb_connect/superset_engine.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,23 +20,29 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 import re
 from datetime import datetime
 from typing import Any, Dict, List, Optional, Tuple
 
+from flask_babel import lazy_gettext
 from sqlalchemy.sql import text
 from sqlalchemy.types import TypeEngine
-from superset.db_engine_specs.base import BaseEngineSpec, BasicParametersMixin, BasicParametersType
+from superset.db_engine_specs.base import (
+    BaseEngineSpec,
+    BasicParametersMixin,
+    BasicParametersType,
+    TimeGrain,
+    builtin_time_grains,
+)
 from superset.utils import core as utils
 from superset.utils.core import GenericDataType
 
-import questdb_connect.dialect as qdbcd
-
-from . import remove_public_schema, types
+from . import remove_public_schema, ts_in_group_by_removing_parse_sql, types
+from .dialect import connection_uri
 from .function_names import FUNCTION_NAMES
 
 # https://superset.apache.org/docs/databases/installing-database-drivers
 # Apache Superset requires a Python DB-API database driver, and a SQLAlchemy dialect
 # https://preset.io/blog/building-database-connector/
 
 
@@ -69,14 +75,20 @@
         'PT6H': "date_trunc('hour', {col})",
         'PT1D': "date_trunc('day', {col})",
         'P1W': "date_trunc('week', {col})",
         'P1M': "date_trunc('month', {col})",
         'P1Y': "date_trunc('year', {col})",
         'P3M': "date_trunc('quarter', {col})",
     }
+    ret_list = []
+    for duration, func in _time_grain_expressions.items():
+        if duration in builtin_time_grains:
+            name = builtin_time_grains[duration]
+            ret_list.append(TimeGrain(name, lazy_gettext(name), func, duration))
+    _engine_time_grains = tuple(ret_list)
     _default_column_type_mappings = (
         (re.compile("^LONG256", re.IGNORECASE), types.Long256, GenericDataType.STRING),
         (re.compile("^BOOLEAN", re.IGNORECASE), types.Boolean, GenericDataType.BOOLEAN),
         (re.compile("^BYTE", re.IGNORECASE), types.Byte, GenericDataType.BOOLEAN),
         (re.compile("^SHORT", re.IGNORECASE), types.Short, GenericDataType.NUMERIC),
         (re.compile("^INT", re.IGNORECASE), types.Int, GenericDataType.NUMERIC),
         (re.compile("^LONG", re.IGNORECASE), types.Long, GenericDataType.NUMERIC),
@@ -94,15 +106,15 @@
 
     @classmethod
     def build_sqlalchemy_uri(
             cls,
             parameters: BasicParametersType,
             encrypted_extra: Optional[Dict[str, str]] = None
     ) -> str:
-        return qdbcd.connection_uri(
+        return connection_uri(
             parameters.get("host"),
             int(parameters.get("port")),
             parameters.get("username"),
             parameters.get("password"),
             parameters.get("database"))
 
     @classmethod
@@ -157,14 +169,21 @@
             return f"TO_DATE('{dttm.date().isoformat()}', 'YYYY-MM-DD')"
         if type_u in ('DATETIME', 'TIMESTAMP'):
             dttm_formatted = dttm.isoformat(sep=" ", timespec="microseconds")
             return f"TO_TIMESTAMP('{dttm_formatted}', 'yyyy-MM-ddTHH:mm:ss.SSSUUUZ')"
         return None
 
     @classmethod
+    def get_time_grains(cls) -> Tuple[TimeGrain, ...]:
+        """Generate a tuple of supported time grains.
+        :return: All time grains supported by the engine
+        """
+        return cls._engine_time_grains
+
+    @classmethod
     def get_datatype(cls, type_code: Any) -> Optional[str]:
         """Change column type code from cursor description to string representation.
         :param type_code: Type code from cursor description
         :return: String representation of type code
         """
         return type_code.upper() if type_code and isinstance(type_code, str) else 'UNKNOWN'
 
@@ -270,8 +289,8 @@
         :param database: The database to get functions for
         :return: A list of function names usable in the database
         """
         return FUNCTION_NAMES
 
     @classmethod
     def parse_sql(cls, sql: str) -> List[str]:
-        return qdbcd.parse_sql(sql, '__timestamp')
+        return ts_in_group_by_removing_parse_sql(sql, '__timestamp')
```

### Comparing `questdb-connect-0.0.47/src/questdb_connect/types.py` & `questdb-connect-0.0.48/src/questdb_connect/types.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.47/src/questdb_connect.egg-info/PKG-INFO` & `questdb-connect-0.0.48/src/questdb_connect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.47
+Version: 0.0.48
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.47/src/questdb_connect.egg-info/SOURCES.txt` & `questdb-connect-0.0.48/src/questdb_connect.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -15,9 +15,10 @@
 src/questdb_connect.egg-info/PKG-INFO
 src/questdb_connect.egg-info/SOURCES.txt
 src/questdb_connect.egg-info/dependency_links.txt
 src/questdb_connect.egg-info/entry_points.txt
 src/questdb_connect.egg-info/requires.txt
 src/questdb_connect.egg-info/top_level.txt
 tests/test_dialect.py
+tests/test_sql_compiler.py
 tests/test_superset.py
 tests/test_types.py
```

### Comparing `questdb-connect-0.0.47/tests/test_dialect.py` & `questdb-connect-0.0.48/tests/test_dialect.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,20 +22,20 @@
 #
 import datetime
 
 import sqlalchemy as sqla
 from questdb_connect import types
 from sqlalchemy.orm import Session
 
-from tests.conftest import TEST_TABLE_NAME, collect_select_all, collect_select_all_raw_connection
+from tests.conftest import ALL_TYPES_TABLE_NAME, collect_select_all, collect_select_all_raw_connection
 
 
 def test_insert(test_engine, test_model):
     with test_engine.connect() as conn:
-        assert test_engine.dialect.has_table(conn, TEST_TABLE_NAME)
+        assert test_engine.dialect.has_table(conn, ALL_TYPES_TABLE_NAME)
         assert not test_engine.dialect.has_table(conn, 'scorchio')
         now = datetime.datetime(2023, 4, 12, 23, 55, 59, 342380)
         now_date = now.date()
         expected = ("(True, 8, 12, 13, 14, 15.234, 16.88993244, 'coconut', 'banana', 'C', "
                     "UUID('6d5eb038-63d1-4971-8484-30c16e13de5b'), datetime.datetime(2023, 4, 12, "
                     "0, 0), datetime.datetime(2023, 4, 12, 23, 55, 59, 342380), 'dfvgsj', "
                     "'0xa3b400fcf6ed707d710d5d4e672305203ed3cc6254d1cefe313e4a465861f42a')\n"
@@ -105,15 +105,15 @@
             col_long256='0xa3b400fcf6ed707d710d5d4e672305203ed3cc6254d1cefe313e4a465861f42a'
         ))
         session.commit()
     finally:
         if session:
             session.close()
     metadata = sqla.MetaData()
-    table = sqla.Table(TEST_TABLE_NAME, metadata, autoload_with=test_engine)
+    table = sqla.Table(ALL_TYPES_TABLE_NAME, metadata, autoload_with=test_engine)
     table_columns = str([(col.name, col.type, col.primary_key) for col in table.columns])
     assert table_columns == str([
         ('col_boolean', types.Boolean(), False),
         ('col_byte', types.Byte(), False),
         ('col_short', types.Short(), False),
         ('col_int', types.Int(), False),
         ('col_long', types.Long(), False),
```

### Comparing `questdb-connect-0.0.47/tests/test_superset.py` & `questdb-connect-0.0.48/tests/test_superset.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.47/tests/test_types.py` & `questdb-connect-0.0.48/tests/test_types.py`

 * *Files identical despite different names*

