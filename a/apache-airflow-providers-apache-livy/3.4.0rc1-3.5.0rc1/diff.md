# Comparing `tmp/apache-airflow-providers-apache-livy-3.4.0rc1.tar.gz` & `tmp/apache-airflow-providers-apache-livy-3.5.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-apache-livy-3.4.0rc1.tar", last modified: Sun Apr  2 05:47:08 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-apache-livy-3.5.0rc1.tar", last modified: Tue May 16 15:53:11 2023, max compression
```

## Comparing `apache-airflow-providers-apache-livy-3.4.0rc1.tar` & `apache-airflow-providers-apache-livy-3.5.0rc1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:08.000000 apache-airflow-providers-apache-livy-3.4.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-livy-3.4.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1122 2023-04-02 05:47:07.000000 apache-airflow-providers-apache-livy-3.4.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-livy-3.4.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    11320 2023-04-02 05:47:08.000000 apache-airflow-providers-apache-livy-3.4.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9757 2023-04-02 05:47:07.000000 apache-airflow-providers-apache-livy-3.4.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:08.000000 apache-airflow-providers-apache-livy-3.4.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:08.000000 apache-airflow-providers-apache-livy-3.4.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:08.000000 apache-airflow-providers-apache-livy-3.4.0rc1/airflow/providers/apache/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:08.000000 apache-airflow-providers-apache-livy-3.4.0rc1/airflow/providers/apache/livy/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-livy-3.4.0rc1/airflow/providers/apache/livy/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3012 2023-04-02 05:47:07.000000 apache-airflow-providers-apache-livy-3.4.0rc1/airflow/providers/apache/livy/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:08.000000 apache-airflow-providers-apache-livy-3.4.0rc1/airflow/providers/apache/livy/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-livy-3.4.0rc1/airflow/providers/apache/livy/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31534 2023-03-27 08:32:49.000000 apache-airflow-providers-apache-livy-3.4.0rc1/airflow/providers/apache/livy/hooks/livy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:08.000000 apache-airflow-providers-apache-livy-3.4.0rc1/airflow/providers/apache/livy/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-livy-3.4.0rc1/airflow/providers/apache/livy/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8738 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-livy-3.4.0rc1/airflow/providers/apache/livy/operators/livy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:08.000000 apache-airflow-providers-apache-livy-3.4.0rc1/airflow/providers/apache/livy/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-livy-3.4.0rc1/airflow/providers/apache/livy/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2574 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-livy-3.4.0rc1/airflow/providers/apache/livy/sensors/livy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:08.000000 apache-airflow-providers-apache-livy-3.4.0rc1/airflow/providers/apache/livy/triggers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-livy-3.4.0rc1/airflow/providers/apache/livy/triggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6240 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-livy-3.4.0rc1/airflow/providers/apache/livy/triggers/livy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:08.000000 apache-airflow-providers-apache-livy-3.4.0rc1/apache_airflow_providers_apache_livy.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11320 2023-04-02 05:47:08.000000 apache-airflow-providers-apache-livy-3.4.0rc1/apache_airflow_providers_apache_livy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      971 2023-04-02 05:47:08.000000 apache-airflow-providers-apache-livy-3.4.0rc1/apache_airflow_providers_apache_livy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-02 05:47:08.000000 apache-airflow-providers-apache-livy-3.4.0rc1/apache_airflow_providers_apache_livy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      108 2023-04-02 05:47:08.000000 apache-airflow-providers-apache-livy-3.4.0rc1/apache_airflow_providers_apache_livy.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-02 05:47:08.000000 apache-airflow-providers-apache-livy-3.4.0rc1/apache_airflow_providers_apache_livy.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      111 2023-04-02 05:47:08.000000 apache-airflow-providers-apache-livy-3.4.0rc1/apache_airflow_providers_apache_livy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-02 05:47:08.000000 apache-airflow-providers-apache-livy-3.4.0rc1/apache_airflow_providers_apache_livy.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5393 2023-04-01 16:40:04.000000 apache-airflow-providers-apache-livy-3.4.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1907 2023-04-02 05:47:08.000000 apache-airflow-providers-apache-livy-3.4.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1547 2023-04-02 05:47:07.000000 apache-airflow-providers-apache-livy-3.4.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:11.000000 apache-airflow-providers-apache-livy-3.5.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-livy-3.5.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-05-16 15:53:10.000000 apache-airflow-providers-apache-livy-3.5.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-livy-3.5.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    12169 2023-05-16 15:53:11.000000 apache-airflow-providers-apache-livy-3.5.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10606 2023-05-16 15:53:10.000000 apache-airflow-providers-apache-livy-3.5.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:11.000000 apache-airflow-providers-apache-livy-3.5.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:11.000000 apache-airflow-providers-apache-livy-3.5.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:11.000000 apache-airflow-providers-apache-livy-3.5.0rc1/airflow/providers/apache/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:11.000000 apache-airflow-providers-apache-livy-3.5.0rc1/airflow/providers/apache/livy/
+-rw-r--r--   0 root         (0) root         (0)     1394 2023-05-16 15:39:21.000000 apache-airflow-providers-apache-livy-3.5.0rc1/airflow/providers/apache/livy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3070 2023-05-16 15:53:10.000000 apache-airflow-providers-apache-livy-3.5.0rc1/airflow/providers/apache/livy/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:11.000000 apache-airflow-providers-apache-livy-3.5.0rc1/airflow/providers/apache/livy/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-livy-3.5.0rc1/airflow/providers/apache/livy/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31534 2023-03-27 08:32:49.000000 apache-airflow-providers-apache-livy-3.5.0rc1/airflow/providers/apache/livy/hooks/livy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:11.000000 apache-airflow-providers-apache-livy-3.5.0rc1/airflow/providers/apache/livy/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-livy-3.5.0rc1/airflow/providers/apache/livy/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8738 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-livy-3.5.0rc1/airflow/providers/apache/livy/operators/livy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:11.000000 apache-airflow-providers-apache-livy-3.5.0rc1/airflow/providers/apache/livy/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-livy-3.5.0rc1/airflow/providers/apache/livy/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2574 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-livy-3.5.0rc1/airflow/providers/apache/livy/sensors/livy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:11.000000 apache-airflow-providers-apache-livy-3.5.0rc1/airflow/providers/apache/livy/triggers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-livy-3.5.0rc1/airflow/providers/apache/livy/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6238 2023-04-24 21:04:25.000000 apache-airflow-providers-apache-livy-3.5.0rc1/airflow/providers/apache/livy/triggers/livy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:11.000000 apache-airflow-providers-apache-livy-3.5.0rc1/apache_airflow_providers_apache_livy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    12169 2023-05-16 15:53:11.000000 apache-airflow-providers-apache-livy-3.5.0rc1/apache_airflow_providers_apache_livy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      971 2023-05-16 15:53:11.000000 apache-airflow-providers-apache-livy-3.5.0rc1/apache_airflow_providers_apache_livy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:53:11.000000 apache-airflow-providers-apache-livy-3.5.0rc1/apache_airflow_providers_apache_livy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      108 2023-05-16 15:53:11.000000 apache-airflow-providers-apache-livy-3.5.0rc1/apache_airflow_providers_apache_livy.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:53:11.000000 apache-airflow-providers-apache-livy-3.5.0rc1/apache_airflow_providers_apache_livy.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      111 2023-05-16 15:53:11.000000 apache-airflow-providers-apache-livy-3.5.0rc1/apache_airflow_providers_apache_livy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-16 15:53:11.000000 apache-airflow-providers-apache-livy-3.5.0rc1/apache_airflow_providers_apache_livy.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5308 2023-05-15 09:39:26.000000 apache-airflow-providers-apache-livy-3.5.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1907 2023-05-16 15:53:11.000000 apache-airflow-providers-apache-livy-3.5.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1709 2023-05-16 15:53:10.000000 apache-airflow-providers-apache-livy-3.5.0rc1/setup.py
```

### Comparing `apache-airflow-providers-apache-livy-3.4.0rc1/LICENSE` & `apache-airflow-providers-apache-livy-3.5.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-livy-3.4.0rc1/MANIFEST.in` & `apache-airflow-providers-apache-livy-3.5.0rc1/MANIFEST.in`

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

### Comparing `apache-airflow-providers-apache-livy-3.4.0rc1/PKG-INFO` & `apache-airflow-providers-apache-livy-3.5.0rc1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-livy
-Version: 3.4.0rc1
+Version: 3.5.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-livy package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-livy/3.4.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-livy/3.5.0/
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
 
 
 Package ``apache-airflow-providers-apache-livy``
 
