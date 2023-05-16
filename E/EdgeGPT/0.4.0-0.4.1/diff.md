# Comparing `tmp/EdgeGPT-0.4.0.tar.gz` & `tmp/EdgeGPT-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EdgeGPT-0.4.0.tar", last modified: Tue May 16 03:14:15 2023, max compression
+gzip compressed data, was "EdgeGPT-0.4.1.tar", last modified: Tue May 16 05:08:21 2023, max compression
```

## Comparing `EdgeGPT-0.4.0.tar` & `EdgeGPT-0.4.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:14:15.728615 EdgeGPT-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-16 03:13:47.000000 EdgeGPT-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-05-16 03:14:15.728615 EdgeGPT-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10581 2023-05-16 03:14:15.000000 EdgeGPT-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-16 03:14:15.728615 EdgeGPT-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-16 03:13:47.000000 EdgeGPT-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:14:15.728615 EdgeGPT-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 03:14:15.728615 EdgeGPT-0.4.0/src/EdgeGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-05-16 03:14:15.000000 EdgeGPT-0.4.0/src/EdgeGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-16 03:14:15.000000 EdgeGPT-0.4.0/src/EdgeGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 03:14:15.000000 EdgeGPT-0.4.0/src/EdgeGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-16 03:14:15.000000 EdgeGPT-0.4.0/src/EdgeGPT.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-16 03:14:15.000000 EdgeGPT-0.4.0/src/EdgeGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 03:14:15.000000 EdgeGPT-0.4.0/src/EdgeGPT.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    38159 2023-05-16 03:13:47.000000 EdgeGPT-0.4.0/src/EdgeGPT.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-16 03:13:47.000000 EdgeGPT-0.4.0/src/ImageGen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:08:21.437254 EdgeGPT-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-16 05:07:49.000000 EdgeGPT-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11297 2023-05-16 05:08:21.437254 EdgeGPT-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10532 2023-05-16 05:08:21.000000 EdgeGPT-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-16 05:08:21.437254 EdgeGPT-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-16 05:07:49.000000 EdgeGPT-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:08:21.433254 EdgeGPT-0.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:08:21.437254 EdgeGPT-0.4.1/src/EdgeGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11297 2023-05-16 05:08:21.000000 EdgeGPT-0.4.1/src/EdgeGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-16 05:08:21.000000 EdgeGPT-0.4.1/src/EdgeGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 05:08:21.000000 EdgeGPT-0.4.1/src/EdgeGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-16 05:08:21.000000 EdgeGPT-0.4.1/src/EdgeGPT.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-16 05:08:21.000000 EdgeGPT-0.4.1/src/EdgeGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 05:08:21.000000 EdgeGPT-0.4.1/src/EdgeGPT.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    38139 2023-05-16 05:07:49.000000 EdgeGPT-0.4.1/src/EdgeGPT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-16 05:07:49.000000 EdgeGPT-0.4.1/src/ImageGen.py
```

### Comparing `EdgeGPT-0.4.0/LICENSE` & `EdgeGPT-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `EdgeGPT-0.4.0/PKG-INFO` & `EdgeGPT-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdgeGPT
-Version: 0.4.0
+Version: 0.4.1
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/acheong08/EdgeGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
@@ -157,15 +157,15 @@
 
 ```python
 import asyncio
 from EdgeGPT import Chatbot, ConversationStyle
 
 async def main():
     bot = await Chatbot.create()
-    print(await bot.ask(prompt="Hello world", conversation_style=ConversationStyle.creative, wss_link="wss://sydney.bing.com/sydney/ChatHub"))
+    print(await bot.ask(prompt="Hello world", conversation_style=ConversationStyle.creative))
     await bot.close()
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 <details>
 <summary>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: EdgeGPT Version: 0.4.0 Summary: Reverse engineered
