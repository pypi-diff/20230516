# Comparing `tmp/apache-airflow-providers-datadog-3.2.0rc1.tar.gz` & `tmp/apache-airflow-providers-datadog-3.3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-datadog-3.2.0rc1.tar", last modified: Sun Apr  2 05:47:29 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-datadog-3.3.0rc1.tar", last modified: Tue May 16 15:53:35 2023, max compression
```

## Comparing `apache-airflow-providers-datadog-3.2.0rc1.tar` & `apache-airflow-providers-datadog-3.3.0rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:29.000000 apache-airflow-providers-datadog-3.2.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-datadog-3.2.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1122 2023-04-02 05:47:27.000000 apache-airflow-providers-datadog-3.2.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-datadog-3.2.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     8905 2023-04-02 05:47:29.000000 apache-airflow-providers-datadog-3.2.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7375 2023-04-02 05:47:27.000000 apache-airflow-providers-datadog-3.2.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:29.000000 apache-airflow-providers-datadog-3.2.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:29.000000 apache-airflow-providers-datadog-3.2.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:29.000000 apache-airflow-providers-datadog-3.2.0rc1/airflow/providers/datadog/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-datadog-3.2.0rc1/airflow/providers/datadog/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2300 2023-04-02 05:47:27.000000 apache-airflow-providers-datadog-3.2.0rc1/airflow/providers/datadog/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:29.000000 apache-airflow-providers-datadog-3.2.0rc1/airflow/providers/datadog/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-datadog-3.2.0rc1/airflow/providers/datadog/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7317 2023-03-16 20:46:35.000000 apache-airflow-providers-datadog-3.2.0rc1/airflow/providers/datadog/hooks/datadog.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:29.000000 apache-airflow-providers-datadog-3.2.0rc1/airflow/providers/datadog/sensors/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-datadog-3.2.0rc1/airflow/providers/datadog/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4060 2023-02-24 18:43:53.000000 apache-airflow-providers-datadog-3.2.0rc1/airflow/providers/datadog/sensors/datadog.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:47:29.000000 apache-airflow-providers-datadog-3.2.0rc1/apache_airflow_providers_datadog.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8905 2023-04-02 05:47:28.000000 apache-airflow-providers-datadog-3.2.0rc1/apache_airflow_providers_datadog.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      727 2023-04-02 05:47:28.000000 apache-airflow-providers-datadog-3.2.0rc1/apache_airflow_providers_datadog.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-02 05:47:28.000000 apache-airflow-providers-datadog-3.2.0rc1/apache_airflow_providers_datadog.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-04-02 05:47:28.000000 apache-airflow-providers-datadog-3.2.0rc1/apache_airflow_providers_datadog.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-02 05:47:28.000000 apache-airflow-providers-datadog-3.2.0rc1/apache_airflow_providers_datadog.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       43 2023-04-02 05:47:28.000000 apache-airflow-providers-datadog-3.2.0rc1/apache_airflow_providers_datadog.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-02 05:47:28.000000 apache-airflow-providers-datadog-3.2.0rc1/apache_airflow_providers_datadog.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5393 2023-04-01 16:40:04.000000 apache-airflow-providers-datadog-3.2.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1851 2023-04-02 05:47:29.000000 apache-airflow-providers-datadog-3.2.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1490 2023-04-02 05:47:27.000000 apache-airflow-providers-datadog-3.2.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:35.000000 apache-airflow-providers-datadog-3.3.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-datadog-3.3.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-05-16 15:53:34.000000 apache-airflow-providers-datadog-3.3.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-datadog-3.3.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     9648 2023-05-16 15:53:35.000000 apache-airflow-providers-datadog-3.3.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8118 2023-05-16 15:53:34.000000 apache-airflow-providers-datadog-3.3.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:35.000000 apache-airflow-providers-datadog-3.3.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:35.000000 apache-airflow-providers-datadog-3.3.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:35.000000 apache-airflow-providers-datadog-3.3.0rc1/airflow/providers/datadog/
+-rw-r--r--   0 root         (0) root         (0)     1390 2023-05-16 15:39:21.000000 apache-airflow-providers-datadog-3.3.0rc1/airflow/providers/datadog/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2349 2023-05-16 15:53:34.000000 apache-airflow-providers-datadog-3.3.0rc1/airflow/providers/datadog/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:35.000000 apache-airflow-providers-datadog-3.3.0rc1/airflow/providers/datadog/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-datadog-3.3.0rc1/airflow/providers/datadog/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7317 2023-03-16 20:46:35.000000 apache-airflow-providers-datadog-3.3.0rc1/airflow/providers/datadog/hooks/datadog.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:35.000000 apache-airflow-providers-datadog-3.3.0rc1/airflow/providers/datadog/sensors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-datadog-3.3.0rc1/airflow/providers/datadog/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4060 2023-02-24 18:43:53.000000 apache-airflow-providers-datadog-3.3.0rc1/airflow/providers/datadog/sensors/datadog.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:35.000000 apache-airflow-providers-datadog-3.3.0rc1/apache_airflow_providers_datadog.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9648 2023-05-16 15:53:35.000000 apache-airflow-providers-datadog-3.3.0rc1/apache_airflow_providers_datadog.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      727 2023-05-16 15:53:35.000000 apache-airflow-providers-datadog-3.3.0rc1/apache_airflow_providers_datadog.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:53:35.000000 apache-airflow-providers-datadog-3.3.0rc1/apache_airflow_providers_datadog.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2023-05-16 15:53:35.000000 apache-airflow-providers-datadog-3.3.0rc1/apache_airflow_providers_datadog.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:53:35.000000 apache-airflow-providers-datadog-3.3.0rc1/apache_airflow_providers_datadog.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       43 2023-05-16 15:53:35.000000 apache-airflow-providers-datadog-3.3.0rc1/apache_airflow_providers_datadog.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-16 15:53:35.000000 apache-airflow-providers-datadog-3.3.0rc1/apache_airflow_providers_datadog.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5308 2023-05-15 09:39:26.000000 apache-airflow-providers-datadog-3.3.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1851 2023-05-16 15:53:35.000000 apache-airflow-providers-datadog-3.3.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1644 2023-05-16 15:53:34.000000 apache-airflow-providers-datadog-3.3.0rc1/setup.py
```

### Comparing `apache-airflow-providers-datadog-3.2.0rc1/LICENSE` & `apache-airflow-providers-datadog-3.3.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-datadog-3.2.0rc1/MANIFEST.in` & `apache-airflow-providers-datadog-3.3.0rc1/MANIFEST.in`

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

### Comparing `apache-airflow-providers-datadog-3.2.0rc1/PKG-INFO` & `apache-airflow-providers-datadog-3.3.0rc1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-datadog
-Version: 3.2.0rc1
+Version: 3.3.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-datadog package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-datadog/3.2.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-datadog/3.3.0/
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
 
 
 Package ``apache-airflow-providers-datadog``
 
