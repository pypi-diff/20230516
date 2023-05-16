# Comparing `tmp/apache-airflow-providers-neo4j-3.2.1rc3.tar.gz` & `tmp/apache-airflow-providers-neo4j-3.3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-neo4j-3.2.1rc3.tar", last modified: Sat Nov 26 10:29:48 2022, max compression
+gzip compressed data, was "dist/apache-airflow-providers-neo4j-3.3.0rc1.tar", last modified: Tue May 16 15:54:42 2023, max compression
```

## Comparing `apache-airflow-providers-neo4j-3.2.1rc3.tar` & `apache-airflow-providers-neo4j-3.3.0rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 10:29:48.000000 apache-airflow-providers-neo4j-3.2.1rc3/
--rw-r--r--   0 root         (0) root         (0)    10850 2022-05-27 19:54:38.000000 apache-airflow-providers-neo4j-3.2.1rc3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1122 2022-11-26 10:29:47.000000 apache-airflow-providers-neo4j-3.2.1rc3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2022-05-27 19:54:38.000000 apache-airflow-providers-neo4j-3.2.1rc3/NOTICE
--rw-r--r--   0 root         (0) root         (0)     9967 2022-11-26 10:29:48.000000 apache-airflow-providers-neo4j-3.2.1rc3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8423 2022-11-26 10:29:47.000000 apache-airflow-providers-neo4j-3.2.1rc3/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 10:29:48.000000 apache-airflow-providers-neo4j-3.2.1rc3/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 10:29:48.000000 apache-airflow-providers-neo4j-3.2.1rc3/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 10:29:48.000000 apache-airflow-providers-neo4j-3.2.1rc3/airflow/providers/neo4j/
--rw-r--r--   0 root         (0) root         (0)      787 2022-09-13 10:31:21.000000 apache-airflow-providers-neo4j-3.2.1rc3/airflow/providers/neo4j/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2280 2022-11-26 10:29:47.000000 apache-airflow-providers-neo4j-3.2.1rc3/airflow/providers/neo4j/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 10:29:48.000000 apache-airflow-providers-neo4j-3.2.1rc3/airflow/providers/neo4j/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2022-09-13 10:31:21.000000 apache-airflow-providers-neo4j-3.2.1rc3/airflow/providers/neo4j/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3784 2022-11-25 22:34:39.000000 apache-airflow-providers-neo4j-3.2.1rc3/airflow/providers/neo4j/hooks/neo4j.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 10:29:48.000000 apache-airflow-providers-neo4j-3.2.1rc3/airflow/providers/neo4j/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2022-09-13 10:31:21.000000 apache-airflow-providers-neo4j-3.2.1rc3/airflow/providers/neo4j/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2051 2022-10-26 03:21:46.000000 apache-airflow-providers-neo4j-3.2.1rc3/airflow/providers/neo4j/operators/neo4j.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 10:29:48.000000 apache-airflow-providers-neo4j-3.2.1rc3/apache_airflow_providers_neo4j.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9967 2022-11-26 10:29:48.000000 apache-airflow-providers-neo4j-3.2.1rc3/apache_airflow_providers_neo4j.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      701 2022-11-26 10:29:48.000000 apache-airflow-providers-neo4j-3.2.1rc3/apache_airflow_providers_neo4j.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-26 10:29:48.000000 apache-airflow-providers-neo4j-3.2.1rc3/apache_airflow_providers_neo4j.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      103 2022-11-26 10:29:48.000000 apache-airflow-providers-neo4j-3.2.1rc3/apache_airflow_providers_neo4j.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-26 10:29:48.000000 apache-airflow-providers-neo4j-3.2.1rc3/apache_airflow_providers_neo4j.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       40 2022-11-26 10:29:48.000000 apache-airflow-providers-neo4j-3.2.1rc3/apache_airflow_providers_neo4j.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2022-11-26 10:29:48.000000 apache-airflow-providers-neo4j-3.2.1rc3/apache_airflow_providers_neo4j.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1836 2022-10-26 03:21:46.000000 apache-airflow-providers-neo4j-3.2.1rc3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1836 2022-11-26 10:29:48.000000 apache-airflow-providers-neo4j-3.2.1rc3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1460 2022-11-26 10:29:47.000000 apache-airflow-providers-neo4j-3.2.1rc3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:42.000000 apache-airflow-providers-neo4j-3.3.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-neo4j-3.3.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-05-16 15:54:41.000000 apache-airflow-providers-neo4j-3.3.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-neo4j-3.3.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    10769 2023-05-16 15:54:42.000000 apache-airflow-providers-neo4j-3.3.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9245 2023-05-16 15:54:41.000000 apache-airflow-providers-neo4j-3.3.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:42.000000 apache-airflow-providers-neo4j-3.3.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:42.000000 apache-airflow-providers-neo4j-3.3.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:42.000000 apache-airflow-providers-neo4j-3.3.0rc1/airflow/providers/neo4j/
+-rw-r--r--   0 root         (0) root         (0)     1388 2023-05-16 15:39:21.000000 apache-airflow-providers-neo4j-3.3.0rc1/airflow/providers/neo4j/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2329 2023-05-16 15:54:41.000000 apache-airflow-providers-neo4j-3.3.0rc1/airflow/providers/neo4j/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:42.000000 apache-airflow-providers-neo4j-3.3.0rc1/airflow/providers/neo4j/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-neo4j-3.3.0rc1/airflow/providers/neo4j/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4344 2023-04-24 21:04:25.000000 apache-airflow-providers-neo4j-3.3.0rc1/airflow/providers/neo4j/hooks/neo4j.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:42.000000 apache-airflow-providers-neo4j-3.3.0rc1/airflow/providers/neo4j/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-neo4j-3.3.0rc1/airflow/providers/neo4j/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2051 2023-02-24 18:43:53.000000 apache-airflow-providers-neo4j-3.3.0rc1/airflow/providers/neo4j/operators/neo4j.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:42.000000 apache-airflow-providers-neo4j-3.3.0rc1/apache_airflow_providers_neo4j.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10769 2023-05-16 15:54:42.000000 apache-airflow-providers-neo4j-3.3.0rc1/apache_airflow_providers_neo4j.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      701 2023-05-16 15:54:42.000000 apache-airflow-providers-neo4j-3.3.0rc1/apache_airflow_providers_neo4j.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:54:42.000000 apache-airflow-providers-neo4j-3.3.0rc1/apache_airflow_providers_neo4j.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      102 2023-05-16 15:54:42.000000 apache-airflow-providers-neo4j-3.3.0rc1/apache_airflow_providers_neo4j.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:54:42.000000 apache-airflow-providers-neo4j-3.3.0rc1/apache_airflow_providers_neo4j.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       40 2023-05-16 15:54:42.000000 apache-airflow-providers-neo4j-3.3.0rc1/apache_airflow_providers_neo4j.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-16 15:54:42.000000 apache-airflow-providers-neo4j-3.3.0rc1/apache_airflow_providers_neo4j.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5308 2023-05-15 09:39:26.000000 apache-airflow-providers-neo4j-3.3.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1836 2023-05-16 15:54:42.000000 apache-airflow-providers-neo4j-3.3.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1632 2023-05-16 15:54:41.000000 apache-airflow-providers-neo4j-3.3.0rc1/setup.py
```

### Comparing `apache-airflow-providers-neo4j-3.2.1rc3/LICENSE` & `apache-airflow-providers-neo4j-3.3.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-neo4j-3.2.1rc3/MANIFEST.in` & `apache-airflow-providers-neo4j-3.3.0rc1/MANIFEST.in`

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

### Comparing `apache-airflow-providers-neo4j-3.2.1rc3/PKG-INFO` & `apache-airflow-providers-neo4j-3.3.0rc1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-neo4j
-Version: 3.2.1rc3
+Version: 3.3.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-neo4j package
 Home-page: https://airflow.apache.org/
+Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Download-URL: https://archive.apache.org/dist/airflow/providers
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-neo4j/3.2.1/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-neo4j/3.3.0/
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
 
 
 Package ``apache-airflow-providers-neo4j``
 
-Release: ``3.2.1rc3``
+Release: ``3.3.0rc1``
 
 
 `Neo4j <https://neo4j.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``neo4j`` provider. All classes for this provider package
 are in ``airflow.providers.neo4j`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-neo4j/3.2.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-neo4j/3.3.0/>`_.
 
 
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
 ``neo4j``           ``>=4.2.1``
 ==================  ==================
 
 
 
  .. Licensed to the Apache Software Foundation (ASF) under one
     or more contributor license agreements.  See the NOTICE file
@@ -111,14 +110,36 @@
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
+* ``Removed Mandatory Encryption in Neo4jHook (#30418)``
+
+Bug Fixes
+~~~~~~~~~
+
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add mechanism to suspend providers (#30422)``
+
 3.2.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
 
 * ``Fix typing problem revealed after recent Neo4J release (#27759)``
@@ -126,16 +147,17 @@
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Prepare for follow-up release for November providers (#27774)``
 
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
 
 .. Below changes are excluded from the changelog. Move them to
@@ -160,16 +182,17 @@
 
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
    * ``Migrate Neo4j example DAGs to new design #22454 (#24143)``
    * ``Prepare provider documentation 2022.05.11 (#23631)``
    * ``Bump pre-commit hook versions (#22887)``
@@ -288,9 +311,7 @@
 * ``Corrections in docs and tools after releasing provider RCs (#14082)``
 
 
 1.0.0
 .....
 
 Initial version of the provider.
-
-
```

