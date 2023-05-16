# Comparing `tmp/apache-airflow-providers-imap-3.1.1rc2.tar.gz` & `tmp/apache-airflow-providers-imap-3.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-imap-3.1.1rc2.tar", last modified: Mon Jan  2 13:09:17 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-imap-3.2.0rc1.tar", last modified: Tue May 16 15:54:23 2023, max compression
```

## Comparing `apache-airflow-providers-imap-3.1.1rc2.tar` & `apache-airflow-providers-imap-3.2.0rc1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-02 13:09:17.000000 apache-airflow-providers-imap-3.1.1rc2/
--rw-r--r--   0 root         (0) root         (0)    10850 2022-10-05 12:15:16.000000 apache-airflow-providers-imap-3.1.1rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1122 2023-01-02 13:09:15.000000 apache-airflow-providers-imap-3.1.1rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2022-10-05 12:15:16.000000 apache-airflow-providers-imap-3.1.1rc2/NOTICE
--rw-r--r--   0 root         (0) root         (0)     9035 2023-01-02 13:09:17.000000 apache-airflow-providers-imap-3.1.1rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7494 2023-01-02 13:09:15.000000 apache-airflow-providers-imap-3.1.1rc2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-02 13:09:16.000000 apache-airflow-providers-imap-3.1.1rc2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-02 13:09:16.000000 apache-airflow-providers-imap-3.1.1rc2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-02 13:09:16.000000 apache-airflow-providers-imap-3.1.1rc2/airflow/providers/imap/
--rw-r--r--   0 root         (0) root         (0)      787 2022-10-05 12:15:15.000000 apache-airflow-providers-imap-3.1.1rc2/airflow/providers/imap/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2504 2023-01-02 13:09:15.000000 apache-airflow-providers-imap-3.1.1rc2/airflow/providers/imap/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-02 13:09:16.000000 apache-airflow-providers-imap-3.1.1rc2/airflow/providers/imap/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2022-10-05 12:15:15.000000 apache-airflow-providers-imap-3.1.1rc2/airflow/providers/imap/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14090 2022-12-20 13:50:43.000000 apache-airflow-providers-imap-3.1.1rc2/airflow/providers/imap/hooks/imap.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-02 13:09:16.000000 apache-airflow-providers-imap-3.1.1rc2/airflow/providers/imap/sensors/
--rw-r--r--   0 root         (0) root         (0)      787 2022-10-05 12:15:15.000000 apache-airflow-providers-imap-3.1.1rc2/airflow/providers/imap/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3054 2022-11-03 13:17:26.000000 apache-airflow-providers-imap-3.1.1rc2/airflow/providers/imap/sensors/imap_attachment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-02 13:09:17.000000 apache-airflow-providers-imap-3.1.1rc2/apache_airflow_providers_imap.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9035 2023-01-02 13:09:16.000000 apache-airflow-providers-imap-3.1.1rc2/apache_airflow_providers_imap.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      641 2023-01-02 13:09:16.000000 apache-airflow-providers-imap-3.1.1rc2/apache_airflow_providers_imap.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-02 13:09:16.000000 apache-airflow-providers-imap-3.1.1rc2/apache_airflow_providers_imap.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      102 2023-01-02 13:09:16.000000 apache-airflow-providers-imap-3.1.1rc2/apache_airflow_providers_imap.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-02 13:09:16.000000 apache-airflow-providers-imap-3.1.1rc2/apache_airflow_providers_imap.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)        8 2023-01-02 13:09:16.000000 apache-airflow-providers-imap-3.1.1rc2/apache_airflow_providers_imap.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1860 2022-12-20 13:50:44.000000 apache-airflow-providers-imap-3.1.1rc2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1788 2023-01-02 13:09:17.000000 apache-airflow-providers-imap-3.1.1rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1456 2023-01-02 13:09:15.000000 apache-airflow-providers-imap-3.1.1rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:23.000000 apache-airflow-providers-imap-3.2.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-imap-3.2.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-05-16 15:54:22.000000 apache-airflow-providers-imap-3.2.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-imap-3.2.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     9593 2023-05-16 15:54:23.000000 apache-airflow-providers-imap-3.2.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8072 2023-05-16 15:54:22.000000 apache-airflow-providers-imap-3.2.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:23.000000 apache-airflow-providers-imap-3.2.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:23.000000 apache-airflow-providers-imap-3.2.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:23.000000 apache-airflow-providers-imap-3.2.0rc1/airflow/providers/imap/
+-rw-r--r--   0 root         (0) root         (0)     1387 2023-05-16 15:39:21.000000 apache-airflow-providers-imap-3.2.0rc1/airflow/providers/imap/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2553 2023-05-16 15:54:22.000000 apache-airflow-providers-imap-3.2.0rc1/airflow/providers/imap/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:23.000000 apache-airflow-providers-imap-3.2.0rc1/airflow/providers/imap/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-imap-3.2.0rc1/airflow/providers/imap/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14090 2023-02-24 18:43:53.000000 apache-airflow-providers-imap-3.2.0rc1/airflow/providers/imap/hooks/imap.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:23.000000 apache-airflow-providers-imap-3.2.0rc1/airflow/providers/imap/sensors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-imap-3.2.0rc1/airflow/providers/imap/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3054 2023-02-24 18:43:53.000000 apache-airflow-providers-imap-3.2.0rc1/airflow/providers/imap/sensors/imap_attachment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:23.000000 apache-airflow-providers-imap-3.2.0rc1/apache_airflow_providers_imap.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9593 2023-05-16 15:54:23.000000 apache-airflow-providers-imap-3.2.0rc1/apache_airflow_providers_imap.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      641 2023-05-16 15:54:23.000000 apache-airflow-providers-imap-3.2.0rc1/apache_airflow_providers_imap.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:54:23.000000 apache-airflow-providers-imap-3.2.0rc1/apache_airflow_providers_imap.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      101 2023-05-16 15:54:23.000000 apache-airflow-providers-imap-3.2.0rc1/apache_airflow_providers_imap.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:54:23.000000 apache-airflow-providers-imap-3.2.0rc1/apache_airflow_providers_imap.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-16 15:54:23.000000 apache-airflow-providers-imap-3.2.0rc1/apache_airflow_providers_imap.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5308 2023-05-15 09:39:26.000000 apache-airflow-providers-imap-3.2.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1788 2023-05-16 15:54:23.000000 apache-airflow-providers-imap-3.2.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1626 2023-05-16 15:54:22.000000 apache-airflow-providers-imap-3.2.0rc1/setup.py
```

### Comparing `apache-airflow-providers-imap-3.1.1rc2/LICENSE` & `apache-airflow-providers-imap-3.2.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-imap-3.1.1rc2/MANIFEST.in` & `apache-airflow-providers-imap-3.2.0rc1/MANIFEST.in`

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

### Comparing `apache-airflow-providers-imap-3.1.1rc2/PKG-INFO` & `apache-airflow-providers-imap-3.2.0rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-imap
-Version: 3.1.1rc2
+Version: 3.2.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-imap package
 Home-page: https://airflow.apache.org/
+Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Download-URL: https://archive.apache.org/dist/airflow/providers
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-imap/3.1.1/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-imap/3.2.0/
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
 
 
 Package ``apache-airflow-providers-imap``
 
-Release: ``3.1.1rc2``
+Release: ``3.2.0rc1``
 
 
 `Internet Message Access Protocol (IMAP) <https://tools.ietf.org/html/rfc3501>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``imap`` provider. All classes for this provider package
 are in ``airflow.providers.imap`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-imap/3.1.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-imap/3.2.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -100,29 +99,41 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.2.0
+.....
+
+.. note::
+  This release of provider is only available for Airflow 2.4+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add mechanism to suspend providers (#30422)``
+   * ``Fix imap change log (#28749)``
+
 3.1.1
 .....
 
 Misc
 ~~~~
-   * ``[misc] Get rid of 'pass' statement in conditions (#27775)``
 
-.. Below changes are excluded from the changelog. Move them to
-   appropriate section above if needed. Do not delete the lines(!):
+* ``[misc] Get rid of 'pass' statement in conditions (#27775)``
 
 3.1.0
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
@@ -138,16 +149,17 @@
 
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
 
@@ -249,9 +261,7 @@
 
 Updated documentation and readme files.
 
 1.0.0
 .....
 
 Initial version of the provider.
-
-
```

### Comparing `apache-airflow-providers-imap-3.1.1rc2/README.rst` & `apache-airflow-providers-imap-3.2.0rc1/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -15,28 +15,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-imap``
 
-Release: ``3.1.1rc2``
+Release: ``3.2.0rc1``
 
 
 `Internet Message Access Protocol (IMAP) <https://tools.ietf.org/html/rfc3501>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``imap`` provider. All classes for this provider package
 are in ``airflow.providers.imap`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-imap/3.1.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-imap/3.2.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -66,29 +66,41 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.2.0
+.....
+
+.. note::
+  This release of provider is only available for Airflow 2.4+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add mechanism to suspend providers (#30422)``
+   * ``Fix imap change log (#28749)``
+
 3.1.1
 .....
 
 Misc
 ~~~~
-   * ``[misc] Get rid of 'pass' statement in conditions (#27775)``
 
-.. Below changes are excluded from the changelog. Move them to
-   appropriate section above if needed. Do not delete the lines(!):
+* ``[misc] Get rid of 'pass' statement in conditions (#27775)``
 
 3.1.0
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
@@ -104,16 +116,17 @@
 
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

### Comparing `apache-airflow-providers-imap-3.1.1rc2/airflow/providers/imap/__init__.py` & `apache-airflow-providers-imap-3.2.0rc1/airflow/providers/imap/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-imap-3.1.1rc2/airflow/providers/imap/get_provider_info.py` & `apache-airflow-providers-imap-3.2.0rc1/airflow/providers/imap/get_provider_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,17 @@
 
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-imap",
         "name": "Internet Message Access Protocol (IMAP)",
         "description": "`Internet Message Access Protocol (IMAP) <https://tools.ietf.org/html/rfc3501>`__\n",
+        "suspended": False,
         "versions": [
+            "3.2.0",
             "3.1.1",
             "3.1.0",
             "3.0.0",
             "2.2.3",
             "2.2.2",
             "2.2.1",
             "2.2.0",
```

### Comparing `apache-airflow-providers-imap-3.1.1rc2/airflow/providers/imap/hooks/__init__.py` & `apache-airflow-providers-imap-3.2.0rc1/airflow/providers/imap/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-imap-3.1.1rc2/airflow/providers/imap/hooks/imap.py` & `apache-airflow-providers-imap-3.2.0rc1/airflow/providers/imap/hooks/imap.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-imap-3.1.1rc2/airflow/providers/imap/sensors/imap_attachment.py` & `apache-airflow-providers-imap-3.2.0rc1/airflow/providers/imap/sensors/imap_attachment.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-imap-3.1.1rc2/apache_airflow_providers_imap.egg-info/PKG-INFO` & `apache-airflow-providers-imap-3.2.0rc1/apache_airflow_providers_imap.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-imap
-Version: 3.1.1rc2
+Version: 3.2.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-imap package
 Home-page: https://airflow.apache.org/
+Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Download-URL: https://archive.apache.org/dist/airflow/providers
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-imap/3.1.1/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-imap/3.2.0/
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
 
 
 Package ``apache-airflow-providers-imap``
 
-Release: ``3.1.1rc2``
+Release: ``3.2.0rc1``
 
 
 `Internet Message Access Protocol (IMAP) <https://tools.ietf.org/html/rfc3501>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``imap`` provider. All classes for this provider package
 are in ``airflow.providers.imap`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-imap/3.1.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-imap/3.2.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -100,29 +99,41 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.2.0
+.....
+
+.. note::
+  This release of provider is only available for Airflow 2.4+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add mechanism to suspend providers (#30422)``
+   * ``Fix imap change log (#28749)``
+
 3.1.1
 .....
 
 Misc
 ~~~~
-   * ``[misc] Get rid of 'pass' statement in conditions (#27775)``
 
-.. Below changes are excluded from the changelog. Move them to
-   appropriate section above if needed. Do not delete the lines(!):
+* ``[misc] Get rid of 'pass' statement in conditions (#27775)``
 
 3.1.0
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
@@ -138,16 +149,17 @@
 
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
 
@@ -249,9 +261,7 @@
 
 Updated documentation and readme files.
 
 1.0.0
 .....
 
 Initial version of the provider.
-
-
```

### Comparing `apache-airflow-providers-imap-3.1.1rc2/apache_airflow_providers_imap.egg-info/SOURCES.txt` & `apache-airflow-providers-imap-3.2.0rc1/apache_airflow_providers_imap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-imap-3.1.1rc2/setup.cfg` & `apache-airflow-providers-imap-3.2.0rc1/setup.cfg`

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-imap/3.1.1/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-imap/3.2.0/
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
@@ -51,10 +51,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.imap.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.imap
 
 [egg_info]
-tag_build = rc2
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-imap-3.1.1rc2/setup.py` & `apache-airflow-providers-imap-3.2.0rc1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,21 +22,28 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-imap package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "3.1.1"
+version = "3.2.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-imap setup."""
     setup(
         version=version,
         extras_require={},
-        packages=find_namespace_packages(include=["airflow.providers.imap", "airflow.providers.imap.*"]),
+        packages=find_namespace_packages(
+            include=[
+                "airflow.providers.imap",
+                "airflow.providers.imap.*",
+                "airflow.providers.imap_vendor",
+                "airflow.providers.imap_vendor.*",
+            ],
+        ),
     )
 
 
 if __name__ == "__main__":
     do_setup()
```

