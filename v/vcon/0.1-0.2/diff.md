# Comparing `tmp/vcon-0.1.tar.gz` & `tmp/vcon-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vcon-0.1.tar", last modified: Thu Apr 27 13:00:28 2023, max compression
+gzip compressed data, was "vcon-0.2.tar", last modified: Tue May 16 16:36:12 2023, max compression
```

## Comparing `vcon-0.1.tar` & `vcon-0.2.tar`

### file list

```diff
@@ -1,35 +1,38 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-27 13:00:28.843029 vcon-0.1/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1065 2023-04-24 03:53:08.000000 vcon-0.1/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5070 2023-04-27 13:00:28.843029 vcon-0.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3174 2023-04-24 03:53:08.000000 vcon-0.1/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1164 2023-04-27 13:00:07.000000 vcon-0.1/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-27 13:00:28.843029 vcon-0.1/setup.cfg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-27 13:00:28.839029 vcon-0.1/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1661 2023-04-24 03:53:08.000000 vcon-0.1/tests/test_dates.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7105 2023-04-24 03:53:08.000000 vcon-0.1/tests/test_external_content.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3359 2023-04-24 03:53:08.000000 vcon-0.1/tests/test_filter_plugins.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9802 2023-04-24 03:53:08.000000 vcon-0.1/tests/test_jwe.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      709 2023-04-24 03:53:08.000000 vcon-0.1/tests/test_migrate.py
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)    10388 2023-04-24 03:53:08.000000 vcon-0.1/tests/test_minimalist.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1278 2023-04-24 03:53:08.000000 vcon-0.1/tests/test_party_search.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1042 2023-04-27 11:20:38.000000 vcon-0.1/tests/test_redis_mgr.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13675 2023-04-24 03:53:08.000000 vcon-0.1/tests/test_signature.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1526 2023-04-24 03:53:08.000000 vcon-0.1/tests/test_uuid.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6940 2023-04-27 11:20:38.000000 vcon-0.1/tests/test_vcon_cli.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5893 2023-04-27 11:20:38.000000 vcon-0.1/tests/test_whisper_plugin.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-27 13:00:28.843029 vcon-0.1/vcon/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    50117 2023-04-24 03:53:08.000000 vcon-0.1/vcon/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14344 2023-04-24 03:53:08.000000 vcon-0.1/vcon/cli.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-27 13:00:28.843029 vcon-0.1/vcon/filter_plugins/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9693 2023-04-24 03:53:08.000000 vcon-0.1/vcon/filter_plugins/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-27 13:00:28.843029 vcon-0.1/vcon/filter_plugins/impl/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7194 2023-04-24 03:53:08.000000 vcon-0.1/vcon/filter_plugins/impl/whisper.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      413 2023-04-24 03:53:08.000000 vcon-0.1/vcon/filter_plugins/whisper.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14395 2023-04-24 03:53:08.000000 vcon-0.1/vcon/security.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3104 2023-04-24 03:53:08.000000 vcon-0.1/vcon/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-27 13:00:28.843029 vcon-0.1/vcon.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5070 2023-04-27 13:00:28.000000 vcon-0.1/vcon.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      621 2023-04-27 13:00:28.000000 vcon-0.1/vcon.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-27 13:00:28.000000 vcon-0.1/vcon.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      155 2023-04-27 13:00:28.000000 vcon-0.1/vcon.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        5 2023-04-27 13:00:28.000000 vcon-0.1/vcon.egg-info/top_level.txt
+drwxr-xr-x   0 dpetrie   (1001) dpetrie   (1001)        0 2023-05-16 16:36:12.354854 vcon-0.2/
+-rw-r--r--   0 dpetrie   (1001) dpetrie   (1001)     1065 2023-05-16 16:34:24.000000 vcon-0.2/LICENSE
+-rw-r--r--   0 dpetrie   (1001) dpetrie   (1001)      243 2023-05-16 16:36:12.354854 vcon-0.2/PKG-INFO
+-rw-r--r--   0 dpetrie   (1001) dpetrie   (1001)     3084 2023-05-16 16:35:10.000000 vcon-0.2/README.md
+-rw-r--r--   0 dpetrie   (1001) dpetrie   (1001)       38 2023-05-16 16:36:12.354854 vcon-0.2/setup.cfg
+-rw-r--r--   0 dpetrie   (1001) dpetrie   (1001)     1859 2023-05-16 16:34:25.000000 vcon-0.2/setup.py
+drwxr-xr-x   0 dpetrie   (1001) dpetrie   (1001)        0 2023-05-16 16:36:12.354854 vcon-0.2/tests/
+-rw-r--r--   0 dpetrie   (1001) dpetrie   (1001)     1661 2023-05-16 16:34:25.000000 vcon-0.2/tests/test_dates.py
+-rw-r--r--   0 dpetrie   (1001) dpetrie   (1001)     7105 2023-05-16 16:34:25.000000 vcon-0.2/tests/test_external_content.py
+-rw-r--r--   0 dpetrie   (1001) dpetrie   (1001)     3359 2023-05-16 16:34:25.000000 vcon-0.2/tests/test_filter_plugins.py
+-rw-r--r--   0 dpetrie   (1001) dpetrie   (1001)     9802 2023-05-16 16:34:25.000000 vcon-0.2/tests/test_jwe.py
+-rw-r--r--   0 dpetrie   (1001) dpetrie   (1001)      709 2023-05-16 16:34:25.000000 vcon-0.2/tests/test_migrate.py
+-rwxr-xr-x   0 dpetrie   (1001) dpetrie   (1001)    10388 2023-05-16 16:34:25.000000 vcon-0.2/tests/test_minimalist.py
+-rw-r--r--   0 dpetrie   (1001) dpetrie   (1001)     1278 2023-05-16 16:34:25.000000 vcon-0.2/tests/test_party_search.py
+-rw-r--r--   0 dpetrie   (1001) dpetrie   (1001)     1042 2023-05-16 16:35:10.000000 vcon-0.2/tests/test_redis_mgr.py
+-rw-r--r--   0 dpetrie   (1001) dpetrie   (1001)    13675 2023-05-16 16:34:25.000000 vcon-0.2/tests/test_signature.py
+-rw-r--r--   0 dpetrie   (1001) dpetrie   (1001)     1526 2023-05-16 16:34:25.000000 vcon-0.2/tests/test_uuid.py
+-rw-r--r--   0 dpetrie   (1001) dpetrie   (1001)     6940 2023-05-16 16:34:25.000000 vcon-0.2/tests/test_vcon_cli.py
+-rw-r--r--   0 dpetrie   (1001) dpetrie   (1001)     5893 2023-05-16 16:34:25.000000 vcon-0.2/tests/test_whisper_plugin.py
+drwxr-xr-x   0 dpetrie   (1001) dpetrie   (1001)        0 2023-05-16 16:36:12.354854 vcon-0.2/vcon/
+-rw-r--r--   0 dpetrie   (1001) dpetrie   (1001)    50137 2023-05-16 16:34:25.000000 vcon-0.2/vcon/__init__.py
+drwxr-xr-x   0 dpetrie   (1001) dpetrie   (1001)        0 2023-05-16 16:36:12.354854 vcon-0.2/vcon/bin/
+-rwxr-xr-x   0 dpetrie   (1001) dpetrie   (1001)      191 2023-05-16 16:34:25.000000 vcon-0.2/vcon/bin/vcon
+-rw-r--r--   0 dpetrie   (1001) dpetrie   (1001)    14344 2023-05-16 16:34:25.000000 vcon-0.2/vcon/cli.py
+drwxr-xr-x   0 dpetrie   (1001) dpetrie   (1001)        0 2023-05-16 16:36:12.354854 vcon-0.2/vcon/filter_plugins/
+-rw-r--r--   0 dpetrie   (1001) dpetrie   (1001)     9693 2023-05-16 16:34:25.000000 vcon-0.2/vcon/filter_plugins/__init__.py
+drwxr-xr-x   0 dpetrie   (1001) dpetrie   (1001)        0 2023-05-16 16:36:12.354854 vcon-0.2/vcon/filter_plugins/impl/
+-rw-r--r--   0 dpetrie   (1001) dpetrie   (1001)     7193 2023-05-16 16:34:25.000000 vcon-0.2/vcon/filter_plugins/impl/whisper.py
+-rw-r--r--   0 dpetrie   (1001) dpetrie   (1001)      413 2023-05-16 16:34:25.000000 vcon-0.2/vcon/filter_plugins/whisper.py
+-rw-r--r--   0 dpetrie   (1001) dpetrie   (1001)    14395 2023-05-16 16:34:25.000000 vcon-0.2/vcon/security.py
+-rw-r--r--   0 dpetrie   (1001) dpetrie   (1001)     3104 2023-05-16 16:34:25.000000 vcon-0.2/vcon/utils.py
+drwxr-xr-x   0 dpetrie   (1001) dpetrie   (1001)        0 2023-05-16 16:36:12.354854 vcon-0.2/vcon.egg-info/
+-rw-r--r--   0 dpetrie   (1001) dpetrie   (1001)      243 2023-05-16 16:36:12.000000 vcon-0.2/vcon.egg-info/PKG-INFO
+-rw-r--r--   0 dpetrie   (1001) dpetrie   (1001)      656 2023-05-16 16:36:12.000000 vcon-0.2/vcon.egg-info/SOURCES.txt
+-rw-r--r--   0 dpetrie   (1001) dpetrie   (1001)        1 2023-05-16 16:36:12.000000 vcon-0.2/vcon.egg-info/dependency_links.txt
+-rw-r--r--   0 dpetrie   (1001) dpetrie   (1001)        1 2023-05-16 16:36:12.000000 vcon-0.2/vcon.egg-info/not-zip-safe
+-rw-r--r--   0 dpetrie   (1001) dpetrie   (1001)      186 2023-05-16 16:36:12.000000 vcon-0.2/vcon.egg-info/requires.txt
+-rw-r--r--   0 dpetrie   (1001) dpetrie   (1001)        5 2023-05-16 16:36:12.000000 vcon-0.2/vcon.egg-info/top_level.txt
```

### Comparing `vcon-0.1/LICENSE` & `vcon-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vcon-0.1/README.md` & `vcon-0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -13,16 +13,14 @@
   + [Presentations, Whitepapers and Tutorials](#presentations-whitepapers-and-tutorials)
   + [vCon Library Quick Start for Python](https://github.com/vcon-dev/vcon/wiki/Library-Quick-Start)
   + [Testing the Vcon Package](#testing-the-vcon-package)
   + [Testing the conserver](#testing-the-conserver)
 
 ## Presentations, Whitepapers and Tutorials
 
-See the [Birds of a Feather session at IETF 116, Yokohama](https://youtu.be/EF2OMbo6Qj4)
-
 See the [presentation at TADSummit](https://youtu.be/ZBRJ6FcVblc)
 
 See the [presentation at IETF](https://youtu.be/dJsPzZITr_g?t=243)
 
 See the [presentation at IIT](https://youtu.be/s-pjgpBOQqc)
 
 Read the [IETF draft proposal](https://datatracker.ietf.org/doc/html/draft-petrie-vcon-01)
```

### Comparing `vcon-0.1/tests/test_dates.py` & `vcon-0.2/tests/test_dates.py`

 * *Files identical despite different names*

### Comparing `vcon-0.1/tests/test_external_content.py` & `vcon-0.2/tests/test_external_content.py`

 * *Files identical despite different names*

### Comparing `vcon-0.1/tests/test_filter_plugins.py` & `vcon-0.2/tests/test_filter_plugins.py`

 * *Files identical despite different names*

### Comparing `vcon-0.1/tests/test_jwe.py` & `vcon-0.2/tests/test_jwe.py`

 * *Files identical despite different names*

### Comparing `vcon-0.1/tests/test_migrate.py` & `vcon-0.2/tests/test_migrate.py`

 * *Files identical despite different names*

### Comparing `vcon-0.1/tests/test_minimalist.py` & `vcon-0.2/tests/test_minimalist.py`

 * *Files identical despite different names*

### Comparing `vcon-0.1/tests/test_party_search.py` & `vcon-0.2/tests/test_party_search.py`

 * *Files identical despite different names*

### Comparing `vcon-0.1/tests/test_redis_mgr.py` & `vcon-0.2/tests/test_redis_mgr.py`

 * *Files identical despite different names*

### Comparing `vcon-0.1/tests/test_signature.py` & `vcon-0.2/tests/test_signature.py`

 * *Files identical despite different names*

### Comparing `vcon-0.1/tests/test_uuid.py` & `vcon-0.2/tests/test_uuid.py`

 * *Files identical despite different names*

### Comparing `vcon-0.1/tests/test_vcon_cli.py` & `vcon-0.2/tests/test_vcon_cli.py`

 * *Files identical despite different names*

### Comparing `vcon-0.1/tests/test_whisper_plugin.py` & `vcon-0.2/tests/test_whisper_plugin.py`

 * *Files identical despite different names*

### Comparing `vcon-0.1/vcon/__init__.py` & `vcon-0.2/vcon/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import typing
 import sys
 import os
 import logging
 import logging.config
 import pythonjsonlogger.jsonlogger
 
+__version__ = "0.2"
 
 def build_logger(name : str) -> logging.Logger:
   logger = logging.getLogger(name)
 
   log_config_filename = "./logging.conf"
   if(os.path.isfile(log_config_filename)):
     logging.config.fileConfig(log_config_filename)
```

### Comparing `vcon-0.1/vcon/cli.py` & `vcon-0.2/vcon/cli.py`

 * *Files identical despite different names*

### Comparing `vcon-0.1/vcon/filter_plugins/__init__.py` & `vcon-0.2/vcon/filter_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `vcon-0.1/vcon/filter_plugins/impl/whisper.py` & `vcon-0.2/vcon/filter_plugins/impl/whisper.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 logger = vcon.build_logger(__name__)
 
 try:
   import stable_whisper
 except Exception as e:
   #patch_url = "https://raw.githubusercontent.com/jianfch/stable-ts/main/stable_whisper.py"
   #print("Please download and install stable_whipser from: {}".format(patch_url))
-  cwlogger.info("please install stable_whisper:  \"pip3 install stble-ts\"")
+  logger.info("please install stable_whisper:  \"pip3 install stable-ts\"")
   raise e
 
 class Whisper(vcon.filter_plugins.FilterPlugin):
   """
   PluginFilter to generate transcriptions for a Von
   """
   _supported_media = [ vcon.Vcon.MIMETYPE_AUDIO_WAV ]
```

### Comparing `vcon-0.1/vcon/security.py` & `vcon-0.2/vcon/security.py`

 * *Files identical despite different names*

### Comparing `vcon-0.1/vcon/utils.py` & `vcon-0.2/vcon/utils.py`

 * *Files identical despite different names*

### Comparing `vcon-0.1/vcon.egg-info/SOURCES.txt` & `vcon-0.2/vcon.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 LICENSE
 README.md
-pyproject.toml
+setup.py
 tests/test_dates.py
 tests/test_external_content.py
 tests/test_filter_plugins.py
 tests/test_jwe.py
 tests/test_migrate.py
 tests/test_minimalist.py
 tests/test_party_search.py
@@ -16,12 +16,14 @@
 vcon/__init__.py
 vcon/cli.py
 vcon/security.py
 vcon/utils.py
 vcon.egg-info/PKG-INFO
 vcon.egg-info/SOURCES.txt
 vcon.egg-info/dependency_links.txt
+vcon.egg-info/not-zip-safe
 vcon.egg-info/requires.txt
 vcon.egg-info/top_level.txt
+vcon/bin/vcon
 vcon/filter_plugins/__init__.py
 vcon/filter_plugins/whisper.py
 vcon/filter_plugins/impl/whisper.py
```

