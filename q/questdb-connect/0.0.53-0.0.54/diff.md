# Comparing `tmp/questdb-connect-0.0.53.tar.gz` & `tmp/questdb-connect-0.0.54.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "questdb-connect-0.0.53.tar", last modified: Tue May 16 18:52:00 2023, max compression
+gzip compressed data, was "questdb-connect-0.0.54.tar", last modified: Tue May 16 18:59:45 2023, max compression
```

## Comparing `questdb-connect-0.0.53.tar` & `questdb-connect-0.0.54.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-16 18:52:00.625564 questdb-connect-0.0.53/
--rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.53/LICENSE
--rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-16 18:52:00.625412 questdb-connect-0.0.53/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)     2734 2023-05-14 12:46:11.000000 questdb-connect-0.0.53/README.md
--rw-r--r--   0 marregui   (501) staff       (20)     2568 2023-05-16 18:51:33.000000 questdb-connect-0.0.53/pyproject.toml
--rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-16 18:52:00.625602 questdb-connect-0.0.53/setup.cfg
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-16 18:52:00.619538 questdb-connect-0.0.53/src/
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-16 18:52:00.621985 questdb-connect-0.0.53/src/examples/
--rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-0.0.53/src/examples/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-08 09:22:31.000000 questdb-connect-0.0.53/src/examples/hello_world.py
--rw-r--r--   0 marregui   (501) staff       (20)     2431 2023-05-10 11:39:52.000000 questdb-connect-0.0.53/src/examples/psycopg2_connect.py
--rw-r--r--   0 marregui   (501) staff       (20)     2831 2023-05-15 10:30:22.000000 questdb-connect-0.0.53/src/examples/server_utilisation.py
--rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-08 09:20:14.000000 questdb-connect-0.0.53/src/examples/sqlalchemy_orm.py
--rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-0.0.53/src/examples/sqlalchemy_raw.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-16 18:52:00.623411 questdb-connect-0.0.53/src/questdb_connect/
--rw-r--r--   0 marregui   (501) staff       (20)     3898 2023-05-16 13:44:22.000000 questdb-connect-0.0.53/src/questdb_connect/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)    11427 2023-05-16 13:44:28.000000 questdb-connect-0.0.53/src/questdb_connect/dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-0.0.53/src/questdb_connect/function_names.py
--rw-r--r--   0 marregui   (501) staff       (20)    11947 2023-05-16 18:50:36.000000 questdb-connect-0.0.53/src/questdb_connect/superset_engine.py
--rw-r--r--   0 marregui   (501) staff       (20)     5787 2023-05-03 12:21:25.000000 questdb-connect-0.0.53/src/questdb_connect/types.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-16 18:52:00.624407 questdb-connect-0.0.53/src/questdb_connect.egg-info/
--rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-16 18:52:00.000000 questdb-connect-0.0.53/src/questdb_connect.egg-info/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)      709 2023-05-16 18:52:00.000000 questdb-connect-0.0.53/src/questdb_connect.egg-info/SOURCES.txt
--rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-16 18:52:00.000000 questdb-connect-0.0.53/src/questdb_connect.egg-info/dependency_links.txt
--rw-r--r--   0 marregui   (501) staff       (20)      148 2023-05-16 18:52:00.000000 questdb-connect-0.0.53/src/questdb_connect.egg-info/entry_points.txt
--rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-16 18:52:00.000000 questdb-connect-0.0.53/src/questdb_connect.egg-info/requires.txt
--rw-r--r--   0 marregui   (501) staff       (20)       25 2023-05-16 18:52:00.000000 questdb-connect-0.0.53/src/questdb_connect.egg-info/top_level.txt
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-16 18:52:00.625009 questdb-connect-0.0.53/tests/
--rw-r--r--   0 marregui   (501) staff       (20)     9766 2023-05-16 09:28:52.000000 questdb-connect-0.0.53/tests/test_dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     3191 2023-05-16 18:50:31.000000 questdb-connect-0.0.53/tests/test_superset.py
--rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.53/tests/test_types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-16 18:59:45.561900 questdb-connect-0.0.54/
+-rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.54/LICENSE
+-rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-16 18:59:45.561771 questdb-connect-0.0.54/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)     2734 2023-05-14 12:46:11.000000 questdb-connect-0.0.54/README.md
+-rw-r--r--   0 marregui   (501) staff       (20)     2568 2023-05-16 18:59:26.000000 questdb-connect-0.0.54/pyproject.toml
+-rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-16 18:59:45.561933 questdb-connect-0.0.54/setup.cfg
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-16 18:59:45.556198 questdb-connect-0.0.54/src/
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-16 18:59:45.558379 questdb-connect-0.0.54/src/examples/
+-rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-0.0.54/src/examples/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-08 09:22:31.000000 questdb-connect-0.0.54/src/examples/hello_world.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2431 2023-05-10 11:39:52.000000 questdb-connect-0.0.54/src/examples/psycopg2_connect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2831 2023-05-15 10:30:22.000000 questdb-connect-0.0.54/src/examples/server_utilisation.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-08 09:20:14.000000 questdb-connect-0.0.54/src/examples/sqlalchemy_orm.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-0.0.54/src/examples/sqlalchemy_raw.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-16 18:59:45.559862 questdb-connect-0.0.54/src/questdb_connect/
+-rw-r--r--   0 marregui   (501) staff       (20)     3898 2023-05-16 13:44:22.000000 questdb-connect-0.0.54/src/questdb_connect/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)    11427 2023-05-16 13:44:28.000000 questdb-connect-0.0.54/src/questdb_connect/dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-0.0.54/src/questdb_connect/function_names.py
+-rw-r--r--   0 marregui   (501) staff       (20)    12330 2023-05-16 18:58:06.000000 questdb-connect-0.0.54/src/questdb_connect/superset_engine.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5787 2023-05-03 12:21:25.000000 questdb-connect-0.0.54/src/questdb_connect/types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-16 18:59:45.560787 questdb-connect-0.0.54/src/questdb_connect.egg-info/
+-rw-r--r--   0 marregui   (501) staff       (20)     3441 2023-05-16 18:59:45.000000 questdb-connect-0.0.54/src/questdb_connect.egg-info/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)      709 2023-05-16 18:59:45.000000 questdb-connect-0.0.54/src/questdb_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-16 18:59:45.000000 questdb-connect-0.0.54/src/questdb_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      148 2023-05-16 18:59:45.000000 questdb-connect-0.0.54/src/questdb_connect.egg-info/entry_points.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-16 18:59:45.000000 questdb-connect-0.0.54/src/questdb_connect.egg-info/requires.txt
+-rw-r--r--   0 marregui   (501) staff       (20)       25 2023-05-16 18:59:45.000000 questdb-connect-0.0.54/src/questdb_connect.egg-info/top_level.txt
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-16 18:59:45.561397 questdb-connect-0.0.54/tests/
+-rw-r--r--   0 marregui   (501) staff       (20)     9766 2023-05-16 09:28:52.000000 questdb-connect-0.0.54/tests/test_dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3191 2023-05-16 18:50:31.000000 questdb-connect-0.0.54/tests/test_superset.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.54/tests/test_types.py
```

### Comparing `questdb-connect-0.0.53/LICENSE` & `questdb-connect-0.0.54/LICENSE`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.53/PKG-INFO` & `questdb-connect-0.0.54/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.53
+Version: 0.0.54
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.53/README.md` & `questdb-connect-0.0.54/README.md`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.53/pyproject.toml` & `questdb-connect-0.0.54/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 # https://pip.pypa.io/en/stable/reference/build-system/pyproject-toml/
 [project]
 name = 'questdb-connect'
