# Comparing `tmp/taskbase-0.1.3.tar.gz` & `tmp/taskbase-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskbase-0.1.3.tar", last modified: Tue May 16 13:29:57 2023, max compression
+gzip compressed data, was "taskbase-0.1.4.tar", last modified: Tue May 16 13:42:29 2023, max compression
```

## Comparing `taskbase-0.1.3.tar` & `taskbase-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 13:29:57.776709 taskbase-0.1.3/
--rw-rw-rw-   0        0        0        4 2023-05-16 10:18:40.000000 taskbase-0.1.3/LICENSE.txt
--rw-rw-rw-   0        0        0      427 2023-05-16 13:29:57.773719 taskbase-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      120 2023-05-16 10:31:38.000000 taskbase-0.1.3/README.md
--rw-rw-rw-   0        0        0       42 2023-05-16 13:29:57.776709 taskbase-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      441 2023-05-16 13:29:45.000000 taskbase-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-16 13:29:57.752241 taskbase-0.1.3/taskbase/
--rw-rw-rw-   0        0        0       31 2023-05-16 13:29:38.000000 taskbase-0.1.3/taskbase/__init__.py
--rw-rw-rw-   0        0        0     2353 2023-05-16 13:28:32.000000 taskbase-0.1.3/taskbase/taskbase.py
-drwxrwxrwx   0        0        0        0 2023-05-16 13:29:57.768731 taskbase-0.1.3/taskbase.egg-info/
--rw-rw-rw-   0        0        0      427 2023-05-16 13:29:57.000000 taskbase-0.1.3/taskbase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      200 2023-05-16 13:29:57.000000 taskbase-0.1.3/taskbase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 13:29:57.000000 taskbase-0.1.3/taskbase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-16 13:29:57.000000 taskbase-0.1.3/taskbase.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 13:42:29.203148 taskbase-0.1.4/
+-rw-rw-rw-   0        0        0        4 2023-05-16 10:18:40.000000 taskbase-0.1.4/LICENSE.txt
+-rw-rw-rw-   0        0        0      427 2023-05-16 13:42:29.201152 taskbase-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      120 2023-05-16 10:31:38.000000 taskbase-0.1.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-16 13:42:29.203148 taskbase-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      441 2023-05-16 13:42:13.000000 taskbase-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 13:42:29.157912 taskbase-0.1.4/taskbase/
+-rw-rw-rw-   0        0        0       44 2023-05-16 13:41:59.000000 taskbase-0.1.4/taskbase/__init__.py
+-rw-rw-rw-   0        0        0     2353 2023-05-16 13:39:12.000000 taskbase-0.1.4/taskbase/taskbase.py
+drwxrwxrwx   0        0        0        0 2023-05-16 13:42:29.197164 taskbase-0.1.4/taskbase.egg-info/
+-rw-rw-rw-   0        0        0      427 2023-05-16 13:42:28.000000 taskbase-0.1.4/taskbase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      200 2023-05-16 13:42:29.000000 taskbase-0.1.4/taskbase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 13:42:28.000000 taskbase-0.1.4/taskbase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-16 13:42:28.000000 taskbase-0.1.4/taskbase.egg-info/top_level.txt
```

### Comparing `taskbase-0.1.3/taskbase/taskbase.py` & `taskbase-0.1.4/taskbase/taskbase.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import random
 import time
 import datetime
 from functools import wraps
 from types import FunctionType
 
-class taskbase:
+class TaskBase:
     # __init_subclass__方法在Python 3.6及之后的版本中被引入，当一个类被子类化时，这个方法就会被调用。
     def __init_subclass__(cls, **kwargs):
         super().__init_subclass__(**kwargs)
         for attr, value in cls.__dict__.items():
             if type(value) is FunctionType:
                 setattr(cls, attr, cls.log_execution_time(value))
 
@@ -39,15 +39,15 @@
             time_taken_str = f"{time_taken:.3f}s"
             log_message = f"{start_time_str}\t{time_taken_str}\t{args[0].__class__.__base__.__name__}.{func.__qualname__}({params})"
             print(log_message)
 
             return result
         return wrapper
 
-# class testSubClass(taskbase):
+# class testSubClass(TaskBase):
 #     def my_method(self, arg1, arg2, arg3):
 #         time.sleep(random.uniform(0.1, 2))
 
 #     def error_test(self):
 #         time.sleep(random.uniform(0.1, 2))
 #         try:
 #             print(1/0)
```

