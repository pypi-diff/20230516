# Comparing `tmp/apache-airflow-providers-airbyte-3.2.1rc1.tar.gz` & `tmp/apache-airflow-providers-airbyte-3.3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-airbyte-3.2.1rc1.tar", last modified: Sun Apr  2 05:46:42 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-airbyte-3.3.0rc1.tar", last modified: Tue May 16 15:52:45 2023, max compression
```

## Comparing `apache-airflow-providers-airbyte-3.2.1rc1.tar` & `apache-airflow-providers-airbyte-3.3.0rc1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:46:42.000000 apache-airflow-providers-airbyte-3.2.1rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-airbyte-3.2.1rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1122 2023-04-02 05:46:40.000000 apache-airflow-providers-airbyte-3.2.1rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-airbyte-3.2.1rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    10607 2023-04-02 05:46:42.000000 apache-airflow-providers-airbyte-3.2.1rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9056 2023-04-02 05:46:40.000000 apache-airflow-providers-airbyte-3.2.1rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:46:42.000000 apache-airflow-providers-airbyte-3.2.1rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:46:42.000000 apache-airflow-providers-airbyte-3.2.1rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:46:42.000000 apache-airflow-providers-airbyte-3.2.1rc1/airflow/providers/airbyte/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-airbyte-3.2.1rc1/airflow/providers/airbyte/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2568 2023-04-02 05:46:40.000000 apache-airflow-providers-airbyte-3.2.1rc1/airflow/providers/airbyte/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:46:42.000000 apache-airflow-providers-airbyte-3.2.1rc1/airflow/providers/airbyte/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-airbyte-3.2.1rc1/airflow/providers/airbyte/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5059 2023-03-11 12:12:47.000000 apache-airflow-providers-airbyte-3.2.1rc1/airflow/providers/airbyte/hooks/airbyte.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:46:42.000000 apache-airflow-providers-airbyte-3.2.1rc1/airflow/providers/airbyte/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-airbyte-3.2.1rc1/airflow/providers/airbyte/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3869 2023-03-11 12:12:47.000000 apache-airflow-providers-airbyte-3.2.1rc1/airflow/providers/airbyte/operators/airbyte.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:46:42.000000 apache-airflow-providers-airbyte-3.2.1rc1/airflow/providers/airbyte/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-airbyte-3.2.1rc1/airflow/providers/airbyte/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2793 2023-03-11 12:12:47.000000 apache-airflow-providers-airbyte-3.2.1rc1/airflow/providers/airbyte/sensors/airbyte.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:46:42.000000 apache-airflow-providers-airbyte-3.2.1rc1/apache_airflow_providers_airbyte.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10607 2023-04-02 05:46:41.000000 apache-airflow-providers-airbyte-3.2.1rc1/apache_airflow_providers_airbyte.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      822 2023-04-02 05:46:41.000000 apache-airflow-providers-airbyte-3.2.1rc1/apache_airflow_providers_airbyte.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-02 05:46:41.000000 apache-airflow-providers-airbyte-3.2.1rc1/apache_airflow_providers_airbyte.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-04-02 05:46:41.000000 apache-airflow-providers-airbyte-3.2.1rc1/apache_airflow_providers_airbyte.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-02 05:46:41.000000 apache-airflow-providers-airbyte-3.2.1rc1/apache_airflow_providers_airbyte.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       95 2023-04-02 05:46:41.000000 apache-airflow-providers-airbyte-3.2.1rc1/apache_airflow_providers_airbyte.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-02 05:46:41.000000 apache-airflow-providers-airbyte-3.2.1rc1/apache_airflow_providers_airbyte.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5393 2023-04-01 16:40:04.000000 apache-airflow-providers-airbyte-3.2.1rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1865 2023-04-02 05:46:42.000000 apache-airflow-providers-airbyte-3.2.1rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1531 2023-04-02 05:46:40.000000 apache-airflow-providers-airbyte-3.2.1rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:45.000000 apache-airflow-providers-airbyte-3.3.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-airbyte-3.3.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-05-16 15:52:44.000000 apache-airflow-providers-airbyte-3.3.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-airbyte-3.3.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    11350 2023-05-16 15:52:45.000000 apache-airflow-providers-airbyte-3.3.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9799 2023-05-16 15:52:44.000000 apache-airflow-providers-airbyte-3.3.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:45.000000 apache-airflow-providers-airbyte-3.3.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:45.000000 apache-airflow-providers-airbyte-3.3.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:45.000000 apache-airflow-providers-airbyte-3.3.0rc1/airflow/providers/airbyte/
+-rw-r--r--   0 root         (0) root         (0)     1390 2023-05-16 15:39:21.000000 apache-airflow-providers-airbyte-3.3.0rc1/airflow/providers/airbyte/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2617 2023-05-16 15:52:44.000000 apache-airflow-providers-airbyte-3.3.0rc1/airflow/providers/airbyte/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:45.000000 apache-airflow-providers-airbyte-3.3.0rc1/airflow/providers/airbyte/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-airbyte-3.3.0rc1/airflow/providers/airbyte/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5059 2023-03-11 12:12:47.000000 apache-airflow-providers-airbyte-3.3.0rc1/airflow/providers/airbyte/hooks/airbyte.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:45.000000 apache-airflow-providers-airbyte-3.3.0rc1/airflow/providers/airbyte/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-airbyte-3.3.0rc1/airflow/providers/airbyte/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3869 2023-03-11 12:12:47.000000 apache-airflow-providers-airbyte-3.3.0rc1/airflow/providers/airbyte/operators/airbyte.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:45.000000 apache-airflow-providers-airbyte-3.3.0rc1/airflow/providers/airbyte/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-airbyte-3.3.0rc1/airflow/providers/airbyte/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2793 2023-03-11 12:12:47.000000 apache-airflow-providers-airbyte-3.3.0rc1/airflow/providers/airbyte/sensors/airbyte.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:45.000000 apache-airflow-providers-airbyte-3.3.0rc1/apache_airflow_providers_airbyte.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11350 2023-05-16 15:52:45.000000 apache-airflow-providers-airbyte-3.3.0rc1/apache_airflow_providers_airbyte.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      822 2023-05-16 15:52:45.000000 apache-airflow-providers-airbyte-3.3.0rc1/apache_airflow_providers_airbyte.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:52:45.000000 apache-airflow-providers-airbyte-3.3.0rc1/apache_airflow_providers_airbyte.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2023-05-16 15:52:45.000000 apache-airflow-providers-airbyte-3.3.0rc1/apache_airflow_providers_airbyte.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:52:45.000000 apache-airflow-providers-airbyte-3.3.0rc1/apache_airflow_providers_airbyte.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       95 2023-05-16 15:52:45.000000 apache-airflow-providers-airbyte-3.3.0rc1/apache_airflow_providers_airbyte.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-16 15:52:45.000000 apache-airflow-providers-airbyte-3.3.0rc1/apache_airflow_providers_airbyte.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5308 2023-05-15 09:39:26.000000 apache-airflow-providers-airbyte-3.3.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1865 2023-05-16 15:52:45.000000 apache-airflow-providers-airbyte-3.3.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1685 2023-05-16 15:52:44.000000 apache-airflow-providers-airbyte-3.3.0rc1/setup.py
```

### Comparing `apache-airflow-providers-airbyte-3.2.1rc1/LICENSE` & `apache-airflow-providers-airbyte-3.3.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-airbyte-3.2.1rc1/MANIFEST.in` & `apache-airflow-providers-airbyte-3.3.0rc1/MANIFEST.in`

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

### Comparing `apache-airflow-providers-airbyte-3.2.1rc1/PKG-INFO` & `apache-airflow-providers-airbyte-3.3.0rc1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-airbyte
-Version: 3.2.1rc1
+Version: 3.3.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-airbyte package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-airbyte/3.2.1/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-airbyte/3.3.0/
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -49,28 +49,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-airbyte``
 
