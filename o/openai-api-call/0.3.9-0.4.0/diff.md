# Comparing `tmp/openai_api_call-0.3.9.tar.gz` & `tmp/openai_api_call-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_api_call-0.3.9.tar", last modified: Mon May  8 01:47:42 2023, max compression
+gzip compressed data, was "openai_api_call-0.4.0.tar", last modified: Tue May 16 08:37:08 2023, max compression
```

## Comparing `openai_api_call-0.3.9.tar` & `openai_api_call-0.4.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:47:42.665205 openai_api_call-0.3.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-08 01:47:31.000000 openai_api_call-0.3.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-05-08 01:47:42.665205 openai_api_call-0.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-05-08 01:47:31.000000 openai_api_call-0.3.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:47:42.665205 openai_api_call-0.3.9/openai_api_call/
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-08 01:47:31.000000 openai_api_call-0.3.9/openai_api_call/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8168 2023-05-08 01:47:31.000000 openai_api_call-0.3.9/openai_api_call/chattool.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-08 01:47:31.000000 openai_api_call-0.3.9/openai_api_call/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-05-08 01:47:31.000000 openai_api_call-0.3.9/openai_api_call/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-05-08 01:47:31.000000 openai_api_call-0.3.9/openai_api_call/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-05-08 01:47:31.000000 openai_api_call-0.3.9/openai_api_call/response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:47:42.665205 openai_api_call-0.3.9/openai_api_call.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-05-08 01:47:42.000000 openai_api_call-0.3.9/openai_api_call.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-08 01:47:42.000000 openai_api_call-0.3.9/openai_api_call.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 01:47:42.000000 openai_api_call-0.3.9/openai_api_call.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-08 01:47:42.000000 openai_api_call-0.3.9/openai_api_call.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 01:47:42.000000 openai_api_call-0.3.9/openai_api_call.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-08 01:47:42.000000 openai_api_call-0.3.9/openai_api_call.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-08 01:47:42.000000 openai_api_call-0.3.9/openai_api_call.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 01:47:42.665205 openai_api_call-0.3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-08 01:47:31.000000 openai_api_call-0.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:37:08.219377 openai_api_call-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-16 08:36:50.000000 openai_api_call-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-05-16 08:37:08.219377 openai_api_call-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-05-16 08:36:50.000000 openai_api_call-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:37:08.219377 openai_api_call-0.4.0/openai_api_call/
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-16 08:36:50.000000 openai_api_call-0.4.0/openai_api_call/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8300 2023-05-16 08:36:50.000000 openai_api_call-0.4.0/openai_api_call/chattool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-16 08:36:50.000000 openai_api_call-0.4.0/openai_api_call/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-05-16 08:36:50.000000 openai_api_call-0.4.0/openai_api_call/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-05-16 08:36:50.000000 openai_api_call-0.4.0/openai_api_call/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-05-16 08:36:50.000000 openai_api_call-0.4.0/openai_api_call/response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:37:08.219377 openai_api_call-0.4.0/openai_api_call.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-05-16 08:37:07.000000 openai_api_call-0.4.0/openai_api_call.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-16 08:37:08.000000 openai_api_call-0.4.0/openai_api_call.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 08:37:07.000000 openai_api_call-0.4.0/openai_api_call.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-16 08:37:07.000000 openai_api_call-0.4.0/openai_api_call.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 08:37:07.000000 openai_api_call-0.4.0/openai_api_call.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-16 08:37:07.000000 openai_api_call-0.4.0/openai_api_call.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-16 08:37:07.000000 openai_api_call-0.4.0/openai_api_call.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 08:37:08.219377 openai_api_call-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-16 08:36:50.000000 openai_api_call-0.4.0/setup.py
```

### Comparing `openai_api_call-0.3.9/LICENSE` & `openai_api_call-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_api_call-0.3.9/PKG-INFO` & `openai_api_call-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: openai_api_call
-Version: 0.3.9
+Version: 0.4.0
 Summary: A short wrapper of the OpenAI api call.
