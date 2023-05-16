# Comparing `tmp/scrapere-0.2.6.tar.gz` & `tmp/scrapere-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapere-0.2.6.tar", last modified: Tue May 16 12:08:33 2023, max compression
+gzip compressed data, was "scrapere-0.2.7.tar", last modified: Tue May 16 12:10:52 2023, max compression
```

## Comparing `scrapere-0.2.6.tar` & `scrapere-0.2.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 vpere     (1000) vpere     (1000)        0 2023-05-16 12:08:33.136120 scrapere-0.2.6/
--rw-rw-r--   0 vpere     (1000) vpere     (1000)     1035 2023-05-16 12:08:33.136120 scrapere-0.2.6/PKG-INFO
--rw-rw-r--   0 vpere     (1000) vpere     (1000)      799 2023-05-16 12:08:26.000000 scrapere-0.2.6/README.md
-drwxrwxr-x   0 vpere     (1000) vpere     (1000)        0 2023-05-16 12:08:33.132120 scrapere-0.2.6/scrapere/
--rw-rw-r--   0 vpere     (1000) vpere     (1000)       22 2023-05-16 10:14:19.000000 scrapere-0.2.6/scrapere/__init__.py
--rw-rw-r--   0 vpere     (1000) vpere     (1000)     5426 2023-05-16 12:08:26.000000 scrapere-0.2.6/scrapere/toolbox.py
--rw-rw-r--   0 vpere     (1000) vpere     (1000)  2656639 2023-05-16 10:19:54.000000 scrapere-0.2.6/scrapere/user_agents.txt
-drwxrwxr-x   0 vpere     (1000) vpere     (1000)        0 2023-05-16 12:08:33.136120 scrapere-0.2.6/scrapere.egg-info/
--rw-rw-r--   0 vpere     (1000) vpere     (1000)     1035 2023-05-16 12:08:33.000000 scrapere-0.2.6/scrapere.egg-info/PKG-INFO
--rw-rw-r--   0 vpere     (1000) vpere     (1000)      243 2023-05-16 12:08:33.000000 scrapere-0.2.6/scrapere.egg-info/SOURCES.txt
--rw-rw-r--   0 vpere     (1000) vpere     (1000)        1 2023-05-16 12:08:33.000000 scrapere-0.2.6/scrapere.egg-info/dependency_links.txt
--rw-rw-r--   0 vpere     (1000) vpere     (1000)       39 2023-05-16 12:08:33.000000 scrapere-0.2.6/scrapere.egg-info/requires.txt
--rw-rw-r--   0 vpere     (1000) vpere     (1000)        9 2023-05-16 12:08:33.000000 scrapere-0.2.6/scrapere.egg-info/top_level.txt
--rw-rw-r--   0 vpere     (1000) vpere     (1000)       38 2023-05-16 12:08:33.136120 scrapere-0.2.6/setup.cfg
--rw-rw-r--   0 vpere     (1000) vpere     (1000)      727 2023-05-16 12:08:26.000000 scrapere-0.2.6/setup.py
+drwxrwxr-x   0 vpere     (1000) vpere     (1000)        0 2023-05-16 12:10:52.603842 scrapere-0.2.7/
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)     1035 2023-05-16 12:10:52.603842 scrapere-0.2.7/PKG-INFO
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)      799 2023-05-16 12:10:50.000000 scrapere-0.2.7/README.md
+drwxrwxr-x   0 vpere     (1000) vpere     (1000)        0 2023-05-16 12:10:52.599842 scrapere-0.2.7/scrapere/
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)       22 2023-05-16 10:14:19.000000 scrapere-0.2.7/scrapere/__init__.py
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)     5426 2023-05-16 12:10:39.000000 scrapere-0.2.7/scrapere/toolbox.py
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)  2656639 2023-05-16 10:19:54.000000 scrapere-0.2.7/scrapere/user_agents.txt
+drwxrwxr-x   0 vpere     (1000) vpere     (1000)        0 2023-05-16 12:10:52.603842 scrapere-0.2.7/scrapere.egg-info/
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)     1035 2023-05-16 12:10:52.000000 scrapere-0.2.7/scrapere.egg-info/PKG-INFO
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)      243 2023-05-16 12:10:52.000000 scrapere-0.2.7/scrapere.egg-info/SOURCES.txt
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)        1 2023-05-16 12:10:52.000000 scrapere-0.2.7/scrapere.egg-info/dependency_links.txt
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)       39 2023-05-16 12:10:52.000000 scrapere-0.2.7/scrapere.egg-info/requires.txt
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)        9 2023-05-16 12:10:52.000000 scrapere-0.2.7/scrapere.egg-info/top_level.txt
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)       38 2023-05-16 12:10:52.603842 scrapere-0.2.7/setup.cfg
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)      727 2023-05-16 12:10:50.000000 scrapere-0.2.7/setup.py
```

### Comparing `scrapere-0.2.6/PKG-INFO` & `scrapere-0.2.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: scrapere
-Version: 0.2.6
+Version: 0.2.7
 Summary: Small set of my web scraping python tools
 Home-page: https://github.com/vPere/scrapere
 Author: vPere
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # Scraping libary
 
 This is a simple toolbox for scraping info from websites which includes methods for generating headers with a random user agent picked from a list of more than 24k user agents, a method for waiting a random time between 1 and 3 seconds, a progress bar for it to look cool ;) and a couple of methods that will help you retreive email addresses and spanish phone numbers from a given url.
 
 As this package may be useful for a bunch of legitimate and non-legitimate use cases, I'm not responsible of whatever you do with it.
 
