# Comparing `tmp/apache-airflow-providers-microsoft-psrp-2.2.0rc1.tar.gz` & `tmp/apache-airflow-providers-microsoft-psrp-2.3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-microsoft-psrp-2.2.0rc1.tar", last modified: Sat Jan 14 12:16:22 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-microsoft-psrp-2.3.0rc1.tar", last modified: Tue May 16 15:54:35 2023, max compression
```

## Comparing `apache-airflow-providers-microsoft-psrp-2.2.0rc1.tar` & `apache-airflow-providers-microsoft-psrp-2.3.0rc1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 12:16:22.000000 apache-airflow-providers-microsoft-psrp-2.2.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2022-10-05 12:15:16.000000 apache-airflow-providers-microsoft-psrp-2.2.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1122 2023-01-14 12:16:21.000000 apache-airflow-providers-microsoft-psrp-2.2.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2022-10-05 12:15:16.000000 apache-airflow-providers-microsoft-psrp-2.2.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     7823 2023-01-14 12:16:22.000000 apache-airflow-providers-microsoft-psrp-2.2.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6252 2023-01-14 12:16:21.000000 apache-airflow-providers-microsoft-psrp-2.2.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 12:16:22.000000 apache-airflow-providers-microsoft-psrp-2.2.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 12:16:22.000000 apache-airflow-providers-microsoft-psrp-2.2.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 12:16:22.000000 apache-airflow-providers-microsoft-psrp-2.2.0rc1/airflow/providers/microsoft/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 12:16:22.000000 apache-airflow-providers-microsoft-psrp-2.2.0rc1/airflow/providers/microsoft/psrp/
--rw-r--r--   0 root         (0) root         (0)      787 2022-10-05 12:15:15.000000 apache-airflow-providers-microsoft-psrp-2.2.0rc1/airflow/providers/microsoft/psrp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2408 2023-01-14 12:16:21.000000 apache-airflow-providers-microsoft-psrp-2.2.0rc1/airflow/providers/microsoft/psrp/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 12:16:22.000000 apache-airflow-providers-microsoft-psrp-2.2.0rc1/airflow/providers/microsoft/psrp/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2022-10-05 12:15:15.000000 apache-airflow-providers-microsoft-psrp-2.2.0rc1/airflow/providers/microsoft/psrp/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10810 2023-01-11 12:48:26.000000 apache-airflow-providers-microsoft-psrp-2.2.0rc1/airflow/providers/microsoft/psrp/hooks/psrp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 12:16:22.000000 apache-airflow-providers-microsoft-psrp-2.2.0rc1/airflow/providers/microsoft/psrp/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2022-10-05 12:15:15.000000 apache-airflow-providers-microsoft-psrp-2.2.0rc1/airflow/providers/microsoft/psrp/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7175 2023-01-11 12:48:26.000000 apache-airflow-providers-microsoft-psrp-2.2.0rc1/airflow/providers/microsoft/psrp/operators/psrp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 12:16:22.000000 apache-airflow-providers-microsoft-psrp-2.2.0rc1/apache_airflow_providers_microsoft_psrp.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7823 2023-01-14 12:16:22.000000 apache-airflow-providers-microsoft-psrp-2.2.0rc1/apache_airflow_providers_microsoft_psrp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      816 2023-01-14 12:16:22.000000 apache-airflow-providers-microsoft-psrp-2.2.0rc1/apache_airflow_providers_microsoft_psrp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-14 12:16:22.000000 apache-airflow-providers-microsoft-psrp-2.2.0rc1/apache_airflow_providers_microsoft_psrp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      112 2023-01-14 12:16:22.000000 apache-airflow-providers-microsoft-psrp-2.2.0rc1/apache_airflow_providers_microsoft_psrp.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-14 12:16:22.000000 apache-airflow-providers-microsoft-psrp-2.2.0rc1/apache_airflow_providers_microsoft_psrp.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       14 2023-01-14 12:16:22.000000 apache-airflow-providers-microsoft-psrp-2.2.0rc1/apache_airflow_providers_microsoft_psrp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-01-14 12:16:22.000000 apache-airflow-providers-microsoft-psrp-2.2.0rc1/apache_airflow_providers_microsoft_psrp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     3814 2023-01-13 19:37:41.000000 apache-airflow-providers-microsoft-psrp-2.2.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1863 2023-01-14 12:16:22.000000 apache-airflow-providers-microsoft-psrp-2.2.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1518 2023-01-14 12:16:21.000000 apache-airflow-providers-microsoft-psrp-2.2.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:35.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-05-16 15:54:34.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     8811 2023-05-16 15:54:35.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7260 2023-05-16 15:54:34.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:35.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:35.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:35.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc1/airflow/providers/microsoft/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:35.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc1/airflow/providers/microsoft/psrp/
+-rw-r--r--   0 root         (0) root         (0)     1397 2023-05-16 15:39:21.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc1/airflow/providers/microsoft/psrp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2482 2023-05-16 15:54:34.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc1/airflow/providers/microsoft/psrp/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:35.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc1/airflow/providers/microsoft/psrp/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc1/airflow/providers/microsoft/psrp/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-05-03 19:47:07.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc1/airflow/providers/microsoft/psrp/hooks/psrp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:35.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc1/airflow/providers/microsoft/psrp/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc1/airflow/providers/microsoft/psrp/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7175 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc1/airflow/providers/microsoft/psrp/operators/psrp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:35.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc1/apache_airflow_providers_microsoft_psrp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8811 2023-05-16 15:54:35.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc1/apache_airflow_providers_microsoft_psrp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      816 2023-05-16 15:54:35.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc1/apache_airflow_providers_microsoft_psrp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:54:35.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc1/apache_airflow_providers_microsoft_psrp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      111 2023-05-16 15:54:35.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc1/apache_airflow_providers_microsoft_psrp.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:54:35.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc1/apache_airflow_providers_microsoft_psrp.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       41 2023-05-16 15:54:35.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc1/apache_airflow_providers_microsoft_psrp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-16 15:54:35.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc1/apache_airflow_providers_microsoft_psrp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5308 2023-05-15 09:39:26.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1891 2023-05-16 15:54:35.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1686 2023-05-16 15:54:34.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc1/setup.py
```

### Comparing `apache-airflow-providers-microsoft-psrp-2.2.0rc1/LICENSE` & `apache-airflow-providers-microsoft-psrp-2.3.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-psrp-2.2.0rc1/MANIFEST.in` & `apache-airflow-providers-microsoft-psrp-2.3.0rc1/MANIFEST.in`

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

### Comparing `apache-airflow-providers-microsoft-psrp-2.2.0rc1/PKG-INFO` & `apache-airflow-providers-microsoft-psrp-2.3.0rc1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-microsoft-psrp
-Version: 2.2.0rc1
+Version: 2.3.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-microsoft-psrp package
 Home-page: https://airflow.apache.org/
+Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Download-URL: https://archive.apache.org/dist/airflow/providers
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-microsoft-psrp/2.2.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-microsoft-psrp/2.3.0/
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
@@ -49,49 +48,50 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-microsoft-psrp``
 
-Release: ``2.2.0rc1``
+Release: ``2.3.0rc1``
 
 
 This package provides remote execution capabilities via the
 `PowerShell Remoting Protocol (PSRP)
 <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/>`__.
 
 
 Provider package
 ----------------
 
 This is a provider package for ``microsoft.psrp`` provider. All classes for this provider package
 are in ``airflow.providers.microsoft.psrp`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-psrp/2.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-psrp/2.3.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-microsoft-psrp``
 
 The package supports the following python versions: 3.7,3.8,3.9,3.10
 
 Requirements
 ------------
 
-=============  ==================
-PIP package    Version required
-=============  ==================
-``pypsrp``     ``>=0.8.0``
-=============  ==================
+==================  ==================
+PIP package         Version required
+==================  ==================
+``apache-airflow``  ``>=2.4.0``
+``pypsrp``          ``>=0.8.0``
+==================  ==================
 
  .. Licensed to the Apache Software Foundation (ASF) under one
     or more contributor license agreements.  See the NOTICE file
     distributed with this work for additional information
     regarding copyright ownership.  The ASF licenses this file
     to you under the Apache License, Version 2.0 (the
     "License"); you may not use this file except in compliance
@@ -111,27 +111,50 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+2.3.0
+.....
+
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
+   * ``Upgrade Mypy to 1.0 (#29468)``
+   * ``Revert "Upgrade mypy to 0.991 (#28926)" (#29470)``
+   * ``Upgrade mypy to 0.991 (#28926)``
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add mechanism to suspend providers (#30422)``
+
 2.2.0
 .....
 
 Features
 ~~~~~~~~
 
 * ``Add option to add arguments to PSRP hook and operator (#27689)``
 
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
 
 .. Below changes are excluded from the changelog. Move them to
@@ -145,16 +168,17 @@
 
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
    * ``Ensure @contextmanager decorates generator func (#23103)``
    * ``Introduce 'flake8-implicit-str-concat' plugin to static checks (#23873)``
    * ``Prepare docs for May 2022 provider's release (#24231)``
@@ -224,9 +248,7 @@
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
 
 1.0.0
 .....
 
 Initial version of the provider.
-
-
```

