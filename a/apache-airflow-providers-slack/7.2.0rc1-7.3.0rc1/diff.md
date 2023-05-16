# Comparing `tmp/apache-airflow-providers-slack-7.2.0rc1.tar.gz` & `tmp/apache-airflow-providers-slack-7.3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-slack-7.2.0rc1.tar", last modified: Sat Jan 14 12:16:39 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-slack-7.3.0rc1.tar", last modified: Tue May 16 15:55:14 2023, max compression
```

## Comparing `apache-airflow-providers-slack-7.2.0rc1.tar` & `apache-airflow-providers-slack-7.3.0rc1.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 12:16:39.000000 apache-airflow-providers-slack-7.2.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2022-10-05 12:15:16.000000 apache-airflow-providers-slack-7.2.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1122 2023-01-14 12:16:37.000000 apache-airflow-providers-slack-7.2.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2022-10-05 12:15:16.000000 apache-airflow-providers-slack-7.2.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    14333 2023-01-14 12:16:39.000000 apache-airflow-providers-slack-7.2.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12762 2023-01-14 12:16:37.000000 apache-airflow-providers-slack-7.2.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 12:16:38.000000 apache-airflow-providers-slack-7.2.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 12:16:38.000000 apache-airflow-providers-slack-7.2.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 12:16:38.000000 apache-airflow-providers-slack-7.2.0rc1/airflow/providers/slack/
--rw-r--r--   0 root         (0) root         (0)      787 2022-10-05 12:15:15.000000 apache-airflow-providers-slack-7.2.0rc1/airflow/providers/slack/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3446 2023-01-14 12:16:37.000000 apache-airflow-providers-slack-7.2.0rc1/airflow/providers/slack/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 12:16:38.000000 apache-airflow-providers-slack-7.2.0rc1/airflow/providers/slack/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2022-10-05 12:15:15.000000 apache-airflow-providers-slack-7.2.0rc1/airflow/providers/slack/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14438 2023-01-11 12:48:26.000000 apache-airflow-providers-slack-7.2.0rc1/airflow/providers/slack/hooks/slack.py
--rw-r--r--   0 root         (0) root         (0)    21132 2023-01-11 12:48:26.000000 apache-airflow-providers-slack-7.2.0rc1/airflow/providers/slack/hooks/slack_webhook.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 12:16:38.000000 apache-airflow-providers-slack-7.2.0rc1/airflow/providers/slack/notifications/
--rw-r--r--   0 root         (0) root         (0)      785 2023-01-11 12:48:26.000000 apache-airflow-providers-slack-7.2.0rc1/airflow/providers/slack/notifications/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3214 2023-01-11 12:48:26.000000 apache-airflow-providers-slack-7.2.0rc1/airflow/providers/slack/notifications/slack_notifier.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 12:16:38.000000 apache-airflow-providers-slack-7.2.0rc1/airflow/providers/slack/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2022-10-05 12:15:15.000000 apache-airflow-providers-slack-7.2.0rc1/airflow/providers/slack/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8359 2023-01-11 12:48:26.000000 apache-airflow-providers-slack-7.2.0rc1/airflow/providers/slack/operators/slack.py
--rw-r--r--   0 root         (0) root         (0)     7351 2023-01-11 12:48:26.000000 apache-airflow-providers-slack-7.2.0rc1/airflow/providers/slack/operators/slack_webhook.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 12:16:38.000000 apache-airflow-providers-slack-7.2.0rc1/airflow/providers/slack/transfers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-01-11 12:48:26.000000 apache-airflow-providers-slack-7.2.0rc1/airflow/providers/slack/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12879 2023-01-11 12:48:26.000000 apache-airflow-providers-slack-7.2.0rc1/airflow/providers/slack/transfers/sql_to_slack.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 12:16:38.000000 apache-airflow-providers-slack-7.2.0rc1/airflow/providers/slack/utils/
--rw-r--r--   0 root         (0) root         (0)     5131 2023-01-11 12:48:26.000000 apache-airflow-providers-slack-7.2.0rc1/airflow/providers/slack/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 12:16:39.000000 apache-airflow-providers-slack-7.2.0rc1/apache_airflow_providers_slack.egg-info/
--rw-r--r--   0 root         (0) root         (0)    14333 2023-01-14 12:16:38.000000 apache-airflow-providers-slack-7.2.0rc1/apache_airflow_providers_slack.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1043 2023-01-14 12:16:38.000000 apache-airflow-providers-slack-7.2.0rc1/apache_airflow_providers_slack.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-14 12:16:38.000000 apache-airflow-providers-slack-7.2.0rc1/apache_airflow_providers_slack.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-01-14 12:16:38.000000 apache-airflow-providers-slack-7.2.0rc1/apache_airflow_providers_slack.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-14 12:16:38.000000 apache-airflow-providers-slack-7.2.0rc1/apache_airflow_providers_slack.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      142 2023-01-14 12:16:38.000000 apache-airflow-providers-slack-7.2.0rc1/apache_airflow_providers_slack.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-01-14 12:16:38.000000 apache-airflow-providers-slack-7.2.0rc1/apache_airflow_providers_slack.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     3814 2023-01-13 19:37:41.000000 apache-airflow-providers-slack-7.2.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1889 2023-01-14 12:16:39.000000 apache-airflow-providers-slack-7.2.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1513 2023-01-14 12:16:37.000000 apache-airflow-providers-slack-7.2.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:14.000000 apache-airflow-providers-slack-7.3.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-slack-7.3.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-05-16 15:55:13.000000 apache-airflow-providers-slack-7.3.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-slack-7.3.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    15299 2023-05-16 15:55:14.000000 apache-airflow-providers-slack-7.3.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    13748 2023-05-16 15:55:13.000000 apache-airflow-providers-slack-7.3.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:14.000000 apache-airflow-providers-slack-7.3.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:14.000000 apache-airflow-providers-slack-7.3.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:14.000000 apache-airflow-providers-slack-7.3.0rc1/airflow/providers/slack/
+-rw-r--r--   0 root         (0) root         (0)     1388 2023-05-16 15:39:21.000000 apache-airflow-providers-slack-7.3.0rc1/airflow/providers/slack/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3592 2023-05-16 15:55:13.000000 apache-airflow-providers-slack-7.3.0rc1/airflow/providers/slack/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:14.000000 apache-airflow-providers-slack-7.3.0rc1/airflow/providers/slack/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-slack-7.3.0rc1/airflow/providers/slack/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14518 2023-05-03 19:47:07.000000 apache-airflow-providers-slack-7.3.0rc1/airflow/providers/slack/hooks/slack.py
+-rw-r--r--   0 root         (0) root         (0)    21257 2023-05-03 19:47:07.000000 apache-airflow-providers-slack-7.3.0rc1/airflow/providers/slack/hooks/slack_webhook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:14.000000 apache-airflow-providers-slack-7.3.0rc1/airflow/providers/slack/notifications/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-slack-7.3.0rc1/airflow/providers/slack/notifications/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3214 2023-05-12 14:26:38.000000 apache-airflow-providers-slack-7.3.0rc1/airflow/providers/slack/notifications/slack.py
+-rw-r--r--   0 root         (0) root         (0)     1243 2023-05-12 14:26:38.000000 apache-airflow-providers-slack-7.3.0rc1/airflow/providers/slack/notifications/slack_notifier.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:14.000000 apache-airflow-providers-slack-7.3.0rc1/airflow/providers/slack/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-slack-7.3.0rc1/airflow/providers/slack/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8439 2023-05-03 19:47:07.000000 apache-airflow-providers-slack-7.3.0rc1/airflow/providers/slack/operators/slack.py
+-rw-r--r--   0 root         (0) root         (0)     7416 2023-05-03 19:47:07.000000 apache-airflow-providers-slack-7.3.0rc1/airflow/providers/slack/operators/slack_webhook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:14.000000 apache-airflow-providers-slack-7.3.0rc1/airflow/providers/slack/transfers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-slack-7.3.0rc1/airflow/providers/slack/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12879 2023-02-24 18:43:53.000000 apache-airflow-providers-slack-7.3.0rc1/airflow/providers/slack/transfers/sql_to_slack.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:14.000000 apache-airflow-providers-slack-7.3.0rc1/airflow/providers/slack/utils/
+-rw-r--r--   0 root         (0) root         (0)     5131 2023-04-30 16:55:11.000000 apache-airflow-providers-slack-7.3.0rc1/airflow/providers/slack/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:14.000000 apache-airflow-providers-slack-7.3.0rc1/apache_airflow_providers_slack.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15299 2023-05-16 15:55:14.000000 apache-airflow-providers-slack-7.3.0rc1/apache_airflow_providers_slack.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1090 2023-05-16 15:55:14.000000 apache-airflow-providers-slack-7.3.0rc1/apache_airflow_providers_slack.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:55:14.000000 apache-airflow-providers-slack-7.3.0rc1/apache_airflow_providers_slack.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      102 2023-05-16 15:55:14.000000 apache-airflow-providers-slack-7.3.0rc1/apache_airflow_providers_slack.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:55:14.000000 apache-airflow-providers-slack-7.3.0rc1/apache_airflow_providers_slack.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      142 2023-05-16 15:55:14.000000 apache-airflow-providers-slack-7.3.0rc1/apache_airflow_providers_slack.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-16 15:55:14.000000 apache-airflow-providers-slack-7.3.0rc1/apache_airflow_providers_slack.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5308 2023-05-15 09:39:26.000000 apache-airflow-providers-slack-7.3.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1889 2023-05-16 15:55:14.000000 apache-airflow-providers-slack-7.3.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1685 2023-05-16 15:55:13.000000 apache-airflow-providers-slack-7.3.0rc1/setup.py
```

### Comparing `apache-airflow-providers-slack-7.2.0rc1/LICENSE` & `apache-airflow-providers-slack-7.3.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-slack-7.2.0rc1/MANIFEST.in` & `apache-airflow-providers-slack-7.3.0rc1/MANIFEST.in`

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

### Comparing `apache-airflow-providers-slack-7.2.0rc1/PKG-INFO` & `apache-airflow-providers-slack-7.3.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-slack
-Version: 7.2.0rc1
+Version: 7.3.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-slack package
 Home-page: https://airflow.apache.org/
+Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Download-URL: https://archive.apache.org/dist/airflow/providers
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-slack/7.2.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-slack/7.3.0/
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
 
 
 Package ``apache-airflow-providers-slack``
 
-Release: ``7.2.0rc1``
+Release: ``7.3.0rc1``
 
 
 `Slack <https://slack.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``slack`` provider. All classes for this provider package
 are in ``airflow.providers.slack`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-slack/7.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-slack/7.3.0/>`_.
 
 
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
 ``slack_sdk``                            ``>=3.0.0``
 =======================================  ==================
 
 Cross provider package dependencies
 -----------------------------------
 
@@ -131,14 +130,35 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+7.3.0
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
+* ``Add Documentation for notification feature extension (#29191)``
+* ``Standardize Slack Notifier (#31244)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
+   * ``Prepare docs for Feb 2023 wave of Providers (#29379)``
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add mechanism to suspend providers (#30422)``
+
 7.2.0
 .....
 
 Features
 ~~~~~~~~
 
 * ``Add general-purpose "notifier" concept to DAGs (#28569)``
@@ -170,16 +190,17 @@
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Prepare for follow-up release for November providers (#27774)``
 
 7.0.0
 .....
 
-This release of provider is only available for Airflow 2.3+ as explained in the
-`Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/README.md#support-for-providers>`_.
+.. note::
+  This release of provider is only available for Airflow 2.3+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
 * In SlackHook and SlackWebhookHook, if both ``extra__<conn type>__foo`` and ``foo`` existed
   in connection extra dict, the prefixed version would be used; now, the non-prefixed version
   will be preferred.  You'll see a warning if there is such a collision.
