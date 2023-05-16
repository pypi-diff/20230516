# Comparing `tmp/apache-airflow-providers-grpc-3.1.0rc1.tar.gz` & `tmp/apache-airflow-providers-grpc-3.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-grpc-3.1.0rc1.tar", last modified: Tue Nov 15 00:14:44 2022, max compression
+gzip compressed data, was "dist/apache-airflow-providers-grpc-3.2.0rc1.tar", last modified: Tue May 16 15:54:18 2023, max compression
```

## Comparing `apache-airflow-providers-grpc-3.1.0rc1.tar` & `apache-airflow-providers-grpc-3.2.0rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:14:44.000000 apache-airflow-providers-grpc-3.1.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2022-05-27 19:54:38.000000 apache-airflow-providers-grpc-3.1.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1122 2022-11-15 00:14:42.000000 apache-airflow-providers-grpc-3.1.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2022-05-27 19:54:38.000000 apache-airflow-providers-grpc-3.1.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     9199 2022-11-15 00:14:44.000000 apache-airflow-providers-grpc-3.1.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7658 2022-11-15 00:14:42.000000 apache-airflow-providers-grpc-3.1.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:14:44.000000 apache-airflow-providers-grpc-3.1.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:14:44.000000 apache-airflow-providers-grpc-3.1.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:14:44.000000 apache-airflow-providers-grpc-3.1.0rc1/airflow/providers/grpc/
--rw-r--r--   0 root         (0) root         (0)      787 2022-09-13 10:31:21.000000 apache-airflow-providers-grpc-3.1.0rc1/airflow/providers/grpc/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2164 2022-11-15 00:14:42.000000 apache-airflow-providers-grpc-3.1.0rc1/airflow/providers/grpc/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:14:44.000000 apache-airflow-providers-grpc-3.1.0rc1/airflow/providers/grpc/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2022-09-13 10:31:21.000000 apache-airflow-providers-grpc-3.1.0rc1/airflow/providers/grpc/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6850 2022-11-06 15:33:45.000000 apache-airflow-providers-grpc-3.1.0rc1/airflow/providers/grpc/hooks/grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:14:44.000000 apache-airflow-providers-grpc-3.1.0rc1/airflow/providers/grpc/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2022-09-13 10:31:21.000000 apache-airflow-providers-grpc-3.1.0rc1/airflow/providers/grpc/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3799 2022-10-26 03:21:46.000000 apache-airflow-providers-grpc-3.1.0rc1/airflow/providers/grpc/operators/grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:14:44.000000 apache-airflow-providers-grpc-3.1.0rc1/apache_airflow_providers_grpc.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9199 2022-11-15 00:14:44.000000 apache-airflow-providers-grpc-3.1.0rc1/apache_airflow_providers_grpc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      686 2022-11-15 00:14:44.000000 apache-airflow-providers-grpc-3.1.0rc1/apache_airflow_providers_grpc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-15 00:14:44.000000 apache-airflow-providers-grpc-3.1.0rc1/apache_airflow_providers_grpc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      102 2022-11-15 00:14:44.000000 apache-airflow-providers-grpc-3.1.0rc1/apache_airflow_providers_grpc.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-15 00:14:44.000000 apache-airflow-providers-grpc-3.1.0rc1/apache_airflow_providers_grpc.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       93 2022-11-15 00:14:44.000000 apache-airflow-providers-grpc-3.1.0rc1/apache_airflow_providers_grpc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2022-11-15 00:14:44.000000 apache-airflow-providers-grpc-3.1.0rc1/apache_airflow_providers_grpc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1836 2022-10-26 03:21:46.000000 apache-airflow-providers-grpc-3.1.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1886 2022-11-15 00:14:44.000000 apache-airflow-providers-grpc-3.1.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1456 2022-11-15 00:14:42.000000 apache-airflow-providers-grpc-3.1.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:18.000000 apache-airflow-providers-grpc-3.2.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-grpc-3.2.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-05-16 15:54:16.000000 apache-airflow-providers-grpc-3.2.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-grpc-3.2.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    10113 2023-05-16 15:54:18.000000 apache-airflow-providers-grpc-3.2.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8592 2023-05-16 15:54:16.000000 apache-airflow-providers-grpc-3.2.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:17.000000 apache-airflow-providers-grpc-3.2.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:17.000000 apache-airflow-providers-grpc-3.2.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:18.000000 apache-airflow-providers-grpc-3.2.0rc1/airflow/providers/grpc/
+-rw-r--r--   0 root         (0) root         (0)     1387 2023-05-16 15:39:21.000000 apache-airflow-providers-grpc-3.2.0rc1/airflow/providers/grpc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2213 2023-05-16 15:54:16.000000 apache-airflow-providers-grpc-3.2.0rc1/airflow/providers/grpc/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:18.000000 apache-airflow-providers-grpc-3.2.0rc1/airflow/providers/grpc/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-grpc-3.2.0rc1/airflow/providers/grpc/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6850 2023-02-24 18:43:53.000000 apache-airflow-providers-grpc-3.2.0rc1/airflow/providers/grpc/hooks/grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:18.000000 apache-airflow-providers-grpc-3.2.0rc1/airflow/providers/grpc/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-grpc-3.2.0rc1/airflow/providers/grpc/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3799 2023-02-24 18:43:53.000000 apache-airflow-providers-grpc-3.2.0rc1/airflow/providers/grpc/operators/grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:18.000000 apache-airflow-providers-grpc-3.2.0rc1/apache_airflow_providers_grpc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10113 2023-05-16 15:54:17.000000 apache-airflow-providers-grpc-3.2.0rc1/apache_airflow_providers_grpc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      686 2023-05-16 15:54:17.000000 apache-airflow-providers-grpc-3.2.0rc1/apache_airflow_providers_grpc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:54:17.000000 apache-airflow-providers-grpc-3.2.0rc1/apache_airflow_providers_grpc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      101 2023-05-16 15:54:17.000000 apache-airflow-providers-grpc-3.2.0rc1/apache_airflow_providers_grpc.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:54:17.000000 apache-airflow-providers-grpc-3.2.0rc1/apache_airflow_providers_grpc.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       96 2023-05-16 15:54:17.000000 apache-airflow-providers-grpc-3.2.0rc1/apache_airflow_providers_grpc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-16 15:54:17.000000 apache-airflow-providers-grpc-3.2.0rc1/apache_airflow_providers_grpc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5308 2023-05-15 09:39:26.000000 apache-airflow-providers-grpc-3.2.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1889 2023-05-16 15:54:18.000000 apache-airflow-providers-grpc-3.2.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1626 2023-05-16 15:54:16.000000 apache-airflow-providers-grpc-3.2.0rc1/setup.py
```

### Comparing `apache-airflow-providers-grpc-3.1.0rc1/LICENSE` & `apache-airflow-providers-grpc-3.2.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-grpc-3.1.0rc1/MANIFEST.in` & `apache-airflow-providers-grpc-3.2.0rc1/MANIFEST.in`

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

### Comparing `apache-airflow-providers-grpc-3.1.0rc1/PKG-INFO` & `apache-airflow-providers-grpc-3.2.0rc1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-grpc
-Version: 3.1.0rc1
+Version: 3.2.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-grpc package
 Home-page: https://airflow.apache.org/
+Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Download-URL: https://archive.apache.org/dist/airflow/providers
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-grpc/3.1.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-grpc/3.2.0/
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
 
 
 Package ``apache-airflow-providers-grpc``
 
-Release: ``3.1.0rc1``
+Release: ``3.2.0rc1``
 
 
 `gRPC <https://grpc.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``grpc`` provider. All classes for this provider package
 are in ``airflow.providers.grpc`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-grpc/3.1.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-grpc/3.2.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -80,15 +79,15 @@
 
 Requirements
 ------------
 
 ========================  ===================
 PIP package               Version required
 ========================  ===================
-``apache-airflow``        ``>=2.3.0``
+``apache-airflow``        ``>=2.4.0``
 ``google-auth``           ``>=1.0.0, <3.0.0``
 ``google-auth-httplib2``  ``>=0.0.1``
 ``grpcio``                ``>=1.15.0``
 ========================  ===================
 
  .. Licensed to the Apache Software Foundation (ASF) under one
     or more contributor license agreements.  See the NOTICE file
@@ -112,55 +111,77 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
-3.1.0
+3.2.0
 .....
 
-This release of provider is only available for Airflow 2.3+ as explained in the
-`Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/README.md#support-for-providers>`_.
+.. note::
+  This release of provider is only available for Airflow 2.4+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Misc
 ~~~~
 