-Release: ``3.4.0rc1``
+Release: ``3.5.0rc1``
 
 
 `Apache Livy <https://livy.apache.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.livy`` provider. All classes for this provider package
 are in ``airflow.providers.apache.livy`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-livy/3.4.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-livy/3.5.0/>`_.
 
 
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
 ``aiohttp``
 ``asgiref``
 =================================  ==================
 
 Cross provider package dependencies
 -----------------------------------
@@ -131,14 +131,33 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.5.0
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
+   * ``Add mechanism to suspend providers (#30422)``
+
 3.4.0
 .....
 
 Features
 ~~~~~~~~
 
 * ``Add non login-password auth support for SimpleHttpOpeator (#29206)``
@@ -159,16 +178,17 @@
    appropriate section above if needed. Do not delete the lines(!):
    * ``Prepare docs for Jan 2023 mid-month wave of Providers (#28929)``
    * ``Fix providers documentation formatting (#28754)``
 
 3.2.0
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
@@ -202,16 +222,17 @@
 
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
    * ``AIP-47 - Migrate livy DAGs to new design #22439 (#24208)``
    * ``Prepare docs for May 2022 provider's release (#24231)``
    * ``Update package description to remove double min-airflow specification (#24292)``
```

### Comparing `apache-airflow-providers-apache-livy-3.4.0rc1/README.rst` & `apache-airflow-providers-apache-livy-3.5.0rc1/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -15,28 +15,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-livy``
 
