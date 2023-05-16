# Comparing `tmp/kotan-0.1.1.tar.gz` & `tmp/kotan-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kotan-0.1.1.tar", max compression
+gzip compressed data, was "kotan-0.1.2.tar", max compression
```

## Comparing `kotan-0.1.1.tar` & `kotan-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2023-05-16 05:09:07.710676 kotan-0.1.1/README.md
--rw-r--r--   0        0        0       41 2023-05-16 05:09:07.710676 kotan-0.1.1/kotan/__init__.py
--rw-r--r--   0        0        0      299 2023-05-16 05:09:07.710676 kotan-0.1.1/kotan/const.py
--rw-r--r--   0        0        0     2123 2023-05-16 05:09:07.710676 kotan-0.1.1/kotan/job.py
--rw-r--r--   0        0        0      112 2023-05-16 05:09:07.710676 kotan-0.1.1/kotan/tasks/__init__.py
--rw-r--r--   0        0        0     3252 2023-05-16 05:09:07.710676 kotan-0.1.1/kotan/tasks/data_augmentation.py
--rw-r--r--   0        0        0     2590 2023-05-16 05:09:07.710676 kotan-0.1.1/kotan/tasks/machine_translation.py
--rw-r--r--   0        0        0      301 2023-05-16 05:13:12.587413 kotan-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      508 1970-01-01 00:00:00.000000 kotan-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-16 05:09:07.710676 kotan-0.1.2/README.md
+-rw-r--r--   0        0        0       41 2023-05-16 05:09:07.710676 kotan-0.1.2/kotan/__init__.py
+-rw-r--r--   0        0        0      299 2023-05-16 05:09:07.710676 kotan-0.1.2/kotan/const.py
+-rw-r--r--   0        0        0     2123 2023-05-16 05:09:07.710676 kotan-0.1.2/kotan/job.py
+-rw-r--r--   0        0        0      112 2023-05-16 05:09:07.710676 kotan-0.1.2/kotan/tasks/__init__.py
+-rw-r--r--   0        0        0     3252 2023-05-16 05:09:07.710676 kotan-0.1.2/kotan/tasks/data_augmentation.py
+-rw-r--r--   0        0        0     2590 2023-05-16 05:09:07.710676 kotan-0.1.2/kotan/tasks/machine_translation.py
+-rw-r--r--   0        0        0      327 2023-05-16 05:22:08.764022 kotan-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      555 1970-01-01 00:00:00.000000 kotan-0.1.2/PKG-INFO
```

### Comparing `kotan-0.1.1/kotan/job.py` & `kotan-0.1.2/kotan/job.py`

 * *Files identical despite different names*

### Comparing `kotan-0.1.1/kotan/tasks/data_augmentation.py` & `kotan-0.1.2/kotan/tasks/data_augmentation.py`

 * *Files identical despite different names*

### Comparing `kotan-0.1.1/kotan/tasks/machine_translation.py` & `kotan-0.1.2/kotan/tasks/machine_translation.py`

 * *Files identical despite different names*

