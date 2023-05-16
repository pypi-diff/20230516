# Comparing `tmp/edx-enterprise-subsidy-client-0.3.1.tar.gz` & `tmp/edx-enterprise-subsidy-client-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-enterprise-subsidy-client-0.3.1.tar", last modified: Mon May  1 19:26:27 2023, max compression
+gzip compressed data, was "edx-enterprise-subsidy-client-0.3.2.tar", last modified: Tue May 16 20:19:17 2023, max compression
```

## Comparing `edx-enterprise-subsidy-client-0.3.1.tar` & `edx-enterprise-subsidy-client-0.3.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 19:26:27.352352 edx-enterprise-subsidy-client-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (122)     1508 2023-05-01 19:26:22.000000 edx-enterprise-subsidy-client-0.3.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    34523 2023-05-01 19:26:22.000000 edx-enterprise-subsidy-client-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-05-01 19:26:22.000000 edx-enterprise-subsidy-client-0.3.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      224 2023-05-01 19:26:22.000000 edx-enterprise-subsidy-client-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     8532 2023-05-01 19:26:27.352352 edx-enterprise-subsidy-client-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6341 2023-05-01 19:26:22.000000 edx-enterprise-subsidy-client-0.3.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 19:26:27.348353 edx-enterprise-subsidy-client-0.3.1/edx_enterprise_subsidy_client/
--rw-r--r--   0 runner    (1001) docker     (122)      175 2023-05-01 19:26:22.000000 edx-enterprise-subsidy-client-0.3.1/edx_enterprise_subsidy_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9747 2023-05-01 19:26:22.000000 edx-enterprise-subsidy-client-0.3.1/edx_enterprise_subsidy_client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 19:26:27.352352 edx-enterprise-subsidy-client-0.3.1/edx_enterprise_subsidy_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     8532 2023-05-01 19:26:27.000000 edx-enterprise-subsidy-client-0.3.1/edx_enterprise_subsidy_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      544 2023-05-01 19:26:27.000000 edx-enterprise-subsidy-client-0.3.1/edx_enterprise_subsidy_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-01 19:26:27.000000 edx-enterprise-subsidy-client-0.3.1/edx_enterprise_subsidy_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-01 19:26:27.000000 edx-enterprise-subsidy-client-0.3.1/edx_enterprise_subsidy_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-05-01 19:26:27.000000 edx-enterprise-subsidy-client-0.3.1/edx_enterprise_subsidy_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-05-01 19:26:27.000000 edx-enterprise-subsidy-client-0.3.1/edx_enterprise_subsidy_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 19:26:27.352352 edx-enterprise-subsidy-client-0.3.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)       86 2023-05-01 19:26:22.000000 edx-enterprise-subsidy-client-0.3.1/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      561 2023-05-01 19:26:22.000000 edx-enterprise-subsidy-client-0.3.1/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      208 2023-05-01 19:26:27.352352 edx-enterprise-subsidy-client-0.3.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     5111 2023-05-01 19:26:22.000000 edx-enterprise-subsidy-client-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 19:26:27.352352 edx-enterprise-subsidy-client-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     1257 2023-05-01 19:26:22.000000 edx-enterprise-subsidy-client-0.3.1/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 20:19:17.794512 edx-enterprise-subsidy-client-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (122)     1699 2023-05-16 20:19:13.000000 edx-enterprise-subsidy-client-0.3.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    34523 2023-05-16 20:19:13.000000 edx-enterprise-subsidy-client-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-05-16 20:19:13.000000 edx-enterprise-subsidy-client-0.3.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      224 2023-05-16 20:19:13.000000 edx-enterprise-subsidy-client-0.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     8723 2023-05-16 20:19:17.794512 edx-enterprise-subsidy-client-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6341 2023-05-16 20:19:13.000000 edx-enterprise-subsidy-client-0.3.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 20:19:17.794512 edx-enterprise-subsidy-client-0.3.2/edx_enterprise_subsidy_client/
+-rw-r--r--   0 runner    (1001) docker     (122)      205 2023-05-16 20:19:13.000000 edx-enterprise-subsidy-client-0.3.2/edx_enterprise_subsidy_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10408 2023-05-16 20:19:13.000000 edx-enterprise-subsidy-client-0.3.2/edx_enterprise_subsidy_client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 20:19:17.794512 edx-enterprise-subsidy-client-0.3.2/edx_enterprise_subsidy_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8723 2023-05-16 20:19:17.000000 edx-enterprise-subsidy-client-0.3.2/edx_enterprise_subsidy_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      544 2023-05-16 20:19:17.000000 edx-enterprise-subsidy-client-0.3.2/edx_enterprise_subsidy_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-16 20:19:17.000000 edx-enterprise-subsidy-client-0.3.2/edx_enterprise_subsidy_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-16 20:19:17.000000 edx-enterprise-subsidy-client-0.3.2/edx_enterprise_subsidy_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-05-16 20:19:17.000000 edx-enterprise-subsidy-client-0.3.2/edx_enterprise_subsidy_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-05-16 20:19:17.000000 edx-enterprise-subsidy-client-0.3.2/edx_enterprise_subsidy_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 20:19:17.794512 edx-enterprise-subsidy-client-0.3.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)       86 2023-05-16 20:19:13.000000 edx-enterprise-subsidy-client-0.3.2/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-05-16 20:19:13.000000 edx-enterprise-subsidy-client-0.3.2/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      208 2023-05-16 20:19:17.794512 edx-enterprise-subsidy-client-0.3.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5111 2023-05-16 20:19:13.000000 edx-enterprise-subsidy-client-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 20:19:17.794512 edx-enterprise-subsidy-client-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     2832 2023-05-16 20:19:13.000000 edx-enterprise-subsidy-client-0.3.2/tests/test_client.py
```

### Comparing `edx-enterprise-subsidy-client-0.3.1/CHANGELOG.rst` & `edx-enterprise-subsidy-client-0.3.2/CHANGELOG.rst`

 * *Files 16% similar despite different names*

```diff
@@ -13,14 +13,19 @@
 
 Unreleased
 **********
 
 * Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
   deprecated
 
