# Comparing `tmp/apache-airflow-providers-http-4.3.0rc1.tar.gz` & `tmp/apache-airflow-providers-http-4.4.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-http-4.3.0rc1.tar", last modified: Sun Apr  2 05:48:49 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-http-4.4.0rc1.tar", last modified: Tue May 16 15:54:21 2023, max compression
```

## Comparing `apache-airflow-providers-http-4.3.0rc1.tar` & `apache-airflow-providers-http-4.4.0rc1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:48:49.000000 apache-airflow-providers-http-4.3.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-http-4.3.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1122 2023-04-02 05:48:48.000000 apache-airflow-providers-http-4.3.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-http-4.3.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    11493 2023-04-02 05:48:49.000000 apache-airflow-providers-http-4.3.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9972 2023-04-02 05:48:48.000000 apache-airflow-providers-http-4.3.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:48:49.000000 apache-airflow-providers-http-4.3.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:48:49.000000 apache-airflow-providers-http-4.3.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:48:49.000000 apache-airflow-providers-http-4.3.0rc1/airflow/providers/http/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-http-4.3.0rc1/airflow/providers/http/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2901 2023-04-02 05:48:48.000000 apache-airflow-providers-http-4.3.0rc1/airflow/providers/http/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:48:49.000000 apache-airflow-providers-http-4.3.0rc1/airflow/providers/http/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-http-4.3.0rc1/airflow/providers/http/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16289 2023-03-27 08:32:49.000000 apache-airflow-providers-http-4.3.0rc1/airflow/providers/http/hooks/http.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:48:49.000000 apache-airflow-providers-http-4.3.0rc1/airflow/providers/http/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-http-4.3.0rc1/airflow/providers/http/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5828 2023-03-27 08:32:49.000000 apache-airflow-providers-http-4.3.0rc1/airflow/providers/http/operators/http.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:48:49.000000 apache-airflow-providers-http-4.3.0rc1/airflow/providers/http/sensors/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-http-4.3.0rc1/airflow/providers/http/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5885 2023-02-24 18:43:53.000000 apache-airflow-providers-http-4.3.0rc1/airflow/providers/http/sensors/http.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:48:49.000000 apache-airflow-providers-http-4.3.0rc1/apache_airflow_providers_http.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11493 2023-04-02 05:48:49.000000 apache-airflow-providers-http-4.3.0rc1/apache_airflow_providers_http.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      768 2023-04-02 05:48:49.000000 apache-airflow-providers-http-4.3.0rc1/apache_airflow_providers_http.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-02 05:48:49.000000 apache-airflow-providers-http-4.3.0rc1/apache_airflow_providers_http.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      101 2023-04-02 05:48:49.000000 apache-airflow-providers-http-4.3.0rc1/apache_airflow_providers_http.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-02 05:48:49.000000 apache-airflow-providers-http-4.3.0rc1/apache_airflow_providers_http.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       51 2023-04-02 05:48:49.000000 apache-airflow-providers-http-4.3.0rc1/apache_airflow_providers_http.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-02 05:48:49.000000 apache-airflow-providers-http-4.3.0rc1/apache_airflow_providers_http.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5393 2023-04-01 16:40:04.000000 apache-airflow-providers-http-4.3.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1843 2023-04-02 05:48:49.000000 apache-airflow-providers-http-4.3.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1456 2023-04-02 05:48:48.000000 apache-airflow-providers-http-4.3.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:21.000000 apache-airflow-providers-http-4.4.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-http-4.4.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-05-16 15:54:20.000000 apache-airflow-providers-http-4.4.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-http-4.4.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    12021 2023-05-16 15:54:21.000000 apache-airflow-providers-http-4.4.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10500 2023-05-16 15:54:20.000000 apache-airflow-providers-http-4.4.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:21.000000 apache-airflow-providers-http-4.4.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:21.000000 apache-airflow-providers-http-4.4.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:21.000000 apache-airflow-providers-http-4.4.0rc1/airflow/providers/http/
+-rw-r--r--   0 root         (0) root         (0)     1387 2023-05-16 15:39:21.000000 apache-airflow-providers-http-4.4.0rc1/airflow/providers/http/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2950 2023-05-16 15:54:20.000000 apache-airflow-providers-http-4.4.0rc1/airflow/providers/http/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:21.000000 apache-airflow-providers-http-4.4.0rc1/airflow/providers/http/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-http-4.4.0rc1/airflow/providers/http/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16287 2023-04-24 21:04:25.000000 apache-airflow-providers-http-4.4.0rc1/airflow/providers/http/hooks/http.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:21.000000 apache-airflow-providers-http-4.4.0rc1/airflow/providers/http/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-http-4.4.0rc1/airflow/providers/http/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5828 2023-03-27 08:32:49.000000 apache-airflow-providers-http-4.4.0rc1/airflow/providers/http/operators/http.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:21.000000 apache-airflow-providers-http-4.4.0rc1/airflow/providers/http/sensors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-http-4.4.0rc1/airflow/providers/http/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5885 2023-02-24 18:43:53.000000 apache-airflow-providers-http-4.4.0rc1/airflow/providers/http/sensors/http.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:21.000000 apache-airflow-providers-http-4.4.0rc1/apache_airflow_providers_http.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    12021 2023-05-16 15:54:21.000000 apache-airflow-providers-http-4.4.0rc1/apache_airflow_providers_http.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      768 2023-05-16 15:54:21.000000 apache-airflow-providers-http-4.4.0rc1/apache_airflow_providers_http.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:54:21.000000 apache-airflow-providers-http-4.4.0rc1/apache_airflow_providers_http.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      101 2023-05-16 15:54:21.000000 apache-airflow-providers-http-4.4.0rc1/apache_airflow_providers_http.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:54:21.000000 apache-airflow-providers-http-4.4.0rc1/apache_airflow_providers_http.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       51 2023-05-16 15:54:21.000000 apache-airflow-providers-http-4.4.0rc1/apache_airflow_providers_http.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-16 15:54:21.000000 apache-airflow-providers-http-4.4.0rc1/apache_airflow_providers_http.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5308 2023-05-15 09:39:26.000000 apache-airflow-providers-http-4.4.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1843 2023-05-16 15:54:21.000000 apache-airflow-providers-http-4.4.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1626 2023-05-16 15:54:20.000000 apache-airflow-providers-http-4.4.0rc1/setup.py
```

### Comparing `apache-airflow-providers-http-4.3.0rc1/LICENSE` & `apache-airflow-providers-http-4.4.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-http-4.3.0rc1/MANIFEST.in` & `apache-airflow-providers-http-4.4.0rc1/MANIFEST.in`

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

### Comparing `apache-airflow-providers-http-4.3.0rc1/PKG-INFO` & `apache-airflow-providers-http-4.4.0rc1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-http
-Version: 4.3.0rc1
+Version: 4.4.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-http package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-http/4.3.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-http/4.4.0/
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -48,28 +48,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-http``
 
