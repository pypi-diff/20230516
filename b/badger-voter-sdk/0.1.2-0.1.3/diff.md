# Comparing `tmp/badger-voter-sdk-0.1.2.tar.gz` & `tmp/badger-voter-sdk-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "badger-voter-sdk-0.1.2.tar", last modified: Thu Sep 22 15:24:33 2022, max compression
+gzip compressed data, was "badger-voter-sdk-0.1.3.tar", last modified: Tue May 16 15:53:57 2023, max compression
```

## Comparing `badger-voter-sdk-0.1.2.tar` & `badger-voter-sdk-0.1.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 shakotn    (501) staff       (20)        0 2022-09-22 15:24:33.857297 badger-voter-sdk-0.1.2/
--rw-r--r--   0 shakotn    (501) staff       (20)     1066 2022-07-25 07:54:04.000000 badger-voter-sdk-0.1.2/LICENSE
--rw-r--r--   0 shakotn    (501) staff       (20)       42 2022-07-25 08:29:57.000000 badger-voter-sdk-0.1.2/MANIFEST.in
--rw-r--r--   0 shakotn    (501) staff       (20)      159 2022-07-25 08:00:22.000000 badger-voter-sdk-0.1.2/Makefile
--rw-r--r--   0 shakotn    (501) staff       (20)     2654 2022-09-22 15:24:33.857357 badger-voter-sdk-0.1.2/PKG-INFO
--rw-r--r--   0 shakotn    (501) staff       (20)     2149 2022-09-19 14:54:52.000000 badger-voter-sdk-0.1.2/README.md
-drwxr-xr-x   0 shakotn    (501) staff       (20)        0 2022-09-22 15:24:33.855295 badger-voter-sdk-0.1.2/badger_voter_sdk/
--rw-r--r--   0 shakotn    (501) staff       (20)        0 2022-07-25 07:31:21.000000 badger-voter-sdk-0.1.2/badger_voter_sdk/__init__.py
--rw-r--r--   0 shakotn    (501) staff       (20)     2135 2022-09-22 13:45:58.000000 badger-voter-sdk-0.1.2/badger_voter_sdk/aws.py
--rw-r--r--   0 shakotn    (501) staff       (20)     6019 2022-09-19 14:54:52.000000 badger-voter-sdk-0.1.2/badger_voter_sdk/cast_vote.py
-drwxr-xr-x   0 shakotn    (501) staff       (20)        0 2022-09-22 15:24:33.857096 badger-voter-sdk-0.1.2/badger_voter_sdk/collectors/
--rw-r--r--   0 shakotn    (501) staff       (20)        0 2022-07-25 19:25:04.000000 badger-voter-sdk-0.1.2/badger_voter_sdk/collectors/__init__.py
--rw-r--r--   0 shakotn    (501) staff       (20)     2292 2022-09-19 14:54:52.000000 badger-voter-sdk-0.1.2/badger_voter_sdk/collectors/api_collectors.py
--rw-r--r--   0 shakotn    (501) staff       (20)     2959 2022-08-02 12:14:02.000000 badger-voter-sdk-0.1.2/badger_voter_sdk/collectors/data_processors.py
--rw-r--r--   0 shakotn    (501) staff       (20)     4075 2022-08-25 11:58:47.000000 badger-voter-sdk-0.1.2/badger_voter_sdk/collectors/snapshot_collectors.py
--rw-r--r--   0 shakotn    (501) staff       (20)      412 2022-07-25 19:25:04.000000 badger-voter-sdk-0.1.2/badger_voter_sdk/collectors/transports.py
--rw-r--r--   0 shakotn    (501) staff       (20)      619 2022-09-09 13:19:11.000000 badger-voter-sdk-0.1.2/badger_voter_sdk/constants.py
--rw-r--r--   0 shakotn    (501) staff       (20)     1447 2022-09-19 14:54:52.000000 badger-voter-sdk-0.1.2/badger_voter_sdk/discord.py
--rw-r--r--   0 shakotn    (501) staff       (20)     1069 2022-09-22 15:24:17.000000 badger-voter-sdk-0.1.2/badger_voter_sdk/json_logger.py
--rw-r--r--   0 shakotn    (501) staff       (20)     1938 2022-08-29 14:33:47.000000 badger-voter-sdk-0.1.2/badger_voter_sdk/utils.py
--rw-r--r--   0 shakotn    (501) staff       (20)      624 2022-07-25 07:47:14.000000 badger-voter-sdk-0.1.2/badger_voter_sdk/web3.py
-drwxr-xr-x   0 shakotn    (501) staff       (20)        0 2022-09-22 15:24:33.856196 badger-voter-sdk-0.1.2/badger_voter_sdk.egg-info/
--rw-r--r--   0 shakotn    (501) staff       (20)     2654 2022-09-22 15:24:33.000000 badger-voter-sdk-0.1.2/badger_voter_sdk.egg-info/PKG-INFO
--rw-r--r--   0 shakotn    (501) staff       (20)      723 2022-09-22 15:24:33.000000 badger-voter-sdk-0.1.2/badger_voter_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 shakotn    (501) staff       (20)        1 2022-09-22 15:24:33.000000 badger-voter-sdk-0.1.2/badger_voter_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 shakotn    (501) staff       (20)      144 2022-09-22 15:24:33.000000 badger-voter-sdk-0.1.2/badger_voter_sdk.egg-info/requires.txt
--rw-r--r--   0 shakotn    (501) staff       (20)       17 2022-09-22 15:24:33.000000 badger-voter-sdk-0.1.2/badger_voter_sdk.egg-info/top_level.txt
--rw-r--r--   0 shakotn    (501) staff       (20)      144 2022-09-19 14:54:52.000000 badger-voter-sdk-0.1.2/requirements.txt
--rw-r--r--   0 shakotn    (501) staff       (20)      131 2022-09-22 15:24:33.857566 badger-voter-sdk-0.1.2/setup.cfg
--rw-r--r--   0 shakotn    (501) staff       (20)      952 2022-09-22 15:24:17.000000 badger-voter-sdk-0.1.2/setup.py
+drwxr-xr-x   0 shakotn    (501) staff       (20)        0 2023-05-16 15:53:57.959518 badger-voter-sdk-0.1.3/
+-rw-r--r--   0 shakotn    (501) staff       (20)     1066 2022-07-25 07:54:04.000000 badger-voter-sdk-0.1.3/LICENSE
+-rw-r--r--   0 shakotn    (501) staff       (20)       42 2022-07-25 08:29:57.000000 badger-voter-sdk-0.1.3/MANIFEST.in
+-rw-r--r--   0 shakotn    (501) staff       (20)      159 2022-07-25 08:00:22.000000 badger-voter-sdk-0.1.3/Makefile
+-rw-r--r--   0 shakotn    (501) staff       (20)     2634 2023-05-16 15:53:57.959602 badger-voter-sdk-0.1.3/PKG-INFO
+-rw-r--r--   0 shakotn    (501) staff       (20)     2149 2022-09-19 14:54:52.000000 badger-voter-sdk-0.1.3/README.md
+drwxr-xr-x   0 shakotn    (501) staff       (20)        0 2023-05-16 15:53:57.957239 badger-voter-sdk-0.1.3/badger_voter_sdk/
+-rw-r--r--   0 shakotn    (501) staff       (20)        0 2022-07-25 07:31:21.000000 badger-voter-sdk-0.1.3/badger_voter_sdk/__init__.py
+-rw-r--r--   0 shakotn    (501) staff       (20)     2135 2022-09-22 13:45:58.000000 badger-voter-sdk-0.1.3/badger_voter_sdk/aws.py
+-rw-r--r--   0 shakotn    (501) staff       (20)     6019 2022-09-19 14:54:52.000000 badger-voter-sdk-0.1.3/badger_voter_sdk/cast_vote.py
+drwxr-xr-x   0 shakotn    (501) staff       (20)        0 2023-05-16 15:53:57.959262 badger-voter-sdk-0.1.3/badger_voter_sdk/collectors/
+-rw-r--r--   0 shakotn    (501) staff       (20)        0 2022-07-25 19:25:04.000000 badger-voter-sdk-0.1.3/badger_voter_sdk/collectors/__init__.py
+-rw-r--r--   0 shakotn    (501) staff       (20)     2292 2022-09-19 14:54:52.000000 badger-voter-sdk-0.1.3/badger_voter_sdk/collectors/api_collectors.py
+-rw-r--r--   0 shakotn    (501) staff       (20)     2959 2022-08-02 12:14:02.000000 badger-voter-sdk-0.1.3/badger_voter_sdk/collectors/data_processors.py
+-rw-r--r--   0 shakotn    (501) staff       (20)     4075 2022-08-25 11:58:47.000000 badger-voter-sdk-0.1.3/badger_voter_sdk/collectors/snapshot_collectors.py
+-rw-r--r--   0 shakotn    (501) staff       (20)      412 2022-07-25 19:25:04.000000 badger-voter-sdk-0.1.3/badger_voter_sdk/collectors/transports.py
+-rw-r--r--   0 shakotn    (501) staff       (20)      645 2023-05-16 15:50:49.000000 badger-voter-sdk-0.1.3/badger_voter_sdk/constants.py
+-rw-r--r--   0 shakotn    (501) staff       (20)     1447 2022-09-19 14:54:52.000000 badger-voter-sdk-0.1.3/badger_voter_sdk/discord.py
+-rw-r--r--   0 shakotn    (501) staff       (20)     1069 2022-09-22 15:24:17.000000 badger-voter-sdk-0.1.3/badger_voter_sdk/json_logger.py
+-rw-r--r--   0 shakotn    (501) staff       (20)     1938 2022-08-29 14:33:47.000000 badger-voter-sdk-0.1.3/badger_voter_sdk/utils.py
+-rw-r--r--   0 shakotn    (501) staff       (20)      624 2022-07-25 07:47:14.000000 badger-voter-sdk-0.1.3/badger_voter_sdk/web3.py
+drwxr-xr-x   0 shakotn    (501) staff       (20)        0 2023-05-16 15:53:57.958153 badger-voter-sdk-0.1.3/badger_voter_sdk.egg-info/
+-rw-r--r--   0 shakotn    (501) staff       (20)     2634 2023-05-16 15:53:57.000000 badger-voter-sdk-0.1.3/badger_voter_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 shakotn    (501) staff       (20)      723 2023-05-16 15:53:57.000000 badger-voter-sdk-0.1.3/badger_voter_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 shakotn    (501) staff       (20)        1 2023-05-16 15:53:57.000000 badger-voter-sdk-0.1.3/badger_voter_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 shakotn    (501) staff       (20)      144 2023-05-16 15:53:57.000000 badger-voter-sdk-0.1.3/badger_voter_sdk.egg-info/requires.txt
+-rw-r--r--   0 shakotn    (501) staff       (20)       17 2023-05-16 15:53:57.000000 badger-voter-sdk-0.1.3/badger_voter_sdk.egg-info/top_level.txt
+-rw-r--r--   0 shakotn    (501) staff       (20)      144 2022-09-19 14:54:52.000000 badger-voter-sdk-0.1.3/requirements.txt
+-rw-r--r--   0 shakotn    (501) staff       (20)      131 2023-05-16 15:53:57.960393 badger-voter-sdk-0.1.3/setup.cfg
+-rw-r--r--   0 shakotn    (501) staff       (20)      952 2023-05-16 15:53:39.000000 badger-voter-sdk-0.1.3/setup.py
```

### Comparing `badger-voter-sdk-0.1.2/LICENSE` & `badger-voter-sdk-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `badger-voter-sdk-0.1.2/PKG-INFO` & `badger-voter-sdk-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: badger-voter-sdk
-Version: 0.1.2
+Version: 0.1.3
 Summary: Shared code for badger autovoters
 Home-page: https://github.com/Badger-Finance/badger-voter-sdk
 Author: SHAKOTN
 Author-email: andrii@badger.com
 License: MIT
 Keywords: badger-voter-sdk
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7,<4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -87,9 +86,7 @@
 You need to combine two previous functions outputs:
 
 ```python
 from badger_voter_sdk.collectors.data_processors import extract_voting_power_per_pool
 
 choices_with_votes = extract_voting_power_per_pool(voters={"<wallet>": {"1": 123}}, scores={"<wallet>": 123333.1})
 ```
-
-
```

