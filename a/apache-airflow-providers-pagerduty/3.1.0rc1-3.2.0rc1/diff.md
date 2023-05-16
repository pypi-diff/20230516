# Comparing `tmp/apache-airflow-providers-pagerduty-3.1.0rc1.tar.gz` & `tmp/apache-airflow-providers-pagerduty-3.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-pagerduty-3.1.0rc1.tar", last modified: Tue Nov 15 00:15:18 2022, max compression
+gzip compressed data, was "dist/apache-airflow-providers-pagerduty-3.2.0rc1.tar", last modified: Tue May 16 15:54:51 2023, max compression
```

## Comparing `apache-airflow-providers-pagerduty-3.1.0rc1.tar` & `apache-airflow-providers-pagerduty-3.2.0rc1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:15:18.000000 apache-airflow-providers-pagerduty-3.1.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2022-05-27 19:54:38.000000 apache-airflow-providers-pagerduty-3.1.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1122 2022-11-15 00:15:17.000000 apache-airflow-providers-pagerduty-3.1.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2022-05-27 19:54:38.000000 apache-airflow-providers-pagerduty-3.1.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     8751 2022-11-15 00:15:18.000000 apache-airflow-providers-pagerduty-3.1.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7195 2022-11-15 00:15:17.000000 apache-airflow-providers-pagerduty-3.1.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:15:18.000000 apache-airflow-providers-pagerduty-3.1.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:15:18.000000 apache-airflow-providers-pagerduty-3.1.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:15:18.000000 apache-airflow-providers-pagerduty-3.1.0rc1/airflow/providers/pagerduty/
--rw-r--r--   0 root         (0) root         (0)      787 2022-09-13 10:31:21.000000 apache-airflow-providers-pagerduty-3.1.0rc1/airflow/providers/pagerduty/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2538 2022-11-15 00:15:17.000000 apache-airflow-providers-pagerduty-3.1.0rc1/airflow/providers/pagerduty/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:15:18.000000 apache-airflow-providers-pagerduty-3.1.0rc1/airflow/providers/pagerduty/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2022-09-13 10:31:21.000000 apache-airflow-providers-pagerduty-3.1.0rc1/airflow/providers/pagerduty/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6871 2022-10-28 02:00:43.000000 apache-airflow-providers-pagerduty-3.1.0rc1/airflow/providers/pagerduty/hooks/pagerduty.py
--rw-r--r--   0 root         (0) root         (0)     6264 2022-10-28 02:00:43.000000 apache-airflow-providers-pagerduty-3.1.0rc1/airflow/providers/pagerduty/hooks/pagerduty_events.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:15:18.000000 apache-airflow-providers-pagerduty-3.1.0rc1/apache_airflow_providers_pagerduty.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8751 2022-11-15 00:15:18.000000 apache-airflow-providers-pagerduty-3.1.0rc1/apache_airflow_providers_pagerduty.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      714 2022-11-15 00:15:18.000000 apache-airflow-providers-pagerduty-3.1.0rc1/apache_airflow_providers_pagerduty.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-15 00:15:18.000000 apache-airflow-providers-pagerduty-3.1.0rc1/apache_airflow_providers_pagerduty.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2022-11-15 00:15:18.000000 apache-airflow-providers-pagerduty-3.1.0rc1/apache_airflow_providers_pagerduty.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-15 00:15:18.000000 apache-airflow-providers-pagerduty-3.1.0rc1/apache_airflow_providers_pagerduty.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       39 2022-11-15 00:15:18.000000 apache-airflow-providers-pagerduty-3.1.0rc1/apache_airflow_providers_pagerduty.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2022-11-15 00:15:18.000000 apache-airflow-providers-pagerduty-3.1.0rc1/apache_airflow_providers_pagerduty.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1836 2022-10-26 03:21:46.000000 apache-airflow-providers-pagerduty-3.1.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1859 2022-11-15 00:15:18.000000 apache-airflow-providers-pagerduty-3.1.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1498 2022-11-15 00:15:17.000000 apache-airflow-providers-pagerduty-3.1.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:51.000000 apache-airflow-providers-pagerduty-3.2.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-pagerduty-3.2.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-05-16 15:54:50.000000 apache-airflow-providers-pagerduty-3.2.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-pagerduty-3.2.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     9607 2023-05-16 15:54:51.000000 apache-airflow-providers-pagerduty-3.2.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8071 2023-05-16 15:54:50.000000 apache-airflow-providers-pagerduty-3.2.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:51.000000 apache-airflow-providers-pagerduty-3.2.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:51.000000 apache-airflow-providers-pagerduty-3.2.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:51.000000 apache-airflow-providers-pagerduty-3.2.0rc1/airflow/providers/pagerduty/
+-rw-r--r--   0 root         (0) root         (0)     1392 2023-05-16 15:39:21.000000 apache-airflow-providers-pagerduty-3.2.0rc1/airflow/providers/pagerduty/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2587 2023-05-16 15:54:50.000000 apache-airflow-providers-pagerduty-3.2.0rc1/airflow/providers/pagerduty/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:51.000000 apache-airflow-providers-pagerduty-3.2.0rc1/airflow/providers/pagerduty/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-pagerduty-3.2.0rc1/airflow/providers/pagerduty/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6921 2023-05-03 19:47:07.000000 apache-airflow-providers-pagerduty-3.2.0rc1/airflow/providers/pagerduty/hooks/pagerduty.py
+-rw-r--r--   0 root         (0) root         (0)     6276 2023-05-12 08:38:07.000000 apache-airflow-providers-pagerduty-3.2.0rc1/airflow/providers/pagerduty/hooks/pagerduty_events.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:51.000000 apache-airflow-providers-pagerduty-3.2.0rc1/apache_airflow_providers_pagerduty.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9607 2023-05-16 15:54:51.000000 apache-airflow-providers-pagerduty-3.2.0rc1/apache_airflow_providers_pagerduty.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      714 2023-05-16 15:54:51.000000 apache-airflow-providers-pagerduty-3.2.0rc1/apache_airflow_providers_pagerduty.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:54:51.000000 apache-airflow-providers-pagerduty-3.2.0rc1/apache_airflow_providers_pagerduty.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      106 2023-05-16 15:54:51.000000 apache-airflow-providers-pagerduty-3.2.0rc1/apache_airflow_providers_pagerduty.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:54:51.000000 apache-airflow-providers-pagerduty-3.2.0rc1/apache_airflow_providers_pagerduty.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       42 2023-05-16 15:54:51.000000 apache-airflow-providers-pagerduty-3.2.0rc1/apache_airflow_providers_pagerduty.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-16 15:54:51.000000 apache-airflow-providers-pagerduty-3.2.0rc1/apache_airflow_providers_pagerduty.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5308 2023-05-15 09:39:26.000000 apache-airflow-providers-pagerduty-3.2.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1862 2023-05-16 15:54:51.000000 apache-airflow-providers-pagerduty-3.2.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1656 2023-05-16 15:54:50.000000 apache-airflow-providers-pagerduty-3.2.0rc1/setup.py
```

### Comparing `apache-airflow-providers-pagerduty-3.1.0rc1/LICENSE` & `apache-airflow-providers-pagerduty-3.2.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-pagerduty-3.1.0rc1/MANIFEST.in` & `apache-airflow-providers-pagerduty-3.2.0rc1/MANIFEST.in`

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

### Comparing `apache-airflow-providers-pagerduty-3.1.0rc1/PKG-INFO` & `apache-airflow-providers-pagerduty-3.2.0rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-pagerduty
-Version: 3.1.0rc1
+Version: 3.2.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-pagerduty package
 Home-page: https://airflow.apache.org/
+Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Download-URL: https://archive.apache.org/dist/airflow/providers
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-pagerduty/3.1.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-pagerduty/3.2.0/
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
 
 
 Package ``apache-airflow-providers-pagerduty``
 
-Release: ``3.1.0rc1``
+Release: ``3.2.0rc1``
 
 
 `Pagerduty <https://www.pagerduty.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``pagerduty`` provider. All classes for this provider package
 are in ``airflow.providers.pagerduty`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-pagerduty/3.1.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-pagerduty/3.2.0/>`_.
 
 
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
 ``pdpyras``         ``>=4.1.2``
 ==================  ==================
 
  .. Licensed to the Apache Software Foundation (ASF) under one
     or more contributor license agreements.  See the NOTICE file
     distributed with this work for additional information
     regarding copyright ownership.  The ASF licenses this file
@@ -110,19 +109,39 @@
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
+* `` Fixed typo in 'PagerdutyEventsHook' docstring (#31209)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add mechanism to suspend providers (#30422)``
+
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
@@ -138,16 +157,17 @@
 
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
 
@@ -237,9 +257,7 @@
 
 Updated documentation and readme files.
 
 1.0.0
 .....
 
 Initial version of the provider.
-
-
```

### Comparing `apache-airflow-providers-pagerduty-3.1.0rc1/README.rst` & `apache-airflow-providers-pagerduty-3.2.0rc1/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -15,28 +15,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-pagerduty``
 
