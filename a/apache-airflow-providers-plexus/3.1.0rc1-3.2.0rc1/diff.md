# Comparing `tmp/apache-airflow-providers-plexus-3.1.0rc1.tar.gz` & `tmp/apache-airflow-providers-plexus-3.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-plexus-3.1.0rc1.tar", last modified: Tue Nov 15 00:15:22 2022, max compression
+gzip compressed data, was "dist/apache-airflow-providers-plexus-3.2.0rc1.tar", last modified: Tue May 16 15:54:55 2023, max compression
```

## Comparing `apache-airflow-providers-plexus-3.1.0rc1.tar` & `apache-airflow-providers-plexus-3.2.0rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:15:22.000000 apache-airflow-providers-plexus-3.1.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2022-05-27 19:54:38.000000 apache-airflow-providers-plexus-3.1.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1122 2022-11-15 00:15:21.000000 apache-airflow-providers-plexus-3.1.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2022-05-27 19:54:38.000000 apache-airflow-providers-plexus-3.1.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     8802 2022-11-15 00:15:22.000000 apache-airflow-providers-plexus-3.1.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7255 2022-11-15 00:15:21.000000 apache-airflow-providers-plexus-3.1.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:15:22.000000 apache-airflow-providers-plexus-3.1.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:15:22.000000 apache-airflow-providers-plexus-3.1.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:15:22.000000 apache-airflow-providers-plexus-3.1.0rc1/airflow/providers/plexus/
--rw-r--r--   0 root         (0) root         (0)      785 2022-09-13 10:31:21.000000 apache-airflow-providers-plexus-3.1.0rc1/airflow/providers/plexus/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1958 2022-11-15 00:15:21.000000 apache-airflow-providers-plexus-3.1.0rc1/airflow/providers/plexus/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:15:22.000000 apache-airflow-providers-plexus-3.1.0rc1/airflow/providers/plexus/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2022-09-13 10:31:21.000000 apache-airflow-providers-plexus-3.1.0rc1/airflow/providers/plexus/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2715 2022-09-14 19:22:24.000000 apache-airflow-providers-plexus-3.1.0rc1/airflow/providers/plexus/hooks/plexus.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:15:22.000000 apache-airflow-providers-plexus-3.1.0rc1/airflow/providers/plexus/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2022-09-13 10:31:21.000000 apache-airflow-providers-plexus-3.1.0rc1/airflow/providers/plexus/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6055 2022-10-26 03:21:46.000000 apache-airflow-providers-plexus-3.1.0rc1/airflow/providers/plexus/operators/job.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:15:22.000000 apache-airflow-providers-plexus-3.1.0rc1/apache_airflow_providers_plexus.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8802 2022-11-15 00:15:22.000000 apache-airflow-providers-plexus-3.1.0rc1/apache_airflow_providers_plexus.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      713 2022-11-15 00:15:22.000000 apache-airflow-providers-plexus-3.1.0rc1/apache_airflow_providers_plexus.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-15 00:15:22.000000 apache-airflow-providers-plexus-3.1.0rc1/apache_airflow_providers_plexus.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      104 2022-11-15 00:15:22.000000 apache-airflow-providers-plexus-3.1.0rc1/apache_airflow_providers_plexus.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-15 00:15:22.000000 apache-airflow-providers-plexus-3.1.0rc1/apache_airflow_providers_plexus.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       38 2022-11-15 00:15:22.000000 apache-airflow-providers-plexus-3.1.0rc1/apache_airflow_providers_plexus.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2022-11-15 00:15:22.000000 apache-airflow-providers-plexus-3.1.0rc1/apache_airflow_providers_plexus.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1836 2022-10-26 03:21:46.000000 apache-airflow-providers-plexus-3.1.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1840 2022-11-15 00:15:22.000000 apache-airflow-providers-plexus-3.1.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1464 2022-11-15 00:15:21.000000 apache-airflow-providers-plexus-3.1.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:55.000000 apache-airflow-providers-plexus-3.2.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-plexus-3.2.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-05-16 15:54:54.000000 apache-airflow-providers-plexus-3.2.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-plexus-3.2.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     9525 2023-05-16 15:54:55.000000 apache-airflow-providers-plexus-3.2.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7998 2023-05-16 15:54:54.000000 apache-airflow-providers-plexus-3.2.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:55.000000 apache-airflow-providers-plexus-3.2.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:55.000000 apache-airflow-providers-plexus-3.2.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:55.000000 apache-airflow-providers-plexus-3.2.0rc1/airflow/providers/plexus/
+-rw-r--r--   0 root         (0) root         (0)     1389 2023-05-16 15:39:21.000000 apache-airflow-providers-plexus-3.2.0rc1/airflow/providers/plexus/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2126 2023-05-16 15:54:54.000000 apache-airflow-providers-plexus-3.2.0rc1/airflow/providers/plexus/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:55.000000 apache-airflow-providers-plexus-3.2.0rc1/airflow/providers/plexus/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-plexus-3.2.0rc1/airflow/providers/plexus/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2715 2023-02-24 18:43:53.000000 apache-airflow-providers-plexus-3.2.0rc1/airflow/providers/plexus/hooks/plexus.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:55.000000 apache-airflow-providers-plexus-3.2.0rc1/airflow/providers/plexus/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-plexus-3.2.0rc1/airflow/providers/plexus/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6055 2023-02-24 18:43:53.000000 apache-airflow-providers-plexus-3.2.0rc1/airflow/providers/plexus/operators/job.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:55.000000 apache-airflow-providers-plexus-3.2.0rc1/apache_airflow_providers_plexus.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9525 2023-05-16 15:54:54.000000 apache-airflow-providers-plexus-3.2.0rc1/apache_airflow_providers_plexus.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      713 2023-05-16 15:54:55.000000 apache-airflow-providers-plexus-3.2.0rc1/apache_airflow_providers_plexus.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:54:54.000000 apache-airflow-providers-plexus-3.2.0rc1/apache_airflow_providers_plexus.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-05-16 15:54:54.000000 apache-airflow-providers-plexus-3.2.0rc1/apache_airflow_providers_plexus.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:54:54.000000 apache-airflow-providers-plexus-3.2.0rc1/apache_airflow_providers_plexus.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       41 2023-05-16 15:54:54.000000 apache-airflow-providers-plexus-3.2.0rc1/apache_airflow_providers_plexus.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-16 15:54:54.000000 apache-airflow-providers-plexus-3.2.0rc1/apache_airflow_providers_plexus.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5308 2023-05-15 09:39:26.000000 apache-airflow-providers-plexus-3.2.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1843 2023-05-16 15:54:55.000000 apache-airflow-providers-plexus-3.2.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1638 2023-05-16 15:54:54.000000 apache-airflow-providers-plexus-3.2.0rc1/setup.py
```

### Comparing `apache-airflow-providers-plexus-3.1.0rc1/LICENSE` & `apache-airflow-providers-plexus-3.2.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-plexus-3.1.0rc1/MANIFEST.in` & `apache-airflow-providers-plexus-3.2.0rc1/MANIFEST.in`

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

### Comparing `apache-airflow-providers-plexus-3.1.0rc1/PKG-INFO` & `apache-airflow-providers-plexus-3.2.0rc1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-plexus
-Version: 3.1.0rc1
+Version: 3.2.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-plexus package
 Home-page: https://airflow.apache.org/
+Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Download-URL: https://archive.apache.org/dist/airflow/providers
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-plexus/3.1.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-plexus/3.2.0/
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
 
 
 Package ``apache-airflow-providers-plexus``
 
-Release: ``3.1.0rc1``
+Release: ``3.2.0rc1``
 
 
 `Plexus <https://plexus.corescientific.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``plexus`` provider. All classes for this provider package
 are in ``airflow.providers.plexus`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-plexus/3.1.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-plexus/3.2.0/>`_.
 
 
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
 ``arrow``           ``>=0.16.0``
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
@@ -136,16 +153,17 @@
 
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
    * ``Migrate Plexus example DAGs to new design #22457 (#24147)``
    * ``Add explanatory note for contributors about updating Changelog (#24229)``
    * ``Prepare docs for May 2022 provider's release (#24231)``
    * ``Update package description to remove double min-airflow specification (#24292)``
@@ -234,9 +252,7 @@
 
 Updated documentation and readme files.
 
 1.0.0
 .....
 
 Initial version of the provider.
-
-
```

### Comparing `apache-airflow-providers-plexus-3.1.0rc1/README.rst` & `apache-airflow-providers-plexus-3.2.0rc1/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -15,28 +15,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-plexus``
 
-Release: ``3.1.0rc1``
+Release: ``3.2.0rc1``
 
 
 `Plexus <https://plexus.corescientific.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``plexus`` provider. All classes for this provider package
 are in ``airflow.providers.plexus`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-plexus/3.1.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-plexus/3.2.0/>`_.
 
 
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
 ``arrow``           ``>=0.16.0``
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
@@ -102,16 +120,17 @@
 
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
    * ``Migrate Plexus example DAGs to new design #22457 (#24147)``
    * ``Add explanatory note for contributors about updating Changelog (#24229)``
    * ``Prepare docs for May 2022 provider's release (#24231)``
    * ``Update package description to remove double min-airflow specification (#24292)``
```

