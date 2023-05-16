# Comparing `tmp/kolyaklimkLab3-0.8.0.tar.gz` & `tmp/kolyaklimkLab3-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kolyaklimkLab3-0.8.0.tar", last modified: Tue May 16 08:05:22 2023, max compression
+gzip compressed data, was "kolyaklimkLab3-0.9.0.tar", last modified: Tue May 16 08:08:40 2023, max compression
```

## Comparing `kolyaklimkLab3-0.8.0.tar` & `kolyaklimkLab3-0.9.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 kolyaklimk  (1000) kolyaklimk  (1000)        0 2023-05-16 08:05:22.624069 kolyaklimkLab3-0.8.0/
--rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)      582 2023-05-16 08:05:22.624069 kolyaklimkLab3-0.8.0/PKG-INFO
-drwxrwxr-x   0 kolyaklimk  (1000) kolyaklimk  (1000)        0 2023-05-16 08:05:22.624069 kolyaklimkLab3-0.8.0/kolyaklimkLab3/
--rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)       76 2023-05-16 07:57:06.000000 kolyaklimkLab3-0.8.0/kolyaklimkLab3/__init__.py
-drwxrwxr-x   0 kolyaklimk  (1000) kolyaklimk  (1000)        0 2023-05-16 08:05:22.624069 kolyaklimkLab3-0.8.0/kolyaklimkLab3.egg-info/
--rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)      582 2023-05-16 08:05:22.000000 kolyaklimkLab3-0.8.0/kolyaklimkLab3.egg-info/PKG-INFO
--rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)      234 2023-05-16 08:05:22.000000 kolyaklimkLab3-0.8.0/kolyaklimkLab3.egg-info/SOURCES.txt
--rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)        1 2023-05-16 08:05:22.000000 kolyaklimkLab3-0.8.0/kolyaklimkLab3.egg-info/dependency_links.txt
--rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)        6 2023-05-16 08:05:22.000000 kolyaklimkLab3-0.8.0/kolyaklimkLab3.egg-info/requires.txt
--rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)       15 2023-05-16 08:05:22.000000 kolyaklimkLab3-0.8.0/kolyaklimkLab3.egg-info/top_level.txt
--rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)       38 2023-05-16 08:05:22.624069 kolyaklimkLab3-0.8.0/setup.cfg
--rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)      913 2023-05-16 08:05:16.000000 kolyaklimkLab3-0.8.0/setup.py
+drwxrwxr-x   0 kolyaklimk  (1000) kolyaklimk  (1000)        0 2023-05-16 08:08:40.651963 kolyaklimkLab3-0.9.0/
+-rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)      117 2023-05-16 08:08:40.651963 kolyaklimkLab3-0.9.0/PKG-INFO
+drwxrwxr-x   0 kolyaklimk  (1000) kolyaklimk  (1000)        0 2023-05-16 08:08:40.651963 kolyaklimkLab3-0.9.0/kolyaklimkLab3/
+-rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)       76 2023-05-16 07:57:06.000000 kolyaklimkLab3-0.9.0/kolyaklimkLab3/__init__.py
+drwxrwxr-x   0 kolyaklimk  (1000) kolyaklimk  (1000)        0 2023-05-16 08:08:40.651963 kolyaklimkLab3-0.9.0/kolyaklimkLab3.egg-info/
+-rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)      117 2023-05-16 08:08:40.000000 kolyaklimkLab3-0.9.0/kolyaklimkLab3.egg-info/PKG-INFO
+-rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)      234 2023-05-16 08:08:40.000000 kolyaklimkLab3-0.9.0/kolyaklimkLab3.egg-info/SOURCES.txt
+-rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)        1 2023-05-16 08:08:40.000000 kolyaklimkLab3-0.9.0/kolyaklimkLab3.egg-info/dependency_links.txt
+-rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)        1 2023-05-16 08:08:40.000000 kolyaklimkLab3-0.9.0/kolyaklimkLab3.egg-info/not-zip-safe
+-rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)       15 2023-05-16 08:08:40.000000 kolyaklimkLab3-0.9.0/kolyaklimkLab3.egg-info/top_level.txt
+-rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)       38 2023-05-16 08:08:40.651963 kolyaklimkLab3-0.9.0/setup.cfg
+-rw-rw-r--   0 kolyaklimk  (1000) kolyaklimk  (1000)      378 2023-05-16 08:08:38.000000 kolyaklimkLab3-0.9.0/setup.py
```

