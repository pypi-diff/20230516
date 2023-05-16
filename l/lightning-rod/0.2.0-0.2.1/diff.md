# Comparing `tmp/lightning_rod-0.2.0.tar.gz` & `tmp/lightning_rod-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightning_rod-0.2.0.tar", max compression
+gzip compressed data, was "lightning_rod-0.2.1.tar", max compression
```

## Comparing `lightning_rod-0.2.0.tar` & `lightning_rod-0.2.1.tar`

### file list

```diff
@@ -1,24 +1,23 @@
--rw-r--r--   0        0        0     1061 2023-05-08 17:00:33.408771 lightning_rod-0.2.0/LICENSE
--rw-r--r--   0        0        0      347 2023-05-08 17:00:33.408771 lightning_rod-0.2.0/README.md
--rw-r--r--   0        0        0      307 2023-05-08 17:01:07.385005 lightning_rod-0.2.0/lightning_rod/__init__.py
--rw-r--r--   0        0        0      667 2023-05-08 17:00:33.408771 lightning_rod-0.2.0/lightning_rod/modules/advancement.bolt
--rw-r--r--   0        0        0      601 2023-05-08 17:00:33.408771 lightning_rod-0.2.0/lightning_rod/modules/api.bolt
--rw-r--r--   0        0        0     4614 2023-05-08 17:00:33.408771 lightning_rod-0.2.0/lightning_rod/modules/bossbar.bolt
--rw-r--r--   0        0        0       36 2023-05-08 17:00:33.408771 lightning_rod-0.2.0/lightning_rod/modules/cancel_momentum.bolt
--rw-r--r--   0        0        0      314 2023-05-08 17:00:33.408771 lightning_rod-0.2.0/lightning_rod/modules/clear.bolt
--rw-r--r--   0        0        0       85 2023-05-08 17:00:33.408771 lightning_rod-0.2.0/lightning_rod/modules/comment.bolt
--rw-r--r--   0        0        0      144 2023-05-08 17:00:33.408771 lightning_rod-0.2.0/lightning_rod/modules/config.bolt
--rw-r--r--   0        0        0     1593 2023-05-08 17:00:33.408771 lightning_rod-0.2.0/lightning_rod/modules/effect.bolt
--rw-r--r--   0        0        0      581 2023-05-08 17:00:33.408771 lightning_rod-0.2.0/lightning_rod/modules/gamemode.bolt
--rw-r--r--   0        0        0      157 2023-05-08 17:00:33.408771 lightning_rod-0.2.0/lightning_rod/modules/give.bolt
--rw-r--r--   0        0        0       25 2023-05-08 17:00:33.408771 lightning_rod-0.2.0/lightning_rod/modules/kill.bolt
--rw-r--r--   0        0        0     2418 2023-05-08 17:00:33.408771 lightning_rod-0.2.0/lightning_rod/modules/math.bolt
--rw-r--r--   0        0        0       35 2023-05-08 17:00:33.408771 lightning_rod-0.2.0/lightning_rod/modules/raw_cmd.bolt
--rw-r--r--   0        0        0      374 2023-05-08 17:00:33.412771 lightning_rod-0.2.0/lightning_rod/modules/rebindable.bolt
--rw-r--r--   0        0        0       86 2023-05-08 17:00:33.412771 lightning_rod-0.2.0/lightning_rod/modules/tag.bolt
--rw-r--r--   0        0        0     1047 2023-05-08 17:00:33.412771 lightning_rod-0.2.0/lightning_rod/modules/time.bolt
--rw-r--r--   0        0        0      300 2023-05-08 17:00:33.412771 lightning_rod-0.2.0/lightning_rod/modules/utils.bolt
--rw-r--r--   0        0        0     2111 2023-05-08 17:00:33.412771 lightning_rod-0.2.0/lightning_rod/modules/xp.bolt
--rw-r--r--   0        0        0        0 2023-05-08 17:00:33.412771 lightning_rod-0.2.0/lightning_rod/py.typed
--rw-r--r--   0        0        0     1238 2023-05-08 17:01:07.401005 lightning_rod-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1111 1970-01-01 00:00:00.000000 lightning_rod-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-05-16 00:00:57.202941 lightning_rod-0.2.1/LICENSE
+-rw-r--r--   0        0        0      347 2023-05-16 00:00:57.202941 lightning_rod-0.2.1/README.md
+-rw-r--r--   0        0        0      307 2023-05-16 00:01:44.315218 lightning_rod-0.2.1/lightning_rod/__init__.py
+-rw-r--r--   0        0        0      667 2023-05-16 00:00:57.206941 lightning_rod-0.2.1/lightning_rod/modules/advancement.bolt
+-rw-r--r--   0        0        0      565 2023-05-16 00:00:57.206941 lightning_rod-0.2.1/lightning_rod/modules/api.bolt
+-rw-r--r--   0        0        0     4590 2023-05-16 00:00:57.206941 lightning_rod-0.2.1/lightning_rod/modules/bossbar.bolt
+-rw-r--r--   0        0        0       38 2023-05-16 00:00:57.206941 lightning_rod-0.2.1/lightning_rod/modules/cancel_momentum.bolt
+-rw-r--r--   0        0        0      314 2023-05-16 00:00:57.206941 lightning_rod-0.2.1/lightning_rod/modules/clear.bolt
+-rw-r--r--   0        0        0       85 2023-05-16 00:00:57.206941 lightning_rod-0.2.1/lightning_rod/modules/comment.bolt
+-rw-r--r--   0        0        0      144 2023-05-16 00:00:57.206941 lightning_rod-0.2.1/lightning_rod/modules/config.bolt
+-rw-r--r--   0        0        0     1593 2023-05-16 00:00:57.206941 lightning_rod-0.2.1/lightning_rod/modules/effect.bolt
+-rw-r--r--   0        0        0      581 2023-05-16 00:00:57.206941 lightning_rod-0.2.1/lightning_rod/modules/gamemode.bolt
+-rw-r--r--   0        0        0      157 2023-05-16 00:00:57.206941 lightning_rod-0.2.1/lightning_rod/modules/give.bolt
+-rw-r--r--   0        0        0       25 2023-05-16 00:00:57.206941 lightning_rod-0.2.1/lightning_rod/modules/kill.bolt
+-rw-r--r--   0        0        0     2418 2023-05-16 00:00:57.206941 lightning_rod-0.2.1/lightning_rod/modules/math.bolt
+-rw-r--r--   0        0        0       35 2023-05-16 00:00:57.206941 lightning_rod-0.2.1/lightning_rod/modules/raw_cmd.bolt
+-rw-r--r--   0        0        0       86 2023-05-16 00:00:57.206941 lightning_rod-0.2.1/lightning_rod/modules/tag.bolt
+-rw-r--r--   0        0        0     1047 2023-05-16 00:00:57.206941 lightning_rod-0.2.1/lightning_rod/modules/time.bolt
+-rw-r--r--   0        0        0      300 2023-05-16 00:00:57.206941 lightning_rod-0.2.1/lightning_rod/modules/utils.bolt
+-rw-r--r--   0        0        0     2111 2023-05-16 00:00:57.206941 lightning_rod-0.2.1/lightning_rod/modules/xp.bolt
+-rw-r--r--   0        0        0        0 2023-05-16 00:00:57.206941 lightning_rod-0.2.1/lightning_rod/py.typed
+-rw-r--r--   0        0        0     1242 2023-05-16 00:01:44.339218 lightning_rod-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1080 1970-01-01 00:00:00.000000 lightning_rod-0.2.1/PKG-INFO
```

### Comparing `lightning_rod-0.2.0/LICENSE` & `lightning_rod-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lightning_rod-0.2.0/lightning_rod/modules/advancement.bolt` & `lightning_rod-0.2.1/lightning_rod/modules/advancement.bolt`

 * *Files identical despite different names*

### Comparing `lightning_rod-0.2.0/lightning_rod/modules/api.bolt` & `lightning_rod-0.2.1/lightning_rod/modules/api.bolt`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from ./raw_cmd import raw_cmd
 from ./advancement import grant_advancement, revoke_advancement
 from ./bossbar import Bossbar
 from ./tag import tag, untag
-from ./rebindable import Rebindable
 from ./kill import kill
 from ./cancel_momentum import cancel_momentum
 from ./effect import effect, raw_effect
 from ./give import give
 from ./clear import clear
 from ./gamemode import get_gamemode, set_gamemode
 from ./math import random, sqrt, pow
```

