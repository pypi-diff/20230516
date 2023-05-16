# Comparing `tmp/apache-airflow-providers-mongo-3.1.1rc1.tar.gz` & `tmp/apache-airflow-providers-mongo-3.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-mongo-3.1.1rc1.tar", last modified: Sat Jan 14 12:16:25 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-mongo-3.2.0rc1.tar", last modified: Tue May 16 15:54:38 2023, max compression
```

## Comparing `apache-airflow-providers-mongo-3.1.1rc1.tar` & `apache-airflow-providers-mongo-3.2.0rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 12:16:25.000000 apache-airflow-providers-mongo-3.1.1rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2022-10-05 12:15:16.000000 apache-airflow-providers-mongo-3.1.1rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1122 2023-01-14 12:16:23.000000 apache-airflow-providers-mongo-3.1.1rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2022-10-05 12:15:16.000000 apache-airflow-providers-mongo-3.1.1rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     9384 2023-01-14 12:16:25.000000 apache-airflow-providers-mongo-3.1.1rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7840 2023-01-14 12:16:23.000000 apache-airflow-providers-mongo-3.1.1rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 12:16:24.000000 apache-airflow-providers-mongo-3.1.1rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 12:16:24.000000 apache-airflow-providers-mongo-3.1.1rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 12:16:24.000000 apache-airflow-providers-mongo-3.1.1rc1/airflow/providers/mongo/
--rw-r--r--   0 root         (0) root         (0)      787 2022-10-05 12:15:15.000000 apache-airflow-providers-mongo-3.1.1rc1/airflow/providers/mongo/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2307 2023-01-14 12:16:23.000000 apache-airflow-providers-mongo-3.1.1rc1/airflow/providers/mongo/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 12:16:25.000000 apache-airflow-providers-mongo-3.1.1rc1/airflow/providers/mongo/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2022-10-05 12:15:15.000000 apache-airflow-providers-mongo-3.1.1rc1/airflow/providers/mongo/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12849 2023-01-11 12:48:26.000000 apache-airflow-providers-mongo-3.1.1rc1/airflow/providers/mongo/hooks/mongo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 12:16:25.000000 apache-airflow-providers-mongo-3.1.1rc1/airflow/providers/mongo/sensors/
--rw-r--r--   0 root         (0) root         (0)      787 2022-10-05 12:15:15.000000 apache-airflow-providers-mongo-3.1.1rc1/airflow/providers/mongo/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2476 2023-01-11 12:48:26.000000 apache-airflow-providers-mongo-3.1.1rc1/airflow/providers/mongo/sensors/mongo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 12:16:25.000000 apache-airflow-providers-mongo-3.1.1rc1/apache_airflow_providers_mongo.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9384 2023-01-14 12:16:24.000000 apache-airflow-providers-mongo-3.1.1rc1/apache_airflow_providers_mongo.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      697 2023-01-14 12:16:24.000000 apache-airflow-providers-mongo-3.1.1rc1/apache_airflow_providers_mongo.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-14 12:16:24.000000 apache-airflow-providers-mongo-3.1.1rc1/apache_airflow_providers_mongo.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-01-14 12:16:24.000000 apache-airflow-providers-mongo-3.1.1rc1/apache_airflow_providers_mongo.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-14 12:16:24.000000 apache-airflow-providers-mongo-3.1.1rc1/apache_airflow_providers_mongo.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       67 2023-01-14 12:16:24.000000 apache-airflow-providers-mongo-3.1.1rc1/apache_airflow_providers_mongo.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-01-14 12:16:24.000000 apache-airflow-providers-mongo-3.1.1rc1/apache_airflow_providers_mongo.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     3814 2023-01-13 19:37:41.000000 apache-airflow-providers-mongo-3.1.1rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1864 2023-01-14 12:16:25.000000 apache-airflow-providers-mongo-3.1.1rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1460 2023-01-14 12:16:23.000000 apache-airflow-providers-mongo-3.1.1rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:38.000000 apache-airflow-providers-mongo-3.2.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-mongo-3.2.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-05-16 15:54:37.000000 apache-airflow-providers-mongo-3.2.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-mongo-3.2.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    10212 2023-05-16 15:54:38.000000 apache-airflow-providers-mongo-3.2.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8688 2023-05-16 15:54:37.000000 apache-airflow-providers-mongo-3.2.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:38.000000 apache-airflow-providers-mongo-3.2.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:38.000000 apache-airflow-providers-mongo-3.2.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:38.000000 apache-airflow-providers-mongo-3.2.0rc1/airflow/providers/mongo/
+-rw-r--r--   0 root         (0) root         (0)     1388 2023-05-16 15:39:21.000000 apache-airflow-providers-mongo-3.2.0rc1/airflow/providers/mongo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2349 2023-05-16 15:54:37.000000 apache-airflow-providers-mongo-3.2.0rc1/airflow/providers/mongo/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:38.000000 apache-airflow-providers-mongo-3.2.0rc1/airflow/providers/mongo/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-mongo-3.2.0rc1/airflow/providers/mongo/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13758 2023-05-16 07:40:59.000000 apache-airflow-providers-mongo-3.2.0rc1/airflow/providers/mongo/hooks/mongo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:38.000000 apache-airflow-providers-mongo-3.2.0rc1/airflow/providers/mongo/sensors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-mongo-3.2.0rc1/airflow/providers/mongo/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2476 2023-02-24 18:43:53.000000 apache-airflow-providers-mongo-3.2.0rc1/airflow/providers/mongo/sensors/mongo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:38.000000 apache-airflow-providers-mongo-3.2.0rc1/apache_airflow_providers_mongo.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10212 2023-05-16 15:54:38.000000 apache-airflow-providers-mongo-3.2.0rc1/apache_airflow_providers_mongo.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      697 2023-05-16 15:54:38.000000 apache-airflow-providers-mongo-3.2.0rc1/apache_airflow_providers_mongo.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:54:38.000000 apache-airflow-providers-mongo-3.2.0rc1/apache_airflow_providers_mongo.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      102 2023-05-16 15:54:38.000000 apache-airflow-providers-mongo-3.2.0rc1/apache_airflow_providers_mongo.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:54:38.000000 apache-airflow-providers-mongo-3.2.0rc1/apache_airflow_providers_mongo.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       60 2023-05-16 15:54:38.000000 apache-airflow-providers-mongo-3.2.0rc1/apache_airflow_providers_mongo.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-16 15:54:38.000000 apache-airflow-providers-mongo-3.2.0rc1/apache_airflow_providers_mongo.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5308 2023-05-15 09:39:26.000000 apache-airflow-providers-mongo-3.2.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1857 2023-05-16 15:54:38.000000 apache-airflow-providers-mongo-3.2.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1632 2023-05-16 15:54:37.000000 apache-airflow-providers-mongo-3.2.0rc1/setup.py
```

### Comparing `apache-airflow-providers-mongo-3.1.1rc1/LICENSE` & `apache-airflow-providers-mongo-3.2.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mongo-3.1.1rc1/MANIFEST.in` & `apache-airflow-providers-mongo-3.2.0rc1/MANIFEST.in`

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

### Comparing `apache-airflow-providers-mongo-3.1.1rc1/PKG-INFO` & `apache-airflow-providers-mongo-3.2.0rc1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-mongo
-Version: 3.1.1rc1
+Version: 3.2.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-mongo package
 Home-page: https://airflow.apache.org/
+Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Download-URL: https://archive.apache.org/dist/airflow/providers
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-mongo/3.1.1/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-mongo/3.2.0/
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
 
 
 Package ``apache-airflow-providers-mongo``
 
-Release: ``3.1.1rc1``
+Release: ``3.2.0rc1``
 
 
 `MongoDB <https://www.mongodb.com/what-is-mongodb>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``mongo`` provider. All classes for this provider package
 are in ``airflow.providers.mongo`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-mongo/3.1.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-mongo/3.2.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -80,17 +79,17 @@
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
-``apache-airflow``  ``>=2.3.0``
+``apache-airflow``  ``>=2.4.0``
 ``dnspython``       ``>=1.13.0``
-``pymongo``         ``>=3.6.0,<4.0.0``
+``pymongo``         ``>=3.6.0``
 ==================  ==================
 
  .. Licensed to the Apache Software Foundation (ASF) under one
     or more contributor license agreements.  See the NOTICE file
     distributed with this work for additional information
     regarding copyright ownership.  The ASF licenses this file
     to you under the Apache License, Version 2.0 (the
@@ -111,26 +110,46 @@
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
+* ``Remove the upper version bound on pymongo (#31189)``
+* ``Add future-compatible mongo Hook typing (#31289)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add mechanism to suspend providers (#30422)``
+
 3.1.1
 .....
 
 Misc
 ~~~~
 * ``MongoHook optimization (#28675)``
 
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
 * ``Fix links to sources for examples (#24386)``
 
@@ -146,16 +165,17 @@
 
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
    * ``Prepare provider documentation 2022.05.11 (#23631)``
    * ``Bump pre-commit hook versions (#22887)``
    * ``Prepare docs for May 2022 provider's release (#24231)``
@@ -265,9 +285,7 @@
 
 Updated documentation and readme files.
 
 1.0.0
 .....
 
 Initial version of the provider.
-
-
```

### Comparing `apache-airflow-providers-mongo-3.1.1rc1/README.rst` & `apache-airflow-providers-mongo-3.2.0rc1/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -15,28 +15,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-mongo``
 
-Release: ``3.1.1rc1``
+Release: ``3.2.0rc1``
 
 
 `MongoDB <https://www.mongodb.com/what-is-mongodb>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``mongo`` provider. All classes for this provider package
 are in ``airflow.providers.mongo`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-mongo/3.1.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-mongo/3.2.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -46,17 +46,17 @@
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
-``apache-airflow``  ``>=2.3.0``
+``apache-airflow``  ``>=2.4.0``
 ``dnspython``       ``>=1.13.0``
-``pymongo``         ``>=3.6.0,<4.0.0``
+``pymongo``         ``>=3.6.0``
 ==================  ==================
 
  .. Licensed to the Apache Software Foundation (ASF) under one
     or more contributor license agreements.  See the NOTICE file
     distributed with this work for additional information
     regarding copyright ownership.  The ASF licenses this file
     to you under the Apache License, Version 2.0 (the
@@ -77,26 +77,46 @@
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
+* ``Remove the upper version bound on pymongo (#31189)``
+* ``Add future-compatible mongo Hook typing (#31289)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add mechanism to suspend providers (#30422)``
+
 3.1.1
 .....
 
 Misc
 ~~~~
 * ``MongoHook optimization (#28675)``
 
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
 * ``Fix links to sources for examples (#24386)``
 
@@ -112,16 +132,17 @@
 
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
    * ``Prepare provider documentation 2022.05.11 (#23631)``
    * ``Bump pre-commit hook versions (#22887)``
    * ``Prepare docs for May 2022 provider's release (#24231)``
```

### Comparing `apache-airflow-providers-mongo-3.1.1rc1/airflow/providers/mongo/__init__.py` & `apache-airflow-providers-mongo-3.2.0rc1/airflow/providers/mongo/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mongo-3.1.1rc1/airflow/providers/mongo/get_provider_info.py` & `apache-airflow-providers-mongo-3.2.0rc1/airflow/providers/mongo/get_provider_info.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,29 +23,31 @@
 
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-mongo",
         "name": "MongoDB",
         "description": "`MongoDB <https://www.mongodb.com/what-is-mongodb>`__\n",
+        "suspended": False,
         "versions": [
+            "3.2.0",
             "3.1.1",
             "3.1.0",
             "3.0.0",
             "2.3.3",
             "2.3.2",
             "2.3.1",
             "2.3.0",
             "2.2.0",
             "2.1.0",
             "2.0.0",
             "1.0.1",
             "1.0.0",
         ],
-        "dependencies": ["apache-airflow>=2.3.0", "dnspython>=1.13.0", "pymongo>=3.6.0,<4.0.0"],
+        "dependencies": ["apache-airflow>=2.4.0", "dnspython>=1.13.0", "pymongo>=3.6.0"],
         "integrations": [
             {
                 "integration-name": "MongoDB",
                 "external-doc-url": "https://www.mongodb.com/what-is-mongodb",
                 "logo": "/integration-logos/mongo/MongoDB.png",
                 "tags": ["software"],
             }
```

### Comparing `apache-airflow-providers-mongo-3.1.1rc1/airflow/providers/mongo/hooks/__init__.py` & `apache-airflow-providers-mongo-3.2.0rc1/airflow/providers/mongo/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mongo-3.1.1rc1/airflow/providers/mongo/hooks/mongo.py` & `apache-airflow-providers-mongo-3.2.0rc1/airflow/providers/mongo/hooks/mongo.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,20 +16,22 @@
 # specific language governing permissions and limitations
 # under the License.
 """Hook for Mongo DB"""
 from __future__ import annotations
 
 from ssl import CERT_NONE
 from types import TracebackType
+from typing import Any, overload
 from urllib.parse import quote_plus, urlunsplit
 
 import pymongo
 from pymongo import MongoClient, ReplaceOne
 
 from airflow.hooks.base import BaseHook
+from airflow.typing_compat import Literal
 
 
 class MongoHook(BaseHook):
     """
     Interact with Mongo. This hook uses the Mongo conn_id.
     PyMongo Wrapper to Interact With Mongo Database
     Mongo Connection Documentation
@@ -52,15 +54,15 @@
     hook_name = "MongoDB"
 
     def __init__(self, conn_id: str = default_conn_name, *args, **kwargs) -> None:
         super().__init__()
         self.mongo_conn_id = conn_id
         self.connection = self.get_connection(conn_id)
         self.extras = self.connection.extra_dejson.copy()
-        self.client = None
+        self.client: MongoClient | None = None
         self.uri = self._create_uri()
 
     def __enter__(self):
         return self
 
     def __exit__(
         self,
@@ -78,15 +80,20 @@
             return self.client
 
         # Mongo Connection Options dict that is unpacked when passed to MongoClient
         options = self.extras
 
         # If we are using SSL disable requiring certs from specific hostname
         if options.get("ssl", False):
-            options.update({"ssl_cert_reqs": CERT_NONE})
+            if pymongo.__version__ >= "4.0.0":
+                # In pymongo 4.0.0+ `tlsAllowInvalidCertificates=True`
+                # replaces `ssl_cert_reqs=CERT_NONE`
+                options.update({"tlsAllowInvalidCertificates": True})
+            else:
+                options.update({"ssl_cert_reqs": CERT_NONE})
 
         self.client = MongoClient(self.uri, **options)
         return self.client
 
     def _create_uri(self) -> str:
         """
         Create URI string from the given credentials.
@@ -125,23 +132,47 @@
         https://pymongo.readthedocs.io/en/stable/api/pymongo/collection.html#pymongo.collection.Collection.aggregate
         https://pymongo.readthedocs.io/en/stable/examples/aggregation.html
         """
         collection = self.get_collection(mongo_collection, mongo_db=mongo_db)
 
         return collection.aggregate(aggregate_query, **kwargs)
 
+    @overload
     def find(
         self,
         mongo_collection: str,
         query: dict,
-        find_one: bool = False,
+        find_one: Literal[False],
         mongo_db: str | None = None,
         projection: list | dict | None = None,
         **kwargs,
     ) -> pymongo.cursor.Cursor:
+        ...
+
+    @overload
+    def find(
+        self,
+        mongo_collection: str,
+        query: dict,
+        find_one: Literal[True],
+        mongo_db: str | None = None,
+        projection: list | dict | None = None,
+        **kwargs,
+    ) -> Any | None:
+        ...
+
+    def find(
+        self,
+        mongo_collection: str,
+        query: dict,
+        find_one: bool = False,
+        mongo_db: str | None = None,
+        projection: list | dict | None = None,
+        **kwargs,
+    ) -> pymongo.cursor.Cursor | Any | None:
         """
         Runs a mongo find query and returns the results
         https://pymongo.readthedocs.io/en/stable/api/pymongo/collection.html#pymongo.collection.Collection.find
         """
         collection = self.get_collection(mongo_collection, mongo_db=mongo_db)
 
         if find_one:
```

### Comparing `apache-airflow-providers-mongo-3.1.1rc1/airflow/providers/mongo/sensors/mongo.py` & `apache-airflow-providers-mongo-3.2.0rc1/airflow/providers/mongo/sensors/mongo.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mongo-3.1.1rc1/apache_airflow_providers_mongo.egg-info/PKG-INFO` & `apache-airflow-providers-mongo-3.2.0rc1/apache_airflow_providers_mongo.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-mongo
-Version: 3.1.1rc1
+Version: 3.2.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-mongo package
 Home-page: https://airflow.apache.org/
+Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Download-URL: https://archive.apache.org/dist/airflow/providers
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-mongo/3.1.1/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-mongo/3.2.0/
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
 
 
 Package ``apache-airflow-providers-mongo``
 
-Release: ``3.1.1rc1``
+Release: ``3.2.0rc1``
 
 
 `MongoDB <https://www.mongodb.com/what-is-mongodb>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``mongo`` provider. All classes for this provider package
 are in ``airflow.providers.mongo`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-mongo/3.1.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-mongo/3.2.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -80,17 +79,17 @@
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
-``apache-airflow``  ``>=2.3.0``
+``apache-airflow``  ``>=2.4.0``
 ``dnspython``       ``>=1.13.0``
-``pymongo``         ``>=3.6.0,<4.0.0``
+``pymongo``         ``>=3.6.0``
 ==================  ==================
 
  .. Licensed to the Apache Software Foundation (ASF) under one
     or more contributor license agreements.  See the NOTICE file
     distributed with this work for additional information
     regarding copyright ownership.  The ASF licenses this file
     to you under the Apache License, Version 2.0 (the
@@ -111,26 +110,46 @@
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
+* ``Remove the upper version bound on pymongo (#31189)``
+* ``Add future-compatible mongo Hook typing (#31289)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add mechanism to suspend providers (#30422)``
+
 3.1.1
 .....
 
 Misc
 ~~~~
 * ``MongoHook optimization (#28675)``
 
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
 * ``Fix links to sources for examples (#24386)``
 
@@ -146,16 +165,17 @@
 
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
    * ``Prepare provider documentation 2022.05.11 (#23631)``
    * ``Bump pre-commit hook versions (#22887)``
    * ``Prepare docs for May 2022 provider's release (#24231)``
@@ -265,9 +285,7 @@
 
 Updated documentation and readme files.
 
 1.0.0
 .....
 
 Initial version of the provider.
-
-
```

### Comparing `apache-airflow-providers-mongo-3.1.1rc1/apache_airflow_providers_mongo.egg-info/SOURCES.txt` & `apache-airflow-providers-mongo-3.2.0rc1/apache_airflow_providers_mongo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mongo-3.1.1rc1/pyproject.toml` & `apache-airflow-providers-mongo-3.2.0rc1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -19,37 +19,39 @@
 target-version = ['py37', 'py38', 'py39', 'py310']
 # The build system section is needed in order to workaround the side-effect introduced by recent
 # setup tools version. The recent setuptools version update (64.0.0) broke paths of editable installations
 # and we have to pin it to 63.4.3 version
 # The problem is tracked (and this limitation might be removed if it is solved) in:
 # https://github.com/pypa/setuptools/issues/3548
 [build-system]
-requires = ['setuptools==63.4.3']
+requires = ['setuptools==67.2.0']
 build-backend = "setuptools.build_meta"
 
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

### Comparing `apache-airflow-providers-mongo-3.1.1rc1/setup.cfg` & `apache-airflow-providers-mongo-3.2.0rc1/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-mongo/3.1.1/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-mongo/3.2.0/
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
@@ -42,17 +42,17 @@
 include_package_data = True
 python_requires = ~=3.7
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
-	apache-airflow>=2.3.0.dev0
+	apache-airflow>=2.4.0.dev0
 	dnspython>=1.13.0
-	pymongo>=3.6.0,<4.0.0
+	pymongo>=3.6.0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.mongo.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.mongo
```

### Comparing `apache-airflow-providers-mongo-3.1.1rc1/setup.py` & `apache-airflow-providers-mongo-3.2.0rc1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,21 +22,28 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-mongo package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "3.1.1"
+version = "3.2.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-mongo setup."""
     setup(
         version=version,
         extras_require={},
-        packages=find_namespace_packages(include=["airflow.providers.mongo", "airflow.providers.mongo.*"]),
+        packages=find_namespace_packages(
+            include=[
+                "airflow.providers.mongo",
+                "airflow.providers.mongo.*",
+                "airflow.providers.mongo_vendor",
+                "airflow.providers.mongo_vendor.*",
+            ],
+        ),
     )
 
 
 if __name__ == "__main__":
     do_setup()
```

