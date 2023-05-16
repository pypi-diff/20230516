# Comparing `tmp/insidecouchbase-2.0.0.tar.gz` & `tmp/insidecouchbase-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "insidecouchbase-2.0.0.tar", last modified: Mon May  1 13:10:19 2023, max compression
+gzip compressed data, was "insidecouchbase-2.1.0.tar", last modified: Tue May 16 06:37:15 2023, max compression
```

## Comparing `insidecouchbase-2.0.0.tar` & `insidecouchbase-2.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-05-01 13:10:19.016147 insidecouchbase-2.0.0/
--rw-rw-r--   0 demir     (1000) demir     (1000)    35149 2023-04-21 20:42:51.000000 insidecouchbase-2.0.0/LICENSE
--rw-rw-r--   0 demir     (1000) demir     (1000)     4557 2023-05-01 13:10:19.016147 insidecouchbase-2.0.0/PKG-INFO
--rw-rw-r--   0 demir     (1000) demir     (1000)     3977 2023-05-01 12:39:43.000000 insidecouchbase-2.0.0/README.md
--rw-rw-r--   0 demir     (1000) demir     (1000)       84 2023-04-21 20:42:51.000000 insidecouchbase-2.0.0/pyproject.toml
--rw-rw-r--   0 demir     (1000) demir     (1000)      713 2023-05-01 13:10:19.016147 insidecouchbase-2.0.0/setup.cfg
--rw-rw-r--   0 demir     (1000) demir     (1000)     1013 2023-05-01 13:09:42.000000 insidecouchbase-2.0.0/setup.py
-drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-05-01 13:10:19.012148 insidecouchbase-2.0.0/src/
-drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-05-01 13:10:19.012148 insidecouchbase-2.0.0/src/couchbase/
--rw-rw-r--   0 demir     (1000) demir     (1000)       24 2023-05-01 13:02:16.000000 insidecouchbase-2.0.0/src/couchbase/__init__.py
--rw-rw-r--   0 demir     (1000) demir     (1000)    14621 2023-05-01 13:04:36.000000 insidecouchbase-2.0.0/src/couchbase/couchbase.py
--rw-rw-r--   0 demir     (1000) demir     (1000)     2059 2023-05-01 12:53:09.000000 insidecouchbase-2.0.0/src/couchbase/rules.py
-drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-05-01 13:10:19.016147 insidecouchbase-2.0.0/src/insidecouchbase.egg-info/
--rw-rw-r--   0 demir     (1000) demir     (1000)     4557 2023-05-01 13:10:19.000000 insidecouchbase-2.0.0/src/insidecouchbase.egg-info/PKG-INFO
--rw-rw-r--   0 demir     (1000) demir     (1000)      341 2023-05-01 13:10:19.000000 insidecouchbase-2.0.0/src/insidecouchbase.egg-info/SOURCES.txt
--rw-rw-r--   0 demir     (1000) demir     (1000)        1 2023-05-01 13:10:19.000000 insidecouchbase-2.0.0/src/insidecouchbase.egg-info/dependency_links.txt
--rw-rw-r--   0 demir     (1000) demir     (1000)       34 2023-05-01 13:10:19.000000 insidecouchbase-2.0.0/src/insidecouchbase.egg-info/requires.txt
--rw-rw-r--   0 demir     (1000) demir     (1000)       10 2023-05-01 13:10:19.000000 insidecouchbase-2.0.0/src/insidecouchbase.egg-info/top_level.txt
+drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-05-16 06:37:15.112198 insidecouchbase-2.1.0/
+-rw-rw-r--   0 demir     (1000) demir     (1000)    35149 2023-04-21 20:42:51.000000 insidecouchbase-2.1.0/LICENSE
+-rw-rw-r--   0 demir     (1000) demir     (1000)     4557 2023-05-16 06:37:15.112198 insidecouchbase-2.1.0/PKG-INFO
+-rw-rw-r--   0 demir     (1000) demir     (1000)     3977 2023-05-01 12:39:43.000000 insidecouchbase-2.1.0/README.md
+-rw-rw-r--   0 demir     (1000) demir     (1000)       84 2023-04-21 20:42:51.000000 insidecouchbase-2.1.0/pyproject.toml
+-rw-rw-r--   0 demir     (1000) demir     (1000)      713 2023-05-16 06:37:15.112198 insidecouchbase-2.1.0/setup.cfg
+-rw-rw-r--   0 demir     (1000) demir     (1000)     1013 2023-05-16 06:25:15.000000 insidecouchbase-2.1.0/setup.py
+drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-05-16 06:37:15.100198 insidecouchbase-2.1.0/src/
+drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-05-16 06:37:15.108198 insidecouchbase-2.1.0/src/couchbase/
+-rw-rw-r--   0 demir     (1000) demir     (1000)       24 2023-05-01 13:02:16.000000 insidecouchbase-2.1.0/src/couchbase/__init__.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)    14635 2023-05-16 06:11:57.000000 insidecouchbase-2.1.0/src/couchbase/couchbase.py
+-rw-rw-r--   0 demir     (1000) demir     (1000)     2345 2023-05-16 06:12:44.000000 insidecouchbase-2.1.0/src/couchbase/rules.py
+drwxrwxr-x   0 demir     (1000) demir     (1000)        0 2023-05-16 06:37:15.112198 insidecouchbase-2.1.0/src/insidecouchbase.egg-info/
+-rw-rw-r--   0 demir     (1000) demir     (1000)     4557 2023-05-16 06:37:15.000000 insidecouchbase-2.1.0/src/insidecouchbase.egg-info/PKG-INFO
+-rw-rw-r--   0 demir     (1000) demir     (1000)      341 2023-05-16 06:37:15.000000 insidecouchbase-2.1.0/src/insidecouchbase.egg-info/SOURCES.txt
+-rw-rw-r--   0 demir     (1000) demir     (1000)        1 2023-05-16 06:37:15.000000 insidecouchbase-2.1.0/src/insidecouchbase.egg-info/dependency_links.txt
+-rw-rw-r--   0 demir     (1000) demir     (1000)       34 2023-05-16 06:37:15.000000 insidecouchbase-2.1.0/src/insidecouchbase.egg-info/requires.txt
+-rw-rw-r--   0 demir     (1000) demir     (1000)       10 2023-05-16 06:37:15.000000 insidecouchbase-2.1.0/src/insidecouchbase.egg-info/top_level.txt
```

### Comparing `insidecouchbase-2.0.0/LICENSE` & `insidecouchbase-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `insidecouchbase-2.0.0/PKG-INFO` & `insidecouchbase-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: insidecouchbase
-Version: 2.0.0
+Version: 2.1.0
 Summary: Check and analyze a couchbase cluster in terms of cluster health,bucket,and replication
 Home-page: https://github.com/adiosamig/insidecocuhbase
 Author: Huseyin Demir
 Author-email: huseyin.d3r@gmail.com
 Project-URL: Bug Tracker, https://github.com/adiosamig/insidecocuhbase/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `insidecouchbase-2.0.0/README.md` & `insidecouchbase-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `insidecouchbase-2.0.0/setup.cfg` & `insidecouchbase-2.1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = insidecocuhbase
-version = 2.0.0
+version = 2.1.0
 author = Huseyin Demir
 author_email = huseyin.d3r@gmail.com
 description = A simple Python package
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 url = https://github.com/adiosamig/insidecocuhbase
 project_urls =
```

