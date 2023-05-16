# Comparing `tmp/dpapi-ng-0.1.0.tar.gz` & `tmp/dpapi-ng-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dpapi-ng-0.1.0.tar", last modified: Tue May  9 06:33:39 2023, max compression
+gzip compressed data, was "dpapi-ng-0.1.1.tar", last modified: Tue May 16 06:10:28 2023, max compression
```

## Comparing `dpapi-ng-0.1.0.tar` & `dpapi-ng-0.1.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:33:39.871078 dpapi-ng-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-09 06:33:30.000000 dpapi-ng-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9887 2023-05-09 06:33:39.871078 dpapi-ng-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7892 2023-05-09 06:33:30.000000 dpapi-ng-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-05-09 06:33:30.000000 dpapi-ng-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 06:33:39.871078 dpapi-ng-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:33:39.859078 dpapi-ng-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:33:39.871078 dpapi-ng-0.1.0/src/dpapi_ng/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-09 06:33:30.000000 dpapi-ng-0.1.0/src/dpapi_ng/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31807 2023-05-09 06:33:30.000000 dpapi-ng-0.1.0/src/dpapi_ng/_asn1.py
--rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-05-09 06:33:30.000000 dpapi-ng-0.1.0/src/dpapi_ng/_blob.py
--rw-r--r--   0 runner    (1001) docker     (123)    20642 2023-05-09 06:33:30.000000 dpapi-ng-0.1.0/src/dpapi_ng/_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-05-09 06:33:30.000000 dpapi-ng-0.1.0/src/dpapi_ng/_crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-05-09 06:33:30.000000 dpapi-ng-0.1.0/src/dpapi_ng/_dns.py
--rw-r--r--   0 runner    (1001) docker     (123)    12183 2023-05-09 06:33:30.000000 dpapi-ng-0.1.0/src/dpapi_ng/_epm.py
--rw-r--r--   0 runner    (1001) docker     (123)    26887 2023-05-09 06:33:30.000000 dpapi-ng-0.1.0/src/dpapi_ng/_gkdi.py
--rw-r--r--   0 runner    (1001) docker     (123)     9837 2023-05-09 06:33:30.000000 dpapi-ng-0.1.0/src/dpapi_ng/_pkcs7.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:33:39.871078 dpapi-ng-0.1.0/src/dpapi_ng/_rpc/
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-05-09 06:33:30.000000 dpapi-ng-0.1.0/src/dpapi_ng/_rpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-05-09 06:33:30.000000 dpapi-ng-0.1.0/src/dpapi_ng/_rpc/_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    10502 2023-05-09 06:33:30.000000 dpapi-ng-0.1.0/src/dpapi_ng/_rpc/_bind.py
--rw-r--r--   0 runner    (1001) docker     (123)    13871 2023-05-09 06:33:30.000000 dpapi-ng-0.1.0/src/dpapi_ng/_rpc/_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8031 2023-05-09 06:33:30.000000 dpapi-ng-0.1.0/src/dpapi_ng/_rpc/_pdu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-05-09 06:33:30.000000 dpapi-ng-0.1.0/src/dpapi_ng/_rpc/_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-05-09 06:33:30.000000 dpapi-ng-0.1.0/src/dpapi_ng/_rpc/_verification.py
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-05-09 06:33:30.000000 dpapi-ng-0.1.0/src/dpapi_ng/_security_descriptor.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-09 06:33:30.000000 dpapi-ng-0.1.0/src/dpapi_ng/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:33:39.871078 dpapi-ng-0.1.0/src/dpapi_ng.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9887 2023-05-09 06:33:39.000000 dpapi-ng-0.1.0/src/dpapi_ng.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-09 06:33:39.000000 dpapi-ng-0.1.0/src/dpapi_ng.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 06:33:39.000000 dpapi-ng-0.1.0/src/dpapi_ng.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-09 06:33:39.000000 dpapi-ng-0.1.0/src/dpapi_ng.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-09 06:33:39.000000 dpapi-ng-0.1.0/src/dpapi_ng.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:33:39.871078 dpapi-ng-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    11991 2023-05-09 06:33:30.000000 dpapi-ng-0.1.0/tests/test_asn1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-09 06:33:30.000000 dpapi-ng-0.1.0/tests/test_blob.py
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-05-09 06:33:30.000000 dpapi-ng-0.1.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-09 06:33:30.000000 dpapi-ng-0.1.0/tests/test_crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)    13182 2023-05-09 06:33:30.000000 dpapi-ng-0.1.0/tests/test_epm.py
--rw-r--r--   0 runner    (1001) docker     (123)    23716 2023-05-09 06:33:30.000000 dpapi-ng-0.1.0/tests/test_gkdi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-05-09 06:33:30.000000 dpapi-ng-0.1.0/tests/test_security_descriptor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:10:28.346913 dpapi-ng-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-16 06:10:20.000000 dpapi-ng-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9887 2023-05-16 06:10:28.346913 dpapi-ng-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7892 2023-05-16 06:10:20.000000 dpapi-ng-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-05-16 06:10:20.000000 dpapi-ng-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 06:10:28.346913 dpapi-ng-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:10:28.342913 dpapi-ng-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:10:28.342913 dpapi-ng-0.1.1/src/dpapi_ng/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-16 06:10:20.000000 dpapi-ng-0.1.1/src/dpapi_ng/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31807 2023-05-16 06:10:20.000000 dpapi-ng-0.1.1/src/dpapi_ng/_asn1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-05-16 06:10:20.000000 dpapi-ng-0.1.1/src/dpapi_ng/_blob.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20700 2023-05-16 06:10:20.000000 dpapi-ng-0.1.1/src/dpapi_ng/_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-05-16 06:10:20.000000 dpapi-ng-0.1.1/src/dpapi_ng/_crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-05-16 06:10:20.000000 dpapi-ng-0.1.1/src/dpapi_ng/_dns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12183 2023-05-16 06:10:20.000000 dpapi-ng-0.1.1/src/dpapi_ng/_epm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26887 2023-05-16 06:10:20.000000 dpapi-ng-0.1.1/src/dpapi_ng/_gkdi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9837 2023-05-16 06:10:20.000000 dpapi-ng-0.1.1/src/dpapi_ng/_pkcs7.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:10:28.346913 dpapi-ng-0.1.1/src/dpapi_ng/_rpc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-05-16 06:10:20.000000 dpapi-ng-0.1.1/src/dpapi_ng/_rpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-05-16 06:10:20.000000 dpapi-ng-0.1.1/src/dpapi_ng/_rpc/_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10502 2023-05-16 06:10:20.000000 dpapi-ng-0.1.1/src/dpapi_ng/_rpc/_bind.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13871 2023-05-16 06:10:20.000000 dpapi-ng-0.1.1/src/dpapi_ng/_rpc/_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8031 2023-05-16 06:10:20.000000 dpapi-ng-0.1.1/src/dpapi_ng/_rpc/_pdu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-05-16 06:10:20.000000 dpapi-ng-0.1.1/src/dpapi_ng/_rpc/_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-05-16 06:10:20.000000 dpapi-ng-0.1.1/src/dpapi_ng/_rpc/_verification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-05-16 06:10:20.000000 dpapi-ng-0.1.1/src/dpapi_ng/_security_descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-16 06:10:20.000000 dpapi-ng-0.1.1/src/dpapi_ng/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:10:28.342913 dpapi-ng-0.1.1/src/dpapi_ng.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9887 2023-05-16 06:10:28.000000 dpapi-ng-0.1.1/src/dpapi_ng.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-16 06:10:28.000000 dpapi-ng-0.1.1/src/dpapi_ng.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 06:10:28.000000 dpapi-ng-0.1.1/src/dpapi_ng.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-16 06:10:28.000000 dpapi-ng-0.1.1/src/dpapi_ng.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-16 06:10:28.000000 dpapi-ng-0.1.1/src/dpapi_ng.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:10:28.346913 dpapi-ng-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    11991 2023-05-16 06:10:20.000000 dpapi-ng-0.1.1/tests/test_asn1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-16 06:10:20.000000 dpapi-ng-0.1.1/tests/test_blob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-05-16 06:10:20.000000 dpapi-ng-0.1.1/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-16 06:10:20.000000 dpapi-ng-0.1.1/tests/test_crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13182 2023-05-16 06:10:20.000000 dpapi-ng-0.1.1/tests/test_epm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23716 2023-05-16 06:10:20.000000 dpapi-ng-0.1.1/tests/test_gkdi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-05-16 06:10:20.000000 dpapi-ng-0.1.1/tests/test_security_descriptor.py
```

### Comparing `dpapi-ng-0.1.0/LICENSE` & `dpapi-ng-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dpapi-ng-0.1.0/PKG-INFO` & `dpapi-ng-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpapi-ng
-Version: 0.1.0
+Version: 0.1.1
 Summary: DPAPI NG decryption for Python
 Author-email: Jordan Borean <jborean93@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Jordan Borean, Red Hat
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dpapi-ng-0.1.0/README.md` & `dpapi-ng-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `dpapi-ng-0.1.0/pyproject.toml` & `dpapi-ng-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dpapi-ng-0.1.0/src/dpapi_ng/_asn1.py` & `dpapi-ng-0.1.1/src/dpapi_ng/_asn1.py`

 * *Files identical despite different names*

