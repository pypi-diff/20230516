# Comparing `tmp/tankioapi-0.1.2.tar.gz` & `tmp/tankioapi-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tankioapi-0.1.2.tar", last modified: Sun May 14 11:48:17 2023, max compression
+gzip compressed data, was "tankioapi-1.0.0.tar", last modified: Tue May 16 18:16:14 2023, max compression
```

## Comparing `tankioapi-0.1.2.tar` & `tankioapi-1.0.0.tar`

### file list

```diff
@@ -1,31 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 11:48:17.247064 tankioapi-0.1.2/
--rw-rw-rw-   0        0        0     1072 2023-05-13 16:20:18.000000 tankioapi-0.1.2/LICENSE
--rw-rw-rw-   0        0        0       89 2023-05-14 11:37:12.000000 tankioapi-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     4497 2023-05-14 11:48:17.244067 tankioapi-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     3116 2023-05-14 11:25:34.000000 tankioapi-0.1.2/README.md
--rw-rw-rw-   0        0        0     1959 2023-05-14 11:44:13.000000 tankioapi-0.1.2/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-14 11:48:17.182065 tankioapi-0.1.2/requirements/
--rw-rw-rw-   0        0        0       29 2023-05-14 11:20:40.000000 tankioapi-0.1.2/requirements/dev.txt
--rw-rw-rw-   0        0        0       24 2023-05-13 16:18:41.000000 tankioapi-0.1.2/requirements/speedup.txt
--rw-rw-rw-   0        0        0        7 2023-05-13 16:15:33.000000 tankioapi-0.1.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-14 11:48:17.248069 tankioapi-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     3784 2023-05-14 11:35:55.000000 tankioapi-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-14 11:48:17.152068 tankioapi-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-14 11:48:17.200064 tankioapi-0.1.2/src/tankioapi.egg-info/
--rw-rw-rw-   0        0        0     4497 2023-05-14 11:48:16.000000 tankioapi-0.1.2/src/tankioapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      584 2023-05-14 11:48:17.000000 tankioapi-0.1.2/src/tankioapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 11:48:16.000000 tankioapi-0.1.2/src/tankioapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2023-05-14 11:48:16.000000 tankioapi-0.1.2/src/tankioapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-14 11:48:16.000000 tankioapi-0.1.2/src/tankioapi.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-14 11:48:17.212068 tankioapi-0.1.2/src/toapi/
--rw-rw-rw-   0        0        0     1309 2023-05-14 11:47:09.000000 tankioapi-0.1.2/src/toapi/__init__.py
--rw-rw-rw-   0        0        0     5367 2023-05-14 11:02:57.000000 tankioapi-0.1.2/src/toapi/client.py
-drwxrwxrwx   0        0        0        0 2023-05-14 11:48:17.241065 tankioapi-0.1.2/src/toapi/dataclasses/
--rw-rw-rw-   0        0        0     1216 2023-05-13 20:00:35.000000 tankioapi-0.1.2/src/toapi/dataclasses/__init__.py
--rw-rw-rw-   0        0        0     4114 2023-05-14 10:07:07.000000 tankioapi-0.1.2/src/toapi/dataclasses/game_object.py
--rw-rw-rw-   0        0        0     2291 2023-05-13 20:14:00.000000 tankioapi-0.1.2/src/toapi/dataclasses/mode.py
--rw-rw-rw-   0        0        0     2010 2023-05-13 17:50:36.000000 tankioapi-0.1.2/src/toapi/dataclasses/rank.py
--rw-rw-rw-   0        0        0     2887 2023-05-14 09:45:15.000000 tankioapi-0.1.2/src/toapi/dataclasses/rating.py
--rw-rw-rw-   0        0        0     1487 2023-05-13 18:08:39.000000 tankioapi-0.1.2/src/toapi/dataclasses/top.py
--rw-rw-rw-   0        0        0     5855 2023-05-14 10:25:17.000000 tankioapi-0.1.2/src/toapi/dataclasses/user.py
--rw-rw-rw-   0        0        0     1609 2023-05-13 18:17:03.000000 tankioapi-0.1.2/src/toapi/errors.py
+drwxrwxrwx   0        0        0        0 2023-05-16 18:16:14.822874 tankioapi-1.0.0/
+-rw-rw-rw-   0        0        0     1072 2023-05-13 16:20:18.000000 tankioapi-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0      116 2023-05-15 17:49:50.000000 tankioapi-1.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4577 2023-05-16 18:16:14.821874 tankioapi-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3196 2023-05-16 18:15:16.000000 tankioapi-1.0.0/README.md
+-rw-rw-rw-   0        0        0     1977 2023-05-16 18:08:50.000000 tankioapi-1.0.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-16 18:16:14.632872 tankioapi-1.0.0/requirements/
+-rw-rw-rw-   0        0        0       29 2023-05-14 11:20:40.000000 tankioapi-1.0.0/requirements/dev.txt
+-rw-rw-rw-   0        0        0       24 2023-05-13 16:18:41.000000 tankioapi-1.0.0/requirements/speedup.txt
+-rw-rw-rw-   0        0        0        7 2023-05-13 16:15:33.000000 tankioapi-1.0.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-16 18:16:14.822874 tankioapi-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     3776 2023-05-16 17:56:05.000000 tankioapi-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 18:16:14.552872 tankioapi-1.0.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-16 18:16:14.745872 tankioapi-1.0.0/src/tankioapi.egg-info/
+-rw-rw-rw-   0        0        0     4577 2023-05-16 18:16:14.000000 tankioapi-1.0.0/src/tankioapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      686 2023-05-16 18:16:14.000000 tankioapi-1.0.0/src/tankioapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 18:16:14.000000 tankioapi-1.0.0/src/tankioapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2023-05-16 18:16:14.000000 tankioapi-1.0.0/src/tankioapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-16 18:16:14.000000 tankioapi-1.0.0/src/tankioapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 18:16:14.758871 tankioapi-1.0.0/src/toapi/
+-rw-rw-rw-   0        0        0     1303 2023-05-16 18:09:30.000000 tankioapi-1.0.0/src/toapi/__init__.py
+-rw-rw-rw-   0        0        0     3674 2023-05-16 18:07:42.000000 tankioapi-1.0.0/src/toapi/client.py
+drwxrwxrwx   0        0        0        0 2023-05-16 18:16:14.779873 tankioapi-1.0.0/src/toapi/data/
+-rw-rw-rw-   0        0        0     1132 2023-05-16 17:39:09.000000 tankioapi-1.0.0/src/toapi/data/__init__.py
+-rw-rw-rw-   0        0        0     3272 2023-05-15 19:06:28.000000 tankioapi-1.0.0/src/toapi/data/ranks.py
+-rw-rw-rw-   0        0        0     2524 2023-05-16 17:38:18.000000 tankioapi-1.0.0/src/toapi/data/test_server.py
+-rw-rw-rw-   0        0        0     1609 2023-05-13 18:17:03.000000 tankioapi-1.0.0/src/toapi/errors.py
+-rw-rw-rw-   0        0        0     2577 2023-05-16 17:56:05.000000 tankioapi-1.0.0/src/toapi/http.py
+-rw-rw-rw-   0        0        0        0 2023-05-15 17:51:02.000000 tankioapi-1.0.0/src/toapi/py.typed
+drwxrwxrwx   0        0        0        0 2023-05-16 18:16:14.817871 tankioapi-1.0.0/src/toapi/types/
+-rw-rw-rw-   0        0        0     1239 2023-05-15 20:04:05.000000 tankioapi-1.0.0/src/toapi/types/__init__.py
+-rw-rw-rw-   0        0        0     5845 2023-05-16 17:56:05.000000 tankioapi-1.0.0/src/toapi/types/game_object.py
+-rw-rw-rw-   0        0        0     2910 2023-05-16 17:56:05.000000 tankioapi-1.0.0/src/toapi/types/mode.py
+-rw-rw-rw-   0        0        0     2567 2023-05-16 17:56:05.000000 tankioapi-1.0.0/src/toapi/types/rank.py
+-rw-rw-rw-   0        0        0     3148 2023-05-15 19:06:18.000000 tankioapi-1.0.0/src/toapi/types/rating.py
+-rw-rw-rw-   0        0        0     7032 2023-05-16 17:56:05.000000 tankioapi-1.0.0/src/toapi/types/status.py
+-rw-rw-rw-   0        0        0     3523 2023-05-15 19:23:46.000000 tankioapi-1.0.0/src/toapi/types/top.py
+-rw-rw-rw-   0        0        0     8211 2023-05-15 19:36:53.000000 tankioapi-1.0.0/src/toapi/types/user.py
```

### Comparing `tankioapi-0.1.2/LICENSE` & `tankioapi-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tankioapi-0.1.2/PKG-INFO` & `tankioapi-1.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: tankioapi
-Version: 0.1.2
+Version: 1.0.0
 Summary: A Python written wrapper for the Tanki Online game API
 Home-page: https://github.com/stngularity/tankioapi.py
 Author: stngularity
 Author-email: stngularity <stngularity@gmail.com>
 License: MIT License
