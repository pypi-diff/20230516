# Comparing `tmp/taskbase-0.1.2.tar.gz` & `tmp/taskbase-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskbase-0.1.2.tar", last modified: Tue May 16 12:56:38 2023, max compression
+gzip compressed data, was "taskbase-0.1.3.tar", last modified: Tue May 16 13:29:57 2023, max compression
```

## Comparing `taskbase-0.1.2.tar` & `taskbase-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 12:56:38.575879 taskbase-0.1.2/
--rw-rw-rw-   0        0        0        4 2023-05-16 10:18:40.000000 taskbase-0.1.2/LICENSE.txt
--rw-rw-rw-   0        0        0      427 2023-05-16 12:56:38.573884 taskbase-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      120 2023-05-16 10:31:38.000000 taskbase-0.1.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-16 12:56:38.575879 taskbase-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      441 2023-05-16 12:56:21.000000 taskbase-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-16 12:56:38.560324 taskbase-0.1.2/taskbase/
--rw-rw-rw-   0        0        0       25 2023-05-16 12:36:24.000000 taskbase-0.1.2/taskbase/__init__.py
--rw-rw-rw-   0        0        0     2375 2023-05-16 12:13:44.000000 taskbase-0.1.2/taskbase/taskbase.py
-drwxrwxrwx   0        0        0        0 2023-05-16 12:56:38.571225 taskbase-0.1.2/taskbase.egg-info/
--rw-rw-rw-   0        0        0      427 2023-05-16 12:56:38.000000 taskbase-0.1.2/taskbase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      200 2023-05-16 12:56:38.000000 taskbase-0.1.2/taskbase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 12:56:38.000000 taskbase-0.1.2/taskbase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-16 12:56:38.000000 taskbase-0.1.2/taskbase.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 13:29:57.776709 taskbase-0.1.3/
+-rw-rw-rw-   0        0        0        4 2023-05-16 10:18:40.000000 taskbase-0.1.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      427 2023-05-16 13:29:57.773719 taskbase-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      120 2023-05-16 10:31:38.000000 taskbase-0.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-16 13:29:57.776709 taskbase-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      441 2023-05-16 13:29:45.000000 taskbase-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 13:29:57.752241 taskbase-0.1.3/taskbase/
+-rw-rw-rw-   0        0        0       31 2023-05-16 13:29:38.000000 taskbase-0.1.3/taskbase/__init__.py
+-rw-rw-rw-   0        0        0     2353 2023-05-16 13:28:32.000000 taskbase-0.1.3/taskbase/taskbase.py
+drwxrwxrwx   0        0        0        0 2023-05-16 13:29:57.768731 taskbase-0.1.3/taskbase.egg-info/
+-rw-rw-rw-   0        0        0      427 2023-05-16 13:29:57.000000 taskbase-0.1.3/taskbase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      200 2023-05-16 13:29:57.000000 taskbase-0.1.3/taskbase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 13:29:57.000000 taskbase-0.1.3/taskbase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-16 13:29:57.000000 taskbase-0.1.3/taskbase.egg-info/top_level.txt
```

### Comparing `taskbase-0.1.2/taskbase/taskbase.py` & `taskbase-0.1.3/taskbase/taskbase.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import random
 import time
 import datetime
 from functools import wraps
 from types import FunctionType
 
-__all__ = ['taskbase']
-
 class taskbase:
     # __init_subclass__方法在Python 3.6及之后的版本中被引入，当一个类被子类化时，这个方法就会被调用。
     def __init_subclass__(cls, **kwargs):
         super().__init_subclass__(**kwargs)
         for attr, value in cls.__dict__.items():
             if type(value) is FunctionType:
                 setattr(cls, attr, cls.log_execution_time(value))
@@ -41,15 +39,15 @@
             time_taken_str = f"{time_taken:.3f}s"
             log_message = f"{start_time_str}\t{time_taken_str}\t{args[0].__class__.__base__.__name__}.{func.__qualname__}({params})"
             print(log_message)
 
             return result
         return wrapper
 
-# class testSubClass(Base):
+# class testSubClass(taskbase):
 #     def my_method(self, arg1, arg2, arg3):
 #         time.sleep(random.uniform(0.1, 2))
 
 #     def error_test(self):
 #         time.sleep(random.uniform(0.1, 2))
 #         try:
 #             print(1/0)
```