+[0.3.2]
+*******
+* admin-list transactions will ask to be filtered for only `committed` and `pending` states by default.
+  Caller may specify other valid states (e.g. `failed` or `created`).
+
 [0.3.1]
 *******
 * fix: correctly pass ``subsidy_uuid`` to subsidy API V2 endpoint string format.
 
 [0.3.0]
 *******
 * feat: add new client for v2 transaction endpoint.
```

### Comparing `edx-enterprise-subsidy-client-0.3.1/LICENSE` & `edx-enterprise-subsidy-client-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `edx-enterprise-subsidy-client-0.3.1/LICENSE.txt` & `edx-enterprise-subsidy-client-0.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-subsidy-client-0.3.1/PKG-INFO` & `edx-enterprise-subsidy-client-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-enterprise-subsidy-client
-Version: 0.3.1
+Version: 0.3.2
 Summary: Client for interacting with the enterprise-subsidy service.
 Home-page: https://github.com/openedx/edx-enterprise-subsidy-client
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -223,14 +223,19 @@
 
 Unreleased
 **********
 
 * Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
   deprecated
 
+[0.3.2]
+*******
+* admin-list transactions will ask to be filtered for only `committed` and `pending` states by default.
+  Caller may specify other valid states (e.g. `failed` or `created`).
+
 [0.3.1]
 *******
 * fix: correctly pass ``subsidy_uuid`` to subsidy API V2 endpoint string format.
 
 [0.3.0]
 *******
 * feat: add new client for v2 transaction endpoint.
```