### Comparing `apache-airflow-providers-plexus-3.1.0rc1/airflow/providers/plexus/__init__.py` & `apache-airflow-providers-plexus-3.2.0rc1/airflow/providers/plexus/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-plexus-3.1.0rc1/airflow/providers/plexus/get_provider_info.py` & `apache-airflow-providers-plexus-3.2.0rc1/airflow/providers/plexus/get_provider_info.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,16 +23,28 @@
 
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-plexus",
         "name": "Plexus",
         "description": "`Plexus <https://plexus.corescientific.com/>`__\n",
-        "versions": ["3.1.0", "3.0.0", "2.0.4", "2.0.3", "2.0.2", "2.0.1", "2.0.0", "1.0.1", "1.0.0"],
-        "dependencies": ["apache-airflow>=2.3.0", "arrow>=0.16.0"],
+        "suspended": False,
+        "versions": [
+            "3.2.0",
+            "3.1.0",
+            "3.0.0",
+            "2.0.4",
+            "2.0.3",
+            "2.0.2",
+            "2.0.1",
+            "2.0.0",
+            "1.0.1",
+            "1.0.0",
+        ],
+        "dependencies": ["apache-airflow>=2.4.0", "arrow>=0.16.0"],
         "integrations": [
             {
                 "integration-name": "Plexus",
                 "external-doc-url": "https://plexus.corescientific.com/",
                 "logo": "/integration-logos/plexus/Plexus.png",
                 "tags": ["service"],
             }
```

### Comparing `apache-airflow-providers-plexus-3.1.0rc1/airflow/providers/plexus/hooks/__init__.py` & `apache-airflow-providers-plexus-3.2.0rc1/airflow/providers/plexus/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-plexus-3.1.0rc1/airflow/providers/plexus/hooks/plexus.py` & `apache-airflow-providers-plexus-3.2.0rc1/airflow/providers/plexus/hooks/plexus.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-plexus-3.1.0rc1/airflow/providers/plexus/operators/job.py` & `apache-airflow-providers-plexus-3.2.0rc1/airflow/providers/plexus/operators/job.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-plexus-3.1.0rc1/apache_airflow_providers_plexus.egg-info/PKG-INFO` & `apache-airflow-providers-plexus-3.2.0rc1/apache_airflow_providers_plexus.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-plexus
-Version: 3.1.0rc1
+Version: 3.2.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-plexus package
 Home-page: https://airflow.apache.org/
+Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Download-URL: https://archive.apache.org/dist/airflow/providers
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-plexus/3.1.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-plexus/3.2.0/
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
 
 
 Package ``apache-airflow-providers-plexus``
 
-Release: ``3.1.0rc1``
+Release: ``3.2.0rc1``
 
 
 `Plexus <https://plexus.corescientific.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``plexus`` provider. All classes for this provider package
 are in ``airflow.providers.plexus`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-plexus/3.1.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-plexus/3.2.0/>`_.
 
 
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
 ``arrow``           ``>=0.16.0``
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
@@ -136,16 +153,17 @@
 
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
    * ``Migrate Plexus example DAGs to new design #22457 (#24147)``
    * ``Add explanatory note for contributors about updating Changelog (#24229)``
    * ``Prepare docs for May 2022 provider's release (#24231)``
    * ``Update package description to remove double min-airflow specification (#24292)``
@@ -234,9 +252,7 @@
 
 Updated documentation and readme files.
 
 1.0.0
 .....
 
 Initial version of the provider.
-
-
```

### Comparing `apache-airflow-providers-plexus-3.1.0rc1/apache_airflow_providers_plexus.egg-info/SOURCES.txt` & `apache-airflow-providers-plexus-3.2.0rc1/apache_airflow_providers_plexus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-plexus-3.1.0rc1/pyproject.toml` & `apache-airflow-providers-plexus-3.2.0rc1/airflow/providers/plexus/__init__.py`

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
+        f"The package `apache-airflow-providers-plexus:{version}` requires Apache Airflow 2.4.0+"
+    )
```

### Comparing `apache-airflow-providers-plexus-3.1.0rc1/setup.cfg` & `apache-airflow-providers-plexus-3.2.0rc1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-plexus/3.1.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-plexus/3.2.0/
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
 	arrow>=0.16.0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.plexus.get_provider_info:get_provider_info
 
 [files]
```

### Comparing `apache-airflow-providers-plexus-3.1.0rc1/setup.py` & `apache-airflow-providers-plexus-3.2.0rc1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,21 +22,28 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-plexus package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "3.1.0"
+version = "3.2.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-plexus setup."""
     setup(
         version=version,
         extras_require={},
-        packages=find_namespace_packages(include=["airflow.providers.plexus", "airflow.providers.plexus.*"]),
+        packages=find_namespace_packages(
+            include=[
+                "airflow.providers.plexus",
+                "airflow.providers.plexus.*",
+                "airflow.providers.plexus_vendor",
+                "airflow.providers.plexus_vendor.*",
+            ],
+        ),
     )
 
 
 if __name__ == "__main__":
     do_setup()
```

