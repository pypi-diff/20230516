# Comparing `tmp/characterai-0.3.2.tar.gz` & `tmp/characterai-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\characterai-0.3.2.tar", last modified: Mon May  1 15:48:13 2023, max compression
+gzip compressed data, was "dist\characterai-0.4.0.tar", last modified: Tue May 16 20:10:00 2023, max compression
```

## Comparing `characterai-0.3.2.tar` & `characterai-0.4.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 15:48:13.764425 characterai-0.3.2/
--rw-rw-rw-   0        0        0     1082 2023-04-28 16:51:34.000000 characterai-0.3.2/LICENSE
--rw-rw-rw-   0        0        0     1873 2023-05-01 15:48:13.762424 characterai-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     1481 2023-05-01 15:25:41.000000 characterai-0.3.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 15:48:13.705547 characterai-0.3.2/characterai/
--rw-rw-rw-   0        0        0       90 2023-04-29 10:41:38.000000 characterai-0.3.2/characterai/__init__.py
--rw-rw-rw-   0        0        0     5640 2023-05-01 09:39:20.000000 characterai-0.3.2/characterai/characterai.py
--rw-rw-rw-   0        0        0      126 2023-04-28 20:05:16.000000 characterai-0.3.2/characterai/errors.py
--rw-rw-rw-   0        0        0     5070 2023-05-01 09:33:52.000000 characterai-0.3.2/characterai/pyasynccai.py
-drwxrwxrwx   0        0        0        0 2023-05-01 15:48:13.757423 characterai-0.3.2/characterai.egg-info/
--rw-rw-rw-   0        0        0     1873 2023-05-01 15:48:13.000000 characterai-0.3.2/characterai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-05-01 15:48:13.000000 characterai-0.3.2/characterai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 15:48:13.000000 characterai-0.3.2/characterai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-05-01 15:48:13.000000 characterai-0.3.2/characterai.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-01 15:48:13.000000 characterai-0.3.2/characterai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-01 15:48:13.764425 characterai-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0      622 2023-05-01 15:47:39.000000 characterai-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 20:10:00.426690 characterai-0.4.0/
+-rw-rw-rw-   0        0        0     1082 2023-04-28 16:51:34.000000 characterai-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0      358 2023-05-16 20:10:00.422687 characterai-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1481 2023-05-01 15:25:41.000000 characterai-0.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-16 20:10:00.292480 characterai-0.4.0/characterai/
+-rw-rw-rw-   0        0        0       90 2023-05-05 18:13:37.000000 characterai-0.4.0/characterai/__init__.py
+-rw-rw-rw-   0        0        0     6548 2023-05-16 20:04:21.000000 characterai-0.4.0/characterai/characterai.py
+-rw-rw-rw-   0        0        0      126 2023-05-16 17:53:10.000000 characterai-0.4.0/characterai/errors.py
+-rw-rw-rw-   0        0        0     6879 2023-05-16 20:02:20.000000 characterai-0.4.0/characterai/pyasynccai.py
+drwxrwxrwx   0        0        0        0 2023-05-16 20:10:00.418687 characterai-0.4.0/characterai.egg-info/
+-rw-rw-rw-   0        0        0      358 2023-05-16 20:09:59.000000 characterai-0.4.0/characterai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-05-16 20:09:59.000000 characterai-0.4.0/characterai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 20:09:59.000000 characterai-0.4.0/characterai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-05-16 20:09:59.000000 characterai-0.4.0/characterai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-16 20:09:59.000000 characterai-0.4.0/characterai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-16 20:10:00.427691 characterai-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0      448 2023-05-16 20:08:52.000000 characterai-0.4.0/setup.py
```

### Comparing `characterai-0.3.2/LICENSE` & `characterai-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `characterai-0.3.2/PKG-INFO` & `characterai-0.4.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: characterai
-Version: 0.3.2
-Summary: An unofficial API for character.ai for Python
-Home-page: https://github.com/kramcat/characterai
-Author: kramcat
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: MIT License
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # CharacterAI
 
 An unofficial API for Character AI for Python using Playwright
 
 ## Installation
 ```bash
 pip install characterai
