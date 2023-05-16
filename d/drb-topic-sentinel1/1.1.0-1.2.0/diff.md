# Comparing `tmp/drb-topic-sentinel1-1.1.0.tar.gz` & `tmp/drb-topic-sentinel1-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drb-topic-sentinel1-1.1.0.tar", last modified: Tue Jan  3 10:51:46 2023, max compression
+gzip compressed data, was "drb-topic-sentinel1-1.2.0.tar", last modified: Tue May 16 12:17:16 2023, max compression
```

## Comparing `drb-topic-sentinel1-1.1.0.tar` & `drb-topic-sentinel1-1.2.0.tar`

### file list

```diff
@@ -1,36 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 10:51:46.052255 drb-topic-sentinel1-1.1.0/
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-01-03 09:34:17.000000 drb-topic-sentinel1-1.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8180 2023-01-03 10:51:46.052255 drb-topic-sentinel1-1.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     7699 2023-01-03 09:34:17.000000 drb-topic-sentinel1-1.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 10:51:46.044255 drb-topic-sentinel1-1.1.0/drb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 10:51:46.044255 drb-topic-sentinel1-1.1.0/drb/topics/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 10:51:46.052255 drb-topic-sentinel1-1.1.0/drb/topics/sentinel1/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-01-03 09:34:17.000000 drb-topic-sentinel1-1.1.0/drb/topics/sentinel1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2023-01-03 10:51:46.052255 drb-topic-sentinel1-1.1.0/drb/topics/sentinel1/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 10:51:46.048255 drb-topic-sentinel1-1.1.0/drb/topics/sentinel1/auxiliary/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 09:34:17.000000 drb-topic-sentinel1-1.1.0/drb/topics/sentinel1/auxiliary/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3326 2023-01-03 09:34:17.000000 drb-topic-sentinel1-1.1.0/drb/topics/sentinel1/auxiliary/cortex.yml
--rw-rw-rw-   0 root         (0) root         (0)     1144 2023-01-03 09:34:17.000000 drb-topic-sentinel1-1.1.0/drb/topics/sentinel1/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 10:51:46.048255 drb-topic-sentinel1-1.1.0/drb/topics/sentinel1/eof/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 09:34:17.000000 drb-topic-sentinel1-1.1.0/drb/topics/sentinel1/eof/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4215 2023-01-03 09:34:17.000000 drb-topic-sentinel1-1.1.0/drb/topics/sentinel1/eof/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 10:51:46.048255 drb-topic-sentinel1-1.1.0/drb/topics/sentinel1/level0/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 09:34:17.000000 drb-topic-sentinel1-1.1.0/drb/topics/sentinel1/level0/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6873 2023-01-03 09:34:17.000000 drb-topic-sentinel1-1.1.0/drb/topics/sentinel1/level0/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 10:51:46.048255 drb-topic-sentinel1-1.1.0/drb/topics/sentinel1/level1/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 09:34:17.000000 drb-topic-sentinel1-1.1.0/drb/topics/sentinel1/level1/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4634 2023-01-03 09:34:17.000000 drb-topic-sentinel1-1.1.0/drb/topics/sentinel1/level1/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 10:51:46.052255 drb-topic-sentinel1-1.1.0/drb/topics/sentinel1/level2/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 09:34:17.000000 drb-topic-sentinel1-1.1.0/drb/topics/sentinel1/level2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2136 2023-01-03 09:34:17.000000 drb-topic-sentinel1-1.1.0/drb/topics/sentinel1/level2/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 10:51:46.052255 drb-topic-sentinel1-1.1.0/drb_topic_sentinel1.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8180 2023-01-03 10:51:45.000000 drb-topic-sentinel1-1.1.0/drb_topic_sentinel1.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      824 2023-01-03 10:51:45.000000 drb-topic-sentinel1-1.1.0/drb_topic_sentinel1.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-03 10:51:45.000000 drb-topic-sentinel1-1.1.0/drb_topic_sentinel1.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      267 2023-01-03 10:51:45.000000 drb-topic-sentinel1-1.1.0/drb_topic_sentinel1.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       33 2023-01-03 10:51:45.000000 drb-topic-sentinel1-1.1.0/drb_topic_sentinel1.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-01-03 10:51:45.000000 drb-topic-sentinel1-1.1.0/drb_topic_sentinel1.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       34 2023-01-03 09:34:17.000000 drb-topic-sentinel1-1.1.0/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      218 2023-01-03 10:51:46.052255 drb-topic-sentinel1-1.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1702 2023-01-03 10:38:59.000000 drb-topic-sentinel1-1.1.0/setup.py
--rw-rw-rw-   0 root         (0) root         (0)    83021 2023-01-03 09:34:17.000000 drb-topic-sentinel1-1.1.0/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 12:17:16.759591 drb-topic-sentinel1-1.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     7651 2023-01-19 14:29:34.000000 drb-topic-sentinel1-1.2.0/LICENCE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-01-03 09:34:17.000000 drb-topic-sentinel1-1.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8167 2023-05-16 12:17:16.759591 drb-topic-sentinel1-1.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     7699 2023-01-03 09:34:17.000000 drb-topic-sentinel1-1.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 12:17:16.739591 drb-topic-sentinel1-1.2.0/drb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 12:17:16.739591 drb-topic-sentinel1-1.2.0/drb/topics/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 12:17:16.763591 drb-topic-sentinel1-1.2.0/drb/topics/sentinel1/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-01-03 09:34:17.000000 drb-topic-sentinel1-1.2.0/drb/topics/sentinel1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-05-16 12:17:16.763591 drb-topic-sentinel1-1.2.0/drb/topics/sentinel1/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 12:17:16.751591 drb-topic-sentinel1-1.2.0/drb/topics/sentinel1/auxiliary/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 09:34:17.000000 drb-topic-sentinel1-1.2.0/drb/topics/sentinel1/auxiliary/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3326 2023-05-16 12:16:36.000000 drb-topic-sentinel1-1.2.0/drb/topics/sentinel1/auxiliary/cortex.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1144 2023-05-16 12:16:36.000000 drb-topic-sentinel1-1.2.0/drb/topics/sentinel1/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 12:17:16.751591 drb-topic-sentinel1-1.2.0/drb/topics/sentinel1/eof/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 09:34:17.000000 drb-topic-sentinel1-1.2.0/drb/topics/sentinel1/eof/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4215 2023-05-16 12:16:36.000000 drb-topic-sentinel1-1.2.0/drb/topics/sentinel1/eof/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 12:17:16.755591 drb-topic-sentinel1-1.2.0/drb/topics/sentinel1/level0/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 09:34:17.000000 drb-topic-sentinel1-1.2.0/drb/topics/sentinel1/level0/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6873 2023-05-16 12:16:36.000000 drb-topic-sentinel1-1.2.0/drb/topics/sentinel1/level0/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 12:17:16.755591 drb-topic-sentinel1-1.2.0/drb/topics/sentinel1/level1/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 09:34:17.000000 drb-topic-sentinel1-1.2.0/drb/topics/sentinel1/level1/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4634 2023-05-16 12:16:36.000000 drb-topic-sentinel1-1.2.0/drb/topics/sentinel1/level1/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 12:17:16.755591 drb-topic-sentinel1-1.2.0/drb/topics/sentinel1/level2/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 09:34:17.000000 drb-topic-sentinel1-1.2.0/drb/topics/sentinel1/level2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2136 2023-05-16 12:16:36.000000 drb-topic-sentinel1-1.2.0/drb/topics/sentinel1/level2/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 12:17:16.759591 drb-topic-sentinel1-1.2.0/drb_topic_sentinel1.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8167 2023-05-16 12:17:16.000000 drb-topic-sentinel1-1.2.0/drb_topic_sentinel1.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      924 2023-05-16 12:17:16.000000 drb-topic-sentinel1-1.2.0/drb_topic_sentinel1.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 12:17:16.000000 drb-topic-sentinel1-1.2.0/drb_topic_sentinel1.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      266 2023-05-16 12:17:16.000000 drb-topic-sentinel1-1.2.0/drb_topic_sentinel1.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 12:17:16.000000 drb-topic-sentinel1-1.2.0/drb_topic_sentinel1.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       33 2023-05-16 12:17:16.000000 drb-topic-sentinel1-1.2.0/drb_topic_sentinel1.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-16 12:17:16.000000 drb-topic-sentinel1-1.2.0/drb_topic_sentinel1.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-05-16 09:58:12.000000 drb-topic-sentinel1-1.2.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       34 2023-05-16 09:58:12.000000 drb-topic-sentinel1-1.2.0/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1419 2023-05-16 12:17:16.763591 drb-topic-sentinel1-1.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      135 2023-05-16 09:58:12.000000 drb-topic-sentinel1-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 12:17:16.759591 drb-topic-sentinel1-1.2.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      788 2023-01-03 09:34:17.000000 drb-topic-sentinel1-1.2.0/tests/test_sentinel1_topics.py
+-rw-rw-rw-   0 root         (0) root         (0)    83021 2023-01-03 09:34:17.000000 drb-topic-sentinel1-1.2.0/versioneer.py
```

### Comparing `drb-topic-sentinel1-1.1.0/PKG-INFO` & `drb-topic-sentinel1-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: drb-topic-sentinel1
-Version: 1.1.0
+Version: 1.2.0
 Summary: Sentinel-1 topic for DRB Python
