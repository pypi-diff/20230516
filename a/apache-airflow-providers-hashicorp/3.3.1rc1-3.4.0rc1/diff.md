# Comparing `tmp/apache-airflow-providers-hashicorp-3.3.1rc1.tar.gz` & `tmp/apache-airflow-providers-hashicorp-3.4.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-hashicorp-3.3.1rc1.tar", last modified: Sun Apr  2 05:48:46 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-hashicorp-3.4.0rc1.tar", last modified: Tue May 16 15:54:19 2023, max compression
```

## Comparing `apache-airflow-providers-hashicorp-3.3.1rc1.tar` & `apache-airflow-providers-hashicorp-3.4.0rc1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:48:46.000000 apache-airflow-providers-hashicorp-3.3.1rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-hashicorp-3.3.1rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1122 2023-04-02 05:48:42.000000 apache-airflow-providers-hashicorp-3.3.1rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-hashicorp-3.3.1rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    11714 2023-04-02 05:48:46.000000 apache-airflow-providers-hashicorp-3.3.1rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10155 2023-04-02 05:48:42.000000 apache-airflow-providers-hashicorp-3.3.1rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:48:46.000000 apache-airflow-providers-hashicorp-3.3.1rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:48:46.000000 apache-airflow-providers-hashicorp-3.3.1rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:48:46.000000 apache-airflow-providers-hashicorp-3.3.1rc1/airflow/providers/hashicorp/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-hashicorp-3.3.1rc1/airflow/providers/hashicorp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:48:46.000000 apache-airflow-providers-hashicorp-3.3.1rc1/airflow/providers/hashicorp/_internal_client/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-hashicorp-3.3.1rc1/airflow/providers/hashicorp/_internal_client/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20535 2023-02-24 18:43:53.000000 apache-airflow-providers-hashicorp-3.3.1rc1/airflow/providers/hashicorp/_internal_client/vault_client.py
--rw-r--r--   0 root         (0) root         (0)     2474 2023-04-02 05:48:42.000000 apache-airflow-providers-hashicorp-3.3.1rc1/airflow/providers/hashicorp/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:48:46.000000 apache-airflow-providers-hashicorp-3.3.1rc1/airflow/providers/hashicorp/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-hashicorp-3.3.1rc1/airflow/providers/hashicorp/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18653 2023-03-16 20:46:35.000000 apache-airflow-providers-hashicorp-3.3.1rc1/airflow/providers/hashicorp/hooks/vault.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:48:46.000000 apache-airflow-providers-hashicorp-3.3.1rc1/airflow/providers/hashicorp/secrets/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-hashicorp-3.3.1rc1/airflow/providers/hashicorp/secrets/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11906 2023-03-06 20:52:28.000000 apache-airflow-providers-hashicorp-3.3.1rc1/airflow/providers/hashicorp/secrets/vault.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:48:46.000000 apache-airflow-providers-hashicorp-3.3.1rc1/apache_airflow_providers_hashicorp.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11714 2023-04-02 05:48:46.000000 apache-airflow-providers-hashicorp-3.3.1rc1/apache_airflow_providers_hashicorp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      867 2023-04-02 05:48:46.000000 apache-airflow-providers-hashicorp-3.3.1rc1/apache_airflow_providers_hashicorp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-02 05:48:46.000000 apache-airflow-providers-hashicorp-3.3.1rc1/apache_airflow_providers_hashicorp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      106 2023-04-02 05:48:46.000000 apache-airflow-providers-hashicorp-3.3.1rc1/apache_airflow_providers_hashicorp.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-02 05:48:46.000000 apache-airflow-providers-hashicorp-3.3.1rc1/apache_airflow_providers_hashicorp.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       80 2023-04-02 05:48:46.000000 apache-airflow-providers-hashicorp-3.3.1rc1/apache_airflow_providers_hashicorp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-02 05:48:46.000000 apache-airflow-providers-hashicorp-3.3.1rc1/apache_airflow_providers_hashicorp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5393 2023-04-01 16:40:04.000000 apache-airflow-providers-hashicorp-3.3.1rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1858 2023-04-02 05:48:46.000000 apache-airflow-providers-hashicorp-3.3.1rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1543 2023-04-02 05:48:42.000000 apache-airflow-providers-hashicorp-3.3.1rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:19.000000 apache-airflow-providers-hashicorp-3.4.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-hashicorp-3.4.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-05-16 15:54:18.000000 apache-airflow-providers-hashicorp-3.4.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-hashicorp-3.4.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    12528 2023-05-16 15:54:19.000000 apache-airflow-providers-hashicorp-3.4.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10969 2023-05-16 15:54:18.000000 apache-airflow-providers-hashicorp-3.4.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:19.000000 apache-airflow-providers-hashicorp-3.4.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:19.000000 apache-airflow-providers-hashicorp-3.4.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:19.000000 apache-airflow-providers-hashicorp-3.4.0rc1/airflow/providers/hashicorp/
+-rw-r--r--   0 root         (0) root         (0)     1392 2023-05-16 15:39:21.000000 apache-airflow-providers-hashicorp-3.4.0rc1/airflow/providers/hashicorp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:19.000000 apache-airflow-providers-hashicorp-3.4.0rc1/airflow/providers/hashicorp/_internal_client/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-hashicorp-3.4.0rc1/airflow/providers/hashicorp/_internal_client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20535 2023-02-24 18:43:53.000000 apache-airflow-providers-hashicorp-3.4.0rc1/airflow/providers/hashicorp/_internal_client/vault_client.py
+-rw-r--r--   0 root         (0) root         (0)     2523 2023-05-16 15:54:18.000000 apache-airflow-providers-hashicorp-3.4.0rc1/airflow/providers/hashicorp/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:19.000000 apache-airflow-providers-hashicorp-3.4.0rc1/airflow/providers/hashicorp/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-hashicorp-3.4.0rc1/airflow/providers/hashicorp/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18748 2023-05-03 19:47:07.000000 apache-airflow-providers-hashicorp-3.4.0rc1/airflow/providers/hashicorp/hooks/vault.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:19.000000 apache-airflow-providers-hashicorp-3.4.0rc1/airflow/providers/hashicorp/secrets/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-hashicorp-3.4.0rc1/airflow/providers/hashicorp/secrets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11986 2023-05-03 19:47:07.000000 apache-airflow-providers-hashicorp-3.4.0rc1/airflow/providers/hashicorp/secrets/vault.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:19.000000 apache-airflow-providers-hashicorp-3.4.0rc1/apache_airflow_providers_hashicorp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    12528 2023-05-16 15:54:19.000000 apache-airflow-providers-hashicorp-3.4.0rc1/apache_airflow_providers_hashicorp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      867 2023-05-16 15:54:19.000000 apache-airflow-providers-hashicorp-3.4.0rc1/apache_airflow_providers_hashicorp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:54:19.000000 apache-airflow-providers-hashicorp-3.4.0rc1/apache_airflow_providers_hashicorp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      106 2023-05-16 15:54:19.000000 apache-airflow-providers-hashicorp-3.4.0rc1/apache_airflow_providers_hashicorp.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:54:19.000000 apache-airflow-providers-hashicorp-3.4.0rc1/apache_airflow_providers_hashicorp.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       80 2023-05-16 15:54:19.000000 apache-airflow-providers-hashicorp-3.4.0rc1/apache_airflow_providers_hashicorp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-16 15:54:19.000000 apache-airflow-providers-hashicorp-3.4.0rc1/apache_airflow_providers_hashicorp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5308 2023-05-15 09:39:26.000000 apache-airflow-providers-hashicorp-3.4.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1858 2023-05-16 15:54:19.000000 apache-airflow-providers-hashicorp-3.4.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1701 2023-05-16 15:54:18.000000 apache-airflow-providers-hashicorp-3.4.0rc1/setup.py
```

### Comparing `apache-airflow-providers-hashicorp-3.3.1rc1/LICENSE` & `apache-airflow-providers-hashicorp-3.4.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-hashicorp-3.3.1rc1/MANIFEST.in` & `apache-airflow-providers-hashicorp-3.4.0rc1/MANIFEST.in`

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

### Comparing `apache-airflow-providers-hashicorp-3.3.1rc1/PKG-INFO` & `apache-airflow-providers-hashicorp-3.4.0rc1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-hashicorp
-Version: 3.3.1rc1
+Version: 3.4.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-hashicorp package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-hashicorp/3.3.1/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-hashicorp/3.4.0/
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
 
 
 Package ``apache-airflow-providers-hashicorp``
 