### Comparing `apache-airflow-providers-microsoft-psrp-2.2.0rc1/README.rst` & `apache-airflow-providers-microsoft-psrp-2.3.0rc1/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -15,49 +15,50 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-microsoft-psrp``
 
-Release: ``2.2.0rc1``
+Release: ``2.3.0rc1``
 
 
 This package provides remote execution capabilities via the
 `PowerShell Remoting Protocol (PSRP)
 <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/>`__.
 
 
 Provider package
 ----------------
 
 This is a provider package for ``microsoft.psrp`` provider. All classes for this provider package
 are in ``airflow.providers.microsoft.psrp`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-psrp/2.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-psrp/2.3.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-microsoft-psrp``
 
 The package supports the following python versions: 3.7,3.8,3.9,3.10
 
 Requirements
 ------------
 
-=============  ==================
-PIP package    Version required
-=============  ==================
-``pypsrp``     ``>=0.8.0``
-=============  ==================
+==================  ==================
+PIP package         Version required
+==================  ==================
+``apache-airflow``  ``>=2.4.0``
+``pypsrp``          ``>=0.8.0``
+==================  ==================
 
  .. Licensed to the Apache Software Foundation (ASF) under one
     or more contributor license agreements.  See the NOTICE file
     distributed with this work for additional information
     regarding copyright ownership.  The ASF licenses this file
     to you under the Apache License, Version 2.0 (the
     "License"); you may not use this file except in compliance
@@ -77,27 +78,50 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+2.3.0
+.....
+
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
+   * ``Upgrade Mypy to 1.0 (#29468)``
+   * ``Revert "Upgrade mypy to 0.991 (#28926)" (#29470)``
+   * ``Upgrade mypy to 0.991 (#28926)``
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add mechanism to suspend providers (#30422)``
+
 2.2.0
 .....
 
 Features
 ~~~~~~~~
 
 * ``Add option to add arguments to PSRP hook and operator (#27689)``
 
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
 
 .. Below changes are excluded from the changelog. Move them to
@@ -111,16 +135,17 @@
 
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
    * ``Ensure @contextmanager decorates generator func (#23103)``
    * ``Introduce 'flake8-implicit-str-concat' plugin to static checks (#23873)``
    * ``Prepare docs for May 2022 provider's release (#24231)``
```

### Comparing `apache-airflow-providers-microsoft-psrp-2.2.0rc1/airflow/providers/microsoft/psrp/__init__.py` & `apache-airflow-providers-microsoft-psrp-2.3.0rc1/airflow/providers/microsoft/psrp/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-psrp-2.2.0rc1/airflow/providers/microsoft/psrp/get_provider_info.py` & `apache-airflow-providers-microsoft-psrp-2.3.0rc1/airflow/providers/microsoft/psrp/get_provider_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,27 +23,29 @@
 
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-microsoft-psrp",
         "name": "PowerShell Remoting Protocol (PSRP)",
         "description": "This package provides remote execution capabilities via the\n`PowerShell Remoting Protocol (PSRP)\n<https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/>`__.\n",