-In GrpcHook, non-prefixed extra fields are supported and are preferred.  E.g. ``auth_type`` will
-be preferred if ``extra__grpc__auth_type`` is also present.
+* ``Bump minimum Airflow version in providers (#30917)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Prepare docs for Jan 2023 wave of Providers (#28651)``
+   * ``Updated docs for RC3 wave of providers (#27937)``
+   * ``Prepare for follow-up relase for November providers (#27774)``
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add mechanism to suspend providers (#30422)``
+
+3.1.0
+.....
+
+.. note::
+  This release of provider is only available for Airflow 2.3+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
+
+Misc
+~~~~
 
 * ``Move min airflow version to 2.3.0 for all providers (#27196)``
 
 Features
 ~~~~~~~~
 
-* ``Look for 'extra__' instead of 'extra_' in 'get_field' (#27489)``
+In GrpcHook, non-prefixed extra fields are supported and are preferred.  E.g. ``auth_type`` will
+be preferred if ``extra__grpc__auth_type`` is also present.
+
 * ``Allow and prefer non-prefixed extra fields for GrpcHook (#27045)``
 
 Bug Fixes
 ~~~~~~~~~
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
+  * ``Look for 'extra__' instead of 'extra_' in 'get_field' (#27489)``
   * ``Add documentation for July 2022 Provider's release (#25030)``
   * ``Enable string normalization in python formatting - providers (#27205)``
   * ``Update docs for September Provider's release (#26731)``
   * ``Apply PEP-563 (Postponed Evaluation of Annotations) to non-core airflow (#26289)``
   * ``Prepare docs for new providers release (August 2022) (#25618)``
   * ``Move provider dependencies to inside provider folders (#24672)``
   * ``Remove 'hook-class-names' from provider.yaml (#24702)``
 
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
 
@@ -250,9 +271,7 @@
 
 Updated documentation and readme files.
 
 1.0.0
 .....
 
 Initial version of the provider.
-
-
```

### Comparing `apache-airflow-providers-grpc-3.1.0rc1/README.rst` & `apache-airflow-providers-grpc-3.2.0rc1/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -15,28 +15,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-grpc``
 
-Release: ``3.1.0rc1``
+Release: ``3.2.0rc1``
 
 
 `gRPC <https://grpc.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``grpc`` provider. All classes for this provider package
 are in ``airflow.providers.grpc`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-grpc/3.1.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-grpc/3.2.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -46,15 +46,15 @@
 
 Requirements
 ------------
 
 ========================  ===================
 PIP package               Version required
 ========================  ===================
-``apache-airflow``        ``>=2.3.0``
+``apache-airflow``        ``>=2.4.0``
 ``google-auth``           ``>=1.0.0, <3.0.0``
 ``google-auth-httplib2``  ``>=0.0.1``
 ``grpcio``                ``>=1.15.0``
 ========================  ===================
 
  .. Licensed to the Apache Software Foundation (ASF) under one
     or more contributor license agreements.  See the NOTICE file
@@ -78,55 +78,77 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
-3.1.0
+3.2.0
 .....
 
-This release of provider is only available for Airflow 2.3+ as explained in the
-`Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/README.md#support-for-providers>`_.
+.. note::
+  This release of provider is only available for Airflow 2.4+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Misc
 ~~~~
 
-In GrpcHook, non-prefixed extra fields are supported and are preferred.  E.g. ``auth_type`` will
-be preferred if ``extra__grpc__auth_type`` is also present.
+* ``Bump minimum Airflow version in providers (#30917)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Prepare docs for Jan 2023 wave of Providers (#28651)``
+   * ``Updated docs for RC3 wave of providers (#27937)``
+   * ``Prepare for follow-up relase for November providers (#27774)``
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add mechanism to suspend providers (#30422)``
+
+3.1.0
+.....
+
+.. note::
+  This release of provider is only available for Airflow 2.3+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
+
+Misc
+~~~~
 
 * ``Move min airflow version to 2.3.0 for all providers (#27196)``
 
 Features
 ~~~~~~~~
 
-* ``Look for 'extra__' instead of 'extra_' in 'get_field' (#27489)``
+In GrpcHook, non-prefixed extra fields are supported and are preferred.  E.g. ``auth_type`` will
+be preferred if ``extra__grpc__auth_type`` is also present.
+
 * ``Allow and prefer non-prefixed extra fields for GrpcHook (#27045)``
 
 Bug Fixes
 ~~~~~~~~~
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
+  * ``Look for 'extra__' instead of 'extra_' in 'get_field' (#27489)``
   * ``Add documentation for July 2022 Provider's release (#25030)``
   * ``Enable string normalization in python formatting - providers (#27205)``
   * ``Update docs for September Provider's release (#26731)``
   * ``Apply PEP-563 (Postponed Evaluation of Annotations) to non-core airflow (#26289)``
   * ``Prepare docs for new providers release (August 2022) (#25618)``
   * ``Move provider dependencies to inside provider folders (#24672)``
   * ``Remove 'hook-class-names' from provider.yaml (#24702)``
 
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

### Comparing `apache-airflow-providers-grpc-3.1.0rc1/airflow/providers/grpc/__init__.py` & `apache-airflow-providers-grpc-3.2.0rc1/airflow/providers/grpc/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-grpc-3.1.0rc1/airflow/providers/grpc/get_provider_info.py` & `apache-airflow-providers-grpc-3.2.0rc1/airflow/providers/grpc/get_provider_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,28 +23,30 @@
 
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-grpc",
         "name": "gRPC",
         "description": "`gRPC <https://grpc.io/>`__\n",
+        "suspended": False,
         "versions": [
+            "3.2.0",
             "3.1.0",
             "3.0.0",
             "2.0.4",
             "2.0.3",
             "2.0.2",
             "2.0.1",
             "2.0.0",
             "1.1.0",
             "1.0.1",
             "1.0.0",
         ],
         "dependencies": [
-            "apache-airflow>=2.3.0",
+            "apache-airflow>=2.4.0",
             "google-auth>=1.0.0, <3.0.0",
             "google-auth-httplib2>=0.0.1",
             "grpcio>=1.15.0",
         ],
         "integrations": [
             {"integration-name": "gRPC", "external-doc-url": "https://grpc.io/", "tags": ["protocol"]}
         ],
```

### Comparing `apache-airflow-providers-grpc-3.1.0rc1/airflow/providers/grpc/hooks/__init__.py` & `apache-airflow-providers-grpc-3.2.0rc1/airflow/providers/grpc/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-grpc-3.1.0rc1/airflow/providers/grpc/hooks/grpc.py` & `apache-airflow-providers-grpc-3.2.0rc1/airflow/providers/grpc/hooks/grpc.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-grpc-3.1.0rc1/airflow/providers/grpc/operators/grpc.py` & `apache-airflow-providers-grpc-3.2.0rc1/airflow/providers/grpc/operators/grpc.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-grpc-3.1.0rc1/apache_airflow_providers_grpc.egg-info/PKG-INFO` & `apache-airflow-providers-grpc-3.2.0rc1/apache_airflow_providers_grpc.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-grpc
-Version: 3.1.0rc1
+Version: 3.2.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-grpc package
 Home-page: https://airflow.apache.org/
+Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Download-URL: https://archive.apache.org/dist/airflow/providers
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-grpc/3.1.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-grpc/3.2.0/
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
 
 
 Package ``apache-airflow-providers-grpc``
 
-Release: ``3.1.0rc1``
+Release: ``3.2.0rc1``
 
 
 `gRPC <https://grpc.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``grpc`` provider. All classes for this provider package
 are in ``airflow.providers.grpc`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-grpc/3.1.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-grpc/3.2.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -80,15 +79,15 @@
 
 Requirements
 ------------
 
 ========================  ===================
 PIP package               Version required
 ========================  ===================
-``apache-airflow``        ``>=2.3.0``
+``apache-airflow``        ``>=2.4.0``
 ``google-auth``           ``>=1.0.0, <3.0.0``
 ``google-auth-httplib2``  ``>=0.0.1``
 ``grpcio``                ``>=1.15.0``
 ========================  ===================
 
  .. Licensed to the Apache Software Foundation (ASF) under one
     or more contributor license agreements.  See the NOTICE file
@@ -112,55 +111,77 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
-3.1.0
+3.2.0
 .....
 
-This release of provider is only available for Airflow 2.3+ as explained in the
-`Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/README.md#support-for-providers>`_.
+.. note::
+  This release of provider is only available for Airflow 2.4+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Misc
 ~~~~
 
-In GrpcHook, non-prefixed extra fields are supported and are preferred.  E.g. ``auth_type`` will
-be preferred if ``extra__grpc__auth_type`` is also present.
+* ``Bump minimum Airflow version in providers (#30917)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Prepare docs for Jan 2023 wave of Providers (#28651)``
+   * ``Updated docs for RC3 wave of providers (#27937)``
+   * ``Prepare for follow-up relase for November providers (#27774)``
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add mechanism to suspend providers (#30422)``
+
+3.1.0
+.....
+
+.. note::
+  This release of provider is only available for Airflow 2.3+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
+
+Misc
+~~~~
 
 * ``Move min airflow version to 2.3.0 for all providers (#27196)``
 
 Features
 ~~~~~~~~
 
-* ``Look for 'extra__' instead of 'extra_' in 'get_field' (#27489)``
+In GrpcHook, non-prefixed extra fields are supported and are preferred.  E.g. ``auth_type`` will
+be preferred if ``extra__grpc__auth_type`` is also present.
+
 * ``Allow and prefer non-prefixed extra fields for GrpcHook (#27045)``
 
 Bug Fixes
 ~~~~~~~~~
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
+  * ``Look for 'extra__' instead of 'extra_' in 'get_field' (#27489)``
   * ``Add documentation for July 2022 Provider's release (#25030)``
   * ``Enable string normalization in python formatting - providers (#27205)``
   * ``Update docs for September Provider's release (#26731)``
   * ``Apply PEP-563 (Postponed Evaluation of Annotations) to non-core airflow (#26289)``
   * ``Prepare docs for new providers release (August 2022) (#25618)``
   * ``Move provider dependencies to inside provider folders (#24672)``
   * ``Remove 'hook-class-names' from provider.yaml (#24702)``
 
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
 
@@ -250,9 +271,7 @@
 
 Updated documentation and readme files.
 
 1.0.0
 .....
 
 Initial version of the provider.
-
-
```

### Comparing `apache-airflow-providers-grpc-3.1.0rc1/apache_airflow_providers_grpc.egg-info/SOURCES.txt` & `apache-airflow-providers-grpc-3.2.0rc1/apache_airflow_providers_grpc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-grpc-3.1.0rc1/setup.cfg` & `apache-airflow-providers-grpc-3.2.0rc1/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-grpc/3.1.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-grpc/3.2.0/
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
 	google-auth-httplib2>=0.0.1
 	google-auth>=1.0.0, <3.0.0
 	grpcio>=1.15.0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.grpc.get_provider_info:get_provider_info
```

### Comparing `apache-airflow-providers-grpc-3.1.0rc1/setup.py` & `apache-airflow-providers-grpc-3.2.0rc1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -22,21 +22,28 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-grpc package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "3.1.0"
+version = "3.2.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-grpc setup."""
     setup(
         version=version,
         extras_require={},
-        packages=find_namespace_packages(include=["airflow.providers.grpc", "airflow.providers.grpc.*"]),
+        packages=find_namespace_packages(
+            include=[
+                "airflow.providers.grpc",
+                "airflow.providers.grpc.*",
+                "airflow.providers.grpc_vendor",
+                "airflow.providers.grpc_vendor.*",
+            ],
+        ),
     )
 
 
 if __name__ == "__main__":
     do_setup()
```

