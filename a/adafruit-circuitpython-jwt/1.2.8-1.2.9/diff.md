# Comparing `tmp/adafruit-circuitpython-jwt-1.2.8.tar.gz` & `tmp/adafruit-circuitpython-jwt-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-jwt-1.2.8.tar", last modified: Thu Jun  9 19:11:52 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-jwt-1.2.9.tar", last modified: Wed Jun 22 17:40:38 2022, max compression
```

## Comparing `adafruit-circuitpython-jwt-1.2.8.tar` & `adafruit-circuitpython-jwt-1.2.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 19:11:52.540711 adafruit-circuitpython-jwt-1.2.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 19:11:52.536711 adafruit-circuitpython-jwt-1.2.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 19:11:52.540711 adafruit-circuitpython-jwt-1.2.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-06-09 19:11:38.000000 adafruit-circuitpython-jwt-1.2.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 19:11:52.540711 adafruit-circuitpython-jwt-1.2.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-06-09 19:11:38.000000 adafruit-circuitpython-jwt-1.2.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-06-09 19:11:38.000000 adafruit-circuitpython-jwt-1.2.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-06-09 19:11:38.000000 adafruit-circuitpython-jwt-1.2.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-06-09 19:11:38.000000 adafruit-circuitpython-jwt-1.2.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-06-09 19:11:38.000000 adafruit-circuitpython-jwt-1.2.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-06-09 19:11:38.000000 adafruit-circuitpython-jwt-1.2.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-06-09 19:11:38.000000 adafruit-circuitpython-jwt-1.2.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-06-09 19:11:38.000000 adafruit-circuitpython-jwt-1.2.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1103 2022-06-09 19:11:38.000000 adafruit-circuitpython-jwt-1.2.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 19:11:52.540711 adafruit-circuitpython-jwt-1.2.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-06-09 19:11:38.000000 adafruit-circuitpython-jwt-1.2.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-06-09 19:11:38.000000 adafruit-circuitpython-jwt-1.2.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-06-09 19:11:38.000000 adafruit-circuitpython-jwt-1.2.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4804 2022-06-09 19:11:52.540711 adafruit-circuitpython-jwt-1.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4098 2022-06-09 19:11:38.000000 adafruit-circuitpython-jwt-1.2.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-09 19:11:38.000000 adafruit-circuitpython-jwt-1.2.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 19:11:52.540711 adafruit-circuitpython-jwt-1.2.8/adafruit_circuitpython_jwt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4804 2022-06-09 19:11:52.000000 adafruit-circuitpython-jwt-1.2.8/adafruit_circuitpython_jwt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      866 2022-06-09 19:11:52.000000 adafruit-circuitpython-jwt-1.2.8/adafruit_circuitpython_jwt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-09 19:11:52.000000 adafruit-circuitpython-jwt-1.2.8/adafruit_circuitpython_jwt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-06-09 19:11:52.000000 adafruit-circuitpython-jwt-1.2.8/adafruit_circuitpython_jwt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-06-09 19:11:52.000000 adafruit-circuitpython-jwt-1.2.8/adafruit_circuitpython_jwt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     7587 2022-06-09 19:11:38.000000 adafruit-circuitpython-jwt-1.2.8/adafruit_jwt.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 19:11:52.540711 adafruit-circuitpython-jwt-1.2.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 19:11:52.540711 adafruit-circuitpython-jwt-1.2.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-06-09 19:11:38.000000 adafruit-circuitpython-jwt-1.2.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-06-09 19:11:38.000000 adafruit-circuitpython-jwt-1.2.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      262 2022-06-09 19:11:38.000000 adafruit-circuitpython-jwt-1.2.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-09 19:11:38.000000 adafruit-circuitpython-jwt-1.2.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5407 2022-06-09 19:11:38.000000 adafruit-circuitpython-jwt-1.2.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      180 2022-06-09 19:11:38.000000 adafruit-circuitpython-jwt-1.2.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-09 19:11:38.000000 adafruit-circuitpython-jwt-1.2.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      970 2022-06-09 19:11:38.000000 adafruit-circuitpython-jwt-1.2.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-09 19:11:38.000000 adafruit-circuitpython-jwt-1.2.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-06-09 19:11:38.000000 adafruit-circuitpython-jwt-1.2.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 19:11:52.540711 adafruit-circuitpython-jwt-1.2.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      752 2022-06-09 19:11:38.000000 adafruit-circuitpython-jwt-1.2.8/examples/jwt_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      208 2022-06-09 19:11:38.000000 adafruit-circuitpython-jwt-1.2.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-09 19:11:52.540711 adafruit-circuitpython-jwt-1.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1995 2022-06-09 19:11:38.000000 adafruit-circuitpython-jwt-1.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 17:40:38.633958 adafruit-circuitpython-jwt-1.2.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 17:40:38.625958 adafruit-circuitpython-jwt-1.2.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 17:40:38.629958 adafruit-circuitpython-jwt-1.2.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-06-22 17:40:14.000000 adafruit-circuitpython-jwt-1.2.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 17:40:38.629958 adafruit-circuitpython-jwt-1.2.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-06-22 17:40:14.000000 adafruit-circuitpython-jwt-1.2.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-06-22 17:40:14.000000 adafruit-circuitpython-jwt-1.2.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-06-22 17:40:14.000000 adafruit-circuitpython-jwt-1.2.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-06-22 17:40:14.000000 adafruit-circuitpython-jwt-1.2.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-06-22 17:40:14.000000 adafruit-circuitpython-jwt-1.2.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-06-22 17:40:14.000000 adafruit-circuitpython-jwt-1.2.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-06-22 17:40:14.000000 adafruit-circuitpython-jwt-1.2.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-06-22 17:40:14.000000 adafruit-circuitpython-jwt-1.2.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1103 2022-06-22 17:40:14.000000 adafruit-circuitpython-jwt-1.2.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 17:40:38.629958 adafruit-circuitpython-jwt-1.2.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-06-22 17:40:14.000000 adafruit-circuitpython-jwt-1.2.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-06-22 17:40:14.000000 adafruit-circuitpython-jwt-1.2.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-06-22 17:40:14.000000 adafruit-circuitpython-jwt-1.2.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4804 2022-06-22 17:40:38.633958 adafruit-circuitpython-jwt-1.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4098 2022-06-22 17:40:14.000000 adafruit-circuitpython-jwt-1.2.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-22 17:40:14.000000 adafruit-circuitpython-jwt-1.2.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 17:40:38.633958 adafruit-circuitpython-jwt-1.2.9/adafruit_circuitpython_jwt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4804 2022-06-22 17:40:38.000000 adafruit-circuitpython-jwt-1.2.9/adafruit_circuitpython_jwt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      866 2022-06-22 17:40:38.000000 adafruit-circuitpython-jwt-1.2.9/adafruit_circuitpython_jwt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-22 17:40:38.000000 adafruit-circuitpython-jwt-1.2.9/adafruit_circuitpython_jwt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-06-22 17:40:38.000000 adafruit-circuitpython-jwt-1.2.9/adafruit_circuitpython_jwt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2022-06-22 17:40:38.000000 adafruit-circuitpython-jwt-1.2.9/adafruit_circuitpython_jwt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     7526 2022-06-22 17:40:14.000000 adafruit-circuitpython-jwt-1.2.9/adafruit_jwt.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 17:40:38.633958 adafruit-circuitpython-jwt-1.2.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 17:40:38.633958 adafruit-circuitpython-jwt-1.2.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-06-22 17:40:14.000000 adafruit-circuitpython-jwt-1.2.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-06-22 17:40:14.000000 adafruit-circuitpython-jwt-1.2.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      262 2022-06-22 17:40:14.000000 adafruit-circuitpython-jwt-1.2.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-22 17:40:14.000000 adafruit-circuitpython-jwt-1.2.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5407 2022-06-22 17:40:14.000000 adafruit-circuitpython-jwt-1.2.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      180 2022-06-22 17:40:14.000000 adafruit-circuitpython-jwt-1.2.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-22 17:40:14.000000 adafruit-circuitpython-jwt-1.2.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      970 2022-06-22 17:40:14.000000 adafruit-circuitpython-jwt-1.2.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-22 17:40:14.000000 adafruit-circuitpython-jwt-1.2.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-06-22 17:40:14.000000 adafruit-circuitpython-jwt-1.2.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 17:40:38.633958 adafruit-circuitpython-jwt-1.2.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)      752 2022-06-22 17:40:14.000000 adafruit-circuitpython-jwt-1.2.9/examples/jwt_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      208 2022-06-22 17:40:14.000000 adafruit-circuitpython-jwt-1.2.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-22 17:40:38.633958 adafruit-circuitpython-jwt-1.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1995 2022-06-22 17:40:14.000000 adafruit-circuitpython-jwt-1.2.9/setup.py
```

### Comparing `adafruit-circuitpython-jwt-1.2.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-jwt-1.2.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-jwt-1.2.8/.github/workflows/build.yml` & `adafruit-circuitpython-jwt-1.2.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-jwt-1.2.8/.github/workflows/release.yml` & `adafruit-circuitpython-jwt-1.2.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-jwt-1.2.8/.gitignore` & `adafruit-circuitpython-jwt-1.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-jwt-1.2.8/.pre-commit-config.yaml` & `adafruit-circuitpython-jwt-1.2.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-jwt-1.2.8/.pylintrc` & `adafruit-circuitpython-jwt-1.2.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-jwt-1.2.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-jwt-1.2.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-jwt-1.2.8/LICENSE` & `adafruit-circuitpython-jwt-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-jwt-1.2.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-jwt-1.2.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-jwt-1.2.8/LICENSES/MIT.txt` & `adafruit-circuitpython-jwt-1.2.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-jwt-1.2.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-jwt-1.2.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-jwt-1.2.8/PKG-INFO` & `adafruit-circuitpython-jwt-1.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-jwt
-Version: 1.2.8
+Version: 1.2.9
 Summary: JSON Web Token Authentication 
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_JWT
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit blinka circuitpython micropython jwt jwt,json,token,authentication
 Platform: UNKNOWN
