# Comparing `tmp/apache-airflow-providers-mysql-5.0.0rc1.tar.gz` & `tmp/apache-airflow-providers-mysql-5.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-mysql-5.0.0rc1.tar", last modified: Fri Apr 21 19:49:45 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-mysql-5.1.0rc1.tar", last modified: Tue May 16 15:54:40 2023, max compression
```

## Comparing `apache-airflow-providers-mysql-5.0.0rc1.tar` & `apache-airflow-providers-mysql-5.1.0rc1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:49:45.000000 apache-airflow-providers-mysql-5.0.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-mysql-5.0.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-04-21 19:49:44.000000 apache-airflow-providers-mysql-5.0.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-mysql-5.0.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    14468 2023-04-21 19:49:45.000000 apache-airflow-providers-mysql-5.0.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12786 2023-04-21 19:49:44.000000 apache-airflow-providers-mysql-5.0.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:49:45.000000 apache-airflow-providers-mysql-5.0.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:49:45.000000 apache-airflow-providers-mysql-5.0.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:49:45.000000 apache-airflow-providers-mysql-5.0.0rc1/airflow/providers/mysql/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-mysql-5.0.0rc1/airflow/providers/mysql/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3727 2023-04-21 19:49:44.000000 apache-airflow-providers-mysql-5.0.0rc1/airflow/providers/mysql/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:49:45.000000 apache-airflow-providers-mysql-5.0.0rc1/airflow/providers/mysql/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-mysql-5.0.0rc1/airflow/providers/mysql/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12081 2023-04-14 10:21:56.000000 apache-airflow-providers-mysql-5.0.0rc1/airflow/providers/mysql/hooks/mysql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:49:45.000000 apache-airflow-providers-mysql-5.0.0rc1/airflow/providers/mysql/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-mysql-5.0.0rc1/airflow/providers/mysql/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2782 2023-02-24 18:43:53.000000 apache-airflow-providers-mysql-5.0.0rc1/airflow/providers/mysql/operators/mysql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:49:45.000000 apache-airflow-providers-mysql-5.0.0rc1/airflow/providers/mysql/transfers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-mysql-5.0.0rc1/airflow/providers/mysql/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3268 2023-02-24 18:43:53.000000 apache-airflow-providers-mysql-5.0.0rc1/airflow/providers/mysql/transfers/presto_to_mysql.py
--rw-r--r--   0 root         (0) root         (0)     3558 2023-02-24 18:43:53.000000 apache-airflow-providers-mysql-5.0.0rc1/airflow/providers/mysql/transfers/s3_to_mysql.py
--rw-r--r--   0 root         (0) root         (0)     3250 2023-02-24 18:43:53.000000 apache-airflow-providers-mysql-5.0.0rc1/airflow/providers/mysql/transfers/trino_to_mysql.py
--rw-r--r--   0 root         (0) root         (0)     6469 2023-02-24 18:43:53.000000 apache-airflow-providers-mysql-5.0.0rc1/airflow/providers/mysql/transfers/vertica_to_mysql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:49:45.000000 apache-airflow-providers-mysql-5.0.0rc1/apache_airflow_providers_mysql.egg-info/
--rw-r--r--   0 root         (0) root         (0)    14468 2023-04-21 19:49:45.000000 apache-airflow-providers-mysql-5.0.0rc1/apache_airflow_providers_mysql.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      955 2023-04-21 19:49:45.000000 apache-airflow-providers-mysql-5.0.0rc1/apache_airflow_providers_mysql.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:49:45.000000 apache-airflow-providers-mysql-5.0.0rc1/apache_airflow_providers_mysql.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      102 2023-04-21 19:49:45.000000 apache-airflow-providers-mysql-5.0.0rc1/apache_airflow_providers_mysql.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:49:45.000000 apache-airflow-providers-mysql-5.0.0rc1/apache_airflow_providers_mysql.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      369 2023-04-21 19:49:45.000000 apache-airflow-providers-mysql-5.0.0rc1/apache_airflow_providers_mysql.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-21 19:49:45.000000 apache-airflow-providers-mysql-5.0.0rc1/apache_airflow_providers_mysql.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5246 2023-04-07 12:28:58.000000 apache-airflow-providers-mysql-5.0.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1891 2023-04-21 19:49:45.000000 apache-airflow-providers-mysql-5.0.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2018 2023-04-21 19:49:44.000000 apache-airflow-providers-mysql-5.0.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:40.000000 apache-airflow-providers-mysql-5.1.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-mysql-5.1.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-05-16 15:54:39.000000 apache-airflow-providers-mysql-5.1.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-mysql-5.1.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    15158 2023-05-16 15:54:40.000000 apache-airflow-providers-mysql-5.1.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    13476 2023-05-16 15:54:39.000000 apache-airflow-providers-mysql-5.1.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:40.000000 apache-airflow-providers-mysql-5.1.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:40.000000 apache-airflow-providers-mysql-5.1.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:40.000000 apache-airflow-providers-mysql-5.1.0rc1/airflow/providers/mysql/
+-rw-r--r--   0 root         (0) root         (0)     1388 2023-05-16 15:39:21.000000 apache-airflow-providers-mysql-5.1.0rc1/airflow/providers/mysql/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3748 2023-05-16 15:54:39.000000 apache-airflow-providers-mysql-5.1.0rc1/airflow/providers/mysql/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:40.000000 apache-airflow-providers-mysql-5.1.0rc1/airflow/providers/mysql/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-mysql-5.1.0rc1/airflow/providers/mysql/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12081 2023-04-14 10:21:56.000000 apache-airflow-providers-mysql-5.1.0rc1/airflow/providers/mysql/hooks/mysql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:40.000000 apache-airflow-providers-mysql-5.1.0rc1/airflow/providers/mysql/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-mysql-5.1.0rc1/airflow/providers/mysql/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2862 2023-05-03 19:47:07.000000 apache-airflow-providers-mysql-5.1.0rc1/airflow/providers/mysql/operators/mysql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:40.000000 apache-airflow-providers-mysql-5.1.0rc1/airflow/providers/mysql/transfers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-mysql-5.1.0rc1/airflow/providers/mysql/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3268 2023-02-24 18:43:53.000000 apache-airflow-providers-mysql-5.1.0rc1/airflow/providers/mysql/transfers/presto_to_mysql.py
+-rw-r--r--   0 root         (0) root         (0)     3558 2023-02-24 18:43:53.000000 apache-airflow-providers-mysql-5.1.0rc1/airflow/providers/mysql/transfers/s3_to_mysql.py
+-rw-r--r--   0 root         (0) root         (0)     3250 2023-02-24 18:43:53.000000 apache-airflow-providers-mysql-5.1.0rc1/airflow/providers/mysql/transfers/trino_to_mysql.py
+-rw-r--r--   0 root         (0) root         (0)     6469 2023-02-24 18:43:53.000000 apache-airflow-providers-mysql-5.1.0rc1/airflow/providers/mysql/transfers/vertica_to_mysql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:40.000000 apache-airflow-providers-mysql-5.1.0rc1/apache_airflow_providers_mysql.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15158 2023-05-16 15:54:40.000000 apache-airflow-providers-mysql-5.1.0rc1/apache_airflow_providers_mysql.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      955 2023-05-16 15:54:40.000000 apache-airflow-providers-mysql-5.1.0rc1/apache_airflow_providers_mysql.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:54:40.000000 apache-airflow-providers-mysql-5.1.0rc1/apache_airflow_providers_mysql.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      102 2023-05-16 15:54:40.000000 apache-airflow-providers-mysql-5.1.0rc1/apache_airflow_providers_mysql.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:54:40.000000 apache-airflow-providers-mysql-5.1.0rc1/apache_airflow_providers_mysql.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      369 2023-05-16 15:54:40.000000 apache-airflow-providers-mysql-5.1.0rc1/apache_airflow_providers_mysql.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-16 15:54:40.000000 apache-airflow-providers-mysql-5.1.0rc1/apache_airflow_providers_mysql.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5308 2023-05-15 09:39:26.000000 apache-airflow-providers-mysql-5.1.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1891 2023-05-16 15:54:40.000000 apache-airflow-providers-mysql-5.1.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2018 2023-05-16 15:54:39.000000 apache-airflow-providers-mysql-5.1.0rc1/setup.py
```

### Comparing `apache-airflow-providers-mysql-5.0.0rc1/LICENSE` & `apache-airflow-providers-mysql-5.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-5.0.0rc1/MANIFEST.in` & `apache-airflow-providers-mysql-5.1.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-5.0.0rc1/PKG-INFO` & `apache-airflow-providers-mysql-5.1.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-mysql
-Version: 5.0.0rc1
+Version: 5.1.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-mysql package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.0.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.1.0/
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -54,28 +54,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-mysql``
 
