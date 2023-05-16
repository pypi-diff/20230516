# Comparing `tmp/scrapere-0.1.7.tar.gz` & `tmp/scrapere-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapere-0.1.7.tar", last modified: Tue May 16 09:40:16 2023, max compression
+gzip compressed data, was "scrapere-0.1.8.tar", last modified: Tue May 16 09:58:53 2023, max compression
```

## Comparing `scrapere-0.1.7.tar` & `scrapere-0.1.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 vpere     (1000) vpere     (1000)        0 2023-05-16 09:40:16.635904 scrapere-0.1.7/
--rw-rw-r--   0 vpere     (1000) vpere     (1000)      979 2023-05-16 09:40:16.635904 scrapere-0.1.7/PKG-INFO
--rw-rw-r--   0 vpere     (1000) vpere     (1000)      743 2023-05-16 09:32:49.000000 scrapere-0.1.7/README.md
-drwxrwxr-x   0 vpere     (1000) vpere     (1000)        0 2023-05-16 09:40:16.627904 scrapere-0.1.7/scrapere/
--rw-rw-r--   0 vpere     (1000) vpere     (1000)       22 2023-05-04 10:22:06.000000 scrapere-0.1.7/scrapere/__init__.py
--rw-rw-r--   0 vpere     (1000) vpere     (1000)     4773 2023-05-16 09:37:08.000000 scrapere-0.1.7/scrapere/toolbox.py
--rw-rw-r--   0 vpere     (1000) vpere     (1000)  2656644 2023-05-04 09:43:57.000000 scrapere-0.1.7/scrapere/user-agents-unique.txt
-drwxrwxr-x   0 vpere     (1000) vpere     (1000)        0 2023-05-16 09:40:16.631904 scrapere-0.1.7/scrapere.egg-info/
--rw-rw-r--   0 vpere     (1000) vpere     (1000)      979 2023-05-16 09:40:16.000000 scrapere-0.1.7/scrapere.egg-info/PKG-INFO
--rw-rw-r--   0 vpere     (1000) vpere     (1000)      250 2023-05-16 09:40:16.000000 scrapere-0.1.7/scrapere.egg-info/SOURCES.txt
--rw-rw-r--   0 vpere     (1000) vpere     (1000)        1 2023-05-16 09:40:16.000000 scrapere-0.1.7/scrapere.egg-info/dependency_links.txt
--rw-rw-r--   0 vpere     (1000) vpere     (1000)       39 2023-05-16 09:40:16.000000 scrapere-0.1.7/scrapere.egg-info/requires.txt
--rw-rw-r--   0 vpere     (1000) vpere     (1000)        9 2023-05-16 09:40:16.000000 scrapere-0.1.7/scrapere.egg-info/top_level.txt
--rw-rw-r--   0 vpere     (1000) vpere     (1000)       38 2023-05-16 09:40:16.635904 scrapere-0.1.7/setup.cfg
--rw-rw-r--   0 vpere     (1000) vpere     (1000)      727 2023-05-16 09:39:05.000000 scrapere-0.1.7/setup.py
+drwxrwxr-x   0 vpere     (1000) vpere     (1000)        0 2023-05-16 09:58:53.279828 scrapere-0.1.8/
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)      979 2023-05-16 09:58:53.279828 scrapere-0.1.8/PKG-INFO
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)      743 2023-05-16 09:56:14.000000 scrapere-0.1.8/README.md
+drwxrwxr-x   0 vpere     (1000) vpere     (1000)        0 2023-05-16 09:58:53.275828 scrapere-0.1.8/scrapere/
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)       22 2023-05-04 10:22:06.000000 scrapere-0.1.8/scrapere/__init__.py
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)     4771 2023-05-16 09:54:43.000000 scrapere-0.1.8/scrapere/toolbox.py
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)  2656644 2023-05-04 09:43:57.000000 scrapere-0.1.8/scrapere/user-agents-unique.txt
+drwxrwxr-x   0 vpere     (1000) vpere     (1000)        0 2023-05-16 09:58:53.279828 scrapere-0.1.8/scrapere.egg-info/
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)      979 2023-05-16 09:58:53.000000 scrapere-0.1.8/scrapere.egg-info/PKG-INFO
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)      250 2023-05-16 09:58:53.000000 scrapere-0.1.8/scrapere.egg-info/SOURCES.txt
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)        1 2023-05-16 09:58:53.000000 scrapere-0.1.8/scrapere.egg-info/dependency_links.txt
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)       39 2023-05-16 09:58:53.000000 scrapere-0.1.8/scrapere.egg-info/requires.txt
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)        9 2023-05-16 09:58:53.000000 scrapere-0.1.8/scrapere.egg-info/top_level.txt
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)       38 2023-05-16 09:58:53.279828 scrapere-0.1.8/setup.cfg
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)      727 2023-05-16 09:55:24.000000 scrapere-0.1.8/setup.py
```

### Comparing `scrapere-0.1.7/PKG-INFO` & `scrapere-0.1.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: scrapere
-Version: 0.1.7
+Version: 0.1.8
 Summary: Small set of my web scraping python tools
 Home-page: https://github.com/vPere/scrapere
 Author: vPere
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # Scraping libary
 
 This is a simple toolbox for scraping info from websites which includes methods for generating headers with a random user agent picked from a list of more than 24k user agents, a method for waiting a random time between 1 and 3 seconds, a progress bar for it to look cool ;) and a couple of methods that will help you retreive email addresses and spanish phone numbers from a given url.
 
 As this package may be useful for a bunch of legitimate and non-legitimate use cases, I'm not responsible of whatever you do with it.
 
 
