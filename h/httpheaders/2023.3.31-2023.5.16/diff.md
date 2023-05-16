# Comparing `tmp/httpheaders-2023.3.31.tar.gz` & `tmp/httpheaders-2023.5.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "httpheaders-2023.3.31.tar", last modified: Fri Mar 31 02:32:34 2023, max compression
+gzip compressed data, was "httpheaders-2023.5.16.tar", last modified: Tue May 16 02:30:10 2023, max compression
```

## Comparing `httpheaders-2023.3.31.tar` & `httpheaders-2023.5.16.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 02:32:34.259650 httpheaders-2023.3.31/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-03-31 02:32:16.000000 httpheaders-2023.3.31/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-03-31 02:32:34.259650 httpheaders-2023.3.31/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-03-31 02:32:16.000000 httpheaders-2023.3.31/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 02:32:34.259650 httpheaders-2023.3.31/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-03-31 02:32:16.000000 httpheaders-2023.3.31/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 02:32:34.255650 httpheaders-2023.3.31/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 02:32:34.255650 httpheaders-2023.3.31/src/headers/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-03-31 02:32:23.000000 httpheaders-2023.3.31/src/headers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25411 2023-03-31 02:32:23.000000 httpheaders-2023.3.31/src/headers/binary.py
--rw-r--r--   0 runner    (1001) docker     (123)    25192 2023-03-31 02:32:23.000000 httpheaders-2023.3.31/src/headers/string.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 02:32:34.255650 httpheaders-2023.3.31/src/httpheaders.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-03-31 02:32:34.000000 httpheaders-2023.3.31/src/httpheaders.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-03-31 02:32:34.000000 httpheaders-2023.3.31/src/httpheaders.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 02:32:34.000000 httpheaders-2023.3.31/src/httpheaders.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-31 02:32:34.000000 httpheaders-2023.3.31/src/httpheaders.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:30:10.201943 httpheaders-2023.5.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-16 02:29:48.000000 httpheaders-2023.5.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-16 02:30:10.201943 httpheaders-2023.5.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-16 02:29:48.000000 httpheaders-2023.5.16/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 02:30:10.201943 httpheaders-2023.5.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-16 02:29:48.000000 httpheaders-2023.5.16/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:30:10.201943 httpheaders-2023.5.16/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:30:10.201943 httpheaders-2023.5.16/src/headers/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-16 02:29:57.000000 httpheaders-2023.5.16/src/headers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25925 2023-05-16 02:29:57.000000 httpheaders-2023.5.16/src/headers/binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25702 2023-05-16 02:29:57.000000 httpheaders-2023.5.16/src/headers/string.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:30:10.201943 httpheaders-2023.5.16/src/httpheaders.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-16 02:30:10.000000 httpheaders-2023.5.16/src/httpheaders.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-16 02:30:10.000000 httpheaders-2023.5.16/src/httpheaders.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 02:30:10.000000 httpheaders-2023.5.16/src/httpheaders.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 02:30:10.000000 httpheaders-2023.5.16/src/httpheaders.egg-info/top_level.txt
```

### Comparing `httpheaders-2023.3.31/LICENSE` & `httpheaders-2023.5.16/LICENSE`

 * *Files identical despite different names*

### Comparing `httpheaders-2023.3.31/PKG-INFO` & `httpheaders-2023.5.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: httpheaders
-Version: 2023.3.31
+Version: 2023.5.16
 Summary: HTTP Headers
 Home-page: https://github.com/joniumGit/headers
 Author: joniumGit
 Project-URL: Bug Reports, https://github.com/joniumGit/headers
 Project-URL: Source, https://github.com/joniumGit/headers
 Keywords: HTTP,headers,API
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `httpheaders-2023.3.31/setup.py` & `httpheaders-2023.5.16/setup.py`

 * *Files identical despite different names*

### Comparing `httpheaders-2023.3.31/src/headers/binary.py` & `httpheaders-2023.5.16/src/headers/binary.py`

 * *Files 2% similar despite different names*

