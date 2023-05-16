# Comparing `tmp/EdgeGPT-0.3.9.tar.gz` & `tmp/EdgeGPT-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EdgeGPT-0.3.9.tar", last modified: Mon May 15 02:33:30 2023, max compression
+gzip compressed data, was "EdgeGPT-0.4.0.tar", last modified: Tue May 16 03:14:15 2023, max compression
```

## Comparing `EdgeGPT-0.3.9.tar` & `EdgeGPT-0.4.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 02:33:30.879199 EdgeGPT-0.3.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-15 02:32:54.000000 EdgeGPT-0.3.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-05-15 02:33:30.879199 EdgeGPT-0.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7493 2023-05-15 02:33:30.000000 EdgeGPT-0.3.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-15 02:33:30.879199 EdgeGPT-0.3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-15 02:32:54.000000 EdgeGPT-0.3.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 02:33:30.879199 EdgeGPT-0.3.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 02:33:30.879199 EdgeGPT-0.3.9/src/EdgeGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-05-15 02:33:30.000000 EdgeGPT-0.3.9/src/EdgeGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-15 02:33:30.000000 EdgeGPT-0.3.9/src/EdgeGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 02:33:30.000000 EdgeGPT-0.3.9/src/EdgeGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-15 02:33:30.000000 EdgeGPT-0.3.9/src/EdgeGPT.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-15 02:33:30.000000 EdgeGPT-0.3.9/src/EdgeGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-15 02:33:30.000000 EdgeGPT-0.3.9/src/EdgeGPT.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    29897 2023-05-15 02:32:54.000000 EdgeGPT-0.3.9/src/EdgeGPT.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-15 02:32:54.000000 EdgeGPT-0.3.9/src/ImageGen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:14:15.728615 EdgeGPT-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-16 03:13:47.000000 EdgeGPT-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-05-16 03:14:15.728615 EdgeGPT-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10581 2023-05-16 03:14:15.000000 EdgeGPT-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-16 03:14:15.728615 EdgeGPT-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-16 03:13:47.000000 EdgeGPT-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:14:15.728615 EdgeGPT-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:14:15.728615 EdgeGPT-0.4.0/src/EdgeGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-05-16 03:14:15.000000 EdgeGPT-0.4.0/src/EdgeGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-16 03:14:15.000000 EdgeGPT-0.4.0/src/EdgeGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 03:14:15.000000 EdgeGPT-0.4.0/src/EdgeGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-16 03:14:15.000000 EdgeGPT-0.4.0/src/EdgeGPT.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-16 03:14:15.000000 EdgeGPT-0.4.0/src/EdgeGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 03:14:15.000000 EdgeGPT-0.4.0/src/EdgeGPT.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    38159 2023-05-16 03:13:47.000000 EdgeGPT-0.4.0/src/EdgeGPT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-16 03:13:47.000000 EdgeGPT-0.4.0/src/ImageGen.py
```

### Comparing `EdgeGPT-0.3.9/LICENSE` & `EdgeGPT-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `EdgeGPT-0.3.9/PKG-INFO` & `EdgeGPT-0.4.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdgeGPT
-Version: 0.3.9
+Version: 0.4.0
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/acheong08/EdgeGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
@@ -33,75 +33,80 @@
 </div>
 
 <p align="center">
   <a href="https://github.com/acheong08/EdgeGPT">
     <img alt="PyPI version" src="https://img.shields.io/pypi/v/EdgeGPT">
   </a>
   <img alt="Python version" src="https://img.shields.io/badge/python-3.8+-blue.svg">
-
   <img alt="Total downloads" src="https://static.pepy.tech/badge/edgegpt">
 
 </p>
 
----
+<details>
 
-## Setup
+<summary>
+
+# Setup
+</summary>
 
 ### Install package
 
+
+
 ```bash
 python3 -m pip install EdgeGPT --upgrade
 ```
 
 ### Requirements
 
 - python 3.8+
 - A Microsoft Account with early access to <https://bing.com/chat> (Required)
 - Required in a supported country with New Bing (Chinese mainland VPN required)
+- [Selenium](https://pypi.org/project/selenium/) (for automatic cookie setup)
 
-<details>
-  <summary>
-
-### Checking access (Required)
-
-  </summary>
-
-- Install the latest version of Microsoft Edge
-- Alternatively, you can use any browser and set the user-agent to look like you're using Edge (e.g., `Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36 Edg/111.0.1661.51`). You can do this easily with an extension like "User-Agent Switcher and Manager" for [Chrome](https://chrome.google.com/webstore/detail/user-agent-switcher-and-m/bhchdcejhohfmigjafbampogmaanbfkg) and [Firefox](https://addons.mozilla.org/en-US/firefox/addon/user-agent-string-switcher/).
-- Open [bing.com/chat](https://bing.com/chat)
-- If you see a chat feature, you are good to go
-
-</details>
-
-<details>
-  <summary>
-
-### Getting authentication (Required)
-
-  </summary>
-
-- Install the cookie editor extension for [Chrome](https://chrome.google.com/webstore/detail/cookie-editor/hlkenndednhfkekhgcdicdfddnkalmdm) or [Firefox](https://addons.mozilla.org/en-US/firefox/addon/cookie-editor/)
-- Go to `bing.com`
-- Open the extension
-- Click "Export" on the bottom right, then "Export as JSON" (This saves your cookies to clipboard)
-- Paste your cookies into a file `cookies.json`
 
+### Authentication (Required)
+1. Install the latest version of Microsoft Edge
+2. Alternatively, you can use any browser and set the user-agent to look like you're using Edge (e.g., `Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36 Edg/111.0.1661.51`). You can do this easily with an extension like "User-Agent Switcher and Manager" for [Chrome](https://chrome.google.com/webstore/detail/user-agent-switcher-and-m/bhchdcejhohfmigjafbampogmaanbfkg) and [Firefox](https://addons.mozilla.org/en-US/firefox/addon/user-agent-string-switcher/).
+3. Open [bing.com/chat](https://bing.com/chat)
+4. If you see a chat feature, you are good to continue...
+5. Install the cookie editor extension for [Chrome](https://chrome.google.com/webstore/detail/cookie-editor/hlkenndednhfkekhgcdicdfddnkalmdm) or [Firefox](https://addons.mozilla.org/en-US/firefox/addon/cookie-editor/)
+6. Go to [bing.com](https://bing.com)
+7. Open the extension
+8. Click "Export" on the bottom right, then "Export as JSON" (This saves your cookies to clipboard)
+9. Paste your cookies into a file `cookies.json`
+
+>Instead of following steps 5-9 you can also use the following experimental helper function which has been tested on Windows 11 and requires `Selenium` and the latest version of Microsoft Edge:
+>
+>```
+>pip install selenium
+>```
+>```
+>from EdgeGPT Cookie
+>Cookie.fetch_default()
+>```
+>This will automatically create a file called `bing_cookies__default.json` in your current working directory.
+>
+>The double underscore in the name ensures it always gets used first if you have other cookie files e.g. `bing_cookies_pete.json` (see below regarding multiple cookie files).
+>
+>The `bing_` prefix in the name should avoid confusion with any other cookie files you might be using and is also used as a default by the `Cookie` helper class (see later).
+>
+>
 </details>
 
 <details>
 
 <summary>
 
-## Chatbot
+# Chatbot
 
 </summary>
 
-## Usage
 
-### Quick start
+## Running from the Command Line
 
 ```
  $ python3 -m EdgeGPT -h
 
         EdgeGPT - A demo of reverse engineering the Bing GPT chatbot
         Repo: github.com/acheong08/EdgeGPT
         By: Antonio Cheong
