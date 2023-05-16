# Comparing `tmp/apache-airflow-providers-apache-spark-4.0.1rc1.tar.gz` & `tmp/apache-airflow-providers-apache-spark-4.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-apache-spark-4.0.1rc1.tar", last modified: Sun Apr  2 05:47:13 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-apache-spark-4.1.0rc1.tar", last modified: Tue May 16 15:53:16 2023, max compression
```

## Comparing `apache-airflow-providers-apache-spark-4.0.1rc1.tar` & `apache-airflow-providers-apache-spark-4.1.0rc1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:13.000000 apache-airflow-providers-apache-spark-4.0.1rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-spark-4.0.1rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1122 2023-04-02 05:47:11.000000 apache-airflow-providers-apache-spark-4.0.1rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-spark-4.0.1rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    10858 2023-04-02 05:47:13.000000 apache-airflow-providers-apache-spark-4.0.1rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9313 2023-04-02 05:47:11.000000 apache-airflow-providers-apache-spark-4.0.1rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:13.000000 apache-airflow-providers-apache-spark-4.0.1rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:13.000000 apache-airflow-providers-apache-spark-4.0.1rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:13.000000 apache-airflow-providers-apache-spark-4.0.1rc1/airflow/providers/apache/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:13.000000 apache-airflow-providers-apache-spark-4.0.1rc1/airflow/providers/apache/spark/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-spark-4.0.1rc1/airflow/providers/apache/spark/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3446 2023-04-02 05:47:11.000000 apache-airflow-providers-apache-spark-4.0.1rc1/airflow/providers/apache/spark/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:13.000000 apache-airflow-providers-apache-spark-4.0.1rc1/airflow/providers/apache/spark/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-spark-4.0.1rc1/airflow/providers/apache/spark/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11382 2023-03-27 08:32:49.000000 apache-airflow-providers-apache-spark-4.0.1rc1/airflow/providers/apache/spark/hooks/spark_jdbc.py
--rw-r--r--   0 root         (0) root         (0)     6750 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-spark-4.0.1rc1/airflow/providers/apache/spark/hooks/spark_jdbc_script.py
--rw-r--r--   0 root         (0) root         (0)     7052 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-spark-4.0.1rc1/airflow/providers/apache/spark/hooks/spark_sql.py
--rw-r--r--   0 root         (0) root         (0)    28715 2023-03-27 08:32:49.000000 apache-airflow-providers-apache-spark-4.0.1rc1/airflow/providers/apache/spark/hooks/spark_submit.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:13.000000 apache-airflow-providers-apache-spark-4.0.1rc1/airflow/providers/apache/spark/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-spark-4.0.1rc1/airflow/providers/apache/spark/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9972 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-spark-4.0.1rc1/airflow/providers/apache/spark/operators/spark_jdbc.py
--rw-r--r--   0 root         (0) root         (0)     4505 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-spark-4.0.1rc1/airflow/providers/apache/spark/operators/spark_sql.py
--rw-r--r--   0 root         (0) root         (0)     8419 2023-03-16 20:46:35.000000 apache-airflow-providers-apache-spark-4.0.1rc1/airflow/providers/apache/spark/operators/spark_submit.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:13.000000 apache-airflow-providers-apache-spark-4.0.1rc1/apache_airflow_providers_apache_spark.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10858 2023-04-02 05:47:13.000000 apache-airflow-providers-apache-spark-4.0.1rc1/apache_airflow_providers_apache_spark.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1074 2023-04-02 05:47:13.000000 apache-airflow-providers-apache-spark-4.0.1rc1/apache_airflow_providers_apache_spark.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-02 05:47:13.000000 apache-airflow-providers-apache-spark-4.0.1rc1/apache_airflow_providers_apache_spark.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      109 2023-04-02 05:47:13.000000 apache-airflow-providers-apache-spark-4.0.1rc1/apache_airflow_providers_apache_spark.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-02 05:47:13.000000 apache-airflow-providers-apache-spark-4.0.1rc1/apache_airflow_providers_apache_spark.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       35 2023-04-02 05:47:13.000000 apache-airflow-providers-apache-spark-4.0.1rc1/apache_airflow_providers_apache_spark.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-02 05:47:13.000000 apache-airflow-providers-apache-spark-4.0.1rc1/apache_airflow_providers_apache_spark.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5393 2023-04-01 16:40:04.000000 apache-airflow-providers-apache-spark-4.0.1rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1873 2023-04-02 05:47:13.000000 apache-airflow-providers-apache-spark-4.0.1rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1510 2023-04-02 05:47:11.000000 apache-airflow-providers-apache-spark-4.0.1rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:16.000000 apache-airflow-providers-apache-spark-4.1.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-spark-4.1.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-05-16 15:53:15.000000 apache-airflow-providers-apache-spark-4.1.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-spark-4.1.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    11601 2023-05-16 15:53:16.000000 apache-airflow-providers-apache-spark-4.1.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10056 2023-05-16 15:53:15.000000 apache-airflow-providers-apache-spark-4.1.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:16.000000 apache-airflow-providers-apache-spark-4.1.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:16.000000 apache-airflow-providers-apache-spark-4.1.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:16.000000 apache-airflow-providers-apache-spark-4.1.0rc1/airflow/providers/apache/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:16.000000 apache-airflow-providers-apache-spark-4.1.0rc1/airflow/providers/apache/spark/
+-rw-r--r--   0 root         (0) root         (0)     1395 2023-05-16 15:39:21.000000 apache-airflow-providers-apache-spark-4.1.0rc1/airflow/providers/apache/spark/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3495 2023-05-16 15:53:15.000000 apache-airflow-providers-apache-spark-4.1.0rc1/airflow/providers/apache/spark/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:16.000000 apache-airflow-providers-apache-spark-4.1.0rc1/airflow/providers/apache/spark/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-spark-4.1.0rc1/airflow/providers/apache/spark/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11382 2023-03-27 08:32:49.000000 apache-airflow-providers-apache-spark-4.1.0rc1/airflow/providers/apache/spark/hooks/spark_jdbc.py
+-rw-r--r--   0 root         (0) root         (0)     6750 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-spark-4.1.0rc1/airflow/providers/apache/spark/hooks/spark_jdbc_script.py
+-rw-r--r--   0 root         (0) root         (0)     7052 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-spark-4.1.0rc1/airflow/providers/apache/spark/hooks/spark_sql.py
+-rw-r--r--   0 root         (0) root         (0)    28715 2023-03-27 08:32:49.000000 apache-airflow-providers-apache-spark-4.1.0rc1/airflow/providers/apache/spark/hooks/spark_submit.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:16.000000 apache-airflow-providers-apache-spark-4.1.0rc1/airflow/providers/apache/spark/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-spark-4.1.0rc1/airflow/providers/apache/spark/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9972 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-spark-4.1.0rc1/airflow/providers/apache/spark/operators/spark_jdbc.py
+-rw-r--r--   0 root         (0) root         (0)     4505 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-spark-4.1.0rc1/airflow/providers/apache/spark/operators/spark_sql.py
+-rw-r--r--   0 root         (0) root         (0)     8419 2023-03-16 20:46:35.000000 apache-airflow-providers-apache-spark-4.1.0rc1/airflow/providers/apache/spark/operators/spark_submit.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:16.000000 apache-airflow-providers-apache-spark-4.1.0rc1/apache_airflow_providers_apache_spark.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11601 2023-05-16 15:53:16.000000 apache-airflow-providers-apache-spark-4.1.0rc1/apache_airflow_providers_apache_spark.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1074 2023-05-16 15:53:16.000000 apache-airflow-providers-apache-spark-4.1.0rc1/apache_airflow_providers_apache_spark.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:53:16.000000 apache-airflow-providers-apache-spark-4.1.0rc1/apache_airflow_providers_apache_spark.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2023-05-16 15:53:16.000000 apache-airflow-providers-apache-spark-4.1.0rc1/apache_airflow_providers_apache_spark.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:53:16.000000 apache-airflow-providers-apache-spark-4.1.0rc1/apache_airflow_providers_apache_spark.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       35 2023-05-16 15:53:16.000000 apache-airflow-providers-apache-spark-4.1.0rc1/apache_airflow_providers_apache_spark.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-16 15:53:16.000000 apache-airflow-providers-apache-spark-4.1.0rc1/apache_airflow_providers_apache_spark.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5308 2023-05-15 09:39:26.000000 apache-airflow-providers-apache-spark-4.1.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1873 2023-05-16 15:53:16.000000 apache-airflow-providers-apache-spark-4.1.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-05-16 15:53:15.000000 apache-airflow-providers-apache-spark-4.1.0rc1/setup.py
```

### Comparing `apache-airflow-providers-apache-spark-4.0.1rc1/LICENSE` & `apache-airflow-providers-apache-spark-4.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-spark-4.0.1rc1/MANIFEST.in` & `apache-airflow-providers-apache-spark-4.1.0rc1/MANIFEST.in`

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

### Comparing `apache-airflow-providers-apache-spark-4.0.1rc1/PKG-INFO` & `apache-airflow-providers-apache-spark-4.1.0rc1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-spark
-Version: 4.0.1rc1
+Version: 4.1.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-spark package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.0.1/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.1.0/
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -48,28 +48,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-spark``
 
