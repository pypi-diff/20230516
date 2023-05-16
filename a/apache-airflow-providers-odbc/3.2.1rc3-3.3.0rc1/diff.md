# Comparing `tmp/apache-airflow-providers-odbc-3.2.1rc3.tar.gz` & `tmp/apache-airflow-providers-odbc-3.3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-odbc-3.2.1rc3.tar", last modified: Sat Nov 26 10:29:50 2022, max compression
+gzip compressed data, was "dist/apache-airflow-providers-odbc-3.3.0rc1.tar", last modified: Tue May 16 15:54:44 2023, max compression
```

## Comparing `apache-airflow-providers-odbc-3.2.1rc3.tar` & `apache-airflow-providers-odbc-3.3.0rc1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 10:29:50.000000 apache-airflow-providers-odbc-3.2.1rc3/
--rw-r--r--   0 root         (0) root         (0)    10850 2022-05-27 19:54:38.000000 apache-airflow-providers-odbc-3.2.1rc3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1122 2022-11-26 10:29:49.000000 apache-airflow-providers-odbc-3.2.1rc3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2022-05-27 19:54:38.000000 apache-airflow-providers-odbc-3.2.1rc3/NOTICE
--rw-r--r--   0 root         (0) root         (0)    10545 2022-11-26 10:29:50.000000 apache-airflow-providers-odbc-3.2.1rc3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8977 2022-11-26 10:29:49.000000 apache-airflow-providers-odbc-3.2.1rc3/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 10:29:50.000000 apache-airflow-providers-odbc-3.2.1rc3/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 10:29:50.000000 apache-airflow-providers-odbc-3.2.1rc3/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 10:29:50.000000 apache-airflow-providers-odbc-3.2.1rc3/airflow/providers/odbc/
--rw-r--r--   0 root         (0) root         (0)      785 2022-09-13 10:31:21.000000 apache-airflow-providers-odbc-3.2.1rc3/airflow/providers/odbc/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2184 2022-11-26 10:29:49.000000 apache-airflow-providers-odbc-3.2.1rc3/airflow/providers/odbc/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 10:29:50.000000 apache-airflow-providers-odbc-3.2.1rc3/airflow/providers/odbc/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2022-09-13 10:31:21.000000 apache-airflow-providers-odbc-3.2.1rc3/airflow/providers/odbc/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7661 2022-10-26 03:21:46.000000 apache-airflow-providers-odbc-3.2.1rc3/airflow/providers/odbc/hooks/odbc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 10:29:50.000000 apache-airflow-providers-odbc-3.2.1rc3/apache_airflow_providers_odbc.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10545 2022-11-26 10:29:50.000000 apache-airflow-providers-odbc-3.2.1rc3/apache_airflow_providers_odbc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      600 2022-11-26 10:29:50.000000 apache-airflow-providers-odbc-3.2.1rc3/apache_airflow_providers_odbc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-26 10:29:50.000000 apache-airflow-providers-odbc-3.2.1rc3/apache_airflow_providers_odbc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      102 2022-11-26 10:29:50.000000 apache-airflow-providers-odbc-3.2.1rc3/apache_airflow_providers_odbc.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-26 10:29:50.000000 apache-airflow-providers-odbc-3.2.1rc3/apache_airflow_providers_odbc.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      132 2022-11-26 10:29:50.000000 apache-airflow-providers-odbc-3.2.1rc3/apache_airflow_providers_odbc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2022-11-26 10:29:50.000000 apache-airflow-providers-odbc-3.2.1rc3/apache_airflow_providers_odbc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1836 2022-10-26 03:21:46.000000 apache-airflow-providers-odbc-3.2.1rc3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1873 2022-11-26 10:29:50.000000 apache-airflow-providers-odbc-3.2.1rc3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1509 2022-11-26 10:29:49.000000 apache-airflow-providers-odbc-3.2.1rc3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:44.000000 apache-airflow-providers-odbc-3.3.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-odbc-3.3.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-05-16 15:54:43.000000 apache-airflow-providers-odbc-3.3.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-odbc-3.3.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    11326 2023-05-16 15:54:44.000000 apache-airflow-providers-odbc-3.3.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9778 2023-05-16 15:54:43.000000 apache-airflow-providers-odbc-3.3.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:44.000000 apache-airflow-providers-odbc-3.3.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:44.000000 apache-airflow-providers-odbc-3.3.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:44.000000 apache-airflow-providers-odbc-3.3.0rc1/airflow/providers/odbc/
+-rw-r--r--   0 root         (0) root         (0)     1387 2023-05-16 15:39:21.000000 apache-airflow-providers-odbc-3.3.0rc1/airflow/providers/odbc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2233 2023-05-16 15:54:43.000000 apache-airflow-providers-odbc-3.3.0rc1/airflow/providers/odbc/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:44.000000 apache-airflow-providers-odbc-3.3.0rc1/airflow/providers/odbc/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-odbc-3.3.0rc1/airflow/providers/odbc/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7661 2023-02-24 18:43:53.000000 apache-airflow-providers-odbc-3.3.0rc1/airflow/providers/odbc/hooks/odbc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:44.000000 apache-airflow-providers-odbc-3.3.0rc1/apache_airflow_providers_odbc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11326 2023-05-16 15:54:44.000000 apache-airflow-providers-odbc-3.3.0rc1/apache_airflow_providers_odbc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      600 2023-05-16 15:54:44.000000 apache-airflow-providers-odbc-3.3.0rc1/apache_airflow_providers_odbc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:54:44.000000 apache-airflow-providers-odbc-3.3.0rc1/apache_airflow_providers_odbc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      101 2023-05-16 15:54:44.000000 apache-airflow-providers-odbc-3.3.0rc1/apache_airflow_providers_odbc.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:54:44.000000 apache-airflow-providers-odbc-3.3.0rc1/apache_airflow_providers_odbc.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      132 2023-05-16 15:54:44.000000 apache-airflow-providers-odbc-3.3.0rc1/apache_airflow_providers_odbc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-16 15:54:44.000000 apache-airflow-providers-odbc-3.3.0rc1/apache_airflow_providers_odbc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5308 2023-05-15 09:39:26.000000 apache-airflow-providers-odbc-3.3.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1873 2023-05-16 15:54:44.000000 apache-airflow-providers-odbc-3.3.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-05-16 15:54:43.000000 apache-airflow-providers-odbc-3.3.0rc1/setup.py
```

### Comparing `apache-airflow-providers-odbc-3.2.1rc3/LICENSE` & `apache-airflow-providers-odbc-3.3.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-odbc-3.2.1rc3/MANIFEST.in` & `apache-airflow-providers-odbc-3.3.0rc1/MANIFEST.in`

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

### Comparing `apache-airflow-providers-odbc-3.2.1rc3/PKG-INFO` & `apache-airflow-providers-odbc-3.3.0rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-odbc
-Version: 3.2.1rc3
+Version: 3.3.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-odbc package
 Home-page: https://airflow.apache.org/
+Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Download-URL: https://archive.apache.org/dist/airflow/providers
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-odbc/3.2.1/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-odbc/3.3.0/
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
 
 
 Package ``apache-airflow-providers-odbc``
 
-Release: ``3.2.1rc3``
+Release: ``3.3.0rc1``
 
 
 `ODBC <https://github.com/mkleehammer/pyodbc/wiki>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``odbc`` provider. All classes for this provider package
 are in ``airflow.providers.odbc`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-odbc/3.2.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-odbc/3.3.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -81,15 +80,15 @@
 
 Requirements
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
-``apache-airflow``                       ``>=2.3.0``
+``apache-airflow``                       ``>=2.4.0``
 ``apache-airflow-providers-common-sql``  ``>=1.3.1``
 ``pyodbc``
 =======================================  ==================
 
 Cross provider package dependencies
 -----------------------------------
 
@@ -131,14 +130,32 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.3.0
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
+   * ``Switch to ruff for faster static checks (#28893)``
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add mechanism to suspend providers (#30422)``
+
 3.2.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
 
 * ``Bump common.sql provider to 1.3.1 (#27888)``
@@ -146,16 +163,17 @@
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Prepare for follow-up release for November providers (#27774)``
 
 3.2.0
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
@@ -197,16 +215,17 @@
 
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
 
@@ -308,9 +327,7 @@
 
 Updated documentation and readme files.
 
 1.0.0
 .....
 
 Initial version of the provider.
-
-
```

### Comparing `apache-airflow-providers-odbc-3.2.1rc3/README.rst` & `apache-airflow-providers-odbc-3.3.0rc1/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -15,28 +15,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-odbc``
 
-Release: ``3.2.1rc3``
+Release: ``3.3.0rc1``
 
 
 `ODBC <https://github.com/mkleehammer/pyodbc/wiki>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``odbc`` provider. All classes for this provider package
 are in ``airflow.providers.odbc`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-odbc/3.2.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-odbc/3.3.0/>`_.
 
 
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
 ``pyodbc``
 =======================================  ==================
 
 Cross provider package dependencies
 -----------------------------------
 
@@ -96,14 +96,32 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.3.0
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
+   * ``Switch to ruff for faster static checks (#28893)``
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add mechanism to suspend providers (#30422)``
+
 3.2.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
 
 * ``Bump common.sql provider to 1.3.1 (#27888)``
@@ -111,16 +129,17 @@
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Prepare for follow-up release for November providers (#27774)``
 
 3.2.0
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
@@ -162,16 +181,17 @@
 
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

### Comparing `apache-airflow-providers-odbc-3.2.1rc3/airflow/providers/odbc/__init__.py` & `apache-airflow-providers-odbc-3.3.0rc1/airflow/providers/odbc/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-odbc-3.2.1rc3/airflow/providers/odbc/get_provider_info.py` & `apache-airflow-providers-odbc-3.3.0rc1/airflow/providers/odbc/get_provider_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,30 +23,32 @@
 
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-odbc",
         "name": "ODBC",
         "description": "`ODBC <https://github.com/mkleehammer/pyodbc/wiki>`__\n",
+        "suspended": False,
         "versions": [
+            "3.3.0",
             "3.2.1",
             "3.2.0",
             "3.1.2",
             "3.1.1",
             "3.1.0",
             "3.0.0",
             "2.0.4",
             "2.0.3",
             "2.0.2",
             "2.0.1",
             "2.0.0",
             "1.0.1",
             "1.0.0",
         ],
-        "dependencies": ["apache-airflow>=2.3.0", "apache-airflow-providers-common-sql>=1.3.1", "pyodbc"],
+        "dependencies": ["apache-airflow>=2.4.0", "apache-airflow-providers-common-sql>=1.3.1", "pyodbc"],
         "integrations": [
             {
                 "integration-name": "ODBC",
                 "external-doc-url": "https://github.com/mkleehammer/pyodbc/wiki",
                 "logo": "/integration-logos/odbc/ODBC.png",
                 "tags": ["protocol"],
             }
```

### Comparing `apache-airflow-providers-odbc-3.2.1rc3/airflow/providers/odbc/hooks/odbc.py` & `apache-airflow-providers-odbc-3.3.0rc1/airflow/providers/odbc/hooks/odbc.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,15 +141,15 @@
             if self.connection.password:
                 conn_str += f"PWD={self.connection.password};"
             if self.connection.port:
                 conn_str += f"PORT={self.connection.port};"
 
             extra_exclude = {"driver", "dsn", "connect_kwargs", "sqlalchemy_scheme"}
             extra_params = {
-                k: v for k, v in self.connection.extra_dejson.items() if not k.lower() in extra_exclude
+                k: v for k, v in self.connection.extra_dejson.items() if k.lower() not in extra_exclude
             }
             for k, v in extra_params.items():
                 conn_str += f"{k}={v};"
 
             self._conn_str = conn_str
         return self._conn_str
```

### Comparing `apache-airflow-providers-odbc-3.2.1rc3/apache_airflow_providers_odbc.egg-info/PKG-INFO` & `apache-airflow-providers-odbc-3.3.0rc1/apache_airflow_providers_odbc.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-odbc
-Version: 3.2.1rc3
+Version: 3.3.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-odbc package
 Home-page: https://airflow.apache.org/
+Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Download-URL: https://archive.apache.org/dist/airflow/providers
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-odbc/3.2.1/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-odbc/3.3.0/
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
 
 
 Package ``apache-airflow-providers-odbc``
 
-Release: ``3.2.1rc3``
+Release: ``3.3.0rc1``
 
 
 `ODBC <https://github.com/mkleehammer/pyodbc/wiki>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``odbc`` provider. All classes for this provider package
 are in ``airflow.providers.odbc`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-odbc/3.2.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-odbc/3.3.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -81,15 +80,15 @@
 
 Requirements
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
-``apache-airflow``                       ``>=2.3.0``
+``apache-airflow``                       ``>=2.4.0``
 ``apache-airflow-providers-common-sql``  ``>=1.3.1``
 ``pyodbc``
 =======================================  ==================
 
 Cross provider package dependencies
 -----------------------------------
 
@@ -131,14 +130,32 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.3.0
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
+   * ``Switch to ruff for faster static checks (#28893)``
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add mechanism to suspend providers (#30422)``
+
 3.2.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
 
 * ``Bump common.sql provider to 1.3.1 (#27888)``
@@ -146,16 +163,17 @@
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Prepare for follow-up release for November providers (#27774)``
 
 3.2.0
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
@@ -197,16 +215,17 @@
 
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
 
@@ -308,9 +327,7 @@
 
 Updated documentation and readme files.
 
 1.0.0
 .....
 
 Initial version of the provider.
-
-
```

### Comparing `apache-airflow-providers-odbc-3.2.1rc3/apache_airflow_providers_odbc.egg-info/SOURCES.txt` & `apache-airflow-providers-odbc-3.3.0rc1/apache_airflow_providers_odbc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-odbc-3.2.1rc3/setup.cfg` & `apache-airflow-providers-odbc-3.3.0rc1/setup.cfg`

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-odbc/3.2.1/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-odbc/3.3.0/
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
 	pyodbc
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.odbc.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.odbc
 
 [egg_info]
-tag_build = rc3
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-odbc-3.2.1rc3/setup.py` & `apache-airflow-providers-odbc-3.3.0rc1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,21 +22,28 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-odbc package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "3.2.1"
+version = "3.3.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-odbc setup."""
     setup(
         version=version,
         extras_require={"common.sql": ["apache-airflow-providers-common-sql"]},
-        packages=find_namespace_packages(include=["airflow.providers.odbc", "airflow.providers.odbc.*"]),
+        packages=find_namespace_packages(
+            include=[
+                "airflow.providers.odbc",
+                "airflow.providers.odbc.*",
+                "airflow.providers.odbc_vendor",
+                "airflow.providers.odbc_vendor.*",
+            ],
+        ),
     )
 
 
 if __name__ == "__main__":
     do_setup()
```