-Release: ``3.4.0rc1``
+Release: ``3.5.0rc1``
 
 
 `Apache Livy <https://livy.apache.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.livy`` provider. All classes for this provider package
 are in ``airflow.providers.apache.livy`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-livy/3.4.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-livy/3.5.0/>`_.
 
 
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
 ``aiohttp``
 ``asgiref``
 =================================  ==================
 
 Cross provider package dependencies
 -----------------------------------
@@ -97,14 +97,33 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.5.0
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
+   * ``Add mechanism to suspend providers (#30422)``
+
 3.4.0
 .....
 
 Features
 ~~~~~~~~
 
 * ``Add non login-password auth support for SimpleHttpOpeator (#29206)``
@@ -125,16 +144,17 @@
    appropriate section above if needed. Do not delete the lines(!):
    * ``Prepare docs for Jan 2023 mid-month wave of Providers (#28929)``
    * ``Fix providers documentation formatting (#28754)``
 
 3.2.0
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
@@ -168,16 +188,17 @@
 
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
    * ``AIP-47 - Migrate livy DAGs to new design #22439 (#24208)``
    * ``Prepare docs for May 2022 provider's release (#24231)``
    * ``Update package description to remove double min-airflow specification (#24292)``
```

### Comparing `apache-airflow-providers-apache-livy-3.4.0rc1/airflow/providers/apache/livy/__init__.py` & `apache-airflow-providers-apache-livy-3.5.0rc1/airflow/providers/apache/livy/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-livy-3.4.0rc1/airflow/providers/apache/livy/get_provider_info.py` & `apache-airflow-providers-apache-livy-3.5.0rc1/airflow/providers/apache/livy/get_provider_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,17 @@
 
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-apache-livy",
         "name": "Apache Livy",
         "description": "`Apache Livy <https://livy.apache.org/>`__\n",
+        "suspended": False,
         "versions": [
+            "3.5.0",
             "3.4.0",
             "3.3.0",
             "3.2.0",
             "3.1.0",
             "3.0.0",
             "2.2.3",
             "2.2.2",
@@ -39,15 +41,15 @@
             "2.2.0",
             "2.1.0",
             "2.0.0",
             "1.1.0",
             "1.0.1",
             "1.0.0",
         ],
-        "dependencies": ["apache-airflow>=2.3.0", "apache-airflow-providers-http", "aiohttp", "asgiref"],
+        "dependencies": ["apache-airflow>=2.4.0", "apache-airflow-providers-http", "aiohttp", "asgiref"],
         "integrations": [
             {
                 "integration-name": "Apache Livy",
                 "external-doc-url": "https://livy.apache.org/",
                 "how-to-guide": ["/docs/apache-airflow-providers-apache-livy/operators.rst"],
                 "logo": "/integration-logos/apache/Livy.png",
                 "tags": ["apache"],
@@ -70,15 +72,15 @@
                 "integration-name": "Apache Livy",
                 "python-modules": ["airflow.providers.apache.livy.hooks.livy"],
             }
         ],
         "triggers": [
             {
                 "integration-name": "Apache Livy",
-                "python-modules": ["airflow.providers.apache.livy.triggers.livy"],
+                "class-names": ["airflow.providers.apache.livy.triggers.livy.LivyTrigger"],
             }
         ],
         "connection-types": [
             {
                 "hook-class-name": "airflow.providers.apache.livy.hooks.livy.LivyHook",
                 "connection-type": "livy",
             }
```

### Comparing `apache-airflow-providers-apache-livy-3.4.0rc1/airflow/providers/apache/livy/hooks/__init__.py` & `apache-airflow-providers-apache-livy-3.5.0rc1/airflow/providers/apache/livy/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-livy-3.4.0rc1/airflow/providers/apache/livy/hooks/livy.py` & `apache-airflow-providers-apache-livy-3.5.0rc1/airflow/providers/apache/livy/hooks/livy.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-livy-3.4.0rc1/airflow/providers/apache/livy/operators/__init__.py` & `apache-airflow-providers-apache-livy-3.5.0rc1/airflow/providers/apache/livy/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-livy-3.4.0rc1/airflow/providers/apache/livy/operators/livy.py` & `apache-airflow-providers-apache-livy-3.5.0rc1/airflow/providers/apache/livy/operators/livy.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-livy-3.4.0rc1/airflow/providers/apache/livy/sensors/__init__.py` & `apache-airflow-providers-apache-livy-3.5.0rc1/airflow/providers/apache/livy/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-livy-3.4.0rc1/airflow/providers/apache/livy/sensors/livy.py` & `apache-airflow-providers-apache-livy-3.5.0rc1/airflow/providers/apache/livy/sensors/livy.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-livy-3.4.0rc1/airflow/providers/apache/livy/triggers/livy.py` & `apache-airflow-providers-apache-livy-3.5.0rc1/airflow/providers/apache/livy/triggers/livy.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
                 "polling_interval": self._polling_interval,
                 "extra_options": self._extra_options,
                 "extra_headers": self._extra_headers,
                 "livy_hook_async": self._livy_hook_async,
             },
         )
 
