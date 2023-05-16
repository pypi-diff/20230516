# Comparing `tmp/gameyamlspiderandgenerator-1.4.3.tar.gz` & `tmp/gameyamlspiderandgenerator-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gameyamlspiderandgenerator-1.4.3.tar", max compression
+gzip compressed data, was "gameyamlspiderandgenerator-1.4.4.tar", max compression
```

## Comparing `gameyamlspiderandgenerator-1.4.3.tar` & `gameyamlspiderandgenerator-1.4.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rwxr-xr-x   0        0        0     1069 2023-05-05 11:54:39.050499 gameyamlspiderandgenerator-1.4.3/LICENSE
--rwxr-xr-x   0        0        0     1321 2023-05-05 11:54:39.050733 gameyamlspiderandgenerator-1.4.3/README.md
--rwxr-xr-x   0        0        0      568 2023-05-05 11:54:39.052482 gameyamlspiderandgenerator-1.4.3/gameyamlspiderandgenerator/__init__.py
--rwxr-xr-x   0        0        0     1751 2023-05-05 11:54:39.052734 gameyamlspiderandgenerator-1.4.3/gameyamlspiderandgenerator/__main__.py
--rwxr-xr-x   0        0        0      753 2023-05-05 11:54:39.052963 gameyamlspiderandgenerator-1.4.3/gameyamlspiderandgenerator/exception.py
--rwxr-xr-x   0        0        0       52 2023-05-05 11:54:39.054143 gameyamlspiderandgenerator-1.4.3/gameyamlspiderandgenerator/hook/__init__.py
--rwxr-xr-x   0        0        0      210 2023-05-05 14:42:52.343793 gameyamlspiderandgenerator-1.4.3/gameyamlspiderandgenerator/hook/_base.py
--rwxr-xr-x   0        0        0     3694 2023-05-05 14:46:20.255955 gameyamlspiderandgenerator-1.4.3/gameyamlspiderandgenerator/hook/search.py
--rwxr-xr-x   0        0        0      582 2023-05-05 14:42:52.437426 gameyamlspiderandgenerator-1.4.3/gameyamlspiderandgenerator/hook/validate.py
--rwxr-xr-x   0        0        0       56 2023-05-05 11:54:39.055255 gameyamlspiderandgenerator-1.4.3/gameyamlspiderandgenerator/plugin/__init__.py
--rwxr-xr-x   0        0        0     2606 2023-05-05 14:47:46.986045 gameyamlspiderandgenerator-1.4.3/gameyamlspiderandgenerator/plugin/_base.py
--rwxr-xr-x   0        0        0     7167 2023-05-05 14:39:08.986302 gameyamlspiderandgenerator-1.4.3/gameyamlspiderandgenerator/plugin/itchio.py
--rwxr-xr-x   0        0        0     7700 2023-05-05 14:39:08.992543 gameyamlspiderandgenerator-1.4.3/gameyamlspiderandgenerator/plugin/steam.py
--rwxr-xr-x   0        0        0        0 2023-05-05 11:54:39.056470 gameyamlspiderandgenerator-1.4.3/gameyamlspiderandgenerator/util/__init__.py
--rwxr-xr-x   0        0        0     1461 2023-05-05 11:54:39.056789 gameyamlspiderandgenerator-1.4.3/gameyamlspiderandgenerator/util/config.py
--rwxr-xr-x   0        0        0     1472 2023-05-05 14:39:08.993151 gameyamlspiderandgenerator-1.4.3/gameyamlspiderandgenerator/util/fgi.py
--rwxr-xr-x   0        0        0     1953 2023-05-05 14:39:08.995558 gameyamlspiderandgenerator-1.4.3/gameyamlspiderandgenerator/util/fgi_yaml.py
--rwxr-xr-x   0        0        0     1944 2023-05-05 11:54:39.057708 gameyamlspiderandgenerator-1.4.3/gameyamlspiderandgenerator/util/plugin_manager.py
--rwxr-xr-x   0        0        0     2611 2023-05-05 11:54:39.066258 gameyamlspiderandgenerator-1.4.3/gameyamlspiderandgenerator/util/spider.py
--rwxr-xr-x   0        0        0      700 2023-05-05 14:48:55.735977 gameyamlspiderandgenerator-1.4.3/pyproject.toml
--rw-r--r--   0        0        0     2408 1970-01-01 00:00:00.000000 gameyamlspiderandgenerator-1.4.3/PKG-INFO
+-rwxr-xr-x   0        0        0     1069 2023-05-05 11:54:39.050499 gameyamlspiderandgenerator-1.4.4/LICENSE
+-rwxr-xr-x   0        0        0     1321 2023-05-05 11:54:39.050733 gameyamlspiderandgenerator-1.4.4/README.md
+-rwxr-xr-x   0        0        0      568 2023-05-05 11:54:39.052482 gameyamlspiderandgenerator-1.4.4/gameyamlspiderandgenerator/__init__.py
+-rwxr-xr-x   0        0        0     1751 2023-05-05 11:54:39.052734 gameyamlspiderandgenerator-1.4.4/gameyamlspiderandgenerator/__main__.py
+-rwxr-xr-x   0        0        0      753 2023-05-05 11:54:39.052963 gameyamlspiderandgenerator-1.4.4/gameyamlspiderandgenerator/exception.py
+-rwxr-xr-x   0        0        0       52 2023-05-05 11:54:39.054143 gameyamlspiderandgenerator-1.4.4/gameyamlspiderandgenerator/hook/__init__.py
+-rwxr-xr-x   0        0        0      235 2023-05-15 23:17:15.527274 gameyamlspiderandgenerator-1.4.4/gameyamlspiderandgenerator/hook/_base.py
+-rwxr-xr-x   0        0        0     3721 2023-05-15 23:18:06.030212 gameyamlspiderandgenerator-1.4.4/gameyamlspiderandgenerator/hook/search.py
+-rwxr-xr-x   0        0        0      560 2023-05-15 23:18:51.608508 gameyamlspiderandgenerator-1.4.4/gameyamlspiderandgenerator/hook/validate.py
+-rwxr-xr-x   0        0        0       56 2023-05-05 11:54:39.055255 gameyamlspiderandgenerator-1.4.4/gameyamlspiderandgenerator/plugin/__init__.py
+-rwxr-xr-x   0        0        0     2722 2023-05-16 00:58:45.661904 gameyamlspiderandgenerator-1.4.4/gameyamlspiderandgenerator/plugin/_base.py
+-rwxr-xr-x   0        0        0     7203 2023-05-14 14:53:55.250700 gameyamlspiderandgenerator-1.4.4/gameyamlspiderandgenerator/plugin/itchio.py
+-rwxr-xr-x   0        0        0     7700 2023-05-05 14:39:08.992543 gameyamlspiderandgenerator-1.4.4/gameyamlspiderandgenerator/plugin/steam.py
+-rwxr-xr-x   0        0        0        0 2023-05-05 11:54:39.056470 gameyamlspiderandgenerator-1.4.4/gameyamlspiderandgenerator/util/__init__.py
+-rwxr-xr-x   0        0        0     1461 2023-05-05 11:54:39.056789 gameyamlspiderandgenerator-1.4.4/gameyamlspiderandgenerator/util/config.py
+-rwxr-xr-x   0        0        0     1472 2023-05-05 14:39:08.993151 gameyamlspiderandgenerator-1.4.4/gameyamlspiderandgenerator/util/fgi.py
+-rwxr-xr-x   0        0        0     1953 2023-05-05 14:39:08.995558 gameyamlspiderandgenerator-1.4.4/gameyamlspiderandgenerator/util/fgi_yaml.py
+-rwxr-xr-x   0        0        0     1944 2023-05-05 11:54:39.057708 gameyamlspiderandgenerator-1.4.4/gameyamlspiderandgenerator/util/plugin_manager.py
+-rwxr-xr-x   0        0        0     2611 2023-05-05 11:54:39.066258 gameyamlspiderandgenerator-1.4.4/gameyamlspiderandgenerator/util/spider.py
+-rwxr-xr-x   0        0        0      700 2023-05-16 00:57:34.403809 gameyamlspiderandgenerator-1.4.4/pyproject.toml
+-rw-r--r--   0        0        0     2408 1970-01-01 00:00:00.000000 gameyamlspiderandgenerator-1.4.4/PKG-INFO
```

### Comparing `gameyamlspiderandgenerator-1.4.3/LICENSE` & `gameyamlspiderandgenerator-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.4.3/README.md` & `gameyamlspiderandgenerator-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.4.3/gameyamlspiderandgenerator/__init__.py` & `gameyamlspiderandgenerator-1.4.4/gameyamlspiderandgenerator/__init__.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.4.3/gameyamlspiderandgenerator/__main__.py` & `gameyamlspiderandgenerator-1.4.4/gameyamlspiderandgenerator/__main__.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.4.3/gameyamlspiderandgenerator/exception.py` & `gameyamlspiderandgenerator-1.4.4/gameyamlspiderandgenerator/exception.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.4.3/gameyamlspiderandgenerator/hook/search.py` & `gameyamlspiderandgenerator-1.4.4/gameyamlspiderandgenerator/hook/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 from ..util.spider import get_json
 
 
 # print(config, type(config))
 
 
 class Search(BaseHook):