### Comparing `insidecouchbase-2.0.0/setup.py` & `insidecouchbase-2.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "insidecouchbase",
-    version = "2.0.0",
+    version = "2.1.0",
     author = "Huseyin Demir",
     author_email = "huseyin.d3r@gmail.com",
     description = "Check and analyze a couchbase cluster in terms of cluster health,bucket,and replication",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/adiosamig/insidecocuhbase",
     install_requires=[
```

### Comparing `insidecouchbase-2.0.0/src/couchbase/couchbase.py` & `insidecouchbase-2.1.0/src/couchbase/couchbase.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
             urlForHealth = f"http://{self.hostname}:8091/nodes/self"
             getNodeDetails = requests.get(
                 url=urlForHealth, auth=(self.logininformation, self.loginsecret))
             resultParsed = getNodeDetails.json()
             nodes=resultParsed
             totalMemoryInMB=int(nodes.get('memoryTotal')/(1024 ** 3))
             totalmemoryQuota=int(nodes.get('memoryQuota')/1024)
-            if totalmemoryQuota < (0.7 * totalMemoryInMB):
+            if totalmemoryQuota < (0.8 * totalMemoryInMB):
                 self.updateRule(code='configuration-01',result='passed')
             else:
                 self.updateRule(code='configuration-01',result='failed')
             
         except Exception as couchbaseBucketException:
             print(couchbaseBucketException)
     def getNodesOnCluster(self):
@@ -313,10 +313,10 @@
         for item in self.ruleList:
             if item["result"] == "passed":
                 item["result"] = u'\u2714' # green checkmark symbol
             else:
                 item["result"] = u'\u2718' # red cross mark symbol
         results=self.ruleList
         dataFrameforNodes=pd.DataFrame(results)
-        print(tabulate(dataFrameforNodes, headers = 'keys', tablefmt = 'psql'))
+        self.formattedOutput=tabulate(dataFrameforNodes, headers = 'keys', tablefmt = 'psql')
         return f''' Finished healtcheck.'''
```

### Comparing `insidecouchbase-2.0.0/src/couchbase/rules.py` & `insidecouchbase-2.1.0/src/couchbase/rules.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,58 +1,67 @@
 def setRules():
     ruleList=[
     {
         "code": "configuration-01",
         "definition" : "Data Memory Quota Configuration",
         "result":"not_checked",
-        "Recommendation" : "Data memory quota can not be greater than %70 of OS memory"
+        "severity": "critical",
+        "recommendation" : "Data memory quota can not be greater than %80 of OS memory"
     },
     {
         "code": "configuration-02",
         "definition" : "SWAP Configuration",
         "result":"not_checked",
-        "Recommendation" : "SWAP can not be used in production couchbase environments"
+        "severity": "critical",
+        "recommendation" : "SWAP can not be used in production couchbase environments"
     },
     {
         "code": "configuration-03",
         "definition" : "All Nodes are Using Same Couchbase Version",
         "result":"not_checked",
-        "Recommendation" : "Different versions of couchbase can not be used inside the same cluster."
+        "severity": "critical",
+        "recommendation" : "Different versions of couchbase can not be used inside the same cluster."
     },
     {
         "code": "configuration-04",
         "definition" : "Cluster is Working Wtih MDS Model",
         "result":"not_checked",
-        "Recommendation" : "1 Couchbase node has to be use 1 service only."
+        "severity": "critical",
+        "recommendation" : "1 Couchbase node has to be use 1 service only."
     },
     {
         "code": "configuration-05",
         "definition" : "Autofailover Enabled",
         "result":"not_checked",
-        "Recommendation" : "Autofailover needs to be enabled to achive better HA"
+        "severity": "critical",
+        "recommendation" : "Autofailover needs to be enabled to achive better HA"
     },
     {
         "code": "health-01",
         "definition" : "All Nodes Up and Running",
         "result":"not_checked",
-        "Recommendation" : "All nodes have to be up and joined cluster."
+        "severity": "critical",
+        "recommendation" : "All nodes have to be up and joined cluster."
     },
     {
         "code": "bucket-01",
         "definition" : "All Buckets Have Resident Ratio Greater Than %50",
         "result":"not_checked",
-        "Recommendation" : "Bucket resident ratio needs to be greater than %50"
+        "severity": "medium",
+        "recommendation" : "Bucket resident ratio needs to be greater than %50"
     },
     {
         "code": "bucket-02",
         "definition" : "All Buckets Have At Least 1 Replica",
         "result":"not_checked",
-        "Recommendation" : "All buckets must have at least one replica to prevent data loss in case of emergency"
+        "severity": "critical",
+        "recommendation" : "All buckets must have at least one replica to prevent data loss in case of emergency"
     },
     {
         "code": "bucket-03",
         "definition" : "All Buckets Have 1024 Primary Vbucket",
         "result":"not_checked",
-        "Recommendation" : "All buckets must carry 1024 primary vbucket."
+        "severity": "critical",
+        "recommendation" : "All buckets must carry 1024 primary vbucket."
     }
 ]
     return ruleList
```

### Comparing `insidecouchbase-2.0.0/src/insidecouchbase.egg-info/PKG-INFO` & `insidecouchbase-2.1.0/src/insidecouchbase.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: insidecouchbase
-Version: 2.0.0
+Version: 2.1.0
 Summary: Check and analyze a couchbase cluster in terms of cluster health,bucket,and replication
 Home-page: https://github.com/adiosamig/insidecocuhbase
 Author: Huseyin Demir
 Author-email: huseyin.d3r@gmail.com
 Project-URL: Bug Tracker, https://github.com/adiosamig/insidecocuhbase/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

