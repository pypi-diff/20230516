# Comparing `tmp/scrapere-0.1.5.tar.gz` & `tmp/scrapere-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapere-0.1.5.tar", last modified: Fri May  5 09:02:57 2023, max compression
+gzip compressed data, was "scrapere-0.1.6.tar", last modified: Tue May 16 09:33:17 2023, max compression
```

## Comparing `scrapere-0.1.5.tar` & `scrapere-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 vpere     (1000) vpere     (1000)        0 2023-05-05 09:02:57.088691 scrapere-0.1.5/
--rw-rw-r--   0 vpere     (1000) vpere     (1000)     1068 2023-05-05 09:02:57.088691 scrapere-0.1.5/PKG-INFO
--rw-rw-r--   0 vpere     (1000) vpere     (1000)      832 2023-05-05 08:58:03.000000 scrapere-0.1.5/README.md
-drwxrwxr-x   0 vpere     (1000) vpere     (1000)        0 2023-05-05 09:02:57.084691 scrapere-0.1.5/scrapere/
--rw-rw-r--   0 vpere     (1000) vpere     (1000)       22 2023-05-04 10:22:06.000000 scrapere-0.1.5/scrapere/__init__.py
--rw-rw-r--   0 vpere     (1000) vpere     (1000)     4741 2023-05-05 07:53:35.000000 scrapere-0.1.5/scrapere/toolbox.py
--rw-rw-r--   0 vpere     (1000) vpere     (1000)  2656644 2023-05-04 09:43:57.000000 scrapere-0.1.5/scrapere/user-agents-unique.txt
-drwxrwxr-x   0 vpere     (1000) vpere     (1000)        0 2023-05-05 09:02:57.088691 scrapere-0.1.5/scrapere.egg-info/
--rw-rw-r--   0 vpere     (1000) vpere     (1000)     1068 2023-05-05 09:02:57.000000 scrapere-0.1.5/scrapere.egg-info/PKG-INFO
--rw-rw-r--   0 vpere     (1000) vpere     (1000)      250 2023-05-05 09:02:57.000000 scrapere-0.1.5/scrapere.egg-info/SOURCES.txt
--rw-rw-r--   0 vpere     (1000) vpere     (1000)        1 2023-05-05 09:02:57.000000 scrapere-0.1.5/scrapere.egg-info/dependency_links.txt
--rw-rw-r--   0 vpere     (1000) vpere     (1000)       39 2023-05-05 09:02:57.000000 scrapere-0.1.5/scrapere.egg-info/requires.txt
--rw-rw-r--   0 vpere     (1000) vpere     (1000)        9 2023-05-05 09:02:57.000000 scrapere-0.1.5/scrapere.egg-info/top_level.txt
--rw-rw-r--   0 vpere     (1000) vpere     (1000)       38 2023-05-05 09:02:57.088691 scrapere-0.1.5/setup.cfg
--rw-rw-r--   0 vpere     (1000) vpere     (1000)      727 2023-05-05 09:00:36.000000 scrapere-0.1.5/setup.py
+drwxrwxr-x   0 vpere     (1000) vpere     (1000)        0 2023-05-16 09:33:17.787330 scrapere-0.1.6/
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)      979 2023-05-16 09:33:17.787330 scrapere-0.1.6/PKG-INFO
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)      743 2023-05-16 09:32:49.000000 scrapere-0.1.6/README.md
+drwxrwxr-x   0 vpere     (1000) vpere     (1000)        0 2023-05-16 09:33:17.771330 scrapere-0.1.6/scrapere/
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)       22 2023-05-04 10:22:06.000000 scrapere-0.1.6/scrapere/__init__.py
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)     4773 2023-05-16 09:32:45.000000 scrapere-0.1.6/scrapere/toolbox.py
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)  2656644 2023-05-04 09:43:57.000000 scrapere-0.1.6/scrapere/user-agents-unique.txt
+drwxrwxr-x   0 vpere     (1000) vpere     (1000)        0 2023-05-16 09:33:17.783330 scrapere-0.1.6/scrapere.egg-info/
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)      979 2023-05-16 09:33:17.000000 scrapere-0.1.6/scrapere.egg-info/PKG-INFO
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)      250 2023-05-16 09:33:17.000000 scrapere-0.1.6/scrapere.egg-info/SOURCES.txt
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)        1 2023-05-16 09:33:17.000000 scrapere-0.1.6/scrapere.egg-info/dependency_links.txt
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)       39 2023-05-16 09:33:17.000000 scrapere-0.1.6/scrapere.egg-info/requires.txt
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)        9 2023-05-16 09:33:17.000000 scrapere-0.1.6/scrapere.egg-info/top_level.txt
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)       38 2023-05-16 09:33:17.787330 scrapere-0.1.6/setup.cfg
+-rw-rw-r--   0 vpere     (1000) vpere     (1000)      727 2023-05-16 09:32:43.000000 scrapere-0.1.6/setup.py
```

### Comparing `scrapere-0.1.5/PKG-INFO` & `scrapere-0.1.6/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: scrapere
-Version: 0.1.5
+Version: 0.1.6
 Summary: Small set of my web scraping python tools
 Home-page: https://github.com/vPere/scrapere
 Author: vPere
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # Scraping libary
 
 This is a simple toolbox for scraping info from websites which includes methods for generating headers with a random user agent picked from a list of more than 24k user agents, a method for waiting a random time between 1 and 3 seconds, a progress bar for it to look cool ;) and a couple of methods that will help you retreive email addresses and spanish phone numbers from a given url.
 
 As this package may be useful for a bunch of legitimate and non-legitimate use cases, I'm not responsible of whatever you do with it.
 
 