@@ -122,35 +127,20 @@
   --proxy PROXY         Proxy URL (e.g. socks5://127.0.0.1:1080)
   --wss-link WSS_LINK   WSS URL(e.g. wss://sydney.bing.com/sydney/ChatHub)
   --style {creative,balanced,precise}
   --cookie-file COOKIE_FILE
                         needed if environment variable COOKIE_FILE is not set
 ```
 
----
 
-## Running with Docker
+## Running in Python
 
-This assumes you have a file cookies.json in your current working directory
+### 1) The `Chatbot` class and `asyncio` for more granular control
 
-``` bash
-
-docker run --rm -it -v $(pwd)/cookies.json:/cookies.json:ro -e COOKIE_FILE='/cookies.json' ghcr.io/acheong08/edgegpt
-```
-
-You can add any extra flags as following
-
-``` bash
-
-docker run --rm -it -v $(pwd)/cookies.json:/cookies.json:ro -e COOKIE_FILE='/cookies.json' ghcr.io/acheong08/edgegpt --rich --style creative
-```
-
-### Developer demo
-
-Three ways to pass in cookies:
+There are three main ways to pass in cookies:
 
 - Environment variable: `export COOKIE_FILE=/path/to/cookies.json`.
 - Specify the path to `cookies.json` in the argument `cookie_path` like this:
 
   ```python
   bot = await Chatbot.create(cookie_path='./cookies.json')
   ```
@@ -159,43 +149,123 @@
 
   ```python
   with open('./cookies.json', 'r') as f:
       cookies = json.load(f)
   bot = await Chatbot.create(cookies=cookies)
   ```
 
-Use Async for the best experience
-
-Reference code for more advanced example of usage:
+Use Async for the best experience, for example:
 
 ```python
 import asyncio
 from EdgeGPT import Chatbot, ConversationStyle
 
 async def main():
     bot = await Chatbot.create()
     print(await bot.ask(prompt="Hello world", conversation_style=ConversationStyle.creative, wss_link="wss://sydney.bing.com/sydney/ChatHub"))
     await bot.close()
 
-
 if __name__ == "__main__":
     asyncio.run(main())
+```
+<details>
+<summary>
+  
+### 2) The `Query` and `Cookie` helper classes
+  </summary>
+  
+Create a simple Bing Chat AI query (using the 'precise' conversation style by default) and see just the main text output rather than the whole API response:
+
+```python
+from EdgeGPT import Query, Cookie
 
+q = Query("What are you? Give your answer as Python code")
+print(q)
+```
+
+Or change the conversation style or cookie file to be used:
+```python
+q = Query(
+  "What are you? Give your answer as Python code",
+  style="creative",  # or 'balanced'
+  cookies="./bing_cookies_alternative.json"
+)
+```
+
+Quickly extract the text output, code snippets, list of sources/references, or suggested follow-on questions using the following attributes:
+
+```python
+q.output
+q.code
+q.suggestions
+q.sources       # for the full json output
+q.sources_dict  # for a dictionary of titles and urls
+```
+
+Get the orginal prompt and the conversation style you specified:
+
+```python
+q.prompt
+q.style
+repr(q)
+```
+
+Access previous Queries made since importing `Query`:
+
+```python
+Query.index  # A list of Query objects; updated dynamically
+Query.request_count  # A tally of requests made using each cookie file
+```
+
+And finally, the `Cookie` class supports multiple cookie files, so if you create additional cookie files with the naming convention `bing_cookies_*.json`, your queries will automatically try using the next file (alphabetically) if you've exceeded your daily quota of requests (currently set at 200).
+
+Here are the main attributes which you can access:
+```python
+Cookie.current_file_index
+Cookie.dirpath
+Cookie.search_pattern  # default is `bing_cookies_*.json`
+Cookie.files()  # list as files that match .search_pattern
+Cookie.current_filepath
+Cookie.current_data
+Cookie.import_next()
+Cookie.image_token
+Cookie.ignore_files
+```
+</details>
+  
+---
+
+## Running with Docker
+
+This assumes you have a file cookies.json in your current working directory
+
+``` bash
+
+docker run --rm -it -v $(pwd)/cookies.json:/cookies.json:ro -e COOKIE_FILE='/cookies.json' ghcr.io/acheong08/edgegpt
+```
+
+You can add any extra flags as following
+
+``` bash
+
+docker run --rm -it -v $(pwd)/cookies.json:/cookies.json:ro -e COOKIE_FILE='/cookies.json' ghcr.io/acheong08/edgegpt --rich --style creative
 ```
 
 </details>
 
 <details>
 
 <summary>
 
-## Image generator
+# Image generator
 
 </summary>
 
+## Running from the Command Line
+
 ```bash
 $ python3 -m ImageGen -h
 usage: ImageGen.py [-h] [-U U] [--cookie-file COOKIE_FILE] --prompt PROMPT [--output-dir OUTPUT_DIR] [--quiet] [--asyncio]
 
 optional arguments:
   -h, --help            show this help message and exit
   -U U                  Auth cookie from browser
@@ -204,15 +274,32 @@
   --prompt PROMPT       Prompt to generate images for
   --output-dir OUTPUT_DIR
                         Output directory
   --quiet               Disable pipeline messages
   --asyncio             Run ImageGen using asyncio
 ```
 
-### Developer demo
+## Running in Python
+
+### 1) The `ImageQuery` helper class
+
+Generate images based on a simple prompt and download to the current working directory:
+
+```python
+from EdgeGPT import ImageQuery
+
+q=ImageQuery("Meerkats at a garden party in Devon")
+```
+Change the download directory for all future images in this session:
+
+```
+Query.image_dirpath = Path("./to_another_folder")
+```
+
+### 2) The `ImageGen` class and `asyncio` for more granular control
 
 ```python
 from ImageGen import ImageGen
 import argparse
 import json
 
 async def async_image_gen(args) -> None:
@@ -264,18 +351,18 @@
     else:
         asyncio.run(async_image_gen(args))
 
 ```
 
 </details>
 
-## Star History
+# Star History
 
 [![Star History Chart](https://api.star-history.com/svg?repos=acheong08/EdgeGPT&type=Date)](https://star-history.com/#acheong08/EdgeGPT&Date)
 
-## Contributors
+# Contributors
 
 This project exists thanks to all the people who contribute.
 
  <a href="https://github.com/acheong08/EdgeGPT/graphs/contributors">
   <img src="https://contrib.rocks/image?repo=acheong08/EdgeGPT" />
  </a>
```

#### html2text {}

```diff
@@ -1,90 +1,128 @@
-Metadata-Version: 2.1 Name: EdgeGPT Version: 0.3.9 Summary: Reverse engineered
+Metadata-Version: 2.1 Name: EdgeGPT Version: 0.4.0 Summary: Reverse engineered
 Edge Chat API Home-page: https://github.com/acheong08/EdgeGPT Author: Antonio
 Cheong Author-email: acheong@student.dalat.org License: GNU General Public
 License v2.0 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/
 issues/new Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Intended Audience :: Developers Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Description-Content-Type: text/markdown License-File: LICENSE
    [EdgeGPT] # Edge GPT _The reverse engineering the chat feature of the new
  version of Bing_ English - ç®ä½ä¸­æ - ç¹é«ä¸­æ - EspaÃ±ol - æ¥æ¬èª
                [PyPI_version] [Python version] [Total downloads]
---- ## Setup ### Install package ```bash python3 -m pip install EdgeGPT --
-upgrade ``` ### Requirements - python 3.8+ - A Microsoft Account with early
-access to
+  # Setup  ### Install package ```bash python3 -m pip install EdgeGPT --upgrade
+``` ### Requirements - python 3.8+ - A Microsoft Account with early access to
 bing.com/chat> (Required) - Required in a supported country with New Bing
-(Chinese mainland VPN required)   ### Checking access (Required)  - Install the
-latest version of Microsoft Edge - Alternatively, you can use any browser and
+(Chinese mainland VPN required) - [Selenium](https://pypi.org/project/selenium/
+) (for automatic cookie setup) ### Authentication (Required) 1. Install the
+latest version of Microsoft Edge 2. Alternatively, you can use any browser and
 set the user-agent to look like you're using Edge (e.g., `Mozilla/5.0 (Windows
 NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0
 Safari/537.36 Edg/111.0.1661.51`). You can do this easily with an extension
 like "User-Agent Switcher and Manager" for [Chrome](https://chrome.google.com/
 webstore/detail/user-agent-switcher-and-m/bhchdcejhohfmigjafbampogmaanbfkg) and
 [Firefox](https://addons.mozilla.org/en-US/firefox/addon/user-agent-string-
-switcher/). - Open [bing.com/chat](https://bing.com/chat) - If you see a chat
-feature, you are good to go    ### Getting authentication (Required)  - Install
-the cookie editor extension for [Chrome](https://chrome.google.com/webstore/
-detail/cookie-editor/hlkenndednhfkekhgcdicdfddnkalmdm) or [Firefox](https://
-addons.mozilla.org/en-US/firefox/addon/cookie-editor/) - Go to `bing.com` -
-Open the extension - Click "Export" on the bottom right, then "Export as JSON"
-(This saves your cookies to clipboard) - Paste your cookies into a file
-`cookies.json`    ## Chatbot  ## Usage ### Quick start ``` $ python3 -m EdgeGPT
--h EdgeGPT - A demo of reverse engineering the Bing GPT chatbot Repo:
-github.com/acheong08/EdgeGPT By: Antonio Cheong !help for help Type !exit to
-exit Enter twice to send message or set --enter-once to send one line message
-usage: EdgeGPT.py [-h] [--enter-once] [--no-stream] [--rich] [--proxy PROXY] [-
--wss-link WSS_LINK] [--style {creative,balanced,precise}] [--cookie-file
-COOKIE_FILE] options: -h, --help show this help message and exit --enter-once -
--no-stream --rich --proxy PROXY Proxy URL (e.g. socks5://127.0.0.1:1080) --wss-
-link WSS_LINK WSS URL(e.g. wss://sydney.bing.com/sydney/ChatHub) --style
-{creative,balanced,precise} --cookie-file COOKIE_FILE needed if environment
-variable COOKIE_FILE is not set ``` --- ## Running with Docker This assumes you
-have a file cookies.json in your current working directory ``` bash docker run
---rm -it -v $(pwd)/cookies.json:/cookies.json:ro -e COOKIE_FILE='/cookies.json'
-ghcr.io/acheong08/edgegpt ``` You can add any extra flags as following ``` bash
-docker run --rm -it -v $(pwd)/cookies.json:/cookies.json:ro -e COOKIE_FILE='/
-cookies.json' ghcr.io/acheong08/edgegpt --rich --style creative ``` ###
-Developer demo Three ways to pass in cookies: - Environment variable: `export
-COOKIE_FILE=/path/to/cookies.json`. - Specify the path to `cookies.json` in the
-argument `cookie_path` like this: ```python bot = await Chatbot.create
-(cookie_path='./cookies.json') ``` - Pass in the cookies directly by the
-argument `cookies`, like this: ```python with open('./cookies.json', 'r') as f:
-cookies = json.load(f) bot = await Chatbot.create(cookies=cookies) ``` Use
-Async for the best experience Reference code for more advanced example of
-usage: ```python import asyncio from EdgeGPT import Chatbot, ConversationStyle
-async def main(): bot = await Chatbot.create() print(await bot.ask
-(prompt="Hello world", conversation_style=ConversationStyle.creative,
-wss_link="wss://sydney.bing.com/sydney/ChatHub")) await bot.close() if __name__
-== "__main__": asyncio.run(main()) ```    ## Image generator  ```bash $ python3
--m ImageGen -h usage: ImageGen.py [-h] [-U U] [--cookie-file COOKIE_FILE] --
-prompt PROMPT [--output-dir OUTPUT_DIR] [--quiet] [--asyncio] optional
-arguments: -h, --help show this help message and exit -U U Auth cookie from
-browser --cookie-file COOKIE_FILE File containing auth cookie --prompt PROMPT
-Prompt to generate images for --output-dir OUTPUT_DIR Output directory --quiet
-Disable pipeline messages --asyncio Run ImageGen using asyncio ``` ###
-Developer demo ```python from ImageGen import ImageGen import argparse import
-json async def async_image_gen(args) -> None: async with ImageGenAsync(args.U,
-args.quiet) as image_generator: images = await image_generator.get_images
-(args.prompt) await image_generator.save_images(images,
-output_dir=args.output_dir) if __name__ == "__main__": parser =
+switcher/). 3. Open [bing.com/chat](https://bing.com/chat) 4. If you see a chat
+feature, you are good to continue... 5. Install the cookie editor extension for
+[Chrome](https://chrome.google.com/webstore/detail/cookie-editor/
+hlkenndednhfkekhgcdicdfddnkalmdm) or [Firefox](https://addons.mozilla.org/en-
+US/firefox/addon/cookie-editor/) 6. Go to [bing.com](https://bing.com) 7. Open
+the extension 8. Click "Export" on the bottom right, then "Export as JSON"
+(This saves your cookies to clipboard) 9. Paste your cookies into a file
+`cookies.json` >Instead of following steps 5-9 you can also use the following
+experimental helper function which has been tested on Windows 11 and requires
+`Selenium` and the latest version of Microsoft Edge: > >``` >pip install
+selenium >``` >``` >from EdgeGPT Cookie >Cookie.fetch_default() >``` >This will
+automatically create a file called `bing_cookies__default.json` in your current
+working directory. > >The double underscore in the name ensures it always gets
+used first if you have other cookie files e.g. `bing_cookies_pete.json` (see
+below regarding multiple cookie files). > >The `bing_` prefix in the name
+should avoid confusion with any other cookie files you might be using and is
+also used as a default by the `Cookie` helper class (see later). > >    #
+Chatbot  ## Running from the Command Line ``` $ python3 -m EdgeGPT -h EdgeGPT -
+A demo of reverse engineering the Bing GPT chatbot Repo: github.com/acheong08/
+EdgeGPT By: Antonio Cheong !help for help Type !exit to exit Enter twice to
+send message or set --enter-once to send one line message usage: EdgeGPT.py [-
+h] [--enter-once] [--no-stream] [--rich] [--proxy PROXY] [--wss-link WSS_LINK]
+[--style {creative,balanced,precise}] [--cookie-file COOKIE_FILE] options: -h,
+--help show this help message and exit --enter-once --no-stream --rich --proxy
+PROXY Proxy URL (e.g. socks5://127.0.0.1:1080) --wss-link WSS_LINK WSS URL(e.g.
+wss://sydney.bing.com/sydney/ChatHub) --style {creative,balanced,precise} --
+cookie-file COOKIE_FILE needed if environment variable COOKIE_FILE is not set
+``` ## Running in Python ### 1) The `Chatbot` class and `asyncio` for more
+granular control There are three main ways to pass in cookies: - Environment
+variable: `export COOKIE_FILE=/path/to/cookies.json`. - Specify the path to
+`cookies.json` in the argument `cookie_path` like this: ```python bot = await
+Chatbot.create(cookie_path='./cookies.json') ``` - Pass in the cookies directly
+by the argument `cookies`, like this: ```python with open('./cookies.json',
+'r') as f: cookies = json.load(f) bot = await Chatbot.create(cookies=cookies)
+``` Use Async for the best experience, for example: ```python import asyncio
+from EdgeGPT import Chatbot, ConversationStyle async def main(): bot = await
+Chatbot.create() print(await bot.ask(prompt="Hello world",
+conversation_style=ConversationStyle.creative, wss_link="wss://sydney.bing.com/
+sydney/ChatHub")) await bot.close() if __name__ == "__main__": asyncio.run(main
+()) ```   ### 2) The `Query` and `Cookie` helper classes  Create a simple Bing
+Chat AI query (using the 'precise' conversation style by default) and see just
+the main text output rather than the whole API response: ```python from EdgeGPT
+import Query, Cookie q = Query("What are you? Give your answer as Python code")
+print(q) ``` Or change the conversation style or cookie file to be used:
+```python q = Query( "What are you? Give your answer as Python code",
+style="creative", # or 'balanced' cookies="./bing_cookies_alternative.json" )
+``` Quickly extract the text output, code snippets, list of sources/references,
+or suggested follow-on questions using the following attributes: ```python
+q.output q.code q.suggestions q.sources # for the full json output
+q.sources_dict # for a dictionary of titles and urls ``` Get the orginal prompt
+and the conversation style you specified: ```python q.prompt q.style repr(q)
+``` Access previous Queries made since importing `Query`: ```python Query.index
+# A list of Query objects; updated dynamically Query.request_count # A tally of
+requests made using each cookie file ``` And finally, the `Cookie` class
+supports multiple cookie files, so if you create additional cookie files with
+the naming convention `bing_cookies_*.json`, your queries will automatically
+try using the next file (alphabetically) if you've exceeded your daily quota of
+requests (currently set at 200). Here are the main attributes which you can
+access: ```python Cookie.current_file_index Cookie.dirpath
+Cookie.search_pattern # default is `bing_cookies_*.json` Cookie.files() # list
+as files that match .search_pattern Cookie.current_filepath Cookie.current_data
+Cookie.import_next() Cookie.image_token Cookie.ignore_files ```  --- ## Running
+with Docker This assumes you have a file cookies.json in your current working
+directory ``` bash docker run --rm -it -v $(pwd)/cookies.json:/cookies.json:ro
+-e COOKIE_FILE='/cookies.json' ghcr.io/acheong08/edgegpt ``` You can add any
+extra flags as following ``` bash docker run --rm -it -v $(pwd)/cookies.json:/
+cookies.json:ro -e COOKIE_FILE='/cookies.json' ghcr.io/acheong08/edgegpt --rich
+--style creative ```    # Image generator  ## Running from the Command Line
+```bash $ python3 -m ImageGen -h usage: ImageGen.py [-h] [-U U] [--cookie-file
+COOKIE_FILE] --prompt PROMPT [--output-dir OUTPUT_DIR] [--quiet] [--asyncio]
+optional arguments: -h, --help show this help message and exit -U U Auth cookie
+from browser --cookie-file COOKIE_FILE File containing auth cookie --prompt
+PROMPT Prompt to generate images for --output-dir OUTPUT_DIR Output directory -
+-quiet Disable pipeline messages --asyncio Run ImageGen using asyncio ``` ##
+Running in Python ### 1) The `ImageQuery` helper class Generate images based on
+a simple prompt and download to the current working directory: ```python from
+EdgeGPT import ImageQuery q=ImageQuery("Meerkats at a garden party in Devon")
+``` Change the download directory for all future images in this session: ```
+Query.image_dirpath = Path("./to_another_folder") ``` ### 2) The `ImageGen`
+class and `asyncio` for more granular control ```python from ImageGen import
+ImageGen import argparse import json async def async_image_gen(args) -> None:
+async with ImageGenAsync(args.U, args.quiet) as image_generator: images = await
+image_generator.get_images(args.prompt) await image_generator.save_images
+(images, output_dir=args.output_dir) if __name__ == "__main__": parser =
 argparse.ArgumentParser() parser.add_argument("-U", help="Auth cookie from
 browser", type=str) parser.add_argument("--cookie-file", help="File containing
 auth cookie", type=str) parser.add_argument( "--prompt", help="Prompt to
 generate images for", type=str, required=True, ) parser.add_argument( "--
 output-dir", help="Output directory", type=str, default="./output", )
 parser.add_argument( "--quiet", help="Disable pipeline messages",
 action="store_true" ) parser.add_argument( "--asyncio", help="Run ImageGen
 using asyncio", action="store_true" ) args = parser.parse_args() # Load auth
 cookie with open(args.cookie_file, encoding="utf-8") as file: cookie_json =
 json.load(file) for cookie in cookie_json: if cookie.get("name") == "_U":
 args.U = cookie.get("value") break if args.U is None: raise Exception("Could
 not find auth cookie") if not args.asyncio: # Create image generator
 image_generator = ImageGen(args.U, args.quiet) image_generator.save_images
 ( image_generator.get_images(args.prompt), output_dir=args.output_dir, ) else:
-asyncio.run(async_image_gen(args)) ```  ## Star History [![Star History Chart]
+asyncio.run(async_image_gen(args)) ```  # Star History [![Star History Chart]
 (https://api.star-history.com/svg?repos=acheong08/EdgeGPT&type=Date)](https://
-star-history.com/#acheong08/EdgeGPT&Date) ## Contributors This project exists
+star-history.com/#acheong08/EdgeGPT&Date) # Contributors This project exists
 thanks to all the people who contribute. [https://contrib.rocks/
 image?repo=acheong08/EdgeGPT]
```

### Comparing `EdgeGPT-0.3.9/setup.py` & `EdgeGPT-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="EdgeGPT",
-    version="0.3.9",
+    version="0.4.0",
     license="GNU General Public License v2.0",
     author="Antonio Cheong",
     author_email="acheong@student.dalat.org",
     description="Reverse engineered Edge Chat API",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/acheong08/EdgeGPT",
```

### Comparing `EdgeGPT-0.3.9/src/EdgeGPT.egg-info/PKG-INFO` & `EdgeGPT-0.4.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: EdgeGPT
-Version: 0.3.9
-Summary: Reverse engineered Edge Chat API
-Home-page: https://github.com/acheong08/EdgeGPT
-Author: Antonio Cheong
-Author-email: acheong@student.dalat.org
-License: GNU General Public License v2.0
-Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/issues/new
-Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <div align="center">
   <img src="https://socialify.git.ci/acheong08/EdgeGPT/image?font=Inter&language=1&logo=https%3A%2F%2Fupload.wikimedia.org%2Fwikipedia%2Fcommons%2F9%2F9c%2FBing_Fluent_Logo.svg&owner=1&pattern=Floating%20Cogs&theme=Auto" alt="EdgeGPT" width="640" height="320" />
 
 # Edge GPT
 
 _The reverse engineering the chat feature of the new version of Bing_
 
@@ -33,75 +14,80 @@
 </div>
 
 <p align="center">
   <a href="https://github.com/acheong08/EdgeGPT">
     <img alt="PyPI version" src="https://img.shields.io/pypi/v/EdgeGPT">
   </a>
   <img alt="Python version" src="https://img.shields.io/badge/python-3.8+-blue.svg">
-
   <img alt="Total downloads" src="https://static.pepy.tech/badge/edgegpt">
 
 </p>
 
----
+<details>
+
+<summary>
 
-## Setup
+# Setup
+</summary>
 
 ### Install package
 
+
+
 ```bash
 python3 -m pip install EdgeGPT --upgrade
 ```
 
 ### Requirements
 
 - python 3.8+
 - A Microsoft Account with early access to <https://bing.com/chat> (Required)
 - Required in a supported country with New Bing (Chinese mainland VPN required)
+- [Selenium](https://pypi.org/project/selenium/) (for automatic cookie setup)
 
-<details>
-  <summary>
-
-### Checking access (Required)
-
-  </summary>
-
-- Install the latest version of Microsoft Edge
-- Alternatively, you can use any browser and set the user-agent to look like you're using Edge (e.g., `Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36 Edg/111.0.1661.51`). You can do this easily with an extension like "User-Agent Switcher and Manager" for [Chrome](https://chrome.google.com/webstore/detail/user-agent-switcher-and-m/bhchdcejhohfmigjafbampogmaanbfkg) and [Firefox](https://addons.mozilla.org/en-US/firefox/addon/user-agent-string-switcher/).
-- Open [bing.com/chat](https://bing.com/chat)
-- If you see a chat feature, you are good to go
-
-</details>
-
-<details>
-  <summary>
-
-### Getting authentication (Required)
-
-  </summary>
-
-- Install the cookie editor extension for [Chrome](https://chrome.google.com/webstore/detail/cookie-editor/hlkenndednhfkekhgcdicdfddnkalmdm) or [Firefox](https://addons.mozilla.org/en-US/firefox/addon/cookie-editor/)
-- Go to `bing.com`
-- Open the extension
-- Click "Export" on the bottom right, then "Export as JSON" (This saves your cookies to clipboard)
-- Paste your cookies into a file `cookies.json`
 
+### Authentication (Required)
+1. Install the latest version of Microsoft Edge
+2. Alternatively, you can use any browser and set the user-agent to look like you're using Edge (e.g., `Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36 Edg/111.0.1661.51`). You can do this easily with an extension like "User-Agent Switcher and Manager" for [Chrome](https://chrome.google.com/webstore/detail/user-agent-switcher-and-m/bhchdcejhohfmigjafbampogmaanbfkg) and [Firefox](https://addons.mozilla.org/en-US/firefox/addon/user-agent-string-switcher/).
+3. Open [bing.com/chat](https://bing.com/chat)
+4. If you see a chat feature, you are good to continue...
+5. Install the cookie editor extension for [Chrome](https://chrome.google.com/webstore/detail/cookie-editor/hlkenndednhfkekhgcdicdfddnkalmdm) or [Firefox](https://addons.mozilla.org/en-US/firefox/addon/cookie-editor/)
+6. Go to [bing.com](https://bing.com)
+7. Open the extension
+8. Click "Export" on the bottom right, then "Export as JSON" (This saves your cookies to clipboard)
+9. Paste your cookies into a file `cookies.json`
+
+>Instead of following steps 5-9 you can also use the following experimental helper function which has been tested on Windows 11 and requires `Selenium` and the latest version of Microsoft Edge:
+>
+>```
+>pip install selenium
+>```
+>```
+>from EdgeGPT Cookie
+>Cookie.fetch_default()
+>```
+>This will automatically create a file called `bing_cookies__default.json` in your current working directory.
+>
+>The double underscore in the name ensures it always gets used first if you have other cookie files e.g. `bing_cookies_pete.json` (see below regarding multiple cookie files).
+>
+>The `bing_` prefix in the name should avoid confusion with any other cookie files you might be using and is also used as a default by the `Cookie` helper class (see later).
+>
+>
 </details>
 
 <details>
 
 <summary>
 
-## Chatbot
+# Chatbot
 
 </summary>
 
-## Usage
 
-### Quick start
+## Running from the Command Line
 
 ```
  $ python3 -m EdgeGPT -h
 
         EdgeGPT - A demo of reverse engineering the Bing GPT chatbot
         Repo: github.com/acheong08/EdgeGPT
         By: Antonio Cheong
@@ -122,35 +108,20 @@
   --proxy PROXY         Proxy URL (e.g. socks5://127.0.0.1:1080)
   --wss-link WSS_LINK   WSS URL(e.g. wss://sydney.bing.com/sydney/ChatHub)
   --style {creative,balanced,precise}
   --cookie-file COOKIE_FILE
                         needed if environment variable COOKIE_FILE is not set
 ```
 
----
 
-## Running with Docker
+## Running in Python
 
-This assumes you have a file cookies.json in your current working directory
-
-``` bash
-
-docker run --rm -it -v $(pwd)/cookies.json:/cookies.json:ro -e COOKIE_FILE='/cookies.json' ghcr.io/acheong08/edgegpt
-```
+### 1) The `Chatbot` class and `asyncio` for more granular control
 
-You can add any extra flags as following
-
-``` bash
-
-docker run --rm -it -v $(pwd)/cookies.json:/cookies.json:ro -e COOKIE_FILE='/cookies.json' ghcr.io/acheong08/edgegpt --rich --style creative
-```
-
-### Developer demo
-
-Three ways to pass in cookies:
+There are three main ways to pass in cookies:
 
 - Environment variable: `export COOKIE_FILE=/path/to/cookies.json`.
 - Specify the path to `cookies.json` in the argument `cookie_path` like this:
 
   ```python
   bot = await Chatbot.create(cookie_path='./cookies.json')
   ```
@@ -159,43 +130,123 @@
 
   ```python
   with open('./cookies.json', 'r') as f:
       cookies = json.load(f)
   bot = await Chatbot.create(cookies=cookies)
   ```
 
-Use Async for the best experience
-
-Reference code for more advanced example of usage:
+Use Async for the best experience, for example:
 
 ```python
 import asyncio
 from EdgeGPT import Chatbot, ConversationStyle
 
 async def main():
     bot = await Chatbot.create()
     print(await bot.ask(prompt="Hello world", conversation_style=ConversationStyle.creative, wss_link="wss://sydney.bing.com/sydney/ChatHub"))
     await bot.close()
 
-
 if __name__ == "__main__":
     asyncio.run(main())
+```
+<details>
+<summary>
+  
+### 2) The `Query` and `Cookie` helper classes
+  </summary>
+  
+Create a simple Bing Chat AI query (using the 'precise' conversation style by default) and see just the main text output rather than the whole API response:
+
+```python
+from EdgeGPT import Query, Cookie
+
+q = Query("What are you? Give your answer as Python code")
+print(q)
+```
+
+Or change the conversation style or cookie file to be used:
+```python
+q = Query(
+  "What are you? Give your answer as Python code",
+  style="creative",  # or 'balanced'
+  cookies="./bing_cookies_alternative.json"
+)
+```
+
+Quickly extract the text output, code snippets, list of sources/references, or suggested follow-on questions using the following attributes:
+
+```python
+q.output
+q.code
+q.suggestions
+q.sources       # for the full json output
+q.sources_dict  # for a dictionary of titles and urls
+```
+
+Get the orginal prompt and the conversation style you specified:
+
+```python
+q.prompt
+q.style
+repr(q)
+```
 
+Access previous Queries made since importing `Query`:
+
+```python
+Query.index  # A list of Query objects; updated dynamically
+Query.request_count  # A tally of requests made using each cookie file
+```
+
+And finally, the `Cookie` class supports multiple cookie files, so if you create additional cookie files with the naming convention `bing_cookies_*.json`, your queries will automatically try using the next file (alphabetically) if you've exceeded your daily quota of requests (currently set at 200).
+
+Here are the main attributes which you can access:
+```python
+Cookie.current_file_index
+Cookie.dirpath
+Cookie.search_pattern  # default is `bing_cookies_*.json`
+Cookie.files()  # list as files that match .search_pattern
+Cookie.current_filepath
+Cookie.current_data
+Cookie.import_next()
+Cookie.image_token
+Cookie.ignore_files
+```
+</details>
+  
+---
+
+## Running with Docker
+
+This assumes you have a file cookies.json in your current working directory
+
+``` bash
+
+docker run --rm -it -v $(pwd)/cookies.json:/cookies.json:ro -e COOKIE_FILE='/cookies.json' ghcr.io/acheong08/edgegpt
+```
+
+You can add any extra flags as following
+
+``` bash
+
+docker run --rm -it -v $(pwd)/cookies.json:/cookies.json:ro -e COOKIE_FILE='/cookies.json' ghcr.io/acheong08/edgegpt --rich --style creative
 ```
 
 </details>
 
 <details>
 
 <summary>
 
-## Image generator
+# Image generator
 
 </summary>
 
+## Running from the Command Line
+
 ```bash
 $ python3 -m ImageGen -h
 usage: ImageGen.py [-h] [-U U] [--cookie-file COOKIE_FILE] --prompt PROMPT [--output-dir OUTPUT_DIR] [--quiet] [--asyncio]
 
 optional arguments:
   -h, --help            show this help message and exit
   -U U                  Auth cookie from browser
@@ -204,15 +255,32 @@
   --prompt PROMPT       Prompt to generate images for
   --output-dir OUTPUT_DIR
                         Output directory
   --quiet               Disable pipeline messages
   --asyncio             Run ImageGen using asyncio
 ```
 
-### Developer demo
+## Running in Python
+
+### 1) The `ImageQuery` helper class
+
+Generate images based on a simple prompt and download to the current working directory:
+
+```python
+from EdgeGPT import ImageQuery
+
+q=ImageQuery("Meerkats at a garden party in Devon")
+```
+Change the download directory for all future images in this session:
+
+```
+Query.image_dirpath = Path("./to_another_folder")
+```
+
+### 2) The `ImageGen` class and `asyncio` for more granular control
 
 ```python
 from ImageGen import ImageGen
 import argparse
 import json
 
 async def async_image_gen(args) -> None:
@@ -264,18 +332,18 @@
     else:
         asyncio.run(async_image_gen(args))
 
 ```
 
 </details>
 
-## Star History
+# Star History
 
 [![Star History Chart](https://api.star-history.com/svg?repos=acheong08/EdgeGPT&type=Date)](https://star-history.com/#acheong08/EdgeGPT&Date)
 
-## Contributors
+# Contributors
 
 This project exists thanks to all the people who contribute.
 
  <a href="https://github.com/acheong08/EdgeGPT/graphs/contributors">
   <img src="https://contrib.rocks/image?repo=acheong08/EdgeGPT" />
  </a>
```

#### html2text {}

```diff
@@ -1,90 +1,118 @@
-Metadata-Version: 2.1 Name: EdgeGPT Version: 0.3.9 Summary: Reverse engineered
-Edge Chat API Home-page: https://github.com/acheong08/EdgeGPT Author: Antonio
-Cheong Author-email: acheong@student.dalat.org License: GNU General Public
-License v2.0 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/
-issues/new Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
-Classifier: Intended Audience :: Developers Classifier: Topic :: Software
-Development :: Libraries :: Python Modules Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Description-Content-Type: text/markdown License-File: LICENSE
    [EdgeGPT] # Edge GPT _The reverse engineering the chat feature of the new
  version of Bing_ English - ç®ä½ä¸­æ - ç¹é«ä¸­æ - EspaÃ±ol - æ¥æ¬èª
                [PyPI_version] [Python version] [Total downloads]
---- ## Setup ### Install package ```bash python3 -m pip install EdgeGPT --
-upgrade ``` ### Requirements - python 3.8+ - A Microsoft Account with early
-access to
+  # Setup  ### Install package ```bash python3 -m pip install EdgeGPT --upgrade
+``` ### Requirements - python 3.8+ - A Microsoft Account with early access to
 bing.com/chat> (Required) - Required in a supported country with New Bing
-(Chinese mainland VPN required)   ### Checking access (Required)  - Install the
-latest version of Microsoft Edge - Alternatively, you can use any browser and
+(Chinese mainland VPN required) - [Selenium](https://pypi.org/project/selenium/
+) (for automatic cookie setup) ### Authentication (Required) 1. Install the
+latest version of Microsoft Edge 2. Alternatively, you can use any browser and
 set the user-agent to look like you're using Edge (e.g., `Mozilla/5.0 (Windows
 NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0
 Safari/537.36 Edg/111.0.1661.51`). You can do this easily with an extension
 like "User-Agent Switcher and Manager" for [Chrome](https://chrome.google.com/
 webstore/detail/user-agent-switcher-and-m/bhchdcejhohfmigjafbampogmaanbfkg) and
 [Firefox](https://addons.mozilla.org/en-US/firefox/addon/user-agent-string-
-switcher/). - Open [bing.com/chat](https://bing.com/chat) - If you see a chat
-feature, you are good to go    ### Getting authentication (Required)  - Install
-the cookie editor extension for [Chrome](https://chrome.google.com/webstore/
-detail/cookie-editor/hlkenndednhfkekhgcdicdfddnkalmdm) or [Firefox](https://
-addons.mozilla.org/en-US/firefox/addon/cookie-editor/) - Go to `bing.com` -
-Open the extension - Click "Export" on the bottom right, then "Export as JSON"
-(This saves your cookies to clipboard) - Paste your cookies into a file
-`cookies.json`    ## Chatbot  ## Usage ### Quick start ``` $ python3 -m EdgeGPT
--h EdgeGPT - A demo of reverse engineering the Bing GPT chatbot Repo:
-github.com/acheong08/EdgeGPT By: Antonio Cheong !help for help Type !exit to
-exit Enter twice to send message or set --enter-once to send one line message
-usage: EdgeGPT.py [-h] [--enter-once] [--no-stream] [--rich] [--proxy PROXY] [-
--wss-link WSS_LINK] [--style {creative,balanced,precise}] [--cookie-file
-COOKIE_FILE] options: -h, --help show this help message and exit --enter-once -
--no-stream --rich --proxy PROXY Proxy URL (e.g. socks5://127.0.0.1:1080) --wss-
-link WSS_LINK WSS URL(e.g. wss://sydney.bing.com/sydney/ChatHub) --style
-{creative,balanced,precise} --cookie-file COOKIE_FILE needed if environment
-variable COOKIE_FILE is not set ``` --- ## Running with Docker This assumes you
-have a file cookies.json in your current working directory ``` bash docker run
---rm -it -v $(pwd)/cookies.json:/cookies.json:ro -e COOKIE_FILE='/cookies.json'
-ghcr.io/acheong08/edgegpt ``` You can add any extra flags as following ``` bash
-docker run --rm -it -v $(pwd)/cookies.json:/cookies.json:ro -e COOKIE_FILE='/
-cookies.json' ghcr.io/acheong08/edgegpt --rich --style creative ``` ###
-Developer demo Three ways to pass in cookies: - Environment variable: `export
-COOKIE_FILE=/path/to/cookies.json`. - Specify the path to `cookies.json` in the
-argument `cookie_path` like this: ```python bot = await Chatbot.create
-(cookie_path='./cookies.json') ``` - Pass in the cookies directly by the
-argument `cookies`, like this: ```python with open('./cookies.json', 'r') as f:
-cookies = json.load(f) bot = await Chatbot.create(cookies=cookies) ``` Use
-Async for the best experience Reference code for more advanced example of
-usage: ```python import asyncio from EdgeGPT import Chatbot, ConversationStyle
-async def main(): bot = await Chatbot.create() print(await bot.ask
-(prompt="Hello world", conversation_style=ConversationStyle.creative,
-wss_link="wss://sydney.bing.com/sydney/ChatHub")) await bot.close() if __name__
-== "__main__": asyncio.run(main()) ```    ## Image generator  ```bash $ python3
--m ImageGen -h usage: ImageGen.py [-h] [-U U] [--cookie-file COOKIE_FILE] --
-prompt PROMPT [--output-dir OUTPUT_DIR] [--quiet] [--asyncio] optional
-arguments: -h, --help show this help message and exit -U U Auth cookie from
-browser --cookie-file COOKIE_FILE File containing auth cookie --prompt PROMPT
-Prompt to generate images for --output-dir OUTPUT_DIR Output directory --quiet
-Disable pipeline messages --asyncio Run ImageGen using asyncio ``` ###
-Developer demo ```python from ImageGen import ImageGen import argparse import
-json async def async_image_gen(args) -> None: async with ImageGenAsync(args.U,
-args.quiet) as image_generator: images = await image_generator.get_images
-(args.prompt) await image_generator.save_images(images,
-output_dir=args.output_dir) if __name__ == "__main__": parser =
+switcher/). 3. Open [bing.com/chat](https://bing.com/chat) 4. If you see a chat
+feature, you are good to continue... 5. Install the cookie editor extension for
+[Chrome](https://chrome.google.com/webstore/detail/cookie-editor/
+hlkenndednhfkekhgcdicdfddnkalmdm) or [Firefox](https://addons.mozilla.org/en-
+US/firefox/addon/cookie-editor/) 6. Go to [bing.com](https://bing.com) 7. Open
+the extension 8. Click "Export" on the bottom right, then "Export as JSON"
+(This saves your cookies to clipboard) 9. Paste your cookies into a file
+`cookies.json` >Instead of following steps 5-9 you can also use the following
+experimental helper function which has been tested on Windows 11 and requires
+`Selenium` and the latest version of Microsoft Edge: > >``` >pip install
+selenium >``` >``` >from EdgeGPT Cookie >Cookie.fetch_default() >``` >This will
+automatically create a file called `bing_cookies__default.json` in your current
+working directory. > >The double underscore in the name ensures it always gets
+used first if you have other cookie files e.g. `bing_cookies_pete.json` (see
+below regarding multiple cookie files). > >The `bing_` prefix in the name
+should avoid confusion with any other cookie files you might be using and is
+also used as a default by the `Cookie` helper class (see later). > >    #
+Chatbot  ## Running from the Command Line ``` $ python3 -m EdgeGPT -h EdgeGPT -
+A demo of reverse engineering the Bing GPT chatbot Repo: github.com/acheong08/
+EdgeGPT By: Antonio Cheong !help for help Type !exit to exit Enter twice to
+send message or set --enter-once to send one line message usage: EdgeGPT.py [-
+h] [--enter-once] [--no-stream] [--rich] [--proxy PROXY] [--wss-link WSS_LINK]
+[--style {creative,balanced,precise}] [--cookie-file COOKIE_FILE] options: -h,
+--help show this help message and exit --enter-once --no-stream --rich --proxy
+PROXY Proxy URL (e.g. socks5://127.0.0.1:1080) --wss-link WSS_LINK WSS URL(e.g.
+wss://sydney.bing.com/sydney/ChatHub) --style {creative,balanced,precise} --
+cookie-file COOKIE_FILE needed if environment variable COOKIE_FILE is not set
+``` ## Running in Python ### 1) The `Chatbot` class and `asyncio` for more
+granular control There are three main ways to pass in cookies: - Environment
+variable: `export COOKIE_FILE=/path/to/cookies.json`. - Specify the path to
+`cookies.json` in the argument `cookie_path` like this: ```python bot = await
+Chatbot.create(cookie_path='./cookies.json') ``` - Pass in the cookies directly
+by the argument `cookies`, like this: ```python with open('./cookies.json',
+'r') as f: cookies = json.load(f) bot = await Chatbot.create(cookies=cookies)
+``` Use Async for the best experience, for example: ```python import asyncio
+from EdgeGPT import Chatbot, ConversationStyle async def main(): bot = await
+Chatbot.create() print(await bot.ask(prompt="Hello world",
+conversation_style=ConversationStyle.creative, wss_link="wss://sydney.bing.com/
+sydney/ChatHub")) await bot.close() if __name__ == "__main__": asyncio.run(main
+()) ```   ### 2) The `Query` and `Cookie` helper classes  Create a simple Bing
+Chat AI query (using the 'precise' conversation style by default) and see just
+the main text output rather than the whole API response: ```python from EdgeGPT
+import Query, Cookie q = Query("What are you? Give your answer as Python code")
+print(q) ``` Or change the conversation style or cookie file to be used:
+```python q = Query( "What are you? Give your answer as Python code",
+style="creative", # or 'balanced' cookies="./bing_cookies_alternative.json" )
+``` Quickly extract the text output, code snippets, list of sources/references,
+or suggested follow-on questions using the following attributes: ```python
+q.output q.code q.suggestions q.sources # for the full json output
+q.sources_dict # for a dictionary of titles and urls ``` Get the orginal prompt
+and the conversation style you specified: ```python q.prompt q.style repr(q)
+``` Access previous Queries made since importing `Query`: ```python Query.index
+# A list of Query objects; updated dynamically Query.request_count # A tally of
+requests made using each cookie file ``` And finally, the `Cookie` class
+supports multiple cookie files, so if you create additional cookie files with
+the naming convention `bing_cookies_*.json`, your queries will automatically
+try using the next file (alphabetically) if you've exceeded your daily quota of
+requests (currently set at 200). Here are the main attributes which you can
+access: ```python Cookie.current_file_index Cookie.dirpath
+Cookie.search_pattern # default is `bing_cookies_*.json` Cookie.files() # list
+as files that match .search_pattern Cookie.current_filepath Cookie.current_data
+Cookie.import_next() Cookie.image_token Cookie.ignore_files ```  --- ## Running
+with Docker This assumes you have a file cookies.json in your current working
+directory ``` bash docker run --rm -it -v $(pwd)/cookies.json:/cookies.json:ro
+-e COOKIE_FILE='/cookies.json' ghcr.io/acheong08/edgegpt ``` You can add any
+extra flags as following ``` bash docker run --rm -it -v $(pwd)/cookies.json:/
+cookies.json:ro -e COOKIE_FILE='/cookies.json' ghcr.io/acheong08/edgegpt --rich
+--style creative ```    # Image generator  ## Running from the Command Line
+```bash $ python3 -m ImageGen -h usage: ImageGen.py [-h] [-U U] [--cookie-file
+COOKIE_FILE] --prompt PROMPT [--output-dir OUTPUT_DIR] [--quiet] [--asyncio]
+optional arguments: -h, --help show this help message and exit -U U Auth cookie
+from browser --cookie-file COOKIE_FILE File containing auth cookie --prompt
+PROMPT Prompt to generate images for --output-dir OUTPUT_DIR Output directory -
+-quiet Disable pipeline messages --asyncio Run ImageGen using asyncio ``` ##
+Running in Python ### 1) The `ImageQuery` helper class Generate images based on
+a simple prompt and download to the current working directory: ```python from
+EdgeGPT import ImageQuery q=ImageQuery("Meerkats at a garden party in Devon")
+``` Change the download directory for all future images in this session: ```
+Query.image_dirpath = Path("./to_another_folder") ``` ### 2) The `ImageGen`
+class and `asyncio` for more granular control ```python from ImageGen import
+ImageGen import argparse import json async def async_image_gen(args) -> None:
+async with ImageGenAsync(args.U, args.quiet) as image_generator: images = await
+image_generator.get_images(args.prompt) await image_generator.save_images
+(images, output_dir=args.output_dir) if __name__ == "__main__": parser =
 argparse.ArgumentParser() parser.add_argument("-U", help="Auth cookie from
 browser", type=str) parser.add_argument("--cookie-file", help="File containing
 auth cookie", type=str) parser.add_argument( "--prompt", help="Prompt to
 generate images for", type=str, required=True, ) parser.add_argument( "--
 output-dir", help="Output directory", type=str, default="./output", )
 parser.add_argument( "--quiet", help="Disable pipeline messages",
 action="store_true" ) parser.add_argument( "--asyncio", help="Run ImageGen
 using asyncio", action="store_true" ) args = parser.parse_args() # Load auth
 cookie with open(args.cookie_file, encoding="utf-8") as file: cookie_json =
 json.load(file) for cookie in cookie_json: if cookie.get("name") == "_U":
 args.U = cookie.get("value") break if args.U is None: raise Exception("Could
 not find auth cookie") if not args.asyncio: # Create image generator
 image_generator = ImageGen(args.U, args.quiet) image_generator.save_images
 ( image_generator.get_images(args.prompt), output_dir=args.output_dir, ) else:
-asyncio.run(async_image_gen(args)) ```  ## Star History [![Star History Chart]
+asyncio.run(async_image_gen(args)) ```  # Star History [![Star History Chart]
 (https://api.star-history.com/svg?repos=acheong08/EdgeGPT&type=Date)](https://
-star-history.com/#acheong08/EdgeGPT&Date) ## Contributors This project exists
+star-history.com/#acheong08/EdgeGPT&Date) # Contributors This project exists
 thanks to all the people who contribute. [https://contrib.rocks/
 image?repo=acheong08/EdgeGPT]
```

### Comparing `EdgeGPT-0.3.9/src/EdgeGPT.py` & `EdgeGPT-0.4.0/src/EdgeGPT.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,26 +7,27 @@
 import asyncio
 import json
 import os
 import random
 import re
 import ssl
 import sys
+import time
 import uuid
 from enum import Enum
 from pathlib import Path
 from typing import Generator
 from typing import Literal
 from typing import Optional
 from typing import Union
 
 import certifi
 import httpx
 import websockets.client as websockets
-from BingImageCreator import ImageGenAsync
+from BingImageCreator import ImageGen, ImageGenAsync
 from prompt_toolkit import PromptSession
 from prompt_toolkit.auto_suggest import AutoSuggestFromHistory
 from prompt_toolkit.completion import WordCompleter
 from prompt_toolkit.history import InMemoryHistory
 from prompt_toolkit.key_binding import KeyBindings
 from rich.live import Live
 from rich.markdown import Markdown
@@ -541,15 +542,17 @@
                                     ][0]["body"][0]["inlines"][0].get("text")
                                     + "\n"
                                 )
                         yield False, resp_txt
 
                 elif response.get("type") == 2:
                     if response["item"]["result"].get("error"):
-                        raise Exception(f"{response['item']['result']['value']}: {response['item']['result']['message']}")
+                        raise Exception(
+                            f"{response['item']['result']['value']}: {response['item']['result']['message']}",
+                        )
                     if draw:
                         cache = response["item"]["messages"][1]["adaptiveCards"][0][
                             "body"
                         ][0]["text"]
                         response["item"]["messages"][1]["adaptiveCards"][0]["body"][0][
                             "text"
                         ] = (cache + resp_txt)
@@ -874,9 +877,236 @@
     except OSError as exc:
         print(f"Could not open cookie file: {exc}", file=sys.stderr)
         sys.exit(1)
 
     asyncio.run(async_main(args))
 
 
+class Cookie:
+    """
+    Convenience class for Bing Cookie files, data, and configuration. This Class
+    is updated dynamically by the Query class to allow cycling through >1
+    cookie/credentials file e.g. when daily request limits (current 200 per
+    account per day) are exceeded.
+    """
+
+    current_file_index = 0
+    dirpath = Path("./").resolve()
+    search_pattern = "bing_cookies_*.json"
+    ignore_files = set()
+
+    @classmethod
+    def fetch_default(cls, path=None):
+        from selenium import webdriver
+        from selenium.webdriver.common.by import By
+
+        driver = webdriver.Edge()
+        driver.get("https://bing.com/chat")
+        time.sleep(5)
+        xpath = '//button[@id="bnp_btn_accept"]'
+        driver.find_element(By.XPATH, xpath).click()
+        time.sleep(2)
+        xpath = '//a[@id="codexPrimaryButton"]'
+        driver.find_element(By.XPATH, xpath).click()
+        if path is None:
+            path = Path("./bing_cookies__default.json")
+            # Double underscore ensures this file is first when sorted
+        cookies = driver.get_cookies()
+        Path(path).write_text(json.dumps(cookies, indent=4))
+        # Path again in case supplied path is: str
+        print(f"Cookies saved to: {path}")
+        driver.quit()
+
+    @classmethod
+    def files(cls):
+        """Return a sorted list of all cookie files matching .search_pattern"""
+        all_files = set(cls.dirpath.glob(cls.search_pattern))
+        return sorted(list(all_files - cls.ignore_files))
+
+    @classmethod
+    def import_data(cls):
+        """
+        Read the active cookie file and populate the following attributes:
+
+          .current_filepath
+          .current_data
+          .image_token
+        """
+        cls.current_filepath = cls.files()[cls.current_file_index]
+        print(f"> Importing cookies from: {cls.current_filepath.name}")
+        with open(cls.current_filepath, encoding="utf-8") as file:
+            cls.current_data = json.load(file)
+        cls.image_token = [x for x in cls.current_data if x.get("name") == "_U"]
+        cls.image_token = cls.image_token[0].get("value")
+
+    @classmethod
+    def import_next(cls):
+        """
+        Cycle through to the next cookies file.  Import it.  Mark the previous
+        file to be ignored for the remainder of the current session.
+        """
+        cls.ignore_files.add(cls.current_filepath)
+        if Cookie.current_file_index >= len(cls.files()):
+            Cookie.current_file_index = 0
+        Cookie.import_data()
+
+
+class Query:
+    """
+    A convenience class that wraps around EdgeGPT.Chatbot to encapsulate input,
+    config, and output all together.  Relies on Cookie class for authentication
+    """
+
+    index = []
+    request_count = {}
+    image_dirpath = Path("./").resolve()
+    Cookie.import_data()
+
+    def __init__(
+        self,
+        prompt,
+        style="precise",
+        content_type="text",
+        cookie_file=0,
+        echo=True,
+        echo_prompt=False,
+    ):
+        """
+        Arguments:
+
+        prompt: Text to enter into Bing Chat
+        style: creative, balanced, or precise
+        content_type: "text" for Bing Chat; "image" for Dall-e
+        cookie_file: Path, filepath string, or index (int) to list of cookie paths
+        echo: Print something to confirm request made
+        echo_prompt: Print confirmation of the evaluated prompt
+        """
+        self.__class__.index += [self]
+        self.prompt = prompt
+        files = Cookie.files()
+        if isinstance(cookie_file, int):
+            index = cookie_file if cookie_file < len(files) else 0
+        else:
+            if not isinstance(cookie_file, (str, Path)):
+                message = "'cookie_file' must be an int, str, or Path object"
+                raise TypeError(message)
+            cookie_file = Path(cookie_file)
+            if cookie_file in files():  # Supplied filepath IS in Cookie.dirpath
+                index = files.index(cookie_file)
+            else:  # Supplied filepath is NOT in Cookie.dirpath
+                if cookie_file.is_file():
+                    Cookie.dirpath = cookie_file.parent.resolve()
+                if cookie_file.is_dir():
+                    Cookie.dirpath = cookie_file.resolve()
+                index = 0
+        Cookie.current_file_index = index
+        if content_type == "text":
+            self.style = style
+            self.log_and_send_query(echo, echo_prompt)
+        if content_type == "image":
+            self.create_image()
+
+    def log_and_send_query(self, echo, echo_prompt):
+        self.response = asyncio.run(self.send_to_bing(echo, echo_prompt))
+        name = str(Cookie.current_filepath.name)
+        if not self.__class__.request_count.get(name):
+            self.__class__.request_count[name] = 1
+        else:
+            self.__class__.request_count[name] += 1
+
+    def create_image(self):
+        image_generator = ImageGen(Cookie.image_token)
+        image_generator.save_images(
+            image_generator.get_images(self.prompt),
+            output_dir=self.__class__.image_dirpath,
+        )
+
+    async def send_to_bing(self, echo=True, echo_prompt=False):
+        """Creat, submit, then close a Chatbot instance.  Return the response"""
+        retries = len(Cookie.files())
+        while retries:
+            try:
+                bot = await Chatbot.create(cookies=Cookie.current_data)
+                if echo_prompt:
+                    print(f"> {self.prompt=}")
+                if echo:
+                    print("> Waiting for response...")
+                if self.style.lower() not in "creative balanced precise".split():
+                    self.style = "precise"
+                response = await bot.ask(
+                    prompt=self.prompt,
+                    conversation_style=getattr(ConversationStyle, self.style),
+                    # wss_link="wss://sydney.bing.com/sydney/ChatHub"
+                    # What other values can this parameter take? It seems to be optional
+                )
+                return response
+            except KeyError:
+                print(
+                    f"> KeyError [{Cookie.current_filepath.name} may have exceeded the daily limit]",
+                )
+                Cookie.import_next()
+                retries -= 1
+            finally:
+                await bot.close()
+
+    @property
+    def output(self):
+        """The response from a completed Chatbot request"""
+        return self.response["item"]["messages"][1]["text"]
+
+    @property
+    def sources(self):
+        """The source names and details parsed from a completed Chatbot request"""
+        return self.response["item"]["messages"][1]["sourceAttributions"]
+
+    @property
+    def sources_dict(self):
+        """The source names and details as a dictionary"""
+        sources_dict = {}
+        name = "providerDisplayName"
+        url = "seeMoreUrl"
+        for source in self.sources:
+            if name in source.keys() and url in source.keys():
+                sources_dict[source[name]] = source[url]
+            else:
+                continue
+        return sources_dict
+
+    @property
+    def code(self):
+        """Extract and join any snippets of Python code in the response"""
+        code_blocks = self.output.split("```")[1:-1:2]
+        code_blocks = ["\n".join(x.splitlines()[1:]) for x in code_blocks]
+        return "\n\n".join(code_blocks)
+
+    @property
+    def languages(self):
+        """Extract all programming languages given in code blocks"""
+        code_blocks = self.output.split("```")[1:-1:2]
+        return {x.splitlines()[0] for x in code_blocks}
+
+    @property
+    def suggestions(self):
+        """Follow-on questions suggested by the Chatbot"""
+        return [
+            x["text"]
+            for x in self.response["item"]["messages"][1]["suggestedResponses"]
+        ]
+
+    def __repr__(self):
+        return f"<EdgeGPT.Query: {self.prompt}>"
+
+    def __str__(self):
+        return self.output
+
+
+class ImageQuery(Query):
+    def __init__(self, prompt, **kwargs):
+        kwargs.update({"content_type": "image"})
+        super().__init__(prompt, **kwargs)
+
+    def __repr__(self):
+        return f"<EdgeGPT.ImageQuery: {self.prompt}>"
+
+
 if __name__ == "__main__":
     main()
```

