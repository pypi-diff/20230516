# Comparing `tmp/questdb-connect-0.0.46.tar.gz` & `tmp/questdb-connect-0.0.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "questdb-connect-0.0.46.tar", last modified: Mon May 15 18:38:15 2023, max compression
+gzip compressed data, was "questdb-connect-0.0.47.tar", last modified: Mon May 15 19:51:04 2023, max compression
```

## Comparing `questdb-connect-0.0.46.tar` & `questdb-connect-0.0.47.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-15 18:38:15.663355 questdb-connect-0.0.46/
--rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.46/LICENSE
--rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-15 18:38:15.663216 questdb-connect-0.0.46/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)     2734 2023-05-14 12:46:11.000000 questdb-connect-0.0.46/README.md
--rw-r--r--   0 marregui   (501) staff       (20)     2568 2023-05-15 18:37:08.000000 questdb-connect-0.0.46/pyproject.toml
--rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-15 18:38:15.663389 questdb-connect-0.0.46/setup.cfg
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-15 18:38:15.656682 questdb-connect-0.0.46/src/
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-15 18:38:15.659161 questdb-connect-0.0.46/src/examples/
--rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-0.0.46/src/examples/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-08 09:22:31.000000 questdb-connect-0.0.46/src/examples/hello_world.py
--rw-r--r--   0 marregui   (501) staff       (20)     2431 2023-05-10 11:39:52.000000 questdb-connect-0.0.46/src/examples/psycopg2_connect.py
--rw-r--r--   0 marregui   (501) staff       (20)     2831 2023-05-15 10:30:22.000000 questdb-connect-0.0.46/src/examples/server_utilisation.py
--rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-08 09:20:14.000000 questdb-connect-0.0.46/src/examples/sqlalchemy_orm.py
--rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-0.0.46/src/examples/sqlalchemy_raw.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-15 18:38:15.660814 questdb-connect-0.0.46/src/questdb_connect/
--rw-r--r--   0 marregui   (501) staff       (20)     1937 2023-05-14 09:35:51.000000 questdb-connect-0.0.46/src/questdb_connect/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)    11427 2023-05-15 10:26:37.000000 questdb-connect-0.0.46/src/questdb_connect/dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-0.0.46/src/questdb_connect/function_names.py
--rw-r--r--   0 marregui   (501) staff       (20)    13956 2023-05-15 18:37:08.000000 questdb-connect-0.0.46/src/questdb_connect/superset_engine.py
--rw-r--r--   0 marregui   (501) staff       (20)     5787 2023-05-03 12:21:25.000000 questdb-connect-0.0.46/src/questdb_connect/types.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-15 18:38:15.661951 questdb-connect-0.0.46/src/questdb_connect.egg-info/
--rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-15 18:38:15.000000 questdb-connect-0.0.46/src/questdb_connect.egg-info/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)      709 2023-05-15 18:38:15.000000 questdb-connect-0.0.46/src/questdb_connect.egg-info/SOURCES.txt
--rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-15 18:38:15.000000 questdb-connect-0.0.46/src/questdb_connect.egg-info/dependency_links.txt
--rw-r--r--   0 marregui   (501) staff       (20)      148 2023-05-15 18:38:15.000000 questdb-connect-0.0.46/src/questdb_connect.egg-info/entry_points.txt
--rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-15 18:38:15.000000 questdb-connect-0.0.46/src/questdb_connect.egg-info/requires.txt
--rw-r--r--   0 marregui   (501) staff       (20)       25 2023-05-15 18:38:15.000000 questdb-connect-0.0.46/src/questdb_connect.egg-info/top_level.txt
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-15 18:38:15.662824 questdb-connect-0.0.46/tests/
--rw-r--r--   0 marregui   (501) staff       (20)     9751 2023-05-15 13:49:03.000000 questdb-connect-0.0.46/tests/test_dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     6270 2023-05-15 18:36:10.000000 questdb-connect-0.0.46/tests/test_superset.py
--rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.46/tests/test_types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-15 19:51:04.843435 questdb-connect-0.0.47/
+-rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.47/LICENSE
+-rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-15 19:51:04.843309 questdb-connect-0.0.47/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)     2734 2023-05-14 12:46:11.000000 questdb-connect-0.0.47/README.md
+-rw-r--r--   0 marregui   (501) staff       (20)     2568 2023-05-15 19:47:06.000000 questdb-connect-0.0.47/pyproject.toml
+-rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-15 19:51:04.843469 questdb-connect-0.0.47/setup.cfg
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-15 19:51:04.836915 questdb-connect-0.0.47/src/
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-15 19:51:04.839354 questdb-connect-0.0.47/src/examples/
+-rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-0.0.47/src/examples/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-08 09:22:31.000000 questdb-connect-0.0.47/src/examples/hello_world.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2431 2023-05-10 11:39:52.000000 questdb-connect-0.0.47/src/examples/psycopg2_connect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2831 2023-05-15 10:30:22.000000 questdb-connect-0.0.47/src/examples/server_utilisation.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-08 09:20:14.000000 questdb-connect-0.0.47/src/examples/sqlalchemy_orm.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-0.0.47/src/examples/sqlalchemy_raw.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-15 19:51:04.841010 questdb-connect-0.0.47/src/questdb_connect/
+-rw-r--r--   0 marregui   (501) staff       (20)     1937 2023-05-14 09:35:51.000000 questdb-connect-0.0.47/src/questdb_connect/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)    13534 2023-05-15 19:46:46.000000 questdb-connect-0.0.47/src/questdb_connect/dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-0.0.47/src/questdb_connect/function_names.py
+-rw-r--r--   0 marregui   (501) staff       (20)    11956 2023-05-15 19:46:46.000000 questdb-connect-0.0.47/src/questdb_connect/superset_engine.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5787 2023-05-03 12:21:25.000000 questdb-connect-0.0.47/src/questdb_connect/types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-15 19:51:04.842124 questdb-connect-0.0.47/src/questdb_connect.egg-info/
+-rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-15 19:51:04.000000 questdb-connect-0.0.47/src/questdb_connect.egg-info/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)      709 2023-05-15 19:51:04.000000 questdb-connect-0.0.47/src/questdb_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-15 19:51:04.000000 questdb-connect-0.0.47/src/questdb_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      148 2023-05-15 19:51:04.000000 questdb-connect-0.0.47/src/questdb_connect.egg-info/entry_points.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-15 19:51:04.000000 questdb-connect-0.0.47/src/questdb_connect.egg-info/requires.txt
+-rw-r--r--   0 marregui   (501) staff       (20)       25 2023-05-15 19:51:04.000000 questdb-connect-0.0.47/src/questdb_connect.egg-info/top_level.txt
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-15 19:51:04.842921 questdb-connect-0.0.47/tests/
+-rw-r--r--   0 marregui   (501) staff       (20)     9751 2023-05-15 13:49:03.000000 questdb-connect-0.0.47/tests/test_dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     6270 2023-05-15 18:36:10.000000 questdb-connect-0.0.47/tests/test_superset.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.47/tests/test_types.py
```

### Comparing `questdb-connect-0.0.46/LICENSE` & `questdb-connect-0.0.47/LICENSE`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.46/PKG-INFO` & `questdb-connect-0.0.47/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.46
+Version: 0.0.47
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.46/README.md` & `questdb-connect-0.0.47/README.md`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.46/pyproject.toml` & `questdb-connect-0.0.47/pyproject.toml`

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
-version = '0.0.46'
+version = '0.0.47'
 authors = [{ name = 'questdb.io', email = 'miguel@questdb.io' }]
 description = "SqlAlchemy/Superset libraries."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
```

