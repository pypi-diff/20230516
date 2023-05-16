# Comparing `tmp/apache-airflow-providers-apache-drill-2.3.2rc1.tar.gz` & `tmp/apache-airflow-providers-apache-drill-2.4.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-apache-drill-2.3.2rc1.tar", last modified: Sun Apr  2 05:46:57 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-apache-drill-2.4.0rc1.tar", last modified: Tue May 16 15:52:56 2023, max compression
```

## Comparing `apache-airflow-providers-apache-drill-2.3.2rc1.tar` & `apache-airflow-providers-apache-drill-2.4.0rc1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:46:57.000000 apache-airflow-providers-apache-drill-2.3.2rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-drill-2.3.2rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1122 2023-04-02 05:46:55.000000 apache-airflow-providers-apache-drill-2.3.2rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-drill-2.3.2rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    10086 2023-04-02 05:46:57.000000 apache-airflow-providers-apache-drill-2.3.2rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8514 2023-04-02 05:46:55.000000 apache-airflow-providers-apache-drill-2.3.2rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:46:57.000000 apache-airflow-providers-apache-drill-2.3.2rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:46:57.000000 apache-airflow-providers-apache-drill-2.3.2rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:46:57.000000 apache-airflow-providers-apache-drill-2.3.2rc1/airflow/providers/apache/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:46:57.000000 apache-airflow-providers-apache-drill-2.3.2rc1/airflow/providers/apache/drill/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-drill-2.3.2rc1/airflow/providers/apache/drill/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2666 2023-04-02 05:46:55.000000 apache-airflow-providers-apache-drill-2.3.2rc1/airflow/providers/apache/drill/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:46:57.000000 apache-airflow-providers-apache-drill-2.3.2rc1/airflow/providers/apache/drill/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-drill-2.3.2rc1/airflow/providers/apache/drill/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3659 2023-03-27 08:32:48.000000 apache-airflow-providers-apache-drill-2.3.2rc1/airflow/providers/apache/drill/hooks/drill.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:46:57.000000 apache-airflow-providers-apache-drill-2.3.2rc1/airflow/providers/apache/drill/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-drill-2.3.2rc1/airflow/providers/apache/drill/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2142 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-drill-2.3.2rc1/airflow/providers/apache/drill/operators/drill.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 05:46:57.000000 apache-airflow-providers-apache-drill-2.3.2rc1/apache_airflow_providers_apache_drill.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10086 2023-04-02 05:46:56.000000 apache-airflow-providers-apache-drill-2.3.2rc1/apache_airflow_providers_apache_drill.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      792 2023-04-02 05:46:57.000000 apache-airflow-providers-apache-drill-2.3.2rc1/apache_airflow_providers_apache_drill.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-02 05:46:57.000000 apache-airflow-providers-apache-drill-2.3.2rc1/apache_airflow_providers_apache_drill.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      109 2023-04-02 05:46:57.000000 apache-airflow-providers-apache-drill-2.3.2rc1/apache_airflow_providers_apache_drill.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-02 05:46:56.000000 apache-airflow-providers-apache-drill-2.3.2rc1/apache_airflow_providers_apache_drill.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      149 2023-04-02 05:46:57.000000 apache-airflow-providers-apache-drill-2.3.2rc1/apache_airflow_providers_apache_drill.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-02 05:46:57.000000 apache-airflow-providers-apache-drill-2.3.2rc1/apache_airflow_providers_apache_drill.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5393 2023-04-01 16:40:04.000000 apache-airflow-providers-apache-drill-2.3.2rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1938 2023-04-02 05:46:57.000000 apache-airflow-providers-apache-drill-2.3.2rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1563 2023-04-02 05:46:55.000000 apache-airflow-providers-apache-drill-2.3.2rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:56.000000 apache-airflow-providers-apache-drill-2.4.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-drill-2.4.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-05-16 15:52:55.000000 apache-airflow-providers-apache-drill-2.4.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-drill-2.4.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    10900 2023-05-16 15:52:56.000000 apache-airflow-providers-apache-drill-2.4.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9328 2023-05-16 15:52:55.000000 apache-airflow-providers-apache-drill-2.4.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:56.000000 apache-airflow-providers-apache-drill-2.4.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:56.000000 apache-airflow-providers-apache-drill-2.4.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:56.000000 apache-airflow-providers-apache-drill-2.4.0rc1/airflow/providers/apache/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:56.000000 apache-airflow-providers-apache-drill-2.4.0rc1/airflow/providers/apache/drill/
+-rw-r--r--   0 root         (0) root         (0)     1395 2023-05-16 15:39:21.000000 apache-airflow-providers-apache-drill-2.4.0rc1/airflow/providers/apache/drill/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2715 2023-05-16 15:52:55.000000 apache-airflow-providers-apache-drill-2.4.0rc1/airflow/providers/apache/drill/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:56.000000 apache-airflow-providers-apache-drill-2.4.0rc1/airflow/providers/apache/drill/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-drill-2.4.0rc1/airflow/providers/apache/drill/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3659 2023-03-27 08:32:48.000000 apache-airflow-providers-apache-drill-2.4.0rc1/airflow/providers/apache/drill/hooks/drill.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:56.000000 apache-airflow-providers-apache-drill-2.4.0rc1/airflow/providers/apache/drill/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-drill-2.4.0rc1/airflow/providers/apache/drill/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2222 2023-05-03 19:47:07.000000 apache-airflow-providers-apache-drill-2.4.0rc1/airflow/providers/apache/drill/operators/drill.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:52:56.000000 apache-airflow-providers-apache-drill-2.4.0rc1/apache_airflow_providers_apache_drill.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10900 2023-05-16 15:52:56.000000 apache-airflow-providers-apache-drill-2.4.0rc1/apache_airflow_providers_apache_drill.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      792 2023-05-16 15:52:56.000000 apache-airflow-providers-apache-drill-2.4.0rc1/apache_airflow_providers_apache_drill.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:52:56.000000 apache-airflow-providers-apache-drill-2.4.0rc1/apache_airflow_providers_apache_drill.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2023-05-16 15:52:56.000000 apache-airflow-providers-apache-drill-2.4.0rc1/apache_airflow_providers_apache_drill.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:52:56.000000 apache-airflow-providers-apache-drill-2.4.0rc1/apache_airflow_providers_apache_drill.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      149 2023-05-16 15:52:56.000000 apache-airflow-providers-apache-drill-2.4.0rc1/apache_airflow_providers_apache_drill.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-16 15:52:56.000000 apache-airflow-providers-apache-drill-2.4.0rc1/apache_airflow_providers_apache_drill.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5308 2023-05-15 09:39:26.000000 apache-airflow-providers-apache-drill-2.4.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1938 2023-05-16 15:52:56.000000 apache-airflow-providers-apache-drill-2.4.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1727 2023-05-16 15:52:55.000000 apache-airflow-providers-apache-drill-2.4.0rc1/setup.py
```

### Comparing `apache-airflow-providers-apache-drill-2.3.2rc1/LICENSE` & `apache-airflow-providers-apache-drill-2.4.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-drill-2.3.2rc1/MANIFEST.in` & `apache-airflow-providers-apache-drill-2.4.0rc1/MANIFEST.in`

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

### Comparing `apache-airflow-providers-apache-drill-2.3.2rc1/PKG-INFO` & `apache-airflow-providers-apache-drill-2.4.0rc1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-drill
-Version: 2.3.2rc1
+Version: 2.4.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-drill package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-drill/2.3.2/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-drill/2.4.0/
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
 
 
 Package ``apache-airflow-providers-apache-drill``
 
