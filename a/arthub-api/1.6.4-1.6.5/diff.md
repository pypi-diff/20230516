# Comparing `tmp/arthub_api-1.6.4.tar.gz` & `tmp/arthub_api-1.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arthub_api-1.6.4.tar", last modified: Tue May 16 03:20:44 2023, max compression
+gzip compressed data, was "arthub_api-1.6.5.tar", last modified: Tue May 16 10:41:07 2023, max compression
```

## Comparing `arthub_api-1.6.4.tar` & `arthub_api-1.6.5.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 03:20:44.060739 arthub_api-1.6.4/
--rw-rw-rw-   0        0        0     1077 2022-09-05 10:15:53.000000 arthub_api-1.6.4/LICENSE
--rw-rw-rw-   0        0        0      107 2022-09-05 10:15:53.000000 arthub_api-1.6.4/MANIFEST.in
--rw-rw-rw-   0        0        0     1412 2023-05-16 03:20:44.060739 arthub_api-1.6.4/PKG-INFO
--rw-rw-rw-   0        0        0      864 2023-05-11 09:00:18.000000 arthub_api-1.6.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-16 03:20:44.041249 arthub_api-1.6.4/arthub_api/
--rw-rw-rw-   0        0        0      666 2023-05-15 09:23:22.000000 arthub_api-1.6.4/arthub_api/__init__.py
--rw-rw-rw-   0        0        0     2316 2023-05-12 03:05:16.000000 arthub_api-1.6.4/arthub_api/__main__.py
--rw-rw-rw-   0        0        0      241 2023-05-16 03:20:38.000000 arthub_api-1.6.4/arthub_api/__version__.py
--rw-rw-rw-   0        0        0    13661 2023-05-11 11:13:51.000000 arthub_api-1.6.4/arthub_api/_internal_utils.py
--rw-rw-rw-   0        0        0       84 2023-05-12 03:05:16.000000 arthub_api-1.6.4/arthub_api/arthub_api_config.py
--rw-rw-rw-   0        0        0      517 2023-03-14 10:44:30.000000 arthub_api-1.6.4/arthub_api/asset_matrix.py
--rw-rw-rw-   0        0        0    38061 2023-05-16 03:19:15.000000 arthub_api-1.6.4/arthub_api/blade_api.py
--rw-rw-rw-   0        0        0     1032 2023-05-15 09:23:22.000000 arthub_api-1.6.4/arthub_api/blade_api_instance.py
--rw-rw-rw-   0        0        0    22945 2023-05-11 11:42:27.000000 arthub_api-1.6.4/arthub_api/blade_storage.py
--rw-rw-rw-   0        0        0       22 2023-02-08 16:32:42.000000 arthub_api-1.6.4/arthub_api/cli.py
--rw-rw-rw-   0        0        0     1365 2023-02-08 16:32:42.000000 arthub_api-1.6.4/arthub_api/config.py
--rw-rw-rw-   0        0        0      523 2023-02-08 16:32:42.000000 arthub_api-1.6.4/arthub_api/exception.py
--rw-rw-rw-   0        0        0     1258 2023-03-14 10:50:34.000000 arthub_api-1.6.4/arthub_api/models.py
--rw-rw-rw-   0        0        0    41857 2023-05-15 09:23:22.000000 arthub_api-1.6.4/arthub_api/open_api.py
--rw-rw-rw-   0        0        0    41828 2023-03-14 11:53:38.000000 arthub_api-1.6.4/arthub_api/storage.py
--rw-rw-rw-   0        0        0     8941 2023-05-12 03:05:16.000000 arthub_api-1.6.4/arthub_api/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-16 03:20:44.050224 arthub_api-1.6.4/arthub_api.egg-info/
--rw-rw-rw-   0        0        0     1412 2023-05-16 03:20:43.000000 arthub_api-1.6.4/arthub_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      847 2023-05-16 03:20:43.000000 arthub_api-1.6.4/arthub_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 03:20:43.000000 arthub_api-1.6.4/arthub_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-16 03:20:43.000000 arthub_api-1.6.4/arthub_api.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-02-09 14:04:12.000000 arthub_api-1.6.4/arthub_api.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       65 2023-05-16 03:20:43.000000 arthub_api-1.6.4/arthub_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-16 03:20:43.000000 arthub_api-1.6.4/arthub_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       63 2022-09-26 03:28:18.000000 arthub_api-1.6.4/requirements-dev.txt
--rw-rw-rw-   0        0        0       42 2023-05-16 03:20:44.060739 arthub_api-1.6.4/setup.cfg
--rw-rw-rw-   0        0        0     2908 2023-05-11 11:42:27.000000 arthub_api-1.6.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-16 03:20:44.059229 arthub_api-1.6.4/tests/
--rw-rw-rw-   0        0        0      139 2023-05-12 03:05:16.000000 arthub_api-1.6.4/tests/__init__.py
--rw-rw-rw-   0        0        0      108 2023-05-12 03:05:16.000000 arthub_api-1.6.4/tests/_utils.py
--rw-rw-rw-   0        0        0      267 2023-05-11 09:00:19.000000 arthub_api-1.6.4/tests/conftest.py
--rw-rw-rw-   0        0        0     5924 2023-05-11 09:00:19.000000 arthub_api-1.6.4/tests/test_open_api.py
--rw-rw-rw-   0        0        0    16852 2023-05-16 03:19:15.000000 arthub_api-1.6.4/tests/test_open_api_blade.py
--rw-rw-rw-   0        0        0     3555 2023-05-11 09:00:19.000000 arthub_api-1.6.4/tests/test_storage.py
--rw-rw-rw-   0        0        0     3691 2023-05-11 11:42:27.000000 arthub_api-1.6.4/tests/test_storage_blade.py
+drwxrwxrwx   0        0        0        0 2023-05-16 10:41:07.947564 arthub_api-1.6.5/
+-rw-rw-rw-   0        0        0     1077 2022-09-05 10:15:53.000000 arthub_api-1.6.5/LICENSE
+-rw-rw-rw-   0        0        0      107 2022-09-05 10:15:53.000000 arthub_api-1.6.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     1412 2023-05-16 10:41:07.946566 arthub_api-1.6.5/PKG-INFO
+-rw-rw-rw-   0        0        0      864 2023-05-11 09:00:18.000000 arthub_api-1.6.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-16 10:41:07.876752 arthub_api-1.6.5/arthub_api/
+-rw-rw-rw-   0        0        0      666 2023-05-15 09:23:22.000000 arthub_api-1.6.5/arthub_api/__init__.py
+-rw-rw-rw-   0        0        0     3483 2023-05-16 10:40:32.000000 arthub_api-1.6.5/arthub_api/__main__.py
+-rw-rw-rw-   0        0        0      241 2023-05-16 10:40:32.000000 arthub_api-1.6.5/arthub_api/__version__.py
+-rw-rw-rw-   0        0        0    13661 2023-05-11 11:13:51.000000 arthub_api-1.6.5/arthub_api/_internal_utils.py
+-rw-rw-rw-   0        0        0       84 2023-05-12 03:05:16.000000 arthub_api-1.6.5/arthub_api/arthub_api_config.py
+-rw-rw-rw-   0        0        0      517 2023-03-14 10:44:30.000000 arthub_api-1.6.5/arthub_api/asset_matrix.py
+-rw-rw-rw-   0        0        0    38387 2023-05-16 10:40:32.000000 arthub_api-1.6.5/arthub_api/blade_api.py
+-rw-rw-rw-   0        0        0     1265 2023-05-16 10:40:32.000000 arthub_api-1.6.5/arthub_api/blade_api_instance.py
+-rw-rw-rw-   0        0        0    22945 2023-05-11 11:42:27.000000 arthub_api-1.6.5/arthub_api/blade_storage.py
+-rw-rw-rw-   0        0        0       22 2023-02-08 16:32:42.000000 arthub_api-1.6.5/arthub_api/cli.py
+-rw-rw-rw-   0        0        0     1365 2023-02-08 16:32:42.000000 arthub_api-1.6.5/arthub_api/config.py
+-rw-rw-rw-   0        0        0      523 2023-02-08 16:32:42.000000 arthub_api-1.6.5/arthub_api/exception.py
+-rw-rw-rw-   0        0        0     1258 2023-03-14 10:50:34.000000 arthub_api-1.6.5/arthub_api/models.py
+-rw-rw-rw-   0        0        0    41857 2023-05-15 09:23:22.000000 arthub_api-1.6.5/arthub_api/open_api.py
+-rw-rw-rw-   0        0        0    41828 2023-03-14 11:53:38.000000 arthub_api-1.6.5/arthub_api/storage.py
+-rw-rw-rw-   0        0        0     8941 2023-05-12 03:05:16.000000 arthub_api-1.6.5/arthub_api/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-16 10:41:07.905676 arthub_api-1.6.5/arthub_api.egg-info/
+-rw-rw-rw-   0        0        0     1412 2023-05-16 10:41:06.000000 arthub_api-1.6.5/arthub_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      847 2023-05-16 10:41:07.000000 arthub_api-1.6.5/arthub_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 10:41:06.000000 arthub_api-1.6.5/arthub_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-16 10:41:06.000000 arthub_api-1.6.5/arthub_api.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-02-09 14:04:12.000000 arthub_api-1.6.5/arthub_api.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       65 2023-05-16 10:41:07.000000 arthub_api-1.6.5/arthub_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-16 10:41:07.000000 arthub_api-1.6.5/arthub_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       63 2022-09-26 03:28:18.000000 arthub_api-1.6.5/requirements-dev.txt
+-rw-rw-rw-   0        0        0       42 2023-05-16 10:41:07.947564 arthub_api-1.6.5/setup.cfg
+-rw-rw-rw-   0        0        0     2908 2023-05-11 11:42:27.000000 arthub_api-1.6.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 10:41:07.944572 arthub_api-1.6.5/tests/
+-rw-rw-rw-   0        0        0      139 2023-05-12 03:05:16.000000 arthub_api-1.6.5/tests/__init__.py
+-rw-rw-rw-   0        0        0      108 2023-05-12 03:05:16.000000 arthub_api-1.6.5/tests/_utils.py
+-rw-rw-rw-   0        0        0      267 2023-05-11 09:00:19.000000 arthub_api-1.6.5/tests/conftest.py
+-rw-rw-rw-   0        0        0     5924 2023-05-11 09:00:19.000000 arthub_api-1.6.5/tests/test_open_api.py
+-rw-rw-rw-   0        0        0    17832 2023-05-16 10:40:32.000000 arthub_api-1.6.5/tests/test_open_api_blade.py
+-rw-rw-rw-   0        0        0     3555 2023-05-11 09:00:19.000000 arthub_api-1.6.5/tests/test_storage.py
+-rw-rw-rw-   0        0        0     3691 2023-05-11 11:42:27.000000 arthub_api-1.6.5/tests/test_storage_blade.py
```

### Comparing `arthub_api-1.6.4/LICENSE` & `arthub_api-1.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.4/PKG-INFO` & `arthub_api-1.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arthub_api
-Version: 1.6.4
+Version: 1.6.5
 Summary: ArHhub Python SDK
 Home-page: UNKNOWN
 Author: Joey Ding
 Author-email: joeyding@tencent.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `arthub_api-1.6.4/README.md` & `arthub_api-1.6.5/README.md`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.4/arthub_api/__init__.py` & `arthub_api-1.6.5/arthub_api/__init__.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.4/arthub_api/__main__.py` & `arthub_api-1.6.5/arthub_api/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,27 @@
 import os
 import logging
 import logging.handlers