-Release: ``3.2.0rc1``
+Release: ``3.3.0rc1``
 
 
 `Datadog <https://www.datadoghq.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``datadog`` provider. All classes for this provider package
 are in ``airflow.providers.datadog`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-datadog/3.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-datadog/3.3.0/>`_.
 
 
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
 ``datadog``         ``>=0.14.0``
 ==================  ==================
 
  .. Licensed to the Apache Software Foundation (ASF) under one
     or more contributor license agreements.  See the NOTICE file
     distributed with this work for additional information
     regarding copyright ownership.  The ASF licenses this file
@@ -109,27 +109,45 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.3.0
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
 3.2.0
 .....
 
 Features
 ~~~~~~~~
 
 * ``Support creating Datadog connection from the UI and add documentation for this conn (#30059)``
 
 3.1.0
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
@@ -145,16 +163,17 @@
 
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
    * ``Support host_name on Datadog provider (#23784)``
    * ``Fix new MyPy errors in main (#22884)``
    * ``Prepare provider documentation 2022.05.11 (#23631)``
```

### Comparing `apache-airflow-providers-datadog-3.2.0rc1/README.rst` & `apache-airflow-providers-datadog-3.3.0rc1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -15,28 +15,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-datadog``
 
-Release: ``3.2.0rc1``
+Release: ``3.3.0rc1``
 
 
 `Datadog <https://www.datadoghq.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``datadog`` provider. All classes for this provider package
 are in ``airflow.providers.datadog`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-datadog/3.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-datadog/3.3.0/>`_.
 
 
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
 ``datadog``         ``>=0.14.0``
 ==================  ==================
 
  .. Licensed to the Apache Software Foundation (ASF) under one
     or more contributor license agreements.  See the NOTICE file
     distributed with this work for additional information
     regarding copyright ownership.  The ASF licenses this file
@@ -76,27 +76,45 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.3.0
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
 3.2.0
 .....
 
 Features
 ~~~~~~~~
 
 * ``Support creating Datadog connection from the UI and add documentation for this conn (#30059)``
 
 3.1.0
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
@@ -112,16 +130,17 @@
 
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
    * ``Support host_name on Datadog provider (#23784)``
    * ``Fix new MyPy errors in main (#22884)``
    * ``Prepare provider documentation 2022.05.11 (#23631)``
```