-Home-page: https://github.com/RexWzh/openai_api_call
+Home-page: https://github.com/cubenlp/openai_api_call
 Author: Rex Wang
 Author-email: 1073853456@qq.com
 License: MIT license
 Description: > **中文文档移步[这里](README_zh_CN.md)。**
         
         # Openai API call
         [![PyPI version](https://img.shields.io/pypi/v/openai_api_call.svg)](https://pypi.python.org/pypi/openai_api_call)
-        [![Tests](https://github.com/RexWzh/openai_api_call/actions/workflows/test.yml/badge.svg)](https://github.com/RexWzh/openai_api_call/actions/workflows/test.yml/)
+        [![Tests](https://github.com/cubenlp/openai_api_call/actions/workflows/test.yml/badge.svg)](https://github.com/cubenlp/openai_api_call/actions/workflows/test.yml/)
         [![Documentation Status](https://img.shields.io/badge/docs-github_pages-blue.svg)](https://apicall.wzhecnu.cn)
-        [![Coverage](https://codecov.io/gh/RexWzh/openai_api_call/branch/master/graph/badge.svg)](https://codecov.io/gh/RexWzh/openai_api_call.jl)
+        [![Coverage](https://codecov.io/gh/cubenlp/openai_api_call/branch/master/graph/badge.svg)](https://codecov.io/gh/cubenlp/openai_api_call.jl)
         
         <!-- 
-        [![Updates](https://pyup.io/repos/github/RexWzh/openai_api_call/shield.svg)](https://pyup.io/repos/github/RexWzh/openai_api_call/) 
+        [![Updates](https://pyup.io/repos/github/cubenlp/openai_api_call/shield.svg)](https://pyup.io/repos/github/cubenlp/openai_api_call/) 
         -->
         
         A simple wrapper for OpenAI API, which can be used to send requests and get responses.
         
         ## Installation
         
         ```bash
@@ -72,14 +72,16 @@
         ```py
         from openai_api_call import request
         
         # set request url
         request.base_url = "https://api.example.com"
         ```
         
+        You can set `OPENAI_BASE_URL` in `~/.bashrc` as well.
+        
         ### Basic Usage
         
         Example 1, send prompt and return response:
         
         ```python
         from openai_api_call import Chat, show_apikey
```

### Comparing `openai_api_call-0.3.9/README.md` & `openai_api_call-0.4.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 > **中文文档移步[这里](README_zh_CN.md)。**
 
 # Openai API call
 [![PyPI version](https://img.shields.io/pypi/v/openai_api_call.svg)](https://pypi.python.org/pypi/openai_api_call)
-[![Tests](https://github.com/RexWzh/openai_api_call/actions/workflows/test.yml/badge.svg)](https://github.com/RexWzh/openai_api_call/actions/workflows/test.yml/)
+[![Tests](https://github.com/cubenlp/openai_api_call/actions/workflows/test.yml/badge.svg)](https://github.com/cubenlp/openai_api_call/actions/workflows/test.yml/)
 [![Documentation Status](https://img.shields.io/badge/docs-github_pages-blue.svg)](https://apicall.wzhecnu.cn)
-[![Coverage](https://codecov.io/gh/RexWzh/openai_api_call/branch/master/graph/badge.svg)](https://codecov.io/gh/RexWzh/openai_api_call.jl)
+[![Coverage](https://codecov.io/gh/cubenlp/openai_api_call/branch/master/graph/badge.svg)](https://codecov.io/gh/cubenlp/openai_api_call.jl)
 
 <!-- 
-[![Updates](https://pyup.io/repos/github/RexWzh/openai_api_call/shield.svg)](https://pyup.io/repos/github/RexWzh/openai_api_call/) 
+[![Updates](https://pyup.io/repos/github/cubenlp/openai_api_call/shield.svg)](https://pyup.io/repos/github/cubenlp/openai_api_call/) 
 -->
 
 A simple wrapper for OpenAI API, which can be used to send requests and get responses.
 
 ## Installation
 
 ```bash
@@ -64,14 +64,16 @@
 ```py
 from openai_api_call import request
 
 # set request url
 request.base_url = "https://api.example.com"
 ```
 
+You can set `OPENAI_BASE_URL` in `~/.bashrc` as well.
+
 ### Basic Usage
 
 Example 1, send prompt and return response:
 
 ```python
 from openai_api_call import Chat, show_apikey
```

### Comparing `openai_api_call-0.3.9/openai_api_call/__init__.py` & `openai_api_call-0.4.0/openai_api_call/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """Top-level package for Openai API call."""
 
 __author__ = """Rex Wang"""
 __email__ = '1073853456@qq.com'
-__version__ = '0.3.9'
+__version__ = '0.4.0'
 
 import os
 from .chattool import Chat, Resp, chat_completion, usage_status
 from .proxy import proxy_on, proxy_off, proxy_status
 
 # read API key from the environment variable
 if os.environ.get('OPENAI_API_KEY') is not None:
     api_key = os.environ.get('OPENAI_API_KEY')
-    if not api_key.startswith("sk-"):
-        print("Warning: The default environment variable `OPENAI_API_KEY` is not a valid API key.")
+    # skip checking the validity of the API key
+    # if not api_key.startswith("sk-"):
+    #     print("Warning: The default environment variable `OPENAI_API_KEY` is not a valid API key.")
 else:
     api_key = None
 
 def show_apikey():
     if api_key is not None:
         print(f"API key:\t{api_key}")
     else:
```

### Comparing `openai_api_call-0.3.9/openai_api_call/chattool.py` & `openai_api_call-0.4.0/openai_api_call/chattool.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,20 +12,20 @@
 def handler(signum, frame):
     raise Exception("API call timed out!")
 
 class Chat():
     def __init__( self
                 , msg:Union[List[Dict], None, str]=None
                 , api_key:Union[None, str]=None) -> None:
-        """Chat object
-        
+        """Initialize the chat log
+
         Args:
             msg (Union[List[Dict], None, str], optional): chat log. Defaults to None.
             api_key (Union[None, str], optional): API key. Defaults to None.
-
+        
         Raises:
             ValueError: msg should be a list of dict, a string or None
         """
         if msg is None:
             self._chat_log = []
         elif isinstance(msg, str):
             if openai_api_call.default_prompt is None:
@@ -140,18 +140,21 @@
             thismonth (bool): 
             recent (int, optional): number of the usage of recent days. Defaults to 10.
             duration (int, optional): duration of the usage. Defaults to 99.
         """
         if thismonth:
             duration = datetime.datetime.now().day - 1
         storage, usage, rem, recent_usage = self.get_usage_status(recent=recent, duration=duration)
-        print(f"Total account: {storage:.4f}$")
-        print(f"Total usage(the last {len(recent_usage)} days): {usage:.4f}$")
+        print(f"Amount: {storage:.4f}$")
         if thismonth:
-            print(f"Total remaining(this month): {rem:.4f}$")
+            print(f"Usage(this month): {usage:.4f}$")
+            print(f"Remaining(this month): {rem:.4f}$")
+        if len(recent_usage) > 0:
+            usage = sum(recent_usage.values())
+            print(f"Usage(the last {len(recent_usage)} days): {usage:.4f}$")
         for date, cost in recent_usage.items():
             print(f"{date}: {cost:.4f}$")
 
     def add(self, role:str, msg:str):
         """Add a message to the chat log"""
         assert role in ['user', 'assistant', 'system'], "role should be 'user', 'assistant' or 'system'"
         self._chat_log.append({"role": role, "content": msg})
```

### Comparing `openai_api_call-0.3.9/openai_api_call/proxy.py` & `openai_api_call-0.4.0/openai_api_call/proxy.py`

 * *Files identical despite different names*

### Comparing `openai_api_call-0.3.9/openai_api_call/request.py` & `openai_api_call-0.4.0/openai_api_call/request.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,56 @@
 # rewrite the request function
 
 from typing import List, Dict
 import requests, json
 import datetime, os, warnings
+from urllib.parse import urlparse, urlunparse
+
+url = None # Deprecated
+
+# Read base_url from the environment
+if os.environ.get('OPENAI_BASE_URL') is not None:
+    base_url = os.environ.get("OPENAI_BASE_URL")
+else:
+    base_url = "https://api.openai.com"
+
+def is_valid_url(url: str) -> bool:
+    """Check if the given URL is valid.
+
+    Args:
+        url (str): The URL to be checked.
+
+    Returns:
+        bool: True if the URL is valid; otherwise False.
+    """
+    parsed_url = urlparse(url)
+    return all([parsed_url.scheme, parsed_url.netloc])
+
+def normalize_url(url: str) -> str:
+    """Normalize the given URL to a canonical form.
+
+    Args:
+        url (str): The URL to be normalized.
+
+    Returns:
+        str: The normalized URL.
+
+    Examples:
+        >>> normalize_url("http://api.example.com")
+        'http://api.example.com'
+
+        >>> normalize_url("api.example.com")
+        'https://api.example.com'
+    """
+    parsed_url = urlparse(url)
+    if not parsed_url.scheme:
+        # If no scheme is specified, default to https protocol.
+        parsed_url = parsed_url._replace(scheme="https")
+    return urlunparse(parsed_url).replace("///", "//")
 
-base_url = "https://api.openai.com"
-url = None
 
 def chat_completion(api_key:str, messages:List[Dict], model:str, **options) -> Dict:
     """Chat completion API call
     
     Args:
         apikey (str): API key
         messages (List[Dict]): prompt message
@@ -34,14 +75,15 @@
     # initialize chat url
     if url is not None: # deprecated warning
         warnings.warn("The `url` parameter is deprecated. Please use `base_url` instead.", DeprecationWarning)
         chat_url = url
     else:
         chat_url = os.path.join(base_url, "v1/chat/completions")
     
+    chat_url = normalize_url(chat_url)
     # get response
     response = requests.post(chat_url, headers=headers, data=json.dumps(payload))
     if response.status_code != 200:
         raise Exception(response.text)
     return response.json()
 
 def usage_status(api_key:str, duration:int=99):
@@ -54,28 +96,29 @@
     Returns:
         Tuple[float, float, List[float]]: total storage, total usage, daily costs
     """
     headers = {
         "Authorization": "Bearer " + api_key,
         "Content-Type": "application/json"
     }
+    url = normalize_url(base_url)
     # Get storage limit
-    subscription_url = os.path.join(base_url, "v1/dashboard/billing/subscription")
+    subscription_url = os.path.join(url, "v1/dashboard/billing/subscription")
     subscription_response = requests.get(subscription_url, headers=headers)
     if subscription_response.status_code == 200:
         data = subscription_response.json()
         total_storage = data.get("hard_limit_usd")
     else:
         raise Exception(subscription_response.text)
     # start_date
     today = datetime.datetime.now()
     start_date = (today - datetime.timedelta(days=duration)).strftime("%Y-%m-%d")
     # end_date = today + 1
     end_date = (today + datetime.timedelta(days=1)).strftime("%Y-%m-%d")
-    billing_url = os.path.join(base_url, f"v1/dashboard/billing/usage?start_date={start_date}&end_date={end_date}")
+    billing_url = os.path.join(url, f"v1/dashboard/billing/usage?start_date={start_date}&end_date={end_date}")
     billing_response = requests.get(billing_url, headers=headers)
     # Get usage status
     if billing_response.status_code == 200:
         data = billing_response.json()
         total_usage = data.get("total_usage") / 100
         daily_costs = data.get("daily_costs")
         return total_storage, total_usage, daily_costs
```

### Comparing `openai_api_call-0.3.9/openai_api_call/response.py` & `openai_api_call-0.4.0/openai_api_call/response.py`

 * *Files identical despite different names*

### Comparing `openai_api_call-0.3.9/openai_api_call.egg-info/PKG-INFO` & `openai_api_call-0.4.0/openai_api_call.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: openai-api-call
-Version: 0.3.9
+Version: 0.4.0
 Summary: A short wrapper of the OpenAI api call.
-Home-page: https://github.com/RexWzh/openai_api_call
+Home-page: https://github.com/cubenlp/openai_api_call
 Author: Rex Wang
 Author-email: 1073853456@qq.com
 License: MIT license
 Description: > **中文文档移步[这里](README_zh_CN.md)。**
         
         # Openai API call
         [![PyPI version](https://img.shields.io/pypi/v/openai_api_call.svg)](https://pypi.python.org/pypi/openai_api_call)
-        [![Tests](https://github.com/RexWzh/openai_api_call/actions/workflows/test.yml/badge.svg)](https://github.com/RexWzh/openai_api_call/actions/workflows/test.yml/)
+        [![Tests](https://github.com/cubenlp/openai_api_call/actions/workflows/test.yml/badge.svg)](https://github.com/cubenlp/openai_api_call/actions/workflows/test.yml/)
         [![Documentation Status](https://img.shields.io/badge/docs-github_pages-blue.svg)](https://apicall.wzhecnu.cn)
-        [![Coverage](https://codecov.io/gh/RexWzh/openai_api_call/branch/master/graph/badge.svg)](https://codecov.io/gh/RexWzh/openai_api_call.jl)
+        [![Coverage](https://codecov.io/gh/cubenlp/openai_api_call/branch/master/graph/badge.svg)](https://codecov.io/gh/cubenlp/openai_api_call.jl)
         
         <!-- 
-        [![Updates](https://pyup.io/repos/github/RexWzh/openai_api_call/shield.svg)](https://pyup.io/repos/github/RexWzh/openai_api_call/) 
+        [![Updates](https://pyup.io/repos/github/cubenlp/openai_api_call/shield.svg)](https://pyup.io/repos/github/cubenlp/openai_api_call/) 
         -->
         
         A simple wrapper for OpenAI API, which can be used to send requests and get responses.
         
         ## Installation
         
         ```bash
@@ -72,14 +72,16 @@
         ```py
         from openai_api_call import request
         
         # set request url
         request.base_url = "https://api.example.com"
         ```
         
+        You can set `OPENAI_BASE_URL` in `~/.bashrc` as well.
+        
         ### Basic Usage
         
         Example 1, send prompt and return response:
         
         ```python
         from openai_api_call import Chat, show_apikey
```

### Comparing `openai_api_call-0.3.9/setup.py` & `openai_api_call-0.4.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """The setup script."""
 
 from setuptools import setup, find_packages
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
-VERSION = '0.3.9'
+VERSION = '0.4.0'
 
 requirements = ['Click>=7.0', 'requests>=2.20']
 
 test_requirements = ['pytest>=3', 'unittest']
 
 setup(
     author="Rex Wang",
@@ -38,11 +38,11 @@
     long_description_content_type='text/markdown',
     include_package_data=True,
     keywords='openai_api_call',
     name='openai_api_call',
     packages=find_packages(include=['openai_api_call', 'openai_api_call.*']),
     test_suite='tests',
     tests_require=test_requirements,
-    url='https://github.com/RexWzh/openai_api_call',
+    url='https://github.com/cubenlp/openai_api_call',
     version=VERSION,
     zip_safe=False,
 )
```

