# Comparing `tmp/rum_with_telegram-1.0.2.tar.gz` & `tmp/rum_with_telegram-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rum_with_telegram-1.0.2.tar", last modified: Sat May 13 14:00:11 2023, max compression
+gzip compressed data, was "rum_with_telegram-1.0.3.tar", last modified: Tue May 16 11:41:22 2023, max compression
```

## Comparing `rum_with_telegram-1.0.2.tar` & `rum_with_telegram-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-13 14:00:11.130677 rum_with_telegram-1.0.2/
--rw-rw-rw-   0        0        0     1087 2023-03-22 04:17:54.000000 rum_with_telegram-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     1032 2023-05-13 14:00:11.129679 rum_with_telegram-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       19 2023-03-22 04:17:54.000000 rum_with_telegram-1.0.2/README.md
--rw-rw-rw-   0        0        0      163 2023-04-25 07:27:09.000000 rum_with_telegram-1.0.2/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-13 14:00:11.116714 rum_with_telegram-1.0.2/rum_with_telegram/
--rw-rw-rw-   0        0        0      215 2023-05-13 13:58:38.000000 rum_with_telegram-1.0.2/rum_with_telegram/__init__.py
--rw-rw-rw-   0        0        0     2092 2023-05-13 13:53:34.000000 rum_with_telegram-1.0.2/rum_with_telegram/config.py
--rw-rw-rw-   0        0        0    26650 2023-05-13 13:58:57.000000 rum_with_telegram-1.0.2/rum_with_telegram/data_exchanger.py
--rw-rw-rw-   0        0        0     3872 2023-05-12 03:14:44.000000 rum_with_telegram-1.0.2/rum_with_telegram/db_handle.py
--rw-rw-rw-   0        0        0     1820 2023-05-12 03:02:22.000000 rum_with_telegram-1.0.2/rum_with_telegram/module.py
-drwxrwxrwx   0        0        0        0 2023-05-13 14:00:11.127694 rum_with_telegram-1.0.2/rum_with_telegram.egg-info/
--rw-rw-rw-   0        0        0     1032 2023-05-13 14:00:11.000000 rum_with_telegram-1.0.2/rum_with_telegram.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      398 2023-05-13 14:00:11.000000 rum_with_telegram-1.0.2/rum_with_telegram.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-13 14:00:11.000000 rum_with_telegram-1.0.2/rum_with_telegram.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2023-05-13 14:00:11.000000 rum_with_telegram-1.0.2/rum_with_telegram.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-05-13 14:00:11.000000 rum_with_telegram-1.0.2/rum_with_telegram.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-13 14:00:11.130677 rum_with_telegram-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1430 2023-05-13 13:58:38.000000 rum_with_telegram-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 11:41:22.267161 rum_with_telegram-1.0.3/
+-rw-rw-rw-   0        0        0     1087 2023-03-22 04:17:54.000000 rum_with_telegram-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1032 2023-05-16 11:41:22.266163 rum_with_telegram-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       19 2023-03-22 04:17:54.000000 rum_with_telegram-1.0.3/README.md
+-rw-rw-rw-   0        0        0      163 2023-04-25 07:27:09.000000 rum_with_telegram-1.0.3/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-16 11:41:22.252200 rum_with_telegram-1.0.3/rum_with_telegram/
+-rw-rw-rw-   0        0        0      215 2023-05-16 11:25:24.000000 rum_with_telegram-1.0.3/rum_with_telegram/__init__.py
+-rw-rw-rw-   0        0        0     2092 2023-05-13 13:53:34.000000 rum_with_telegram-1.0.3/rum_with_telegram/config.py
+-rw-rw-rw-   0        0        0    26650 2023-05-16 11:25:31.000000 rum_with_telegram-1.0.3/rum_with_telegram/data_exchanger.py
+-rw-rw-rw-   0        0        0     3872 2023-05-14 08:49:50.000000 rum_with_telegram-1.0.3/rum_with_telegram/db_handle.py
+-rw-rw-rw-   0        0        0     1820 2023-05-12 03:02:22.000000 rum_with_telegram-1.0.3/rum_with_telegram/module.py
+drwxrwxrwx   0        0        0        0 2023-05-16 11:41:22.263173 rum_with_telegram-1.0.3/rum_with_telegram.egg-info/
+-rw-rw-rw-   0        0        0     1032 2023-05-16 11:41:22.000000 rum_with_telegram-1.0.3/rum_with_telegram.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      398 2023-05-16 11:41:22.000000 rum_with_telegram-1.0.3/rum_with_telegram.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 11:41:22.000000 rum_with_telegram-1.0.3/rum_with_telegram.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2023-05-16 11:41:22.000000 rum_with_telegram-1.0.3/rum_with_telegram.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-16 11:41:22.000000 rum_with_telegram-1.0.3/rum_with_telegram.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-16 11:41:22.267161 rum_with_telegram-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1430 2023-05-16 11:25:24.000000 rum_with_telegram-1.0.3/setup.py
```

### Comparing `rum_with_telegram-1.0.2/LICENSE` & `rum_with_telegram-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rum_with_telegram-1.0.2/PKG-INFO` & `rum_with_telegram-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rum_with_telegram
-Version: 1.0.2
+Version: 1.0.3
 Summary: A bot, send telegram update to rum group as trx, and get new trx from rum group to channel.
 Home-page: https://github.com/liujuanjuan1984/rum_with_telegram
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/rum_with_telegram
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/rum_with_telegram/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `rum_with_telegram-1.0.2/rum_with_telegram/config.py` & `rum_with_telegram-1.0.3/rum_with_telegram/config.py`

 * *Files identical despite different names*