### Comparing `badger-voter-sdk-0.1.2/README.md` & `badger-voter-sdk-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `badger-voter-sdk-0.1.2/badger_voter_sdk/aws.py` & `badger-voter-sdk-0.1.3/badger_voter_sdk/aws.py`

 * *Files identical despite different names*

### Comparing `badger-voter-sdk-0.1.2/badger_voter_sdk/cast_vote.py` & `badger-voter-sdk-0.1.3/badger_voter_sdk/cast_vote.py`

 * *Files identical despite different names*

### Comparing `badger-voter-sdk-0.1.2/badger_voter_sdk/collectors/api_collectors.py` & `badger-voter-sdk-0.1.3/badger_voter_sdk/collectors/api_collectors.py`

 * *Files identical despite different names*

### Comparing `badger-voter-sdk-0.1.2/badger_voter_sdk/collectors/data_processors.py` & `badger-voter-sdk-0.1.3/badger_voter_sdk/collectors/data_processors.py`

 * *Files identical despite different names*

### Comparing `badger-voter-sdk-0.1.2/badger_voter_sdk/collectors/snapshot_collectors.py` & `badger-voter-sdk-0.1.3/badger_voter_sdk/collectors/snapshot_collectors.py`

 * *Files identical despite different names*

### Comparing `badger-voter-sdk-0.1.2/badger_voter_sdk/constants.py` & `badger-voter-sdk-0.1.3/badger_voter_sdk/constants.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Secrets settings
 from enum import Enum
 
