# Comparing `tmp/drb-topic-sentinel2-1.1.0.tar.gz` & `tmp/drb-topic-sentinel2-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drb-topic-sentinel2-1.1.0.tar", last modified: Tue Jan  3 13:23:42 2023, max compression
+gzip compressed data, was "drb-topic-sentinel2-1.2.0.tar", last modified: Tue May 16 13:28:20 2023, max compression
```

## Comparing `drb-topic-sentinel2-1.1.0.tar` & `drb-topic-sentinel2-1.2.0.tar`

### file list

```diff
@@ -1,36 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 13:23:42.665843 drb-topic-sentinel2-1.1.0/
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-01-03 10:30:21.000000 drb-topic-sentinel2-1.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6052 2023-01-03 13:23:42.669843 drb-topic-sentinel2-1.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5572 2022-07-25 14:59:39.000000 drb-topic-sentinel2-1.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 13:23:42.661842 drb-topic-sentinel2-1.1.0/drb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 13:23:42.661842 drb-topic-sentinel2-1.1.0/drb/topics/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 13:23:42.669843 drb-topic-sentinel2-1.1.0/drb/topics/sentinel2/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-01-03 10:30:21.000000 drb-topic-sentinel2-1.1.0/drb/topics/sentinel2/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2023-01-03 13:23:42.669843 drb-topic-sentinel2-1.1.0/drb/topics/sentinel2/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 13:23:42.665843 drb-topic-sentinel2-1.1.0/drb/topics/sentinel2/aux/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:30:21.000000 drb-topic-sentinel2-1.1.0/drb/topics/sentinel2/aux/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4448 2023-01-03 10:30:21.000000 drb-topic-sentinel2-1.1.0/drb/topics/sentinel2/aux/cortex.yml
--rw-rw-rw-   0 root         (0) root         (0)      503 2023-01-03 10:30:21.000000 drb-topic-sentinel2-1.1.0/drb/topics/sentinel2/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 13:23:42.665843 drb-topic-sentinel2-1.1.0/drb/topics/sentinel2/pdi/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:30:21.000000 drb-topic-sentinel2-1.1.0/drb/topics/sentinel2/pdi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2171 2023-01-03 10:30:21.000000 drb-topic-sentinel2-1.1.0/drb/topics/sentinel2/pdi/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 13:23:42.665843 drb-topic-sentinel2-1.1.0/drb/topics/sentinel2/pdi/datastrip/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:30:21.000000 drb-topic-sentinel2-1.1.0/drb/topics/sentinel2/pdi/datastrip/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5290 2023-01-03 10:30:21.000000 drb-topic-sentinel2-1.1.0/drb/topics/sentinel2/pdi/datastrip/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 13:23:42.665843 drb-topic-sentinel2-1.1.0/drb/topics/sentinel2/pdi/granule/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:30:21.000000 drb-topic-sentinel2-1.1.0/drb/topics/sentinel2/pdi/granule/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5030 2023-01-03 10:30:21.000000 drb-topic-sentinel2-1.1.0/drb/topics/sentinel2/pdi/granule/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 13:23:42.665843 drb-topic-sentinel2-1.1.0/drb/topics/sentinel2/user/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:30:21.000000 drb-topic-sentinel2-1.1.0/drb/topics/sentinel2/user/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3875 2023-01-03 10:30:21.000000 drb-topic-sentinel2-1.1.0/drb/topics/sentinel2/user/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 13:23:42.665843 drb-topic-sentinel2-1.1.0/drb_topic_sentinel2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6052 2023-01-03 13:23:42.000000 drb-topic-sentinel2-1.1.0/drb_topic_sentinel2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      832 2023-01-03 13:23:42.000000 drb-topic-sentinel2-1.1.0/drb_topic_sentinel2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-03 13:23:42.000000 drb-topic-sentinel2-1.1.0/drb_topic_sentinel2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      269 2023-01-03 13:23:42.000000 drb-topic-sentinel2-1.1.0/drb_topic_sentinel2.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-01-03 13:23:42.000000 drb-topic-sentinel2-1.1.0/drb_topic_sentinel2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-01-03 13:23:42.000000 drb-topic-sentinel2-1.1.0/drb_topic_sentinel2.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       56 2023-01-03 10:30:21.000000 drb-topic-sentinel2-1.1.0/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      218 2023-01-03 13:23:42.669843 drb-topic-sentinel2-1.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1708 2023-01-03 10:39:45.000000 drb-topic-sentinel2-1.1.0/setup.py
--rw-rw-rw-   0 root         (0) root         (0)    83607 2023-01-03 10:30:21.000000 drb-topic-sentinel2-1.1.0/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 13:28:20.754413 drb-topic-sentinel2-1.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     7651 2023-01-19 15:45:26.000000 drb-topic-sentinel2-1.2.0/LICENCE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-01-03 10:30:21.000000 drb-topic-sentinel2-1.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6040 2023-05-16 13:28:20.754413 drb-topic-sentinel2-1.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5572 2022-07-25 14:59:39.000000 drb-topic-sentinel2-1.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 13:28:20.738412 drb-topic-sentinel2-1.2.0/drb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 13:28:20.738412 drb-topic-sentinel2-1.2.0/drb/topics/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 13:28:20.754413 drb-topic-sentinel2-1.2.0/drb/topics/sentinel2/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-01-03 10:30:21.000000 drb-topic-sentinel2-1.2.0/drb/topics/sentinel2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-05-16 13:28:20.754413 drb-topic-sentinel2-1.2.0/drb/topics/sentinel2/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 13:28:20.750413 drb-topic-sentinel2-1.2.0/drb/topics/sentinel2/aux/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:30:21.000000 drb-topic-sentinel2-1.2.0/drb/topics/sentinel2/aux/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4448 2023-05-16 13:27:43.000000 drb-topic-sentinel2-1.2.0/drb/topics/sentinel2/aux/cortex.yml
+-rw-rw-rw-   0 root         (0) root         (0)      503 2023-05-16 13:27:43.000000 drb-topic-sentinel2-1.2.0/drb/topics/sentinel2/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 13:28:20.750413 drb-topic-sentinel2-1.2.0/drb/topics/sentinel2/pdi/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:30:21.000000 drb-topic-sentinel2-1.2.0/drb/topics/sentinel2/pdi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2171 2023-05-16 13:27:43.000000 drb-topic-sentinel2-1.2.0/drb/topics/sentinel2/pdi/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 13:28:20.750413 drb-topic-sentinel2-1.2.0/drb/topics/sentinel2/pdi/datastrip/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:30:21.000000 drb-topic-sentinel2-1.2.0/drb/topics/sentinel2/pdi/datastrip/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5290 2023-05-16 13:27:43.000000 drb-topic-sentinel2-1.2.0/drb/topics/sentinel2/pdi/datastrip/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 13:28:20.750413 drb-topic-sentinel2-1.2.0/drb/topics/sentinel2/pdi/granule/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:30:21.000000 drb-topic-sentinel2-1.2.0/drb/topics/sentinel2/pdi/granule/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5030 2023-05-16 13:27:43.000000 drb-topic-sentinel2-1.2.0/drb/topics/sentinel2/pdi/granule/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 13:28:20.750413 drb-topic-sentinel2-1.2.0/drb/topics/sentinel2/user/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:30:21.000000 drb-topic-sentinel2-1.2.0/drb/topics/sentinel2/user/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3875 2023-05-16 13:27:43.000000 drb-topic-sentinel2-1.2.0/drb/topics/sentinel2/user/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 13:28:20.754413 drb-topic-sentinel2-1.2.0/drb_topic_sentinel2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6040 2023-05-16 13:28:20.000000 drb-topic-sentinel2-1.2.0/drb_topic_sentinel2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      932 2023-05-16 13:28:20.000000 drb-topic-sentinel2-1.2.0/drb_topic_sentinel2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 13:28:20.000000 drb-topic-sentinel2-1.2.0/drb_topic_sentinel2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      268 2023-05-16 13:28:20.000000 drb-topic-sentinel2-1.2.0/drb_topic_sentinel2.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 13:28:20.000000 drb-topic-sentinel2-1.2.0/drb_topic_sentinel2.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       55 2023-05-16 13:28:20.000000 drb-topic-sentinel2-1.2.0/drb_topic_sentinel2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-16 13:28:20.000000 drb-topic-sentinel2-1.2.0/drb_topic_sentinel2.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-05-16 12:37:11.000000 drb-topic-sentinel2-1.2.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       55 2023-05-16 12:37:11.000000 drb-topic-sentinel2-1.2.0/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1424 2023-05-16 13:28:20.754413 drb-topic-sentinel2-1.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      135 2023-05-16 12:37:11.000000 drb-topic-sentinel2-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 13:28:20.754413 drb-topic-sentinel2-1.2.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      788 2022-07-06 15:33:55.000000 drb-topic-sentinel2-1.2.0/tests/test_sentinel2_topics.py
+-rw-rw-rw-   0 root         (0) root         (0)    83607 2023-01-03 10:30:21.000000 drb-topic-sentinel2-1.2.0/versioneer.py
```

### Comparing `drb-topic-sentinel2-1.1.0/PKG-INFO` & `drb-topic-sentinel2-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: drb-topic-sentinel2
-Version: 1.1.0
-Summary: sentinel-2 topic for DRB Python
-Home-page: https://gitlab.com/drb-python/topics/sentinel2
+Version: 1.2.0
+Summary: Sentinel-2 topic for DRB Python
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: Apache Software License
+License: LGPLv3
+Project-URL: Source, https://gitlab.com/drb-python/topics/sentinel2
 Classifier: Programming Language :: Python :: 3.8
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENCE.txt
 
 # drb-topic-sentinel2
 The `drb-topic-sentinel2` is a DRB plugin declaring topics about
 [Sentinel-2](https://sentinels.copernicus.eu/web/sentinel/missions/sentinel-2)
 EO satellite.
 
 ## Installation
@@ -146,8 +145,7 @@
         K([Sentinel-2 Level-2A Datastrip<br/>0cbf0d70-f2fd-11ec-b939-0242ac120002])
         L([Sentinel-2 Level-2A Datastrip tar<br/>564d3d42-0bf6-11ed-861d-0242ac120002])
     end
     
     B --> A
     C & D & E & F & G --> B
 ```
-
```

### Comparing `drb-topic-sentinel2-1.1.0/README.md` & `drb-topic-sentinel2-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `drb-topic-sentinel2-1.1.0/drb/topics/sentinel2/aux/cortex.yml` & `drb-topic-sentinel2-1.2.0/drb/topics/sentinel2/aux/cortex.yml`

 * *Files identical despite different names*

### Comparing `drb-topic-sentinel2-1.1.0/drb/topics/sentinel2/pdi/cortex.yml` & `drb-topic-sentinel2-1.2.0/drb/topics/sentinel2/pdi/cortex.yml`

 * *Files identical despite different names*

### Comparing `drb-topic-sentinel2-1.1.0/drb/topics/sentinel2/pdi/datastrip/cortex.yml` & `drb-topic-sentinel2-1.2.0/drb/topics/sentinel2/pdi/datastrip/cortex.yml`

 * *Files identical despite different names*

### Comparing `drb-topic-sentinel2-1.1.0/drb/topics/sentinel2/pdi/granule/cortex.yml` & `drb-topic-sentinel2-1.2.0/drb/topics/sentinel2/pdi/granule/cortex.yml`

 * *Files identical despite different names*

### Comparing `drb-topic-sentinel2-1.1.0/drb/topics/sentinel2/user/cortex.yml` & `drb-topic-sentinel2-1.2.0/drb/topics/sentinel2/user/cortex.yml`

 * *Files identical despite different names*

### Comparing `drb-topic-sentinel2-1.1.0/drb_topic_sentinel2.egg-info/PKG-INFO` & `drb-topic-sentinel2-1.2.0/drb_topic_sentinel2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: drb-topic-sentinel2
-Version: 1.1.0
-Summary: sentinel-2 topic for DRB Python
-Home-page: https://gitlab.com/drb-python/topics/sentinel2
+Version: 1.2.0
+Summary: Sentinel-2 topic for DRB Python
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: Apache Software License
+License: LGPLv3
+Project-URL: Source, https://gitlab.com/drb-python/topics/sentinel2
 Classifier: Programming Language :: Python :: 3.8
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENCE.txt
 
 # drb-topic-sentinel2
 The `drb-topic-sentinel2` is a DRB plugin declaring topics about
 [Sentinel-2](https://sentinels.copernicus.eu/web/sentinel/missions/sentinel-2)
 EO satellite.
 
 ## Installation
@@ -146,8 +145,7 @@
         K([Sentinel-2 Level-2A Datastrip<br/>0cbf0d70-f2fd-11ec-b939-0242ac120002])
         L([Sentinel-2 Level-2A Datastrip tar<br/>564d3d42-0bf6-11ed-861d-0242ac120002])
     end
     
     B --> A
     C & D & E & F & G --> B
 ```
-
```

### Comparing `drb-topic-sentinel2-1.1.0/drb_topic_sentinel2.egg-info/SOURCES.txt` & `drb-topic-sentinel2-1.2.0/drb_topic_sentinel2.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

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
 drb/topics/sentinel2/__init__.py
 drb/topics/sentinel2/_version.py
 drb/topics/sentinel2/cortex.yml
@@ -17,9 +19,11 @@
 drb/topics/sentinel2/pdi/granule/cortex.yml
 drb/topics/sentinel2/user/__init__.py
 drb/topics/sentinel2/user/cortex.yml
 drb_topic_sentinel2.egg-info/PKG-INFO
 drb_topic_sentinel2.egg-info/SOURCES.txt
 drb_topic_sentinel2.egg-info/dependency_links.txt
 drb_topic_sentinel2.egg-info/entry_points.txt
+drb_topic_sentinel2.egg-info/not-zip-safe
 drb_topic_sentinel2.egg-info/requires.txt
-drb_topic_sentinel2.egg-info/top_level.txt
+drb_topic_sentinel2.egg-info/top_level.txt
+tests/test_sentinel2_topics.py
```

### Comparing `drb-topic-sentinel2-1.1.0/setup.py` & `drb-topic-sentinel2-1.2.0/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -1,49 +1,61 @@
-import versioneer
-from setuptools import setup, find_namespace_packages
+[metadata]
+name = drb-topic-sentinel2
+author = GAEL Systems
+author_email = drb-python@gael.fr
+description = Sentinel-2 topic for DRB Python
+long_description = file: README.md
+long_description_content_type = text/markdown
+license = LGPLv3
+classifiers = 
+	Programming Language :: Python :: 3.8
+	License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
+project_urls = 
+	Source = https://gitlab.com/drb-python/topics/sentinel2
 
+[options]
+zip_safe = False
+include_package_data = True
+packages = find_namespace:
+python_requires = >=3.8
+install_requires = file: requirements.txt
 
-with open('requirements.txt', 'r') as file:
-    REQUIREMENTS = file.readlines()
+[options.packages.find]
+exclude = 
+	tests*
+	docs*
+
+[options.package_data]
+drb.topics.sentinel2 = 
+	cortex.yml
+drb.topics.sentinel2.user = 
+	cortex.yml
+drb.topics.sentinel2.pdi = 
+	cortex.yml
+drb.topics.sentinel2.pdi.datastrip = 
+	cortex.yml
+drb.topics.sentinel2.pdi.granule = 
+	cortex.yml
+drb.topics.sentinel2.aux = 
+	cortex.yml
+
+[options.entry_points]
+drb.topic = 
+	sentinel2=drb.topics.sentinel2
+	sentinel2_user=drb.topics.sentinel2.user
+	sentinel2_pdi=drb.topics.sentinel2.pdi
+	sentinel2_ds=drb.topics.sentinel2.pdi.datastrip
+	sentinel2_gs=drb.topics.sentinel2.pdi.granule
+	sentinel2_aux=drb.topics.sentinel2.aux
+
+[versioneer]
+VCS = git
+style = pep440
+versionfile_source = drb/topics/sentinel2/_version.py
+versionfile_build = drb/topics/sentinel2/_version.py
+tag_prefix = 
+parentdir_prefix = 
+
+[egg_info]
+tag_build = 
+tag_date = 0
 
-with open('README.md', 'r') as file:
-    long_description = file.read()
-
-
-setup(
-    name='drb-topic-sentinel2',
-    description='sentinel-2 topic for DRB Python',
-    long_description=long_description,
-    long_description_content_type='text/markdown',
-    author='GAEL Systems',
-    author_email='drb-python@gael.fr',
-    url='https://gitlab.com/drb-python/topics/sentinel2',
-    python_requires='>=3.8',
-    install_requires=REQUIREMENTS,
-    packages=find_namespace_packages(include=['drb.*']),
-    classifiers=[
-        "Programming Language :: Python :: 3.8",
-        "License :: OSI Approved :: Apache Software License",
-        "Programming Language :: Python :: 3.8",
-    ],
-    package_data={
-        'drb.topics.sentinel2': ['cortex.yml'],
-        'drb.topics.sentinel2.user': ['cortex.yml'],
-        'drb.topics.sentinel2.pdi': ['cortex.yml'],
-        'drb.topics.sentinel2.pdi.datastrip': ['cortex.yml'],
-        'drb.topics.sentinel2.pdi.granule': ['cortex.yml'],
-        'drb.topics.sentinel2.aux': ['cortex.yml']
-    },
-    data_files=[('.', ['requirements.txt'])],
-    entry_points={
-        'drb.topic': [
-            'sentinel2=drb.topics.sentinel2',
-            'sentinel2_user=drb.topics.sentinel2.user',
-            'sentinel2_pdi=drb.topics.sentinel2.pdi',
-            'sentinel2_ds=drb.topics.sentinel2.pdi.datastrip',
-            'sentinel2_gs=drb.topics.sentinel2.pdi.granule',
-            'sentinel2_aux=drb.topics.sentinel2.aux'
-        ]
-    },
-    version=versioneer.get_version(),
-    cmdclass=versioneer.get_cmdclass()
-)
```

### Comparing `drb-topic-sentinel2-1.1.0/versioneer.py` & `drb-topic-sentinel2-1.2.0/versioneer.py`

 * *Files identical despite different names*

