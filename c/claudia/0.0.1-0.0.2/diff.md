# Comparing `tmp/claudia-0.0.1.tar.gz` & `tmp/claudia-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "claudia-0.0.1.tar", last modified: Mon May 15 19:29:37 2023, max compression
+gzip compressed data, was "claudia-0.0.2.tar", last modified: Mon May 15 21:50:43 2023, max compression
```

## Comparing `claudia-0.0.1.tar` & `claudia-0.0.2.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-15 19:29:37.616114 claudia-0.0.1/
--rw-r--r--   0 ksaxena    (502) staff       (20)     1073 2023-05-11 10:47:00.000000 claudia-0.0.1/LICENSE
--rw-r--r--   0 ksaxena    (502) staff       (20)     1866 2023-05-15 19:29:37.615854 claudia-0.0.1/PKG-INFO
--rw-r--r--   0 ksaxena    (502) staff       (20)     3114 2023-05-12 13:50:25.000000 claudia-0.0.1/README.md
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-15 19:29:37.600920 claudia-0.0.1/claudia.egg-info/
--rw-r--r--   0 ksaxena    (502) staff       (20)     1866 2023-05-15 19:29:37.000000 claudia-0.0.1/claudia.egg-info/PKG-INFO
--rw-r--r--   0 ksaxena    (502) staff       (20)     1624 2023-05-15 19:29:37.000000 claudia-0.0.1/claudia.egg-info/SOURCES.txt
--rw-r--r--   0 ksaxena    (502) staff       (20)        1 2023-05-15 19:29:37.000000 claudia-0.0.1/claudia.egg-info/dependency_links.txt
--rw-r--r--   0 ksaxena    (502) staff       (20)       49 2023-05-15 19:29:37.000000 claudia-0.0.1/claudia.egg-info/entry_points.txt
--rw-r--r--   0 ksaxena    (502) staff       (20)       79 2023-05-15 19:29:37.000000 claudia-0.0.1/claudia.egg-info/requires.txt
--rw-r--r--   0 ksaxena    (502) staff       (20)        8 2023-05-15 19:29:37.000000 claudia-0.0.1/claudia.egg-info/top_level.txt
--rw-r--r--   0 ksaxena    (502) staff       (20)       38 2023-05-15 19:29:37.616239 claudia-0.0.1/setup.cfg
--rw-r--r--   0 ksaxena    (502) staff       (20)     1982 2023-05-15 19:29:33.000000 claudia-0.0.1/setup.py
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-15 19:29:37.594810 claudia-0.0.1/src/
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-15 19:29:37.601502 claudia-0.0.1/src/claudia/
--rw-r--r--   0 ksaxena    (502) staff       (20)        0 2023-05-15 18:14:02.000000 claudia-0.0.1/src/claudia/__init__.py
--rw-r--r--   0 ksaxena    (502) staff       (20)     9412 2023-05-15 18:14:02.000000 claudia-0.0.1/src/claudia/claudia.py
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-15 19:29:37.602774 claudia-0.0.1/src/claudia/features/
--rw-r--r--   0 ksaxena    (502) staff       (20)    14321 2023-05-15 18:14:02.000000 claudia-0.0.1/src/claudia/features/nft_burn_mint.feature
--rw-r--r--   0 ksaxena    (502) staff       (20)     5371 2023-05-15 18:14:02.000000 claudia-0.0.1/src/claudia/features/payments.feature
--rw-r--r--   0 ksaxena    (502) staff       (20)    11071 2023-05-15 18:14:02.000000 claudia-0.0.1/src/claudia/features/trustline.feature
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-15 19:29:37.605615 claudia-0.0.1/src/claudia/javascript/
--rwxr-xr-x   0 ksaxena    (502) staff       (20)      118 2023-05-15 18:14:02.000000 claudia-0.0.1/src/claudia/javascript/cleanup
--rw-r--r--   0 ksaxena    (502) staff       (20)      145 2023-05-15 18:14:02.000000 claudia-0.0.1/src/claudia/javascript/cucumber.js
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-15 19:29:37.605970 claudia-0.0.1/src/claudia/javascript/features/
--rw-r--r--   0 ksaxena    (502) staff       (20)     1226 2023-05-15 18:14:02.000000 claudia-0.0.1/src/claudia/javascript/features/context.js
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-15 19:29:37.606283 claudia-0.0.1/src/claudia/javascript/features/lib/
--rw-r--r--   0 ksaxena    (502) staff       (20)     2106 2023-05-15 18:14:02.000000 claudia-0.0.1/src/claudia/javascript/features/lib/ObjFactory.js
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-15 19:29:37.608519 claudia-0.0.1/src/claudia/javascript/features/steps/
--rw-r--r--   0 ksaxena    (502) staff       (20)    38728 2023-05-15 18:14:02.000000 claudia-0.0.1/src/claudia/javascript/features/steps/common.js
--rw-r--r--   0 ksaxena    (502) staff       (20)      300 2023-05-15 18:14:02.000000 claudia-0.0.1/src/claudia/javascript/features/steps/constants.js
--rw-r--r--   0 ksaxena    (502) staff       (20)    71153 2023-05-15 18:14:02.000000 claudia-0.0.1/src/claudia/javascript/features/steps/nft_mint_burn.js
--rw-r--r--   0 ksaxena    (502) staff       (20)    19024 2023-05-15 18:14:02.000000 claudia-0.0.1/src/claudia/javascript/features/steps/payments.js
--rw-r--r--   0 ksaxena    (502) staff       (20)    59478 2023-05-15 18:14:02.000000 claudia-0.0.1/src/claudia/javascript/features/steps/trustline.js
--rw-r--r--   0 ksaxena    (502) staff       (20)   129466 2023-05-15 18:14:02.000000 claudia-0.0.1/src/claudia/javascript/package-lock.json
--rw-r--r--   0 ksaxena    (502) staff       (20)      221 2023-05-15 18:14:02.000000 claudia-0.0.1/src/claudia/javascript/package.json
--rwxr-xr-x   0 ksaxena    (502) staff       (20)      869 2023-05-15 18:14:02.000000 claudia-0.0.1/src/claudia/javascript/runSetup
--rwxr-xr-x   0 ksaxena    (502) staff       (20)     4674 2023-05-15 18:14:02.000000 claudia-0.0.1/src/claudia/javascript/runTest
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-15 19:29:37.610615 claudia-0.0.1/src/claudia/python/
--rw-r--r--   0 ksaxena    (502) staff       (20)        0 2023-05-15 18:14:02.000000 claudia-0.0.1/src/claudia/python/__init__.py
--rw-r--r--   0 ksaxena    (502) staff       (20)      107 2023-05-15 18:14:02.000000 claudia-0.0.1/src/claudia/python/behave.ini
--rwxr-xr-x   0 ksaxena    (502) staff       (20)      123 2023-05-15 18:14:02.000000 claudia-0.0.1/src/claudia/python/cleanup
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-15 19:29:37.611476 claudia-0.0.1/src/claudia/python/features/
--rw-r--r--   0 ksaxena    (502) staff       (20)        0 2023-05-15 18:14:02.000000 claudia-0.0.1/src/claudia/python/features/__init__.py
--rw-r--r--   0 ksaxena    (502) staff       (20)     2977 2023-05-15 18:14:02.000000 claudia-0.0.1/src/claudia/python/features/environment.py
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-15 19:29:37.612312 claudia-0.0.1/src/claudia/python/features/exceptions/
--rw-r--r--   0 ksaxena    (502) staff       (20)       49 2023-05-15 18:14:02.000000 claudia-0.0.1/src/claudia/python/features/exceptions/InvalidInputException.py
--rw-r--r--   0 ksaxena    (502) staff       (20)       60 2023-05-15 18:14:02.000000 claudia-0.0.1/src/claudia/python/features/exceptions/UnconfiguredEnvironmentException.py
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-15 19:29:37.613116 claudia-0.0.1/src/claudia/python/features/lib/
--rw-r--r--   0 ksaxena    (502) staff       (20)      301 2023-05-15 18:14:02.000000 claudia-0.0.1/src/claudia/python/features/lib/Helpers.py
--rw-r--r--   0 ksaxena    (502) staff       (20)     7674 2023-05-15 18:14:02.000000 claudia-0.0.1/src/claudia/python/features/lib/ObjFactory.py
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-15 19:29:37.615339 claudia-0.0.1/src/claudia/python/features/steps/
--rw-r--r--   0 ksaxena    (502) staff       (20)    24750 2023-05-15 18:14:02.000000 claudia-0.0.1/src/claudia/python/features/steps/common.py
--rw-r--r--   0 ksaxena    (502) staff       (20)      251 2023-05-15 18:14:02.000000 claudia-0.0.1/src/claudia/python/features/steps/constants.py
--rw-r--r--   0 ksaxena    (502) staff       (20)    66340 2023-05-15 18:14:02.000000 claudia-0.0.1/src/claudia/python/features/steps/nft_mint_burn.py
--rw-r--r--   0 ksaxena    (502) staff       (20)    21822 2023-05-15 18:14:02.000000 claudia-0.0.1/src/claudia/python/features/steps/payments.py
--rw-r--r--   0 ksaxena    (502) staff       (20)    54620 2023-05-15 18:14:02.000000 claudia-0.0.1/src/claudia/python/features/steps/trustline.py
--rwxr-xr-x   0 ksaxena    (502) staff       (20)     1381 2023-05-15 18:14:02.000000 claudia-0.0.1/src/claudia/python/runSetup
--rwxr-xr-x   0 ksaxena    (502) staff       (20)     5634 2023-05-15 18:14:02.000000 claudia-0.0.1/src/claudia/python/runTest
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-15 21:50:43.648445 claudia-0.0.2/
+-rw-r--r--   0 ksaxena    (502) staff       (20)     1073 2023-05-11 10:47:00.000000 claudia-0.0.2/LICENSE
+-rw-r--r--   0 ksaxena    (502) staff       (20)     1866 2023-05-15 21:50:43.648235 claudia-0.0.2/PKG-INFO
+-rw-r--r--   0 ksaxena    (502) staff       (20)     3088 2023-05-15 19:36:08.000000 claudia-0.0.2/README.md
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-15 21:50:43.631653 claudia-0.0.2/claudia.egg-info/
+-rw-r--r--   0 ksaxena    (502) staff       (20)     1866 2023-05-15 21:50:43.000000 claudia-0.0.2/claudia.egg-info/PKG-INFO
+-rw-r--r--   0 ksaxena    (502) staff       (20)     1624 2023-05-15 21:50:43.000000 claudia-0.0.2/claudia.egg-info/SOURCES.txt
+-rw-r--r--   0 ksaxena    (502) staff       (20)        1 2023-05-15 21:50:43.000000 claudia-0.0.2/claudia.egg-info/dependency_links.txt
+-rw-r--r--   0 ksaxena    (502) staff       (20)       49 2023-05-15 21:50:43.000000 claudia-0.0.2/claudia.egg-info/entry_points.txt
+-rw-r--r--   0 ksaxena    (502) staff       (20)       79 2023-05-15 21:50:43.000000 claudia-0.0.2/claudia.egg-info/requires.txt
+-rw-r--r--   0 ksaxena    (502) staff       (20)        8 2023-05-15 21:50:43.000000 claudia-0.0.2/claudia.egg-info/top_level.txt
+-rw-r--r--   0 ksaxena    (502) staff       (20)       38 2023-05-15 21:50:43.648517 claudia-0.0.2/setup.cfg
+-rw-r--r--   0 ksaxena    (502) staff       (20)     1982 2023-05-15 21:50:02.000000 claudia-0.0.2/setup.py
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-15 21:50:43.625474 claudia-0.0.2/src/
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-15 21:50:43.632552 claudia-0.0.2/src/claudia/
+-rw-r--r--   0 ksaxena    (502) staff       (20)        0 2023-05-15 18:14:02.000000 claudia-0.0.2/src/claudia/__init__.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)     9411 2023-05-15 21:49:11.000000 claudia-0.0.2/src/claudia/claudia.py
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-15 21:50:43.634154 claudia-0.0.2/src/claudia/features/
+-rw-r--r--   0 ksaxena    (502) staff       (20)    14321 2023-05-15 18:14:02.000000 claudia-0.0.2/src/claudia/features/nft_burn_mint.feature
+-rw-r--r--   0 ksaxena    (502) staff       (20)     5371 2023-05-15 18:14:02.000000 claudia-0.0.2/src/claudia/features/payments.feature
+-rw-r--r--   0 ksaxena    (502) staff       (20)    11071 2023-05-15 18:14:02.000000 claudia-0.0.2/src/claudia/features/trustline.feature
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-15 21:50:43.637416 claudia-0.0.2/src/claudia/javascript/
+-rwxr-xr-x   0 ksaxena    (502) staff       (20)      118 2023-05-15 18:14:02.000000 claudia-0.0.2/src/claudia/javascript/cleanup
+-rw-r--r--   0 ksaxena    (502) staff       (20)      145 2023-05-15 18:14:02.000000 claudia-0.0.2/src/claudia/javascript/cucumber.js
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-15 21:50:43.637807 claudia-0.0.2/src/claudia/javascript/features/
+-rw-r--r--   0 ksaxena    (502) staff       (20)     1226 2023-05-15 18:14:02.000000 claudia-0.0.2/src/claudia/javascript/features/context.js
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-15 21:50:43.638106 claudia-0.0.2/src/claudia/javascript/features/lib/
+-rw-r--r--   0 ksaxena    (502) staff       (20)     2106 2023-05-15 18:14:02.000000 claudia-0.0.2/src/claudia/javascript/features/lib/ObjFactory.js
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-15 21:50:43.640441 claudia-0.0.2/src/claudia/javascript/features/steps/
+-rw-r--r--   0 ksaxena    (502) staff       (20)    38728 2023-05-15 18:14:02.000000 claudia-0.0.2/src/claudia/javascript/features/steps/common.js
+-rw-r--r--   0 ksaxena    (502) staff       (20)      300 2023-05-15 18:14:02.000000 claudia-0.0.2/src/claudia/javascript/features/steps/constants.js
+-rw-r--r--   0 ksaxena    (502) staff       (20)    71153 2023-05-15 18:14:02.000000 claudia-0.0.2/src/claudia/javascript/features/steps/nft_mint_burn.js
+-rw-r--r--   0 ksaxena    (502) staff       (20)    19024 2023-05-15 18:14:02.000000 claudia-0.0.2/src/claudia/javascript/features/steps/payments.js
+-rw-r--r--   0 ksaxena    (502) staff       (20)    59478 2023-05-15 18:14:02.000000 claudia-0.0.2/src/claudia/javascript/features/steps/trustline.js
+-rw-r--r--   0 ksaxena    (502) staff       (20)   129466 2023-05-15 18:14:02.000000 claudia-0.0.2/src/claudia/javascript/package-lock.json
+-rw-r--r--   0 ksaxena    (502) staff       (20)      221 2023-05-15 18:14:02.000000 claudia-0.0.2/src/claudia/javascript/package.json
+-rwxr-xr-x   0 ksaxena    (502) staff       (20)      869 2023-05-15 18:14:02.000000 claudia-0.0.2/src/claudia/javascript/runSetup
+-rwxr-xr-x   0 ksaxena    (502) staff       (20)     4674 2023-05-15 18:14:02.000000 claudia-0.0.2/src/claudia/javascript/runTest
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-15 21:50:43.643149 claudia-0.0.2/src/claudia/python/
+-rw-r--r--   0 ksaxena    (502) staff       (20)        0 2023-05-15 18:14:02.000000 claudia-0.0.2/src/claudia/python/__init__.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)      107 2023-05-15 18:14:02.000000 claudia-0.0.2/src/claudia/python/behave.ini
+-rwxr-xr-x   0 ksaxena    (502) staff       (20)      123 2023-05-15 18:14:02.000000 claudia-0.0.2/src/claudia/python/cleanup
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-15 21:50:43.643835 claudia-0.0.2/src/claudia/python/features/
+-rw-r--r--   0 ksaxena    (502) staff       (20)        0 2023-05-15 18:14:02.000000 claudia-0.0.2/src/claudia/python/features/__init__.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)     2977 2023-05-15 18:14:02.000000 claudia-0.0.2/src/claudia/python/features/environment.py
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-15 21:50:43.644636 claudia-0.0.2/src/claudia/python/features/exceptions/
+-rw-r--r--   0 ksaxena    (502) staff       (20)       49 2023-05-15 18:14:02.000000 claudia-0.0.2/src/claudia/python/features/exceptions/InvalidInputException.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)       60 2023-05-15 18:14:02.000000 claudia-0.0.2/src/claudia/python/features/exceptions/UnconfiguredEnvironmentException.py
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-15 21:50:43.645387 claudia-0.0.2/src/claudia/python/features/lib/
+-rw-r--r--   0 ksaxena    (502) staff       (20)      301 2023-05-15 18:14:02.000000 claudia-0.0.2/src/claudia/python/features/lib/Helpers.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)     7674 2023-05-15 18:14:02.000000 claudia-0.0.2/src/claudia/python/features/lib/ObjFactory.py
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-15 21:50:43.647724 claudia-0.0.2/src/claudia/python/features/steps/
+-rw-r--r--   0 ksaxena    (502) staff       (20)    24750 2023-05-15 18:14:02.000000 claudia-0.0.2/src/claudia/python/features/steps/common.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)      251 2023-05-15 18:14:02.000000 claudia-0.0.2/src/claudia/python/features/steps/constants.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)    66340 2023-05-15 18:14:02.000000 claudia-0.0.2/src/claudia/python/features/steps/nft_mint_burn.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)    21822 2023-05-15 18:14:02.000000 claudia-0.0.2/src/claudia/python/features/steps/payments.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)    54620 2023-05-15 18:14:02.000000 claudia-0.0.2/src/claudia/python/features/steps/trustline.py
+-rwxr-xr-x   0 ksaxena    (502) staff       (20)     1381 2023-05-15 18:14:02.000000 claudia-0.0.2/src/claudia/python/runSetup
+-rwxr-xr-x   0 ksaxena    (502) staff       (20)     5634 2023-05-15 18:14:02.000000 claudia-0.0.2/src/claudia/python/runTest
```

### Comparing `claudia-0.0.1/LICENSE` & `claudia-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `claudia-0.0.1/PKG-INFO` & `claudia-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: claudia
-Version: 0.0.1
+Version: 0.0.2
 Summary: Run XRPL Automated Tests
 Home-page: https://xrpl.org/
 Download-URL: https://gitlab.ops.ripple.com/xrpledger/xrpl-nocode-automation
 Author: Kausty Saxena
 Author-email: ksaxena@ripple.com
 Keywords: ripple xrpl python javascript
 Description-Content-Type: text/markdown
```