+    REQUIRED = "get_name"
+
     @staticmethod
     def name_filter(string: str, pattern: str = r"[^A-z]", repl: str = ""):
         """
         
         Args:
             string: The string to be replaced
             pattern: Regular expression, replace non-English letters by default
```

### Comparing `gameyamlspiderandgenerator-1.4.3/gameyamlspiderandgenerator/hook/validate.py` & `gameyamlspiderandgenerator-1.4.4/gameyamlspiderandgenerator/hook/validate.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,18 +2,17 @@
 from ..util.spider import get_text
 from jsonschema import validate
 from yaml import safe_load
 from loguru import logger
 
 
 class Verify(BaseHook):
+    REQUIRED = None
+
     def setup(self, data: dict):
         try:
             validate(data, safe_load(get_text('https://raw.githubusercontent.com/FurryGamesIndex/games/master/schemas'
                                               '/game.schema.yaml')))
             logger.success("verification complete")
         except Exception as e:
             logger.error(e)
         return data
-
-    def __init__(self, arg):
-        pass
```

### Comparing `gameyamlspiderandgenerator-1.4.3/gameyamlspiderandgenerator/plugin/_base.py` & `gameyamlspiderandgenerator-1.4.4/gameyamlspiderandgenerator/plugin/_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,18 @@
 
         Args:
             data: 钩子数据
         """
         from gameyamlspiderandgenerator.util.plugin_manager import pkg
         pkg.__init__()
         for i in pkg.hook.values():