### Comparing `questdb-connect-0.0.46/src/examples/__init__.py` & `questdb-connect-0.0.47/src/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.46/src/examples/hello_world.py` & `questdb-connect-0.0.47/src/examples/hello_world.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.46/src/examples/psycopg2_connect.py` & `questdb-connect-0.0.47/src/examples/psycopg2_connect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.46/src/examples/server_utilisation.py` & `questdb-connect-0.0.47/src/examples/server_utilisation.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.46/src/examples/sqlalchemy_orm.py` & `questdb-connect-0.0.47/src/examples/sqlalchemy_orm.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.46/src/examples/sqlalchemy_raw.py` & `questdb-connect-0.0.47/src/examples/sqlalchemy_raw.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.46/src/questdb_connect/__init__.py` & `questdb-connect-0.0.47/src/questdb_connect/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.46/src/questdb_connect/dialect.py` & `questdb-connect-0.0.47/src/questdb_connect/dialect.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,28 +17,31 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 import abc
+from typing import List
 
 import sqlalchemy
+import sqlparse
 from sqlalchemy import Column, MetaData, text
 from sqlalchemy.dialects.postgresql.psycopg2 import PGDialect_psycopg2
 from sqlalchemy.engine.reflection import Inspector
 from sqlalchemy.orm.exc import NoResultFound
 from sqlalchemy.sql.base import SchemaEventTarget
 from sqlalchemy.sql.compiler import (
     DDLCompiler,
     GenericTypeCompiler,
     IdentifierPreparer,
     SQLCompiler,
 )
 from sqlalchemy.sql.visitors import Traversible
