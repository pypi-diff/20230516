# Comparing `tmp/apache-airflow-providers-elasticsearch-4.4.0rc1.tar.gz` & `tmp/apache-airflow-providers-elasticsearch-4.5.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-elasticsearch-4.4.0rc1.tar", last modified: Wed Feb  8 08:28:02 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-elasticsearch-4.5.0rc1.tar", last modified: Tue May 16 15:53:45 2023, max compression
```

## Comparing `apache-airflow-providers-elasticsearch-4.4.0rc1.tar` & `apache-airflow-providers-elasticsearch-4.5.0rc1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 08:28:02.000000 apache-airflow-providers-elasticsearch-4.4.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2022-10-05 12:15:16.000000 apache-airflow-providers-elasticsearch-4.4.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1122 2023-02-08 08:28:00.000000 apache-airflow-providers-elasticsearch-4.4.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2022-10-05 12:15:16.000000 apache-airflow-providers-elasticsearch-4.4.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    14387 2023-02-08 08:28:02.000000 apache-airflow-providers-elasticsearch-4.4.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12792 2023-02-08 08:28:00.000000 apache-airflow-providers-elasticsearch-4.4.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 08:28:02.000000 apache-airflow-providers-elasticsearch-4.4.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 08:28:02.000000 apache-airflow-providers-elasticsearch-4.4.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 08:28:02.000000 apache-airflow-providers-elasticsearch-4.4.0rc1/airflow/providers/elasticsearch/
--rw-r--r--   0 root         (0) root         (0)      787 2022-10-05 12:15:15.000000 apache-airflow-providers-elasticsearch-4.4.0rc1/airflow/providers/elasticsearch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2847 2023-02-08 08:28:00.000000 apache-airflow-providers-elasticsearch-4.4.0rc1/airflow/providers/elasticsearch/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 08:28:02.000000 apache-airflow-providers-elasticsearch-4.4.0rc1/airflow/providers/elasticsearch/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2022-10-05 12:15:15.000000 apache-airflow-providers-elasticsearch-4.4.0rc1/airflow/providers/elasticsearch/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5408 2023-01-11 12:48:25.000000 apache-airflow-providers-elasticsearch-4.4.0rc1/airflow/providers/elasticsearch/hooks/elasticsearch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 08:28:02.000000 apache-airflow-providers-elasticsearch-4.4.0rc1/airflow/providers/elasticsearch/log/
--rw-r--r--   0 root         (0) root         (0)      785 2022-10-05 12:15:15.000000 apache-airflow-providers-elasticsearch-4.4.0rc1/airflow/providers/elasticsearch/log/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1808 2023-01-11 12:48:25.000000 apache-airflow-providers-elasticsearch-4.4.0rc1/airflow/providers/elasticsearch/log/es_json_formatter.py
--rw-r--r--   0 root         (0) root         (0)    17182 2023-02-05 09:48:53.000000 apache-airflow-providers-elasticsearch-4.4.0rc1/airflow/providers/elasticsearch/log/es_task_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-08 08:28:02.000000 apache-airflow-providers-elasticsearch-4.4.0rc1/apache_airflow_providers_elasticsearch.egg-info/
--rw-r--r--   0 root         (0) root         (0)    14387 2023-02-08 08:28:01.000000 apache-airflow-providers-elasticsearch-4.4.0rc1/apache_airflow_providers_elasticsearch.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      868 2023-02-08 08:28:01.000000 apache-airflow-providers-elasticsearch-4.4.0rc1/apache_airflow_providers_elasticsearch.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-08 08:28:01.000000 apache-airflow-providers-elasticsearch-4.4.0rc1/apache_airflow_providers_elasticsearch.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      111 2023-02-08 08:28:01.000000 apache-airflow-providers-elasticsearch-4.4.0rc1/apache_airflow_providers_elasticsearch.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-08 08:28:01.000000 apache-airflow-providers-elasticsearch-4.4.0rc1/apache_airflow_providers_elasticsearch.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      186 2023-02-08 08:28:01.000000 apache-airflow-providers-elasticsearch-4.4.0rc1/apache_airflow_providers_elasticsearch.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-02-08 08:28:01.000000 apache-airflow-providers-elasticsearch-4.4.0rc1/apache_airflow_providers_elasticsearch.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     3814 2023-01-13 19:37:41.000000 apache-airflow-providers-elasticsearch-4.4.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1983 2023-02-08 08:28:02.000000 apache-airflow-providers-elasticsearch-4.4.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1567 2023-02-08 08:28:00.000000 apache-airflow-providers-elasticsearch-4.4.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:45.000000 apache-airflow-providers-elasticsearch-4.5.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-elasticsearch-4.5.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-05-16 15:53:43.000000 apache-airflow-providers-elasticsearch-4.5.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-elasticsearch-4.5.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    15352 2023-05-16 15:53:45.000000 apache-airflow-providers-elasticsearch-4.5.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    13777 2023-05-16 15:53:43.000000 apache-airflow-providers-elasticsearch-4.5.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:45.000000 apache-airflow-providers-elasticsearch-4.5.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:45.000000 apache-airflow-providers-elasticsearch-4.5.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:45.000000 apache-airflow-providers-elasticsearch-4.5.0rc1/airflow/providers/elasticsearch/
+-rw-r--r--   0 root         (0) root         (0)     1396 2023-05-16 15:39:21.000000 apache-airflow-providers-elasticsearch-4.5.0rc1/airflow/providers/elasticsearch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2904 2023-05-16 15:53:43.000000 apache-airflow-providers-elasticsearch-4.5.0rc1/airflow/providers/elasticsearch/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:45.000000 apache-airflow-providers-elasticsearch-4.5.0rc1/airflow/providers/elasticsearch/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-elasticsearch-4.5.0rc1/airflow/providers/elasticsearch/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5488 2023-05-03 19:47:07.000000 apache-airflow-providers-elasticsearch-4.5.0rc1/airflow/providers/elasticsearch/hooks/elasticsearch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:45.000000 apache-airflow-providers-elasticsearch-4.5.0rc1/airflow/providers/elasticsearch/log/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-elasticsearch-4.5.0rc1/airflow/providers/elasticsearch/log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1808 2023-02-24 18:43:53.000000 apache-airflow-providers-elasticsearch-4.5.0rc1/airflow/providers/elasticsearch/log/es_json_formatter.py
+-rw-r--r--   0 root         (0) root         (0)    17262 2023-05-03 19:47:07.000000 apache-airflow-providers-elasticsearch-4.5.0rc1/airflow/providers/elasticsearch/log/es_task_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:45.000000 apache-airflow-providers-elasticsearch-4.5.0rc1/apache_airflow_providers_elasticsearch.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15352 2023-05-16 15:53:44.000000 apache-airflow-providers-elasticsearch-4.5.0rc1/apache_airflow_providers_elasticsearch.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      868 2023-05-16 15:53:44.000000 apache-airflow-providers-elasticsearch-4.5.0rc1/apache_airflow_providers_elasticsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:53:44.000000 apache-airflow-providers-elasticsearch-4.5.0rc1/apache_airflow_providers_elasticsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      110 2023-05-16 15:53:44.000000 apache-airflow-providers-elasticsearch-4.5.0rc1/apache_airflow_providers_elasticsearch.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:53:44.000000 apache-airflow-providers-elasticsearch-4.5.0rc1/apache_airflow_providers_elasticsearch.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      194 2023-05-16 15:53:44.000000 apache-airflow-providers-elasticsearch-4.5.0rc1/apache_airflow_providers_elasticsearch.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-16 15:53:44.000000 apache-airflow-providers-elasticsearch-4.5.0rc1/apache_airflow_providers_elasticsearch.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5308 2023-05-15 09:39:26.000000 apache-airflow-providers-elasticsearch-4.5.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1991 2023-05-16 15:53:45.000000 apache-airflow-providers-elasticsearch-4.5.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1733 2023-05-16 15:53:43.000000 apache-airflow-providers-elasticsearch-4.5.0rc1/setup.py
```

### Comparing `apache-airflow-providers-elasticsearch-4.4.0rc1/LICENSE` & `apache-airflow-providers-elasticsearch-4.5.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-elasticsearch-4.4.0rc1/MANIFEST.in` & `apache-airflow-providers-elasticsearch-4.5.0rc1/MANIFEST.in`

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

### Comparing `apache-airflow-providers-elasticsearch-4.4.0rc1/PKG-INFO` & `apache-airflow-providers-elasticsearch-4.5.0rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-elasticsearch
-Version: 4.4.0rc1
+Version: 4.5.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-elasticsearch package
 Home-page: https://airflow.apache.org/
+Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Download-URL: https://archive.apache.org/dist/airflow/providers
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-elasticsearch/4.4.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-elasticsearch/4.5.0/
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
 
 
 Package ``apache-airflow-providers-elasticsearch``
 
-Release: ``4.4.0rc1``
+Release: ``4.5.0rc1``
 
 
 `Elasticsearch <https://www.elastic.co/elasticsearch>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``elasticsearch`` provider. All classes for this provider package
 are in ``airflow.providers.elasticsearch`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-elasticsearch/4.4.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-elasticsearch/4.5.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -81,17 +80,17 @@
 
 Requirements
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
-``apache-airflow``                       ``>=2.3.0``
+``apache-airflow``                       ``>=2.4.0``
 ``apache-airflow-providers-common-sql``  ``>=1.3.1``
-``elasticsearch``                        ``>7``
+``elasticsearch``                        ``>7,<7.15.0``
 ``elasticsearch-dbapi``
 ``elasticsearch-dsl``                    ``>=5.0.0``
 =======================================  ==================
 
 Cross provider package dependencies
 -----------------------------------
 
@@ -133,14 +132,35 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+4.5.0
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
+* ``Upper-bind elasticearch integration (#31255)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
+   * ``Restore trigger logging (#29482)``
+   * ``Revert "Enable individual trigger logging (#27758)" (#29472)``
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add mechanism to suspend providers (#30422)``
+
 4.4.0
 .....
 
 Features
 ~~~~~~~~
 
 * ``Enable individual trigger logging (#27758)``
@@ -172,16 +192,17 @@
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Prepare for follow-up release for November providers (#27774)``
 
 4.3.0
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
@@ -232,16 +253,17 @@
 
 4.0.0
 .....
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
-* This release of provider is only available for Airflow 2.2+ as explained in the Apache Airflow
-  providers support policy https://github.com/apache/airflow/blob/main/README.md#support-for-providers
+.. note::
+  This release of provider is only available for Airflow 2.2+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Misc
 ~~~~
 
 * ``Apply per-run log templates to log handlers (#24153)``
 
 .. Below changes are excluded from the changelog. Move them to
@@ -449,9 +471,7 @@
 * ``Respect LogFormat when using ES logging with Json Format (#13310)``
 
 
 1.0.0
 .....
 
 Initial version of the provider.
-
-
```

### Comparing `apache-airflow-providers-elasticsearch-4.4.0rc1/README.rst` & `apache-airflow-providers-elasticsearch-4.5.0rc1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -15,28 +15,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-elasticsearch``
 
-Release: ``4.4.0rc1``
+Release: ``4.5.0rc1``
 
 
 `Elasticsearch <https://www.elastic.co/elasticsearch>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``elasticsearch`` provider. All classes for this provider package
 are in ``airflow.providers.elasticsearch`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-elasticsearch/4.4.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-elasticsearch/4.5.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -46,17 +46,17 @@
 
 Requirements
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
-``apache-airflow``                       ``>=2.3.0``
+``apache-airflow``                       ``>=2.4.0``
 ``apache-airflow-providers-common-sql``  ``>=1.3.1``
-``elasticsearch``                        ``>7``
+``elasticsearch``                        ``>7,<7.15.0``
 ``elasticsearch-dbapi``
 ``elasticsearch-dsl``                    ``>=5.0.0``
 =======================================  ==================
 
 Cross provider package dependencies
 -----------------------------------
 
@@ -98,14 +98,35 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+4.5.0
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
+* ``Upper-bind elasticearch integration (#31255)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
+   * ``Restore trigger logging (#29482)``
+   * ``Revert "Enable individual trigger logging (#27758)" (#29472)``
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add mechanism to suspend providers (#30422)``
+
 4.4.0
 .....
 
 Features
 ~~~~~~~~
 
 * ``Enable individual trigger logging (#27758)``
@@ -137,16 +158,17 @@
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Prepare for follow-up release for November providers (#27774)``
 
 4.3.0
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
@@ -197,16 +219,17 @@
 
 4.0.0
 .....
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
-* This release of provider is only available for Airflow 2.2+ as explained in the Apache Airflow
-  providers support policy https://github.com/apache/airflow/blob/main/README.md#support-for-providers
+.. note::
+  This release of provider is only available for Airflow 2.2+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Misc
 ~~~~
 
 * ``Apply per-run log templates to log handlers (#24153)``
 
 .. Below changes are excluded from the changelog. Move them to
```

### Comparing `apache-airflow-providers-elasticsearch-4.4.0rc1/airflow/providers/elasticsearch/__init__.py` & `apache-airflow-providers-elasticsearch-4.5.0rc1/airflow/providers/elasticsearch/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-elasticsearch-4.4.0rc1/airflow/providers/elasticsearch/get_provider_info.py` & `apache-airflow-providers-elasticsearch-4.5.0rc1/airflow/providers/elasticsearch/get_provider_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,17 @@
 
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-elasticsearch",
         "name": "Elasticsearch",
         "description": "`Elasticsearch <https://www.elastic.co/elasticsearch>`__\n",
+        "suspended": False,
         "versions": [
+            "4.5.0",
             "4.4.0",
             "4.3.3",
             "4.3.2",
             "4.3.1",
             "4.3.0",
             "4.2.1",
             "4.2.0",
@@ -49,17 +51,17 @@
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
-            "elasticsearch>7",
+            "elasticsearch>7,<7.15.0",
             "elasticsearch-dbapi",
             "elasticsearch-dsl>=5.0.0",
         ],
         "integrations": [
             {
                 "integration-name": "Elasticsearch",
                 "external-doc-url": "https://www.elastic.co/elasticsearch",
```

### Comparing `apache-airflow-providers-elasticsearch-4.4.0rc1/airflow/providers/elasticsearch/hooks/__init__.py` & `apache-airflow-providers-elasticsearch-4.5.0rc1/airflow/providers/elasticsearch/log/__init__.py`

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

### Comparing `apache-airflow-providers-elasticsearch-4.4.0rc1/airflow/providers/elasticsearch/hooks/elasticsearch.py` & `apache-airflow-providers-elasticsearch-4.5.0rc1/airflow/providers/elasticsearch/hooks/elasticsearch.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 import warnings
 from typing import Any
 
 from elasticsearch import Elasticsearch
 from es.elastic.api import Connection as ESConnection, connect
 
 from airflow.compat.functools import cached_property
+from airflow.exceptions import AirflowProviderDeprecationWarning
 from airflow.hooks.base import BaseHook
 from airflow.models.connection import Connection as AirflowConnection
 from airflow.providers.common.sql.hooks.sql import DbApiHook
 
 
 class ElasticsearchSQLHook(DbApiHook):
     """
@@ -106,15 +107,15 @@
     Please use `airflow.providers.elasticsearch.hooks.elasticsearch.ElasticsearchSQLHook`.
     """
 
     def __init__(self, *args, **kwargs):
         warnings.warn(
             """This class is deprecated.
             Please use `airflow.providers.elasticsearch.hooks.elasticsearch.ElasticsearchSQLHook`.""",
-            DeprecationWarning,
+            AirflowProviderDeprecationWarning,
             stacklevel=3,
         )
         super().__init__(*args, **kwargs)
 
 
 class ElasticsearchPythonHook(BaseHook):
     """
```

### Comparing `apache-airflow-providers-elasticsearch-4.4.0rc1/airflow/providers/elasticsearch/log/es_json_formatter.py` & `apache-airflow-providers-elasticsearch-4.5.0rc1/airflow/providers/elasticsearch/log/es_json_formatter.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-elasticsearch-4.4.0rc1/airflow/providers/elasticsearch/log/es_task_handler.py` & `apache-airflow-providers-elasticsearch-4.5.0rc1/airflow/providers/elasticsearch/log/es_task_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 
 # Using `from elasticsearch import *` would break elasticsearch mocking used in unit test.
 import elasticsearch
 import pendulum
 from elasticsearch_dsl import Search
 
 from airflow.configuration import conf
+from airflow.exceptions import AirflowProviderDeprecationWarning
 from airflow.models.dagrun import DagRun
 from airflow.models.taskinstance import TaskInstance
 from airflow.providers.elasticsearch.log.es_json_formatter import ElasticsearchJSONFormatter
 from airflow.utils import timezone
 from airflow.utils.log.file_task_handler import FileTaskHandler
 from airflow.utils.log.logging_mixin import ExternalLoggingMixin, LoggingMixin
 from airflow.utils.session import create_session
@@ -101,15 +102,15 @@
         self.closed = False
 
         self.client = elasticsearch.Elasticsearch(host.split(";"), **es_kwargs)  # type: ignore[attr-defined]
 
         if USE_PER_RUN_LOG_ID and log_id_template is not None:
             warnings.warn(
                 "Passing log_id_template to ElasticsearchTaskHandler is deprecated and has no effect",
-                DeprecationWarning,
+                AirflowProviderDeprecationWarning,
             )
 
         self.log_id_template = log_id_template  # Only used on Airflow < 2.3.2.
         self.frontend = frontend
         self.mark_end_on_close = True
         self.end_of_log_mark = end_of_log_mark.strip()
         self.write_stdout = write_stdout
```

### Comparing `apache-airflow-providers-elasticsearch-4.4.0rc1/apache_airflow_providers_elasticsearch.egg-info/PKG-INFO` & `apache-airflow-providers-elasticsearch-4.5.0rc1/apache_airflow_providers_elasticsearch.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-elasticsearch
-Version: 4.4.0rc1
+Version: 4.5.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-elasticsearch package
 Home-page: https://airflow.apache.org/
+Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Download-URL: https://archive.apache.org/dist/airflow/providers
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-elasticsearch/4.4.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-elasticsearch/4.5.0/
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
 
 
 Package ``apache-airflow-providers-elasticsearch``
 
-Release: ``4.4.0rc1``
+Release: ``4.5.0rc1``
 
 
 `Elasticsearch <https://www.elastic.co/elasticsearch>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``elasticsearch`` provider. All classes for this provider package
 are in ``airflow.providers.elasticsearch`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-elasticsearch/4.4.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-elasticsearch/4.5.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -81,17 +80,17 @@
 
 Requirements
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
-``apache-airflow``                       ``>=2.3.0``
+``apache-airflow``                       ``>=2.4.0``
 ``apache-airflow-providers-common-sql``  ``>=1.3.1``
-``elasticsearch``                        ``>7``
+``elasticsearch``                        ``>7,<7.15.0``
 ``elasticsearch-dbapi``
 ``elasticsearch-dsl``                    ``>=5.0.0``
 =======================================  ==================
 
 Cross provider package dependencies
 -----------------------------------
 
@@ -133,14 +132,35 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+4.5.0
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
+* ``Upper-bind elasticearch integration (#31255)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
+   * ``Restore trigger logging (#29482)``
+   * ``Revert "Enable individual trigger logging (#27758)" (#29472)``
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add mechanism to suspend providers (#30422)``
+
 4.4.0
 .....
 
 Features
 ~~~~~~~~
 
 * ``Enable individual trigger logging (#27758)``
@@ -172,16 +192,17 @@
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Prepare for follow-up release for November providers (#27774)``
 
 4.3.0
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
@@ -232,16 +253,17 @@
 
 4.0.0
 .....
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
-* This release of provider is only available for Airflow 2.2+ as explained in the Apache Airflow
-  providers support policy https://github.com/apache/airflow/blob/main/README.md#support-for-providers
+.. note::
+  This release of provider is only available for Airflow 2.2+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Misc
 ~~~~
 
 * ``Apply per-run log templates to log handlers (#24153)``
 
 .. Below changes are excluded from the changelog. Move them to
@@ -449,9 +471,7 @@
 * ``Respect LogFormat when using ES logging with Json Format (#13310)``
 
 
 1.0.0
 .....
 
 Initial version of the provider.
-
-
```

### Comparing `apache-airflow-providers-elasticsearch-4.4.0rc1/apache_airflow_providers_elasticsearch.egg-info/SOURCES.txt` & `apache-airflow-providers-elasticsearch-4.5.0rc1/apache_airflow_providers_elasticsearch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-elasticsearch-4.4.0rc1/pyproject.toml` & `apache-airflow-providers-elasticsearch-4.5.0rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-elasticsearch-4.4.0rc1/setup.cfg` & `apache-airflow-providers-elasticsearch-4.5.0rc1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-elasticsearch/4.4.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-elasticsearch/4.5.0/
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
@@ -43,18 +43,18 @@
 python_requires = ~=3.7
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
 	apache-airflow-providers-common-sql>=1.3.1.dev0
-	apache-airflow>=2.3.0.dev0
+	apache-airflow>=2.4.0.dev0
 	elasticsearch-dbapi
 	elasticsearch-dsl>=5.0.0
-	elasticsearch>7
+	elasticsearch>7,<7.15.0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.elasticsearch.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.elasticsearch
```

### Comparing `apache-airflow-providers-elasticsearch-4.4.0rc1/setup.py` & `apache-airflow-providers-elasticsearch-4.5.0rc1/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -22,23 +22,28 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-elasticsearch package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "4.4.0"
+version = "4.5.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-elasticsearch setup."""
     setup(
         version=version,
         extras_require={"common.sql": ["apache-airflow-providers-common-sql"]},
         packages=find_namespace_packages(
-            include=["airflow.providers.elasticsearch", "airflow.providers.elasticsearch.*"]
+            include=[
+                "airflow.providers.elasticsearch",
+                "airflow.providers.elasticsearch.*",
+                "airflow.providers.elasticsearch_vendor",
+                "airflow.providers.elasticsearch_vendor.*",
+            ],
         ),
     )
 
 
 if __name__ == "__main__":
     do_setup()
```

