# Comparing `tmp/apache-airflow-providers-apache-sqoop-3.1.1rc1.tar.gz` & `tmp/apache-airflow-providers-apache-sqoop-3.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-apache-sqoop-3.1.1rc1.tar", last modified: Sat Feb 18 20:35:17 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-apache-sqoop-3.2.0rc1.tar", last modified: Tue May 16 15:53:18 2023, max compression
```

## Comparing `apache-airflow-providers-apache-sqoop-3.1.1rc1.tar` & `apache-airflow-providers-apache-sqoop-3.2.0rc1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-18 20:35:17.000000 apache-airflow-providers-apache-sqoop-3.1.1rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2022-10-05 12:15:16.000000 apache-airflow-providers-apache-sqoop-3.1.1rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1122 2023-02-18 20:35:15.000000 apache-airflow-providers-apache-sqoop-3.1.1rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2022-10-05 12:15:16.000000 apache-airflow-providers-apache-sqoop-3.1.1rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     9449 2023-02-18 20:35:17.000000 apache-airflow-providers-apache-sqoop-3.1.1rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7884 2023-02-18 20:35:15.000000 apache-airflow-providers-apache-sqoop-3.1.1rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-18 20:35:16.000000 apache-airflow-providers-apache-sqoop-3.1.1rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-18 20:35:16.000000 apache-airflow-providers-apache-sqoop-3.1.1rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-18 20:35:16.000000 apache-airflow-providers-apache-sqoop-3.1.1rc1/airflow/providers/apache/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-18 20:35:16.000000 apache-airflow-providers-apache-sqoop-3.1.1rc1/airflow/providers/apache/sqoop/
--rw-r--r--   0 root         (0) root         (0)      787 2022-10-05 12:15:15.000000 apache-airflow-providers-apache-sqoop-3.1.1rc1/airflow/providers/apache/sqoop/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2545 2023-02-18 20:35:15.000000 apache-airflow-providers-apache-sqoop-3.1.1rc1/airflow/providers/apache/sqoop/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-18 20:35:17.000000 apache-airflow-providers-apache-sqoop-3.1.1rc1/airflow/providers/apache/sqoop/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2022-10-05 12:15:15.000000 apache-airflow-providers-apache-sqoop-3.1.1rc1/airflow/providers/apache/sqoop/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15813 2023-02-17 12:32:17.000000 apache-airflow-providers-apache-sqoop-3.1.1rc1/airflow/providers/apache/sqoop/hooks/sqoop.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-18 20:35:17.000000 apache-airflow-providers-apache-sqoop-3.1.1rc1/airflow/providers/apache/sqoop/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2022-10-05 12:15:15.000000 apache-airflow-providers-apache-sqoop-3.1.1rc1/airflow/providers/apache/sqoop/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11404 2023-02-17 12:32:17.000000 apache-airflow-providers-apache-sqoop-3.1.1rc1/airflow/providers/apache/sqoop/operators/sqoop.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-18 20:35:17.000000 apache-airflow-providers-apache-sqoop-3.1.1rc1/apache_airflow_providers_apache_sqoop.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9449 2023-02-18 20:35:16.000000 apache-airflow-providers-apache-sqoop-3.1.1rc1/apache_airflow_providers_apache_sqoop.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      792 2023-02-18 20:35:16.000000 apache-airflow-providers-apache-sqoop-3.1.1rc1/apache_airflow_providers_apache_sqoop.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-18 20:35:16.000000 apache-airflow-providers-apache-sqoop-3.1.1rc1/apache_airflow_providers_apache_sqoop.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      110 2023-02-18 20:35:16.000000 apache-airflow-providers-apache-sqoop-3.1.1rc1/apache_airflow_providers_apache_sqoop.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-18 20:35:16.000000 apache-airflow-providers-apache-sqoop-3.1.1rc1/apache_airflow_providers_apache_sqoop.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       27 2023-02-18 20:35:16.000000 apache-airflow-providers-apache-sqoop-3.1.1rc1/apache_airflow_providers_apache_sqoop.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-02-18 20:35:16.000000 apache-airflow-providers-apache-sqoop-3.1.1rc1/apache_airflow_providers_apache_sqoop.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     3814 2023-02-11 18:49:53.000000 apache-airflow-providers-apache-sqoop-3.1.1rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1864 2023-02-18 20:35:17.000000 apache-airflow-providers-apache-sqoop-3.1.1rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1510 2023-02-18 20:35:15.000000 apache-airflow-providers-apache-sqoop-3.1.1rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:18.000000 apache-airflow-providers-apache-sqoop-3.2.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-sqoop-3.2.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-05-16 15:53:17.000000 apache-airflow-providers-apache-sqoop-3.2.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-sqoop-3.2.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    10172 2023-05-16 15:53:18.000000 apache-airflow-providers-apache-sqoop-3.2.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8627 2023-05-16 15:53:17.000000 apache-airflow-providers-apache-sqoop-3.2.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:18.000000 apache-airflow-providers-apache-sqoop-3.2.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:18.000000 apache-airflow-providers-apache-sqoop-3.2.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:18.000000 apache-airflow-providers-apache-sqoop-3.2.0rc1/airflow/providers/apache/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:18.000000 apache-airflow-providers-apache-sqoop-3.2.0rc1/airflow/providers/apache/sqoop/
+-rw-r--r--   0 root         (0) root         (0)     1395 2023-05-16 15:39:21.000000 apache-airflow-providers-apache-sqoop-3.2.0rc1/airflow/providers/apache/sqoop/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2594 2023-05-16 15:53:17.000000 apache-airflow-providers-apache-sqoop-3.2.0rc1/airflow/providers/apache/sqoop/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:18.000000 apache-airflow-providers-apache-sqoop-3.2.0rc1/airflow/providers/apache/sqoop/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-sqoop-3.2.0rc1/airflow/providers/apache/sqoop/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15813 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-sqoop-3.2.0rc1/airflow/providers/apache/sqoop/hooks/sqoop.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:18.000000 apache-airflow-providers-apache-sqoop-3.2.0rc1/airflow/providers/apache/sqoop/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-sqoop-3.2.0rc1/airflow/providers/apache/sqoop/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11404 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-sqoop-3.2.0rc1/airflow/providers/apache/sqoop/operators/sqoop.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:18.000000 apache-airflow-providers-apache-sqoop-3.2.0rc1/apache_airflow_providers_apache_sqoop.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10172 2023-05-16 15:53:18.000000 apache-airflow-providers-apache-sqoop-3.2.0rc1/apache_airflow_providers_apache_sqoop.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      792 2023-05-16 15:53:18.000000 apache-airflow-providers-apache-sqoop-3.2.0rc1/apache_airflow_providers_apache_sqoop.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:53:18.000000 apache-airflow-providers-apache-sqoop-3.2.0rc1/apache_airflow_providers_apache_sqoop.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2023-05-16 15:53:18.000000 apache-airflow-providers-apache-sqoop-3.2.0rc1/apache_airflow_providers_apache_sqoop.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:53:18.000000 apache-airflow-providers-apache-sqoop-3.2.0rc1/apache_airflow_providers_apache_sqoop.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       27 2023-05-16 15:53:18.000000 apache-airflow-providers-apache-sqoop-3.2.0rc1/apache_airflow_providers_apache_sqoop.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-16 15:53:18.000000 apache-airflow-providers-apache-sqoop-3.2.0rc1/apache_airflow_providers_apache_sqoop.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5308 2023-05-15 09:39:26.000000 apache-airflow-providers-apache-sqoop-3.2.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1864 2023-05-16 15:53:18.000000 apache-airflow-providers-apache-sqoop-3.2.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-05-16 15:53:17.000000 apache-airflow-providers-apache-sqoop-3.2.0rc1/setup.py
```

### Comparing `apache-airflow-providers-apache-sqoop-3.1.1rc1/LICENSE` & `apache-airflow-providers-apache-sqoop-3.2.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-sqoop-3.1.1rc1/MANIFEST.in` & `apache-airflow-providers-apache-sqoop-3.2.0rc1/MANIFEST.in`

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

### Comparing `apache-airflow-providers-apache-sqoop-3.1.1rc1/PKG-INFO` & `apache-airflow-providers-apache-sqoop-3.2.0rc1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-sqoop
-Version: 3.1.1rc1
+Version: 3.2.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-sqoop package
 Home-page: https://airflow.apache.org/
+Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Download-URL: https://archive.apache.org/dist/airflow/providers
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-sqoop/3.1.1/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-sqoop/3.2.0/
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
@@ -49,28 +48,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-sqoop``
 
-Release: ``3.1.1rc1``
+Release: ``3.2.0rc1``
 
 
 `Apache Sqoop <https://sqoop.apache.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.sqoop`` provider. All classes for this provider package
 are in ``airflow.providers.apache.sqoop`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-sqoop/3.1.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-sqoop/3.2.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -80,15 +79,15 @@
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
-``apache-airflow``  ``>=2.3.0``
+``apache-airflow``  ``>=2.4.0``
 ==================  ==================
 
  .. Licensed to the Apache Software Foundation (ASF) under one
     or more contributor license agreements.  See the NOTICE file
     distributed with this work for additional information
     regarding copyright ownership.  The ASF licenses this file
     to you under the Apache License, Version 2.0 (the
@@ -109,26 +108,44 @@
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
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add mechanism to suspend providers (#30422)``
+
 3.1.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
 * ``Move libjars parameter in Sqoop Hook to Hook parameter (#29500)``
 
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
@@ -143,16 +160,17 @@
 
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
    * ``Prepare docs for May 2022 provider's release (#24231)``
    * ``Update package description to remove double min-airflow specification (#24292)``
 
@@ -260,9 +278,7 @@
 
 Updated documentation and readme files.
 
 1.0.0
 .....
 
 Initial version of the provider.
-
-
```

### Comparing `apache-airflow-providers-apache-sqoop-3.1.1rc1/README.rst` & `apache-airflow-providers-apache-sqoop-3.2.0rc1/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -15,28 +15,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-sqoop``
 
-Release: ``3.1.1rc1``
+Release: ``3.2.0rc1``
 
 
 `Apache Sqoop <https://sqoop.apache.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.sqoop`` provider. All classes for this provider package
 are in ``airflow.providers.apache.sqoop`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-sqoop/3.1.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-sqoop/3.2.0/>`_.
 
 
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
 ==================  ==================
 
  .. Licensed to the Apache Software Foundation (ASF) under one
     or more contributor license agreements.  See the NOTICE file
     distributed with this work for additional information
     regarding copyright ownership.  The ASF licenses this file
     to you under the Apache License, Version 2.0 (the
@@ -75,26 +75,44 @@
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
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add mechanism to suspend providers (#30422)``
+
 3.1.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
 * ``Move libjars parameter in Sqoop Hook to Hook parameter (#29500)``
 
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
@@ -109,16 +127,17 @@
 
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
    * ``Prepare docs for May 2022 provider's release (#24231)``
    * ``Update package description to remove double min-airflow specification (#24292)``
```

### Comparing `apache-airflow-providers-apache-sqoop-3.1.1rc1/airflow/providers/apache/sqoop/__init__.py` & `apache-airflow-providers-apache-sqoop-3.2.0rc1/airflow/providers/apache/sqoop/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-sqoop-3.1.1rc1/airflow/providers/apache/sqoop/get_provider_info.py` & `apache-airflow-providers-apache-sqoop-3.2.0rc1/airflow/providers/apache/sqoop/get_provider_info.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,29 +23,31 @@
 
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-apache-sqoop",
         "name": "Apache Sqoop",
         "description": "`Apache Sqoop <https://sqoop.apache.org/>`__\n",
+        "suspended": False,
         "versions": [
+            "3.2.0",
             "3.1.1",
             "3.1.0",
             "3.0.0",
             "2.1.3",
             "2.1.2",
             "2.1.1",
             "2.1.0",
             "2.0.2",
             "2.0.1",
             "2.0.0",
             "1.0.1",
             "1.0.0",
         ],
-        "dependencies": ["apache-airflow>=2.3.0"],
+        "dependencies": ["apache-airflow>=2.4.0"],
         "integrations": [
             {
                 "integration-name": "Apache Sqoop",
                 "external-doc-url": "https://sqoop.apache.org/",
                 "logo": "/integration-logos/apache/sqoop.png",
                 "how-to-guide": ["/docs/apache-airflow-providers-apache-sqoop/operators.rst"],
                 "tags": ["apache"],
```

### Comparing `apache-airflow-providers-apache-sqoop-3.1.1rc1/airflow/providers/apache/sqoop/hooks/__init__.py` & `apache-airflow-providers-apache-sqoop-3.2.0rc1/airflow/providers/apache/sqoop/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-sqoop-3.1.1rc1/airflow/providers/apache/sqoop/hooks/sqoop.py` & `apache-airflow-providers-apache-sqoop-3.2.0rc1/airflow/providers/apache/sqoop/hooks/sqoop.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-sqoop-3.1.1rc1/airflow/providers/apache/sqoop/operators/sqoop.py` & `apache-airflow-providers-apache-sqoop-3.2.0rc1/airflow/providers/apache/sqoop/operators/sqoop.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-sqoop-3.1.1rc1/apache_airflow_providers_apache_sqoop.egg-info/PKG-INFO` & `apache-airflow-providers-apache-sqoop-3.2.0rc1/apache_airflow_providers_apache_sqoop.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-sqoop
-Version: 3.1.1rc1
+Version: 3.2.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-sqoop package
 Home-page: https://airflow.apache.org/
+Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Download-URL: https://archive.apache.org/dist/airflow/providers
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-sqoop/3.1.1/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-sqoop/3.2.0/
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
@@ -49,28 +48,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-sqoop``
 
-Release: ``3.1.1rc1``
+Release: ``3.2.0rc1``
 
 
 `Apache Sqoop <https://sqoop.apache.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.sqoop`` provider. All classes for this provider package
 are in ``airflow.providers.apache.sqoop`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-sqoop/3.1.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-sqoop/3.2.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -80,15 +79,15 @@
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
-``apache-airflow``  ``>=2.3.0``
+``apache-airflow``  ``>=2.4.0``
 ==================  ==================
 
  .. Licensed to the Apache Software Foundation (ASF) under one
     or more contributor license agreements.  See the NOTICE file
     distributed with this work for additional information
     regarding copyright ownership.  The ASF licenses this file
     to you under the Apache License, Version 2.0 (the
@@ -109,26 +108,44 @@
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
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add mechanism to suspend providers (#30422)``
+
 3.1.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
 * ``Move libjars parameter in Sqoop Hook to Hook parameter (#29500)``
 
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
@@ -143,16 +160,17 @@
 
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
    * ``Prepare docs for May 2022 provider's release (#24231)``
    * ``Update package description to remove double min-airflow specification (#24292)``
 
@@ -260,9 +278,7 @@
 
 Updated documentation and readme files.
 
 1.0.0
 .....
 
 Initial version of the provider.
-
-
```

### Comparing `apache-airflow-providers-apache-sqoop-3.1.1rc1/apache_airflow_providers_apache_sqoop.egg-info/SOURCES.txt` & `apache-airflow-providers-apache-sqoop-3.2.0rc1/apache_airflow_providers_apache_sqoop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-sqoop-3.1.1rc1/pyproject.toml` & `apache-airflow-providers-apache-sqoop-3.2.0rc1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -28,28 +28,30 @@
 
 [tool.ruff]
 typing-modules = ["airflow.typing_compat"]
 line-length = 110
 extend-exclude = [
     ".eggs",
     "airflow/_vendor/*",
-
+    "airflow/providers/google/ads/_vendor/*",
     # The files generated by stubgen aren't 100% valid syntax it turns out, and we don't ship them, so we can
     # ignore them in ruff
     "airflow/providers/common/sql/*/*.pyi"
 ]
 
 # TODO: Bump to Python 3.8 when support for Python 3.7 is dropped in Airflow.
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
@@ -63,14 +65,46 @@
     "D212",
     "D213",
     "D214",
     "D215",
     "E731",
 ]
 
+[tool.pytest.ini_options]
+# * Disable `flaky` plugin for pytest. This plugin conflicts with `rerunfailures` because provide same marker.
+# * Disable `nose` builtin plugin for pytest. This feature deprecated in 7.2 and will be removed in pytest>=8
+# * And we focus on use native pytest capabilities rather than adopt another frameworks.
+addopts = "-rasl --verbosity=2 -p no:flaky -p no:nose --asyncio-mode=strict"
+norecursedirs = [
+    ".eggs",
+    "airflow",
+    "tests/dags_with_system_exit",
+    "tests/test_utils",
+    "tests/dags_corrupted",
+    "tests/dags",
+    "tests/system/providers/google/cloud/dataproc/resources",
+    "tests/system/providers/google/cloud/gcs/resources",
+]
+log_level = "INFO"
+filterwarnings = [
+    "error::pytest.PytestCollectionWarning",
+    "ignore::DeprecationWarning:flask_appbuilder.filemanager",
+    "ignore::DeprecationWarning:flask_appbuilder.widgets",
+    # https://github.com/dpgaspar/Flask-AppBuilder/pull/1940
+    "ignore::DeprecationWarning:flask_sqlalchemy",
+    # https://github.com/dpgaspar/Flask-AppBuilder/pull/1903
+    "ignore::DeprecationWarning:apispec.utils",
+]
+python_files = [
+    "*.py",
+]
+testpaths = [
+    "tests",
+]
+
 [tool.ruff.isort]
 known-first-party = ["airflow", "airflow_breeze", "docker_tests", "docs", "kubernetes_tests", "tests"]
 required-imports = ["from __future__ import annotations"]
 combine-as-imports = true
 
 # TODO: for now, https://github.com/charliermarsh/ruff/issues/1817
 known-third-party = [
@@ -101,14 +135,18 @@
 "airflow/models/sqla_models.py" = ["F401"]
 
 
 # The test_python.py is needed because adding __future__.annotations breaks runtime checks that are
 # needed for the test to work
 "tests/decorators/test_python.py" = ["I002"]
 
+# The Pydantic representations of SqlAlchemy Models are not parsed well with Pydantic
+# when __future__.annotations is used so we need to skip them from upgrading
+"airflow/serialization/pydantic/*.py" = ["I002"]
+
 # Ignore pydoc style from these
 "*.pyi" = ["D"]
 "tests/*" = ["D"]
 "scripts/*" = ["D"]
 "dev/*" = ["D"]
 "docs/*" = ["D"]
 "provider_packages/*" = ["D"]
```

### Comparing `apache-airflow-providers-apache-sqoop-3.1.1rc1/setup.cfg` & `apache-airflow-providers-apache-sqoop-3.2.0rc1/setup.cfg`

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-apache-sqoop/3.1.1/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-apache-sqoop/3.2.0/
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
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.apache.sqoop.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.apache.sqoop
```

### Comparing `apache-airflow-providers-apache-sqoop-3.1.1rc1/setup.py` & `apache-airflow-providers-apache-sqoop-3.2.0rc1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,23 +22,28 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-apache-sqoop package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "3.1.1"
+version = "3.2.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-apache-sqoop setup."""
     setup(
         version=version,
         extras_require={},
         packages=find_namespace_packages(
-            include=["airflow.providers.apache.sqoop", "airflow.providers.apache.sqoop.*"]
+            include=[
+                "airflow.providers.apache.sqoop",
+                "airflow.providers.apache.sqoop.*",
+                "airflow.providers.apache.sqoop_vendor",
+                "airflow.providers.apache.sqoop_vendor.*",
+            ],
         ),
     )
 
 
 if __name__ == "__main__":
     do_setup()
```

