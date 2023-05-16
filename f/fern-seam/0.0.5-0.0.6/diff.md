# Comparing `tmp/fern_seam-0.0.5.tar.gz` & `tmp/fern_seam-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fern_seam-0.0.5.tar", max compression
+gzip compressed data, was "fern_seam-0.0.6.tar", max compression
```

## Comparing `fern_seam-0.0.5.tar` & `fern_seam-0.0.6.tar`

### file list

```diff
@@ -1,37 +1,38 @@
--rw-r--r--   0        0        0     1630 2023-05-16 04:37:19.978061 fern_seam-0.0.5/README.md
--rw-r--r--   0        0        0      368 2023-05-16 04:37:19.978061 fern_seam-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      913 2023-05-16 04:37:19.978061 fern_seam-0.0.5/src/seam/__init__.py
--rw-r--r--   0        0        0     1056 2023-05-16 04:37:19.978061 fern_seam-0.0.5/src/seam/base_client.py
--rw-r--r--   0        0        0      348 2023-05-16 04:37:19.978061 fern_seam-0.0.5/src/seam/core/__init__.py
--rw-r--r--   0        0        0      426 2023-05-16 04:37:19.978061 fern_seam-0.0.5/src/seam/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-05-16 04:37:19.978061 fern_seam-0.0.5/src/seam/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-05-16 04:37:19.978061 fern_seam-0.0.5/src/seam/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-05-16 04:37:19.978061 fern_seam-0.0.5/src/seam/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      160 2023-05-16 04:37:19.978061 fern_seam-0.0.5/src/seam/environment.py
--rw-r--r--   0        0        0        0 2023-05-16 04:37:19.978061 fern_seam-0.0.5/src/seam/py.typed
--rw-r--r--   0        0        0      889 2023-05-16 04:37:19.978061 fern_seam-0.0.5/src/seam/resources/__init__.py
--rw-r--r--   0        0        0      437 2023-05-16 04:37:19.978061 fern_seam-0.0.5/src/seam/resources/access_codes/__init__.py
--rw-r--r--   0        0        0     9385 2023-05-16 04:37:19.978061 fern_seam-0.0.5/src/seam/resources/access_codes/client.py
--rw-r--r--   0        0        0      610 2023-05-16 04:37:19.978061 fern_seam-0.0.5/src/seam/resources/access_codes/types/__init__.py
--rw-r--r--   0        0        0     1871 2023-05-16 04:37:19.978061 fern_seam-0.0.5/src/seam/resources/access_codes/types/access_code.py
--rw-r--r--   0        0        0      782 2023-05-16 04:37:19.978061 fern_seam-0.0.5/src/seam/resources/access_codes/types/access_code_error.py
--rw-r--r--   0        0        0      103 2023-05-16 04:37:19.978061 fern_seam-0.0.5/src/seam/resources/access_codes/types/access_code_id.py
--rw-r--r--   0        0        0     1002 2023-05-16 04:37:19.978061 fern_seam-0.0.5/src/seam/resources/access_codes/types/access_code_status.py
--rw-r--r--   0        0        0      784 2023-05-16 04:37:19.978061 fern_seam-0.0.5/src/seam/resources/access_codes/types/access_code_warning.py
--rw-r--r--   0        0        0      910 2023-05-16 04:37:19.978061 fern_seam-0.0.5/src/seam/resources/access_codes/types/create_access_code_response.py
--rw-r--r--   0        0        0      846 2023-05-16 04:37:19.978061 fern_seam-0.0.5/src/seam/resources/access_codes/types/update_access_code_response.py
--rw-r--r--   0        0        0      219 2023-05-16 04:37:19.978061 fern_seam-0.0.5/src/seam/resources/action_attempts/__init__.py
--rw-r--r--   0        0        0     2718 2023-05-16 04:37:19.978061 fern_seam-0.0.5/src/seam/resources/action_attempts/client.py
--rw-r--r--   0        0        0      308 2023-05-16 04:37:19.978061 fern_seam-0.0.5/src/seam/resources/action_attempts/types/__init__.py
--rw-r--r--   0        0        0      995 2023-05-16 04:37:19.978061 fern_seam-0.0.5/src/seam/resources/action_attempts/types/action_attempt.py
--rw-r--r--   0        0        0      106 2023-05-16 04:37:19.978061 fern_seam-0.0.5/src/seam/resources/action_attempts/types/action_attempt_id.py
--rw-r--r--   0        0        0      633 2023-05-16 04:37:19.978061 fern_seam-0.0.5/src/seam/resources/action_attempts/types/action_status.py
--rw-r--r--   0        0        0     1150 2023-05-16 04:37:19.978061 fern_seam-0.0.5/src/seam/resources/action_attempts/types/action_type.py
--rw-r--r--   0        0        0      164 2023-05-16 04:37:19.978061 fern_seam-0.0.5/src/seam/resources/commons/__init__.py
--rw-r--r--   0        0        0      203 2023-05-16 04:37:19.978061 fern_seam-0.0.5/src/seam/resources/commons/errors/__init__.py
--rw-r--r--   0        0        0      250 2023-05-16 04:37:19.978061 fern_seam-0.0.5/src/seam/resources/commons/errors/bad_request_error.py
--rw-r--r--   0        0        0      248 2023-05-16 04:37:19.978061 fern_seam-0.0.5/src/seam/resources/commons/errors/not_found_error.py
--rw-r--r--   0        0        0      117 2023-05-16 04:37:19.978061 fern_seam-0.0.5/src/seam/resources/devices/__init__.py
--rw-r--r--   0        0        0      121 2023-05-16 04:37:19.978061 fern_seam-0.0.5/src/seam/resources/devices/types/__init__.py
--rw-r--r--   0        0        0       99 2023-05-16 04:37:19.978061 fern_seam-0.0.5/src/seam/resources/devices/types/device_id.py
--rw-r--r--   0        0        0     2136 1970-01-01 00:00:00.000000 fern_seam-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1630 2023-05-16 04:54:16.203045 fern_seam-0.0.6/README.md
+-rw-r--r--   0        0        0      368 2023-05-16 04:54:16.203045 fern_seam-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      913 2023-05-16 04:54:16.203045 fern_seam-0.0.6/src/seam/__init__.py
+-rw-r--r--   0        0        0     1056 2023-05-16 04:54:16.203045 fern_seam-0.0.6/src/seam/base_client.py
+-rw-r--r--   0        0        0     3432 2023-05-16 04:54:16.203045 fern_seam-0.0.6/src/seam/client.py
+-rw-r--r--   0        0        0      348 2023-05-16 04:54:16.203045 fern_seam-0.0.6/src/seam/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-05-16 04:54:16.203045 fern_seam-0.0.6/src/seam/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-05-16 04:54:16.203045 fern_seam-0.0.6/src/seam/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-05-16 04:54:16.203045 fern_seam-0.0.6/src/seam/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-05-16 04:54:16.203045 fern_seam-0.0.6/src/seam/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      160 2023-05-16 04:54:16.203045 fern_seam-0.0.6/src/seam/environment.py
+-rw-r--r--   0        0        0        0 2023-05-16 04:54:16.203045 fern_seam-0.0.6/src/seam/py.typed
+-rw-r--r--   0        0        0      889 2023-05-16 04:54:16.203045 fern_seam-0.0.6/src/seam/resources/__init__.py
+-rw-r--r--   0        0        0      437 2023-05-16 04:54:16.203045 fern_seam-0.0.6/src/seam/resources/access_codes/__init__.py
+-rw-r--r--   0        0        0     9385 2023-05-16 04:54:16.203045 fern_seam-0.0.6/src/seam/resources/access_codes/client.py
+-rw-r--r--   0        0        0      610 2023-05-16 04:54:16.203045 fern_seam-0.0.6/src/seam/resources/access_codes/types/__init__.py
+-rw-r--r--   0        0        0     1871 2023-05-16 04:54:16.203045 fern_seam-0.0.6/src/seam/resources/access_codes/types/access_code.py
+-rw-r--r--   0        0        0      782 2023-05-16 04:54:16.203045 fern_seam-0.0.6/src/seam/resources/access_codes/types/access_code_error.py
+-rw-r--r--   0        0        0      103 2023-05-16 04:54:16.203045 fern_seam-0.0.6/src/seam/resources/access_codes/types/access_code_id.py
+-rw-r--r--   0        0        0     1002 2023-05-16 04:54:16.203045 fern_seam-0.0.6/src/seam/resources/access_codes/types/access_code_status.py
+-rw-r--r--   0        0        0      784 2023-05-16 04:54:16.203045 fern_seam-0.0.6/src/seam/resources/access_codes/types/access_code_warning.py
+-rw-r--r--   0        0        0      910 2023-05-16 04:54:16.203045 fern_seam-0.0.6/src/seam/resources/access_codes/types/create_access_code_response.py
+-rw-r--r--   0        0        0      846 2023-05-16 04:54:16.203045 fern_seam-0.0.6/src/seam/resources/access_codes/types/update_access_code_response.py
+-rw-r--r--   0        0        0      219 2023-05-16 04:54:16.203045 fern_seam-0.0.6/src/seam/resources/action_attempts/__init__.py
+-rw-r--r--   0        0        0     2718 2023-05-16 04:54:16.203045 fern_seam-0.0.6/src/seam/resources/action_attempts/client.py
+-rw-r--r--   0        0        0      308 2023-05-16 04:54:16.203045 fern_seam-0.0.6/src/seam/resources/action_attempts/types/__init__.py
+-rw-r--r--   0        0        0      995 2023-05-16 04:54:16.203045 fern_seam-0.0.6/src/seam/resources/action_attempts/types/action_attempt.py
+-rw-r--r--   0        0        0      106 2023-05-16 04:54:16.203045 fern_seam-0.0.6/src/seam/resources/action_attempts/types/action_attempt_id.py
+-rw-r--r--   0        0        0      633 2023-05-16 04:54:16.203045 fern_seam-0.0.6/src/seam/resources/action_attempts/types/action_status.py
+-rw-r--r--   0        0        0     1150 2023-05-16 04:54:16.203045 fern_seam-0.0.6/src/seam/resources/action_attempts/types/action_type.py
+-rw-r--r--   0        0        0      164 2023-05-16 04:54:16.203045 fern_seam-0.0.6/src/seam/resources/commons/__init__.py
+-rw-r--r--   0        0        0      203 2023-05-16 04:54:16.203045 fern_seam-0.0.6/src/seam/resources/commons/errors/__init__.py
+-rw-r--r--   0        0        0      250 2023-05-16 04:54:16.203045 fern_seam-0.0.6/src/seam/resources/commons/errors/bad_request_error.py
+-rw-r--r--   0        0        0      248 2023-05-16 04:54:16.203045 fern_seam-0.0.6/src/seam/resources/commons/errors/not_found_error.py
+-rw-r--r--   0        0        0      117 2023-05-16 04:54:16.203045 fern_seam-0.0.6/src/seam/resources/devices/__init__.py
+-rw-r--r--   0        0        0      121 2023-05-16 04:54:16.207045 fern_seam-0.0.6/src/seam/resources/devices/types/__init__.py
+-rw-r--r--   0        0        0       99 2023-05-16 04:54:16.207045 fern_seam-0.0.6/src/seam/resources/devices/types/device_id.py
+-rw-r--r--   0        0        0     2136 1970-01-01 00:00:00.000000 fern_seam-0.0.6/PKG-INFO
```

### Comparing `fern_seam-0.0.5/README.md` & `fern_seam-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `fern_seam-0.0.5/src/seam/__init__.py` & `fern_seam-0.0.6/src/seam/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_seam-0.0.5/src/seam/base_client.py` & `fern_seam-0.0.6/src/seam/base_client.py`

 * *Files identical despite different names*

