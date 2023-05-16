# Comparing `tmp/apache-airflow-providers-dbt-cloud-3.1.1rc1.tar.gz` & `tmp/apache-airflow-providers-dbt-cloud-3.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-dbt-cloud-3.1.1rc1.tar", last modified: Fri Apr 21 19:48:19 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-dbt-cloud-3.2.0rc1.tar", last modified: Tue May 16 15:53:37 2023, max compression
```

## Comparing `apache-airflow-providers-dbt-cloud-3.1.1rc1.tar` & `apache-airflow-providers-dbt-cloud-3.2.0rc1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:19.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-04-21 19:48:17.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     9999 2023-04-21 19:48:19.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8442 2023-04-21 19:48:17.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:19.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:19.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:19.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:19.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2903 2023-04-21 19:48:17.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:19.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24269 2023-03-10 19:31:58.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/hooks/dbt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:19.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12832 2023-02-24 18:43:53.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/operators/dbt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:19.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/sensors/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5341 2023-04-07 12:28:58.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/sensors/dbt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:19.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/triggers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/triggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4841 2023-02-24 18:43:53.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/triggers/dbt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:19.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/apache_airflow_providers_dbt_cloud.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9999 2023-04-21 19:48:19.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/apache_airflow_providers_dbt_cloud.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      933 2023-04-21 19:48:19.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/apache_airflow_providers_dbt_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:48:19.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/apache_airflow_providers_dbt_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      106 2023-04-21 19:48:19.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/apache_airflow_providers_dbt_cloud.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:48:19.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/apache_airflow_providers_dbt_cloud.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      111 2023-04-21 19:48:19.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/apache_airflow_providers_dbt_cloud.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-21 19:48:19.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/apache_airflow_providers_dbt_cloud.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5246 2023-04-07 12:28:58.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1895 2023-04-21 19:48:19.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1697 2023-04-21 19:48:17.000000 apache-airflow-providers-dbt-cloud-3.1.1rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:37.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-05-16 15:53:36.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    10938 2023-05-16 15:53:37.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9381 2023-05-16 15:53:36.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:37.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:37.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:37.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/airflow/providers/dbt/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:37.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/airflow/providers/dbt/cloud/
+-rw-r--r--   0 root         (0) root         (0)     1392 2023-05-16 15:39:21.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/airflow/providers/dbt/cloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2990 2023-05-16 15:53:36.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/airflow/providers/dbt/cloud/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:37.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/airflow/providers/dbt/cloud/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/airflow/providers/dbt/cloud/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24269 2023-03-10 19:31:58.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/airflow/providers/dbt/cloud/hooks/dbt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:37.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/airflow/providers/dbt/cloud/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/airflow/providers/dbt/cloud/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13638 2023-05-16 07:40:59.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/airflow/providers/dbt/cloud/operators/dbt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:37.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/airflow/providers/dbt/cloud/sensors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/airflow/providers/dbt/cloud/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5508 2023-05-03 19:47:07.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/airflow/providers/dbt/cloud/sensors/dbt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:37.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/airflow/providers/dbt/cloud/triggers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/airflow/providers/dbt/cloud/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4839 2023-04-24 21:04:25.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/airflow/providers/dbt/cloud/triggers/dbt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:37.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/apache_airflow_providers_dbt_cloud.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10938 2023-05-16 15:53:37.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/apache_airflow_providers_dbt_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      933 2023-05-16 15:53:37.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/apache_airflow_providers_dbt_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:53:37.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/apache_airflow_providers_dbt_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      106 2023-05-16 15:53:37.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/apache_airflow_providers_dbt_cloud.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:53:37.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/apache_airflow_providers_dbt_cloud.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      111 2023-05-16 15:53:37.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/apache_airflow_providers_dbt_cloud.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-16 15:53:37.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/apache_airflow_providers_dbt_cloud.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5308 2023-05-15 09:39:26.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1895 2023-05-16 15:53:37.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1697 2023-05-16 15:53:36.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/setup.py
```

### Comparing `apache-airflow-providers-dbt-cloud-3.1.1rc1/LICENSE` & `apache-airflow-providers-dbt-cloud-3.2.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.1.1rc1/MANIFEST.in` & `apache-airflow-providers-dbt-cloud-3.2.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.1.1rc1/PKG-INFO` & `apache-airflow-providers-dbt-cloud-3.2.0rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-dbt-cloud
-Version: 3.1.1rc1
+Version: 3.2.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-dbt-cloud package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-dbt-cloud/3.1.1/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-dbt-cloud/3.2.0/
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
 
 
 Package ``apache-airflow-providers-dbt-cloud``
 
