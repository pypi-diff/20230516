# Comparing `tmp/oglio-0.7.5.tar.gz` & `tmp/oglio-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oglio-0.7.5.tar", last modified: Mon May 15 01:04:10 2023, max compression
+gzip compressed data, was "oglio-0.7.6.tar", last modified: Tue May 16 20:01:19 2023, max compression
```

## Comparing `oglio-0.7.5.tar` & `oglio-0.7.6.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-15 01:04:10.641010 oglio-0.7.5/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2022-07-20 17:57:30.000000 oglio-0.7.5/LICENSE
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2335 2023-05-15 01:04:10.640888 oglio-0.7.5/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2011 2023-04-13 20:29:58.000000 oglio-0.7.5/README.md
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-15 01:04:10.638350 oglio-0.7.5/oglio/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1016 2023-05-08 19:24:39.000000 oglio-0.7.5/oglio/IDFactory.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       82 2023-02-13 18:01:45.000000 oglio-0.7.5/oglio/OglVersion.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4580 2023-05-06 14:32:39.000000 oglio-0.7.5/oglio/Reader.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3826 2023-05-06 14:32:39.000000 oglio-0.7.5/oglio/Types.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      123 2022-10-13 12:50:37.000000 oglio-0.7.5/oglio/UnsupportedFileTypeException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2111 2023-05-06 14:32:39.000000 oglio-0.7.5/oglio/Writer.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-05-15 01:03:15.000000 oglio-0.7.5/oglio/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       26 2023-05-15 01:00:40.000000 oglio-0.7.5/oglio/_version.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-08-07 19:55:58.000000 oglio-0.7.5/oglio/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-15 01:04:10.640748 oglio-0.7.5/oglio/toXmlV10/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1913 2023-05-06 19:50:19.000000 oglio-0.7.5/oglio/toXmlV10/BaseOglToDom.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      569 2022-08-26 20:55:45.000000 oglio-0.7.5/oglio/toXmlV10/BasePyutToDom.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      132 2023-05-08 00:21:01.000000 oglio-0.7.5/oglio/toXmlV10/BaseToDom.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1646 2023-05-06 19:50:36.000000 oglio-0.7.5/oglio/toXmlV10/OglClassesToDom.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5803 2023-05-06 19:50:47.000000 oglio-0.7.5/oglio/toXmlV10/OglLinksToDom.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1598 2023-05-06 19:51:01.000000 oglio-0.7.5/oglio/toXmlV10/OglNotesToDom.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2622 2023-05-10 20:43:22.000000 oglio-0.7.5/oglio/toXmlV10/OglSequenceToDom.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1569 2023-05-06 14:32:39.000000 oglio-0.7.5/oglio/toXmlV10/OglTextsToDom.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6676 2023-05-06 14:32:39.000000 oglio-0.7.5/oglio/toXmlV10/OglToDom.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2787 2023-05-06 19:51:31.000000 oglio-0.7.5/oglio/toXmlV10/OglUseCasesToDom.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    14155 2023-05-08 17:31:58.000000 oglio-0.7.5/oglio/toXmlV10/PyutToDom.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3831 2022-08-19 17:25:32.000000 oglio-0.7.5/oglio/toXmlV10/XmlConstants.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-08-16 17:46:46.000000 oglio-0.7.5/oglio/toXmlV10/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-08-07 19:55:58.000000 oglio-0.7.5/oglio/toXmlV10/py.typed
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-15 01:04:10.638940 oglio-0.7.5/oglio.egg-info/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2335 2023-05-15 01:04:10.000000 oglio-0.7.5/oglio.egg-info/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      773 2023-05-15 01:04:10.000000 oglio-0.7.5/oglio.egg-info/SOURCES.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-05-15 01:04:10.000000 oglio-0.7.5/oglio.egg-info/dependency_links.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      105 2023-05-15 01:04:10.000000 oglio-0.7.5/oglio.egg-info/requires.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        6 2023-05-15 01:04:10.000000 oglio-0.7.5/oglio.egg-info/top_level.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-05-15 01:04:10.641044 oglio-0.7.5/setup.cfg
--rw-------   0 humberto.a.sanchez.ii   (501) staff       (20)      966 2023-05-15 01:03:42.000000 oglio-0.7.5/setup.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-16 20:01:19.698501 oglio-0.7.6/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2022-07-20 17:57:30.000000 oglio-0.7.6/LICENSE
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2335 2023-05-16 20:01:19.698375 oglio-0.7.6/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2011 2023-04-13 20:29:58.000000 oglio-0.7.6/README.md
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-16 20:01:19.695731 oglio-0.7.6/oglio/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1016 2023-05-08 19:24:39.000000 oglio-0.7.6/oglio/IDFactory.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       82 2023-02-13 18:01:45.000000 oglio-0.7.6/oglio/OglVersion.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4580 2023-05-06 14:32:39.000000 oglio-0.7.6/oglio/Reader.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3826 2023-05-06 14:32:39.000000 oglio-0.7.6/oglio/Types.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      123 2022-10-13 12:50:37.000000 oglio-0.7.6/oglio/UnsupportedFileTypeException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2111 2023-05-06 14:32:39.000000 oglio-0.7.6/oglio/Writer.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-05-15 01:03:15.000000 oglio-0.7.6/oglio/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       27 2023-05-16 19:47:05.000000 oglio-0.7.6/oglio/_version.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-08-07 19:55:58.000000 oglio-0.7.6/oglio/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-16 20:01:19.698247 oglio-0.7.6/oglio/toXmlV10/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1913 2023-05-06 19:50:19.000000 oglio-0.7.6/oglio/toXmlV10/BaseOglToDom.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      569 2022-08-26 20:55:45.000000 oglio-0.7.6/oglio/toXmlV10/BasePyutToDom.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      132 2023-05-08 00:21:01.000000 oglio-0.7.6/oglio/toXmlV10/BaseToDom.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1646 2023-05-06 19:50:36.000000 oglio-0.7.6/oglio/toXmlV10/OglClassesToDom.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5803 2023-05-06 19:50:47.000000 oglio-0.7.6/oglio/toXmlV10/OglLinksToDom.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1598 2023-05-06 19:51:01.000000 oglio-0.7.6/oglio/toXmlV10/OglNotesToDom.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2622 2023-05-10 20:43:22.000000 oglio-0.7.6/oglio/toXmlV10/OglSequenceToDom.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1569 2023-05-06 14:32:39.000000 oglio-0.7.6/oglio/toXmlV10/OglTextsToDom.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6676 2023-05-06 14:32:39.000000 oglio-0.7.6/oglio/toXmlV10/OglToDom.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2787 2023-05-06 19:51:31.000000 oglio-0.7.6/oglio/toXmlV10/OglUseCasesToDom.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    14155 2023-05-08 17:31:58.000000 oglio-0.7.6/oglio/toXmlV10/PyutToDom.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3831 2022-08-19 17:25:32.000000 oglio-0.7.6/oglio/toXmlV10/XmlConstants.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-08-16 17:46:46.000000 oglio-0.7.6/oglio/toXmlV10/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2022-08-07 19:55:58.000000 oglio-0.7.6/oglio/toXmlV10/py.typed
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-16 20:01:19.696498 oglio-0.7.6/oglio.egg-info/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2335 2023-05-16 20:01:19.000000 oglio-0.7.6/oglio.egg-info/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      773 2023-05-16 20:01:19.000000 oglio-0.7.6/oglio.egg-info/SOURCES.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-05-16 20:01:19.000000 oglio-0.7.6/oglio.egg-info/dependency_links.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      105 2023-05-16 20:01:19.000000 oglio-0.7.6/oglio.egg-info/requires.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        6 2023-05-16 20:01:19.000000 oglio-0.7.6/oglio.egg-info/top_level.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-05-16 20:01:19.698533 oglio-0.7.6/setup.cfg
+-rw-------   0 humberto.a.sanchez.ii   (501) staff       (20)      966 2023-05-16 19:54:59.000000 oglio-0.7.6/setup.py
```

### Comparing `oglio-0.7.5/LICENSE` & `oglio-0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `oglio-0.7.5/PKG-INFO` & `oglio-0.7.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oglio
-Version: 0.7.5
+Version: 0.7.6
 Summary: External Pyut Persistence
 Home-page: https://github.com/hasii2011/oglio
 Author-email: Humberto.A.Sanchez.II@gmail.com
 Maintainer: Humberto A. Sanchez II
 Maintainer-email: humberto.a.sanchez.ii@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: oglio Version: 0.7.5 Summary: External Pyut
+Metadata-Version: 2.1 Name: oglio Version: 0.7.6 Summary: External Pyut
 Persistence Home-page: https://github.com/hasii2011/oglio Author-email:
 Humberto.A.Sanchez.II@gmail.com Maintainer: Humberto A. Sanchez II Maintainer-
 email: humberto.a.sanchez.ii@gmail.com Description-Content-Type: text/markdown
 License-File: LICENSE [./docs/agpl-license-web-badge-version-2-256x48.png] [!
 [Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https:
 //GitHub.com/Naereen/StrapDown.js/graphs/commit-activity) [![CircleCI](https://
 dl.circleci.com/status-badge/img/gh/hasii2011/oglio/tree/
```