### Comparing `apache-airflow-providers-datadog-3.2.0rc1/airflow/providers/datadog/__init__.py` & `apache-airflow-providers-datadog-3.3.0rc1/airflow/providers/datadog/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-datadog-3.2.0rc1/airflow/providers/datadog/get_provider_info.py` & `apache-airflow-providers-datadog-3.3.0rc1/airflow/providers/datadog/get_provider_info.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,27 +23,29 @@
 
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-datadog",
         "name": "Datadog",
         "description": "`Datadog <https://www.datadoghq.com/>`__\n",
+        "suspended": False,
         "versions": [
+            "3.3.0",
             "3.2.0",
             "3.1.0",
             "3.0.0",
             "2.0.4",
             "2.0.3",
             "2.0.2",
             "2.0.1",
             "2.0.0",
             "1.0.1",
             "1.0.0",
         ],
-        "dependencies": ["apache-airflow>=2.3.0", "datadog>=0.14.0"],
+        "dependencies": ["apache-airflow>=2.4.0", "datadog>=0.14.0"],
         "integrations": [
             {
                 "integration-name": "Datadog",
                 "external-doc-url": "https://www.datadoghq.com/",
                 "logo": "/integration-logos/datadog/datadog.png",
                 "tags": ["service"],
             }
```

### Comparing `apache-airflow-providers-datadog-3.2.0rc1/airflow/providers/datadog/hooks/__init__.py` & `apache-airflow-providers-datadog-3.3.0rc1/airflow/providers/datadog/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-datadog-3.2.0rc1/airflow/providers/datadog/hooks/datadog.py` & `apache-airflow-providers-datadog-3.3.0rc1/airflow/providers/datadog/hooks/datadog.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-datadog-3.2.0rc1/airflow/providers/datadog/sensors/datadog.py` & `apache-airflow-providers-datadog-3.3.0rc1/airflow/providers/datadog/sensors/datadog.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-datadog-3.2.0rc1/apache_airflow_providers_datadog.egg-info/PKG-INFO` & `apache-airflow-providers-datadog-3.3.0rc1/apache_airflow_providers_datadog.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-datadog
-Version: 3.2.0rc1
+Version: 3.3.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-datadog package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-datadog/3.2.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-datadog/3.3.0/
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
 
 
 Package ``apache-airflow-providers-datadog``
 
-Release: ``3.2.0rc1``
+Release: ``3.3.0rc1``
 
 
 `Datadog <https://www.datadoghq.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``datadog`` provider. All classes for this provider package
 are in ``airflow.providers.datadog`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-datadog/3.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-datadog/3.3.0/>`_.
 
 
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
 ``datadog``         ``>=0.14.0``
 ==================  ==================
 
  .. Licensed to the Apache Software Foundation (ASF) under one
     or more contributor license agreements.  See the NOTICE file
     distributed with this work for additional information
     regarding copyright ownership.  The ASF licenses this file
@@ -109,27 +109,45 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.3.0
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
 3.2.0
 .....
 
 Features
 ~~~~~~~~
 
 * ``Support creating Datadog connection from the UI and add documentation for this conn (#30059)``
 
 3.1.0
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
@@ -145,16 +163,17 @@
 
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
    * ``Support host_name on Datadog provider (#23784)``
    * ``Fix new MyPy errors in main (#22884)``
    * ``Prepare provider documentation 2022.05.11 (#23631)``
```

### Comparing `apache-airflow-providers-datadog-3.2.0rc1/apache_airflow_providers_datadog.egg-info/SOURCES.txt` & `apache-airflow-providers-datadog-3.3.0rc1/apache_airflow_providers_datadog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-datadog-3.2.0rc1/pyproject.toml` & `apache-airflow-providers-datadog-3.3.0rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-datadog-3.2.0rc1/setup.cfg` & `apache-airflow-providers-datadog-3.3.0rc1/setup.cfg`

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-datadog/3.2.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-datadog/3.3.0/
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
 	datadog>=0.14.0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.datadog.get_provider_info:get_provider_info
 
 [files]
```

### Comparing `apache-airflow-providers-datadog-3.2.0rc1/setup.py` & `apache-airflow-providers-datadog-3.3.0rc1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,23 +22,28 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-datadog package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "3.2.0"
+version = "3.3.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-datadog setup."""
     setup(
         version=version,
         extras_require={},
         packages=find_namespace_packages(
-            include=["airflow.providers.datadog", "airflow.providers.datadog.*"]
+            include=[
+                "airflow.providers.datadog",
+                "airflow.providers.datadog.*",
+                "airflow.providers.datadog_vendor",
+                "airflow.providers.datadog_vendor.*",
+            ],
         ),
     )
 
 
 if __name__ == "__main__":
     do_setup()
```

