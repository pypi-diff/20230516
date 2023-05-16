# Comparing `tmp/apache-airflow-providers-apache-beam-5.0.0rc1.tar.gz` & `tmp/apache-airflow-providers-apache-beam-5.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-apache-beam-5.0.0rc1.tar", last modified: Fri Apr 21 19:47:56 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-apache-beam-5.1.0rc1.tar", last modified: Tue May 16 15:52:53 2023, max compression
```

## Comparing `apache-airflow-providers-apache-beam-5.0.0rc1.tar` & `apache-airflow-providers-apache-beam-5.1.0rc1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:47:56.000000 apache-airflow-providers-apache-beam-5.0.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-beam-5.0.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-04-21 19:47:54.000000 apache-airflow-providers-apache-beam-5.0.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-beam-5.0.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    14551 2023-04-21 19:47:56.000000 apache-airflow-providers-apache-beam-5.0.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12986 2023-04-21 19:47:54.000000 apache-airflow-providers-apache-beam-5.0.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:47:56.000000 apache-airflow-providers-apache-beam-5.0.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:47:56.000000 apache-airflow-providers-apache-beam-5.0.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:47:56.000000 apache-airflow-providers-apache-beam-5.0.0rc1/airflow/providers/apache/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:47:56.000000 apache-airflow-providers-apache-beam-5.0.0rc1/airflow/providers/apache/beam/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-beam-5.0.0rc1/airflow/providers/apache/beam/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2490 2023-04-21 19:47:54.000000 apache-airflow-providers-apache-beam-5.0.0rc1/airflow/providers/apache/beam/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:47:56.000000 apache-airflow-providers-apache-beam-5.0.0rc1/airflow/providers/apache/beam/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-beam-5.0.0rc1/airflow/providers/apache/beam/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14199 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-beam-5.0.0rc1/airflow/providers/apache/beam/hooks/beam.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:47:56.000000 apache-airflow-providers-apache-beam-5.0.0rc1/airflow/providers/apache/beam/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-beam-5.0.0rc1/airflow/providers/apache/beam/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32492 2023-04-21 10:05:41.000000 apache-airflow-providers-apache-beam-5.0.0rc1/airflow/providers/apache/beam/operators/beam.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:47:56.000000 apache-airflow-providers-apache-beam-5.0.0rc1/apache_airflow_providers_apache_beam.egg-info/
--rw-r--r--   0 root         (0) root         (0)    14551 2023-04-21 19:47:56.000000 apache-airflow-providers-apache-beam-5.0.0rc1/apache_airflow_providers_apache_beam.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      777 2023-04-21 19:47:56.000000 apache-airflow-providers-apache-beam-5.0.0rc1/apache_airflow_providers_apache_beam.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:47:56.000000 apache-airflow-providers-apache-beam-5.0.0rc1/apache_airflow_providers_apache_beam.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      108 2023-04-21 19:47:56.000000 apache-airflow-providers-apache-beam-5.0.0rc1/apache_airflow_providers_apache_beam.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:47:56.000000 apache-airflow-providers-apache-beam-5.0.0rc1/apache_airflow_providers_apache_beam.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      106 2023-04-21 19:47:56.000000 apache-airflow-providers-apache-beam-5.0.0rc1/apache_airflow_providers_apache_beam.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-21 19:47:56.000000 apache-airflow-providers-apache-beam-5.0.0rc1/apache_airflow_providers_apache_beam.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5246 2023-04-07 12:28:58.000000 apache-airflow-providers-apache-beam-5.0.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1879 2023-04-21 19:47:56.000000 apache-airflow-providers-apache-beam-5.0.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1733 2023-04-21 19:47:54.000000 apache-airflow-providers-apache-beam-5.0.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:53.000000 apache-airflow-providers-apache-beam-5.1.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-beam-5.1.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-05-16 15:52:52.000000 apache-airflow-providers-apache-beam-5.1.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-beam-5.1.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    15241 2023-05-16 15:52:53.000000 apache-airflow-providers-apache-beam-5.1.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    13676 2023-05-16 15:52:52.000000 apache-airflow-providers-apache-beam-5.1.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:53.000000 apache-airflow-providers-apache-beam-5.1.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:53.000000 apache-airflow-providers-apache-beam-5.1.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:53.000000 apache-airflow-providers-apache-beam-5.1.0rc1/airflow/providers/apache/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:53.000000 apache-airflow-providers-apache-beam-5.1.0rc1/airflow/providers/apache/beam/
+-rw-r--r--   0 root         (0) root         (0)     1394 2023-05-16 15:39:21.000000 apache-airflow-providers-apache-beam-5.1.0rc1/airflow/providers/apache/beam/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2511 2023-05-16 15:52:52.000000 apache-airflow-providers-apache-beam-5.1.0rc1/airflow/providers/apache/beam/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:53.000000 apache-airflow-providers-apache-beam-5.1.0rc1/airflow/providers/apache/beam/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-beam-5.1.0rc1/airflow/providers/apache/beam/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14199 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-beam-5.1.0rc1/airflow/providers/apache/beam/hooks/beam.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:53.000000 apache-airflow-providers-apache-beam-5.1.0rc1/airflow/providers/apache/beam/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-beam-5.1.0rc1/airflow/providers/apache/beam/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32492 2023-04-21 10:05:41.000000 apache-airflow-providers-apache-beam-5.1.0rc1/airflow/providers/apache/beam/operators/beam.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:53.000000 apache-airflow-providers-apache-beam-5.1.0rc1/apache_airflow_providers_apache_beam.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15241 2023-05-16 15:52:53.000000 apache-airflow-providers-apache-beam-5.1.0rc1/apache_airflow_providers_apache_beam.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      777 2023-05-16 15:52:53.000000 apache-airflow-providers-apache-beam-5.1.0rc1/apache_airflow_providers_apache_beam.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:52:53.000000 apache-airflow-providers-apache-beam-5.1.0rc1/apache_airflow_providers_apache_beam.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      108 2023-05-16 15:52:53.000000 apache-airflow-providers-apache-beam-5.1.0rc1/apache_airflow_providers_apache_beam.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:52:53.000000 apache-airflow-providers-apache-beam-5.1.0rc1/apache_airflow_providers_apache_beam.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      106 2023-05-16 15:52:53.000000 apache-airflow-providers-apache-beam-5.1.0rc1/apache_airflow_providers_apache_beam.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-16 15:52:53.000000 apache-airflow-providers-apache-beam-5.1.0rc1/apache_airflow_providers_apache_beam.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5308 2023-05-15 09:39:26.000000 apache-airflow-providers-apache-beam-5.1.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1879 2023-05-16 15:52:53.000000 apache-airflow-providers-apache-beam-5.1.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1733 2023-05-16 15:52:52.000000 apache-airflow-providers-apache-beam-5.1.0rc1/setup.py
```

### Comparing `apache-airflow-providers-apache-beam-5.0.0rc1/LICENSE` & `apache-airflow-providers-apache-beam-5.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-beam-5.0.0rc1/MANIFEST.in` & `apache-airflow-providers-apache-beam-5.1.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-beam-5.0.0rc1/PKG-INFO` & `apache-airflow-providers-apache-beam-5.1.0rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-beam
-Version: 5.0.0rc1
+Version: 5.1.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-beam package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-beam/5.0.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-beam/5.1.0/
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
 
 
 Package ``apache-airflow-providers-apache-beam``
 