-Release: ``3.1.0rc1``
+Release: ``3.2.0rc1``
 
 
 `Pagerduty <https://www.pagerduty.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``pagerduty`` provider. All classes for this provider package
 are in ``airflow.providers.pagerduty`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-pagerduty/3.1.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-pagerduty/3.2.0/>`_.
 
 
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
 ``pdpyras``         ``>=4.1.2``
 ==================  ==================
 
  .. Licensed to the Apache Software Foundation (ASF) under one
     or more contributor license agreements.  See the NOTICE file
     distributed with this work for additional information
     regarding copyright ownership.  The ASF licenses this file
@@ -76,19 +76,39 @@
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
+* `` Fixed typo in 'PagerdutyEventsHook' docstring (#31209)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add mechanism to suspend providers (#30422)``
+
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
@@ -104,16 +124,17 @@
 
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

### Comparing `apache-airflow-providers-pagerduty-3.1.0rc1/airflow/providers/pagerduty/__init__.py` & `apache-airflow-providers-pagerduty-3.2.0rc1/airflow/providers/pagerduty/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-pagerduty-3.1.0rc1/airflow/providers/pagerduty/get_provider_info.py` & `apache-airflow-providers-pagerduty-3.2.0rc1/airflow/providers/pagerduty/get_provider_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,27 +23,29 @@
 
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-pagerduty",
         "name": "Pagerduty",
         "description": "`Pagerduty <https://www.pagerduty.com/>`__\n",
+        "suspended": False,
         "versions": [
+            "3.2.0",
             "3.1.0",
             "3.0.0",
             "2.1.3",
             "2.1.2",
             "2.1.1",
             "2.1.0",
             "2.0.1",
             "2.0.0",
             "1.0.1",
             "1.0.0",
         ],
