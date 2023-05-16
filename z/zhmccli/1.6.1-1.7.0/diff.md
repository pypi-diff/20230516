# Comparing `tmp/zhmccli-1.6.1.tar.gz` & `tmp/zhmccli-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhmccli-1.6.1.tar", last modified: Thu May 11 15:50:14 2023, max compression
+gzip compressed data, was "zhmccli-1.7.0.tar", last modified: Tue May 16 09:30:39 2023, max compression
```

## Comparing `zhmccli-1.6.1.tar` & `zhmccli-1.7.0.tar`

### file list

```diff
@@ -1,42 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:50:14.812418 zhmccli-1.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)    10143 2023-05-11 15:49:19.000000 zhmccli-1.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-11 15:50:02.000000 zhmccli-1.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-05-11 15:50:14.812418 zhmccli-1.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-05-11 15:49:19.000000 zhmccli-1.6.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-05-11 15:49:19.000000 zhmccli-1.6.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 15:50:14.812418 zhmccli-1.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-05-11 15:49:19.000000 zhmccli-1.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:50:14.808418 zhmccli-1.6.1/zhmccli/
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-11 15:49:19.000000 zhmccli-1.6.1/zhmccli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17363 2023-05-11 15:49:19.000000 zhmccli-1.6.1/zhmccli/_cmd_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)    17148 2023-05-11 15:49:19.000000 zhmccli-1.6.1/zhmccli/_cmd_capacitygroup.py
--rw-r--r--   0 runner    (1001) docker     (123)    14919 2023-05-11 15:49:19.000000 zhmccli-1.6.1/zhmccli/_cmd_character_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-05-11 15:49:19.000000 zhmccli-1.6.1/zhmccli/_cmd_console.py
--rw-r--r--   0 runner    (1001) docker     (123)    37856 2023-05-11 15:49:19.000000 zhmccli-1.6.1/zhmccli/_cmd_cpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11127 2023-05-11 15:49:19.000000 zhmccli-1.6.1/zhmccli/_cmd_hba.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-11 15:49:19.000000 zhmccli-1.6.1/zhmccli/_cmd_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    32122 2023-05-11 15:49:19.000000 zhmccli-1.6.1/zhmccli/_cmd_lpar.py
--rw-r--r--   0 runner    (1001) docker     (123)    25429 2023-05-11 15:49:19.000000 zhmccli-1.6.1/zhmccli/_cmd_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    22552 2023-05-11 15:49:19.000000 zhmccli-1.6.1/zhmccli/_cmd_nic.py
--rw-r--r--   0 runner    (1001) docker     (123)    73313 2023-05-11 15:49:19.000000 zhmccli-1.6.1/zhmccli/_cmd_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-05-11 15:49:19.000000 zhmccli-1.6.1/zhmccli/_cmd_password_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     6634 2023-05-11 15:49:19.000000 zhmccli-1.6.1/zhmccli/_cmd_port.py
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-05-11 15:49:19.000000 zhmccli-1.6.1/zhmccli/_cmd_session.py
--rw-r--r--   0 runner    (1001) docker     (123)    28044 2023-05-11 15:49:19.000000 zhmccli-1.6.1/zhmccli/_cmd_storagegroup.py
--rw-r--r--   0 runner    (1001) docker     (123)    18123 2023-05-11 15:49:19.000000 zhmccli-1.6.1/zhmccli/_cmd_storagevolume.py
--rw-r--r--   0 runner    (1001) docker     (123)    47796 2023-05-11 15:49:19.000000 zhmccli-1.6.1/zhmccli/_cmd_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    23920 2023-05-11 15:49:19.000000 zhmccli-1.6.1/zhmccli/_cmd_user_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    13052 2023-05-11 15:49:19.000000 zhmccli-1.6.1/zhmccli/_cmd_vfunction.py
--rw-r--r--   0 runner    (1001) docker     (123)    11934 2023-05-11 15:49:19.000000 zhmccli-1.6.1/zhmccli/_cmd_vstorageresource.py
--rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-05-11 15:49:19.000000 zhmccli-1.6.1/zhmccli/_cmd_vswitch.py
--rw-r--r--   0 runner    (1001) docker     (123)    54900 2023-05-11 15:49:19.000000 zhmccli-1.6.1/zhmccli/_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-11 15:49:19.000000 zhmccli-1.6.1/zhmccli/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    16299 2023-05-11 15:49:19.000000 zhmccli-1.6.1/zhmccli/zhmccli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:50:14.812418 zhmccli-1.6.1/zhmccli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-05-11 15:50:14.000000 zhmccli-1.6.1/zhmccli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-11 15:50:14.000000 zhmccli-1.6.1/zhmccli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 15:50:14.000000 zhmccli-1.6.1/zhmccli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-11 15:50:14.000000 zhmccli-1.6.1/zhmccli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-11 15:50:14.000000 zhmccli-1.6.1/zhmccli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-11 15:50:14.000000 zhmccli-1.6.1/zhmccli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 15:50:14.000000 zhmccli-1.6.1/zhmccli.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:30:39.505578 zhmccli-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10143 2023-05-16 09:29:42.000000 zhmccli-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-16 09:30:26.000000 zhmccli-1.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-05-16 09:30:39.505578 zhmccli-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-05-16 09:29:42.000000 zhmccli-1.7.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-05-16 09:29:42.000000 zhmccli-1.7.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 09:30:39.505578 zhmccli-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-05-16 09:29:42.000000 zhmccli-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:30:39.501578 zhmccli-1.7.0/zhmccli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-16 09:29:42.000000 zhmccli-1.7.0/zhmccli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21483 2023-05-16 09:29:42.000000 zhmccli-1.7.0/zhmccli/_cmd_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17148 2023-05-16 09:29:42.000000 zhmccli-1.7.0/zhmccli/_cmd_capacitygroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9083 2023-05-16 09:29:42.000000 zhmccli-1.7.0/zhmccli/_cmd_certificates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14919 2023-05-16 09:29:42.000000 zhmccli-1.7.0/zhmccli/_cmd_character_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7880 2023-05-16 09:29:42.000000 zhmccli-1.7.0/zhmccli/_cmd_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39073 2023-05-16 09:29:42.000000 zhmccli-1.7.0/zhmccli/_cmd_cpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11127 2023-05-16 09:29:42.000000 zhmccli-1.7.0/zhmccli/_cmd_hba.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-16 09:29:42.000000 zhmccli-1.7.0/zhmccli/_cmd_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14832 2023-05-16 09:29:42.000000 zhmccli-1.7.0/zhmccli/_cmd_ldap_server_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34886 2023-05-16 09:29:42.000000 zhmccli-1.7.0/zhmccli/_cmd_lpar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25429 2023-05-16 09:29:42.000000 zhmccli-1.7.0/zhmccli/_cmd_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22552 2023-05-16 09:29:42.000000 zhmccli-1.7.0/zhmccli/_cmd_nic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76333 2023-05-16 09:29:42.000000 zhmccli-1.7.0/zhmccli/_cmd_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-05-16 09:29:42.000000 zhmccli-1.7.0/zhmccli/_cmd_password_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6634 2023-05-16 09:29:42.000000 zhmccli-1.7.0/zhmccli/_cmd_port.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-05-16 09:29:42.000000 zhmccli-1.7.0/zhmccli/_cmd_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28044 2023-05-16 09:29:42.000000 zhmccli-1.7.0/zhmccli/_cmd_storagegroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18123 2023-05-16 09:29:42.000000 zhmccli-1.7.0/zhmccli/_cmd_storagevolume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-05-16 09:29:42.000000 zhmccli-1.7.0/zhmccli/_cmd_unmanaged_cpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47796 2023-05-16 09:29:42.000000 zhmccli-1.7.0/zhmccli/_cmd_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23920 2023-05-16 09:29:42.000000 zhmccli-1.7.0/zhmccli/_cmd_user_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13052 2023-05-16 09:29:42.000000 zhmccli-1.7.0/zhmccli/_cmd_vfunction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11934 2023-05-16 09:29:42.000000 zhmccli-1.7.0/zhmccli/_cmd_vstorageresource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-05-16 09:29:42.000000 zhmccli-1.7.0/zhmccli/_cmd_vswitch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56112 2023-05-16 09:29:42.000000 zhmccli-1.7.0/zhmccli/_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-16 09:29:42.000000 zhmccli-1.7.0/zhmccli/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16527 2023-05-16 09:29:42.000000 zhmccli-1.7.0/zhmccli/zhmccli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:30:39.505578 zhmccli-1.7.0/zhmccli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-05-16 09:30:39.000000 zhmccli-1.7.0/zhmccli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-16 09:30:39.000000 zhmccli-1.7.0/zhmccli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 09:30:39.000000 zhmccli-1.7.0/zhmccli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-16 09:30:39.000000 zhmccli-1.7.0/zhmccli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-16 09:30:39.000000 zhmccli-1.7.0/zhmccli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 09:30:39.000000 zhmccli-1.7.0/zhmccli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 09:30:39.000000 zhmccli-1.7.0/zhmccli.egg-info/zip-safe
```

### Comparing `zhmccli-1.6.1/LICENSE` & `zhmccli-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zhmccli-1.6.1/MANIFEST.in` & `zhmccli-1.7.0/MANIFEST.in`

 * *Files 7% similar despite different names*

```diff
@@ -2,28 +2,31 @@
 include setup.py
 include LICENSE
 include README.rst
 include requirements.txt
 include zhmccli/__init__.py
 include zhmccli/_cmd_adapter.py
 include zhmccli/_cmd_capacitygroup.py