-Release: ``4.3.0rc1``
+Release: ``4.4.0rc1``
 
 
 `Hypertext Transfer Protocol (HTTP) <https://www.w3.org/Protocols/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``http`` provider. All classes for this provider package
 are in ``airflow.providers.http`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-http/4.3.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-http/4.4.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -111,53 +111,58 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
-4.3.0
+4.4.0
 .....
 
-Breaking changes
-~~~~~~~~~~~~~~~~
+.. note::
+  This release of provider is only available for Airflow 2.4+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
+
 
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Upgrade ruff to 0.0.262 (#30809)``
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add mechanism to suspend providers (#30422)``
+
+4.3.0
+.....
 
 Features
 ~~~~~~~~
 
 * ``Add non login-password auth support for SimpleHttpOpeator (#29206)``
 
-Bug Fixes
-~~~~~~~~~
-
-
-.. Below changes are excluded from the changelog. Move them to
-   appropriate section above if needed. Do not delete the lines(!):
-
 4.2.0
 .....
 
 Features
 ~~~~~~~~
 
 * ``Add HttpHookAsync for deferrable implementation (#29038)``
 
 4.1.1
 .....
 
 Misc
 ~~~~
+
 * ``Change logging for HttpHook to debug (#28911)``
 
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
@@ -191,16 +196,17 @@
 
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
    * ``Migrate HTTP example DAGs to new design AIP-47 (#23991)``
    * ``Add explanatory note for contributors about updating Changelog (#24229)``
    * ``Prepare docs for May 2022 provider's release (#24231)``
    * ``Update package description to remove double min-airflow specification (#24292)``
```

### Comparing `apache-airflow-providers-http-4.3.0rc1/README.rst` & `apache-airflow-providers-http-4.4.0rc1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -15,28 +15,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-http``
 
-Release: ``4.3.0rc1``
+Release: ``4.4.0rc1``
 
 
 `Hypertext Transfer Protocol (HTTP) <https://www.w3.org/Protocols/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``http`` provider. All classes for this provider package
 are in ``airflow.providers.http`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-http/4.3.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-http/4.4.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -78,53 +78,58 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
-4.3.0
+4.4.0
 .....
 
-Breaking changes
-~~~~~~~~~~~~~~~~
+.. note::
+  This release of provider is only available for Airflow 2.4+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
+
 
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Upgrade ruff to 0.0.262 (#30809)``
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add mechanism to suspend providers (#30422)``
+
+4.3.0
+.....
 
 Features
 ~~~~~~~~
 
 * ``Add non login-password auth support for SimpleHttpOpeator (#29206)``
 
-Bug Fixes
-~~~~~~~~~
-
-
-.. Below changes are excluded from the changelog. Move them to
-   appropriate section above if needed. Do not delete the lines(!):
-
 4.2.0
 .....
 
 Features
 ~~~~~~~~
 
 * ``Add HttpHookAsync for deferrable implementation (#29038)``
 
 4.1.1
 .....
 
 Misc
 ~~~~
+
 * ``Change logging for HttpHook to debug (#28911)``
 
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
@@ -158,16 +163,17 @@
 
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
    * ``Migrate HTTP example DAGs to new design AIP-47 (#23991)``
    * ``Add explanatory note for contributors about updating Changelog (#24229)``
    * ``Prepare docs for May 2022 provider's release (#24231)``
    * ``Update package description to remove double min-airflow specification (#24292)``
```

### Comparing `apache-airflow-providers-http-4.3.0rc1/airflow/providers/http/__init__.py` & `apache-airflow-providers-http-4.4.0rc1/airflow/providers/http/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-http-4.3.0rc1/airflow/providers/http/get_provider_info.py` & `apache-airflow-providers-http-4.4.0rc1/airflow/providers/http/get_provider_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,17 @@
 
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-http",
         "name": "Hypertext Transfer Protocol (HTTP)",
         "description": "`Hypertext Transfer Protocol (HTTP) <https://www.w3.org/Protocols/>`__\n",
+        "suspended": False,
         "versions": [
+            "4.4.0",
             "4.3.0",
             "4.2.0",
             "4.1.1",
             "4.1.0",
             "4.0.0",
             "3.0.0",
             "2.1.2",
```

### Comparing `apache-airflow-providers-http-4.3.0rc1/airflow/providers/http/hooks/__init__.py` & `apache-airflow-providers-http-4.4.0rc1/airflow/providers/http/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-http-4.3.0rc1/airflow/providers/http/hooks/http.py` & `apache-airflow-providers-http-4.4.0rc1/airflow/providers/http/hooks/http.py`

 * *Files 0% similar despite different names*

```diff
@@ -302,15 +302,15 @@
 
     async def run(
         self,
         endpoint: str | None = None,
         data: dict[str, Any] | str | None = None,
         headers: dict[str, Any] | None = None,
         extra_options: dict[str, Any] | None = None,
-    ) -> "ClientResponse":
+    ) -> ClientResponse:
         r"""
         Performs an asynchronous HTTP request call
 
         :param endpoint: the endpoint to be called i.e. resource/v1/query?
         :param data: payload to be uploaded or request parameters
         :param headers: additional headers to be passed through as a dictionary
         :param extra_options: Additional kwargs to pass when creating a request.
```

### Comparing `apache-airflow-providers-http-4.3.0rc1/airflow/providers/http/operators/__init__.py` & `apache-airflow-providers-http-4.4.0rc1/airflow/providers/http/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-http-4.3.0rc1/airflow/providers/http/operators/http.py` & `apache-airflow-providers-http-4.4.0rc1/airflow/providers/http/operators/http.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-http-4.3.0rc1/airflow/providers/http/sensors/http.py` & `apache-airflow-providers-http-4.4.0rc1/airflow/providers/http/sensors/http.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-http-4.3.0rc1/apache_airflow_providers_http.egg-info/PKG-INFO` & `apache-airflow-providers-http-4.4.0rc1/apache_airflow_providers_http.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-http
-Version: 4.3.0rc1
+Version: 4.4.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-http package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-http/4.3.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-http/4.4.0/
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -48,28 +48,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-http``
 
-Release: ``4.3.0rc1``
+Release: ``4.4.0rc1``
 
 
 `Hypertext Transfer Protocol (HTTP) <https://www.w3.org/Protocols/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``http`` provider. All classes for this provider package
 are in ``airflow.providers.http`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-http/4.3.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-http/4.4.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -111,53 +111,58 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
-4.3.0
+4.4.0
 .....
 
-Breaking changes
-~~~~~~~~~~~~~~~~
+.. note::
+  This release of provider is only available for Airflow 2.4+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
+
 
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Upgrade ruff to 0.0.262 (#30809)``
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add mechanism to suspend providers (#30422)``
+
+4.3.0
+.....
 
 Features
 ~~~~~~~~
 
 * ``Add non login-password auth support for SimpleHttpOpeator (#29206)``
 
-Bug Fixes
-~~~~~~~~~
-
-
-.. Below changes are excluded from the changelog. Move them to
-   appropriate section above if needed. Do not delete the lines(!):
-
 4.2.0
 .....
 
 Features
 ~~~~~~~~
 
 * ``Add HttpHookAsync for deferrable implementation (#29038)``
 
 4.1.1
 .....
 
 Misc
 ~~~~
+
 * ``Change logging for HttpHook to debug (#28911)``
 
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
@@ -191,16 +196,17 @@
 
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
    * ``Migrate HTTP example DAGs to new design AIP-47 (#23991)``
    * ``Add explanatory note for contributors about updating Changelog (#24229)``
    * ``Prepare docs for May 2022 provider's release (#24231)``
    * ``Update package description to remove double min-airflow specification (#24292)``
```

### Comparing `apache-airflow-providers-http-4.3.0rc1/apache_airflow_providers_http.egg-info/SOURCES.txt` & `apache-airflow-providers-http-4.4.0rc1/apache_airflow_providers_http.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-http-4.3.0rc1/pyproject.toml` & `apache-airflow-providers-http-4.4.0rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-http-4.3.0rc1/setup.cfg` & `apache-airflow-providers-http-4.4.0rc1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-http/4.3.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-http/4.4.0/
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
```

### Comparing `apache-airflow-providers-http-4.3.0rc1/setup.py` & `apache-airflow-providers-http-4.4.0rc1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,21 +22,28 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-http package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "4.3.0"
+version = "4.4.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-http setup."""
     setup(
         version=version,
         extras_require={},
-        packages=find_namespace_packages(include=["airflow.providers.http", "airflow.providers.http.*"]),
+        packages=find_namespace_packages(
+            include=[
+                "airflow.providers.http",
+                "airflow.providers.http.*",
+                "airflow.providers.http_vendor",
+                "airflow.providers.http_vendor.*",
+            ],
+        ),
     )
 
 
 if __name__ == "__main__":
     do_setup()
```

