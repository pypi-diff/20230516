# Comparing `tmp/jira_agile_toolbox-0.0.8.tar.gz` & `tmp/jira_agile_toolbox-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jira_agile_toolbox-0.0.8.tar", last modified: Sun May 16 00:35:07 2021, max compression
+gzip compressed data, was "jira_agile_toolbox-0.0.9.tar", last modified: Fri Jun  4 17:08:20 2021, max compression
```

## Comparing `jira_agile_toolbox-0.0.8.tar` & `jira_agile_toolbox-0.0.9.tar`

### file list

```diff
@@ -1,39 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-16 00:35:07.632753 jira_agile_toolbox-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1107 2021-05-16 00:34:58.000000 jira_agile_toolbox-0.0.8/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-16 00:35:07.628753 jira_agile_toolbox-0.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-16 00:35:07.632753 jira_agile_toolbox-0.0.8/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      677 2021-05-16 00:34:58.000000 jira_agile_toolbox-0.0.8/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (121)      617 2021-05-16 00:34:58.000000 jira_agile_toolbox-0.0.8/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-16 00:35:07.632753 jira_agile_toolbox-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1710 2021-05-16 00:34:58.000000 jira_agile_toolbox-0.0.8/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (121)      918 2021-05-16 00:34:58.000000 jira_agile_toolbox-0.0.8/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)     4591 2021-05-16 00:34:58.000000 jira_agile_toolbox-0.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      160 2021-05-16 00:34:58.000000 jira_agile_toolbox-0.0.8/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     5475 2021-05-16 00:34:58.000000 jira_agile_toolbox-0.0.8/CODE_OF_CONDUCT.MD
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2021-05-16 00:34:58.000000 jira_agile_toolbox-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3497 2021-05-16 00:35:07.632753 jira_agile_toolbox-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1562 2021-05-16 00:34:58.000000 jira_agile_toolbox-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-16 00:35:07.632753 jira_agile_toolbox-0.0.8/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      638 2021-05-16 00:34:58.000000 jira_agile_toolbox-0.0.8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      764 2021-05-16 00:34:58.000000 jira_agile_toolbox-0.0.8/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-16 00:35:07.632753 jira_agile_toolbox-0.0.8/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-16 00:35:07.628753 jira_agile_toolbox-0.0.8/docs/source/_static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-16 00:35:07.632753 jira_agile_toolbox-0.0.8/docs/source/_static/css/
--rw-r--r--   0 runner    (1001) docker     (121)      129 2021-05-16 00:34:58.000000 jira_agile_toolbox-0.0.8/docs/source/_static/css/custom_width.css
--rw-r--r--   0 runner    (1001) docker     (121)     2094 2021-05-16 00:34:58.000000 jira_agile_toolbox-0.0.8/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      501 2021-05-16 00:34:58.000000 jira_agile_toolbox-0.0.8/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-16 00:35:07.632753 jira_agile_toolbox-0.0.8/jira_agile_toolbox/
--rw-r--r--   0 runner    (1001) docker     (121)     5797 2021-05-16 00:34:58.000000 jira_agile_toolbox-0.0.8/jira_agile_toolbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-16 00:34:58.000000 jira_agile_toolbox-0.0.8/jira_agile_toolbox/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-16 00:35:07.632753 jira_agile_toolbox-0.0.8/jira_agile_toolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3497 2021-05-16 00:35:07.000000 jira_agile_toolbox-0.0.8/jira_agile_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      703 2021-05-16 00:35:07.000000 jira_agile_toolbox-0.0.8/jira_agile_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-16 00:35:07.000000 jira_agile_toolbox-0.0.8/jira_agile_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2021-05-16 00:35:07.000000 jira_agile_toolbox-0.0.8/jira_agile_toolbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2021-05-16 00:35:07.000000 jira_agile_toolbox-0.0.8/jira_agile_toolbox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2021-05-16 00:34:58.000000 jira_agile_toolbox-0.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1532 2021-05-16 00:35:07.632753 jira_agile_toolbox-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      104 2021-05-16 00:34:58.000000 jira_agile_toolbox-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-16 00:35:07.632753 jira_agile_toolbox-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     8300 2021-05-16 00:34:58.000000 jira_agile_toolbox-0.0.8/tests/test_epic_interactions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2498 2021-05-16 00:34:58.000000 jira_agile_toolbox-0.0.8/tests/test_ranking.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-04 17:08:20.679618 jira_agile_toolbox-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1107 2021-06-04 17:08:09.000000 jira_agile_toolbox-0.0.9/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-04 17:08:20.667618 jira_agile_toolbox-0.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-04 17:08:20.671618 jira_agile_toolbox-0.0.9/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      677 2021-06-04 17:08:09.000000 jira_agile_toolbox-0.0.9/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (121)      617 2021-06-04 17:08:09.000000 jira_agile_toolbox-0.0.9/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-04 17:08:20.675618 jira_agile_toolbox-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     1710 2021-06-04 17:08:09.000000 jira_agile_toolbox-0.0.9/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      918 2021-06-04 17:08:09.000000 jira_agile_toolbox-0.0.9/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     4591 2021-06-04 17:08:09.000000 jira_agile_toolbox-0.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      160 2021-06-04 17:08:09.000000 jira_agile_toolbox-0.0.9/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     5475 2021-06-04 17:08:09.000000 jira_agile_toolbox-0.0.9/CODE_OF_CONDUCT.MD
+-rw-r--r--   0 runner    (1001) docker     (121)     1064 2021-06-04 17:08:09.000000 jira_agile_toolbox-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     3076 2021-06-04 17:08:20.679618 jira_agile_toolbox-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1562 2021-06-04 17:08:09.000000 jira_agile_toolbox-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-04 17:08:20.675618 jira_agile_toolbox-0.0.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)      638 2021-06-04 17:08:09.000000 jira_agile_toolbox-0.0.9/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)      764 2021-06-04 17:08:09.000000 jira_agile_toolbox-0.0.9/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-04 17:08:20.675618 jira_agile_toolbox-0.0.9/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-04 17:08:20.667618 jira_agile_toolbox-0.0.9/docs/source/_static/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-04 17:08:20.675618 jira_agile_toolbox-0.0.9/docs/source/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (121)      129 2021-06-04 17:08:09.000000 jira_agile_toolbox-0.0.9/docs/source/_static/css/custom_width.css
+-rw-r--r--   0 runner    (1001) docker     (121)     2094 2021-06-04 17:08:09.000000 jira_agile_toolbox-0.0.9/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      501 2021-06-04 17:08:09.000000 jira_agile_toolbox-0.0.9/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-04 17:08:20.675618 jira_agile_toolbox-0.0.9/jira_agile_toolbox/
+-rw-r--r--   0 runner    (1001) docker     (121)     9371 2021-06-04 17:08:09.000000 jira_agile_toolbox-0.0.9/jira_agile_toolbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-04 17:08:09.000000 jira_agile_toolbox-0.0.9/jira_agile_toolbox/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-04 17:08:20.679618 jira_agile_toolbox-0.0.9/jira_agile_toolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3076 2021-06-04 17:08:20.000000 jira_agile_toolbox-0.0.9/jira_agile_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      759 2021-06-04 17:08:20.000000 jira_agile_toolbox-0.0.9/jira_agile_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-04 17:08:20.000000 jira_agile_toolbox-0.0.9/jira_agile_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       20 2021-06-04 17:08:20.000000 jira_agile_toolbox-0.0.9/jira_agile_toolbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       19 2021-06-04 17:08:20.000000 jira_agile_toolbox-0.0.9/jira_agile_toolbox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       11 2021-06-04 17:08:09.000000 jira_agile_toolbox-0.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1532 2021-06-04 17:08:20.679618 jira_agile_toolbox-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      104 2021-06-04 17:08:09.000000 jira_agile_toolbox-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-04 17:08:20.679618 jira_agile_toolbox-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)     1126 2021-06-04 17:08:09.000000 jira_agile_toolbox-0.0.9/tests/lib_for_tests.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9573 2021-06-04 17:08:09.000000 jira_agile_toolbox-0.0.9/tests/test_epic_interactions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2608 2021-06-04 17:08:09.000000 jira_agile_toolbox-0.0.9/tests/test_label_interactions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2498 2021-06-04 17:08:09.000000 jira_agile_toolbox-0.0.9/tests/test_ranking.py
```

### Comparing `jira_agile_toolbox-0.0.8/.gitattributes` & `jira_agile_toolbox-0.0.9/.gitattributes`

 * *Files identical despite different names*

### Comparing `jira_agile_toolbox-0.0.8/.github/ISSUE_TEMPLATE/bug_report.md` & `jira_agile_toolbox-0.0.9/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `jira_agile_toolbox-0.0.8/.github/ISSUE_TEMPLATE/feature_request.md` & `jira_agile_toolbox-0.0.9/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `jira_agile_toolbox-0.0.8/.github/workflows/python-package.yml` & `jira_agile_toolbox-0.0.9/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `jira_agile_toolbox-0.0.8/.github/workflows/python-publish.yml` & `jira_agile_toolbox-0.0.9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `jira_agile_toolbox-0.0.8/.gitignore` & `jira_agile_toolbox-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `jira_agile_toolbox-0.0.8/CODE_OF_CONDUCT.MD` & `jira_agile_toolbox-0.0.9/CODE_OF_CONDUCT.MD`

 * *Files identical despite different names*

