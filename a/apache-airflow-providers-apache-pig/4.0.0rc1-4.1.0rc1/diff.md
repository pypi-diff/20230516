# Comparing `tmp/apache-airflow-providers-apache-pig-4.0.0rc1.tar.gz` & `tmp/apache-airflow-providers-apache-pig-4.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-apache-pig-4.0.0rc1.tar", last modified: Tue Nov 15 00:13:59 2022, max compression
+gzip compressed data, was "dist/apache-airflow-providers-apache-pig-4.1.0rc1.tar", last modified: Tue May 16 15:53:13 2023, max compression
```

## Comparing `apache-airflow-providers-apache-pig-4.0.0rc1.tar` & `apache-airflow-providers-apache-pig-4.1.0rc1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:13:59.000000 apache-airflow-providers-apache-pig-4.0.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2022-05-27 19:54:38.000000 apache-airflow-providers-apache-pig-4.0.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1122 2022-11-15 00:13:58.000000 apache-airflow-providers-apache-pig-4.0.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2022-05-27 19:54:38.000000 apache-airflow-providers-apache-pig-4.0.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     9749 2022-11-15 00:13:59.000000 apache-airflow-providers-apache-pig-4.0.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8190 2022-11-15 00:13:58.000000 apache-airflow-providers-apache-pig-4.0.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:13:59.000000 apache-airflow-providers-apache-pig-4.0.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:13:59.000000 apache-airflow-providers-apache-pig-4.0.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:13:59.000000 apache-airflow-providers-apache-pig-4.0.0rc1/airflow/providers/apache/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:13:59.000000 apache-airflow-providers-apache-pig-4.0.0rc1/airflow/providers/apache/pig/
--rw-r--r--   0 root         (0) root         (0)      787 2022-09-13 10:31:21.000000 apache-airflow-providers-apache-pig-4.0.0rc1/airflow/providers/apache/pig/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2287 2022-11-15 00:13:58.000000 apache-airflow-providers-apache-pig-4.0.0rc1/airflow/providers/apache/pig/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:13:59.000000 apache-airflow-providers-apache-pig-4.0.0rc1/airflow/providers/apache/pig/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2022-09-13 10:31:21.000000 apache-airflow-providers-apache-pig-4.0.0rc1/airflow/providers/apache/pig/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4251 2022-11-13 22:55:59.000000 apache-airflow-providers-apache-pig-4.0.0rc1/airflow/providers/apache/pig/hooks/pig.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:13:59.000000 apache-airflow-providers-apache-pig-4.0.0rc1/airflow/providers/apache/pig/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2022-09-13 10:31:21.000000 apache-airflow-providers-apache-pig-4.0.0rc1/airflow/providers/apache/pig/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2978 2022-11-13 22:55:59.000000 apache-airflow-providers-apache-pig-4.0.0rc1/airflow/providers/apache/pig/operators/pig.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:13:59.000000 apache-airflow-providers-apache-pig-4.0.0rc1/apache_airflow_providers_apache_pig.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9749 2022-11-15 00:13:59.000000 apache-airflow-providers-apache-pig-4.0.0rc1/apache_airflow_providers_apache_pig.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      762 2022-11-15 00:13:59.000000 apache-airflow-providers-apache-pig-4.0.0rc1/apache_airflow_providers_apache_pig.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-15 00:13:59.000000 apache-airflow-providers-apache-pig-4.0.0rc1/apache_airflow_providers_apache_pig.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      108 2022-11-15 00:13:59.000000 apache-airflow-providers-apache-pig-4.0.0rc1/apache_airflow_providers_apache_pig.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-15 00:13:59.000000 apache-airflow-providers-apache-pig-4.0.0rc1/apache_airflow_providers_apache_pig.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       24 2022-11-15 00:13:59.000000 apache-airflow-providers-apache-pig-4.0.0rc1/apache_airflow_providers_apache_pig.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2022-11-15 00:13:59.000000 apache-airflow-providers-apache-pig-4.0.0rc1/apache_airflow_providers_apache_pig.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1836 2022-10-26 03:21:46.000000 apache-airflow-providers-apache-pig-4.0.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1849 2022-11-15 00:13:59.000000 apache-airflow-providers-apache-pig-4.0.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1502 2022-11-15 00:13:58.000000 apache-airflow-providers-apache-pig-4.0.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:13.000000 apache-airflow-providers-apache-pig-4.1.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-pig-4.1.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-05-16 15:53:12.000000 apache-airflow-providers-apache-pig-4.1.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-pig-4.1.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    10472 2023-05-16 15:53:13.000000 apache-airflow-providers-apache-pig-4.1.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8933 2023-05-16 15:53:12.000000 apache-airflow-providers-apache-pig-4.1.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:13.000000 apache-airflow-providers-apache-pig-4.1.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:13.000000 apache-airflow-providers-apache-pig-4.1.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:13.000000 apache-airflow-providers-apache-pig-4.1.0rc1/airflow/providers/apache/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:13.000000 apache-airflow-providers-apache-pig-4.1.0rc1/airflow/providers/apache/pig/
+-rw-r--r--   0 root         (0) root         (0)     1393 2023-05-16 15:39:21.000000 apache-airflow-providers-apache-pig-4.1.0rc1/airflow/providers/apache/pig/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2455 2023-05-16 15:53:12.000000 apache-airflow-providers-apache-pig-4.1.0rc1/airflow/providers/apache/pig/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:13.000000 apache-airflow-providers-apache-pig-4.1.0rc1/airflow/providers/apache/pig/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-pig-4.1.0rc1/airflow/providers/apache/pig/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4251 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-pig-4.1.0rc1/airflow/providers/apache/pig/hooks/pig.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:13.000000 apache-airflow-providers-apache-pig-4.1.0rc1/airflow/providers/apache/pig/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-pig-4.1.0rc1/airflow/providers/apache/pig/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2978 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-pig-4.1.0rc1/airflow/providers/apache/pig/operators/pig.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:13.000000 apache-airflow-providers-apache-pig-4.1.0rc1/apache_airflow_providers_apache_pig.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10472 2023-05-16 15:53:13.000000 apache-airflow-providers-apache-pig-4.1.0rc1/apache_airflow_providers_apache_pig.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      762 2023-05-16 15:53:13.000000 apache-airflow-providers-apache-pig-4.1.0rc1/apache_airflow_providers_apache_pig.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:53:13.000000 apache-airflow-providers-apache-pig-4.1.0rc1/apache_airflow_providers_apache_pig.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-05-16 15:53:13.000000 apache-airflow-providers-apache-pig-4.1.0rc1/apache_airflow_providers_apache_pig.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:53:13.000000 apache-airflow-providers-apache-pig-4.1.0rc1/apache_airflow_providers_apache_pig.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       27 2023-05-16 15:53:13.000000 apache-airflow-providers-apache-pig-4.1.0rc1/apache_airflow_providers_apache_pig.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-16 15:53:13.000000 apache-airflow-providers-apache-pig-4.1.0rc1/apache_airflow_providers_apache_pig.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5308 2023-05-15 09:39:26.000000 apache-airflow-providers-apache-pig-4.1.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1852 2023-05-16 15:53:13.000000 apache-airflow-providers-apache-pig-4.1.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1662 2023-05-16 15:53:12.000000 apache-airflow-providers-apache-pig-4.1.0rc1/setup.py
```

### Comparing `apache-airflow-providers-apache-pig-4.0.0rc1/LICENSE` & `apache-airflow-providers-apache-pig-4.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-pig-4.0.0rc1/MANIFEST.in` & `apache-airflow-providers-apache-pig-4.1.0rc1/MANIFEST.in`

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

### Comparing `apache-airflow-providers-apache-pig-4.0.0rc1/PKG-INFO` & `apache-airflow-providers-apache-pig-4.1.0rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-pig
-Version: 4.0.0rc1
+Version: 4.1.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-pig package
 Home-page: https://airflow.apache.org/
+Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Download-URL: https://archive.apache.org/dist/airflow/providers
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-pig/4.0.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-pig/4.1.0/
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
 
 
 Package ``apache-airflow-providers-apache-pig``
 
-Release: ``4.0.0rc1``
+Release: ``4.1.0rc1``
 
 
 `Apache Pig <https://pig.apache.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.pig`` provider. All classes for this provider package
 are in ``airflow.providers.apache.pig`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-pig/4.0.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-pig/4.1.0/>`_.
 
 
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
@@ -109,19 +108,37 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+4.1.0
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
 4.0.0
 .....
 
-This release of provider is only available for Airflow 2.3+ as explained in the
-`Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/README.md#support-for-providers>`_.
+.. note::
+  This release of provider is only available for Airflow 2.3+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
 You cannot use ``pig_properties`` any more as connection extras. If you want to add extra parameters
 to ``pig`` command, you need to do it via ``pig_properties`` (string list) of the PigCliHook (new parameter)
 or via ``pig_opts`` (string with options separated by spaces) or ``pig_properties`` (string list) in
@@ -150,16 +167,17 @@
 
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
    * ``AIP-47 - Migrate apache pig DAGs to new design #22439 (#24212)``
    * ``Prepare docs for May 2022 provider's release (#24231)``
    * ``Update package description to remove double min-airflow specification (#24292)``
@@ -246,9 +264,7 @@
 
 Updated documentation and readme files.
 
 1.0.0
 .....
 
 Initial version of the provider.
-
-
```

### Comparing `apache-airflow-providers-apache-pig-4.0.0rc1/README.rst` & `apache-airflow-providers-apache-pig-4.1.0rc1/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -15,28 +15,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-pig``
 
-Release: ``4.0.0rc1``
+Release: ``4.1.0rc1``
 
 
 `Apache Pig <https://pig.apache.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.pig`` provider. All classes for this provider package
 are in ``airflow.providers.apache.pig`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-pig/4.0.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-pig/4.1.0/>`_.
 
 
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
@@ -75,19 +75,37 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+4.1.0
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
 4.0.0
 .....
 
-This release of provider is only available for Airflow 2.3+ as explained in the
-`Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/README.md#support-for-providers>`_.
+.. note::
+  This release of provider is only available for Airflow 2.3+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
 You cannot use ``pig_properties`` any more as connection extras. If you want to add extra parameters
 to ``pig`` command, you need to do it via ``pig_properties`` (string list) of the PigCliHook (new parameter)
 or via ``pig_opts`` (string with options separated by spaces) or ``pig_properties`` (string list) in
@@ -116,16 +134,17 @@
 
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
    * ``AIP-47 - Migrate apache pig DAGs to new design #22439 (#24212)``
    * ``Prepare docs for May 2022 provider's release (#24231)``
    * ``Update package description to remove double min-airflow specification (#24292)``
```

### Comparing `apache-airflow-providers-apache-pig-4.0.0rc1/airflow/providers/apache/pig/__init__.py` & `apache-airflow-providers-apache-pig-4.1.0rc1/airflow/providers/apache/pig/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-pig-4.0.0rc1/airflow/providers/apache/pig/get_provider_info.py` & `apache-airflow-providers-apache-pig-4.1.0rc1/airflow/providers/apache/pig/get_provider_info.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,16 +23,28 @@
 
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-apache-pig",
         "name": "Apache Pig",
         "description": "`Apache Pig <https://pig.apache.org/>`__\n",
-        "versions": ["4.0.0", "3.0.0", "2.0.4", "2.0.3", "2.0.2", "2.0.1", "2.0.0", "1.0.1", "1.0.0"],
-        "dependencies": ["apache-airflow>=2.3.0"],
+        "suspended": False,
+        "versions": [
+            "4.1.0",
+            "4.0.0",
+            "3.0.0",
+            "2.0.4",
+            "2.0.3",
+            "2.0.2",
+            "2.0.1",
+            "2.0.0",
+            "1.0.1",
+            "1.0.0",
+        ],
+        "dependencies": ["apache-airflow>=2.4.0"],
         "integrations": [
             {
                 "integration-name": "Apache Pig",
                 "external-doc-url": "https://pig.apache.org/",
                 "how-to-guide": ["/docs/apache-airflow-providers-apache-pig/operators.rst"],
                 "logo": "/integration-logos/apache/pig.png",
                 "tags": ["apache"],
```

### Comparing `apache-airflow-providers-apache-pig-4.0.0rc1/airflow/providers/apache/pig/hooks/__init__.py` & `apache-airflow-providers-apache-pig-4.1.0rc1/airflow/providers/apache/pig/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-pig-4.0.0rc1/airflow/providers/apache/pig/hooks/pig.py` & `apache-airflow-providers-apache-pig-4.1.0rc1/airflow/providers/apache/pig/hooks/pig.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-pig-4.0.0rc1/airflow/providers/apache/pig/operators/pig.py` & `apache-airflow-providers-apache-pig-4.1.0rc1/airflow/providers/apache/pig/operators/pig.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-pig-4.0.0rc1/apache_airflow_providers_apache_pig.egg-info/PKG-INFO` & `apache-airflow-providers-apache-pig-4.1.0rc1/apache_airflow_providers_apache_pig.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-pig
-Version: 4.0.0rc1
+Version: 4.1.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-pig package
 Home-page: https://airflow.apache.org/
+Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Download-URL: https://archive.apache.org/dist/airflow/providers
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-pig/4.0.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-pig/4.1.0/
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
 
 
 Package ``apache-airflow-providers-apache-pig``
 
-Release: ``4.0.0rc1``
+Release: ``4.1.0rc1``
 
 
 `Apache Pig <https://pig.apache.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.pig`` provider. All classes for this provider package
 are in ``airflow.providers.apache.pig`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-pig/4.0.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-pig/4.1.0/>`_.
 
 
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
@@ -109,19 +108,37 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+4.1.0
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
 4.0.0
 .....
 
-This release of provider is only available for Airflow 2.3+ as explained in the
-`Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/README.md#support-for-providers>`_.
+.. note::
+  This release of provider is only available for Airflow 2.3+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
 You cannot use ``pig_properties`` any more as connection extras. If you want to add extra parameters
 to ``pig`` command, you need to do it via ``pig_properties`` (string list) of the PigCliHook (new parameter)
 or via ``pig_opts`` (string with options separated by spaces) or ``pig_properties`` (string list) in
@@ -150,16 +167,17 @@
 
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
    * ``AIP-47 - Migrate apache pig DAGs to new design #22439 (#24212)``
    * ``Prepare docs for May 2022 provider's release (#24231)``
    * ``Update package description to remove double min-airflow specification (#24292)``
@@ -246,9 +264,7 @@
 
 Updated documentation and readme files.
 
 1.0.0
 .....
 
 Initial version of the provider.
-
-
```

### Comparing `apache-airflow-providers-apache-pig-4.0.0rc1/apache_airflow_providers_apache_pig.egg-info/SOURCES.txt` & `apache-airflow-providers-apache-pig-4.1.0rc1/apache_airflow_providers_apache_pig.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-pig-4.0.0rc1/pyproject.toml` & `apache-airflow-providers-apache-pig-4.1.0rc1/airflow/providers/apache/pig/__init__.py`

 * *Files 25% similar despite different names*

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
+version = "4.1.0"
+
+if packaging.version.parse(airflow.version.version) < packaging.version.parse("2.4.0"):
+    raise RuntimeError(
+        f"The package `apache-airflow-providers-apache-pig:{version}` requires Apache Airflow 2.4.0+"
+    )
```

### Comparing `apache-airflow-providers-apache-pig-4.0.0rc1/setup.cfg` & `apache-airflow-providers-apache-pig-4.1.0rc1/setup.cfg`

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-apache-pig/4.0.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-apache-pig/4.1.0/
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
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.apache.pig.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.apache.pig
```

### Comparing `apache-airflow-providers-apache-pig-4.0.0rc1/setup.py` & `apache-airflow-providers-apache-pig-4.1.0rc1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,23 +22,28 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-apache-pig package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "4.0.0"
+version = "4.1.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-apache-pig setup."""
     setup(
         version=version,
         extras_require={},
         packages=find_namespace_packages(
-            include=["airflow.providers.apache.pig", "airflow.providers.apache.pig.*"]
+            include=[
+                "airflow.providers.apache.pig",
+                "airflow.providers.apache.pig.*",
+                "airflow.providers.apache.pig_vendor",
+                "airflow.providers.apache.pig_vendor.*",
+            ],
         ),
     )
 
 
 if __name__ == "__main__":
     do_setup()
```

