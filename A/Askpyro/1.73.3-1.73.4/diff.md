# Comparing `tmp/Askpyro-1.73.3.tar.gz` & `tmp/Askpyro-1.73.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Askpyro-1.73.3.tar", last modified: Thu Apr 27 15:34:30 2023, max compression
+gzip compressed data, was "Askpyro-1.73.4.tar", last modified: Tue May 16 18:48:45 2023, max compression
```

## Comparing `Askpyro-1.73.3.tar` & `Askpyro-1.73.4.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 15:34:30.005124 Askpyro-1.73.3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 15:34:30.001124 Askpyro-1.73.3/Askpyro.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4433 2023-04-27 15:34:29.000000 Askpyro-1.73.3/Askpyro.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      474 2023-04-27 15:34:29.000000 Askpyro-1.73.3/Askpyro.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 15:34:29.000000 Askpyro-1.73.3/Askpyro.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 15:34:29.000000 Askpyro-1.73.3/Askpyro.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       17 2023-04-27 15:34:29.000000 Askpyro-1.73.3/Askpyro.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)    35149 2023-04-27 15:25:05.000000 Askpyro-1.73.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4433 2023-04-27 15:34:30.005124 Askpyro-1.73.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2588 2023-04-27 15:25:05.000000 Askpyro-1.73.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 15:34:30.001124 Askpyro-1.73.3/askpyro/
--rw-r--r--   0 root         (0) root         (0)      242 2023-04-27 15:25:05.000000 Askpyro-1.73.3/askpyro/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5532 2023-04-27 15:25:05.000000 Askpyro-1.73.3/askpyro/conversation.py
--rw-r--r--   0 root         (0) root         (0)      824 2023-04-27 15:25:05.000000 Askpyro-1.73.3/askpyro/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 15:34:30.001124 Askpyro-1.73.3/askpyro/helpers/
--rw-r--r--   0 root         (0) root         (0)      804 2023-04-27 15:25:05.000000 Askpyro-1.73.3/askpyro/helpers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3208 2023-04-27 15:25:05.000000 Askpyro-1.73.3/askpyro/helpers/helpers.py
--rw-r--r--   0 root         (0) root         (0)     1444 2023-04-27 15:25:05.000000 Askpyro-1.73.3/askpyro/helpers/http_helper.py
--rw-r--r--   0 root         (0) root         (0)     1282 2023-04-27 15:25:05.000000 Askpyro-1.73.3/askpyro/helpers/parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 15:34:30.005124 Askpyro-1.73.3/examples/
--rw-r--r--   0 root         (0) root         (0)      161 2023-04-27 15:25:05.000000 Askpyro-1.73.3/examples/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1442 2023-04-27 15:25:05.000000 Askpyro-1.73.3/examples/buttons.py
--rw-r--r--   0 root         (0) root         (0)      519 2023-04-27 15:25:05.000000 Askpyro-1.73.3/examples/callback.py
--rw-r--r--   0 root         (0) root         (0)     1775 2023-04-27 15:25:05.000000 Askpyro-1.73.3/examples/captcha.py
--rw-r--r--   0 root         (0) root         (0)      502 2023-04-27 15:25:05.000000 Askpyro-1.73.3/examples/filters.py
--rw-r--r--   0 root         (0) root         (0)      444 2023-04-27 15:25:05.000000 Askpyro-1.73.3/examples/start.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-27 15:34:30.005124 Askpyro-1.73.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3199 2023-04-27 15:25:05.000000 Askpyro-1.73.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 18:48:45.587699 Askpyro-1.73.4/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 18:48:45.579699 Askpyro-1.73.4/Askpyro.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5038 2023-05-16 18:48:45.000000 Askpyro-1.73.4/Askpyro.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      523 2023-05-16 18:48:45.000000 Askpyro-1.73.4/Askpyro.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 18:48:45.000000 Askpyro-1.73.4/Askpyro.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 18:48:45.000000 Askpyro-1.73.4/Askpyro.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       17 2023-05-16 18:48:45.000000 Askpyro-1.73.4/Askpyro.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5038 2023-05-16 18:48:45.583699 Askpyro-1.73.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2588 2023-05-16 18:45:24.000000 Askpyro-1.73.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 18:48:45.579699 Askpyro-1.73.4/askpyro/
+-rw-r--r--   0 root         (0) root         (0)      242 2023-05-16 18:45:24.000000 Askpyro-1.73.4/askpyro/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5532 2023-05-16 18:45:24.000000 Askpyro-1.73.4/askpyro/conversation.py
+-rw-r--r--   0 root         (0) root         (0)      824 2023-05-16 18:45:24.000000 Askpyro-1.73.4/askpyro/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 18:48:45.583699 Askpyro-1.73.4/askpyro/helpers/
+-rw-r--r--   0 root         (0) root         (0)      833 2023-05-16 18:45:24.000000 Askpyro-1.73.4/askpyro/helpers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3208 2023-05-16 18:45:24.000000 Askpyro-1.73.4/askpyro/helpers/helpers.py
+-rw-r--r--   0 root         (0) root         (0)     1597 2023-05-16 18:45:24.000000 Askpyro-1.73.4/askpyro/helpers/http_helper.py
+-rw-r--r--   0 root         (0) root         (0)       52 2023-05-16 18:45:24.000000 Askpyro-1.73.4/askpyro/helpers/lock.py
+-rw-r--r--   0 root         (0) root         (0)     1282 2023-05-16 18:45:24.000000 Askpyro-1.73.4/askpyro/helpers/parser.py
+-rw-r--r--   0 root         (0) root         (0)     2452 2023-05-16 18:45:24.000000 Askpyro-1.73.4/askpyro/helpers/pyro_progress.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 18:48:45.583699 Askpyro-1.73.4/examples/
+-rw-r--r--   0 root         (0) root         (0)      161 2023-05-16 18:45:24.000000 Askpyro-1.73.4/examples/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1442 2023-05-16 18:45:24.000000 Askpyro-1.73.4/examples/buttons.py
+-rw-r--r--   0 root         (0) root         (0)      519 2023-05-16 18:45:24.000000 Askpyro-1.73.4/examples/callback.py
+-rw-r--r--   0 root         (0) root         (0)     1775 2023-05-16 18:45:24.000000 Askpyro-1.73.4/examples/captcha.py
+-rw-r--r--   0 root         (0) root         (0)      502 2023-05-16 18:45:24.000000 Askpyro-1.73.4/examples/filters.py
+-rw-r--r--   0 root         (0) root         (0)      444 2023-05-16 18:45:24.000000 Askpyro-1.73.4/examples/start.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-16 18:48:45.587699 Askpyro-1.73.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3199 2023-05-16 18:45:24.000000 Askpyro-1.73.4/setup.py
```

### Comparing `Askpyro-1.73.3/Askpyro.egg-info/PKG-INFO` & `Askpyro-1.73.4/Askpyro.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,98 @@
 Metadata-Version: 2.1
 Name: Askpyro
