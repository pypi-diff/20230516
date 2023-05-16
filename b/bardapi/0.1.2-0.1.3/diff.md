# Comparing `tmp/bardapi-0.1.2.tar.gz` & `tmp/bardapi-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bardapi-0.1.2.tar", last modified: Thu May 11 19:19:55 2023, max compression
+gzip compressed data, was "bardapi-0.1.3.tar", last modified: Tue May 16 08:01:57 2023, max compression
```

## Comparing `bardapi-0.1.2.tar` & `bardapi-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 19:19:55.149331 bardapi-0.1.2/
--rw-rw-rw-   0        0        0     3538 2023-05-11 19:19:55.147848 bardapi-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2637 2023-05-11 19:19:14.000000 bardapi-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-11 19:19:55.126198 bardapi-0.1.2/bardapi/
--rw-rw-rw-   0        0        0      198 2023-05-11 19:19:42.000000 bardapi-0.1.2/bardapi/__init__.py
--rw-rw-rw-   0        0        0     2809 2023-05-11 19:18:58.000000 bardapi-0.1.2/bardapi/core.py
-drwxrwxrwx   0        0        0        0 2023-05-11 19:19:55.144693 bardapi-0.1.2/bardapi.egg-info/
--rw-rw-rw-   0        0        0     3538 2023-05-11 19:19:55.000000 bardapi-0.1.2/bardapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      212 2023-05-11 19:19:55.000000 bardapi-0.1.2/bardapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 19:19:55.000000 bardapi-0.1.2/bardapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-05-11 19:19:55.000000 bardapi-0.1.2/bardapi.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        8 2023-05-11 19:19:55.000000 bardapi-0.1.2/bardapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-11 19:19:55.149331 bardapi-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1747 2023-05-11 19:19:39.000000 bardapi-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 08:01:57.844025 bardapi-0.1.3/
+-rw-rw-rw-   0        0        0     1087 2023-04-13 16:54:50.000000 bardapi-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     6803 2023-05-16 08:01:57.842026 bardapi-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5871 2023-05-16 08:01:33.000000 bardapi-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-16 08:01:57.823303 bardapi-0.1.3/bardapi/
+-rw-rw-rw-   0        0        0      198 2023-05-16 08:00:37.000000 bardapi-0.1.3/bardapi/__init__.py
+-rw-rw-rw-   0        0        0     3421 2023-05-16 08:01:33.000000 bardapi-0.1.3/bardapi/core.py
+drwxrwxrwx   0        0        0        0 2023-05-16 08:01:57.840031 bardapi-0.1.3/bardapi.egg-info/
+-rw-rw-rw-   0        0        0     6803 2023-05-16 08:01:57.000000 bardapi-0.1.3/bardapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      220 2023-05-16 08:01:57.000000 bardapi-0.1.3/bardapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 08:01:57.000000 bardapi-0.1.3/bardapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-05-16 08:01:57.000000 bardapi-0.1.3/bardapi.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        8 2023-05-16 08:01:57.000000 bardapi-0.1.3/bardapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-16 08:01:57.844530 bardapi-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1755 2023-05-16 08:00:32.000000 bardapi-0.1.3/setup.py
```

### Comparing `bardapi-0.1.2/bardapi/core.py` & `bardapi-0.1.3/bardapi/core.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,26 @@
 import re
 import string
 import os
 import requests
 
 
 class Bard:
-    def __init__(self):
+    def __init__(self, timeout=6, proxies=None):
+        '''
+        Initialize Bard
+
+        :param timeout: (`int`, *optional*)
+            Timeout in seconds when connecting bard server. The timeout is used on each request.
+        :param proxies: (`Dict[str, str]`, *optional*)
+            A dictionary of proxy servers to use by protocol or endpoint, e.g., `{'http': 'foo.bar:3128',
+            'http://hostname': 'foo.bar:4012'}`. The proxies are used on each request.
+        '''
+        self.proxies = proxies
+        self.timeout = timeout
         headers = {
             "Host": "bard.google.com",
             "X-Same-Domain": "1",
             "User-Agent": "Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.114 Safari/537.36",
             "Content-Type": "application/x-www-form-urlencoded;charset=UTF-8",
             "Origin": "https://bard.google.com",
             "Referer": "https://bard.google.com/",
@@ -22,15 +33,15 @@
         self.choice_id = ""
         self.session = requests.Session()
         self.session.headers = headers
         self.session.cookies.set("__Secure-1PSID", os.environ["_BARD_API_KEY"])
         self.SNlM0e = self._get_snim0e()
 
     def _get_snim0e(self):
-        resp = self.session.get(url="https://bard.google.com/", timeout=5)
+        resp = self.session.get(url="https://bard.google.com/", timeout=self.timeout, proxies=self.proxies)
         if resp.status_code != 200:
             raise Exception(f"Response Status: {resp.status_code}")
         return re.search(r"SNlM0e\":\"(.*?)\"", resp.text).group(1)
 
     def get_answer(self, input_text: str) -> dict:
         params = {
             "bl": "boq_assistant-bard-web-server_20230419.00_p1",
@@ -46,15 +57,16 @@
             "f.req": json.dumps([None, json.dumps(input_text_struct)]),
             "at": self.SNlM0e,
         }
         resp = self.session.post(
             "https://bard.google.com/_/BardChatUi/data/assistant.lamda.BardFrontendService/StreamGenerate",
             params=params,
             data=data,
-            timeout=100,
+            timeout=self.timeout,
+            proxies=self.proxies
         )
 
         resp_dict = json.loads(resp.content.splitlines()[3])[0][2]
         if resp_dict is None:
             return {"content": f"Response Error: {resp.content}."}
         parsed_answer = json.loads(resp_dict)
         bard_answer = {
```

### Comparing `bardapi-0.1.2/setup.py` & `bardapi-0.1.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,27 +21,27 @@
 
 
 version = get_version()
 
 
 setup(
     name="bardapi",
-    version="0.1.2",
+    version="0.1.3",
     author="daniel park",
     author_email="parkminwoo1991@gmail.com",
-    description="A package that returns Response of Google BARD through API.",
+    description="The python package that returns Response of Google Bard through API.",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
-    url="https://github.com/dsdanielpark/BARD_API",
+    url="https://github.com/dsdanielpark/Bard-API",
     packages=find_packages(exclude=[]),
     python_requires=">=3.6",
     install_requires=[],
     keywords="BARD, Python, Google Bard, Large Language Model, Chatbot API, Google API, Chatbot",
     classifiers=[
-        "Development Status :: 3 - Alpha",
+        "Development Status :: 4 - Beta",
         "Intended Audience :: Science/Research",
         "Natural Language :: English",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "License :: OSI Approved :: MIT License",
```