+include zhmccli/_cmd_certificates.py
 include zhmccli/_cmd_character_rule.py
 include zhmccli/_cmd_console.py
 include zhmccli/_cmd_cpc.py
 include zhmccli/_cmd_hba.py
 include zhmccli/_cmd_info.py
+include zhmccli/_cmd_ldap_server_definition.py
 include zhmccli/_cmd_lpar.py
 include zhmccli/_cmd_metrics.py
 include zhmccli/_cmd_nic.py
 include zhmccli/_cmd_partition.py
 include zhmccli/_cmd_password_rule.py
 include zhmccli/_cmd_port.py
 include zhmccli/_cmd_session.py
 include zhmccli/_cmd_storagegroup.py
 include zhmccli/_cmd_storagevolume.py
+include zhmccli/_cmd_unmanaged_cpc.py
 include zhmccli/_cmd_user.py
 include zhmccli/_cmd_user_role.py
 include zhmccli/_cmd_vfunction.py
 include zhmccli/_cmd_vstorageresource.py
 include zhmccli/_cmd_vswitch.py
 include zhmccli/_helper.py
 include zhmccli/_version.py
```

### Comparing `zhmccli-1.6.1/PKG-INFO` & `zhmccli-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhmccli
-Version: 1.6.1
+Version: 1.7.0
 Summary: A CLI for the IBM Z HMC, written in pure Python
 Home-page: https://github.com/zhmcclient/zhmccli
 Author: Juergen Leopold, Andreas Maier
 Author-email: leopoldj@de.ibm.com, maiera@de.ibm.com
 Maintainer: Andreas Maier, Kathir Velusamy
 Maintainer-email: maiera@de.ibm.com, kathir.velu@in.ibm.com
 License: Apache License, Version 2.0
```

### Comparing `zhmccli-1.6.1/README.rst` & `zhmccli-1.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `zhmccli-1.6.1/requirements.txt` & `zhmccli-1.7.0/requirements.txt`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Make sure that the package versions in minimum-constraints.txt are also
 # the minimum versions required in requirements.txt and dev-requirements.txt.
 
 # Direct dependencies (except pip, setuptools, wheel):
 
 # zhmcclient @ git+https://github.com/zhmcclient/python-zhmcclient.git@master
-zhmcclient>=1.7.0  # Apache
+zhmcclient>=1.8.0  # Apache
 
 # click <7.0 did not properly declare supported Python versions
 # click 8.0 has dropped support for Python 2.7,3.5
 # safety 2.2.0 depends on click>=8.0.2 and is run only on Python>=3.6
 click>=7.0,<8.0; python_version <= '3.5'
 click>=8.0.2; python_version >= '3.6'
 
@@ -40,28 +40,26 @@
 # PyYAML 5.3 fixed narrow build error on Python 2.7
 # PyYAML 5.3.1 addressed issue 38100 reported by safety
 # PyYAML 5.2 addressed issue 38639 reported by safety
 # PyYAML 5.4 fixes safety issue 39611
 PyYAML>=5.3.1; python_version <= '3.5'
 PyYAML>=5.4; python_version >= '3.6'
 
-jsonschema>=2.6.0
+jsonschema>=3.0.1
 yamlloader>=0.5.5
 
-# requests.packages.urllib3 is used to disable warnings
-# Keep this consistent with zhmcclient project
-requests>=2.22.0; python_version <= '3.9'
-requests>=2.25.0; python_version >= '3.10'
+# urllib3 is used to disable warnings
+urllib3>=1.26.5  # MIT
+
 
 # Indirect dependencies (commented out, only listed to document their license):
 
 # certifi # MPL 2.0, from requests
 # chardet # LGPL, from requests
 # decorator # BSD, from zhmcclient
 # docopt # MIT, from stomp.py
 # idna # BSD, from requests
 # python-utils # BSD, from progressbar2
 # pytz # MIT, from zhmcclient
 # requests # Apache, from zhmcclient
 # stomp.py # Apache, from zhmcclient
