# Comparing `tmp/std-logger-0.0.3.tar.gz` & `tmp/std-logger-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "std-logger-0.0.3.tar", last modified: Tue Feb 14 02:54:41 2023, max compression
+gzip compressed data, was "std-logger-0.0.6.tar", last modified: Tue May 16 03:56:25 2023, max compression
```

## Comparing `std-logger-0.0.3.tar` & `std-logger-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 wei.fu     (502) staff       (20)        0 2023-02-14 02:54:41.670497 std-logger-0.0.3/
--rw-r--r--   0 wei.fu     (502) staff       (20)      369 2023-02-14 02:54:41.670338 std-logger-0.0.3/PKG-INFO
--rw-r--r--   0 wei.fu     (502) staff       (20)       38 2023-02-14 02:54:41.670544 std-logger-0.0.3/setup.cfg
--rw-r--r--   0 wei.fu     (502) staff       (20)      772 2023-02-14 02:54:38.000000 std-logger-0.0.3/setup.py
-drwxr-xr-x   0 wei.fu     (502) staff       (20)        0 2023-02-14 02:54:41.668797 std-logger-0.0.3/stdLogger/
--rw-r--r--   0 wei.fu     (502) staff       (20)       32 2023-02-10 09:35:37.000000 std-logger-0.0.3/stdLogger/__init__.py
--rw-r--r--   0 wei.fu     (502) staff       (20)     3902 2023-02-10 09:35:20.000000 std-logger-0.0.3/stdLogger/std_logs.py
-drwxr-xr-x   0 wei.fu     (502) staff       (20)        0 2023-02-14 02:54:41.670138 std-logger-0.0.3/std_logger.egg-info/
--rw-r--r--   0 wei.fu     (502) staff       (20)      369 2023-02-14 02:54:41.000000 std-logger-0.0.3/std_logger.egg-info/PKG-INFO
--rw-r--r--   0 wei.fu     (502) staff       (20)      221 2023-02-14 02:54:41.000000 std-logger-0.0.3/std_logger.egg-info/SOURCES.txt
--rw-r--r--   0 wei.fu     (502) staff       (20)        1 2023-02-14 02:54:41.000000 std-logger-0.0.3/std_logger.egg-info/dependency_links.txt
--rw-r--r--   0 wei.fu     (502) staff       (20)       28 2023-02-14 02:54:41.000000 std-logger-0.0.3/std_logger.egg-info/requires.txt
--rw-r--r--   0 wei.fu     (502) staff       (20)       10 2023-02-14 02:54:41.000000 std-logger-0.0.3/std_logger.egg-info/top_level.txt
+drwxr-xr-x   0 wei.fu     (502) staff       (20)        0 2023-05-16 03:56:25.014644 std-logger-0.0.6/
+-rw-r--r--   0 wei.fu     (502) staff       (20)      369 2023-05-16 03:56:25.014477 std-logger-0.0.6/PKG-INFO
+-rw-r--r--   0 wei.fu     (502) staff       (20)       38 2023-05-16 03:56:25.014696 std-logger-0.0.6/setup.cfg
+-rw-r--r--   0 wei.fu     (502) staff       (20)      745 2023-02-15 09:05:01.000000 std-logger-0.0.6/setup.py
+drwxr-xr-x   0 wei.fu     (502) staff       (20)        0 2023-05-16 03:56:25.012698 std-logger-0.0.6/stdLogger/
+-rw-r--r--   0 wei.fu     (502) staff       (20)       32 2023-02-10 09:35:37.000000 std-logger-0.0.6/stdLogger/__init__.py
+-rw-r--r--   0 wei.fu     (502) staff       (20)     3923 2023-05-16 03:31:35.000000 std-logger-0.0.6/stdLogger/std_logs.py
+drwxr-xr-x   0 wei.fu     (502) staff       (20)        0 2023-05-16 03:56:25.014207 std-logger-0.0.6/std_logger.egg-info/
+-rw-r--r--   0 wei.fu     (502) staff       (20)      369 2023-05-16 03:56:24.000000 std-logger-0.0.6/std_logger.egg-info/PKG-INFO
+-rw-r--r--   0 wei.fu     (502) staff       (20)      221 2023-05-16 03:56:24.000000 std-logger-0.0.6/std_logger.egg-info/SOURCES.txt
+-rw-r--r--   0 wei.fu     (502) staff       (20)        1 2023-05-16 03:56:24.000000 std-logger-0.0.6/std_logger.egg-info/dependency_links.txt
+-rw-r--r--   0 wei.fu     (502) staff       (20)       28 2023-05-16 03:56:24.000000 std-logger-0.0.6/std_logger.egg-info/requires.txt
+-rw-r--r--   0 wei.fu     (502) staff       (20)       10 2023-05-16 03:56:24.000000 std-logger-0.0.6/std_logger.egg-info/top_level.txt
```

### Comparing `std-logger-0.0.3/stdLogger/std_logs.py` & `std-logger-0.0.6/stdLogger/std_logs.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,16 +45,16 @@
 
         _logger.remove()
         _logger.add(sys.stdout, format=_FORMAT_CONFIG)
         #只记录INFO级别日志
         _logger.add("./runtime/app.log",
                     rotation="500 MB",
                     format=_FORMAT_CONFIG,
-                    level=10,
-                    filter=self.info_only)
+                    level=10
+                    )
         # 记录warning以上的日志
         _logger.add(
             "./runtime/app_error.log",
             level=30,
             format=_FORMAT_CONFIG,
             rotation="500 MB",
         )
@@ -89,16 +89,17 @@
         _logger.trace(msg, *args, **kwargs)
 
     def debug(self, __message: str, *args, **kwargs) -> None:
         """
         level 10
         """
         _msg = self.custom_message_context()
-        message = "%s | %s" % (_msg, __message)
-        _logger.debug(message, *args, **kwargs)
+        print(type(__message))
+        #message = "%s | %s" % (_msg, __message)
+        #_logger.debug(message, *args, **kwargs)
 
     def info(self, __message: str, *args, **kwargs) -> None:
         """
         level 20
         """
 
         _msg = self.custom_message_context()
@@ -126,8 +127,11 @@
     def exception(self, __message: str, *args, **kwargs) -> None:
         """level 50"""
         _msg = self.custom_message_context()
         message = "%s | %s" % (_msg, __message)
         _logger.exception(message, *args, **kwargs)
 
 
-std_logger = StdLogger()
+std_logger=logger = StdLogger()
+
+
+
```