-Release: ``3.1.1rc1``
+Release: ``3.2.0rc1``
 
 
 `dbt Cloud <https://www.getdbt.com/product/what-is-dbt/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``dbt.cloud`` provider. All classes for this provider package
 are in ``airflow.providers.dbt.cloud`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-dbt-cloud/3.1.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-dbt-cloud/3.2.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -80,15 +80,15 @@
 
 Requirements
 ------------
 
 =================================  ==================
 PIP package                        Version required
 =================================  ==================
-``apache-airflow``                 ``>=2.3.0``
+``apache-airflow``                 ``>=2.4.0``
 ``apache-airflow-providers-http``
 ``asgiref``
 ``aiohttp``
 =================================  ==================
 
 Cross provider package dependencies
 -----------------------------------
@@ -131,14 +131,34 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.2.0
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
+* ``Optimize deferred execution mode in DbtCloudJobRunSensor (#30968)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add cli cmd to list the provider trigger info (#30822)``
+   * ``Upgrade ruff to 0.0.262 (#30809)``
+
 3.1.1
 .....
 
 Misc
 ~~~~
 
 * ``Merge DbtCloudJobRunAsyncSensor logic to DbtCloudJobRunSensor (#30227)``
@@ -194,16 +214,17 @@
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
 
 2.3.0
 .....
 
-This release of provider is only available for Airflow 2.3+ as explained in the
-`Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/README.md#support-for-providers>`_.
+.. note::
+  This release of provider is only available for Airflow 2.3+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Misc
 ~~~~
 
 * ``Move min airflow version to 2.3.0 for all providers (#27196)``
 
 .. Below changes are excluded from the changelog. Move them to
@@ -245,16 +266,17 @@
 
 2.0.0
 .....
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
-* This release of provider is only available for Airflow 2.2+ as explained in the Apache Airflow
-  providers support policy https://github.com/apache/airflow/blob/main/README.md#support-for-providers
+.. note::
+  This release of provider is only available for Airflow 2.2+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Features
 ~~~~~~~~
 
 * ``Enable dbt Cloud provider to interact with single tenant instances (#24264)``
 
 Bug Fixes
```

### Comparing `apache-airflow-providers-dbt-cloud-3.1.1rc1/README.rst` & `apache-airflow-providers-dbt-cloud-3.2.0rc1/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -15,28 +15,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-dbt-cloud``
 
-Release: ``3.1.1rc1``
+Release: ``3.2.0rc1``
 
 
 `dbt Cloud <https://www.getdbt.com/product/what-is-dbt/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``dbt.cloud`` provider. All classes for this provider package
 are in ``airflow.providers.dbt.cloud`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-dbt-cloud/3.1.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-dbt-cloud/3.2.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -46,15 +46,15 @@
 
 Requirements
 ------------
 
 =================================  ==================
 PIP package                        Version required
 =================================  ==================
-``apache-airflow``                 ``>=2.3.0``
+``apache-airflow``                 ``>=2.4.0``
 ``apache-airflow-providers-http``
 ``asgiref``
 ``aiohttp``
 =================================  ==================
 
 Cross provider package dependencies
 -----------------------------------
@@ -97,14 +97,34 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.2.0
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
+* ``Optimize deferred execution mode in DbtCloudJobRunSensor (#30968)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add cli cmd to list the provider trigger info (#30822)``
+   * ``Upgrade ruff to 0.0.262 (#30809)``
+
 3.1.1
 .....
 
 Misc
 ~~~~
 
 * ``Merge DbtCloudJobRunAsyncSensor logic to DbtCloudJobRunSensor (#30227)``
@@ -160,16 +180,17 @@
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
 
 2.3.0
 .....
 
-This release of provider is only available for Airflow 2.3+ as explained in the
-`Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/README.md#support-for-providers>`_.
+.. note::
+  This release of provider is only available for Airflow 2.3+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Misc
 ~~~~
 
 * ``Move min airflow version to 2.3.0 for all providers (#27196)``
 
 .. Below changes are excluded from the changelog. Move them to
@@ -211,16 +232,17 @@
 
 2.0.0
 .....
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
-* This release of provider is only available for Airflow 2.2+ as explained in the Apache Airflow
-  providers support policy https://github.com/apache/airflow/blob/main/README.md#support-for-providers
+.. note::
+  This release of provider is only available for Airflow 2.2+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Features
 ~~~~~~~~
 
 * ``Enable dbt Cloud provider to interact with single tenant instances (#24264)``
 
 Bug Fixes
```

### Comparing `apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/__init__.py` & `apache-airflow-providers-dbt-cloud-3.2.0rc1/airflow/providers/dbt/cloud/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/get_provider_info.py` & `apache-airflow-providers-dbt-cloud-3.2.0rc1/airflow/providers/dbt/cloud/get_provider_info.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,27 +25,28 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-dbt-cloud",
         "name": "dbt Cloud",
         "description": "`dbt Cloud <https://www.getdbt.com/product/what-is-dbt/>`__\n",
         "suspended": False,
         "versions": [
+            "3.2.0",
             "3.1.1",
             "3.1.0",
             "3.0.0",
             "2.3.1",
             "2.3.0",
             "2.2.0",
             "2.1.0",
             "2.0.1",
             "2.0.0",
             "1.0.2",
             "1.0.1",
         ],
-        "dependencies": ["apache-airflow>=2.3.0", "apache-airflow-providers-http", "asgiref", "aiohttp"],
+        "dependencies": ["apache-airflow>=2.4.0", "apache-airflow-providers-http", "asgiref", "aiohttp"],
         "integrations": [
             {
                 "integration-name": "dbt Cloud",
                 "external-doc-url": "https://docs.getdbt.com/docs/dbt-cloud/cloud-overview",
                 "logo": "/integration-logos/dbt/dbt.png",
                 "how-to-guide": ["/docs/apache-airflow-providers-dbt-cloud/operators.rst"],
                 "tags": ["dbt"],
@@ -57,15 +58,18 @@
         "sensors": [
             {"integration-name": "dbt Cloud", "python-modules": ["airflow.providers.dbt.cloud.sensors.dbt"]}
         ],
         "hooks": [
             {"integration-name": "dbt Cloud", "python-modules": ["airflow.providers.dbt.cloud.hooks.dbt"]}
         ],
         "triggers": [
-            {"integration-name": "dbt Cloud", "python-modules": ["airflow.providers.dbt.cloud.triggers.dbt"]}
+            {
+                "integration-name": "dbt Cloud",
+                "class-names": ["airflow.providers.dbt.cloud.triggers.dbt.DbtCloudRunJobTrigger"],
+            }
         ],
         "connection-types": [
             {
                 "hook-class-name": "airflow.providers.dbt.cloud.hooks.dbt.DbtCloudHook",
                 "connection-type": "dbt_cloud",
             }
         ],
```

### Comparing `apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/hooks/__init__.py` & `apache-airflow-providers-dbt-cloud-3.2.0rc1/airflow/providers/dbt/cloud/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/hooks/dbt.py` & `apache-airflow-providers-dbt-cloud-3.2.0rc1/airflow/providers/dbt/cloud/hooks/dbt.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/operators/__init__.py` & `apache-airflow-providers-dbt-cloud-3.2.0rc1/airflow/providers/dbt/cloud/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/operators/dbt.py` & `apache-airflow-providers-dbt-cloud-3.2.0rc1/airflow/providers/dbt/cloud/operators/dbt.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,20 @@
 import time
 import warnings
 from pathlib import Path
 from typing import TYPE_CHECKING, Any
 
 from airflow.exceptions import AirflowException
 from airflow.models import BaseOperator, BaseOperatorLink, XCom
-from airflow.providers.dbt.cloud.hooks.dbt import DbtCloudHook, DbtCloudJobRunException, DbtCloudJobRunStatus
+from airflow.providers.dbt.cloud.hooks.dbt import (
+    DbtCloudHook,
+    DbtCloudJobRunException,
+    DbtCloudJobRunStatus,
+    JobRunInfo,
+)
 from airflow.providers.dbt.cloud.triggers.dbt import DbtCloudRunJobTrigger
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
 class DbtCloudRunJobOperatorLink(BaseOperatorLink):
@@ -150,34 +155,45 @@
                     self.log.info("Job run %s has completed successfully.", str(self.run_id))
                 else:
                     raise DbtCloudJobRunException(f"Job run {self.run_id} has failed or has been cancelled.")
 
                 return self.run_id
             else:
                 end_time = time.time() + self.timeout
-                self.defer(
-                    timeout=self.execution_timeout,
-                    trigger=DbtCloudRunJobTrigger(
-                        conn_id=self.dbt_cloud_conn_id,
-                        run_id=self.run_id,
-                        end_time=end_time,
-                        account_id=self.account_id,
-                        poll_interval=self.check_interval,
-                    ),
-                    method_name="execute_complete",
-                )
+                job_run_info = JobRunInfo(account_id=self.account_id, run_id=self.run_id)
+                job_run_status = self.hook.get_job_run_status(**job_run_info)
+                if not DbtCloudJobRunStatus.is_terminal(job_run_status):
+                    self.defer(
+                        timeout=self.execution_timeout,
+                        trigger=DbtCloudRunJobTrigger(
+                            conn_id=self.dbt_cloud_conn_id,
+                            run_id=self.run_id,
+                            end_time=end_time,
+                            account_id=self.account_id,
+                            poll_interval=self.check_interval,
+                        ),
+                        method_name="execute_complete",
+                    )
+                elif job_run_status == DbtCloudJobRunStatus.SUCCESS.value:
+                    self.log.info("Job run %s has completed successfully.", str(self.run_id))
+                    return self.run_id
+                elif job_run_status in (
+                    DbtCloudJobRunStatus.CANCELLED.value,
+                    DbtCloudJobRunStatus.ERROR.value,
+                ):
+                    raise DbtCloudJobRunException(f"Job run {self.run_id} has failed or has been cancelled.")
         else:
             if self.deferrable is True:
                 warnings.warn(
                     "Argument `wait_for_termination` is False and `deferrable` is True , hence "
                     "`deferrable` parameter doesn't have any effect",
                 )
             return self.run_id
 
-    def execute_complete(self, context: "Context", event: dict[str, Any]) -> int:
+    def execute_complete(self, context: Context, event: dict[str, Any]) -> int:
         """
         Callback for when the trigger fires - returns immediately.
         Relies on trigger to throw an exception, otherwise it assumes execution was
         successful.
         """
         if event["status"] == "error":
             raise AirflowException(event["message"])
```

### Comparing `apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/sensors/__init__.py` & `apache-airflow-providers-dbt-cloud-3.2.0rc1/airflow/providers/dbt/cloud/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/sensors/dbt.py` & `apache-airflow-providers-dbt-cloud-3.2.0rc1/airflow/providers/dbt/cloud/sensors/dbt.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # under the License.
 from __future__ import annotations
 
 import time
 import warnings
 from typing import TYPE_CHECKING, Any
 
-from airflow import AirflowException
+from airflow.exceptions import AirflowException, AirflowProviderDeprecationWarning
 from airflow.providers.dbt.cloud.hooks.dbt import DbtCloudHook, DbtCloudJobRunException, DbtCloudJobRunStatus
 from airflow.providers.dbt.cloud.triggers.dbt import DbtCloudRunJobTrigger
 from airflow.sensors.base import BaseSensorOperator
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
@@ -58,15 +58,15 @@
             if "poke_interval" not in kwargs:
                 # TODO: Remove once deprecated
                 if "polling_interval" in kwargs:
                     kwargs["poke_interval"] = kwargs["polling_interval"]
                     warnings.warn(
                         "Argument `poll_interval` is deprecated and will be removed "
                         "in a future release.  Please use `poke_interval` instead.",
-                        DeprecationWarning,
+                        AirflowProviderDeprecationWarning,
                         stacklevel=2,
                     )
                 else:
                     kwargs["poke_interval"] = 5
 
                 if "timeout" not in kwargs:
                     kwargs["timeout"] = 60 * 60 * 24 * 7
@@ -95,25 +95,26 @@
         Defers to Trigger class to poll for state of the job run until
         it reaches a failure state or success state
         """
         if not self.deferrable:
             super().execute(context)
         else:
             end_time = time.time() + self.timeout
-            self.defer(
-                timeout=self.execution_timeout,
-                trigger=DbtCloudRunJobTrigger(
-                    run_id=self.run_id,
-                    conn_id=self.dbt_cloud_conn_id,
-                    account_id=self.account_id,
-                    poll_interval=self.poke_interval,
-                    end_time=end_time,
-                ),
-                method_name="execute_complete",
-            )
+            if not self.poke(context=context):
+                self.defer(
+                    timeout=self.execution_timeout,
+                    trigger=DbtCloudRunJobTrigger(
+                        run_id=self.run_id,
+                        conn_id=self.dbt_cloud_conn_id,
+                        account_id=self.account_id,
+                        poll_interval=self.poke_interval,
+                        end_time=end_time,
+                    ),
+                    method_name="execute_complete",
+                )
 
     def execute_complete(self, context: Context, event: dict[str, Any]) -> int:
         """
         Callback for when the trigger fires - returns immediately.
         Relies on trigger to throw an exception, otherwise it assumes execution was
         successful.
         """
@@ -130,11 +131,11 @@
     :class:`airflow.providers.dbt.cloud.sensor.dbt.DbtCloudJobRunSensor`.
     """
 
     def __init__(self, **kwargs: Any) -> None:
         warnings.warn(
             "Class `DbtCloudJobRunAsyncSensor` is deprecated and will be removed in a future release. "
             "Please use `DbtCloudJobRunSensor` and set `deferrable` attribute to `True` instead",
-            DeprecationWarning,
+            AirflowProviderDeprecationWarning,
             stacklevel=2,
         )
         super().__init__(deferrable=True, **kwargs)
```

### Comparing `apache-airflow-providers-dbt-cloud-3.1.1rc1/airflow/providers/dbt/cloud/triggers/dbt.py` & `apache-airflow-providers-dbt-cloud-3.2.0rc1/airflow/providers/dbt/cloud/triggers/dbt.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
                 "account_id": self.account_id,
                 "conn_id": self.conn_id,
                 "end_time": self.end_time,
                 "poll_interval": self.poll_interval,
             },
         )
 
-    async def run(self) -> AsyncIterator["TriggerEvent"]:
+    async def run(self) -> AsyncIterator[TriggerEvent]:
         """Make async connection to Dbt, polls for the pipeline run status"""
         hook = DbtCloudHook(self.conn_id)
         try:
             while await self.is_still_running(hook):
                 if self.end_time < time.time():
                     yield TriggerEvent(
                         {
```

### Comparing `apache-airflow-providers-dbt-cloud-3.1.1rc1/apache_airflow_providers_dbt_cloud.egg-info/PKG-INFO` & `apache-airflow-providers-dbt-cloud-3.2.0rc1/apache_airflow_providers_dbt_cloud.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-dbt-cloud
-Version: 3.1.1rc1
+Version: 3.2.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-dbt-cloud package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-dbt-cloud/3.1.1/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-dbt-cloud/3.2.0/
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
 
 
 Package ``apache-airflow-providers-dbt-cloud``
 
-Release: ``3.1.1rc1``
+Release: ``3.2.0rc1``
 
 
 `dbt Cloud <https://www.getdbt.com/product/what-is-dbt/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``dbt.cloud`` provider. All classes for this provider package
 are in ``airflow.providers.dbt.cloud`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-dbt-cloud/3.1.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-dbt-cloud/3.2.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -80,15 +80,15 @@
 
 Requirements
 ------------
 
 =================================  ==================
 PIP package                        Version required
 =================================  ==================
-``apache-airflow``                 ``>=2.3.0``
+``apache-airflow``                 ``>=2.4.0``
 ``apache-airflow-providers-http``
 ``asgiref``
 ``aiohttp``
 =================================  ==================
 
 Cross provider package dependencies
 -----------------------------------
@@ -131,14 +131,34 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.2.0
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
+* ``Optimize deferred execution mode in DbtCloudJobRunSensor (#30968)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add cli cmd to list the provider trigger info (#30822)``
+   * ``Upgrade ruff to 0.0.262 (#30809)``
+
 3.1.1
 .....
 
 Misc
 ~~~~
 
 * ``Merge DbtCloudJobRunAsyncSensor logic to DbtCloudJobRunSensor (#30227)``
@@ -194,16 +214,17 @@
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
 
 2.3.0
 .....
 
-This release of provider is only available for Airflow 2.3+ as explained in the
-`Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/README.md#support-for-providers>`_.
+.. note::
+  This release of provider is only available for Airflow 2.3+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Misc
 ~~~~
 
 * ``Move min airflow version to 2.3.0 for all providers (#27196)``
 
 .. Below changes are excluded from the changelog. Move them to
@@ -245,16 +266,17 @@
 
 2.0.0
 .....
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
-* This release of provider is only available for Airflow 2.2+ as explained in the Apache Airflow
-  providers support policy https://github.com/apache/airflow/blob/main/README.md#support-for-providers
+.. note::
+  This release of provider is only available for Airflow 2.2+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Features
 ~~~~~~~~
 
 * ``Enable dbt Cloud provider to interact with single tenant instances (#24264)``
 
 Bug Fixes
```

### Comparing `apache-airflow-providers-dbt-cloud-3.1.1rc1/apache_airflow_providers_dbt_cloud.egg-info/SOURCES.txt` & `apache-airflow-providers-dbt-cloud-3.2.0rc1/apache_airflow_providers_dbt_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.1.1rc1/pyproject.toml` & `apache-airflow-providers-dbt-cloud-3.2.0rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-dbt-cloud-3.1.1rc1/setup.cfg` & `apache-airflow-providers-dbt-cloud-3.2.0rc1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-dbt-cloud/3.1.1/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-dbt-cloud/3.2.0/
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
@@ -44,15 +44,15 @@
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
 	aiohttp
 	apache-airflow-providers-http
-	apache-airflow>=2.3.0.dev0
+	apache-airflow>=2.4.0.dev0
 	asgiref
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.dbt.cloud.get_provider_info:get_provider_info
 
 [files]
```

### Comparing `apache-airflow-providers-dbt-cloud-3.1.1rc1/setup.py` & `apache-airflow-providers-dbt-cloud-3.2.0rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-dbt-cloud package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "3.1.1"
+version = "3.2.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-dbt-cloud setup."""
     setup(
         version=version,
         extras_require={"http": ["apache-airflow-providers-http"]},
```