### Comparing `claudia-0.0.1/README.md` & `claudia-0.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # xrpl-nocode-automation
-This repository contains code which allows users to run automated XRPL tests on different networks. It also generates a python package named 'claudia', which can be installed from [PyPi](https://test.pypi.org/project/claudia/).
+This repository contains code which allows users to run automated XRPL tests on different networks. It also generates a python package named 'claudia', which can be installed from [PyPi](https://pypi.org/project/claudia/).
 
 ---
 
 ## General prerequisites
 Please have the following installed on your machine before proceeding further:
 - [Python3](https://www.python.org/downloads/)
 - [pip](https://pip.pypa.io/en/stable/installation/)
@@ -22,17 +22,17 @@
 ---
 
 ## How to run the tests?
 This section contains instructions for running the tests either directly using both `claudia` and the codebase directly.
 
 
 ### Run tests using claudia
- - Install claudia from [PyPi](https://test.pypi.org/project/claudia/), using the following command:
+ - Install claudia from [PyPi](https://pypi.org/project/claudia/), using the following command:
    
-        pip install -i https://test.pypi.org/simple/ claudia
+        pip install claudia
  - From your terminal, run: `claudia`
    - Use `--help` option with the CLI to view supported options.
    - Example Usage:
      - `claudia build`: Builds rippled locally.
      - `claudia network`: Launches local network using Rippled. Needs access to built rippled.
      - `claudia run python`: Runs Python tests on local network. Use `--help` to view other supported options. 
      - `claudia run javascript`: Runs Javascript tests on local network. Use `--help` to view other supported options. 
@@ -43,15 +43,15 @@
 - Run `./runSetup`. This is a one time step and does not need to be repeated each time.
 - Run the tests:
   - If you wish to run the tests on a local network, run `./runTest`. Please view [Local Network](#launch-local-network) to launch a local network.
   - If you wish to run the tests on different networks, use `./runTest --help` flag to see more options.
 ---
 
 ### How to publish claudia to PyPi?
-- Create an account with PyPi, if you don't have one. Verify the email.
+- Create an account with [PyPi](https://pypi.org/), if you don't have one. Verify the email.
 - Clone this [repo](https://gitlab.ops.ripple.com/xrpledger/xrpl-nocode-automation)
 - Install/update pip, if needed:
   
         python3 -m pip install --upgrade pip
 - Install /update setuptools, if needed.
   
         pip install --upgrade setuptools
@@ -61,8 +61,8 @@
         rm -fr build/ dist/ claudia.egg-info
 - Generate the package locally using the following command:
 
         python3 setup.py sdist bdist_wheel
 
 - Upload the package to PyPi, using the following command (you will need to enter your PyPi credentials):
         
-        python3 -m twine upload --verbose --repository testpypi dist/*
+        python3 -m twine upload --verbose --repository pypi dist/*
```

### Comparing `claudia-0.0.1/claudia.egg-info/PKG-INFO` & `claudia-0.0.2/claudia.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: claudia
-Version: 0.0.1
+Version: 0.0.2
 Summary: Run XRPL Automated Tests
 Home-page: https://xrpl.org/
 Download-URL: https://gitlab.ops.ripple.com/xrpledger/xrpl-nocode-automation
 Author: Kausty Saxena
 Author-email: ksaxena@ripple.com
 Keywords: ripple xrpl python javascript
 Description-Content-Type: text/markdown
```

### Comparing `claudia-0.0.1/claudia.egg-info/SOURCES.txt` & `claudia-0.0.2/claudia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `claudia-0.0.1/setup.py` & `claudia-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         requirements = content.split('\n')
 
     return requirements
 
 
 setup(
     name='claudia',
-    version='0.0.1',
+    version='0.0.2',
     description='Run XRPL Automated Tests',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     author="Kausty Saxena",
     author_email="ksaxena@ripple.com",
     keywords="ripple xrpl python javascript",
     url='https://xrpl.org/',
```

### Comparing `claudia-0.0.1/src/claudia/claudia.py` & `claudia-0.0.2/src/claudia/claudia.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,19 +107,19 @@
     install_js_dependencies_if_needed()
 
 
 def set_python_launch_vars(network, client_type):
     if network == "local":
         if client_type == "websocket":
             connectionScheme = "ws"
-            connectionURL = "127.0.0.5:6006"
+            connectionURL = "127.0.0.5:6001"
             connectionType = "websocket"
         elif client_type == "jsonrpc":
             connectionScheme = "http"
-            connectionURL = "127.0.0.5:51234"
+            connectionURL = "127.0.0.5:5001"
             connectionType = "jsonrpc"
         else:
             raise Exception("{} is not a valid connectionType".format(client_type))
     elif network == "devnet":
         if client_type == "websocket":
             connectionScheme = "wss"
             connectionURL = "s.devnet.rippletest.net:51233"
```

### Comparing `claudia-0.0.1/src/claudia/features/nft_burn_mint.feature` & `claudia-0.0.2/src/claudia/features/nft_burn_mint.feature`

 * *Files identical despite different names*

### Comparing `claudia-0.0.1/src/claudia/features/payments.feature` & `claudia-0.0.2/src/claudia/features/payments.feature`

 * *Files identical despite different names*

### Comparing `claudia-0.0.1/src/claudia/features/trustline.feature` & `claudia-0.0.2/src/claudia/features/trustline.feature`

 * *Files identical despite different names*

### Comparing `claudia-0.0.1/src/claudia/javascript/features/context.js` & `claudia-0.0.2/src/claudia/javascript/features/context.js`

 * *Files identical despite different names*

### Comparing `claudia-0.0.1/src/claudia/javascript/features/lib/ObjFactory.js` & `claudia-0.0.2/src/claudia/javascript/features/lib/ObjFactory.js`

 * *Files identical despite different names*

### Comparing `claudia-0.0.1/src/claudia/javascript/features/steps/common.js` & `claudia-0.0.2/src/claudia/javascript/features/steps/common.js`

 * *Files identical despite different names*

### Comparing `claudia-0.0.1/src/claudia/javascript/features/steps/nft_mint_burn.js` & `claudia-0.0.2/src/claudia/javascript/features/steps/nft_mint_burn.js`

 * *Files identical despite different names*

### Comparing `claudia-0.0.1/src/claudia/javascript/features/steps/payments.js` & `claudia-0.0.2/src/claudia/javascript/features/steps/payments.js`

 * *Files identical despite different names*

### Comparing `claudia-0.0.1/src/claudia/javascript/features/steps/trustline.js` & `claudia-0.0.2/src/claudia/javascript/features/steps/trustline.js`

 * *Files identical despite different names*

### Comparing `claudia-0.0.1/src/claudia/javascript/package-lock.json` & `claudia-0.0.2/src/claudia/javascript/package-lock.json`

 * *Files identical despite different names*

### Comparing `claudia-0.0.1/src/claudia/javascript/runSetup` & `claudia-0.0.2/src/claudia/javascript/runSetup`

 * *Files identical despite different names*

### Comparing `claudia-0.0.1/src/claudia/javascript/runTest` & `claudia-0.0.2/src/claudia/javascript/runTest`

 * *Files identical despite different names*

### Comparing `claudia-0.0.1/src/claudia/python/features/environment.py` & `claudia-0.0.2/src/claudia/python/features/environment.py`

 * *Files identical despite different names*

### Comparing `claudia-0.0.1/src/claudia/python/features/lib/ObjFactory.py` & `claudia-0.0.2/src/claudia/python/features/lib/ObjFactory.py`

 * *Files identical despite different names*

### Comparing `claudia-0.0.1/src/claudia/python/features/steps/common.py` & `claudia-0.0.2/src/claudia/python/features/steps/common.py`

 * *Files identical despite different names*

### Comparing `claudia-0.0.1/src/claudia/python/features/steps/nft_mint_burn.py` & `claudia-0.0.2/src/claudia/python/features/steps/nft_mint_burn.py`

 * *Files identical despite different names*

### Comparing `claudia-0.0.1/src/claudia/python/features/steps/payments.py` & `claudia-0.0.2/src/claudia/python/features/steps/payments.py`

 * *Files identical despite different names*

### Comparing `claudia-0.0.1/src/claudia/python/features/steps/trustline.py` & `claudia-0.0.2/src/claudia/python/features/steps/trustline.py`

 * *Files identical despite different names*

### Comparing `claudia-0.0.1/src/claudia/python/runSetup` & `claudia-0.0.2/src/claudia/python/runSetup`

 * *Files identical despite different names*

### Comparing `claudia-0.0.1/src/claudia/python/runTest` & `claudia-0.0.2/src/claudia/python/runTest`

 * *Files identical despite different names*

