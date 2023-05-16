# Comparing `tmp/yifeipdf-1.0.tar.gz` & `tmp/yifeipdf-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yifeipdf-1.0.tar", last modified: Tue May 16 12:20:35 2023, max compression
+gzip compressed data, was "yifeipdf-1.1.tar", last modified: Tue May 16 14:17:04 2023, max compression
```

## Comparing `yifeipdf-1.0.tar` & `yifeipdf-1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 himmeltian   (501) staff       (20)        0 2023-05-16 12:20:35.642577 yifeipdf-1.0/
--rw-r--r--   0 himmeltian   (501) staff       (20)    35148 2023-05-16 11:51:07.000000 yifeipdf-1.0/LICENSE
--rw-r--r--   0 himmeltian   (501) staff       (20)      110 2023-05-16 12:20:35.641992 yifeipdf-1.0/PKG-INFO
--rw-r--r--   0 himmeltian   (501) staff       (20)       36 2023-05-16 11:49:45.000000 yifeipdf-1.0/README.md
-drwxr-xr-x   0 himmeltian   (501) staff       (20)        0 2023-05-16 12:20:35.635568 yifeipdf-1.0/moshpdf/
--rw-r--r--   0 himmeltian   (501) staff       (20)        0 2023-05-16 10:04:06.000000 yifeipdf-1.0/moshpdf/__init__.py
--rw-r--r--   0 himmeltian   (501) staff       (20)        0 2023-05-16 10:05:15.000000 yifeipdf-1.0/moshpdf/pdf2image.py
--rw-r--r--   0 himmeltian   (501) staff       (20)        0 2023-05-16 10:04:20.000000 yifeipdf-1.0/moshpdf/pdf2text.py
--rw-r--r--   0 himmeltian   (501) staff       (20)       38 2023-05-16 12:20:35.642720 yifeipdf-1.0/setup.cfg
--rw-r--r--   0 himmeltian   (501) staff       (20)      221 2023-05-16 12:20:31.000000 yifeipdf-1.0/setup.py
-drwxr-xr-x   0 himmeltian   (501) staff       (20)        0 2023-05-16 12:20:35.640576 yifeipdf-1.0/yifeipdf.egg-info/
--rw-r--r--   0 himmeltian   (501) staff       (20)      110 2023-05-16 12:20:35.000000 yifeipdf-1.0/yifeipdf.egg-info/PKG-INFO
--rw-r--r--   0 himmeltian   (501) staff       (20)      215 2023-05-16 12:20:35.000000 yifeipdf-1.0/yifeipdf.egg-info/SOURCES.txt
--rw-r--r--   0 himmeltian   (501) staff       (20)        1 2023-05-16 12:20:35.000000 yifeipdf-1.0/yifeipdf.egg-info/dependency_links.txt
--rw-r--r--   0 himmeltian   (501) staff       (20)        8 2023-05-16 12:20:35.000000 yifeipdf-1.0/yifeipdf.egg-info/top_level.txt
+drwxr-xr-x   0 himmeltian   (501) staff       (20)        0 2023-05-16 14:17:04.182354 yifeipdf-1.1/
+-rw-r--r--   0 himmeltian   (501) staff       (20)    35148 2023-05-16 11:51:07.000000 yifeipdf-1.1/LICENSE
+-rw-r--r--   0 himmeltian   (501) staff       (20)      110 2023-05-16 14:17:04.181363 yifeipdf-1.1/PKG-INFO
+-rw-r--r--   0 himmeltian   (501) staff       (20)       36 2023-05-16 11:49:45.000000 yifeipdf-1.1/README.md
+-rw-r--r--   0 himmeltian   (501) staff       (20)       38 2023-05-16 14:17:04.182517 yifeipdf-1.1/setup.cfg
+-rw-r--r--   0 himmeltian   (501) staff       (20)      221 2023-05-16 14:16:34.000000 yifeipdf-1.1/setup.py
+drwxr-xr-x   0 himmeltian   (501) staff       (20)        0 2023-05-16 14:17:04.176257 yifeipdf-1.1/yifeipdf/
+-rw-r--r--   0 himmeltian   (501) staff       (20)        0 2023-05-16 10:04:06.000000 yifeipdf-1.1/yifeipdf/__init__.py
+-rw-r--r--   0 himmeltian   (501) staff       (20)        0 2023-05-16 10:05:15.000000 yifeipdf-1.1/yifeipdf/pdf2image.py
+-rw-r--r--   0 himmeltian   (501) staff       (20)       36 2023-05-16 13:31:53.000000 yifeipdf-1.1/yifeipdf/pdf2text.py
+drwxr-xr-x   0 himmeltian   (501) staff       (20)        0 2023-05-16 14:17:04.180360 yifeipdf-1.1/yifeipdf.egg-info/
+-rw-r--r--   0 himmeltian   (501) staff       (20)      110 2023-05-16 14:17:04.000000 yifeipdf-1.1/yifeipdf.egg-info/PKG-INFO
+-rw-r--r--   0 himmeltian   (501) staff       (20)      218 2023-05-16 14:17:04.000000 yifeipdf-1.1/yifeipdf.egg-info/SOURCES.txt
+-rw-r--r--   0 himmeltian   (501) staff       (20)        1 2023-05-16 14:17:04.000000 yifeipdf-1.1/yifeipdf.egg-info/dependency_links.txt
+-rw-r--r--   0 himmeltian   (501) staff       (20)        9 2023-05-16 14:17:04.000000 yifeipdf-1.1/yifeipdf.egg-info/top_level.txt
```

### Comparing `yifeipdf-1.0/LICENSE` & `yifeipdf-1.1/LICENSE`

 * *Files identical despite different names*

