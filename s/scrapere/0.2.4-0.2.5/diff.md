# Comparing `tmp/scrapere-0.2.4.tar.gz` & `tmp/scrapere-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapere-0.2.4.tar", last modified: Tue May 16 11:53:56 2023, max compression
+gzip compressed data, was "scrapere-0.2.5.tar", last modified: Tue May 16 11:57:35 2023, max compression
```

## Comparing `scrapere-0.2.4.tar` & `scrapere-0.2.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 vpere     (1000) vpere     (1000)        0 2023-05-16 11:53:56.870625 scrapere-0.2.4/
--rw-rw-r--   0 vpere     (1000) vpere     (1000)     1035 2023-05-16 11:53:56.870625 scrapere-0.2.4/PKG-INFO
--rw-rw-r--   0 vpere     (1000) vpere     (1000)      799 2023-05-16 11:53:44.000000 scrapere-0.2.4/README.md
-drwxrwxr-x   0 vpere     (1000) vpere     (1000)        0 2023-05-16 11:53:56.870625 scrapere-0.2.4/scrapere/
--rw-rw-r--   0 vpere     (1000) vpere     (1000)       22 2023-05-16 10:14:19.000000 scrapere-0.2.4/scrapere/__init__.py
--rw-rw-r--   0 vpere     (1000) vpere     (1000)     5402 2023-05-16 11:53:44.000000 scrapere-0.2.4/scrapere/toolbox.py
--rw-rw-r--   0 vpere     (1000) vpere     (1000)  2656639 2023-05-16 10:19:54.000000 scrapere-0.2.4/scrapere/user_agents.txt
-drwxrwxr-x   0 vpere     (1000) vpere     (1000)        0 2023-05-16 11:53:56.870625 scrapere-0.2.4/scrapere.egg-info/
--rw-rw-r--   0 vpere     (1000) vpere     (1000)     1035 2023-05-16 11:53:56.000000 scrapere-0.2.4/scrapere.egg-info/PKG-INFO
--rw-rw-r--   0 vpere     (1000) vpere     (1000)      243 2023-05-16 11:53:56.000000 scrapere-0.2.4/scrapere.egg-info/SOURCES.txt
--rw-rw-r--   0 vpere     (1000) vpere     (1000)        1 2023-05-16 11:53:56.000000 scrapere-0.2.4/scrapere.egg-info/dependency_links.txt
--rw-rw-r--   0 vpere     (1000) vpere     (1000)       39 2023-05-16 11:53:56.000000 scrapere-0.2.4/scrapere.egg-info/requires.txt
--rw-rw-r--   0 vpere     (1000) vpere     (1000)        9 2023-05-16 11:53:56.000000 scrapere-0.2.4/scrapere.egg-info/top_level.txt
--rw-rw-r--   0 vpere     (1000) vpere     (1000)       38 2023-05-16 11:53:56.870625 scrapere-0.2.4/setup.cfg
--rw-rw-r--   0 vpere     (1000) vpere     (1000)      727 2023-05-16 11:53:54.000000 scrapere-0.2.4/setup.py
+drwxrwxr-x   0 vpere     (1000) vpere     (1000)        0 2023-05-16 11:57:35.346147 scrapere-0.2.5/
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)     1035 2023-05-16 11:57:35.346147 scrapere-0.2.5/PKG-INFO
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)      799 2023-05-16 11:57:28.000000 scrapere-0.2.5/README.md
+drwxrwxr-x   0 vpere     (1000) vpere     (1000)        0 2023-05-16 11:57:35.342147 scrapere-0.2.5/scrapere/
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)       22 2023-05-16 10:14:19.000000 scrapere-0.2.5/scrapere/__init__.py
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)     5387 2023-05-16 11:57:28.000000 scrapere-0.2.5/scrapere/toolbox.py
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)  2656639 2023-05-16 10:19:54.000000 scrapere-0.2.5/scrapere/user_agents.txt
+drwxrwxr-x   0 vpere     (1000) vpere     (1000)        0 2023-05-16 11:57:35.346147 scrapere-0.2.5/scrapere.egg-info/
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)     1035 2023-05-16 11:57:35.000000 scrapere-0.2.5/scrapere.egg-info/PKG-INFO
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)      243 2023-05-16 11:57:35.000000 scrapere-0.2.5/scrapere.egg-info/SOURCES.txt
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)        1 2023-05-16 11:57:35.000000 scrapere-0.2.5/scrapere.egg-info/dependency_links.txt
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)       39 2023-05-16 11:57:35.000000 scrapere-0.2.5/scrapere.egg-info/requires.txt
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)        9 2023-05-16 11:57:35.000000 scrapere-0.2.5/scrapere.egg-info/top_level.txt
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)       38 2023-05-16 11:57:35.346147 scrapere-0.2.5/setup.cfg
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)      727 2023-05-16 11:57:28.000000 scrapere-0.2.5/setup.py
```

### Comparing `scrapere-0.2.4/PKG-INFO` & `scrapere-0.2.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: scrapere
-Version: 0.2.4
+Version: 0.2.5
 Summary: Small set of my web scraping python tools
 Home-page: https://github.com/vPere/scrapere
 Author: vPere
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # Scraping libary
 
 This is a simple toolbox for scraping info from websites which includes methods for generating headers with a random user agent picked from a list of more than 24k user agents, a method for waiting a random time between 1 and 3 seconds, a progress bar for it to look cool ;) and a couple of methods that will help you retreive email addresses and spanish phone numbers from a given url.
 
 As this package may be useful for a bunch of legitimate and non-legitimate use cases, I'm not responsible of whatever you do with it.
 