-Release: ``4.0.1rc1``
+Release: ``4.1.0rc1``
 
 
 `Apache Spark <https://spark.apache.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.spark`` provider. All classes for this provider package
 are in ``airflow.providers.apache.spark`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.0.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.1.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -79,15 +79,15 @@
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
-``apache-airflow``  ``>=2.3.0``
+``apache-airflow``  ``>=2.4.0``
 ``pyspark``
 ==================  ==================
 
  .. Licensed to the Apache Software Foundation (ASF) under one
     or more contributor license agreements.  See the NOTICE file
     distributed with this work for additional information
     regarding copyright ownership.  The ASF licenses this file
@@ -109,29 +109,47 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+4.1.0
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
+   * ``Add mechanism to suspend providers (#30422)``
+
 4.0.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
 
 * ``Only restrict spark binary passed via extra (#30213)``
 * ``Validate host and schema for Spark JDBC Hook (#30223)``
 * ``Add spark3-submit to list of allowed spark-binary values (#30068)``
 
 4.0.0
 .....
 
-This release of provider is only available for Airflow 2.3+ as explained in the
-`Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/README.md#support-for-providers>`_.
+.. note::
+  This release of provider is only available for Airflow 2.3+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
 The ``spark-binary`` connection extra could be set to any binary, but with 4.0.0 version only two values
 are allowed for it ``spark-submit`` and ``spark2-submit``.
 
@@ -157,16 +175,17 @@
 
 3.0.0
 .....
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
-* This release of provider is only available for Airflow 2.2+ as explained in the Apache Airflow
-  providers support policy https://github.com/apache/airflow/blob/main/README.md#support-for-providers
+.. note::
+  This release of provider is only available for Airflow 2.2+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Bug Fixes
 ~~~~~~~~~
 
 * ``Add typing for airflow/configuration.py (#23716)``
 * ``Fix backwards-compatibility introduced by fixing mypy problems (#24230)``
```

### Comparing `apache-airflow-providers-apache-spark-4.0.1rc1/README.rst` & `apache-airflow-providers-apache-spark-4.1.0rc1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -15,28 +15,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-spark``
 
-Release: ``4.0.1rc1``
+Release: ``4.1.0rc1``
 
 
 `Apache Spark <https://spark.apache.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.spark`` provider. All classes for this provider package
 are in ``airflow.providers.apache.spark`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.0.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.1.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -46,15 +46,15 @@
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
-``apache-airflow``  ``>=2.3.0``
+``apache-airflow``  ``>=2.4.0``
 ``pyspark``
 ==================  ==================
 
  .. Licensed to the Apache Software Foundation (ASF) under one
     or more contributor license agreements.  See the NOTICE file
     distributed with this work for additional information
     regarding copyright ownership.  The ASF licenses this file
@@ -76,29 +76,47 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+4.1.0
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
+   * ``Add mechanism to suspend providers (#30422)``
+
 4.0.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
 
 * ``Only restrict spark binary passed via extra (#30213)``
 * ``Validate host and schema for Spark JDBC Hook (#30223)``
 * ``Add spark3-submit to list of allowed spark-binary values (#30068)``
 
 4.0.0
 .....
 
-This release of provider is only available for Airflow 2.3+ as explained in the
-`Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/README.md#support-for-providers>`_.
+.. note::
+  This release of provider is only available for Airflow 2.3+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
 The ``spark-binary`` connection extra could be set to any binary, but with 4.0.0 version only two values
 are allowed for it ``spark-submit`` and ``spark2-submit``.
 
@@ -124,16 +142,17 @@
 
 3.0.0
 .....
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
-* This release of provider is only available for Airflow 2.2+ as explained in the Apache Airflow
-  providers support policy https://github.com/apache/airflow/blob/main/README.md#support-for-providers
+.. note::
+  This release of provider is only available for Airflow 2.2+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Bug Fixes
 ~~~~~~~~~
 
 * ``Add typing for airflow/configuration.py (#23716)``
 * ``Fix backwards-compatibility introduced by fixing mypy problems (#24230)``
```

### Comparing `apache-airflow-providers-apache-spark-4.0.1rc1/airflow/providers/apache/spark/__init__.py` & `apache-airflow-providers-apache-spark-4.1.0rc1/airflow/providers/apache/spark/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-spark-4.0.1rc1/airflow/providers/apache/spark/get_provider_info.py` & `apache-airflow-providers-apache-spark-4.1.0rc1/airflow/providers/apache/spark/get_provider_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,17 @@
 
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-apache-spark",
         "name": "Apache Spark",
         "description": "`Apache Spark <https://spark.apache.org/>`__\n",
+        "suspended": False,
         "versions": [
+            "4.1.0",
             "4.0.1",
             "4.0.0",
             "3.0.0",
             "2.1.3",
             "2.1.2",
             "2.1.1",
             "2.1.0",
@@ -40,15 +42,15 @@
             "2.0.1",
             "2.0.0",
             "1.0.3",
             "1.0.2",
             "1.0.1",
             "1.0.0",
         ],
-        "dependencies": ["apache-airflow>=2.3.0", "pyspark"],
+        "dependencies": ["apache-airflow>=2.4.0", "pyspark"],
         "integrations": [
             {
                 "integration-name": "Apache Spark",
                 "external-doc-url": "https://spark.apache.org/",
                 "how-to-guide": ["/docs/apache-airflow-providers-apache-spark/operators.rst"],
                 "logo": "/integration-logos/apache/spark.png",
                 "tags": ["apache"],
```

### Comparing `apache-airflow-providers-apache-spark-4.0.1rc1/airflow/providers/apache/spark/hooks/__init__.py` & `apache-airflow-providers-apache-spark-4.1.0rc1/airflow/providers/apache/spark/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-spark-4.0.1rc1/airflow/providers/apache/spark/hooks/spark_jdbc.py` & `apache-airflow-providers-apache-spark-4.1.0rc1/airflow/providers/apache/spark/hooks/spark_jdbc.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-spark-4.0.1rc1/airflow/providers/apache/spark/hooks/spark_jdbc_script.py` & `apache-airflow-providers-apache-spark-4.1.0rc1/airflow/providers/apache/spark/hooks/spark_jdbc_script.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-spark-4.0.1rc1/airflow/providers/apache/spark/hooks/spark_sql.py` & `apache-airflow-providers-apache-spark-4.1.0rc1/airflow/providers/apache/spark/hooks/spark_sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-spark-4.0.1rc1/airflow/providers/apache/spark/hooks/spark_submit.py` & `apache-airflow-providers-apache-spark-4.1.0rc1/airflow/providers/apache/spark/hooks/spark_submit.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-spark-4.0.1rc1/airflow/providers/apache/spark/operators/spark_jdbc.py` & `apache-airflow-providers-apache-spark-4.1.0rc1/airflow/providers/apache/spark/operators/spark_jdbc.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-spark-4.0.1rc1/airflow/providers/apache/spark/operators/spark_sql.py` & `apache-airflow-providers-apache-spark-4.1.0rc1/airflow/providers/apache/spark/operators/spark_sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-spark-4.0.1rc1/airflow/providers/apache/spark/operators/spark_submit.py` & `apache-airflow-providers-apache-spark-4.1.0rc1/airflow/providers/apache/spark/operators/spark_submit.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-spark-4.0.1rc1/apache_airflow_providers_apache_spark.egg-info/PKG-INFO` & `apache-airflow-providers-apache-spark-4.1.0rc1/apache_airflow_providers_apache_spark.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-spark
-Version: 4.0.1rc1
+Version: 4.1.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-spark package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.0.1/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.1.0/
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -48,28 +48,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-spark``
 
-Release: ``4.0.1rc1``
+Release: ``4.1.0rc1``
 
 
 `Apache Spark <https://spark.apache.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.spark`` provider. All classes for this provider package
 are in ``airflow.providers.apache.spark`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.0.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.1.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -79,15 +79,15 @@
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
-``apache-airflow``  ``>=2.3.0``
+``apache-airflow``  ``>=2.4.0``
 ``pyspark``
 ==================  ==================
 
  .. Licensed to the Apache Software Foundation (ASF) under one
     or more contributor license agreements.  See the NOTICE file
     distributed with this work for additional information
     regarding copyright ownership.  The ASF licenses this file
@@ -109,29 +109,47 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+4.1.0
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
+   * ``Add mechanism to suspend providers (#30422)``
+
 4.0.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
 
 * ``Only restrict spark binary passed via extra (#30213)``
 * ``Validate host and schema for Spark JDBC Hook (#30223)``
 * ``Add spark3-submit to list of allowed spark-binary values (#30068)``
 
 4.0.0
 .....
 
-This release of provider is only available for Airflow 2.3+ as explained in the
-`Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/README.md#support-for-providers>`_.
+.. note::
+  This release of provider is only available for Airflow 2.3+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
 The ``spark-binary`` connection extra could be set to any binary, but with 4.0.0 version only two values
 are allowed for it ``spark-submit`` and ``spark2-submit``.
 
@@ -157,16 +175,17 @@
 
 3.0.0
 .....
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
-* This release of provider is only available for Airflow 2.2+ as explained in the Apache Airflow
-  providers support policy https://github.com/apache/airflow/blob/main/README.md#support-for-providers
+.. note::
+  This release of provider is only available for Airflow 2.2+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Bug Fixes
 ~~~~~~~~~
 
 * ``Add typing for airflow/configuration.py (#23716)``
 * ``Fix backwards-compatibility introduced by fixing mypy problems (#24230)``
```

### Comparing `apache-airflow-providers-apache-spark-4.0.1rc1/apache_airflow_providers_apache_spark.egg-info/SOURCES.txt` & `apache-airflow-providers-apache-spark-4.1.0rc1/apache_airflow_providers_apache_spark.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-spark-4.0.1rc1/pyproject.toml` & `apache-airflow-providers-apache-spark-4.1.0rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-apache-spark-4.0.1rc1/setup.cfg` & `apache-airflow-providers-apache-spark-4.1.0rc1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.0.1/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.1.0/
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
@@ -42,15 +42,15 @@
 include_package_data = True
 python_requires = ~=3.7
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
-	apache-airflow>=2.3.0.dev0
+	apache-airflow>=2.4.0.dev0
 	pyspark
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.apache.spark.get_provider_info:get_provider_info
 
 [files]
```

### Comparing `apache-airflow-providers-apache-spark-4.0.1rc1/setup.py` & `apache-airflow-providers-apache-spark-4.1.0rc1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,23 +22,28 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-apache-spark package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "4.0.1"
+version = "4.1.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-apache-spark setup."""
     setup(
         version=version,
         extras_require={},
         packages=find_namespace_packages(
-            include=["airflow.providers.apache.spark", "airflow.providers.apache.spark.*"]
+            include=[
+                "airflow.providers.apache.spark",
+                "airflow.providers.apache.spark.*",
+                "airflow.providers.apache.spark_vendor",
+                "airflow.providers.apache.spark_vendor.*",
+            ],
         ),
     )
 
 
 if __name__ == "__main__":
     do_setup()
```

