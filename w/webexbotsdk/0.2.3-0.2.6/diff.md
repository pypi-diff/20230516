# Comparing `tmp/webexbotsdk-0.2.3.tar.gz` & `tmp/webexbotsdk-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webexbotsdk-0.2.3.tar", last modified: Fri Apr 28 21:31:40 2023, max compression
+gzip compressed data, was "webexbotsdk-0.2.6.tar", last modified: Tue May 16 13:56:01 2023, max compression
```

## Comparing `webexbotsdk-0.2.3.tar` & `webexbotsdk-0.2.6.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:31:40.415064 webexbotsdk-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-28 21:31:21.000000 webexbotsdk-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-28 21:31:21.000000 webexbotsdk-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-04-28 21:31:40.415064 webexbotsdk-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-04-28 21:31:21.000000 webexbotsdk-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-28 21:31:21.000000 webexbotsdk-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 21:31:40.415064 webexbotsdk-0.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:31:40.411064 webexbotsdk-0.2.3/webexbotsdk/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 21:31:21.000000 webexbotsdk-0.2.3/webexbotsdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:31:40.415064 webexbotsdk-0.2.3/webexbotsdk/teams/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-28 21:31:21.000000 webexbotsdk-0.2.3/webexbotsdk/teams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-04-28 21:31:21.000000 webexbotsdk-0.2.3/webexbotsdk/teams/bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-04-28 21:31:21.000000 webexbotsdk-0.2.3/webexbotsdk/teams/hook.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-28 21:31:21.000000 webexbotsdk-0.2.3/webexbotsdk/teams/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-28 21:31:21.000000 webexbotsdk-0.2.3/webexbotsdk/tinydb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:31:40.411064 webexbotsdk-0.2.3/webexbotsdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-04-28 21:31:40.000000 webexbotsdk-0.2.3/webexbotsdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-28 21:31:40.000000 webexbotsdk-0.2.3/webexbotsdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 21:31:40.000000 webexbotsdk-0.2.3/webexbotsdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-28 21:31:40.000000 webexbotsdk-0.2.3/webexbotsdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-28 21:31:40.000000 webexbotsdk-0.2.3/webexbotsdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:56:01.954842 webexbotsdk-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-16 13:55:48.000000 webexbotsdk-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-16 13:55:48.000000 webexbotsdk-0.2.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-05-16 13:56:01.950842 webexbotsdk-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5852 2023-05-16 13:55:48.000000 webexbotsdk-0.2.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-16 13:55:48.000000 webexbotsdk-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 13:56:01.954842 webexbotsdk-0.2.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:56:01.950842 webexbotsdk-0.2.6/webexbotsdk/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:55:48.000000 webexbotsdk-0.2.6/webexbotsdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-16 13:55:48.000000 webexbotsdk-0.2.6/webexbotsdk/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:56:01.950842 webexbotsdk-0.2.6/webexbotsdk/teams/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-16 13:55:48.000000 webexbotsdk-0.2.6/webexbotsdk/teams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-05-16 13:55:48.000000 webexbotsdk-0.2.6/webexbotsdk/teams/bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-05-16 13:55:48.000000 webexbotsdk-0.2.6/webexbotsdk/teams/hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-16 13:55:48.000000 webexbotsdk-0.2.6/webexbotsdk/teams/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-16 13:55:48.000000 webexbotsdk-0.2.6/webexbotsdk/tinydb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:56:01.950842 webexbotsdk-0.2.6/webexbotsdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-05-16 13:56:01.000000 webexbotsdk-0.2.6/webexbotsdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-16 13:56:01.000000 webexbotsdk-0.2.6/webexbotsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 13:56:01.000000 webexbotsdk-0.2.6/webexbotsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-16 13:56:01.000000 webexbotsdk-0.2.6/webexbotsdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-16 13:56:01.000000 webexbotsdk-0.2.6/webexbotsdk.egg-info/top_level.txt
```

### Comparing `webexbotsdk-0.2.3/LICENSE` & `webexbotsdk-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `webexbotsdk-0.2.3/PKG-INFO` & `webexbotsdk-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webexbotsdk
-Version: 0.2.3
+Version: 0.2.6
 Summary: Webex bot creation framework and tools
 License: The MIT License (MIT)
         
         Copyright (c) 2016-2020 Cisco and/or its affiliates.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -20,15 +20,15 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: repository, https://github.com/xharriscisco/WebexPythonBotSDK
+Project-URL: Source, https://github.com/xharriscisco/WebexPythonBotSDK
 Keywords: cisco,webex,teams,bot,python,framework,enterprise,messaging
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Communications :: Chat
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -46,15 +46,15 @@
 
 ##### [Contributing](#contributing)
 
 <br/>
 
 ## <a id='teams'></a> `webexbotsdk.teams`
 
-###### [#EG](#teams-eg) | [#API](#teams-api) | A framework for creating a Webex Teams bot
+###### [#EG](#teams-eg) | [#API](#teams-api) | A framework for creating a Webex Teams bot with automatic ngrok setup
 
 <br/>
 
 ### <a id='teams-eg'></a> [^](#toc) EG
 
 ---
 
@@ -115,15 +115,15 @@
 ```
 
 ##### [webexteamssdk](https://webexteamssdk.readthedocs.io/en/latest/) is included
 
 ```python
 from webexbotsdk.teams import Bot
 bot = Bot()
-all_rooms = api.rooms.list()
+all_rooms = bot.api.rooms.list()
 demo_rooms = [room for room in all_rooms if 'webexteamssdk Demo' in room.title]
 ```
 
 ##### local DB with [TinyDB](https://tinydb.readthedocs.io/en/latest/index.html) to remember things even after the bot is restarted
 
 ```python
 from webexbotsdk.teams import Bot
```