@@ -246,16 +267,17 @@
 
 5.0.0
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
 
@@ -408,9 +430,7 @@
 * ``Upgrade slack_sdk to v3 (#13745)``
 
 
 1.0.0
 .....
 
 Initial version of the provider.
-
-
```

### Comparing `apache-airflow-providers-slack-7.2.0rc1/README.rst` & `apache-airflow-providers-slack-7.3.0rc1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -15,28 +15,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-slack``
 
-Release: ``7.2.0rc1``
+Release: ``7.3.0rc1``
 
 
 `Slack <https://slack.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``slack`` provider. All classes for this provider package
 are in ``airflow.providers.slack`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-slack/7.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-slack/7.3.0/>`_.
 
 
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
 ``slack_sdk``                            ``>=3.0.0``
 =======================================  ==================
 
 Cross provider package dependencies
 -----------------------------------
 
@@ -96,14 +96,35 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+7.3.0
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
+* ``Add Documentation for notification feature extension (#29191)``
+* ``Standardize Slack Notifier (#31244)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
+   * ``Prepare docs for Feb 2023 wave of Providers (#29379)``
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add mechanism to suspend providers (#30422)``
+
 7.2.0
 .....
 
 Features
 ~~~~~~~~
 
 * ``Add general-purpose "notifier" concept to DAGs (#28569)``
@@ -135,16 +156,17 @@
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Prepare for follow-up release for November providers (#27774)``
 
 7.0.0
 .....
 
-This release of provider is only available for Airflow 2.3+ as explained in the
-`Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/README.md#support-for-providers>`_.
+.. note::
+  This release of provider is only available for Airflow 2.3+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
 * In SlackHook and SlackWebhookHook, if both ``extra__<conn type>__foo`` and ``foo`` existed
   in connection extra dict, the prefixed version would be used; now, the non-prefixed version
   will be preferred.  You'll see a warning if there is such a collision.
@@ -211,16 +233,17 @@
 
 5.0.0
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

### Comparing `apache-airflow-providers-slack-7.2.0rc1/airflow/providers/slack/__init__.py` & `apache-airflow-providers-slack-7.3.0rc1/airflow/providers/slack/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-slack-7.2.0rc1/airflow/providers/slack/get_provider_info.py` & `apache-airflow-providers-slack-7.3.0rc1/airflow/providers/slack/get_provider_info.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,17 @@
 
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-slack",
         "name": "Slack",
         "description": "`Slack <https://slack.com/>`__\n",
+        "suspended": False,
         "versions": [
+            "7.3.0",
             "7.2.0",
             "7.1.1",
             "7.1.0",
             "7.0.0",
             "6.0.0",
             "5.1.0",
             "5.0.0",
@@ -43,15 +45,15 @@
             "4.0.1",
             "4.0.0",
             "3.0.0",
             "2.0.0",
             "1.0.0",
         ],
         "dependencies": [
-            "apache-airflow>=2.3.0",
+            "apache-airflow>=2.4.0",
             "apache-airflow-providers-common-sql>=1.3.1",
             "slack_sdk>=3.0.0",
         ],
         "integrations": [
             {
                 "integration-name": "Slack",
                 "external-doc-url": "https://slack.com/",
@@ -91,8 +93,9 @@
         "connection-types": [
             {"hook-class-name": "airflow.providers.slack.hooks.slack.SlackHook", "connection-type": "slack"},
             {
                 "hook-class-name": "airflow.providers.slack.hooks.slack_webhook.SlackWebhookHook",
                 "connection-type": "slackwebhook",
             },
         ],
+        "notifications": ["airflow.providers.slack.notifications.slack_notifier.SlackNotifier"],
     }
```

### Comparing `apache-airflow-providers-slack-7.2.0rc1/airflow/providers/slack/hooks/__init__.py` & `apache-airflow-providers-slack-7.3.0rc1/airflow/providers/slack/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-slack-7.2.0rc1/airflow/providers/slack/hooks/slack.py` & `apache-airflow-providers-slack-7.3.0rc1/airflow/providers/slack/hooks/slack.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Sequence
 
 from slack_sdk import WebClient
 from slack_sdk.errors import SlackApiError
 
 from airflow.compat.functools import cached_property
-from airflow.exceptions import AirflowException, AirflowNotFoundException
+from airflow.exceptions import AirflowException, AirflowNotFoundException, AirflowProviderDeprecationWarning
 from airflow.hooks.base import BaseHook
 from airflow.providers.slack.utils import ConnectionExtraConfig
 from airflow.utils.helpers import exactly_one
 from airflow.utils.log.secrets_masker import mask_secret
 
 if TYPE_CHECKING:
     from slack_sdk.http_retry import RetryHandler
@@ -127,15 +127,15 @@
         if not token and not slack_conn_id:
             raise AirflowException("Either `slack_conn_id` or `token` should be provided.")
         if token:
             mask_secret(token)
             warnings.warn(
                 "Provide token as hook argument deprecated by security reason and will be removed "
                 "in a future releases. Please specify token in `Slack API` connection.",
-                DeprecationWarning,
+                AirflowProviderDeprecationWarning,
                 stacklevel=2,
             )
         if not slack_conn_id:
             warnings.warn(
                 "You have not set parameter `slack_conn_id`. Currently `Slack API` connection id optional "
                 "but in a future release it will mandatory.",
                 FutureWarning,
@@ -198,23 +198,23 @@
 
         return {k: v for k, v in conn_params.items() if v is not None}
 
     @cached_property
     def token(self) -> str:
         warnings.warn(
             "`SlackHook.token` property deprecated and will be removed in a future releases.",
-            DeprecationWarning,
+            AirflowProviderDeprecationWarning,
             stacklevel=2,
         )
         return self._get_conn_params()["token"]
 
     def __get_token(self, token: Any, slack_conn_id: Any) -> str:
         warnings.warn(
             "`SlackHook.__get_token` method deprecated and will be removed in a future releases.",
-            DeprecationWarning,
+            AirflowProviderDeprecationWarning,
             stacklevel=2,
         )
         if token is not None:
             return token
 
         if slack_conn_id is not None:
             conn = self.get_connection(slack_conn_id)
```

### Comparing `apache-airflow-providers-slack-7.2.0rc1/airflow/providers/slack/hooks/slack_webhook.py` & `apache-airflow-providers-slack-7.3.0rc1/airflow/providers/slack/hooks/slack_webhook.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from functools import wraps
 from typing import TYPE_CHECKING, Any, Callable
 from urllib.parse import urlsplit
 
 from slack_sdk import WebhookClient
 
 from airflow.compat.functools import cached_property
-from airflow.exceptions import AirflowException
+from airflow.exceptions import AirflowException, AirflowProviderDeprecationWarning
 from airflow.hooks.base import BaseHook
 from airflow.models import Connection
 from airflow.providers.slack.utils import ConnectionExtraConfig
 from airflow.utils.log.secrets_masker import mask_secret
 
 if TYPE_CHECKING:
     from slack_sdk.http_retry import RetryHandler
@@ -147,29 +147,29 @@
     ):
         super().__init__()
 
         http_conn_id = kwargs.pop("http_conn_id", None)
         if http_conn_id:
             warnings.warn(
                 "Parameter `http_conn_id` is deprecated. Please use `slack_webhook_conn_id` instead.",
-                DeprecationWarning,
+                AirflowProviderDeprecationWarning,
                 stacklevel=2,
             )
             if slack_webhook_conn_id:
                 raise AirflowException("You cannot provide both `slack_webhook_conn_id` and `http_conn_id`.")
             slack_webhook_conn_id = http_conn_id
 
         if not slack_webhook_conn_id and not webhook_token:
             raise AirflowException("Either `slack_webhook_conn_id` or `webhook_token` should be provided.")
         if webhook_token:
             mask_secret(webhook_token)
             warnings.warn(
                 "Provide `webhook_token` as hook argument deprecated by security reason and will be removed "
                 "in a future releases. Please specify it in `Slack Webhook` connection.",
-                DeprecationWarning,
+                AirflowProviderDeprecationWarning,
                 stacklevel=2,
             )
         if not slack_webhook_conn_id:
             warnings.warn(
                 "You have not set parameter `slack_webhook_conn_id`. Currently `Slack Incoming Webhook` "
                 "connection id optional but in a future release it will mandatory.",
                 FutureWarning,
@@ -210,15 +210,15 @@
                     )
 
         if deprecated_class_attrs:
             warnings.warn(
                 f"Provide {','.join(repr(a) for a in deprecated_class_attrs)} as hook argument(s) "
                 f"is deprecated and will be removed in a future releases. "
                 f"Please specify attributes in `{self.__class__.__name__}.send` method instead.",
-                DeprecationWarning,
+                AirflowProviderDeprecationWarning,
                 stacklevel=2,
             )
 
         self.extra_client_args = kwargs
 
     @cached_property
     def client(self) -> WebhookClient:
@@ -230,15 +230,15 @@
         return self.client
 
     @cached_property
     def webhook_token(self) -> str:
         """Return Slack Webhook Token URL."""
         warnings.warn(
             "`SlackHook.webhook_token` property deprecated and will be removed in a future releases.",
-            DeprecationWarning,
+            AirflowProviderDeprecationWarning,
             stacklevel=2,
         )
         return self._get_conn_params()["url"]
 
     def _get_conn_params(self) -> dict[str, Any]:
         """Fetch connection params as a dict and merge it with hook parameters."""
         default_schema, _, default_host = DEFAULT_SLACK_WEBHOOK_ENDPOINT.partition("://")
@@ -294,15 +294,15 @@
                         "Cannot get token: No valid Slack token nor valid Connection ID supplied."
                     )
                 mask_secret(parsed_token)
                 warnings.warn(
                     f"Found Slack Webhook Token URL in Connection {conn.conn_id!r} `host` "
                     "and `password` field is empty. This behaviour deprecated "
                     "and could expose you token in the UI and will be removed in a future releases.",
-                    DeprecationWarning,
+                    AirflowProviderDeprecationWarning,
                     stacklevel=2,
                 )
             url = (base_url.rstrip("/") + "/" + webhook_token.lstrip("/")).rstrip("/")
 
         conn_params["url"] = url
         # Merge Hook parameters with Connection config
         conn_params.update(
@@ -493,11 +493,11 @@
             and expected that Slack Incoming Webhook message constructing from class attributes rather than
             pass as method arguments.
         """
         warnings.warn(
             "`SlackWebhookHook.execute` method deprecated and will be removed in a future releases. "
             "Please use `SlackWebhookHook.send` or `SlackWebhookHook.send_dict` or "
             "`SlackWebhookHook.send_text` methods instead.",
-            DeprecationWarning,
+            AirflowProviderDeprecationWarning,
             stacklevel=2,
         )
         self.send()
```

### Comparing `apache-airflow-providers-slack-7.2.0rc1/airflow/providers/slack/notifications/__init__.py` & `apache-airflow-providers-slack-7.3.0rc1/airflow/providers/slack/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-slack-7.2.0rc1/airflow/providers/slack/notifications/slack_notifier.py` & `apache-airflow-providers-slack-7.3.0rc1/airflow/providers/slack/notifications/slack.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-slack-7.2.0rc1/airflow/providers/slack/operators/__init__.py` & `apache-airflow-providers-slack-7.3.0rc1/airflow/providers/slack/transfers/__init__.py`

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

### Comparing `apache-airflow-providers-slack-7.2.0rc1/airflow/providers/slack/operators/slack.py` & `apache-airflow-providers-slack-7.3.0rc1/airflow/providers/slack/operators/slack.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from __future__ import annotations
 
 import json
 import warnings
 from typing import Any, Sequence
 
 from airflow.compat.functools import cached_property
+from airflow.exceptions import AirflowProviderDeprecationWarning
 from airflow.models import BaseOperator
 from airflow.providers.slack.hooks.slack import SlackHook
 from airflow.utils.log.secrets_masker import mask_secret
 
 
 class SlackAPIOperator(BaseOperator):
     """
@@ -207,15 +208,15 @@
         channel: str | None = None,
         **kwargs,
     ) -> None:
         if channel:
             warnings.warn(
                 "Argument `channel` is deprecated and will removed in a future releases. "
                 "Please use `channels` instead.",
-                DeprecationWarning,
+                AirflowProviderDeprecationWarning,
                 stacklevel=2,
             )
             if channels:
                 raise ValueError(f"Cannot set both arguments: channel={channel!r} and channels={channels!r}.")
             channels = channel
 
         self.channels = channels
```

### Comparing `apache-airflow-providers-slack-7.2.0rc1/airflow/providers/slack/operators/slack_webhook.py` & `apache-airflow-providers-slack-7.3.0rc1/airflow/providers/slack/operators/slack_webhook.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # under the License.
 from __future__ import annotations
 
 import warnings
 from typing import TYPE_CHECKING, Sequence
 
 from airflow.compat.functools import cached_property
-from airflow.exceptions import AirflowException
+from airflow.exceptions import AirflowException, AirflowProviderDeprecationWarning
 from airflow.models import BaseOperator
 from airflow.providers.slack.hooks.slack_webhook import SlackWebhookHook
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
@@ -92,15 +92,15 @@
         proxy: str | None = None,
         **kwargs,
     ) -> None:
         http_conn_id = kwargs.pop("http_conn_id", None)
         if http_conn_id:
             warnings.warn(
                 "Parameter `http_conn_id` is deprecated. Please use `slack_webhook_conn_id` instead.",
-                DeprecationWarning,
+                AirflowProviderDeprecationWarning,
                 stacklevel=2,
             )
             if slack_webhook_conn_id:
                 raise AirflowException("You cannot provide both `slack_webhook_conn_id` and `http_conn_id`.")
             slack_webhook_conn_id = http_conn_id
 
         # Compatibility with previous version of operator which based on SimpleHttpOperator.
