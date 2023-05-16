# Comparing `tmp/econfiguration-0.5.2.tar.gz` & `tmp/econfiguration-0.5.3.tar.gz`

## Comparing `econfiguration-0.5.2.tar` & `econfiguration-0.5.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     4806 2020-02-02 00:00:00.000000 econfiguration-0.5.2/src/econfiguration/__init__.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 econfiguration-0.5.2/LICENSE
--rw-r--r--   0        0        0     2656 2020-02-02 00:00:00.000000 econfiguration-0.5.2/README.md
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 econfiguration-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 econfiguration-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     4873 2020-02-02 00:00:00.000000 econfiguration-0.5.3/src/econfiguration/__init__.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 econfiguration-0.5.3/LICENSE
+-rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 econfiguration-0.5.3/README.md
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 econfiguration-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     3262 2020-02-02 00:00:00.000000 econfiguration-0.5.3/PKG-INFO
```

### Comparing `econfiguration-0.5.2/src/econfiguration/__init__.py` & `econfiguration-0.5.3/src/econfiguration/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import os
 import json
 
 from typing import Union
 
 
-__version__ = "0.5.2"
+__version__ = "0.5.3"
 
 
 class Configuration(object):
     def __init__(self, _file: Union[str, list, tuple] = ..., _type: str = 'json', read_only: bool = False):
         self._con_clear_data()
         if _file is not Ellipsis: self._con_update_from_json(_file)
         self._con_set_read_only(read_only)
@@ -95,27 +95,27 @@
         __data = self._con_get_data()
         string = json.dumps(__data)
         with open(target, 'w') as fobj:
             fobj.write(string)
             fobj.flush()
 
 
-    def _con_get_value(self, __key: str) -> Union[int, float, str, bool, list, tuple, dict]:
+    def _con_get_value(self, __key: str) -> Union[int, float, str, bool, list, tuple, dict, None]:
         if not isinstance(__key, str):
             raise TypeError("The key type can only be str.")
 
         return self.__configuration.get(__key, None)
 
 
-    def _con_set_value(self, __key: str, __value: Union[int, float, str, bool, list, tuple, dict]) -> None:
+    def _con_set_value(self, __key: str, __value: Union[int, float, str, bool, list, tuple, dict, None]) -> None:
         if not isinstance(__key, str):
             raise TypeError("The key type can only be str.")
 
-        if not isinstance(__value, (int, float, str, bool, list, tuple, dict, Configuration)):
-            raise TypeError("The value type is not int, float, str, bool, list, tuple, dict or Configuration.")
+        if not isinstance(__value, (int, float, str, bool, list, tuple, dict, Configuration)) and __value is not None:
+            raise TypeError("The value type is not int, float, str, bool, list, tuple, dict, Configuration or None.")
 
         if len(__key) >= 5 and __key[:5] == '_con_':
             raise ValueError("The _con is reserved field.")
 
         if self._con_is_read_only():
             raise KeyError("The configuration object is read only.")
 
@@ -127,25 +127,25 @@
     #         len(__name) >= 5 and __name[:2] == __name[-2:] == '__') or (
     #         len(__name) >= 14 and __name[:14] == '_Configuration'):
     #         return super().__getattribute__(__name)
     #     else:
     #         return self._con_get_data(__name)
 
 
-    def __getattr__(self, __name: str) -> Union[int, float, str, bool, list, tuple, dict]:
+    def __getattr__(self, __name: str) -> Union[int, float, str, bool, list, tuple, dict, None]:
         return self._con_get_value(__name)
 
 
-    def __setattr__(self, __name: str, __value: Union[int, float, str, bool, list, tuple, dict]) -> None:
+    def __setattr__(self, __name: str, __value: Union[int, float, str, bool, list, tuple, dict, None]) -> None:
         if (len(__name) >= 14 and __name[:14] == '_Configuration'):
             return super().__setattr__(__name, __value)
 
         return self._con_set_value(__name, __value)
 
 
-    def __getitem__(self, __key: str) -> Union[int, float, str, bool, list, tuple, dict]:
-        return self._con_get_data(__key)
+    def __getitem__(self, __key: str) -> Union[int, float, str, bool, list, tuple, dict, None]:
+        return self._con_get_value(__key)
 
 
-    def __setitem__(self, __key: str, __value: Union[int, float, str, bool, list, tuple, dict]) -> None:
+    def __setitem__(self, __key: str, __value: Union[int, float, str, bool, list, tuple, dict, None]) -> None:
         return self._con_set_value(__key, __value)
```

### Comparing `econfiguration-0.5.2/LICENSE` & `econfiguration-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `econfiguration-0.5.2/README.md` & `econfiguration-0.5.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -111,7 +111,15 @@
 # 当 key 不存在时返回 None
 
 ._con_set_value(__key: str, __value: Union[int, float, str, bool, list, tuple, dict]) -> None
 # 设置条目数据
 # key 不允许使用 "_con_" 字段开头
 # value 不允许使用复杂数据类型
 ```
+
+
+## 其它
+
+### 字典重载
+
+使用 Configuration._con_update_from_data 更新数据时
+当某项数据的类型为 dict 且其中包含 '.con_is_configuration' 且值为 True, 那么这个字典会被重载成 Configuration 对象
```

### Comparing `econfiguration-0.5.2/pyproject.toml` & `econfiguration-0.5.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "econfiguration"
-version = "0.5.2"
+version = "0.5.3"
 authors = [
   { name="numLinka", email="numlinka@163.com" },
 ]
 description = "A simple log module"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `econfiguration-0.5.2/PKG-INFO` & `econfiguration-0.5.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: econfiguration
-Version: 0.5.2
+Version: 0.5.3
 Summary: A simple log module
 Project-URL: Homepage, https://github.com/numlinka/pylogop
 Project-URL: Bug Tracker, https://github.com/numlinka/pylogop/issues
 Author-email: numLinka <numlinka@163.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -125,7 +125,15 @@
 # 当 key 不存在时返回 None
 
 ._con_set_value(__key: str, __value: Union[int, float, str, bool, list, tuple, dict]) -> None
 # 设置条目数据
 # key 不允许使用 "_con_" 字段开头
 # value 不允许使用复杂数据类型
 ```
+
+
+## 其它
+
+### 字典重载
+
+使用 Configuration._con_update_from_data 更新数据时
+当某项数据的类型为 dict 且其中包含 '.con_is_configuration' 且值为 True, 那么这个字典会被重载成 Configuration 对象
```

