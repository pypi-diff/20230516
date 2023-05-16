# Comparing `tmp/numbers-c2pa-0.0.6.tar.gz` & `tmp/numbers-c2pa-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/numbers-c2pa/numbers-c2pa/dist/.tmp-u5ex6h_3/numbers-c2pa-0.0.6.tar", last modified: Mon May 15 10:34:39 2023, max compression
+gzip compressed data, was "/home/runner/work/numbers-c2pa/numbers-c2pa/dist/.tmp-l6vx6c5z/numbers-c2pa-0.0.7.tar", last modified: Tue May 16 08:05:50 2023, max compression
```

## Comparing `numbers-c2pa-0.0.6.tar` & `numbers-c2pa-0.0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:34:39.000000 numbers-c2pa-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-15 10:34:25.000000 numbers-c2pa-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-05-15 10:34:39.000000 numbers-c2pa-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-05-15 10:34:25.000000 numbers-c2pa-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-15 10:34:25.000000 numbers-c2pa-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-15 10:34:39.000000 numbers-c2pa-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-15 10:34:25.000000 numbers-c2pa-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:34:39.000000 numbers-c2pa-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:34:39.000000 numbers-c2pa-0.0.6/src/numbers_c2pa/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-15 10:34:25.000000 numbers-c2pa-0.0.6/src/numbers_c2pa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-05-15 10:34:25.000000 numbers-c2pa-0.0.6/src/numbers_c2pa/core.py
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-15 10:34:25.000000 numbers-c2pa-0.0.6/src/numbers_c2pa/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-05-15 10:34:25.000000 numbers-c2pa-0.0.6/src/numbers_c2pa/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:34:39.000000 numbers-c2pa-0.0.6/src/numbers_c2pa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-05-15 10:34:39.000000 numbers-c2pa-0.0.6/src/numbers_c2pa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-15 10:34:39.000000 numbers-c2pa-0.0.6/src/numbers_c2pa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 10:34:39.000000 numbers-c2pa-0.0.6/src/numbers_c2pa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-15 10:34:39.000000 numbers-c2pa-0.0.6/src/numbers_c2pa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-15 10:34:39.000000 numbers-c2pa-0.0.6/src/numbers_c2pa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 10:34:39.000000 numbers-c2pa-0.0.6/src/numbers_c2pa.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:34:39.000000 numbers-c2pa-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-15 10:34:25.000000 numbers-c2pa-0.0.6/tests/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:05:50.000000 numbers-c2pa-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-16 08:05:36.000000 numbers-c2pa-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-05-16 08:05:50.000000 numbers-c2pa-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-05-16 08:05:36.000000 numbers-c2pa-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-16 08:05:36.000000 numbers-c2pa-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-16 08:05:50.000000 numbers-c2pa-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-16 08:05:36.000000 numbers-c2pa-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:05:50.000000 numbers-c2pa-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:05:50.000000 numbers-c2pa-0.0.7/src/numbers_c2pa/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-16 08:05:36.000000 numbers-c2pa-0.0.7/src/numbers_c2pa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7411 2023-05-16 08:05:36.000000 numbers-c2pa-0.0.7/src/numbers_c2pa/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-16 08:05:36.000000 numbers-c2pa-0.0.7/src/numbers_c2pa/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-05-16 08:05:36.000000 numbers-c2pa-0.0.7/src/numbers_c2pa/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:05:50.000000 numbers-c2pa-0.0.7/src/numbers_c2pa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-05-16 08:05:50.000000 numbers-c2pa-0.0.7/src/numbers_c2pa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-16 08:05:50.000000 numbers-c2pa-0.0.7/src/numbers_c2pa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 08:05:50.000000 numbers-c2pa-0.0.7/src/numbers_c2pa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-16 08:05:50.000000 numbers-c2pa-0.0.7/src/numbers_c2pa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-16 08:05:50.000000 numbers-c2pa-0.0.7/src/numbers_c2pa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 08:05:49.000000 numbers-c2pa-0.0.7/src/numbers_c2pa.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:05:50.000000 numbers-c2pa-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-16 08:05:36.000000 numbers-c2pa-0.0.7/tests/test_core.py
```

### Comparing `numbers-c2pa-0.0.6/LICENSE` & `numbers-c2pa-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `numbers-c2pa-0.0.6/PKG-INFO` & `numbers-c2pa-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numbers-c2pa
-Version: 0.0.6
+Version: 0.0.7
 Summary: Numbers C2PA tool
 Home-page: https://github.com/numbersprotocol/numbers-c2pa
 Author: Numbers Co., Inc
 Author-email: dev@numbersprotocol.io
 Keywords: authenticity
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `numbers-c2pa-0.0.6/README.md` & `numbers-c2pa-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `numbers-c2pa-0.0.6/setup.cfg` & `numbers-c2pa-0.0.7/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = numbers-c2pa
-version = 0.0.6
+version = 0.0.7
 author = Numbers Co., Inc
 author_email = dev@numbersprotocol.io
 description = Numbers C2PA tool
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = authenticity
 url = https://github.com/numbersprotocol/numbers-c2pa
```

### Comparing `numbers-c2pa-0.0.6/src/numbers_c2pa/__init__.py` & `numbers-c2pa-0.0.7/src/numbers_c2pa/__init__.py`

 * *Files identical despite different names*