-Release: ``2.3.2rc1``
+Release: ``2.4.0rc1``
 
 
 `Apache Drill <https://drill.apache.org/>`__.
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.drill`` provider. All classes for this provider package
 are in ``airflow.providers.apache.drill`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-drill/2.3.2/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-drill/2.4.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -80,15 +80,15 @@
 
 Requirements
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
-``apache-airflow``                       ``>=2.3.0``
+``apache-airflow``                       ``>=2.4.0``
 ``apache-airflow-providers-common-sql``  ``>=1.3.1``
 ``sqlalchemy-drill``                     ``>=1.1.0``
 =======================================  ==================
 
 Cross provider package dependencies
 -----------------------------------
 
@@ -130,14 +130,32 @@
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
+   * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add mechanism to suspend providers (#30422)``
+
 2.3.2
 .....
 
 Bug Fixes
 ~~~~~~~~~
 
 * ``Sanitize host in drill hook (#30215)``
@@ -153,16 +171,17 @@
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Prepare for follow-up release for November providers (#27774)``
 
 2.3.0
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
@@ -210,16 +229,17 @@
 
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
    * ``AIP-47 - Migrate drill DAGs to new design #22439 (#24206)``
    * ``Prepare provider documentation 2022.05.11 (#23631)``
    * ``Clean up in-line f-string concatenation (#23591)``
```

