# Comparing `tmp/trendingbot-0.0.1.tar.gz` & `tmp/trendingbot-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trendingbot-0.0.1.tar", last modified: Tue May 16 08:26:37 2023, max compression
+gzip compressed data, was "trendingbot-0.0.2.tar", last modified: Tue May 16 08:39:28 2023, max compression
```

## Comparing `trendingbot-0.0.1.tar` & `trendingbot-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 08:26:37.287335 trendingbot-0.0.1/
--rw-rw-rw-   0        0        0      442 2023-05-16 08:26:37.287335 trendingbot-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       16 2023-05-16 08:13:40.000000 trendingbot-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-16 08:26:37.287335 trendingbot-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1073 2023-05-16 08:14:04.000000 trendingbot-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-16 08:26:37.281878 trendingbot-0.0.1/trendingbot/
--rw-rw-rw-   0        0        0       33 2023-05-16 08:16:38.000000 trendingbot-0.0.1/trendingbot/__init__.py
--rw-rw-rw-   0        0        0     8369 2023-05-16 08:20:45.000000 trendingbot-0.0.1/trendingbot/schedule.py
--rw-rw-rw-   0        0        0     2148 2023-05-16 06:17:47.000000 trendingbot-0.0.1/trendingbot/scrape.py
-drwxrwxrwx   0        0        0        0 2023-05-16 08:26:37.286336 trendingbot-0.0.1/trendingbot.egg-info/
--rw-rw-rw-   0        0        0      442 2023-05-16 08:26:37.000000 trendingbot-0.0.1/trendingbot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2023-05-16 08:26:37.000000 trendingbot-0.0.1/trendingbot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 08:26:37.000000 trendingbot-0.0.1/trendingbot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-16 08:26:37.000000 trendingbot-0.0.1/trendingbot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-16 08:26:37.000000 trendingbot-0.0.1/trendingbot.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 08:39:28.944678 trendingbot-0.0.2/
+-rw-rw-rw-   0        0        0      442 2023-05-16 08:39:28.944678 trendingbot-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       16 2023-05-16 08:13:40.000000 trendingbot-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-16 08:39:28.944678 trendingbot-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1073 2023-05-16 08:39:13.000000 trendingbot-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 08:39:28.938688 trendingbot-0.0.2/trendingbot/
+-rw-rw-rw-   0        0        0       33 2023-05-16 08:16:38.000000 trendingbot-0.0.2/trendingbot/__init__.py
+-rw-rw-rw-   0        0        0     8359 2023-05-16 08:38:45.000000 trendingbot-0.0.2/trendingbot/schedule.py
+-rw-rw-rw-   0        0        0     2148 2023-05-16 06:17:47.000000 trendingbot-0.0.2/trendingbot/scrape.py
+drwxrwxrwx   0        0        0        0 2023-05-16 08:39:28.943680 trendingbot-0.0.2/trendingbot.egg-info/
+-rw-rw-rw-   0        0        0      442 2023-05-16 08:39:28.000000 trendingbot-0.0.2/trendingbot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2023-05-16 08:39:28.000000 trendingbot-0.0.2/trendingbot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 08:39:28.000000 trendingbot-0.0.2/trendingbot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-16 08:39:28.000000 trendingbot-0.0.2/trendingbot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-16 08:39:28.000000 trendingbot-0.0.2/trendingbot.egg-info/top_level.txt
```

### Comparing `trendingbot-0.0.1/setup.py` & `trendingbot-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 BASE_DIR = os.path.abspath(os.path.dirname(__file__))
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='trendingbot',
-    version="0.0.1",
+    version="0.0.2",
     description='trendingbot',
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords='trendingbot',
     url='https://github.com/yasuo626/TrendingBot',
     author='aidroid',
     author_email='yasuo626.com@gmail.com',
```

### Comparing `trendingbot-0.0.1/trendingbot/schedule.py` & `trendingbot-0.0.2/trendingbot/schedule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os,sys,time,datetime
-from trendingbot.trendings.scrape import scrape_site
+from trendingbot.scrape import scrape_site
 
 class SITE:
     def __init__(self,name,url,locate):
         self.name=name
         self.url=url
         self.locate=locate
```

### Comparing `trendingbot-0.0.1/trendingbot/scrape.py` & `trendingbot-0.0.2/trendingbot/scrape.py`

 * *Files identical despite different names*

