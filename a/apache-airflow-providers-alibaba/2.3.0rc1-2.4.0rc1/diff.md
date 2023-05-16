# Comparing `tmp/apache-airflow-providers-alibaba-2.3.0rc1.tar.gz` & `tmp/apache-airflow-providers-alibaba-2.4.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-alibaba-2.3.0rc1.tar", last modified: Sun Apr  2 05:46:45 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-alibaba-2.4.0rc1.tar", last modified: Tue May 16 15:52:47 2023, max compression
```

## Comparing `apache-airflow-providers-alibaba-2.3.0rc1.tar` & `apache-airflow-providers-alibaba-2.4.0rc1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:46:45.000000 apache-airflow-providers-alibaba-2.3.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-alibaba-2.3.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1122 2023-04-02 05:46:43.000000 apache-airflow-providers-alibaba-2.3.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-alibaba-2.3.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     8890 2023-04-02 05:46:45.000000 apache-airflow-providers-alibaba-2.3.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7360 2023-04-02 05:46:43.000000 apache-airflow-providers-alibaba-2.3.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:46:44.000000 apache-airflow-providers-alibaba-2.3.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:46:44.000000 apache-airflow-providers-alibaba-2.3.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:46:44.000000 apache-airflow-providers-alibaba-2.3.0rc1/airflow/providers/alibaba/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-alibaba-2.3.0rc1/airflow/providers/alibaba/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:46:44.000000 apache-airflow-providers-alibaba-2.3.0rc1/airflow/providers/alibaba/cloud/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-alibaba-2.3.0rc1/airflow/providers/alibaba/cloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:46:44.000000 apache-airflow-providers-alibaba-2.3.0rc1/airflow/providers/alibaba/cloud/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-alibaba-2.3.0rc1/airflow/providers/alibaba/cloud/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12634 2023-02-24 18:43:53.000000 apache-airflow-providers-alibaba-2.3.0rc1/airflow/providers/alibaba/cloud/hooks/oss.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:46:44.000000 apache-airflow-providers-alibaba-2.3.0rc1/airflow/providers/alibaba/cloud/log/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-alibaba-2.3.0rc1/airflow/providers/alibaba/cloud/log/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8645 2023-03-10 19:31:58.000000 apache-airflow-providers-alibaba-2.3.0rc1/airflow/providers/alibaba/cloud/log/oss_task_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:46:45.000000 apache-airflow-providers-alibaba-2.3.0rc1/airflow/providers/alibaba/cloud/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-alibaba-2.3.0rc1/airflow/providers/alibaba/cloud/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6314 2023-02-24 18:43:53.000000 apache-airflow-providers-alibaba-2.3.0rc1/airflow/providers/alibaba/cloud/operators/oss.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:46:45.000000 apache-airflow-providers-alibaba-2.3.0rc1/airflow/providers/alibaba/cloud/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-alibaba-2.3.0rc1/airflow/providers/alibaba/cloud/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3673 2023-02-24 18:43:53.000000 apache-airflow-providers-alibaba-2.3.0rc1/airflow/providers/alibaba/cloud/sensors/oss_key.py
--rw-r--r--   0 root         (0) root         (0)     2715 2023-04-02 05:46:43.000000 apache-airflow-providers-alibaba-2.3.0rc1/airflow/providers/alibaba/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:46:45.000000 apache-airflow-providers-alibaba-2.3.0rc1/apache_airflow_providers_alibaba.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8890 2023-04-02 05:46:44.000000 apache-airflow-providers-alibaba-2.3.0rc1/apache_airflow_providers_alibaba.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      998 2023-04-02 05:46:44.000000 apache-airflow-providers-alibaba-2.3.0rc1/apache_airflow_providers_alibaba.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-02 05:46:44.000000 apache-airflow-providers-alibaba-2.3.0rc1/apache_airflow_providers_alibaba.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-04-02 05:46:44.000000 apache-airflow-providers-alibaba-2.3.0rc1/apache_airflow_providers_alibaba.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-02 05:46:44.000000 apache-airflow-providers-alibaba-2.3.0rc1/apache_airflow_providers_alibaba.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       40 2023-04-02 05:46:44.000000 apache-airflow-providers-alibaba-2.3.0rc1/apache_airflow_providers_alibaba.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-02 05:46:44.000000 apache-airflow-providers-alibaba-2.3.0rc1/apache_airflow_providers_alibaba.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5393 2023-04-01 16:40:04.000000 apache-airflow-providers-alibaba-2.3.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1848 2023-04-02 05:46:45.000000 apache-airflow-providers-alibaba-2.3.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1490 2023-04-02 05:46:43.000000 apache-airflow-providers-alibaba-2.3.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:47.000000 apache-airflow-providers-alibaba-2.4.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-alibaba-2.4.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-05-16 15:52:46.000000 apache-airflow-providers-alibaba-2.4.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-alibaba-2.4.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     9633 2023-05-16 15:52:47.000000 apache-airflow-providers-alibaba-2.4.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8103 2023-05-16 15:52:46.000000 apache-airflow-providers-alibaba-2.4.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:47.000000 apache-airflow-providers-alibaba-2.4.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:47.000000 apache-airflow-providers-alibaba-2.4.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:47.000000 apache-airflow-providers-alibaba-2.4.0rc1/airflow/providers/alibaba/
+-rw-r--r--   0 root         (0) root         (0)     1390 2023-05-16 15:39:21.000000 apache-airflow-providers-alibaba-2.4.0rc1/airflow/providers/alibaba/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:47.000000 apache-airflow-providers-alibaba-2.4.0rc1/airflow/providers/alibaba/cloud/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-alibaba-2.4.0rc1/airflow/providers/alibaba/cloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:47.000000 apache-airflow-providers-alibaba-2.4.0rc1/airflow/providers/alibaba/cloud/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-alibaba-2.4.0rc1/airflow/providers/alibaba/cloud/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12634 2023-02-24 18:43:53.000000 apache-airflow-providers-alibaba-2.4.0rc1/airflow/providers/alibaba/cloud/hooks/oss.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:47.000000 apache-airflow-providers-alibaba-2.4.0rc1/airflow/providers/alibaba/cloud/log/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-alibaba-2.4.0rc1/airflow/providers/alibaba/cloud/log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8645 2023-03-10 19:31:58.000000 apache-airflow-providers-alibaba-2.4.0rc1/airflow/providers/alibaba/cloud/log/oss_task_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:47.000000 apache-airflow-providers-alibaba-2.4.0rc1/airflow/providers/alibaba/cloud/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-alibaba-2.4.0rc1/airflow/providers/alibaba/cloud/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6314 2023-02-24 18:43:53.000000 apache-airflow-providers-alibaba-2.4.0rc1/airflow/providers/alibaba/cloud/operators/oss.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:47.000000 apache-airflow-providers-alibaba-2.4.0rc1/airflow/providers/alibaba/cloud/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-alibaba-2.4.0rc1/airflow/providers/alibaba/cloud/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3673 2023-02-24 18:43:53.000000 apache-airflow-providers-alibaba-2.4.0rc1/airflow/providers/alibaba/cloud/sensors/oss_key.py
+-rw-r--r--   0 root         (0) root         (0)     2883 2023-05-16 15:52:46.000000 apache-airflow-providers-alibaba-2.4.0rc1/airflow/providers/alibaba/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:47.000000 apache-airflow-providers-alibaba-2.4.0rc1/apache_airflow_providers_alibaba.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9633 2023-05-16 15:52:47.000000 apache-airflow-providers-alibaba-2.4.0rc1/apache_airflow_providers_alibaba.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      998 2023-05-16 15:52:47.000000 apache-airflow-providers-alibaba-2.4.0rc1/apache_airflow_providers_alibaba.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:52:47.000000 apache-airflow-providers-alibaba-2.4.0rc1/apache_airflow_providers_alibaba.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2023-05-16 15:52:47.000000 apache-airflow-providers-alibaba-2.4.0rc1/apache_airflow_providers_alibaba.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:52:47.000000 apache-airflow-providers-alibaba-2.4.0rc1/apache_airflow_providers_alibaba.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       40 2023-05-16 15:52:47.000000 apache-airflow-providers-alibaba-2.4.0rc1/apache_airflow_providers_alibaba.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-16 15:52:47.000000 apache-airflow-providers-alibaba-2.4.0rc1/apache_airflow_providers_alibaba.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5308 2023-05-15 09:39:26.000000 apache-airflow-providers-alibaba-2.4.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1848 2023-05-16 15:52:47.000000 apache-airflow-providers-alibaba-2.4.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1644 2023-05-16 15:52:46.000000 apache-airflow-providers-alibaba-2.4.0rc1/setup.py
```

### Comparing `apache-airflow-providers-alibaba-2.3.0rc1/LICENSE` & `apache-airflow-providers-alibaba-2.4.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-alibaba-2.3.0rc1/MANIFEST.in` & `apache-airflow-providers-alibaba-2.4.0rc1/MANIFEST.in`

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

### Comparing `apache-airflow-providers-alibaba-2.3.0rc1/PKG-INFO` & `apache-airflow-providers-alibaba-2.4.0rc1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-alibaba
-Version: 2.3.0rc1
+Version: 2.4.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-alibaba package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-alibaba/2.3.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-alibaba/2.4.0/
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
 
 
 Package ``apache-airflow-providers-alibaba``
 