-    async def run(self) -> AsyncIterator["TriggerEvent"]:
+    async def run(self) -> AsyncIterator[TriggerEvent]:
         """
         Checks if the _polling_interval > 0, in that case it pools Livy for
         batch termination asynchronously.
         else returns the success response
         """
         try:
             if self._polling_interval > 0:
```

### Comparing `apache-airflow-providers-apache-livy-3.4.0rc1/apache_airflow_providers_apache_livy.egg-info/PKG-INFO` & `apache-airflow-providers-apache-livy-3.5.0rc1/apache_airflow_providers_apache_livy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-livy
-Version: 3.4.0rc1
+Version: 3.5.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-livy package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-livy/3.4.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-livy/3.5.0/
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
 
 
 Package ``apache-airflow-providers-apache-livy``
 
-Release: ``3.4.0rc1``
+Release: ``3.5.0rc1``
 
 
 `Apache Livy <https://livy.apache.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.livy`` provider. All classes for this provider package
 are in ``airflow.providers.apache.livy`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-livy/3.4.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-livy/3.5.0/>`_.
 
 
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
 ``aiohttp``
 ``asgiref``
 =================================  ==================
 
 Cross provider package dependencies
 -----------------------------------
@@ -131,14 +131,33 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.5.0
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
+   * ``Add mechanism to suspend providers (#30422)``
+
 3.4.0
 .....
 
 Features
 ~~~~~~~~
 
 * ``Add non login-password auth support for SimpleHttpOpeator (#29206)``
@@ -159,16 +178,17 @@
    appropriate section above if needed. Do not delete the lines(!):
    * ``Prepare docs for Jan 2023 mid-month wave of Providers (#28929)``
    * ``Fix providers documentation formatting (#28754)``
 
 3.2.0
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
@@ -202,16 +222,17 @@
 
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
    * ``AIP-47 - Migrate livy DAGs to new design #22439 (#24208)``
    * ``Prepare docs for May 2022 provider's release (#24231)``
    * ``Update package description to remove double min-airflow specification (#24292)``
```

### Comparing `apache-airflow-providers-apache-livy-3.4.0rc1/apache_airflow_providers_apache_livy.egg-info/SOURCES.txt` & `apache-airflow-providers-apache-livy-3.5.0rc1/apache_airflow_providers_apache_livy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-livy-3.4.0rc1/pyproject.toml` & `apache-airflow-providers-apache-livy-3.5.0rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-apache-livy-3.4.0rc1/setup.cfg` & `apache-airflow-providers-apache-livy-3.5.0rc1/setup.cfg`

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-apache-livy/3.4.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-apache-livy/3.5.0/
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
 	provider_info=airflow.providers.apache.livy.get_provider_info:get_provider_info
 
 [files]
```

### Comparing `apache-airflow-providers-apache-livy-3.4.0rc1/setup.py` & `apache-airflow-providers-apache-livy-3.5.0rc1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,23 +22,28 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-apache-livy package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "3.4.0"
+version = "3.5.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-apache-livy setup."""
     setup(
         version=version,
         extras_require={"http": ["apache-airflow-providers-http"]},
         packages=find_namespace_packages(
-            include=["airflow.providers.apache.livy", "airflow.providers.apache.livy.*"]
+            include=[
+                "airflow.providers.apache.livy",
+                "airflow.providers.apache.livy.*",
+                "airflow.providers.apache.livy_vendor",
+                "airflow.providers.apache.livy_vendor.*",
+            ],
         ),
     )
 
 
 if __name__ == "__main__":
     do_setup()
```