### Comparing `webexbotsdk-0.2.3/README.md` & `webexbotsdk-0.2.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 ##### [Contributing](#contributing)
 
 <br/>
 
 ## <a id='teams'></a> `webexbotsdk.teams`
 
-###### [#EG](#teams-eg) | [#API](#teams-api) | A framework for creating a Webex Teams bot
+###### [#EG](#teams-eg) | [#API](#teams-api) | A framework for creating a Webex Teams bot with automatic ngrok setup
 
 <br/>
 
 ### <a id='teams-eg'></a> [^](#toc) EG
 
 ---
 
@@ -80,15 +80,15 @@
 ```
 
 ##### [webexteamssdk](https://webexteamssdk.readthedocs.io/en/latest/) is included
 
 ```python
 from webexbotsdk.teams import Bot
 bot = Bot()
-all_rooms = api.rooms.list()
+all_rooms = bot.api.rooms.list()
 demo_rooms = [room for room in all_rooms if 'webexteamssdk Demo' in room.title]
 ```
 
 ##### local DB with [TinyDB](https://tinydb.readthedocs.io/en/latest/index.html) to remember things even after the bot is restarted
 
 ```python
 from webexbotsdk.teams import Bot
```

### Comparing `webexbotsdk-0.2.3/pyproject.toml` & `webexbotsdk-0.2.6/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "webexbotsdk"
 description = "Webex bot creation framework and tools"
-version = "0.2.3"
+version = "0.2.6"
 readme = "README.md"
 license = { file = "LICENSE" }
 classifiers = [
   "License :: OSI Approved :: MIT License",
   "Development Status :: 3 - Alpha",
   "Topic :: Communications :: Chat"
 ]
@@ -23,8 +23,8 @@
   "webexteamssdk",
   "pyngrok",
   "tinydb",
   "tinydb-encrypted-jsonstorage"
 ]
 
 [project.urls]
-repository = "https://github.com/xharriscisco/WebexPythonBotSDK"
+Source = "https://github.com/xharriscisco/WebexPythonBotSDK"
```

### Comparing `webexbotsdk-0.2.3/webexbotsdk/teams/bot.py` & `webexbotsdk-0.2.6/webexbotsdk/teams/bot.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from bottle import Bottle, request
 from webexteamssdk import WebexTeamsAPI, Webhook, Message, Person, Membership
 from webexteamssdk.models.cards import AdaptiveCard
