# Comparing `tmp/scrapere-0.1.9.tar.gz` & `tmp/scrapere-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapere-0.1.9.tar", last modified: Tue May 16 10:07:13 2023, max compression
+gzip compressed data, was "scrapere-0.2.0.tar", last modified: Tue May 16 10:18:40 2023, max compression
```

## Comparing `scrapere-0.1.9.tar` & `scrapere-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 vpere     (1000) vpere     (1000)        0 2023-05-16 10:07:13.243823 scrapere-0.1.9/
--rw-rw-r--   0 vpere     (1000) vpere     (1000)      979 2023-05-16 10:07:13.243823 scrapere-0.1.9/PKG-INFO
--rw-rw-r--   0 vpere     (1000) vpere     (1000)      743 2023-05-16 10:06:03.000000 scrapere-0.1.9/README.md
-drwxrwxr-x   0 vpere     (1000) vpere     (1000)        0 2023-05-16 10:07:13.239823 scrapere-0.1.9/scrapere/
--rw-rw-r--   0 vpere     (1000) vpere     (1000)       22 2023-05-04 10:22:06.000000 scrapere-0.1.9/scrapere/__init__.py
--rw-rw-r--   0 vpere     (1000) vpere     (1000)     4783 2023-05-16 10:05:18.000000 scrapere-0.1.9/scrapere/toolbox.py
--rw-rw-r--   0 vpere     (1000) vpere     (1000)  2656644 2023-05-04 09:43:57.000000 scrapere-0.1.9/scrapere/user-agents-unique.txt
-drwxrwxr-x   0 vpere     (1000) vpere     (1000)        0 2023-05-16 10:07:13.243823 scrapere-0.1.9/scrapere.egg-info/
--rw-rw-r--   0 vpere     (1000) vpere     (1000)      979 2023-05-16 10:07:13.000000 scrapere-0.1.9/scrapere.egg-info/PKG-INFO
--rw-rw-r--   0 vpere     (1000) vpere     (1000)      250 2023-05-16 10:07:13.000000 scrapere-0.1.9/scrapere.egg-info/SOURCES.txt
--rw-rw-r--   0 vpere     (1000) vpere     (1000)        1 2023-05-16 10:07:13.000000 scrapere-0.1.9/scrapere.egg-info/dependency_links.txt
--rw-rw-r--   0 vpere     (1000) vpere     (1000)       39 2023-05-16 10:07:13.000000 scrapere-0.1.9/scrapere.egg-info/requires.txt
--rw-rw-r--   0 vpere     (1000) vpere     (1000)        9 2023-05-16 10:07:13.000000 scrapere-0.1.9/scrapere.egg-info/top_level.txt
--rw-rw-r--   0 vpere     (1000) vpere     (1000)       38 2023-05-16 10:07:13.243823 scrapere-0.1.9/setup.cfg
--rw-rw-r--   0 vpere     (1000) vpere     (1000)      727 2023-05-16 10:06:03.000000 scrapere-0.1.9/setup.py
+drwxrwxr-x   0 vpere     (1000) vpere     (1000)        0 2023-05-16 10:18:40.914041 scrapere-0.2.0/
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)      979 2023-05-16 10:18:40.914041 scrapere-0.2.0/PKG-INFO
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)      743 2023-05-16 10:18:33.000000 scrapere-0.2.0/README.md
+drwxrwxr-x   0 vpere     (1000) vpere     (1000)        0 2023-05-16 10:18:40.910041 scrapere-0.2.0/scrapere/
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)       22 2023-05-16 10:14:19.000000 scrapere-0.2.0/scrapere/__init__.py
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)     4854 2023-05-16 10:18:04.000000 scrapere-0.2.0/scrapere/toolbox.py
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)  2656644 2023-05-04 09:43:57.000000 scrapere-0.2.0/scrapere/user-agents-unique.txt
+drwxrwxr-x   0 vpere     (1000) vpere     (1000)        0 2023-05-16 10:18:40.914041 scrapere-0.2.0/scrapere.egg-info/
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)      979 2023-05-16 10:18:40.000000 scrapere-0.2.0/scrapere.egg-info/PKG-INFO
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)      250 2023-05-16 10:18:40.000000 scrapere-0.2.0/scrapere.egg-info/SOURCES.txt
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)        1 2023-05-16 10:18:40.000000 scrapere-0.2.0/scrapere.egg-info/dependency_links.txt
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)       39 2023-05-16 10:18:40.000000 scrapere-0.2.0/scrapere.egg-info/requires.txt
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)        9 2023-05-16 10:18:40.000000 scrapere-0.2.0/scrapere.egg-info/top_level.txt
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)       38 2023-05-16 10:18:40.914041 scrapere-0.2.0/setup.cfg
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)      727 2023-05-16 10:18:33.000000 scrapere-0.2.0/setup.py
```

### Comparing `scrapere-0.1.9/PKG-INFO` & `scrapere-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: scrapere
-Version: 0.1.9
+Version: 0.2.0
 Summary: Small set of my web scraping python tools
 Home-page: https://github.com/vPere/scrapere
 Author: vPere
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # Scraping libary
 
 This is a simple toolbox for scraping info from websites which includes methods for generating headers with a random user agent picked from a list of more than 24k user agents, a method for waiting a random time between 1 and 3 seconds, a progress bar for it to look cool ;) and a couple of methods that will help you retreive email addresses and spanish phone numbers from a given url.
 
 As this package may be useful for a bunch of legitimate and non-legitimate use cases, I'm not responsible of whatever you do with it.
 
 
