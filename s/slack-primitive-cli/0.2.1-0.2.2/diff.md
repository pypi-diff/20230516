# Comparing `tmp/slack_primitive_cli-0.2.1.tar.gz` & `tmp/slack_primitive_cli-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slack_primitive_cli-0.2.1.tar", max compression
+gzip compressed data, was "slack_primitive_cli-0.2.2.tar", max compression
```

## Comparing `slack_primitive_cli-0.2.1.tar` & `slack_primitive_cli-0.2.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1067 2023-05-15 07:50:24.563694 slack_primitive_cli-0.2.1/LICENSE
--rw-r--r--   0        0        0     6159 2023-05-15 07:50:24.563694 slack_primitive_cli-0.2.1/README.md
--rw-r--r--   0        0        0     1145 2023-05-15 07:50:47.443778 slack_primitive_cli-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       64 2023-05-15 07:50:24.563694 slack_primitive_cli-0.2.1/slack_primitive_cli/__init__.py
--rw-r--r--   0        0        0      414 2023-05-15 07:50:24.563694 slack_primitive_cli-0.2.1/slack_primitive_cli/__main__.py
--rw-r--r--   0        0        0      131 2023-05-15 07:50:47.443778 slack_primitive_cli-0.2.1/slack_primitive_cli/__version__.py
--rw-r--r--   0        0        0        0 2023-05-15 07:50:24.563694 slack_primitive_cli-0.2.1/slack_primitive_cli/command/__init__.py
--rw-r--r--   0        0        0     4259 2023-05-15 07:50:24.563694 slack_primitive_cli-0.2.1/slack_primitive_cli/command/chat.py
--rw-r--r--   0        0        0     2393 2023-05-15 07:50:24.563694 slack_primitive_cli-0.2.1/slack_primitive_cli/command/files.py
--rw-r--r--   0        0        0        0 2023-05-15 07:50:24.563694 slack_primitive_cli-0.2.1/slack_primitive_cli/common/__init__.py
--rw-r--r--   0        0        0     1247 2023-05-15 07:50:24.563694 slack_primitive_cli-0.2.1/slack_primitive_cli/common/utils.py
--rw-r--r--   0        0        0     7152 1970-01-01 00:00:00.000000 slack_primitive_cli-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-05-16 03:50:16.610510 slack_primitive_cli-0.2.2/LICENSE
+-rw-r--r--   0        0        0     6303 2023-05-16 03:50:16.610510 slack_primitive_cli-0.2.2/README.md
+-rw-r--r--   0        0        0     1093 2023-05-16 03:50:33.043161 slack_primitive_cli-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0       64 2023-05-16 03:50:16.610510 slack_primitive_cli-0.2.2/slack_primitive_cli/__init__.py
+-rw-r--r--   0        0        0      414 2023-05-16 03:50:16.610510 slack_primitive_cli-0.2.2/slack_primitive_cli/__main__.py
+-rw-r--r--   0        0        0      131 2023-05-16 03:50:33.047161 slack_primitive_cli-0.2.2/slack_primitive_cli/__version__.py
+-rw-r--r--   0        0        0        0 2023-05-16 03:50:16.610510 slack_primitive_cli-0.2.2/slack_primitive_cli/command/__init__.py
+-rw-r--r--   0        0        0     4259 2023-05-16 03:50:16.610510 slack_primitive_cli-0.2.2/slack_primitive_cli/command/chat.py
+-rw-r--r--   0        0        0     2393 2023-05-16 03:50:16.610510 slack_primitive_cli-0.2.2/slack_primitive_cli/command/files.py
+-rw-r--r--   0        0        0        0 2023-05-16 03:50:16.610510 slack_primitive_cli-0.2.2/slack_primitive_cli/common/__init__.py
+-rw-r--r--   0        0        0     1247 2023-05-16 03:50:16.610510 slack_primitive_cli-0.2.2/slack_primitive_cli/common/utils.py
+-rw-r--r--   0        0        0     7231 1970-01-01 00:00:00.000000 slack_primitive_cli-0.2.2/PKG-INFO
```

### Comparing `slack_primitive_cli-0.2.1/LICENSE` & `slack_primitive_cli-0.2.2/LICENSE`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2020 yuji38kwmt
+Copyright (c) 2020 Kurusugawa Computer Inc.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `slack_primitive_cli-0.2.1/README.md` & `slack_primitive_cli-0.2.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # slack-primitive-cli
-[![Build Status](https://travis-ci.org/yuji38kwmt/slack-primitive-cli.svg?branch=master)](https://travis-ci.org/yuji38kwmt/slack-primitive-cli)
+[![Build Status](https://travis-ci.org/kurusugawa-computer/slack-primitive-cli.svg?branch=main)](https://travis-ci.org/kurusugawa-computer/slack-primitive-cli)
 [![PyPI version](https://badge.fury.io/py/slack-primitive-cli.svg)](https://badge.fury.io/py/slack-primitive-cli)
 [![Python Versions](https://img.shields.io/pypi/pyversions/slack-primitive-cli.svg)](https://pypi.org/project/slack-primitive-cli/)
 
 `slack-primitive-cli` can execute [Slack web api methods](https://api.slack.com/methods) from command line.
 Command line argument is correspont to web api arguments, so `slack-primitive-cli` is **primitive**.
 
 
 # Requirements
-* Python 3.7+
+* Python 3.8.1+
 
 # Install
 
 ```
 $ pip install slack-primitive-cli
 ```
 
@@ -156,7 +156,10 @@
 ```
 $ eval "$(_SLACKCLI_COMPLETE=source slackcli)"
 ```
 
 
 See [here](https://click.palletsprojects.com/en/7.x/bashcomplete/) for details.
 
+
+# Usage for Developer
+Refer to https://github.com/kurusugawa-computer/slack-primitive-cli/blob/main/README_for_developer.md .
```

### Comparing `slack_primitive_cli-0.2.1/pyproject.toml` & `slack_primitive_cli-0.2.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 [tool.poetry]
 name = "slack-primitive-cli"
-version = "0.2.1"  # `poetry-dynamic-versioning`を使ってGitHubのバージョンタグを取得している。変更不要
+version = "0.2.2"  # `poetry-dynamic-versioning`を使ってGitHubのバージョンタグを取得している。変更不要
 description = "Primitive Slack CLI"
-authors = ["yuji38kwmt <yuji38kwmt@gmail.com>"]
-maintainers = ["yuji38kwmt <yuji38kwmt@gmail.com>"]
+authors = ["Kurusugawa Computer Inc."]
 keywords=["slack", "cli"]
 license="MIT"
 readme="README.md"
-repository="https://github.com/yuji38kwmt/slack-primitive-cli"
+repository="https://github.com/kurusugawa-computer/slack-primitive-cli"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Intended Audience :: Developers",
     "Topic :: Utilities",
     "Operating System :: OS Independent",
 ]
```

### Comparing `slack_primitive_cli-0.2.1/slack_primitive_cli/command/chat.py` & `slack_primitive_cli-0.2.2/slack_primitive_cli/command/chat.py`

 * *Files identical despite different names*

### Comparing `slack_primitive_cli-0.2.1/slack_primitive_cli/command/files.py` & `slack_primitive_cli-0.2.2/slack_primitive_cli/command/files.py`

 * *Files identical despite different names*

### Comparing `slack_primitive_cli-0.2.1/slack_primitive_cli/common/utils.py` & `slack_primitive_cli-0.2.2/slack_primitive_cli/common/utils.py`

 * *Files identical despite different names*

### Comparing `slack_primitive_cli-0.2.1/PKG-INFO` & `slack_primitive_cli-0.2.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,46 +1,43 @@
 Metadata-Version: 2.1
 Name: slack-primitive-cli
-Version: 0.2.1
+Version: 0.2.2
 Summary: Primitive Slack CLI
-Home-page: https://github.com/yuji38kwmt/slack-primitive-cli
+Home-page: https://github.com/kurusugawa-computer/slack-primitive-cli
 License: MIT
 Keywords: slack,cli
-Author: yuji38kwmt
-Author-email: yuji38kwmt@gmail.com
-Maintainer: yuji38kwmt
-Maintainer-email: yuji38kwmt@gmail.com
+Author: Kurusugawa Computer Inc.
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Requires-Dist: backoff
 Requires-Dist: click (>=8,<9)
 Requires-Dist: click-option-group
 Requires-Dist: slack-sdk (>=3,<4)
-Project-URL: Repository, https://github.com/yuji38kwmt/slack-primitive-cli
+Project-URL: Repository, https://github.com/kurusugawa-computer/slack-primitive-cli
 Description-Content-Type: text/markdown
 
 # slack-primitive-cli
-[![Build Status](https://travis-ci.org/yuji38kwmt/slack-primitive-cli.svg?branch=master)](https://travis-ci.org/yuji38kwmt/slack-primitive-cli)
+[![Build Status](https://travis-ci.org/kurusugawa-computer/slack-primitive-cli.svg?branch=main)](https://travis-ci.org/kurusugawa-computer/slack-primitive-cli)
 [![PyPI version](https://badge.fury.io/py/slack-primitive-cli.svg)](https://badge.fury.io/py/slack-primitive-cli)
 [![Python Versions](https://img.shields.io/pypi/pyversions/slack-primitive-cli.svg)](https://pypi.org/project/slack-primitive-cli/)
 
 `slack-primitive-cli` can execute [Slack web api methods](https://api.slack.com/methods) from command line.
 Command line argument is correspont to web api arguments, so `slack-primitive-cli` is **primitive**.
 
 
 # Requirements
-* Python 3.7+
+* Python 3.8.1+
 
 # Install
 
 ```
 $ pip install slack-primitive-cli
 ```
 
@@ -185,7 +182,9 @@
 $ eval "$(_SLACKCLI_COMPLETE=source slackcli)"
 ```
 
 
 See [here](https://click.palletsprojects.com/en/7.x/bashcomplete/) for details.
 
 
+# Usage for Developer
+Refer to https://github.com/kurusugawa-computer/slack-primitive-cli/blob/main/README_for_developer.md .
```

