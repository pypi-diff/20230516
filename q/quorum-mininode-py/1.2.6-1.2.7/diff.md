# Comparing `tmp/quorum_mininode_py-1.2.6.tar.gz` & `tmp/quorum_mininode_py-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quorum_mininode_py-1.2.6.tar", last modified: Wed May  3 11:41:42 2023, max compression
+gzip compressed data, was "quorum_mininode_py-1.2.7.tar", last modified: Tue May 16 12:57:39 2023, max compression
```

## Comparing `quorum_mininode_py-1.2.6.tar` & `quorum_mininode_py-1.2.7.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 11:41:42.626737 quorum_mininode_py-1.2.6/
--rw-rw-rw-   0        0        0     1087 2023-04-03 04:23:18.000000 quorum_mininode_py-1.2.6/LICENSE
--rw-rw-rw-   0        0        0     2440 2023-05-03 11:41:42.625785 quorum_mininode_py-1.2.6/PKG-INFO
--rw-rw-rw-   0        0        0     1580 2023-04-03 04:24:50.000000 quorum_mininode_py-1.2.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 11:41:42.515497 quorum_mininode_py-1.2.6/quorum_mininode_py/
--rw-rw-rw-   0        0        0      364 2023-05-03 11:40:00.000000 quorum_mininode_py-1.2.6/quorum_mininode_py/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 11:41:42.573584 quorum_mininode_py-1.2.6/quorum_mininode_py/api/
--rw-rw-rw-   0        0        0       59 2023-03-11 06:14:59.000000 quorum_mininode_py-1.2.6/quorum_mininode_py/api/__init__.py
--rw-rw-rw-   0        0        0     3705 2023-04-28 04:18:02.000000 quorum_mininode_py-1.2.6/quorum_mininode_py/api/base.py
--rw-rw-rw-   0        0        0     3812 2023-05-03 11:14:28.000000 quorum_mininode_py-1.2.6/quorum_mininode_py/api/lightnode.py
-drwxrwxrwx   0        0        0        0 2023-05-03 11:41:42.582562 quorum_mininode_py-1.2.6/quorum_mininode_py/client/
--rw-rw-rw-   0        0        0      134 2023-03-17 17:21:12.000000 quorum_mininode_py-1.2.6/quorum_mininode_py/client/__init__.py
--rw-rw-rw-   0        0        0     1858 2023-04-28 04:16:53.000000 quorum_mininode_py-1.2.6/quorum_mininode_py/client/_http.py
--rw-rw-rw-   0        0        0     3487 2023-05-03 11:17:18.000000 quorum_mininode_py-1.2.6/quorum_mininode_py/client/mininode.py
-drwxrwxrwx   0        0        0        0 2023-05-03 11:41:42.594356 quorum_mininode_py-1.2.6/quorum_mininode_py/crypto/
--rw-rw-rw-   0        0        0      117 2023-03-11 06:14:59.000000 quorum_mininode_py-1.2.6/quorum_mininode_py/crypto/__init__.py
--rw-rw-rw-   0        0        0     2361 2023-05-03 11:14:57.000000 quorum_mininode_py-1.2.6/quorum_mininode_py/crypto/account.py
--rw-rw-rw-   0        0        0      517 2023-03-17 17:44:01.000000 quorum_mininode_py-1.2.6/quorum_mininode_py/crypto/aes.py
--rw-rw-rw-   0        0        0     1824 2023-05-03 11:15:00.000000 quorum_mininode_py-1.2.6/quorum_mininode_py/crypto/age.py
--rw-rw-rw-   0        0        0     3846 2023-05-03 11:36:39.000000 quorum_mininode_py-1.2.6/quorum_mininode_py/crypto/trx.py
-drwxrwxrwx   0        0        0        0 2023-05-03 11:41:42.599883 quorum_mininode_py-1.2.6/quorum_mininode_py/proto/
--rw-rw-rw-   0        0        0       87 2023-03-10 05:56:49.000000 quorum_mininode_py-1.2.6/quorum_mininode_py/proto/__init__.py
--rw-rw-rw-   0        0        0    15822 2023-03-30 04:24:35.000000 quorum_mininode_py-1.2.6/quorum_mininode_py/proto/quorum_pb2.py
-drwxrwxrwx   0        0        0        0 2023-05-03 11:41:42.605021 quorum_mininode_py-1.2.6/quorum_mininode_py/utils/
--rw-rw-rw-   0        0        0       75 2023-04-28 04:06:26.000000 quorum_mininode_py-1.2.6/quorum_mininode_py/utils/__init__.py
--rw-rw-rw-   0        0        0     4554 2023-03-30 08:24:57.000000 quorum_mininode_py-1.2.6/quorum_mininode_py/utils/url.py
-drwxrwxrwx   0        0        0        0 2023-05-03 11:41:42.529455 quorum_mininode_py-1.2.6/quorum_mininode_py.egg-info/
--rw-rw-rw-   0        0        0     2440 2023-05-03 11:41:42.000000 quorum_mininode_py-1.2.6/quorum_mininode_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      798 2023-05-03 11:41:42.000000 quorum_mininode_py-1.2.6/quorum_mininode_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 11:41:42.000000 quorum_mininode_py-1.2.6/quorum_mininode_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-05-03 11:41:42.000000 quorum_mininode_py-1.2.6/quorum_mininode_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-05-03 11:41:42.000000 quorum_mininode_py-1.2.6/quorum_mininode_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-03 11:41:42.626737 quorum_mininode_py-1.2.6/setup.cfg
--rw-rw-rw-   0        0        0     1301 2023-05-03 11:37:26.000000 quorum_mininode_py-1.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 12:57:39.862223 quorum_mininode_py-1.2.7/
+-rw-rw-rw-   0        0        0     1087 2023-04-03 04:23:18.000000 quorum_mininode_py-1.2.7/LICENSE
+-rw-rw-rw-   0        0        0     2440 2023-05-16 12:57:39.861226 quorum_mininode_py-1.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1580 2023-04-03 04:24:50.000000 quorum_mininode_py-1.2.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-16 12:57:39.819362 quorum_mininode_py-1.2.7/quorum_mininode_py/
+-rw-rw-rw-   0        0        0      364 2023-05-16 12:47:34.000000 quorum_mininode_py-1.2.7/quorum_mininode_py/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 12:57:39.835295 quorum_mininode_py-1.2.7/quorum_mininode_py/api/
+-rw-rw-rw-   0        0        0       59 2023-03-11 06:14:59.000000 quorum_mininode_py-1.2.7/quorum_mininode_py/api/__init__.py
+-rw-rw-rw-   0        0        0     2281 2023-05-16 12:50:30.000000 quorum_mininode_py-1.2.7/quorum_mininode_py/api/base.py
+-rw-rw-rw-   0        0        0     3812 2023-05-03 11:14:28.000000 quorum_mininode_py-1.2.7/quorum_mininode_py/api/lightnode.py
+drwxrwxrwx   0        0        0        0 2023-05-16 12:57:39.840283 quorum_mininode_py-1.2.7/quorum_mininode_py/client/
+-rw-rw-rw-   0        0        0      134 2023-03-17 17:21:12.000000 quorum_mininode_py-1.2.7/quorum_mininode_py/client/__init__.py
+-rw-rw-rw-   0        0        0     2667 2023-05-16 12:50:32.000000 quorum_mininode_py-1.2.7/quorum_mininode_py/client/_http.py
+-rw-rw-rw-   0        0        0     2625 2023-05-16 12:50:30.000000 quorum_mininode_py-1.2.7/quorum_mininode_py/client/mininode.py
+drwxrwxrwx   0        0        0        0 2023-05-16 12:57:39.850254 quorum_mininode_py-1.2.7/quorum_mininode_py/crypto/
+-rw-rw-rw-   0        0        0      117 2023-03-11 06:14:59.000000 quorum_mininode_py-1.2.7/quorum_mininode_py/crypto/__init__.py
+-rw-rw-rw-   0        0        0     2361 2023-05-03 11:14:57.000000 quorum_mininode_py-1.2.7/quorum_mininode_py/crypto/account.py
+-rw-rw-rw-   0        0        0      517 2023-03-17 17:44:01.000000 quorum_mininode_py-1.2.7/quorum_mininode_py/crypto/aes.py
+-rw-rw-rw-   0        0        0     1824 2023-05-03 11:15:00.000000 quorum_mininode_py-1.2.7/quorum_mininode_py/crypto/age.py
+-rw-rw-rw-   0        0        0     3846 2023-05-03 11:36:39.000000 quorum_mininode_py-1.2.7/quorum_mininode_py/crypto/trx.py
+drwxrwxrwx   0        0        0        0 2023-05-16 12:57:39.854246 quorum_mininode_py-1.2.7/quorum_mininode_py/proto/
+-rw-rw-rw-   0        0        0       87 2023-03-10 05:56:49.000000 quorum_mininode_py-1.2.7/quorum_mininode_py/proto/__init__.py
+-rw-rw-rw-   0        0        0    15822 2023-03-30 04:24:35.000000 quorum_mininode_py-1.2.7/quorum_mininode_py/proto/quorum_pb2.py
+drwxrwxrwx   0        0        0        0 2023-05-16 12:57:39.858234 quorum_mininode_py-1.2.7/quorum_mininode_py/utils/
+-rw-rw-rw-   0        0        0       75 2023-04-28 04:06:26.000000 quorum_mininode_py-1.2.7/quorum_mininode_py/utils/__init__.py
+-rw-rw-rw-   0        0        0     4554 2023-03-30 08:24:57.000000 quorum_mininode_py-1.2.7/quorum_mininode_py/utils/url.py
+drwxrwxrwx   0        0        0        0 2023-05-16 12:57:39.829311 quorum_mininode_py-1.2.7/quorum_mininode_py.egg-info/
+-rw-rw-rw-   0        0        0     2440 2023-05-16 12:57:39.000000 quorum_mininode_py-1.2.7/quorum_mininode_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      798 2023-05-16 12:57:39.000000 quorum_mininode_py-1.2.7/quorum_mininode_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 12:57:39.000000 quorum_mininode_py-1.2.7/quorum_mininode_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-05-16 12:57:39.000000 quorum_mininode_py-1.2.7/quorum_mininode_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-16 12:57:39.000000 quorum_mininode_py-1.2.7/quorum_mininode_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-16 12:57:39.862223 quorum_mininode_py-1.2.7/setup.cfg
+-rw-rw-rw-   0        0        0     1301 2023-05-16 12:47:34.000000 quorum_mininode_py-1.2.7/setup.py
```

### Comparing `quorum_mininode_py-1.2.6/LICENSE` & `quorum_mininode_py-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `quorum_mininode_py-1.2.6/PKG-INFO` & `quorum_mininode_py-1.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quorum_mininode_py
-Version: 1.2.6
+Version: 1.2.7
 Summary: a mini python sdk for quorum lightnode with http/https requests to quorum fullnode
 Home-page: https://github.com/liujuanjuan1984/quorum_mininode_py
 Author: liujuanjuan1984, zhangwm404
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/quorum_mininode_py
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/quorum_mininode_py/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `quorum_mininode_py-1.2.6/README.md` & `quorum_mininode_py-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `quorum_mininode_py-1.2.6/quorum_mininode_py/api/lightnode.py` & `quorum_mininode_py-1.2.7/quorum_mininode_py/api/lightnode.py`

 * *Files identical despite different names*

