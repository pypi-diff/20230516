# Comparing `tmp/gitlab_release_notes-0.2.tar.gz` & `tmp/gitlab_release_notes-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitlab_release_notes-0.2.tar", last modified: Tue May 31 17:03:55 2022, max compression
+gzip compressed data, was "gitlab_release_notes-0.2.1.tar", last modified: Tue May 16 15:12:38 2023, max compression
```

## Comparing `gitlab_release_notes-0.2.tar` & `gitlab_release_notes-0.2.1.tar`

### file list

```diff
@@ -1,26 +1,17 @@
-drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-05-31 17:03:55.978354 gitlab_release_notes-0.2/
-drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-05-31 17:03:55.966314 gitlab_release_notes-0.2/.github/
-drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-05-31 17:03:55.969784 gitlab_release_notes-0.2/.github/workflows/
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     1065 2022-05-31 17:03:50.000000 gitlab_release_notes-0.2/.github/workflows/pypi-publish.yml
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)      701 2022-05-31 17:03:50.000000 gitlab_release_notes-0.2/.github/workflows/tests.yml
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     1799 2022-05-31 15:54:35.000000 gitlab_release_notes-0.2/.gitignore
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     1073 2022-05-31 17:03:50.000000 gitlab_release_notes-0.2/LICENSE
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)      719 2022-05-31 17:03:55.977915 gitlab_release_notes-0.2/PKG-INFO
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)      407 2022-05-31 17:03:50.000000 gitlab_release_notes-0.2/README.md
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     1237 2022-05-31 17:03:50.000000 gitlab_release_notes-0.2/generate.ipynb
-drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-05-31 17:03:55.971730 gitlab_release_notes-0.2/gitlab_release_notes/
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)       77 2022-05-31 17:03:50.000000 gitlab_release_notes-0.2/gitlab_release_notes/__init__.py
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     3225 2022-05-31 17:03:50.000000 gitlab_release_notes-0.2/gitlab_release_notes/generate.py
-drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-05-31 17:03:55.977326 gitlab_release_notes-0.2/gitlab_release_notes/tests/
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)      213 2022-05-31 17:03:50.000000 gitlab_release_notes-0.2/gitlab_release_notes/tests/test_generate.py
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)      143 2022-05-31 17:03:50.000000 gitlab_release_notes-0.2/gitlab_release_notes/tests/test_scripts.py
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)       18 2022-05-31 17:03:50.000000 gitlab_release_notes-0.2/gitlab_release_notes/version.py
-drwxr-xr-x   0 thomasvuillaume   (502) staff       (20)        0 2022-05-31 17:03:55.976068 gitlab_release_notes-0.2/gitlab_release_notes.egg-info/
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)      719 2022-05-31 17:03:54.000000 gitlab_release_notes-0.2/gitlab_release_notes.egg-info/PKG-INFO
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)      566 2022-05-31 17:03:55.000000 gitlab_release_notes-0.2/gitlab_release_notes.egg-info/SOURCES.txt
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)        1 2022-05-31 17:03:54.000000 gitlab_release_notes-0.2/gitlab_release_notes.egg-info/dependency_links.txt
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)       76 2022-05-31 17:03:54.000000 gitlab_release_notes-0.2/gitlab_release_notes.egg-info/entry_points.txt
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)       34 2022-05-31 17:03:55.000000 gitlab_release_notes-0.2/gitlab_release_notes.egg-info/requires.txt
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)       21 2022-05-31 17:03:55.000000 gitlab_release_notes-0.2/gitlab_release_notes.egg-info/top_level.txt
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)       38 2022-05-31 17:03:55.978558 gitlab_release_notes-0.2/setup.cfg
--rw-r--r--   0 thomasvuillaume   (502) staff       (20)     1526 2022-05-31 17:03:50.000000 gitlab_release_notes-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:12:38.164733 gitlab_release_notes-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-16 15:12:22.000000 gitlab_release_notes-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-16 15:12:38.164733 gitlab_release_notes-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-16 15:12:22.000000 gitlab_release_notes-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:12:38.164733 gitlab_release_notes-0.2.1/gitlab_release_notes/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-16 15:12:22.000000 gitlab_release_notes-0.2.1/gitlab_release_notes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-05-16 15:12:22.000000 gitlab_release_notes-0.2.1/gitlab_release_notes/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-16 15:12:22.000000 gitlab_release_notes-0.2.1/gitlab_release_notes/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:12:38.164733 gitlab_release_notes-0.2.1/gitlab_release_notes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-16 15:12:38.000000 gitlab_release_notes-0.2.1/gitlab_release_notes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-16 15:12:38.000000 gitlab_release_notes-0.2.1/gitlab_release_notes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 15:12:38.000000 gitlab_release_notes-0.2.1/gitlab_release_notes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-16 15:12:38.000000 gitlab_release_notes-0.2.1/gitlab_release_notes.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-16 15:12:38.000000 gitlab_release_notes-0.2.1/gitlab_release_notes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-16 15:12:38.000000 gitlab_release_notes-0.2.1/gitlab_release_notes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 15:12:38.164733 gitlab_release_notes-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-16 15:12:22.000000 gitlab_release_notes-0.2.1/setup.py
```

### Comparing `gitlab_release_notes-0.2/LICENSE` & `gitlab_release_notes-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gitlab_release_notes-0.2/PKG-INFO` & `gitlab_release_notes-0.2.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,36 @@
 Metadata-Version: 2.1
 Name: gitlab_release_notes