+        "suspended": False,
         "versions": [
+            "2.3.0",
             "2.2.0",
             "2.1.0",
             "2.0.0",
             "1.1.4",
             "1.1.3",
             "1.1.2",
             "1.1.1",
             "1.1.0",
             "1.0.1",
             "1.0.0",
         ],
-        "dependencies": ["pypsrp>=0.8.0"],
+        "dependencies": ["apache-airflow>=2.4.0", "pypsrp>=0.8.0"],
         "integrations": [
             {
                 "integration-name": "Windows PowerShell Remoting Protocol",
                 "external-doc-url": "https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/",
                 "tags": ["protocol"],
             }
         ],
```

### Comparing `apache-airflow-providers-microsoft-psrp-2.2.0rc1/airflow/providers/microsoft/psrp/hooks/__init__.py` & `apache-airflow-providers-microsoft-psrp-2.3.0rc1/airflow/providers/microsoft/psrp/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-psrp-2.2.0rc1/airflow/providers/microsoft/psrp/hooks/psrp.py` & `apache-airflow-providers-microsoft-psrp-2.3.0rc1/airflow/providers/microsoft/psrp/hooks/psrp.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from weakref import WeakKeyDictionary
 
 from pypsrp.host import PSHost
 from pypsrp.messages import MessageType
 from pypsrp.powershell import PowerShell, PSInvocationState, RunspacePool
 from pypsrp.wsman import WSMan
 
