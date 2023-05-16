# Comparing `tmp/apache-airflow-providers-apache-flink-1.0.1rc1.tar.gz` & `tmp/apache-airflow-providers-apache-flink-1.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-apache-flink-1.0.1rc1.tar", last modified: Fri Mar  3 13:46:36 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-apache-flink-1.1.0rc1.tar", last modified: Tue May 16 15:53:00 2023, max compression
```

## Comparing `apache-airflow-providers-apache-flink-1.0.1rc1.tar` & `apache-airflow-providers-apache-flink-1.1.0rc1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 13:46:36.000000 apache-airflow-providers-apache-flink-1.0.1rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-flink-1.0.1rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1122 2023-03-03 13:46:34.000000 apache-airflow-providers-apache-flink-1.0.1rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-flink-1.0.1rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     6272 2023-03-03 13:46:36.000000 apache-airflow-providers-apache-flink-1.0.1rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4675 2023-03-03 13:46:34.000000 apache-airflow-providers-apache-flink-1.0.1rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 13:46:35.000000 apache-airflow-providers-apache-flink-1.0.1rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 13:46:35.000000 apache-airflow-providers-apache-flink-1.0.1rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 13:46:35.000000 apache-airflow-providers-apache-flink-1.0.1rc1/airflow/providers/apache/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 13:46:35.000000 apache-airflow-providers-apache-flink-1.0.1rc1/airflow/providers/apache/flink/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-flink-1.0.1rc1/airflow/providers/apache/flink/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2278 2023-03-03 13:46:34.000000 apache-airflow-providers-apache-flink-1.0.1rc1/airflow/providers/apache/flink/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 13:46:35.000000 apache-airflow-providers-apache-flink-1.0.1rc1/airflow/providers/apache/flink/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-flink-1.0.1rc1/airflow/providers/apache/flink/hooks/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 13:46:35.000000 apache-airflow-providers-apache-flink-1.0.1rc1/airflow/providers/apache/flink/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-flink-1.0.1rc1/airflow/providers/apache/flink/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4613 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-flink-1.0.1rc1/airflow/providers/apache/flink/operators/flink_kubernetes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 13:46:36.000000 apache-airflow-providers-apache-flink-1.0.1rc1/airflow/providers/apache/flink/sensors/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-flink-1.0.1rc1/airflow/providers/apache/flink/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5714 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-flink-1.0.1rc1/airflow/providers/apache/flink/sensors/flink_kubernetes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 13:46:36.000000 apache-airflow-providers-apache-flink-1.0.1rc1/apache_airflow_providers_apache_flink.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6272 2023-03-03 13:46:35.000000 apache-airflow-providers-apache-flink-1.0.1rc1/apache_airflow_providers_apache_flink.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      867 2023-03-03 13:46:35.000000 apache-airflow-providers-apache-flink-1.0.1rc1/apache_airflow_providers_apache_flink.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-03 13:46:35.000000 apache-airflow-providers-apache-flink-1.0.1rc1/apache_airflow_providers_apache_flink.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      110 2023-03-03 13:46:35.000000 apache-airflow-providers-apache-flink-1.0.1rc1/apache_airflow_providers_apache_flink.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-03 13:46:35.000000 apache-airflow-providers-apache-flink-1.0.1rc1/apache_airflow_providers_apache_flink.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      160 2023-03-03 13:46:35.000000 apache-airflow-providers-apache-flink-1.0.1rc1/apache_airflow_providers_apache_flink.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-03-03 13:46:35.000000 apache-airflow-providers-apache-flink-1.0.1rc1/apache_airflow_providers_apache_flink.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     3814 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-flink-1.0.1rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1939 2023-03-03 13:46:36.000000 apache-airflow-providers-apache-flink-1.0.1rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1573 2023-03-03 13:46:34.000000 apache-airflow-providers-apache-flink-1.0.1rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:00.000000 apache-airflow-providers-apache-flink-1.1.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-flink-1.1.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-05-16 15:52:59.000000 apache-airflow-providers-apache-flink-1.1.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-flink-1.1.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     6863 2023-05-16 15:53:00.000000 apache-airflow-providers-apache-flink-1.1.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5286 2023-05-16 15:52:59.000000 apache-airflow-providers-apache-flink-1.1.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:00.000000 apache-airflow-providers-apache-flink-1.1.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:00.000000 apache-airflow-providers-apache-flink-1.1.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:00.000000 apache-airflow-providers-apache-flink-1.1.0rc1/airflow/providers/apache/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:00.000000 apache-airflow-providers-apache-flink-1.1.0rc1/airflow/providers/apache/flink/
+-rw-r--r--   0 root         (0) root         (0)     1395 2023-05-16 15:39:21.000000 apache-airflow-providers-apache-flink-1.1.0rc1/airflow/providers/apache/flink/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2315 2023-05-16 15:52:59.000000 apache-airflow-providers-apache-flink-1.1.0rc1/airflow/providers/apache/flink/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:00.000000 apache-airflow-providers-apache-flink-1.1.0rc1/airflow/providers/apache/flink/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-flink-1.1.0rc1/airflow/providers/apache/flink/hooks/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:00.000000 apache-airflow-providers-apache-flink-1.1.0rc1/airflow/providers/apache/flink/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-flink-1.1.0rc1/airflow/providers/apache/flink/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4613 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-flink-1.1.0rc1/airflow/providers/apache/flink/operators/flink_kubernetes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:00.000000 apache-airflow-providers-apache-flink-1.1.0rc1/airflow/providers/apache/flink/sensors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-flink-1.1.0rc1/airflow/providers/apache/flink/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5714 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-flink-1.1.0rc1/airflow/providers/apache/flink/sensors/flink_kubernetes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:00.000000 apache-airflow-providers-apache-flink-1.1.0rc1/apache_airflow_providers_apache_flink.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6863 2023-05-16 15:53:00.000000 apache-airflow-providers-apache-flink-1.1.0rc1/apache_airflow_providers_apache_flink.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      867 2023-05-16 15:53:00.000000 apache-airflow-providers-apache-flink-1.1.0rc1/apache_airflow_providers_apache_flink.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:53:00.000000 apache-airflow-providers-apache-flink-1.1.0rc1/apache_airflow_providers_apache_flink.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2023-05-16 15:53:00.000000 apache-airflow-providers-apache-flink-1.1.0rc1/apache_airflow_providers_apache_flink.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:53:00.000000 apache-airflow-providers-apache-flink-1.1.0rc1/apache_airflow_providers_apache_flink.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      160 2023-05-16 15:53:00.000000 apache-airflow-providers-apache-flink-1.1.0rc1/apache_airflow_providers_apache_flink.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-16 15:53:00.000000 apache-airflow-providers-apache-flink-1.1.0rc1/apache_airflow_providers_apache_flink.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5308 2023-05-15 09:39:26.000000 apache-airflow-providers-apache-flink-1.1.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1939 2023-05-16 15:53:00.000000 apache-airflow-providers-apache-flink-1.1.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1737 2023-05-16 15:52:59.000000 apache-airflow-providers-apache-flink-1.1.0rc1/setup.py
```

### Comparing `apache-airflow-providers-apache-flink-1.0.1rc1/LICENSE` & `apache-airflow-providers-apache-flink-1.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-flink-1.0.1rc1/MANIFEST.in` & `apache-airflow-providers-apache-flink-1.1.0rc1/MANIFEST.in`

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

### Comparing `apache-airflow-providers-apache-flink-1.0.1rc1/PKG-INFO` & `apache-airflow-providers-apache-flink-1.1.0rc1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-flink
-Version: 1.0.1rc1
+Version: 1.1.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-flink package
 Home-page: https://airflow.apache.org/
+Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Download-URL: https://archive.apache.org/dist/airflow/providers
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-flink/1.0.1/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-flink/1.1.0/
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
 
 
 Package ``apache-airflow-providers-apache-flink``
 
-Release: ``1.0.1rc1``
+Release: ``1.1.0rc1``
 
 
 `Apache Flink <https://flink.apache.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.flink`` provider. All classes for this provider package
 are in ``airflow.providers.apache.flink`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-flink/1.0.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-flink/1.1.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -81,15 +80,15 @@
 
 Requirements
 ------------
 
 ============================================  ==================
 PIP package                                   Version required
 ============================================  ==================
-``apache-airflow``                            ``>=2.3.0``
+``apache-airflow``                            ``>=2.4.0``
 ``cryptography``                              ``>=2.0.0``
 ``apache-airflow-providers-cncf-kubernetes``  ``>=5.1.0``
 ============================================  ==================
 
 Cross provider package dependencies
 -----------------------------------
 
@@ -131,14 +130,31 @@
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
+   * ``Add mechanism to suspend providers (#30422)``
+
 1.0.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
 
 * ``Make cncf.kubernetes required for flink provider (#29710)``
@@ -147,9 +163,7 @@
    appropriate section above if needed. Do not delete the lines(!):
    * ``Add more precise optional dependency to cncf.kubernetes from flink (#29707)``
 
 1.0.0
 .....
 
 Initial version of the Flink provider.
-
-
```

### Comparing `apache-airflow-providers-apache-flink-1.0.1rc1/README.rst` & `apache-airflow-providers-apache-flink-1.1.0rc1/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -15,28 +15,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-flink``
 
-Release: ``1.0.1rc1``
+Release: ``1.1.0rc1``
 
 
 `Apache Flink <https://flink.apache.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.flink`` provider. All classes for this provider package
 are in ``airflow.providers.apache.flink`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-flink/1.0.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-flink/1.1.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -46,15 +46,15 @@
 
 Requirements
 ------------
 
 ============================================  ==================
 PIP package                                   Version required
 ============================================  ==================
-``apache-airflow``                            ``>=2.3.0``
+``apache-airflow``                            ``>=2.4.0``
 ``cryptography``                              ``>=2.0.0``
 ``apache-airflow-providers-cncf-kubernetes``  ``>=5.1.0``
 ============================================  ==================
 
 Cross provider package dependencies
 -----------------------------------
 
@@ -96,14 +96,31 @@
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
+   * ``Add mechanism to suspend providers (#30422)``
+
 1.0.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
 
 * ``Make cncf.kubernetes required for flink provider (#29710)``
```

### Comparing `apache-airflow-providers-apache-flink-1.0.1rc1/airflow/providers/apache/flink/__init__.py` & `apache-airflow-providers-apache-flink-1.1.0rc1/airflow/providers/apache/flink/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-flink-1.0.1rc1/airflow/providers/apache/flink/get_provider_info.py` & `apache-airflow-providers-apache-flink-1.1.0rc1/airflow/providers/apache/flink/get_provider_info.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,17 +23,18 @@
 
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-apache-flink",
         "name": "Apache Flink",
         "description": "`Apache Flink <https://flink.apache.org/>`__\n",
-        "versions": ["1.0.1", "1.0.0"],
+        "suspended": False,
+        "versions": ["1.1.0", "1.0.1", "1.0.0"],
         "dependencies": [
-            "apache-airflow>=2.3.0",
+            "apache-airflow>=2.4.0",
             "cryptography>=2.0.0",
             "apache-airflow-providers-cncf-kubernetes>=5.1.0",
         ],
         "integrations": [
             {
                 "integration-name": "Apache Flink",
                 "external-doc-url": "https://github.com/apache/flink-kubernetes-operator",
```

### Comparing `apache-airflow-providers-apache-flink-1.0.1rc1/airflow/providers/apache/flink/hooks/__init__.py` & `apache-airflow-providers-apache-flink-1.1.0rc1/airflow/providers/apache/flink/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-flink-1.0.1rc1/airflow/providers/apache/flink/operators/__init__.py` & `apache-airflow-providers-apache-flink-1.1.0rc1/airflow/providers/apache/flink/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-flink-1.0.1rc1/airflow/providers/apache/flink/operators/flink_kubernetes.py` & `apache-airflow-providers-apache-flink-1.1.0rc1/airflow/providers/apache/flink/operators/flink_kubernetes.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-flink-1.0.1rc1/airflow/providers/apache/flink/sensors/flink_kubernetes.py` & `apache-airflow-providers-apache-flink-1.1.0rc1/airflow/providers/apache/flink/sensors/flink_kubernetes.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-flink-1.0.1rc1/apache_airflow_providers_apache_flink.egg-info/PKG-INFO` & `apache-airflow-providers-apache-flink-1.1.0rc1/apache_airflow_providers_apache_flink.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-flink
-Version: 1.0.1rc1
+Version: 1.1.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-flink package
 Home-page: https://airflow.apache.org/
+Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Download-URL: https://archive.apache.org/dist/airflow/providers
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-flink/1.0.1/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-flink/1.1.0/
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
 
 
 Package ``apache-airflow-providers-apache-flink``
 
-Release: ``1.0.1rc1``
+Release: ``1.1.0rc1``
 
 
 `Apache Flink <https://flink.apache.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.flink`` provider. All classes for this provider package
 are in ``airflow.providers.apache.flink`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-flink/1.0.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-flink/1.1.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -81,15 +80,15 @@
 
 Requirements
 ------------
 
 ============================================  ==================
 PIP package                                   Version required
 ============================================  ==================
-``apache-airflow``                            ``>=2.3.0``
+``apache-airflow``                            ``>=2.4.0``
 ``cryptography``                              ``>=2.0.0``
 ``apache-airflow-providers-cncf-kubernetes``  ``>=5.1.0``
 ============================================  ==================
 
 Cross provider package dependencies
 -----------------------------------
 
@@ -131,14 +130,31 @@
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
+   * ``Add mechanism to suspend providers (#30422)``
+
 1.0.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
 
 * ``Make cncf.kubernetes required for flink provider (#29710)``
@@ -147,9 +163,7 @@
    appropriate section above if needed. Do not delete the lines(!):
    * ``Add more precise optional dependency to cncf.kubernetes from flink (#29707)``
 
 1.0.0
 .....
 
 Initial version of the Flink provider.
-
-
```

### Comparing `apache-airflow-providers-apache-flink-1.0.1rc1/apache_airflow_providers_apache_flink.egg-info/SOURCES.txt` & `apache-airflow-providers-apache-flink-1.1.0rc1/apache_airflow_providers_apache_flink.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-flink-1.0.1rc1/pyproject.toml` & `apache-airflow-providers-apache-flink-1.1.0rc1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -28,28 +28,30 @@
 
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

### Comparing `apache-airflow-providers-apache-flink-1.0.1rc1/setup.cfg` & `apache-airflow-providers-apache-flink-1.1.0rc1/setup.cfg`

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-apache-flink/1.0.1/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-apache-flink/1.1.0/
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
 	apache-airflow-providers-cncf-kubernetes>=5.1.0.dev0
-	apache-airflow>=2.3.0.dev0
+	apache-airflow>=2.4.0.dev0
 	cryptography>=2.0.0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.apache.flink.get_provider_info:get_provider_info
 
 [files]
```

### Comparing `apache-airflow-providers-apache-flink-1.0.1rc1/setup.py` & `apache-airflow-providers-apache-flink-1.1.0rc1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,23 +22,28 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-apache-flink package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "1.0.1"
+version = "1.1.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-apache-flink setup."""
     setup(
         version=version,
         extras_require={"cncf.kubernetes": ["apache-airflow-providers-cncf-kubernetes"]},
         packages=find_namespace_packages(
-            include=["airflow.providers.apache.flink", "airflow.providers.apache.flink.*"]
+            include=[
+                "airflow.providers.apache.flink",
+                "airflow.providers.apache.flink.*",
+                "airflow.providers.apache.flink_vendor",
+                "airflow.providers.apache.flink_vendor.*",
+            ],
         ),
     )
 
 
 if __name__ == "__main__":
     do_setup()
```