-## Version 0.1.5 issues:
+## Version 0.1.6 issues:
 - There are no tests...
 - scrap_phones() only works for spanish phone numbers
-- Honestly, scrap_emails() was generated by github copilot and has not been tried yet...
 
 As this is my first python package, I might not mantain it, so better try finding another one...
```

### Comparing `scrapere-0.1.5/README.md` & `scrapere-0.1.6/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # Scraping libary
 
 This is a simple toolbox for scraping info from websites which includes methods for generating headers with a random user agent picked from a list of more than 24k user agents, a method for waiting a random time between 1 and 3 seconds, a progress bar for it to look cool ;) and a couple of methods that will help you retreive email addresses and spanish phone numbers from a given url.
 
 As this package may be useful for a bunch of legitimate and non-legitimate use cases, I'm not responsible of whatever you do with it.
 
 
-## Version 0.1.5 issues:
+## Version 0.1.6 issues:
 - There are no tests...
 - scrap_phones() only works for spanish phone numbers
-- Honestly, scrap_emails() was generated by github copilot and has not been tried yet...
 
 As this is my first python package, I might not mantain it, so better try finding another one...
```

### Comparing `scrapere-0.1.5/scrapere/toolbox.py` & `scrapere-0.1.6/scrapere/toolbox.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,15 @@
             writer = csv.DictWriter(f, fieldnames=['url', 'email'])
             writer.writerow({'url': row[0], 'email': row[1]})
     print("Wrote CSV file with " + str(len(valid_emails)) + " valid emails")
 
 
 def scrap_phones(url):
     phones = []
+    counter = 0
     try:
         counter += 1
         print(f"Crawling through {url}...")
         response = requests.get(url, generate_header())
         soup = BeautifulSoup(response.content, 'html.parser')
         for phone in re.findall(r'(?:\+34|0034)?\s?(?:6|9)(?:\d\s?\d{2}\s?\d{2}\s?\d{2}|\d{2}\s?\d{3}\s?\d{3}|\d{3}\s?\d{2}\s?\d{2})', str(soup)):
             phone = phone.replace(" ", "")
@@ -103,14 +104,15 @@
     except requests.exceptions.RequestException as e:
         print(f"Failed to crawl {url}: {e}")
     print(Fore.LIGHTGREEN_EX + "Found " + str(len(phones)) + " phone numbers in " + url)
 
 
 def scrap_emails(url):
     emails = []
+    counter = 0
     try:
         counter += 1
         print(f"Crawling through {url}...")
         response = requests.get(url, generate_header())
         soup = BeautifulSoup(response.content, 'html.parser')
         for email in re.findall(r'[\w\.-]+@[\w\.-]+', str(soup)):
             if is_valid_email(email):
```

### Comparing `scrapere-0.1.5/scrapere/user-agents-unique.txt` & `scrapere-0.1.6/scrapere/user-agents-unique.txt`

 * *Files identical despite different names*

### Comparing `scrapere-0.1.5/scrapere.egg-info/PKG-INFO` & `scrapere-0.1.6/scrapere.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: scrapere
-Version: 0.1.5
+Version: 0.1.6
 Summary: Small set of my web scraping python tools
 Home-page: https://github.com/vPere/scrapere
 Author: vPere
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # Scraping libary
 
 This is a simple toolbox for scraping info from websites which includes methods for generating headers with a random user agent picked from a list of more than 24k user agents, a method for waiting a random time between 1 and 3 seconds, a progress bar for it to look cool ;) and a couple of methods that will help you retreive email addresses and spanish phone numbers from a given url.
 
 As this package may be useful for a bunch of legitimate and non-legitimate use cases, I'm not responsible of whatever you do with it.
 
 
-## Version 0.1.5 issues:
+## Version 0.1.6 issues:
 - There are no tests...
 - scrap_phones() only works for spanish phone numbers
-- Honestly, scrap_emails() was generated by github copilot and has not been tried yet...
 
 As this is my first python package, I might not mantain it, so better try finding another one...
```

### Comparing `scrapere-0.1.5/setup.py` & `scrapere-0.1.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='scrapere',
     packages=find_packages(),
-    version='0.1.5',
+    version='0.1.6',
     description='Small set of my web scraping python tools',
     author='vPere',
     license='MIT',
     readme='README.md',
     install_requires=[
         'requests',
         'beautifulsoup4',
```

