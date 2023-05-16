# Comparing `tmp/pyxform-1.8.0.tar.gz` & `tmp/pyxform-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxform-1.8.0.tar", last modified: Tue Feb 15 17:11:04 2022, max compression
+gzip compressed data, was "pyxform-1.9.0.tar", last modified: Wed Mar 16 16:59:57 2022, max compression
```

## Comparing `pyxform-1.8.0.tar` & `pyxform-1.9.0.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 17:11:04.052221 pyxform-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1290 2022-02-15 17:10:56.000000 pyxform-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     9185 2022-02-15 17:11:04.052221 pyxform-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7680 2022-02-15 17:10:56.000000 pyxform-1.8.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      314 2022-02-15 17:10:56.000000 pyxform-1.8.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 17:11:04.048221 pyxform-1.8.0/pyxform/
--rw-r--r--   0 runner    (1001) docker     (121)      703 2022-02-15 17:10:56.000000 pyxform-1.8.0/pyxform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5831 2022-02-15 17:10:56.000000 pyxform-1.8.0/pyxform/aliases.py
--rw-r--r--   0 runner    (1001) docker     (121)    14698 2022-02-15 17:10:56.000000 pyxform-1.8.0/pyxform/builder.py
--rw-r--r--   0 runner    (1001) docker     (121)     3070 2022-02-15 17:10:56.000000 pyxform-1.8.0/pyxform/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)      283 2022-02-15 17:10:56.000000 pyxform-1.8.0/pyxform/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)      373 2022-02-15 17:10:56.000000 pyxform-1.8.0/pyxform/external_instance.py
--rw-r--r--   0 runner    (1001) docker     (121)     1209 2022-02-15 17:10:56.000000 pyxform-1.8.0/pyxform/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    32366 2022-02-15 17:10:56.000000 pyxform-1.8.0/pyxform/iana_subtags.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3147 2022-02-15 17:10:56.000000 pyxform-1.8.0/pyxform/instance.py
--rw-r--r--   0 runner    (1001) docker     (121)      350 2022-02-15 17:10:56.000000 pyxform-1.8.0/pyxform/instance_info.py
--rw-r--r--   0 runner    (1001) docker     (121)    12371 2022-02-15 17:10:56.000000 pyxform-1.8.0/pyxform/question.py
--rw-r--r--   0 runner    (1001) docker     (121)    13190 2022-02-15 17:10:56.000000 pyxform-1.8.0/pyxform/question_type_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (121)     7620 2022-02-15 17:10:56.000000 pyxform-1.8.0/pyxform/section.py
--rw-r--r--   0 runner    (1001) docker     (121)    45924 2022-02-15 17:10:56.000000 pyxform-1.8.0/pyxform/survey.py
--rw-r--r--   0 runner    (1001) docker     (121)    18581 2022-02-15 17:10:56.000000 pyxform-1.8.0/pyxform/survey_element.py
--rw-r--r--   0 runner    (1001) docker     (121)     2731 2022-02-15 17:10:56.000000 pyxform-1.8.0/pyxform/translator.py
--rw-r--r--   0 runner    (1001) docker     (121)    11366 2022-02-15 17:10:56.000000 pyxform-1.8.0/pyxform/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 17:11:04.052221 pyxform-1.8.0/pyxform/validators/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-15 17:10:56.000000 pyxform-1.8.0/pyxform/validators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 17:11:04.052221 pyxform-1.8.0/pyxform/validators/enketo_validate/
--rw-r--r--   0 runner    (1001) docker     (121)     2491 2022-02-15 17:10:56.000000 pyxform-1.8.0/pyxform/validators/enketo_validate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3060 2022-02-15 17:10:56.000000 pyxform-1.8.0/pyxform/validators/error_cleaner.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 17:11:04.052221 pyxform-1.8.0/pyxform/validators/odk_validate/
--rw-r--r--   0 runner    (1001) docker     (121)     3322 2022-02-15 17:10:56.000000 pyxform-1.8.0/pyxform/validators/odk_validate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 17:11:04.052221 pyxform-1.8.0/pyxform/validators/odk_validate/bin/
--rwxr-xr-x   0 runner    (1001) docker     (121)  1692279 2022-02-15 17:10:56.000000 pyxform-1.8.0/pyxform/validators/odk_validate/bin/ODK_Validate.jar
--rw-r--r--   0 runner    (1001) docker     (121)     3846 2022-02-15 17:10:56.000000 pyxform-1.8.0/pyxform/validators/odk_validate/bin/installed.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 17:11:04.052221 pyxform-1.8.0/pyxform/validators/pyxform/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-15 17:10:56.000000 pyxform-1.8.0/pyxform/validators/pyxform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5514 2022-02-15 17:10:56.000000 pyxform-1.8.0/pyxform/validators/pyxform/missing_translations_check.py
--rw-r--r--   0 runner    (1001) docker     (121)    23748 2022-02-15 17:10:56.000000 pyxform-1.8.0/pyxform/validators/updater.py
--rw-r--r--   0 runner    (1001) docker     (121)     6822 2022-02-15 17:10:56.000000 pyxform-1.8.0/pyxform/validators/util.py
--rw-r--r--   0 runner    (1001) docker     (121)    24709 2022-02-15 17:10:56.000000 pyxform-1.8.0/pyxform/xform2json.py
--rw-r--r--   0 runner    (1001) docker     (121)     4521 2022-02-15 17:10:56.000000 pyxform-1.8.0/pyxform/xform_instance_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)    65091 2022-02-15 17:10:56.000000 pyxform-1.8.0/pyxform/xls2json.py
--rw-r--r--   0 runner    (1001) docker     (121)    14222 2022-02-15 17:10:56.000000 pyxform-1.8.0/pyxform/xls2json_backends.py
--rw-r--r--   0 runner    (1001) docker     (121)     6142 2022-02-15 17:10:56.000000 pyxform-1.8.0/pyxform/xls2xform.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 17:11:04.052221 pyxform-1.8.0/pyxform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9185 2022-02-15 17:11:04.000000 pyxform-1.8.0/pyxform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1156 2022-02-15 17:11:04.000000 pyxform-1.8.0/pyxform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-15 17:11:04.000000 pyxform-1.8.0/pyxform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-02-15 17:11:04.000000 pyxform-1.8.0/pyxform.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-02-15 17:11:04.000000 pyxform-1.8.0/pyxform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-02-15 17:11:04.000000 pyxform-1.8.0/pyxform.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-02-15 17:11:04.056221 pyxform-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      941 2022-02-15 17:10:56.000000 pyxform-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 16:59:57.554525 pyxform-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     1290 2022-03-16 16:59:48.000000 pyxform-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     9434 2022-03-16 16:59:57.554525 pyxform-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     7881 2022-03-16 16:59:48.000000 pyxform-1.9.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      314 2022-03-16 16:59:48.000000 pyxform-1.9.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 16:59:57.550525 pyxform-1.9.0/pyxform/
+-rw-r--r--   0 runner    (1001) docker     (121)      703 2022-03-16 16:59:48.000000 pyxform-1.9.0/pyxform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5831 2022-03-16 16:59:48.000000 pyxform-1.9.0/pyxform/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14698 2022-03-16 16:59:48.000000 pyxform-1.9.0/pyxform/builder.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3364 2022-03-16 16:59:48.000000 pyxform-1.9.0/pyxform/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)      283 2022-03-16 16:59:48.000000 pyxform-1.9.0/pyxform/errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)      373 2022-03-16 16:59:48.000000 pyxform-1.9.0/pyxform/external_instance.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1209 2022-03-16 16:59:48.000000 pyxform-1.9.0/pyxform/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32366 2022-03-16 16:59:48.000000 pyxform-1.9.0/pyxform/iana_subtags.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3147 2022-03-16 16:59:48.000000 pyxform-1.9.0/pyxform/instance.py
+-rw-r--r--   0 runner    (1001) docker     (121)      350 2022-03-16 16:59:48.000000 pyxform-1.9.0/pyxform/instance_info.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13010 2022-03-16 16:59:48.000000 pyxform-1.9.0/pyxform/question.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13190 2022-03-16 16:59:48.000000 pyxform-1.9.0/pyxform/question_type_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7620 2022-03-16 16:59:48.000000 pyxform-1.9.0/pyxform/section.py
+-rw-r--r--   0 runner    (1001) docker     (121)    45981 2022-03-16 16:59:48.000000 pyxform-1.9.0/pyxform/survey.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18581 2022-03-16 16:59:48.000000 pyxform-1.9.0/pyxform/survey_element.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2731 2022-03-16 16:59:48.000000 pyxform-1.9.0/pyxform/translator.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11366 2022-03-16 16:59:48.000000 pyxform-1.9.0/pyxform/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 16:59:57.550525 pyxform-1.9.0/pyxform/validators/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-16 16:59:48.000000 pyxform-1.9.0/pyxform/validators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 16:59:57.554525 pyxform-1.9.0/pyxform/validators/enketo_validate/
+-rw-r--r--   0 runner    (1001) docker     (121)     2491 2022-03-16 16:59:48.000000 pyxform-1.9.0/pyxform/validators/enketo_validate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3060 2022-03-16 16:59:48.000000 pyxform-1.9.0/pyxform/validators/error_cleaner.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 16:59:57.554525 pyxform-1.9.0/pyxform/validators/odk_validate/
+-rw-r--r--   0 runner    (1001) docker     (121)     3322 2022-03-16 16:59:48.000000 pyxform-1.9.0/pyxform/validators/odk_validate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 16:59:57.554525 pyxform-1.9.0/pyxform/validators/odk_validate/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (121)  1692279 2022-03-16 16:59:48.000000 pyxform-1.9.0/pyxform/validators/odk_validate/bin/ODK_Validate.jar
+-rw-r--r--   0 runner    (1001) docker     (121)     3846 2022-03-16 16:59:48.000000 pyxform-1.9.0/pyxform/validators/odk_validate/bin/installed.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 16:59:57.554525 pyxform-1.9.0/pyxform/validators/pyxform/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-16 16:59:48.000000 pyxform-1.9.0/pyxform/validators/pyxform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5514 2022-03-16 16:59:48.000000 pyxform-1.9.0/pyxform/validators/pyxform/missing_translations_check.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1541 2022-03-16 16:59:48.000000 pyxform-1.9.0/pyxform/validators/pyxform/select_from_file_params.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23748 2022-03-16 16:59:48.000000 pyxform-1.9.0/pyxform/validators/updater.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6822 2022-03-16 16:59:48.000000 pyxform-1.9.0/pyxform/validators/util.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24709 2022-03-16 16:59:48.000000 pyxform-1.9.0/pyxform/xform2json.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4521 2022-03-16 16:59:48.000000 pyxform-1.9.0/pyxform/xform_instance_parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)    66062 2022-03-16 16:59:48.000000 pyxform-1.9.0/pyxform/xls2json.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14449 2022-03-16 16:59:48.000000 pyxform-1.9.0/pyxform/xls2json_backends.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6142 2022-03-16 16:59:48.000000 pyxform-1.9.0/pyxform/xls2xform.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 16:59:57.550525 pyxform-1.9.0/pyxform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     9434 2022-03-16 16:59:57.000000 pyxform-1.9.0/pyxform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1210 2022-03-16 16:59:57.000000 pyxform-1.9.0/pyxform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-16 16:59:57.000000 pyxform-1.9.0/pyxform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      121 2022-03-16 16:59:57.000000 pyxform-1.9.0/pyxform.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       46 2022-03-16 16:59:57.000000 pyxform-1.9.0/pyxform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-03-16 16:59:57.000000 pyxform-1.9.0/pyxform.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      153 2022-03-16 16:59:57.554525 pyxform-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      941 2022-03-16 16:59:48.000000 pyxform-1.9.0/setup.py
```

### Comparing `pyxform-1.8.0/LICENSE` & `pyxform-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxform-1.8.0/PKG-INFO` & `pyxform-1.9.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 1.2
 Name: pyxform