@@ -75,9 +62,7 @@
 ## Features
 - The only library for character.ai
 - Asynchronous
 - So easy to use
 
 ## Disclaimer
 This library is written by a beginner in python, if you have any problems, write to me in [Telegram](https://t.me/kramcat)
-
-
```

### Comparing `characterai-0.3.2/characterai/characterai.py` & `characterai-0.4.0/characterai/characterai.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 from typing import Dict
 import json
-import time
 
 from playwright.sync_api import sync_playwright
 
 from characterai import errors
 from characterai.pyasynccai import pyAsyncCAI
 
 __all__ = ['pyCAI', 'pyAsyncCAI']
 
-text = []
 page = None
 
 def goto(link: str, *, wait: bool = False, token: str = None):
     if token != None:
         page.set_extra_http_headers({"Authorization": f"Token {token}"})
 
     page.goto(link)
@@ -29,29 +27,30 @@
             page.wait_for_selector('div#wrapper', state='detached', timeout=0)
             goto(link=link, wait=wait)
         else:
             raise errors.NoResponse('The Site is Overloaded')
 
 def GetResponse(link: str, *, wait: bool = False, token: str = None) -> Dict[str, str]:
     goto(f'https://beta.character.ai/{link}/', wait=wait, token=token)
-    data = json.loads(page.locator('pre').inner_text())
+    data = json.loads(page.locator('body').inner_text())
 
     return data
 
 
 class pyCAI:
     def __init__(self, token: str, *, headless: bool = True):
         global page
 
         self.token = token
         self.headless = headless
 
         self.browser = sync_playwright().start().firefox.launch(headless=headless)
         self.context = self.browser.new_context(
-            extra_http_headers={"Authorization": f"Token {self.token}"})
+            extra_http_headers={"Authorization": f"Token {self.token}"}
+        )
         page = self.context.new_page()
 
         self.user = self.user()
         self.character = self.character()
         self.chat = self.chat()
 
     class user:
@@ -69,76 +68,93 @@
 
         def followers(self, *, wait: bool = False, token: str = None) -> Dict[str, str]:
             return GetResponse(link='chat/user/followers', wait=wait, token=token)
 
         def following(self, *, wait: bool = False, token: str = None) -> Dict[str, str]:
             return GetResponse(link='chat/user/following', wait=wait, token=token)
 
+        def recent(self, *, wait: bool = False, token: str = None) -> Dict[str, str]:
+            return GetResponse('chat/characters/recent/', wait=wait, token=token)
+
     class character:
         """
         Just a Responses from site for characters
 
         character.trending()
-        character.get_info('CHAR')
+        character.info('CHAR')
+        character.search('SEARCH')
         """
-
         def trending(self, *, wait: bool = False, token: str = None) -> Dict[str, str]:
             return GetResponse(link='chat/characters/trending', wait=wait, token=token)
 
         def recommended(self, *, wait: bool = False, token: str = None) -> Dict[str, str]:
             return GetResponse(link='chat/characters/recommended', wait=wait, token=token)
 
         def categories(self, *, wait: bool = False, token: str = None) -> Dict[str, str]:
             return GetResponse(link='chat/character/categories', wait=wait, token=token)
 
-        def get_info(self, char: str, *, wait: bool = False, token: str = None) -> Dict[str, str]:
-            try:
-                return GetResponse(link=f'chat/character/info-cached/{char}', wait=wait, token=token)
-            except:
+        def info(self, char: str, *, wait: bool = False, token: str = None) -> Dict[str, str]:
+            data = GetResponse(f'chat/character/info-cached/{char}/', wait=wait, token=token)
+
+            if data != "{'error': 'Server Error (500)'}":
+                return data
+            else:
                 raise errors.CharNotFound('Wrong Char')