-ETHNODEURL_SECRET_ID = "quiknode/eth-node-url"
+ETHNODEURL_SECRET_ID = "autovoter/web3_ethereum_mainnet_alchemy_api_key"
 ETHNODEURL_SECRET_KEY = "NODE_URL"
 REGION = "us-west-1"
 
 
 # API URLs
 SNAPSHOT_GQL_API_URL = "https://hub.snapshot.org/graphql"
 SNAPSHOT_SCORES_URL = "https://score.snapshot.org/api/scores"
```

### Comparing `badger-voter-sdk-0.1.2/badger_voter_sdk/discord.py` & `badger-voter-sdk-0.1.3/badger_voter_sdk/discord.py`

 * *Files identical despite different names*

### Comparing `badger-voter-sdk-0.1.2/badger_voter_sdk/json_logger.py` & `badger-voter-sdk-0.1.3/badger_voter_sdk/json_logger.py`

 * *Files identical despite different names*

### Comparing `badger-voter-sdk-0.1.2/badger_voter_sdk/utils.py` & `badger-voter-sdk-0.1.3/badger_voter_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `badger-voter-sdk-0.1.2/badger_voter_sdk/web3.py` & `badger-voter-sdk-0.1.3/badger_voter_sdk/web3.py`

 * *Files identical despite different names*

