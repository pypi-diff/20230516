# Comparing `tmp/apache-airflow-providers-smtp-1.0.1rc1.tar.gz` & `tmp/apache-airflow-providers-smtp-1.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-smtp-1.0.1rc1.tar", last modified: Sun Apr  9 13:49:56 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-smtp-1.1.0rc1.tar", last modified: Tue May 16 15:55:16 2023, max compression
```

## Comparing `apache-airflow-providers-smtp-1.0.1rc1.tar` & `apache-airflow-providers-smtp-1.1.0rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:49:56.000000 apache-airflow-providers-smtp-1.0.1rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-smtp-1.0.1rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-04-09 13:49:54.000000 apache-airflow-providers-smtp-1.0.1rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-smtp-1.0.1rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     4888 2023-04-09 13:49:56.000000 apache-airflow-providers-smtp-1.0.1rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3367 2023-04-09 13:49:54.000000 apache-airflow-providers-smtp-1.0.1rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:49:56.000000 apache-airflow-providers-smtp-1.0.1rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:49:56.000000 apache-airflow-providers-smtp-1.0.1rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:49:56.000000 apache-airflow-providers-smtp-1.0.1rc1/airflow/providers/smtp/
--rw-r--r--   0 root         (0) root         (0)      787 2023-03-15 08:58:48.000000 apache-airflow-providers-smtp-1.0.1rc1/airflow/providers/smtp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2288 2023-04-09 13:49:54.000000 apache-airflow-providers-smtp-1.0.1rc1/airflow/providers/smtp/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:49:56.000000 apache-airflow-providers-smtp-1.0.1rc1/airflow/providers/smtp/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-03-15 08:58:48.000000 apache-airflow-providers-smtp-1.0.1rc1/airflow/providers/smtp/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13824 2023-04-07 21:10:19.000000 apache-airflow-providers-smtp-1.0.1rc1/airflow/providers/smtp/hooks/smtp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:49:56.000000 apache-airflow-providers-smtp-1.0.1rc1/airflow/providers/smtp/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-03-15 08:58:48.000000 apache-airflow-providers-smtp-1.0.1rc1/airflow/providers/smtp/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3434 2023-04-09 06:57:27.000000 apache-airflow-providers-smtp-1.0.1rc1/airflow/providers/smtp/operators/smtp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 13:49:56.000000 apache-airflow-providers-smtp-1.0.1rc1/apache_airflow_providers_smtp.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4888 2023-04-09 13:49:56.000000 apache-airflow-providers-smtp-1.0.1rc1/apache_airflow_providers_smtp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      686 2023-04-09 13:49:56.000000 apache-airflow-providers-smtp-1.0.1rc1/apache_airflow_providers_smtp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-09 13:49:56.000000 apache-airflow-providers-smtp-1.0.1rc1/apache_airflow_providers_smtp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      101 2023-04-09 13:49:56.000000 apache-airflow-providers-smtp-1.0.1rc1/apache_airflow_providers_smtp.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-09 13:49:56.000000 apache-airflow-providers-smtp-1.0.1rc1/apache_airflow_providers_smtp.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       27 2023-04-09 13:49:56.000000 apache-airflow-providers-smtp-1.0.1rc1/apache_airflow_providers_smtp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-09 13:49:56.000000 apache-airflow-providers-smtp-1.0.1rc1/apache_airflow_providers_smtp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5246 2023-04-07 12:28:58.000000 apache-airflow-providers-smtp-1.0.1rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1816 2023-04-09 13:49:56.000000 apache-airflow-providers-smtp-1.0.1rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1626 2023-04-09 13:49:54.000000 apache-airflow-providers-smtp-1.0.1rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:16.000000 apache-airflow-providers-smtp-1.1.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-smtp-1.1.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-05-16 15:55:15.000000 apache-airflow-providers-smtp-1.1.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-smtp-1.1.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5446 2023-05-16 15:55:16.000000 apache-airflow-providers-smtp-1.1.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3925 2023-05-16 15:55:15.000000 apache-airflow-providers-smtp-1.1.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:16.000000 apache-airflow-providers-smtp-1.1.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:16.000000 apache-airflow-providers-smtp-1.1.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:16.000000 apache-airflow-providers-smtp-1.1.0rc1/airflow/providers/smtp/
+-rw-r--r--   0 root         (0) root         (0)     1387 2023-05-16 15:39:21.000000 apache-airflow-providers-smtp-1.1.0rc1/airflow/providers/smtp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2297 2023-05-16 15:55:15.000000 apache-airflow-providers-smtp-1.1.0rc1/airflow/providers/smtp/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:16.000000 apache-airflow-providers-smtp-1.1.0rc1/airflow/providers/smtp/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-03-15 08:58:48.000000 apache-airflow-providers-smtp-1.1.0rc1/airflow/providers/smtp/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13824 2023-04-07 21:10:19.000000 apache-airflow-providers-smtp-1.1.0rc1/airflow/providers/smtp/hooks/smtp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:16.000000 apache-airflow-providers-smtp-1.1.0rc1/airflow/providers/smtp/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-03-15 08:58:48.000000 apache-airflow-providers-smtp-1.1.0rc1/airflow/providers/smtp/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3434 2023-04-13 08:25:20.000000 apache-airflow-providers-smtp-1.1.0rc1/airflow/providers/smtp/operators/smtp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:16.000000 apache-airflow-providers-smtp-1.1.0rc1/apache_airflow_providers_smtp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5446 2023-05-16 15:55:16.000000 apache-airflow-providers-smtp-1.1.0rc1/apache_airflow_providers_smtp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      686 2023-05-16 15:55:16.000000 apache-airflow-providers-smtp-1.1.0rc1/apache_airflow_providers_smtp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:55:16.000000 apache-airflow-providers-smtp-1.1.0rc1/apache_airflow_providers_smtp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      101 2023-05-16 15:55:16.000000 apache-airflow-providers-smtp-1.1.0rc1/apache_airflow_providers_smtp.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:55:16.000000 apache-airflow-providers-smtp-1.1.0rc1/apache_airflow_providers_smtp.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       27 2023-05-16 15:55:16.000000 apache-airflow-providers-smtp-1.1.0rc1/apache_airflow_providers_smtp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-16 15:55:16.000000 apache-airflow-providers-smtp-1.1.0rc1/apache_airflow_providers_smtp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5308 2023-05-15 09:39:26.000000 apache-airflow-providers-smtp-1.1.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1816 2023-05-16 15:55:16.000000 apache-airflow-providers-smtp-1.1.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1626 2023-05-16 15:55:15.000000 apache-airflow-providers-smtp-1.1.0rc1/setup.py
```

### Comparing `apache-airflow-providers-smtp-1.0.1rc1/LICENSE` & `apache-airflow-providers-smtp-1.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-smtp-1.0.1rc1/MANIFEST.in` & `apache-airflow-providers-smtp-1.1.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-smtp-1.0.1rc1/PKG-INFO` & `apache-airflow-providers-smtp-1.1.0rc1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-smtp
-Version: 1.0.1rc1
+Version: 1.1.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-smtp package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-smtp/1.0.1/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-smtp/1.1.0/
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
 
 
 Package ``apache-airflow-providers-smtp``
 
