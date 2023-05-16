# Comparing `tmp/apache-airflow-providers-common-sql-1.4.0rc1.tar.gz` & `tmp/apache-airflow-providers-common-sql-1.5.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-common-sql-1.4.0rc1.tar", last modified: Sun Apr  2 05:47:23 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-common-sql-1.5.0rc1.tar", last modified: Tue May 16 15:53:31 2023, max compression
```

## Comparing `apache-airflow-providers-common-sql-1.4.0rc1.tar` & `apache-airflow-providers-common-sql-1.5.0rc1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:23.000000 apache-airflow-providers-common-sql-1.4.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-common-sql-1.4.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1122 2023-04-02 05:47:21.000000 apache-airflow-providers-common-sql-1.4.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-common-sql-1.4.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     9401 2023-04-02 05:47:23.000000 apache-airflow-providers-common-sql-1.4.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7839 2023-04-02 05:47:21.000000 apache-airflow-providers-common-sql-1.4.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:23.000000 apache-airflow-providers-common-sql-1.4.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:23.000000 apache-airflow-providers-common-sql-1.4.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:23.000000 apache-airflow-providers-common-sql-1.4.0rc1/airflow/providers/common/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:23.000000 apache-airflow-providers-common-sql-1.4.0rc1/airflow/providers/common/sql/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-common-sql-1.4.0rc1/airflow/providers/common/sql/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2343 2023-04-02 05:47:21.000000 apache-airflow-providers-common-sql-1.4.0rc1/airflow/providers/common/sql/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:23.000000 apache-airflow-providers-common-sql-1.4.0rc1/airflow/providers/common/sql/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-common-sql-1.4.0rc1/airflow/providers/common/sql/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21739 2023-03-06 20:52:28.000000 apache-airflow-providers-common-sql-1.4.0rc1/airflow/providers/common/sql/hooks/sql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:23.000000 apache-airflow-providers-common-sql-1.4.0rc1/airflow/providers/common/sql/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-common-sql-1.4.0rc1/airflow/providers/common/sql/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    44390 2023-03-10 19:31:58.000000 apache-airflow-providers-common-sql-1.4.0rc1/airflow/providers/common/sql/operators/sql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:23.000000 apache-airflow-providers-common-sql-1.4.0rc1/airflow/providers/common/sql/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-common-sql-1.4.0rc1/airflow/providers/common/sql/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4691 2023-02-24 18:43:53.000000 apache-airflow-providers-common-sql-1.4.0rc1/airflow/providers/common/sql/sensors/sql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:23.000000 apache-airflow-providers-common-sql-1.4.0rc1/apache_airflow_providers_common_sql.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9401 2023-04-02 05:47:23.000000 apache-airflow-providers-common-sql-1.4.0rc1/apache_airflow_providers_common_sql.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      855 2023-04-02 05:47:23.000000 apache-airflow-providers-common-sql-1.4.0rc1/apache_airflow_providers_common_sql.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-02 05:47:23.000000 apache-airflow-providers-common-sql-1.4.0rc1/apache_airflow_providers_common_sql.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-04-02 05:47:23.000000 apache-airflow-providers-common-sql-1.4.0rc1/apache_airflow_providers_common_sql.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-02 05:47:23.000000 apache-airflow-providers-common-sql-1.4.0rc1/apache_airflow_providers_common_sql.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       41 2023-04-02 05:47:23.000000 apache-airflow-providers-common-sql-1.4.0rc1/apache_airflow_providers_common_sql.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-02 05:47:23.000000 apache-airflow-providers-common-sql-1.4.0rc1/apache_airflow_providers_common_sql.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5393 2023-04-01 16:40:04.000000 apache-airflow-providers-common-sql-1.4.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1841 2023-04-02 05:47:23.000000 apache-airflow-providers-common-sql-1.4.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1530 2023-04-02 05:47:21.000000 apache-airflow-providers-common-sql-1.4.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:31.000000 apache-airflow-providers-common-sql-1.5.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-common-sql-1.5.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-05-16 15:53:30.000000 apache-airflow-providers-common-sql-1.5.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-common-sql-1.5.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    10159 2023-05-16 15:53:31.000000 apache-airflow-providers-common-sql-1.5.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8597 2023-05-16 15:53:30.000000 apache-airflow-providers-common-sql-1.5.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:31.000000 apache-airflow-providers-common-sql-1.5.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:31.000000 apache-airflow-providers-common-sql-1.5.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:31.000000 apache-airflow-providers-common-sql-1.5.0rc1/airflow/providers/common/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:31.000000 apache-airflow-providers-common-sql-1.5.0rc1/airflow/providers/common/sql/
+-rw-r--r--   0 root         (0) root         (0)     1393 2023-05-16 15:39:21.000000 apache-airflow-providers-common-sql-1.5.0rc1/airflow/providers/common/sql/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2511 2023-05-16 15:53:30.000000 apache-airflow-providers-common-sql-1.5.0rc1/airflow/providers/common/sql/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:31.000000 apache-airflow-providers-common-sql-1.5.0rc1/airflow/providers/common/sql/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-common-sql-1.5.0rc1/airflow/providers/common/sql/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21739 2023-03-06 20:52:28.000000 apache-airflow-providers-common-sql-1.5.0rc1/airflow/providers/common/sql/hooks/sql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:31.000000 apache-airflow-providers-common-sql-1.5.0rc1/airflow/providers/common/sql/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-common-sql-1.5.0rc1/airflow/providers/common/sql/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    44516 2023-05-12 08:38:07.000000 apache-airflow-providers-common-sql-1.5.0rc1/airflow/providers/common/sql/operators/sql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:31.000000 apache-airflow-providers-common-sql-1.5.0rc1/airflow/providers/common/sql/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-common-sql-1.5.0rc1/airflow/providers/common/sql/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4691 2023-02-24 18:43:53.000000 apache-airflow-providers-common-sql-1.5.0rc1/airflow/providers/common/sql/sensors/sql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:31.000000 apache-airflow-providers-common-sql-1.5.0rc1/apache_airflow_providers_common_sql.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10159 2023-05-16 15:53:31.000000 apache-airflow-providers-common-sql-1.5.0rc1/apache_airflow_providers_common_sql.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      855 2023-05-16 15:53:31.000000 apache-airflow-providers-common-sql-1.5.0rc1/apache_airflow_providers_common_sql.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:53:31.000000 apache-airflow-providers-common-sql-1.5.0rc1/apache_airflow_providers_common_sql.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-05-16 15:53:31.000000 apache-airflow-providers-common-sql-1.5.0rc1/apache_airflow_providers_common_sql.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:53:31.000000 apache-airflow-providers-common-sql-1.5.0rc1/apache_airflow_providers_common_sql.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       41 2023-05-16 15:53:31.000000 apache-airflow-providers-common-sql-1.5.0rc1/apache_airflow_providers_common_sql.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-16 15:53:31.000000 apache-airflow-providers-common-sql-1.5.0rc1/apache_airflow_providers_common_sql.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5308 2023-05-15 09:39:26.000000 apache-airflow-providers-common-sql-1.5.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1841 2023-05-16 15:53:31.000000 apache-airflow-providers-common-sql-1.5.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1690 2023-05-16 15:53:30.000000 apache-airflow-providers-common-sql-1.5.0rc1/setup.py
```

### Comparing `apache-airflow-providers-common-sql-1.4.0rc1/LICENSE` & `apache-airflow-providers-common-sql-1.5.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.4.0rc1/MANIFEST.in` & `apache-airflow-providers-common-sql-1.5.0rc1/MANIFEST.in`

 * *Files 6% similar despite different names*

```diff
@@ -23,10 +23,9 @@
 # `MANIFEST_TEMPLATE.py.jinja2` IN the `provider_packages` DIRECTORY
 
 
 
 
 include NOTICE
 include LICENSE
