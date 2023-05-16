# Comparing `tmp/apache-airflow-providers-samba-4.1.0rc1.tar.gz` & `tmp/apache-airflow-providers-samba-4.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-samba-4.1.0rc1.tar", last modified: Tue Nov 15 00:15:33 2022, max compression
+gzip compressed data, was "dist/apache-airflow-providers-samba-4.2.0rc1.tar", last modified: Tue May 16 15:55:05 2023, max compression
```

## Comparing `apache-airflow-providers-samba-4.1.0rc1.tar` & `apache-airflow-providers-samba-4.2.0rc1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:15:33.000000 apache-airflow-providers-samba-4.1.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2022-05-27 19:54:38.000000 apache-airflow-providers-samba-4.1.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1122 2022-11-15 00:15:32.000000 apache-airflow-providers-samba-4.1.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2022-05-27 19:54:38.000000 apache-airflow-providers-samba-4.1.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     8858 2022-11-15 00:15:33.000000 apache-airflow-providers-samba-4.1.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7314 2022-11-15 00:15:32.000000 apache-airflow-providers-samba-4.1.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:15:33.000000 apache-airflow-providers-samba-4.1.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:15:33.000000 apache-airflow-providers-samba-4.1.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:15:33.000000 apache-airflow-providers-samba-4.1.0rc1/airflow/providers/samba/
--rw-r--r--   0 root         (0) root         (0)      787 2022-09-13 10:31:21.000000 apache-airflow-providers-samba-4.1.0rc1/airflow/providers/samba/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2060 2022-11-15 00:15:32.000000 apache-airflow-providers-samba-4.1.0rc1/airflow/providers/samba/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:15:33.000000 apache-airflow-providers-samba-4.1.0rc1/airflow/providers/samba/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2022-09-13 10:31:21.000000 apache-airflow-providers-samba-4.1.0rc1/airflow/providers/samba/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8453 2022-10-26 03:21:46.000000 apache-airflow-providers-samba-4.1.0rc1/airflow/providers/samba/hooks/samba.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:15:33.000000 apache-airflow-providers-samba-4.1.0rc1/apache_airflow_providers_samba.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8858 2022-11-15 00:15:33.000000 apache-airflow-providers-samba-4.1.0rc1/apache_airflow_providers_samba.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      612 2022-11-15 00:15:33.000000 apache-airflow-providers-samba-4.1.0rc1/apache_airflow_providers_samba.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-15 00:15:33.000000 apache-airflow-providers-samba-4.1.0rc1/apache_airflow_providers_samba.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      103 2022-11-15 00:15:33.000000 apache-airflow-providers-samba-4.1.0rc1/apache_airflow_providers_samba.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-15 00:15:33.000000 apache-airflow-providers-samba-4.1.0rc1/apache_airflow_providers_samba.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       43 2022-11-15 00:15:33.000000 apache-airflow-providers-samba-4.1.0rc1/apache_airflow_providers_samba.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2022-11-15 00:15:33.000000 apache-airflow-providers-samba-4.1.0rc1/apache_airflow_providers_samba.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1836 2022-10-26 03:21:46.000000 apache-airflow-providers-samba-4.1.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1839 2022-11-15 00:15:33.000000 apache-airflow-providers-samba-4.1.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1460 2022-11-15 00:15:32.000000 apache-airflow-providers-samba-4.1.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:05.000000 apache-airflow-providers-samba-4.2.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-samba-4.2.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-05-16 15:55:04.000000 apache-airflow-providers-samba-4.2.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-samba-4.2.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     9581 2023-05-16 15:55:05.000000 apache-airflow-providers-samba-4.2.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8057 2023-05-16 15:55:04.000000 apache-airflow-providers-samba-4.2.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:05.000000 apache-airflow-providers-samba-4.2.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:05.000000 apache-airflow-providers-samba-4.2.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:05.000000 apache-airflow-providers-samba-4.2.0rc1/airflow/providers/samba/
+-rw-r--r--   0 root         (0) root         (0)     1388 2023-05-16 15:39:21.000000 apache-airflow-providers-samba-4.2.0rc1/airflow/providers/samba/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2109 2023-05-16 15:55:04.000000 apache-airflow-providers-samba-4.2.0rc1/airflow/providers/samba/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:05.000000 apache-airflow-providers-samba-4.2.0rc1/airflow/providers/samba/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-samba-4.2.0rc1/airflow/providers/samba/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8453 2023-02-24 18:43:53.000000 apache-airflow-providers-samba-4.2.0rc1/airflow/providers/samba/hooks/samba.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:05.000000 apache-airflow-providers-samba-4.2.0rc1/apache_airflow_providers_samba.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9581 2023-05-16 15:55:05.000000 apache-airflow-providers-samba-4.2.0rc1/apache_airflow_providers_samba.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      612 2023-05-16 15:55:05.000000 apache-airflow-providers-samba-4.2.0rc1/apache_airflow_providers_samba.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:55:05.000000 apache-airflow-providers-samba-4.2.0rc1/apache_airflow_providers_samba.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      102 2023-05-16 15:55:05.000000 apache-airflow-providers-samba-4.2.0rc1/apache_airflow_providers_samba.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:55:05.000000 apache-airflow-providers-samba-4.2.0rc1/apache_airflow_providers_samba.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       46 2023-05-16 15:55:05.000000 apache-airflow-providers-samba-4.2.0rc1/apache_airflow_providers_samba.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-16 15:55:05.000000 apache-airflow-providers-samba-4.2.0rc1/apache_airflow_providers_samba.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5308 2023-05-15 09:39:26.000000 apache-airflow-providers-samba-4.2.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1842 2023-05-16 15:55:05.000000 apache-airflow-providers-samba-4.2.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1632 2023-05-16 15:55:04.000000 apache-airflow-providers-samba-4.2.0rc1/setup.py
```

### Comparing `apache-airflow-providers-samba-4.1.0rc1/LICENSE` & `apache-airflow-providers-samba-4.2.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-samba-4.1.0rc1/MANIFEST.in` & `apache-airflow-providers-samba-4.2.0rc1/MANIFEST.in`

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

### Comparing `apache-airflow-providers-samba-4.1.0rc1/PKG-INFO` & `apache-airflow-providers-samba-4.2.0rc1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-samba
-Version: 4.1.0rc1
+Version: 4.2.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-samba package
 Home-page: https://airflow.apache.org/
+Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Download-URL: https://archive.apache.org/dist/airflow/providers
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-samba/4.1.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-samba/4.2.0/
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
 
 
 Package ``apache-airflow-providers-samba``
 
-Release: ``4.1.0rc1``
+Release: ``4.2.0rc1``
 
 
 `Samba <https://www.samba.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``samba`` provider. All classes for this provider package
 are in ``airflow.providers.samba`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-samba/4.1.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-samba/4.2.0/>`_.
 
 
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
 ``smbprotocol``     ``>=1.5.0``
 ==================  ==================
 
  .. Licensed to the Apache Software Foundation (ASF) under one
     or more contributor license agreements.  See the NOTICE file
     distributed with this work for additional information
     regarding copyright ownership.  The ASF licenses this file
@@ -110,19 +109,37 @@
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
 4.1.0
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
@@ -137,16 +154,17 @@
 
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
    * ``Add explanatory note for contributors about updating Changelog (#24229)``
    * ``Prepare docs for May 2022 provider's release (#24231)``
    * ``Update package description to remove double min-airflow specification (#24292)``
 
@@ -247,9 +265,7 @@
 
 Updated documentation and readme files.
 
 1.0.0
 .....
 
 Initial version of the provider.
-
-
```

### Comparing `apache-airflow-providers-samba-4.1.0rc1/README.rst` & `apache-airflow-providers-samba-4.2.0rc1/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -15,28 +15,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-samba``
 
-Release: ``4.1.0rc1``
+Release: ``4.2.0rc1``
 
 
 `Samba <https://www.samba.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``samba`` provider. All classes for this provider package
 are in ``airflow.providers.samba`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-samba/4.1.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-samba/4.2.0/>`_.
 
 
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
 ``smbprotocol``     ``>=1.5.0``
 ==================  ==================
 
  .. Licensed to the Apache Software Foundation (ASF) under one
     or more contributor license agreements.  See the NOTICE file
     distributed with this work for additional information
     regarding copyright ownership.  The ASF licenses this file
@@ -76,19 +76,37 @@
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
 4.1.0
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
@@ -103,16 +121,17 @@
 
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
    * ``Add explanatory note for contributors about updating Changelog (#24229)``
    * ``Prepare docs for May 2022 provider's release (#24231)``
    * ``Update package description to remove double min-airflow specification (#24292)``
```