-# urllib3 # MIT, from requests
 # wcwidth # MIT, from prompt-toolkit
```

### Comparing `zhmccli-1.6.1/setup.py` & `zhmccli-1.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.6.1/zhmccli/__init__.py` & `zhmccli-1.7.0/zhmccli/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 from __future__ import absolute_import
 
 from ._version import *        # noqa: F401
 from ._cmd_info import *       # noqa: F401
 from ._cmd_session import *    # noqa: F401
 from ._cmd_console import *    # noqa: F401
 from ._cmd_cpc import *        # noqa: F401
+from ._cmd_unmanaged_cpc import *  # noqa: F401
+from ._cmd_ldap_server_definition import *  # noqa: F401
 from ._cmd_lpar import *       # noqa: F401
 from ._cmd_partition import *  # noqa: F401
 from ._cmd_adapter import *    # noqa: F401
 from ._cmd_port import *       # noqa: F401
 from ._cmd_hba import *        # noqa: F401
 from ._cmd_nic import *        # noqa: F401
 from ._cmd_vfunction import *  # noqa: F401
@@ -36,7 +38,8 @@
 from ._cmd_storagevolume import *  # noqa: F401
 from ._cmd_vstorageresource import *  # noqa: F401
 from ._cmd_capacitygroup import *  # noqa: F401
 from ._cmd_user import *       # noqa: F401
 from ._cmd_user_role import *  # noqa: F401
 from ._cmd_password_rule import *  # noqa: F401
 from ._cmd_character_rule import *  # noqa: F401
+from ._cmd_certificates import *  # noqa: F401
```

### Comparing `zhmccli-1.6.1/zhmccli/_cmd_adapter.py` & `zhmccli-1.7.0/zhmccli/_cmd_adapter.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,24 +14,52 @@
 
 """
 Commands for adapters.
 """
 
 from __future__ import absolute_import
 
+import time
+import re
+from datetime import datetime
 import click
 
 import zhmcclient
 from .zhmccli import cli
 from ._helper import print_properties, print_resources, abort_if_false, \
     options_to_properties, original_options, COMMAND_OPTIONS_METAVAR, \
     click_exception, add_options, LIST_OPTIONS
 from ._cmd_cpc import find_cpc
 
 
+# Mapping of --crypto-type option values to crypto-type adapter property values
+CRYPTO_TYPE_PROPERTIES = {
+    'acc': 'accelerator',
+    'cca': 'cca-coprocessor',
+    'ep11': 'ep11-coprocessor',
+}
+
+# List of --crypto-type option values
+CRYPTO_TYPE_OPTIONS = sorted(list(CRYPTO_TYPE_PROPERTIES.keys()))
+
+# Default crypto adapter name patterns
+CRYPTO_DEFAULT_NAMES = re.compile(
+    r"^(Accel|CCA|EP11) [0-9A-F]{4} [0-9A-F]{4}-[0-9]{2}$")
+
+# Mapping of --storage-type option values to type adapter property values
+STORAGE_TYPE_PROPERTIES = {
+    'fcp': 'fcp',
+    'fc': 'fc',
+    'not-configured': 'not-configured',
+}
+
+# List of --storage-type option values
+STORAGE_TYPE_OPTIONS = sorted(list(STORAGE_TYPE_PROPERTIES.keys()))
+
+
 def find_adapter(cmd_ctx, client, cpc_or_name, adapter_name):
     """
     Find an adapter by name and return its resource object.
     """
     if isinstance(cpc_or_name, zhmcclient.Cpc):
         cpc = cpc_or_name
     else:
@@ -115,38 +143,49 @@
 @click.option('--port-description', type=str, required=False,
               help='The new description of the single port of the adapter.')
 @click.option('--mtu-size', type=click.Choice(['8', '16', '32', '56']),
               required=False,
               help='The new MTU size of the adapter in KiB. '
               '(HiperSockets only).')
 @click.option('--allowed-capacity', type=int, required=False,
-              help='The maximum number of HBAs per partition. '
-              '(FCP only).')
+              help='The new maximum number of HBAs per partition. '
+              '(only certain adapter types).')
 @click.option('--chpid', type=str, required=False,
-              help='Channel path ID (CHPID, 2 hex chars) used by the '
-              'adapter\'s port. '
-              '(OSA, FICON, HiperSockets only).')
-@click.option('--crypto-number', type=int, required=False,
-              help='Identifier of the crypto adapter in the range 0-15 '
-              'Must be unique within the CPC. '
-              '(Crypto only).')
+              help='The new channel path ID (CHPID, 2 hex chars) used by the '
+              'adapter\'s partition. (OSA, FICON, HiperSockets only; Adapter '
+              'must not be used by any partition).')
 @click.option('--crypto-tke/--no-crypto-tke', default=None, required=False,
-              help='Permit TKE commands on the crypto adapter. '
-              '(Crypto only).')
+              help='The new setting whether TKE commands are permitted on the '
+              'crypto adapter. (Crypto only).')
+@click.option('--crypto-type', default=None, required=False,
+              type=click.Choice(CRYPTO_TYPE_OPTIONS),
+              help='The new crypto type (Crypto only; Adapter must be '
+              'offline).')
+@click.option('--storage-type', default=None, required=False,
+              type=click.Choice(STORAGE_TYPE_OPTIONS),
+              help='The new ficon type (FICON only; Adapter must be '
+              'offline).')
+@click.option('--dont-zeroize', is_flag=True, default=False, required=False,
+              help='Do not zeroize when changing crypto type to '
+              'accelerator. (Crypto only; Default is to zeroize).')
 @click.pass_obj
 def adapter_update(cmd_ctx, cpc, adapter, **options):
     """
     Update the properties of an adapter.
 
     Only the properties will be changed for which a corresponding option is
     specified, so the default for all options is not to change properties.
 
     The adapter may be a physical adapter (e.g. a discovered OSA card) or a
     logical adapter (e.g. HiperSockets).
 
+    For Crypto Express adapters, the crypto type can be changed.
+
+    For FICON Express adapters, the ficon type can be changed.
+
     In addition to the command-specific options shown in this help text, the
     general options (see 'zhmc --help') can also be specified right after the
     'zhmc' command name.
     """
     cmd_ctx.execute_cmd(lambda: cmd_adapter_update(cmd_ctx, cpc, adapter,
                                                    options))
 