-Version: 1.8.0
+Version: 1.9.0
 Summary: A Python package to create XForms for ODK Collect.
 Home-page: http://pypi.python.org/pypi/pyxform/
 Author: github.com/xlsform
 Author-email: info@xlsform.org
 License: UNKNOWN
 Description: ===============
-        pyxform v1.8.0
+        pyxform v1.9.0
         ===============
         
         |python| |black|
         
         .. |python| image:: https://img.shields.io/badge/python-3.7,3.8,3.9-blue.svg
             :target: https://www.python.org/downloads
         
@@ -130,34 +130,40 @@
         
         2. Run all tests through Validate by setting the default for ``run_odk_validate`` to ``kwargs.get("run_odk_validate", True)`` in ``pyxform/tests_v1/pyxform_test_case.py``.
         3. Draft a new GitHub release with the list of merged PRs. Follow the title and description pattern of the previous release.
         4. Checkout a release branch from latest upstream master.
         5. Update ``CHANGES.txt`` with the text of the draft release.
         6. Update ``README.rst``, ``setup.py``, ``pyxform/__init__.py`` with the new release version number.
         7. Commit, push the branch, and initiate a pull request. Wait for tests to pass, then merge the PR.
-        8. In a clean new release only directory, checkout master.
-        9. Create a new virtualenv in this directory to ensure a clean Python environment::
+        8. Tag the release and it will automatically be published
+        
+        Manually releasing
+        ===================
+        Releases are now automatic. These instructions are provided for forks or for a future change in process.
+        
+        1. In a clean new release only directory, check out master.
+        2. Create a new virtualenv in this directory to ensure a clean Python environment::
         
              /usr/local/bin/python3.8 -m venv pyxform-release
              . pyxform-release/bin/activate
         
