# Comparing `tmp/characterai-0.4.0.tar.gz` & `tmp/characterai-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\characterai-0.4.0.tar", last modified: Tue May 16 20:10:00 2023, max compression
+gzip compressed data, was "dist\characterai-0.4.1.tar", last modified: Tue May 16 20:11:17 2023, max compression
```

## Comparing `characterai-0.4.0.tar` & `characterai-0.4.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 20:10:00.426690 characterai-0.4.0/
--rw-rw-rw-   0        0        0     1082 2023-04-28 16:51:34.000000 characterai-0.4.0/LICENSE
--rw-rw-rw-   0        0        0      358 2023-05-16 20:10:00.422687 characterai-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     1481 2023-05-01 15:25:41.000000 characterai-0.4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-16 20:10:00.292480 characterai-0.4.0/characterai/
--rw-rw-rw-   0        0        0       90 2023-05-05 18:13:37.000000 characterai-0.4.0/characterai/__init__.py
--rw-rw-rw-   0        0        0     6548 2023-05-16 20:04:21.000000 characterai-0.4.0/characterai/characterai.py
--rw-rw-rw-   0        0        0      126 2023-05-16 17:53:10.000000 characterai-0.4.0/characterai/errors.py
--rw-rw-rw-   0        0        0     6879 2023-05-16 20:02:20.000000 characterai-0.4.0/characterai/pyasynccai.py
-drwxrwxrwx   0        0        0        0 2023-05-16 20:10:00.418687 characterai-0.4.0/characterai.egg-info/
--rw-rw-rw-   0        0        0      358 2023-05-16 20:09:59.000000 characterai-0.4.0/characterai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-05-16 20:09:59.000000 characterai-0.4.0/characterai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 20:09:59.000000 characterai-0.4.0/characterai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-05-16 20:09:59.000000 characterai-0.4.0/characterai.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-16 20:09:59.000000 characterai-0.4.0/characterai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-16 20:10:00.427691 characterai-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0      448 2023-05-16 20:08:52.000000 characterai-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 20:11:17.812631 characterai-0.4.1/
+-rw-rw-rw-   0        0        0     1082 2023-04-28 16:51:34.000000 characterai-0.4.1/LICENSE
+-rw-rw-rw-   0        0        0     1873 2023-05-16 20:11:17.807631 characterai-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1481 2023-05-01 15:25:41.000000 characterai-0.4.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-16 20:11:17.736160 characterai-0.4.1/characterai/
+-rw-rw-rw-   0        0        0       90 2023-05-05 18:13:37.000000 characterai-0.4.1/characterai/__init__.py
+-rw-rw-rw-   0        0        0     6548 2023-05-16 20:04:21.000000 characterai-0.4.1/characterai/characterai.py
+-rw-rw-rw-   0        0        0      126 2023-05-16 17:53:10.000000 characterai-0.4.1/characterai/errors.py
+-rw-rw-rw-   0        0        0     6879 2023-05-16 20:02:20.000000 characterai-0.4.1/characterai/pyasynccai.py
+drwxrwxrwx   0        0        0        0 2023-05-16 20:11:17.801631 characterai-0.4.1/characterai.egg-info/
+-rw-rw-rw-   0        0        0     1873 2023-05-16 20:11:17.000000 characterai-0.4.1/characterai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-05-16 20:11:17.000000 characterai-0.4.1/characterai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 20:11:17.000000 characterai-0.4.1/characterai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-05-16 20:11:17.000000 characterai-0.4.1/characterai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-16 20:11:17.000000 characterai-0.4.1/characterai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-16 20:11:17.813634 characterai-0.4.1/setup.cfg
+-rw-rw-rw-   0        0        0      622 2023-05-16 20:11:12.000000 characterai-0.4.1/setup.py
```

### Comparing `characterai-0.4.0/LICENSE` & `characterai-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `characterai-0.4.0/README.md` & `characterai-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `characterai-0.4.0/characterai/characterai.py` & `characterai-0.4.1/characterai/characterai.py`

 * *Files identical despite different names*

### Comparing `characterai-0.4.0/characterai/pyasynccai.py` & `characterai-0.4.1/characterai/pyasynccai.py`

 * *Files identical despite different names*