-Release: ``2.3.0rc1``
+Release: ``2.4.0rc1``
 
 
 Alibaba Cloud integration (including `Alibaba Cloud <https://www.alibabacloud.com//>`__).
 
 
 Provider package
 ----------------
 
 This is a provider package for ``alibaba`` provider. All classes for this provider package
 are in ``airflow.providers.alibaba`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-alibaba/2.3.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-alibaba/2.4.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -79,15 +79,15 @@
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
-``apache-airflow``  ``>=2.3.0``
+``apache-airflow``  ``>=2.4.0``
 ``oss2``            ``>=2.14.0``
 ==================  ==================
 
  .. Licensed to the Apache Software Foundation (ASF) under one
     or more contributor license agreements.  See the NOTICE file
     distributed with this work for additional information
     regarding copyright ownership.  The ASF licenses this file
@@ -109,27 +109,45 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+2.4.0
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
 2.3.0
 .....
 
 Features
 ~~~~~~~~
 
 * ``Support deleting the local log files when using remote logging (#29772)``
 
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
 * ``Use log.exception where more economical than log.error (#27517)``
 * ``Replace urlparse with urlsplit (#27389)``
@@ -166,16 +184,17 @@
 
 2.0.0
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
 
    * ``SSL Bucket, Light Logic Refactor and Docstring Update for Alibaba Provider (#23891)``
 
 Misc
```