-include CHANGELOG.txt
-include README.md
+include CHANGELOG.rst
 global-exclude __pycache__  *.pyc
```

### Comparing `apache-airflow-providers-common-sql-1.4.0rc1/PKG-INFO` & `apache-airflow-providers-common-sql-1.5.0rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-common-sql
-Version: 1.4.0rc1
+Version: 1.5.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-common-sql package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.4.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.5.0/
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -49,28 +49,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-common-sql``
 
-Release: ``1.4.0rc1``
+Release: ``1.5.0rc1``
 
 
 `Common SQL Provider <https://en.wikipedia.org/wiki/SQL>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``common.sql`` provider. All classes for this provider package
 are in ``airflow.providers.common.sql`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.4.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.5.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -109,14 +109,36 @@
     and you want to add an explanation to the users on how they are supposed to deal with them.
     The changelog is updated and maintained semi-automatically by release manager.
 
 
 Changelog
 ---------
 
+1.5.0
+.....
+
+.. note::
+  This release of provider is only available for Airflow 2.4+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
+
+Features
+~~~~~~~~
+
+* ``Add conditional output processing in SQL operators (#31136)``
+
+Misc
+~~~~
+
+* ``Remove noisy log from SQL table check (#31037)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add mechanism to suspend providers (#30422)``
+
 1.4.0
 .....
 
 Features
 ~~~~~~~~
 
 * ``Add option to show output of 'SQLExecuteQueryOperator' in the log (#29954)``
@@ -192,16 +214,17 @@
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Prepare for follow-up release for November providers (#27774)``
 
 1.3.0
 .....
 
-This release of provider is only available for Airflow 2.3+ as explained in the
-`Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/README.md#support-for-providers>`_.
+.. note::
+  This release of provider is only available for Airflow 2.3+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Misc
 ~~~~
 
 * ``Move min airflow version to 2.3.0 for all providers (#27196)``
 
 Features
```

### Comparing `apache-airflow-providers-common-sql-1.4.0rc1/README.rst` & `apache-airflow-providers-common-sql-1.5.0rc1/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -15,28 +15,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-common-sql``
 
-Release: ``1.4.0rc1``
+Release: ``1.5.0rc1``
 
 
 `Common SQL Provider <https://en.wikipedia.org/wiki/SQL>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``common.sql`` provider. All classes for this provider package
 are in ``airflow.providers.common.sql`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.4.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.5.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -75,14 +75,36 @@
     and you want to add an explanation to the users on how they are supposed to deal with them.
     The changelog is updated and maintained semi-automatically by release manager.
 
 
 Changelog
 ---------
 
+1.5.0
+.....
+
+.. note::
+  This release of provider is only available for Airflow 2.4+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
+
+Features
+~~~~~~~~
+
+* ``Add conditional output processing in SQL operators (#31136)``
+
+Misc
+~~~~
+
+* ``Remove noisy log from SQL table check (#31037)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add mechanism to suspend providers (#30422)``
+
 1.4.0
 .....
 
 Features
 ~~~~~~~~
 
 * ``Add option to show output of 'SQLExecuteQueryOperator' in the log (#29954)``
@@ -158,16 +180,17 @@
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Prepare for follow-up release for November providers (#27774)``
 
 1.3.0
 .....
 
-This release of provider is only available for Airflow 2.3+ as explained in the
-`Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/README.md#support-for-providers>`_.
+.. note::
+  This release of provider is only available for Airflow 2.3+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Misc
 ~~~~
 
 * ``Move min airflow version to 2.3.0 for all providers (#27196)``
 
 Features
```

### Comparing `apache-airflow-providers-common-sql-1.4.0rc1/airflow/providers/common/sql/__init__.py` & `apache-airflow-providers-common-sql-1.5.0rc1/airflow/providers/common/sql/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.4.0rc1/airflow/providers/common/sql/get_provider_info.py` & `apache-airflow-providers-common-sql-1.5.0rc1/airflow/providers/common/sql/get_provider_info.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,15 +23,27 @@
 
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-common-sql",
         "name": "Common SQL",
         "description": "`Common SQL Provider <https://en.wikipedia.org/wiki/SQL>`__\n",
-        "versions": ["1.4.0", "1.3.4", "1.3.3", "1.3.2", "1.3.1", "1.3.0", "1.2.0", "1.1.0", "1.0.0"],
+        "suspended": False,
+        "versions": [
+            "1.5.0",
+            "1.4.0",
+            "1.3.4",
+            "1.3.3",
+            "1.3.2",
+            "1.3.1",
+            "1.3.0",
+            "1.2.0",
+            "1.1.0",
+            "1.0.0",
+        ],
         "dependencies": ["sqlparse>=0.4.2"],
         "additional-extras": [{"name": "pandas", "dependencies": ["pandas>=0.17.1"]}],
         "integrations": [
             {
                 "integration-name": "Common SQL",
                 "external-doc-url": "https://en.wikipedia.org/wiki/SQL",
                 "how-to-guide": ["/docs/apache-airflow-providers-common-sql/operators.rst"],
```

### Comparing `apache-airflow-providers-common-sql-1.4.0rc1/airflow/providers/common/sql/hooks/__init__.py` & `apache-airflow-providers-common-sql-1.5.0rc1/airflow/providers/common/sql/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.4.0rc1/airflow/providers/common/sql/hooks/sql.py` & `apache-airflow-providers-common-sql-1.5.0rc1/airflow/providers/common/sql/hooks/sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.4.0rc1/airflow/providers/common/sql/operators/__init__.py` & `apache-airflow-providers-common-sql-1.5.0rc1/airflow/providers/common/sql/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.4.0rc1/airflow/providers/common/sql/operators/sql.py` & `apache-airflow-providers-common-sql-1.5.0rc1/airflow/providers/common/sql/operators/sql.py`

 * *Files 0% similar despite different names*

```diff
@@ -254,30 +254,33 @@
         :param results: results in the form of list of rows.
         :param descriptions: list of descriptions returned by ``cur.description`` in the Python DBAPI
         """
         if self.show_return_value_in_logs:
             self.log.info("Operator output is: %s", results)
         return results
 
+    def _should_run_output_processing(self) -> bool:
+        return self.do_xcom_push
+
     def execute(self, context):
         self.log.info("Executing: %s", self.sql)
         hook = self.get_db_hook()
         if self.split_statements is not None:
             extra_kwargs = {"split_statements": self.split_statements}
         else:
             extra_kwargs = {}
         output = hook.run(
             sql=self.sql,
             autocommit=self.autocommit,
             parameters=self.parameters,
-            handler=self.handler if self.do_xcom_push else None,
+            handler=self.handler if self._should_run_output_processing() else None,
             return_last=self.return_last,
             **extra_kwargs,
         )
-        if not self.do_xcom_push:
+        if not self._should_run_output_processing():
             return None
         if return_single_query_results(self.sql, self.return_last, self.split_statements):
             # For simplicity, we pass always list as input to _process_output, regardless if
             # single query results are going to be returned, and we return the first element
             # of the list in this case from the (always) list returned by _process_output
             return self._process_output([output], hook.descriptions)[-1]
         return self._process_output(output, hook.descriptions)
@@ -618,15 +621,15 @@
                 f"The following tests have failed:\n{', '.join(failed_tests)}"
             )
             self._raise_exception(exception_string)
 
         self.log.info("All tests have passed")
 
     def _generate_sql_query(self):
-        self.log.info("Partition clause: %s", self.partition_clause)
+        self.log.debug("Partition clause: %s", self.partition_clause)
 
         def _generate_partition_clause(check_name):
             if self.partition_clause and "partition_clause" not in self.checks[check_name]:
                 return f"WHERE {self.partition_clause}"
             elif not self.partition_clause and "partition_clause" in self.checks[check_name]:
                 return f"WHERE {self.checks[check_name]['partition_clause']}"
             elif self.partition_clause and "partition_clause" in self.checks[check_name]:
```

### Comparing `apache-airflow-providers-common-sql-1.4.0rc1/airflow/providers/common/sql/sensors/sql.py` & `apache-airflow-providers-common-sql-1.5.0rc1/airflow/providers/common/sql/sensors/sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.4.0rc1/apache_airflow_providers_common_sql.egg-info/PKG-INFO` & `apache-airflow-providers-common-sql-1.5.0rc1/apache_airflow_providers_common_sql.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-common-sql
-Version: 1.4.0rc1
+Version: 1.5.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-common-sql package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.4.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.5.0/
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -49,28 +49,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-common-sql``
 
-Release: ``1.4.0rc1``
+Release: ``1.5.0rc1``
 
 
 `Common SQL Provider <https://en.wikipedia.org/wiki/SQL>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``common.sql`` provider. All classes for this provider package
 are in ``airflow.providers.common.sql`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.4.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.5.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -109,14 +109,36 @@
     and you want to add an explanation to the users on how they are supposed to deal with them.
     The changelog is updated and maintained semi-automatically by release manager.
 
 
 Changelog
 ---------
 
+1.5.0
+.....
+
+.. note::
+  This release of provider is only available for Airflow 2.4+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
+
+Features
+~~~~~~~~
+
+* ``Add conditional output processing in SQL operators (#31136)``
+
+Misc
+~~~~
+
+* ``Remove noisy log from SQL table check (#31037)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add mechanism to suspend providers (#30422)``
+
 1.4.0
 .....
 
 Features
 ~~~~~~~~
 
 * ``Add option to show output of 'SQLExecuteQueryOperator' in the log (#29954)``
@@ -192,16 +214,17 @@
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Prepare for follow-up release for November providers (#27774)``
 
 1.3.0
 .....
 
-This release of provider is only available for Airflow 2.3+ as explained in the
-`Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/README.md#support-for-providers>`_.
+.. note::
+  This release of provider is only available for Airflow 2.3+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Misc
 ~~~~
 
 * ``Move min airflow version to 2.3.0 for all providers (#27196)``
 
 Features
```

### Comparing `apache-airflow-providers-common-sql-1.4.0rc1/apache_airflow_providers_common_sql.egg-info/SOURCES.txt` & `apache-airflow-providers-common-sql-1.5.0rc1/apache_airflow_providers_common_sql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.4.0rc1/pyproject.toml` & `apache-airflow-providers-common-sql-1.5.0rc1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,16 @@
 target-version = "py37"
 
 extend-select = [
     "I", # Missing required import (auto-fixable)
     "UP", # Pyupgrade
     "RUF100", # Unused noqa (auto-fixable)
 
+    # implicit single-line string concatenation
+    "ISC001",
     # We ignore more pydocstyle than we enable, so be more selective at what we enable
     "D101",
     "D106",
     "D2",
     "D3",
     # "D401", # Not enabled by ruff, but we don't want it
     "D402",
@@ -135,18 +137,15 @@
 
 # The test_python.py is needed because adding __future__.annotations breaks runtime checks that are
 # needed for the test to work
 "tests/decorators/test_python.py" = ["I002"]
 
 # The Pydantic representations of SqlAlchemy Models are not parsed well with Pydantic
 # when __future__.annotations is used so we need to skip them from upgrading
-"airflow/models/pydantic/taskinstance.py" = ["I002"]
-"airflow/models/pydantic/dag_run.py" = ["I002"]
-"airflow/models/pydantic/dataset.py" = ["I002"]
-"airflow/jobs/pydantic/base_job.py" = ["I002"]
+"airflow/serialization/pydantic/*.py" = ["I002"]
 
 # Ignore pydoc style from these
 "*.pyi" = ["D"]
 "tests/*" = ["D"]
 "scripts/*" = ["D"]
 "dev/*" = ["D"]
 "docs/*" = ["D"]
```

### Comparing `apache-airflow-providers-common-sql-1.4.0rc1/setup.cfg` & `apache-airflow-providers-common-sql-1.5.0rc1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.4.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.5.0/
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
```

### Comparing `apache-airflow-providers-common-sql-1.4.0rc1/setup.py` & `apache-airflow-providers-common-sql-1.5.0rc1/airflow/providers/common/sql/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,34 +11,28 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
-
+#
 # NOTE! THIS FILE IS AUTOMATICALLY GENERATED AND WILL BE
-# OVERWRITTEN WHEN PREPARING PACKAGES.
+# OVERWRITTEN WHEN PREPARING DOCUMENTATION FOR THE PACKAGES.
 #
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
-# `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
+# `PROVIDER__INIT__PY_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
+#
+from __future__ import annotations
 
-"""Setup.py for the apache-airflow-providers-common-sql package."""
+import packaging.version
 
-from setuptools import find_namespace_packages, setup
+import airflow
 
-version = "1.4.0"
+__all__ = ["version"]
 
+version = "1.5.0"
 
-def do_setup():
-    """Perform the package apache-airflow-providers-common-sql setup."""
-    setup(
-        version=version,
-        extras_require={"pandas": ["pandas>=0.17.1"]},
-        packages=find_namespace_packages(
-            include=["airflow.providers.common.sql", "airflow.providers.common.sql.*"]
-        ),
+if packaging.version.parse(airflow.version.version) < packaging.version.parse("2.4.0"):
+    raise RuntimeError(
+        f"The package `apache-airflow-providers-common-sql:{version}` requires Apache Airflow 2.4.0+"
     )
-
-
-if __name__ == "__main__":
-    do_setup()
```