### Comparing `apache-airflow-providers-neo4j-3.2.1rc3/README.rst` & `apache-airflow-providers-neo4j-3.3.0rc1/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -15,28 +15,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-neo4j``
 
-Release: ``3.2.1rc3``
+Release: ``3.3.0rc1``
 
 
 `Neo4j <https://neo4j.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``neo4j`` provider. All classes for this provider package
 are in ``airflow.providers.neo4j`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-neo4j/3.2.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-neo4j/3.3.0/>`_.
 
 
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
 ``neo4j``           ``>=4.2.1``
 ==================  ==================
 
 
 
  .. Licensed to the Apache Software Foundation (ASF) under one
     or more contributor license agreements.  See the NOTICE file
@@ -77,14 +77,36 @@
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
+* ``Removed Mandatory Encryption in Neo4jHook (#30418)``
+
+Bug Fixes
+~~~~~~~~~
+
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add mechanism to suspend providers (#30422)``
+
 3.2.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
 
 * ``Fix typing problem revealed after recent Neo4J release (#27759)``
@@ -92,16 +114,17 @@
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Prepare for follow-up release for November providers (#27774)``
 
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
 
 .. Below changes are excluded from the changelog. Move them to
@@ -126,16 +149,17 @@
 
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
    * ``Migrate Neo4j example DAGs to new design #22454 (#24143)``
    * ``Prepare provider documentation 2022.05.11 (#23631)``
    * ``Bump pre-commit hook versions (#22887)``
```

### Comparing `apache-airflow-providers-neo4j-3.2.1rc3/airflow/providers/neo4j/__init__.py` & `apache-airflow-providers-neo4j-3.3.0rc1/airflow/providers/neo4j/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-neo4j-3.2.1rc3/airflow/providers/neo4j/get_provider_info.py` & `apache-airflow-providers-neo4j-3.3.0rc1/airflow/providers/neo4j/get_provider_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,30 +23,32 @@
 
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-neo4j",
         "name": "Neo4j",
         "description": "`Neo4j <https://neo4j.com/>`__\n",