+        
+        def search(self, search, *, wait: bool = False, token: str = None) -> Dict[str, str]:
+            return GetResponse(f'chat/characters/search/?query={search}', wait=wait, token=token)
 
     class chat:
         def get_history(self, char: str, *, wait: bool = False, token: str = None) -> Dict[str, str]:
             """
-            Getting character chat history, return json Response
-
-            The post method doesn't work, so i get this from page.on('Response')
+            Getting character chat history, return json response
 
             chat.get_history('CHAR')
             """
-            page.on("response", lambda response: text.append(response.text()) if response.url.startswith(
-                'https://beta.character.ai/chat/history/msgs/user/') else None)
             goto(f'https://beta.character.ai/chat?char={char}', wait=wait, token=token)
-            page.wait_for_selector('.msg.char-msg').is_visible()
-
-            return json.loads(text[0])
+            
+            if page.query_selector('h1') == None:
+                with page.expect_response(lambda response: response.url.startswith('https://beta.character.ai/chat/history/msgs/user/')) as response_info:
+                    goto(f'https://beta.character.ai/chat?char={char}', wait=wait, token=token)
+
+                response = response_info.value.text()
+                return json.loads(response)
+            else:
+                raise errors.CharNotFound('Wrong Char')
 
         def send_message(self, char: str, message: str, *, wait: bool = False, token: str = None) -> Dict[str, str]:
             """
-            Sending a message
+            Sending a message, return json
 
             chat.send_message('CHAR', 'MESSAGE')
             """
             goto(f'https://beta.character.ai/chat?char={char}', wait=wait, token=token)
+            
+            # BIG THANKS - HearYourWaifu
+            page.evaluate("""
+            const { fetch: origFetch } = window;
+            window.fetch = async (...args) => {
+            const response = await origFetch(...args);
+            const raw_text = await new Response(response.clone().body).text();
+            return response;};""")
+            
+            with page.expect_response("https://beta.character.ai/chat/streaming/") as response_info:
+                page.get_by_placeholder("Type a message").fill(message)
+                page.get_by_role("button", name="Submit Message").click()
 
-            # time.sleep because the code is running too fast and there are problems with sending the message
-            time.sleep(1)
-            page.wait_for_selector("textarea", state="visible").fill(message)
-            time.sleep(1)
-            page.get_by_role("button", name="Submit Message").click()
-
-            page.wait_for_selector('.swiper-button-next',
-                                   timeout=0).is_visible()
-            div = page.query_selector(
-                'div.markdown-wrapper.markdown-wrapper-last-msg.swiper-no-swiping')
-
-            return div.inner_text()
+            response = response_info.value.text()
+            return json.loads('{"replies": ' + response.split(r'{"replies": ')[-1])
 
         def new_chat(self, char: str, *, wait: bool = False, token: str = None) -> None:
             """
-            Starting new chat
+            Starting new chat, return json
 
             chat.new_chat('CHAR')
             """
             goto(f'https://beta.character.ai/chat?char={char}', wait=wait, token=token)
-            page.wait_for_selector('.col-auto.px-2.dropdown').click()
-            page.locator('//html/body/div[1]/div[2]/div/div[1]/div[3]/div[1]/div[3]/div/div/div/div/div/button[2]').click()
+
+            with page.expect_response("https://beta.character.ai/chat/history/create/") as response_info:
+                page.wait_for_selector('.col-auto.px-2.dropdown').click()
+                page.wait_for_selector('"Save and Start New Chat"').click()
+
+            response = response_info.value.text()
+            return json.loads(response)
```

### Comparing `characterai-0.3.2/characterai/pyasynccai.py` & `characterai-0.4.0/characterai/pyasynccai.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 from typing import Dict
 import asyncio
 import json
-import time
 
 from playwright.async_api import async_playwright
 
 from characterai import errors
 
 __all__ = ['pyCAI', 'pyAsyncCAI']
 
