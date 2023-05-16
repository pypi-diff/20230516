# Comparing `tmp/apache-airflow-providers-influxdb-2.1.0rc1.tar.gz` & `tmp/apache-airflow-providers-influxdb-2.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-influxdb-2.1.0rc1.tar", last modified: Tue Nov 15 00:14:51 2022, max compression
+gzip compressed data, was "dist/apache-airflow-providers-influxdb-2.2.0rc1.tar", last modified: Tue May 16 15:54:25 2023, max compression
```

## Comparing `apache-airflow-providers-influxdb-2.1.0rc1.tar` & `apache-airflow-providers-influxdb-2.2.0rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:14:51.000000 apache-airflow-providers-influxdb-2.1.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2022-05-27 19:54:38.000000 apache-airflow-providers-influxdb-2.1.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1122 2022-11-15 00:14:50.000000 apache-airflow-providers-influxdb-2.1.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2022-05-27 19:54:38.000000 apache-airflow-providers-influxdb-2.1.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     7559 2022-11-15 00:14:51.000000 apache-airflow-providers-influxdb-2.1.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6006 2022-11-15 00:14:50.000000 apache-airflow-providers-influxdb-2.1.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:14:51.000000 apache-airflow-providers-influxdb-2.1.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:14:51.000000 apache-airflow-providers-influxdb-2.1.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:14:51.000000 apache-airflow-providers-influxdb-2.1.0rc1/airflow/providers/influxdb/
--rw-r--r--   0 root         (0) root         (0)      785 2022-09-13 10:31:21.000000 apache-airflow-providers-influxdb-2.1.0rc1/airflow/providers/influxdb/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2172 2022-11-15 00:14:50.000000 apache-airflow-providers-influxdb-2.1.0rc1/airflow/providers/influxdb/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:14:51.000000 apache-airflow-providers-influxdb-2.1.0rc1/airflow/providers/influxdb/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2022-09-13 10:31:21.000000 apache-airflow-providers-influxdb-2.1.0rc1/airflow/providers/influxdb/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5697 2022-10-26 03:21:46.000000 apache-airflow-providers-influxdb-2.1.0rc1/airflow/providers/influxdb/hooks/influxdb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:14:51.000000 apache-airflow-providers-influxdb-2.1.0rc1/airflow/providers/influxdb/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2022-09-13 10:31:21.000000 apache-airflow-providers-influxdb-2.1.0rc1/airflow/providers/influxdb/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1998 2022-10-26 03:21:46.000000 apache-airflow-providers-influxdb-2.1.0rc1/airflow/providers/influxdb/operators/influxdb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:14:51.000000 apache-airflow-providers-influxdb-2.1.0rc1/apache_airflow_providers_influxdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7559 2022-11-15 00:14:51.000000 apache-airflow-providers-influxdb-2.1.0rc1/apache_airflow_providers_influxdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      746 2022-11-15 00:14:51.000000 apache-airflow-providers-influxdb-2.1.0rc1/apache_airflow_providers_influxdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-15 00:14:51.000000 apache-airflow-providers-influxdb-2.1.0rc1/apache_airflow_providers_influxdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      106 2022-11-15 00:14:51.000000 apache-airflow-providers-influxdb-2.1.0rc1/apache_airflow_providers_influxdb.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-15 00:14:51.000000 apache-airflow-providers-influxdb-2.1.0rc1/apache_airflow_providers_influxdb.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       65 2022-11-15 00:14:51.000000 apache-airflow-providers-influxdb-2.1.0rc1/apache_airflow_providers_influxdb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2022-11-15 00:14:51.000000 apache-airflow-providers-influxdb-2.1.0rc1/apache_airflow_providers_influxdb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1836 2022-10-26 03:21:46.000000 apache-airflow-providers-influxdb-2.1.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1880 2022-11-15 00:14:51.000000 apache-airflow-providers-influxdb-2.1.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1494 2022-11-15 00:14:50.000000 apache-airflow-providers-influxdb-2.1.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:25.000000 apache-airflow-providers-influxdb-2.2.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-influxdb-2.2.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-05-16 15:54:24.000000 apache-airflow-providers-influxdb-2.2.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-influxdb-2.2.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     8282 2023-05-16 15:54:25.000000 apache-airflow-providers-influxdb-2.2.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6749 2023-05-16 15:54:24.000000 apache-airflow-providers-influxdb-2.2.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:25.000000 apache-airflow-providers-influxdb-2.2.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:25.000000 apache-airflow-providers-influxdb-2.2.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:25.000000 apache-airflow-providers-influxdb-2.2.0rc1/airflow/providers/influxdb/
+-rw-r--r--   0 root         (0) root         (0)     1391 2023-05-16 15:39:21.000000 apache-airflow-providers-influxdb-2.2.0rc1/airflow/providers/influxdb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2209 2023-05-16 15:54:24.000000 apache-airflow-providers-influxdb-2.2.0rc1/airflow/providers/influxdb/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:25.000000 apache-airflow-providers-influxdb-2.2.0rc1/airflow/providers/influxdb/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-influxdb-2.2.0rc1/airflow/providers/influxdb/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5697 2023-02-24 18:43:53.000000 apache-airflow-providers-influxdb-2.2.0rc1/airflow/providers/influxdb/hooks/influxdb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:25.000000 apache-airflow-providers-influxdb-2.2.0rc1/airflow/providers/influxdb/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-influxdb-2.2.0rc1/airflow/providers/influxdb/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1998 2023-02-24 18:43:53.000000 apache-airflow-providers-influxdb-2.2.0rc1/airflow/providers/influxdb/operators/influxdb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:25.000000 apache-airflow-providers-influxdb-2.2.0rc1/apache_airflow_providers_influxdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8282 2023-05-16 15:54:25.000000 apache-airflow-providers-influxdb-2.2.0rc1/apache_airflow_providers_influxdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      746 2023-05-16 15:54:25.000000 apache-airflow-providers-influxdb-2.2.0rc1/apache_airflow_providers_influxdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:54:25.000000 apache-airflow-providers-influxdb-2.2.0rc1/apache_airflow_providers_influxdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2023-05-16 15:54:25.000000 apache-airflow-providers-influxdb-2.2.0rc1/apache_airflow_providers_influxdb.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:54:25.000000 apache-airflow-providers-influxdb-2.2.0rc1/apache_airflow_providers_influxdb.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       68 2023-05-16 15:54:25.000000 apache-airflow-providers-influxdb-2.2.0rc1/apache_airflow_providers_influxdb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-16 15:54:25.000000 apache-airflow-providers-influxdb-2.2.0rc1/apache_airflow_providers_influxdb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5308 2023-05-15 09:39:26.000000 apache-airflow-providers-influxdb-2.2.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1883 2023-05-16 15:54:25.000000 apache-airflow-providers-influxdb-2.2.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1650 2023-05-16 15:54:24.000000 apache-airflow-providers-influxdb-2.2.0rc1/setup.py
```

### Comparing `apache-airflow-providers-influxdb-2.1.0rc1/LICENSE` & `apache-airflow-providers-influxdb-2.2.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-influxdb-2.1.0rc1/MANIFEST.in` & `apache-airflow-providers-influxdb-2.2.0rc1/MANIFEST.in`

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

### Comparing `apache-airflow-providers-influxdb-2.1.0rc1/PKG-INFO` & `apache-airflow-providers-influxdb-2.2.0rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-influxdb
-Version: 2.1.0rc1
+Version: 2.2.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-influxdb package
 Home-page: https://airflow.apache.org/
+Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Download-URL: https://archive.apache.org/dist/airflow/providers
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-influxdb/2.1.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-influxdb/2.2.0/
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
 
 
 Package ``apache-airflow-providers-influxdb``
 
-Release: ``2.1.0rc1``
+Release: ``2.2.0rc1``
 
 
 `InfluxDB <https://www.influxdata.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``influxdb`` provider. All classes for this provider package
 are in ``airflow.providers.influxdb`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-influxdb/2.1.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-influxdb/2.2.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -80,15 +79,15 @@
 
 Requirements
 ------------
 
 ===================  ==================
 PIP package          Version required
 ===================  ==================
-``apache-airflow``   ``>=2.3.0``
+``apache-airflow``   ``>=2.4.0``
 ``influxdb-client``  ``>=1.19.0``
 ``requests``         ``>=2.26.0``
 ===================  ==================
 
 
 
  .. Licensed to the Apache Software Foundation (ASF) under one
@@ -112,19 +111,37 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+2.2.0
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
 2.1.0
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
@@ -141,16 +158,17 @@
 
 2.0.0
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
    * ``Migrate Influx example DAGs to new design #22449 (#24136)``
    * ``Prepare provider documentation 2022.05.11 (#23631)``
    * ``Bump pre-commit hook versions (#22887)``
@@ -209,9 +227,7 @@
    * ``Prepare documentation for October Provider's release (#19321)``
    * ``Remove empty doc from influxdb provider (#18647)``
 
 1.0.0
 .....
 
 Initial version of the provider.
-
-
```

### Comparing `apache-airflow-providers-influxdb-2.1.0rc1/README.rst` & `apache-airflow-providers-influxdb-2.2.0rc1/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -15,28 +15,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-influxdb``
 
-Release: ``2.1.0rc1``
+Release: ``2.2.0rc1``
 
 
 `InfluxDB <https://www.influxdata.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``influxdb`` provider. All classes for this provider package
 are in ``airflow.providers.influxdb`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-influxdb/2.1.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-influxdb/2.2.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -46,15 +46,15 @@
 
 Requirements
 ------------
 
 ===================  ==================
 PIP package          Version required
 ===================  ==================
-``apache-airflow``   ``>=2.3.0``
+``apache-airflow``   ``>=2.4.0``
 ``influxdb-client``  ``>=1.19.0``
 ``requests``         ``>=2.26.0``
 ===================  ==================
 
 
 
  .. Licensed to the Apache Software Foundation (ASF) under one
@@ -78,19 +78,37 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+2.2.0
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
 2.1.0
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
@@ -107,16 +125,17 @@
 
 2.0.0
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
    * ``Migrate Influx example DAGs to new design #22449 (#24136)``
    * ``Prepare provider documentation 2022.05.11 (#23631)``
    * ``Bump pre-commit hook versions (#22887)``
```

### Comparing `apache-airflow-providers-influxdb-2.1.0rc1/airflow/providers/influxdb/__init__.py` & `apache-airflow-providers-influxdb-2.2.0rc1/airflow/providers/influxdb/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-influxdb-2.1.0rc1/airflow/providers/influxdb/get_provider_info.py` & `apache-airflow-providers-influxdb-2.2.0rc1/airflow/providers/influxdb/get_provider_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,16 +23,17 @@
 
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-influxdb",
         "name": "Influxdb",
         "description": "`InfluxDB <https://www.influxdata.com/>`__\n",
-        "dependencies": ["apache-airflow>=2.3.0", "influxdb-client>=1.19.0", "requests>=2.26.0"],
-        "versions": ["2.1.0", "2.0.0", "1.1.3", "1.1.2", "1.1.1", "1.1.0", "1.0.0"],
+        "dependencies": ["apache-airflow>=2.4.0", "influxdb-client>=1.19.0", "requests>=2.26.0"],
+        "suspended": False,
+        "versions": ["2.2.0", "2.1.0", "2.0.0", "1.1.3", "1.1.2", "1.1.1", "1.1.0", "1.0.0"],
         "integrations": [
             {
                 "integration-name": "Influxdb",
                 "external-doc-url": "https://www.influxdata.com/",
                 "tags": ["software"],
             }
         ],
```

### Comparing `apache-airflow-providers-influxdb-2.1.0rc1/airflow/providers/influxdb/hooks/__init__.py` & `apache-airflow-providers-influxdb-2.2.0rc1/airflow/providers/influxdb/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-influxdb-2.1.0rc1/airflow/providers/influxdb/hooks/influxdb.py` & `apache-airflow-providers-influxdb-2.2.0rc1/airflow/providers/influxdb/hooks/influxdb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-influxdb-2.1.0rc1/airflow/providers/influxdb/operators/influxdb.py` & `apache-airflow-providers-influxdb-2.2.0rc1/airflow/providers/influxdb/operators/influxdb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-influxdb-2.1.0rc1/apache_airflow_providers_influxdb.egg-info/PKG-INFO` & `apache-airflow-providers-influxdb-2.2.0rc1/apache_airflow_providers_influxdb.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-influxdb
-Version: 2.1.0rc1
+Version: 2.2.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-influxdb package
 Home-page: https://airflow.apache.org/
+Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Download-URL: https://archive.apache.org/dist/airflow/providers
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-influxdb/2.1.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-influxdb/2.2.0/
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
 
 
 Package ``apache-airflow-providers-influxdb``
 
-Release: ``2.1.0rc1``
+Release: ``2.2.0rc1``
 
 
 `InfluxDB <https://www.influxdata.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``influxdb`` provider. All classes for this provider package
 are in ``airflow.providers.influxdb`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-influxdb/2.1.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-influxdb/2.2.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -80,15 +79,15 @@
 
 Requirements
 ------------
 
 ===================  ==================
 PIP package          Version required
 ===================  ==================
-``apache-airflow``   ``>=2.3.0``
+``apache-airflow``   ``>=2.4.0``
 ``influxdb-client``  ``>=1.19.0``
 ``requests``         ``>=2.26.0``
 ===================  ==================
 
 
 
  .. Licensed to the Apache Software Foundation (ASF) under one
@@ -112,19 +111,37 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+2.2.0
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
 2.1.0
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
@@ -141,16 +158,17 @@
 
 2.0.0
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
    * ``Migrate Influx example DAGs to new design #22449 (#24136)``
    * ``Prepare provider documentation 2022.05.11 (#23631)``
    * ``Bump pre-commit hook versions (#22887)``
@@ -209,9 +227,7 @@
    * ``Prepare documentation for October Provider's release (#19321)``
    * ``Remove empty doc from influxdb provider (#18647)``
 
 1.0.0
 .....
 
 Initial version of the provider.
-
-
```

### Comparing `apache-airflow-providers-influxdb-2.1.0rc1/apache_airflow_providers_influxdb.egg-info/SOURCES.txt` & `apache-airflow-providers-influxdb-2.2.0rc1/apache_airflow_providers_influxdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-influxdb-2.1.0rc1/setup.cfg` & `apache-airflow-providers-influxdb-2.2.0rc1/setup.cfg`

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-influxdb/2.1.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-influxdb/2.2.0/
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
 	influxdb-client>=1.19.0
 	requests>=2.26.0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.influxdb.get_provider_info:get_provider_info
```

### Comparing `apache-airflow-providers-influxdb-2.1.0rc1/setup.py` & `apache-airflow-providers-influxdb-2.2.0rc1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -22,23 +22,28 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-influxdb package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "2.1.0"
+version = "2.2.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-influxdb setup."""
     setup(
         version=version,
         extras_require={},
         packages=find_namespace_packages(
-            include=["airflow.providers.influxdb", "airflow.providers.influxdb.*"]
+            include=[
+                "airflow.providers.influxdb",
+                "airflow.providers.influxdb.*",
+                "airflow.providers.influxdb_vendor",
+                "airflow.providers.influxdb_vendor.*",
+            ],
         ),
     )
 
 
 if __name__ == "__main__":
     do_setup()
```