-## Version 0.2.4 features:
+## Version 0.2.5 features:
  - Improves the email regex.
 
-## Version 0.2.4 issues:
+## Version 0.2.5 issues:
 - There are no tests...
 - scrap_phones() only works for spanish phone numbers
 
 As this is my first python package, I might not mantain it, so better try finding another one...
```

### Comparing `scrapere-0.2.4/README.md` & `scrapere-0.2.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Scraping libary
 
 This is a simple toolbox for scraping info from websites which includes methods for generating headers with a random user agent picked from a list of more than 24k user agents, a method for waiting a random time between 1 and 3 seconds, a progress bar for it to look cool ;) and a couple of methods that will help you retreive email addresses and spanish phone numbers from a given url.
 
 As this package may be useful for a bunch of legitimate and non-legitimate use cases, I'm not responsible of whatever you do with it.
 
-## Version 0.2.4 features:
+## Version 0.2.5 features:
  - Improves the email regex.
 
-## Version 0.2.4 issues:
+## Version 0.2.5 issues:
 - There are no tests...
 - scrap_phones() only works for spanish phone numbers
 
 As this is my first python package, I might not mantain it, so better try finding another one...
```

### Comparing `scrapere-0.2.4/scrapere/toolbox.py` & `scrapere-0.2.5/scrapere/toolbox.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
 
 def is_valid_email(email):
     if email.endswith('.png') or email.endswith('.jpg') or email.endswith('.gif') or email.endswith('.svg'):
         return False
     if email.endswith('@sentry-next.wixpress.com') or email.endswith('@sentry.io') or email.endswith('@sentry.wixpress.com') or email.endswith('@example.com') or email.endswith('@prestashop.com') or email.endswith('@202-ecommerce.com') or email.endswith('@e-mail.com'):
         return False
-    match = re.match(r'^[a-zA-Z]+[.][a-zA-Z]+@', email)
+    match = re.match(EMAIL_REGEX, email)
     if match and match.group() == 'nombre.apellido@':
         return False
     return True
 
 
 def filter_valid_emails_from_file(file_name):
     valid_emails = []
```

### Comparing `scrapere-0.2.4/scrapere/user_agents.txt` & `scrapere-0.2.5/scrapere/user_agents.txt`

 * *Files identical despite different names*

### Comparing `scrapere-0.2.4/scrapere.egg-info/PKG-INFO` & `scrapere-0.2.5/scrapere.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: scrapere
-Version: 0.2.4
+Version: 0.2.5
 Summary: Small set of my web scraping python tools
 Home-page: https://github.com/vPere/scrapere
 Author: vPere
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # Scraping libary
 
 This is a simple toolbox for scraping info from websites which includes methods for generating headers with a random user agent picked from a list of more than 24k user agents, a method for waiting a random time between 1 and 3 seconds, a progress bar for it to look cool ;) and a couple of methods that will help you retreive email addresses and spanish phone numbers from a given url.
 
 As this package may be useful for a bunch of legitimate and non-legitimate use cases, I'm not responsible of whatever you do with it.
 
-## Version 0.2.4 features:
+## Version 0.2.5 features:
  - Improves the email regex.
 
-## Version 0.2.4 issues:
+## Version 0.2.5 issues:
 - There are no tests...
 - scrap_phones() only works for spanish phone numbers
 
 As this is my first python package, I might not mantain it, so better try finding another one...
```

### Comparing `scrapere-0.2.4/setup.py` & `scrapere-0.2.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='scrapere',
     packages=find_packages(),
-    version='0.2.4',
+    version='0.2.5',
     description='Small set of my web scraping python tools',
     author='vPere',
     license='MIT',
     readme='README.md',
     install_requires=[
         'requests',
         'beautifulsoup4',
```

