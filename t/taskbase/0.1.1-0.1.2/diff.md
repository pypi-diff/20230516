# Comparing `tmp/taskbase-0.1.1.tar.gz` & `tmp/taskbase-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskbase-0.1.1.tar", last modified: Tue May 16 12:41:20 2023, max compression
+gzip compressed data, was "taskbase-0.1.2.tar", last modified: Tue May 16 12:56:38 2023, max compression
```

## Comparing `taskbase-0.1.1.tar` & `taskbase-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 12:41:20.243155 taskbase-0.1.1/
--rw-rw-rw-   0        0        0        4 2023-05-16 10:18:40.000000 taskbase-0.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0      427 2023-05-16 12:41:20.241072 taskbase-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      120 2023-05-16 10:31:38.000000 taskbase-0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-16 12:41:20.243155 taskbase-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      441 2023-05-16 12:40:09.000000 taskbase-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-16 12:41:20.229451 taskbase-0.1.1/taskbase/
--rw-rw-rw-   0        0        0       25 2023-05-16 12:36:24.000000 taskbase-0.1.1/taskbase/__init__.py
--rw-rw-rw-   0        0        0     2375 2023-05-16 12:13:44.000000 taskbase-0.1.1/taskbase/taskbase.py
-drwxrwxrwx   0        0        0        0 2023-05-16 12:41:20.236286 taskbase-0.1.1/taskbase.egg-info/
--rw-rw-rw-   0        0        0      427 2023-05-16 12:41:20.000000 taskbase-0.1.1/taskbase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      200 2023-05-16 12:41:20.000000 taskbase-0.1.1/taskbase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 12:41:20.000000 taskbase-0.1.1/taskbase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-16 12:41:20.000000 taskbase-0.1.1/taskbase.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 12:56:38.575879 taskbase-0.1.2/
+-rw-rw-rw-   0        0        0        4 2023-05-16 10:18:40.000000 taskbase-0.1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      427 2023-05-16 12:56:38.573884 taskbase-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      120 2023-05-16 10:31:38.000000 taskbase-0.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-16 12:56:38.575879 taskbase-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      441 2023-05-16 12:56:21.000000 taskbase-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 12:56:38.560324 taskbase-0.1.2/taskbase/
+-rw-rw-rw-   0        0        0       25 2023-05-16 12:36:24.000000 taskbase-0.1.2/taskbase/__init__.py
+-rw-rw-rw-   0        0        0     2375 2023-05-16 12:13:44.000000 taskbase-0.1.2/taskbase/taskbase.py
+drwxrwxrwx   0        0        0        0 2023-05-16 12:56:38.571225 taskbase-0.1.2/taskbase.egg-info/
+-rw-rw-rw-   0        0        0      427 2023-05-16 12:56:38.000000 taskbase-0.1.2/taskbase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      200 2023-05-16 12:56:38.000000 taskbase-0.1.2/taskbase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 12:56:38.000000 taskbase-0.1.2/taskbase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-16 12:56:38.000000 taskbase-0.1.2/taskbase.egg-info/top_level.txt
```

### Comparing `taskbase-0.1.1/taskbase/taskbase.py` & `taskbase-0.1.2/taskbase/taskbase.py`

 * *Files identical despite different names*

