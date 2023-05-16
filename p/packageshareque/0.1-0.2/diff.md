# Comparing `tmp/packageshareque-0.1.tar.gz` & `tmp/packageshareque-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "packageshareque-0.1.tar", last modified: Tue May 16 07:48:12 2023, max compression
+gzip compressed data, was "packageshareque-0.2.tar", last modified: Tue May 16 08:19:47 2023, max compression
```

## Comparing `packageshareque-0.1.tar` & `packageshareque-0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 07:48:12.409606 packageshareque-0.1/
--rw-rw-rw-   0        0        0        0 2023-05-15 07:12:56.000000 packageshareque-0.1/Licence.txt
--rw-rw-rw-   0        0        0      173 2023-05-16 07:48:12.390576 packageshareque-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-16 07:48:12.103240 packageshareque-0.1/packageshareque/
--rw-rw-rw-   0        0        0       76 2023-05-16 07:37:35.000000 packageshareque-0.1/packageshareque/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 07:48:12.381560 packageshareque-0.1/packageshareque.egg-info/
--rw-rw-rw-   0        0        0      173 2023-05-16 07:48:11.000000 packageshareque-0.1/packageshareque.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      204 2023-05-16 07:48:11.000000 packageshareque-0.1/packageshareque.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 07:48:11.000000 packageshareque-0.1/packageshareque.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-16 07:48:11.000000 packageshareque-0.1/packageshareque.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-16 07:48:12.411607 packageshareque-0.1/setup.cfg
--rw-rw-rw-   0        0        0      288 2023-05-16 07:43:56.000000 packageshareque-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 08:19:47.741747 packageshareque-0.2/
+-rw-rw-rw-   0        0        0        0 2023-05-15 07:12:56.000000 packageshareque-0.2/Licence.txt
+-rw-rw-rw-   0        0        0      174 2023-05-16 08:19:47.658016 packageshareque-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-16 08:19:46.968553 packageshareque-0.2/packageshareque/
+-rw-rw-rw-   0        0        0       76 2023-05-16 07:37:35.000000 packageshareque-0.2/packageshareque/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 08:19:47.651998 packageshareque-0.2/packageshareque.egg-info/
+-rw-rw-rw-   0        0        0      174 2023-05-16 08:19:46.000000 packageshareque-0.2/packageshareque.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      204 2023-05-16 08:19:46.000000 packageshareque-0.2/packageshareque.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 08:19:46.000000 packageshareque-0.2/packageshareque.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-05-16 08:19:46.000000 packageshareque-0.2/packageshareque.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-16 08:19:47.760801 packageshareque-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      289 2023-05-16 08:17:41.000000 packageshareque-0.2/setup.py
```