-version = '0.0.53'
+version = '0.0.54'
 authors = [{ name = 'questdb.io', email = 'miguel@questdb.io' }]
 description = "SqlAlchemy/Superset libraries."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
```

### Comparing `questdb-connect-0.0.53/src/examples/__init__.py` & `questdb-connect-0.0.54/src/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.53/src/examples/hello_world.py` & `questdb-connect-0.0.54/src/examples/hello_world.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.53/src/examples/psycopg2_connect.py` & `questdb-connect-0.0.54/src/examples/psycopg2_connect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.53/src/examples/server_utilisation.py` & `questdb-connect-0.0.54/src/examples/server_utilisation.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.53/src/examples/sqlalchemy_orm.py` & `questdb-connect-0.0.54/src/examples/sqlalchemy_orm.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.53/src/examples/sqlalchemy_raw.py` & `questdb-connect-0.0.54/src/examples/sqlalchemy_raw.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.53/src/questdb_connect/__init__.py` & `questdb-connect-0.0.54/src/questdb_connect/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.53/src/questdb_connect/dialect.py` & `questdb-connect-0.0.54/src/questdb_connect/dialect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.53/src/questdb_connect/function_names.py` & `questdb-connect-0.0.54/src/questdb_connect/function_names.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.53/src/questdb_connect/superset_engine.py` & `questdb-connect-0.0.54/src/questdb_connect/superset_engine.py`

 * *Files 3% similar despite different names*

```diff
@@ -138,14 +138,23 @@
         :return: text clause with escaped characters
         """
         if cls.allows_escaped_colons:
             clause = clause.replace(":", "\\:")
         return text(remove_public_schema(clause))
 
     @classmethod
+    def get_time_grain_expressions(cls) -> Dict[Optional[str], str]:
+        """Return a dict of all supported time grains including any
+        potential added grains but excluding any potentially disabled
+        grains in the config file.
+        :return: All time grain expressions supported by the engine
+        """
+        return cls._time_grain_expressions
+
+    @classmethod
     def epoch_to_dttm(cls) -> str:
         """SQL expression that converts epoch (seconds) to datetime that can be used in a
         query. The reference column should be denoted as `{col}` in the return
         expression, e.g. "FROM_UNIXTIME({col})"
         :return: SQL Expression
         """
         return '{col} * 1000000'
```

### Comparing `questdb-connect-0.0.53/src/questdb_connect/types.py` & `questdb-connect-0.0.54/src/questdb_connect/types.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.53/src/questdb_connect.egg-info/PKG-INFO` & `questdb-connect-0.0.54/src/questdb_connect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.53
+Version: 0.0.54
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.53/src/questdb_connect.egg-info/SOURCES.txt` & `questdb-connect-0.0.54/src/questdb_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.53/tests/test_dialect.py` & `questdb-connect-0.0.54/tests/test_dialect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.53/tests/test_superset.py` & `questdb-connect-0.0.54/tests/test_superset.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.53/tests/test_types.py` & `questdb-connect-0.0.54/tests/test_types.py`

 * *Files identical despite different names*

