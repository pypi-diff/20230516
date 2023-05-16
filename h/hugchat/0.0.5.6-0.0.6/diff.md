# Comparing `tmp/hugchat-0.0.5.6.tar.gz` & `tmp/hugchat-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hugchat-0.0.5.6.tar", last modified: Mon May  8 09:40:36 2023, max compression
+gzip compressed data, was "hugchat-0.0.6.tar", last modified: Tue May 16 00:55:46 2023, max compression
```

## Comparing `hugchat-0.0.5.6.tar` & `hugchat-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-08 09:40:36.088144 hugchat-0.0.5.6/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    34523 2023-05-01 00:33:11.000000 hugchat-0.0.5.6/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3217 2023-05-08 09:40:36.088144 hugchat-0.0.5.6/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2197 2023-05-08 09:39:22.000000 hugchat-0.0.5.6/README.md
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-05-08 09:40:36.088144 hugchat-0.0.5.6/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1436 2023-05-08 09:40:13.000000 hugchat-0.0.5.6/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-08 09:40:36.080144 hugchat-0.0.5.6/src/
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-08 09:40:36.084144 hugchat-0.0.5.6/src/hugchat/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-03 15:54:22.000000 hugchat-0.0.5.6/src/hugchat/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      179 2023-05-03 15:54:22.000000 hugchat-0.0.5.6/src/hugchat/cli.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9752 2023-05-08 09:39:29.000000 hugchat-0.0.5.6/src/hugchat/hugchat.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-08 09:40:36.088144 hugchat-0.0.5.6/src/hugchat.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3217 2023-05-08 09:40:35.000000 hugchat-0.0.5.6/src/hugchat.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      266 2023-05-08 09:40:35.000000 hugchat-0.0.5.6/src/hugchat.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-05-08 09:40:35.000000 hugchat-0.0.5.6/src/hugchat.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       27 2023-05-08 09:40:35.000000 hugchat-0.0.5.6/src/hugchat.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        8 2023-05-08 09:40:35.000000 hugchat-0.0.5.6/src/hugchat.egg-info/top_level.txt
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-16 00:55:46.116840 hugchat-0.0.6/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    34523 2023-05-01 00:33:11.000000 hugchat-0.0.6/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3827 2023-05-16 00:55:46.116840 hugchat-0.0.6/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2809 2023-05-16 00:53:53.000000 hugchat-0.0.6/README.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-05-16 00:55:46.116840 hugchat-0.0.6/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1434 2023-05-16 00:55:39.000000 hugchat-0.0.6/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-16 00:55:46.108840 hugchat-0.0.6/src/
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-16 00:55:46.116840 hugchat-0.0.6/src/hugchat/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-03 15:54:22.000000 hugchat-0.0.6/src/hugchat/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      179 2023-05-03 15:54:22.000000 hugchat-0.0.6/src/hugchat/cli.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10664 2023-05-16 00:53:53.000000 hugchat-0.0.6/src/hugchat/hugchat.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-16 00:55:46.116840 hugchat-0.0.6/src/hugchat.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3827 2023-05-16 00:55:45.000000 hugchat-0.0.6/src/hugchat.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      266 2023-05-16 00:55:45.000000 hugchat-0.0.6/src/hugchat.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-05-16 00:55:45.000000 hugchat-0.0.6/src/hugchat.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       27 2023-05-16 00:55:45.000000 hugchat-0.0.6/src/hugchat.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        8 2023-05-16 00:55:45.000000 hugchat-0.0.6/src/hugchat.egg-info/top_level.txt
```

### Comparing `hugchat-0.0.5.6/LICENSE` & `hugchat-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hugchat-0.0.5.6/PKG-INFO` & `hugchat-0.0.6/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hugchat
-Version: 0.0.5.6
+Version: 0.0.6
 Summary: A huggingchat python api.
 Home-page: https://github.com/Soulter/hugging-chat-api
 Author: Soulter
 Author-email: 905617992@qq.com
 License: GNU Affero General Public License v3.0
 Project-URL: Bug Report, https://github.com/Soulter/hugging-chat-api/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -30,29 +30,45 @@
 
 [![PyPi](https://img.shields.io/pypi/v/hugchat.svg)](https://pypi.python.org/pypi/hugchat)
 [![Support_Platform](https://img.shields.io/pypi/pyversions/hugchat)](https://pypi.python.org/pypi/hugchat)
 [![Downloads](https://static.pepy.tech/badge/hugchat)](https://pypi.python.org/pypi/hugchat)
 
 Leave a star :)
 
-> When you use this project, it means that you have agreed to the following two requirements of the HuggingChat: 
-> 1. AI is an area of active research with known problems such as biased generation and misinformation. Do not use this application for high-stakes decisions or advice.
+> When you use this project, it means that you have agreed to the following two requirements of the HuggingChat:  
+>
+> 1. AI is an area of active research with known problems such as biased generation and misinformation. Do not use this application for high-stakes decisions or advice.  
 > 2. Your conversations will be shared with model authors.
 
-## How to Use
+## Authentication (Required Now)
+
+### Cookies
+
+<details>
+<summary>How to Get Cookies ?</summary>
+
+- Install the `Cookie-Editor` extension for [Chrome](https://chrome.google.com/webstore/detail/cookie-editor/hlkenndednhfkekhgcdicdfddnkalmdm) or [Firefox](https://addons.mozilla.org/en-US/firefox/addon/cookie-editor/)
+- Go to [HuggingChat](https://huggingface.co/chat) and **login**
+- Open the extension
+- Click `Export` on the bottom right, then `Export as JSON`(This saves your cookies to the clipboard)
+- Paste your cookies into a file `cookies.json`
+
+</details>
+
+## Usage
 
 ### Basic mode
 
 ```bash
 pip install hugchat
 ```
 
 ```py
 from hugchat import hugchat
-chatbot = hugchat.ChatBot()
+chatbot = hugchat.ChatBot(cookie_path="cookies.json")  # or cookies=[...]
 print(chatbot.chat("HI"))
 
 # Create a new conversation
 id = chatbot.new_conversation()
 chatbot.change_conversation(id)
 
 # Get conversation list
```

### Comparing `hugchat-0.0.5.6/README.md` & `hugchat-0.0.6/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -6,29 +6,45 @@
 
 [![PyPi](https://img.shields.io/pypi/v/hugchat.svg)](https://pypi.python.org/pypi/hugchat)
 [![Support_Platform](https://img.shields.io/pypi/pyversions/hugchat)](https://pypi.python.org/pypi/hugchat)
 [![Downloads](https://static.pepy.tech/badge/hugchat)](https://pypi.python.org/pypi/hugchat)
 
 Leave a star :)
 
-> When you use this project, it means that you have agreed to the following two requirements of the HuggingChat: 
-> 1. AI is an area of active research with known problems such as biased generation and misinformation. Do not use this application for high-stakes decisions or advice.
+> When you use this project, it means that you have agreed to the following two requirements of the HuggingChat:  
+>
+> 1. AI is an area of active research with known problems such as biased generation and misinformation. Do not use this application for high-stakes decisions or advice.  
 > 2. Your conversations will be shared with model authors.
 
-## How to Use
+## Authentication (Required Now)
+
+### Cookies
+
+<details>
+<summary>How to Get Cookies ?</summary>
+
+- Install the `Cookie-Editor` extension for [Chrome](https://chrome.google.com/webstore/detail/cookie-editor/hlkenndednhfkekhgcdicdfddnkalmdm) or [Firefox](https://addons.mozilla.org/en-US/firefox/addon/cookie-editor/)
+- Go to [HuggingChat](https://huggingface.co/chat) and **login**
+- Open the extension
+- Click `Export` on the bottom right, then `Export as JSON`(This saves your cookies to the clipboard)
+- Paste your cookies into a file `cookies.json`
+
+</details>
+
+## Usage
 
 ### Basic mode
 
 ```bash
 pip install hugchat
 ```
 
 ```py
 from hugchat import hugchat
-chatbot = hugchat.ChatBot()
+chatbot = hugchat.ChatBot(cookie_path="cookies.json")  # or cookies=[...]
 print(chatbot.chat("HI"))
 
 # Create a new conversation
 id = chatbot.new_conversation()
 chatbot.change_conversation(id)
 
 # Get conversation list
```

### Comparing `hugchat-0.0.5.6/setup.py` & `hugchat-0.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_namespace_packages
 from setuptools import setup
 
 setup(
     name="hugchat",
-    version="0.0.5.6",
+    version="0.0.6",
     description="A huggingchat python api.",
     long_description=open("README.md", "rt", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Soulter/hugging-chat-api",
     project_urls={
         "Bug Report": "https://github.com/Soulter/hugging-chat-api/issues"
     },
```

### Comparing `hugchat-0.0.5.6/src/hugchat/hugchat.py` & `hugchat-0.0.6/src/hugchat/hugchat.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,52 @@
 from requests import Session
 import json
 import uuid
 
 class ChatBot:
-    def __init__(self) -> None:
+    
+    cookies: dict
+    """Cookies for authentication"""
+
+    session: Session
+    """HuggingChat session"""
+
+    def __init__(
+        self,
+        cookies: dict = None,
+        cookie_path: str = ""
+    ) -> None:
+        if cookies is None and cookie_path == "":
+            raise Exception("Authentication is required now, but no cookies provided")
+        elif cookies is not None and cookie_path != "":
+            raise Exception("Both cookies and cookie_path provided")
+        
+        if cookies is None and cookie_path != "":
+            # read cookies from path
+            with open(cookie_path, "r") as f:
+                cookies = json.load(f)
+
+        # convert cookies to KV format
+        if isinstance(cookies, list):
+            cookies = {cookie["name"]: cookie["value"] for cookie in cookies}
+
+        self.cookies = cookies
+
         self.hf_base_url = "https://huggingface.co"
         self.json_header = {"Content-Type": "application/json"}
         self.session = self.get_hc_session()
         self.conversation_id_list = []
         self.active_model = "OpenAssistant/oasst-sft-6-llama-30b-xor"
         self.accepted_welcome_modal = False # Only when accepted, it can create a new conversation.
         self.current_conversation = self.new_conversation()
 
-
     def get_hc_session(self) -> Session:
         session = Session()
+        # set cookies
+        session.cookies.update(self.cookies)
         session.get(self.hf_base_url + "/chat")
         return session
     
     def get_headers(self, ref=True) -> dict:
         _h = {
             "Accept": "*/*",
             "Connection": "keep-alive",
@@ -194,15 +222,15 @@
                     elif "error" in obj:
                         raise Exception(obj["error"])
             return res_text
 
 def cli():
     print("-------HuggingChat-------")
     print("1. AI is an area of active research with known problems such as biased generation and misinformation. Do not use this application for high-stakes decisions or advice.\n2. Your conversations will be shared with model authors.\nContinuing to use means that you accept the above points")
-    chatbot = ChatBot()
+    chatbot = ChatBot(cookie_path="cookies.json")
     running = True
     while running:
         question = input("> ")
         if question == "/new":
             cid = chatbot.new_conversation()
             print("The new conversation ID is: " + cid)
             chatbot.change_conversation(cid)
```

### Comparing `hugchat-0.0.5.6/src/hugchat.egg-info/PKG-INFO` & `hugchat-0.0.6/src/hugchat.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hugchat
-Version: 0.0.5.6
+Version: 0.0.6
 Summary: A huggingchat python api.
 Home-page: https://github.com/Soulter/hugging-chat-api
 Author: Soulter
 Author-email: 905617992@qq.com
 License: GNU Affero General Public License v3.0
 Project-URL: Bug Report, https://github.com/Soulter/hugging-chat-api/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -30,29 +30,45 @@
 
 [![PyPi](https://img.shields.io/pypi/v/hugchat.svg)](https://pypi.python.org/pypi/hugchat)
 [![Support_Platform](https://img.shields.io/pypi/pyversions/hugchat)](https://pypi.python.org/pypi/hugchat)
 [![Downloads](https://static.pepy.tech/badge/hugchat)](https://pypi.python.org/pypi/hugchat)
 
 Leave a star :)
 
-> When you use this project, it means that you have agreed to the following two requirements of the HuggingChat: 
-> 1. AI is an area of active research with known problems such as biased generation and misinformation. Do not use this application for high-stakes decisions or advice.
+> When you use this project, it means that you have agreed to the following two requirements of the HuggingChat:  
+>
+> 1. AI is an area of active research with known problems such as biased generation and misinformation. Do not use this application for high-stakes decisions or advice.  
 > 2. Your conversations will be shared with model authors.
 
-## How to Use
+## Authentication (Required Now)
+
+### Cookies
+
+<details>
+<summary>How to Get Cookies ?</summary>
+
+- Install the `Cookie-Editor` extension for [Chrome](https://chrome.google.com/webstore/detail/cookie-editor/hlkenndednhfkekhgcdicdfddnkalmdm) or [Firefox](https://addons.mozilla.org/en-US/firefox/addon/cookie-editor/)
+- Go to [HuggingChat](https://huggingface.co/chat) and **login**
+- Open the extension
+- Click `Export` on the bottom right, then `Export as JSON`(This saves your cookies to the clipboard)
+- Paste your cookies into a file `cookies.json`
+
+</details>
+
+## Usage
 
 ### Basic mode
 
 ```bash
 pip install hugchat
 ```
 
 ```py
 from hugchat import hugchat
-chatbot = hugchat.ChatBot()
+chatbot = hugchat.ChatBot(cookie_path="cookies.json")  # or cookies=[...]
 print(chatbot.chat("HI"))
 
 # Create a new conversation
 id = chatbot.new_conversation()
 chatbot.change_conversation(id)
 
 # Get conversation list
```