@@ -326,38 +365,100 @@
 
 
 def cmd_adapter_update(cmd_ctx, cpc_name, adapter_name, options):
     # pylint: disable=missing-function-docstring
 
     client = zhmcclient.Client(cmd_ctx.session)
     adapter = find_adapter(cmd_ctx, client, cpc_name, adapter_name)
+    new_name = None  # New name if adapter name has changed
 
     name_map = {
         'mtu-size': 'maximum-transmission-unit-size',
         'chpid': 'channel-path-id',
         'crypto-tke': 'tke-commands-enabled',
+        'crypto-type': None,
+        'dont-zeroize': None,
+        'storage-type': None,
     }
     org_options = original_options(options)
     properties = options_to_properties(org_options, name_map)
+    crypto_type_option = options['crypto_type']
+    storage_type_option = options['storage_type']
 
-    if not properties:
+    if not properties and not crypto_type_option and not storage_type_option:
         cmd_ctx.spinner.stop()
-        click.echo("No properties specified for updating adapter '{a}'.".
+        click.echo("No changes specified for updating adapter '{a}'.".
                    format(a=adapter_name))
         return
 
+    if 'name' in properties and properties['name'] != adapter_name:
+        new_name = properties['name']
     try:
         adapter.update_properties(properties)
     except zhmcclient.Error as exc:
         raise click_exception(exc, cmd_ctx.error_format)
 
+    if crypto_type_option:
+        crypto_type_prop = CRYPTO_TYPE_PROPERTIES[crypto_type_option]
+        if crypto_type_option == 'acc':
+            zeroize = not options['dont_zeroize']
+        else:
+            if options['dont_zeroize']:
+                cmd_ctx.spinner.stop()
+                click.echo("Ignoring --dont-zeroize option for adapter '{a}'.".
+                           format(a=adapter_name))
+            zeroize = None
+        try:
+            adapter.change_crypto_type(crypto_type_prop, zeroize)
+        except zhmcclient.Error as exc:
+            raise click_exception(exc, cmd_ctx.error_format)
+
+        # Changing the crypto type triggers a change of the adapter name,
+        # if the current name is the default name (e.g. 'CCA 0104 A14B-03')
+        # The new name will be visible at the API only after about 2 seconds.
+        if CRYPTO_DEFAULT_NAMES.match(adapter.name):
+
+            # This debug code can be used to test whether the behavior of
+            # changing the adapter name has changed.
+            DEBUG_CRYPTO_NAME_CHANGE = False
+
+            if DEBUG_CRYPTO_NAME_CHANGE:
+                t1 = datetime.now()
+                cmd_ctx.spinner.stop()
+                for _ in range(0, 20):
+                    adapter.pull_full_properties()
+                    dt = datetime.now() - t1
+                    print("Debug: Adapter name after {}: {!r}".
+                          format(dt, adapter.name))
+            else:
+                time.sleep(4)
+                adapter.pull_full_properties()
+
+            if adapter.name != adapter_name:
+                new_name = adapter.name
+
+    if storage_type_option:
+        storage_type_prop = STORAGE_TYPE_PROPERTIES[storage_type_option]
+        try:
+            adapter.change_adapter_type(storage_type_prop)
+        except zhmcclient.Error as exc:
+            raise click_exception(exc, cmd_ctx.error_format)
+        sibling_adapters = adapter.list_sibling_adapters()
+        sibling_adapter_names = ', '.join(
+            ["'{}'".format(a.name) for a in sibling_adapters])
+        cmd_ctx.spinner.stop()
+        click.echo("FICON adapter {a} and its sibling adapter {s} have "
+                   "been changed to type '{t}'.".
+                   format(a=adapter.name, s=sibling_adapter_names,
+                          t=storage_type_option))
+
     cmd_ctx.spinner.stop()
-    if 'name' in properties and properties['name'] != adapter_name:
-        click.echo("Adapter '{a}' has been renamed to '{an}' and was updated.".
-                   format(a=adapter_name, an=properties['name']))
+    if new_name:
+        click.echo("Adapter '{a}' has been renamed to '{n}' and was updated.".
+                   format(a=adapter_name, n=new_name))
     else:
         click.echo("Adapter '{a}' has been updated.".format(a=adapter_name))
 
 
 def cmd_adapter_create_hipersocket(cmd_ctx, cpc_name, options):
     # pylint: disable=missing-function-docstring
```

### Comparing `zhmccli-1.6.1/zhmccli/_cmd_capacitygroup.py` & `zhmccli-1.7.0/zhmccli/_cmd_capacitygroup.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.6.1/zhmccli/_cmd_character_rule.py` & `zhmccli-1.7.0/zhmccli/_cmd_character_rule.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.6.1/zhmccli/_cmd_console.py` & `zhmccli-1.7.0/zhmccli/_cmd_console.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from __future__ import absolute_import
 
 import click
 import dateutil.parser
 
 import zhmcclient
 from .zhmccli import cli
-from ._helper import print_properties, print_dicts, \
+from ._helper import print_properties, print_dicts, print_list, \
     TABLE_FORMATS, hide_property, COMMAND_OPTIONS_METAVAR, click_exception
 
 
 @cli.group('console', options_metavar=COMMAND_OPTIONS_METAVAR)
 def console_group():
     """
     Command group for the HMC console.
@@ -97,14 +97,34 @@
     In addition to the command-specific options shown in this help text, the
     general options (see 'zhmc --help') can also be specified right after the
     'zhmc' command name.
     """
     cmd_ctx.execute_cmd(lambda: cmd_get_security_log(cmd_ctx, options))
 
 
+@console_group.command('list-api-features',
+                       options_metavar=COMMAND_OPTIONS_METAVAR)
+@click.option('--name', type=str, metavar='NAME',
+              required=False,
+              help='A regular expression used to limit returned objects to '
+                   'those that have a matching name field.')
+@click.pass_obj
+def list_api_features(cmd_ctx, **options):
+    """
+    Lists the Web Services API features available of the console of the
+    targeted HMC.
+
+    In addition to the command-specific options shown in this help text, the
+    general options (see 'zhmc --help') can also be specified right after the
+    'zhmc' command name.
+    """
+    cmd_ctx.execute_cmd(
+        lambda: cmd_list_api_features(cmd_ctx, options))
+
+
 def cmd_console_show(cmd_ctx, options):
     # pylint: disable=missing-function-docstring
 
     client = zhmcclient.Client(cmd_ctx.session)
     console = client.consoles.console
 
     try:
@@ -196,7 +216,22 @@
     additions = {
         'timestamp': ts_additions,
     }
 
     cmd_ctx.spinner.stop()
     print_dicts(cmd_ctx, log_items, cmd_ctx.output_format,
                 show_list=show_list, additions=additions, all=False)
+
+
+def cmd_list_api_features(cmd_ctx, options):
+    # pylint: disable=missing-function-docstring
+
+    client = zhmcclient.Client(cmd_ctx.session)
+    console = client.consoles.console
+
+    name = options['name']
+    try:
+        features = console.list_api_features(name)
+    except zhmcclient.Error as exc:
+        raise click_exception(exc, cmd_ctx.error_format)
+
+    print_list(cmd_ctx, features, cmd_ctx.output_format)
```

### Comparing `zhmccli-1.6.1/zhmccli/_cmd_cpc.py` & `zhmccli-1.7.0/zhmccli/_cmd_cpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 import yaml
 import yamlloader
 import click
 from tabulate import tabulate
 
 import zhmcclient
 from .zhmccli import cli
-from ._helper import print_properties, print_resources, \
+from ._helper import print_properties, print_resources, print_list, \
     options_to_properties, original_options, COMMAND_OPTIONS_METAVAR, \
     click_exception, add_options, LIST_OPTIONS, TABLE_FORMATS, hide_property, \
     required_option, abort_if_false, validate, print_dicts
 
 
 POWER_SAVING_TYPES = ['high-performance', 'low-power', 'custom']
 DEFAULT_POWER_SAVING_TYPE = 'high-performance'
@@ -499,14 +499,33 @@
     general options (see 'zhmc --help') can also be specified right after the
     'zhmc' command name.
     """
     cmd_ctx.execute_cmd(
         lambda: cmd_cpc_autostart_clear(cmd_ctx, cpc))
 
 
+@cpc_group.command('list-api-features', options_metavar=COMMAND_OPTIONS_METAVAR)
+@click.argument('CPC', type=str, metavar='CPC')
+@click.option('--name', type=str, metavar='NAME',
+              required=False,
+              help='A regular expression used to limit returned objects to '
+                   'those that have a matching name field.')
+@click.pass_obj
+def cpc_list_api_features(cmd_ctx, cpc, **options):
+    """
+    Lists the Web Services API features available on a CPC.
+
+    In addition to the command-specific options shown in this help text, the
+    general options (see 'zhmc --help') can also be specified right after the
+    'zhmc' command name.
+    """
+    cmd_ctx.execute_cmd(
+        lambda: cmd_cpc_list_api_features(cmd_ctx, cpc, options))
+
+
 def cmd_cpc_list(cmd_ctx, options):
     # pylint: disable=missing-function-docstring
 
     client = zhmcclient.Client(cmd_ctx.session)
 
     try:
         cpcs = client.cpcs.list()
@@ -981,7 +1000,22 @@
         cpc.set_auto_start_list(as_list)
     except zhmcclient.Error as exc:
         raise click_exception(exc, cmd_ctx.error_format)
 
     cmd_ctx.spinner.stop()
     click.echo("Auto-start list for CPC '{c}' has been cleared.".
                format(c=cpc_name))
+
+
+def cmd_cpc_list_api_features(cmd_ctx, cpc_name, options):
+    # pylint: disable=missing-function-docstring
+
+    client = zhmcclient.Client(cmd_ctx.session)
+    cpc = find_cpc(cmd_ctx, client, cpc_name)
+
+    name = options['name']
+    try:
+        features = cpc.list_api_features(name)
+    except zhmcclient.Error as exc:
+        raise click_exception(exc, cmd_ctx.error_format)
+
+    print_list(cmd_ctx, features, cmd_ctx.output_format)
```

### Comparing `zhmccli-1.6.1/zhmccli/_cmd_hba.py` & `zhmccli-1.7.0/zhmccli/_cmd_hba.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.6.1/zhmccli/_cmd_info.py` & `zhmccli-1.7.0/zhmccli/_cmd_info.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.6.1/zhmccli/_cmd_lpar.py` & `zhmccli-1.7.0/zhmccli/_cmd_lpar.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 import zhmcclient
 from .zhmccli import cli, CONSOLE_LOGGER_NAME
 from ._helper import print_properties, print_resources, abort_if_false, \
     options_to_properties, original_options, COMMAND_OPTIONS_METAVAR, \
     part_console, click_exception, add_options, LIST_OPTIONS, TABLE_FORMATS, \
     hide_property, ASYNC_TIMEOUT_OPTIONS, API_VERSION_HMC_2_14_0
 from ._cmd_cpc import find_cpc
+from ._cmd_certificates import find_certificate
 
 
 def find_lpar(cmd_ctx, client, cpc_or_name, lpar_name):
     """
     Find an LPAR by name and return its resource object.
     """
     if isinstance(cpc_or_name, zhmcclient.Cpc):
@@ -180,15 +181,15 @@
     general options (see 'zhmc --help') can also be specified right after the
     'zhmc' command name.
 
     \b
     Limitations:
       * The processor capping/sharing/weight related properties cannot be
         updated.
-      * The network-related properties for zaware and ssc cannot beupdated.
+      * The network-related properties for zaware and ssc cannot be updated.
       * The --zaware-master-password and --ssc-master-password options do not
         ask for the password.
     """
     cmd_ctx.execute_cmd(lambda: cmd_lpar_update(cmd_ctx, cpc, lpar, options))
 
 
 @lpar_group.command('activate', options_metavar=COMMAND_OPTIONS_METAVAR)
@@ -481,14 +482,53 @@
     'zhmc' command name.
     """
     cmd_ctx.execute_cmd(lambda: cmd_lpar_scsi_dump(cmd_ctx, cpc, lpar,
                                                    load_address, wwpn, lun,
                                                    options))
 
 
+@lpar_group.command('assign-certificate',
+                    options_metavar=COMMAND_OPTIONS_METAVAR)
+@click.argument('CPC', type=str, metavar='CPC')
+@click.argument('LPAR', type=str, metavar='LPAR')
+@click.option('--certificate', type=str, required=True,
+              help='The name of the certificate.')
+@click.pass_obj
+def lpar_assign_certificate(cmd_ctx, cpc, lpar, **options):
+    """
+    Assign a certificate to an LPAR.
+
+    In addition to the command-specific options shown in this help text, the
+    general options (see 'zhmc --help') can also be specified right after the
+    'zhmc' command name.
+    """
+    cmd_ctx.execute_cmd(
+        lambda: cmd_lpar_assign_certificate(cmd_ctx, cpc, lpar, options))
+
+
+@lpar_group.command('unassign-certificate',
+                    options_metavar=COMMAND_OPTIONS_METAVAR)
+@click.argument('CPC', type=str, metavar='CPC')
+@click.argument('LPAR', type=str, metavar='LPAR')
+@click.option('--certificate', type=str, required=True,
+              help='The name of the certificate.')
+@click.pass_obj
+def lpar_unassign_certificate(cmd_ctx, cpc, lpar, **options):
+    """
+    Unassign a certificate from an LPAR.
+
+    In addition to the command-specific options shown in this help text, the
+    general options (see 'zhmc --help') can also be specified right after the
+    'zhmc' command name.
+    """
+    cmd_ctx.execute_cmd(
+        lambda: cmd_lpar_unassign_certificate(cmd_ctx, cpc, lpar,
+                                              options))
+
+
 def cmd_lpar_list(cmd_ctx, cpc_name, options):
     # pylint: disable=missing-function-docstring
 
     client = zhmcclient.Client(cmd_ctx.session)
 
     if client.version_info() >= API_VERSION_HMC_2_14_0:
         # This approach is faster than going through the CPC.
@@ -518,16 +558,15 @@
     if options['type']:
         click.echo("The --type option is deprecated and type information "
                    "is now always shown.")
 
     # Prepare the additions dict of dicts. It contains additional
     # (=non-resource) property values by property name and by resource URI.
     # Depending on options, some of them will not be populated.
-    additions = {}
-    additions['cpc'] = {}
+    additions = {'cpc': {}}
 
     show_list = [
         'name',
         'cpc',
     ]
     if not options['names_only']:
         show_list.extend([
@@ -775,7 +814,45 @@
         lpar.scsi_dump(load_address, wwpn, lun, wait_for_completion=True,
                        **options)
     except zhmcclient.Error as exc:
         raise click_exception(exc, cmd_ctx.error_format)
 
     cmd_ctx.spinner.stop()
     click.echo("SCSI Dump of LPAR '{p}' is complete.".format(p=lpar_name))
+
+
+def cmd_lpar_assign_certificate(cmd_ctx, cpc_name, lpar_name, options):
+    # pylint: disable=missing-function-docstring
+
+    client = zhmcclient.Client(cmd_ctx.session)
+    lpar = find_lpar(cmd_ctx, client, cpc_name, lpar_name)
+
+    cert_name = options['certificate']
+    cert = find_certificate(cmd_ctx, client, cert_name)
+
+    try:
+        lpar.assign_certificate(cert)
+    except zhmcclient.Error as exc:
+        raise click_exception(exc, cmd_ctx.error_format)
+
+    cmd_ctx.spinner.stop()
+    click.echo("Certificate '{cert}' was assigned to LPAR '{p}'.".
+               format(cert=cert_name, p=lpar_name))
+
+
+def cmd_lpar_unassign_certificate(cmd_ctx, cpc_name, lpar_name, options):
+    # pylint: disable=missing-function-docstring
+
+    client = zhmcclient.Client(cmd_ctx.session)
+    lpar = find_lpar(cmd_ctx, client, cpc_name, lpar_name)
+
+    cert_name = options['certificate']
+    cert = find_certificate(cmd_ctx, client, cert_name)
+
+    try:
+        lpar.unassign_certificate(cert)
+    except zhmcclient.Error as exc:
+        raise click_exception(exc, cmd_ctx.error_format)
+
+    cmd_ctx.spinner.stop()
+    click.echo("Certificate '{cert}' was unassigned from LPAR '{p}'.".
+               format(cert=cert_name, p=lpar_name))
```

### Comparing `zhmccli-1.6.1/zhmccli/_cmd_metrics.py` & `zhmccli-1.7.0/zhmccli/_cmd_metrics.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.6.1/zhmccli/_cmd_nic.py` & `zhmccli-1.7.0/zhmccli/_cmd_nic.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.6.1/zhmccli/_cmd_partition.py` & `zhmccli-1.7.0/zhmccli/_cmd_partition.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 from ._helper import print_properties, print_resources, abort_if_false, \
     options_to_properties, original_options, COMMAND_OPTIONS_METAVAR, \
     part_console, click_exception, storage_management_feature, \
     add_options, LIST_OPTIONS, TABLE_FORMATS, hide_property, \
     ASYNC_TIMEOUT_OPTIONS, API_VERSION_HMC_2_14_0
 from ._cmd_cpc import find_cpc
 from ._cmd_storagegroup import find_storagegroup
+from ._cmd_certificates import find_certificate
 from ._cmd_metrics import get_metric_values
 
 
 # Defaults for partition creation
 DEFAULT_IFL_PROCESSORS = 1
 DEFAULT_INITIAL_MEMORY_MB = 1024
 DEFAULT_MAXIMUM_MEMORY_MB = 1024
@@ -691,14 +692,54 @@
     'zhmc' command name.
     """
     cmd_ctx.execute_cmd(
         lambda: cmd_partition_detach_storagegroup(cmd_ctx, cpc, partition,
                                                   options))
 
 
+@partition_group.command('assign-certificate',
+                         options_metavar=COMMAND_OPTIONS_METAVAR)
+@click.argument('CPC', type=str, metavar='CPC')
+@click.argument('PARTITION', type=str, metavar='PARTITION')
+@click.option('--certificate', type=str, required=True,
+              help='The name of the certificate.')
+@click.pass_obj
+def partition_assign_certificate(cmd_ctx, cpc, partition, **options):
+    """
+    Assign a certificate to a partition.
+
+    In addition to the command-specific options shown in this help text, the
+    general options (see 'zhmc --help') can also be specified right after the
+    'zhmc' command name.
+    """
+    cmd_ctx.execute_cmd(
+        lambda: cmd_partition_assign_certificate(cmd_ctx, cpc, partition,
+                                                 options))
+
+
+@partition_group.command('unassign-certificate',
+                         options_metavar=COMMAND_OPTIONS_METAVAR)
+@click.argument('CPC', type=str, metavar='CPC')
+@click.argument('PARTITION', type=str, metavar='PARTITION')
+@click.option('--certificate', type=str, required=True,
+              help='The name of the certificate.')
+@click.pass_obj
+def partition_unassign_certificate(cmd_ctx, cpc, partition, **options):
+    """
+    Unassign a certificate from a partition.
+
+    In addition to the command-specific options shown in this help text, the
+    general options (see 'zhmc --help') can also be specified right after the
+    'zhmc' command name.
+    """
+    cmd_ctx.execute_cmd(
+        lambda: cmd_partition_unassign_certificate(cmd_ctx, cpc, partition,
+                                                   options))
+
+
 def cmd_partition_list(cmd_ctx, cpc_name, options):
     # pylint: disable=missing-function-docstring
 
     if options['help_usage']:
         help_lines = """
 Help for usage related options of the partition list command:
 
@@ -1550,14 +1591,54 @@
         raise click_exception(exc, cmd_ctx.error_format)
 
     cmd_ctx.spinner.stop()
     click.echo("Storage group '{sg}' was detached from partition '{p}'.".
                format(sg=stogrp_name, p=partition.name))
 
 
+def cmd_partition_assign_certificate(
+        cmd_ctx, cpc_name, partition_name, options):
+    # pylint: disable=missing-function-docstring
+
+    client = zhmcclient.Client(cmd_ctx.session)
+    partition = find_partition(cmd_ctx, client, cpc_name, partition_name)
+
+    cert_name = options['certificate']
+    cert = find_certificate(cmd_ctx, client, cert_name)
+
+    try:
+        partition.assign_certificate(cert)
+    except zhmcclient.Error as exc:
+        raise click_exception(exc, cmd_ctx.error_format)
+
+    cmd_ctx.spinner.stop()
+    click.echo("Certificate '{cert}' was assigned to partition '{p}'.".
+               format(cert=cert_name, p=partition.name))
+
+
+def cmd_partition_unassign_certificate(
+        cmd_ctx, cpc_name, partition_name, options):
+    # pylint: disable=missing-function-docstring
+
+    client = zhmcclient.Client(cmd_ctx.session)
+    partition = find_partition(cmd_ctx, client, cpc_name, partition_name)
+
+    cert_name = options['certificate']
+    cert = find_certificate(cmd_ctx, client, cert_name)
+
+    try:
+        partition.unassign_certificate(cert)
+    except zhmcclient.Error as exc:
+        raise click_exception(exc, cmd_ctx.error_format)
+
+    cmd_ctx.spinner.stop()
+    click.echo("Certificate '{cert}' was unassigned from partition '{p}'.".
+               format(cert=cert_name, p=partition.name))
+
+
 # pylint: disable=inconsistent-return-statements
 def parse_volume_with_sm(volume_specifier, partition, where, error_format):
     """
     Parse a volume specifier for a CPC with the storage management feature
     (i.e. z14 or later) and return its StorageVolume resource object.
 
     The partition that has the storage group of the volume attached, must be
```

### Comparing `zhmccli-1.6.1/zhmccli/_cmd_password_rule.py` & `zhmccli-1.7.0/zhmccli/_cmd_password_rule.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.6.1/zhmccli/_cmd_port.py` & `zhmccli-1.7.0/zhmccli/_cmd_port.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.6.1/zhmccli/_cmd_session.py` & `zhmccli-1.7.0/zhmccli/_cmd_session.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.6.1/zhmccli/_cmd_storagegroup.py` & `zhmccli-1.7.0/zhmccli/_cmd_storagegroup.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.6.1/zhmccli/_cmd_storagevolume.py` & `zhmccli-1.7.0/zhmccli/_cmd_storagevolume.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.6.1/zhmccli/_cmd_user.py` & `zhmccli-1.7.0/zhmccli/_cmd_user.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.6.1/zhmccli/_cmd_user_role.py` & `zhmccli-1.7.0/zhmccli/_cmd_user_role.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.6.1/zhmccli/_cmd_vfunction.py` & `zhmccli-1.7.0/zhmccli/_cmd_vfunction.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.6.1/zhmccli/_cmd_vstorageresource.py` & `zhmccli-1.7.0/zhmccli/_cmd_vstorageresource.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.6.1/zhmccli/_cmd_vswitch.py` & `zhmccli-1.7.0/zhmccli/_cmd_vswitch.py`

 * *Files identical despite different names*

### Comparing `zhmccli-1.6.1/zhmccli/_helper.py` & `zhmccli-1.7.0/zhmccli/_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -220,28 +220,29 @@
     A context object we attach to the :class:`click.Context` object in its
     ``obj`` attribute. It is used to provide command line options and other
     data.
     """
 
     def __init__(self, host, userid, password, no_verify, ca_certs,
                  output_format, transpose, error_format, timestats, session_id,
-                 get_password):
+                 get_password, pdb):
         self._host = host
         self._userid = userid
         self._password = password
         self._no_verify = no_verify
         self._ca_certs = ca_certs
         self._output_format = output_format
         self._transpose = transpose
         self._error_format = error_format
         self._timestats = timestats
         self._session_id = session_id
         self._get_password = get_password
         self._session = None
         self._spinner = click_spinner.Spinner()
+        self._pdb = pdb
 
     def __repr__(self):
         ret = "CmdContext(at 0x{ctx:08x}, host={s._host!r}, " \
             "userid={s._userid!r}, password={pw!r}, " \
             "no_verify={s._no_verify!r}, ca_certs={s._ca_certs!r}, " \
             "output_format={s._output_format!r}, transpose={s._transpose!r}, " \
             "error_format={s._error_format!r}, timestats={s._timestats!r}," \
@@ -341,14 +342,21 @@
 
         Since click_spinner 0.1.5, the Spinner object takes care of suppressing
         the spinner when not on a tty, and is able to suspend/resume the
         spinner via its stop() and start() methods.
         """
         return self._spinner
 
+    @property
+    def pdb(self):
+        """
+        bool: Indicates whether to break in the debugger.
+        """
+        return self._pdb
+
     def execute_cmd(self, cmd):
         """
         Execute the command.
         """
         if self._session is None:
             if isinstance(self._session_id, zhmcclient_mock.FakedSession):
                 self._session = self._session_id
@@ -365,21 +373,30 @@
                 self._session = zhmcclient.Session(
                     self._host, self._userid, self._password,
                     session_id=self._session_id,
                     get_password=self._get_password,
                     verify_cert=verify_cert)
         if self.timestats:
             self._session.time_stats_keeper.enable()
-        self.spinner.start()
+        if not self.pdb:
+            self.spinner.start()
+
         try:
-            cmd()
+            if self.pdb:
+                import pdb  # pylint: disable=import-outside-toplevel
+                pdb.set_trace()  # pylint: disable=forgotten-debug-statement
+
+            cmd()  # The zhmc command function call.
+
         except zhmcclient.Error as exc:
             raise click_exception(exc, self.error_format)
+
         finally:
-            self.spinner.stop()
+            if not self.pdb:
+                self.spinner.stop()
             if self._session.time_stats_keeper.enabled:
                 click.echo(self._session.time_stats_keeper)
 
 
 def original_options(options):
     """
     Return the input options with their original names.
@@ -444,14 +461,43 @@
         if name_map:
             name = name_map.get(name, name)
         if name is not None:
             properties[name] = value
     return properties
 
 
+def print_list(cmd_ctx, values, output_format):
+    """
+    Print a list of values in the desired output format.
+
+    The spinner is stopped just before printing.
+
+    Parameters:
+
+      cmd_ctx (CmdContext): Context object of the command.
+
+      values (list): The list of values.
+
+      output_format (string): Output format from the command line.
+    """
+    output = ""
+    if output_format in TABLE_FORMATS:
+        if output_format == 'table':
+            output_format = 'psql'
+        data = [[v] for v in values]
+        output = tabulate(data, [], tablefmt=output_format)
+    elif output_format == 'json':
+        output = json.dumps(values)
+    else:
+        raise InvalidOutputFormatError(output_format)
+
+    cmd_ctx.spinner.stop()
+    click.echo(output)
+
+
 def print_properties(cmd_ctx, properties, output_format, show_list=None):
     """
     Print properties in the desired output format.
 
     The spinner is stopped just before printing.
 
     Parameters:
```

### Comparing `zhmccli-1.6.1/zhmccli/_version.py` & `zhmccli-1.7.0/zhmccli/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,8 +21,8 @@
 #: The full version of this package including any development levels, as a
 #: :term:`string`.
 #:
 #: Possible formats for this version string are:
 #:
 #: * "M.N.U.dev1": A not yet released version M.N.U
 #: * "M.N.U": A released version M.N.U
-__version__ = '1.6.1'
+__version__ = '1.7.0'
```

### Comparing `zhmccli-1.6.1/zhmccli/zhmccli.py` & `zhmccli-1.7.0/zhmccli/zhmccli.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 import sys
 import logging
 from logging.handlers import SysLogHandler
 from logging import StreamHandler, NullHandler
 import platform
-from requests.packages import urllib3
+import urllib3
 import click
 import click_repl
 from prompt_toolkit.history import FileHistory
 
 import zhmcclient
 import zhmcclient_mock
 from ._helper import CmdContext, GENERAL_OPTIONS_METAVAR, REPL_HISTORY_FILE, \
@@ -130,21 +130,25 @@
 @click.option('--log-dest', type=click.Choice(LOG_DESTINATIONS),
               help="Log destination for this command (Default: {def_dest}).".
               format(def_dest=DEFAULT_LOG_DESTINATION))
 @click.option('--syslog-facility', type=click.Choice(SYSLOG_FACILITIES),
               help="Syslog facility when logging to the syslog "
               "(Default: {def_slf}).".
               format(def_slf=DEFAULT_SYSLOG_FACILITY))
+@click.option('--pdb', is_flag=True, hidden=True,
+              help=u'Break execution in the pdb debugger just before '
+                   u'executing the command within zhmc.')
 @click.version_option(
     message='%(prog)s, version %(version)s\n' + ZHMCCLIENT_VERSION,
     help="Show the versions of this command and of the zhmcclient package and "
     "exit.")
 @click.pass_context
 def cli(ctx, host, userid, password, no_verify, ca_certs, output_format,
-        transpose, error_format, timestats, log, log_dest, syslog_facility):
+        transpose, error_format, timestats, log, log_dest, syslog_facility,
+        pdb):
     """
     Command line interface for the IBM Z HMC.
 
     The options shown in this help text are general options that can also
     be specified on any of the (sub-)commands.
     """
 
