# Comparing `tmp/better_slack_logger-0.12.0.tar.gz` & `tmp/better_slack_logger-0.12.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "better_slack_logger-0.12.0.tar", max compression
+gzip compressed data, was "better_slack_logger-0.12.0.post1.tar", max compression
```

## Comparing `better_slack_logger-0.12.0.tar` & `better_slack_logger-0.12.0.post1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1066 2023-05-16 12:02:52.082080 better_slack_logger-0.12.0/LICENSE
--rw-r--r--   0        0        0     8478 2023-05-16 12:02:52.082080 better_slack_logger-0.12.0/README.md
--rw-r--r--   0        0        0     1409 2023-05-16 12:02:52.086080 better_slack_logger-0.12.0/pyproject.toml
--rw-r--r--   0        0        0       67 2023-05-16 12:02:52.086080 better_slack_logger-0.12.0/slack_logger/__init__.py
--rw-r--r--   0        0        0     5168 2023-05-16 12:02:52.086080 better_slack_logger-0.12.0/slack_logger/message_logger.py
--rw-r--r--   0        0        0      720 2023-05-16 12:02:52.086080 better_slack_logger-0.12.0/slack_logger/utils.py
--rw-r--r--   0        0        0     9860 1970-01-01 00:00:00.000000 better_slack_logger-0.12.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-05-16 12:07:28.007887 better_slack_logger-0.12.0.post1/LICENSE
+-rw-r--r--   0        0        0     8478 2023-05-16 12:07:28.007887 better_slack_logger-0.12.0.post1/README.md
+-rw-r--r--   0        0        0     1330 2023-05-16 12:07:28.011887 better_slack_logger-0.12.0.post1/pyproject.toml
+-rw-r--r--   0        0        0       67 2023-05-16 12:07:28.011887 better_slack_logger-0.12.0.post1/slack_logger/__init__.py
+-rw-r--r--   0        0        0     5168 2023-05-16 12:07:28.011887 better_slack_logger-0.12.0.post1/slack_logger/message_logger.py
+-rw-r--r--   0        0        0      720 2023-05-16 12:07:28.015888 better_slack_logger-0.12.0.post1/slack_logger/utils.py
+-rw-r--r--   0        0        0     9767 1970-01-01 00:00:00.000000 better_slack_logger-0.12.0.post1/PKG-INFO
```

### Comparing `better_slack_logger-0.12.0/LICENSE` & `better_slack_logger-0.12.0.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `better_slack_logger-0.12.0/README.md` & `better_slack_logger-0.12.0.post1/README.md`

 * *Files identical despite different names*

### Comparing `better_slack_logger-0.12.0/pyproject.toml` & `better_slack_logger-0.12.0.post1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 profile = "black"
 py_version = 38
 line_length = 100
 combine_as_imports = true
 
 [tool.poetry]
 name = "better-slack-logger"
-version = "0.12.0"
+version = "0.12.0.post1"
 description = "Slack Logger is a custom message logger to Slack for Python 3"
 authors = [
   "Chinni Chaitanya <chchaitanya95@gmail.com>",
   "Jay Turner <jaynicholasturner@gmail.com>",
 ]
 maintainers = ["Jay Turner <jaynicholasturner@gmail.com>"]
 license = "MIT License"
@@ -32,17 +32,15 @@
   "slack-api",
 ]
 classifiers = [
   "Environment :: Web Environment",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
-  "Programming Language :: Python :: 3.5",
-  "Programming Language :: Python :: 3.6",
-  "Programming Language :: Python :: 3.7",
+  "Programming Language :: Python :: 3.11",
   "Topic :: Internet :: WWW/HTTP",
   "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
 ]
 
 
 [tool.poetry.dependencies]
 python = ">=3.7"
```

### Comparing `better_slack_logger-0.12.0/slack_logger/message_logger.py` & `better_slack_logger-0.12.0.post1/slack_logger/message_logger.py`

 * *Files identical despite different names*

### Comparing `better_slack_logger-0.12.0/slack_logger/utils.py` & `better_slack_logger-0.12.0.post1/slack_logger/utils.py`

 * *Files identical despite different names*

### Comparing `better_slack_logger-0.12.0/PKG-INFO` & `better_slack_logger-0.12.0.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: better-slack-logger
-Version: 0.12.0
+Version: 0.12.0.post1
 Summary: Slack Logger is a custom message logger to Slack for Python 3
 Home-page: https://github.com/TurnrDev/better-slack-logger
 License: MIT
 Keywords: monitoring,slack,messaging,logging,health-check,notification-service,notification,slack-api
 Author: Chinni Chaitanya
 Author-email: chchaitanya95@gmail.com
 Maintainer: Jay Turner
