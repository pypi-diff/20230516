# Comparing `tmp/apache-airflow-providers-microsoft-mssql-3.3.2rc2.tar.gz` & `tmp/apache-airflow-providers-microsoft-mssql-3.4.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-microsoft-mssql-3.3.2rc2.tar", last modified: Mon Jan  2 13:09:25 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-microsoft-mssql-3.4.0rc1.tar", last modified: Tue May 16 15:54:33 2023, max compression
```

## Comparing `apache-airflow-providers-microsoft-mssql-3.3.2rc2.tar` & `apache-airflow-providers-microsoft-mssql-3.4.0rc1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-02 13:09:25.000000 apache-airflow-providers-microsoft-mssql-3.3.2rc2/
--rw-r--r--   0 root         (0) root         (0)    10850 2022-10-05 12:15:16.000000 apache-airflow-providers-microsoft-mssql-3.3.2rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1122 2023-01-02 13:09:23.000000 apache-airflow-providers-microsoft-mssql-3.3.2rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2022-10-05 12:15:16.000000 apache-airflow-providers-microsoft-mssql-3.3.2rc2/NOTICE
--rw-r--r--   0 root         (0) root         (0)    11460 2023-01-02 13:09:25.000000 apache-airflow-providers-microsoft-mssql-3.3.2rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9859 2023-01-02 13:09:23.000000 apache-airflow-providers-microsoft-mssql-3.3.2rc2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-02 13:09:24.000000 apache-airflow-providers-microsoft-mssql-3.3.2rc2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-02 13:09:24.000000 apache-airflow-providers-microsoft-mssql-3.3.2rc2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-02 13:09:24.000000 apache-airflow-providers-microsoft-mssql-3.3.2rc2/airflow/providers/microsoft/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-02 13:09:24.000000 apache-airflow-providers-microsoft-mssql-3.3.2rc2/airflow/providers/microsoft/mssql/
--rw-r--r--   0 root         (0) root         (0)      787 2022-10-05 12:15:15.000000 apache-airflow-providers-microsoft-mssql-3.3.2rc2/airflow/providers/microsoft/mssql/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2927 2023-01-02 13:09:23.000000 apache-airflow-providers-microsoft-mssql-3.3.2rc2/airflow/providers/microsoft/mssql/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-02 13:09:24.000000 apache-airflow-providers-microsoft-mssql-3.3.2rc2/airflow/providers/microsoft/mssql/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2022-10-05 12:15:15.000000 apache-airflow-providers-microsoft-mssql-3.3.2rc2/airflow/providers/microsoft/mssql/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4021 2022-11-09 14:25:13.000000 apache-airflow-providers-microsoft-mssql-3.3.2rc2/airflow/providers/microsoft/mssql/hooks/mssql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-02 13:09:25.000000 apache-airflow-providers-microsoft-mssql-3.3.2rc2/airflow/providers/microsoft/mssql/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2022-10-05 12:15:15.000000 apache-airflow-providers-microsoft-mssql-3.3.2rc2/airflow/providers/microsoft/mssql/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2705 2022-11-03 13:17:26.000000 apache-airflow-providers-microsoft-mssql-3.3.2rc2/airflow/providers/microsoft/mssql/operators/mssql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-02 13:09:25.000000 apache-airflow-providers-microsoft-mssql-3.3.2rc2/apache_airflow_providers_microsoft_mssql.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11460 2023-01-02 13:09:24.000000 apache-airflow-providers-microsoft-mssql-3.3.2rc2/apache_airflow_providers_microsoft_mssql.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      831 2023-01-02 13:09:24.000000 apache-airflow-providers-microsoft-mssql-3.3.2rc2/apache_airflow_providers_microsoft_mssql.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-02 13:09:24.000000 apache-airflow-providers-microsoft-mssql-3.3.2rc2/apache_airflow_providers_microsoft_mssql.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      113 2023-01-02 13:09:24.000000 apache-airflow-providers-microsoft-mssql-3.3.2rc2/apache_airflow_providers_microsoft_mssql.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-02 13:09:24.000000 apache-airflow-providers-microsoft-mssql-3.3.2rc2/apache_airflow_providers_microsoft_mssql.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      140 2023-01-02 13:09:24.000000 apache-airflow-providers-microsoft-mssql-3.3.2rc2/apache_airflow_providers_microsoft_mssql.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-01-02 13:09:24.000000 apache-airflow-providers-microsoft-mssql-3.3.2rc2/apache_airflow_providers_microsoft_mssql.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1860 2022-12-20 13:50:44.000000 apache-airflow-providers-microsoft-mssql-3.3.2rc2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1947 2023-01-02 13:09:25.000000 apache-airflow-providers-microsoft-mssql-3.3.2rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1575 2023-01-02 13:09:23.000000 apache-airflow-providers-microsoft-mssql-3.3.2rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:33.000000 apache-airflow-providers-microsoft-mssql-3.4.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-microsoft-mssql-3.4.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-05-16 15:54:32.000000 apache-airflow-providers-microsoft-mssql-3.4.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-microsoft-mssql-3.4.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    12254 2023-05-16 15:54:33.000000 apache-airflow-providers-microsoft-mssql-3.4.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10673 2023-05-16 15:54:32.000000 apache-airflow-providers-microsoft-mssql-3.4.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:33.000000 apache-airflow-providers-microsoft-mssql-3.4.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:33.000000 apache-airflow-providers-microsoft-mssql-3.4.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:33.000000 apache-airflow-providers-microsoft-mssql-3.4.0rc1/airflow/providers/microsoft/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:33.000000 apache-airflow-providers-microsoft-mssql-3.4.0rc1/airflow/providers/microsoft/mssql/
+-rw-r--r--   0 root         (0) root         (0)     1398 2023-05-16 15:39:21.000000 apache-airflow-providers-microsoft-mssql-3.4.0rc1/airflow/providers/microsoft/mssql/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2976 2023-05-16 15:54:32.000000 apache-airflow-providers-microsoft-mssql-3.4.0rc1/airflow/providers/microsoft/mssql/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:33.000000 apache-airflow-providers-microsoft-mssql-3.4.0rc1/airflow/providers/microsoft/mssql/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-mssql-3.4.0rc1/airflow/providers/microsoft/mssql/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4021 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-mssql-3.4.0rc1/airflow/providers/microsoft/mssql/hooks/mssql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:33.000000 apache-airflow-providers-microsoft-mssql-3.4.0rc1/airflow/providers/microsoft/mssql/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-mssql-3.4.0rc1/airflow/providers/microsoft/mssql/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2785 2023-05-03 19:47:07.000000 apache-airflow-providers-microsoft-mssql-3.4.0rc1/airflow/providers/microsoft/mssql/operators/mssql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:33.000000 apache-airflow-providers-microsoft-mssql-3.4.0rc1/apache_airflow_providers_microsoft_mssql.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    12254 2023-05-16 15:54:33.000000 apache-airflow-providers-microsoft-mssql-3.4.0rc1/apache_airflow_providers_microsoft_mssql.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      831 2023-05-16 15:54:33.000000 apache-airflow-providers-microsoft-mssql-3.4.0rc1/apache_airflow_providers_microsoft_mssql.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:54:33.000000 apache-airflow-providers-microsoft-mssql-3.4.0rc1/apache_airflow_providers_microsoft_mssql.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      112 2023-05-16 15:54:33.000000 apache-airflow-providers-microsoft-mssql-3.4.0rc1/apache_airflow_providers_microsoft_mssql.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:54:33.000000 apache-airflow-providers-microsoft-mssql-3.4.0rc1/apache_airflow_providers_microsoft_mssql.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      140 2023-05-16 15:54:33.000000 apache-airflow-providers-microsoft-mssql-3.4.0rc1/apache_airflow_providers_microsoft_mssql.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-16 15:54:33.000000 apache-airflow-providers-microsoft-mssql-3.4.0rc1/apache_airflow_providers_microsoft_mssql.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5308 2023-05-15 09:39:26.000000 apache-airflow-providers-microsoft-mssql-3.4.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1947 2023-05-16 15:54:33.000000 apache-airflow-providers-microsoft-mssql-3.4.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1745 2023-05-16 15:54:32.000000 apache-airflow-providers-microsoft-mssql-3.4.0rc1/setup.py
```

### Comparing `apache-airflow-providers-microsoft-mssql-3.3.2rc2/LICENSE` & `apache-airflow-providers-microsoft-mssql-3.4.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-mssql-3.3.2rc2/MANIFEST.in` & `apache-airflow-providers-microsoft-mssql-3.4.0rc1/MANIFEST.in`

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

### Comparing `apache-airflow-providers-microsoft-mssql-3.3.2rc2/PKG-INFO` & `apache-airflow-providers-microsoft-mssql-3.4.0rc1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-microsoft-mssql
-Version: 3.3.2rc2
+Version: 3.4.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-microsoft-mssql package
 Home-page: https://airflow.apache.org/
+Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Download-URL: https://archive.apache.org/dist/airflow/providers
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-microsoft-mssql/3.3.2/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-microsoft-mssql/3.4.0/
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
@@ -50,28 +49,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-microsoft-mssql``
 
-Release: ``3.3.2rc2``
+Release: ``3.4.0rc1``
 
 
 `Microsoft SQL Server (MSSQL) <https://www.microsoft.com/en-us/sql-server/sql-server-downloads>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``microsoft.mssql`` provider. All classes for this provider package
 are in ``airflow.providers.microsoft.mssql`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-mssql/3.3.2/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-mssql/3.4.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -81,15 +80,15 @@
 
 Requirements
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
-``apache-airflow``                       ``>=2.3.0``
+``apache-airflow``                       ``>=2.4.0``
 ``apache-airflow-providers-common-sql``  ``>=1.3.1``
 ``pymssql``                              ``>=2.1.5``
 =======================================  ==================
 
 Cross provider package dependencies
 -----------------------------------
 
@@ -131,14 +130,32 @@
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
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add mechanism to suspend providers (#30422)``
+   * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
+
 3.3.2
 .....
 
 Misc
 ~~~~
 * ``Re-enable 'pymsql' on ARM as it now builds cleanly (#28530)``
 
@@ -156,16 +173,17 @@
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Prepare for follow-up release for November providers (#27774)``
 
 3.3.0
 .....
 
-This release of provider is only available for Airflow 2.3+ as explained in the
-`Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/README.md#support-for-providers>`_.
+.. note::
+  This release of provider is only available for Airflow 2.3+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Misc
 ~~~~
 
 * ``Move min airflow version to 2.3.0 for all providers (#27196)``
 * ``Remove unnecessary newlines around single arg in signature (#27525)``
 
@@ -219,16 +237,17 @@
 
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
    * ``Migrate Microsoft example DAGs to new design #22452 - mssql (#24139)``
    * ``Add explanatory note for contributors about updating Changelog (#24229)``
    * ``Prepare docs for May 2022 provider's release (#24231)``
    * ``Update package description to remove double min-airflow specification (#24292)``
@@ -334,9 +353,7 @@
 
 Updated documentation and readme files.
 
 1.0.0
 .....
 
 Initial version of the provider.
-
-
```

### Comparing `apache-airflow-providers-microsoft-mssql-3.3.2rc2/README.rst` & `apache-airflow-providers-microsoft-mssql-3.4.0rc1/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -15,28 +15,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-microsoft-mssql``
 
-Release: ``3.3.2rc2``
+Release: ``3.4.0rc1``
 
 
 `Microsoft SQL Server (MSSQL) <https://www.microsoft.com/en-us/sql-server/sql-server-downloads>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``microsoft.mssql`` provider. All classes for this provider package
 are in ``airflow.providers.microsoft.mssql`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-mssql/3.3.2/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-mssql/3.4.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -46,15 +46,15 @@
 
 Requirements
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
-``apache-airflow``                       ``>=2.3.0``
+``apache-airflow``                       ``>=2.4.0``
 ``apache-airflow-providers-common-sql``  ``>=1.3.1``
 ``pymssql``                              ``>=2.1.5``
 =======================================  ==================
 
 Cross provider package dependencies
 -----------------------------------
 
@@ -96,14 +96,32 @@
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
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add mechanism to suspend providers (#30422)``
+   * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
+
 3.3.2
 .....
 
 Misc
 ~~~~
 * ``Re-enable 'pymsql' on ARM as it now builds cleanly (#28530)``
 
@@ -121,16 +139,17 @@
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Prepare for follow-up release for November providers (#27774)``
 
 3.3.0
 .....
 
-This release of provider is only available for Airflow 2.3+ as explained in the
-`Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/README.md#support-for-providers>`_.
+.. note::
+  This release of provider is only available for Airflow 2.3+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Misc
 ~~~~
 
 * ``Move min airflow version to 2.3.0 for all providers (#27196)``
 * ``Remove unnecessary newlines around single arg in signature (#27525)``
 
@@ -184,16 +203,17 @@
 
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
    * ``Migrate Microsoft example DAGs to new design #22452 - mssql (#24139)``
    * ``Add explanatory note for contributors about updating Changelog (#24229)``
    * ``Prepare docs for May 2022 provider's release (#24231)``
    * ``Update package description to remove double min-airflow specification (#24292)``
```

### Comparing `apache-airflow-providers-microsoft-mssql-3.3.2rc2/airflow/providers/microsoft/mssql/__init__.py` & `apache-airflow-providers-microsoft-mssql-3.4.0rc1/airflow/providers/microsoft/mssql/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-mssql-3.3.2rc2/airflow/providers/microsoft/mssql/get_provider_info.py` & `apache-airflow-providers-microsoft-mssql-3.4.0rc1/airflow/providers/microsoft/mssql/get_provider_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,17 @@
 
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-microsoft-mssql",
         "name": "Microsoft SQL Server (MSSQL)",
         "description": "`Microsoft SQL Server (MSSQL) <https://www.microsoft.com/en-us/sql-server/sql-server-downloads>`__\n",
+        "suspended": False,
         "versions": [
+            "3.4.0",
             "3.3.2",
             "3.3.1",
             "3.3.0",
             "3.2.1",
             "3.2.0",
             "3.1.0",
             "3.0.0",
@@ -42,15 +44,15 @@
             "2.0.1",
             "2.0.0",
             "1.1.0",
             "1.0.1",
             "1.0.0",
         ],
         "dependencies": [
-            "apache-airflow>=2.3.0",
+            "apache-airflow>=2.4.0",
             "apache-airflow-providers-common-sql>=1.3.1",
             "pymssql>=2.1.5",
         ],
         "integrations": [
             {
                 "integration-name": "Microsoft SQL Server (MSSQL)",
                 "external-doc-url": "https://www.microsoft.com/en-us/sql-server/sql-server-downloads",
```

### Comparing `apache-airflow-providers-microsoft-mssql-3.3.2rc2/airflow/providers/microsoft/mssql/hooks/__init__.py` & `apache-airflow-providers-microsoft-mssql-3.4.0rc1/airflow/providers/microsoft/mssql/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-mssql-3.3.2rc2/airflow/providers/microsoft/mssql/hooks/mssql.py` & `apache-airflow-providers-microsoft-mssql-3.4.0rc1/airflow/providers/microsoft/mssql/hooks/mssql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-mssql-3.3.2rc2/airflow/providers/microsoft/mssql/operators/mssql.py` & `apache-airflow-providers-microsoft-mssql-3.4.0rc1/airflow/providers/microsoft/mssql/operators/mssql.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
 import warnings
 from typing import Sequence
 
+from airflow.exceptions import AirflowProviderDeprecationWarning
 from airflow.providers.common.sql.operators.sql import SQLExecuteQueryOperator
 
 
 class MsSqlOperator(SQLExecuteQueryOperator):
     """
     Executes sql code in a specific Microsoft SQL database
 
@@ -57,10 +58,10 @@
             kwargs["hook_params"] = {"schema": database, **hook_params}
 
         super().__init__(conn_id=mssql_conn_id, **kwargs)
         warnings.warn(
             """This class is deprecated.
             Please use `airflow.providers.common.sql.operators.sql.SQLExecuteQueryOperator`.
             Also, you can provide `hook_params={'schema': <database>}`.""",
-            DeprecationWarning,
+            AirflowProviderDeprecationWarning,
             stacklevel=2,
         )
```

### Comparing `apache-airflow-providers-microsoft-mssql-3.3.2rc2/apache_airflow_providers_microsoft_mssql.egg-info/PKG-INFO` & `apache-airflow-providers-microsoft-mssql-3.4.0rc1/apache_airflow_providers_microsoft_mssql.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-microsoft-mssql
-Version: 3.3.2rc2
+Version: 3.4.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-microsoft-mssql package
 Home-page: https://airflow.apache.org/
+Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Download-URL: https://archive.apache.org/dist/airflow/providers
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-microsoft-mssql/3.3.2/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-microsoft-mssql/3.4.0/
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
@@ -50,28 +49,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-microsoft-mssql``
 
-Release: ``3.3.2rc2``
+Release: ``3.4.0rc1``
 
 
 `Microsoft SQL Server (MSSQL) <https://www.microsoft.com/en-us/sql-server/sql-server-downloads>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``microsoft.mssql`` provider. All classes for this provider package
 are in ``airflow.providers.microsoft.mssql`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-mssql/3.3.2/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-mssql/3.4.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -81,15 +80,15 @@
 
 Requirements
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
-``apache-airflow``                       ``>=2.3.0``
+``apache-airflow``                       ``>=2.4.0``
 ``apache-airflow-providers-common-sql``  ``>=1.3.1``
 ``pymssql``                              ``>=2.1.5``
 =======================================  ==================
 
 Cross provider package dependencies
 -----------------------------------
 
@@ -131,14 +130,32 @@
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
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add mechanism to suspend providers (#30422)``
+   * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
+
 3.3.2
 .....
 
 Misc
 ~~~~
 * ``Re-enable 'pymsql' on ARM as it now builds cleanly (#28530)``
 
@@ -156,16 +173,17 @@
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Prepare for follow-up release for November providers (#27774)``
 
 3.3.0
 .....
 
-This release of provider is only available for Airflow 2.3+ as explained in the
-`Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/README.md#support-for-providers>`_.
+.. note::
+  This release of provider is only available for Airflow 2.3+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Misc
 ~~~~
 
 * ``Move min airflow version to 2.3.0 for all providers (#27196)``
 * ``Remove unnecessary newlines around single arg in signature (#27525)``
 
@@ -219,16 +237,17 @@
 
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
    * ``Migrate Microsoft example DAGs to new design #22452 - mssql (#24139)``
    * ``Add explanatory note for contributors about updating Changelog (#24229)``
    * ``Prepare docs for May 2022 provider's release (#24231)``
    * ``Update package description to remove double min-airflow specification (#24292)``
@@ -334,9 +353,7 @@
 
 Updated documentation and readme files.
 
 1.0.0
 .....
 
 Initial version of the provider.
-
-
```

### Comparing `apache-airflow-providers-microsoft-mssql-3.3.2rc2/apache_airflow_providers_microsoft_mssql.egg-info/SOURCES.txt` & `apache-airflow-providers-microsoft-mssql-3.4.0rc1/apache_airflow_providers_microsoft_mssql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-mssql-3.3.2rc2/setup.cfg` & `apache-airflow-providers-microsoft-mssql-3.4.0rc1/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-microsoft-mssql/3.3.2/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-microsoft-mssql/3.4.0/
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
@@ -43,21 +43,21 @@
 python_requires = ~=3.7
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
 	apache-airflow-providers-common-sql>=1.3.1.dev0
-	apache-airflow>=2.3.0.dev0
+	apache-airflow>=2.4.0.dev0
 	pymssql>=2.1.5
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.microsoft.mssql.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.microsoft.mssql
 
 [egg_info]
-tag_build = rc2
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-microsoft-mssql-3.3.2rc2/setup.py` & `apache-airflow-providers-microsoft-mssql-3.4.0rc1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,23 +22,28 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-microsoft-mssql package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "3.3.2"
+version = "3.4.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-microsoft-mssql setup."""
     setup(
         version=version,
         extras_require={"common.sql": ["apache-airflow-providers-common-sql"]},
         packages=find_namespace_packages(
-            include=["airflow.providers.microsoft.mssql", "airflow.providers.microsoft.mssql.*"]
+            include=[
+                "airflow.providers.microsoft.mssql",
+                "airflow.providers.microsoft.mssql.*",
+                "airflow.providers.microsoft.mssql_vendor",
+                "airflow.providers.microsoft.mssql_vendor.*",
+            ],
         ),
     )
 
 
 if __name__ == "__main__":
     do_setup()
```
