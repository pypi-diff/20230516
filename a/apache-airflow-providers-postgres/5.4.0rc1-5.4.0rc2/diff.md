# Comparing `tmp/apache-airflow-providers-postgres-5.4.0rc1.tar.gz` & `tmp/apache-airflow-providers-postgres-5.4.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-postgres-5.4.0rc1.tar", last modified: Fri Dec 30 17:24:17 2022, max compression
+gzip compressed data, was "dist/apache-airflow-providers-postgres-5.4.0rc2.tar", last modified: Mon Jan  2 13:09:39 2023, max compression
```

## Comparing `apache-airflow-providers-postgres-5.4.0rc1.tar` & `apache-airflow-providers-postgres-5.4.0rc2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-30 17:24:17.000000 apache-airflow-providers-postgres-5.4.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2022-10-05 12:15:16.000000 apache-airflow-providers-postgres-5.4.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1122 2022-12-30 17:24:16.000000 apache-airflow-providers-postgres-5.4.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2022-10-05 12:15:16.000000 apache-airflow-providers-postgres-5.4.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    14231 2022-12-30 17:24:17.000000 apache-airflow-providers-postgres-5.4.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12628 2022-12-30 17:24:16.000000 apache-airflow-providers-postgres-5.4.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-30 17:24:17.000000 apache-airflow-providers-postgres-5.4.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-30 17:24:17.000000 apache-airflow-providers-postgres-5.4.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-30 17:24:17.000000 apache-airflow-providers-postgres-5.4.0rc1/airflow/providers/postgres/
--rw-r--r--   0 root         (0) root         (0)      787 2022-10-05 12:15:15.000000 apache-airflow-providers-postgres-5.4.0rc1/airflow/providers/postgres/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3007 2022-12-30 17:24:16.000000 apache-airflow-providers-postgres-5.4.0rc1/airflow/providers/postgres/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-30 17:24:17.000000 apache-airflow-providers-postgres-5.4.0rc1/airflow/providers/postgres/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2022-10-05 12:15:15.000000 apache-airflow-providers-postgres-5.4.0rc1/airflow/providers/postgres/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12891 2022-11-14 15:45:54.000000 apache-airflow-providers-postgres-5.4.0rc1/airflow/providers/postgres/hooks/postgres.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-30 17:24:17.000000 apache-airflow-providers-postgres-5.4.0rc1/airflow/providers/postgres/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2022-10-05 12:15:15.000000 apache-airflow-providers-postgres-5.4.0rc1/airflow/providers/postgres/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3654 2022-11-03 13:17:26.000000 apache-airflow-providers-postgres-5.4.0rc1/airflow/providers/postgres/operators/postgres.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-30 17:24:17.000000 apache-airflow-providers-postgres-5.4.0rc1/apache_airflow_providers_postgres.egg-info/
--rw-r--r--   0 root         (0) root         (0)    14231 2022-12-30 17:24:17.000000 apache-airflow-providers-postgres-5.4.0rc1/apache_airflow_providers_postgres.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      746 2022-12-30 17:24:17.000000 apache-airflow-providers-postgres-5.4.0rc1/apache_airflow_providers_postgres.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-30 17:24:17.000000 apache-airflow-providers-postgres-5.4.0rc1/apache_airflow_providers_postgres.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      106 2022-12-30 17:24:17.000000 apache-airflow-providers-postgres-5.4.0rc1/apache_airflow_providers_postgres.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-30 17:24:17.000000 apache-airflow-providers-postgres-5.4.0rc1/apache_airflow_providers_postgres.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      197 2022-12-30 17:24:17.000000 apache-airflow-providers-postgres-5.4.0rc1/apache_airflow_providers_postgres.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2022-12-30 17:24:17.000000 apache-airflow-providers-postgres-5.4.0rc1/apache_airflow_providers_postgres.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1860 2022-12-20 13:50:44.000000 apache-airflow-providers-postgres-5.4.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1913 2022-12-30 17:24:17.000000 apache-airflow-providers-postgres-5.4.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1636 2022-12-30 17:24:16.000000 apache-airflow-providers-postgres-5.4.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-02 13:09:39.000000 apache-airflow-providers-postgres-5.4.0rc2/
+-rw-r--r--   0 root         (0) root         (0)    10850 2022-10-05 12:15:16.000000 apache-airflow-providers-postgres-5.4.0rc2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1122 2023-01-02 13:09:37.000000 apache-airflow-providers-postgres-5.4.0rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2022-10-05 12:15:16.000000 apache-airflow-providers-postgres-5.4.0rc2/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    14169 2023-01-02 13:09:39.000000 apache-airflow-providers-postgres-5.4.0rc2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12566 2023-01-02 13:09:37.000000 apache-airflow-providers-postgres-5.4.0rc2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-02 13:09:38.000000 apache-airflow-providers-postgres-5.4.0rc2/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-02 13:09:38.000000 apache-airflow-providers-postgres-5.4.0rc2/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-02 13:09:38.000000 apache-airflow-providers-postgres-5.4.0rc2/airflow/providers/postgres/
+-rw-r--r--   0 root         (0) root         (0)      787 2022-10-05 12:15:15.000000 apache-airflow-providers-postgres-5.4.0rc2/airflow/providers/postgres/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3007 2023-01-02 13:09:37.000000 apache-airflow-providers-postgres-5.4.0rc2/airflow/providers/postgres/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-02 13:09:39.000000 apache-airflow-providers-postgres-5.4.0rc2/airflow/providers/postgres/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2022-10-05 12:15:15.000000 apache-airflow-providers-postgres-5.4.0rc2/airflow/providers/postgres/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12891 2022-11-14 15:45:54.000000 apache-airflow-providers-postgres-5.4.0rc2/airflow/providers/postgres/hooks/postgres.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-02 13:09:39.000000 apache-airflow-providers-postgres-5.4.0rc2/airflow/providers/postgres/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2022-10-05 12:15:15.000000 apache-airflow-providers-postgres-5.4.0rc2/airflow/providers/postgres/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3654 2022-11-03 13:17:26.000000 apache-airflow-providers-postgres-5.4.0rc2/airflow/providers/postgres/operators/postgres.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-02 13:09:39.000000 apache-airflow-providers-postgres-5.4.0rc2/apache_airflow_providers_postgres.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    14169 2023-01-02 13:09:38.000000 apache-airflow-providers-postgres-5.4.0rc2/apache_airflow_providers_postgres.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      746 2023-01-02 13:09:38.000000 apache-airflow-providers-postgres-5.4.0rc2/apache_airflow_providers_postgres.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-01-02 13:09:38.000000 apache-airflow-providers-postgres-5.4.0rc2/apache_airflow_providers_postgres.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      106 2023-01-02 13:09:38.000000 apache-airflow-providers-postgres-5.4.0rc2/apache_airflow_providers_postgres.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-01-02 13:09:38.000000 apache-airflow-providers-postgres-5.4.0rc2/apache_airflow_providers_postgres.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      197 2023-01-02 13:09:38.000000 apache-airflow-providers-postgres-5.4.0rc2/apache_airflow_providers_postgres.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-01-02 13:09:38.000000 apache-airflow-providers-postgres-5.4.0rc2/apache_airflow_providers_postgres.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1860 2022-12-20 13:50:44.000000 apache-airflow-providers-postgres-5.4.0rc2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1913 2023-01-02 13:09:39.000000 apache-airflow-providers-postgres-5.4.0rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1636 2023-01-02 13:09:37.000000 apache-airflow-providers-postgres-5.4.0rc2/setup.py
```

### Comparing `apache-airflow-providers-postgres-5.4.0rc1/LICENSE` & `apache-airflow-providers-postgres-5.4.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-postgres-5.4.0rc1/MANIFEST.in` & `apache-airflow-providers-postgres-5.4.0rc2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-postgres-5.4.0rc1/PKG-INFO` & `apache-airflow-providers-postgres-5.4.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-postgres
-Version: 5.4.0rc1
+Version: 5.4.0rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-postgres package
 Home-page: https://airflow.apache.org/
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-postgres/5.4.0/
@@ -51,15 +51,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-postgres``
 