-Version: 0.2
+Version: 0.2.1
 Summary: Generate release notes for a gitlab project
 Home-page: https://github.com/vuillaut/gitlab_release_notes
 Author: vuillaut
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # Gitlab Release Notes Generator
 
 Generate a changelog listing all merged requests since the last release of the repository.
 
 ## Do it online: 
 [![Heroku](https://pyheroku-badge.herokuapp.com/?app=gitlab-release-notes)](https://gitlab-release-notes.herokuapp.com/)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/vuillaut/GitlabReleaseNotesGenerator/HEAD?labpath=generate.ipynb)
 
+
+## Install and run locally
+
+To install: 
+```
+pip install gitlab_release_notes
+```
+
+Then run:
+```
+gitlab-release-notes --help
+```
+
+## Heroku 
+
+Heroku is setup in the `heroku` branch.
+- make a new release of `gitlab_release_notes`
+- manually deploy from https://dashboard.heroku.com/apps/gitlab-release-notes/deploy/github choosing the heroku branch
```

### Comparing `gitlab_release_notes-0.2/gitlab_release_notes/generate.py` & `gitlab_release_notes-0.2.1/gitlab_release_notes/generate.py`

 * *Files identical despite different names*

### Comparing `gitlab_release_notes-0.2/gitlab_release_notes.egg-info/PKG-INFO` & `gitlab_release_notes-0.2.1/gitlab_release_notes.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,36 @@
 Metadata-Version: 2.1
 Name: gitlab-release-notes
-Version: 0.2
+Version: 0.2.1
 Summary: Generate release notes for a gitlab project
 Home-page: https://github.com/vuillaut/gitlab_release_notes
 Author: vuillaut
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # Gitlab Release Notes Generator
 
 Generate a changelog listing all merged requests since the last release of the repository.
 
 ## Do it online: 
 [![Heroku](https://pyheroku-badge.herokuapp.com/?app=gitlab-release-notes)](https://gitlab-release-notes.herokuapp.com/)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/vuillaut/GitlabReleaseNotesGenerator/HEAD?labpath=generate.ipynb)
 
+
+## Install and run locally
+
+To install: 
+```
+pip install gitlab_release_notes
+```
+
+Then run:
+```
+gitlab-release-notes --help
+```
+
+## Heroku 
+
+Heroku is setup in the `heroku` branch.
+- make a new release of `gitlab_release_notes`
+- manually deploy from https://dashboard.heroku.com/apps/gitlab-release-notes/deploy/github choosing the heroku branch
```

### Comparing `gitlab_release_notes-0.2/setup.py` & `gitlab_release_notes-0.2.1/setup.py`

 * *Files identical despite different names*