-Release: ``1.0.1rc1``
+Release: ``1.1.0rc1``
 
 
 `Simple Mail Transfer Protocol (SMTP) <https://tools.ietf.org/html/rfc5321>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``smtp`` provider. All classes for this provider package
 are in ``airflow.providers.smtp`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-smtp/1.0.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-smtp/1.1.0/>`_.
 
 
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
 ==================  ==================
 
  .. Licensed to the Apache Software Foundation (ASF) under one
     or more contributor license agreements.  See the NOTICE file
     distributed with this work for additional information
     regarding copyright ownership.  The ASF licenses this file
     to you under the Apache License, Version 2.0 (the
@@ -108,14 +108,30 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+1.1.0
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
+
 1.0.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
 
 * ``'EmailOperator': fix wrong assignment of 'from_email' (#30524)``
```

### Comparing `apache-airflow-providers-smtp-1.0.1rc1/README.rst` & `apache-airflow-providers-smtp-1.1.0rc1/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -15,28 +15,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-smtp``
 
-Release: ``1.0.1rc1``
+Release: ``1.1.0rc1``
 
 
 `Simple Mail Transfer Protocol (SMTP) <https://tools.ietf.org/html/rfc5321>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``smtp`` provider. All classes for this provider package
 are in ``airflow.providers.smtp`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-smtp/1.0.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-smtp/1.1.0/>`_.
 
 
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
@@ -75,14 +75,30 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+1.1.0
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
+
 1.0.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
 
 * ``'EmailOperator': fix wrong assignment of 'from_email' (#30524)``
```

