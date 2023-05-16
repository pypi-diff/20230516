# Comparing `tmp/python-snippets-0.0.3.tar.gz` & `tmp/python-snippets-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-snippets-0.0.3.tar", last modified: Tue Aug  2 08:14:26 2022, max compression
+gzip compressed data, was "python-snippets-0.0.6.tar", last modified: Tue Nov  1 06:44:17 2022, max compression
```

## Comparing `python-snippets-0.0.3.tar` & `python-snippets-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 08:14:26.146979 python-snippets-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (121)      247 2022-08-02 08:14:26.146979 python-snippets-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       98 2022-08-02 08:14:12.000000 python-snippets-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 08:14:26.146979 python-snippets-0.0.3/python_snippets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      247 2022-08-02 08:14:26.000000 python-snippets-0.0.3/python_snippets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      314 2022-08-02 08:14:26.000000 python-snippets-0.0.3/python_snippets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-02 08:14:26.000000 python-snippets-0.0.3/python_snippets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-08-02 08:14:26.000000 python-snippets-0.0.3/python_snippets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-08-02 08:14:26.000000 python-snippets-0.0.3/python_snippets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-02 08:14:25.000000 python-snippets-0.0.3/python_snippets.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-02 08:14:26.146979 python-snippets-0.0.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)      849 2022-08-02 08:14:12.000000 python-snippets-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 08:14:26.146979 python-snippets-0.0.3/snippets/
--rw-r--r--   0 runner    (1001) docker     (121)      514 2022-08-02 08:14:12.000000 python-snippets-0.0.3/snippets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2917 2022-08-02 08:14:12.000000 python-snippets-0.0.3/snippets/decorators.py
--rw-r--r--   0 runner    (1001) docker     (121)     7626 2022-08-02 08:14:12.000000 python-snippets-0.0.3/snippets/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 06:44:17.188819 python-snippets-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (121)      247 2022-11-01 06:44:17.188819 python-snippets-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)       98 2022-11-01 06:44:01.000000 python-snippets-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 06:44:17.188819 python-snippets-0.0.6/python_snippets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      247 2022-11-01 06:44:17.000000 python-snippets-0.0.6/python_snippets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      314 2022-11-01 06:44:17.000000 python-snippets-0.0.6/python_snippets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 06:44:17.000000 python-snippets-0.0.6/python_snippets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-11-01 06:44:17.000000 python-snippets-0.0.6/python_snippets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2022-11-01 06:44:17.000000 python-snippets-0.0.6/python_snippets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 06:44:16.000000 python-snippets-0.0.6/python_snippets.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 06:44:17.188819 python-snippets-0.0.6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (121)      849 2022-11-01 06:44:01.000000 python-snippets-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 06:44:17.188819 python-snippets-0.0.6/snippets/
+-rw-r--r--   0 runner    (1001) docker     (121)      514 2022-11-01 06:44:01.000000 python-snippets-0.0.6/snippets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3459 2022-11-01 06:44:01.000000 python-snippets-0.0.6/snippets/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7856 2022-11-01 06:44:01.000000 python-snippets-0.0.6/snippets/utils.py
```

### Comparing `python-snippets-0.0.3/setup.py` & `python-snippets-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 REQ = [
     "tqdm",
     "pydantic"
 ]
 
 setup(
     name='python-snippets',
-    version='0.0.3',
+    version='0.0.6',
     install_requires=REQ,
     packages=find_packages(exclude=['tests*']),
     package_dir={"": "."},
     package_data={},
     url='https://github.com/jerrychen1990/python-snippets.git',
     license='MIT',
     author='Chen Hao',
```

### Comparing `python-snippets-0.0.3/snippets/__init__.py` & `python-snippets-0.0.6/snippets/__init__.py`

 * *Files identical despite different names*

### Comparing `python-snippets-0.0.3/snippets/decorators.py` & `python-snippets-0.0.6/snippets/decorators.py`

 * *Files 12% similar despite different names*

```diff
@@ -98,7 +98,28 @@
     arg_names = inspect.signature(func).parameters.keys()
 
     def wrap(*args, **kwargs):
         kwargs = {k: v for k, v in kwargs.items() if k in arg_names}
         return func(*args, **kwargs)
 
     return wrap
+
+
+# adapt function with single elements
+def adapt_single(ele_name):
+    def wrapper(func):
+        @wraps(func)
+        def wrapped(*args, **kwargs):
+            if ele_name in kwargs:
+                is_single = not isinstance(kwargs[ele_name], list)
+            else:
+                is_single = False
+            if is_single:
+                kwargs[ele_name] = [kwargs[ele_name]]
+            rs = func(*args, **kwargs)
+            if is_single:
+                rs = rs[0]
+            return rs
+
+        return wrapped
+
+    return wrapper
```

### Comparing `python-snippets-0.0.3/snippets/utils.py` & `python-snippets-0.0.6/snippets/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import collections
 import os
 import json
 import pickle
 import subprocess
 import time
 import logging
+import numpy as np
 from pydantic import BaseModel
 from datetime import datetime
 
 from typing import Any, List, Sequence, Tuple, Iterable, Dict, _GenericAlias
 
 from tqdm import tqdm
 
@@ -39,16 +40,22 @@
             return str(obj)
         if isinstance(obj, set):
             return list(obj)
         if isinstance(obj, BaseModel):
             return obj.dict(exclude_none=True, exclude_defaults=True)
         if isinstance(obj, datetime):
             return obj.strftime("%Y-%M-%d %H:%m:%S")
-
-        return {'_python_object': pickle.dumps(obj)}
+        if isinstance(obj, np.integer):
+            return int(obj)
+        if isinstance(obj, np.floating):
+            return float(obj)
+        if isinstance(obj, np.ndarray):
+            return obj.tolist()
+        else:
+            return super().default(obj)
 
 
 # 将$obj转json string。默认ensure_ascii=False,并用indent=4展示
 def jdumps(obj: Any, encoder=PythonObjectEncoder) -> str:
     return json.dumps(obj, ensure_ascii=False, indent=4, cls=encoder)
 
 
@@ -223,31 +230,29 @@
 def star_surround_info(info: str, fix_length=128) -> str:
     star_num = max(fix_length - len(info), 2)
     left_star_num = star_num // 2
     right_star_num = star_num - left_star_num
     rs = "*" * left_star_num + info + "*" * right_star_num
     return rs
 
+
 # # 将star_surround_info处理后的信息用logger或者print方法输出
 def print_info(info, target_logger=None, fix_length=128):
     star_info = star_surround_info(info, fix_length)
     if target_logger:
         target_logger.info(star_info)
     else:
         print(star_info)
 
+
 def get_cur_dir():
     return os.path.abspath(os.path.dirname(__file__))
 
-def union_parse_obj(union:_GenericAlias, d:dict):
+
+def union_parse_obj(union: _GenericAlias, d: dict):
     for cls in union.__args__:
         try:
             obj = cls(**d)
             return obj
         except:
             pass
     raise Exception(f"fail to convert {d} to union {union}")
-
-
-
-
-
```

