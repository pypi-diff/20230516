# Comparing `tmp/azure_datalake_utils-0.5.5.tar.gz` & `tmp/azure_datalake_utils-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure_datalake_utils-0.5.5.tar", max compression
+gzip compressed data, was "azure_datalake_utils-0.5.6.tar", max compression
```

## Comparing `azure_datalake_utils-0.5.5.tar` & `azure_datalake_utils-0.5.6.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0    11357 2023-02-15 17:28:37.738967 azure_datalake_utils-0.5.5/LICENSE
--rw-r--r--   0        0        0     2311 2023-02-15 17:28:37.738967 azure_datalake_utils-0.5.5/README.md
--rw-r--r--   0        0        0      297 2023-02-15 17:28:37.738967 azure_datalake_utils-0.5.5/azure_datalake_utils/__init__.py
--rw-r--r--   0        0        0    13183 2023-02-15 17:28:37.738967 azure_datalake_utils-0.5.5/azure_datalake_utils/azure_datalake_utils.py
--rw-r--r--   0        0        0     2171 2023-02-15 17:28:37.738967 azure_datalake_utils-0.5.5/azure_datalake_utils/exepctions.py
--rw-r--r--   0        0        0     1685 2023-02-15 17:28:37.738967 azure_datalake_utils-0.5.5/azure_datalake_utils/experimental.py
--rw-r--r--   0        0        0     8728 2023-02-15 17:28:37.738967 azure_datalake_utils-0.5.5/azure_datalake_utils/partitions.py
--rw-r--r--   0        0        0     3106 2023-02-15 17:28:37.742967 azure_datalake_utils-0.5.5/pyproject.toml
--rw-r--r--   0        0        0       50 2023-02-15 17:28:37.742967 azure_datalake_utils-0.5.5/tests/__init__.py
--rw-r--r--   0        0        0     8810 2023-02-15 17:28:37.742967 azure_datalake_utils-0.5.5/tests/test_azure_datalake_utils.py
--rw-r--r--   0        0        0      561 2023-02-15 17:28:37.742967 azure_datalake_utils-0.5.5/tests/test_azure_exepctions.py
--rw-r--r--   0        0        0    13027 2023-02-15 17:28:37.742967 azure_datalake_utils-0.5.5/tests/test_partitions.py
--rw-r--r--   0        0        0     4040 1970-01-01 00:00:00.000000 azure_datalake_utils-0.5.5/setup.py
--rw-r--r--   0        0        0     4899 1970-01-01 00:00:00.000000 azure_datalake_utils-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-16 11:19:41.153928 azure_datalake_utils-0.5.6/LICENSE
+-rw-r--r--   0        0        0     2311 2023-05-16 11:19:41.153928 azure_datalake_utils-0.5.6/README.md
+-rw-r--r--   0        0        0      297 2023-05-16 11:19:41.153928 azure_datalake_utils-0.5.6/azure_datalake_utils/__init__.py
+-rw-r--r--   0        0        0    13240 2023-05-16 11:19:41.153928 azure_datalake_utils-0.5.6/azure_datalake_utils/azure_datalake_utils.py
+-rw-r--r--   0        0        0     2171 2023-05-16 11:19:41.153928 azure_datalake_utils-0.5.6/azure_datalake_utils/exepctions.py
+-rw-r--r--   0        0        0     1685 2023-05-16 11:19:41.153928 azure_datalake_utils-0.5.6/azure_datalake_utils/experimental.py
+-rw-r--r--   0        0        0     8728 2023-05-16 11:19:41.153928 azure_datalake_utils-0.5.6/azure_datalake_utils/partitions.py
+-rw-r--r--   0        0        0     3106 2023-05-16 11:19:41.157928 azure_datalake_utils-0.5.6/pyproject.toml
+-rw-r--r--   0        0        0       50 2023-05-16 11:19:41.157928 azure_datalake_utils-0.5.6/tests/__init__.py
+-rw-r--r--   0        0        0     8892 2023-05-16 11:19:41.157928 azure_datalake_utils-0.5.6/tests/test_azure_datalake_utils.py
+-rw-r--r--   0        0        0      561 2023-05-16 11:19:41.157928 azure_datalake_utils-0.5.6/tests/test_azure_exepctions.py
+-rw-r--r--   0        0        0    13027 2023-05-16 11:19:41.157928 azure_datalake_utils-0.5.6/tests/test_partitions.py
+-rw-r--r--   0        0        0     4899 1970-01-01 00:00:00.000000 azure_datalake_utils-0.5.6/PKG-INFO
```

### Comparing `azure_datalake_utils-0.5.5/LICENSE` & `azure_datalake_utils-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `azure_datalake_utils-0.5.5/README.md` & `azure_datalake_utils-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `azure_datalake_utils-0.5.5/azure_datalake_utils/azure_datalake_utils.py` & `azure_datalake_utils-0.5.6/azure_datalake_utils/azure_datalake_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,14 @@
                 Para ver los efectos, ver los siguientes issues:
                 - https://github.com/fsspec/adlfs/issues/391
                 - https://github.com/Azure/azure-sdk-for-python/issues/28312
         """
         self.datalake_name = datalake_name
 
         if account_key is None:
-
             self.tenant_id = tenant_id
             credentials = InteractiveBrowserCredential(tenant_id=self.tenant_id)
             credentials.authenticate()
             self._credentials = credentials
             # TODO: verificar https://github.com/fsspec/adlfs/issues/270
             # para ver como evoluciona y evitar este condicional.
             if platform.system().lower() != 'windows':
@@ -58,16 +57,17 @@
                 }
 
         else:
             storage_options = {'account_name': self.datalake_name, 'account_key': account_key}
             self.fs = AzureBlobFileSystem(account_name=self.datalake_name, account_key=account_key)
 
         if not fsspec_cache:
-            storage_options['default_cache_type'] = None
+            storage_options["default_cache_type"] = None
             storage_options["default_fill_cache"] = False
+            storage_options["skip_instance_cache"] = True
 
         self.storage_options = storage_options
 
     @classmethod
     def from_account_key(cls, datalake_name: str, account_key: str, fsspec_cache: bool = True):
         """Opcion de inicializar con account key."""
         return cls(datalake_name=datalake_name, account_key=account_key, tenant_id=None, fsspec_cache=fsspec_cache)
```

### Comparing `azure_datalake_utils-0.5.5/azure_datalake_utils/exepctions.py` & `azure_datalake_utils-0.5.6/azure_datalake_utils/exepctions.py`

 * *Files identical despite different names*

### Comparing `azure_datalake_utils-0.5.5/azure_datalake_utils/experimental.py` & `azure_datalake_utils-0.5.6/azure_datalake_utils/experimental.py`

 * *Files identical despite different names*

### Comparing `azure_datalake_utils-0.5.5/azure_datalake_utils/partitions.py` & `azure_datalake_utils-0.5.6/azure_datalake_utils/partitions.py`

 * *Files identical despite different names*

### Comparing `azure_datalake_utils-0.5.5/pyproject.toml` & `azure_datalake_utils-0.5.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "azure_datalake_utils"
-version = "0.5.5"
+version = "0.5.6"
 homepage = "https://github.com/centraal-api/azure-datalake-utils"
 description = "Utilidades para interactuar con Azure Datalake."
 authors = ["centraal.studio <equipo@centraal.studio>"]
 readme = "README.md"
 license =  "Apache-2.0"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
```

### Comparing `azure_datalake_utils-0.5.5/tests/test_azure_datalake_utils.py` & `azure_datalake_utils-0.5.6/tests/test_azure_datalake_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,14 +64,15 @@
         dl = Datalake('name', 'tenant', fsspec_cache=False)
         if platform.system().lower() != 'windows':
             assert dl.storage_options == {
                 'account_name': 'name',
                 'anon': False,
                 'default_cache_type': None,
                 'default_fill_cache': False,
+                'skip_instance_cache': True,
             }
         else:
             assert dl.storage_options['account_name'] == 'name'
             assert dl.storage_options['default_cache_type'] is None, "no se esta invalidando el cache."
             assert not dl.storage_options['anon']
             assert isinstance(dl.storage_options['credential'], DefaultAzureCredential)
 
@@ -83,14 +84,15 @@
 
     dl = Datalake.from_account_key('name', 'key', False)
     assert dl.storage_options == {
         'account_name': 'name',
         'account_key': 'key',
         'default_cache_type': None,
         'default_fill_cache': False,
+        'skip_instance_cache': True,
     }, "no se esta invalidando el cache."
 
 
 def test_verificar_extension_should_check_extensions():
     """Test de verificar de Datalake."""
     with patch('azure.identity.InteractiveBrowserCredential.authenticate', return_value=fake_record):
         dl = Datalake('name', 'tenant')
```

### Comparing `azure_datalake_utils-0.5.5/tests/test_azure_exepctions.py` & `azure_datalake_utils-0.5.6/tests/test_azure_exepctions.py`

 * *Files identical despite different names*

### Comparing `azure_datalake_utils-0.5.5/tests/test_partitions.py` & `azure_datalake_utils-0.5.6/tests/test_partitions.py`

 * *Files identical despite different names*

### Comparing `azure_datalake_utils-0.5.5/PKG-INFO` & `azure_datalake_utils-0.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-datalake-utils
-Version: 0.5.5
+Version: 0.5.6
 Summary: Utilidades para interactuar con Azure Datalake.
 Home-page: https://github.com/centraal-api/azure-datalake-utils
 License: Apache-2.0
 Author: centraal.studio
 Author-email: equipo@centraal.studio
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