@@ -187,14 +191,16 @@
             output_format = ctx.obj.output_format
         if transpose is None:
             transpose = ctx.obj.transpose
         if error_format is None:
             error_format = ctx.obj.error_format
         if timestats is None:
             timestats = ctx.obj.timestats
+        if pdb is None:
+            pdb = ctx.obj.pdb
 
     if transpose and output_format == 'json':
         raise click_exception(
             "Transposing output tables (-x / --transpose) conflicts with "
             "non-table output format (-o / --output-format): {of}".
             format(of=output_format),
             error_format)
@@ -324,15 +330,15 @@
                               error_format)
 
     # We create a command context for each command: An interactive command has
     # its own command context different from the command context for the
     # command line.
     ctx.obj = CmdContext(host, userid, password, no_verify, ca_certs,
                          output_format, transpose, error_format, timestats,
-                         session_id, get_password_via_prompt)
+                         session_id, get_password_via_prompt, pdb)
 
     # Invoke default command
     if ctx.invoked_subcommand is None:
         ctx.invoke(repl)
 
 
 def reset_logger(log_comp):
```

### Comparing `zhmccli-1.6.1/zhmccli.egg-info/PKG-INFO` & `zhmccli-1.7.0/zhmccli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhmccli
-Version: 1.6.1
+Version: 1.7.0
 Summary: A CLI for the IBM Z HMC, written in pure Python
 Home-page: https://github.com/zhmcclient/zhmccli
 Author: Juergen Leopold, Andreas Maier
 Author-email: leopoldj@de.ibm.com, maiera@de.ibm.com
 Maintainer: Andreas Maier, Kathir Velusamy
 Maintainer-email: maiera@de.ibm.com, kathir.velu@in.ibm.com
 License: Apache License, Version 2.0