-Home-page: https://gitlab.com/drb-python/topics/sentinel-1
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: Apache Software License
+License: LGPLv3
+Project-URL: Source, https://gitlab.com/drb-python/topics/sentinel-1
 Classifier: Programming Language :: Python :: 3.8
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENCE.txt
 
 # drb-topic-sentinel1
 The `drb-topic-sentinel1` is a DRB plugin declaring topics about
 [Sentinel-1](https://sentinels.copernicus.eu/web/sentinel/missions/sentinel-1)
 EO satellite.
 
 ## Installation
@@ -168,9 +167,7 @@
     RESORB([Sentinel-1 EOF Restituted Orbit File Auxiliary Product<br/>1462dbde-5f3b-4adf-98da-ecd66ceaebbd])
     POEORB([Sentinel-1 EOF Precise Orbit Ephemerides Orbit File Auxiliary Product<br/>f82c26d7-26fd-406d-beeb-3230733c0d0b])
     PREORB([Sentinel-1 EOF Predicted Orbit File Auxiliary Product<br/>0bb12b1e-deed-4dec-aaa5-bdf663aaa6b9])
 
     MPL & AMH & AMV & POD --> EOF
     RESORB & POEORB & PREORB --> POD
 ```
-
-
```

### Comparing `drb-topic-sentinel1-1.1.0/README.md` & `drb-topic-sentinel1-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `drb-topic-sentinel1-1.1.0/drb/topics/sentinel1/auxiliary/cortex.yml` & `drb-topic-sentinel1-1.2.0/drb/topics/sentinel1/auxiliary/cortex.yml`

 * *Files identical despite different names*

### Comparing `drb-topic-sentinel1-1.1.0/drb/topics/sentinel1/cortex.yml` & `drb-topic-sentinel1-1.2.0/drb/topics/sentinel1/cortex.yml`

 * *Files identical despite different names*

### Comparing `drb-topic-sentinel1-1.1.0/drb/topics/sentinel1/eof/cortex.yml` & `drb-topic-sentinel1-1.2.0/drb/topics/sentinel1/eof/cortex.yml`

 * *Files identical despite different names*

### Comparing `drb-topic-sentinel1-1.1.0/drb/topics/sentinel1/level0/cortex.yml` & `drb-topic-sentinel1-1.2.0/drb/topics/sentinel1/level0/cortex.yml`

 * *Files identical despite different names*

### Comparing `drb-topic-sentinel1-1.1.0/drb/topics/sentinel1/level1/cortex.yml` & `drb-topic-sentinel1-1.2.0/drb/topics/sentinel1/level1/cortex.yml`

 * *Files identical despite different names*

### Comparing `drb-topic-sentinel1-1.1.0/drb/topics/sentinel1/level2/cortex.yml` & `drb-topic-sentinel1-1.2.0/drb/topics/sentinel1/level2/cortex.yml`

 * *Files identical despite different names*

### Comparing `drb-topic-sentinel1-1.1.0/drb_topic_sentinel1.egg-info/PKG-INFO` & `drb-topic-sentinel1-1.2.0/drb_topic_sentinel1.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: drb-topic-sentinel1
-Version: 1.1.0
+Version: 1.2.0
 Summary: Sentinel-1 topic for DRB Python
-Home-page: https://gitlab.com/drb-python/topics/sentinel-1
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: Apache Software License
+License: LGPLv3
+Project-URL: Source, https://gitlab.com/drb-python/topics/sentinel-1
 Classifier: Programming Language :: Python :: 3.8
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENCE.txt
 
 # drb-topic-sentinel1
 The `drb-topic-sentinel1` is a DRB plugin declaring topics about
 [Sentinel-1](https://sentinels.copernicus.eu/web/sentinel/missions/sentinel-1)
 EO satellite.
 
 ## Installation
@@ -168,9 +167,7 @@
     RESORB([Sentinel-1 EOF Restituted Orbit File Auxiliary Product<br/>1462dbde-5f3b-4adf-98da-ecd66ceaebbd])
     POEORB([Sentinel-1 EOF Precise Orbit Ephemerides Orbit File Auxiliary Product<br/>f82c26d7-26fd-406d-beeb-3230733c0d0b])
     PREORB([Sentinel-1 EOF Predicted Orbit File Auxiliary Product<br/>0bb12b1e-deed-4dec-aaa5-bdf663aaa6b9])
 
     MPL & AMH & AMV & POD --> EOF
     RESORB & POEORB & PREORB --> POD
 ```
-
-
```

### Comparing `drb-topic-sentinel1-1.1.0/drb_topic_sentinel1.egg-info/SOURCES.txt` & `drb-topic-sentinel1-1.2.0/drb_topic_sentinel1.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+LICENCE.txt
 MANIFEST.in
 README.md
+pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 versioneer.py
 drb/topics/sentinel1/__init__.py
 drb/topics/sentinel1/_version.py
 drb/topics/sentinel1/cortex.yml
@@ -17,9 +19,11 @@
 drb/topics/sentinel1/level1/cortex.yml
 drb/topics/sentinel1/level2/__init__.py
 drb/topics/sentinel1/level2/cortex.yml
 drb_topic_sentinel1.egg-info/PKG-INFO
 drb_topic_sentinel1.egg-info/SOURCES.txt
 drb_topic_sentinel1.egg-info/dependency_links.txt
 drb_topic_sentinel1.egg-info/entry_points.txt
+drb_topic_sentinel1.egg-info/not-zip-safe
 drb_topic_sentinel1.egg-info/requires.txt
-drb_topic_sentinel1.egg-info/top_level.txt
+drb_topic_sentinel1.egg-info/top_level.txt
+tests/test_sentinel1_topics.py
```

### Comparing `drb-topic-sentinel1-1.1.0/setup.py` & `drb-topic-sentinel1-1.2.0/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,48 +1,61 @@
-import versioneer
-from setuptools import setup, find_namespace_packages
+[metadata]
+name = drb-topic-sentinel1
+author = GAEL Systems
+author_email = drb-python@gael.fr
+description = Sentinel-1 topic for DRB Python
+long_description = file: README.md
+long_description_content_type = text/markdown
+license = LGPLv3
+classifiers = 
+	Programming Language :: Python :: 3.8
+	License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
+project_urls = 
+	Source = https://gitlab.com/drb-python/topics/sentinel-1
 
-with open('requirements.txt', 'r') as file:
-    REQUIREMENTS = file.readlines()
+[options]
+zip_safe = False
+include_package_data = True
+packages = find_namespace:
+python_requires = >=3.8
+install_requires = file: requirements.txt
 
-with open('README.md', 'r') as file:
-    long_description = file.read()
+[options.packages.find]
+exclude = 
+	tests*
+	docs*
 
+[options.package_data]
+drb.topics.sentinel1 = 
+	cortex.yml
+drb.topics.sentinel1.level0 = 
+	cortex.yml
+drb.topics.sentinel1.level1 = 
+	cortex.yml
+drb.topics.sentinel1.level2 = 
+	cortex.yml
+drb.topics.sentinel1.auxiliary = 
+	cortex.yml
+drb.topics.sentinel1.eof = 
+	cortex.yml
+
+[options.entry_points]
+drb.topic = 
+	sentinel1=drb.topics.sentinel1
+	sentinel1_l0=drb.topics.sentinel1.level0
+	sentinel1_l1=drb.topics.sentinel1.level1
+	sentinel1_l2=drb.topics.sentinel1.level2
+	sentinel1_aux=drb.topics.sentinel1.auxiliary
+	sentinel1_eof_aux=drb.topics.sentinel1.eof
+
+[versioneer]
+VCS = git
+style = pep440
+versionfile_source = drb/topics/sentinel1/_version.py
+versionfile_build = drb/topics/sentinel1/_version.py
+tag_prefix = 
+parentdir_prefix = 
+
+[egg_info]
+tag_build = 
+tag_date = 0
 
-setup(
-    name='drb-topic-sentinel1',
-    description='Sentinel-1 topic for DRB Python',
-    long_description=long_description,
-    long_description_content_type='text/markdown',
-    author='GAEL Systems',
-    author_email='drb-python@gael.fr',
-    url='https://gitlab.com/drb-python/topics/sentinel-1',
-    python_requires='>=3.8',
-    install_requires=REQUIREMENTS,
-    packages=find_namespace_packages(include=['drb.*']),
-    classifiers=[
-        "Programming Language :: Python :: 3.8",
-        "License :: OSI Approved :: Apache Software License",
-        "Programming Language :: Python :: 3.8",
-    ],
-    package_data={
-        'drb.topics.sentinel1': ['cortex.yml'],
-        'drb.topics.sentinel1.level0': ['cortex.yml'],
-        'drb.topics.sentinel1.level1': ['cortex.yml'],
-        'drb.topics.sentinel1.level2': ['cortex.yml'],
-        'drb.topics.sentinel1.auxiliary': ['cortex.yml'],
-        'drb.topics.sentinel1.eof': ['cortex.yml']
-    },
-    data_files=[('.', ['requirements.txt'])],
-    entry_points={
-        'drb.topic': [
-            'sentinel1=drb.topics.sentinel1',
-            'sentinel1_l0=drb.topics.sentinel1.level0',
-            'sentinel1_l1=drb.topics.sentinel1.level1',
-            'sentinel1_l2=drb.topics.sentinel1.level2',
-            'sentinel1_aux=drb.topics.sentinel1.auxiliary',
-            'sentinel1_eof_aux=drb.topics.sentinel1.eof'
-        ]
-    },
-    version=versioneer.get_version(),
-    cmdclass=versioneer.get_cmdclass()
-)
```

### Comparing `drb-topic-sentinel1-1.1.0/versioneer.py` & `drb-topic-sentinel1-1.2.0/versioneer.py`

 * *Files identical despite different names*