-Release: ``3.2.1rc1``
+Release: ``3.3.0rc1``
 
 
 `Airbyte <https://airbyte.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``airbyte`` provider. All classes for this provider package
 are in ``airflow.providers.airbyte`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-airbyte/3.2.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-airbyte/3.3.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -80,15 +80,15 @@
 
 Requirements
 ------------
 
 =================================  ==================
 PIP package                        Version required
 =================================  ==================
-``apache-airflow``                 ``>=2.3.0``
+``apache-airflow``                 ``>=2.4.0``
 ``apache-airflow-providers-http``
 =================================  ==================
 
 Cross provider package dependencies
 -----------------------------------
 
 Those are dependencies that might be needed in order to use all the features of the package.
@@ -129,27 +129,45 @@
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
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add mechanism to suspend providers (#30422)``
+
 3.2.1
 .....
 
 Misc
 ~~~~
 
 * ``Clarify optional parameters in Airbyte docstrings (#30031)``
 
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
@@ -175,16 +193,17 @@
 
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

### Comparing `apache-airflow-providers-airbyte-3.2.1rc1/README.rst` & `apache-airflow-providers-airbyte-3.3.0rc1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -15,28 +15,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-airbyte``
 
-Release: ``3.2.1rc1``
+Release: ``3.3.0rc1``
 
 
 `Airbyte <https://airbyte.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``airbyte`` provider. All classes for this provider package
 are in ``airflow.providers.airbyte`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-airbyte/3.2.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-airbyte/3.3.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -46,15 +46,15 @@
 
 Requirements
 ------------
 
 =================================  ==================
 PIP package                        Version required
 =================================  ==================
-``apache-airflow``                 ``>=2.3.0``
+``apache-airflow``                 ``>=2.4.0``
 ``apache-airflow-providers-http``
 =================================  ==================
 
 Cross provider package dependencies
 -----------------------------------
 
 Those are dependencies that might be needed in order to use all the features of the package.
@@ -95,27 +95,45 @@
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
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add mechanism to suspend providers (#30422)``
+
 3.2.1
 .....
 
 Misc
 ~~~~
 
 * ``Clarify optional parameters in Airbyte docstrings (#30031)``
 
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
@@ -141,16 +159,17 @@
 
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

### Comparing `apache-airflow-providers-airbyte-3.2.1rc1/airflow/providers/airbyte/__init__.py` & `apache-airflow-providers-airbyte-3.3.0rc1/airflow/providers/airbyte/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-airbyte-3.2.1rc1/airflow/providers/airbyte/get_provider_info.py` & `apache-airflow-providers-airbyte-3.3.0rc1/airflow/providers/airbyte/get_provider_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,28 +23,30 @@
 
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-airbyte",
         "name": "Airbyte",
         "description": "`Airbyte <https://airbyte.io/>`__\n",
+        "suspended": False,
         "versions": [
+            "3.3.0",
             "3.2.1",
             "3.2.0",
             "3.1.0",
             "3.0.0",
             "2.1.4",
             "2.1.3",
             "2.1.2",
             "2.1.1",
             "2.1.0",
             "2.0.0",
             "1.0.0",
         ],
-        "dependencies": ["apache-airflow>=2.3.0", "apache-airflow-providers-http"],
+        "dependencies": ["apache-airflow>=2.4.0", "apache-airflow-providers-http"],
         "integrations": [
             {
                 "integration-name": "Airbyte",
                 "external-doc-url": "https://www.airbyte.io/",
                 "logo": "/integration-logos/airbyte/Airbyte.png",
                 "how-to-guide": ["/docs/apache-airflow-providers-airbyte/operators/airbyte.rst"],
                 "tags": ["service"],
```

### Comparing `apache-airflow-providers-airbyte-3.2.1rc1/airflow/providers/airbyte/hooks/__init__.py` & `apache-airflow-providers-airbyte-3.3.0rc1/airflow/providers/airbyte/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-airbyte-3.2.1rc1/airflow/providers/airbyte/hooks/airbyte.py` & `apache-airflow-providers-airbyte-3.3.0rc1/airflow/providers/airbyte/hooks/airbyte.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-airbyte-3.2.1rc1/airflow/providers/airbyte/operators/__init__.py` & `apache-airflow-providers-airbyte-3.3.0rc1/airflow/providers/airbyte/sensors/__init__.py`

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

### Comparing `apache-airflow-providers-airbyte-3.2.1rc1/airflow/providers/airbyte/operators/airbyte.py` & `apache-airflow-providers-airbyte-3.3.0rc1/airflow/providers/airbyte/operators/airbyte.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-airbyte-3.2.1rc1/airflow/providers/airbyte/sensors/airbyte.py` & `apache-airflow-providers-airbyte-3.3.0rc1/airflow/providers/airbyte/sensors/airbyte.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-airbyte-3.2.1rc1/apache_airflow_providers_airbyte.egg-info/PKG-INFO` & `apache-airflow-providers-airbyte-3.3.0rc1/apache_airflow_providers_airbyte.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-airbyte
-Version: 3.2.1rc1
+Version: 3.3.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-airbyte package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-airbyte/3.2.1/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-airbyte/3.3.0/
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -49,28 +49,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-airbyte``
 
-Release: ``3.2.1rc1``
+Release: ``3.3.0rc1``
 
 
 `Airbyte <https://airbyte.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``airbyte`` provider. All classes for this provider package
 are in ``airflow.providers.airbyte`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-airbyte/3.2.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-airbyte/3.3.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -80,15 +80,15 @@
 
 Requirements
 ------------
 
 =================================  ==================
 PIP package                        Version required
 =================================  ==================
-``apache-airflow``                 ``>=2.3.0``
+``apache-airflow``                 ``>=2.4.0``
 ``apache-airflow-providers-http``
 =================================  ==================
 
 Cross provider package dependencies
 -----------------------------------
 
 Those are dependencies that might be needed in order to use all the features of the package.
@@ -129,27 +129,45 @@
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
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add mechanism to suspend providers (#30422)``
+
 3.2.1
 .....
 
 Misc
 ~~~~
 
 * ``Clarify optional parameters in Airbyte docstrings (#30031)``
 
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
@@ -175,16 +193,17 @@
 
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

### Comparing `apache-airflow-providers-airbyte-3.2.1rc1/apache_airflow_providers_airbyte.egg-info/SOURCES.txt` & `apache-airflow-providers-airbyte-3.3.0rc1/apache_airflow_providers_airbyte.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-airbyte-3.2.1rc1/pyproject.toml` & `apache-airflow-providers-airbyte-3.3.0rc1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,16 @@
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
@@ -135,18 +137,15 @@
 
 # The test_python.py is needed because adding __future__.annotations breaks runtime checks that are
 # needed for the test to work
 "tests/decorators/test_python.py" = ["I002"]
 
 # The Pydantic representations of SqlAlchemy Models are not parsed well with Pydantic
 # when __future__.annotations is used so we need to skip them from upgrading
-"airflow/models/pydantic/taskinstance.py" = ["I002"]
-"airflow/models/pydantic/dag_run.py" = ["I002"]
-"airflow/models/pydantic/dataset.py" = ["I002"]
-"airflow/jobs/pydantic/base_job.py" = ["I002"]
+"airflow/serialization/pydantic/*.py" = ["I002"]
 
 # Ignore pydoc style from these
 "*.pyi" = ["D"]
 "tests/*" = ["D"]
 "scripts/*" = ["D"]
 "dev/*" = ["D"]
 "docs/*" = ["D"]
```

### Comparing `apache-airflow-providers-airbyte-3.2.1rc1/setup.cfg` & `apache-airflow-providers-airbyte-3.3.0rc1/setup.cfg`

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-airbyte/3.2.1/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-airbyte/3.3.0/
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
 	apache-airflow-providers-http
-	apache-airflow>=2.3.0.dev0
+	apache-airflow>=2.4.0.dev0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.airbyte.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.airbyte
```

### Comparing `apache-airflow-providers-airbyte-3.2.1rc1/setup.py` & `apache-airflow-providers-airbyte-3.3.0rc1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,23 +22,28 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-airbyte package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "3.2.1"
+version = "3.3.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-airbyte setup."""
     setup(
         version=version,
         extras_require={"http": ["apache-airflow-providers-http"]},
         packages=find_namespace_packages(
-            include=["airflow.providers.airbyte", "airflow.providers.airbyte.*"]
+            include=[
+                "airflow.providers.airbyte",
+                "airflow.providers.airbyte.*",
+                "airflow.providers.airbyte_vendor",
+                "airflow.providers.airbyte_vendor.*",
+            ],
         ),
     )
 
 
 if __name__ == "__main__":
     do_setup()
```