-from airflow.exceptions import AirflowException
+from airflow.exceptions import AirflowException, AirflowProviderDeprecationWarning
 from airflow.hooks.base import BaseHook
 
 INFORMATIONAL_RECORD_LEVEL_MAP = {
     MessageType.DEBUG_RECORD: DEBUG,
     MessageType.ERROR_RECORD: ERROR,
     MessageType.VERBOSE_RECORD: INFO,
     MessageType.WARNING_RECORD: WARNING,
@@ -71,16 +71,15 @@
         Optional PowerShell host instance. If this is not set, the default
         implementation will be used.
 
     You can provide an alternative `configuration_name` using either `runspace_options`
     or by setting this key as the extra fields of your connection.
     """
 
-    _conn = None
-    _configuration_name = None
+    _conn: RunspacePool | None = None
     _wsman_ref: WeakKeyDictionary[RunspacePool, WSMan] = WeakKeyDictionary()
 
     def __init__(
         self,
         psrp_conn_id: str,
         logging_level: int = DEBUG,
         operation_timeout: int | None = None,
@@ -228,15 +227,15 @@
         if kwargs:
             if parameters:
                 raise ValueError("**kwargs not allowed when 'parameters' is used at the same time.")
             warn(
                 "Passing **kwargs to 'invoke_cmdlet' is deprecated "
                 "and will be removed in a future release. Please use 'parameters' "
                 "instead.",
-                DeprecationWarning,
+                AirflowProviderDeprecationWarning,
                 stacklevel=2,
             )
             parameters = kwargs
 
         with self.invoke() as ps:
             ps.add_cmdlet(name, use_local_scope=use_local_scope)
             for argument in arguments or ():
```

### Comparing `apache-airflow-providers-microsoft-psrp-2.2.0rc1/airflow/providers/microsoft/psrp/operators/psrp.py` & `apache-airflow-providers-microsoft-psrp-2.3.0rc1/airflow/providers/microsoft/psrp/operators/psrp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-psrp-2.2.0rc1/apache_airflow_providers_microsoft_psrp.egg-info/PKG-INFO` & `apache-airflow-providers-microsoft-psrp-2.3.0rc1/apache_airflow_providers_microsoft_psrp.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-microsoft-psrp
-Version: 2.2.0rc1
+Version: 2.3.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-microsoft-psrp package
 Home-page: https://airflow.apache.org/
+Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Download-URL: https://archive.apache.org/dist/airflow/providers
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-microsoft-psrp/2.2.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-microsoft-psrp/2.3.0/
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
@@ -49,49 +48,50 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-microsoft-psrp``
 
-Release: ``2.2.0rc1``
+Release: ``2.3.0rc1``
 
 
 This package provides remote execution capabilities via the
 `PowerShell Remoting Protocol (PSRP)
 <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/>`__.
 
 
 Provider package
 ----------------
 
 This is a provider package for ``microsoft.psrp`` provider. All classes for this provider package
 are in ``airflow.providers.microsoft.psrp`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-psrp/2.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-psrp/2.3.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-microsoft-psrp``
 
 The package supports the following python versions: 3.7,3.8,3.9,3.10
 
 Requirements
 ------------
 
-=============  ==================
-PIP package    Version required
-=============  ==================
-``pypsrp``     ``>=0.8.0``
-=============  ==================
+==================  ==================
+PIP package         Version required
+==================  ==================
+``apache-airflow``  ``>=2.4.0``
+``pypsrp``          ``>=0.8.0``
+==================  ==================
 
  .. Licensed to the Apache Software Foundation (ASF) under one
     or more contributor license agreements.  See the NOTICE file
     distributed with this work for additional information
     regarding copyright ownership.  The ASF licenses this file
     to you under the Apache License, Version 2.0 (the
     "License"); you may not use this file except in compliance
@@ -111,27 +111,50 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+2.3.0
+.....
+
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
+   * ``Upgrade Mypy to 1.0 (#29468)``
+   * ``Revert "Upgrade mypy to 0.991 (#28926)" (#29470)``
+   * ``Upgrade mypy to 0.991 (#28926)``
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add mechanism to suspend providers (#30422)``
+
 2.2.0
 .....
 
 Features
 ~~~~~~~~
 
 * ``Add option to add arguments to PSRP hook and operator (#27689)``
 
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
 
 .. Below changes are excluded from the changelog. Move them to
@@ -145,16 +168,17 @@
 
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
    * ``Ensure @contextmanager decorates generator func (#23103)``
    * ``Introduce 'flake8-implicit-str-concat' plugin to static checks (#23873)``
    * ``Prepare docs for May 2022 provider's release (#24231)``
@@ -224,9 +248,7 @@
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
 
 1.0.0
 .....
 
 Initial version of the provider.
-
-
```

### Comparing `apache-airflow-providers-microsoft-psrp-2.2.0rc1/apache_airflow_providers_microsoft_psrp.egg-info/SOURCES.txt` & `apache-airflow-providers-microsoft-psrp-2.3.0rc1/apache_airflow_providers_microsoft_psrp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-psrp-2.2.0rc1/pyproject.toml` & `apache-airflow-providers-microsoft-psrp-2.3.0rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-microsoft-psrp-2.2.0rc1/setup.cfg` & `apache-airflow-providers-microsoft-psrp-2.3.0rc1/setup.cfg`

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-microsoft-psrp/2.2.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-microsoft-psrp/2.3.0/
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
@@ -42,14 +42,15 @@
 include_package_data = True
 python_requires = ~=3.7
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
+	apache-airflow>=2.4.0.dev0
 	pypsrp>=0.8.0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.microsoft.psrp.get_provider_info:get_provider_info
 
 [files]
```

### Comparing `apache-airflow-providers-microsoft-psrp-2.2.0rc1/setup.py` & `apache-airflow-providers-microsoft-psrp-2.3.0rc1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,23 +22,28 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-microsoft-psrp package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "2.2.0"
+version = "2.3.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-microsoft-psrp setup."""
     setup(
         version=version,
         extras_require={},
         packages=find_namespace_packages(
-            include=["airflow.providers.microsoft.psrp", "airflow.providers.microsoft.psrp.*"]
+            include=[
+                "airflow.providers.microsoft.psrp",
+                "airflow.providers.microsoft.psrp.*",
+                "airflow.providers.microsoft.psrp_vendor",
+                "airflow.providers.microsoft.psrp_vendor.*",
+            ],
         ),
     )
 
 
 if __name__ == "__main__":
     do_setup()
```

