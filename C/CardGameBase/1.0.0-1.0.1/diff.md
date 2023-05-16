# Comparing `tmp/CardGameBase-1.0.0.tar.gz` & `tmp/CardGameBase-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CardGameBase-1.0.0.tar", last modified: Tue May 16 11:04:52 2023, max compression
+gzip compressed data, was "CardGameBase-1.0.1.tar", last modified: Tue May 16 13:02:37 2023, max compression
```

## Comparing `CardGameBase-1.0.0.tar` & `CardGameBase-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 11:04:52.452119 CardGameBase-1.0.0/
-drwxrwxrwx   0        0        0        0 2023-05-16 11:04:52.442054 CardGameBase-1.0.0/CardGameBase/
--rw-rw-rw-   0        0        0     3116 2023-05-16 09:08:46.000000 CardGameBase-1.0.0/CardGameBase/Card.py
--rw-rw-rw-   0        0        0     6242 2023-05-16 10:12:24.000000 CardGameBase-1.0.0/CardGameBase/Deck.py
--rw-rw-rw-   0        0        0       39 2023-04-13 10:08:54.000000 CardGameBase-1.0.0/CardGameBase/Exceptions.py
--rw-rw-rw-   0        0        0     7743 2023-05-16 10:42:22.000000 CardGameBase-1.0.0/CardGameBase/Hand.py
--rw-rw-rw-   0        0        0      970 2023-04-14 08:52:08.000000 CardGameBase-1.0.0/CardGameBase/Utility.py
--rw-rw-rw-   0        0        0      119 2023-04-13 10:09:58.000000 CardGameBase-1.0.0/CardGameBase/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 11:04:52.452119 CardGameBase-1.0.0/CardGameBase.egg-info/
--rw-rw-rw-   0        0        0     1509 2023-05-16 11:04:52.000000 CardGameBase-1.0.0/CardGameBase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      344 2023-05-16 11:04:52.000000 CardGameBase-1.0.0/CardGameBase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 11:04:52.000000 CardGameBase-1.0.0/CardGameBase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-16 11:04:52.000000 CardGameBase-1.0.0/CardGameBase.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-16 11:04:52.000000 CardGameBase-1.0.0/CardGameBase.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1235 2023-05-16 07:57:54.000000 CardGameBase-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     1509 2023-05-16 11:04:52.452119 CardGameBase-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      889 2023-05-16 11:03:15.000000 CardGameBase-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-16 11:04:52.452119 CardGameBase-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1208 2023-03-22 11:39:12.000000 CardGameBase-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 13:02:37.930577 CardGameBase-1.0.1/
+drwxrwxrwx   0        0        0        0 2023-05-16 13:02:37.925488 CardGameBase-1.0.1/CardGameBase/
+-rw-rw-rw-   0        0        0     3116 2023-05-16 09:08:46.000000 CardGameBase-1.0.1/CardGameBase/Card.py
+-rw-rw-rw-   0        0        0     6242 2023-05-16 10:12:24.000000 CardGameBase-1.0.1/CardGameBase/Deck.py
+-rw-rw-rw-   0        0        0       39 2023-04-13 10:08:54.000000 CardGameBase-1.0.1/CardGameBase/Exceptions.py
+-rw-rw-rw-   0        0        0     7743 2023-05-16 10:42:22.000000 CardGameBase-1.0.1/CardGameBase/Hand.py
+-rw-rw-rw-   0        0        0      970 2023-04-14 08:52:08.000000 CardGameBase-1.0.1/CardGameBase/Utility.py
+-rw-rw-rw-   0        0        0      119 2023-04-13 10:09:58.000000 CardGameBase-1.0.1/CardGameBase/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 13:02:37.930577 CardGameBase-1.0.1/CardGameBase.egg-info/
+-rw-rw-rw-   0        0        0     1509 2023-05-16 13:02:37.000000 CardGameBase-1.0.1/CardGameBase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      309 2023-05-16 13:02:37.000000 CardGameBase-1.0.1/CardGameBase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 13:02:37.000000 CardGameBase-1.0.1/CardGameBase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-16 13:02:37.000000 CardGameBase-1.0.1/CardGameBase.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1235 2023-05-16 07:57:54.000000 CardGameBase-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     1509 2023-05-16 13:02:37.930577 CardGameBase-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      889 2023-05-16 11:03:15.000000 CardGameBase-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-16 13:02:37.930577 CardGameBase-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1208 2023-05-16 13:02:35.000000 CardGameBase-1.0.1/setup.py
```

### Comparing `CardGameBase-1.0.0/CardGameBase/Card.py` & `CardGameBase-1.0.1/CardGameBase/Card.py`

 * *Files identical despite different names*

### Comparing `CardGameBase-1.0.0/CardGameBase/Deck.py` & `CardGameBase-1.0.1/CardGameBase/Deck.py`

 * *Files identical despite different names*

### Comparing `CardGameBase-1.0.0/CardGameBase/Hand.py` & `CardGameBase-1.0.1/CardGameBase/Hand.py`

 * *Files identical despite different names*

### Comparing `CardGameBase-1.0.0/CardGameBase/Utility.py` & `CardGameBase-1.0.1/CardGameBase/Utility.py`

 * *Files identical despite different names*

### Comparing `CardGameBase-1.0.0/CardGameBase.egg-info/PKG-INFO` & `CardGameBase-1.0.1/CardGameBase.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CardGameBase
-Version: 1.0.0
+Version: 1.0.1
 Summary: Card Game Base with basic deck and card class
 Author: DerSchinken
 Maintainer: DerSchinken
 Project-URL: Source, https://github.com/DerSchinken/CardGameBase/
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `CardGameBase-1.0.0/LICENSE` & `CardGameBase-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `CardGameBase-1.0.0/PKG-INFO` & `CardGameBase-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CardGameBase
-Version: 1.0.0
+Version: 1.0.1
 Summary: Card Game Base with basic deck and card class
 Author: DerSchinken
 Maintainer: DerSchinken
 Project-URL: Source, https://github.com/DerSchinken/CardGameBase/
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `CardGameBase-1.0.0/README.md` & `CardGameBase-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `CardGameBase-1.0.0/setup.py` & `CardGameBase-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Get requirements
 with open("requirements.txt", "r") as reqs:
     requirements = reqs.read().splitlines()
 
 setup(
     name="CardGameBase",
-    version="1.0.0",
+    version="1.0.1",
     # Major version 1
     # Minor version 0
     # Maintenance version 0
 
     author="DerSchinken",
     maintainer="DerSchinken",
     description="Card Game Base with basic deck and card class",
```