### Comparing `numbers-c2pa-0.0.6/src/numbers_c2pa/core.py` & `numbers-c2pa-0.0.7/src/numbers_c2pa/core.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,14 +12,42 @@
 def _mimetype_to_ext(asset_mime_type: str):
     ext = mimetypes.guess_extension(asset_mime_type)
     if not ext:
         raise ValueError(f'Could not find a file extension for MIME type: {asset_mime_type}')
     return ext
 
 
+def c2patool_inject(
+    file_path: str,
+    manifest_path: str,
+    output_path: str,
+    force_overwrite: bool,
+    private_key: Optional[str] = None,
+    sign_cert: Optional[str] = None,
+):
+    env_vars = os.environ.copy()
+    if private_key:
+        env_vars['C2PA_PRIVATE_KEY'] = private_key
+    if sign_cert:
+        env_vars['C2PA_SIGN_CERT'] = sign_cert
+    command = f'c2patool "{file_path}" -m "{manifest_path}" -o "{output_path}"'
+    if force_overwrite:
+        command += ' -f'
+    try:
+        subprocess.run(
+            command,
+            shell=True,
+            env=env_vars,
+            check=True,
+            stderr=subprocess.PIPE,
+        )
+    except subprocess.CalledProcessError as e:
+        raise UnknownError(e.stderr)
+
+
 def create_c2pa_manifest(
     nid: str,
     creator_public_key: str,
     asset_hash: str,
     date_created: datetime,
     location_created: str,
     date_captured: Optional[datetime],
@@ -136,32 +164,22 @@
             json.dump(manifest, f)
 
         asset_file = os.path.join(temp_dir, f'asset.{file_ext}')
         with open(asset_file, 'wb') as f:
             f.write(asset_bytes)
 
         asset_c2pa_file = os.path.join(temp_dir, f'asset-c2pa.{file_ext}')
-        env_vars = os.environ.copy()
-        if private_key:
-            env_vars['C2PA_PRIVATE_KEY'] = private_key
-        if sign_cert:
-            env_vars['C2PA_SIGN_CERT'] = sign_cert
-        command = f'c2patool {asset_file} -m {manifest_file} -o {asset_c2pa_file}'
-        if force_overwrite:
-            command += ' -f'
-        try:
-            subprocess.run(
-                command,
-                shell=True,
-                env=env_vars,
-                check=True,
-                stderr=subprocess.PIPE,
-            )
-        except subprocess.CalledProcessError as e:
-            raise UnknownError(e.stderr)
+        c2patool_inject(
+            asset_file,
+            manifest_file,
+            asset_c2pa_file,
+            force_overwrite=force_overwrite,
+            private_key=private_key,
+            sign_cert=sign_cert,
+        )
 
         with open(asset_c2pa_file, 'rb') as f:
             asset_c2pa_bytes = f.read()
         return asset_c2pa_bytes
 
 
 def inject_file(
@@ -174,32 +192,22 @@
 ):
     """Perform C2PA injection given an existing asset file.
     """
     with NamedTemporaryFile(prefix='manifest_', mode='w') as manifest_temp_file:
         json.dump(manifest, manifest_temp_file)
         manifest_temp_file.flush()
 
-        env_vars = os.environ.copy()
-        if private_key:
-            env_vars['C2PA_PRIVATE_KEY'] = private_key
-        if sign_cert:
-            env_vars['C2PA_SIGN_CERT'] = sign_cert
-        command = f'c2patool {asset_file} -m {manifest_temp_file.name} -o {c2pa_output_file}'
-        if force_overwrite:
-            command += ' -f'
-        try:
-            subprocess.run(
-                command,
-                shell=True,
-                env=env_vars,
-                check=True,
-                stderr=subprocess.PIPE,
-            )
-        except subprocess.CalledProcessError as e:
-            raise UnknownError(e.stderr)
+        c2patool_inject(
+            asset_file,
+            manifest_temp_file.name,
+            c2pa_output_file,
+            force_overwrite=force_overwrite,
+            private_key=private_key,
+            sign_cert=sign_cert,
+        )
 
 
 def read_c2pa(asset_c2pa_bytes: bytes, asset_mime_type: str):
     file_ext = _mimetype_to_ext(asset_mime_type)
     with TemporaryDirectory(prefix='temp_dir') as temp_dir:
         asset_c2pa_file = os.path.join(temp_dir, f'asset-c2pa.{file_ext}')
         with open(asset_c2pa_file, 'wb') as f:
```

### Comparing `numbers-c2pa-0.0.6/src/numbers_c2pa/utils.py` & `numbers-c2pa-0.0.7/src/numbers_c2pa/utils.py`

 * *Files identical despite different names*

### Comparing `numbers-c2pa-0.0.6/src/numbers_c2pa.egg-info/PKG-INFO` & `numbers-c2pa-0.0.7/src/numbers_c2pa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numbers-c2pa
-Version: 0.0.6
+Version: 0.0.7
 Summary: Numbers C2PA tool
 Home-page: https://github.com/numbersprotocol/numbers-c2pa
 Author: Numbers Co., Inc
 Author-email: dev@numbersprotocol.io
 Keywords: authenticity
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