### Comparing `rum_with_telegram-1.0.2/rum_with_telegram/data_exchanger.py` & `rum_with_telegram-1.0.3/rum_with_telegram/data_exchanger.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,15 @@
         _trx_id = self.start_trx
         while True:
             if self.start_trx != _trx_id:
                 logger.info("handle_rum %s", self.start_trx)
                 _trx_id = self.start_trx
             start_trx = await self._handle_rum(self.start_trx)
             if start_trx == self.start_trx:
-                await asyncio.sleep(5)
+                await asyncio.sleep(1)
             self.start_trx = start_trx
 
     async def _handle_rum(self, start_trx):
         trxs = self.rum.api.get_content(num=20, start_trx=start_trx)
         for trx in trxs:
             start_trx = trx["TrxId"]
             if self.config.POST_AUTH_TYPE == "whitelist":
```

### Comparing `rum_with_telegram-1.0.2/rum_with_telegram/db_handle.py` & `rum_with_telegram-1.0.3/rum_with_telegram/db_handle.py`

 * *Files identical despite different names*

### Comparing `rum_with_telegram-1.0.2/rum_with_telegram/module.py` & `rum_with_telegram-1.0.3/rum_with_telegram/module.py`

 * *Files identical despite different names*

### Comparing `rum_with_telegram-1.0.2/rum_with_telegram.egg-info/PKG-INFO` & `rum_with_telegram-1.0.3/rum_with_telegram.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rum-with-telegram
-Version: 1.0.2
+Version: 1.0.3
 Summary: A bot, send telegram update to rum group as trx, and get new trx from rum group to channel.
 Home-page: https://github.com/liujuanjuan1984/rum_with_telegram
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/rum_with_telegram
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/rum_with_telegram/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `rum_with_telegram-1.0.2/setup.py` & `rum_with_telegram-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="rum_with_telegram",
-    version="1.0.2",
+    version="1.0.3",
     author="liujuanjuan1984",
     author_email="qiaoanlu@163.com",
     description="A bot, send telegram update to rum group as trx, and get new trx from rum group to channel.",
     keywords=["python-telegram-bot", "rumsystem", "quorum"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/liujuanjuan1984/rum_with_telegram",
```