-text = []
 page = None
 
 async def goto(link: str, *, wait: bool = False, token: str = None):
     if token != None:
         await page.set_extra_http_headers({"Authorization": f"Token {token}"})
 
     await page.goto(link)
@@ -28,16 +26,16 @@
         if wait:
             await page.wait_for_selector('div#wrapper', state='detached', timeout=0)
             await goto(link=link, wait=wait)
         else:
             raise errors.NoResponse('The Site is Overloaded')
 
 async def GetResponse(link: str, *, wait: bool = False, token: str = None) -> Dict[str, str]:
-    await goto(f'https://beta.character.ai/{link}/')
-    data = json.loads(await (page.locator('pre').inner_text()))
+    await goto(f'https://beta.character.ai/{link}/', wait=wait, token=token)
+    data = json.loads(await (page.locator('body').inner_text()))
 
     return data
 
 
 class pyAsyncCAI:
     def __init__(self, token: str):
         self.token = token
@@ -46,79 +44,116 @@
         self.character = self.character()
         self.chat = self.chat()
 
     async def start(self, *, headless: bool = True):
         global page
 
         self.browser = await (await async_playwright().start()).firefox.launch(headless=headless)
-        self.context = await self.browser.new_context(extra_http_headers={"Authorization": f"Token {self.token}"})
+        self.context = await self.browser.new_context(
+            extra_http_headers={"Authorization": f"Token {self.token}"}
+        )
         page = await self.context.new_page()
 
     class user:
         """
         Just a Responses from site for user info
 
         user.info()
         """
         async def info(self, *, wait: bool = False, token: str = None) -> Dict[str, str]:
-            return await GetResponse(link='chat/user', wait=wait, token=token)
+            return await GetResponse('chat/user', wait=wait, token=token)
 
         async def posts(self, *, wait: bool = False, token: str = None) -> Dict[str, str]:
-            return await GetResponse(link='chat/posts/user/?scope=user&page=1&posts_to_load=5', wait=wait, token=token)
+            return await GetResponse('chat/posts/user/?scope=user&page=1&posts_to_load=5', wait=wait, token=token)
 
         async def followers(self, *, wait: bool = False, token: str = None) -> Dict[str, str]:
-            return await GetResponse(link='chat/user/followers', wait=wait, token=token)
+            return await GetResponse('chat/user/followers', wait=wait, token=token)
 
         async def following(self, *, wait: bool = False, token: str = None) -> Dict[str, str]:
-            return await GetResponse(link='chat/user/following', wait=wait, token=token)
+            return await GetResponse('chat/user/following', wait=wait, token=token)
+        
+        async def recent(self, *, wait: bool = False, token: str = None) -> Dict[str, str]:
+            return await GetResponse('chat/characters/recent', wait=wait, token=token)
 
     class character:
         """
         Just a Responses from site for characters
 
         character.trending()
-        character.get_info('CHAR')
+        character.info('CHAR')
+        character.search('SEARCH')
         """
         async def trending(self, *, wait: bool = False, token: str = None) -> Dict[str, str]:
-            return await GetResponse(link='chat/characters/trending', wait=wait, token=token)
+            return await GetResponse('chat/characters/trending', wait=wait, token=token)
 
         async def recommended(self, *, wait: bool = False, token: str = None) -> Dict[str, str]:
-            return await GetResponse(link='chat/characters/recommended', wait=wait, token=token)
+            return await GetResponse('chat/characters/recommended', wait=wait, token=token)
 
         async def categories(self, *, wait: bool = False, token: str = None) -> Dict[str, str]:
-            return await GetResponse(link='chat/character/categories', wait=wait, token=token)
+            return await GetResponse('chat/character/categories', wait=wait, token=token)
 
-        async def get_info(self, char: str, *, wait: bool = False, token: str = None) -> Dict[str, str]:
-            try:
-                return GetResponse(link=f'chat/character/info-cached/{char}', wait=wait, token=token)
-            except:
-                raise errors.CharNotFound('Wrong Char')
+        async def info(self, char: str, *, wait: bool = False, token: str = None) -> Dict[str, str]:
+            data = await GetResponse(f'chat/character/info-cached/{char}/', wait=wait, token=token)
 
