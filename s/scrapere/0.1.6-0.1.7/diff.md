# Comparing `tmp/scrapere-0.1.6.tar.gz` & `tmp/scrapere-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapere-0.1.6.tar", last modified: Tue May 16 09:33:17 2023, max compression
+gzip compressed data, was "scrapere-0.1.7.tar", last modified: Tue May 16 09:40:16 2023, max compression
```

## Comparing `scrapere-0.1.6.tar` & `scrapere-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 vpere     (1000) vpere     (1000)        0 2023-05-16 09:33:17.787330 scrapere-0.1.6/
--rw-rw-r--   0 vpere     (1000) vpere     (1000)      979 2023-05-16 09:33:17.787330 scrapere-0.1.6/PKG-INFO
--rw-rw-r--   0 vpere     (1000) vpere     (1000)      743 2023-05-16 09:32:49.000000 scrapere-0.1.6/README.md
-drwxrwxr-x   0 vpere     (1000) vpere     (1000)        0 2023-05-16 09:33:17.771330 scrapere-0.1.6/scrapere/
--rw-rw-r--   0 vpere     (1000) vpere     (1000)       22 2023-05-04 10:22:06.000000 scrapere-0.1.6/scrapere/__init__.py
--rw-rw-r--   0 vpere     (1000) vpere     (1000)     4773 2023-05-16 09:32:45.000000 scrapere-0.1.6/scrapere/toolbox.py
--rw-rw-r--   0 vpere     (1000) vpere     (1000)  2656644 2023-05-04 09:43:57.000000 scrapere-0.1.6/scrapere/user-agents-unique.txt
-drwxrwxr-x   0 vpere     (1000) vpere     (1000)        0 2023-05-16 09:33:17.783330 scrapere-0.1.6/scrapere.egg-info/
--rw-rw-r--   0 vpere     (1000) vpere     (1000)      979 2023-05-16 09:33:17.000000 scrapere-0.1.6/scrapere.egg-info/PKG-INFO
--rw-rw-r--   0 vpere     (1000) vpere     (1000)      250 2023-05-16 09:33:17.000000 scrapere-0.1.6/scrapere.egg-info/SOURCES.txt
--rw-rw-r--   0 vpere     (1000) vpere     (1000)        1 2023-05-16 09:33:17.000000 scrapere-0.1.6/scrapere.egg-info/dependency_links.txt
--rw-rw-r--   0 vpere     (1000) vpere     (1000)       39 2023-05-16 09:33:17.000000 scrapere-0.1.6/scrapere.egg-info/requires.txt
--rw-rw-r--   0 vpere     (1000) vpere     (1000)        9 2023-05-16 09:33:17.000000 scrapere-0.1.6/scrapere.egg-info/top_level.txt
--rw-rw-r--   0 vpere     (1000) vpere     (1000)       38 2023-05-16 09:33:17.787330 scrapere-0.1.6/setup.cfg
--rw-rw-r--   0 vpere     (1000) vpere     (1000)      727 2023-05-16 09:32:43.000000 scrapere-0.1.6/setup.py
+drwxrwxr-x   0 vpere     (1000) vpere     (1000)        0 2023-05-16 09:40:16.635904 scrapere-0.1.7/
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)      979 2023-05-16 09:40:16.635904 scrapere-0.1.7/PKG-INFO
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)      743 2023-05-16 09:32:49.000000 scrapere-0.1.7/README.md
+drwxrwxr-x   0 vpere     (1000) vpere     (1000)        0 2023-05-16 09:40:16.627904 scrapere-0.1.7/scrapere/
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)       22 2023-05-04 10:22:06.000000 scrapere-0.1.7/scrapere/__init__.py
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)     4773 2023-05-16 09:37:08.000000 scrapere-0.1.7/scrapere/toolbox.py
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)  2656644 2023-05-04 09:43:57.000000 scrapere-0.1.7/scrapere/user-agents-unique.txt
+drwxrwxr-x   0 vpere     (1000) vpere     (1000)        0 2023-05-16 09:40:16.631904 scrapere-0.1.7/scrapere.egg-info/
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)      979 2023-05-16 09:40:16.000000 scrapere-0.1.7/scrapere.egg-info/PKG-INFO
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)      250 2023-05-16 09:40:16.000000 scrapere-0.1.7/scrapere.egg-info/SOURCES.txt
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)        1 2023-05-16 09:40:16.000000 scrapere-0.1.7/scrapere.egg-info/dependency_links.txt
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)       39 2023-05-16 09:40:16.000000 scrapere-0.1.7/scrapere.egg-info/requires.txt
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)        9 2023-05-16 09:40:16.000000 scrapere-0.1.7/scrapere.egg-info/top_level.txt
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)       38 2023-05-16 09:40:16.635904 scrapere-0.1.7/setup.cfg
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)      727 2023-05-16 09:39:05.000000 scrapere-0.1.7/setup.py
```

### Comparing `scrapere-0.1.6/PKG-INFO` & `scrapere-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapere
-Version: 0.1.6
+Version: 0.1.7
 Summary: Small set of my web scraping python tools
 Home-page: https://github.com/vPere/scrapere
 Author: vPere
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `scrapere-0.1.6/README.md` & `scrapere-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `scrapere-0.1.6/scrapere/toolbox.py` & `scrapere-0.1.7/scrapere/toolbox.py`

 * *Files identical despite different names*

### Comparing `scrapere-0.1.6/scrapere/user-agents-unique.txt` & `scrapere-0.1.7/scrapere/user-agents-unique.txt`

 * *Files identical despite different names*

### Comparing `scrapere-0.1.6/scrapere.egg-info/PKG-INFO` & `scrapere-0.1.7/scrapere.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapere
-Version: 0.1.6
+Version: 0.1.7
 Summary: Small set of my web scraping python tools
 Home-page: https://github.com/vPere/scrapere
 Author: vPere
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `scrapere-0.1.6/setup.py` & `scrapere-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='scrapere',
     packages=find_packages(),
-    version='0.1.6',
+    version='0.1.7',
     description='Small set of my web scraping python tools',
     author='vPere',
     license='MIT',
     readme='README.md',
     install_requires=[
         'requests',
         'beautifulsoup4',
```

