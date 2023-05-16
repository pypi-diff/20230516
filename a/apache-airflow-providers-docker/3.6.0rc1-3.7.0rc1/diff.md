# Comparing `tmp/apache-airflow-providers-docker-3.6.0rc1.tar.gz` & `tmp/apache-airflow-providers-docker-3.7.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-docker-3.6.0rc1.tar", last modified: Fri Apr 21 19:48:23 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-docker-3.7.0rc1.tar", last modified: Tue May 16 15:53:43 2023, max compression
```

## Comparing `apache-airflow-providers-docker-3.6.0rc1.tar` & `apache-airflow-providers-docker-3.7.0rc1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:23.000000 apache-airflow-providers-docker-3.6.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-docker-3.6.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-04-21 19:48:21.000000 apache-airflow-providers-docker-3.6.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-docker-3.6.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    15898 2023-04-21 19:48:23.000000 apache-airflow-providers-docker-3.6.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    14371 2023-04-21 19:48:21.000000 apache-airflow-providers-docker-3.6.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:22.000000 apache-airflow-providers-docker-3.6.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:22.000000 apache-airflow-providers-docker-3.6.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:23.000000 apache-airflow-providers-docker-3.6.0rc1/airflow/providers/docker/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-docker-3.6.0rc1/airflow/providers/docker/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:23.000000 apache-airflow-providers-docker-3.6.0rc1/airflow/providers/docker/decorators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-docker-3.6.0rc1/airflow/providers/docker/decorators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6805 2023-03-16 20:46:35.000000 apache-airflow-providers-docker-3.6.0rc1/airflow/providers/docker/decorators/docker.py
--rw-r--r--   0 root         (0) root         (0)     3238 2023-04-21 19:48:21.000000 apache-airflow-providers-docker-3.6.0rc1/airflow/providers/docker/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:23.000000 apache-airflow-providers-docker-3.6.0rc1/airflow/providers/docker/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-docker-3.6.0rc1/airflow/providers/docker/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7953 2023-04-14 11:39:41.000000 apache-airflow-providers-docker-3.6.0rc1/airflow/providers/docker/hooks/docker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:23.000000 apache-airflow-providers-docker-3.6.0rc1/airflow/providers/docker/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-docker-3.6.0rc1/airflow/providers/docker/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22633 2023-04-21 10:05:41.000000 apache-airflow-providers-docker-3.6.0rc1/airflow/providers/docker/operators/docker.py
--rw-r--r--   0 root         (0) root         (0)     9635 2023-02-24 18:43:53.000000 apache-airflow-providers-docker-3.6.0rc1/airflow/providers/docker/operators/docker_swarm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:23.000000 apache-airflow-providers-docker-3.6.0rc1/apache_airflow_providers_docker.egg-info/
--rw-r--r--   0 root         (0) root         (0)    15898 2023-04-21 19:48:22.000000 apache-airflow-providers-docker-3.6.0rc1/apache_airflow_providers_docker.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      861 2023-04-21 19:48:22.000000 apache-airflow-providers-docker-3.6.0rc1/apache_airflow_providers_docker.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:48:22.000000 apache-airflow-providers-docker-3.6.0rc1/apache_airflow_providers_docker.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-04-21 19:48:22.000000 apache-airflow-providers-docker-3.6.0rc1/apache_airflow_providers_docker.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:48:22.000000 apache-airflow-providers-docker-3.6.0rc1/apache_airflow_providers_docker.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       63 2023-04-21 19:48:22.000000 apache-airflow-providers-docker-3.6.0rc1/apache_airflow_providers_docker.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-21 19:48:22.000000 apache-airflow-providers-docker-3.6.0rc1/apache_airflow_providers_docker.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5246 2023-04-07 12:28:58.000000 apache-airflow-providers-docker-3.6.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1866 2023-04-21 19:48:23.000000 apache-airflow-providers-docker-3.6.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1638 2023-04-21 19:48:21.000000 apache-airflow-providers-docker-3.6.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:43.000000 apache-airflow-providers-docker-3.7.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-docker-3.7.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-05-16 15:53:42.000000 apache-airflow-providers-docker-3.7.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-docker-3.7.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    16588 2023-05-16 15:53:43.000000 apache-airflow-providers-docker-3.7.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    15061 2023-05-16 15:53:42.000000 apache-airflow-providers-docker-3.7.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:43.000000 apache-airflow-providers-docker-3.7.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:43.000000 apache-airflow-providers-docker-3.7.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:43.000000 apache-airflow-providers-docker-3.7.0rc1/airflow/providers/docker/
+-rw-r--r--   0 root         (0) root         (0)     1389 2023-05-16 15:39:21.000000 apache-airflow-providers-docker-3.7.0rc1/airflow/providers/docker/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:43.000000 apache-airflow-providers-docker-3.7.0rc1/airflow/providers/docker/decorators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-docker-3.7.0rc1/airflow/providers/docker/decorators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6805 2023-03-16 20:46:35.000000 apache-airflow-providers-docker-3.7.0rc1/airflow/providers/docker/decorators/docker.py
+-rw-r--r--   0 root         (0) root         (0)     3259 2023-05-16 15:53:42.000000 apache-airflow-providers-docker-3.7.0rc1/airflow/providers/docker/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:43.000000 apache-airflow-providers-docker-3.7.0rc1/airflow/providers/docker/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-docker-3.7.0rc1/airflow/providers/docker/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7953 2023-04-14 11:39:41.000000 apache-airflow-providers-docker-3.7.0rc1/airflow/providers/docker/hooks/docker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:43.000000 apache-airflow-providers-docker-3.7.0rc1/airflow/providers/docker/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-docker-3.7.0rc1/airflow/providers/docker/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22731 2023-05-03 19:47:07.000000 apache-airflow-providers-docker-3.7.0rc1/airflow/providers/docker/operators/docker.py
+-rw-r--r--   0 root         (0) root         (0)     9635 2023-02-24 18:43:53.000000 apache-airflow-providers-docker-3.7.0rc1/airflow/providers/docker/operators/docker_swarm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:43.000000 apache-airflow-providers-docker-3.7.0rc1/apache_airflow_providers_docker.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    16588 2023-05-16 15:53:43.000000 apache-airflow-providers-docker-3.7.0rc1/apache_airflow_providers_docker.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      861 2023-05-16 15:53:43.000000 apache-airflow-providers-docker-3.7.0rc1/apache_airflow_providers_docker.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:53:43.000000 apache-airflow-providers-docker-3.7.0rc1/apache_airflow_providers_docker.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-05-16 15:53:43.000000 apache-airflow-providers-docker-3.7.0rc1/apache_airflow_providers_docker.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:53:43.000000 apache-airflow-providers-docker-3.7.0rc1/apache_airflow_providers_docker.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       63 2023-05-16 15:53:43.000000 apache-airflow-providers-docker-3.7.0rc1/apache_airflow_providers_docker.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-16 15:53:43.000000 apache-airflow-providers-docker-3.7.0rc1/apache_airflow_providers_docker.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5308 2023-05-15 09:39:26.000000 apache-airflow-providers-docker-3.7.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1866 2023-05-16 15:53:43.000000 apache-airflow-providers-docker-3.7.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1638 2023-05-16 15:53:42.000000 apache-airflow-providers-docker-3.7.0rc1/setup.py
```

### Comparing `apache-airflow-providers-docker-3.6.0rc1/LICENSE` & `apache-airflow-providers-docker-3.7.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-docker-3.6.0rc1/MANIFEST.in` & `apache-airflow-providers-docker-3.7.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-docker-3.6.0rc1/PKG-INFO` & `apache-airflow-providers-docker-3.7.0rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-docker
-Version: 3.6.0rc1
+Version: 3.7.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-docker package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-docker/3.6.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-docker/3.7.0/
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
 
 
 Package ``apache-airflow-providers-docker``
 