+Metadata-Version: 2.1 Name: EdgeGPT Version: 0.4.1 Summary: Reverse engineered
 Edge Chat API Home-page: https://github.com/acheong08/EdgeGPT Author: Antonio
 Cheong Author-email: acheong@student.dalat.org License: GNU General Public
 License v2.0 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/
 issues/new Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Intended Audience :: Developers Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
@@ -56,46 +56,46 @@
 `cookies.json` in the argument `cookie_path` like this: ```python bot = await
 Chatbot.create(cookie_path='./cookies.json') ``` - Pass in the cookies directly
 by the argument `cookies`, like this: ```python with open('./cookies.json',
 'r') as f: cookies = json.load(f) bot = await Chatbot.create(cookies=cookies)
 ``` Use Async for the best experience, for example: ```python import asyncio
 from EdgeGPT import Chatbot, ConversationStyle async def main(): bot = await
 Chatbot.create() print(await bot.ask(prompt="Hello world",
-conversation_style=ConversationStyle.creative, wss_link="wss://sydney.bing.com/
-sydney/ChatHub")) await bot.close() if __name__ == "__main__": asyncio.run(main
-()) ```   ### 2) The `Query` and `Cookie` helper classes  Create a simple Bing
-Chat AI query (using the 'precise' conversation style by default) and see just
-the main text output rather than the whole API response: ```python from EdgeGPT
-import Query, Cookie q = Query("What are you? Give your answer as Python code")
-print(q) ``` Or change the conversation style or cookie file to be used:
-```python q = Query( "What are you? Give your answer as Python code",
-style="creative", # or 'balanced' cookies="./bing_cookies_alternative.json" )
-``` Quickly extract the text output, code snippets, list of sources/references,
-or suggested follow-on questions using the following attributes: ```python
-q.output q.code q.suggestions q.sources # for the full json output
-q.sources_dict # for a dictionary of titles and urls ``` Get the orginal prompt
-and the conversation style you specified: ```python q.prompt q.style repr(q)
-``` Access previous Queries made since importing `Query`: ```python Query.index
-# A list of Query objects; updated dynamically Query.request_count # A tally of
-requests made using each cookie file ``` And finally, the `Cookie` class
-supports multiple cookie files, so if you create additional cookie files with
-the naming convention `bing_cookies_*.json`, your queries will automatically
-try using the next file (alphabetically) if you've exceeded your daily quota of
-requests (currently set at 200). Here are the main attributes which you can
-access: ```python Cookie.current_file_index Cookie.dirpath
-Cookie.search_pattern # default is `bing_cookies_*.json` Cookie.files() # list
-as files that match .search_pattern Cookie.current_filepath Cookie.current_data
-Cookie.import_next() Cookie.image_token Cookie.ignore_files ```  --- ## Running
-with Docker This assumes you have a file cookies.json in your current working
-directory ``` bash docker run --rm -it -v $(pwd)/cookies.json:/cookies.json:ro
--e COOKIE_FILE='/cookies.json' ghcr.io/acheong08/edgegpt ``` You can add any
-extra flags as following ``` bash docker run --rm -it -v $(pwd)/cookies.json:/
-cookies.json:ro -e COOKIE_FILE='/cookies.json' ghcr.io/acheong08/edgegpt --rich
---style creative ```    # Image generator  ## Running from the Command Line
-```bash $ python3 -m ImageGen -h usage: ImageGen.py [-h] [-U U] [--cookie-file
+conversation_style=ConversationStyle.creative)) await bot.close() if __name__
+== "__main__": asyncio.run(main()) ```   ### 2) The `Query` and `Cookie` helper
+classes  Create a simple Bing Chat AI query (using the 'precise' conversation
+style by default) and see just the main text output rather than the whole API
+response: ```python from EdgeGPT import Query, Cookie q = Query("What are you?
+Give your answer as Python code") print(q) ``` Or change the conversation style
+or cookie file to be used: ```python q = Query( "What are you? Give your answer
+as Python code", style="creative", # or 'balanced' cookies="./
+bing_cookies_alternative.json" ) ``` Quickly extract the text output, code
+snippets, list of sources/references, or suggested follow-on questions using
+the following attributes: ```python q.output q.code q.suggestions q.sources #
+for the full json output q.sources_dict # for a dictionary of titles and urls
+``` Get the orginal prompt and the conversation style you specified: ```python
+q.prompt q.style repr(q) ``` Access previous Queries made since importing
+`Query`: ```python Query.index # A list of Query objects; updated dynamically
+Query.request_count # A tally of requests made using each cookie file ``` And
+finally, the `Cookie` class supports multiple cookie files, so if you create
+additional cookie files with the naming convention `bing_cookies_*.json`, your
+queries will automatically try using the next file (alphabetically) if you've
+exceeded your daily quota of requests (currently set at 200). Here are the main
+attributes which you can access: ```python Cookie.current_file_index
+Cookie.dirpath Cookie.search_pattern # default is `bing_cookies_*.json`
+Cookie.files() # list as files that match .search_pattern
+Cookie.current_filepath Cookie.current_data Cookie.import_next()
+Cookie.image_token Cookie.ignore_files ```  --- ## Running with Docker This
+assumes you have a file cookies.json in your current working directory ``` bash
+docker run --rm -it -v $(pwd)/cookies.json:/cookies.json:ro -e COOKIE_FILE='/
+cookies.json' ghcr.io/acheong08/edgegpt ``` You can add any extra flags as
+following ``` bash docker run --rm -it -v $(pwd)/cookies.json:/cookies.json:ro
+-e COOKIE_FILE='/cookies.json' ghcr.io/acheong08/edgegpt --rich --style
+creative ```    # Image generator  ## Running from the Command Line ```bash $
+python3 -m ImageGen -h usage: ImageGen.py [-h] [-U U] [--cookie-file
 COOKIE_FILE] --prompt PROMPT [--output-dir OUTPUT_DIR] [--quiet] [--asyncio]
 optional arguments: -h, --help show this help message and exit -U U Auth cookie
 from browser --cookie-file COOKIE_FILE File containing auth cookie --prompt
 PROMPT Prompt to generate images for --output-dir OUTPUT_DIR Output directory -
 -quiet Disable pipeline messages --asyncio Run ImageGen using asyncio ``` ##
 Running in Python ### 1) The `ImageQuery` helper class Generate images based on
 a simple prompt and download to the current working directory: ```python from