-        "dependencies": ["apache-airflow>=2.3.0", "pdpyras>=4.1.2"],
+        "dependencies": ["apache-airflow>=2.4.0", "pdpyras>=4.1.2"],
         "integrations": [
             {
                 "integration-name": "Pagerduty",
                 "external-doc-url": "https://www.pagerduty.com/",
                 "logo": "/integration-logos/pagerduty/PagerDuty.png",
                 "tags": ["service"],
             }
```

### Comparing `apache-airflow-providers-pagerduty-3.1.0rc1/airflow/providers/pagerduty/hooks/pagerduty.py` & `apache-airflow-providers-pagerduty-3.2.0rc1/airflow/providers/pagerduty/hooks/pagerduty.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from __future__ import annotations
 
 import warnings
 from typing import Any
 
 import pdpyras
 
-from airflow.exceptions import AirflowException
+from airflow.exceptions import AirflowException, AirflowProviderDeprecationWarning
 from airflow.hooks.base import BaseHook
 from airflow.providers.pagerduty.hooks.pagerduty_events import PagerdutyEventsHook
 
 
 class PagerdutyHook(BaseHook):
     """
     The PagerdutyHook can be used to interact with both the PagerDuty API and the PagerDuty Events API.
@@ -136,15 +136,15 @@
             `text`: [Optional] Plain text that describes the purpose of the link, and can be used as the
             link's text.
         :return: PagerDuty Events API v2 response.
         """
         warnings.warn(
             "This method will be deprecated. Please use the "
             "`airflow.providers.pagerduty.hooks.PagerdutyEventsHook` to interact with the Events API",
-            DeprecationWarning,
+            AirflowProviderDeprecationWarning,
             stacklevel=2,
         )
 
         routing_key = routing_key or self.routing_key
 
         return PagerdutyEventsHook(integration_key=routing_key).create_event(
             summary=summary,
```

### Comparing `apache-airflow-providers-pagerduty-3.1.0rc1/airflow/providers/pagerduty/hooks/pagerduty_events.py` & `apache-airflow-providers-pagerduty-3.2.0rc1/airflow/providers/pagerduty/hooks/pagerduty_events.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,16 @@
     """
     This class can be used to interact with the Pagerduty Events API.
 
     It takes both an Events API token and a PagerDuty connection with the Events API token
      (i.e. Integration key) as the password/Pagerduty API token. If both supplied, the token will be used.
 
     :param integration_key: PagerDuty Events API token
-    :param pagerduty_conn_id: connection that has PagerDuty integration key in the Pagerduty API token field
+    :param pagerduty_events_conn_id: connection that has PagerDuty integration key in the Pagerduty
+     API token field
     """
 
     conn_name_attr = "pagerduty_events_conn_id"
     default_conn_name = "pagerduty_events_default"
     conn_type = "pagerduty_events"
     hook_name = "Pagerduty Events"
```

### Comparing `apache-airflow-providers-pagerduty-3.1.0rc1/apache_airflow_providers_pagerduty.egg-info/PKG-INFO` & `apache-airflow-providers-pagerduty-3.2.0rc1/apache_airflow_providers_pagerduty.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-pagerduty
-Version: 3.1.0rc1
+Version: 3.2.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-pagerduty package
 Home-page: https://airflow.apache.org/
+Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Download-URL: https://archive.apache.org/dist/airflow/providers
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-pagerduty/3.1.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-pagerduty/3.2.0/
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
 
 
 Package ``apache-airflow-providers-pagerduty``
 
-Release: ``3.1.0rc1``
+Release: ``3.2.0rc1``
 
 
 `Pagerduty <https://www.pagerduty.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``pagerduty`` provider. All classes for this provider package
 are in ``airflow.providers.pagerduty`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-pagerduty/3.1.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-pagerduty/3.2.0/>`_.
 
 
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
 ``pdpyras``         ``>=4.1.2``
 ==================  ==================
 
  .. Licensed to the Apache Software Foundation (ASF) under one
     or more contributor license agreements.  See the NOTICE file
     distributed with this work for additional information
     regarding copyright ownership.  The ASF licenses this file
@@ -110,19 +109,39 @@
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
+* `` Fixed typo in 'PagerdutyEventsHook' docstring (#31209)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add mechanism to suspend providers (#30422)``
+
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
@@ -138,16 +157,17 @@
 
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
 
@@ -237,9 +257,7 @@
 
 Updated documentation and readme files.
 
 1.0.0
 .....
 
 Initial version of the provider.
-
-
```

### Comparing `apache-airflow-providers-pagerduty-3.1.0rc1/apache_airflow_providers_pagerduty.egg-info/SOURCES.txt` & `apache-airflow-providers-pagerduty-3.2.0rc1/apache_airflow_providers_pagerduty.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-pagerduty-3.1.0rc1/pyproject.toml` & `apache-airflow-providers-pagerduty-3.2.0rc1/airflow/providers/pagerduty/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+#
 # Licensed to the Apache Software Foundation (ASF) under one
 # or more contributor license agreements.  See the NOTICE file
 # distributed with this work for additional information
 # regarding copyright ownership.  The ASF licenses this file
 # to you under the Apache License, Version 2.0 (the
 # "License"); you may not use this file except in compliance
 # with the License.  You may obtain a copy of the License at
@@ -10,30 +11,28 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
-[tool.black]
-line-length = 110
-target-version = ['py37', 'py38', 'py39', 'py310']
-# The build system section is needed in order to workaround the side-effect introduced by recent
-# setup tools version. The recent setuptools version update (64.0.0) broke paths of editable installations
-# and we have to pin it to 63.4.3 version
-# The problem is tracked (and this limitation might be removed if it is solved) in:
-# https://github.com/pypa/setuptools/issues/3548
-[build-system]
-requires = ['setuptools==63.4.3']
-build-backend = "setuptools.build_meta"
-[tool.isort]
-add_imports = ["from __future__ import annotations"]
-append_only = true
-line_length = 110
-combine_as_imports = true
-default_section = "THIRDPARTY"
-known_first_party = ["airflow", "airflow_breeze", "docker_tests", "docs", "kubernetes_tests", "tests"]
-# The test_python.py is needed because adding __future__.annotations breaks runtime checks that are
-# needed for the test to work
-skip = ["build", ".tox", "venv", "tests/decorators/test_python.py"]
-skip_glob = ["*.pyi"]
-profile = "black"
+#
+# NOTE! THIS FILE IS AUTOMATICALLY GENERATED AND WILL BE
+# OVERWRITTEN WHEN PREPARING DOCUMENTATION FOR THE PACKAGES.
+#
+# IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
+# `PROVIDER__INIT__PY_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
+#
+from __future__ import annotations
+
+import packaging.version
+
+import airflow
+
+__all__ = ["version"]
+
+version = "3.2.0"
+
+if packaging.version.parse(airflow.version.version) < packaging.version.parse("2.4.0"):
+    raise RuntimeError(
+        f"The package `apache-airflow-providers-pagerduty:{version}` requires Apache Airflow 2.4.0+"
+    )
```

### Comparing `apache-airflow-providers-pagerduty-3.1.0rc1/setup.cfg` & `apache-airflow-providers-pagerduty-3.2.0rc1/setup.cfg`

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-pagerduty/3.1.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-pagerduty/3.2.0/
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
-	apache-airflow>=2.3.0.*
+	apache-airflow>=2.4.0.dev0
 	pdpyras>=4.1.2
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.pagerduty.get_provider_info:get_provider_info
 
 [files]
```

### Comparing `apache-airflow-providers-pagerduty-3.1.0rc1/setup.py` & `apache-airflow-providers-pagerduty-3.2.0rc1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,23 +22,28 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-pagerduty package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "3.1.0"
+version = "3.2.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-pagerduty setup."""
     setup(
         version=version,
         extras_require={},
         packages=find_namespace_packages(
-            include=["airflow.providers.pagerduty", "airflow.providers.pagerduty.*"]
+            include=[
+                "airflow.providers.pagerduty",
+                "airflow.providers.pagerduty.*",
+                "airflow.providers.pagerduty_vendor",
+                "airflow.providers.pagerduty_vendor.*",
+            ],
         ),
     )
 
 
 if __name__ == "__main__":
     do_setup()
```