### Comparing `oglio-0.7.5/README.md` & `oglio-0.7.6/README.md`

 * *Files identical despite different names*

### Comparing `oglio-0.7.5/oglio/IDFactory.py` & `oglio-0.7.6/oglio/IDFactory.py`

 * *Files identical despite different names*

### Comparing `oglio-0.7.5/oglio/Reader.py` & `oglio-0.7.6/oglio/Reader.py`

 * *Files identical despite different names*

### Comparing `oglio-0.7.5/oglio/Types.py` & `oglio-0.7.6/oglio/Types.py`

 * *Files identical despite different names*

### Comparing `oglio-0.7.5/oglio/Writer.py` & `oglio-0.7.6/oglio/Writer.py`

 * *Files identical despite different names*

### Comparing `oglio-0.7.5/oglio/toXmlV10/BaseOglToDom.py` & `oglio-0.7.6/oglio/toXmlV10/BaseOglToDom.py`

 * *Files identical despite different names*

### Comparing `oglio-0.7.5/oglio/toXmlV10/BasePyutToDom.py` & `oglio-0.7.6/oglio/toXmlV10/BasePyutToDom.py`

 * *Files identical despite different names*

### Comparing `oglio-0.7.5/oglio/toXmlV10/OglClassesToDom.py` & `oglio-0.7.6/oglio/toXmlV10/OglClassesToDom.py`

 * *Files identical despite different names*