-Release: ``5.0.0rc1``
+Release: ``5.1.0rc1``
 
 
 `Apache Beam <https://beam.apache.org/>`__.
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.beam`` provider. All classes for this provider package
 are in ``airflow.providers.apache.beam`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-beam/5.0.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-beam/5.1.0/>`_.
 
 
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
 ``apache-beam``     ``>=2.33.0``
 ==================  ==================
 
 Cross provider package dependencies
 -----------------------------------
 
 Those are dependencies that might be needed in order to use all the features of the package.
@@ -129,14 +129,30 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+5.1.0
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
 5.0.0
 ......
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
 .. warning::
@@ -177,16 +193,17 @@
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
 
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
 
 Features
@@ -206,16 +223,17 @@
 
 4.0.0
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
 
 * ``Added missing project_id to the wait_for_job (#24020)``
 * ``Support impersonation service account parameter for Dataflow runner (#23961)``
```

### Comparing `apache-airflow-providers-apache-beam-5.0.0rc1/README.rst` & `apache-airflow-providers-apache-beam-5.1.0rc1/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -15,28 +15,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-beam``
 
-Release: ``5.0.0rc1``
+Release: ``5.1.0rc1``
 
 
 `Apache Beam <https://beam.apache.org/>`__.
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.beam`` provider. All classes for this provider package
 are in ``airflow.providers.apache.beam`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-beam/5.0.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-beam/5.1.0/>`_.
 
 
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
 ``apache-beam``     ``>=2.33.0``
 ==================  ==================
 
 Cross provider package dependencies
 -----------------------------------
 
 Those are dependencies that might be needed in order to use all the features of the package.
@@ -95,14 +95,30 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+5.1.0
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
 5.0.0
 ......
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
 .. warning::
@@ -143,16 +159,17 @@
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
 
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
 
 Features
@@ -172,16 +189,17 @@
 
 4.0.0
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
 
 * ``Added missing project_id to the wait_for_job (#24020)``
 * ``Support impersonation service account parameter for Dataflow runner (#23961)``
```

### Comparing `apache-airflow-providers-apache-beam-5.0.0rc1/airflow/providers/apache/beam/__init__.py` & `apache-airflow-providers-apache-beam-5.1.0rc1/airflow/providers/apache/beam/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-beam-5.0.0rc1/airflow/providers/apache/beam/get_provider_info.py` & `apache-airflow-providers-apache-beam-5.1.0rc1/airflow/providers/apache/beam/get_provider_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-apache-beam",
         "name": "Apache Beam",
         "description": "`Apache Beam <https://beam.apache.org/>`__.\n",
         "suspended": False,
         "versions": [
+            "5.1.0",
             "5.0.0",
             "4.3.0",
             "4.2.0",
             "4.1.1",
             "4.1.0",
             "4.0.0",
             "3.4.0",
@@ -42,15 +43,15 @@
             "3.1.0",
             "3.0.1",
             "3.0.0",
             "2.0.0",
             "1.0.1",
             "1.0.0",
         ],
-        "dependencies": ["apache-airflow>=2.3.0", "apache-beam>=2.33.0"],
+        "dependencies": ["apache-airflow>=2.4.0", "apache-beam>=2.33.0"],
         "integrations": [
             {
                 "integration-name": "Apache Beam",
                 "external-doc-url": "https://beam.apache.org/",
                 "how-to-guide": ["/docs/apache-airflow-providers-apache-beam/operators.rst"],
                 "tags": ["apache"],
             }
```

### Comparing `apache-airflow-providers-apache-beam-5.0.0rc1/airflow/providers/apache/beam/hooks/__init__.py` & `apache-airflow-providers-apache-beam-5.1.0rc1/airflow/providers/apache/beam/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-beam-5.0.0rc1/airflow/providers/apache/beam/hooks/beam.py` & `apache-airflow-providers-apache-beam-5.1.0rc1/airflow/providers/apache/beam/hooks/beam.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-beam-5.0.0rc1/airflow/providers/apache/beam/operators/beam.py` & `apache-airflow-providers-apache-beam-5.1.0rc1/airflow/providers/apache/beam/operators/beam.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-beam-5.0.0rc1/apache_airflow_providers_apache_beam.egg-info/PKG-INFO` & `apache-airflow-providers-apache-beam-5.1.0rc1/apache_airflow_providers_apache_beam.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-beam
-Version: 5.0.0rc1
+Version: 5.1.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-beam package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-beam/5.0.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-beam/5.1.0/
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
 
 
 Package ``apache-airflow-providers-apache-beam``
 
-Release: ``5.0.0rc1``
+Release: ``5.1.0rc1``
 
 
 `Apache Beam <https://beam.apache.org/>`__.
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.beam`` provider. All classes for this provider package
 are in ``airflow.providers.apache.beam`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-beam/5.0.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-beam/5.1.0/>`_.
 
 
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
 ``apache-beam``     ``>=2.33.0``
 ==================  ==================
 
 Cross provider package dependencies
 -----------------------------------
 
 Those are dependencies that might be needed in order to use all the features of the package.
@@ -129,14 +129,30 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+5.1.0
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
 5.0.0
 ......
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
 .. warning::
@@ -177,16 +193,17 @@
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
 
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
 
 Features
@@ -206,16 +223,17 @@
 
 4.0.0
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
 
 * ``Added missing project_id to the wait_for_job (#24020)``
 * ``Support impersonation service account parameter for Dataflow runner (#23961)``
```

### Comparing `apache-airflow-providers-apache-beam-5.0.0rc1/apache_airflow_providers_apache_beam.egg-info/SOURCES.txt` & `apache-airflow-providers-apache-beam-5.1.0rc1/apache_airflow_providers_apache_beam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-beam-5.0.0rc1/pyproject.toml` & `apache-airflow-providers-apache-beam-5.1.0rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-apache-beam-5.0.0rc1/setup.cfg` & `apache-airflow-providers-apache-beam-5.1.0rc1/setup.cfg`

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-apache-beam/5.0.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-apache-beam/5.1.0/
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
 	apache-beam>=2.33.0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.apache.beam.get_provider_info:get_provider_info
 
 [files]
```

### Comparing `apache-airflow-providers-apache-beam-5.0.0rc1/setup.py` & `apache-airflow-providers-apache-beam-5.1.0rc1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-apache-beam package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "5.0.0"
+version = "5.1.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-apache-beam setup."""
     setup(
         version=version,
         extras_require={"google": ["apache-airflow-providers-google", "apache-beam[gcp]"]},
```