```

### Comparing `EdgeGPT-0.4.0/README.md` & `EdgeGPT-0.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -138,15 +138,15 @@
 
 ```python
 import asyncio
 from EdgeGPT import Chatbot, ConversationStyle
 
 async def main():
     bot = await Chatbot.create()
-    print(await bot.ask(prompt="Hello world", conversation_style=ConversationStyle.creative, wss_link="wss://sydney.bing.com/sydney/ChatHub"))
+    print(await bot.ask(prompt="Hello world", conversation_style=ConversationStyle.creative))
     await bot.close()
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 <details>
 <summary>
```

#### html2text {}

```diff
@@ -46,46 +46,46 @@
 `cookies.json` in the argument `cookie_path` like this: ```python bot = await
 Chatbot.create(cookie_path='./cookies.json') ``` - Pass in the cookies directly
 by the argument `cookies`, like this: ```python with open('./cookies.json',
 'r') as f: cookies = json.load(f) bot = await Chatbot.create(cookies=cookies)
 ``` Use Async for the best experience, for example: ```python import asyncio
 from EdgeGPT import Chatbot, ConversationStyle async def main(): bot = await
 Chatbot.create() print(await bot.ask(prompt="Hello world",
-conversation_style=ConversationStyle.creative, wss_link="wss://sydney.bing.com/
-sydney/ChatHub")) await bot.close() if __name__ == "__main__": asyncio.run(main
-()) ```   ### 2) The `Query` and `Cookie` helper classes  Create a simple Bing
-Chat AI query (using the 'precise' conversation style by default) and see just
-the main text output rather than the whole API response: ```python from EdgeGPT
-import Query, Cookie q = Query("What are you? Give your answer as Python code")
-print(q) ``` Or change the conversation style or cookie file to be used:
-```python q = Query( "What are you? Give your answer as Python code",
-style="creative", # or 'balanced' cookies="./bing_cookies_alternative.json" )
-``` Quickly extract the text output, code snippets, list of sources/references,
-or suggested follow-on questions using the following attributes: ```python
-q.output q.code q.suggestions q.sources # for the full json output
-q.sources_dict # for a dictionary of titles and urls ``` Get the orginal prompt
-and the conversation style you specified: ```python q.prompt q.style repr(q)
-``` Access previous Queries made since importing `Query`: ```python Query.index
-# A list of Query objects; updated dynamically Query.request_count # A tally of
-requests made using each cookie file ``` And finally, the `Cookie` class
-supports multiple cookie files, so if you create additional cookie files with
-the naming convention `bing_cookies_*.json`, your queries will automatically
-try using the next file (alphabetically) if you've exceeded your daily quota of
-requests (currently set at 200). Here are the main attributes which you can
-access: ```python Cookie.current_file_index Cookie.dirpath
-Cookie.search_pattern # default is `bing_cookies_*.json` Cookie.files() # list
-as files that match .search_pattern Cookie.current_filepath Cookie.current_data
-Cookie.import_next() Cookie.image_token Cookie.ignore_files ```  --- ## Running
-with Docker This assumes you have a file cookies.json in your current working
-directory ``` bash docker run --rm -it -v $(pwd)/cookies.json:/cookies.json:ro
--e COOKIE_FILE='/cookies.json' ghcr.io/acheong08/edgegpt ``` You can add any
-extra flags as following ``` bash docker run --rm -it -v $(pwd)/cookies.json:/
-cookies.json:ro -e COOKIE_FILE='/cookies.json' ghcr.io/acheong08/edgegpt --rich
---style creative ```    # Image generator  ## Running from the Command Line
-```bash $ python3 -m ImageGen -h usage: ImageGen.py [-h] [-U U] [--cookie-file
+conversation_style=ConversationStyle.creative)) await bot.close() if __name__
+== "__main__": asyncio.run(main()) ```   ### 2) The `Query` and `Cookie` helper
+classes  Create a simple Bing Chat AI query (using the 'precise' conversation
+style by default) and see just the main text output rather than the whole API
+response: ```python from EdgeGPT import Query, Cookie q = Query("What are you?
+Give your answer as Python code") print(q) ``` Or change the conversation style
+or cookie file to be used: ```python q = Query( "What are you? Give your answer
+as Python code", style="creative", # or 'balanced' cookies="./
+bing_cookies_alternative.json" ) ``` Quickly extract the text output, code
+snippets, list of sources/references, or suggested follow-on questions using
+the following attributes: ```python q.output q.code q.suggestions q.sources #
+for the full json output q.sources_dict # for a dictionary of titles and urls
+``` Get the orginal prompt and the conversation style you specified: ```python
+q.prompt q.style repr(q) ``` Access previous Queries made since importing
+`Query`: ```python Query.index # A list of Query objects; updated dynamically
+Query.request_count # A tally of requests made using each cookie file ``` And
+finally, the `Cookie` class supports multiple cookie files, so if you create
+additional cookie files with the naming convention `bing_cookies_*.json`, your
+queries will automatically try using the next file (alphabetically) if you've
+exceeded your daily quota of requests (currently set at 200). Here are the main
+attributes which you can access: ```python Cookie.current_file_index
+Cookie.dirpath Cookie.search_pattern # default is `bing_cookies_*.json`
+Cookie.files() # list as files that match .search_pattern
+Cookie.current_filepath Cookie.current_data Cookie.import_next()
+Cookie.image_token Cookie.ignore_files ```  --- ## Running with Docker This
+assumes you have a file cookies.json in your current working directory ``` bash
+docker run --rm -it -v $(pwd)/cookies.json:/cookies.json:ro -e COOKIE_FILE='/
+cookies.json' ghcr.io/acheong08/edgegpt ``` You can add any extra flags as
+following ``` bash docker run --rm -it -v $(pwd)/cookies.json:/cookies.json:ro
+-e COOKIE_FILE='/cookies.json' ghcr.io/acheong08/edgegpt --rich --style
+creative ```    # Image generator  ## Running from the Command Line ```bash $
+python3 -m ImageGen -h usage: ImageGen.py [-h] [-U U] [--cookie-file
 COOKIE_FILE] --prompt PROMPT [--output-dir OUTPUT_DIR] [--quiet] [--asyncio]
 optional arguments: -h, --help show this help message and exit -U U Auth cookie
 from browser --cookie-file COOKIE_FILE File containing auth cookie --prompt
 PROMPT Prompt to generate images for --output-dir OUTPUT_DIR Output directory -
 -quiet Disable pipeline messages --asyncio Run ImageGen using asyncio ``` ##
 Running in Python ### 1) The `ImageQuery` helper class Generate images based on
 a simple prompt and download to the current working directory: ```python from
```

### Comparing `EdgeGPT-0.4.0/setup.py` & `EdgeGPT-0.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="EdgeGPT",
-    version="0.4.0",
+    version="0.4.1",
     license="GNU General Public License v2.0",
     author="Antonio Cheong",
     author_email="acheong@student.dalat.org",
     description="Reverse engineered Edge Chat API",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/acheong08/EdgeGPT",
```

### Comparing `EdgeGPT-0.4.0/src/EdgeGPT.egg-info/PKG-INFO` & `EdgeGPT-0.4.1/src/EdgeGPT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdgeGPT
-Version: 0.4.0
+Version: 0.4.1
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/acheong08/EdgeGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
@@ -157,15 +157,15 @@
 
 ```python
 import asyncio
 from EdgeGPT import Chatbot, ConversationStyle
 
 async def main():
     bot = await Chatbot.create()
-    print(await bot.ask(prompt="Hello world", conversation_style=ConversationStyle.creative, wss_link="wss://sydney.bing.com/sydney/ChatHub"))
+    print(await bot.ask(prompt="Hello world", conversation_style=ConversationStyle.creative))
     await bot.close()
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 <details>
 <summary>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: EdgeGPT Version: 0.4.0 Summary: Reverse engineered
+Metadata-Version: 2.1 Name: EdgeGPT Version: 0.4.1 Summary: Reverse engineered
 Edge Chat API Home-page: https://github.com/acheong08/EdgeGPT Author: Antonio
 Cheong Author-email: acheong@student.dalat.org License: GNU General Public
 License v2.0 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/
 issues/new Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Intended Audience :: Developers Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
@@ -56,46 +56,46 @@
 `cookies.json` in the argument `cookie_path` like this: ```python bot = await
 Chatbot.create(cookie_path='./cookies.json') ``` - Pass in the cookies directly
 by the argument `cookies`, like this: ```python with open('./cookies.json',
 'r') as f: cookies = json.load(f) bot = await Chatbot.create(cookies=cookies)
 ``` Use Async for the best experience, for example: ```python import asyncio
 from EdgeGPT import Chatbot, ConversationStyle async def main(): bot = await
 Chatbot.create() print(await bot.ask(prompt="Hello world",
-conversation_style=ConversationStyle.creative, wss_link="wss://sydney.bing.com/
-sydney/ChatHub")) await bot.close() if __name__ == "__main__": asyncio.run(main
-()) ```   ### 2) The `Query` and `Cookie` helper classes  Create a simple Bing
-Chat AI query (using the 'precise' conversation style by default) and see just
-the main text output rather than the whole API response: ```python from EdgeGPT
-import Query, Cookie q = Query("What are you? Give your answer as Python code")
-print(q) ``` Or change the conversation style or cookie file to be used:
-```python q = Query( "What are you? Give your answer as Python code",
-style="creative", # or 'balanced' cookies="./bing_cookies_alternative.json" )
-``` Quickly extract the text output, code snippets, list of sources/references,
-or suggested follow-on questions using the following attributes: ```python
-q.output q.code q.suggestions q.sources # for the full json output
-q.sources_dict # for a dictionary of titles and urls ``` Get the orginal prompt
-and the conversation style you specified: ```python q.prompt q.style repr(q)
-``` Access previous Queries made since importing `Query`: ```python Query.index
-# A list of Query objects; updated dynamically Query.request_count # A tally of
-requests made using each cookie file ``` And finally, the `Cookie` class
-supports multiple cookie files, so if you create additional cookie files with
-the naming convention `bing_cookies_*.json`, your queries will automatically
-try using the next file (alphabetically) if you've exceeded your daily quota of
-requests (currently set at 200). Here are the main attributes which you can
-access: ```python Cookie.current_file_index Cookie.dirpath
-Cookie.search_pattern # default is `bing_cookies_*.json` Cookie.files() # list
-as files that match .search_pattern Cookie.current_filepath Cookie.current_data
-Cookie.import_next() Cookie.image_token Cookie.ignore_files ```  --- ## Running
-with Docker This assumes you have a file cookies.json in your current working
-directory ``` bash docker run --rm -it -v $(pwd)/cookies.json:/cookies.json:ro
--e COOKIE_FILE='/cookies.json' ghcr.io/acheong08/edgegpt ``` You can add any
-extra flags as following ``` bash docker run --rm -it -v $(pwd)/cookies.json:/
-cookies.json:ro -e COOKIE_FILE='/cookies.json' ghcr.io/acheong08/edgegpt --rich
---style creative ```    # Image generator  ## Running from the Command Line
-```bash $ python3 -m ImageGen -h usage: ImageGen.py [-h] [-U U] [--cookie-file
+conversation_style=ConversationStyle.creative)) await bot.close() if __name__
+== "__main__": asyncio.run(main()) ```   ### 2) The `Query` and `Cookie` helper
+classes  Create a simple Bing Chat AI query (using the 'precise' conversation
+style by default) and see just the main text output rather than the whole API
+response: ```python from EdgeGPT import Query, Cookie q = Query("What are you?
+Give your answer as Python code") print(q) ``` Or change the conversation style
+or cookie file to be used: ```python q = Query( "What are you? Give your answer
+as Python code", style="creative", # or 'balanced' cookies="./
+bing_cookies_alternative.json" ) ``` Quickly extract the text output, code
+snippets, list of sources/references, or suggested follow-on questions using
+the following attributes: ```python q.output q.code q.suggestions q.sources #
+for the full json output q.sources_dict # for a dictionary of titles and urls
+``` Get the orginal prompt and the conversation style you specified: ```python
+q.prompt q.style repr(q) ``` Access previous Queries made since importing
+`Query`: ```python Query.index # A list of Query objects; updated dynamically
+Query.request_count # A tally of requests made using each cookie file ``` And
+finally, the `Cookie` class supports multiple cookie files, so if you create
+additional cookie files with the naming convention `bing_cookies_*.json`, your
+queries will automatically try using the next file (alphabetically) if you've
+exceeded your daily quota of requests (currently set at 200). Here are the main
+attributes which you can access: ```python Cookie.current_file_index
+Cookie.dirpath Cookie.search_pattern # default is `bing_cookies_*.json`
+Cookie.files() # list as files that match .search_pattern
+Cookie.current_filepath Cookie.current_data Cookie.import_next()
+Cookie.image_token Cookie.ignore_files ```  --- ## Running with Docker This
+assumes you have a file cookies.json in your current working directory ``` bash
+docker run --rm -it -v $(pwd)/cookies.json:/cookies.json:ro -e COOKIE_FILE='/
+cookies.json' ghcr.io/acheong08/edgegpt ``` You can add any extra flags as
+following ``` bash docker run --rm -it -v $(pwd)/cookies.json:/cookies.json:ro
+-e COOKIE_FILE='/cookies.json' ghcr.io/acheong08/edgegpt --rich --style
+creative ```    # Image generator  ## Running from the Command Line ```bash $
+python3 -m ImageGen -h usage: ImageGen.py [-h] [-U U] [--cookie-file
 COOKIE_FILE] --prompt PROMPT [--output-dir OUTPUT_DIR] [--quiet] [--asyncio]
 optional arguments: -h, --help show this help message and exit -U U Auth cookie
 from browser --cookie-file COOKIE_FILE File containing auth cookie --prompt
 PROMPT Prompt to generate images for --output-dir OUTPUT_DIR Output directory -
 -quiet Disable pipeline messages --asyncio Run ImageGen using asyncio ``` ##
 Running in Python ### 1) The `ImageQuery` helper class Generate images based on
 a simple prompt and download to the current working directory: ```python from
```

### Comparing `EdgeGPT-0.4.0/src/EdgeGPT.py` & `EdgeGPT-0.4.1/src/EdgeGPT.py`

 * *Files 0% similar despite different names*

```diff
@@ -952,19 +952,14 @@
 
 class Query:
     """
     A convenience class that wraps around EdgeGPT.Chatbot to encapsulate input,
     config, and output all together.  Relies on Cookie class for authentication
     """
 
-    index = []
-    request_count = {}
-    image_dirpath = Path("./").resolve()
-    Cookie.import_data()
-
     def __init__(
         self,
         prompt,
         style="precise",
         content_type="text",
         cookie_file=0,
         echo=True,
@@ -976,15 +971,19 @@
         prompt: Text to enter into Bing Chat
         style: creative, balanced, or precise
         content_type: "text" for Bing Chat; "image" for Dall-e
         cookie_file: Path, filepath string, or index (int) to list of cookie paths
         echo: Print something to confirm request made
         echo_prompt: Print confirmation of the evaluated prompt
         """
-        self.__class__.index += [self]
+        self.index = []
+        self.request_count = {}
+        self.image_dirpath = Path("./").resolve()
+        Cookie.import_data()
+        self.index += [self]
         self.prompt = prompt
         files = Cookie.files()
         if isinstance(cookie_file, int):
             index = cookie_file if cookie_file < len(files) else 0
         else:
             if not isinstance(cookie_file, (str, Path)):
                 message = "'cookie_file' must be an int, str, or Path object"
@@ -1004,24 +1003,24 @@
             self.log_and_send_query(echo, echo_prompt)
         if content_type == "image":
             self.create_image()
 
     def log_and_send_query(self, echo, echo_prompt):
         self.response = asyncio.run(self.send_to_bing(echo, echo_prompt))
         name = str(Cookie.current_filepath.name)
-        if not self.__class__.request_count.get(name):
-            self.__class__.request_count[name] = 1
+        if not self.request_count.get(name):
+            self.request_count[name] = 1
         else:
-            self.__class__.request_count[name] += 1
+            self.request_count[name] += 1
 
     def create_image(self):
         image_generator = ImageGen(Cookie.image_token)
         image_generator.save_images(
             image_generator.get_images(self.prompt),
-            output_dir=self.__class__.image_dirpath,
+            output_dir=self.image_dirpath,
         )
 
     async def send_to_bing(self, echo=True, echo_prompt=False):
         """Creat, submit, then close a Chatbot instance.  Return the response"""
         retries = len(Cookie.files())
         while retries:
             try:
```

