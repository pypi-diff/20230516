# Comparing `tmp/apache-airflow-providers-apache-kafka-1.0.0rc1.tar.gz` & `tmp/apache-airflow-providers-apache-kafka-1.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-apache-kafka-1.0.0rc1.tar", last modified: Fri Apr 21 19:48:03 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-apache-kafka-1.1.0rc1.tar", last modified: Tue May 16 15:53:07 2023, max compression
```

## Comparing `apache-airflow-providers-apache-kafka-1.0.0rc1.tar` & `apache-airflow-providers-apache-kafka-1.1.0rc1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:03.000000 apache-airflow-providers-apache-kafka-1.0.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-kafka-1.0.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-04-21 19:48:01.000000 apache-airflow-providers-apache-kafka-1.0.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-kafka-1.0.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     4273 2023-04-21 19:48:03.000000 apache-airflow-providers-apache-kafka-1.0.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2728 2023-04-21 19:48:01.000000 apache-airflow-providers-apache-kafka-1.0.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:02.000000 apache-airflow-providers-apache-kafka-1.0.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:02.000000 apache-airflow-providers-apache-kafka-1.0.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:02.000000 apache-airflow-providers-apache-kafka-1.0.0rc1/airflow/providers/apache/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:02.000000 apache-airflow-providers-apache-kafka-1.0.0rc1/airflow/providers/apache/kafka/
--rw-r--r--   0 root         (0) root         (0)      787 2023-04-21 18:38:06.000000 apache-airflow-providers-apache-kafka-1.0.0rc1/airflow/providers/apache/kafka/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3021 2023-04-21 19:48:01.000000 apache-airflow-providers-apache-kafka-1.0.0rc1/airflow/providers/apache/kafka/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:03.000000 apache-airflow-providers-apache-kafka-1.0.0rc1/airflow/providers/apache/kafka/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-04-21 18:38:06.000000 apache-airflow-providers-apache-kafka-1.0.0rc1/airflow/providers/apache/kafka/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2746 2023-04-21 18:38:06.000000 apache-airflow-providers-apache-kafka-1.0.0rc1/airflow/providers/apache/kafka/hooks/base.py
--rw-r--r--   0 root         (0) root         (0)     2351 2023-04-21 18:38:06.000000 apache-airflow-providers-apache-kafka-1.0.0rc1/airflow/providers/apache/kafka/hooks/client.py
--rw-r--r--   0 root         (0) root         (0)     1676 2023-04-21 18:38:06.000000 apache-airflow-providers-apache-kafka-1.0.0rc1/airflow/providers/apache/kafka/hooks/consume.py
--rw-r--r--   0 root         (0) root         (0)     1549 2023-04-21 18:38:06.000000 apache-airflow-providers-apache-kafka-1.0.0rc1/airflow/providers/apache/kafka/hooks/produce.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:03.000000 apache-airflow-providers-apache-kafka-1.0.0rc1/airflow/providers/apache/kafka/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-04-21 18:38:06.000000 apache-airflow-providers-apache-kafka-1.0.0rc1/airflow/providers/apache/kafka/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8020 2023-04-21 18:38:06.000000 apache-airflow-providers-apache-kafka-1.0.0rc1/airflow/providers/apache/kafka/operators/consume.py
--rw-r--r--   0 root         (0) root         (0)     4950 2023-04-21 18:38:06.000000 apache-airflow-providers-apache-kafka-1.0.0rc1/airflow/providers/apache/kafka/operators/produce.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:03.000000 apache-airflow-providers-apache-kafka-1.0.0rc1/airflow/providers/apache/kafka/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-04-21 18:38:06.000000 apache-airflow-providers-apache-kafka-1.0.0rc1/airflow/providers/apache/kafka/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8272 2023-04-21 18:38:06.000000 apache-airflow-providers-apache-kafka-1.0.0rc1/airflow/providers/apache/kafka/sensors/kafka.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:03.000000 apache-airflow-providers-apache-kafka-1.0.0rc1/airflow/providers/apache/kafka/triggers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-04-21 18:38:06.000000 apache-airflow-providers-apache-kafka-1.0.0rc1/airflow/providers/apache/kafka/triggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4913 2023-04-21 18:38:06.000000 apache-airflow-providers-apache-kafka-1.0.0rc1/airflow/providers/apache/kafka/triggers/await_message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:03.000000 apache-airflow-providers-apache-kafka-1.0.0rc1/apache_airflow_providers_apache_kafka.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4273 2023-04-21 19:48:02.000000 apache-airflow-providers-apache-kafka-1.0.0rc1/apache_airflow_providers_apache_kafka.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1196 2023-04-21 19:48:02.000000 apache-airflow-providers-apache-kafka-1.0.0rc1/apache_airflow_providers_apache_kafka.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:48:02.000000 apache-airflow-providers-apache-kafka-1.0.0rc1/apache_airflow_providers_apache_kafka.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      109 2023-04-21 19:48:02.000000 apache-airflow-providers-apache-kafka-1.0.0rc1/apache_airflow_providers_apache_kafka.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:48:02.000000 apache-airflow-providers-apache-kafka-1.0.0rc1/apache_airflow_providers_apache_kafka.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       58 2023-04-21 19:48:02.000000 apache-airflow-providers-apache-kafka-1.0.0rc1/apache_airflow_providers_apache_kafka.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-21 19:48:02.000000 apache-airflow-providers-apache-kafka-1.0.0rc1/apache_airflow_providers_apache_kafka.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5246 2023-04-07 12:28:58.000000 apache-airflow-providers-apache-kafka-1.0.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1897 2023-04-21 19:48:03.000000 apache-airflow-providers-apache-kafka-1.0.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1674 2023-04-21 19:48:01.000000 apache-airflow-providers-apache-kafka-1.0.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:07.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-05-16 15:53:06.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     4937 2023-05-16 15:53:07.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3392 2023-05-16 15:53:06.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:07.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:07.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:07.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:07.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/kafka/
+-rw-r--r--   0 root         (0) root         (0)     1395 2023-05-16 15:39:21.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/kafka/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3047 2023-05-16 15:53:06.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/kafka/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:07.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/kafka/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-04-21 18:38:06.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/kafka/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2746 2023-04-24 21:04:25.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/kafka/hooks/base.py
+-rw-r--r--   0 root         (0) root         (0)     2351 2023-04-24 21:04:25.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/kafka/hooks/client.py
+-rw-r--r--   0 root         (0) root         (0)     1676 2023-04-21 18:38:06.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/kafka/hooks/consume.py
+-rw-r--r--   0 root         (0) root         (0)     1549 2023-04-21 18:38:06.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/kafka/hooks/produce.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:07.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/kafka/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-04-21 18:38:06.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/kafka/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8020 2023-04-21 18:38:06.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/kafka/operators/consume.py
+-rw-r--r--   0 root         (0) root         (0)     4950 2023-04-21 18:38:06.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/kafka/operators/produce.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:07.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/kafka/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-04-21 18:38:06.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/kafka/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8272 2023-04-21 18:38:06.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/kafka/sensors/kafka.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:07.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/kafka/triggers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-04-21 18:38:06.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/kafka/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4913 2023-04-21 18:38:06.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/kafka/triggers/await_message.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:07.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/apache_airflow_providers_apache_kafka.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4937 2023-05-16 15:53:07.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/apache_airflow_providers_apache_kafka.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1196 2023-05-16 15:53:07.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/apache_airflow_providers_apache_kafka.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:53:07.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/apache_airflow_providers_apache_kafka.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2023-05-16 15:53:07.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/apache_airflow_providers_apache_kafka.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:53:07.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/apache_airflow_providers_apache_kafka.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       58 2023-05-16 15:53:07.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/apache_airflow_providers_apache_kafka.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-16 15:53:07.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/apache_airflow_providers_apache_kafka.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5308 2023-05-15 09:39:26.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1897 2023-05-16 15:53:07.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-05-16 15:53:06.000000 apache-airflow-providers-apache-kafka-1.1.0rc1/setup.py
```

### Comparing `apache-airflow-providers-apache-kafka-1.0.0rc1/LICENSE` & `apache-airflow-providers-apache-kafka-1.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.0.0rc1/MANIFEST.in` & `apache-airflow-providers-apache-kafka-1.1.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.0.0rc1/PKG-INFO` & `apache-airflow-providers-apache-kafka-1.1.0rc1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-kafka
-Version: 1.0.0rc1
+Version: 1.1.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-kafka package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-kafka/1.0.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-kafka/1.1.0/
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
 
 
 Package ``apache-airflow-providers-apache-kafka``
 