```

### Comparing `adafruit-circuitpython-jwt-1.2.8/README.rst` & `adafruit-circuitpython-jwt-1.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-jwt-1.2.8/adafruit_circuitpython_jwt.egg-info/PKG-INFO` & `adafruit-circuitpython-jwt-1.2.9/adafruit_circuitpython_jwt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-jwt
-Version: 1.2.8
+Version: 1.2.9
 Summary: JSON Web Token Authentication 
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_JWT
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit blinka circuitpython micropython jwt jwt,json,token,authentication
 Platform: UNKNOWN
```

### Comparing `adafruit-circuitpython-jwt-1.2.8/adafruit_circuitpython_jwt.egg-info/SOURCES.txt` & `adafruit-circuitpython-jwt-1.2.9/adafruit_circuitpython_jwt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-jwt-1.2.8/adafruit_jwt.py` & `adafruit-circuitpython-jwt-1.2.9/adafruit_jwt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # SPDX-FileCopyrightText: 2019 Brent Rubell for Adafruit Industries
 #
 # SPDX-License-Identifier: MIT
 
 """
 `adafruit_jwt`
-================================================================================
+==============
 
 JSON Web Token Authentication
 
 * Author(s): Brent Rubell
 
 Implementation Notes
 --------------------
@@ -23,43 +23,44 @@
 * Adafruit's RSA library:
   https://github.com/adafruit/Adafruit_CircuitPython_RSA
 
 * Adafruit's binascii library:
   https://github.com/adafruit/Adafruit_CircuitPython_RSA
 
 """