+        "suspended": False,
         "versions": [
+            "3.3.0",
             "3.2.1",
             "3.2.0",
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
-        "dependencies": ["apache-airflow>=2.3.0", "neo4j>=4.2.1"],
+        "dependencies": ["apache-airflow>=2.4.0", "neo4j>=4.2.1"],
         "integrations": [
             {
                 "integration-name": "Neo4j",
                 "external-doc-url": "https://neo4j.com/",
                 "how-to-guide": ["/docs/apache-airflow-providers-neo4j/operators/neo4j.rst"],
                 "tags": ["software"],
             }
```

### Comparing `apache-airflow-providers-neo4j-3.2.1rc3/airflow/providers/neo4j/hooks/__init__.py` & `apache-airflow-providers-neo4j-3.3.0rc1/airflow/providers/neo4j/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-neo4j-3.2.1rc3/airflow/providers/neo4j/hooks/neo4j.py` & `apache-airflow-providers-neo4j-3.3.0rc1/airflow/providers/neo4j/hooks/neo4j.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 """This module allows to connect to a Neo4j database."""
 from __future__ import annotations
 
 from typing import Any
+from urllib.parse import urlsplit
 
 from neo4j import Driver, GraphDatabase
 
 from airflow.hooks.base import BaseHook
 from airflow.models import Connection
 
 
@@ -57,20 +58,32 @@
         self.connection = self.get_connection(self.neo4j_conn_id)
 
         uri = self.get_uri(self.connection)
         self.log.info("URI: %s", uri)
 
         is_encrypted = self.connection.extra_dejson.get("encrypted", False)
 
-        self.client = GraphDatabase.driver(
-            uri, auth=(self.connection.login, self.connection.password), encrypted=is_encrypted
-        )
+        self.client = self.get_client(self.connection, is_encrypted, uri)
 
         return self.client
 
+    def get_client(self, conn: Connection, encrypted: bool, uri: str) -> Driver:
+        """
+        Function to determine that relevant driver based on extras.
+        :param conn: Connection object.
+        :param encrypted: boolean if encrypted connection or not.
+        :param uri: uri string for connection.
+        :return: Driver
+        """
+        parsed_uri = urlsplit(uri)
+        kwargs: dict[str, Any] = {}
+        if parsed_uri.scheme in ["bolt", "neo4j"]:
+            kwargs["encrypted"] = encrypted
+        return GraphDatabase.driver(uri, auth=(conn.login, conn.password), **kwargs)
+
     def get_uri(self, conn: Connection) -> str:
         """
         Build the uri based on extras
         - Default - uses bolt scheme(bolt://)
         - neo4j_scheme - neo4j://
         - certs_self_signed - neo4j+ssc://
         - certs_trusted_ca - neo4j+s://
```

### Comparing `apache-airflow-providers-neo4j-3.2.1rc3/airflow/providers/neo4j/operators/neo4j.py` & `apache-airflow-providers-neo4j-3.3.0rc1/airflow/providers/neo4j/operators/neo4j.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-neo4j-3.2.1rc3/apache_airflow_providers_neo4j.egg-info/PKG-INFO` & `apache-airflow-providers-neo4j-3.3.0rc1/apache_airflow_providers_neo4j.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-neo4j
-Version: 3.2.1rc3
+Version: 3.3.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-neo4j package
 Home-page: https://airflow.apache.org/
+Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Download-URL: https://archive.apache.org/dist/airflow/providers
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-neo4j/3.2.1/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-neo4j/3.3.0/
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
 
 
 Package ``apache-airflow-providers-neo4j``
 
-Release: ``3.2.1rc3``
+Release: ``3.3.0rc1``
 
 
 `Neo4j <https://neo4j.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``neo4j`` provider. All classes for this provider package
 are in ``airflow.providers.neo4j`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-neo4j/3.2.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-neo4j/3.3.0/>`_.
 
 
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
 ``neo4j``           ``>=4.2.1``
 ==================  ==================
 
 
 
  .. Licensed to the Apache Software Foundation (ASF) under one
     or more contributor license agreements.  See the NOTICE file
@@ -111,14 +110,36 @@
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
+* ``Removed Mandatory Encryption in Neo4jHook (#30418)``
+
+Bug Fixes
+~~~~~~~~~
+
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add mechanism to suspend providers (#30422)``
+
 3.2.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
 
 * ``Fix typing problem revealed after recent Neo4J release (#27759)``
@@ -126,16 +147,17 @@
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Prepare for follow-up release for November providers (#27774)``
 
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
 
 .. Below changes are excluded from the changelog. Move them to
@@ -160,16 +182,17 @@
 
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
    * ``Migrate Neo4j example DAGs to new design #22454 (#24143)``
    * ``Prepare provider documentation 2022.05.11 (#23631)``
    * ``Bump pre-commit hook versions (#22887)``
@@ -288,9 +311,7 @@
 * ``Corrections in docs and tools after releasing provider RCs (#14082)``
 
 
 1.0.0
 .....
 
 Initial version of the provider.
-
-
```

### Comparing `apache-airflow-providers-neo4j-3.2.1rc3/apache_airflow_providers_neo4j.egg-info/SOURCES.txt` & `apache-airflow-providers-neo4j-3.3.0rc1/apache_airflow_providers_neo4j.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-neo4j-3.2.1rc3/setup.cfg` & `apache-airflow-providers-neo4j-3.3.0rc1/setup.cfg`

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-neo4j/3.2.1/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-neo4j/3.3.0/
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
@@ -42,21 +42,21 @@
 include_package_data = True
 python_requires = ~=3.7
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
-	apache-airflow>=2.3.0.dev0
+	apache-airflow>=2.4.0.dev0
 	neo4j>=4.2.1
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.neo4j.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.neo4j
 
 [egg_info]
-tag_build = rc3
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-neo4j-3.2.1rc3/setup.py` & `apache-airflow-providers-neo4j-3.3.0rc1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,21 +22,28 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-neo4j package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "3.2.1"
+version = "3.3.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-neo4j setup."""
     setup(
         version=version,
         extras_require={},
-        packages=find_namespace_packages(include=["airflow.providers.neo4j", "airflow.providers.neo4j.*"]),
+        packages=find_namespace_packages(
+            include=[
+                "airflow.providers.neo4j",
+                "airflow.providers.neo4j.*",
+                "airflow.providers.neo4j_vendor",
+                "airflow.providers.neo4j_vendor.*",
+            ],
+        ),
     )
 
 
 if __name__ == "__main__":
     do_setup()
```