-        10. Install the production and packaging requirements::
+        3. Install the production and packaging requirements::
         
              pip install -e .
              pip install wheel twine
         
-        11. Cleanup build and dist folders::
+        4. Clean up build and dist folders::
         
              rm -rf build dist pyxform.egg-info
         
-        12. Prepare ``sdist`` and ``bdist_wheel`` distributions::
+        5. Prepare ``sdist`` and ``bdist_wheel`` distributions::
         
              python setup.py sdist bdist_wheel
         
-        13. Publish release to PyPI with ``twine``::
+        6. Publish release to PyPI with ``twine``::
         
              twine upload dist/pyxform-*-py3-none-any.whl dist/pyxform-*.tar.gz
         
-        14. Tag the GitHub release and publish it.
+        7. Tag the GitHub release and publish it.
         
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pyxform-1.8.0/README.rst` & `pyxform-1.9.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ===============
-pyxform v1.8.0
+pyxform v1.9.0
 ===============
 
 |python| |black|
 
 .. |python| image:: https://img.shields.io/badge/python-3.7,3.8,3.9-blue.svg
     :target: https://www.python.org/downloads
 
@@ -122,31 +122,37 @@
 
 2. Run all tests through Validate by setting the default for ``run_odk_validate`` to ``kwargs.get("run_odk_validate", True)`` in ``pyxform/tests_v1/pyxform_test_case.py``.
 3. Draft a new GitHub release with the list of merged PRs. Follow the title and description pattern of the previous release.
 4. Checkout a release branch from latest upstream master.
 5. Update ``CHANGES.txt`` with the text of the draft release.
 6. Update ``README.rst``, ``setup.py``, ``pyxform/__init__.py`` with the new release version number.
 7. Commit, push the branch, and initiate a pull request. Wait for tests to pass, then merge the PR.
-8. In a clean new release only directory, checkout master.
-9. Create a new virtualenv in this directory to ensure a clean Python environment::
+8. Tag the release and it will automatically be published
+
+Manually releasing
+===================
+Releases are now automatic. These instructions are provided for forks or for a future change in process.
+
+1. In a clean new release only directory, check out master.
+2. Create a new virtualenv in this directory to ensure a clean Python environment::
 
      /usr/local/bin/python3.8 -m venv pyxform-release
      . pyxform-release/bin/activate
 
-10. Install the production and packaging requirements::
+3. Install the production and packaging requirements::
 
      pip install -e .
      pip install wheel twine
 
-11. Cleanup build and dist folders::
+4. Clean up build and dist folders::
 
      rm -rf build dist pyxform.egg-info
 
-12. Prepare ``sdist`` and ``bdist_wheel`` distributions::
+5. Prepare ``sdist`` and ``bdist_wheel`` distributions::
 
      python setup.py sdist bdist_wheel
 
-13. Publish release to PyPI with ``twine``::
+6. Publish release to PyPI with ``twine``::
 
      twine upload dist/pyxform-*-py3-none-any.whl dist/pyxform-*.tar.gz
 
-14. Tag the GitHub release and publish it.
+7. Tag the GitHub release and publish it.
```

### Comparing `pyxform-1.8.0/pyxform/__init__.py` & `pyxform-1.9.0/pyxform/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 """
 pyxform is a Python library designed to make authoring XForms for ODK
 Collect easy.
 """
 