### Comparing `fern_seam-0.0.5/src/seam/core/datetime_utils.py` & `fern_seam-0.0.6/src/seam/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `fern_seam-0.0.5/src/seam/core/jsonable_encoder.py` & `fern_seam-0.0.6/src/seam/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `fern_seam-0.0.5/src/seam/resources/__init__.py` & `fern_seam-0.0.6/src/seam/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_seam-0.0.5/src/seam/resources/access_codes/client.py` & `fern_seam-0.0.6/src/seam/resources/access_codes/client.py`

 * *Files identical despite different names*

### Comparing `fern_seam-0.0.5/src/seam/resources/access_codes/types/__init__.py` & `fern_seam-0.0.6/src/seam/resources/access_codes/types/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_seam-0.0.5/src/seam/resources/access_codes/types/access_code.py` & `fern_seam-0.0.6/src/seam/resources/access_codes/types/access_code.py`

 * *Files identical despite different names*

### Comparing `fern_seam-0.0.5/src/seam/resources/access_codes/types/access_code_error.py` & `fern_seam-0.0.6/src/seam/resources/access_codes/types/access_code_error.py`

 * *Files identical despite different names*

### Comparing `fern_seam-0.0.5/src/seam/resources/access_codes/types/access_code_status.py` & `fern_seam-0.0.6/src/seam/resources/access_codes/types/access_code_status.py`

 * *Files identical despite different names*

