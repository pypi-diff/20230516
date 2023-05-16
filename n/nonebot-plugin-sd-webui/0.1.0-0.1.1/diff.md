# Comparing `tmp/nonebot_plugin_sd_webui-0.1.0.tar.gz` & `tmp/nonebot_plugin_sd_webui-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_sd_webui-0.1.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_sd_webui-0.1.1.tar", max compression
```

## Comparing `nonebot_plugin_sd_webui-0.1.0.tar` & `nonebot_plugin_sd_webui-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1087 2023-05-16 05:38:13.204378 nonebot_plugin_sd_webui-0.1.0/LICENSE
--rw-r--r--   0        0        0    11352 2023-05-16 02:48:16.236280 nonebot_plugin_sd_webui-0.1.0/nonebot_plugin_sd_webui/__init__.py
--rw-r--r--   0        0        0      860 2023-05-16 02:48:16.237205 nonebot_plugin_sd_webui-0.1.0/nonebot_plugin_sd_webui/config.py
--rw-r--r--   0        0        0      405 2023-05-16 06:45:36.500218 nonebot_plugin_sd_webui-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4291 2023-05-16 06:02:41.998378 nonebot_plugin_sd_webui-0.1.0/README.md
--rw-r--r--   0        0        0     4889 1970-01-01 00:00:00.000000 nonebot_plugin_sd_webui-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1087 2023-05-16 05:38:13.204378 nonebot_plugin_sd_webui-0.1.1/LICENSE
+-rw-r--r--   0        0        0    11352 2023-05-16 02:48:16.236280 nonebot_plugin_sd_webui-0.1.1/nonebot_plugin_sd_webui/__init__.py
+-rw-r--r--   0        0        0      860 2023-05-16 02:48:16.237205 nonebot_plugin_sd_webui-0.1.1/nonebot_plugin_sd_webui/config.py
+-rw-r--r--   0        0        0      528 2023-05-16 07:44:52.270606 nonebot_plugin_sd_webui-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4291 2023-05-16 06:02:41.998378 nonebot_plugin_sd_webui-0.1.1/README.md
+-rw-r--r--   0        0        0     5006 1970-01-01 00:00:00.000000 nonebot_plugin_sd_webui-0.1.1/PKG-INFO
```

### Comparing `nonebot_plugin_sd_webui-0.1.0/LICENSE` & `nonebot_plugin_sd_webui-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sd_webui-0.1.0/nonebot_plugin_sd_webui/__init__.py` & `nonebot_plugin_sd_webui-0.1.1/nonebot_plugin_sd_webui/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sd_webui-0.1.0/nonebot_plugin_sd_webui/config.py` & `nonebot_plugin_sd_webui-0.1.1/nonebot_plugin_sd_webui/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sd_webui-0.1.0/README.md` & `nonebot_plugin_sd_webui-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sd_webui-0.1.0/PKG-INFO` & `nonebot_plugin_sd_webui-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-sd-webui
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 License: MIT
 Author: evan-gyy
 Author-email: evangu1104@foxmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: requests (>=2.30.0,<3.0.0)
-Requires-Dist: webuiapi (>=0.7.0,<0.8.0)
+Requires-Dist: nonebot-adapter-onebot (>=2.0.0-beta.1,<3.0.0)
+Requires-Dist: nonebot-plugin-guild-patch
+Requires-Dist: nonebot2 (>=2.0.0-beta.1,<3.0.0)
+Requires-Dist: requests
+Requires-Dist: webuiapi
 Description-Content-Type: text/markdown
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
 </div>
```

#### html2text {}

```diff
@@ -1,15 +1,17 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-sd-webui Version: 0.1.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-sd-webui Version: 0.1.1 Summary:
 License: MIT Author: evan-gyy Author-email: evangu1104@foxmail.com Requires-
 Python: >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Requires-Dist: requests (>=2.30.0,<3.0.0) Requires-
-Dist: webuiapi (>=0.7.0,<0.8.0) Description-Content-Type: text/markdown
+Language :: Python :: 3.11 Requires-Dist: nonebot-adapter-onebot (>=2.0.0-
+beta.1,<3.0.0) Requires-Dist: nonebot-plugin-guild-patch Requires-Dist:
+nonebot2 (>=2.0.0-beta.1,<3.0.0) Requires-Dist: requests Requires-Dist:
+webuiapi Description-Content-Type: text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
             # nonebot_plugin_sd_webui _â¨ åºäºstable-diffusion-
 webuiçnonebotç»ç»æä»¶ â¨_ [GitHub_stars] [GitHub_issues] [GitHub_forks]
                            [license] [pypi] [python]
 ## ð ä»ç» nonebotç»ç»æä»¶ï¼åºäºsd-
 webuiå®ç°ï¼æ¯ææå®æ¨¡åãåæ°ç­ ## ð§ å¼åç¯å¢
```

