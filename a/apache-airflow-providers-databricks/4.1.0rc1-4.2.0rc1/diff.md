# Comparing `tmp/apache-airflow-providers-databricks-4.1.0rc1.tar.gz` & `tmp/apache-airflow-providers-databricks-4.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-databricks-4.1.0rc1.tar", last modified: Fri Apr 21 19:48:16 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-databricks-4.2.0rc1.tar", last modified: Tue May 16 15:53:33 2023, max compression
```

## Comparing `apache-airflow-providers-databricks-4.1.0rc1.tar` & `apache-airflow-providers-databricks-4.2.0rc1.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:16.000000 apache-airflow-providers-databricks-4.1.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-databricks-4.1.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-04-21 19:48:14.000000 apache-airflow-providers-databricks-4.1.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-databricks-4.1.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    18787 2023-04-21 19:48:16.000000 apache-airflow-providers-databricks-4.1.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    17221 2023-04-21 19:48:14.000000 apache-airflow-providers-databricks-4.1.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:15.000000 apache-airflow-providers-databricks-4.1.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:15.000000 apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:16.000000 apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5344 2023-04-21 19:48:14.000000 apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:16.000000 apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16105 2023-04-15 10:20:41.000000 apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/hooks/databricks.py
--rw-r--r--   0 root         (0) root         (0)    26704 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/hooks/databricks_base.py
--rw-r--r--   0 root         (0) root         (0)     9278 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/hooks/databricks_sql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:16.000000 apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31391 2023-03-10 19:31:58.000000 apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/operators/databricks.py
--rw-r--r--   0 root         (0) root         (0)    13226 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/operators/databricks_repos.py
--rw-r--r--   0 root         (0) root         (0)    16679 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/operators/databricks_sql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:16.000000 apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-04-13 08:25:21.000000 apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5558 2023-04-13 08:25:21.000000 apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/sensors/databricks_sql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:16.000000 apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/triggers/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/triggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2811 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/triggers/databricks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:16.000000 apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/utils/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2909 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/utils/databricks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:48:16.000000 apache-airflow-providers-databricks-4.1.0rc1/apache_airflow_providers_databricks.egg-info/
--rw-r--r--   0 root         (0) root         (0)    18787 2023-04-21 19:48:15.000000 apache-airflow-providers-databricks-4.1.0rc1/apache_airflow_providers_databricks.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1301 2023-04-21 19:48:15.000000 apache-airflow-providers-databricks-4.1.0rc1/apache_airflow_providers_databricks.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:48:15.000000 apache-airflow-providers-databricks-4.1.0rc1/apache_airflow_providers_databricks.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-04-21 19:48:15.000000 apache-airflow-providers-databricks-4.1.0rc1/apache_airflow_providers_databricks.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:48:15.000000 apache-airflow-providers-databricks-4.1.0rc1/apache_airflow_providers_databricks.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      200 2023-04-21 19:48:15.000000 apache-airflow-providers-databricks-4.1.0rc1/apache_airflow_providers_databricks.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-21 19:48:15.000000 apache-airflow-providers-databricks-4.1.0rc1/apache_airflow_providers_databricks.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5246 2023-04-07 12:28:58.000000 apache-airflow-providers-databricks-4.1.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1981 2023-04-21 19:48:16.000000 apache-airflow-providers-databricks-4.1.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1715 2023-04-21 19:48:14.000000 apache-airflow-providers-databricks-4.1.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:33.000000 apache-airflow-providers-databricks-4.2.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-databricks-4.2.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-05-16 15:53:32.000000 apache-airflow-providers-databricks-4.2.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-databricks-4.2.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    20044 2023-05-16 15:53:33.000000 apache-airflow-providers-databricks-4.2.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    18478 2023-05-16 15:53:32.000000 apache-airflow-providers-databricks-4.2.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:33.000000 apache-airflow-providers-databricks-4.2.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:33.000000 apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:33.000000 apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/
+-rw-r--r--   0 root         (0) root         (0)     1393 2023-05-16 15:39:21.000000 apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5547 2023-05-16 15:53:32.000000 apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:33.000000 apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16761 2023-05-12 08:38:07.000000 apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/hooks/databricks.py
+-rw-r--r--   0 root         (0) root         (0)    26704 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/hooks/databricks_base.py
+-rw-r--r--   0 root         (0) root         (0)     9278 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/hooks/databricks_sql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:33.000000 apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33394 2023-05-04 19:17:30.000000 apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/operators/databricks.py
+-rw-r--r--   0 root         (0) root         (0)    13226 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/operators/databricks_repos.py
+-rw-r--r--   0 root         (0) root         (0)    16793 2023-05-12 08:38:07.000000 apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/operators/databricks_sql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:33.000000 apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-04-13 08:25:21.000000 apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10015 2023-05-15 07:14:11.000000 apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/sensors/databricks_partition.py
+-rw-r--r--   0 root         (0) root         (0)     5558 2023-04-13 08:25:21.000000 apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/sensors/databricks_sql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:33.000000 apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/triggers/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3997 2023-04-24 21:04:25.000000 apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/triggers/databricks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:33.000000 apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/utils/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2909 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/utils/databricks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:33.000000 apache-airflow-providers-databricks-4.2.0rc1/apache_airflow_providers_databricks.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    20044 2023-05-16 15:53:33.000000 apache-airflow-providers-databricks-4.2.0rc1/apache_airflow_providers_databricks.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1362 2023-05-16 15:53:33.000000 apache-airflow-providers-databricks-4.2.0rc1/apache_airflow_providers_databricks.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:53:33.000000 apache-airflow-providers-databricks-4.2.0rc1/apache_airflow_providers_databricks.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-05-16 15:53:33.000000 apache-airflow-providers-databricks-4.2.0rc1/apache_airflow_providers_databricks.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:53:33.000000 apache-airflow-providers-databricks-4.2.0rc1/apache_airflow_providers_databricks.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      200 2023-05-16 15:53:33.000000 apache-airflow-providers-databricks-4.2.0rc1/apache_airflow_providers_databricks.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-16 15:53:33.000000 apache-airflow-providers-databricks-4.2.0rc1/apache_airflow_providers_databricks.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5308 2023-05-15 09:39:26.000000 apache-airflow-providers-databricks-4.2.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1981 2023-05-16 15:53:33.000000 apache-airflow-providers-databricks-4.2.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1715 2023-05-16 15:53:32.000000 apache-airflow-providers-databricks-4.2.0rc1/setup.py
```

### Comparing `apache-airflow-providers-databricks-4.1.0rc1/LICENSE` & `apache-airflow-providers-databricks-4.2.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.1.0rc1/MANIFEST.in` & `apache-airflow-providers-databricks-4.2.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.1.0rc1/PKG-INFO` & `apache-airflow-providers-databricks-4.2.0rc1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-databricks
-Version: 4.1.0rc1
+Version: 4.2.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-databricks package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.1.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.2.0/
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
 
 
 Package ``apache-airflow-providers-databricks``
 