-Project-URL: homepage, https://github.com/stngularity/tankioapi
+Project-URL: Homepage, https://github.com/stngularity/tankioapi
 Project-URL: Source Code, https://github.com/stngularity/tankioapi
-Project-URL: changelog, https://github.com/stngularity/tankioapi/blob/main/CHANGELOG.md
+Project-URL: Changelog, https://github.com/stngularity/tankioapi/blob/main/CHANGELOG.md
 Project-URL: Bug Tracker, https://github.com/stngularity/tankioapi/issues
 Keywords: game,api,to,tanki online
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -43,17 +43,19 @@
 ## Notification
 This project was created just to exist. Of course, I will update it when the API itself changes, but not immediately. Well, if You want to support this project, You can give it a star.
 
 ## Information
 As mentioned earlier, this project is created just to exist. And so, the module itself is needed to get the top of players and get information about the player separately. If You know more functionality of the API of the game `Tanki Online`, then please report this functionality in the [`Issues`](https://github.com/stngularity/tankioapi/issues).
 
 ###### Features
-- `async`/`await` support
+- Fully `async`/`await`
 - Getting top of players
 - Getting information of any player by him name
+- Getting status of stable server `Maybe deprecated`
+- Getting status of test servers
 
 ## Installing
 **[Python 3.8](https://www.python.org/downloads/) or higher is required**
 
 To install a non-`speedup` version of the library, do the following:
 > ```sh
 > # Linux/macOS
@@ -81,39 +83,39 @@
 
 ## Examples
 Here are examples of some of the features of the library. More examples in [`examples/`](/examples)
 
 ###### Getting all tops of players
 ```py
 import asyncio
-from toapi import TankiOnline
+from toapi import Top, TopLists, get_tops
 
-tops = asyncio.run(TankiOnline.get_tops())
-for top in tops.values():
-    print(f"----- {top.name} -----")
-    for number, user in enumerate(top.users):
-        print(f"#{number+1}   {user.name} ({user.top_value})")
 
-    print()
+tops: TopLists = asyncio.run(get_tops())
+efficiency_top: Top = tops.efficiency
+print("----- Efficiency top -----")
+for number, user in enumerate(efficiency_top.users):
+    print(f"#{number+1}   {user.name} ({user.top_value})")
 ```
 
 ###### Getting information of player
 ```py
 import asyncio
-from toapi import TankiOnline
+from toapi import User, get_user
 
-user = asyncio.run(TankiOnline.get_user("sty"))
+user = asyncio.run(get_user("sty"))
 # and You can specify language
-# user = asyncio.run(TankiOnline.get_user("sty", lang="ru"))
+# user = asyncio.run(get_user("sty", lang="ru"))
 
 print(f"Name: {user.name}")
-print(f"Rank: #{user.rank.number} ({user.score}/{user.score_next} {round(user.score/user.score_next*100)}%)")
+rank: str = user.rank.name.title()
+print(f"Rank: {rank} ({user.score}/{user.score_next} {round(user.score/user.score_next*100)}%)")
 print(f"Has premium: {'Yes' if user.premium else 'No'}")
 print()
-print(f"KD: {user.kills}/{user.deaths} ({round(user.kills/user.deaths, 2)})")
+print(f"KD: {user.kills}/{user.deaths} ({user.kd_ratio})")
 print(f"Caught golds: {user.caught_golds}")
 print(f"Crystals: {user.crystals}")
 print(f"GS: {user.gear_score}")
 ```
 
 ## License
 This project is distributed under the `MIT` license. You can learn more from the [**LICENSE**](/LICENSE) file.
```

### Comparing `tankioapi-0.1.2/README.md` & `tankioapi-1.0.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -11,17 +11,19 @@
 ## Notification
 This project was created just to exist. Of course, I will update it when the API itself changes, but not immediately. Well, if You want to support this project, You can give it a star.
 
 ## Information
 As mentioned earlier, this project is created just to exist. And so, the module itself is needed to get the top of players and get information about the player separately. If You know more functionality of the API of the game `Tanki Online`, then please report this functionality in the [`Issues`](https://github.com/stngularity/tankioapi/issues).
 
 ###### Features
-- `async`/`await` support
+- Fully `async`/`await`
 - Getting top of players
 - Getting information of any player by him name
+- Getting status of stable server `Maybe deprecated`
+- Getting status of test servers
 
 ## Installing
 **[Python 3.8](https://www.python.org/downloads/) or higher is required**
 
 To install a non-`speedup` version of the library, do the following:
 > ```sh
 > # Linux/macOS
@@ -49,39 +51,39 @@
 
 ## Examples
 Here are examples of some of the features of the library. More examples in [`examples/`](/examples)
 
 ###### Getting all tops of players
 ```py
 import asyncio
-from toapi import TankiOnline
+from toapi import Top, TopLists, get_tops
 
-tops = asyncio.run(TankiOnline.get_tops())
-for top in tops.values():
-    print(f"----- {top.name} -----")
-    for number, user in enumerate(top.users):
-        print(f"#{number+1}   {user.name} ({user.top_value})")
 
-    print()
+tops: TopLists = asyncio.run(get_tops())
+efficiency_top: Top = tops.efficiency
+print("----- Efficiency top -----")
+for number, user in enumerate(efficiency_top.users):
+    print(f"#{number+1}   {user.name} ({user.top_value})")
 ```
 
 ###### Getting information of player
 ```py
 import asyncio
-from toapi import TankiOnline
+from toapi import User, get_user
 
-user = asyncio.run(TankiOnline.get_user("sty"))
+user = asyncio.run(get_user("sty"))
 # and You can specify language
-# user = asyncio.run(TankiOnline.get_user("sty", lang="ru"))
+# user = asyncio.run(get_user("sty", lang="ru"))
 
 print(f"Name: {user.name}")
-print(f"Rank: #{user.rank.number} ({user.score}/{user.score_next} {round(user.score/user.score_next*100)}%)")
+rank: str = user.rank.name.title()
+print(f"Rank: {rank} ({user.score}/{user.score_next} {round(user.score/user.score_next*100)}%)")
 print(f"Has premium: {'Yes' if user.premium else 'No'}")
 print()
-print(f"KD: {user.kills}/{user.deaths} ({round(user.kills/user.deaths, 2)})")
+print(f"KD: {user.kills}/{user.deaths} ({user.kd_ratio})")
 print(f"Caught golds: {user.caught_golds}")
 print(f"Crystals: {user.crystals}")
 print(f"GS: {user.gear_score}")
 ```
 
 ## License
 This project is distributed under the `MIT` license. You can learn more from the [**LICENSE**](/LICENSE) file.
```

### Comparing `tankioapi-0.1.2/pyproject.toml` & `tankioapi-1.0.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # The configuration of project
 [build-system]
-requires = ["setuptools"]
+requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tankioapi"
 authors = [{name = "stngularity", email = "stngularity@gmail.com"}]
 description = "A Python written wrapper for the Tanki Online game API"
 readme = "README.md"
@@ -25,17 +25,17 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Utilities",
     "Typing :: Typed"
 ]
 
 [project.urls]
-homepage = "https://github.com/stngularity/tankioapi"
+"Homepage"    = "https://github.com/stngularity/tankioapi"
 "Source Code" = "https://github.com/stngularity/tankioapi"
-changelog = "https://github.com/stngularity/tankioapi/blob/main/CHANGELOG.md"
+"Changelog"   = "https://github.com/stngularity/tankioapi/blob/main/CHANGELOG.md"
 "Bug Tracker" = "https://github.com/stngularity/tankioapi/issues"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 include = ["toapi*"]
 namespaces = false
```

### Comparing `tankioapi-0.1.2/setup.py` & `tankioapi-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE."""
 
 import re
-from setuptools import setup, find_packages
+
+from setuptools import find_packages, setup
+
 
 def read_requirements(file):
     """List[:class:`str`]: Reads specified in :param:`file` requirements
     
     Parameters
     ----------
     file: :class:`str`
@@ -43,18 +45,18 @@
 
         description="A Python written wrapper for the Tanki Online game API",
         long_description=README,
         long_description_content_type="text/markdown",
 
         url="https://github.com/stngularity/tankioapi.py",
         project_urls={
-            "Homepage": "https://github.com/stngularity/tankioapi.py",
-            "Source Code": "https://github.com/stngularity/tankioapi.py",
-            "Changelog": "https://github.com/stngularity/tankioapi.py/blob/main/CHANGELOG.md",
-            "Bug Tracker": "https://github.com/stngularity/tankioapi.py/issues"
+            "Homepage": "https://github.com/stngularity/tankioapi",
+            "Source Code": "https://github.com/stngularity/tankioapi",
+            "Changelog": "https://github.com/stngularity/tankioapi/blob/main/CHANGELOG.md",
+            "Bug Tracker": "https://github.com/stngularity/tankioapi/issues"
         },
 
         python_requires=">=3.8",
         install_requires=read_requirements("requirements.txt"),
         extras_require={
             "speedup": read_requirements("requirements/speedup.txt"),
             "dev": read_requirements("requirements/dev.txt")
```

### Comparing `tankioapi-0.1.2/src/tankioapi.egg-info/PKG-INFO` & `tankioapi-1.0.0/src/tankioapi.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: tankioapi
-Version: 0.1.2
+Version: 1.0.0
 Summary: A Python written wrapper for the Tanki Online game API
 Home-page: https://github.com/stngularity/tankioapi.py
 Author: stngularity
 Author-email: stngularity <stngularity@gmail.com>
 License: MIT License
-Project-URL: homepage, https://github.com/stngularity/tankioapi
+Project-URL: Homepage, https://github.com/stngularity/tankioapi
 Project-URL: Source Code, https://github.com/stngularity/tankioapi
-Project-URL: changelog, https://github.com/stngularity/tankioapi/blob/main/CHANGELOG.md
+Project-URL: Changelog, https://github.com/stngularity/tankioapi/blob/main/CHANGELOG.md
 Project-URL: Bug Tracker, https://github.com/stngularity/tankioapi/issues
 Keywords: game,api,to,tanki online
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -43,17 +43,19 @@
 ## Notification
 This project was created just to exist. Of course, I will update it when the API itself changes, but not immediately. Well, if You want to support this project, You can give it a star.
 
 ## Information
 As mentioned earlier, this project is created just to exist. And so, the module itself is needed to get the top of players and get information about the player separately. If You know more functionality of the API of the game `Tanki Online`, then please report this functionality in the [`Issues`](https://github.com/stngularity/tankioapi/issues).
 
 ###### Features
-- `async`/`await` support
+- Fully `async`/`await`
 - Getting top of players
 - Getting information of any player by him name
+- Getting status of stable server `Maybe deprecated`
+- Getting status of test servers
 
 ## Installing
 **[Python 3.8](https://www.python.org/downloads/) or higher is required**
 
 To install a non-`speedup` version of the library, do the following:
 > ```sh
 > # Linux/macOS
@@ -81,39 +83,39 @@
 
 ## Examples
 Here are examples of some of the features of the library. More examples in [`examples/`](/examples)
 
 ###### Getting all tops of players
 ```py
 import asyncio
-from toapi import TankiOnline
+from toapi import Top, TopLists, get_tops
 
-tops = asyncio.run(TankiOnline.get_tops())
-for top in tops.values():
-    print(f"----- {top.name} -----")
-    for number, user in enumerate(top.users):
-        print(f"#{number+1}   {user.name} ({user.top_value})")
 
-    print()
+tops: TopLists = asyncio.run(get_tops())
+efficiency_top: Top = tops.efficiency
+print("----- Efficiency top -----")
+for number, user in enumerate(efficiency_top.users):
+    print(f"#{number+1}   {user.name} ({user.top_value})")
 ```
 
 ###### Getting information of player
 ```py
 import asyncio
-from toapi import TankiOnline
+from toapi import User, get_user
 
-user = asyncio.run(TankiOnline.get_user("sty"))
+user = asyncio.run(get_user("sty"))
 # and You can specify language
-# user = asyncio.run(TankiOnline.get_user("sty", lang="ru"))
+# user = asyncio.run(get_user("sty", lang="ru"))
 
 print(f"Name: {user.name}")
-print(f"Rank: #{user.rank.number} ({user.score}/{user.score_next} {round(user.score/user.score_next*100)}%)")
+rank: str = user.rank.name.title()
+print(f"Rank: {rank} ({user.score}/{user.score_next} {round(user.score/user.score_next*100)}%)")
 print(f"Has premium: {'Yes' if user.premium else 'No'}")
 print()
-print(f"KD: {user.kills}/{user.deaths} ({round(user.kills/user.deaths, 2)})")
+print(f"KD: {user.kills}/{user.deaths} ({user.kd_ratio})")
 print(f"Caught golds: {user.caught_golds}")
 print(f"Crystals: {user.crystals}")
 print(f"GS: {user.gear_score}")
 ```
 
 ## License
 This project is distributed under the `MIT` license. You can learn more from the [**LICENSE**](/LICENSE) file.
```

### Comparing `tankioapi-0.1.2/src/tankioapi.egg-info/SOURCES.txt` & `tankioapi-1.0.0/src/tankioapi.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -10,14 +10,20 @@
 src/tankioapi.egg-info/SOURCES.txt
 src/tankioapi.egg-info/dependency_links.txt
 src/tankioapi.egg-info/requires.txt
 src/tankioapi.egg-info/top_level.txt
 src/toapi/__init__.py
 src/toapi/client.py
 src/toapi/errors.py
-src/toapi/dataclasses/__init__.py
-src/toapi/dataclasses/game_object.py
-src/toapi/dataclasses/mode.py
-src/toapi/dataclasses/rank.py
-src/toapi/dataclasses/rating.py
-src/toapi/dataclasses/top.py
-src/toapi/dataclasses/user.py
+src/toapi/http.py
+src/toapi/py.typed
+src/toapi/data/__init__.py
+src/toapi/data/ranks.py
+src/toapi/data/test_server.py
+src/toapi/types/__init__.py
+src/toapi/types/game_object.py
+src/toapi/types/mode.py
+src/toapi/types/rank.py
+src/toapi/types/rating.py
+src/toapi/types/status.py
+src/toapi/types/top.py
+src/toapi/types/user.py
```

### Comparing `tankioapi-0.1.2/src/toapi/__init__.py` & `tankioapi-1.0.0/src/toapi/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE."""
 
-from .dataclasses import *
 from .client import *
 from .errors import *
+from .types import *
 
 __name__ = "tankio_api"
 __author__ = "stngularity"
 __license__ = "MIT"
 __copyright__ = "Copyright 2023-present stngularity"
-__version__ = "0.1.2"
+__version__ = "1.0.0"
```

### Comparing `tankioapi-0.1.2/src/toapi/dataclasses/__init__.py` & `tankioapi-1.0.0/src/toapi/types/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,9 +6,10 @@
 
 THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE."""
 
 from .game_object import *
 from .mode import *
 from .rank import *
 from .rating import *
+from .status import *
 from .top import *
 from .user import *
```

### Comparing `tankioapi-0.1.2/src/toapi/dataclasses/game_object.py` & `tankioapi-1.0.0/src/toapi/types/game_object.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,24 +2,62 @@
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE."""
 
-from datetime import timedelta as td
+# pylint: disable=C0103
+
 from dataclasses import dataclass
-from typing import Any, Dict, List, Optional
+from datetime import timedelta as td
+from typing import Any, List, Mapping, Optional, Type
+
+from ..http import request_bytes
 
 __all__ = ("GameObject", "SuppliesObject")
 
 
 @dataclass
-class GameObject:
-    """The dataclass of the object from Tanki Online
+class BaseGameObject:
+    """The base dataclass for the objects from Tanki Online
+    
+    Attributes
+    ----------
+    id: :class:`int`
+        The ID of the game's object
+        
+    image: :class:`str`
+        The URL to the image of this object. The image is `.tnk` file, but
+        it's possible to render as `.png`
+        
+    name: :class:`str`
+        The name of the object"""
+
+    id: int
+    image: str
+    name: str
+
+    def __repr__(self) -> str:
+        return f"{self.__class__.__name__}(id={self.id}, name=\"{self.name}\")"
+
+    def __str__(self) -> str:
+        return self.name
+    
+    def __hash__(self) -> int:
+        return hash(self.id)
+
+    async def read_image(self) -> bytes:
+        """:class:`bytes`: Reads the image data of this object and returns it"""
+        return await request_bytes("GET", self.image)
+
+
+@dataclass
+class GameObject(BaseGameObject):
+    """The dataclass for the objects from Tanki Online
     
     Attributes
     ----------
     grade: :class:`int`
         The level of the object (Mk-`N`, where `N` is the level). If the
         object doesn't have such a property (that's, our object is a drone
         or paint), then it's equal to `-1`
@@ -41,43 +79,50 @@
         The count of experience points that were earned when the player
         played with this object
         
     time_played: :class:`timedelta`
         The time in the game that was spent with these objects"""
 
     grade: int
-    id: int
-    image: str
-    name: str
     properties: Optional[List[str]]
     score_earned: int
     time_played: td
 
+    @classmethod
+    def from_json(cls: Type["GameObject"], data: Mapping[str, Any]) -> "GameObject":
+        """:class:`GameObject`: Converts JSON data to :class:`GameObject`
+        
+        Parameters
+        ----------
+        data: Mapping[:class:`str`, :class:`Any`]
+            The JSON data"""
+        self = cls.__new__(cls)
+        self.grade = data["grade"] + 1
+        self.id = data["id"]
+        self.image = data["imageUrl"]
+        self.name = data["name"]
+        self.properties = data["properties"]
+        self.score_earned = data["scoreEarned"]
+        self.time_played = td(seconds=data["timePlayed"])
+        return self
+
     @staticmethod
-    def from_list(list: List[Dict[str, Any]]) -> List["GameObject"]:
+    def from_list(list: List[Mapping[str, Any]]) -> List["GameObject"]:
         """List[:class:`GameObject`]: Converts list to list with game's object
         
         Parameters
         ----------
-        list: List[Dict[:class:`str`, :class:`Any`]]
-            The list with dicionaries"""
-        return [GameObject(
-            grade=x["grade"]+1,
-            id=x["id"],
-            image=x["imageUrl"],
-            name=x["name"],
-            properties=x["properties"],
-            score_earned=x["scoreEarned"],
-            time_played=td(seconds=x["timePlayed"])
-        ) for x in list]
+        list: List[Mapping[:class:`str`, :class:`Any`]]
+            The list with dictionaries"""
+        return [GameObject.from_json(x) for x in list]
 
 
 @dataclass
-class SuppliesObject:
-    """The dataclass of the supplies object from Tanki Online
+class SuppliesObject(BaseGameObject):
+    """The dataclass for the supplies objects from Tanki Online
     
     Attributes
     ----------
     id: :class:`int`
         The ID of the game's object
         
     image: :class:`str`
@@ -86,26 +131,33 @@
         
     name: :class:`str`
         The name of the object
         
     usages: :class:`int`
         The count of these supplies usages"""
 
-    id: int
-    image: str
-    name: str
     usages: int
 
+    @classmethod
+    def from_json(cls: Type["SuppliesObject"], data: Mapping[str, Any]) -> "SuppliesObject":
+        """:class:`SuppliesObject`: Converts JSON data to :class:`SuppliesObject`
+        
+        Parameters
+        ----------
+        data: Mapping[:class:`str`, :class:`Any`]
+            The JSON data"""
+        self = cls.__new__(cls)
+        self.id = data["id"]
+        self.image = data["imageUrl"]
+        self.name = data["name"]
+        self.usages = data["usages"]
+        return self
+
     @staticmethod
-    def from_list(list: List[Dict[str, Any]]) -> List["SuppliesObject"]:
+    def from_list(list: List[Mapping[str, Any]]) -> List["SuppliesObject"]:
         """List[:class:`SuppliesObject`]: Converts list to list with supplies
         
         Parameters
         ----------
-        list: List[Dict[:class:`str`, :class:`Any`]]
+        list: List[Mapping[:class:`str`, :class:`Any`]]
             The list with dicionaries"""
-        return [SuppliesObject(
-            id=x["id"],
-            image=x["imageUrl"],
-            name=x["name"],
-            usages=x["usages"]
-        ) for x in list]
+        return [SuppliesObject.from_json(x) for x in list]
```

### Comparing `tankioapi-0.1.2/src/toapi/dataclasses/mode.py` & `tankioapi-1.0.0/src/toapi/errors.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,52 +2,26 @@
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE."""
 
-from datetime import timedelta as td
-from dataclasses import dataclass
-from typing import Any, Dict, List
+__all__ = ("TankiOnlineException", "UserNotFoundError")
 
-__all__ = ("Mode",)
 
+class TankiOnlineException(Exception):
+    """The class of Tanki Online's API exceptions"""
+    ...
 
-@dataclass
-class Mode:
-    """The dataclass for the game modes
+
+class UserNotFoundError(TankiOnlineException):
+    """The class for "Could not find user" errors
     
     Attributes
     ----------
-    name: :class:`str`
-        The name of the mode
-        
-    score_earned: :class:`int`
-        The count of experience points that were earned when the player
-        played in this mode
-        
-    time_played: :class:`timedelta`
-        The time in the game that was spent in this mode
-        
-    type: :class:`str`
-        The short name of the mode"""
-
-    name: str
-    score_earned: int
-    time_played: td
-    type: str
-
-    @staticmethod
-    def from_list(list: List[Dict[str, Any]]) -> List["Mode"]:
-        """List[:class:`Mode`]: Converts list to list with game's object
-        
-        Parameters
-        ----------
-        list: List[Dict[:class:`str`, :class:`Any`]]
-            The list with dicionaries"""
-        return [Mode(
-            name=x["name"].strip(),
-            score_earned=x["scoreEarned"],
-            time_played=td(seconds=x["timePlayed"]),
-            type=x["type"]
-        ) for x in list]
+    username: :class:`str`
+        The name of the user which you tried to find"""
+
+    def __init__(self, username: str, *args: object) -> None:
+        self.username: str = username
+        super().__init__(*args)
```

### Comparing `tankioapi-0.1.2/src/toapi/dataclasses/rank.py` & `tankioapi-1.0.0/src/toapi/types/rank.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE."""
 
 from dataclasses import dataclass
+from typing import Union
+
+from ..data import get_rank_name
 
 __all__ = ("Rank",)
 
 
 @dataclass
 class Rank:
     """The dataclass of user rank
@@ -24,19 +27,36 @@
     legend_number: :class:`int`
         Only if player has `Legend` rank! The number of `Legend` rank"""
 
     number: int
 
     @property
     def legend_number(self) -> int:
-        """:class:`int`: if the player has the `Legend` rank, then returns
+        """:class:`int`: If the player has the `Legend` rank, then returns
         the number of this rank, otherwise returns `-1`"""
         return -1 if self.number < 31 else self.number-30
 
+    @property
+    def name(self) -> str:
+        """:class:`str`: The name of player's rank"""
+        return get_rank_name(self.number)
+
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(number={self.number})"
 
     def __str__(self) -> str:
-        return f"Rank #{self.number}"
+        return self.name
 
     def __hash__(self) -> int:
         return hash(self.number)
+
+    def __eq__(self, other: Union[int, "Rank"]) -> bool:
+        if isinstance(other, int) and other == self.number:
+            return True
+
+        if isinstance(other, Rank) and other.number == self.number:
+            return True
+
+        return False
+
+    def __ne__(self, other: Union[int, "Rank"]) -> bool:
+        return not self.__eq__(other)
```

### Comparing `tankioapi-0.1.2/src/toapi/dataclasses/rating.py` & `tankioapi-1.0.0/src/toapi/types/rating.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,14 +24,23 @@
     value: :class:`int`
         The value of characteristic of the player, according to which the
         top was compiled"""
 
     position: int
     value: int
 
+    def __repr__(self) -> str:
+        return f"{self.__class__.__name__}(position={self.position}, value={self.value})"
+
+    def __str__(self) -> str:
+        return f"#{self.position}"
+
+    def __hash__(self) -> int:
+        return hash(self.value)
+
 
 @dataclass
 class Ratings:
     """The dataclass for the player's ratings
     
     Attributes
     ----------
```

### Comparing `tankioapi-0.1.2/src/toapi/dataclasses/user.py` & `tankioapi-1.0.0/src/toapi/types/user.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE."""
 
 from dataclasses import dataclass
-from typing import Any, Dict, List
+from typing import Any, Dict, List, Mapping, Type
 
 from .game_object import GameObject, SuppliesObject
 from .mode import Mode
 from .rank import Rank
 from .rating import Ratings
 
 __all__ = ("PartialUser", "TopListUser", "User")
@@ -45,15 +45,15 @@
     def __hash__(self) -> int:
         return hash(self.name + str(self.rank.number))
 
     def __eq__(self, other: object) -> bool:
         return isinstance(other, PartialUser) and other.name == self.name
 
     def __ne__(self, other: object) -> bool:
-        return not isinstance(other, PartialUser) or other.name != self.name
+        return not self.__eq__(other)
 
 
 @dataclass
 class TopListUser(PartialUser):
     """The dataclass of user from a top
     
     Attributes
@@ -73,14 +73,33 @@
     top_value: :class:`int`
         The value of the characteristic of this player, according to which
         the :attr:`top` was compiled"""
 
     top: str
     top_value: int
 
+    @classmethod
+    def from_json(cls: Type["TopListUser"], data: Mapping[str, Any], *, top: str) -> "TopListUser":
+        """:class:`TopListUser`: Converts JSON data to :class:`TopListUser`
+        
+        Parameters
+        ----------
+        data: Mapping[:class:`str`, :class:`Any`]
+            The JSON data
+            
+        top: :class:`str`
+            The name of the top which this player from"""
+        self = cls.__new__(cls)
+        self.name = data["uid"]
+        self.rank = Rank(data["rank"])
+        self.premium = data["hasPremium"]
+        self.top = top
+        self.top_value = data["value"]
+        return self
+
 
 @dataclass
 class User(PartialUser):
     """The dataclass of user from a top
     
     Attributes
     ----------
@@ -168,7 +187,45 @@
     rating: Ratings
     resistance_modules: List[GameObject]
     score: int
     score_base: int
     score_next: int
     supplies_usage: List[SuppliesObject]
     turrets_played: List[GameObject]
+
+    @property
+    def kd_ratio(self) -> float:
+        """:class:`float`: Kill/death ratio of this player. The bigger, the better"""
+        return round(self.kills/self.deaths, 2)
+
+    @classmethod
+    def from_json(cls: Type["User"], data: Mapping[str, Any]) -> "User":
+        """:class:`User`: Converts JSON data to :class:`User`
+        
+        Parameters
+        ----------
+        data: Mapping[:class:`str`, :class:`Any`]
+            The JSON data"""
+        self = cls.__new__(cls)
+        self.name = data["name"]
+        self.rank = Rank(data["rank"])
+        self.premium = data["hasPremium"]
+        self.kills = data["kills"]
+        self.deaths = data["deaths"]
+        self.caught_golds = data["caughtGolds"]
+        self.drones_played = GameObject.from_list(data["dronesPlayed"])
+        self.crystals = data["earnedCrystals"]
+        self.gear_score = data["gearScore"]
+        self.hulls_played = GameObject.from_list(data["hullsPlayed"])
+        self.modes_played = Mode.from_list(data["modesPlayed"])
+        self.mounted = data["mounted"]
+        self.paints_played = GameObject.from_list(data["paintsPlayed"])
+        self.presents = data["presents"]
+        self.previous_rating = Ratings.from_json(data["previousRating"])
+        self.rating = Ratings.from_json(data["rating"])
+        self.resistance_modules = GameObject.from_list(data["resistanceModules"])
+        self.score = data["score"]
+        self.score_base = data["scoreBase"]
+        self.score_next = data["scoreNext"]
+        self.supplies_usage = SuppliesObject.from_list(data["suppliesUsage"])
+        self.turrets_played = GameObject.from_list(data["turretsPlayed"])
+        return self
```

