# Comparing `tmp/scrapere-0.2.3.tar.gz` & `tmp/scrapere-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapere-0.2.3.tar", last modified: Tue May 16 10:24:04 2023, max compression
+gzip compressed data, was "scrapere-0.2.4.tar", last modified: Tue May 16 11:53:56 2023, max compression
```

## Comparing `scrapere-0.2.3.tar` & `scrapere-0.2.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 vpere     (1000) vpere     (1000)        0 2023-05-16 10:24:04.676679 scrapere-0.2.3/
--rw-rw-r--   0 vpere     (1000) vpere     (1000)      979 2023-05-16 10:24:04.676679 scrapere-0.2.3/PKG-INFO
--rw-rw-r--   0 vpere     (1000) vpere     (1000)      743 2023-05-16 10:23:57.000000 scrapere-0.2.3/README.md
-drwxrwxr-x   0 vpere     (1000) vpere     (1000)        0 2023-05-16 10:24:04.672679 scrapere-0.2.3/scrapere/
--rw-rw-r--   0 vpere     (1000) vpere     (1000)       22 2023-05-16 10:14:19.000000 scrapere-0.2.3/scrapere/__init__.py
--rw-rw-r--   0 vpere     (1000) vpere     (1000)     4986 2023-05-16 10:23:42.000000 scrapere-0.2.3/scrapere/toolbox.py
--rw-rw-r--   0 vpere     (1000) vpere     (1000)  2656639 2023-05-16 10:19:54.000000 scrapere-0.2.3/scrapere/user_agents.txt
-drwxrwxr-x   0 vpere     (1000) vpere     (1000)        0 2023-05-16 10:24:04.676679 scrapere-0.2.3/scrapere.egg-info/
--rw-rw-r--   0 vpere     (1000) vpere     (1000)      979 2023-05-16 10:24:04.000000 scrapere-0.2.3/scrapere.egg-info/PKG-INFO
--rw-rw-r--   0 vpere     (1000) vpere     (1000)      243 2023-05-16 10:24:04.000000 scrapere-0.2.3/scrapere.egg-info/SOURCES.txt
--rw-rw-r--   0 vpere     (1000) vpere     (1000)        1 2023-05-16 10:24:04.000000 scrapere-0.2.3/scrapere.egg-info/dependency_links.txt
--rw-rw-r--   0 vpere     (1000) vpere     (1000)       39 2023-05-16 10:24:04.000000 scrapere-0.2.3/scrapere.egg-info/requires.txt
--rw-rw-r--   0 vpere     (1000) vpere     (1000)        9 2023-05-16 10:24:04.000000 scrapere-0.2.3/scrapere.egg-info/top_level.txt
--rw-rw-r--   0 vpere     (1000) vpere     (1000)       38 2023-05-16 10:24:04.676679 scrapere-0.2.3/setup.cfg
--rw-rw-r--   0 vpere     (1000) vpere     (1000)      727 2023-05-16 10:23:57.000000 scrapere-0.2.3/setup.py
+drwxrwxr-x   0 vpere     (1000) vpere     (1000)        0 2023-05-16 11:53:56.870625 scrapere-0.2.4/
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)     1035 2023-05-16 11:53:56.870625 scrapere-0.2.4/PKG-INFO
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)      799 2023-05-16 11:53:44.000000 scrapere-0.2.4/README.md
+drwxrwxr-x   0 vpere     (1000) vpere     (1000)        0 2023-05-16 11:53:56.870625 scrapere-0.2.4/scrapere/
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)       22 2023-05-16 10:14:19.000000 scrapere-0.2.4/scrapere/__init__.py
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)     5402 2023-05-16 11:53:44.000000 scrapere-0.2.4/scrapere/toolbox.py
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)  2656639 2023-05-16 10:19:54.000000 scrapere-0.2.4/scrapere/user_agents.txt
+drwxrwxr-x   0 vpere     (1000) vpere     (1000)        0 2023-05-16 11:53:56.870625 scrapere-0.2.4/scrapere.egg-info/
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)     1035 2023-05-16 11:53:56.000000 scrapere-0.2.4/scrapere.egg-info/PKG-INFO
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)      243 2023-05-16 11:53:56.000000 scrapere-0.2.4/scrapere.egg-info/SOURCES.txt
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)        1 2023-05-16 11:53:56.000000 scrapere-0.2.4/scrapere.egg-info/dependency_links.txt
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)       39 2023-05-16 11:53:56.000000 scrapere-0.2.4/scrapere.egg-info/requires.txt
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)        9 2023-05-16 11:53:56.000000 scrapere-0.2.4/scrapere.egg-info/top_level.txt
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)       38 2023-05-16 11:53:56.870625 scrapere-0.2.4/setup.cfg
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)      727 2023-05-16 11:53:54.000000 scrapere-0.2.4/setup.py
```

### Comparing `scrapere-0.2.3/PKG-INFO` & `scrapere-0.2.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: scrapere
-Version: 0.2.3
+Version: 0.2.4
 Summary: Small set of my web scraping python tools
 Home-page: https://github.com/vPere/scrapere
 Author: vPere
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # Scraping libary
 
 This is a simple toolbox for scraping info from websites which includes methods for generating headers with a random user agent picked from a list of more than 24k user agents, a method for waiting a random time between 1 and 3 seconds, a progress bar for it to look cool ;) and a couple of methods that will help you retreive email addresses and spanish phone numbers from a given url.
 
 As this package may be useful for a bunch of legitimate and non-legitimate use cases, I'm not responsible of whatever you do with it.
 