-## Version 0.2.6 features:
+## Version 0.2.7 features:
  - Improves the email regex.
 
-## Version 0.2.6 issues:
+## Version 0.2.7 issues:
 - There are no tests...
 - scrap_phones() only works for spanish phone numbers
 
 As this is my first python package, I might not mantain it, so better try finding another one...
```

### Comparing `scrapere-0.2.6/README.md` & `scrapere-0.2.7/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Scraping libary
 
 This is a simple toolbox for scraping info from websites which includes methods for generating headers with a random user agent picked from a list of more than 24k user agents, a method for waiting a random time between 1 and 3 seconds, a progress bar for it to look cool ;) and a couple of methods that will help you retreive email addresses and spanish phone numbers from a given url.
 
 As this package may be useful for a bunch of legitimate and non-legitimate use cases, I'm not responsible of whatever you do with it.
 
-## Version 0.2.6 features:
+## Version 0.2.7 features:
  - Improves the email regex.
 
-## Version 0.2.6 issues:
+## Version 0.2.7 issues:
 - There are no tests...
 - scrap_phones() only works for spanish phone numbers
 
 As this is my first python package, I might not mantain it, so better try finding another one...
```

### Comparing `scrapere-0.2.6/scrapere/toolbox.py` & `scrapere-0.2.7/scrapere/toolbox.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import requests
 import re
 import csv
 import pkg_resources
 from bs4 import BeautifulSoup
 from colorama import Fore, Style
 
-EMAIL_REGEX = r'^("[\w-\s]+")|([\w-]+(?:\.[\w-]+)*)|("[\w-\s]+")([\w-]+(?:\.[\w-]+)*))(@((?:[\w-]+\.)*\w[\w-]{0,66})\.([a-z]{2,6}(?:\.[a-z]{2})?)$)|(@\[?((25[0-5]\.|2[0-4][0-9]\.|1[0-9]{2}\.|[0-9]{1,2}\.))((25[0-5]|2[0-4][0-9]|1[0-9]{2}|[0-9]{1,2})\.){2}(25[0-5]|2[0-4][0-9]|1[0-9]{2}|[0-9]{1,2})\]?$)'
+EMAIL_REGEX = r'^("[\w\s-]+")|([\w-]+(?:\.[\w-]+)*)|("[\w\s-]+")([\w-]+(?:\.[\w-]+)*))(@((?:[\w-]+\.)*\w[\w-]{0,66})\.([a-z]{2,6}(?:\.[a-z]{2})?)$)|(@\[?((25[0-5]\.|2[0-4][0-9]\.|1[0-9]{2}\.|[0-9]{1,2}\.))((25[0-5]|2[0-4][0-9]|1[0-9]{2}|[0-9]{1,2})\.){2}(25[0-5]|2[0-4][0-9]|1[0-9]{2}|[0-9]{1,2})\]?$)'
 PHONE_REGEX = r'(?:\+34|0034)?\s?(?:6|9)(?:\d\s?\d{2}\s?\d{2}\s?\d{2}|\d{2}\s?\d{3}\s?\d{3}|\d{3}\s?\d{2}\s?\d{2})'
 def progress_bar(row_count, total_rows):
     percent = round((row_count / total_rows) * 100, 2)
     progress = int(100 * row_count / total_rows)
     bar = Fore.LIGHTGREEN_EX + "[" + "\u25AE" * progress + "_" * (100 - progress) + "]"
     print(f"{bar} {percent}%" + Style.RESET_ALL)
```

### Comparing `scrapere-0.2.6/scrapere/user_agents.txt` & `scrapere-0.2.7/scrapere/user_agents.txt`

 * *Files identical despite different names*

### Comparing `scrapere-0.2.6/scrapere.egg-info/PKG-INFO` & `scrapere-0.2.7/scrapere.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: scrapere
-Version: 0.2.6
+Version: 0.2.7
 Summary: Small set of my web scraping python tools
 Home-page: https://github.com/vPere/scrapere
 Author: vPere
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # Scraping libary
 
 This is a simple toolbox for scraping info from websites which includes methods for generating headers with a random user agent picked from a list of more than 24k user agents, a method for waiting a random time between 1 and 3 seconds, a progress bar for it to look cool ;) and a couple of methods that will help you retreive email addresses and spanish phone numbers from a given url.
 
 As this package may be useful for a bunch of legitimate and non-legitimate use cases, I'm not responsible of whatever you do with it.
 
-## Version 0.2.6 features:
+## Version 0.2.7 features:
  - Improves the email regex.
 
-## Version 0.2.6 issues:
+## Version 0.2.7 issues:
 - There are no tests...
 - scrap_phones() only works for spanish phone numbers
 
 As this is my first python package, I might not mantain it, so better try finding another one...
```

### Comparing `scrapere-0.2.6/setup.py` & `scrapere-0.2.7/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='scrapere',
     packages=find_packages(),
-    version='0.2.6',
+    version='0.2.7',
     description='Small set of my web scraping python tools',
     author='vPere',
     license='MIT',
     readme='README.md',
     install_requires=[
         'requests',
         'beautifulsoup4',
```