### Comparing `dpapi-ng-0.1.0/src/dpapi_ng/_blob.py` & `dpapi-ng-0.1.1/src/dpapi_ng/_blob.py`

 * *Files identical despite different names*

### Comparing `dpapi-ng-0.1.0/src/dpapi_ng/_client.py` & `dpapi-ng-0.1.1/src/dpapi_ng/_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,18 +108,18 @@
 
     raise ValueError("Did not find expected TCP Port in ept_map response")
 
 
 def _process_get_key_result(
     response: Response,
 ) -> GroupKeyEnvelope:
-    pad_length = 0
-    if response.sec_trailer:
-        pad_length = response.sec_trailer.pad_length
-    raw_resp = response.stub_data[:-pad_length]
+    pad_length = len(response.stub_data)
+    if response.sec_trailer and response.sec_trailer.pad_length:
+        pad_length -= response.sec_trailer.pad_length
+    raw_resp = response.stub_data[:pad_length]
     return GetKey.unpack_response(raw_resp)
 
 
 async def _async_get_key(
     server: str,
     target_sd: bytes,
     root_key_id: t.Optional[uuid.UUID],
```

### Comparing `dpapi-ng-0.1.0/src/dpapi_ng/_crypto.py` & `dpapi-ng-0.1.1/src/dpapi_ng/_crypto.py`

 * *Files identical despite different names*

### Comparing `dpapi-ng-0.1.0/src/dpapi_ng/_dns.py` & `dpapi-ng-0.1.1/src/dpapi_ng/_dns.py`

 * *Files identical despite different names*

### Comparing `dpapi-ng-0.1.0/src/dpapi_ng/_epm.py` & `dpapi-ng-0.1.1/src/dpapi_ng/_epm.py`

 * *Files identical despite different names*

### Comparing `dpapi-ng-0.1.0/src/dpapi_ng/_gkdi.py` & `dpapi-ng-0.1.1/src/dpapi_ng/_gkdi.py`

 * *Files identical despite different names*

### Comparing `dpapi-ng-0.1.0/src/dpapi_ng/_pkcs7.py` & `dpapi-ng-0.1.1/src/dpapi_ng/_pkcs7.py`

 * *Files identical despite different names*

### Comparing `dpapi-ng-0.1.0/src/dpapi_ng/_rpc/__init__.py` & `dpapi-ng-0.1.1/src/dpapi_ng/_rpc/__init__.py`

 * *Files identical despite different names*

### Comparing `dpapi-ng-0.1.0/src/dpapi_ng/_rpc/_auth.py` & `dpapi-ng-0.1.1/src/dpapi_ng/_rpc/_auth.py`

 * *Files identical despite different names*

### Comparing `dpapi-ng-0.1.0/src/dpapi_ng/_rpc/_bind.py` & `dpapi-ng-0.1.1/src/dpapi_ng/_rpc/_bind.py`

 * *Files identical despite different names*

### Comparing `dpapi-ng-0.1.0/src/dpapi_ng/_rpc/_client.py` & `dpapi-ng-0.1.1/src/dpapi_ng/_rpc/_client.py`

 * *Files identical despite different names*

### Comparing `dpapi-ng-0.1.0/src/dpapi_ng/_rpc/_pdu.py` & `dpapi-ng-0.1.1/src/dpapi_ng/_rpc/_pdu.py`

 * *Files identical despite different names*

### Comparing `dpapi-ng-0.1.0/src/dpapi_ng/_rpc/_request.py` & `dpapi-ng-0.1.1/src/dpapi_ng/_rpc/_request.py`

 * *Files identical despite different names*

### Comparing `dpapi-ng-0.1.0/src/dpapi_ng/_rpc/_verification.py` & `dpapi-ng-0.1.1/src/dpapi_ng/_rpc/_verification.py`

 * *Files identical despite different names*

### Comparing `dpapi-ng-0.1.0/src/dpapi_ng/_security_descriptor.py` & `dpapi-ng-0.1.1/src/dpapi_ng/_security_descriptor.py`

 * *Files identical despite different names*

### Comparing `dpapi-ng-0.1.0/src/dpapi_ng.egg-info/PKG-INFO` & `dpapi-ng-0.1.1/src/dpapi_ng.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpapi-ng
-Version: 0.1.0
+Version: 0.1.1
 Summary: DPAPI NG decryption for Python
 Author-email: Jordan Borean <jborean93@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Jordan Borean, Red Hat
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dpapi-ng-0.1.0/src/dpapi_ng.egg-info/SOURCES.txt` & `dpapi-ng-0.1.1/src/dpapi_ng.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dpapi-ng-0.1.0/tests/test_asn1.py` & `dpapi-ng-0.1.1/tests/test_asn1.py`

 * *Files identical despite different names*

### Comparing `dpapi-ng-0.1.0/tests/test_blob.py` & `dpapi-ng-0.1.1/tests/test_blob.py`

 * *Files identical despite different names*

### Comparing `dpapi-ng-0.1.0/tests/test_client.py` & `dpapi-ng-0.1.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `dpapi-ng-0.1.0/tests/test_crypto.py` & `dpapi-ng-0.1.1/tests/test_crypto.py`

 * *Files identical despite different names*

### Comparing `dpapi-ng-0.1.0/tests/test_epm.py` & `dpapi-ng-0.1.1/tests/test_epm.py`

 * *Files identical despite different names*

### Comparing `dpapi-ng-0.1.0/tests/test_gkdi.py` & `dpapi-ng-0.1.1/tests/test_gkdi.py`

 * *Files identical despite different names*

### Comparing `dpapi-ng-0.1.0/tests/test_security_descriptor.py` & `dpapi-ng-0.1.1/tests/test_security_descriptor.py`

 * *Files identical despite different names*

