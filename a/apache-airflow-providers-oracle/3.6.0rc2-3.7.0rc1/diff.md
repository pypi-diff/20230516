# Comparing `tmp/apache-airflow-providers-oracle-3.6.0rc2.tar.gz` & `tmp/apache-airflow-providers-oracle-3.7.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-oracle-3.6.0rc2.tar", last modified: Mon Jan  2 13:09:34 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-oracle-3.7.0rc1.tar", last modified: Tue May 16 15:54:49 2023, max compression
```

## Comparing `apache-airflow-providers-oracle-3.6.0rc2.tar` & `apache-airflow-providers-oracle-3.7.0rc1.tar`

### file list

```diff
@@ -1,31 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-02 13:09:34.000000 apache-airflow-providers-oracle-3.6.0rc2/
--rw-r--r--   0 root         (0) root         (0)    10850 2022-10-05 12:15:16.000000 apache-airflow-providers-oracle-3.6.0rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1122 2023-01-02 13:09:32.000000 apache-airflow-providers-oracle-3.6.0rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2022-10-05 12:15:16.000000 apache-airflow-providers-oracle-3.6.0rc2/NOTICE
--rw-r--r--   0 root         (0) root         (0)    12508 2023-01-02 13:09:34.000000 apache-airflow-providers-oracle-3.6.0rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10912 2023-01-02 13:09:32.000000 apache-airflow-providers-oracle-3.6.0rc2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-02 13:09:33.000000 apache-airflow-providers-oracle-3.6.0rc2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-02 13:09:33.000000 apache-airflow-providers-oracle-3.6.0rc2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-02 13:09:34.000000 apache-airflow-providers-oracle-3.6.0rc2/airflow/providers/oracle/
--rw-r--r--   0 root         (0) root         (0)      787 2022-10-05 12:15:15.000000 apache-airflow-providers-oracle-3.6.0rc2/airflow/providers/oracle/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2901 2023-01-02 13:09:32.000000 apache-airflow-providers-oracle-3.6.0rc2/airflow/providers/oracle/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-02 13:09:34.000000 apache-airflow-providers-oracle-3.6.0rc2/airflow/providers/oracle/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2022-10-05 12:15:15.000000 apache-airflow-providers-oracle-3.6.0rc2/airflow/providers/oracle/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17453 2022-11-03 13:17:26.000000 apache-airflow-providers-oracle-3.6.0rc2/airflow/providers/oracle/hooks/oracle.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-02 13:09:34.000000 apache-airflow-providers-oracle-3.6.0rc2/airflow/providers/oracle/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2022-10-05 12:15:15.000000 apache-airflow-providers-oracle-3.6.0rc2/airflow/providers/oracle/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4031 2022-12-20 13:50:43.000000 apache-airflow-providers-oracle-3.6.0rc2/airflow/providers/oracle/operators/oracle.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-02 13:09:34.000000 apache-airflow-providers-oracle-3.6.0rc2/airflow/providers/oracle/transfers/
--rw-r--r--   0 root         (0) root         (0)      785 2022-10-05 12:15:15.000000 apache-airflow-providers-oracle-3.6.0rc2/airflow/providers/oracle/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3647 2022-11-03 13:17:26.000000 apache-airflow-providers-oracle-3.6.0rc2/airflow/providers/oracle/transfers/oracle_to_oracle.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-02 13:09:34.000000 apache-airflow-providers-oracle-3.6.0rc2/apache_airflow_providers_oracle.egg-info/
--rw-r--r--   0 root         (0) root         (0)    12508 2023-01-02 13:09:33.000000 apache-airflow-providers-oracle-3.6.0rc2/apache_airflow_providers_oracle.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      818 2023-01-02 13:09:33.000000 apache-airflow-providers-oracle-3.6.0rc2/apache_airflow_providers_oracle.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-02 13:09:33.000000 apache-airflow-providers-oracle-3.6.0rc2/apache_airflow_providers_oracle.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-01-02 13:09:33.000000 apache-airflow-providers-oracle-3.6.0rc2/apache_airflow_providers_oracle.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-02 13:09:33.000000 apache-airflow-providers-oracle-3.6.0rc2/apache_airflow_providers_oracle.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      156 2023-01-02 13:09:33.000000 apache-airflow-providers-oracle-3.6.0rc2/apache_airflow_providers_oracle.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-01-02 13:09:33.000000 apache-airflow-providers-oracle-3.6.0rc2/apache_airflow_providers_oracle.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1860 2022-12-20 13:50:44.000000 apache-airflow-providers-oracle-3.6.0rc2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1894 2023-01-02 13:09:34.000000 apache-airflow-providers-oracle-3.6.0rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1537 2023-01-02 13:09:32.000000 apache-airflow-providers-oracle-3.6.0rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:49.000000 apache-airflow-providers-oracle-3.7.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-oracle-3.7.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-05-16 15:54:48.000000 apache-airflow-providers-oracle-3.7.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-oracle-3.7.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    13402 2023-05-16 15:54:49.000000 apache-airflow-providers-oracle-3.7.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11826 2023-05-16 15:54:48.000000 apache-airflow-providers-oracle-3.7.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:49.000000 apache-airflow-providers-oracle-3.7.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:49.000000 apache-airflow-providers-oracle-3.7.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:49.000000 apache-airflow-providers-oracle-3.7.0rc1/airflow/providers/oracle/
+-rw-r--r--   0 root         (0) root         (0)     1389 2023-05-16 15:39:21.000000 apache-airflow-providers-oracle-3.7.0rc1/airflow/providers/oracle/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:49.000000 apache-airflow-providers-oracle-3.7.0rc1/airflow/providers/oracle/example_dags/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-05-12 08:38:07.000000 apache-airflow-providers-oracle-3.7.0rc1/airflow/providers/oracle/example_dags/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2193 2023-05-12 08:38:07.000000 apache-airflow-providers-oracle-3.7.0rc1/airflow/providers/oracle/example_dags/example_oracle.py
+-rw-r--r--   0 root         (0) root         (0)     2950 2023-05-16 15:54:48.000000 apache-airflow-providers-oracle-3.7.0rc1/airflow/providers/oracle/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:49.000000 apache-airflow-providers-oracle-3.7.0rc1/airflow/providers/oracle/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-oracle-3.7.0rc1/airflow/providers/oracle/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17534 2023-05-03 19:47:07.000000 apache-airflow-providers-oracle-3.7.0rc1/airflow/providers/oracle/hooks/oracle.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:49.000000 apache-airflow-providers-oracle-3.7.0rc1/airflow/providers/oracle/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-oracle-3.7.0rc1/airflow/providers/oracle/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4111 2023-05-03 19:47:07.000000 apache-airflow-providers-oracle-3.7.0rc1/airflow/providers/oracle/operators/oracle.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:49.000000 apache-airflow-providers-oracle-3.7.0rc1/airflow/providers/oracle/transfers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-oracle-3.7.0rc1/airflow/providers/oracle/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3647 2023-02-24 18:43:53.000000 apache-airflow-providers-oracle-3.7.0rc1/airflow/providers/oracle/transfers/oracle_to_oracle.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:49.000000 apache-airflow-providers-oracle-3.7.0rc1/apache_airflow_providers_oracle.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    13402 2023-05-16 15:54:49.000000 apache-airflow-providers-oracle-3.7.0rc1/apache_airflow_providers_oracle.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      924 2023-05-16 15:54:49.000000 apache-airflow-providers-oracle-3.7.0rc1/apache_airflow_providers_oracle.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:54:49.000000 apache-airflow-providers-oracle-3.7.0rc1/apache_airflow_providers_oracle.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-05-16 15:54:49.000000 apache-airflow-providers-oracle-3.7.0rc1/apache_airflow_providers_oracle.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:54:49.000000 apache-airflow-providers-oracle-3.7.0rc1/apache_airflow_providers_oracle.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      156 2023-05-16 15:54:49.000000 apache-airflow-providers-oracle-3.7.0rc1/apache_airflow_providers_oracle.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-16 15:54:49.000000 apache-airflow-providers-oracle-3.7.0rc1/apache_airflow_providers_oracle.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5308 2023-05-15 09:39:26.000000 apache-airflow-providers-oracle-3.7.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1894 2023-05-16 15:54:49.000000 apache-airflow-providers-oracle-3.7.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1711 2023-05-16 15:54:48.000000 apache-airflow-providers-oracle-3.7.0rc1/setup.py
```

### Comparing `apache-airflow-providers-oracle-3.6.0rc2/LICENSE` & `apache-airflow-providers-oracle-3.7.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-oracle-3.6.0rc2/MANIFEST.in` & `apache-airflow-providers-oracle-3.7.0rc1/MANIFEST.in`

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

### Comparing `apache-airflow-providers-oracle-3.6.0rc2/PKG-INFO` & `apache-airflow-providers-oracle-3.7.0rc1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-oracle
-Version: 3.6.0rc2
+Version: 3.7.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-oracle package
 Home-page: https://airflow.apache.org/
+Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Download-URL: https://archive.apache.org/dist/airflow/providers
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-oracle/3.6.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-oracle/3.7.0/
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
@@ -51,28 +50,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-oracle``
 
-Release: ``3.6.0rc2``
+Release: ``3.7.0rc1``
 
 
 `Oracle <https://www.oracle.com/en/database/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``oracle`` provider. All classes for this provider package
 are in ``airflow.providers.oracle`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-oracle/3.6.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-oracle/3.7.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -82,15 +81,15 @@
 
 Requirements
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
-``apache-airflow``                       ``>=2.3.0``
+``apache-airflow``                       ``>=2.4.0``
 ``apache-airflow-providers-common-sql``  ``>=1.3.1``
 ``oracledb``                             ``>=1.0.0``
 =======================================  ==================
 
 Cross provider package dependencies
 -----------------------------------
 
@@ -132,14 +131,34 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.7.0
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
+* ``Add docs for Oracle operators (#30979)``
+* ``Fix deprecated import in Oracle example (#31166)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add mechanism to suspend providers (#30422)``
+
 3.6.0
 .....
 
 Features
 ~~~~~~~~
 * ``XCOM push ORA error code in OracleStoredProcedure (#27319)``
 
@@ -157,16 +176,17 @@
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Prepare for follow-up release for November providers (#27774)``
 
 3.5.0
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
@@ -230,16 +250,17 @@
 
 3.0.0
 .....
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
-* This release of provider is only available for Airflow 2.2+ as explained in the Apache Airflow
-  providers support policy https://github.com/apache/airflow/blob/main/README.md#support-for-providers
+.. note::
+  This release of provider is only available for Airflow 2.2+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Features
 ~~~~~~~~
 
 * ``Add 'parameters' to templated fields in 'OracleOperator' (#22857)``
 
 Misc
@@ -381,9 +402,7 @@
 
 Updated documentation and readme files.
 
 1.0.0
 .....
 
 Initial version of the provider.
-
-
```

### Comparing `apache-airflow-providers-oracle-3.6.0rc2/README.rst` & `apache-airflow-providers-oracle-3.7.0rc1/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -15,28 +15,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-oracle``
 
-Release: ``3.6.0rc2``
+Release: ``3.7.0rc1``
 
 
 `Oracle <https://www.oracle.com/en/database/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``oracle`` provider. All classes for this provider package
 are in ``airflow.providers.oracle`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-oracle/3.6.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-oracle/3.7.0/>`_.
 
 
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
 ``oracledb``                             ``>=1.0.0``
 =======================================  ==================
 
 Cross provider package dependencies
 -----------------------------------
 
@@ -96,14 +96,34 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.7.0
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
+* ``Add docs for Oracle operators (#30979)``
+* ``Fix deprecated import in Oracle example (#31166)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add mechanism to suspend providers (#30422)``
+
 3.6.0
 .....
 
 Features
 ~~~~~~~~
 * ``XCOM push ORA error code in OracleStoredProcedure (#27319)``
 
@@ -121,16 +141,17 @@
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Prepare for follow-up release for November providers (#27774)``
 
 3.5.0
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
@@ -194,16 +215,17 @@
 
 3.0.0
 .....
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
-* This release of provider is only available for Airflow 2.2+ as explained in the Apache Airflow
-  providers support policy https://github.com/apache/airflow/blob/main/README.md#support-for-providers
+.. note::
+  This release of provider is only available for Airflow 2.2+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Features
 ~~~~~~~~
 
 * ``Add 'parameters' to templated fields in 'OracleOperator' (#22857)``
 
 Misc
```

### Comparing `apache-airflow-providers-oracle-3.6.0rc2/airflow/providers/oracle/__init__.py` & `apache-airflow-providers-oracle-3.7.0rc1/airflow/providers/oracle/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-oracle-3.6.0rc2/airflow/providers/oracle/get_provider_info.py` & `apache-airflow-providers-oracle-3.7.0rc1/airflow/providers/oracle/get_provider_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,17 @@
 
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-oracle",
         "name": "Oracle",
         "description": "`Oracle <https://www.oracle.com/en/database/>`__\n",
+        "suspended": False,
         "versions": [
+            "3.7.0",
             "3.6.0",
             "3.5.1",
             "3.5.0",
             "3.4.0",
             "3.3.0",
             "3.2.0",
             "3.1.0",
@@ -44,15 +46,15 @@
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
             "oracledb>=1.0.0",
         ],
         "integrations": [
             {
                 "integration-name": "Oracle",
                 "external-doc-url": "https://www.oracle.com/en/database/",
```

### Comparing `apache-airflow-providers-oracle-3.6.0rc2/airflow/providers/oracle/hooks/__init__.py` & `apache-airflow-providers-oracle-3.7.0rc1/airflow/providers/oracle/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-oracle-3.6.0rc2/airflow/providers/oracle/hooks/oracle.py` & `apache-airflow-providers-oracle-3.7.0rc1/airflow/providers/oracle/hooks/oracle.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 
 import math
 import warnings
 from datetime import datetime
 
 import oracledb
 
+from airflow.exceptions import AirflowProviderDeprecationWarning
+
 try:
     import numpy
 except ImportError:
     numpy = None  # type: ignore
 
 from airflow.providers.common.sql.hooks.sql import DbApiHook
 
@@ -201,15 +203,15 @@
                     dsn += ":" + str(conn.port)
                 if service_name:
                     dsn += "/" + service_name
                 elif conn.schema:
                     warnings.warn(
                         """Using conn.schema to pass the Oracle Service Name is deprecated.
                         Please use conn.extra.service_name instead.""",
-                        DeprecationWarning,
+                        AirflowProviderDeprecationWarning,
                         stacklevel=2,
                     )
                     dsn += "/" + conn.schema
             conn_config["dsn"] = dsn
 
         if "events" in conn.extra_dejson:
             conn_config["events"] = conn.extra_dejson.get("events")
```

### Comparing `apache-airflow-providers-oracle-3.6.0rc2/airflow/providers/oracle/operators/__init__.py` & `apache-airflow-providers-oracle-3.7.0rc1/airflow/providers/oracle/example_dags/__init__.py`

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

### Comparing `apache-airflow-providers-oracle-3.6.0rc2/airflow/providers/oracle/operators/oracle.py` & `apache-airflow-providers-oracle-3.7.0rc1/airflow/providers/oracle/operators/oracle.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 import re
 import warnings
 from typing import TYPE_CHECKING, Sequence
 
 import oracledb
 
+from airflow.exceptions import AirflowProviderDeprecationWarning
 from airflow.models import BaseOperator
 from airflow.providers.common.sql.operators.sql import SQLExecuteQueryOperator
 from airflow.providers.oracle.hooks.oracle import OracleHook
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
@@ -55,15 +56,15 @@
     ui_color = "#ededed"
 
     def __init__(self, *, oracle_conn_id: str = "oracle_default", **kwargs) -> None:
         super().__init__(conn_id=oracle_conn_id, **kwargs)
         warnings.warn(
             """This class is deprecated.
             Please use `airflow.providers.common.sql.operators.sql.SQLExecuteQueryOperator`.""",
-            DeprecationWarning,
+            AirflowProviderDeprecationWarning,
             stacklevel=2,
         )
 
 
 class OracleStoredProcedureOperator(BaseOperator):
     """
     Executes stored procedure in a specific Oracle database.
```

### Comparing `apache-airflow-providers-oracle-3.6.0rc2/airflow/providers/oracle/transfers/__init__.py` & `apache-airflow-providers-oracle-3.7.0rc1/airflow/providers/oracle/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-oracle-3.6.0rc2/airflow/providers/oracle/transfers/oracle_to_oracle.py` & `apache-airflow-providers-oracle-3.7.0rc1/airflow/providers/oracle/transfers/oracle_to_oracle.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-oracle-3.6.0rc2/apache_airflow_providers_oracle.egg-info/PKG-INFO` & `apache-airflow-providers-oracle-3.7.0rc1/apache_airflow_providers_oracle.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-oracle
-Version: 3.6.0rc2
+Version: 3.7.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-oracle package
 Home-page: https://airflow.apache.org/
+Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Download-URL: https://archive.apache.org/dist/airflow/providers
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-oracle/3.6.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-oracle/3.7.0/
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
@@ -51,28 +50,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-oracle``
 
-Release: ``3.6.0rc2``
+Release: ``3.7.0rc1``
 
 
 `Oracle <https://www.oracle.com/en/database/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``oracle`` provider. All classes for this provider package
 are in ``airflow.providers.oracle`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-oracle/3.6.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-oracle/3.7.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -82,15 +81,15 @@
 
 Requirements
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
-``apache-airflow``                       ``>=2.3.0``
+``apache-airflow``                       ``>=2.4.0``
 ``apache-airflow-providers-common-sql``  ``>=1.3.1``
 ``oracledb``                             ``>=1.0.0``
 =======================================  ==================
 
 Cross provider package dependencies
 -----------------------------------
 
@@ -132,14 +131,34 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.7.0
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
+* ``Add docs for Oracle operators (#30979)``
+* ``Fix deprecated import in Oracle example (#31166)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add mechanism to suspend providers (#30422)``
+
 3.6.0
 .....
 
 Features
 ~~~~~~~~
 * ``XCOM push ORA error code in OracleStoredProcedure (#27319)``
 
@@ -157,16 +176,17 @@
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Prepare for follow-up release for November providers (#27774)``
 
 3.5.0
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
@@ -230,16 +250,17 @@
 
 3.0.0
 .....
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
-* This release of provider is only available for Airflow 2.2+ as explained in the Apache Airflow
-  providers support policy https://github.com/apache/airflow/blob/main/README.md#support-for-providers
+.. note::
+  This release of provider is only available for Airflow 2.2+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Features
 ~~~~~~~~
 
 * ``Add 'parameters' to templated fields in 'OracleOperator' (#22857)``
 
 Misc
@@ -381,9 +402,7 @@
 
 Updated documentation and readme files.
 
 1.0.0
 .....
 
 Initial version of the provider.
-
-
```

### Comparing `apache-airflow-providers-oracle-3.6.0rc2/setup.cfg` & `apache-airflow-providers-oracle-3.7.0rc1/setup.cfg`

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-oracle/3.6.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-oracle/3.7.0/
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
 	oracledb>=1.0.0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.oracle.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.oracle
 
 [egg_info]
-tag_build = rc2
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-oracle-3.6.0rc2/setup.py` & `apache-airflow-providers-oracle-3.7.0rc1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,21 +22,28 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-oracle package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "3.6.0"
+version = "3.7.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-oracle setup."""
     setup(
         version=version,
         extras_require={"common.sql": ["apache-airflow-providers-common-sql"], "numpy": ["numpy"]},
-        packages=find_namespace_packages(include=["airflow.providers.oracle", "airflow.providers.oracle.*"]),
+        packages=find_namespace_packages(
+            include=[
+                "airflow.providers.oracle",
+                "airflow.providers.oracle.*",
+                "airflow.providers.oracle_vendor",
+                "airflow.providers.oracle_vendor.*",
+            ],
+        ),
     )
 
 
 if __name__ == "__main__":
     do_setup()
```

