# Comparing `tmp/Swaiter-1.0.1.tar.gz` & `tmp/Swaiter-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Swaiter-1.0.1.tar", last modified: Tue May 16 07:31:26 2023, max compression
+gzip compressed data, was "Swaiter-1.0.2.tar", last modified: Tue May 16 07:44:38 2023, max compression
```

## Comparing `Swaiter-1.0.1.tar` & `Swaiter-1.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 07:31:26.641282 Swaiter-1.0.1/
--rw-rw-rw-   0        0        0       54 2023-05-16 07:31:26.641282 Swaiter-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-16 07:31:26.639272 Swaiter-1.0.1/Swaiter.egg-info/
--rw-rw-rw-   0        0        0       54 2023-05-16 07:31:26.000000 Swaiter-1.0.1/Swaiter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-05-16 07:31:26.000000 Swaiter-1.0.1/Swaiter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 07:31:26.000000 Swaiter-1.0.1/Swaiter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-16 07:31:26.000000 Swaiter-1.0.1/Swaiter.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-16 07:31:26.000000 Swaiter-1.0.1/Swaiter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4209 2023-05-16 07:13:32.000000 Swaiter-1.0.1/Waiter.py
--rw-rw-rw-   0        0        0       97 2023-05-16 07:31:07.000000 Swaiter-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-16 07:31:26.641282 Swaiter-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-16 07:44:38.856897 Swaiter-1.0.2/
+-rw-rw-rw-   0        0        0       54 2023-05-16 07:44:38.854741 Swaiter-1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-16 07:44:38.854741 Swaiter-1.0.2/Swaiter.egg-info/
+-rw-rw-rw-   0        0        0       54 2023-05-16 07:44:38.000000 Swaiter-1.0.2/Swaiter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-05-16 07:44:38.000000 Swaiter-1.0.2/Swaiter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 07:44:38.000000 Swaiter-1.0.2/Swaiter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-05-16 07:44:38.000000 Swaiter-1.0.2/Swaiter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-16 07:44:38.000000 Swaiter-1.0.2/Swaiter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4209 2023-05-16 07:13:32.000000 Swaiter-1.0.2/Waiter.py
+-rw-rw-rw-   0        0        0       97 2023-05-16 07:44:15.000000 Swaiter-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-16 07:44:38.856897 Swaiter-1.0.2/setup.cfg
```

### Comparing `Swaiter-1.0.1/Waiter.py` & `Swaiter-1.0.2/Waiter.py`

 * *Files identical despite different names*

