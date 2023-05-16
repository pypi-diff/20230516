# Comparing `tmp/arequestsHelper-0.4.2.tar.gz` & `tmp/arequestsHelper-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arequestsHelper-0.4.2.tar", last modified: Sun May  7 16:42:22 2023, max compression
+gzip compressed data, was "arequestsHelper-0.4.3.tar", last modified: Tue May 16 10:00:48 2023, max compression
```

## Comparing `arequestsHelper-0.4.2.tar` & `arequestsHelper-0.4.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 kaixenix  (1000) kaixenix  (1000)        0 2023-05-07 16:42:22.803092 arequestsHelper-0.4.2/
--rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)     1074 2023-05-07 16:38:56.000000 arequestsHelper-0.4.2/LICENSE
--rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)      789 2023-05-07 16:42:22.803092 arequestsHelper-0.4.2/PKG-INFO
--rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)      365 2023-05-07 16:38:56.000000 arequestsHelper-0.4.2/README.md
-drwxr-xr-x   0 kaixenix  (1000) kaixenix  (1000)        0 2023-05-07 16:42:22.802092 arequestsHelper-0.4.2/arequestsHelper/
--rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)       61 2023-05-07 16:38:56.000000 arequestsHelper-0.4.2/arequestsHelper/__init__.py
--rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)     4578 2023-05-07 16:40:12.000000 arequestsHelper-0.4.2/arequestsHelper/arequestsHelper.py
--rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)      149 2023-05-07 16:38:56.000000 arequestsHelper-0.4.2/arequestsHelper/errors.py
-drwxr-xr-x   0 kaixenix  (1000) kaixenix  (1000)        0 2023-05-07 16:42:22.803092 arequestsHelper-0.4.2/arequestsHelper.egg-info/
--rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)      789 2023-05-07 16:42:22.000000 arequestsHelper-0.4.2/arequestsHelper.egg-info/PKG-INFO
--rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)      319 2023-05-07 16:42:22.000000 arequestsHelper-0.4.2/arequestsHelper.egg-info/SOURCES.txt
--rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)        1 2023-05-07 16:42:22.000000 arequestsHelper-0.4.2/arequestsHelper.egg-info/dependency_links.txt
--rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)       17 2023-05-07 16:42:22.000000 arequestsHelper-0.4.2/arequestsHelper.egg-info/requires.txt
--rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)       16 2023-05-07 16:42:22.000000 arequestsHelper-0.4.2/arequestsHelper.egg-info/top_level.txt
--rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)       79 2023-05-07 16:42:22.803092 arequestsHelper-0.4.2/setup.cfg
--rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)     1757 2023-05-07 16:42:06.000000 arequestsHelper-0.4.2/setup.py
+drwxr-xr-x   0 kaixenix  (1000) kaixenix  (1000)        0 2023-05-16 10:00:48.284650 arequestsHelper-0.4.3/
+-rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)     1074 2023-05-07 16:38:56.000000 arequestsHelper-0.4.3/LICENSE
+-rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)      789 2023-05-16 10:00:48.284650 arequestsHelper-0.4.3/PKG-INFO
+-rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)      365 2023-05-07 16:38:56.000000 arequestsHelper-0.4.3/README.md
+drwxr-xr-x   0 kaixenix  (1000) kaixenix  (1000)        0 2023-05-16 10:00:48.283650 arequestsHelper-0.4.3/arequestsHelper/
+-rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)       61 2023-05-07 16:38:56.000000 arequestsHelper-0.4.3/arequestsHelper/__init__.py
+-rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)     5287 2023-05-16 09:55:03.000000 arequestsHelper-0.4.3/arequestsHelper/arequestsHelper.py
+-rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)      149 2023-05-07 16:38:56.000000 arequestsHelper-0.4.3/arequestsHelper/errors.py
+drwxr-xr-x   0 kaixenix  (1000) kaixenix  (1000)        0 2023-05-16 10:00:48.284650 arequestsHelper-0.4.3/arequestsHelper.egg-info/
+-rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)      789 2023-05-16 10:00:48.000000 arequestsHelper-0.4.3/arequestsHelper.egg-info/PKG-INFO
+-rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)      319 2023-05-16 10:00:48.000000 arequestsHelper-0.4.3/arequestsHelper.egg-info/SOURCES.txt
+-rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)        1 2023-05-16 10:00:48.000000 arequestsHelper-0.4.3/arequestsHelper.egg-info/dependency_links.txt
+-rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)       17 2023-05-16 10:00:48.000000 arequestsHelper-0.4.3/arequestsHelper.egg-info/requires.txt
+-rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)       16 2023-05-16 10:00:48.000000 arequestsHelper-0.4.3/arequestsHelper.egg-info/top_level.txt
+-rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)       79 2023-05-16 10:00:48.284650 arequestsHelper-0.4.3/setup.cfg
+-rw-r--r--   0 kaixenix  (1000) kaixenix  (1000)     1757 2023-05-16 10:00:42.000000 arequestsHelper-0.4.3/setup.py
```

### Comparing `arequestsHelper-0.4.2/LICENSE` & `arequestsHelper-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `arequestsHelper-0.4.2/PKG-INFO` & `arequestsHelper-0.4.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: arequestsHelper
-Version: 0.4.2
+Version: 0.4.3
 Summary: This pakage helps to work with aiohttp requests in many threads
 Home-page: https://github.com/Harukvitalii
-Download-URL: https://github.com/Harukvitalii/ArequestHelper/archive/refs/tags/v0.4.2.zip
+Download-URL: https://github.com/Harukvitalii/ArequestHelper/archive/refs/tags/v0.4.3.zip
 Author: Vitalii Haruk
 Author-email: garuk1vitalik@gmail.com
 License: MIT
 Keywords: aiohttp,requests,threads
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `arequestsHelper-0.4.2/arequestsHelper/arequestsHelper.py` & `arequestsHelper-0.4.3/arequestsHelper/arequestsHelper.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import aiohttp
 import requests
 import json
 import sys,os
 import asyncio
 import time
 from .errors import errs