### Comparing `quorum_mininode_py-1.2.6/quorum_mininode_py/crypto/account.py` & `quorum_mininode_py-1.2.7/quorum_mininode_py/crypto/account.py`

 * *Files identical despite different names*

### Comparing `quorum_mininode_py-1.2.6/quorum_mininode_py/crypto/aes.py` & `quorum_mininode_py-1.2.7/quorum_mininode_py/crypto/aes.py`

 * *Files identical despite different names*

### Comparing `quorum_mininode_py-1.2.6/quorum_mininode_py/crypto/age.py` & `quorum_mininode_py-1.2.7/quorum_mininode_py/crypto/age.py`

 * *Files identical despite different names*

### Comparing `quorum_mininode_py-1.2.6/quorum_mininode_py/crypto/trx.py` & `quorum_mininode_py-1.2.7/quorum_mininode_py/crypto/trx.py`

 * *Files identical despite different names*

### Comparing `quorum_mininode_py-1.2.6/quorum_mininode_py/proto/quorum_pb2.py` & `quorum_mininode_py-1.2.7/quorum_mininode_py/proto/quorum_pb2.py`

 * *Files identical despite different names*

### Comparing `quorum_mininode_py-1.2.6/quorum_mininode_py/utils/url.py` & `quorum_mininode_py-1.2.7/quorum_mininode_py/utils/url.py`

 * *Files identical despite different names*

### Comparing `quorum_mininode_py-1.2.6/quorum_mininode_py.egg-info/PKG-INFO` & `quorum_mininode_py-1.2.7/quorum_mininode_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quorum-mininode-py
-Version: 1.2.6
+Version: 1.2.7
 Summary: a mini python sdk for quorum lightnode with http/https requests to quorum fullnode
 Home-page: https://github.com/liujuanjuan1984/quorum_mininode_py
 Author: liujuanjuan1984, zhangwm404
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/quorum_mininode_py
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/quorum_mininode_py/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `quorum_mininode_py-1.2.6/quorum_mininode_py.egg-info/SOURCES.txt` & `quorum_mininode_py-1.2.7/quorum_mininode_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quorum_mininode_py-1.2.6/setup.py` & `quorum_mininode_py-1.2.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="quorum_mininode_py",
-    version="1.2.6",
+    version="1.2.7",
     author="liujuanjuan1984, zhangwm404",
     author_email="qiaoanlu@163.com",
     description="a mini python sdk for quorum lightnode with http/https requests to quorum fullnode",
     keywords=["rumsystem", "quorum", "lightnode", "sdk"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/liujuanjuan1984/quorum_mininode_py",
```