-Release: ``3.6.0rc1``
+Release: ``3.7.0rc1``
 
 
 `Docker <https://docs.docker.com/install/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``docker`` provider. All classes for this provider package
 are in ``airflow.providers.docker`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-docker/3.6.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-docker/3.7.0/>`_.
 
 
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
 ``docker``          ``>=5.0.3``
 ``python-dotenv``   ``>=0.21.0``
 ==================  ==================
 
  .. Licensed to the Apache Software Foundation (ASF) under one
     or more contributor license agreements.  See the NOTICE file
     distributed with this work for additional information
@@ -110,14 +110,30 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.7.0
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
 3.6.0
 .....
 
 Features
 ~~~~~~~~
 
 * ``Add multiple exit code handling in skip logic for 'DockerOperator' and 'KubernetesPodOperator' (#30769)``
@@ -169,16 +185,17 @@
 
 * ``add hostname argument to DockerOperator (#27822)``
 * ``Move min airflow version down for Docker Provider to 2.3.0 (#28648)``
 
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
@@ -230,16 +247,17 @@
 
 3.0.0
 .....
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
-* This release of provider is only available for Airflow 2.2+ as explained in the Apache Airflow
-  providers support policy https://github.com/apache/airflow/blob/main/README.md#support-for-providers
+.. note::
+  This release of provider is only available for Airflow 2.2+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Misc
 ~~~~
 
 * ``Remove 'xcom_push' from 'DockerOperator' (#23981)``
 * ``docker new system test (#23167)``
```

