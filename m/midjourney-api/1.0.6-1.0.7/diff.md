# Comparing `tmp/midjourney_api-1.0.6.tar.gz` & `tmp/midjourney_api-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "midjourney_api-1.0.6.tar", last modified: Mon May 15 05:19:23 2023, max compression
+gzip compressed data, was "midjourney_api-1.0.7.tar", last modified: Tue May 16 01:26:42 2023, max compression
```

## Comparing `midjourney_api-1.0.6.tar` & `midjourney_api-1.0.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 05:19:23.100782 midjourney_api-1.0.6/
--rw-rw-rw-   0        0        0     7408 2023-05-15 05:19:23.100782 midjourney_api-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     6576 2023-05-15 05:12:35.000000 midjourney_api-1.0.6/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-15 05:19:23.084771 midjourney_api-1.0.6/midjourney_api/
--rw-rw-rw-   0        0        0     6002 2023-05-15 05:18:58.000000 midjourney_api-1.0.6/midjourney_api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 05:19:23.092768 midjourney_api-1.0.6/midjourney_api.egg-info/
--rw-rw-rw-   0        0        0     7408 2023-05-15 05:19:22.000000 midjourney_api-1.0.6/midjourney_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      198 2023-05-15 05:19:22.000000 midjourney_api-1.0.6/midjourney_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 05:19:22.000000 midjourney_api-1.0.6/midjourney_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-15 05:19:22.000000 midjourney_api-1.0.6/midjourney_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-15 05:19:23.100782 midjourney_api-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1747 2023-05-15 05:09:01.000000 midjourney_api-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 01:26:42.781098 midjourney_api-1.0.7/
+-rw-rw-rw-   0        0        0     7408 2023-05-16 01:26:42.778076 midjourney_api-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     6576 2023-05-15 05:12:35.000000 midjourney_api-1.0.7/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-16 01:26:42.766968 midjourney_api-1.0.7/midjourney_api/
+-rw-rw-rw-   0        0        0     6005 2023-05-16 01:24:58.000000 midjourney_api-1.0.7/midjourney_api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 01:26:42.775965 midjourney_api-1.0.7/midjourney_api.egg-info/
+-rw-rw-rw-   0        0        0     7408 2023-05-16 01:26:42.000000 midjourney_api-1.0.7/midjourney_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      198 2023-05-16 01:26:42.000000 midjourney_api-1.0.7/midjourney_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 01:26:42.000000 midjourney_api-1.0.7/midjourney_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-16 01:26:42.000000 midjourney_api-1.0.7/midjourney_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-16 01:26:42.782091 midjourney_api-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1747 2023-05-16 01:26:40.000000 midjourney_api-1.0.7/setup.py
```

### Comparing `midjourney_api-1.0.6/PKG-INFO` & `midjourney_api-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midjourney_api
-Version: 1.0.6
+Version: 1.0.7
 Summary: Midjourney API wrapper by The Next Leg
 Home-page: https://github.com/midjourney-api-the-next-leg/python-midjourney-api
 Download-URL: https://github.com/midjourney-api-the-next-leg/python-midjourney-api/archive/refs/tags/v1.0.0.tar.gz
 Author: The Next leg
 Author-email: support@thenextleg.io
 License: MIT
 Keywords: MIDJOURNEY,API,THE_NEXT_LEG
```

### Comparing `midjourney_api-1.0.6/README.rst` & `midjourney_api-1.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `midjourney_api-1.0.6/midjourney_api/__init__.py` & `midjourney_api-1.0.7/midjourney_api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         ARGS:
             button: str - The button to press.
             button_message_id: str - The message id of the button.
             ref: str - A reference string passed back in the webhook
             webhook_override: str - A webhook to override the default webhook.
         """
         request = {
-            "cmd": button,
+            "button": button,
             "buttonMessageId": button_message_id,
             "ref": ref,
             "webhookOverride": webhook_override,
         }
 
         res = requests.post(
             f"{BASE_URL}/button", json=request, headers=self.create_headers()
```

### Comparing `midjourney_api-1.0.6/midjourney_api.egg-info/PKG-INFO` & `midjourney_api-1.0.7/midjourney_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midjourney-api
-Version: 1.0.6
+Version: 1.0.7
 Summary: Midjourney API wrapper by The Next Leg
 Home-page: https://github.com/midjourney-api-the-next-leg/python-midjourney-api
 Download-URL: https://github.com/midjourney-api-the-next-leg/python-midjourney-api/archive/refs/tags/v1.0.0.tar.gz
 Author: The Next leg
 Author-email: support@thenextleg.io
 License: MIT
 Keywords: MIDJOURNEY,API,THE_NEXT_LEG
```

### Comparing `midjourney_api-1.0.6/setup.py` & `midjourney_api-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 setuptools.setup(
     name="midjourney_api",  # How you named your package folder (MyLib)
     packages=["midjourney_api"],  # Chose the same as "name"
-    version="1.0.6",  # Start with a small number and increase it with every change you make
+    version="1.0.7",  # Start with a small number and increase it with every change you make
     license="MIT",  # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     long_description=open("README.rst").read(),
     description="Midjourney API wrapper by The Next Leg",  # Give a short description about your library
     author="The Next leg",  # Type in your name
     author_email="support@thenextleg.io",  # Type in your E-Mail
     url="https://github.com/midjourney-api-the-next-leg/python-midjourney-api",  # Provide either the link to your github or to your website
     download_url="https://github.com/midjourney-api-the-next-leg/python-midjourney-api/archive/refs/tags/v1.0.0.tar.gz",  # I explain this later on
```