-Release: ``4.1.0rc1``
+Release: ``4.2.0rc1``
 
 
 `Databricks <https://databricks.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``databricks`` provider. All classes for this provider package
 are in ``airflow.providers.databricks`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.1.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.2.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -80,16 +80,16 @@
 
 Requirements
 ------------
 
 =======================================  ===================
 PIP package                              Version required
 =======================================  ===================
-``apache-airflow``                       ``>=2.3.0``
-``apache-airflow-providers-common-sql``  ``>=1.3.1``
+``apache-airflow``                       ``>=2.4.0``
+``apache-airflow-providers-common-sql``  ``>=1.5.0``
 ``requests``                             ``>=2.27,<3``
 ``databricks-sql-connector``             ``>=2.0.0, <3.0.0``
 ``aiohttp``                              ``>=3.6.3, <4``
 =======================================  ===================
 
 Cross provider package dependencies
 -----------------------------------
@@ -132,14 +132,43 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+4.2.0
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
+* ``Add cancel all runs functionality to Databricks hook (#31038)``
+* ``Add retry param in databrics async operator (#30744)``
+* ``Add repair job functionality to databricks hook (#30786)``
+* ``Add 'DatabricksPartitionSensor' (#30980)``
+
+Misc
+~~~~
+
+* ``Bump minimum Airflow version in providers (#30917)``
+* ``Deprecate databricks async operator (#30761)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Move TaskInstanceKey to a separate file (#31033)``
+   * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add cli cmd to list the provider trigger info (#30822)``
+
 4.1.0
 .....
 
 Features
 ~~~~~~~~
 
 * ``Add delete inactive run functionality to databricks provider (#30646)``
@@ -199,16 +228,17 @@
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Prepare for follow-up release for November providers (#27774)``
 
 3.4.0
 .....
 
-This release of provider is only available for Airflow 2.3+ as explained in the
-`Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/README.md#support-for-providers>`_.
+.. note::
+  This release of provider is only available for Airflow 2.3+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Misc
 ~~~~
 
 * ``Move min airflow version to 2.3.0 for all providers (#27196)``
 * ``Replace urlparse with urlsplit (#27389)``
 
@@ -296,16 +326,17 @@
 
 3.0.0
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
 
 * ``Add Deferrable Databricks operators (#19736)``
 * ``Add git_source to DatabricksSubmitRunOperator (#23620)``
```

### Comparing `apache-airflow-providers-databricks-4.1.0rc1/README.rst` & `apache-airflow-providers-databricks-4.2.0rc1/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -15,28 +15,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-databricks``
 
-Release: ``4.1.0rc1``
+Release: ``4.2.0rc1``
 
 
 `Databricks <https://databricks.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``databricks`` provider. All classes for this provider package
 are in ``airflow.providers.databricks`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.1.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.2.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -46,16 +46,16 @@
 
 Requirements
 ------------
 
 =======================================  ===================
 PIP package                              Version required
 =======================================  ===================
-``apache-airflow``                       ``>=2.3.0``
-``apache-airflow-providers-common-sql``  ``>=1.3.1``
+``apache-airflow``                       ``>=2.4.0``
+``apache-airflow-providers-common-sql``  ``>=1.5.0``
 ``requests``                             ``>=2.27,<3``
 ``databricks-sql-connector``             ``>=2.0.0, <3.0.0``
 ``aiohttp``                              ``>=3.6.3, <4``
 =======================================  ===================
 
 Cross provider package dependencies
 -----------------------------------
@@ -98,14 +98,43 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+4.2.0
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
+* ``Add cancel all runs functionality to Databricks hook (#31038)``
+* ``Add retry param in databrics async operator (#30744)``
+* ``Add repair job functionality to databricks hook (#30786)``
+* ``Add 'DatabricksPartitionSensor' (#30980)``
+
+Misc
+~~~~
+
+* ``Bump minimum Airflow version in providers (#30917)``
+* ``Deprecate databricks async operator (#30761)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Move TaskInstanceKey to a separate file (#31033)``
+   * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add cli cmd to list the provider trigger info (#30822)``
+
 4.1.0
 .....
 
 Features
 ~~~~~~~~
 
 * ``Add delete inactive run functionality to databricks provider (#30646)``
@@ -165,16 +194,17 @@
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Prepare for follow-up release for November providers (#27774)``
 
 3.4.0
 .....
 
-This release of provider is only available for Airflow 2.3+ as explained in the
-`Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/README.md#support-for-providers>`_.
+.. note::
+  This release of provider is only available for Airflow 2.3+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Misc
 ~~~~
 
 * ``Move min airflow version to 2.3.0 for all providers (#27196)``
 * ``Replace urlparse with urlsplit (#27389)``
 
@@ -262,16 +292,17 @@
 
 3.0.0
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
 
 * ``Add Deferrable Databricks operators (#19736)``
 * ``Add git_source to DatabricksSubmitRunOperator (#23620)``
```

### Comparing `apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/__init__.py` & `apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/get_provider_info.py` & `apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/get_provider_info.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-databricks",
         "name": "Databricks",
         "description": "`Databricks <https://databricks.com/>`__\n",
         "suspended": False,
         "versions": [
+            "4.2.0",
             "4.1.0",
             "4.0.1",
             "4.0.0",
             "3.4.0",
             "3.3.0",
             "3.2.0",
             "3.1.0",
@@ -47,16 +48,16 @@
             "2.0.2",
             "2.0.1",
             "2.0.0",
             "1.0.1",
             "1.0.0",
         ],
         "dependencies": [
-            "apache-airflow>=2.3.0",
-            "apache-airflow-providers-common-sql>=1.3.1",
+            "apache-airflow>=2.4.0",
+            "apache-airflow-providers-common-sql>=1.5.0",
             "requests>=2.27,<3",
             "databricks-sql-connector>=2.0.0, <3.0.0",
             "aiohttp>=3.6.3, <4",
         ],
         "integrations": [
             {
                 "integration-name": "Databricks",
@@ -116,21 +117,26 @@
                 "integration-name": "Databricks SQL",
                 "python-modules": ["airflow.providers.databricks.hooks.databricks_sql"],
             },
         ],
         "triggers": [
             {
                 "integration-name": "Databricks",
-                "python-modules": ["airflow.providers.databricks.triggers.databricks"],
+                "class-names": [
+                    "airflow.providers.databricks.triggers.databricks.DatabricksExecutionTrigger"
+                ],
             }
         ],
         "sensors": [
             {
                 "integration-name": "Databricks",
-                "python-modules": ["airflow.providers.databricks.sensors.databricks_sql"],
+                "python-modules": [
+                    "airflow.providers.databricks.sensors.databricks_sql",
+                    "airflow.providers.databricks.sensors.databricks_partition",
+                ],
             }
         ],
         "connection-types": [
             {
                 "hook-class-name": "airflow.providers.databricks.hooks.databricks.DatabricksHook",
                 "connection-type": "databricks",
             }
```

### Comparing `apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/hooks/__init__.py` & `apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/hooks/databricks.py` & `apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/hooks/databricks.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,17 @@
 TERMINATE_CLUSTER_ENDPOINT = ("POST", "api/2.0/clusters/delete")
 
 RUN_NOW_ENDPOINT = ("POST", "api/2.1/jobs/run-now")
 SUBMIT_RUN_ENDPOINT = ("POST", "api/2.1/jobs/runs/submit")
 GET_RUN_ENDPOINT = ("GET", "api/2.1/jobs/runs/get")
 CANCEL_RUN_ENDPOINT = ("POST", "api/2.1/jobs/runs/cancel")
 DELETE_RUN_ENDPOINT = ("POST", "api/2.1/jobs/runs/delete")
+REPAIR_RUN_ENDPOINT = ("POST", "api/2.1/jobs/runs/repair")
 OUTPUT_RUNS_JOB_ENDPOINT = ("GET", "api/2.1/jobs/runs/get-output")
+CANCEL_ALL_RUNS_ENDPOINT = ("POST", "api/2.1/jobs/runs/cancel-all")
 
 INSTALL_LIBS_ENDPOINT = ("POST", "api/2.0/libraries/install")
 UNINSTALL_LIBS_ENDPOINT = ("POST", "api/2.0/libraries/uninstall")
 
 LIST_JOBS_ENDPOINT = ("GET", "api/2.1/jobs/list")
 
 WORKSPACE_GET_STATUS_ENDPOINT = ("GET", "api/2.0/workspace/get-status")
@@ -348,23 +350,40 @@
         Cancels the run.
 
         :param run_id: id of the run
         """
         json = {"run_id": run_id}
         self._do_api_call(CANCEL_RUN_ENDPOINT, json)
 
+    def cancel_all_runs(self, job_id: int) -> None:
+        """
+        Cancels all active runs of a job. The runs are canceled asynchronously.
+
+        :param job_id: The canonical identifier of the job to cancel all runs of
+        """
+        json = {"job_id": job_id}
+        self._do_api_call(CANCEL_ALL_RUNS_ENDPOINT, json)
+
     def delete_run(self, run_id: int) -> None:
         """
         Deletes a non-active run.
 
         :param run_id: id of the run
         """
         json = {"run_id": run_id}
         self._do_api_call(DELETE_RUN_ENDPOINT, json)
 
+    def repair_run(self, json: dict) -> None:
+        """
+        Re-run one or more tasks.
+
+        :param json: repair a job run.
+        """
+        self._do_api_call(REPAIR_RUN_ENDPOINT, json)
+
     def restart_cluster(self, json: dict) -> None:
         """
         Restarts the cluster.
 
         :param json: json dictionary containing cluster specification.
         """
         self._do_api_call(RESTART_CLUSTER_ENDPOINT, json)
```

### Comparing `apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/hooks/databricks_base.py` & `apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/hooks/databricks_base.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/hooks/databricks_sql.py` & `apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/hooks/databricks_sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/operators/__init__.py` & `apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/operators/databricks.py` & `apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/operators/databricks.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,30 +15,32 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 """This module contains Databricks operators."""
 from __future__ import annotations
 
 import time
+import warnings
 from logging import Logger
 from typing import TYPE_CHECKING, Any, Sequence
 
 from airflow.compat.functools import cached_property
-from airflow.exceptions import AirflowException
+from airflow.exceptions import AirflowException, AirflowProviderDeprecationWarning
 from airflow.models import BaseOperator, BaseOperatorLink, XCom
 from airflow.providers.databricks.hooks.databricks import DatabricksHook, RunState
 from airflow.providers.databricks.triggers.databricks import DatabricksExecutionTrigger
 from airflow.providers.databricks.utils.databricks import normalise_json_content, validate_trigger_event
 
 if TYPE_CHECKING:
-    from airflow.models.taskinstance import TaskInstanceKey
+    from airflow.models.taskinstancekey import TaskInstanceKey
     from airflow.utils.context import Context
 
 DEFER_METHOD_NAME = "execute_complete"
 XCOM_RUN_ID_KEY = "run_id"
+XCOM_JOB_ID_KEY = "job_id"
 XCOM_RUN_PAGE_URL_KEY = "run_page_url"
 
 
 def _handle_databricks_operator_execution(operator, hook, log, context) -> None:
     """
     Handles the Airflow + Databricks lifecycle logic for a Databricks operator
 
@@ -99,14 +101,17 @@
 def _handle_deferrable_databricks_operator_execution(operator, hook, log, context) -> None:
     """
     Handles the Airflow + Databricks lifecycle logic for deferrable Databricks operators
 
     :param operator: Databricks async operator being handled
     :param context: Airflow context
     """
+    job_id = hook.get_job_id(operator.run_id)
+    if operator.do_xcom_push and context is not None:
+        context["ti"].xcom_push(key=XCOM_JOB_ID_KEY, value=job_id)
     if operator.do_xcom_push and context is not None:
         context["ti"].xcom_push(key=XCOM_RUN_ID_KEY, value=operator.run_id)
     log.info("Run submitted with run_id: %s", operator.run_id)
 
     run_page_url = hook.get_run_page_url(operator.run_id)
     if operator.do_xcom_push and context is not None:
         context["ti"].xcom_push(key=XCOM_RUN_PAGE_URL_KEY, value=run_page_url)
@@ -114,14 +119,18 @@
 
     if operator.wait_for_termination:
         operator.defer(
             trigger=DatabricksExecutionTrigger(
                 run_id=operator.run_id,
                 databricks_conn_id=operator.databricks_conn_id,
                 polling_period_seconds=operator.polling_period_seconds,
+                retry_limit=operator.databricks_retry_limit,
+                retry_delay=operator.databricks_retry_delay,
+                retry_args=operator.databricks_retry_args,
+                run_page_url=run_page_url,
             ),
             method_name=DEFER_METHOD_NAME,
         )
 
 
 def _handle_deferrable_databricks_operator_completion(event: dict, log: Logger) -> None:
     validate_trigger_event(event)
@@ -263,14 +272,15 @@
         unreachable. Its value must be greater than or equal to 1.
     :param databricks_retry_delay: Number of seconds to wait between retries (it
             might be a floating point number).
     :param databricks_retry_args: An optional dictionary with arguments passed to ``tenacity.Retrying`` class.
     :param do_xcom_push: Whether we should push run_id and run_page_url to xcom.
     :param git_source: Optional specification of a remote git repository from which
         supported task types are retrieved.
+    :param deferrable: Run operator in the deferrable mode.
 
         .. seealso::
             https://docs.databricks.com/dev-tools/api/latest/jobs.html#operation/JobsRunsSubmit
     """
 
     # Used in airflow.models.BaseOperator
     template_fields: Sequence[str] = ("json", "databricks_conn_id")
@@ -302,25 +312,27 @@
         databricks_retry_delay: int = 1,
         databricks_retry_args: dict[Any, Any] | None = None,
         do_xcom_push: bool = True,
         idempotency_token: str | None = None,
         access_control_list: list[dict[str, str]] | None = None,
         wait_for_termination: bool = True,
         git_source: dict[str, str] | None = None,
+        deferrable: bool = False,
         **kwargs,
     ) -> None:
         """Creates a new ``DatabricksSubmitRunOperator``."""
         super().__init__(**kwargs)
         self.json = json or {}
         self.databricks_conn_id = databricks_conn_id
         self.polling_period_seconds = polling_period_seconds
         self.databricks_retry_limit = databricks_retry_limit
         self.databricks_retry_delay = databricks_retry_delay
         self.databricks_retry_args = databricks_retry_args
         self.wait_for_termination = wait_for_termination
+        self.deferrable = deferrable
         if tasks is not None:
             self.json["tasks"] = tasks
         if spark_jar_task is not None:
             self.json["spark_jar_task"] = spark_jar_task
         if notebook_task is not None:
             self.json["notebook_task"] = notebook_task
         if spark_python_task is not None:
@@ -369,29 +381,45 @@
             retry_args=self.databricks_retry_args,
             caller=caller,
         )
 
     def execute(self, context: Context):
         json_normalised = normalise_json_content(self.json)
         self.run_id = self._hook.submit_run(json_normalised)
-        _handle_databricks_operator_execution(self, self._hook, self.log, context)
+        if self.deferrable:
+            _handle_deferrable_databricks_operator_execution(self, self._hook, self.log, context)
+        else:
+            _handle_databricks_operator_execution(self, self._hook, self.log, context)
 
     def on_kill(self):
         if self.run_id:
             self._hook.cancel_run(self.run_id)
             self.log.info(
                 "Task: %s with run_id: %s was requested to be cancelled.", self.task_id, self.run_id
             )
         else:
             self.log.error("Error: Task: %s with invalid run_id was requested to be cancelled.", self.task_id)
 
+    def execute_complete(self, context: dict | None, event: dict):
+        _handle_deferrable_databricks_operator_completion(event, self.log)
+
 
 class DatabricksSubmitRunDeferrableOperator(DatabricksSubmitRunOperator):
     """Deferrable version of ``DatabricksSubmitRunOperator``"""
 
+    def __init__(self, *args, **kwargs):
+        warnings.warn(
+            "`DatabricksSubmitRunDeferrableOperator` has been deprecated. "
+            "Please use `airflow.providers.databricks.operators.DatabricksSubmitRunOperator` with "
+            "`deferrable=True` instead.",
+            AirflowProviderDeprecationWarning,
+            stacklevel=2,
+        )
+        super().__init__(deferrable=True, *args, **kwargs)
+
     def execute(self, context):
         hook = self._get_hook(caller="DatabricksSubmitRunDeferrableOperator")
         json_normalised = normalise_json_content(self.json)
         self.run_id = hook.submit_run(json_normalised)
         _handle_deferrable_databricks_operator_execution(self, hook, self.log, context)
 
     def execute_complete(self, context: dict | None, event: dict):
@@ -545,14 +573,15 @@
     :param databricks_retry_limit: Amount of times retry if the Databricks backend is
         unreachable. Its value must be greater than or equal to 1.
     :param databricks_retry_delay: Number of seconds to wait between retries (it
             might be a floating point number).
     :param databricks_retry_args: An optional dictionary with arguments passed to ``tenacity.Retrying`` class.
     :param do_xcom_push: Whether we should push run_id and run_page_url to xcom.
     :param wait_for_termination: if we should wait for termination of the job run. ``True`` by default.
+    :param deferrable: Run operator in the deferrable mode.
     """
 
     # Used in airflow.models.BaseOperator
     template_fields: Sequence[str] = ("json", "databricks_conn_id")
     template_ext: Sequence[str] = (".json-tpl",)
     # Databricks brand color (blue) under white text
     ui_color = "#1CB1C2"
@@ -574,25 +603,27 @@
         databricks_conn_id: str = "databricks_default",
         polling_period_seconds: int = 30,
         databricks_retry_limit: int = 3,
         databricks_retry_delay: int = 1,
         databricks_retry_args: dict[Any, Any] | None = None,
         do_xcom_push: bool = True,
         wait_for_termination: bool = True,
+        deferrable: bool = False,
         **kwargs,
     ) -> None:
         """Creates a new ``DatabricksRunNowOperator``."""
         super().__init__(**kwargs)
         self.json = json or {}
         self.databricks_conn_id = databricks_conn_id
         self.polling_period_seconds = polling_period_seconds
         self.databricks_retry_limit = databricks_retry_limit
         self.databricks_retry_delay = databricks_retry_delay
         self.databricks_retry_args = databricks_retry_args
         self.wait_for_termination = wait_for_termination
+        self.deferrable = deferrable
 
         if job_id is not None:
             self.json["job_id"] = job_id
         if job_name is not None:
             self.json["job_name"] = job_name
         if "job_id" in self.json and "job_name" in self.json:
             raise AirflowException("Argument 'job_name' is not allowed with argument 'job_id'")
@@ -632,29 +663,42 @@
         if "job_name" in self.json:
             job_id = hook.find_job_id_by_name(self.json["job_name"])
             if job_id is None:
                 raise AirflowException(f"Job ID for job name {self.json['job_name']} can not be found")
             self.json["job_id"] = job_id
             del self.json["job_name"]
         self.run_id = hook.run_now(self.json)
-        _handle_databricks_operator_execution(self, hook, self.log, context)
+        if self.deferrable:
+            _handle_deferrable_databricks_operator_execution(self, hook, self.log, context)
+        else:
+            _handle_databricks_operator_execution(self, hook, self.log, context)
 
     def on_kill(self):
         if self.run_id:
             self._hook.cancel_run(self.run_id)
             self.log.info(
                 "Task: %s with run_id: %s was requested to be cancelled.", self.task_id, self.run_id
             )
         else:
             self.log.error("Error: Task: %s with invalid run_id was requested to be cancelled.", self.task_id)
 
 
 class DatabricksRunNowDeferrableOperator(DatabricksRunNowOperator):
     """Deferrable version of ``DatabricksRunNowOperator``"""
 
+    def __init__(self, *args, **kwargs):
+        warnings.warn(
+            "`DatabricksRunNowDeferrableOperator` has been deprecated. "
+            "Please use `airflow.providers.databricks.operators.DatabricksRunNowOperator` with "
+            "`deferrable=True` instead.",
+            AirflowProviderDeprecationWarning,
+            stacklevel=2,
+        )
+        super().__init__(deferrable=True, *args, **kwargs)
+
     def execute(self, context):
         hook = self._get_hook(caller="DatabricksRunNowDeferrableOperator")
         self.run_id = hook.run_now(self.json)
         _handle_deferrable_databricks_operator_execution(self, hook, self.log, context)
 
     def execute_complete(self, context: dict | None, event: dict):
         _handle_deferrable_databricks_operator_completion(event, self.log)
```

### Comparing `apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/operators/databricks_repos.py` & `apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/operators/databricks_repos.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/operators/databricks_sql.py` & `apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/operators/databricks_sql.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,14 +116,17 @@
             "schema": self.schema,
             "caller": "DatabricksSqlOperator",
             **self.client_parameters,
             **self.hook_params,
         }
         return DatabricksSqlHook(self.databricks_conn_id, **hook_params)
 
+    def _should_run_output_processing(self) -> bool:
+        return self.do_xcom_push or bool(self._output_path)
+
     def _process_output(self, results: list[Any], descriptions: list[Sequence[Sequence] | None]) -> list[Any]:
         if not self._output_path:
             return list(zip(descriptions, results))
         if not self._output_format:
             raise AirflowException("Output format should be specified!")
         # Output to a file only the result of last query
         last_description = descriptions[-1]
```

### Comparing `apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/sensors/__init__.py` & `apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/sensors/databricks_sql.py` & `apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/sensors/databricks_sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/triggers/__init__.py` & `apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/utils/__init__.py`

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

### Comparing `apache-airflow-providers-databricks-4.1.0rc1/airflow/providers/databricks/utils/databricks.py` & `apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/utils/databricks.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.1.0rc1/apache_airflow_providers_databricks.egg-info/PKG-INFO` & `apache-airflow-providers-databricks-4.2.0rc1/apache_airflow_providers_databricks.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-databricks
-Version: 4.1.0rc1
+Version: 4.2.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-databricks package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.1.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.2.0/
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
 
 
 Package ``apache-airflow-providers-databricks``
 
-Release: ``4.1.0rc1``
+Release: ``4.2.0rc1``
 
 
 `Databricks <https://databricks.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``databricks`` provider. All classes for this provider package
 are in ``airflow.providers.databricks`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.1.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.2.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -80,16 +80,16 @@
 
 Requirements
 ------------
 
 =======================================  ===================
 PIP package                              Version required
 =======================================  ===================
-``apache-airflow``                       ``>=2.3.0``
-``apache-airflow-providers-common-sql``  ``>=1.3.1``
+``apache-airflow``                       ``>=2.4.0``
+``apache-airflow-providers-common-sql``  ``>=1.5.0``
 ``requests``                             ``>=2.27,<3``
 ``databricks-sql-connector``             ``>=2.0.0, <3.0.0``
 ``aiohttp``                              ``>=3.6.3, <4``
 =======================================  ===================
 
 Cross provider package dependencies
 -----------------------------------
@@ -132,14 +132,43 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+4.2.0
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
+* ``Add cancel all runs functionality to Databricks hook (#31038)``
+* ``Add retry param in databrics async operator (#30744)``
+* ``Add repair job functionality to databricks hook (#30786)``
+* ``Add 'DatabricksPartitionSensor' (#30980)``
+
+Misc
+~~~~
+
+* ``Bump minimum Airflow version in providers (#30917)``
+* ``Deprecate databricks async operator (#30761)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Move TaskInstanceKey to a separate file (#31033)``
+   * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add cli cmd to list the provider trigger info (#30822)``
+
 4.1.0
 .....
 
 Features
 ~~~~~~~~
 
 * ``Add delete inactive run functionality to databricks provider (#30646)``
@@ -199,16 +228,17 @@
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Prepare for follow-up release for November providers (#27774)``
 
 3.4.0
 .....
 
-This release of provider is only available for Airflow 2.3+ as explained in the
-`Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/README.md#support-for-providers>`_.
+.. note::
+  This release of provider is only available for Airflow 2.3+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Misc
 ~~~~
 
 * ``Move min airflow version to 2.3.0 for all providers (#27196)``
 * ``Replace urlparse with urlsplit (#27389)``
 
@@ -296,16 +326,17 @@
 
 3.0.0
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
 
 * ``Add Deferrable Databricks operators (#19736)``
 * ``Add git_source to DatabricksSubmitRunOperator (#23620)``
```

### Comparing `apache-airflow-providers-databricks-4.1.0rc1/apache_airflow_providers_databricks.egg-info/SOURCES.txt` & `apache-airflow-providers-databricks-4.2.0rc1/apache_airflow_providers_databricks.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 airflow/providers/databricks/hooks/databricks_base.py
 airflow/providers/databricks/hooks/databricks_sql.py
 airflow/providers/databricks/operators/__init__.py
 airflow/providers/databricks/operators/databricks.py
 airflow/providers/databricks/operators/databricks_repos.py
 airflow/providers/databricks/operators/databricks_sql.py
 airflow/providers/databricks/sensors/__init__.py
+airflow/providers/databricks/sensors/databricks_partition.py
 airflow/providers/databricks/sensors/databricks_sql.py
 airflow/providers/databricks/triggers/__init__.py
 airflow/providers/databricks/triggers/databricks.py
 airflow/providers/databricks/utils/__init__.py
 airflow/providers/databricks/utils/databricks.py
 apache_airflow_providers_databricks.egg-info/PKG-INFO
 apache_airflow_providers_databricks.egg-info/SOURCES.txt
```

### Comparing `apache-airflow-providers-databricks-4.1.0rc1/pyproject.toml` & `apache-airflow-providers-databricks-4.2.0rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-databricks-4.1.0rc1/setup.cfg` & `apache-airflow-providers-databricks-4.2.0rc1/setup.cfg`

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.1.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.2.0/
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
@@ -43,16 +43,16 @@
 python_requires = ~=3.7
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
 	aiohttp>=3.6.3, <4
-	apache-airflow-providers-common-sql>=1.3.1.dev0
-	apache-airflow>=2.3.0.dev0
+	apache-airflow-providers-common-sql>=1.5.0.dev0
+	apache-airflow>=2.4.0.dev0
 	databricks-sql-connector>=2.0.0, <3.0.0
 	requests>=2.27,<3
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.databricks.get_provider_info:get_provider_info
```

### Comparing `apache-airflow-providers-databricks-4.1.0rc1/setup.py` & `apache-airflow-providers-databricks-4.2.0rc1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-databricks package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "4.1.0"
+version = "4.2.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-databricks setup."""
     setup(
         version=version,
         extras_require={"common.sql": ["apache-airflow-providers-common-sql"]},
```