### Comparing `fern_seam-0.0.5/src/seam/resources/access_codes/types/access_code_warning.py` & `fern_seam-0.0.6/src/seam/resources/access_codes/types/access_code_warning.py`

 * *Files identical despite different names*

### Comparing `fern_seam-0.0.5/src/seam/resources/access_codes/types/create_access_code_response.py` & `fern_seam-0.0.6/src/seam/resources/access_codes/types/create_access_code_response.py`

 * *Files identical despite different names*

### Comparing `fern_seam-0.0.5/src/seam/resources/access_codes/types/update_access_code_response.py` & `fern_seam-0.0.6/src/seam/resources/access_codes/types/update_access_code_response.py`

 * *Files identical despite different names*

### Comparing `fern_seam-0.0.5/src/seam/resources/action_attempts/client.py` & `fern_seam-0.0.6/src/seam/resources/action_attempts/client.py`

 * *Files identical despite different names*

### Comparing `fern_seam-0.0.5/src/seam/resources/action_attempts/types/action_attempt.py` & `fern_seam-0.0.6/src/seam/resources/action_attempts/types/action_attempt.py`

 * *Files identical despite different names*

### Comparing `fern_seam-0.0.5/src/seam/resources/action_attempts/types/action_status.py` & `fern_seam-0.0.6/src/seam/resources/action_attempts/types/action_status.py`

 * *Files identical despite different names*

### Comparing `fern_seam-0.0.5/src/seam/resources/action_attempts/types/action_type.py` & `fern_seam-0.0.6/src/seam/resources/action_attempts/types/action_type.py`

 * *Files identical despite different names*

### Comparing `fern_seam-0.0.5/PKG-INFO` & `fern_seam-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fern-seam
-Version: 0.0.5
+Version: 0.0.6
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