-Release: ``1.0.0rc1``
+Release: ``1.1.0rc1``
 
 
 `Apache Kafka  <https://kafka.apache.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.kafka`` provider. All classes for this provider package
 are in ``airflow.providers.apache.kafka`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-kafka/1.0.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-kafka/1.1.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -79,15 +79,15 @@
 
 Requirements
 ------------
 
 ===================  ==================
 PIP package          Version required
 ===================  ==================
-``apache-airflow``   ``>=2.3.0``
+``apache-airflow``   ``>=2.4.0``
 ``asgiref``
 ``confluent-kafka``  ``>=1.8.2``
 ===================  ==================
 
  .. Licensed to the Apache Software Foundation (ASF) under one
     or more contributor license agreements.  See the NOTICE file
     distributed with this work for additional information
@@ -105,11 +105,29 @@
     specific language governing permissions and limitations
     under the License.
 
 
 Changelog
 ---------
 
+1.1.0
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
+   * ``Upgrade ruff to 0.0.262 (#30809)``
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add cli cmd to list the provider trigger info (#30822)``
+
 1.0.0
 .....
 
 Initial version of the provider.
```

### Comparing `apache-airflow-providers-apache-kafka-1.0.0rc1/README.rst` & `apache-airflow-providers-apache-kafka-1.1.0rc1/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -15,28 +15,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-kafka``
 
-Release: ``1.0.0rc1``
+Release: ``1.1.0rc1``
 
 
 `Apache Kafka  <https://kafka.apache.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.kafka`` provider. All classes for this provider package
 are in ``airflow.providers.apache.kafka`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-kafka/1.0.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-kafka/1.1.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -46,15 +46,15 @@
 
 Requirements
 ------------
 
 ===================  ==================
 PIP package          Version required
 ===================  ==================
-``apache-airflow``   ``>=2.3.0``
+``apache-airflow``   ``>=2.4.0``
 ``asgiref``
 ``confluent-kafka``  ``>=1.8.2``
 ===================  ==================
 
  .. Licensed to the Apache Software Foundation (ASF) under one
     or more contributor license agreements.  See the NOTICE file
     distributed with this work for additional information
@@ -72,11 +72,29 @@
     specific language governing permissions and limitations
     under the License.
 
 
 Changelog
 ---------
 
+1.1.0
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
+   * ``Upgrade ruff to 0.0.262 (#30809)``
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add cli cmd to list the provider trigger info (#30822)``
+
 1.0.0
 .....
 
 Initial version of the provider.
```

### Comparing `apache-airflow-providers-apache-kafka-1.0.0rc1/airflow/providers/apache/kafka/__init__.py` & `apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/kafka/hooks/__init__.py`

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

### Comparing `apache-airflow-providers-apache-kafka-1.0.0rc1/airflow/providers/apache/kafka/get_provider_info.py` & `apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/kafka/get_provider_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-apache-kafka",
         "name": "Apache Kafka",
         "suspended": False,
         "description": "`Apache Kafka  <https://kafka.apache.org/>`__\n",
-        "versions": ["1.0.0"],
-        "dependencies": ["apache-airflow>=2.3.0", "asgiref", "confluent-kafka>=1.8.2"],
+        "versions": ["1.1.0", "1.0.0"],
+        "dependencies": ["apache-airflow>=2.4.0", "asgiref", "confluent-kafka>=1.8.2"],
         "integrations": [
             {
                 "integration-name": "Apache Kafka",
                 "external-doc-url": "https://kafka.apache.org/",
                 "logo": "/integration-logos/apache/kafka.svg",
                 "tags": ["apache"],
             }
@@ -63,15 +63,15 @@
                 "integration-name": "Apache Kafka",
                 "python-modules": ["airflow.providers.apache.kafka.sensors.kafka"],
             }
         ],
         "triggers": [
             {
                 "integration-name": "Apache Kafka",
-                "python-modules": ["airflow.providers.apache.kafka.triggers.await_message"],
+                "class-names": ["airflow.providers.apache.kafka.triggers.await_message.AwaitMessageTrigger"],
             }
         ],
         "connection-types": [
             {
                 "hook-class-name": "airflow.providers.apache.kafka.hooks.base.KafkaBaseHook",
                 "connection-type": "kafka",
             }
```

### Comparing `apache-airflow-providers-apache-kafka-1.0.0rc1/airflow/providers/apache/kafka/hooks/__init__.py` & `apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/kafka/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.0.0rc1/airflow/providers/apache/kafka/hooks/base.py` & `apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/kafka/hooks/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         }
 
     def _get_client(self, config):
         raise NotImplementedError
 
     @cached_property
     def get_conn(self) -> Any:
-        """get the configuration object"""
+        """Get the configuration object"""
         config = self.get_connection(self.kafka_config_id).extra_dejson
 
         if not (config.get("bootstrap.servers", None)):
             raise ValueError("config['bootstrap.servers'] must be provided.")
 
         return self._get_client(config)
```

### Comparing `apache-airflow-providers-apache-kafka-1.0.0rc1/airflow/providers/apache/kafka/hooks/client.py` & `apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/kafka/hooks/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     def _get_client(self, config) -> AdminClient:
         return AdminClient(config)
 
     def create_topic(
         self,
         topics: Sequence[Sequence[Any]],
     ) -> None:
-        """creates a topic
+        """Creates a topic
 
         :param topics: a list of topics to create including the number of partitions for the topic
           and the replication factor. Format: [ ("topic_name", number of partitions, replication factor)]
         """
         admin_client = self.get_conn
 
         new_topics = [NewTopic(t[0], num_partitions=t[1], replication_factor=t[2]) for t in topics]
```

### Comparing `apache-airflow-providers-apache-kafka-1.0.0rc1/airflow/providers/apache/kafka/hooks/consume.py` & `apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/kafka/hooks/consume.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.0.0rc1/airflow/providers/apache/kafka/hooks/produce.py` & `apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/kafka/hooks/produce.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.0.0rc1/airflow/providers/apache/kafka/operators/__init__.py` & `apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/kafka/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.0.0rc1/airflow/providers/apache/kafka/operators/consume.py` & `apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/kafka/operators/consume.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.0.0rc1/airflow/providers/apache/kafka/operators/produce.py` & `apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/kafka/operators/produce.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.0.0rc1/airflow/providers/apache/kafka/sensors/__init__.py` & `apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/kafka/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.0.0rc1/airflow/providers/apache/kafka/sensors/kafka.py` & `apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/kafka/sensors/kafka.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.0.0rc1/airflow/providers/apache/kafka/triggers/await_message.py` & `apache-airflow-providers-apache-kafka-1.1.0rc1/airflow/providers/apache/kafka/triggers/await_message.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.0.0rc1/apache_airflow_providers_apache_kafka.egg-info/PKG-INFO` & `apache-airflow-providers-apache-kafka-1.1.0rc1/apache_airflow_providers_apache_kafka.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-kafka
-Version: 1.0.0rc1
+Version: 1.1.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-kafka package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-kafka/1.0.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-kafka/1.1.0/
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
 
 
 Package ``apache-airflow-providers-apache-kafka``
 
-Release: ``1.0.0rc1``
+Release: ``1.1.0rc1``
 
 
 `Apache Kafka  <https://kafka.apache.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.kafka`` provider. All classes for this provider package
 are in ``airflow.providers.apache.kafka`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-kafka/1.0.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-kafka/1.1.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -79,15 +79,15 @@
 
 Requirements
 ------------
 
 ===================  ==================
 PIP package          Version required
 ===================  ==================
-``apache-airflow``   ``>=2.3.0``
+``apache-airflow``   ``>=2.4.0``
 ``asgiref``
 ``confluent-kafka``  ``>=1.8.2``
 ===================  ==================
 
  .. Licensed to the Apache Software Foundation (ASF) under one
     or more contributor license agreements.  See the NOTICE file
     distributed with this work for additional information
@@ -105,11 +105,29 @@
     specific language governing permissions and limitations
     under the License.
 
 
 Changelog
 ---------
 
+1.1.0
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
+   * ``Upgrade ruff to 0.0.262 (#30809)``
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add cli cmd to list the provider trigger info (#30822)``
+
 1.0.0
 .....
 
 Initial version of the provider.
```

### Comparing `apache-airflow-providers-apache-kafka-1.0.0rc1/apache_airflow_providers_apache_kafka.egg-info/SOURCES.txt` & `apache-airflow-providers-apache-kafka-1.1.0rc1/apache_airflow_providers_apache_kafka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.0.0rc1/pyproject.toml` & `apache-airflow-providers-apache-kafka-1.1.0rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-apache-kafka-1.0.0rc1/setup.cfg` & `apache-airflow-providers-apache-kafka-1.1.0rc1/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-apache-kafka/1.0.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-apache-kafka/1.1.0/
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
 	asgiref
 	confluent-kafka>=1.8.2
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.apache.kafka.get_provider_info:get_provider_info
```

### Comparing `apache-airflow-providers-apache-kafka-1.0.0rc1/setup.py` & `apache-airflow-providers-apache-kafka-1.1.0rc1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-apache-kafka package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "1.0.0"
+version = "1.1.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-apache-kafka setup."""
     setup(
         version=version,
         extras_require={},
```