### Comparing `lightning_rod-0.2.0/lightning_rod/modules/bossbar.bolt` & `lightning_rod-0.2.1/lightning_rod/modules/bossbar.bolt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from typing import ClassVar
 from dataclasses import dataclass
 
-from wicked_expressions:api import StaticVar, Int, ExpressionNode
-from ./rebindable import Rebindable
+from wicked_expressions:api import StaticVar, Int, ExpressionNode, Rebindable
 from ./utils import logger
 from ./raw_cmd import raw_cmd
 from ./tag import tag, untag
 from ./config import Config
 
 import inspect
```

### Comparing `lightning_rod-0.2.0/lightning_rod/modules/effect.bolt` & `lightning_rod-0.2.1/lightning_rod/modules/effect.bolt`

 * *Files identical despite different names*

### Comparing `lightning_rod-0.2.0/lightning_rod/modules/gamemode.bolt` & `lightning_rod-0.2.1/lightning_rod/modules/gamemode.bolt`

 * *Files identical despite different names*

### Comparing `lightning_rod-0.2.0/lightning_rod/modules/math.bolt` & `lightning_rod-0.2.1/lightning_rod/modules/math.bolt`

 * *Files identical despite different names*

### Comparing `lightning_rod-0.2.0/lightning_rod/modules/time.bolt` & `lightning_rod-0.2.1/lightning_rod/modules/time.bolt`

 * *Files identical despite different names*

### Comparing `lightning_rod-0.2.0/lightning_rod/modules/xp.bolt` & `lightning_rod-0.2.1/lightning_rod/modules/xp.bolt`

 * *Files identical despite different names*

### Comparing `lightning_rod-0.2.0/pyproject.toml` & `lightning_rod-0.2.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lightning_rod"
-version = "0.2.0"
+version = "0.2.1"
 description = "Function library for the Bolt scripting language."
 authors = ["ArcticYeti <arcticyeti1@gmail.com>"]
 license = "MIT"
 
 homepage = "https://github.com/reapermc/lightning-rod"
 readme = "README.md"
 