### Comparing `apache-airflow-providers-docker-3.6.0rc1/README.rst` & `apache-airflow-providers-docker-3.7.0rc1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -15,28 +15,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-docker``
 
-Release: ``3.6.0rc1``
+Release: ``3.7.0rc1``
 
 
 `Docker <https://docs.docker.com/install/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``docker`` provider. All classes for this provider package
 are in ``airflow.providers.docker`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-docker/3.6.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-docker/3.7.0/>`_.
 
 
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
 ``docker``          ``>=5.0.3``
 ``python-dotenv``   ``>=0.21.0``
 ==================  ==================
 
  .. Licensed to the Apache Software Foundation (ASF) under one
     or more contributor license agreements.  See the NOTICE file
     distributed with this work for additional information
@@ -77,14 +77,30 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.7.0
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
 3.6.0
 .....
 
 Features
 ~~~~~~~~
 
 * ``Add multiple exit code handling in skip logic for 'DockerOperator' and 'KubernetesPodOperator' (#30769)``
@@ -136,16 +152,17 @@
 
 * ``add hostname argument to DockerOperator (#27822)``
 * ``Move min airflow version down for Docker Provider to 2.3.0 (#28648)``
 
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
@@ -197,16 +214,17 @@
 
 3.0.0
 .....
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
-* This release of provider is only available for Airflow 2.2+ as explained in the Apache Airflow
-  providers support policy https://github.com/apache/airflow/blob/main/README.md#support-for-providers
+.. note::
+  This release of provider is only available for Airflow 2.2+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Misc
 ~~~~
 
 * ``Remove 'xcom_push' from 'DockerOperator' (#23981)``
 * ``docker new system test (#23167)``
```

### Comparing `apache-airflow-providers-docker-3.6.0rc1/airflow/providers/docker/__init__.py` & `apache-airflow-providers-docker-3.7.0rc1/airflow/providers/docker/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-docker-3.6.0rc1/airflow/providers/docker/decorators/__init__.py` & `apache-airflow-providers-docker-3.7.0rc1/airflow/providers/docker/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-docker-3.6.0rc1/airflow/providers/docker/decorators/docker.py` & `apache-airflow-providers-docker-3.7.0rc1/airflow/providers/docker/decorators/docker.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-docker-3.6.0rc1/airflow/providers/docker/get_provider_info.py` & `apache-airflow-providers-docker-3.7.0rc1/airflow/providers/docker/get_provider_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-docker",
         "name": "Docker",
         "description": "`Docker <https://docs.docker.com/install/>`__\n",
         "suspended": False,
         "versions": [
+            "3.7.0",
             "3.6.0",
             "3.5.1",
             "3.5.0",
             "3.4.0",
             "3.3.0",
             "3.2.0",
             "3.1.0",
@@ -51,15 +52,15 @@
             "2.0.0",
             "1.2.0",
             "1.1.0",
             "1.0.2",
             "1.0.1",
             "1.0.0",
         ],
-        "dependencies": ["apache-airflow>=2.3.0", "docker>=5.0.3", "python-dotenv>=0.21.0"],
+        "dependencies": ["apache-airflow>=2.4.0", "docker>=5.0.3", "python-dotenv>=0.21.0"],
         "integrations": [
             {
                 "integration-name": "Docker",
                 "external-doc-url": "https://docs.docker.com/",
                 "logo": "/integration-logos/docker/Docker.png",
                 "tags": ["software"],
             },
```

### Comparing `apache-airflow-providers-docker-3.6.0rc1/airflow/providers/docker/hooks/__init__.py` & `apache-airflow-providers-docker-3.7.0rc1/airflow/providers/docker/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-docker-3.6.0rc1/airflow/providers/docker/hooks/docker.py` & `apache-airflow-providers-docker-3.7.0rc1/airflow/providers/docker/hooks/docker.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-docker-3.6.0rc1/airflow/providers/docker/operators/docker.py` & `apache-airflow-providers-docker-3.7.0rc1/airflow/providers/docker/operators/docker.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 from docker.constants import DEFAULT_TIMEOUT_SECONDS
 from docker.errors import APIError
 from docker.types import LogConfig, Mount
 from dotenv import dotenv_values
 
 from airflow.compat.functools import cached_property
-from airflow.exceptions import AirflowException, AirflowSkipException
+from airflow.exceptions import AirflowException, AirflowProviderDeprecationWarning, AirflowSkipException
 from airflow.models import BaseOperator
 from airflow.providers.docker.hooks.docker import DockerHook
 
 if TYPE_CHECKING:
     from docker import APIClient
     from docker.types import DeviceRequest
 
@@ -220,15 +220,15 @@
         **kwargs,
     ) -> None:
         super().__init__(**kwargs)
         self.api_version = api_version
         if type(auto_remove) == bool:
             warnings.warn(
                 "bool value for auto_remove is deprecated, please use 'never', 'success', or 'force' instead",
-                DeprecationWarning,
+                AirflowProviderDeprecationWarning,
                 stacklevel=2,
             )
         if str(auto_remove) == "False":
             self.auto_remove = "never"
         elif str(auto_remove) == "True":
             self.auto_remove = "success"
         elif str(auto_remove) in ("never", "success", "force"):
