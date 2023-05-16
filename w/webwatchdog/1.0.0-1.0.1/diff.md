# Comparing `tmp/webwatchdog-1.0.0.tar.gz` & `tmp/webwatchdog-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webwatchdog-1.0.0.tar", last modified: Tue May 16 17:25:49 2023, max compression
+gzip compressed data, was "webwatchdog-1.0.1.tar", last modified: Tue May 16 17:31:00 2023, max compression
```

## Comparing `webwatchdog-1.0.0.tar` & `webwatchdog-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 itsknk     (501) staff       (20)        0 2023-05-16 17:25:49.043774 webwatchdog-1.0.0/
--rw-r--r--   0 itsknk     (501) staff       (20)      489 2023-05-16 17:25:49.043237 webwatchdog-1.0.0/PKG-INFO
--rw-r--r--   0 itsknk     (501) staff       (20)      315 2023-05-16 17:09:18.000000 webwatchdog-1.0.0/README.md
--rw-r--r--   0 itsknk     (501) staff       (20)       38 2023-05-16 17:25:49.043910 webwatchdog-1.0.0/setup.cfg
--rw-r--r--   0 itsknk     (501) staff       (20)      432 2023-05-16 17:25:42.000000 webwatchdog-1.0.0/setup.py
-drwxr-xr-x   0 itsknk     (501) staff       (20)        0 2023-05-16 17:25:49.040565 webwatchdog-1.0.0/up_or_down/
--rw-r--r--   0 itsknk     (501) staff       (20)        0 2023-05-16 16:41:54.000000 webwatchdog-1.0.0/up_or_down/__init__.py
--rw-r--r--   0 itsknk     (501) staff       (20)      572 2023-05-16 16:40:52.000000 webwatchdog-1.0.0/up_or_down/up_or_down.py
-drwxr-xr-x   0 itsknk     (501) staff       (20)        0 2023-05-16 17:25:49.042717 webwatchdog-1.0.0/webwatchdog.egg-info/
--rw-r--r--   0 itsknk     (501) staff       (20)      489 2023-05-16 17:25:48.000000 webwatchdog-1.0.0/webwatchdog.egg-info/PKG-INFO
--rw-r--r--   0 itsknk     (501) staff       (20)      240 2023-05-16 17:25:49.000000 webwatchdog-1.0.0/webwatchdog.egg-info/SOURCES.txt
--rw-r--r--   0 itsknk     (501) staff       (20)        1 2023-05-16 17:25:48.000000 webwatchdog-1.0.0/webwatchdog.egg-info/dependency_links.txt
--rw-r--r--   0 itsknk     (501) staff       (20)       18 2023-05-16 17:25:48.000000 webwatchdog-1.0.0/webwatchdog.egg-info/requires.txt
--rw-r--r--   0 itsknk     (501) staff       (20)       11 2023-05-16 17:25:48.000000 webwatchdog-1.0.0/webwatchdog.egg-info/top_level.txt
+drwxr-xr-x   0 itsknk     (501) staff       (20)        0 2023-05-16 17:31:00.427024 webwatchdog-1.0.1/
+-rw-r--r--   0 itsknk     (501) staff       (20)      493 2023-05-16 17:31:00.426602 webwatchdog-1.0.1/PKG-INFO
+-rw-r--r--   0 itsknk     (501) staff       (20)      319 2023-05-16 17:30:36.000000 webwatchdog-1.0.1/README.md
+-rw-r--r--   0 itsknk     (501) staff       (20)       38 2023-05-16 17:31:00.427161 webwatchdog-1.0.1/setup.cfg
+-rw-r--r--   0 itsknk     (501) staff       (20)      432 2023-05-16 17:30:55.000000 webwatchdog-1.0.1/setup.py
+drwxr-xr-x   0 itsknk     (501) staff       (20)        0 2023-05-16 17:31:00.423345 webwatchdog-1.0.1/up_or_down/
+-rw-r--r--   0 itsknk     (501) staff       (20)        0 2023-05-16 16:41:54.000000 webwatchdog-1.0.1/up_or_down/__init__.py
+-rw-r--r--   0 itsknk     (501) staff       (20)      572 2023-05-16 16:40:52.000000 webwatchdog-1.0.1/up_or_down/up_or_down.py
+drwxr-xr-x   0 itsknk     (501) staff       (20)        0 2023-05-16 17:31:00.426055 webwatchdog-1.0.1/webwatchdog.egg-info/
+-rw-r--r--   0 itsknk     (501) staff       (20)      493 2023-05-16 17:31:00.000000 webwatchdog-1.0.1/webwatchdog.egg-info/PKG-INFO
+-rw-r--r--   0 itsknk     (501) staff       (20)      240 2023-05-16 17:31:00.000000 webwatchdog-1.0.1/webwatchdog.egg-info/SOURCES.txt
+-rw-r--r--   0 itsknk     (501) staff       (20)        1 2023-05-16 17:31:00.000000 webwatchdog-1.0.1/webwatchdog.egg-info/dependency_links.txt
+-rw-r--r--   0 itsknk     (501) staff       (20)       18 2023-05-16 17:31:00.000000 webwatchdog-1.0.1/webwatchdog.egg-info/requires.txt
+-rw-r--r--   0 itsknk     (501) staff       (20)       11 2023-05-16 17:31:00.000000 webwatchdog-1.0.1/webwatchdog.egg-info/top_level.txt
```

### Comparing `webwatchdog-1.0.0/up_or_down/up_or_down.py` & `webwatchdog-1.0.1/up_or_down/up_or_down.py`

 * *Files identical despite different names*