@@ -19,18 +19,18 @@
   "reapermc",
 ]
 
 include = ["lightning_rod/py.typed"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-beet = "^0.84.0"
-mecha = "^0.67.0"
-bolt = "^0.31.0"
-wicked-expressions = "^0.5.2"
+beet = ">=0.84.0"
+mecha = ">=0.67.0"
+bolt = ">=0.31.0"
+wicked-expressions = ">=0.6.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1.3"
 black = "^22.10.0"
 isort = "^5.10.1"
 pytest-insta = "^0.1.11"
 lectern = ">=0.25.0"
```

### Comparing `lightning_rod-0.2.0/PKG-INFO` & `lightning_rod-0.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: lightning-rod
-Version: 0.2.0
+Version: 0.2.1
 Summary: Function library for the Bolt scripting language.
 Home-page: https://github.com/reapermc/lightning-rod
 License: MIT
 Keywords: beet,bolt,minecraft,datapack,minecraft-commands,mcfunction,library,reapermc
 Author: ArcticYeti
 Author-email: arcticyeti1@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: beet (>=0.84.0,<0.85.0)
-Requires-Dist: bolt (>=0.31.0,<0.32.0)
-Requires-Dist: mecha (>=0.67.0,<0.68.0)
-Requires-Dist: wicked-expressions (>=0.5.2,<0.6.0)
+Requires-Dist: beet (>=0.84.0)
+Requires-Dist: bolt (>=0.31.0)
+Requires-Dist: mecha (>=0.67.0)
+Requires-Dist: wicked-expressions (>=0.6.0)
 Description-Content-Type: text/markdown
 
 # lightning-rod
 
 [![GitHub Actions](https://github.com/reapermc/lightning-rod/workflows/CI/badge.svg)](https://github.com/reapermc/lightning-rod/actions)
 
 > Function library for the Bolt scripting language.
```