-__version__ = "1.8.0"
+__version__ = "1.9.0"
 
 from pyxform.builder import (
     SurveyElementBuilder,
     create_survey,
     create_survey_element_from_dict,
     create_survey_from_path,
     create_survey_from_xls,
```

### Comparing `pyxform-1.8.0/pyxform/aliases.py` & `pyxform-1.9.0/pyxform/aliases.py`

 * *Files identical despite different names*

### Comparing `pyxform-1.8.0/pyxform/builder.py` & `pyxform-1.9.0/pyxform/builder.py`

 * *Files identical despite different names*

### Comparing `pyxform-1.8.0/pyxform/constants.py` & `pyxform-1.9.0/pyxform/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -101,7 +101,17 @@
 
 DEPRECATED_DEVICE_ID_METADATA_FIELDS = ["subscriberid", "simserial"]
 
 AUDIO_QUALITY_VOICE_ONLY = "voice-only"
 AUDIO_QUALITY_LOW = "low"
 AUDIO_QUALITY_NORMAL = "normal"
 AUDIO_QUALITY_EXTERNAL = "external"
+
+EXTERNAL_INSTANCE_EXTENSIONS = [".xml", ".csv", ".geojson"]
+
+EXTERNAL_CHOICES_ITEMSET_REF_LABEL = "label"
+EXTERNAL_CHOICES_ITEMSET_REF_VALUE = "name"
+
+EXTERNAL_CHOICES_ITEMSET_REF_LABEL_GEOJSON = "title"
+EXTERNAL_CHOICES_ITEMSET_REF_VALUE_GEOJSON = "id"
+
+ROW_FORMAT_STRING: str = "[row : %s]"
```

### Comparing `pyxform-1.8.0/pyxform/file_utils.py` & `pyxform-1.9.0/pyxform/file_utils.py`

 * *Files identical despite different names*

### Comparing `pyxform-1.8.0/pyxform/iana_subtags.txt` & `pyxform-1.9.0/pyxform/iana_subtags.txt`

 * *Files identical despite different names*

### Comparing `pyxform-1.8.0/pyxform/instance.py` & `pyxform-1.9.0/pyxform/instance.py`

 * *Files identical despite different names*

### Comparing `pyxform-1.8.0/pyxform/question.py` & `pyxform-1.9.0/pyxform/question.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 # -*- coding: utf-8 -*-
 """
 XForm Survey element classes for different question types.
 """
 import os.path
 import re
 
+from pyxform.constants import (
+    EXTERNAL_CHOICES_ITEMSET_REF_LABEL,
+    EXTERNAL_CHOICES_ITEMSET_REF_LABEL_GEOJSON,
+    EXTERNAL_CHOICES_ITEMSET_REF_VALUE,
+    EXTERNAL_CHOICES_ITEMSET_REF_VALUE_GEOJSON,
+    EXTERNAL_INSTANCE_EXTENSIONS,
+)
 from pyxform.errors import PyXFormError
 from pyxform.question_type_dictionary import QUESTION_TYPE_DICT
 from pyxform.survey_element import SurveyElement
 from pyxform.utils import default_is_dynamic, has_dynamic_label, node
 
 
 class Question(SurveyElement):
@@ -194,31 +201,42 @@
             first_choices = next(iter(choices.values()))
             multi_language = isinstance(first_choices[0].get("label"), dict)
 
         # itemset are only supposed to be strings,
         # check to prevent the rare dicts that show up
         if self["itemset"] and isinstance(self["itemset"], str):
             choice_filter = self.get("choice_filter")
-            itemset_value_ref = "name"
+
             itemset, file_extension = os.path.splitext(self["itemset"])
+            itemset_value_ref = self.parameters.get(
+                "value",
+                EXTERNAL_CHOICES_ITEMSET_REF_VALUE_GEOJSON
+                if file_extension == ".geojson"
+                else EXTERNAL_CHOICES_ITEMSET_REF_VALUE,
+            )
+            itemset_label_ref = self.parameters.get(
+                "label",
+                EXTERNAL_CHOICES_ITEMSET_REF_LABEL_GEOJSON
+                if file_extension == ".geojson"
+                else EXTERNAL_CHOICES_ITEMSET_REF_LABEL,
+            )
+
             has_media = False
             has_dyn_label = False
             is_previous_question = bool(re.match(r"^\${.*}$", self.get("itemset")))
 
             if choices.get(itemset):
                 has_media = bool(choices[itemset][0].get("media"))
                 has_dyn_label = has_dynamic_label(choices[itemset], multi_language)
 
-            if file_extension in [".csv", ".xml"]:
+            if file_extension in EXTERNAL_INSTANCE_EXTENSIONS:
                 itemset = itemset
-                itemset_label_ref = "label"
             else:
                 if not multi_language and not has_media and not has_dyn_label:
                     itemset = self["itemset"]
-                    itemset_label_ref = "label"
                 else:
                     itemset = self["itemset"]
                     itemset_label_ref = "jr:itext(itextId)"
 
             choice_filter = survey.insert_xpaths(
                 choice_filter, self, True, is_previous_question
             )
```

### Comparing `pyxform-1.8.0/pyxform/question_type_dictionary.py` & `pyxform-1.9.0/pyxform/question_type_dictionary.py`

 * *Files identical despite different names*

### Comparing `pyxform-1.8.0/pyxform/section.py` & `pyxform-1.9.0/pyxform/section.py`

 * *Files identical despite different names*

### Comparing `pyxform-1.8.0/pyxform/survey.py` & `pyxform-1.9.0/pyxform/survey.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import tempfile
 import xml.etree.ElementTree as ETree
 from collections import defaultdict
 from datetime import datetime
 from functools import lru_cache
 
 from pyxform import constants
+from pyxform.constants import EXTERNAL_INSTANCE_EXTENSIONS
 from pyxform.errors import PyXFormError, ValidationError
 from pyxform.external_instance import ExternalInstance
 from pyxform.instance import SurveyInstance
 from pyxform.instance_info import InstanceInfo
 from pyxform.question import Question
 from pyxform.section import Section
 from pyxform.survey_element import SurveyElement
@@ -403,18 +404,18 @@
                         )
             return pulldata_instances
         return None
 
     @staticmethod
     def _generate_from_file_instances(element):
         itemset = element.get("itemset")
