# Comparing `tmp/nepali-1.0.0.tar.gz` & `tmp/nepali-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nepali-1.0.0.tar", last modified: Tue May  2 15:35:41 2023, max compression
+gzip compressed data, was "nepali-1.0.1.tar", last modified: Tue May 16 15:34:07 2023, max compression
```

## Comparing `nepali-1.0.0.tar` & `nepali-1.0.1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:35:41.442139 nepali-1.0.0/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1073 2023-05-02 15:35:29.000000 nepali-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14148 2023-05-02 15:35:41.442139 nepali-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13454 2023-05-02 15:35:29.000000 nepali-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:35:41.438139 nepali-1.0.0/nepali/
--rwxr-xr-x   0 runner    (1001) docker     (123)       16 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3437 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/char.py
--rw-r--r--   0 runner    (1001) docker     (123)    13551 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/date_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:35:41.438139 nepali-1.0.0/nepali/datetime/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/datetime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12071 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/datetime/_datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     8750 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/datetime/_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/datetime/_humanize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/datetime/_nepalimonth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/datetime/_nepaliweek.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/datetime/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:35:41.438139 nepali-1.0.0/nepali/datetime/parser/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/datetime/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/datetime/parser/_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8546 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/datetime/parser/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/datetime/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      329 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:35:41.442139 nepali-1.0.0/nepali/locations/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/locations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   216494 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/locations/_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/locations/_locations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/locations/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/locations/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:35:41.442139 nepali-1.0.0/nepali/number/
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/number/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19019 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/number/_nepalinumber.py
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/number/_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/number/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/phone_number.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:35:41.442139 nepali-1.0.0/nepali/templatetags/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/templatetags/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1245 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/templatetags/nepalidatetime.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/templatetags/nepalinumber.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:35:41.442139 nepali-1.0.0/nepali/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/tests/test_date_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13621 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/tests/test_datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/tests/test_humanize.py
--rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/tests/test_locations.py
--rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/tests/test_nepalimonth.py
--rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/tests/test_nepaliweek.py
--rw-r--r--   0 runner    (1001) docker     (123)   117623 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/tests/test_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    11726 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/tests/test_phone_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/tests/test_timezone.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1962 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/timezone.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      241 2023-05-02 15:35:29.000000 nepali-1.0.0/nepali/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 15:35:41.438139 nepali-1.0.0/nepali.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14148 2023-05-02 15:35:41.000000 nepali-1.0.0/nepali.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-02 15:35:41.000000 nepali-1.0.0/nepali.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 15:35:41.000000 nepali-1.0.0/nepali.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-02 15:35:41.000000 nepali-1.0.0/nepali.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 15:35:41.442139 nepali-1.0.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1625 2023-05-02 15:35:29.000000 nepali-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:34:07.179097 nepali-1.0.1/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1073 2023-05-16 15:33:53.000000 nepali-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14992 2023-05-16 15:34:07.179097 nepali-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14298 2023-05-16 15:33:53.000000 nepali-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:34:07.171095 nepali-1.0.1/nepali/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       16 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3437 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/char.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13551 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/date_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:34:07.175096 nepali-1.0.1/nepali/datetime/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/datetime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12071 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/datetime/_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8750 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/datetime/_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/datetime/_humanize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/datetime/_nepalimonth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/datetime/_nepaliweek.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/datetime/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:34:07.175096 nepali-1.0.1/nepali/datetime/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/datetime/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/datetime/parser/_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8546 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/datetime/parser/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/datetime/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      329 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:34:07.175096 nepali-1.0.1/nepali/locations/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/locations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   216494 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/locations/_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/locations/_locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/locations/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/locations/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:34:07.175096 nepali-1.0.1/nepali/number/
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/number/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19019 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/number/_nepalinumber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/number/_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/number/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/phone_number.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:34:07.175096 nepali-1.0.1/nepali/templatetags/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/templatetags/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4754 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/templatetags/nepalidatetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/templatetags/nepalinumber.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:34:07.179097 nepali-1.0.1/nepali/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/tests/test_date_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13621 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/tests/test_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/tests/test_humanize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/tests/test_locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/tests/test_nepalimonth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/tests/test_nepaliweek.py
+-rw-r--r--   0 runner    (1001) docker     (123)   117623 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/tests/test_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11726 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/tests/test_phone_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/tests/test_timezone.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1962 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/timezone.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      241 2023-05-16 15:33:53.000000 nepali-1.0.1/nepali/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:34:07.175096 nepali-1.0.1/nepali.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14992 2023-05-16 15:34:07.000000 nepali-1.0.1/nepali.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-16 15:34:07.000000 nepali-1.0.1/nepali.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 15:34:07.000000 nepali-1.0.1/nepali.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-16 15:34:07.000000 nepali-1.0.1/nepali.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 15:34:07.179097 nepali-1.0.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1625 2023-05-16 15:33:53.000000 nepali-1.0.1/setup.py
```

### Comparing `nepali-1.0.0/LICENSE` & `nepali-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nepali-1.0.0/PKG-INFO` & `nepali-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: nepali
-Version: 1.0.0
-Summary: nepalidatetime compatible with python's datetime feature. Converting nepali date to english, parsing nepali datetime, nepali timezone, and timedelta support in nepali datetime
-Home-page: https://github.com/opensource-nepal/py-nepali
-Author: opensource-nepal
-Author-email: aj3sshh@gmail.com, sugatbajracharya49@gmail.com
-Keywords: nepali date conversion,convert date,nepali date time,python convert date,parse nepali date time
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # nepali
 
 [![PyPI version](https://badge.fury.io/py/nepali.svg)](https://badge.fury.io/py/nepali)
 [![CI status](https://github.com/opensource-nepal/py-nepali/actions/workflows/python-package.yml/badge.svg?branch=master)](https://github.com/opensource-nepal/py-nepali/actions)
 [![Downloads](https://img.shields.io/pypi/dm/nepali.svg?maxAge=180)](https://pypi.org/project/nepali/)
 [![codecov](https://codecov.io/gh/opensource-nepal/py-nepali/branch/master/graph/badge.svg?token=PTUHYWCJ4I)](https://codecov.io/gh/opensource-nepal/py-nepali)
 
@@ -59,18 +45,19 @@
    - [date_converter](#date_converter)
    - [nepalidate](#nepalidate)
    - [nepalidatetime](#nepalidatetime)
    - [nepalihumanize](#nepalihumanize)
    - [timezone](#timezone)
    - [parse](#parse)
    - [strftime() and strptime() Format Codes](#strftime-and-strptime-format-codes)
-2. [Numbers](#numbers)
-    - [nepalinumber](#nepalinumber)
-3. [Phone Number](#phone-number)
-4. [Locations](#locations)
+1. [Numbers](#numbers)
+   - [nepalinumber](#nepalinumber)
+1. [Phone Number](#phone-number)
+1. [Locations](#locations)
+1. [For Django Template](#for-django-template)
 
 ## Date and Time
 
 ### date_converter
 
 Date converter module converts english date to nepali and nepali date to english. It doesn't contain any extra functionality.
 
@@ -454,37 +441,79 @@
 INSTALLED_APPS = [
     ...
     'nepali',
     ...
 ]
 ```
 
+### nepalidatetime
+
 In your Template
 
 ```python
 {% load nepalidatetime %}
 ```
 
+#### nepalinow
+
+`nepalinow` renders the current Nepali date and time in 'en-US' locale (English).
+
 ```python
 {% nepalinow %}
 ```
 
 ```python
 {% nepalinow '%Y-%m-%d' %}
 ```
 
+#### nepalinow_ne
+
+`nepalinow_ne` renders the current Nepali date and time in 'ne' locale (Nepali).
+
 ```python
-{{ datetimeobj|nepalidate:"%Y-%m-%d" }}
-{{ datetimeobj|nepalidate_en:"%Y-%m-%d" }}
+{% nepalinow_ne %}
 ```
 
+#### nepalidate
+
+`nepalidate` renders the datetime object into nepali datetime format in 'en-US' locale (English).
+
 ```python
-{{ datetimeobj|nepalihumanize }}
+{{ datetime_obj|nepalidate:"%Y-%m-%d" }}
 ```
 
+#### nepalidate_ne
+
+`nepalidate_ne` renders the datetime object into nepali datetime format in 'ne' locale (Nepali).
+
+```python
+{{ datetime_obj|nepalidate_ne:"%Y-%m-%d" }}
+```
+
+#### nepalihumanize
+
+`nepalihumanize` renders the datetime object to a human readable form for 'ne' locale (Nepali)
+
+```python
+{{ datetime_obj|nepalihumanize }}
+```
+
+### nepalinumber
+
+In your Template
+
+```python
+{% load nepalinumber %}
+```
+
+`nepalinumber` renders the english number into nepali format (devanagari)
+
 ```python
 {{ forloop.counter|nepalinumber }}
+
+{{ 150|nepalinumber }}
 ```
 
+
 ## Contribution
 
 We appreciate feedback and contribution to this package. To get started please see our [contribution guide](CONTRIBUTION.md)
```

### Comparing `nepali-1.0.0/README.md` & `nepali-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: nepali
+Version: 1.0.1
+Summary: nepalidatetime compatible with python's datetime feature. Converting nepali date to english, parsing nepali datetime, nepali timezone, and timedelta support in nepali datetime
+Home-page: https://github.com/opensource-nepal/py-nepali
+Author: opensource-nepal
+Author-email: aj3sshh@gmail.com, sugatbajracharya49@gmail.com
+Keywords: nepali date conversion,convert date,nepali date time,python convert date,parse nepali date time
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # nepali
 
 [![PyPI version](https://badge.fury.io/py/nepali.svg)](https://badge.fury.io/py/nepali)
 [![CI status](https://github.com/opensource-nepal/py-nepali/actions/workflows/python-package.yml/badge.svg?branch=master)](https://github.com/opensource-nepal/py-nepali/actions)
 [![Downloads](https://img.shields.io/pypi/dm/nepali.svg?maxAge=180)](https://pypi.org/project/nepali/)
 [![codecov](https://codecov.io/gh/opensource-nepal/py-nepali/branch/master/graph/badge.svg?token=PTUHYWCJ4I)](https://codecov.io/gh/opensource-nepal/py-nepali)
 
@@ -45,18 +59,19 @@
    - [date_converter](#date_converter)
    - [nepalidate](#nepalidate)
    - [nepalidatetime](#nepalidatetime)
    - [nepalihumanize](#nepalihumanize)
    - [timezone](#timezone)
    - [parse](#parse)
    - [strftime() and strptime() Format Codes](#strftime-and-strptime-format-codes)
-2. [Numbers](#numbers)
-    - [nepalinumber](#nepalinumber)
-3. [Phone Number](#phone-number)
-4. [Locations](#locations)
+1. [Numbers](#numbers)
+   - [nepalinumber](#nepalinumber)
+1. [Phone Number](#phone-number)
+1. [Locations](#locations)
+1. [For Django Template](#for-django-template)
 
 ## Date and Time
 
 ### date_converter
 
 Date converter module converts english date to nepali and nepali date to english. It doesn't contain any extra functionality.
 
@@ -440,37 +455,79 @@
 INSTALLED_APPS = [
     ...
     'nepali',
     ...
 ]
 ```
 
+### nepalidatetime
+
 In your Template
 
 ```python
 {% load nepalidatetime %}
 ```
 
+#### nepalinow
+
+`nepalinow` renders the current Nepali date and time in 'en-US' locale (English).
+
 ```python
 {% nepalinow %}
 ```
 
 ```python
 {% nepalinow '%Y-%m-%d' %}
 ```
 
+#### nepalinow_ne
+
+`nepalinow_ne` renders the current Nepali date and time in 'ne' locale (Nepali).
+
 ```python
-{{ datetimeobj|nepalidate:"%Y-%m-%d" }}
-{{ datetimeobj|nepalidate_en:"%Y-%m-%d" }}
+{% nepalinow_ne %}
 ```
 
+#### nepalidate
+
+`nepalidate` renders the datetime object into nepali datetime format in 'en-US' locale (English).
+
 ```python
-{{ datetimeobj|nepalihumanize }}
+{{ datetime_obj|nepalidate:"%Y-%m-%d" }}
 ```
 
+#### nepalidate_ne
+
+`nepalidate_ne` renders the datetime object into nepali datetime format in 'ne' locale (Nepali).
+
+```python
+{{ datetime_obj|nepalidate_ne:"%Y-%m-%d" }}
+```
+
+#### nepalihumanize
+
+`nepalihumanize` renders the datetime object to a human readable form for 'ne' locale (Nepali)
+
+```python
+{{ datetime_obj|nepalihumanize }}
+```
+
+### nepalinumber
+
+In your Template
+
+```python
+{% load nepalinumber %}
+```
+
+`nepalinumber` renders the english number into nepali format (devanagari)
+
 ```python
 {{ forloop.counter|nepalinumber }}
+
+{{ 150|nepalinumber }}
 ```
 
+
 ## Contribution
 
 We appreciate feedback and contribution to this package. To get started please see our [contribution guide](CONTRIBUTION.md)
```

### Comparing `nepali-1.0.0/nepali/char.py` & `nepali-1.0.1/nepali/char.py`

 * *Files identical despite different names*

### Comparing `nepali-1.0.0/nepali/date_converter.py` & `nepali-1.0.1/nepali/date_converter.py`

 * *Files identical despite different names*

### Comparing `nepali-1.0.0/nepali/datetime/_datetime.py` & `nepali-1.0.1/nepali/datetime/_datetime.py`

 * *Files identical despite different names*

### Comparing `nepali-1.0.0/nepali/datetime/_formatter.py` & `nepali-1.0.1/nepali/datetime/_formatter.py`

 * *Files identical despite different names*

### Comparing `nepali-1.0.0/nepali/datetime/_humanize.py` & `nepali-1.0.1/nepali/datetime/_humanize.py`

 * *Files identical despite different names*

### Comparing `nepali-1.0.0/nepali/datetime/_nepalimonth.py` & `nepali-1.0.1/nepali/datetime/_nepalimonth.py`

 * *Files identical despite different names*

### Comparing `nepali-1.0.0/nepali/datetime/_nepaliweek.py` & `nepali-1.0.1/nepali/datetime/_nepaliweek.py`

 * *Files identical despite different names*

### Comparing `nepali-1.0.0/nepali/datetime/constants.py` & `nepali-1.0.1/nepali/datetime/constants.py`

 * *Files identical despite different names*

### Comparing `nepali-1.0.0/nepali/datetime/parser/_parser.py` & `nepali-1.0.1/nepali/datetime/parser/_parser.py`

 * *Files identical despite different names*

### Comparing `nepali-1.0.0/nepali/datetime/parser/validators.py` & `nepali-1.0.1/nepali/datetime/parser/validators.py`

 * *Files identical despite different names*

### Comparing `nepali-1.0.0/nepali/datetime/utils.py` & `nepali-1.0.1/nepali/datetime/utils.py`

 * *Files identical despite different names*

### Comparing `nepali-1.0.0/nepali/locations/_data.py` & `nepali-1.0.1/nepali/locations/_data.py`

 * *Files identical despite different names*

### Comparing `nepali-1.0.0/nepali/locations/_locations.py` & `nepali-1.0.1/nepali/locations/_locations.py`

 * *Files identical despite different names*

### Comparing `nepali-1.0.0/nepali/locations/models.py` & `nepali-1.0.1/nepali/locations/models.py`

 * *Files identical despite different names*

### Comparing `nepali-1.0.0/nepali/locations/utils.py` & `nepali-1.0.1/nepali/locations/utils.py`

 * *Files identical despite different names*

### Comparing `nepali-1.0.0/nepali/number/_nepalinumber.py` & `nepali-1.0.1/nepali/number/_nepalinumber.py`

 * *Files identical despite different names*

### Comparing `nepali-1.0.0/nepali/number/_number.py` & `nepali-1.0.1/nepali/number/_number.py`

 * *Files identical despite different names*

### Comparing `nepali-1.0.0/nepali/number/utils.py` & `nepali-1.0.1/nepali/number/utils.py`

 * *Files identical despite different names*

### Comparing `nepali-1.0.0/nepali/phone_number.py` & `nepali-1.0.1/nepali/phone_number.py`

 * *Files identical despite different names*

### Comparing `nepali-1.0.0/nepali/tests/test_date_converter.py` & `nepali-1.0.1/nepali/tests/test_date_converter.py`

 * *Files identical despite different names*

### Comparing `nepali-1.0.0/nepali/tests/test_datetime.py` & `nepali-1.0.1/nepali/tests/test_datetime.py`

 * *Files identical despite different names*

### Comparing `nepali-1.0.0/nepali/tests/test_humanize.py` & `nepali-1.0.1/nepali/tests/test_humanize.py`

 * *Files identical despite different names*

### Comparing `nepali-1.0.0/nepali/tests/test_locations.py` & `nepali-1.0.1/nepali/tests/test_locations.py`

 * *Files identical despite different names*

### Comparing `nepali-1.0.0/nepali/tests/test_nepalimonth.py` & `nepali-1.0.1/nepali/tests/test_nepalimonth.py`

 * *Files identical despite different names*

### Comparing `nepali-1.0.0/nepali/tests/test_nepaliweek.py` & `nepali-1.0.1/nepali/tests/test_nepaliweek.py`

 * *Files identical despite different names*

### Comparing `nepali-1.0.0/nepali/tests/test_number.py` & `nepali-1.0.1/nepali/tests/test_number.py`

 * *Files identical despite different names*

### Comparing `nepali-1.0.0/nepali/tests/test_parser.py` & `nepali-1.0.1/nepali/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `nepali-1.0.0/nepali/tests/test_phone_number.py` & `nepali-1.0.1/nepali/tests/test_phone_number.py`

 * *Files identical despite different names*

### Comparing `nepali-1.0.0/nepali/tests/test_timezone.py` & `nepali-1.0.1/nepali/tests/test_timezone.py`

 * *Files identical despite different names*

### Comparing `nepali-1.0.0/nepali/timezone.py` & `nepali-1.0.1/nepali/timezone.py`

 * *Files identical despite different names*

### Comparing `nepali-1.0.0/nepali.egg-info/PKG-INFO` & `nepali-1.0.1/nepali.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nepali
-Version: 1.0.0
+Version: 1.0.1
 Summary: nepalidatetime compatible with python's datetime feature. Converting nepali date to english, parsing nepali datetime, nepali timezone, and timedelta support in nepali datetime
 Home-page: https://github.com/opensource-nepal/py-nepali
 Author: opensource-nepal
 Author-email: aj3sshh@gmail.com, sugatbajracharya49@gmail.com
 Keywords: nepali date conversion,convert date,nepali date time,python convert date,parse nepali date time
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -59,18 +59,19 @@
    - [date_converter](#date_converter)
    - [nepalidate](#nepalidate)
    - [nepalidatetime](#nepalidatetime)
    - [nepalihumanize](#nepalihumanize)
    - [timezone](#timezone)
    - [parse](#parse)
    - [strftime() and strptime() Format Codes](#strftime-and-strptime-format-codes)
-2. [Numbers](#numbers)
-    - [nepalinumber](#nepalinumber)
-3. [Phone Number](#phone-number)
-4. [Locations](#locations)
+1. [Numbers](#numbers)
+   - [nepalinumber](#nepalinumber)
+1. [Phone Number](#phone-number)
+1. [Locations](#locations)
+1. [For Django Template](#for-django-template)
 
 ## Date and Time
 
 ### date_converter
 
 Date converter module converts english date to nepali and nepali date to english. It doesn't contain any extra functionality.
 
@@ -454,37 +455,79 @@
 INSTALLED_APPS = [
     ...
     'nepali',
     ...
 ]
 ```
 
+### nepalidatetime
+
 In your Template
 
 ```python
 {% load nepalidatetime %}
 ```
 
+#### nepalinow
+
+`nepalinow` renders the current Nepali date and time in 'en-US' locale (English).
+
 ```python
 {% nepalinow %}
 ```
 
 ```python
 {% nepalinow '%Y-%m-%d' %}
 ```
 
+#### nepalinow_ne
+
+`nepalinow_ne` renders the current Nepali date and time in 'ne' locale (Nepali).
+
+```python
+{% nepalinow_ne %}
+```
+
+#### nepalidate
+
+`nepalidate` renders the datetime object into nepali datetime format in 'en-US' locale (English).
+
+```python
+{{ datetime_obj|nepalidate:"%Y-%m-%d" }}
+```
+
+#### nepalidate_ne
+
+`nepalidate_ne` renders the datetime object into nepali datetime format in 'ne' locale (Nepali).
+
+```python
+{{ datetime_obj|nepalidate_ne:"%Y-%m-%d" }}
+```
+
+#### nepalihumanize
+
+`nepalihumanize` renders the datetime object to a human readable form for 'ne' locale (Nepali)
+
 ```python
-{{ datetimeobj|nepalidate:"%Y-%m-%d" }}
-{{ datetimeobj|nepalidate_en:"%Y-%m-%d" }}
+{{ datetime_obj|nepalihumanize }}
 ```
 
+### nepalinumber
+
+In your Template
+
 ```python
-{{ datetimeobj|nepalihumanize }}
+{% load nepalinumber %}
 ```
 
+`nepalinumber` renders the english number into nepali format (devanagari)
+
 ```python
 {{ forloop.counter|nepalinumber }}
+
+{{ 150|nepalinumber }}
 ```
 
+
 ## Contribution
 
 We appreciate feedback and contribution to this package. To get started please see our [contribution guide](CONTRIBUTION.md)
```

### Comparing `nepali-1.0.0/nepali.egg-info/SOURCES.txt` & `nepali-1.0.1/nepali.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nepali-1.0.0/setup.py` & `nepali-1.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     os.system("python3 setup.py sdist bdist_wheel")
     os.system("twine upload dist/*")
     sys.exit()
 
 
 setuptools.setup(
     name="nepali",
-    version="1.0.0",
+    version="1.0.1",
     author="opensource-nepal",
     author_email="aj3sshh@gmail.com, sugatbajracharya49@gmail.com",
     description="nepalidatetime compatible with python's datetime feature. "
     "Converting nepali date to english, parsing nepali datetime, "
     "nepali timezone, and timedelta support in nepali datetime",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