+
+import environ
+
 from . import arthub_api_config
 from . import cli
 from . import utils
 
 
+@environ.config(prefix="AH_BLADE")
+class DefaultEnvConfig(object):
+    """This creates a env config loads from AH_XXXXX and AH_BLADE_XXXX."""
+    api_config_name = environ.var(os.getenv("AH_API_CONFIG_NAME"), help="Api config name. one of ['oa', 'qq']")
+    public_token = environ.var("",  help="Value for blade public token auth method.")
+    account_email = environ.var(os.getenv("AH_ACCOUNT_NAME"),  help="User name for login auth method.")
+    password = environ.var(os.getenv("AH_PASSWORD"),  help="User password for login auth method.")
+
+
 def load_config(file_path=None):
     UserError = type("UserError", (Exception,), {})
 
     file_path = file_path or os.getenv("ARTHUB_API_CONFIG",
                                        os.path.expanduser("~/Documents/ArtHub/arthub_api_config.py"))
     if not os.path.isfile(file_path):
         return
@@ -67,18 +79,32 @@
     # to stdout
     s_handler = logging.StreamHandler()
     s_handler.setLevel(logging.DEBUG)
     s_handler.setFormatter(logging.Formatter("%(message)s"))
     logger.addHandler(s_handler)
 
 
