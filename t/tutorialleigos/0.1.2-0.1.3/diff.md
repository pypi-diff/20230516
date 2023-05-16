# Comparing `tmp/tutorialleigos-0.1.2.tar.gz` & `tmp/tutorialleigos-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tutorialleigos-0.1.2.tar", max compression
+gzip compressed data, was "tutorialleigos-0.1.3.tar", max compression
```

## Comparing `tutorialleigos-0.1.2.tar` & `tutorialleigos-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       27 2023-05-16 14:55:17.484464 tutorialleigos-0.1.2/README.md
--rw-r--r--   0        0        0      377 2023-05-16 15:05:36.524121 tutorialleigos-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-16 13:23:11.886299 tutorialleigos-0.1.2/tutorialleigos/__init__.py
--rw-r--r--   0        0        0      106 2023-05-16 13:41:25.715136 tutorialleigos-0.1.2/tutorialleigos/codigo.py
--rw-r--r--   0        0        0      357 1970-01-01 00:00:00.000000 tutorialleigos-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       27 2023-05-16 14:55:17.484464 tutorialleigos-0.1.3/README.md
+-rw-r--r--   0        0        0      376 2023-05-16 15:18:15.180712 tutorialleigos-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-16 13:23:11.886299 tutorialleigos-0.1.3/tutorialleigos/__init__.py
+-rw-r--r--   0        0        0      106 2023-05-16 13:41:25.715136 tutorialleigos-0.1.3/tutorialleigos/codigo.py
+-rw-r--r--   0        0        0      507 1970-01-01 00:00:00.000000 tutorialleigos-0.1.3/PKG-INFO
```