+import traceback
 
 from requests.packages.urllib3.exceptions import InsecureRequestWarning
 requests.packages.urllib3.disable_warnings(InsecureRequestWarning)
 
 
 
 class AREQUEST_MANAGER:
@@ -86,32 +87,42 @@
         URL = 'https://api.telegram.org/bot' + BOT_TOKEN +'/sendMessage'
         PARAMS = {'chat_id':self.admin_id,
                     "text":text}
         r = requests.get(url = URL, params = PARAMS,verify=False)
         return r
     
     
-    def run_function_with_exception(self, func, start_abr_for_notification: str, func_args = (),  tries: int = 10,attempt = 1, otladka: bool = False):
+    def run_function_with_exception(self, func, start_abr_for_notification: str, func_args = (),  tries: int = 10,attempt = 1, otladka: bool = False, error_trace = False):
         if otladka:
             asyncio.run(func(func_args))
-            print('done Success')
+            print('test Run successfully')
             exit()
             
             
-        while True:
+        while attempt != tries:
             try: 
                 asyncio.run(func(func_args))
                 
-            except Exception as e:
-                print(e)
-                # print(errs['ERROR'])
-                exc_type, exc_obj, exc_tb = sys.exc_info()
-                fname = os.path.split(exc_tb.tb_frame.f_code.co_filename)[1]
-                print(exc_type, fname, exc_tb.tb_lineno)
+            except aiohttp.client_exceptions.ClientOSError:
+                print(errs['System ERROR'])
                 time.sleep(10)
-                self.bot_notify_normal(f'{exc_type}, {fname}, { exc_tb.tb_lineno}')
-                self.bot_notify_normal(f'{start_abr_for_notification} ERROR {e}\nAttempt {attempt+1}')
                 self.run_function_with_exception(func,start_abr_for_notification,attempt=attempt+1)
-        
+                self.bot_notify_normal(f'{start_abr_for_notification} ERROR Winodws closed connection\nAttempt {attempt+1}')
+            except Exception as e:
+                print(e)
+                exc_type, exc_value, exc_traceback = sys.exc_info()
+                if error_trace: 
+                    traceback_text = ''.join(traceback.format_tb(exc_traceback))
+                    self.bot_notify_normal(traceback_text)
+                
+                tb_entry = traceback.extract_tb(exc_traceback)[-1]
+                fname = tb_entry.filename
+                line_number = tb_entry.lineno
+                print(f"Error occurred at line {line_number} in {fname}")
+                time.sleep(7)
+                self.bot_notify_normal(f"Error occurred at line {line_number} in {fname}")
+                self.bot_notify_normal(f'{start_abr_for_notification} ERROR {e}\nAttempt {attempt + 1}')
+                self.run_function_with_exception(func, start_abr_for_notification, attempt=attempt + 1)
+                
+    
         self.bot_notify_normal(f'{start_abr_for_notification} RESTART')
 
-
```

### Comparing `arequestsHelper-0.4.2/arequestsHelper.egg-info/PKG-INFO` & `arequestsHelper-0.4.3/arequestsHelper.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: arequestsHelper
-Version: 0.4.2
+Version: 0.4.3
 Summary: This pakage helps to work with aiohttp requests in many threads
 Home-page: https://github.com/Harukvitalii
-Download-URL: https://github.com/Harukvitalii/ArequestHelper/archive/refs/tags/v0.4.2.zip
+Download-URL: https://github.com/Harukvitalii/ArequestHelper/archive/refs/tags/v0.4.3.zip
 Author: Vitalii Haruk
 Author-email: garuk1vitalik@gmail.com
 License: MIT
 Keywords: aiohttp,requests,threads
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `arequestsHelper-0.4.2/setup.py` & `arequestsHelper-0.4.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from distutils.core import setup
 setup(
   name = 'arequestsHelper',         # How you named your package folder (MyLib)
   packages = ['arequestsHelper'],   # Chose the same as "name"
-  version = '0.4.2',      # Start with a small number and increase it with every change you make
+  version = '0.4.3',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = "This pakage helps to work with aiohttp requests in many threads",   # Give a short description about your library
   author = 'Vitalii Haruk',                   # Type in your name
   author_email = "garuk1vitalik@gmail.com",      # Type in your E-Mail
   url = "https://github.com/Harukvitalii",   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/Harukvitalii/ArequestHelper/archive/refs/tags/v0.4.2.zip',    # I explain this later on
+  download_url = 'https://github.com/Harukvitalii/ArequestHelper/archive/refs/tags/v0.4.3.zip',    # I explain this later on
   keywords = ['aiohttp', 'requests', 'threads'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'requests',
           'aiohttp',
       ],
   classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
```