+def apply_environ_to_config():
+    """This loads config from env and set into arthub_api_config."""
+    ENV_CONFIG = environ.to_config(DefaultEnvConfig)
+    if ENV_CONFIG.api_config_name:
+        arthub_api_config.api_config_name = ENV_CONFIG.api_config_name
+    if ENV_CONFIG.public_token:
+        arthub_api_config.blade_public_token = ENV_CONFIG.public_token
+    if ENV_CONFIG.account_email:
+        arthub_api_config.account_email = ENV_CONFIG.account_email
+    if ENV_CONFIG.password:
+        arthub_api_config.password = ENV_CONFIG.password
+
+
 def init_config():
     setup_logging()
     patch_config()
     load_config()
+    apply_environ_to_config()
 
 
 def main():
     init_config()
     cli.cli()
```

### Comparing `arthub_api-1.6.4/arthub_api/_internal_utils.py` & `arthub_api-1.6.5/arthub_api/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.4/arthub_api/asset_matrix.py` & `arthub_api-1.6.5/arthub_api/asset_matrix.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.4/arthub_api/blade_api.py` & `arthub_api-1.6.5/arthub_api/blade_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1002,7 +1002,17 @@
             }
             leaf object contains {name, version, requires, variants}
         """
         url = self._blade_resolving_url("get-rez-repo")
         res = self._make_api_request(url, {"refresh": force_refresh})
         res.set_result_as_first_item()
         return res
+
+    def blade_get_package_count(self):
+        r"""
+        :rtype: arthub_api.APIResponse
+            result: (number) count of packages
+        """
+        url = self._blade_resolving_url("get-package-count")
+        res = self._make_api_request(url, {})
+        res.set_result_by_key("count")
+        return res
```

### Comparing `arthub_api-1.6.4/arthub_api/blade_storage.py` & `arthub_api-1.6.5/arthub_api/blade_storage.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.4/arthub_api/config.py` & `arthub_api-1.6.5/arthub_api/config.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.4/arthub_api/exception.py` & `arthub_api-1.6.5/arthub_api/exception.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.4/arthub_api/models.py` & `arthub_api-1.6.5/arthub_api/models.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.4/arthub_api/open_api.py` & `arthub_api-1.6.5/arthub_api/open_api.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.4/arthub_api/storage.py` & `arthub_api-1.6.5/arthub_api/storage.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.4/arthub_api/utils.py` & `arthub_api-1.6.5/arthub_api/utils.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.4/arthub_api.egg-info/PKG-INFO` & `arthub_api-1.6.5/arthub_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arthub-api
-Version: 1.6.4
+Version: 1.6.5
 Summary: ArHhub Python SDK
 Home-page: UNKNOWN
 Author: Joey Ding
 Author-email: joeyding@tencent.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `arthub_api-1.6.4/arthub_api.egg-info/SOURCES.txt` & `arthub_api-1.6.5/arthub_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.4/setup.py` & `arthub_api-1.6.5/setup.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.4/tests/test_open_api.py` & `arthub_api-1.6.5/tests/test_open_api.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.4/tests/test_open_api_blade.py` & `arthub_api-1.6.5/tests/test_open_api_blade.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,38 @@
+import os
+from contextlib import contextmanager
+
 from requests import JSONDecodeError
 
 import arthub_api
 import pytest
 import logging
 
 from arthub_api.open_api import NotLoginError
 from . import _utils
 from arthub_api import (
     arthub_api_config,
-    BladeAPI,
+    BladeAPI, init_config,
 )
 from arthub_api.blade_api_instance import BladeInstance
 
 
+@contextmanager
+def set_env_var(name, value):
+    original_value = os.environ.get(name)
+    os.environ[name] = value
+    try:
+        yield
+    finally:
+        if original_value is None:
+            del os.environ[name]
+        else:
+            os.environ[name] = original_value
+
+
 def on_api_failed(res):
     logging.error("[TEST][API][API] \"%s\" failed, error: %s" % (res.url, res.error_message()))
 
 
 def init_api(env, login=True):
     api = BladeAPI(_utils.get_config(env), False)
     if login:
@@ -549,7 +565,22 @@
 
 
 def test_global_instance(env):
     backend=BladeInstance.backend()
     assert isinstance(backend, BladeAPI)
     backend2=BladeInstance.backend()
     assert backend2 == backend
+
+
+def test_env_config(env):
+    with set_env_var("AH_BLADE_API_CONFIG_NAME", "test_input"):
+        init_config()
+        assert arthub_api_config.api_config_name == "test_input"
+    with set_env_var("AH_BLADE_PUBLIC_TOKEN", "test_input2"):
+        init_config()
+        assert arthub_api_config.blade_public_token == "test_input2"
+    with set_env_var("AH_BLADE_ACCOUNT_EMAIL", "email1"):
+        init_config()
+        assert arthub_api_config.account_email == "email1"
+    with set_env_var("AH_BLADE_PASSWORD", "password1"):
+        init_config()
+        assert arthub_api_config.password == "password1"
```

### Comparing `arthub_api-1.6.4/tests/test_storage.py` & `arthub_api-1.6.5/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.4/tests/test_storage_blade.py` & `arthub_api-1.6.5/tests/test_storage_blade.py`

 * *Files identical despite different names*