-## Version 0.1.9 issues:
+## Version 0.2.0 issues:
 - There are no tests...
 - scrap_phones() only works for spanish phone numbers
 
 As this is my first python package, I might not mantain it, so better try finding another one...
```

### Comparing `scrapere-0.1.9/README.md` & `scrapere-0.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Scraping libary
 
 This is a simple toolbox for scraping info from websites which includes methods for generating headers with a random user agent picked from a list of more than 24k user agents, a method for waiting a random time between 1 and 3 seconds, a progress bar for it to look cool ;) and a couple of methods that will help you retreive email addresses and spanish phone numbers from a given url.
 
 As this package may be useful for a bunch of legitimate and non-legitimate use cases, I'm not responsible of whatever you do with it.
 
 
-## Version 0.1.9 issues:
+## Version 0.2.0 issues:
 - There are no tests...
 - scrap_phones() only works for spanish phone numbers
 
 As this is my first python package, I might not mantain it, so better try finding another one...
```

### Comparing `scrapere-0.1.9/scrapere/toolbox.py` & `scrapere-0.2.0/scrapere/toolbox.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import random
 import time
 import requests
 import re
 import csv
 from datetime import datetime
+import pkg_resources
 from bs4 import BeautifulSoup
 from colorama import Fore, Style
 import emoji
 
 
 def progress_bar(row_count, total_rows):
     percent = round((row_count / total_rows) * 100, 2)
@@ -22,15 +23,16 @@
         for _ in fp:
             total += 1
     return total
 
 
 def get_user_agent_list():
     user_agent_list = []
-    with open('../scrapere/user-agents-unique.txt', 'r') as f:
+    file_path = pkg_resources.resource_filename(__name__, 'user_agents.txt')
+    with open(file_path, 'r') as f:
         for line in f:
             user_agent_list.append(line.strip())
     return user_agent_list
 
 
 def get_random_user_agent():
     user_agent_list = get_user_agent_list()
```

### Comparing `scrapere-0.1.9/scrapere/user-agents-unique.txt` & `scrapere-0.2.0/scrapere/user-agents-unique.txt`

 * *Files identical despite different names*

### Comparing `scrapere-0.1.9/scrapere.egg-info/PKG-INFO` & `scrapere-0.2.0/scrapere.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: scrapere
-Version: 0.1.9
+Version: 0.2.0
 Summary: Small set of my web scraping python tools
 Home-page: https://github.com/vPere/scrapere
 Author: vPere
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # Scraping libary
 
 This is a simple toolbox for scraping info from websites which includes methods for generating headers with a random user agent picked from a list of more than 24k user agents, a method for waiting a random time between 1 and 3 seconds, a progress bar for it to look cool ;) and a couple of methods that will help you retreive email addresses and spanish phone numbers from a given url.
 
 As this package may be useful for a bunch of legitimate and non-legitimate use cases, I'm not responsible of whatever you do with it.
 
 
-## Version 0.1.9 issues:
+## Version 0.2.0 issues:
 - There are no tests...
 - scrap_phones() only works for spanish phone numbers
 
 As this is my first python package, I might not mantain it, so better try finding another one...
```

### Comparing `scrapere-0.1.9/setup.py` & `scrapere-0.2.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='scrapere',
     packages=find_packages(),
-    version='0.1.9',
+    version='0.2.0',
     description='Small set of my web scraping python tools',
     author='vPere',
     license='MIT',
     readme='README.md',
     install_requires=[
         'requests',
         'beautifulsoup4',
```