### Comparing `apache-airflow-providers-apache-drill-2.3.2rc1/README.rst` & `apache-airflow-providers-apache-drill-2.4.0rc1/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -15,28 +15,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-drill``
 
-Release: ``2.3.2rc1``
+Release: ``2.4.0rc1``
 
 
 `Apache Drill <https://drill.apache.org/>`__.
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.drill`` provider. All classes for this provider package
 are in ``airflow.providers.apache.drill`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-drill/2.3.2/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-drill/2.4.0/>`_.
 
 
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
 ``sqlalchemy-drill``                     ``>=1.1.0``
 =======================================  ==================
 
 Cross provider package dependencies
 -----------------------------------
 
@@ -96,14 +96,32 @@
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
+   * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add mechanism to suspend providers (#30422)``
+
 2.3.2
 .....
 
 Bug Fixes
 ~~~~~~~~~
 
 * ``Sanitize host in drill hook (#30215)``
@@ -119,16 +137,17 @@
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Prepare for follow-up release for November providers (#27774)``
 
 2.3.0
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
@@ -176,16 +195,17 @@
 
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
    * ``AIP-47 - Migrate drill DAGs to new design #22439 (#24206)``
    * ``Prepare provider documentation 2022.05.11 (#23631)``
    * ``Clean up in-line f-string concatenation (#23591)``
```

### Comparing `apache-airflow-providers-apache-drill-2.3.2rc1/airflow/providers/apache/drill/__init__.py` & `apache-airflow-providers-apache-drill-2.4.0rc1/airflow/providers/apache/drill/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-drill-2.3.2rc1/airflow/providers/apache/drill/get_provider_info.py` & `apache-airflow-providers-apache-drill-2.4.0rc1/airflow/providers/apache/drill/get_provider_info.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,30 +23,32 @@
 
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-apache-drill",
         "name": "Apache Drill",
         "description": "`Apache Drill <https://drill.apache.org/>`__.\n",
+        "suspended": False,
         "versions": [
+            "2.4.0",
             "2.3.2",
             "2.3.1",
             "2.3.0",
             "2.2.1",
             "2.2.0",
             "2.1.0",
             "2.0.0",
             "1.0.4",
             "1.0.3",
             "1.0.2",
             "1.0.1",
             "1.0.0",
         ],
         "dependencies": [
-            "apache-airflow>=2.3.0",
+            "apache-airflow>=2.4.0",
             "apache-airflow-providers-common-sql>=1.3.1",
             "sqlalchemy-drill>=1.1.0",
         ],
         "integrations": [
             {
                 "integration-name": "Apache Drill",
                 "external-doc-url": "https://drill.apache.org/",
```

### Comparing `apache-airflow-providers-apache-drill-2.3.2rc1/airflow/providers/apache/drill/hooks/__init__.py` & `apache-airflow-providers-apache-drill-2.4.0rc1/airflow/providers/apache/drill/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-drill-2.3.2rc1/airflow/providers/apache/drill/hooks/drill.py` & `apache-airflow-providers-apache-drill-2.4.0rc1/airflow/providers/apache/drill/hooks/drill.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-drill-2.3.2rc1/airflow/providers/apache/drill/operators/drill.py` & `apache-airflow-providers-apache-drill-2.4.0rc1/airflow/providers/apache/drill/operators/drill.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
 import warnings
 from typing import Sequence
 
+from airflow.exceptions import AirflowProviderDeprecationWarning
 from airflow.providers.common.sql.operators.sql import SQLExecuteQueryOperator
 
 
 class DrillOperator(SQLExecuteQueryOperator):
     """
     Executes the provided SQL in the identified Drill environment.
 
@@ -45,10 +46,10 @@
     ui_color = "#ededed"
 
     def __init__(self, *, drill_conn_id: str = "drill_default", **kwargs) -> None:
         super().__init__(conn_id=drill_conn_id, **kwargs)
         warnings.warn(
             """This class is deprecated.
             Please use `airflow.providers.common.sql.operators.sql.SQLExecuteQueryOperator`.""",
-            DeprecationWarning,
+            AirflowProviderDeprecationWarning,
             stacklevel=2,
         )
```

### Comparing `apache-airflow-providers-apache-drill-2.3.2rc1/apache_airflow_providers_apache_drill.egg-info/PKG-INFO` & `apache-airflow-providers-apache-drill-2.4.0rc1/apache_airflow_providers_apache_drill.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-drill
-Version: 2.3.2rc1
+Version: 2.4.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-drill package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-drill/2.3.2/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-drill/2.4.0/
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
 
 
 Package ``apache-airflow-providers-apache-drill``
 
-Release: ``2.3.2rc1``
+Release: ``2.4.0rc1``
 
 
 `Apache Drill <https://drill.apache.org/>`__.
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.drill`` provider. All classes for this provider package
 are in ``airflow.providers.apache.drill`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-drill/2.3.2/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-drill/2.4.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -80,15 +80,15 @@
 
 Requirements
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
-``apache-airflow``                       ``>=2.3.0``
+``apache-airflow``                       ``>=2.4.0``
 ``apache-airflow-providers-common-sql``  ``>=1.3.1``
 ``sqlalchemy-drill``                     ``>=1.1.0``
 =======================================  ==================
 
 Cross provider package dependencies
 -----------------------------------
 
@@ -130,14 +130,32 @@
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
+   * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add mechanism to suspend providers (#30422)``
+
 2.3.2
 .....
 
 Bug Fixes
 ~~~~~~~~~
 
 * ``Sanitize host in drill hook (#30215)``
@@ -153,16 +171,17 @@
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Prepare for follow-up release for November providers (#27774)``
 
 2.3.0
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
@@ -210,16 +229,17 @@
 
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
    * ``AIP-47 - Migrate drill DAGs to new design #22439 (#24206)``
    * ``Prepare provider documentation 2022.05.11 (#23631)``
    * ``Clean up in-line f-string concatenation (#23591)``
```

### Comparing `apache-airflow-providers-apache-drill-2.3.2rc1/apache_airflow_providers_apache_drill.egg-info/SOURCES.txt` & `apache-airflow-providers-apache-drill-2.4.0rc1/apache_airflow_providers_apache_drill.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-drill-2.3.2rc1/pyproject.toml` & `apache-airflow-providers-apache-drill-2.4.0rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-apache-drill-2.3.2rc1/setup.cfg` & `apache-airflow-providers-apache-drill-2.4.0rc1/setup.cfg`

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-apache-drill/2.3.2/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-apache-drill/2.4.0/
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
 	apache-airflow-providers-common-sql>=1.3.1.dev0
-	apache-airflow>=2.3.0.dev0
+	apache-airflow>=2.4.0.dev0
 	sqlalchemy-drill>=1.1.0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.apache.drill.get_provider_info:get_provider_info
 
 [files]
```

### Comparing `apache-airflow-providers-apache-drill-2.3.2rc1/setup.py` & `apache-airflow-providers-apache-drill-2.4.0rc1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,23 +22,28 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-apache-drill package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "2.3.2"
+version = "2.4.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-apache-drill setup."""
     setup(
         version=version,
         extras_require={"common.sql": ["apache-airflow-providers-common-sql"]},
         packages=find_namespace_packages(
-            include=["airflow.providers.apache.drill", "airflow.providers.apache.drill.*"]
+            include=[
+                "airflow.providers.apache.drill",
+                "airflow.providers.apache.drill.*",
+                "airflow.providers.apache.drill_vendor",
+                "airflow.providers.apache.drill_vendor.*",
+            ],
         ),
     )
 
 
 if __name__ == "__main__":
     do_setup()
```