### Comparing `apache-airflow-providers-smtp-1.0.1rc1/airflow/providers/smtp/__init__.py` & `apache-airflow-providers-smtp-1.1.0rc1/airflow/providers/smtp/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-smtp-1.0.1rc1/airflow/providers/smtp/get_provider_info.py` & `apache-airflow-providers-smtp-1.1.0rc1/airflow/providers/smtp/get_provider_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-smtp",
         "name": "Simple Mail Transfer Protocol (SMTP)",
         "description": "`Simple Mail Transfer Protocol (SMTP) <https://tools.ietf.org/html/rfc5321>`__\n",
         "suspended": False,
-        "versions": ["1.0.1", "1.0.0"],
-        "dependencies": ["apache-airflow>=2.3.0"],
+        "versions": ["1.1.0", "1.0.1", "1.0.0"],
+        "dependencies": ["apache-airflow>=2.4.0"],
         "integrations": [
             {
                 "integration-name": "Simple Mail Transfer Protocol (SMTP)",
                 "external-doc-url": "https://tools.ietf.org/html/rfc5321",
                 "logo": "/integration-logos/smtp/SMTP.png",
                 "tags": ["protocol"],
             }
```

### Comparing `apache-airflow-providers-smtp-1.0.1rc1/airflow/providers/smtp/hooks/__init__.py` & `apache-airflow-providers-smtp-1.1.0rc1/airflow/providers/smtp/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-smtp-1.0.1rc1/airflow/providers/smtp/hooks/smtp.py` & `apache-airflow-providers-smtp-1.1.0rc1/airflow/providers/smtp/hooks/smtp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-smtp-1.0.1rc1/airflow/providers/smtp/operators/smtp.py` & `apache-airflow-providers-smtp-1.1.0rc1/airflow/providers/smtp/operators/smtp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-smtp-1.0.1rc1/apache_airflow_providers_smtp.egg-info/PKG-INFO` & `apache-airflow-providers-smtp-1.1.0rc1/apache_airflow_providers_smtp.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-smtp
-Version: 1.0.1rc1
+Version: 1.1.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-smtp package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-smtp/1.0.1/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-smtp/1.1.0/
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
 
 
 Package ``apache-airflow-providers-smtp``
 
-Release: ``1.0.1rc1``
+Release: ``1.1.0rc1``
 
 
 `Simple Mail Transfer Protocol (SMTP) <https://tools.ietf.org/html/rfc5321>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``smtp`` provider. All classes for this provider package
 are in ``airflow.providers.smtp`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-smtp/1.0.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-smtp/1.1.0/>`_.
 
 
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
 ==================  ==================
 
  .. Licensed to the Apache Software Foundation (ASF) under one
     or more contributor license agreements.  See the NOTICE file
     distributed with this work for additional information
     regarding copyright ownership.  The ASF licenses this file
     to you under the Apache License, Version 2.0 (the
@@ -108,14 +108,30 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+1.1.0
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
+
 1.0.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
 
 * ``'EmailOperator': fix wrong assignment of 'from_email' (#30524)``
```

### Comparing `apache-airflow-providers-smtp-1.0.1rc1/apache_airflow_providers_smtp.egg-info/SOURCES.txt` & `apache-airflow-providers-smtp-1.1.0rc1/apache_airflow_providers_smtp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-smtp-1.0.1rc1/pyproject.toml` & `apache-airflow-providers-smtp-1.1.0rc1/pyproject.toml`

 * *Files 2% similar despite different names*

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
```

### Comparing `apache-airflow-providers-smtp-1.0.1rc1/setup.cfg` & `apache-airflow-providers-smtp-1.1.0rc1/setup.cfg`

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-smtp/1.0.1/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-smtp/1.1.0/
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
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.smtp.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.smtp
```

### Comparing `apache-airflow-providers-smtp-1.0.1rc1/setup.py` & `apache-airflow-providers-smtp-1.1.0rc1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-smtp package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "1.0.1"
+version = "1.1.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-smtp setup."""
     setup(
         version=version,
         extras_require={},
```