-Release: ``5.0.0rc1``
+Release: ``5.1.0rc1``
 
 
 `MySQL <https://www.mysql.com/products/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``mysql`` provider. All classes for this provider package
 are in ``airflow.providers.mysql`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.0.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.1.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -85,15 +85,15 @@
 
 Requirements
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
-``apache-airflow``                       ``>=2.3.0``
+``apache-airflow``                       ``>=2.4.0``
 ``apache-airflow-providers-common-sql``  ``>=1.3.1``
 ``mysqlclient``                          ``>=1.3.6``
 =======================================  ==================
 
 Cross provider package dependencies
 -----------------------------------
 
@@ -138,14 +138,30 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+5.1.0
+.....
+
+.. note::
+  This release of provider is only available for Airflow 2.4+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
+
+Misc
+~~~~
+
+* ``Bump minimum Airflow version in providers (#30917)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add full automation for min Airflow version for providers (#30994)``
+
 5.0.0
 .....
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
 .. warning::
@@ -206,16 +222,17 @@
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Prepare for follow-up release for November providers (#27774)``
 
 3.3.0
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
@@ -271,16 +288,17 @@
 
 3.0.0
 .....
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
-* This release of provider is only available for Airflow 2.2+ as explained in the Apache Airflow
-  providers support policy https://github.com/apache/airflow/blob/main/README.md#support-for-providers
+.. note::
+  This release of provider is only available for Airflow 2.2+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Add explanatory note for contributors about updating Changelog (#24229)``
    * ``Migrate MySQL example DAGs to new design #22453 (#24142)``
    * ``Prepare docs for May 2022 provider's release (#24231)``
    * ``Update package description to remove double min-airflow specification (#24292)``
```

### Comparing `apache-airflow-providers-mysql-5.0.0rc1/README.rst` & `apache-airflow-providers-mysql-5.1.0rc1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -15,28 +15,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-mysql``
 
-Release: ``5.0.0rc1``
+Release: ``5.1.0rc1``
 
 
 `MySQL <https://www.mysql.com/products/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``mysql`` provider. All classes for this provider package
 are in ``airflow.providers.mysql`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.0.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.1.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -46,15 +46,15 @@
 
 Requirements
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
-``apache-airflow``                       ``>=2.3.0``
+``apache-airflow``                       ``>=2.4.0``
 ``apache-airflow-providers-common-sql``  ``>=1.3.1``
 ``mysqlclient``                          ``>=1.3.6``
 =======================================  ==================
 
 Cross provider package dependencies
 -----------------------------------
 
@@ -99,14 +99,30 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+5.1.0
+.....
+
+.. note::
+  This release of provider is only available for Airflow 2.4+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
+
+Misc
+~~~~
+
+* ``Bump minimum Airflow version in providers (#30917)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add full automation for min Airflow version for providers (#30994)``
+
 5.0.0
 .....
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
 .. warning::
@@ -167,16 +183,17 @@
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Prepare for follow-up release for November providers (#27774)``
 
 3.3.0
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
@@ -232,16 +249,17 @@
 
 3.0.0
 .....
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
-* This release of provider is only available for Airflow 2.2+ as explained in the Apache Airflow
-  providers support policy https://github.com/apache/airflow/blob/main/README.md#support-for-providers
+.. note::
+  This release of provider is only available for Airflow 2.2+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Add explanatory note for contributors about updating Changelog (#24229)``
    * ``Migrate MySQL example DAGs to new design #22453 (#24142)``
    * ``Prepare docs for May 2022 provider's release (#24231)``
    * ``Update package description to remove double min-airflow specification (#24292)``
```

### Comparing `apache-airflow-providers-mysql-5.0.0rc1/airflow/providers/mysql/__init__.py` & `apache-airflow-providers-mysql-5.1.0rc1/airflow/providers/mysql/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-5.0.0rc1/airflow/providers/mysql/get_provider_info.py` & `apache-airflow-providers-mysql-5.1.0rc1/airflow/providers/mysql/get_provider_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-mysql",
         "name": "MySQL",
         "description": "`MySQL <https://www.mysql.com/products/>`__\n",
         "suspended": False,
         "versions": [
+            "5.1.0",
             "5.0.0",
             "4.0.2",
             "4.0.1",
             "4.0.0",
             "3.4.0",
             "3.3.0",
             "3.2.1",
@@ -48,15 +49,15 @@
             "2.0.0",
             "1.1.0",
             "1.0.2",
             "1.0.1",
             "1.0.0",
         ],
         "dependencies": [
-            "apache-airflow>=2.3.0",
+            "apache-airflow>=2.4.0",
             "apache-airflow-providers-common-sql>=1.3.1",
             "mysqlclient>=1.3.6",
         ],
         "integrations": [
             {
                 "integration-name": "MySQL",
                 "external-doc-url": "https://www.mysql.com/",
```

### Comparing `apache-airflow-providers-mysql-5.0.0rc1/airflow/providers/mysql/hooks/__init__.py` & `apache-airflow-providers-mysql-5.1.0rc1/airflow/providers/mysql/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-5.0.0rc1/airflow/providers/mysql/hooks/mysql.py` & `apache-airflow-providers-mysql-5.1.0rc1/airflow/providers/mysql/hooks/mysql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-5.0.0rc1/airflow/providers/mysql/operators/__init__.py` & `apache-airflow-providers-mysql-5.1.0rc1/airflow/providers/mysql/transfers/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#
 # Licensed to the Apache Software Foundation (ASF) under one
 # or more contributor license agreements.  See the NOTICE file
 # distributed with this work for additional information
 # regarding copyright ownership.  The ASF licenses this file
 # to you under the Apache License, Version 2.0 (the
 # "License"); you may not use this file except in compliance
 # with the License.  You may obtain a copy of the License at
```

### Comparing `apache-airflow-providers-mysql-5.0.0rc1/airflow/providers/mysql/operators/mysql.py` & `apache-airflow-providers-mysql-5.1.0rc1/airflow/providers/mysql/operators/mysql.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
 import warnings
 from typing import Sequence
 
+from airflow.exceptions import AirflowProviderDeprecationWarning
 from airflow.providers.common.sql.operators.sql import SQLExecuteQueryOperator
 
 
 class MySqlOperator(SQLExecuteQueryOperator):
     """
     Executes sql code in a specific MySQL database
 
@@ -60,10 +61,10 @@
             kwargs["hook_params"] = {"schema": database, **hook_params}
 
         super().__init__(conn_id=mysql_conn_id, **kwargs)
         warnings.warn(
             """This class is deprecated.
             Please use `airflow.providers.common.sql.operators.sql.SQLExecuteQueryOperator`.
             Also, you can provide `hook_params={'schema': <database>}`.""",
-            DeprecationWarning,
+            AirflowProviderDeprecationWarning,
             stacklevel=2,
         )
```

### Comparing `apache-airflow-providers-mysql-5.0.0rc1/airflow/providers/mysql/transfers/presto_to_mysql.py` & `apache-airflow-providers-mysql-5.1.0rc1/airflow/providers/mysql/transfers/presto_to_mysql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-5.0.0rc1/airflow/providers/mysql/transfers/s3_to_mysql.py` & `apache-airflow-providers-mysql-5.1.0rc1/airflow/providers/mysql/transfers/s3_to_mysql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-5.0.0rc1/airflow/providers/mysql/transfers/trino_to_mysql.py` & `apache-airflow-providers-mysql-5.1.0rc1/airflow/providers/mysql/transfers/trino_to_mysql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-5.0.0rc1/airflow/providers/mysql/transfers/vertica_to_mysql.py` & `apache-airflow-providers-mysql-5.1.0rc1/airflow/providers/mysql/transfers/vertica_to_mysql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-5.0.0rc1/apache_airflow_providers_mysql.egg-info/PKG-INFO` & `apache-airflow-providers-mysql-5.1.0rc1/apache_airflow_providers_mysql.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-mysql
-Version: 5.0.0rc1
+Version: 5.1.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-mysql package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.0.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.1.0/
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -54,28 +54,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-mysql``
 
-Release: ``5.0.0rc1``
+Release: ``5.1.0rc1``
 
 
 `MySQL <https://www.mysql.com/products/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``mysql`` provider. All classes for this provider package
 are in ``airflow.providers.mysql`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.0.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.1.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -85,15 +85,15 @@
 
 Requirements
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
-``apache-airflow``                       ``>=2.3.0``
+``apache-airflow``                       ``>=2.4.0``
 ``apache-airflow-providers-common-sql``  ``>=1.3.1``
 ``mysqlclient``                          ``>=1.3.6``
 =======================================  ==================
 
 Cross provider package dependencies
 -----------------------------------
 
@@ -138,14 +138,30 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+5.1.0
+.....
+
+.. note::
+  This release of provider is only available for Airflow 2.4+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
+
+Misc
+~~~~
+
+* ``Bump minimum Airflow version in providers (#30917)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add full automation for min Airflow version for providers (#30994)``
+
 5.0.0
 .....
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
 .. warning::
@@ -206,16 +222,17 @@
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Prepare for follow-up release for November providers (#27774)``
 
 3.3.0
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
@@ -271,16 +288,17 @@
 
 3.0.0
 .....
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
-* This release of provider is only available for Airflow 2.2+ as explained in the Apache Airflow
-  providers support policy https://github.com/apache/airflow/blob/main/README.md#support-for-providers
+.. note::
+  This release of provider is only available for Airflow 2.2+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Add explanatory note for contributors about updating Changelog (#24229)``
    * ``Migrate MySQL example DAGs to new design #22453 (#24142)``
    * ``Prepare docs for May 2022 provider's release (#24231)``
    * ``Update package description to remove double min-airflow specification (#24292)``
```

### Comparing `apache-airflow-providers-mysql-5.0.0rc1/apache_airflow_providers_mysql.egg-info/SOURCES.txt` & `apache-airflow-providers-mysql-5.1.0rc1/apache_airflow_providers_mysql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-5.0.0rc1/pyproject.toml` & `apache-airflow-providers-mysql-5.1.0rc1/pyproject.toml`

 * *Files 2% similar despite different names*

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
```

### Comparing `apache-airflow-providers-mysql-5.0.0rc1/setup.cfg` & `apache-airflow-providers-mysql-5.1.0rc1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.0.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.1.0/
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
@@ -43,15 +43,15 @@
 python_requires = ~=3.7
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
 	apache-airflow-providers-common-sql>=1.3.1.dev0
-	apache-airflow>=2.3.0.dev0
+	apache-airflow>=2.4.0.dev0
 	mysqlclient>=1.3.6
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.mysql.get_provider_info:get_provider_info
 
 [files]
```

### Comparing `apache-airflow-providers-mysql-5.0.0rc1/setup.py` & `apache-airflow-providers-mysql-5.1.0rc1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-mysql package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "5.0.0"
+version = "5.1.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-mysql setup."""
     setup(
         version=version,
         extras_require={
```