### Comparing `apache-airflow-providers-alibaba-2.3.0rc1/README.rst` & `apache-airflow-providers-alibaba-2.4.0rc1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -15,28 +15,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-alibaba``
 
-Release: ``2.3.0rc1``
+Release: ``2.4.0rc1``
 
 
 Alibaba Cloud integration (including `Alibaba Cloud <https://www.alibabacloud.com//>`__).
 
 
 Provider package
 ----------------
 
 This is a provider package for ``alibaba`` provider. All classes for this provider package
 are in ``airflow.providers.alibaba`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-alibaba/2.3.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-alibaba/2.4.0/>`_.
 
 
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
 ``oss2``            ``>=2.14.0``
 ==================  ==================
 
  .. Licensed to the Apache Software Foundation (ASF) under one
     or more contributor license agreements.  See the NOTICE file
     distributed with this work for additional information
     regarding copyright ownership.  The ASF licenses this file
@@ -76,27 +76,45 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+2.4.0
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
 2.3.0
 .....
 
 Features
 ~~~~~~~~
 
 * ``Support deleting the local log files when using remote logging (#29772)``
 
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
 * ``Use log.exception where more economical than log.error (#27517)``
 * ``Replace urlparse with urlsplit (#27389)``
@@ -133,16 +151,17 @@
 
 2.0.0
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
 
    * ``SSL Bucket, Light Logic Refactor and Docstring Update for Alibaba Provider (#23891)``
 
 Misc
```

### Comparing `apache-airflow-providers-alibaba-2.3.0rc1/airflow/providers/alibaba/__init__.py` & `apache-airflow-providers-alibaba-2.4.0rc1/airflow/providers/alibaba/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-alibaba-2.3.0rc1/airflow/providers/alibaba/cloud/__init__.py` & `apache-airflow-providers-alibaba-2.4.0rc1/airflow/providers/alibaba/cloud/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-alibaba-2.3.0rc1/airflow/providers/alibaba/cloud/hooks/__init__.py` & `apache-airflow-providers-alibaba-2.4.0rc1/airflow/providers/alibaba/cloud/log/__init__.py`

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

### Comparing `apache-airflow-providers-alibaba-2.3.0rc1/airflow/providers/alibaba/cloud/hooks/oss.py` & `apache-airflow-providers-alibaba-2.4.0rc1/airflow/providers/alibaba/cloud/hooks/oss.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-alibaba-2.3.0rc1/airflow/providers/alibaba/cloud/log/__init__.py` & `apache-airflow-providers-alibaba-2.4.0rc1/airflow/providers/alibaba/cloud/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-alibaba-2.3.0rc1/airflow/providers/alibaba/cloud/log/oss_task_handler.py` & `apache-airflow-providers-alibaba-2.4.0rc1/airflow/providers/alibaba/cloud/log/oss_task_handler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-alibaba-2.3.0rc1/airflow/providers/alibaba/cloud/operators/__init__.py` & `apache-airflow-providers-alibaba-2.4.0rc1/airflow/providers/alibaba/cloud/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-alibaba-2.3.0rc1/airflow/providers/alibaba/cloud/operators/oss.py` & `apache-airflow-providers-alibaba-2.4.0rc1/airflow/providers/alibaba/cloud/operators/oss.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-alibaba-2.3.0rc1/airflow/providers/alibaba/cloud/sensors/oss_key.py` & `apache-airflow-providers-alibaba-2.4.0rc1/airflow/providers/alibaba/cloud/sensors/oss_key.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-alibaba-2.3.0rc1/airflow/providers/alibaba/get_provider_info.py` & `apache-airflow-providers-alibaba-2.4.0rc1/airflow/providers/alibaba/get_provider_info.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,16 +23,28 @@
 
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-alibaba",
         "name": "Alibaba",
         "description": "Alibaba Cloud integration (including `Alibaba Cloud <https://www.alibabacloud.com//>`__).\n",
-        "versions": ["2.3.0", "2.2.0", "2.1.0", "2.0.1", "2.0.0", "1.1.1", "1.1.0", "1.0.1", "1.0.0"],
-        "dependencies": ["apache-airflow>=2.3.0", "oss2>=2.14.0"],
+        "suspended": False,
+        "versions": [
+            "2.4.0",
+            "2.3.0",
+            "2.2.0",
+            "2.1.0",
+            "2.0.1",
+            "2.0.0",
+            "1.1.1",
+            "1.1.0",
+            "1.0.1",
+            "1.0.0",
+        ],
+        "dependencies": ["apache-airflow>=2.4.0", "oss2>=2.14.0"],
         "integrations": [
             {
                 "integration-name": "Alibaba Cloud OSS",
                 "external-doc-url": "https://www.alibabacloud.com/help/product/31815.htm",
                 "logo": "/integration-logos/alibaba/cloud/alibabacloud-oss.png",
                 "how-to-guide": ["/docs/apache-airflow-providers-alibaba/operators/oss.rst"],
                 "tags": ["alibaba"],
```

### Comparing `apache-airflow-providers-alibaba-2.3.0rc1/apache_airflow_providers_alibaba.egg-info/PKG-INFO` & `apache-airflow-providers-alibaba-2.4.0rc1/apache_airflow_providers_alibaba.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-alibaba
-Version: 2.3.0rc1
+Version: 2.4.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-alibaba package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-alibaba/2.3.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-alibaba/2.4.0/
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
 
 
 Package ``apache-airflow-providers-alibaba``
 
-Release: ``2.3.0rc1``
+Release: ``2.4.0rc1``
 
 
 Alibaba Cloud integration (including `Alibaba Cloud <https://www.alibabacloud.com//>`__).
 
 
 Provider package
 ----------------
 
 This is a provider package for ``alibaba`` provider. All classes for this provider package
 are in ``airflow.providers.alibaba`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-alibaba/2.3.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-alibaba/2.4.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -79,15 +79,15 @@
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
-``apache-airflow``  ``>=2.3.0``
+``apache-airflow``  ``>=2.4.0``
 ``oss2``            ``>=2.14.0``
 ==================  ==================
 
  .. Licensed to the Apache Software Foundation (ASF) under one
     or more contributor license agreements.  See the NOTICE file
     distributed with this work for additional information
     regarding copyright ownership.  The ASF licenses this file
@@ -109,27 +109,45 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+2.4.0
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
 2.3.0
 .....
 
 Features
 ~~~~~~~~
 
 * ``Support deleting the local log files when using remote logging (#29772)``
 
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
 * ``Use log.exception where more economical than log.error (#27517)``
 * ``Replace urlparse with urlsplit (#27389)``
@@ -166,16 +184,17 @@
 
 2.0.0
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
 
    * ``SSL Bucket, Light Logic Refactor and Docstring Update for Alibaba Provider (#23891)``
 
 Misc
```

### Comparing `apache-airflow-providers-alibaba-2.3.0rc1/apache_airflow_providers_alibaba.egg-info/SOURCES.txt` & `apache-airflow-providers-alibaba-2.4.0rc1/apache_airflow_providers_alibaba.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-alibaba-2.3.0rc1/pyproject.toml` & `apache-airflow-providers-alibaba-2.4.0rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-alibaba-2.3.0rc1/setup.cfg` & `apache-airflow-providers-alibaba-2.4.0rc1/setup.cfg`

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-alibaba/2.3.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-alibaba/2.4.0/
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
 	oss2>=2.14.0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.alibaba.get_provider_info:get_provider_info
 
 [files]
```

### Comparing `apache-airflow-providers-alibaba-2.3.0rc1/setup.py` & `apache-airflow-providers-alibaba-2.4.0rc1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,23 +22,28 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-alibaba package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "2.3.0"
+version = "2.4.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-alibaba setup."""
     setup(
         version=version,
         extras_require={},
         packages=find_namespace_packages(
-            include=["airflow.providers.alibaba", "airflow.providers.alibaba.*"]
+            include=[
+                "airflow.providers.alibaba",
+                "airflow.providers.alibaba.*",
+                "airflow.providers.alibaba_vendor",
+                "airflow.providers.alibaba_vendor.*",
+            ],
         ),
     )
 
 
 if __name__ == "__main__":
     do_setup()
```