+
 try:
     from typing import Tuple, Union, Optional
     from circuitpython_typing import ReadableBuffer
 except ImportError:
     pass
 
 import io
 import json
 from adafruit_rsa import PrivateKey, sign
-
 from adafruit_binascii import b2a_base64, a2b_base64
 
 
 __version__ = "0.0.0-auto.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_JWT.git"
 
 # pylint: disable=no-member
 class JWT:
     """JSON Web Token helper for CircuitPython. Warning: JWTs are
     credentials, which can grant access to resources. Be careful
     where you paste them!
-    :param str algo: Encryption algorithm used for claims. Can be None.
 
+    :param str algo: Encryption algorithm used for claims. Can be None.
     """
 
     @staticmethod
     def validate(jwt: str) -> Tuple[str, dict]:
         """Validates a provided JWT. Does not support validating
         nested signing. Returns JOSE Header and claim set.
+
         :param str jwt: JSON Web Token.
         :returns: The message's decoded JOSE header and claims.
         :rtype: tuple
         """
         # Verify JWT contains at least one period ('.')
         if jwt.find(".") == -1:
             raise ValueError("ProvidedJWT must have at least one period")
@@ -86,14 +87,15 @@
     def generate(
         claims: dict,
         private_key_data: Optional[str] = None,
         algo: Optional[str] = None,
         headers: Optional[dict] = None,
     ) -> str:
         """Generates and returns a new JSON Web Token.
+
         :param dict claims: JWT claims set
         :param str private_key_data: Decoded RSA private key data.
         :param str algo: algorithm to be used. One of None, RS256, RS384 or RS512.
         :param dict headers: additional headers for the claim.
         :rtype: str
         """
         # Allow for unencrypted JWTs
