# Comparing `tmp/taskbase-0.1.4.tar.gz` & `tmp/taskbase-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskbase-0.1.4.tar", last modified: Tue May 16 13:42:29 2023, max compression
+gzip compressed data, was "taskbase-0.1.5.tar", last modified: Tue May 16 13:51:12 2023, max compression
```

## Comparing `taskbase-0.1.4.tar` & `taskbase-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 13:42:29.203148 taskbase-0.1.4/
--rw-rw-rw-   0        0        0        4 2023-05-16 10:18:40.000000 taskbase-0.1.4/LICENSE.txt
--rw-rw-rw-   0        0        0      427 2023-05-16 13:42:29.201152 taskbase-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      120 2023-05-16 10:31:38.000000 taskbase-0.1.4/README.md
--rw-rw-rw-   0        0        0       42 2023-05-16 13:42:29.203148 taskbase-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      441 2023-05-16 13:42:13.000000 taskbase-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-16 13:42:29.157912 taskbase-0.1.4/taskbase/
--rw-rw-rw-   0        0        0       44 2023-05-16 13:41:59.000000 taskbase-0.1.4/taskbase/__init__.py
--rw-rw-rw-   0        0        0     2353 2023-05-16 13:39:12.000000 taskbase-0.1.4/taskbase/taskbase.py
-drwxrwxrwx   0        0        0        0 2023-05-16 13:42:29.197164 taskbase-0.1.4/taskbase.egg-info/
--rw-rw-rw-   0        0        0      427 2023-05-16 13:42:28.000000 taskbase-0.1.4/taskbase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      200 2023-05-16 13:42:29.000000 taskbase-0.1.4/taskbase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 13:42:28.000000 taskbase-0.1.4/taskbase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-16 13:42:28.000000 taskbase-0.1.4/taskbase.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 13:51:12.927576 taskbase-0.1.5/
+-rw-rw-rw-   0        0        0        4 2023-05-16 10:18:40.000000 taskbase-0.1.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      427 2023-05-16 13:51:12.926579 taskbase-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      120 2023-05-16 10:31:38.000000 taskbase-0.1.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-16 13:51:12.928582 taskbase-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      441 2023-05-16 13:50:57.000000 taskbase-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 13:51:12.914611 taskbase-0.1.5/taskbase/
+-rw-rw-rw-   0        0        0       44 2023-05-16 13:41:59.000000 taskbase-0.1.5/taskbase/__init__.py
+-rw-rw-rw-   0        0        0     2353 2023-05-16 13:39:12.000000 taskbase-0.1.5/taskbase/taskbase.py
+drwxrwxrwx   0        0        0        0 2023-05-16 13:51:12.923587 taskbase-0.1.5/taskbase.egg-info/
+-rw-rw-rw-   0        0        0      427 2023-05-16 13:51:12.000000 taskbase-0.1.5/taskbase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      200 2023-05-16 13:51:12.000000 taskbase-0.1.5/taskbase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 13:51:12.000000 taskbase-0.1.5/taskbase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-16 13:51:12.000000 taskbase-0.1.5/taskbase.egg-info/top_level.txt
```

### Comparing `taskbase-0.1.4/taskbase/taskbase.py` & `taskbase-0.1.5/taskbase/taskbase.py`

 * *Files identical despite different names*

