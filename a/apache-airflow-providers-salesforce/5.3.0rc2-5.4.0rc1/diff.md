# Comparing `tmp/apache-airflow-providers-salesforce-5.3.0rc2.tar.gz` & `tmp/apache-airflow-providers-salesforce-5.4.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-salesforce-5.3.0rc2.tar", last modified: Mon Jan  2 13:09:44 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-salesforce-5.4.0rc1.tar", last modified: Tue May 16 15:55:04 2023, max compression
```

## Comparing `apache-airflow-providers-salesforce-5.3.0rc2.tar` & `apache-airflow-providers-salesforce-5.4.0rc1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-02 13:09:44.000000 apache-airflow-providers-salesforce-5.3.0rc2/
--rw-r--r--   0 root         (0) root         (0)    10850 2022-10-05 12:15:16.000000 apache-airflow-providers-salesforce-5.3.0rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1122 2023-01-02 13:09:43.000000 apache-airflow-providers-salesforce-5.3.0rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2022-10-05 12:15:16.000000 apache-airflow-providers-salesforce-5.3.0rc2/NOTICE
--rw-r--r--   0 root         (0) root         (0)    10874 2023-01-02 13:09:44.000000 apache-airflow-providers-salesforce-5.3.0rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9315 2023-01-02 13:09:43.000000 apache-airflow-providers-salesforce-5.3.0rc2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-02 13:09:44.000000 apache-airflow-providers-salesforce-5.3.0rc2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-02 13:09:44.000000 apache-airflow-providers-salesforce-5.3.0rc2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-02 13:09:44.000000 apache-airflow-providers-salesforce-5.3.0rc2/airflow/providers/salesforce/
--rw-r--r--   0 root         (0) root         (0)      787 2022-10-05 12:15:15.000000 apache-airflow-providers-salesforce-5.3.0rc2/airflow/providers/salesforce/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2975 2023-01-02 13:09:43.000000 apache-airflow-providers-salesforce-5.3.0rc2/airflow/providers/salesforce/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-02 13:09:44.000000 apache-airflow-providers-salesforce-5.3.0rc2/airflow/providers/salesforce/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2022-10-05 12:15:15.000000 apache-airflow-providers-salesforce-5.3.0rc2/airflow/providers/salesforce/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18074 2022-12-20 13:50:43.000000 apache-airflow-providers-salesforce-5.3.0rc2/airflow/providers/salesforce/hooks/salesforce.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-02 13:09:44.000000 apache-airflow-providers-salesforce-5.3.0rc2/airflow/providers/salesforce/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2022-10-05 12:15:15.000000 apache-airflow-providers-salesforce-5.3.0rc2/airflow/providers/salesforce/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4762 2022-11-03 13:17:26.000000 apache-airflow-providers-salesforce-5.3.0rc2/airflow/providers/salesforce/operators/bulk.py
--rw-r--r--   0 root         (0) root         (0)     2553 2022-11-03 13:17:26.000000 apache-airflow-providers-salesforce-5.3.0rc2/airflow/providers/salesforce/operators/salesforce_apex_rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-02 13:09:44.000000 apache-airflow-providers-salesforce-5.3.0rc2/apache_airflow_providers_salesforce.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10874 2023-01-02 13:09:44.000000 apache-airflow-providers-salesforce-5.3.0rc2/apache_airflow_providers_salesforce.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      833 2023-01-02 13:09:44.000000 apache-airflow-providers-salesforce-5.3.0rc2/apache_airflow_providers_salesforce.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-02 13:09:44.000000 apache-airflow-providers-salesforce-5.3.0rc2/apache_airflow_providers_salesforce.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      108 2023-01-02 13:09:44.000000 apache-airflow-providers-salesforce-5.3.0rc2/apache_airflow_providers_salesforce.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-02 13:09:44.000000 apache-airflow-providers-salesforce-5.3.0rc2/apache_airflow_providers_salesforce.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       67 2023-01-02 13:09:44.000000 apache-airflow-providers-salesforce-5.3.0rc2/apache_airflow_providers_salesforce.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-01-02 13:09:44.000000 apache-airflow-providers-salesforce-5.3.0rc2/apache_airflow_providers_salesforce.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1860 2022-12-20 13:50:44.000000 apache-airflow-providers-salesforce-5.3.0rc2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1894 2023-01-02 13:09:44.000000 apache-airflow-providers-salesforce-5.3.0rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1502 2023-01-02 13:09:43.000000 apache-airflow-providers-salesforce-5.3.0rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:04.000000 apache-airflow-providers-salesforce-5.4.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-salesforce-5.4.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-05-16 15:55:03.000000 apache-airflow-providers-salesforce-5.4.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-salesforce-5.4.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    11597 2023-05-16 15:55:04.000000 apache-airflow-providers-salesforce-5.4.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10058 2023-05-16 15:55:03.000000 apache-airflow-providers-salesforce-5.4.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:04.000000 apache-airflow-providers-salesforce-5.4.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:04.000000 apache-airflow-providers-salesforce-5.4.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:04.000000 apache-airflow-providers-salesforce-5.4.0rc1/airflow/providers/salesforce/
+-rw-r--r--   0 root         (0) root         (0)     1393 2023-05-16 15:39:21.000000 apache-airflow-providers-salesforce-5.4.0rc1/airflow/providers/salesforce/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3024 2023-05-16 15:55:03.000000 apache-airflow-providers-salesforce-5.4.0rc1/airflow/providers/salesforce/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:04.000000 apache-airflow-providers-salesforce-5.4.0rc1/airflow/providers/salesforce/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-salesforce-5.4.0rc1/airflow/providers/salesforce/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18074 2023-02-24 18:43:53.000000 apache-airflow-providers-salesforce-5.4.0rc1/airflow/providers/salesforce/hooks/salesforce.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:04.000000 apache-airflow-providers-salesforce-5.4.0rc1/airflow/providers/salesforce/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-salesforce-5.4.0rc1/airflow/providers/salesforce/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4762 2023-02-24 18:43:53.000000 apache-airflow-providers-salesforce-5.4.0rc1/airflow/providers/salesforce/operators/bulk.py
+-rw-r--r--   0 root         (0) root         (0)     2553 2023-02-24 18:43:53.000000 apache-airflow-providers-salesforce-5.4.0rc1/airflow/providers/salesforce/operators/salesforce_apex_rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:04.000000 apache-airflow-providers-salesforce-5.4.0rc1/apache_airflow_providers_salesforce.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11597 2023-05-16 15:55:04.000000 apache-airflow-providers-salesforce-5.4.0rc1/apache_airflow_providers_salesforce.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      833 2023-05-16 15:55:04.000000 apache-airflow-providers-salesforce-5.4.0rc1/apache_airflow_providers_salesforce.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:55:04.000000 apache-airflow-providers-salesforce-5.4.0rc1/apache_airflow_providers_salesforce.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-05-16 15:55:04.000000 apache-airflow-providers-salesforce-5.4.0rc1/apache_airflow_providers_salesforce.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:55:04.000000 apache-airflow-providers-salesforce-5.4.0rc1/apache_airflow_providers_salesforce.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       67 2023-05-16 15:55:04.000000 apache-airflow-providers-salesforce-5.4.0rc1/apache_airflow_providers_salesforce.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-16 15:55:04.000000 apache-airflow-providers-salesforce-5.4.0rc1/apache_airflow_providers_salesforce.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5308 2023-05-15 09:39:26.000000 apache-airflow-providers-salesforce-5.4.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1894 2023-05-16 15:55:04.000000 apache-airflow-providers-salesforce-5.4.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1662 2023-05-16 15:55:03.000000 apache-airflow-providers-salesforce-5.4.0rc1/setup.py
```

### Comparing `apache-airflow-providers-salesforce-5.3.0rc2/LICENSE` & `apache-airflow-providers-salesforce-5.4.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-salesforce-5.3.0rc2/MANIFEST.in` & `apache-airflow-providers-salesforce-5.4.0rc1/MANIFEST.in`

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

### Comparing `apache-airflow-providers-salesforce-5.3.0rc2/PKG-INFO` & `apache-airflow-providers-salesforce-5.4.0rc1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-salesforce
-Version: 5.3.0rc2
+Version: 5.4.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-salesforce package
 Home-page: https://airflow.apache.org/
+Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Download-URL: https://archive.apache.org/dist/airflow/providers
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-salesforce/5.3.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-salesforce/5.4.0/
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
 
 
 Package ``apache-airflow-providers-salesforce``
 
-Release: ``5.3.0rc2``
+Release: ``5.4.0rc1``
 
 
 `Salesforce <https://www.salesforce.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``salesforce`` provider. All classes for this provider package
 are in ``airflow.providers.salesforce`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-salesforce/5.3.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-salesforce/5.4.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -80,15 +79,15 @@
 
 Requirements
 ------------
 
 =====================  ==================
 PIP package            Version required
 =====================  ==================
-``apache-airflow``     ``>=2.3.0``
+``apache-airflow``     ``>=2.4.0``
 ``simple-salesforce``  ``>=1.0.0``
 ``pandas``             ``>=0.17.1``
 =====================  ==================
 
  .. Licensed to the Apache Software Foundation (ASF) under one
     or more contributor license agreements.  See the NOTICE file
     distributed with this work for additional information
@@ -111,30 +110,48 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+5.4.0
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
 5.3.0
 .....
 
 Features
 ~~~~~~~~
 
 * ``Add test_connection to SalesforceHook (#27921)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
 
 5.2.0
 .....
 
-This release of provider is only available for Airflow 2.3+ as explained in the
-`Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/README.md#support-for-providers>`_.
+.. note::
+  This release of provider is only available for Airflow 2.3+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Misc
 ~~~~
 
 * ``Move min airflow version to 2.3.0 for all providers (#27196)``
 * ``Allow and prefer non-prefixed extra fields for SalesforceHook (#27075)``
 
@@ -184,16 +201,17 @@
 
 4.0.0
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
    * ``Migrate Salesforce example DAGs to new design #22463 (#24127)``
    * ``Add explanatory note for contributors about updating Changelog (#24229)``
    * ``Prepare docs for May 2022 provider's release (#24231)``
    * ``Update package description to remove double min-airflow specification (#24292)``
@@ -337,9 +355,7 @@
 Updated documentation and readme files.
 
 
 1.0.0
 .....
 
 Initial version of the provider.
-
-
```

### Comparing `apache-airflow-providers-salesforce-5.3.0rc2/README.rst` & `apache-airflow-providers-salesforce-5.4.0rc1/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -15,28 +15,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-salesforce``
 
-Release: ``5.3.0rc2``
+Release: ``5.4.0rc1``
 
 
 `Salesforce <https://www.salesforce.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``salesforce`` provider. All classes for this provider package
 are in ``airflow.providers.salesforce`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-salesforce/5.3.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-salesforce/5.4.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -46,15 +46,15 @@
 
 Requirements
 ------------
 
 =====================  ==================
 PIP package            Version required
 =====================  ==================
-``apache-airflow``     ``>=2.3.0``
+``apache-airflow``     ``>=2.4.0``
 ``simple-salesforce``  ``>=1.0.0``
 ``pandas``             ``>=0.17.1``
 =====================  ==================
 
  .. Licensed to the Apache Software Foundation (ASF) under one
     or more contributor license agreements.  See the NOTICE file
     distributed with this work for additional information
@@ -77,30 +77,48 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+5.4.0
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
 5.3.0
 .....
 
 Features
 ~~~~~~~~
 
 * ``Add test_connection to SalesforceHook (#27921)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
 
 5.2.0
 .....
 
-This release of provider is only available for Airflow 2.3+ as explained in the
-`Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/README.md#support-for-providers>`_.
+.. note::
+  This release of provider is only available for Airflow 2.3+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Misc
 ~~~~
 
 * ``Move min airflow version to 2.3.0 for all providers (#27196)``
 * ``Allow and prefer non-prefixed extra fields for SalesforceHook (#27075)``
 
@@ -150,16 +168,17 @@
 
 4.0.0
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
    * ``Migrate Salesforce example DAGs to new design #22463 (#24127)``
    * ``Add explanatory note for contributors about updating Changelog (#24229)``
    * ``Prepare docs for May 2022 provider's release (#24231)``
    * ``Update package description to remove double min-airflow specification (#24292)``
```

### Comparing `apache-airflow-providers-salesforce-5.3.0rc2/airflow/providers/salesforce/__init__.py` & `apache-airflow-providers-salesforce-5.4.0rc1/airflow/providers/salesforce/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-salesforce-5.3.0rc2/airflow/providers/salesforce/get_provider_info.py` & `apache-airflow-providers-salesforce-5.4.0rc1/airflow/providers/salesforce/get_provider_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,17 @@
 
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-salesforce",
         "name": "Salesforce",
         "description": "`Salesforce <https://www.salesforce.com/>`__\n",
+        "suspended": False,
         "versions": [
+            "5.4.0",
             "5.3.0",
             "5.2.0",
             "5.1.0",
             "5.0.0",
             "4.0.0",
             "3.4.4",
             "3.4.3",
@@ -42,15 +44,15 @@
             "3.2.0",
             "3.1.0",
             "3.0.0",
             "2.0.0",
             "1.0.1",
             "1.0.0",
         ],
-        "dependencies": ["apache-airflow>=2.3.0", "simple-salesforce>=1.0.0", "pandas>=0.17.1"],
+        "dependencies": ["apache-airflow>=2.4.0", "simple-salesforce>=1.0.0", "pandas>=0.17.1"],
         "integrations": [
             {
                 "integration-name": "Salesforce",
                 "external-doc-url": "https://www.salesforce.com/",
                 "how-to-guide": [
                     "/docs/apache-airflow-providers-salesforce/operators/salesforce_apex_rest.rst",
                     "/docs/apache-airflow-providers-salesforce/operators/bulk.rst",
```

### Comparing `apache-airflow-providers-salesforce-5.3.0rc2/airflow/providers/salesforce/hooks/__init__.py` & `apache-airflow-providers-salesforce-5.4.0rc1/airflow/providers/salesforce/operators/__init__.py`

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

### Comparing `apache-airflow-providers-salesforce-5.3.0rc2/airflow/providers/salesforce/hooks/salesforce.py` & `apache-airflow-providers-salesforce-5.4.0rc1/airflow/providers/salesforce/hooks/salesforce.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-salesforce-5.3.0rc2/airflow/providers/salesforce/operators/bulk.py` & `apache-airflow-providers-salesforce-5.4.0rc1/airflow/providers/salesforce/operators/bulk.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-salesforce-5.3.0rc2/airflow/providers/salesforce/operators/salesforce_apex_rest.py` & `apache-airflow-providers-salesforce-5.4.0rc1/airflow/providers/salesforce/operators/salesforce_apex_rest.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-salesforce-5.3.0rc2/apache_airflow_providers_salesforce.egg-info/PKG-INFO` & `apache-airflow-providers-salesforce-5.4.0rc1/apache_airflow_providers_salesforce.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-salesforce
-Version: 5.3.0rc2
+Version: 5.4.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-salesforce package
 Home-page: https://airflow.apache.org/
+Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Download-URL: https://archive.apache.org/dist/airflow/providers
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-salesforce/5.3.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-salesforce/5.4.0/
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
 
 
 Package ``apache-airflow-providers-salesforce``
 
-Release: ``5.3.0rc2``
+Release: ``5.4.0rc1``
 
 
 `Salesforce <https://www.salesforce.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``salesforce`` provider. All classes for this provider package
 are in ``airflow.providers.salesforce`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-salesforce/5.3.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-salesforce/5.4.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -80,15 +79,15 @@
 
 Requirements
 ------------
 
 =====================  ==================
 PIP package            Version required
 =====================  ==================
-``apache-airflow``     ``>=2.3.0``
+``apache-airflow``     ``>=2.4.0``
 ``simple-salesforce``  ``>=1.0.0``
 ``pandas``             ``>=0.17.1``
 =====================  ==================
 
  .. Licensed to the Apache Software Foundation (ASF) under one
     or more contributor license agreements.  See the NOTICE file
     distributed with this work for additional information
@@ -111,30 +110,48 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+5.4.0
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
 5.3.0
 .....
 
 Features
 ~~~~~~~~
 
 * ``Add test_connection to SalesforceHook (#27921)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
 
 5.2.0
 .....
 
-This release of provider is only available for Airflow 2.3+ as explained in the
-`Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/README.md#support-for-providers>`_.
+.. note::
+  This release of provider is only available for Airflow 2.3+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Misc
 ~~~~
 
 * ``Move min airflow version to 2.3.0 for all providers (#27196)``
 * ``Allow and prefer non-prefixed extra fields for SalesforceHook (#27075)``
 
@@ -184,16 +201,17 @@
 
 4.0.0
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
    * ``Migrate Salesforce example DAGs to new design #22463 (#24127)``
    * ``Add explanatory note for contributors about updating Changelog (#24229)``
    * ``Prepare docs for May 2022 provider's release (#24231)``
    * ``Update package description to remove double min-airflow specification (#24292)``
@@ -337,9 +355,7 @@
 Updated documentation and readme files.
 
 
 1.0.0
 .....
 
 Initial version of the provider.
-
-
```

### Comparing `apache-airflow-providers-salesforce-5.3.0rc2/apache_airflow_providers_salesforce.egg-info/SOURCES.txt` & `apache-airflow-providers-salesforce-5.4.0rc1/apache_airflow_providers_salesforce.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-salesforce-5.3.0rc2/setup.cfg` & `apache-airflow-providers-salesforce-5.4.0rc1/setup.cfg`

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-salesforce/5.3.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-salesforce/5.4.0/
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
@@ -42,22 +42,22 @@
 include_package_data = True
 python_requires = ~=3.7
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
-	apache-airflow>=2.3.0.dev0
+	apache-airflow>=2.4.0.dev0
 	pandas>=0.17.1
 	simple-salesforce>=1.0.0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.salesforce.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.salesforce
 
 [egg_info]
-tag_build = rc2
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-salesforce-5.3.0rc2/setup.py` & `apache-airflow-providers-salesforce-5.4.0rc1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,23 +22,28 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-salesforce package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "5.3.0"
+version = "5.4.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-salesforce setup."""
     setup(
         version=version,
         extras_require={},
         packages=find_namespace_packages(
-            include=["airflow.providers.salesforce", "airflow.providers.salesforce.*"]
+            include=[
+                "airflow.providers.salesforce",
+                "airflow.providers.salesforce.*",
+                "airflow.providers.salesforce_vendor",
+                "airflow.providers.salesforce_vendor.*",
+            ],
         ),
     )
 
 
 if __name__ == "__main__":
     do_setup()
```