-from pyngrok import ngrok, conf, exception
+from pyngrok import ngrok, exception
 from typing import Literal, overload
 from re import Pattern, sub
 from tinydb import TinyDB
 from tinydb.storages import JSONStorage
 import tinydb_encrypted_jsonstorage as tae
 from os.path import dirname, join
 from logging import Logger, basicConfig, getLogger, INFO
 import json
 
+from webexbotsdk import exception
 from .util import get_config_value
 from .hook import WebhookEvent, WebhookResource, Hook
 
 __all__ = ["Bot"]
 
 class Bot():
   app: Bottle
@@ -28,17 +29,30 @@
   def __init__(self, config:dict = {}) -> None:
     self.app = Bottle()
     self.config = config
     self.hooks = []
     self.db = None
     self.log = None
 
+  def initDb(self):
+    disaleDb = get_config_value(self.config, 'disableDb', False)
+    if not disaleDb:
+      botDbkey = get_config_value(self.config, 'botDbKey', 's0meDefaultK3y?')
+      dbPath = f"{get_config_value(self.config, 'botName', 'bot')}.db"
+      if get_config_value(self.config, 'encryptDb', False):
+        self.db = TinyDB(encryption_key=botDbkey, path=dbPath, storage=tae.EncryptedJSONStorage)
+      else:
+        self.db = TinyDB(path=dbPath, storage=JSONStorage)
+    return not disaleDb
+      
+
   def table(self, name:str):
