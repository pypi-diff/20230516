# Comparing `tmp/apache-airflow-providers-github-2.2.1rc1.tar.gz` & `tmp/apache-airflow-providers-github-2.3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-github-2.2.1rc1.tar", last modified: Fri Mar  3 13:46:50 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-github-2.3.0rc1.tar", last modified: Tue May 16 15:53:52 2023, max compression
```

## Comparing `apache-airflow-providers-github-2.2.1rc1.tar` & `apache-airflow-providers-github-2.3.0rc1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 13:46:50.000000 apache-airflow-providers-github-2.2.1rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-github-2.2.1rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1122 2023-03-03 13:46:49.000000 apache-airflow-providers-github-2.2.1rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-github-2.2.1rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     6955 2023-03-03 13:46:50.000000 apache-airflow-providers-github-2.2.1rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5408 2023-03-03 13:46:49.000000 apache-airflow-providers-github-2.2.1rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 13:46:50.000000 apache-airflow-providers-github-2.2.1rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 13:46:50.000000 apache-airflow-providers-github-2.2.1rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 13:46:50.000000 apache-airflow-providers-github-2.2.1rc1/airflow/providers/github/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-github-2.2.1rc1/airflow/providers/github/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2207 2023-03-03 13:46:49.000000 apache-airflow-providers-github-2.2.1rc1/airflow/providers/github/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 13:46:50.000000 apache-airflow-providers-github-2.2.1rc1/airflow/providers/github/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-github-2.2.1rc1/airflow/providers/github/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3349 2023-02-24 18:43:53.000000 apache-airflow-providers-github-2.2.1rc1/airflow/providers/github/hooks/github.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 13:46:50.000000 apache-airflow-providers-github-2.2.1rc1/airflow/providers/github/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-github-2.2.1rc1/airflow/providers/github/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3025 2023-02-24 18:43:53.000000 apache-airflow-providers-github-2.2.1rc1/airflow/providers/github/operators/github.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 13:46:50.000000 apache-airflow-providers-github-2.2.1rc1/airflow/providers/github/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-github-2.2.1rc1/airflow/providers/github/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5277 2023-02-24 18:43:53.000000 apache-airflow-providers-github-2.2.1rc1/airflow/providers/github/sensors/github.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 13:46:50.000000 apache-airflow-providers-github-2.2.1rc1/apache_airflow_providers_github.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6955 2023-03-03 13:46:50.000000 apache-airflow-providers-github-2.2.1rc1/apache_airflow_providers_github.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      804 2023-03-03 13:46:50.000000 apache-airflow-providers-github-2.2.1rc1/apache_airflow_providers_github.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-03 13:46:50.000000 apache-airflow-providers-github-2.2.1rc1/apache_airflow_providers_github.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-03-03 13:46:50.000000 apache-airflow-providers-github-2.2.1rc1/apache_airflow_providers_github.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-03 13:46:50.000000 apache-airflow-providers-github-2.2.1rc1/apache_airflow_providers_github.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       42 2023-03-03 13:46:50.000000 apache-airflow-providers-github-2.2.1rc1/apache_airflow_providers_github.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-03-03 13:46:50.000000 apache-airflow-providers-github-2.2.1rc1/apache_airflow_providers_github.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     3814 2023-02-24 18:43:54.000000 apache-airflow-providers-github-2.2.1rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1844 2023-03-03 13:46:50.000000 apache-airflow-providers-github-2.2.1rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1464 2023-03-03 13:46:49.000000 apache-airflow-providers-github-2.2.1rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:52.000000 apache-airflow-providers-github-2.3.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-github-2.3.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-05-16 15:53:51.000000 apache-airflow-providers-github-2.3.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-github-2.3.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     7678 2023-05-16 15:53:52.000000 apache-airflow-providers-github-2.3.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6151 2023-05-16 15:53:51.000000 apache-airflow-providers-github-2.3.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:52.000000 apache-airflow-providers-github-2.3.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:52.000000 apache-airflow-providers-github-2.3.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:52.000000 apache-airflow-providers-github-2.3.0rc1/airflow/providers/github/
+-rw-r--r--   0 root         (0) root         (0)     1389 2023-05-16 15:39:21.000000 apache-airflow-providers-github-2.3.0rc1/airflow/providers/github/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2244 2023-05-16 15:53:51.000000 apache-airflow-providers-github-2.3.0rc1/airflow/providers/github/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:52.000000 apache-airflow-providers-github-2.3.0rc1/airflow/providers/github/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-github-2.3.0rc1/airflow/providers/github/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3349 2023-02-24 18:43:53.000000 apache-airflow-providers-github-2.3.0rc1/airflow/providers/github/hooks/github.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:52.000000 apache-airflow-providers-github-2.3.0rc1/airflow/providers/github/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-github-2.3.0rc1/airflow/providers/github/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3025 2023-02-24 18:43:53.000000 apache-airflow-providers-github-2.3.0rc1/airflow/providers/github/operators/github.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:52.000000 apache-airflow-providers-github-2.3.0rc1/airflow/providers/github/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-github-2.3.0rc1/airflow/providers/github/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5277 2023-02-24 18:43:53.000000 apache-airflow-providers-github-2.3.0rc1/airflow/providers/github/sensors/github.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:52.000000 apache-airflow-providers-github-2.3.0rc1/apache_airflow_providers_github.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7678 2023-05-16 15:53:52.000000 apache-airflow-providers-github-2.3.0rc1/apache_airflow_providers_github.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      804 2023-05-16 15:53:52.000000 apache-airflow-providers-github-2.3.0rc1/apache_airflow_providers_github.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:53:52.000000 apache-airflow-providers-github-2.3.0rc1/apache_airflow_providers_github.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-05-16 15:53:52.000000 apache-airflow-providers-github-2.3.0rc1/apache_airflow_providers_github.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:53:52.000000 apache-airflow-providers-github-2.3.0rc1/apache_airflow_providers_github.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       42 2023-05-16 15:53:52.000000 apache-airflow-providers-github-2.3.0rc1/apache_airflow_providers_github.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-16 15:53:52.000000 apache-airflow-providers-github-2.3.0rc1/apache_airflow_providers_github.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5308 2023-05-15 09:39:26.000000 apache-airflow-providers-github-2.3.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1844 2023-05-16 15:53:52.000000 apache-airflow-providers-github-2.3.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1638 2023-05-16 15:53:51.000000 apache-airflow-providers-github-2.3.0rc1/setup.py
```

### Comparing `apache-airflow-providers-github-2.2.1rc1/LICENSE` & `apache-airflow-providers-github-2.3.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-github-2.2.1rc1/MANIFEST.in` & `apache-airflow-providers-github-2.3.0rc1/MANIFEST.in`

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

### Comparing `apache-airflow-providers-github-2.2.1rc1/PKG-INFO` & `apache-airflow-providers-github-2.3.0rc1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-github
-Version: 2.2.1rc1
+Version: 2.3.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-github package
 Home-page: https://airflow.apache.org/
+Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Download-URL: https://archive.apache.org/dist/airflow/providers
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-github/2.2.1/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-github/2.3.0/
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
 
 
 Package ``apache-airflow-providers-github``
 
-Release: ``2.2.1rc1``
+Release: ``2.3.0rc1``
 
 
 `GitHub <https://www.github.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``github`` provider. All classes for this provider package
 are in ``airflow.providers.github`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-github/2.2.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-github/2.3.0/>`_.
 
 
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
 ``PyGithub!``       ``=1.58``
 ==================  ==================
 
 
 
  .. Licensed to the Apache Software Foundation (ASF) under one
     or more contributor license agreements.  See the NOTICE file
@@ -106,14 +105,31 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 Changelog
 ---------
 
+2.3.0
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
 2.2.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
 
 * ``Handle 'github_method_args' in GithubOperator when not provided (#29699)``
@@ -121,16 +137,17 @@
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Exclude v1.58 of 'PyGithub' package in GitHub provider (#29728)``
 
 2.2.0
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
@@ -154,16 +171,17 @@
 
 2.0.0
 .....
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
-* This release of provider is only available for Airflow 2.2+ as explained in the Apache Airflow
-  providers support policy https://github.com/apache/airflow/blob/main/README.md#support-for-providers
+.. note::
+  This release of provider is only available for Airflow 2.2+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Bug Fixes
 ~~~~~~~~~
 
    * ``Remove 'GithubOperator' use in  'GithubSensor.__init__()'' (#24214)``
 
 .. Below changes are excluded from the changelog. Move them to
@@ -205,9 +223,7 @@
    * ``Add pre-commit check for docstring param types (#21398)``
 
 
 1.0.0
 .....
 
 Initial version of the provider.
-
-
```