### Comparing `jira_agile_toolbox-0.0.8/LICENSE` & `jira_agile_toolbox-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `jira_agile_toolbox-0.0.8/PKG-INFO` & `jira_agile_toolbox-0.0.9/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,69 +1,14 @@
 Metadata-Version: 2.1
 Name: jira_agile_toolbox
-Version: 0.0.8
+Version: 0.0.9
 Summary: Extends standard jira package with agile specific tooling for metrics and administration
 Home-page: https://github.com/studioj/jira-agile-toolbox
 Author: Jef Neefs
 License: MIT
-Description: # jira_agile_toolbox
-        
-        ![python package workflow](https://github.com/studioj/jira-agile-toolbox/actions/workflows/python-publish.yml/badge.svg)
-        ![python package workflow](https://github.com/studioj/jira-agile-toolbox/actions/workflows/python-package.yml/badge.svg)
-        
-        A python package which extends the jira package with agile related functionality
-        
-        For more info about the jira package
-        
-        - PyPi: https://pypi.org/project/jira/
-        - rtd:  https://jira.readthedocs.io/en/latest/
-        
-        ## Installation
-        ```bash
-        pip install jira-agile-toolbox
-        ```
-        
-        ## Documentation
-        https://jira-agile-toolbox.readthedocs.io/
-        
-        ## Features
-        
-        - ### Getting story points from an epic
-        
-        Example:
-        ```python
-        >>> from jira_agile_toolbox import JiraAgileToolBox
-        >>> from jira import JIRA
-        >>> my_jira_client = JIRA("https://my-jira-server.com", basic_auth("MYUSERNAME","MYPASSWORD")
-        >>> tb = JiraAgileToolBox(my_jira_client)
-        >>> tb.get_storypoints_from_epic("JAT-001")
-        {'total': 100, "Reported": 50, "Closed": 50}
-        ```
-        
-        - ### Ranking a list of epics on top of another one
-        
-        Example:
-        ```python
-        >>> from jira_agile_toolbox import JiraAgileToolBox
-        >>> from jira import JIRA
-        >>> my_jira_client = JIRA("https://my-jira-server.com", basic_auth("MYUSERNAME","MYPASSWORD")
-        >>> tb = JiraAgileToolBox(my_jira_client)
-        >>> tb.rank_issues_by_list([my_jira_client.issue("JAT-001"), my_jira_client.issue("JAT-003")], my_jira_client.issue("JAT-005"))
-        ```
-        
-        will rank issues like:
-        
-        | original | result |
-        | -------- | ------ |
-        | JAT-010 | JAT-010
-        | JAT-005 | JAT-001
-        | JAT-003 | JAT-003 
-        | JAT-002 | JAT-005
-        | JAT-001 | JAT-002
-        
 Keywords: api,atlassian,jira,rest,web,agile,scrum,kanban
 Platform: unix
 Platform: linux
 Platform: osx
 Platform: cygwin
 Platform: win32
 Classifier: Development Status :: 1 - Planning
@@ -86,7 +31,65 @@
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
+License-File: LICENSE
+
+# jira_agile_toolbox
+
+![python package workflow](https://github.com/studioj/jira-agile-toolbox/actions/workflows/python-publish.yml/badge.svg)
+![python package workflow](https://github.com/studioj/jira-agile-toolbox/actions/workflows/python-package.yml/badge.svg)
+
+A python package which extends the jira package with agile related functionality
+
+For more info about the jira package
+
+- PyPi: https://pypi.org/project/jira/
+- rtd:  https://jira.readthedocs.io/en/latest/
+
+## Installation
+```bash
+pip install jira-agile-toolbox
+```
+
+## Documentation
+https://jira-agile-toolbox.readthedocs.io/
+
+## Features
+
+- ### Getting story points from an epic
+
+Example:
+```python
+>>> from jira_agile_toolbox import JiraAgileToolBox
+>>> from jira import JIRA
+>>> my_jira_client = JIRA("https://my-jira-server.com", basic_auth("MYUSERNAME","MYPASSWORD")
+>>> tb = JiraAgileToolBox(my_jira_client)
+>>> tb.get_storypoints_from_epic("JAT-001")
+{'total': 100, "Reported": 50, "Closed": 50}
+```
+
+- ### Ranking a list of epics on top of another one
+
+Example:
+```python
+>>> from jira_agile_toolbox import JiraAgileToolBox
+>>> from jira import JIRA
+>>> my_jira_client = JIRA("https://my-jira-server.com", basic_auth("MYUSERNAME","MYPASSWORD")
+>>> tb = JiraAgileToolBox(my_jira_client)
+>>> tb.rank_issues_by_list([my_jira_client.issue("JAT-001"), my_jira_client.issue("JAT-003")], my_jira_client.issue("JAT-005"))
+```
+
+will rank issues like:
+
+| original | result |
+| -------- | ------ |
+| JAT-010 | JAT-010
+| JAT-005 | JAT-001
+| JAT-003 | JAT-003 
+| JAT-002 | JAT-005
+| JAT-001 | JAT-002
+
+
```

### Comparing `jira_agile_toolbox-0.0.8/README.md` & `jira_agile_toolbox-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `jira_agile_toolbox-0.0.8/docs/Makefile` & `jira_agile_toolbox-0.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jira_agile_toolbox-0.0.8/docs/make.bat` & `jira_agile_toolbox-0.0.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `jira_agile_toolbox-0.0.8/docs/source/conf.py` & `jira_agile_toolbox-0.0.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `jira_agile_toolbox-0.0.8/jira_agile_toolbox.egg-info/PKG-INFO` & `jira_agile_toolbox-0.0.9/jira_agile_toolbox.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,69 +1,14 @@
 Metadata-Version: 2.1
 Name: jira-agile-toolbox
-Version: 0.0.8
+Version: 0.0.9
 Summary: Extends standard jira package with agile specific tooling for metrics and administration
 Home-page: https://github.com/studioj/jira-agile-toolbox
 Author: Jef Neefs
 License: MIT
-Description: # jira_agile_toolbox
-        
-        ![python package workflow](https://github.com/studioj/jira-agile-toolbox/actions/workflows/python-publish.yml/badge.svg)
-        ![python package workflow](https://github.com/studioj/jira-agile-toolbox/actions/workflows/python-package.yml/badge.svg)
-        
-        A python package which extends the jira package with agile related functionality
-        
-        For more info about the jira package
-        
-        - PyPi: https://pypi.org/project/jira/
-        - rtd:  https://jira.readthedocs.io/en/latest/
-        
-        ## Installation
-        ```bash
-        pip install jira-agile-toolbox
-        ```
-        
-        ## Documentation
-        https://jira-agile-toolbox.readthedocs.io/
-        
-        ## Features
-        
-        - ### Getting story points from an epic
-        
-        Example:
-        ```python
-        >>> from jira_agile_toolbox import JiraAgileToolBox
-        >>> from jira import JIRA
-        >>> my_jira_client = JIRA("https://my-jira-server.com", basic_auth("MYUSERNAME","MYPASSWORD")
-        >>> tb = JiraAgileToolBox(my_jira_client)
-        >>> tb.get_storypoints_from_epic("JAT-001")
-        {'total': 100, "Reported": 50, "Closed": 50}
-        ```
-        
-        - ### Ranking a list of epics on top of another one
-        
-        Example:
-        ```python
-        >>> from jira_agile_toolbox import JiraAgileToolBox
-        >>> from jira import JIRA
-        >>> my_jira_client = JIRA("https://my-jira-server.com", basic_auth("MYUSERNAME","MYPASSWORD")
-        >>> tb = JiraAgileToolBox(my_jira_client)
-        >>> tb.rank_issues_by_list([my_jira_client.issue("JAT-001"), my_jira_client.issue("JAT-003")], my_jira_client.issue("JAT-005"))
-        ```
-        
-        will rank issues like:
-        
-        | original | result |
-        | -------- | ------ |
-        | JAT-010 | JAT-010
-        | JAT-005 | JAT-001
-        | JAT-003 | JAT-003 
-        | JAT-002 | JAT-005
-        | JAT-001 | JAT-002
-        
 Keywords: api,atlassian,jira,rest,web,agile,scrum,kanban
 Platform: unix
 Platform: linux
 Platform: osx
 Platform: cygwin
 Platform: win32
 Classifier: Development Status :: 1 - Planning
@@ -86,7 +31,65 @@
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
+License-File: LICENSE
+
+# jira_agile_toolbox
+
+![python package workflow](https://github.com/studioj/jira-agile-toolbox/actions/workflows/python-publish.yml/badge.svg)
+![python package workflow](https://github.com/studioj/jira-agile-toolbox/actions/workflows/python-package.yml/badge.svg)
+
+A python package which extends the jira package with agile related functionality
+
+For more info about the jira package
+
+- PyPi: https://pypi.org/project/jira/
+- rtd:  https://jira.readthedocs.io/en/latest/
+
+## Installation
+```bash
+pip install jira-agile-toolbox
+```
+
+## Documentation
+https://jira-agile-toolbox.readthedocs.io/
+
+## Features
+
+- ### Getting story points from an epic
+
+Example:
+```python
+>>> from jira_agile_toolbox import JiraAgileToolBox
+>>> from jira import JIRA
+>>> my_jira_client = JIRA("https://my-jira-server.com", basic_auth("MYUSERNAME","MYPASSWORD")
+>>> tb = JiraAgileToolBox(my_jira_client)
+>>> tb.get_storypoints_from_epic("JAT-001")
+{'total': 100, "Reported": 50, "Closed": 50}
+```
+
+- ### Ranking a list of epics on top of another one
+
+Example:
+```python
+>>> from jira_agile_toolbox import JiraAgileToolBox
+>>> from jira import JIRA
+>>> my_jira_client = JIRA("https://my-jira-server.com", basic_auth("MYUSERNAME","MYPASSWORD")
+>>> tb = JiraAgileToolBox(my_jira_client)
+>>> tb.rank_issues_by_list([my_jira_client.issue("JAT-001"), my_jira_client.issue("JAT-003")], my_jira_client.issue("JAT-005"))
+```
+
+will rank issues like:
+
+| original | result |
+| -------- | ------ |
+| JAT-010 | JAT-010
+| JAT-005 | JAT-001
+| JAT-003 | JAT-003 
+| JAT-002 | JAT-005
+| JAT-001 | JAT-002
+
+
```

### Comparing `jira_agile_toolbox-0.0.8/jira_agile_toolbox.egg-info/SOURCES.txt` & `jira_agile_toolbox-0.0.9/jira_agile_toolbox.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -19,9 +19,11 @@
 jira_agile_toolbox/__init__.py
 jira_agile_toolbox/version.py
 jira_agile_toolbox.egg-info/PKG-INFO
 jira_agile_toolbox.egg-info/SOURCES.txt
 jira_agile_toolbox.egg-info/dependency_links.txt
 jira_agile_toolbox.egg-info/requires.txt
 jira_agile_toolbox.egg-info/top_level.txt
+tests/lib_for_tests.py
 tests/test_epic_interactions.py
+tests/test_label_interactions.py
 tests/test_ranking.py
```

### Comparing `jira_agile_toolbox-0.0.8/setup.cfg` & `jira_agile_toolbox-0.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `jira_agile_toolbox-0.0.8/tests/test_epic_interactions.py` & `jira_agile_toolbox-0.0.9/tests/test_epic_interactions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,173 +1,149 @@
 from unittest import TestCase
-from unittest.mock import Mock, MagicMock
+from unittest.mock import Mock
 
 import jira
 
 from jira_agile_toolbox import JiraAgileToolBox
-
-DEFAULT_FIELDS_RETURN_VALUE = [
-    {
-        "id": "customfield_11280",
-        "name": "Release Note",
-        "custom": True,
-        "orderable": True,
-        "navigable": True,
-        "searchable": True,
-        "clauseNames": ["cf[11280]", "Release Note"],
-        "schema": {"type": "option", "custom": "com.atlassian.jira.plugin.system.customfieldtypes:select", "customId": 11280},
-    },
-    {
-        "id": "customfield_10282",
-        "name": "Story Points",
-        "custom": True,
-        "orderable": True,
-        "navigable": True,
-        "searchable": True,
-        "clauseNames": ["cf[10282]", "Story Points"],
-        "schema": {"type": "number", "custom": "com.atlassian.jira.plugin.system.customfieldtypes:float", "customId": 10282},
-    },
-]
-
-
-class MockedJiraIssue(jira.Issue):
-    def __init__(self, story_points=None, status="Reported"):
-        self.fields = MagicMock()
-        self.fields.customfield_10282 = story_points
-        self.fields.status.name = status
+from lib_for_tests import DEFAULT_FIELDS_RETURN_VALUE, MockedJiraIssue
 
 
 class TestEpicStoryPointRetrieval(TestCase):
+    def setUp(self) -> None:
+        self.jira_client = Mock(spec=jira.JIRA)
+
     def test_get_story_points_from_epic_returns_a_dict_containing_the_total_story_points(self):
         # Given
-        jira_client = Mock()
-        jira_client.fields.return_value = DEFAULT_FIELDS_RETURN_VALUE
-        jira_client.search_issues.return_value = [
+
+        self.jira_client.fields.return_value = DEFAULT_FIELDS_RETURN_VALUE
+        self.jira_client.search_issues.return_value = [
             MockedJiraIssue(story_points=0),
             MockedJiraIssue(story_points=1),
             MockedJiraIssue(story_points=2),
         ]
-        jat = JiraAgileToolBox(jira_client)
+        jat = JiraAgileToolBox(self.jira_client)
 
         # When
         result = jat.get_storypoints_from_epic("PROJ001-001")
 
         # Then
         self.assertIn("total", result.keys())
 
     def test_get_story_points_from_epic_looks_in_jira_for_all_children_of_the_epic(self):
         # Given
-        jira_client = Mock()
-        jira_client.fields.return_value = DEFAULT_FIELDS_RETURN_VALUE
-        jira_client.search_issues.return_value = [
+
+        self.jira_client.fields.return_value = DEFAULT_FIELDS_RETURN_VALUE
+        self.jira_client.search_issues.return_value = [
             MockedJiraIssue(story_points=0),
             MockedJiraIssue(story_points=1),
             MockedJiraIssue(story_points=2),
         ]
-        jat = JiraAgileToolBox(jira_client)
+        jat = JiraAgileToolBox(self.jira_client)
 
         # When
         jat.get_storypoints_from_epic("PROJ001-001")
 
         # Then
-        jira_client.search_issues.assert_called_with("'Epic Link' = " + "PROJ001-001", fields=["customfield_10282", "status"], maxResults=0)
+        self.jira_client.search_issues.assert_called_with(
+            "'Epic Link' = " + "PROJ001-001", fields=["customfield_10282", "status"], maxResults=0
+        )
 
     def test_get_story_points_from_epic_calculates_the_total_story_pointS_for_3_issues(self):
         # Given
-        jira_client = Mock()
-        jira_client.fields.return_value = DEFAULT_FIELDS_RETURN_VALUE
-        jira_client.search_issues.return_value = [
+
+        self.jira_client.fields.return_value = DEFAULT_FIELDS_RETURN_VALUE
+        self.jira_client.search_issues.return_value = [
             MockedJiraIssue(story_points=0),
             MockedJiraIssue(story_points=1),
             MockedJiraIssue(story_points=2),
         ]
-        jat = JiraAgileToolBox(jira_client)
+        jat = JiraAgileToolBox(self.jira_client)
 
         # When
         sps = jat.get_storypoints_from_epic("PROJ001-001")
 
         # Then
         self.assertEqual(3, sps["total"])
 
     def test_get_story_points_from_epic_calculates_the_total_story_pointS_for_300_issues(self):
         # Given
-        jira_client = Mock()
-        jira_client.fields.return_value = DEFAULT_FIELDS_RETURN_VALUE
-        jira_client.search_issues.return_value = [
+
+        self.jira_client.fields.return_value = DEFAULT_FIELDS_RETURN_VALUE
+        self.jira_client.search_issues.return_value = [
             MockedJiraIssue(story_points=0),
             MockedJiraIssue(story_points=1),
             MockedJiraIssue(story_points=2),
         ] * 100
-        jat = JiraAgileToolBox(jira_client)
+        jat = JiraAgileToolBox(self.jira_client)
 
         # When
         sps = jat.get_storypoints_from_epic("PROJ001-001")
 
         # Then
         self.assertEqual(300, sps["total"])
 
     def test_get_story_points_from_epic_calculates_the_total_of_zero_story_point_when_none_are_assigned(self):
         # Given
-        jira_client = Mock()
-        jira_client.fields.return_value = DEFAULT_FIELDS_RETURN_VALUE
-        jira_client.search_issues.return_value = [
+
+        self.jira_client.fields.return_value = DEFAULT_FIELDS_RETURN_VALUE
+        self.jira_client.search_issues.return_value = [
             MockedJiraIssue(story_points=None),
             MockedJiraIssue(),
             MockedJiraIssue(),
         ] * 1000
-        jat = JiraAgileToolBox(jira_client)
+        jat = JiraAgileToolBox(self.jira_client)
 
         # When
         sps = jat.get_storypoints_from_epic("PROJ001-001")
 
         # Then
         self.assertEqual(0, sps["total"])
 
     def test_get_story_points_from_epic_returns_a_dict_containing_the_found_statuses_as_keyword(self):
         # Given
-        jira_client = Mock()
-        jira_client.fields.return_value = DEFAULT_FIELDS_RETURN_VALUE
-        jira_client.search_issues.return_value = [
+
+        self.jira_client.fields.return_value = DEFAULT_FIELDS_RETURN_VALUE
+        self.jira_client.search_issues.return_value = [
             MockedJiraIssue(0, "Reported"),
             MockedJiraIssue(1, "Investigated"),
             MockedJiraIssue(2, "Closed"),
         ]
-        jat = JiraAgileToolBox(jira_client)
+        jat = JiraAgileToolBox(self.jira_client)
 
         # When
         result = jat.get_storypoints_from_epic("PROJ001-001")
 
         # Then
         self.assertIn("Reported", result.keys())
         self.assertIn("Investigated", result.keys())
         self.assertIn("Closed", result.keys())
         self.assertNotIn("In Progress", result.keys())
 
     def test_get_story_points_from_epic_returns_a_dict_containing_the_found_statuses_with_their_totals(self):
         # Given
-        jira_client = Mock()
-        jira_client.fields.return_value = DEFAULT_FIELDS_RETURN_VALUE
-        jira_client.search_issues.return_value = [
+
+        self.jira_client.fields.return_value = DEFAULT_FIELDS_RETURN_VALUE
+        self.jira_client.search_issues.return_value = [
             MockedJiraIssue(0, "Reported"),
             MockedJiraIssue(1, "Investigated"),
             MockedJiraIssue(1, "Closed"),
             MockedJiraIssue(1, "Closed"),
         ]
-        jat = JiraAgileToolBox(jira_client)
+        jat = JiraAgileToolBox(self.jira_client)
 
         # When
         result = jat.get_storypoints_from_epic("PROJ001-001")
 
         # Then
         self.assertEqual({"total": 3, "Reported": 0, "Investigated": 1, "Closed": 2}, result)
 
     def test_if_storypoints_custom_field_is_unknown_we_get_it_first_via_the_fields_getter(self):
         # Given
-        jira_client = Mock()
-        jira_client.fields.return_value = [
+
+        self.jira_client.fields.return_value = [
             {
                 "id": "customfield_11280",
                 "name": "Release Note",
                 "custom": True,
                 "orderable": True,
                 "navigable": True,
                 "searchable": True,
@@ -185,40 +161,101 @@
                 "schema": {"type": "number", "custom": "com.atlassian.jira.plugin.system.customfieldtypes:float", "customId": 10333},
             },
         ]
         mocked_jira_issue = MockedJiraIssue()
         mocked_jira_issue.fields.customfield_10333 = 100
         mocked_jira_issue2 = MockedJiraIssue()
         mocked_jira_issue2.fields.customfield_10333 = 0
-        jira_client.search_issues.return_value = [mocked_jira_issue2, mocked_jira_issue]
-        jat = JiraAgileToolBox(jira_client)
+        self.jira_client.search_issues.return_value = [mocked_jira_issue2, mocked_jira_issue]
+        jat = JiraAgileToolBox(self.jira_client)
 
         # When
         result = jat.get_storypoints_from_epic("PROJ001-001")
 
         # Then
-        jira_client.fields.assert_called_once()
+        self.jira_client.fields.assert_called_once()
 
-        jira_client.search_issues.assert_called_with("'Epic Link' = " + "PROJ001-001", fields=["customfield_10333", "status"], maxResults=0)
+        self.jira_client.search_issues.assert_called_with(
+            "'Epic Link' = " + "PROJ001-001", fields=["customfield_10333", "status"], maxResults=0
+        )
 
         self.assertEqual({"total": 100, "Reported": 100}, result)
 
     def test_if_storypoints_can_be_retrieved_from_a_jira_issue(self):
         # Given
-        jira_client = Mock()
-        jira_client.fields.return_value = DEFAULT_FIELDS_RETURN_VALUE
+
+        self.jira_client.fields.return_value = DEFAULT_FIELDS_RETURN_VALUE
         mocked_jira_issue = MockedJiraIssue(story_points=100)
         mocked_jira_issue2 = MockedJiraIssue()
         mocked_jira_epic = MockedJiraIssue()
         mocked_jira_epic.key = "PROJ001-001"
-        jira_client.search_issues.return_value = [mocked_jira_issue2, mocked_jira_issue]
-        jat = JiraAgileToolBox(jira_client)
+        self.jira_client.search_issues.return_value = [mocked_jira_issue2, mocked_jira_issue]
+        jat = JiraAgileToolBox(self.jira_client)
 
         # When
         result = jat.get_storypoints_from_epic(mocked_jira_epic)
 
         # Then
-        jira_client.fields.assert_called_once()
+        self.jira_client.fields.assert_called_once()
 
-        jira_client.search_issues.assert_called_with("'Epic Link' = " + "PROJ001-001", fields=["customfield_10282", "status"], maxResults=0)
+        self.jira_client.search_issues.assert_called_with(
+            "'Epic Link' = " + "PROJ001-001", fields=["customfield_10282", "status"], maxResults=0
+        )
 
         self.assertEqual({"total": 100, "Reported": 100}, result)
+
+
+class TestGetIssuesInEpic(TestCase):
+    def setUp(self) -> None:
+        self.jira_client = Mock(spec=jira.JIRA)
+
+    def test_get_issues_from_epic_searches_for_the_right_epic_key(self):
+        # Given
+
+        self.jira_client.fields.return_value = DEFAULT_FIELDS_RETURN_VALUE
+        self.jira_client.search_issues.return_value = [
+            MockedJiraIssue(story_points=0),
+            MockedJiraIssue(story_points=1),
+            MockedJiraIssue(story_points=2),
+        ]
+        jat = JiraAgileToolBox(self.jira_client)
+
+        # When
+        result = jat.get_all_issues_in_epic("PROJ001-001")
+
+        # Then
+        self.assertEqual(self.jira_client.search_issues.return_value, result)
+        self.jira_client.search_issues.assert_called_with(f"'Epic Link' = PROJ001-001", maxResults=0)
+
+    def test_get_issues_from_epic_can_filter_on_the_fields_to_retrieve_to_reduce_data_retrieval(self):
+        # Given
+
+        self.jira_client.fields.return_value = DEFAULT_FIELDS_RETURN_VALUE
+        self.jira_client.search_issues.return_value = [
+            MockedJiraIssue(story_points=0),
+            MockedJiraIssue(story_points=1),
+            MockedJiraIssue(story_points=2),
+        ]
+        jat = JiraAgileToolBox(self.jira_client)
+
+        # When
+        jat.get_all_issues_in_epic("PROJ001-001", fields=["a_specific_field"])
+
+        # Then
+        self.jira_client.search_issues.assert_called_with(f"'Epic Link' = PROJ001-001", fields=["a_specific_field"], maxResults=0)
+
+    def test_get_issues_from_epic_takes_a_string_field_or_a_list_of_fields(self):
+        # Given
+
+        self.jira_client.fields.return_value = DEFAULT_FIELDS_RETURN_VALUE
+        self.jira_client.search_issues.return_value = [
+            MockedJiraIssue(story_points=0),
+            MockedJiraIssue(story_points=1),
+            MockedJiraIssue(story_points=2),
+        ]
+        jat = JiraAgileToolBox(self.jira_client)
+
+        # When
+        jat.get_all_issues_in_epic("PROJ001-001", fields="a_specific_field")
+
+        # Then
+        self.jira_client.search_issues.assert_called_with(f"'Epic Link' = PROJ001-001", fields=["a_specific_field"], maxResults=0)
```

### Comparing `jira_agile_toolbox-0.0.8/tests/test_ranking.py` & `jira_agile_toolbox-0.0.9/tests/test_ranking.py`

 * *Files identical despite different names*