### Comparing `apache-airflow-providers-samba-4.1.0rc1/airflow/providers/samba/__init__.py` & `apache-airflow-providers-samba-4.2.0rc1/airflow/providers/samba/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-samba-4.1.0rc1/airflow/providers/samba/get_provider_info.py` & `apache-airflow-providers-samba-4.2.0rc1/airflow/providers/samba/get_provider_info.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,27 +23,29 @@
 
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-samba",
         "name": "Samba",
         "description": "`Samba <https://www.samba.org/>`__\n",
+        "suspended": False,
         "versions": [
+            "4.2.0",
             "4.1.0",
             "4.0.0",
             "3.0.4",
             "3.0.3",
             "3.0.2",
             "3.0.1",
             "3.0.0",
             "2.0.0",
             "1.0.1",
             "1.0.0",
         ],
-        "dependencies": ["apache-airflow>=2.3.0", "smbprotocol>=1.5.0"],
+        "dependencies": ["apache-airflow>=2.4.0", "smbprotocol>=1.5.0"],
         "integrations": [
             {
                 "integration-name": "Samba",
                 "external-doc-url": "https://www.samba.org/",
                 "logo": "/integration-logos/samba/Samba.png",
                 "tags": ["protocol"],
             }
```

### Comparing `apache-airflow-providers-samba-4.1.0rc1/airflow/providers/samba/hooks/samba.py` & `apache-airflow-providers-samba-4.2.0rc1/airflow/providers/samba/hooks/samba.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-samba-4.1.0rc1/apache_airflow_providers_samba.egg-info/PKG-INFO` & `apache-airflow-providers-samba-4.2.0rc1/apache_airflow_providers_samba.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-samba
-Version: 4.1.0rc1
+Version: 4.2.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-samba package
 Home-page: https://airflow.apache.org/
+Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Download-URL: https://archive.apache.org/dist/airflow/providers
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-samba/4.1.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-samba/4.2.0/
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
 
 
 Package ``apache-airflow-providers-samba``
 
-Release: ``4.1.0rc1``
+Release: ``4.2.0rc1``
 
 
 `Samba <https://www.samba.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``samba`` provider. All classes for this provider package
 are in ``airflow.providers.samba`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-samba/4.1.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-samba/4.2.0/>`_.
 
 
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
 ``smbprotocol``     ``>=1.5.0``
 ==================  ==================
 
  .. Licensed to the Apache Software Foundation (ASF) under one
     or more contributor license agreements.  See the NOTICE file
     distributed with this work for additional information
     regarding copyright ownership.  The ASF licenses this file
@@ -110,19 +109,37 @@
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
 4.1.0
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
@@ -137,16 +154,17 @@
 
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
    * ``Add explanatory note for contributors about updating Changelog (#24229)``
    * ``Prepare docs for May 2022 provider's release (#24231)``
    * ``Update package description to remove double min-airflow specification (#24292)``
 
@@ -247,9 +265,7 @@
 
 Updated documentation and readme files.
 
 1.0.0
 .....
 
 Initial version of the provider.
-
-
```

### Comparing `apache-airflow-providers-samba-4.1.0rc1/apache_airflow_providers_samba.egg-info/SOURCES.txt` & `apache-airflow-providers-samba-4.2.0rc1/apache_airflow_providers_samba.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-samba-4.1.0rc1/setup.cfg` & `apache-airflow-providers-samba-4.2.0rc1/setup.cfg`

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-samba/4.1.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-samba/4.2.0/
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
 	smbprotocol>=1.5.0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.samba.get_provider_info:get_provider_info
 
 [files]
```

### Comparing `apache-airflow-providers-samba-4.1.0rc1/setup.py` & `apache-airflow-providers-samba-4.2.0rc1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,21 +22,28 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-samba package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "4.1.0"
+version = "4.2.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-samba setup."""
     setup(
         version=version,
         extras_require={},
-        packages=find_namespace_packages(include=["airflow.providers.samba", "airflow.providers.samba.*"]),
+        packages=find_namespace_packages(
+            include=[
+                "airflow.providers.samba",
+                "airflow.providers.samba.*",
+                "airflow.providers.samba_vendor",
+                "airflow.providers.samba_vendor.*",
+            ],
+        ),
     )
 
 
 if __name__ == "__main__":
     do_setup()
```

