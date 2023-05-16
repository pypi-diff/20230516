# Comparing `tmp/shayhan-0.0.1.tar.gz` & `tmp/shayhan-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shayhan-0.0.1.tar", last modified: Sat May 21 23:43:31 2022, max compression
+gzip compressed data, was "shayhan-0.0.2.tar", last modified: Tue May 16 11:15:55 2023, max compression
```

## Comparing `shayhan-0.0.1.tar` & `shayhan-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2022-05-21 23:43:31.045198 shayhan-0.0.1/
--rw-rw-rw-   0        0        0       89 2022-05-21 23:22:54.000000 shayhan-0.0.1/CHANGELOG.md
--rw-rw-rw-   0        0        0     1083 2022-05-21 23:27:50.000000 shayhan-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0       30 2022-05-21 23:35:18.000000 shayhan-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      671 2022-05-21 23:43:31.045198 shayhan-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       34 2022-05-21 23:14:55.000000 shayhan-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2022-05-21 23:43:31.045198 shayhan-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      708 2022-05-21 23:30:33.000000 shayhan-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2022-05-21 23:43:31.013958 shayhan-0.0.1/shayhan/
--rw-rw-rw-   0        0        0     1245 2022-05-21 23:09:21.000000 shayhan-0.0.1/shayhan/__init__.py
-drwxrwxrwx   0        0        0        0 2022-05-21 23:43:31.045198 shayhan-0.0.1/shayhan.egg-info/
--rw-rw-rw-   0        0        0      671 2022-05-21 23:43:30.000000 shayhan-0.0.1/shayhan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      199 2022-05-21 23:43:30.000000 shayhan-0.0.1/shayhan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-05-21 23:43:30.000000 shayhan-0.0.1/shayhan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2022-05-21 23:43:30.000000 shayhan-0.0.1/shayhan.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 11:15:55.464717 shayhan-0.0.2/
+-rw-rw-rw-   0        0        0      241 2023-05-16 11:08:24.000000 shayhan-0.0.2/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1083 2022-05-21 23:27:50.000000 shayhan-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       30 2022-05-21 23:35:18.000000 shayhan-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      795 2023-05-16 11:15:55.464717 shayhan-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       34 2022-05-21 23:14:55.000000 shayhan-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-16 11:15:55.465715 shayhan-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      708 2023-05-16 11:08:58.000000 shayhan-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 11:15:55.453715 shayhan-0.0.2/shayhan/
+-rw-rw-rw-   0        0        0     4387 2023-05-16 11:04:18.000000 shayhan-0.0.2/shayhan/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 11:15:55.462718 shayhan-0.0.2/shayhan.egg-info/
+-rw-rw-rw-   0        0        0      795 2023-05-16 11:15:55.000000 shayhan-0.0.2/shayhan.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      199 2023-05-16 11:15:55.000000 shayhan-0.0.2/shayhan.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 11:15:55.000000 shayhan-0.0.2/shayhan.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-16 11:15:55.000000 shayhan-0.0.2/shayhan.egg-info/top_level.txt
```

### Comparing `shayhan-0.0.1/LICENSE.txt` & `shayhan-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `shayhan-0.0.1/PKG-INFO` & `shayhan-0.0.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 Metadata-Version: 2.1
 Name: shayhan
-Version: 0.0.1
+Version: 0.0.2
 Summary: This is a libriry of some fuctions
-Home-page: UNKNOWN
+Home-page: 
 Author: Shayhan Ameen Chowdhury
 Author-email: shayhan.ameen@gmail.com
 License: MIT
 Keywords: print
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE.txt
 
 This is a libriry of some fuctions
 
 Change Log
 ============
 
+0.0.2 (May 16, 2023)
+----------------------
+- Can now display information of multiple variables in a table
+- Support torch, tensorflow ans sparse
+
 0.0.1 (May 22, 2022)
 ----------------------
 - First Release
-
```

### Comparing `shayhan-0.0.1/shayhan.egg-info/PKG-INFO` & `shayhan-0.0.2/shayhan.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 Metadata-Version: 2.1
 Name: shayhan
-Version: 0.0.1
+Version: 0.0.2
 Summary: This is a libriry of some fuctions
-Home-page: UNKNOWN
+Home-page: 
 Author: Shayhan Ameen Chowdhury
 Author-email: shayhan.ameen@gmail.com
 License: MIT
 Keywords: print
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE.txt
 
 This is a libriry of some fuctions
 
 Change Log
 ============
 
+0.0.2 (May 16, 2023)
+----------------------
+- Can now display information of multiple variables in a table
+- Support torch, tensorflow ans sparse
+
 0.0.1 (May 22, 2022)
 ----------------------
 - First Release
-
```