@@ -16,17 +16,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Dist: pyyaml (>=5.1)
 Requires-Dist: slack-sdk (>=3.0.0)
 Project-URL: Repository, https://github.com/TurnrDev/better-slack-logger
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,34 +1,33 @@
-Metadata-Version: 2.1 Name: better-slack-logger Version: 0.12.0 Summary: Slack
-Logger is a custom message logger to Slack for Python 3 Home-page: https://
-github.com/TurnrDev/better-slack-logger License: MIT Keywords:
+Metadata-Version: 2.1 Name: better-slack-logger Version: 0.12.0.post1 Summary:
+Slack Logger is a custom message logger to Slack for Python 3 Home-page: https:
+//github.com/TurnrDev/better-slack-logger License: MIT Keywords:
 monitoring,slack,messaging,logging,health-check,notification-
 service,notification,slack-api Author: Chinni Chaitanya Author-email:
 chchaitanya95@gmail.com Maintainer: Jay Turner Maintainer-email:
 jaynicholasturner@gmail.com Requires-Python: >=3.7 Classifier: Environment ::
 Web Environment Classifier: Intended Audience :: Developers Classifier: License
 :: OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.5 Classifier: Programming
-Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
-Classifier: Topic :: Internet :: WWW/HTTP Classifier: Topic :: Internet :: WWW/
-HTTP :: Dynamic Content Requires-Dist: pyyaml (>=5.1) Requires-Dist: slack-sdk
-(>=3.0.0) Project-URL: Repository, https://github.com/TurnrDev/better-slack-
-logger Description-Content-Type: text/markdown # Better Slack Logger This is a
-fork is [`python-slack-logger`](https://github.com/chinnichaitanya/python-
-slack-logger) package by [Chaitanya Chinni](https://github.com/chinnichaitanya/
-). If using this, please remove that from your environment. A custom message
-logger to Slack for Python 3. This project was built using [`slackclient`]
-(https://github.com/slackapi/python-slackclient) and the latest [Block Kit UI]
-(https://api.slack.com/block-kit). [PyPI_-_Python_Version] [![PyPI version]
-(https://badge.fury.io/py/better-slack-logger.svg)](https://badge.fury.io/py/
-better-slack-logger) [Downloads] [PyPI_-_Wheel] [![License: MIT](https://
+Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
+Internet :: WWW/HTTP Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic
+Content Requires-Dist: pyyaml (>=5.1) Requires-Dist: slack-sdk (>=3.0.0)
+Project-URL: Repository, https://github.com/TurnrDev/better-slack-logger
+Description-Content-Type: text/markdown # Better Slack Logger This is a fork is
+[`python-slack-logger`](https://github.com/chinnichaitanya/python-slack-logger)
+package by [Chaitanya Chinni](https://github.com/chinnichaitanya/). If using
+this, please remove that from your environment. A custom message logger to
+Slack for Python 3. This project was built using [`slackclient`](https://
+github.com/slackapi/python-slackclient) and the latest [Block Kit UI](https://
+api.slack.com/block-kit). [PyPI_-_Python_Version] [![PyPI version](https://
+badge.fury.io/py/better-slack-logger.svg)](https://badge.fury.io/py/better-
+slack-logger) [Downloads] [PyPI_-_Wheel] [![License: MIT](https://
 img.shields.io/pypi/l/better-slack-logger)](https://github.com/TurnrDev/better-
 slack-logger/blob/master/LICENSE) [![Code style: black](https://img.shields.io/
 badge/code%20style-black-000000.svg)](https://github.com/python/black) ##
 Install Uninstall [`python-slack-logger`](https://github.com/chinnichaitanya/
 python-slack-logger) package by [Chaitanya Chinni](https://github.com/
 chinnichaitanya/) first: `pip uninstall python-slack-logger` Install via pip:
 `pip install better-slack-logger` ## Basic Usage ```python from slack_logger
```

