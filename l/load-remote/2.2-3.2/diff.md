# Comparing `tmp/load_remote-2.2.tar.gz` & `tmp/load_remote-3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/load_remote-2.2.tar", last modified: Thu Oct 24 09:10:16 2019, max compression
+gzip compressed data, was "load_remote-3.2.tar", last modified: Tue May 16 15:33:44 2023, max compression
```

## Comparing `load_remote-2.2.tar` & `load_remote-3.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 huangbo    (501) staff       (20)        0 2019-10-24 09:10:16.000000 load_remote-2.2/
--rw-r--r--   0 huangbo    (501) staff       (20)      195 2019-10-24 09:10:16.000000 load_remote-2.2/PKG-INFO
-drwxr-xr-x   0 huangbo    (501) staff       (20)        0 2019-10-24 09:10:16.000000 load_remote-2.2/load/
--rw-r--r--   0 huangbo    (501) staff       (20)        0 2019-07-16 04:11:37.000000 load_remote-2.2/load/__init__.py
--rw-r--r--   0 huangbo    (501) staff       (20)      787 2019-10-24 09:01:50.000000 load_remote-2.2/load/load_remote.py
-drwxr-xr-x   0 huangbo    (501) staff       (20)        0 2019-10-24 09:10:16.000000 load_remote-2.2/load_remote.egg-info/
--rw-r--r--   0 huangbo    (501) staff       (20)      195 2019-10-24 09:10:16.000000 load_remote-2.2/load_remote.egg-info/PKG-INFO
--rw-r--r--   0 huangbo    (501) staff       (20)      219 2019-10-24 09:10:16.000000 load_remote-2.2/load_remote.egg-info/SOURCES.txt
--rw-r--r--   0 huangbo    (501) staff       (20)        1 2019-10-24 09:10:16.000000 load_remote-2.2/load_remote.egg-info/dependency_links.txt
--rw-r--r--   0 huangbo    (501) staff       (20)        1 2019-07-16 10:28:44.000000 load_remote-2.2/load_remote.egg-info/not-zip-safe
--rw-r--r--   0 huangbo    (501) staff       (20)        5 2019-10-24 09:10:16.000000 load_remote-2.2/load_remote.egg-info/top_level.txt
--rw-r--r--   0 huangbo    (501) staff       (20)       38 2019-10-24 09:10:16.000000 load_remote-2.2/setup.cfg
--rw-r--r--   0 huangbo    (501) staff       (20)      257 2019-10-24 09:10:09.000000 load_remote-2.2/setup.py
+drwxr-xr-x   0 huangbo    (501) staff       (20)        0 2023-05-16 15:33:44.544527 load_remote-3.2/
+-rw-r--r--   0 huangbo    (501) staff       (20)      149 2023-05-16 15:33:44.543201 load_remote-3.2/PKG-INFO
+drwxr-xr-x   0 huangbo    (501) staff       (20)        0 2023-05-16 15:33:44.537301 load_remote-3.2/load/
+-rw-r--r--   0 huangbo    (501) staff       (20)        0 2019-07-16 04:11:37.000000 load_remote-3.2/load/__init__.py
+-rw-r--r--   0 huangbo    (501) staff       (20)      815 2023-05-16 15:01:42.000000 load_remote-3.2/load/load_remote.py
+drwxr-xr-x   0 huangbo    (501) staff       (20)        0 2023-05-16 15:33:44.542029 load_remote-3.2/load_remote.egg-info/
+-rw-r--r--   0 huangbo    (501) staff       (20)      149 2023-05-16 15:33:44.000000 load_remote-3.2/load_remote.egg-info/PKG-INFO
+-rw-r--r--   0 huangbo    (501) staff       (20)      219 2023-05-16 15:33:44.000000 load_remote-3.2/load_remote.egg-info/SOURCES.txt
+-rw-r--r--   0 huangbo    (501) staff       (20)        1 2023-05-16 15:33:44.000000 load_remote-3.2/load_remote.egg-info/dependency_links.txt
+-rw-r--r--   0 huangbo    (501) staff       (20)        1 2019-07-16 10:28:44.000000 load_remote-3.2/load_remote.egg-info/not-zip-safe
+-rw-r--r--   0 huangbo    (501) staff       (20)        5 2023-05-16 15:33:44.000000 load_remote-3.2/load_remote.egg-info/top_level.txt
+-rw-r--r--   0 huangbo    (501) staff       (20)       38 2023-05-16 15:33:44.545122 load_remote-3.2/setup.cfg
+-rw-r--r--   0 huangbo    (501) staff       (20)      257 2023-05-16 15:32:02.000000 load_remote-3.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