-            data = i(self.get_name()).setup(data)
+            if i.REQUIRED is None:
+                data = i().setup(data)
+            else:
+                data = i(self.__getattribute__(i.REQUIRED)()).setup(data)
         return data
 
     @abc.abstractmethod
     def get_name(self) -> str:
         """
         获取游戏名称
```

### Comparing `gameyamlspiderandgenerator-1.4.3/gameyamlspiderandgenerator/plugin/itchio.py` & `gameyamlspiderandgenerator-1.4.4/gameyamlspiderandgenerator/plugin/itchio.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         elif "Author" in self.more_info:
             temp = self.more_info["Author"]
         return [{"name": i.strip(), "role": ["producer"]} for i in temp]
 
     def get_tags(self) -> list[str]:
         temp = self.more_info["Genre"] if "Genre" in self.more_info else []
         temp1 = self.more_info["Made with"] if "Made with" in self.more_info else []
-        temp2 = self.more_info["Tags"]
+        temp2 = self.more_info["Tags"] if "Tags" in self.more_info else []
         return [i.strip() for i in (temp2 + temp1 + temp)]
 
     def get_misc_tags(self):
         repl = {
             "3D": "3d",
             "Pixel Art": "pixel-art",
             "free": "freeware",
@@ -169,15 +169,15 @@
             "screenshots": self.get_screenshots()  # + self.get_video(),
         }
         return YamlData(self.__load_hook__(ret))
 
     def get_type_tag(self):
         repl = {
             "Visual Novel": "visual-nove",
-            "Real time strategy": "Real time strategy",
+            "Real time strategy": "real-time-strategy",
             "Strategy": "strategy",
             "Casual": "casual",
             "Adventure": "adventure",
             "Board Game": "board",
             "Action": "action",
             "Fantasy": "fantasy",
             "Fighting": "fighting",
```

### Comparing `gameyamlspiderandgenerator-1.4.3/gameyamlspiderandgenerator/plugin/steam.py` & `gameyamlspiderandgenerator-1.4.4/gameyamlspiderandgenerator/plugin/steam.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.4.3/gameyamlspiderandgenerator/util/config.py` & `gameyamlspiderandgenerator-1.4.4/gameyamlspiderandgenerator/util/config.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.4.3/gameyamlspiderandgenerator/util/fgi.py` & `gameyamlspiderandgenerator-1.4.4/gameyamlspiderandgenerator/util/fgi.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.4.3/gameyamlspiderandgenerator/util/fgi_yaml.py` & `gameyamlspiderandgenerator-1.4.4/gameyamlspiderandgenerator/util/fgi_yaml.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.4.3/gameyamlspiderandgenerator/util/plugin_manager.py` & `gameyamlspiderandgenerator-1.4.4/gameyamlspiderandgenerator/util/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.4.3/gameyamlspiderandgenerator/util/spider.py` & `gameyamlspiderandgenerator-1.4.4/gameyamlspiderandgenerator/util/spider.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.4.3/pyproject.toml` & `gameyamlspiderandgenerator-1.4.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gameyamlspiderandgenerator"
-version = "1.4.3"
+version = "1.4.4"
 description = "A useful tool for generating Furrygameindex yaml files"
 authors = ["kaesinol"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `gameyamlspiderandgenerator-1.4.3/PKG-INFO` & `gameyamlspiderandgenerator-1.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gameyamlspiderandgenerator
-Version: 1.4.3
+Version: 1.4.4
 Summary: A useful tool for generating Furrygameindex yaml files
 License: MIT
 Author: kaesinol
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