+from sqlparse import tokens as T
 
 from . import remove_public_schema
 from .types import *
 
 # ===== SQLAlchemy Dialect ======
 # https://docs.sqlalchemy.org/en/14/ apache-superset requires SQLAlchemy 1.4
 
@@ -113,14 +116,52 @@
 def _has_special_char(_value):
     for candidate in _value:
         if candidate in _special_chars:
             return True
     return False
 
 
+def parse_sql(sql: str, timestamp_alias: str = '__timestamp') -> List[str]:
+    parsed_sql_text = []
+    for parsed_sql in sqlparse.parse(sql):
+        if parsed_sql.get_type().lower() == 'select':
+            # remove timestamp column from any group by
+            ts_col_name = None
+            has_group_by = False
+            for tok in parsed_sql.tokens:
+                if not ts_col_name and isinstance(tok, sqlparse.sql.IdentifierList):
+                    for select_tok in tok.tokens:
+                        if timestamp_alias in select_tok.value:
+                            ts_col_name = select_tok.normalized
+                            break
+                elif ts_col_name and tok.value.lower() == 'group by':
+                    has_group_by = True
+                elif ts_col_name and has_group_by and isinstance(tok, sqlparse.sql.IdentifierList):
+                    remove_idx = None
+                    comma_idxs = []
+                    for idx, group_tok in enumerate(tok.tokens):
+                        if group_tok.match(T.Punctuation, ','):
+                            comma_idxs.append(idx)
+                        elif group_tok.normalized == ts_col_name:
+                            remove_idx = idx
+                    if remove_idx is not None:
+                        tok.tokens.pop(remove_idx)
+                        if remove_idx == 0:
+                            tok.tokens.pop(comma_idxs[0] - 1)
+                        else:
+                            remove_comma_idx = -1
+                            for i, c_i in enumerate(comma_idxs):
+                                if c_i > remove_idx:
+                                    remove_comma_idx = i - 1
+                                    break
+                            tok.tokens.pop(comma_idxs[remove_comma_idx])
+        parsed_sql_text.append(str(parsed_sql).strip(' ;'))
+    return parsed_sql_text
+
+
 class QDBIdentifierPreparer(IdentifierPreparer, abc.ABC):
     schema_for_object = staticmethod(_none)
 
     def __init__(
             self,
             dialect,
             initial_quote='"',
@@ -172,15 +213,17 @@
 
 
 class QDBSQLCompiler(SQLCompiler, abc.ABC):
     def _is_safe_for_fast_insert_values_helper(self):
         return True
 
     def visit_textclause(self, textclause, add_to_result_map=None, **kw):
-        textclause.text = remove_public_schema(textclause.text)
+        no_public_schema_sql = remove_public_schema(textclause.text)
+        final_sql = parse_sql(no_public_schema_sql)
+        textclause.text = final_sql[0] if final_sql else no_public_schema_sql
         return super().visit_textclause(textclause, add_to_result_map, **kw)
 
 
 class QDBInspector(Inspector, abc.ABC):
     def reflecttable(
             self,
             table,
```

### Comparing `questdb-connect-0.0.46/src/questdb_connect/function_names.py` & `questdb-connect-0.0.47/src/questdb_connect/function_names.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.46/src/questdb_connect/superset_engine.py` & `questdb-connect-0.0.47/src/questdb_connect/superset_engine.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 import re
 from datetime import datetime
 from typing import Any, Dict, List, Optional, Tuple
 
-import sqlparse
 from sqlalchemy.sql import text
 from sqlalchemy.types import TypeEngine
 from superset.db_engine_specs.base import BaseEngineSpec, BasicParametersMixin, BasicParametersType
 from superset.utils import core as utils
 from superset.utils.core import GenericDataType
 
 import questdb_connect.dialect as qdbcd
@@ -271,43 +270,8 @@
         :param database: The database to get functions for
         :return: A list of function names usable in the database
         """
         return FUNCTION_NAMES
 
     @classmethod
     def parse_sql(cls, sql: str) -> List[str]:
-        parsed_sql_text = []
-        for parsed_sql in sqlparse.parse(sql):
-            if parsed_sql.get_type() == 'SELECT':
-                # remove timestamp column from any group by
-                ts_col_name = None
-                has_group_by = False
-                for tok in parsed_sql.tokens:
-                    if not ts_col_name and isinstance(tok, sqlparse.sql.IdentifierList):
-                        for select_tok in tok.tokens:
-                            if isinstance(select_tok, sqlparse.sql.Identifier):
-                                if '__timestamp' in select_tok.value:
-                                    ts_col_name = select_tok.normalized
-                                    break
-                    elif ts_col_name and tok.value.lower() == 'group by':
-                        has_group_by = True
-                    elif ts_col_name and has_group_by and isinstance(tok, sqlparse.sql.IdentifierList):
-                        remove_idx = None
-                        comma_idxs = []
-                        for idx, group_tok in enumerate(tok.tokens):
-                            if group_tok.normalized == ',':
-                                comma_idxs.append(idx)
-                            elif group_tok.normalized == ts_col_name:
-                                remove_idx = idx
-                        if remove_idx is not None:
-                            tok.tokens.pop(remove_idx)
-                            if remove_idx == 0:
-                                tok.tokens.pop(comma_idxs[0] - 1)
-                            else:
-                                remove_comma_idx = -1
-                                for i, c_i in enumerate(comma_idxs):
-                                    if c_i > remove_idx:
-                                        remove_comma_idx = i - 1
-                                        break
-                                tok.tokens.pop(comma_idxs[remove_comma_idx])
-            parsed_sql_text.append(str(parsed_sql).strip(' ;'))
-        return parsed_sql_text
+        return qdbcd.parse_sql(sql, '__timestamp')
```

### Comparing `questdb-connect-0.0.46/src/questdb_connect/types.py` & `questdb-connect-0.0.47/src/questdb_connect/types.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.46/src/questdb_connect.egg-info/PKG-INFO` & `questdb-connect-0.0.47/src/questdb_connect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.46
+Version: 0.0.47
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.46/src/questdb_connect.egg-info/SOURCES.txt` & `questdb-connect-0.0.47/src/questdb_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.46/tests/test_dialect.py` & `questdb-connect-0.0.47/tests/test_dialect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.46/tests/test_superset.py` & `questdb-connect-0.0.47/tests/test_superset.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.46/tests/test_types.py` & `questdb-connect-0.0.47/tests/test_types.py`

 * *Files identical despite different names*