```

### Comparing `zhmccli-1.6.1/zhmccli.egg-info/SOURCES.txt` & `zhmccli-1.7.0/zhmccli.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -2,28 +2,31 @@
 MANIFEST.in
 README.rst
 requirements.txt
 setup.py
 zhmccli/__init__.py
 zhmccli/_cmd_adapter.py
 zhmccli/_cmd_capacitygroup.py
+zhmccli/_cmd_certificates.py
 zhmccli/_cmd_character_rule.py
 zhmccli/_cmd_console.py
 zhmccli/_cmd_cpc.py
 zhmccli/_cmd_hba.py
 zhmccli/_cmd_info.py
+zhmccli/_cmd_ldap_server_definition.py
 zhmccli/_cmd_lpar.py
 zhmccli/_cmd_metrics.py
 zhmccli/_cmd_nic.py
 zhmccli/_cmd_partition.py
 zhmccli/_cmd_password_rule.py
 zhmccli/_cmd_port.py
 zhmccli/_cmd_session.py
 zhmccli/_cmd_storagegroup.py
 zhmccli/_cmd_storagevolume.py
+zhmccli/_cmd_unmanaged_cpc.py
 zhmccli/_cmd_user.py
 zhmccli/_cmd_user_role.py
 zhmccli/_cmd_vfunction.py
 zhmccli/_cmd_vstorageresource.py
 zhmccli/_cmd_vswitch.py
 zhmccli/_helper.py
 zhmccli/_version.py
```