```diff
@@ -507,14 +507,26 @@
 
 DIGEST = b"Digest"
 """Digest [permanent]
 
 [RFC 3230: Instance Digests in HTTP]
 """
 
+DPOP = b"DPoP"
+"""DPoP [permanent]
+
+[RFC-ietf-oauth-dpop-16: OAuth 2.0 Demonstrating Proof-of-Possession at the Application Layer (DPoP)]
+"""
+
+DPOP_NONCE = b"DPoP-Nonce"
+"""DPoP-Nonce [permanent]
+
+[RFC-ietf-oauth-dpop-16: OAuth 2.0 Demonstrating Proof-of-Possession at the Application Layer (DPoP)]
+"""
+
 EARLY_DATA = b"Early-Data"
 """Early-Data [permanent]
 
 [RFC 8470: Using Early Data in HTTP]
 """
 
 EDIINT_FEATURES = b"EDIINT-Features"
@@ -827,14 +839,20 @@
 
 PEP_INFO = b"Pep-Info"
 """Pep-Info [obsoleted]
 
 [PEP - an Extension Mechanism for HTTP]
 """
 
+PERMISSIONS_POLICY = b"Permissions-Policy"
+"""Permissions-Policy [provisional]
+
+[Permissions Policy]
+"""
+
 PICS_LABEL = b"PICS-Label"
 """PICS-Label [obsoleted]
 
 [PICS Label Distribution Label Syntax and Communication Protocols]
 """
 
 PING_FROM = b"Ping-From"
@@ -1019,14 +1037,20 @@
 
 REPLAY_NONCE = b"Replay-Nonce"
 """Replay-Nonce [permanent]
 
 [RFC 8555, Section 6.5.1: Automatic Certificate Management Environment (ACME)]
 """
 
+REPORTING_ENDPOINTS = b"Reporting-Endpoints"
+"""Reporting-Endpoints [provisional]
+
+[Reporting API]
+"""
+
 RETRY_AFTER = b"Retry-After"
 """Retry-After [permanent]
 
 [RFC9110, Section 10.2.3: HTTP Semantics]
 """
 
 SAFE = b"Safe"
```

### Comparing `httpheaders-2023.3.31/src/headers/string.py` & `httpheaders-2023.5.16/src/headers/string.py`

 * *Files 3% similar despite different names*

```diff
@@ -507,14 +507,26 @@
 
 DIGEST = "Digest"
 """Digest [permanent]
 
 [RFC 3230: Instance Digests in HTTP]
 """
 
+DPOP = "DPoP"
+"""DPoP [permanent]
+
+[RFC-ietf-oauth-dpop-16: OAuth 2.0 Demonstrating Proof-of-Possession at the Application Layer (DPoP)]
+"""
+
+DPOP_NONCE = "DPoP-Nonce"
+"""DPoP-Nonce [permanent]
+
+[RFC-ietf-oauth-dpop-16: OAuth 2.0 Demonstrating Proof-of-Possession at the Application Layer (DPoP)]
+"""
+
 EARLY_DATA = "Early-Data"
 """Early-Data [permanent]
 
 [RFC 8470: Using Early Data in HTTP]
 """
 
 EDIINT_FEATURES = "EDIINT-Features"
@@ -827,14 +839,20 @@
 
 PEP_INFO = "Pep-Info"
 """Pep-Info [obsoleted]
 
 [PEP - an Extension Mechanism for HTTP]
 """
 
+PERMISSIONS_POLICY = "Permissions-Policy"
+"""Permissions-Policy [provisional]
+
+[Permissions Policy]
+"""
+
 PICS_LABEL = "PICS-Label"
 """PICS-Label [obsoleted]
 
 [PICS Label Distribution Label Syntax and Communication Protocols]
 """
 
 PING_FROM = "Ping-From"
@@ -1019,14 +1037,20 @@
 
 REPLAY_NONCE = "Replay-Nonce"
 """Replay-Nonce [permanent]
 
 [RFC 8555, Section 6.5.1: Automatic Certificate Management Environment (ACME)]
 """
 
+REPORTING_ENDPOINTS = "Reporting-Endpoints"
+"""Reporting-Endpoints [provisional]
+
+[Reporting API]
+"""
+
 RETRY_AFTER = "Retry-After"
 """Retry-After [permanent]
 
 [RFC9110, Section 10.2.3: HTTP Semantics]
 """
 
 SAFE = "Safe"
```

### Comparing `httpheaders-2023.3.31/src/httpheaders.egg-info/PKG-INFO` & `httpheaders-2023.5.16/src/httpheaders.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: httpheaders
-Version: 2023.3.31
+Version: 2023.5.16
 Summary: HTTP Headers
 Home-page: https://github.com/joniumGit/headers
 Author: joniumGit
 Project-URL: Bug Reports, https://github.com/joniumGit/headers
 Project-URL: Source, https://github.com/joniumGit/headers
 Keywords: HTTP,headers,API
 Classifier: Development Status :: 5 - Production/Stable
```