### Comparing `apache-airflow-providers-github-2.2.1rc1/README.rst` & `apache-airflow-providers-github-2.3.0rc1/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -15,28 +15,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-github``
 
-Release: ``2.2.1rc1``
+Release: ``2.3.0rc1``
 
 
 `GitHub <https://www.github.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``github`` provider. All classes for this provider package
 are in ``airflow.providers.github`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-github/2.2.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-github/2.3.0/>`_.
 
 
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
 ``PyGithub!``       ``=1.58``
 ==================  ==================
 
 
 
  .. Licensed to the Apache Software Foundation (ASF) under one
     or more contributor license agreements.  See the NOTICE file
@@ -72,14 +72,31 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 Changelog
 ---------
 
+2.3.0
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
 2.2.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
 
 * ``Handle 'github_method_args' in GithubOperator when not provided (#29699)``
@@ -87,16 +104,17 @@
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Exclude v1.58 of 'PyGithub' package in GitHub provider (#29728)``
 
 2.2.0
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
@@ -120,16 +138,17 @@
 
 2.0.0
 .....
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
-* This release of provider is only available for Airflow 2.2+ as explained in the Apache Airflow
-  providers support policy https://github.com/apache/airflow/blob/main/README.md#support-for-providers
+.. note::
+  This release of provider is only available for Airflow 2.2+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Bug Fixes
 ~~~~~~~~~
 
    * ``Remove 'GithubOperator' use in  'GithubSensor.__init__()'' (#24214)``
 
 .. Below changes are excluded from the changelog. Move them to
```

### Comparing `apache-airflow-providers-github-2.2.1rc1/airflow/providers/github/__init__.py` & `apache-airflow-providers-github-2.3.0rc1/airflow/providers/github/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-github-2.2.1rc1/airflow/providers/github/get_provider_info.py` & `apache-airflow-providers-github-2.3.0rc1/airflow/providers/github/get_provider_info.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,16 +23,17 @@
 
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-github",
         "name": "Github",
         "description": "`GitHub <https://www.github.com/>`__\n",
-        "dependencies": ["apache-airflow>=2.3.0", "PyGithub!=1.58"],
-        "versions": ["2.2.1", "2.2.0", "2.1.0", "2.0.0", "1.0.3", "1.0.2", "1.0.1", "1.0.0"],
+        "dependencies": ["apache-airflow>=2.4.0", "PyGithub!=1.58"],
+        "suspended": False,
+        "versions": ["2.3.0", "2.2.1", "2.2.0", "2.1.0", "2.0.0", "1.0.3", "1.0.2", "1.0.1", "1.0.0"],
         "integrations": [
             {
                 "integration-name": "Github",
                 "external-doc-url": "https://www.github.com/",
                 "tags": ["software"],
             }
         ],
```

### Comparing `apache-airflow-providers-github-2.2.1rc1/airflow/providers/github/hooks/__init__.py` & `apache-airflow-providers-github-2.3.0rc1/airflow/providers/github/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-github-2.2.1rc1/airflow/providers/github/hooks/github.py` & `apache-airflow-providers-github-2.3.0rc1/airflow/providers/github/hooks/github.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-github-2.2.1rc1/airflow/providers/github/operators/__init__.py` & `apache-airflow-providers-github-2.3.0rc1/airflow/providers/github/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-github-2.2.1rc1/airflow/providers/github/operators/github.py` & `apache-airflow-providers-github-2.3.0rc1/airflow/providers/github/operators/github.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-github-2.2.1rc1/airflow/providers/github/sensors/github.py` & `apache-airflow-providers-github-2.3.0rc1/airflow/providers/github/sensors/github.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-github-2.2.1rc1/apache_airflow_providers_github.egg-info/PKG-INFO` & `apache-airflow-providers-github-2.3.0rc1/apache_airflow_providers_github.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-github
-Version: 2.2.1rc1
+Version: 2.3.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-github package
 Home-page: https://airflow.apache.org/
+Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Download-URL: https://archive.apache.org/dist/airflow/providers
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-github/2.2.1/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-github/2.3.0/
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
 
 
 Package ``apache-airflow-providers-github``
 
-Release: ``2.2.1rc1``
+Release: ``2.3.0rc1``
 
 
 `GitHub <https://www.github.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``github`` provider. All classes for this provider package
 are in ``airflow.providers.github`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-github/2.2.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-github/2.3.0/>`_.
 
 
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
 ``PyGithub!``       ``=1.58``
 ==================  ==================
 
 
 
  .. Licensed to the Apache Software Foundation (ASF) under one
     or more contributor license agreements.  See the NOTICE file
@@ -106,14 +105,31 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 Changelog
 ---------
 
+2.3.0
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
 2.2.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
 
 * ``Handle 'github_method_args' in GithubOperator when not provided (#29699)``
@@ -121,16 +137,17 @@
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Exclude v1.58 of 'PyGithub' package in GitHub provider (#29728)``
 
 2.2.0
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
@@ -154,16 +171,17 @@
 
 2.0.0
 .....
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
-* This release of provider is only available for Airflow 2.2+ as explained in the Apache Airflow
-  providers support policy https://github.com/apache/airflow/blob/main/README.md#support-for-providers
+.. note::
+  This release of provider is only available for Airflow 2.2+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Bug Fixes
 ~~~~~~~~~
 
    * ``Remove 'GithubOperator' use in  'GithubSensor.__init__()'' (#24214)``
 
 .. Below changes are excluded from the changelog. Move them to
@@ -205,9 +223,7 @@
    * ``Add pre-commit check for docstring param types (#21398)``
 
 
 1.0.0
 .....
 
 Initial version of the provider.
-
-
```

### Comparing `apache-airflow-providers-github-2.2.1rc1/apache_airflow_providers_github.egg-info/SOURCES.txt` & `apache-airflow-providers-github-2.3.0rc1/apache_airflow_providers_github.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-github-2.2.1rc1/pyproject.toml` & `apache-airflow-providers-github-2.3.0rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-github-2.2.1rc1/setup.cfg` & `apache-airflow-providers-github-2.3.0rc1/setup.cfg`

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-github/2.2.1/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-github/2.3.0/
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
@@ -43,15 +43,15 @@
 python_requires = ~=3.7
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
 	PyGithub!=1.58
-	apache-airflow>=2.3.0.dev0
+	apache-airflow>=2.4.0.dev0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.github.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.github
```

### Comparing `apache-airflow-providers-github-2.2.1rc1/setup.py` & `apache-airflow-providers-github-2.3.0rc1/airflow/providers/github/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,32 +11,28 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
-
+#
 # NOTE! THIS FILE IS AUTOMATICALLY GENERATED AND WILL BE
-# OVERWRITTEN WHEN PREPARING PACKAGES.
+# OVERWRITTEN WHEN PREPARING DOCUMENTATION FOR THE PACKAGES.
 #
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
-# `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
+# `PROVIDER__INIT__PY_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
+#
+from __future__ import annotations
 
-"""Setup.py for the apache-airflow-providers-github package."""
+import packaging.version
 
-from setuptools import find_namespace_packages, setup
+import airflow
 
-version = "2.2.1"
+__all__ = ["version"]
 
+version = "2.3.0"
 
-def do_setup():
-    """Perform the package apache-airflow-providers-github setup."""
-    setup(
-        version=version,
-        extras_require={},
-        packages=find_namespace_packages(include=["airflow.providers.github", "airflow.providers.github.*"]),
+if packaging.version.parse(airflow.version.version) < packaging.version.parse("2.4.0"):
+    raise RuntimeError(
+        f"The package `apache-airflow-providers-github:{version}` requires Apache Airflow 2.4.0+"
     )
-
-
-if __name__ == "__main__":
-    do_setup()
```