@@ -276,15 +276,17 @@
         self.timeout = timeout
         self.device_requests = device_requests
         self.log_opts_max_size = log_opts_max_size
         self.log_opts_max_file = log_opts_max_file
         self.ipc_mode = ipc_mode
         if skip_exit_code is not None:
             warnings.warn(
-                "skip_exit_code is deprecated. Please use skip_on_exit_code", DeprecationWarning, stacklevel=2
+                "skip_exit_code is deprecated. Please use skip_on_exit_code",
+                AirflowProviderDeprecationWarning,
+                stacklevel=2,
             )
             skip_on_exit_code = skip_exit_code
 
         self.skip_on_exit_code = (
             skip_on_exit_code
             if isinstance(skip_on_exit_code, Container)
             else [skip_on_exit_code]
```

### Comparing `apache-airflow-providers-docker-3.6.0rc1/airflow/providers/docker/operators/docker_swarm.py` & `apache-airflow-providers-docker-3.7.0rc1/airflow/providers/docker/operators/docker_swarm.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-docker-3.6.0rc1/apache_airflow_providers_docker.egg-info/PKG-INFO` & `apache-airflow-providers-docker-3.7.0rc1/apache_airflow_providers_docker.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-docker
-Version: 3.6.0rc1
+Version: 3.7.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-docker package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-docker/3.6.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-docker/3.7.0/
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
 
 
 Package ``apache-airflow-providers-docker``
 
-Release: ``3.6.0rc1``
+Release: ``3.7.0rc1``
 
 
 `Docker <https://docs.docker.com/install/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``docker`` provider. All classes for this provider package
 are in ``airflow.providers.docker`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-docker/3.6.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-docker/3.7.0/>`_.
 
 
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
 ``docker``          ``>=5.0.3``
 ``python-dotenv``   ``>=0.21.0``
 ==================  ==================
 
  .. Licensed to the Apache Software Foundation (ASF) under one
     or more contributor license agreements.  See the NOTICE file
     distributed with this work for additional information
@@ -110,14 +110,30 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.7.0
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
 3.6.0
 .....
 
 Features
 ~~~~~~~~
 
 * ``Add multiple exit code handling in skip logic for 'DockerOperator' and 'KubernetesPodOperator' (#30769)``
@@ -169,16 +185,17 @@
 
 * ``add hostname argument to DockerOperator (#27822)``
 * ``Move min airflow version down for Docker Provider to 2.3.0 (#28648)``
 
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
@@ -230,16 +247,17 @@
 
 3.0.0
 .....
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
-* This release of provider is only available for Airflow 2.2+ as explained in the Apache Airflow
-  providers support policy https://github.com/apache/airflow/blob/main/README.md#support-for-providers
+.. note::
+  This release of provider is only available for Airflow 2.2+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Misc
 ~~~~
 
 * ``Remove 'xcom_push' from 'DockerOperator' (#23981)``
 * ``docker new system test (#23167)``
```

### Comparing `apache-airflow-providers-docker-3.6.0rc1/apache_airflow_providers_docker.egg-info/SOURCES.txt` & `apache-airflow-providers-docker-3.7.0rc1/apache_airflow_providers_docker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-docker-3.6.0rc1/pyproject.toml` & `apache-airflow-providers-docker-3.7.0rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-docker-3.6.0rc1/setup.cfg` & `apache-airflow-providers-docker-3.7.0rc1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-docker/3.6.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-docker/3.7.0/
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
 	docker>=5.0.3
 	python-dotenv>=0.21.0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.docker.get_provider_info:get_provider_info
```

### Comparing `apache-airflow-providers-docker-3.6.0rc1/setup.py` & `apache-airflow-providers-docker-3.7.0rc1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-docker package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "3.6.0"
+version = "3.7.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-docker setup."""
     setup(
         version=version,
         extras_require={},
```

