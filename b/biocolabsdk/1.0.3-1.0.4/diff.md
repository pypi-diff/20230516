# Comparing `tmp/biocolabsdk-1.0.3.tar.gz` & `tmp/biocolabsdk-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biocolabsdk-1.0.3.tar", max compression
+gzip compressed data, was "biocolabsdk-1.0.4.tar", max compression
```

## Comparing `biocolabsdk-1.0.3.tar` & `biocolabsdk-1.0.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     6833 2023-05-16 12:07:13.986784 biocolabsdk-1.0.3/README.md
--rw-r--r--   0        0        0     6148 2023-04-13 03:18:11.944270 biocolabsdk-1.0.3/biocolabsdk/.DS_Store
--rw-r--r--   0        0        0       92 2023-05-16 11:52:44.788427 biocolabsdk-1.0.3/biocolabsdk/__init__.py
--rw-r--r--   0        0        0     4189 2023-05-16 11:52:44.788427 biocolabsdk-1.0.3/biocolabsdk/connector.py
--rw-r--r--   0        0        0      756 2023-05-16 11:52:44.788427 biocolabsdk-1.0.3/biocolabsdk/identity.py
--rw-r--r--   0        0        0     1305 2023-05-16 11:52:44.788427 biocolabsdk-1.0.3/biocolabsdk/util.py
--rw-r--r--   0        0        0      437 2023-05-16 12:07:13.986784 biocolabsdk-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     7490 1970-01-01 00:00:00.000000 biocolabsdk-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     6833 2023-05-16 12:10:15.514555 biocolabsdk-1.0.4/README.md
+-rw-r--r--   0        0        0     6148 2023-04-13 03:18:11.944270 biocolabsdk-1.0.4/biocolabsdk/.DS_Store
+-rw-r--r--   0        0        0       92 2023-05-16 11:52:44.788427 biocolabsdk-1.0.4/biocolabsdk/__init__.py
+-rw-r--r--   0        0        0     4189 2023-05-16 11:52:44.788427 biocolabsdk-1.0.4/biocolabsdk/connector.py
+-rw-r--r--   0        0        0      756 2023-05-16 11:52:44.788427 biocolabsdk-1.0.4/biocolabsdk/identity.py
+-rw-r--r--   0        0        0     1305 2023-05-16 11:52:44.788427 biocolabsdk-1.0.4/biocolabsdk/util.py
+-rw-r--r--   0        0        0      437 2023-05-16 12:10:15.514555 biocolabsdk-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     7490 1970-01-01 00:00:00.000000 biocolabsdk-1.0.4/PKG-INFO
```

### Comparing `biocolabsdk-1.0.3/README.md` & `biocolabsdk-1.0.4/README.md`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # How to use biocolabsdk ?
 
-## 1. Access to BBrowserX private server via biocolabsdk:
-
 **The package only allows data submission via BioColab private server. Please configure your tokens in the `User Settings` page.**
 
 </br>
 <img alt="setting" src="https://cdn.bioturing.com/documentation/md/user-setting.png" width="100%">
 </br>
 
+## 1. Access to BBrowserX private server via biocolabsdk:
+
 ### 1.1. Test the connection to BBrowserX private server:
 
 ```python
 
 from biocolabsdk.connector import EConnector
 
 connector = EConnector(
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-# How to use biocolabsdk ? ## 1. Access to BBrowserX private server via
-biocolabsdk: **The package only allows data submission via BioColab private
-server. Please configure your tokens in the `User Settings` page.**  [setting]
+# How to use biocolabsdk ? **The package only allows data submission via
+BioColab private server. Please configure your tokens in the `User Settings`
+page.**  [setting]  ## 1. Access to BBrowserX private server via biocolabsdk:
 ### 1.1. Test the connection to BBrowserX private server: ```python from
 biocolabsdk.connector import EConnector connector = EConnector
 ( private_host="https://yourcompany/t2d_index_tool/, private_token="
 [                    ]" ) connector.get_bbrowserx().test_connection() ```
 Example output: ``` Connecting to host at https://yourcompany/t2d_index_tool/
 api/v1/test_connection Connection successful ``` ### 1.2. Get user groups
 available for your token in BBrowserX private server: ```python from
```

### Comparing `biocolabsdk-1.0.3/biocolabsdk/.DS_Store` & `biocolabsdk-1.0.4/biocolabsdk/.DS_Store`

 * *Files identical despite different names*

### Comparing `biocolabsdk-1.0.3/biocolabsdk/connector.py` & `biocolabsdk-1.0.4/biocolabsdk/connector.py`

 * *Files identical despite different names*

### Comparing `biocolabsdk-1.0.3/biocolabsdk/identity.py` & `biocolabsdk-1.0.4/biocolabsdk/identity.py`

 * *Files identical despite different names*

### Comparing `biocolabsdk-1.0.3/biocolabsdk/util.py` & `biocolabsdk-1.0.4/biocolabsdk/util.py`

 * *Files identical despite different names*

### Comparing `biocolabsdk-1.0.3/PKG-INFO` & `biocolabsdk-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biocolabsdk
-Version: 1.0.3
+Version: 1.0.4
 Summary: A set of python modules for accessing BioTuring Ecosystem on BioColab private server
 Author: BioTuring
 Author-email: support@bioturing.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -13,22 +13,22 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: bioflex (>=1.1,<2.0)
 Requires-Dist: bioturing-connector (>=1.1,<2.0)
 Description-Content-Type: text/markdown
 
 # How to use biocolabsdk ?
 
-## 1. Access to BBrowserX private server via biocolabsdk:
-
 **The package only allows data submission via BioColab private server. Please configure your tokens in the `User Settings` page.**
 
 </br>
 <img alt="setting" src="https://cdn.bioturing.com/documentation/md/user-setting.png" width="100%">
 </br>
 
+## 1. Access to BBrowserX private server via biocolabsdk:
+
 ### 1.1. Test the connection to BBrowserX private server:
 
 ```python
 
 from biocolabsdk.connector import EConnector
 
 connector = EConnector(
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: biocolabsdk Version: 1.0.3 Summary: A set of python
+Metadata-Version: 2.1 Name: biocolabsdk Version: 1.0.4 Summary: A set of python
 modules for accessing BioTuring Ecosystem on BioColab private server Author:
 BioTuring Author-email: support@bioturing.com Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: bioflex (>=1.1,<2.0) Requires-Dist: bioturing-connector
 (>=1.1,<2.0) Description-Content-Type: text/markdown # How to use biocolabsdk ?
-## 1. Access to BBrowserX private server via biocolabsdk: **The package only
-allows data submission via BioColab private server. Please configure your
-tokens in the `User Settings` page.**  [setting]  ### 1.1. Test the connection
-to BBrowserX private server: ```python from biocolabsdk.connector import
+**The package only allows data submission via BioColab private server. Please
+configure your tokens in the `User Settings` page.**  [setting]  ## 1. Access
+to BBrowserX private server via biocolabsdk: ### 1.1. Test the connection to
+BBrowserX private server: ```python from biocolabsdk.connector import
 EConnector connector = EConnector( private_host="https://yourcompany/
 t2d_index_tool/, private_token="[                    ]" )
 connector.get_bbrowserx().test_connection() ``` Example output: ``` Connecting
 to host at https://yourcompany/t2d_index_tool/api/v1/test_connection Connection
 successful ``` ### 1.2. Get user groups available for your token in BBrowserX
 private server: ```python from biocolabsdk.connector import EConnector
 connector = EConnector( private_host="https://yourcompany/t2d_index_tool/,
```