-Release: ``5.4.0rc1``
+Release: ``5.4.0rc2``
 
 
 `PostgreSQL <https://www.postgresql.org/>`__
 
 
 Provider package
 ----------------
@@ -136,29 +136,20 @@
 
 Changelog
 ---------
 
 5.4.0
 .....
 
-Breaking changes
-~~~~~~~~~~~~~~~~
-
-
 Features
 ~~~~~~~~
-
-
-Bug Fixes
-~~~~~~~~~
-
+* ``Bring back psycopg2-binary as dependency instead of psycopg (#28316)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
-   * ``Bring back psycopg2-binary as dependency instead of psycopg (#28316)``
 
 5.3.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
```

### Comparing `apache-airflow-providers-postgres-5.4.0rc1/README.rst` & `apache-airflow-providers-postgres-5.4.0rc2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-postgres``
 
-Release: ``5.4.0rc1``
+Release: ``5.4.0rc2``
 
 
 `PostgreSQL <https://www.postgresql.org/>`__
 
 
 Provider package
 ----------------
@@ -100,29 +100,20 @@
 
 Changelog
 ---------
 
 5.4.0
 .....
 
-Breaking changes
-~~~~~~~~~~~~~~~~
-
-
 Features
 ~~~~~~~~
-
-
-Bug Fixes
-~~~~~~~~~
-
+* ``Bring back psycopg2-binary as dependency instead of psycopg (#28316)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
-   * ``Bring back psycopg2-binary as dependency instead of psycopg (#28316)``
 
 5.3.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
```

### Comparing `apache-airflow-providers-postgres-5.4.0rc1/airflow/providers/postgres/__init__.py` & `apache-airflow-providers-postgres-5.4.0rc2/airflow/providers/postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-postgres-5.4.0rc1/airflow/providers/postgres/get_provider_info.py` & `apache-airflow-providers-postgres-5.4.0rc2/airflow/providers/postgres/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-postgres-5.4.0rc1/airflow/providers/postgres/hooks/__init__.py` & `apache-airflow-providers-postgres-5.4.0rc2/airflow/providers/postgres/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-postgres-5.4.0rc1/airflow/providers/postgres/hooks/postgres.py` & `apache-airflow-providers-postgres-5.4.0rc2/airflow/providers/postgres/hooks/postgres.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-postgres-5.4.0rc1/airflow/providers/postgres/operators/__init__.py` & `apache-airflow-providers-postgres-5.4.0rc2/airflow/providers/postgres/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-postgres-5.4.0rc1/airflow/providers/postgres/operators/postgres.py` & `apache-airflow-providers-postgres-5.4.0rc2/airflow/providers/postgres/operators/postgres.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-postgres-5.4.0rc1/apache_airflow_providers_postgres.egg-info/PKG-INFO` & `apache-airflow-providers-postgres-5.4.0rc2/apache_airflow_providers_postgres.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-postgres
-Version: 5.4.0rc1
+Version: 5.4.0rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-postgres package
 Home-page: https://airflow.apache.org/
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-postgres/5.4.0/
@@ -51,15 +51,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-postgres``
 
-Release: ``5.4.0rc1``
+Release: ``5.4.0rc2``
 
 
 `PostgreSQL <https://www.postgresql.org/>`__
 
 
 Provider package
 ----------------
@@ -136,29 +136,20 @@
 
 Changelog
 ---------
 
 5.4.0
 .....
 
-Breaking changes
-~~~~~~~~~~~~~~~~
-
-
 Features
 ~~~~~~~~
-
-
-Bug Fixes
-~~~~~~~~~
-
+* ``Bring back psycopg2-binary as dependency instead of psycopg (#28316)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
-   * ``Bring back psycopg2-binary as dependency instead of psycopg (#28316)``
 
 5.3.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
```

### Comparing `apache-airflow-providers-postgres-5.4.0rc1/apache_airflow_providers_postgres.egg-info/SOURCES.txt` & `apache-airflow-providers-postgres-5.4.0rc2/apache_airflow_providers_postgres.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-postgres-5.4.0rc1/pyproject.toml` & `apache-airflow-providers-postgres-5.4.0rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-postgres-5.4.0rc1/setup.cfg` & `apache-airflow-providers-postgres-5.4.0rc2/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -54,10 +54,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.postgres.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.postgres
 
 [egg_info]
-tag_build = rc1
+tag_build = rc2
 tag_date = 0
```

### Comparing `apache-airflow-providers-postgres-5.4.0rc1/setup.py` & `apache-airflow-providers-postgres-5.4.0rc2/setup.py`

 * *Files identical despite different names*