-        if itemset and (itemset.endswith(".csv") or itemset.endswith(".xml")):
-            file_id, ext = os.path.splitext(itemset)
+        file_id, ext = os.path.splitext(itemset)
+        if itemset and ext in EXTERNAL_INSTANCE_EXTENSIONS:
             uri = "jr://%s/%s" % (
-                "file" if ext == ".xml" else "file-%s" % ext[1:],
+                "file" if ext == ".xml" or ext == ".geojson" else "file-%s" % ext[1:],
                 itemset,
             )
             return InstanceInfo(
                 type="file",
                 context="[type: {t}, name: {n}]".format(
                     t=element["parent"]["type"], n=element["parent"]["name"]
                 ),
```

### Comparing `pyxform-1.8.0/pyxform/survey_element.py` & `pyxform-1.9.0/pyxform/survey_element.py`

 * *Files identical despite different names*

### Comparing `pyxform-1.8.0/pyxform/translator.py` & `pyxform-1.9.0/pyxform/translator.py`

 * *Files identical despite different names*

### Comparing `pyxform-1.8.0/pyxform/utils.py` & `pyxform-1.9.0/pyxform/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,21 +186,20 @@
                 continue
             writer.writerow(csv_data)
 
     return True
 
 
 def xlsx_sheet_to_csv(workbook_path, csv_path, sheet_name):
-    wb = openpyxl.open(workbook_path)
+    wb = openpyxl.open(workbook_path, read_only=True, data_only=True)
     try:
         sheet = wb.get_sheet_by_name(sheet_name)
     except KeyError:
         return False
-    if sheet.max_row < 2:
-        return False
+
     with open(csv_path, "w", newline="") as f:
         writer = csv.writer(f, quoting=csv.QUOTE_ALL)
         mask = [not is_empty(cell.value) for cell in sheet[1]]
         for row in sheet.rows:
             csv_data = []
             try:
                 for v, m in zip(row, mask):
@@ -208,15 +207,15 @@
                         data = xlsx_value_to_str(v.value)
                         # clean the values of leading and trailing whitespaces
                         data = data.strip()
                         csv_data.append(data)
             except TypeError:
                 continue
             writer.writerow(csv_data)
-
+    wb.close()
     return True
 
 
 def has_external_choices(json_struct):
     """
     Returns true if a select one external prompt is used in the survey.
     """
```

### Comparing `pyxform-1.8.0/pyxform/validators/enketo_validate/__init__.py` & `pyxform-1.9.0/pyxform/validators/enketo_validate/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxform-1.8.0/pyxform/validators/error_cleaner.py` & `pyxform-1.9.0/pyxform/validators/error_cleaner.py`

 * *Files identical despite different names*

### Comparing `pyxform-1.8.0/pyxform/validators/odk_validate/__init__.py` & `pyxform-1.9.0/pyxform/validators/odk_validate/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxform-1.8.0/pyxform/validators/odk_validate/bin/ODK_Validate.jar` & `pyxform-1.9.0/pyxform/validators/odk_validate/bin/ODK_Validate.jar`

 * *Files identical despite different names*

### Comparing `pyxform-1.8.0/pyxform/validators/odk_validate/bin/installed.json` & `pyxform-1.9.0/pyxform/validators/odk_validate/bin/installed.json`

 * *Files identical despite different names*

### Comparing `pyxform-1.8.0/pyxform/validators/pyxform/missing_translations_check.py` & `pyxform-1.9.0/pyxform/validators/pyxform/missing_translations_check.py`

 * *Files identical despite different names*

### Comparing `pyxform-1.8.0/pyxform/validators/updater.py` & `pyxform-1.9.0/pyxform/validators/updater.py`

 * *Files identical despite different names*

### Comparing `pyxform-1.8.0/pyxform/validators/util.py` & `pyxform-1.9.0/pyxform/validators/util.py`

 * *Files identical despite different names*

### Comparing `pyxform-1.8.0/pyxform/xform2json.py` & `pyxform-1.9.0/pyxform/xform2json.py`

 * *Files identical despite different names*

### Comparing `pyxform-1.8.0/pyxform/xform_instance_parser.py` & `pyxform-1.9.0/pyxform/xform_instance_parser.py`

 * *Files identical despite different names*

### Comparing `pyxform-1.8.0/pyxform/xls2json.py` & `pyxform-1.9.0/pyxform/xls2json.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,18 @@
 import os
 import re
 import sys
 from collections import Counter
 from typing import TYPE_CHECKING
 
 from pyxform import aliases, constants
+from pyxform.constants import EXTERNAL_INSTANCE_EXTENSIONS, ROW_FORMAT_STRING
 from pyxform.errors import PyXFormError
 from pyxform.utils import default_is_dynamic, is_valid_xml_tag, levenshtein_distance
+from pyxform.validators.pyxform import select_from_file_params
 from pyxform.validators.pyxform.missing_translations_check import (
     missing_translations_check,
 )
 from pyxform.xls2json_backends import csv_to_dict, xls_to_dict, xlsx_to_dict
 
 if TYPE_CHECKING:
     from typing import Any, Dict, KeysView, List, Optional
@@ -387,16 +389,14 @@
             break
     if not is_valid:
         # TODO - could we state what headers are missing?
         raise PyXFormError(
             "The survey sheet is either empty or missing important column headers."
         )
 
-    row_format_string = "[row : %s]"
-
     # Make sure the passed in vars are unicode
     form_name = str(form_name)
     default_language = str(default_language)
 
     # We check for double columns to determine whether to use them
     # or single colons to delimit grouped headers.
     # Single colons are bad because they conflict with with the xform namespace
@@ -635,15 +635,15 @@
         else:
             prev_control_type = None
             parent_children_array = []
         # Disabled should probably be first
         # so the attributes below can be disabled.
         if "disabled" in row:
             warnings.append(
-                row_format_string % row_number
+                ROW_FORMAT_STRING % row_number
                 + " The 'disabled' column header is not part of the current"
                 + " spec. We recommend using relevant instead."
             )
             disabled = row.pop("disabled")
             if aliases.yes_no.get(disabled):
                 continue
 
@@ -656,29 +656,29 @@
         question_name = row.get(constants.NAME)
 
         if not question_type:
             # if name and label are also missing,
             # then its a comment row, and we skip it with warning
             if not ((constants.NAME in row) or (constants.LABEL in row)):
                 warnings.append(
-                    row_format_string % row_number
+                    ROW_FORMAT_STRING % row_number
                     + " Row without name, text, or label is being skipped:\n"
                     + str(row)
                 )
                 continue
             raise PyXFormError(
-                row_format_string % row_number + " Question with no type.\n" + str(row)
+                ROW_FORMAT_STRING % row_number + " Question with no type.\n" + str(row)
             )
 
         # Pull out questions that will go in meta block
         if question_type == "audit":
             # Force audit name to always be "audit" to follow XForms spec
             if "name" in row and row["name"] not in [None, "", "audit"]:
                 raise PyXFormError(
-                    row_format_string % row_number
+                    ROW_FORMAT_STRING % row_number
                     + " Audits must always be named 'audit.'"
                     + " The name column should be left blank."
                 )
             row["name"] = "audit"
 
             new_dict = row.copy()
             parameters = get_parameters(
@@ -839,19 +839,19 @@
         if question_type == "calculate":
             calculation = row.get("bind", {}).get("calculate")
             question_default = row.get("default")
             if not calculation and not (
                 question_default and default_is_dynamic(question_default, question_type)
             ):
                 raise PyXFormError(
-                    row_format_string % row_number + " Missing calculation."
+                    ROW_FORMAT_STRING % row_number + " Missing calculation."
                 )
         if question_type in constants.DEPRECATED_DEVICE_ID_METADATA_FIELDS:
             warnings.append(
-                (row_format_string % row_number)
+                (ROW_FORMAT_STRING % row_number)
                 + " "
                 + question_type
                 + " is no longer supported on most devices. "
                 "Only old versions of Collect on Android versions older than 11 still support it."
             )
         # Check if the question is actually a setting specified
         # on the survey sheet
@@ -866,15 +866,15 @@
         if end_control_parse:
             parse_dict = end_control_parse.groupdict()
             if parse_dict.get("end") and "type" in parse_dict:
                 control_type = aliases.control[parse_dict["type"]]
                 control_name = question_name
                 if prev_control_type != control_type or len(stack) == 1:
                     raise PyXFormError(
-                        row_format_string % row_number
+                        ROW_FORMAT_STRING % row_number
                         + " Unmatched end statement. Previous control type: "
                         + str(prev_control_type)
                         + ", Control type: "
                         + str(control_type)
                         + ", Control name: "
                         + str(control_name)
                     )
@@ -888,21 +888,21 @@
                 # autogenerate names for notes without them
                 row["name"] = "generated_note_name_" + str(row_number)
             # elif 'group' in row['type'].lower():
             #     # autogenerate names for groups without them
             #     row['name'] = "generated_group_name_" + str(row_number)
             else:
                 raise PyXFormError(
-                    row_format_string % row_number + " Question or group with no name."
+                    ROW_FORMAT_STRING % row_number + " Question or group with no name."
                 )
         question_name = str(row[constants.NAME])
         if not is_valid_xml_tag(question_name):
             if isinstance(question_name, bytes):
                 question_name = question_name.encode("utf-8")
-            error_message = row_format_string % row_number
+            error_message = ROW_FORMAT_STRING % row_number
             error_message += " Invalid question name [" + question_name + "] "
             error_message += "Names must begin with a letter, colon," + " or underscore."
             error_message += (
                 "Subsequent characters can include numbers," + " dashes, and periods."
             )
             raise PyXFormError(error_message)
 
@@ -940,34 +940,34 @@
                         == constants.FIELD_LIST
                     )
                 ):
                     # Row number, name, and type probably enough for user message.
                     # Also means the error message text is stable for tests.
                     msg_dict = {"name": row.get("name"), "type": row.get("type")}
                     warnings.append(
-                        row_format_string % row_number
+                        ROW_FORMAT_STRING % row_number
                         + " %s has no label: " % control_type.capitalize()
                         + str(msg_dict)
                     )
 
                 new_json_dict = row.copy()
                 new_json_dict[constants.TYPE] = control_type
                 child_list = list()
                 new_json_dict[constants.CHILDREN] = child_list
                 if control_type is constants.LOOP:
                     if not parse_dict.get("list_name"):
                         # TODO: Perhaps warn and make repeat into a group?
                         raise PyXFormError(
-                            row_format_string % row_number
+                            ROW_FORMAT_STRING % row_number
                             + " Repeat loop without list name."
                         )
                     list_name = parse_dict["list_name"]
                     if list_name not in choices:
                         raise PyXFormError(
-                            row_format_string % row_number
+                            ROW_FORMAT_STRING % row_number
                             + " List name not in columns sheet: "
                             + list_name
                         )
                     new_json_dict[constants.COLUMNS] = choices[list_name]
 
                 # Generate a new node for the jr:count column so
                 # xpath expressions can be used.