-## Version 0.1.6 issues:
+## Version 0.1.8 issues:
 - There are no tests...
 - scrap_phones() only works for spanish phone numbers
 
 As this is my first python package, I might not mantain it, so better try finding another one...
```

### Comparing `scrapere-0.1.7/scrapere/toolbox.py` & `scrapere-0.1.8/scrapere/toolbox.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         for _ in fp:
             total += 1
     return total
 
 
 def get_user_agent_list():
     user_agent_list = []
-    with open('./user-agents-unique.txt', 'r') as f:
+    with open('user-agents-unique.txt', 'r') as f:
         for line in f:
             user_agent_list.append(line.strip())
     return user_agent_list
 
 
 def get_random_user_agent():
     user_agent_list = get_user_agent_list()
```

### Comparing `scrapere-0.1.7/scrapere/user-agents-unique.txt` & `scrapere-0.1.8/scrapere/user-agents-unique.txt`

 * *Files identical despite different names*

### Comparing `scrapere-0.1.7/scrapere.egg-info/PKG-INFO` & `scrapere-0.1.8/scrapere.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: scrapere
-Version: 0.1.7
+Version: 0.1.8
 Summary: Small set of my web scraping python tools
 Home-page: https://github.com/vPere/scrapere
 Author: vPere
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # Scraping libary
 
 This is a simple toolbox for scraping info from websites which includes methods for generating headers with a random user agent picked from a list of more than 24k user agents, a method for waiting a random time between 1 and 3 seconds, a progress bar for it to look cool ;) and a couple of methods that will help you retreive email addresses and spanish phone numbers from a given url.
 
 As this package may be useful for a bunch of legitimate and non-legitimate use cases, I'm not responsible of whatever you do with it.
 
 
-## Version 0.1.6 issues:
+## Version 0.1.8 issues:
 - There are no tests...
 - scrap_phones() only works for spanish phone numbers
 
 As this is my first python package, I might not mantain it, so better try finding another one...
```

### Comparing `scrapere-0.1.7/setup.py` & `scrapere-0.1.8/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='scrapere',
     packages=find_packages(),
-    version='0.1.7',
+    version='0.1.8',
     description='Small set of my web scraping python tools',
     author='vPere',
     license='MIT',
     readme='README.md',
     install_requires=[
         'requests',
         'beautifulsoup4',
```

