# Comparing `tmp/arthub_api-1.6.3.tar.gz` & `tmp/arthub_api-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arthub_api-1.6.3.tar", last modified: Mon May 15 09:23:52 2023, max compression
+gzip compressed data, was "arthub_api-1.6.4.tar", last modified: Tue May 16 03:20:44 2023, max compression
```

## Comparing `arthub_api-1.6.3.tar` & `arthub_api-1.6.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 09:23:52.454767 arthub_api-1.6.3/
--rw-rw-rw-   0        0        0     1077 2022-09-05 10:15:53.000000 arthub_api-1.6.3/LICENSE
--rw-rw-rw-   0        0        0      107 2022-09-05 10:15:53.000000 arthub_api-1.6.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1412 2023-05-15 09:23:52.453767 arthub_api-1.6.3/PKG-INFO
--rw-rw-rw-   0        0        0      864 2023-05-11 09:00:18.000000 arthub_api-1.6.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 09:23:52.383916 arthub_api-1.6.3/arthub_api/
--rw-rw-rw-   0        0        0      666 2023-05-15 09:23:22.000000 arthub_api-1.6.3/arthub_api/__init__.py
--rw-rw-rw-   0        0        0     2316 2023-05-12 03:05:16.000000 arthub_api-1.6.3/arthub_api/__main__.py
--rw-rw-rw-   0        0        0      241 2023-05-15 09:23:22.000000 arthub_api-1.6.3/arthub_api/__version__.py
--rw-rw-rw-   0        0        0    13661 2023-05-11 11:13:51.000000 arthub_api-1.6.3/arthub_api/_internal_utils.py
--rw-rw-rw-   0        0        0       84 2023-05-12 03:05:16.000000 arthub_api-1.6.3/arthub_api/arthub_api_config.py
--rw-rw-rw-   0        0        0      517 2023-03-14 10:44:30.000000 arthub_api-1.6.3/arthub_api/asset_matrix.py
--rw-rw-rw-   0        0        0    37291 2023-05-12 03:05:16.000000 arthub_api-1.6.3/arthub_api/blade_api.py
--rw-rw-rw-   0        0        0     1032 2023-05-15 09:23:22.000000 arthub_api-1.6.3/arthub_api/blade_api_instance.py
--rw-rw-rw-   0        0        0    22945 2023-05-11 11:42:27.000000 arthub_api-1.6.3/arthub_api/blade_storage.py
--rw-rw-rw-   0        0        0       22 2023-02-08 16:32:42.000000 arthub_api-1.6.3/arthub_api/cli.py
--rw-rw-rw-   0        0        0     1365 2023-02-08 16:32:42.000000 arthub_api-1.6.3/arthub_api/config.py
--rw-rw-rw-   0        0        0      523 2023-02-08 16:32:42.000000 arthub_api-1.6.3/arthub_api/exception.py
--rw-rw-rw-   0        0        0     1258 2023-03-14 10:50:34.000000 arthub_api-1.6.3/arthub_api/models.py
--rw-rw-rw-   0        0        0    41857 2023-05-15 09:23:22.000000 arthub_api-1.6.3/arthub_api/open_api.py
--rw-rw-rw-   0        0        0    41828 2023-03-14 11:53:38.000000 arthub_api-1.6.3/arthub_api/storage.py
--rw-rw-rw-   0        0        0     8941 2023-05-12 03:05:16.000000 arthub_api-1.6.3/arthub_api/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-15 09:23:52.411904 arthub_api-1.6.3/arthub_api.egg-info/
--rw-rw-rw-   0        0        0     1412 2023-05-15 09:23:51.000000 arthub_api-1.6.3/arthub_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      847 2023-05-15 09:23:51.000000 arthub_api-1.6.3/arthub_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 09:23:51.000000 arthub_api-1.6.3/arthub_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-15 09:23:51.000000 arthub_api-1.6.3/arthub_api.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-02-09 14:04:12.000000 arthub_api-1.6.3/arthub_api.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       65 2023-05-15 09:23:51.000000 arthub_api-1.6.3/arthub_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-15 09:23:51.000000 arthub_api-1.6.3/arthub_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       63 2022-09-26 03:28:18.000000 arthub_api-1.6.3/requirements-dev.txt
--rw-rw-rw-   0        0        0       42 2023-05-15 09:23:52.454767 arthub_api-1.6.3/setup.cfg
--rw-rw-rw-   0        0        0     2908 2023-05-11 11:42:27.000000 arthub_api-1.6.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-15 09:23:52.451737 arthub_api-1.6.3/tests/
--rw-rw-rw-   0        0        0      139 2023-05-12 03:05:16.000000 arthub_api-1.6.3/tests/__init__.py
--rw-rw-rw-   0        0        0      108 2023-05-12 03:05:16.000000 arthub_api-1.6.3/tests/_utils.py
--rw-rw-rw-   0        0        0      267 2023-05-11 09:00:19.000000 arthub_api-1.6.3/tests/conftest.py
--rw-rw-rw-   0        0        0     5924 2023-05-11 09:00:19.000000 arthub_api-1.6.3/tests/test_open_api.py
--rw-rw-rw-   0        0        0    16594 2023-05-15 09:23:22.000000 arthub_api-1.6.3/tests/test_open_api_blade.py
--rw-rw-rw-   0        0        0     3555 2023-05-11 09:00:19.000000 arthub_api-1.6.3/tests/test_storage.py
--rw-rw-rw-   0        0        0     3691 2023-05-11 11:42:27.000000 arthub_api-1.6.3/tests/test_storage_blade.py
+drwxrwxrwx   0        0        0        0 2023-05-16 03:20:44.060739 arthub_api-1.6.4/
+-rw-rw-rw-   0        0        0     1077 2022-09-05 10:15:53.000000 arthub_api-1.6.4/LICENSE
+-rw-rw-rw-   0        0        0      107 2022-09-05 10:15:53.000000 arthub_api-1.6.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1412 2023-05-16 03:20:44.060739 arthub_api-1.6.4/PKG-INFO
+-rw-rw-rw-   0        0        0      864 2023-05-11 09:00:18.000000 arthub_api-1.6.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-16 03:20:44.041249 arthub_api-1.6.4/arthub_api/
+-rw-rw-rw-   0        0        0      666 2023-05-15 09:23:22.000000 arthub_api-1.6.4/arthub_api/__init__.py
+-rw-rw-rw-   0        0        0     2316 2023-05-12 03:05:16.000000 arthub_api-1.6.4/arthub_api/__main__.py
+-rw-rw-rw-   0        0        0      241 2023-05-16 03:20:38.000000 arthub_api-1.6.4/arthub_api/__version__.py
+-rw-rw-rw-   0        0        0    13661 2023-05-11 11:13:51.000000 arthub_api-1.6.4/arthub_api/_internal_utils.py
+-rw-rw-rw-   0        0        0       84 2023-05-12 03:05:16.000000 arthub_api-1.6.4/arthub_api/arthub_api_config.py
+-rw-rw-rw-   0        0        0      517 2023-03-14 10:44:30.000000 arthub_api-1.6.4/arthub_api/asset_matrix.py
+-rw-rw-rw-   0        0        0    38061 2023-05-16 03:19:15.000000 arthub_api-1.6.4/arthub_api/blade_api.py
+-rw-rw-rw-   0        0        0     1032 2023-05-15 09:23:22.000000 arthub_api-1.6.4/arthub_api/blade_api_instance.py
+-rw-rw-rw-   0        0        0    22945 2023-05-11 11:42:27.000000 arthub_api-1.6.4/arthub_api/blade_storage.py
+-rw-rw-rw-   0        0        0       22 2023-02-08 16:32:42.000000 arthub_api-1.6.4/arthub_api/cli.py
+-rw-rw-rw-   0        0        0     1365 2023-02-08 16:32:42.000000 arthub_api-1.6.4/arthub_api/config.py
+-rw-rw-rw-   0        0        0      523 2023-02-08 16:32:42.000000 arthub_api-1.6.4/arthub_api/exception.py
+-rw-rw-rw-   0        0        0     1258 2023-03-14 10:50:34.000000 arthub_api-1.6.4/arthub_api/models.py
+-rw-rw-rw-   0        0        0    41857 2023-05-15 09:23:22.000000 arthub_api-1.6.4/arthub_api/open_api.py
+-rw-rw-rw-   0        0        0    41828 2023-03-14 11:53:38.000000 arthub_api-1.6.4/arthub_api/storage.py
+-rw-rw-rw-   0        0        0     8941 2023-05-12 03:05:16.000000 arthub_api-1.6.4/arthub_api/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-16 03:20:44.050224 arthub_api-1.6.4/arthub_api.egg-info/
+-rw-rw-rw-   0        0        0     1412 2023-05-16 03:20:43.000000 arthub_api-1.6.4/arthub_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      847 2023-05-16 03:20:43.000000 arthub_api-1.6.4/arthub_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 03:20:43.000000 arthub_api-1.6.4/arthub_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-16 03:20:43.000000 arthub_api-1.6.4/arthub_api.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-02-09 14:04:12.000000 arthub_api-1.6.4/arthub_api.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       65 2023-05-16 03:20:43.000000 arthub_api-1.6.4/arthub_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-16 03:20:43.000000 arthub_api-1.6.4/arthub_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       63 2022-09-26 03:28:18.000000 arthub_api-1.6.4/requirements-dev.txt
+-rw-rw-rw-   0        0        0       42 2023-05-16 03:20:44.060739 arthub_api-1.6.4/setup.cfg
+-rw-rw-rw-   0        0        0     2908 2023-05-11 11:42:27.000000 arthub_api-1.6.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 03:20:44.059229 arthub_api-1.6.4/tests/
+-rw-rw-rw-   0        0        0      139 2023-05-12 03:05:16.000000 arthub_api-1.6.4/tests/__init__.py
+-rw-rw-rw-   0        0        0      108 2023-05-12 03:05:16.000000 arthub_api-1.6.4/tests/_utils.py
+-rw-rw-rw-   0        0        0      267 2023-05-11 09:00:19.000000 arthub_api-1.6.4/tests/conftest.py
+-rw-rw-rw-   0        0        0     5924 2023-05-11 09:00:19.000000 arthub_api-1.6.4/tests/test_open_api.py
+-rw-rw-rw-   0        0        0    16852 2023-05-16 03:19:15.000000 arthub_api-1.6.4/tests/test_open_api_blade.py
+-rw-rw-rw-   0        0        0     3555 2023-05-11 09:00:19.000000 arthub_api-1.6.4/tests/test_storage.py
+-rw-rw-rw-   0        0        0     3691 2023-05-11 11:42:27.000000 arthub_api-1.6.4/tests/test_storage_blade.py
```

### Comparing `arthub_api-1.6.3/LICENSE` & `arthub_api-1.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.3/PKG-INFO` & `arthub_api-1.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arthub_api
-Version: 1.6.3
+Version: 1.6.4
 Summary: ArHhub Python SDK
 Home-page: UNKNOWN
 Author: Joey Ding
 Author-email: joeyding@tencent.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `arthub_api-1.6.3/README.md` & `arthub_api-1.6.4/README.md`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.3/arthub_api/__init__.py` & `arthub_api-1.6.4/arthub_api/__init__.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.3/arthub_api/__main__.py` & `arthub_api-1.6.4/arthub_api/__main__.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.3/arthub_api/_internal_utils.py` & `arthub_api-1.6.4/arthub_api/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.3/arthub_api/asset_matrix.py` & `arthub_api-1.6.4/arthub_api/asset_matrix.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.3/arthub_api/blade_api.py` & `arthub_api-1.6.4/arthub_api/blade_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -982,7 +982,27 @@
                 "origin_url": str,
                 "size": 1601
             }, ...]
             size is bytes size of existed file, useful for multipart download
         """
         url = self._blade_resolving_url("download-package")
         return self._make_api_request(url, {"packages": packages})
+
+    def blade_get_rez_repo(self, force_refresh=False):
+        r"""
+        :param packages: force_refresh: bool.  indicates whether to refresh rez_repo with the latest package info
+        :rtype: arthub_api.APIResponse
+            {
+                "data": {
+                    "pkg_name": {
+                        "pkg_version1": {...},
+                        "pkg_version2": {...},
+                    }
+                 },
+                "api_modified": "xxxx"
+            }
+            leaf object contains {name, version, requires, variants}
+        """
+        url = self._blade_resolving_url("get-rez-repo")
+        res = self._make_api_request(url, {"refresh": force_refresh})
+        res.set_result_as_first_item()
+        return res
```

### Comparing `arthub_api-1.6.3/arthub_api/blade_api_instance.py` & `arthub_api-1.6.4/arthub_api/blade_api_instance.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.3/arthub_api/blade_storage.py` & `arthub_api-1.6.4/arthub_api/blade_storage.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.3/arthub_api/config.py` & `arthub_api-1.6.4/arthub_api/config.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.3/arthub_api/exception.py` & `arthub_api-1.6.4/arthub_api/exception.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.3/arthub_api/models.py` & `arthub_api-1.6.4/arthub_api/models.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.3/arthub_api/open_api.py` & `arthub_api-1.6.4/arthub_api/open_api.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.3/arthub_api/storage.py` & `arthub_api-1.6.4/arthub_api/storage.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.3/arthub_api/utils.py` & `arthub_api-1.6.4/arthub_api/utils.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.3/arthub_api.egg-info/PKG-INFO` & `arthub_api-1.6.4/arthub_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arthub-api
-Version: 1.6.3
+Version: 1.6.4
 Summary: ArHhub Python SDK
 Home-page: UNKNOWN
 Author: Joey Ding
 Author-email: joeyding@tencent.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `arthub_api-1.6.3/arthub_api.egg-info/SOURCES.txt` & `arthub_api-1.6.4/arthub_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.3/setup.py` & `arthub_api-1.6.4/setup.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.3/tests/test_open_api.py` & `arthub_api-1.6.4/tests/test_open_api.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.3/tests/test_open_api_blade.py` & `arthub_api-1.6.4/tests/test_open_api_blade.py`

 * *Files 1% similar despite different names*

```diff
@@ -380,27 +380,33 @@
     # delete
     res = blade_api.blade_delete_permission_on_toolbox_by_account_name(toolbox_id, [perm_item])
     assert res.is_succeeded()
 
     # delete toolbox
     delete_node(env, toolbox_id, root_id)
 
+    # delete token
+    blade_api.blade_delete_public_token_by_id(token_id)
+    assert res.is_succeeded()
+
 
 def test_permission_on_config(env):
     blade_api = init_api(env)
     root_id = get_root_id(env)
 
     res = blade_api.blade_create_public_token("sdk_test_token_config", 100)
     assert res.is_succeeded()
+    token_id = res.result["id"]
     token_str = res.result["name"]
 
     # set public token to config permission
     # add
     perm_item = {"account_name": token_str, "type": "public_token"}
     res = blade_api.blade_add_permission_on_config_by_account_name("developer", [perm_item])
+    res.raise_for_err()
     assert res.is_succeeded()
 
     # get
     res = blade_api.blade_get_permission_on_config()
     assert res.is_succeeded()
     assert res.result["developer"][0] == perm_item
 
@@ -414,14 +420,17 @@
     res = blade_api_token.blade_delete_config("token_test", root_id, "node")
     assert res.is_succeeded()
 
     # delete
     res = blade_api.blade_delete_permission_on_config_by_account_name([perm_item])
     assert res.is_succeeded()
 
+    blade_api.blade_delete_public_token_by_id(token_id)
+    assert res.is_succeeded()
+
 def test_convert_context_string(env):
     blade_api = init_api(env)
     root_id = get_root_id(env)
 
     res = blade_api.blade_convert_context_string("globals:globals", "lightbox_config")
     assert res.is_succeeded()
     out = res.first_result()
```

### Comparing `arthub_api-1.6.3/tests/test_storage.py` & `arthub_api-1.6.4/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `arthub_api-1.6.3/tests/test_storage_blade.py` & `arthub_api-1.6.4/tests/test_storage_blade.py`

 * *Files identical despite different names*