+## Version 0.2.4 features:
+ - Improves the email regex.
 
-## Version 0.2.3 issues:
+## Version 0.2.4 issues:
 - There are no tests...
 - scrap_phones() only works for spanish phone numbers
 
 As this is my first python package, I might not mantain it, so better try finding another one...
```

### Comparing `scrapere-0.2.3/README.md` & `scrapere-0.2.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # Scraping libary
 
 This is a simple toolbox for scraping info from websites which includes methods for generating headers with a random user agent picked from a list of more than 24k user agents, a method for waiting a random time between 1 and 3 seconds, a progress bar for it to look cool ;) and a couple of methods that will help you retreive email addresses and spanish phone numbers from a given url.
 
 As this package may be useful for a bunch of legitimate and non-legitimate use cases, I'm not responsible of whatever you do with it.
 
+## Version 0.2.4 features:
+ - Improves the email regex.
 
-## Version 0.2.3 issues:
+## Version 0.2.4 issues:
 - There are no tests...
 - scrap_phones() only works for spanish phone numbers
 
 As this is my first python package, I might not mantain it, so better try finding another one...
```

### Comparing `scrapere-0.2.3/scrapere/toolbox.py` & `scrapere-0.2.4/scrapere/toolbox.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import random
 import time
 import requests
 import re
 import csv
-from datetime import datetime
 import pkg_resources
 from bs4 import BeautifulSoup
 from colorama import Fore, Style
-import emoji
 
+EMAIL_REGEX = r"""(?:[a-z0-9!#$%&'*+/=?^_`{|}~-]+(?:\.[a-z0-9!#$%&'*+/=?^_`{|}~-]+)*|"(?:[\x01-\x08\x0b\x0c\x0e-\x1f\x21\x23-\x5b\x5d-\x7f]|\\[\x01-\x09\x0b\x0c\x0e-\x7f])*")@(?:(?:[a-z0-9](?:[a-z0-9-]*[a-z0-9])?\.)+[a-z0-9](?:[a-z0-9-]*[a-z0-9])?|\[(?:(?:(2(5[0-5]|[0-4][0-9])|1[0-9][0-9]|[1-9]?[0-9]))\.){3}(?:(2(5[0-5]|[0-4][0-9])|1[0-9][0-9]|[1-9]?[0-9])|[a-z0-9-]*[a-z0-9]:(?:[\x01-\x08\x0b\x0c\x0e-\x1f\x21-\x5a\x53-\x7f]|\\[\x01-\x09\x0b\x0c\x0e-\x7f])+)\])"""
 
 def progress_bar(row_count, total_rows):
     percent = round((row_count / total_rows) * 100, 2)
     progress = int(100 * row_count / total_rows)
     bar = Fore.LIGHTGREEN_EX + "[" + "\u25AE" * progress + "_" * (100 - progress) + "]"
     print(f"{bar} {percent}%" + Style.RESET_ALL)
 
@@ -115,15 +114,15 @@
         counter += 1
         print(f"Crawling through {url}...")
         # check if url has http or https and add it if not
         if not url.startswith('http'):
             url = 'http://' + url
         response = requests.get(url, generate_header())
         soup = BeautifulSoup(response.content, 'html.parser')
-        for email in re.findall(r'[\w\.-]+@[\w\.-]+', str(soup)):
+        for email in re.findall(EMAIL_REGEX, str(soup)):
             if is_valid_email(email):
                 emails.append(email)
                 with open('emails.csv', 'a', newline='') as csvfile:
                     fieldnames = ['url', 'email']
                     writer = csv.DictWriter(csvfile, fieldnames=fieldnames)
                     writer.writerow({'url': url, 'email': email})
                 print(f"Found email: {email}, added to emails.csv")
```

### Comparing `scrapere-0.2.3/scrapere/user_agents.txt` & `scrapere-0.2.4/scrapere/user_agents.txt`

 * *Files identical despite different names*

### Comparing `scrapere-0.2.3/scrapere.egg-info/PKG-INFO` & `scrapere-0.2.4/scrapere.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: scrapere
-Version: 0.2.3
+Version: 0.2.4
 Summary: Small set of my web scraping python tools
 Home-page: https://github.com/vPere/scrapere
 Author: vPere
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # Scraping libary
 
 This is a simple toolbox for scraping info from websites which includes methods for generating headers with a random user agent picked from a list of more than 24k user agents, a method for waiting a random time between 1 and 3 seconds, a progress bar for it to look cool ;) and a couple of methods that will help you retreive email addresses and spanish phone numbers from a given url.
 
 As this package may be useful for a bunch of legitimate and non-legitimate use cases, I'm not responsible of whatever you do with it.
 
+## Version 0.2.4 features:
+ - Improves the email regex.
 
-## Version 0.2.3 issues:
+## Version 0.2.4 issues:
 - There are no tests...
 - scrap_phones() only works for spanish phone numbers
 
 As this is my first python package, I might not mantain it, so better try finding another one...
```

### Comparing `scrapere-0.2.3/setup.py` & `scrapere-0.2.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='scrapere',
     packages=find_packages(),
-    version='0.2.3',
+    version='0.2.4',
     description='Small set of my web scraping python tools',
     author='vPere',
     license='MIT',
     readme='README.md',
     install_requires=[
         'requests',
         'beautifulsoup4',
```