@@ -151,24 +153,26 @@
     printable = digits + ascii_letters + punctuation + whitespace
 
     @staticmethod
     def urlsafe_b64encode(payload: ReadableBuffer) -> str:
         """Encode bytes-like object using the URL- and filesystem-safe alphabet,
         which substitutes - instead of + and _ instead of / in
         the standard Base64 alphabet, and return the encoded bytes.
+
         :param bytes payload: bytes-like object.
         """
         return STRING_TOOLS.translate(
             b2a_base64(payload)[:-1].decode("utf-8"), {ord("+"): "-", ord("/"): "_"}
         )
 
     @staticmethod
     def urlsafe_b64decode(payload: Union[ReadableBuffer, str]) -> str:
         """Decode bytes-like object or ASCII string using the URL
         and filesystem-safe alphabet
+
         :param bytes payload: bytes-like object or ASCII string
         """
         return a2b_base64(STRING_TOOLS._bytes_from_decode_data(payload)).decode("utf-8")
 
     @staticmethod
     def _bytes_from_decode_data(str_data: Union[ReadableBuffer, str]) -> bytes:
         # Types acceptable as binary data
@@ -190,14 +194,15 @@
 
     # Port of CPython str.translate to Pure-Python by Johan Brichau, 2019
     # https://github.com/jbrichau/TrackingPrototype/blob/master/Device/lib/string.py
     @staticmethod
     def translate(s: str, table: dict) -> str:
         """Return a copy of the string in which each character
         has been mapped through the given translation table.
+
         :param string s: String to-be-character-table.
         :param dict table: Translation table.
         """
         sb = io.StringIO()
         for c in s:
             v = ord(c)
             if v in table:
```

### Comparing `adafruit-circuitpython-jwt-1.2.8/docs/_static/favicon.ico` & `adafruit-circuitpython-jwt-1.2.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-jwt-1.2.8/docs/conf.py` & `adafruit-circuitpython-jwt-1.2.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-jwt-1.2.8/docs/index.rst` & `adafruit-circuitpython-jwt-1.2.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-jwt-1.2.8/examples/jwt_simpletest.py` & `adafruit-circuitpython-jwt-1.2.9/examples/jwt_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-jwt-1.2.8/setup.py` & `adafruit-circuitpython-jwt-1.2.9/setup.py`

 * *Files identical despite different names*

