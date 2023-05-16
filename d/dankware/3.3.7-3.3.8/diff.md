# Comparing `tmp/dankware-3.3.7.tar.gz` & `tmp/dankware-3.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dankware-3.3.7.tar", last modified: Thu May  4 16:17:41 2023, max compression
+gzip compressed data, was "dankware-3.3.8.tar", last modified: Tue May 16 10:17:15 2023, max compression
```

## Comparing `dankware-3.3.7.tar` & `dankware-3.3.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:17:41.173611 dankware-3.3.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-04 16:17:28.000000 dankware-3.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13801 2023-05-04 16:17:41.173611 dankware-3.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12862 2023-05-04 16:17:28.000000 dankware-3.3.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:17:41.169611 dankware-3.3.7/dankware/
--rw-r--r--   0 runner    (1001) docker     (123)    46069 2023-05-04 16:17:28.000000 dankware-3.3.7/dankware/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:17:41.173611 dankware-3.3.7/dankware.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13801 2023-05-04 16:17:41.000000 dankware-3.3.7/dankware.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-04 16:17:41.000000 dankware-3.3.7/dankware.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 16:17:41.000000 dankware-3.3.7/dankware.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-04 16:17:41.000000 dankware-3.3.7/dankware.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-04 16:17:41.000000 dankware-3.3.7/dankware.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 16:17:41.173611 dankware-3.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-04 16:17:28.000000 dankware-3.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:17:15.805780 dankware-3.3.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-16 10:16:59.000000 dankware-3.3.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13801 2023-05-16 10:17:15.805780 dankware-3.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12862 2023-05-16 10:16:59.000000 dankware-3.3.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:17:15.801780 dankware-3.3.8/dankware/
+-rw-r--r--   0 runner    (1001) docker     (123)    46421 2023-05-16 10:16:59.000000 dankware-3.3.8/dankware/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:17:15.805780 dankware-3.3.8/dankware.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13801 2023-05-16 10:17:15.000000 dankware-3.3.8/dankware.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-16 10:17:15.000000 dankware-3.3.8/dankware.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 10:17:15.000000 dankware-3.3.8/dankware.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-16 10:17:15.000000 dankware-3.3.8/dankware.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-16 10:17:15.000000 dankware-3.3.8/dankware.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 10:17:15.805780 dankware-3.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-16 10:16:59.000000 dankware-3.3.8/setup.py
```

### Comparing `dankware-3.3.7/LICENSE` & `dankware-3.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dankware-3.3.7/PKG-INFO` & `dankware-3.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dankware
-Version: 3.3.7
+Version: 3.3.8
 Summary: Python package with various features!
 Home-page: https://github.com/SirDank/dankware
 Author: SirDank
 Author-email: SirDankenstein@protonmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/SirDank/dankware
 Project-URL: Bug Tracker, https://github.com/SirDank/dankware/issues
```

### Comparing `dankware-3.3.7/README.md` & `dankware-3.3.8/README.md`

 * *Files identical despite different names*

### Comparing `dankware-3.3.7/dankware/__init__.py` & `dankware-3.3.8/dankware/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -619,50 +619,59 @@
     valid intervals:
     - years -> int
     - days -> int
     - hours -> int
     - minutes -> int
     - seconds -> int
     - dynamic -> str
+    - dynamic-mini -> str
     - default -> str
     """
     
     if now is None: now = datetime.now()
 
     duration = now - then
 
     if interval in ("year", "years"): return int(duration.days / 365)
     elif interval in ("day", "days"): return duration.days
     elif interval in ("hour", "hours"): return int(duration.total_seconds() / 3600)
     elif interval in ("minute", "minutes"): return int(duration.total_seconds() / 60)
     elif interval in ("second", "seconds"): return int(duration.total_seconds())
-    elif interval == "dynamic":
+    elif interval in ("dynamic", "dynamic-mini"):
+        
+        mini = True if interval == "dynamic-mini" else False
 
         seconds = duration.total_seconds()
 
         if seconds < 60:
-            return f"{int(seconds)} second{'s' if seconds > 1 else ''}"
+            if mini: return f"{int(seconds)}s"
+            else: return f"{int(seconds)} second{'s' if seconds > 1 else ''}"
         
         elif seconds < 3600:
             minutes = int(seconds / 60)
-            return f"{minutes} minute{'s' if minutes > 1 else ''}"
+            if mini: return f"{minutes}m"
+            else:return f"{minutes} minute{'s' if minutes > 1 else ''}"
         
         elif seconds < 86400:
             hours = int(seconds / 3600)
-            return f"{hours} hour{'s' if hours > 1 else ''}"
+            if mini: return f"{hours}h"
+            else: return f"{hours} hour{'s' if hours > 1 else ''}"
        
         elif seconds < 31536000:
             days = int(seconds / 86400)
-            return f"{days} day{'s' if days > 1 else ''}"
+            if mini: return f"{days}d"
+            else: return f"{days} day{'s' if days > 1 else ''}"
         
         else:
             years = int(seconds / 31536000)
-            return f"{years} year{'s' if years > 1 else ''}"
+            if mini: return f"{years}y"
+            else: return f"{years} year{'s' if years > 1 else ''}"
     
     else:
+
         seconds = duration.total_seconds()
 
         years = int(seconds / 31536000)
         days = int((seconds % 31536000) / 86400)
         hours = int((seconds % 86400) / 3600)
         minutes = int((seconds % 3600) / 60)
         seconds = int(seconds % 60)
```

### Comparing `dankware-3.3.7/dankware.egg-info/PKG-INFO` & `dankware-3.3.8/dankware.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dankware
-Version: 3.3.7
+Version: 3.3.8
 Summary: Python package with various features!
 Home-page: https://github.com/SirDank/dankware
 Author: SirDank
 Author-email: SirDankenstein@protonmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/SirDank/dankware
 Project-URL: Bug Tracker, https://github.com/SirDank/dankware/issues
```

### Comparing `dankware-3.3.7/setup.py` & `dankware-3.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
 
     license = "MIT",
     name = "dankware",
-    version = "3.3.7",
+    version = "3.3.8",
     author = "SirDank",
     
     author_email = "SirDankenstein@protonmail.com",
     description = "Python package with various features!",
     long_description = open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type = "text/markdown",
     url = "https://github.com/SirDank/dankware",
```