-Version: 1.73.3
+Version: 1.73.4
 Summary: Easy conversation handler for pyrogram
 Home-page: https://github.com/Abishnoi69
 Author: Abishnoi
 Author-email: abishnoi@askpyro.org
 License: LGPLv3
 Download-URL: https://github.com/Abishnoi69/Askpyro/releases/latest
 Project-URL: Tracker, https://github.com/Abishnoi69/Askpyro/issues
 Project-URL: Community, https://t.me/AbishnoiMF
 Project-URL: Source, https://github.com/Abishnoi69/Askpyro
 Project-URL: Documentation, https://github.com/Abishnoi69/askpyro/wiki
+Description: # ᴀsᴋ-ᴘʏʀᴏ :->
+        
+        > sᴛᴀʀᴛ ᴀsᴋ-ᴄʟɪᴇɴᴛ ᴡɪᴛʜ @ᴀᴘᴘ [ᴘʏʀᴏɢʀᴀᴍ ᴄʟɪᴇɴᴛ]
+        ```python
+          from askpyro import Askclient
+          from pyrogram import Client ,filters
+          
+          app = Client("my_account")
+          read = Askclient(app)
+        
+          @app.on_message(filters.command("start"))
+          async def start_pm(c: app, m: Message):
+            answer = await read.ask(m, text)
+            if answer.text:
+             print(answer.text)
+            await answer.reply("ɪ ɢᴏᴛ ᴀɴsᴡᴇʀ..")
+        
+          app.run()
+        ```
+        
+        
+        ### ɪɴsᴛᴀʟʟɪɴɢ :->
+        
+        ```bash
+        pip3 install askpyro
+        ```
+        
+        <details>
+        <summary><h3>
+        - <b> ᴄᴏɴᴠᴇʀsᴀᴛɪᴏɴ ɪɴ ᴘʏʀᴏɢʀᴀᴍ :-></b>
+        </h3></summary>
+        <a href="https://github.com/Abishnoi69/Askpyro/wiki/Conversation"><img src="https://img.shields.io/badge/ᴄᴏɴᴠᴇʀsᴀᴛɪᴏɴ-903022f?logo=github"></a>
+        </details>
+        
+        <details>
+        <summary><h3>
+        - <b> ᴡɪᴋɪ / ʜᴏᴡ ᴛᴏ ᴜsᴇ :-></b>
+        </h3></summary>
+        <a href="https://github.com/Abishnoi69/askpyro/wiki"><img src="https://img.shields.io/badge/ᴡɪᴋɪ-1589F0?logo=github"></a>
+        </details>
+        
+        <details>
+        <summary><h3>
+        - <b> ᴇxᴀᴍᴘʟᴇ :-></b>
+        </h3></summary>
+        <a href="https://github.com/Abishnoi69/askpyro/tree/main/examples"><img src="https://img.shields.io/badge/ᴇxᴀᴍᴘʟᴇs-c5f015?logo=github"></a>
+        </details>
+        
+        <details>
+        <summary><h3>
+        - <b> ᴛᴇʟᴇɢʀᴀᴍ ɢʀᴏᴜᴘ :-></b>
+        </h3></summary>
+        <a href="https://telegram.me/AbishnoiMF"><img src="https://img.shields.io/badge/-Support%20Group-blue.svg?style=for-the-badge&logo=Telegram"></a>
+        </details>
+        
+        
+        ━━━━━━━━━━━━━━━━━━━━
+        ## ɴᴏᴛᴇ :->
+        
+        - This library is made for my personal Project so don't take it deeply  [you can use this 24*7 running ] 
+        - My Project [AbgRobot](https://t.me/AbgRobot) & [Exon_Robot](https://t.me/Exon_Robot) 
+        - Enjoy Baby 
+        
+        ━━━━━━━━━━━━━━━━━━━━ 
+         
+        <details>
+        <summary><h3>
+        - <b>ᴄʀᴇᴅɪᴛs :-></b>
+        </h3></summary>
+        
+        ➥ [𝐀𝖻𝗂𝗌𝗁𝗇𝗈𝗂] ↬ <a href="https://github.com/Abishnoi69" alt="Abishnoi69"> <img src="https://img.shields.io/badge/ᴀʙɪsʜɴᴏɪ-90302f?logo=github" /></a>  
+        
+        ➥ [𝐏ʏʀᴏɢʀᴀᴍ] ↬ <a href="https://github.com/pyrogram" alt="Pyrogram"> <img src="https://img.shields.io/badge/Pyrogram-90302f?logo=github" /></a>  
+          
+        ➥ [𝐒ᴘɪᴅᴇʀ] ↬ <a href="https://github.com/Surendra9123" alt="Surendra9123"> <img src="https://img.shields.io/badge/SPiDER-90302f?logo=github" /></a>  
+        ━━━━━━━━━━━━━━━━━━━━
+        </details>
+        
 Keywords: telegram chat messenger mtproto api client library python conversation
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
@@ -32,88 +110,7 @@
 Classifier: Topic :: Communications
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# ᴀsᴋ-ᴘʏʀᴏ :->
-
-> sᴛᴀʀᴛ ᴀsᴋ-ᴄʟɪᴇɴᴛ ᴡɪᴛʜ @ᴀᴘᴘ [ᴘʏʀᴏɢʀᴀᴍ ᴄʟɪᴇɴᴛ]
-```python
-  from askpyro import Askclient
-  from pyrogram import Client ,filters
-  
-  app = Client("my_account")
-  read = Askclient(app)
-
-  @app.on_message(filters.command("start"))
-  async def start_pm(c: app, m: Message):
-    answer = await read.ask(m, text)
-    if answer.text:
-     print(answer.text)
-    await answer.reply("ɪ ɢᴏᴛ ᴀɴsᴡᴇʀ..")
-
-  app.run()
-```
-
-
-### ɪɴsᴛᴀʟʟɪɴɢ :->
-
-```bash
-pip3 install askpyro
-```
-
-<details>
-<summary><h3>
-- <b> ᴄᴏɴᴠᴇʀsᴀᴛɪᴏɴ ɪɴ ᴘʏʀᴏɢʀᴀᴍ :-></b>
-</h3></summary>
-<a href="https://github.com/Abishnoi69/Askpyro/wiki/Conversation"><img src="https://img.shields.io/badge/ᴄᴏɴᴠᴇʀsᴀᴛɪᴏɴ-903022f?logo=github"></a>
-</details>
-
-<details>
-<summary><h3>
-- <b> ᴡɪᴋɪ / ʜᴏᴡ ᴛᴏ ᴜsᴇ :-></b>
-</h3></summary>
-<a href="https://github.com/Abishnoi69/askpyro/wiki"><img src="https://img.shields.io/badge/ᴡɪᴋɪ-1589F0?logo=github"></a>
-</details>
-
-<details>
-<summary><h3>
-- <b> ᴇxᴀᴍᴘʟᴇ :-></b>
-</h3></summary>
-<a href="https://github.com/Abishnoi69/askpyro/tree/main/examples"><img src="https://img.shields.io/badge/ᴇxᴀᴍᴘʟᴇs-c5f015?logo=github"></a>
-</details>
-
-<details>
-<summary><h3>
-- <b> ᴛᴇʟᴇɢʀᴀᴍ ɢʀᴏᴜᴘ :-></b>
-</h3></summary>
-<a href="https://telegram.me/AbishnoiMF"><img src="https://img.shields.io/badge/-Support%20Group-blue.svg?style=for-the-badge&logo=Telegram"></a>
-</details>
-
-
-━━━━━━━━━━━━━━━━━━━━
-## ɴᴏᴛᴇ :->
-
-- This library is made for my personal Project so don't take it deeply  [you can use this 24*7 running ] 
-- My Project [AbgRobot](https://t.me/AbgRobot) & [Exon_Robot](https://t.me/Exon_Robot) 
-- Enjoy Baby 
-
-━━━━━━━━━━━━━━━━━━━━ 
- 
-<details>
-<summary><h3>
-- <b>ᴄʀᴇᴅɪᴛs :-></b>
-</h3></summary>
-
-➥ [𝐀𝖻𝗂𝗌𝗁𝗇𝗈𝗂] ↬ <a href="https://github.com/Abishnoi69" alt="Abishnoi69"> <img src="https://img.shields.io/badge/ᴀʙɪsʜɴᴏɪ-90302f?logo=github" /></a>  
-
-➥ [𝐏ʏʀᴏɢʀᴀᴍ] ↬ <a href="https://github.com/pyrogram" alt="Pyrogram"> <img src="https://img.shields.io/badge/Pyrogram-90302f?logo=github" /></a>  
-  
-➥ [𝐒ᴘɪᴅᴇʀ] ↬ <a href="https://github.com/Surendra9123" alt="Surendra9123"> <img src="https://img.shields.io/badge/SPiDER-90302f?logo=github" /></a>  
-━━━━━━━━━━━━━━━━━━━━
-</details>
-
-
```

#### html2text {}

```diff
@@ -1,39 +1,21 @@
-Metadata-Version: 2.1 Name: Askpyro Version: 1.73.3 Summary: Easy conversation
+Metadata-Version: 2.1 Name: Askpyro Version: 1.73.4 Summary: Easy conversation
 handler for pyrogram Home-page: https://github.com/Abishnoi69 Author: Abishnoi
 Author-email: abishnoi@askpyro.org License: LGPLv3 Download-URL: https://
 github.com/Abishnoi69/Askpyro/releases/latest Project-URL: Tracker, https://
 github.com/Abishnoi69/Askpyro/issues Project-URL: Community, https://t.me/
 AbishnoiMF Project-URL: Source, https://github.com/Abishnoi69/Askpyro Project-
-URL: Documentation, https://github.com/Abishnoi69/askpyro/wiki Keywords:
-telegram chat messenger mtproto api client library python conversation
-Platform: UNKNOWN Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers Classifier: Natural Language ::
-English Classifier: License :: OSI Approved :: GNU Lesser General Public
-License v3 (LGPLv3) Classifier: Operating System :: OS Independent Classifier:
-Programming Language :: Python Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Programming Language :: Python ::
-Implementation Classifier: Programming Language :: Python :: Implementation ::
-CPython Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Topic :: Internet Classifier: Topic :: Communications Classifier:
-Topic :: Communications :: Chat Classifier: Topic :: Software Development ::
-Libraries Classifier: Topic :: Software Development :: Libraries :: Python
-Modules Classifier: Topic :: Software Development :: Libraries :: Application
-Frameworks Requires-Python: ~=3.7 Description-Content-Type: text/markdown
-License-File: LICENSE # á´sá´-á´ÊÊá´ :-> > sá´á´Êá´ á´sá´-
-á´ÊÉªá´É´á´ á´¡Éªá´Ê @á´á´á´ [á´ÊÊá´É¢Êá´á´ á´ÊÉªá´É´á´]
-```python from askpyro import Askclient from pyrogram import Client ,filters
-app = Client("my_account") read = Askclient(app) @app.on_message
-(filters.command("start")) async def start_pm(c: app, m: Message): answer =
-await read.ask(m, text) if answer.text: print(answer.text) await answer.reply
-("Éª É¢á´á´ á´É´sá´¡á´Ê..") app.run() ``` ### ÉªÉ´sá´á´ÊÊÉªÉ´É¢ :-
-> ```bash pip3 install askpyro ```
+URL: Documentation, https://github.com/Abishnoi69/askpyro/wiki Description: #
+á´sá´-á´ÊÊá´ :-> > sá´á´Êá´ á´sá´-á´ÊÉªá´É´á´ á´¡Éªá´Ê
+@á´á´á´ [á´ÊÊá´É¢Êá´á´ á´ÊÉªá´É´á´] ```python from askpyro import
+Askclient from pyrogram import Client ,filters app = Client("my_account") read
+= Askclient(app) @app.on_message(filters.command("start")) async def start_pm
+(c: app, m: Message): answer = await read.ask(m, text) if answer.text: print
+(answer.text) await answer.reply("Éª É¢á´á´ á´É´sá´¡á´Ê..") app.run() ```
+### ÉªÉ´sá´á´ÊÊÉªÉ´É¢ :-> ```bash pip3 install askpyro ```
 **** - á´á´É´á´ á´Êsá´á´Éªá´É´ ÉªÉ´ á´ÊÊá´É¢Êá´á´ :-> ****
 [https://img.shields.io/badge/á´á´É´á´ á´Êsá´á´Éªá´É´-
 903022f?logo=github]
 **** - á´¡Éªá´Éª / Êá´á´¡ á´á´ á´sá´ :-> ****
 [https://img.shields.io/badge/á´¡Éªá´Éª-1589F0?logo=github]
 **** - á´xá´á´á´Êá´ :-> ****
 [https://img.shields.io/badge/á´xá´á´á´Êá´s-c5f015?logo=github]
@@ -46,8 +28,25 @@
 [Exon_Robot](https://t.me/Exon_Robot) - Enjoy Baby
 ââââââââââââââââââââ
 **** - á´Êá´á´Éªá´s :-> ****
 â¥ [ðð»ðððððð] â¬ [https://img.shields.io/badge/
 á´ÊÉªsÊÉ´á´Éª-90302f?logo=github] â¥ [ðÊÊá´É¢Êá´á´] â¬ [https://
 img.shields.io/badge/Pyrogram-90302f?logo=github] â¥ [ðá´Éªá´á´Ê] â¬
 [https://img.shields.io/badge/SPiDER-90302f?logo=github]
-ââââââââââââââââââââ
+ââââââââââââââââââââ  Keywords:
+telegram chat messenger mtproto api client library python conversation
+Platform: UNKNOWN Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers Classifier: Natural Language ::
+English Classifier: License :: OSI Approved :: GNU Lesser General Public
+License v3 (LGPLv3) Classifier: Operating System :: OS Independent Classifier:
+Programming Language :: Python Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python ::
+Implementation Classifier: Programming Language :: Python :: Implementation ::
+CPython Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Topic :: Internet Classifier: Topic :: Communications Classifier:
+Topic :: Communications :: Chat Classifier: Topic :: Software Development ::
+Libraries Classifier: Topic :: Software Development :: Libraries :: Python
+Modules Classifier: Topic :: Software Development :: Libraries :: Application
+Frameworks Requires-Python: ~=3.7 Description-Content-Type: text/markdown
```

### Comparing `Askpyro-1.73.3/PKG-INFO` & `Askpyro-1.73.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,98 @@
 Metadata-Version: 2.1
 Name: Askpyro
-Version: 1.73.3
+Version: 1.73.4
 Summary: Easy conversation handler for pyrogram
 Home-page: https://github.com/Abishnoi69
 Author: Abishnoi
 Author-email: abishnoi@askpyro.org
 License: LGPLv3
 Download-URL: https://github.com/Abishnoi69/Askpyro/releases/latest
 Project-URL: Tracker, https://github.com/Abishnoi69/Askpyro/issues
 Project-URL: Community, https://t.me/AbishnoiMF
 Project-URL: Source, https://github.com/Abishnoi69/Askpyro
 Project-URL: Documentation, https://github.com/Abishnoi69/askpyro/wiki
+Description: # ᴀsᴋ-ᴘʏʀᴏ :->
+        
+        > sᴛᴀʀᴛ ᴀsᴋ-ᴄʟɪᴇɴᴛ ᴡɪᴛʜ @ᴀᴘᴘ [ᴘʏʀᴏɢʀᴀᴍ ᴄʟɪᴇɴᴛ]
+        ```python
+          from askpyro import Askclient
+          from pyrogram import Client ,filters
+          
+          app = Client("my_account")
+          read = Askclient(app)
+        
+          @app.on_message(filters.command("start"))
+          async def start_pm(c: app, m: Message):
+            answer = await read.ask(m, text)
+            if answer.text:
+             print(answer.text)
+            await answer.reply("ɪ ɢᴏᴛ ᴀɴsᴡᴇʀ..")
+        
+          app.run()
+        ```
+        
+        
+        ### ɪɴsᴛᴀʟʟɪɴɢ :->
+        
+        ```bash
+        pip3 install askpyro
+        ```
+        
+        <details>
+        <summary><h3>
+        - <b> ᴄᴏɴᴠᴇʀsᴀᴛɪᴏɴ ɪɴ ᴘʏʀᴏɢʀᴀᴍ :-></b>
+        </h3></summary>
+        <a href="https://github.com/Abishnoi69/Askpyro/wiki/Conversation"><img src="https://img.shields.io/badge/ᴄᴏɴᴠᴇʀsᴀᴛɪᴏɴ-903022f?logo=github"></a>
+        </details>
+        
+        <details>
+        <summary><h3>
+        - <b> ᴡɪᴋɪ / ʜᴏᴡ ᴛᴏ ᴜsᴇ :-></b>
+        </h3></summary>
+        <a href="https://github.com/Abishnoi69/askpyro/wiki"><img src="https://img.shields.io/badge/ᴡɪᴋɪ-1589F0?logo=github"></a>
+        </details>
+        
+        <details>
+        <summary><h3>
+        - <b> ᴇxᴀᴍᴘʟᴇ :-></b>
+        </h3></summary>
+        <a href="https://github.com/Abishnoi69/askpyro/tree/main/examples"><img src="https://img.shields.io/badge/ᴇxᴀᴍᴘʟᴇs-c5f015?logo=github"></a>
+        </details>
+        
+        <details>
+        <summary><h3>
+        - <b> ᴛᴇʟᴇɢʀᴀᴍ ɢʀᴏᴜᴘ :-></b>
+        </h3></summary>
+        <a href="https://telegram.me/AbishnoiMF"><img src="https://img.shields.io/badge/-Support%20Group-blue.svg?style=for-the-badge&logo=Telegram"></a>
+        </details>
+        
+        
+        ━━━━━━━━━━━━━━━━━━━━
+        ## ɴᴏᴛᴇ :->
+        
+        - This library is made for my personal Project so don't take it deeply  [you can use this 24*7 running ] 
+        - My Project [AbgRobot](https://t.me/AbgRobot) & [Exon_Robot](https://t.me/Exon_Robot) 
+        - Enjoy Baby 
+        
+        ━━━━━━━━━━━━━━━━━━━━ 
+         
+        <details>
+        <summary><h3>
+        - <b>ᴄʀᴇᴅɪᴛs :-></b>
+        </h3></summary>
+        
+        ➥ [𝐀𝖻𝗂𝗌𝗁𝗇𝗈𝗂] ↬ <a href="https://github.com/Abishnoi69" alt="Abishnoi69"> <img src="https://img.shields.io/badge/ᴀʙɪsʜɴᴏɪ-90302f?logo=github" /></a>  
+        
+        ➥ [𝐏ʏʀᴏɢʀᴀᴍ] ↬ <a href="https://github.com/pyrogram" alt="Pyrogram"> <img src="https://img.shields.io/badge/Pyrogram-90302f?logo=github" /></a>  
+          
+        ➥ [𝐒ᴘɪᴅᴇʀ] ↬ <a href="https://github.com/Surendra9123" alt="Surendra9123"> <img src="https://img.shields.io/badge/SPiDER-90302f?logo=github" /></a>  
+        ━━━━━━━━━━━━━━━━━━━━
+        </details>
+        
 Keywords: telegram chat messenger mtproto api client library python conversation
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
@@ -32,88 +110,7 @@
 Classifier: Topic :: Communications
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# ᴀsᴋ-ᴘʏʀᴏ :->
-
-> sᴛᴀʀᴛ ᴀsᴋ-ᴄʟɪᴇɴᴛ ᴡɪᴛʜ @ᴀᴘᴘ [ᴘʏʀᴏɢʀᴀᴍ ᴄʟɪᴇɴᴛ]
-```python
-  from askpyro import Askclient
-  from pyrogram import Client ,filters
-  
-  app = Client("my_account")
-  read = Askclient(app)
-
-  @app.on_message(filters.command("start"))
-  async def start_pm(c: app, m: Message):
-    answer = await read.ask(m, text)
-    if answer.text:
-     print(answer.text)
-    await answer.reply("ɪ ɢᴏᴛ ᴀɴsᴡᴇʀ..")
-
-  app.run()
-```
-
-
-### ɪɴsᴛᴀʟʟɪɴɢ :->
-
-```bash
-pip3 install askpyro
-```
-
-<details>
-<summary><h3>
-- <b> ᴄᴏɴᴠᴇʀsᴀᴛɪᴏɴ ɪɴ ᴘʏʀᴏɢʀᴀᴍ :-></b>
-</h3></summary>
-<a href="https://github.com/Abishnoi69/Askpyro/wiki/Conversation"><img src="https://img.shields.io/badge/ᴄᴏɴᴠᴇʀsᴀᴛɪᴏɴ-903022f?logo=github"></a>
-</details>
-
-<details>
-<summary><h3>
-- <b> ᴡɪᴋɪ / ʜᴏᴡ ᴛᴏ ᴜsᴇ :-></b>
-</h3></summary>
-<a href="https://github.com/Abishnoi69/askpyro/wiki"><img src="https://img.shields.io/badge/ᴡɪᴋɪ-1589F0?logo=github"></a>
-</details>
-
-<details>
-<summary><h3>
-- <b> ᴇxᴀᴍᴘʟᴇ :-></b>
-</h3></summary>
-<a href="https://github.com/Abishnoi69/askpyro/tree/main/examples"><img src="https://img.shields.io/badge/ᴇxᴀᴍᴘʟᴇs-c5f015?logo=github"></a>
-</details>
-
-<details>
-<summary><h3>
-- <b> ᴛᴇʟᴇɢʀᴀᴍ ɢʀᴏᴜᴘ :-></b>
-</h3></summary>
-<a href="https://telegram.me/AbishnoiMF"><img src="https://img.shields.io/badge/-Support%20Group-blue.svg?style=for-the-badge&logo=Telegram"></a>
-</details>
-
-
-━━━━━━━━━━━━━━━━━━━━
-## ɴᴏᴛᴇ :->
-
-- This library is made for my personal Project so don't take it deeply  [you can use this 24*7 running ] 
-- My Project [AbgRobot](https://t.me/AbgRobot) & [Exon_Robot](https://t.me/Exon_Robot) 
-- Enjoy Baby 
-
-━━━━━━━━━━━━━━━━━━━━ 
- 
-<details>
-<summary><h3>
-- <b>ᴄʀᴇᴅɪᴛs :-></b>
-</h3></summary>
-
-➥ [𝐀𝖻𝗂𝗌𝗁𝗇𝗈𝗂] ↬ <a href="https://github.com/Abishnoi69" alt="Abishnoi69"> <img src="https://img.shields.io/badge/ᴀʙɪsʜɴᴏɪ-90302f?logo=github" /></a>  
-
-➥ [𝐏ʏʀᴏɢʀᴀᴍ] ↬ <a href="https://github.com/pyrogram" alt="Pyrogram"> <img src="https://img.shields.io/badge/Pyrogram-90302f?logo=github" /></a>  
-  
-➥ [𝐒ᴘɪᴅᴇʀ] ↬ <a href="https://github.com/Surendra9123" alt="Surendra9123"> <img src="https://img.shields.io/badge/SPiDER-90302f?logo=github" /></a>  
-━━━━━━━━━━━━━━━━━━━━
-</details>
-
-
```

#### html2text {}

```diff
@@ -1,39 +1,21 @@
-Metadata-Version: 2.1 Name: Askpyro Version: 1.73.3 Summary: Easy conversation
+Metadata-Version: 2.1 Name: Askpyro Version: 1.73.4 Summary: Easy conversation
 handler for pyrogram Home-page: https://github.com/Abishnoi69 Author: Abishnoi
 Author-email: abishnoi@askpyro.org License: LGPLv3 Download-URL: https://
 github.com/Abishnoi69/Askpyro/releases/latest Project-URL: Tracker, https://
 github.com/Abishnoi69/Askpyro/issues Project-URL: Community, https://t.me/
 AbishnoiMF Project-URL: Source, https://github.com/Abishnoi69/Askpyro Project-
-URL: Documentation, https://github.com/Abishnoi69/askpyro/wiki Keywords:
-telegram chat messenger mtproto api client library python conversation
-Platform: UNKNOWN Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers Classifier: Natural Language ::
-English Classifier: License :: OSI Approved :: GNU Lesser General Public
-License v3 (LGPLv3) Classifier: Operating System :: OS Independent Classifier:
-Programming Language :: Python Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Programming Language :: Python ::
-Implementation Classifier: Programming Language :: Python :: Implementation ::
-CPython Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Topic :: Internet Classifier: Topic :: Communications Classifier:
-Topic :: Communications :: Chat Classifier: Topic :: Software Development ::
-Libraries Classifier: Topic :: Software Development :: Libraries :: Python
-Modules Classifier: Topic :: Software Development :: Libraries :: Application
-Frameworks Requires-Python: ~=3.7 Description-Content-Type: text/markdown
-License-File: LICENSE # á´sá´-á´ÊÊá´ :-> > sá´á´Êá´ á´sá´-
-á´ÊÉªá´É´á´ á´¡Éªá´Ê @á´á´á´ [á´ÊÊá´É¢Êá´á´ á´ÊÉªá´É´á´]
-```python from askpyro import Askclient from pyrogram import Client ,filters
-app = Client("my_account") read = Askclient(app) @app.on_message
-(filters.command("start")) async def start_pm(c: app, m: Message): answer =
-await read.ask(m, text) if answer.text: print(answer.text) await answer.reply
-("Éª É¢á´á´ á´É´sá´¡á´Ê..") app.run() ``` ### ÉªÉ´sá´á´ÊÊÉªÉ´É¢ :-
-> ```bash pip3 install askpyro ```
+URL: Documentation, https://github.com/Abishnoi69/askpyro/wiki Description: #
+á´sá´-á´ÊÊá´ :-> > sá´á´Êá´ á´sá´-á´ÊÉªá´É´á´ á´¡Éªá´Ê
+@á´á´á´ [á´ÊÊá´É¢Êá´á´ á´ÊÉªá´É´á´] ```python from askpyro import
+Askclient from pyrogram import Client ,filters app = Client("my_account") read
+= Askclient(app) @app.on_message(filters.command("start")) async def start_pm
+(c: app, m: Message): answer = await read.ask(m, text) if answer.text: print
+(answer.text) await answer.reply("Éª É¢á´á´ á´É´sá´¡á´Ê..") app.run() ```
+### ÉªÉ´sá´á´ÊÊÉªÉ´É¢ :-> ```bash pip3 install askpyro ```
 **** - á´á´É´á´ á´Êsá´á´Éªá´É´ ÉªÉ´ á´ÊÊá´É¢Êá´á´ :-> ****
 [https://img.shields.io/badge/á´á´É´á´ á´Êsá´á´Éªá´É´-
 903022f?logo=github]
 **** - á´¡Éªá´Éª / Êá´á´¡ á´á´ á´sá´ :-> ****
 [https://img.shields.io/badge/á´¡Éªá´Éª-1589F0?logo=github]
 **** - á´xá´á´á´Êá´ :-> ****
 [https://img.shields.io/badge/á´xá´á´á´Êá´s-c5f015?logo=github]
@@ -46,8 +28,25 @@
 [Exon_Robot](https://t.me/Exon_Robot) - Enjoy Baby
 ââââââââââââââââââââ
 **** - á´Êá´á´Éªá´s :-> ****
 â¥ [ðð»ðððððð] â¬ [https://img.shields.io/badge/
 á´ÊÉªsÊÉ´á´Éª-90302f?logo=github] â¥ [ðÊÊá´É¢Êá´á´] â¬ [https://
 img.shields.io/badge/Pyrogram-90302f?logo=github] â¥ [ðá´Éªá´á´Ê] â¬
 [https://img.shields.io/badge/SPiDER-90302f?logo=github]
-ââââââââââââââââââââ
+ââââââââââââââââââââ  Keywords:
+telegram chat messenger mtproto api client library python conversation
+Platform: UNKNOWN Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers Classifier: Natural Language ::
+English Classifier: License :: OSI Approved :: GNU Lesser General Public
+License v3 (LGPLv3) Classifier: Operating System :: OS Independent Classifier:
+Programming Language :: Python Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python ::
+Implementation Classifier: Programming Language :: Python :: Implementation ::
+CPython Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Topic :: Internet Classifier: Topic :: Communications Classifier:
+Topic :: Communications :: Chat Classifier: Topic :: Software Development ::
+Libraries Classifier: Topic :: Software Development :: Libraries :: Python
+Modules Classifier: Topic :: Software Development :: Libraries :: Application
+Frameworks Requires-Python: ~=3.7 Description-Content-Type: text/markdown
```

### Comparing `Askpyro-1.73.3/README.md` & `Askpyro-1.73.4/README.md`

 * *Files identical despite different names*

### Comparing `Askpyro-1.73.3/askpyro/conversation.py` & `Askpyro-1.73.4/askpyro/conversation.py`

 * *Files identical despite different names*

### Comparing `Askpyro-1.73.3/askpyro/errors.py` & `Askpyro-1.73.4/askpyro/errors.py`

 * *Files identical despite different names*

### Comparing `Askpyro-1.73.3/askpyro/helpers/__init__.py` & `Askpyro-1.73.4/askpyro/helpers/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,7 +15,8 @@
 
 along with Askpyro.  If not, see <https://www.gnu.org/licenses/>.
 """
 
 from .helpers import *
 from .http_helper import *
 from .parser import *
+from .pyro_progress import *
```

### Comparing `Askpyro-1.73.3/askpyro/helpers/helpers.py` & `Askpyro-1.73.4/askpyro/helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `Askpyro-1.73.3/askpyro/helpers/http_helper.py` & `Askpyro-1.73.4/askpyro/helpers/http_helper.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,24 @@
 from asyncio import gather
-
+import httpx
 from aiohttp import ClientSession
 
+# Aiohttp Async Client
 aiohttpsession = ClientSession()
 
+
+# HTTPx Async Client
+
+http = httpx.AsyncClient(
+    http2=True,
+    verify=False,
+    timeout=httpx.Timeout(40),
+)
+
+
 async def get(url: str, *args, **kwargs):
     async with aiohttpsession.get(url, *args, **kwargs) as resp:
         try:
             data = await resp.json()
         except Exception:
             data = await resp.text()
     return data
```

### Comparing `Askpyro-1.73.3/askpyro/helpers/parser.py` & `Askpyro-1.73.4/askpyro/helpers/parser.py`

 * *Files identical despite different names*

### Comparing `Askpyro-1.73.3/examples/buttons.py` & `Askpyro-1.73.4/examples/buttons.py`

 * *Files identical despite different names*

### Comparing `Askpyro-1.73.3/examples/callback.py` & `Askpyro-1.73.4/examples/callback.py`

 * *Files identical despite different names*

### Comparing `Askpyro-1.73.3/examples/captcha.py` & `Askpyro-1.73.4/examples/captcha.py`

 * *Files identical despite different names*

### Comparing `Askpyro-1.73.3/setup.py` & `Askpyro-1.73.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     with open(file, encoding="utf-8") as r:
         return [i.strip() for i in r]
 """
 
 setuptools.setup(
     name="Askpyro",
     packages=setuptools.find_packages(),
-    version="1.73.3",
+    version="1.73.4",
     description="Easy conversation handler for pyrogram",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Abishnoi69",
     download_url="https://github.com/Abishnoi69/Askpyro/releases/latest",
     author="Abishnoi",
     author_email="abishnoi@askpyro.org",
```

