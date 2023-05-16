# Comparing `tmp/taskbase-0.1.tar.gz` & `tmp/taskbase-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskbase-0.1.tar", last modified: Tue May 16 10:33:30 2023, max compression
+gzip compressed data, was "taskbase-0.1.1.tar", last modified: Tue May 16 12:41:20 2023, max compression
```

## Comparing `taskbase-0.1.tar` & `taskbase-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 10:33:30.164336 taskbase-0.1/
--rw-rw-rw-   0        0        0        4 2023-05-16 10:18:40.000000 taskbase-0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      425 2023-05-16 10:33:30.163340 taskbase-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      120 2023-05-16 10:31:38.000000 taskbase-0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-16 10:33:30.164336 taskbase-0.1/setup.cfg
--rw-rw-rw-   0        0        0      439 2023-05-16 10:28:06.000000 taskbase-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-16 10:33:30.152364 taskbase-0.1/taskbase/
--rw-rw-rw-   0        0        0        0 2023-05-16 09:47:59.000000 taskbase-0.1/taskbase/__init__.py
--rw-rw-rw-   0        0        0     2345 2023-05-16 10:27:55.000000 taskbase-0.1/taskbase/taskbase.py
-drwxrwxrwx   0        0        0        0 2023-05-16 10:33:30.160346 taskbase-0.1/taskbase.egg-info/
--rw-rw-rw-   0        0        0      425 2023-05-16 10:33:29.000000 taskbase-0.1/taskbase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      200 2023-05-16 10:33:30.000000 taskbase-0.1/taskbase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 10:33:29.000000 taskbase-0.1/taskbase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-16 10:33:29.000000 taskbase-0.1/taskbase.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 12:41:20.243155 taskbase-0.1.1/
+-rw-rw-rw-   0        0        0        4 2023-05-16 10:18:40.000000 taskbase-0.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      427 2023-05-16 12:41:20.241072 taskbase-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      120 2023-05-16 10:31:38.000000 taskbase-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-16 12:41:20.243155 taskbase-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      441 2023-05-16 12:40:09.000000 taskbase-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 12:41:20.229451 taskbase-0.1.1/taskbase/
+-rw-rw-rw-   0        0        0       25 2023-05-16 12:36:24.000000 taskbase-0.1.1/taskbase/__init__.py
+-rw-rw-rw-   0        0        0     2375 2023-05-16 12:13:44.000000 taskbase-0.1.1/taskbase/taskbase.py
+drwxrwxrwx   0        0        0        0 2023-05-16 12:41:20.236286 taskbase-0.1.1/taskbase.egg-info/
+-rw-rw-rw-   0        0        0      427 2023-05-16 12:41:20.000000 taskbase-0.1.1/taskbase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      200 2023-05-16 12:41:20.000000 taskbase-0.1.1/taskbase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 12:41:20.000000 taskbase-0.1.1/taskbase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-16 12:41:20.000000 taskbase-0.1.1/taskbase.egg-info/top_level.txt
```

### Comparing `taskbase-0.1/taskbase/taskbase.py` & `taskbase-0.1.1/taskbase/taskbase.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import random
 import time
 import datetime
 from functools import wraps
 from types import FunctionType
 
-class Base:
+__all__ = ['taskbase']
+
+class taskbase:
     # __init_subclass__方法在Python 3.6及之后的版本中被引入，当一个类被子类化时，这个方法就会被调用。
     def __init_subclass__(cls, **kwargs):
         super().__init_subclass__(**kwargs)
         for attr, value in cls.__dict__.items():
             if type(value) is FunctionType:
                 setattr(cls, attr, cls.log_execution_time(value))
```