@@ -126,15 +126,15 @@
                 deprecated_class_attrs.append(deprecated_attr)
                 kwargs.pop(deprecated_attr)
         if deprecated_class_attrs:
             warnings.warn(
                 f"Provide {','.join(repr(a) for a in deprecated_class_attrs)} is deprecated "
                 f"and as has no affect, please remove it from {self.__class__.__name__} "
                 "constructor attributes otherwise in future version of provider it might cause an issue.",
-                DeprecationWarning,
+                AirflowProviderDeprecationWarning,
                 stacklevel=2,
             )
 
         super().__init__(**kwargs)
         self.slack_webhook_conn_id = slack_webhook_conn_id
         self.webhook_token = webhook_token
         self.proxy = proxy
```

### Comparing `apache-airflow-providers-slack-7.2.0rc1/airflow/providers/slack/transfers/sql_to_slack.py` & `apache-airflow-providers-slack-7.3.0rc1/airflow/providers/slack/transfers/sql_to_slack.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-slack-7.2.0rc1/airflow/providers/slack/utils/__init__.py` & `apache-airflow-providers-slack-7.3.0rc1/airflow/providers/slack/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-slack-7.2.0rc1/apache_airflow_providers_slack.egg-info/PKG-INFO` & `apache-airflow-providers-slack-7.3.0rc1/apache_airflow_providers_slack.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-slack
-Version: 7.2.0rc1
+Version: 7.3.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-slack package
 Home-page: https://airflow.apache.org/
+Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Download-URL: https://archive.apache.org/dist/airflow/providers
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-slack/7.2.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-slack/7.3.0/
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
 
 
 Package ``apache-airflow-providers-slack``
 
-Release: ``7.2.0rc1``
+Release: ``7.3.0rc1``
 
 
 `Slack <https://slack.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``slack`` provider. All classes for this provider package
 are in ``airflow.providers.slack`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-slack/7.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-slack/7.3.0/>`_.
 
 
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
 ``slack_sdk``                            ``>=3.0.0``
 =======================================  ==================
 
 Cross provider package dependencies
 -----------------------------------
 
@@ -131,14 +130,35 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+7.3.0
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
+* ``Add Documentation for notification feature extension (#29191)``
+* ``Standardize Slack Notifier (#31244)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
+   * ``Prepare docs for Feb 2023 wave of Providers (#29379)``
+   * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Add mechanism to suspend providers (#30422)``
+
 7.2.0
 .....
 
 Features
 ~~~~~~~~
 
 * ``Add general-purpose "notifier" concept to DAGs (#28569)``
@@ -170,16 +190,17 @@
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Prepare for follow-up release for November providers (#27774)``
 
 7.0.0
 .....
 
-This release of provider is only available for Airflow 2.3+ as explained in the
-`Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/README.md#support-for-providers>`_.
+.. note::
+  This release of provider is only available for Airflow 2.3+ as explained in the
+  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
 * In SlackHook and SlackWebhookHook, if both ``extra__<conn type>__foo`` and ``foo`` existed
   in connection extra dict, the prefixed version would be used; now, the non-prefixed version
   will be preferred.  You'll see a warning if there is such a collision.