-Release: ``3.3.1rc1``
+Release: ``3.4.0rc1``
 
 
 Hashicorp including `Hashicorp Vault <https://www.vaultproject.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``hashicorp`` provider. All classes for this provider package
 are in ``airflow.providers.hashicorp`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-hashicorp/3.3.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-hashicorp/3.4.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -80,15 +80,15 @@
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
-``apache-airflow``  ``>=2.3.0``
+``apache-airflow``  ``>=2.4.0``
 ``hvac``            ``>=0.10``
 ==================  ==================
 
 Cross provider package dependencies
 -----------------------------------
 
 Those are dependencies that might be needed in order to use all the features of the package.
@@ -129,14 +129,32 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.4.0
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
+   * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add mechanism to suspend providers (#30422)``
+
 3.3.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
 
 * ``Improve creating Vault connection from the UI and add documentation for this conn (#30057)``
@@ -158,16 +176,17 @@
 
 .. Review and move the new changes to one of the sections above:
    * ``Prepare docs for 03/2023 wave of Providers (#29878)``
 
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
 * ``Add Airflow specific warning classes (#25799)``
 
@@ -203,16 +222,17 @@
 
 3.0.0
 .....
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
-* This release of provider is only available for Airflow 2.2+ as explained in the Apache Airflow
-  providers support policy https://github.com/apache/airflow/blob/main/README.md#support-for-providers
+.. note::
+  This release of provider is only available for Airflow 2.2+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
    * ``Add explanatory note for contributors about updating Changelog (#24229)``
    * ``Prepare provider documentation 2022.05.11 (#23631)``
    * ``pydocstyle D202 added (#24221)``
    * ``Prepare docs for May 2022 provider's release (#24231)``
 
 .. Below changes are excluded from the changelog. Move them to
```

### Comparing `apache-airflow-providers-hashicorp-3.3.1rc1/README.rst` & `apache-airflow-providers-hashicorp-3.4.0rc1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -15,28 +15,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-hashicorp``
 
-Release: ``3.3.1rc1``
+Release: ``3.4.0rc1``
 
 
 Hashicorp including `Hashicorp Vault <https://www.vaultproject.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``hashicorp`` provider. All classes for this provider package
 are in ``airflow.providers.hashicorp`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-hashicorp/3.3.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-hashicorp/3.4.0/>`_.
 
 
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
 ``hvac``            ``>=0.10``
 ==================  ==================
 
 Cross provider package dependencies
 -----------------------------------
 
 Those are dependencies that might be needed in order to use all the features of the package.
@@ -95,14 +95,32 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.4.0
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
+   * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add mechanism to suspend providers (#30422)``
+
 3.3.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
 
 * ``Improve creating Vault connection from the UI and add documentation for this conn (#30057)``
@@ -124,16 +142,17 @@
 
 .. Review and move the new changes to one of the sections above:
    * ``Prepare docs for 03/2023 wave of Providers (#29878)``
 
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
 * ``Add Airflow specific warning classes (#25799)``
 
@@ -169,16 +188,17 @@
 
 3.0.0
 .....
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
-* This release of provider is only available for Airflow 2.2+ as explained in the Apache Airflow
-  providers support policy https://github.com/apache/airflow/blob/main/README.md#support-for-providers
+.. note::
+  This release of provider is only available for Airflow 2.2+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
    * ``Add explanatory note for contributors about updating Changelog (#24229)``
    * ``Prepare provider documentation 2022.05.11 (#23631)``
    * ``pydocstyle D202 added (#24221)``
    * ``Prepare docs for May 2022 provider's release (#24231)``
 
 .. Below changes are excluded from the changelog. Move them to
```

### Comparing `apache-airflow-providers-hashicorp-3.3.1rc1/airflow/providers/hashicorp/__init__.py` & `apache-airflow-providers-hashicorp-3.4.0rc1/airflow/providers/hashicorp/_internal_client/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-hashicorp-3.3.1rc1/airflow/providers/hashicorp/_internal_client/__init__.py` & `apache-airflow-providers-hashicorp-3.4.0rc1/airflow/providers/hashicorp/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-hashicorp-3.3.1rc1/airflow/providers/hashicorp/_internal_client/vault_client.py` & `apache-airflow-providers-hashicorp-3.4.0rc1/airflow/providers/hashicorp/_internal_client/vault_client.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-hashicorp-3.3.1rc1/airflow/providers/hashicorp/get_provider_info.py` & `apache-airflow-providers-hashicorp-3.4.0rc1/airflow/providers/hashicorp/get_provider_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,17 @@
 
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-hashicorp",
         "name": "Hashicorp",
         "description": "Hashicorp including `Hashicorp Vault <https://www.vaultproject.io/>`__\n",
+        "suspended": False,
         "versions": [
+            "3.4.0",
             "3.3.1",
             "3.3.0",
             "3.2.0",
             "3.1.0",
             "3.0.1",
             "3.0.0",
             "2.2.0",
@@ -41,15 +43,15 @@
             "2.1.1",
             "2.1.0",
             "2.0.0",
             "1.0.2",
             "1.0.1",
             "1.0.0",
         ],
-        "dependencies": ["apache-airflow>=2.3.0", "hvac>=0.10"],
+        "dependencies": ["apache-airflow>=2.4.0", "hvac>=0.10"],
         "integrations": [
             {
                 "integration-name": "Hashicorp Vault",
                 "external-doc-url": "https://www.vaultproject.io/",
                 "logo": "/integration-logos/hashicorp/Hashicorp-Vault.png",
                 "tags": ["software"],
             }
```

### Comparing `apache-airflow-providers-hashicorp-3.3.1rc1/airflow/providers/hashicorp/hooks/__init__.py` & `apache-airflow-providers-hashicorp-3.4.0rc1/airflow/providers/hashicorp/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-hashicorp-3.3.1rc1/airflow/providers/hashicorp/hooks/vault.py` & `apache-airflow-providers-hashicorp-3.4.0rc1/airflow/providers/hashicorp/hooks/vault.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 import warnings
 from typing import Any
 
 import hvac
 from hvac.exceptions import VaultError
 from requests import Response
 
+from airflow.exceptions import AirflowProviderDeprecationWarning
 from airflow.hooks.base import BaseHook
 from airflow.providers.hashicorp._internal_client.vault_client import (
     DEFAULT_KUBERNETES_JWT_PATH,
     DEFAULT_KV_ENGINE_VERSION,
     _VaultClient,
 )
 from airflow.utils.helpers import merge_dicts
@@ -144,23 +145,23 @@
             client_kwargs = merge_dicts(client_kwargs, kwargs)
 
         if auth_type == "approle":
             if role_id:
                 warnings.warn(
                     """The usage of role_id for AppRole authentication has been deprecated.
                     Please use connection login.""",
-                    DeprecationWarning,
+                    AirflowProviderDeprecationWarning,
                     stacklevel=2,
                 )
             elif self.connection.extra_dejson.get("role_id"):
                 role_id = self.connection.extra_dejson.get("role_id")
                 warnings.warn(
                     """The usage of role_id in connection extra for AppRole authentication has been
                     deprecated. Please use connection login.""",
-                    DeprecationWarning,
+                    AirflowProviderDeprecationWarning,
                     stacklevel=2,
                 )
             elif self.connection.login:
                 role_id = self.connection.login
 
         if auth_type == "aws_iam":
             if not role_id:
```

### Comparing `apache-airflow-providers-hashicorp-3.3.1rc1/airflow/providers/hashicorp/secrets/vault.py` & `apache-airflow-providers-hashicorp-3.4.0rc1/airflow/providers/hashicorp/secrets/vault.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 # under the License.
 """Objects relating to sourcing connections & variables from Hashicorp Vault"""
 from __future__ import annotations
 
 import warnings
 from typing import TYPE_CHECKING
 
+from airflow.exceptions import AirflowProviderDeprecationWarning
 from airflow.providers.hashicorp._internal_client.vault_client import _VaultClient
 from airflow.secrets import BaseSecretsBackend
 from airflow.utils.log.logging_mixin import LoggingMixin
 
 
 class VaultBackend(BaseSecretsBackend, LoggingMixin):
     """
@@ -191,15 +192,15 @@
         :return: The connection uri retrieved from the secret
         """
         # Since VaultBackend implements `get_connection`, `get_conn_uri` is not used. So we
         # don't need to implement (or direct users to use) method `get_conn_value` instead
         warnings.warn(
             f"Method `{self.__class__.__name__}.get_conn_uri` is deprecated and will be removed "
             "in a future release.",
-            DeprecationWarning,
+            AirflowProviderDeprecationWarning,
             stacklevel=2,
         )
         response = self.get_response(conn_id)
         return response.get("conn_uri") if response else None
 
     # Make sure connection is imported this way for type checking, otherwise when importing
     # the backend it will get a circular dependency and fail
```

### Comparing `apache-airflow-providers-hashicorp-3.3.1rc1/apache_airflow_providers_hashicorp.egg-info/PKG-INFO` & `apache-airflow-providers-hashicorp-3.4.0rc1/apache_airflow_providers_hashicorp.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-hashicorp
-Version: 3.3.1rc1
+Version: 3.4.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-hashicorp package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-hashicorp/3.3.1/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-hashicorp/3.4.0/
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
 
 
 Package ``apache-airflow-providers-hashicorp``
 
-Release: ``3.3.1rc1``
+Release: ``3.4.0rc1``
 
 
 Hashicorp including `Hashicorp Vault <https://www.vaultproject.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``hashicorp`` provider. All classes for this provider package
 are in ``airflow.providers.hashicorp`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-hashicorp/3.3.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-hashicorp/3.4.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -80,15 +80,15 @@
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
-``apache-airflow``  ``>=2.3.0``
+``apache-airflow``  ``>=2.4.0``
 ``hvac``            ``>=0.10``
 ==================  ==================
 
 Cross provider package dependencies
 -----------------------------------
 
 Those are dependencies that might be needed in order to use all the features of the package.
@@ -129,14 +129,32 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.4.0
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
+   * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add mechanism to suspend providers (#30422)``
+
 3.3.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
 
 * ``Improve creating Vault connection from the UI and add documentation for this conn (#30057)``
@@ -158,16 +176,17 @@
 
 .. Review and move the new changes to one of the sections above:
    * ``Prepare docs for 03/2023 wave of Providers (#29878)``
 
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
 * ``Add Airflow specific warning classes (#25799)``
 
@@ -203,16 +222,17 @@
 
 3.0.0
 .....
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
-* This release of provider is only available for Airflow 2.2+ as explained in the Apache Airflow
-  providers support policy https://github.com/apache/airflow/blob/main/README.md#support-for-providers
+.. note::
+  This release of provider is only available for Airflow 2.2+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
    * ``Add explanatory note for contributors about updating Changelog (#24229)``
    * ``Prepare provider documentation 2022.05.11 (#23631)``
    * ``pydocstyle D202 added (#24221)``
    * ``Prepare docs for May 2022 provider's release (#24231)``
 
 .. Below changes are excluded from the changelog. Move them to
```

### Comparing `apache-airflow-providers-hashicorp-3.3.1rc1/apache_airflow_providers_hashicorp.egg-info/SOURCES.txt` & `apache-airflow-providers-hashicorp-3.4.0rc1/apache_airflow_providers_hashicorp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-hashicorp-3.3.1rc1/pyproject.toml` & `apache-airflow-providers-hashicorp-3.4.0rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-hashicorp-3.3.1rc1/setup.cfg` & `apache-airflow-providers-hashicorp-3.4.0rc1/setup.cfg`

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-hashicorp/3.3.1/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-hashicorp/3.4.0/
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
-	apache-airflow>=2.3.0.dev0
+	apache-airflow>=2.4.0.dev0
 	hvac>=0.10
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.hashicorp.get_provider_info:get_provider_info
 
 [files]
```

### Comparing `apache-airflow-providers-hashicorp-3.3.1rc1/setup.py` & `apache-airflow-providers-hashicorp-3.4.0rc1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,23 +22,28 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-hashicorp package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "3.3.1"
+version = "3.4.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-hashicorp setup."""
     setup(
         version=version,
         extras_require={"google": ["apache-airflow-providers-google"]},
         packages=find_namespace_packages(
-            include=["airflow.providers.hashicorp", "airflow.providers.hashicorp.*"]
+            include=[
+                "airflow.providers.hashicorp",
+                "airflow.providers.hashicorp.*",
+                "airflow.providers.hashicorp_vendor",
+                "airflow.providers.hashicorp_vendor.*",
+            ],
         ),
     )
 
 
 if __name__ == "__main__":
     do_setup()
```