### Comparing `edx-enterprise-subsidy-client-0.3.1/README.rst` & `edx-enterprise-subsidy-client-0.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `edx-enterprise-subsidy-client-0.3.1/edx_enterprise_subsidy_client/client.py` & `edx-enterprise-subsidy-client-0.3.2/edx_enterprise_subsidy_client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,32 @@
 import requests
 from django.conf import settings
 from edx_rest_api_client.client import OAuthAPIClient
 
 logger = logging.getLogger(__name__)
 
 
+class TransactionStateChoices:
+    """
+    Lifecycle states for a ledger transaction.
+    """
+
+    CREATED = 'created'
+    PENDING = 'pending'
+    COMMITTED = 'committed'
+    FAILED = 'failed'
+
+    VALID_CHOICES = {
+        CREATED,
+        PENDING,
+        COMMITTED,
+        FAILED,
+    }
+
+
 class EnterpriseSubsidyAPIClientException(Exception):
     """
     A general exception to represent non-http errors
     arising during Subsidy API client usage.
     """
 
 
@@ -224,28 +242,36 @@
     """
     V2_BASE_URL = EnterpriseSubsidyAPIClient.API_BASE_URL + 'v2/'
     TRANSACTIONS_LIST_ENDPOINT = V2_BASE_URL + 'subsidies/{subsidy_uuid}/admin/transactions/'
 
     def list_subsidy_transactions(
         self, subsidy_uuid, include_aggregates=True,
         lms_user_id=None, content_key=None,
-        subsidy_access_policy_uuid=None,
+        subsidy_access_policy_uuid=None, transaction_states=None,
     ):
         """
         List transactions in a subsidy with admin- or operator-level permissions.
         """
-        query_params = {}
+        query_params = {
+            'state': [TransactionStateChoices.COMMITTED, TransactionStateChoices.PENDING],
+        }
         if include_aggregates:
             query_params['include_aggregates'] = include_aggregates
         if lms_user_id:
             query_params['lms_user_id'] = lms_user_id
         if content_key:
             query_params['content_key'] = content_key
         if subsidy_access_policy_uuid:
             query_params['subsidy_access_policy_uuid'] = str(subsidy_access_policy_uuid)
+        if transaction_states:
+            valid_states = [
+                state for state in transaction_states
+                if state in TransactionStateChoices.VALID_CHOICES
+            ]
+            query_params['state'] = valid_states
 
         response = self.client.get(
             self.TRANSACTIONS_LIST_ENDPOINT.format(subsidy_uuid=subsidy_uuid),
             params=query_params,
         )
         response.raise_for_status()
         return response.json()
```

### Comparing `edx-enterprise-subsidy-client-0.3.1/edx_enterprise_subsidy_client.egg-info/PKG-INFO` & `edx-enterprise-subsidy-client-0.3.2/edx_enterprise_subsidy_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-enterprise-subsidy-client
-Version: 0.3.1
+Version: 0.3.2
 Summary: Client for interacting with the enterprise-subsidy service.
 Home-page: https://github.com/openedx/edx-enterprise-subsidy-client
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -223,14 +223,19 @@
 
 Unreleased
 **********
 
 * Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
   deprecated
 
+[0.3.2]
+*******
+* admin-list transactions will ask to be filtered for only `committed` and `pending` states by default.
+  Caller may specify other valid states (e.g. `failed` or `created`).
+
 [0.3.1]
 *******
 * fix: correctly pass ``subsidy_uuid`` to subsidy API V2 endpoint string format.
 
 [0.3.0]
 *******
 * feat: add new client for v2 transaction endpoint.
```

### Comparing `edx-enterprise-subsidy-client-0.3.1/edx_enterprise_subsidy_client.egg-info/SOURCES.txt` & `edx-enterprise-subsidy-client-0.3.2/edx_enterprise_subsidy_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-subsidy-client-0.3.1/requirements/constraints.txt` & `edx-enterprise-subsidy-client-0.3.2/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-subsidy-client-0.3.1/setup.py` & `edx-enterprise-subsidy-client-0.3.2/setup.py`

 * *Files identical despite different names*