@@ -246,16 +267,17 @@
 
 5.0.0
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
 
@@ -408,9 +430,7 @@
 * ``Upgrade slack_sdk to v3 (#13745)``
 
 
 1.0.0
 .....
 
 Initial version of the provider.
-
-
```

### Comparing `apache-airflow-providers-slack-7.2.0rc1/apache_airflow_providers_slack.egg-info/SOURCES.txt` & `apache-airflow-providers-slack-7.3.0rc1/apache_airflow_providers_slack.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 setup.py
 airflow/providers/slack/__init__.py
 airflow/providers/slack/get_provider_info.py
 airflow/providers/slack/hooks/__init__.py
 airflow/providers/slack/hooks/slack.py
 airflow/providers/slack/hooks/slack_webhook.py
 airflow/providers/slack/notifications/__init__.py
+airflow/providers/slack/notifications/slack.py
 airflow/providers/slack/notifications/slack_notifier.py
 airflow/providers/slack/operators/__init__.py
 airflow/providers/slack/operators/slack.py
 airflow/providers/slack/operators/slack_webhook.py
 airflow/providers/slack/transfers/__init__.py
 airflow/providers/slack/transfers/sql_to_slack.py
 airflow/providers/slack/utils/__init__.py
```

### Comparing `apache-airflow-providers-slack-7.2.0rc1/pyproject.toml` & `apache-airflow-providers-slack-7.3.0rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-slack-7.2.0rc1/setup.cfg` & `apache-airflow-providers-slack-7.3.0rc1/setup.cfg`

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-slack/7.2.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-slack/7.3.0/
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
 	slack_sdk>=3.0.0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.slack.get_provider_info:get_provider_info
 
 [files]
```

### Comparing `apache-airflow-providers-slack-7.2.0rc1/setup.py` & `apache-airflow-providers-slack-7.3.0rc1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -22,21 +22,28 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-slack package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "7.2.0"
+version = "7.3.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-slack setup."""
     setup(
         version=version,
         extras_require={"common.sql": ["apache-airflow-providers-common-sql"]},
-        packages=find_namespace_packages(include=["airflow.providers.slack", "airflow.providers.slack.*"]),
+        packages=find_namespace_packages(
+            include=[
+                "airflow.providers.slack",
+                "airflow.providers.slack.*",
+                "airflow.providers.slack_vendor",
+                "airflow.providers.slack_vendor.*",
+            ],
+        ),
     )
 
 
 if __name__ == "__main__":
     do_setup()
```