+            if data != "{'error': 'Server Error (500)'}":
+                return data
+            else:
+                raise errors.CharNotFound('Wrong Char')
+        
+        async def search(self, search, *, wait: bool = False, token: str = None) -> Dict[str, str]:
+            return await GetResponse(f'chat/characters/search/?query={search}', wait=wait, token=token)
+            
     class chat:
-        async def send_message(self, char: str, message: str, *, wait: bool = False, token: str = None) -> bool:
+        async def get_history(self, char: str, *, wait: bool = False, token: str = None) -> Dict[str, str]:
             """
-            Sending a message
+            Getting character chat history, return json response
 
-            chat.send_message('CHAR', 'MESSAGE')
+            chat.get_history('CHAR')
             """
             await goto(f'https://beta.character.ai/chat?char={char}', wait=wait, token=token)
+            
+            if await page.query_selector('h1') == None:
+                async with page.expect_response(lambda response: response.url.startswith('https://beta.character.ai/chat/history/msgs/user/')) as response_info:
+                    await goto(f'https://beta.character.ai/chat?char={char}', wait=wait, token=token)
+
+                response = await (await response_info.value).text()
+                return json.loads(response)
+            else:
+                raise errors.CharNotFound('Wrong Char')
 
-            # time.sleep because the code is running too fast and there are problems with sending the message
-            time.sleep(1)
-            await page.get_by_placeholder("Type a message").fill(message)
-            time.sleep(1)
-            await page.get_by_role("button", name="Submit Message").click()
+        async def send_message(self, char: str, message: str, *, wait: bool = False, token: str = None) -> Dict[str, str]:
+            """
+            Sending a message, return json
 
-            await (await page.wait_for_selector('.swiper-button-next', timeout=0)).is_visible()
-            div = await page.query_selector('div.markdown-wrapper.markdown-wrapper-last-msg.swiper-no-swiping')
+            chat.send_message('CHAR', 'MESSAGE')
+            """
+            await goto(f'https://beta.character.ai/chat?char={char}', wait=wait, token=token)
+            
+            # BIG THANKS - HearYourWaifu
+            await page.evaluate("""
+            const { fetch: origFetch } = window;
+            window.fetch = async (...args) => {
+            const response = await origFetch(...args);
+            const raw_text = await new Response(response.clone().body).text();
+            return response;};""")
+            
+            async with page.expect_response("https://beta.character.ai/chat/streaming/") as response_info:
+                await page.get_by_placeholder("Type a message").fill(message)
+                await page.get_by_role("button", name="Submit Message").click()
 
-            return (await div.inner_text())
+            response = await (await response_info.value).text()
+            return json.loads('{"replies": ' + response.split(r'{"replies": ')[-1])
 
-        async def new_chat(self, char: str, *, wait: bool = False, token: str = None) -> None:
+        async def new_chat(self, char: str, *, wait: bool = False, token: str = None) -> Dict[str, str]:
             """
-            Starting new chat, return True when done
+            Starting new chat, return json
 
             chat.new_chat('CHAR')
             """
             await goto(f'https://beta.character.ai/chat?char={char}', wait=wait, token=token)
-            await (await page.wait_for_selector('.col-auto.px-2.dropdown')).click()
-            await page.locator('//html/body/div[1]/div[2]/div/div[1]/div[3]/div[1]/div[3]/div/div/div/div/div/button[2]').click()
+
+            async with page.expect_response("https://beta.character.ai/chat/history/create/") as response_info:
+                await (await page.wait_for_selector('.col-auto.px-2.dropdown')).click()
+                await (await page.wait_for_selector('"Save and Start New Chat"')).click()
+
+            response = await (await response_info.value).text()
+            return json.loads(response)
```