@@ -1039,15 +1039,15 @@
         select_parse = select_regexp.search(question_type)
         if select_parse:
             parse_dict = select_parse.groupdict()
             if parse_dict.get("select_command"):
                 select_type = aliases.select[parse_dict["select_command"]]
                 if select_type == "select one external" and "choice_filter" not in row:
                     warnings.append(
-                        row_format_string % row_number
+                        ROW_FORMAT_STRING % row_number
                         + " select one external is only meant for"
                         " filtered selects."
                     )
                 list_name = parse_dict["list_name"]
                 list_file_name, file_extension = os.path.splitext(list_name)
                 if (
                     select_type == "select one external"
@@ -1061,45 +1061,45 @@
                             msg = msg + " " + similar
                         raise PyXFormError(
                             msg
                             + " Please ensure that the external_choices sheet has columns"
                             " 'list name', and 'name'."
                         )
                     raise PyXFormError(
-                        row_format_string % row_number
+                        ROW_FORMAT_STRING % row_number
                         + "List name not in external choices sheet: "
                         + list_name
                     )
                 if (
                     list_name not in choices
                     and select_type != "select one external"
-                    and file_extension not in [".csv", ".xml"]
+                    and file_extension not in EXTERNAL_INSTANCE_EXTENSIONS
                     and not re.match(r"\$\{(.*?)\}", list_name)
                 ):
                     if not choices:
                         k = constants.CHOICES
                         msg = "There should be a choices sheet in this xlsform."
                         similar = find_sheet_misspellings(key=k, keys=workbook_keys)
                         if similar is not None:
                             msg = msg + " " + similar
                         raise PyXFormError(
                             msg + " Please ensure that the choices sheet has the"
                             " mandatory columns 'list_name', 'name', and 'label'."
                         )
                     raise PyXFormError(
-                        row_format_string % row_number
+                        ROW_FORMAT_STRING % row_number
                         + " List name not in choices sheet: "
                         + list_name
                     )
 
                 # Validate select_multiple choice names by making sure
                 # they have no spaces (will cause errors in exports).
                 if (
                     select_type == constants.SELECT_ALL_THAT_APPLY
-                    and file_extension not in [".csv", ".xml"]
+                    and file_extension not in EXTERNAL_INSTANCE_EXTENSIONS
                 ):
                     for choice in choices[list_name]:
                         if " " in choice[constants.NAME]:
                             raise PyXFormError(
                                 "Choice names with spaces cannot be added "
                                 "to multiple choice selects. See ["
                                 + choice[constants.NAME]
@@ -1111,17 +1111,24 @@
                 specify_other_question = None
                 if parse_dict.get("specify_other") is not None:
                     select_type += " or specify other"
 
                 new_json_dict = row.copy()
                 new_json_dict[constants.TYPE] = select_type
 
-                # Look at parameters column for randomization parameters
+                select_params_allowed = ["randomize", "seed"]
+                if parse_dict["select_command"] in (
+                    "select_one_from_file",
+                    "select_multiple_from_file",
+                ):
+                    select_params_allowed += ["value", "label"]
+
+                # Look at parameters column for select parameters
                 parameters = get_parameters(
-                    row.get("parameters", ""), ["randomize", "seed"]
+                    row.get("parameters", ""), select_params_allowed
                 )
 
                 if "randomize" in parameters.keys():
                     if (
                         parameters["randomize"] != "true"
                         and parameters["randomize"] != "false"
                     ):
@@ -1139,14 +1146,27 @@
                                     "seed value must be a number or a reference to another field."
                                 )
                 elif "seed" in parameters.keys():
                     raise PyXFormError(
                         "Parameters must include randomize=true to use a seed."
                     )
 
+                if "value" in parameters.keys():
+                    select_from_file_params.value_or_label_check(
+                        name="value",
+                        value=parameters["value"],
+                        row_number=row_number,
+                    )
+                if "label" in parameters.keys():
+                    select_from_file_params.value_or_label_check(
+                        name="label",
+                        value=parameters["label"],
+                        row_number=row_number,
+                    )
+
                 new_json_dict["parameters"] = parameters
 
                 if row.get("choice_filter"):
                     if select_type == "select one external":
                         new_json_dict["query"] = list_name
                     else:
                         new_json_dict["itemset"] = list_name
@@ -1155,15 +1175,15 @@
                             new_json_dict["list_name"] = list_name
                             new_json_dict[constants.CHOICES] = choices[list_name]
                 elif (
                     "randomize" in parameters.keys() and parameters["randomize"] == "true"
                 ):
                     new_json_dict["itemset"] = list_name
                     json_dict["choices"] = choices
-                elif file_extension in [".csv", ".xml"] or re.match(
+                elif file_extension in EXTERNAL_INSTANCE_EXTENSIONS or re.match(
                     r"\$\{(.*?)\}", list_name
                 ):
                     new_json_dict["itemset"] = list_name
                 else:
                     new_json_dict["list_name"] = list_name
                     new_json_dict[constants.CHOICES] = choices[list_name]
 
@@ -1182,15 +1202,15 @@
                             constants.CHOICES: choices[list_name],
                             # Do we care about filtered selects in table lists?
                             # 'itemset' : list_name,
                         }
                         parent_children_array.append(table_list_header)
 
                     if table_list != list_name:
-                        error_message = row_format_string % row_number
+                        error_message = ROW_FORMAT_STRING % row_number
                         error_message += (
                             " Badly formatted table list,"
                             " list names don't match: " + table_list + " vs. " + list_name
                         )
                         raise PyXFormError(error_message)
 
                     control = new_json_dict["control"] = new_json_dict.get("control", {})
@@ -1237,15 +1257,15 @@
                 except ValueError:
                     raise PyXFormError("Parameter max-pixels must have an integer value.")
 
                 new_dict["bind"] = new_dict.get("bind", {})
                 new_dict["bind"].update({"orx:max-pixels": parameters["max-pixels"]})
             else:
                 warnings.append(
-                    (row_format_string % row_number)
+                    (ROW_FORMAT_STRING % row_number)
                     + " Use the max-pixels parameter to speed up submission sending and save storage space. Learn more: https://xlsform.org/#image"
                 )
             parent_children_array.append(new_dict)
             continue
 
         if question_type == "audio":
             new_dict = row.copy()
```

### Comparing `pyxform-1.8.0/pyxform/xls2json_backends.py` & `pyxform-1.9.0/pyxform/xls2json_backends.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,23 +171,25 @@
     name. For each sheet there is a list of dictionaries, each
     dictionary corresponds to a single row in the worksheet. A
     dictionary has keys taken from the column headers and values
     equal to the cell value for that row and column.
     All the keys and leaf elements are strings.
     """
     try:
-        workbook = openpyxl.open(filename=path_or_file, data_only=True)
+        workbook = openpyxl.open(filename=path_or_file, read_only=True, data_only=True)
     except (OSError, BadZipFile, KeyError) as error:
         raise PyXFormError("Error reading .xlsx file: %s" % error)
 
     def xlsx_to_dict_normal_sheet(sheet):
 
         # Check for duplicate column headers
         column_header_list = list()
-        for cell in sheet[1]:
+
+        first_row = next(sheet.rows, [])
+        for cell in first_row:
             column_header = cell.value
             # xls file with 3 columns mostly have a 3 more columns that are
             # blank by default or something, skip during check
             if is_empty(column_header):
                 # Preserve column order (will filter later)
                 column_header_list.append(None)
             else:
@@ -200,24 +202,28 @@
         result = []
         for row in sheet.iter_rows(min_row=2):
             row_dict = OrderedDict()
             for column, key in enumerate(column_header_list):
                 if key is None:
                     continue
 
-                value = row[column].value
-                if isinstance(value, str):
-                    value = value.strip()
-
-                if not is_empty(value):
-                    row_dict[key] = xlsx_value_to_str(value)
+                try:
+                    value = row[column].value
+                    if isinstance(value, str):
+                        value = value.strip()
+
+                    if not is_empty(value):
+                        row_dict[key] = xlsx_value_to_str(value)
+                except IndexError:
+                    pass  # rows may not have values for every column
 
             result.append(row_dict)
 
         column_header_list = [key for key in column_header_list if key is not None]
+
         return result, _list_to_dict_list(column_header_list)
 
     result = OrderedDict()
     for sheetname in workbook.sheetnames:
         sheet = workbook[sheetname]
         # Note that the sheet exists but do no further processing here.
         result[sheetname] = []
@@ -232,14 +238,15 @@
                 continue
         else:
             (
                 result[sheetname],
                 result[f"{sheetname}_header"],
             ) = xlsx_to_dict_normal_sheet(sheet)
 
+    workbook.close()
     return result
 
 
 def xlsx_value_to_str(value):
     """
     Take a xls formatted value and try to make a string representation.
     """
```

### Comparing `pyxform-1.8.0/pyxform/xls2xform.py` & `pyxform-1.9.0/pyxform/xls2xform.py`

 * *Files identical despite different names*

### Comparing `pyxform-1.8.0/pyxform.egg-info/PKG-INFO` & `pyxform-1.9.0/pyxform.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 1.2
 Name: pyxform
-Version: 1.8.0
+Version: 1.9.0
 Summary: A Python package to create XForms for ODK Collect.
 Home-page: http://pypi.python.org/pypi/pyxform/
 Author: github.com/xlsform
 Author-email: info@xlsform.org
 License: UNKNOWN
 Description: ===============
-        pyxform v1.8.0
+        pyxform v1.9.0
         ===============
         
         |python| |black|
         
         .. |python| image:: https://img.shields.io/badge/python-3.7,3.8,3.9-blue.svg
             :target: https://www.python.org/downloads
         
@@ -130,34 +130,40 @@
         
         2. Run all tests through Validate by setting the default for ``run_odk_validate`` to ``kwargs.get("run_odk_validate", True)`` in ``pyxform/tests_v1/pyxform_test_case.py``.
         3. Draft a new GitHub release with the list of merged PRs. Follow the title and description pattern of the previous release.
         4. Checkout a release branch from latest upstream master.
         5. Update ``CHANGES.txt`` with the text of the draft release.
         6. Update ``README.rst``, ``setup.py``, ``pyxform/__init__.py`` with the new release version number.
         7. Commit, push the branch, and initiate a pull request. Wait for tests to pass, then merge the PR.
-        8. In a clean new release only directory, checkout master.
-        9. Create a new virtualenv in this directory to ensure a clean Python environment::
+        8. Tag the release and it will automatically be published
+        
+        Manually releasing
+        ===================
+        Releases are now automatic. These instructions are provided for forks or for a future change in process.
+        
+        1. In a clean new release only directory, check out master.
+        2. Create a new virtualenv in this directory to ensure a clean Python environment::
         
              /usr/local/bin/python3.8 -m venv pyxform-release
              . pyxform-release/bin/activate
         
-        10. Install the production and packaging requirements::
+        3. Install the production and packaging requirements::
         
              pip install -e .
              pip install wheel twine
         
-        11. Cleanup build and dist folders::
+        4. Clean up build and dist folders::
         
              rm -rf build dist pyxform.egg-info
         
-        12. Prepare ``sdist`` and ``bdist_wheel`` distributions::
+        5. Prepare ``sdist`` and ``bdist_wheel`` distributions::
         
              python setup.py sdist bdist_wheel
         
-        13. Publish release to PyPI with ``twine``::
+        6. Publish release to PyPI with ``twine``::
         
              twine upload dist/pyxform-*-py3-none-any.whl dist/pyxform-*.tar.gz
         
-        14. Tag the GitHub release and publish it.
+        7. Tag the GitHub release and publish it.
         
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pyxform-1.8.0/pyxform.egg-info/SOURCES.txt` & `pyxform-1.9.0/pyxform.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -36,8 +36,9 @@
 pyxform/validators/updater.py
 pyxform/validators/util.py
 pyxform/validators/enketo_validate/__init__.py
 pyxform/validators/odk_validate/__init__.py
 pyxform/validators/odk_validate/bin/ODK_Validate.jar
 pyxform/validators/odk_validate/bin/installed.json
 pyxform/validators/pyxform/__init__.py
-pyxform/validators/pyxform/missing_translations_check.py
+pyxform/validators/pyxform/missing_translations_check.py
+pyxform/validators/pyxform/select_from_file_params.py
```

### Comparing `pyxform-1.8.0/setup.py` & `pyxform-1.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 pyxform - Python library that converts XLSForms to XForms.
 """
 from setuptools import find_packages, setup
 
 
 setup(
     name="pyxform",
-    version="1.8.0",
+    version="1.9.0",
     author="github.com/xlsform",
     author_email="info@xlsform.org",
     packages=find_packages(exclude=["tests", "tests.*"]),
     package_data={
         "pyxform.validators.odk_validate": ["bin/*.*"],
         "pyxform": ["iana_subtags.txt"],
     },
```