### Comparing `badger-voter-sdk-0.1.2/badger_voter_sdk.egg-info/PKG-INFO` & `badger-voter-sdk-0.1.3/badger_voter_sdk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: badger-voter-sdk
-Version: 0.1.2
+Version: 0.1.3
 Summary: Shared code for badger autovoters
 Home-page: https://github.com/Badger-Finance/badger-voter-sdk
 Author: SHAKOTN
 Author-email: andrii@badger.com
 License: MIT
 Keywords: badger-voter-sdk
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7,<4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -87,9 +86,7 @@
 You need to combine two previous functions outputs:
 
 ```python
 from badger_voter_sdk.collectors.data_processors import extract_voting_power_per_pool
 
 choices_with_votes = extract_voting_power_per_pool(voters={"<wallet>": {"1": 123}}, scores={"<wallet>": 123333.1})
 ```
-
-
```

### Comparing `badger-voter-sdk-0.1.2/badger_voter_sdk.egg-info/SOURCES.txt` & `badger-voter-sdk-0.1.3/badger_voter_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `badger-voter-sdk-0.1.2/setup.py` & `badger-voter-sdk-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     author_email="andrii@badger.com",
     description="Shared code for badger autovoters",
     long_description=README,
     keywords=["badger-voter-sdk"],
     long_description_content_type="text/markdown",
     packages=find_packages(exclude=['tests*']),
     include_package_data=True,
-    version="0.1.2",
+    version="0.1.3",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
     ],
     license="MIT",
     url="https://github.com/Badger-Finance/badger-voter-sdk",
```