### Comparing `oglio-0.7.5/oglio/toXmlV10/OglLinksToDom.py` & `oglio-0.7.6/oglio/toXmlV10/OglLinksToDom.py`

 * *Files identical despite different names*

### Comparing `oglio-0.7.5/oglio/toXmlV10/OglNotesToDom.py` & `oglio-0.7.6/oglio/toXmlV10/OglNotesToDom.py`

 * *Files identical despite different names*

### Comparing `oglio-0.7.5/oglio/toXmlV10/OglSequenceToDom.py` & `oglio-0.7.6/oglio/toXmlV10/OglSequenceToDom.py`

 * *Files identical despite different names*

### Comparing `oglio-0.7.5/oglio/toXmlV10/OglTextsToDom.py` & `oglio-0.7.6/oglio/toXmlV10/OglTextsToDom.py`

 * *Files identical despite different names*

### Comparing `oglio-0.7.5/oglio/toXmlV10/OglToDom.py` & `oglio-0.7.6/oglio/toXmlV10/OglToDom.py`

 * *Files identical despite different names*

### Comparing `oglio-0.7.5/oglio/toXmlV10/OglUseCasesToDom.py` & `oglio-0.7.6/oglio/toXmlV10/OglUseCasesToDom.py`

 * *Files identical despite different names*

### Comparing `oglio-0.7.5/oglio/toXmlV10/PyutToDom.py` & `oglio-0.7.6/oglio/toXmlV10/PyutToDom.py`

 * *Files identical despite different names*

### Comparing `oglio-0.7.5/oglio/toXmlV10/XmlConstants.py` & `oglio-0.7.6/oglio/toXmlV10/XmlConstants.py`

 * *Files identical despite different names*

### Comparing `oglio-0.7.5/oglio.egg-info/PKG-INFO` & `oglio-0.7.6/oglio.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oglio
-Version: 0.7.5
+Version: 0.7.6
 Summary: External Pyut Persistence
 Home-page: https://github.com/hasii2011/oglio
 Author-email: Humberto.A.Sanchez.II@gmail.com
 Maintainer: Humberto A. Sanchez II
 Maintainer-email: humberto.a.sanchez.ii@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: oglio Version: 0.7.5 Summary: External Pyut
+Metadata-Version: 2.1 Name: oglio Version: 0.7.6 Summary: External Pyut
 Persistence Home-page: https://github.com/hasii2011/oglio Author-email:
 Humberto.A.Sanchez.II@gmail.com Maintainer: Humberto A. Sanchez II Maintainer-
 email: humberto.a.sanchez.ii@gmail.com Description-Content-Type: text/markdown
 License-File: LICENSE [./docs/agpl-license-web-badge-version-2-256x48.png] [!
 [Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https:
 //GitHub.com/Naereen/StrapDown.js/graphs/commit-activity) [![CircleCI](https://
 dl.circleci.com/status-badge/img/gh/hasii2011/oglio/tree/
```

### Comparing `oglio-0.7.5/oglio.egg-info/SOURCES.txt` & `oglio-0.7.6/oglio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oglio-0.7.5/setup.py` & `oglio-0.7.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,10 +22,10 @@
     packages=[
         'oglio', 'oglio.toXmlV10'
     ],
     package_data={
         'oglio':          ['py.typed'],
         'oglio.toXmlV10': ['py.typed']
     },
-    install_requires=['wxPython==4.2.0', 'hasiihelper~=0.2.0', 'hasiicommon~=0.2.2', 'pyutmodel~=1.4.3', 'ogl==0.70.30', 'untanglepyut==0.6.61',
+    install_requires=['wxPython==4.2.0', 'hasiihelper~=0.2.0', 'hasiicommon~=0.2.2', 'pyutmodel~=1.4.3', 'ogl==0.70.40', 'untanglepyut==0.6.62',
     ],
 )
```
