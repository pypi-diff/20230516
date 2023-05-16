# Comparing `tmp/VPworldPDF-1.0.tar.gz` & `tmp/VPworldPDF-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VPworldPDF-1.0.tar", last modified: Mon May 15 10:29:28 2023, max compression
+gzip compressed data, was "VPworldPDF-1.1.tar", last modified: Tue May 16 08:30:30 2023, max compression
```

## Comparing `VPworldPDF-1.0.tar` & `VPworldPDF-1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 10:29:28.250949 VPworldPDF-1.0/
--rw-rw-rw-   0        0        0    35821 2023-05-15 10:28:50.000000 VPworldPDF-1.0/LICENSE
--rw-rw-rw-   0        0        0      194 2023-05-15 10:29:28.250949 VPworldPDF-1.0/PKG-INFO
--rw-rw-rw-   0        0        0      112 2023-05-15 10:28:49.000000 VPworldPDF-1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 10:29:28.198860 VPworldPDF-1.0/VPworldPDF/
--rw-rw-rw-   0        0        0        0 2023-05-15 10:14:55.000000 VPworldPDF-1.0/VPworldPDF/__init__.py
--rw-rw-rw-   0        0        0        0 2023-05-15 10:16:19.000000 VPworldPDF-1.0/VPworldPDF/pdf2image.py
--rw-rw-rw-   0        0        0       39 2023-05-15 10:15:49.000000 VPworldPDF-1.0/VPworldPDF/pdf2text.py
-drwxrwxrwx   0        0        0        0 2023-05-15 10:29:28.250949 VPworldPDF-1.0/VPworldPDF.egg-info/
--rw-rw-rw-   0        0        0      194 2023-05-15 10:29:28.000000 VPworldPDF-1.0/VPworldPDF.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      232 2023-05-15 10:29:28.000000 VPworldPDF-1.0/VPworldPDF.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 10:29:28.000000 VPworldPDF-1.0/VPworldPDF.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-15 10:29:28.000000 VPworldPDF-1.0/VPworldPDF.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-15 10:29:28.250949 VPworldPDF-1.0/setup.cfg
--rw-rw-rw-   0        0        0      230 2023-05-15 10:28:56.000000 VPworldPDF-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 08:30:30.872795 VPworldPDF-1.1/
+-rw-rw-rw-   0        0        0    35821 2023-05-15 10:28:50.000000 VPworldPDF-1.1/LICENSE
+-rw-rw-rw-   0        0        0      425 2023-05-16 08:30:30.872795 VPworldPDF-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      112 2023-05-15 10:28:49.000000 VPworldPDF-1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-16 08:30:30.861931 VPworldPDF-1.1/VPworldPDF/
+-rw-rw-rw-   0        0        0        0 2023-05-15 10:14:55.000000 VPworldPDF-1.1/VPworldPDF/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-05-15 10:16:19.000000 VPworldPDF-1.1/VPworldPDF/pdf2image.py
+-rw-rw-rw-   0        0        0     1285 2023-05-16 08:21:38.000000 VPworldPDF-1.1/VPworldPDF/pdf2text.py
+drwxrwxrwx   0        0        0        0 2023-05-16 08:30:30.872048 VPworldPDF-1.1/VPworldPDF.egg-info/
+-rw-rw-rw-   0        0        0      425 2023-05-16 08:30:30.000000 VPworldPDF-1.1/VPworldPDF.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2023-05-16 08:30:30.000000 VPworldPDF-1.1/VPworldPDF.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 08:30:30.000000 VPworldPDF-1.1/VPworldPDF.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-16 08:30:30.000000 VPworldPDF-1.1/VPworldPDF.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-16 08:30:30.872795 VPworldPDF-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      504 2023-05-16 08:28:38.000000 VPworldPDF-1.1/setup.py
```

### Comparing `VPworldPDF-1.0/LICENSE` & `VPworldPDF-1.1/LICENSE`

 * *Files identical despite different names*

