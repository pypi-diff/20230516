# Comparing `tmp/tutorialleigos-0.1.0.tar.gz` & `tmp/tutorialleigos-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tutorialleigos-0.1.0.tar", max compression
+gzip compressed data, was "tutorialleigos-0.1.1.tar", max compression
```

## Comparing `tutorialleigos-0.1.0.tar` & `tutorialleigos-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       27 2023-05-16 14:55:17.484464 tutorialleigos-0.1.0/README.md
--rw-r--r--   0        0        0      377 2023-05-16 14:53:16.956531 tutorialleigos-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-16 13:23:11.886299 tutorialleigos-0.1.0/tutorialleigos/__init__.py
--rw-r--r--   0        0        0      106 2023-05-16 13:41:25.715136 tutorialleigos-0.1.0/tutorialleigos/codigo.py
--rw-r--r--   0        0        0      357 1970-01-01 00:00:00.000000 tutorialleigos-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       27 2023-05-16 14:55:17.484464 tutorialleigos-0.1.1/README.md
+-rw-r--r--   0        0        0      377 2023-05-16 15:00:41.548285 tutorialleigos-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-16 13:23:11.886299 tutorialleigos-0.1.1/tutorialleigos/__init__.py
+-rw-r--r--   0        0        0      106 2023-05-16 13:41:25.715136 tutorialleigos-0.1.1/tutorialleigos/codigo.py
+-rw-r--r--   0        0        0      357 1970-01-01 00:00:00.000000 tutorialleigos-0.1.1/PKG-INFO
```