-    if self.db is not None:
-      return self.db.table(name)
+    if not self.db and not self.initDb():
+      raise exception.DbError('disabled')
+    return self.db.table(name)
 
   @overload
   def setup(self, config:str = None): pass
   @overload
   def setup(self, config:dict = None): pass
   def setup(self, config:str|dict = None, withDb = True):
     '''
@@ -63,56 +77,50 @@
     if config:
       self.config.update(config)
     botAccessToken:str|None = get_config_value(self.config, 'botAccessToken')
     ngrokAuthToken:str|Literal[False] = get_config_value(self.config, 'ngrokAuthToken', False)
     botName = get_config_value(self.config, 'botName', 'mywebexbot')
     if ngrokAuthToken and len(ngrokAuthToken) > 5:
       ngrok.set_auth_token(ngrokAuthToken)
+    # Init webex api
     self.api = WebexTeamsAPI(botAccessToken)    
     # Set up logging 
     basicConfig(filename=f"{botName}.log",
       format='%(asctime)s %(message)s',
       filemode='w')
     self.log = getLogger(__name__)
     self.log.setLevel(INFO)
     print(f"Output written to {botName}.log")
     # Init db
-    disaleDb = get_config_value(self.config, 'disableDb', False)
-    if disaleDb:
-      botDbkey = get_config_value(self.config, 'botDbKey', 's0meDefaultK3y?')
-      dbPath = join(dirname(__file__), f"{get_config_value(self.config, 'botName', 'bot')}.db")
-      if get_config_value(self.config, 'encryptDb', False):
-        self.db = TinyDB(encryption_key=botDbkey, path=dbPath, storage=tae.EncryptedJSONStorage)
-      else:
-        self.db = TinyDB(path=dbPath, storage=JSONStorage)
+    self.initDb()
     self.log.info('Setup complete')
 
   def run(self):
     port = get_config_value(self.config, 'port', 8080)
     botName = get_config_value(self.config, 'botName', 'mywebexbot')
     # Set up ngrok tunnel
     for tunnel in ngrok.get_tunnels():
       if botName in tunnel.public_url:
         try:
           ngrok.disconnect(tunnel.public_url)
         except exception.PyngrokNgrokHTTPError as e:
           self.log.error(f"Could not close tunnel: {e.message}")
     tunnel:ngrok.NgrokTunnel = ngrok.connect(port)
     public_url = sub(r'https?', 'https', tunnel.public_url)
-    # Init webex api
+    # Create webex hooks
     for webhook in self.api.webhooks.list():
       self.api.webhooks.delete(webhookId=webhook.id)
     self.webhook = self.api.webhooks.create("bot_webhook_events", f"{public_url}/{botName}/events", WebhookResource.ALL.value, WebhookEvent.ALL.value)
     self.webhook = self.api.webhooks.create("bot_webhook_aa", f"{public_url}/{botName}/attachmentActions", WebhookResource.ATTACHMENT_ACTIONS.value, WebhookEvent.ALL.value)
     # Start server
     def callback(*args, **kwargs):
       for hook in self.hooks:
         ret = hook.matches(self.api, request.json)
-        if ret is not None:
-          hook.fn(ret, request.json)
+        if any([retItem is not None for retItem in ret]):
+          hook.fn(*ret)
     self.app.route(f'/{botName}/events', method=['GET','POST'], callback=callback)
     self.app.route(f'/{botName}/attachmentActions', method=['GET','POST'], callback=callback)
     self.app.run(host='127.0.0.1', port=port)
 
     # pidfile = join(getcwd(), f"{botName}.pid")
     # daemon_run(host='127.0.0.1', port=port, pidfile=pidfile)
```

### Comparing `webexbotsdk-0.2.3/webexbotsdk/teams/hook.py` & `webexbotsdk-0.2.6/webexbotsdk/teams/hook.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,14 +36,17 @@
     self.event = event
     regex = [regex] if not isinstance(regex, list) else regex
     self.regex = [compile(re) for re in regex if re is not None] # list[str|Pattern] -> list[Pattern]
     self.name = name or '/'.join([re.pattern for re in self.regex])
     self.description = description
     self.log = log or getLogger()
 
+  def __str__(self) -> str:
+    return f"Hook(name={self.name}, regex={','.join([re.pattern for re in self.regex])})"
+
   def matches(self, api:WebexTeamsAPI, data:dict = None):
     resource = data['resource'] if 'resource' in data else ''
     event = data['event'] if 'event' in data else ''
     extra = {}
     # card interaction
     if self.resource == resource:
       if resource == 'attachmentActions':
```

### Comparing `webexbotsdk-0.2.3/webexbotsdk.egg-info/PKG-INFO` & `webexbotsdk-0.2.6/webexbotsdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webexbotsdk
-Version: 0.2.3
+Version: 0.2.6
 Summary: Webex bot creation framework and tools
 License: The MIT License (MIT)
         
         Copyright (c) 2016-2020 Cisco and/or its affiliates.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -20,15 +20,15 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: repository, https://github.com/xharriscisco/WebexPythonBotSDK
+Project-URL: Source, https://github.com/xharriscisco/WebexPythonBotSDK
 Keywords: cisco,webex,teams,bot,python,framework,enterprise,messaging
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Communications :: Chat
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -46,15 +46,15 @@
 
 ##### [Contributing](#contributing)
 
 <br/>
 
 ## <a id='teams'></a> `webexbotsdk.teams`
 
-###### [#EG](#teams-eg) | [#API](#teams-api) | A framework for creating a Webex Teams bot
+###### [#EG](#teams-eg) | [#API](#teams-api) | A framework for creating a Webex Teams bot with automatic ngrok setup
 
 <br/>
 
 ### <a id='teams-eg'></a> [^](#toc) EG
 
 ---
 
@@ -115,15 +115,15 @@
 ```
 
 ##### [webexteamssdk](https://webexteamssdk.readthedocs.io/en/latest/) is included
 
 ```python
 from webexbotsdk.teams import Bot
 bot = Bot()
-all_rooms = api.rooms.list()
+all_rooms = bot.api.rooms.list()
 demo_rooms = [room for room in all_rooms if 'webexteamssdk Demo' in room.title]
 ```
 
 ##### local DB with [TinyDB](https://tinydb.readthedocs.io/en/latest/index.html) to remember things even after the bot is restarted
 
 ```python
 from webexbotsdk.teams import Bot
```

