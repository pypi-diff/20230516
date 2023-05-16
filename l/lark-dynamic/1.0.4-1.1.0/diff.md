# Comparing `tmp/lark_dynamic-1.0.4.tar.gz` & `tmp/lark_dynamic-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\lark_dynamic-1.0.4.tar", last modified: Sun Jun 26 15:47:33 2022, max compression
+gzip compressed data, was "lark_dynamic-1.1.0.tar", max compression
```

## Comparing `lark_dynamic-1.0.4.tar` & `lark_dynamic-1.1.0.tar`

### file list

```diff
@@ -1,12 +1,14 @@
-drwxrwxrwx   0        0        0        0 2022-06-26 15:47:33.109653 lark_dynamic-1.0.4/
--rw-rw-rw-   0        0        0    17545 2022-06-26 15:47:33.109653 lark_dynamic-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0    12727 2022-06-26 15:46:58.000000 lark_dynamic-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2022-06-26 15:47:33.108652 lark_dynamic-1.0.4/lark_dynamic.egg-info/
--rw-rw-rw-   0        0        0    17545 2022-06-26 15:47:33.000000 lark_dynamic-1.0.4/lark_dynamic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      213 2022-06-26 15:47:33.000000 lark_dynamic-1.0.4/lark_dynamic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-26 15:47:33.000000 lark_dynamic-1.0.4/lark_dynamic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2022-06-26 15:47:33.000000 lark_dynamic-1.0.4/lark_dynamic.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2022-06-26 15:47:33.000000 lark_dynamic-1.0.4/lark_dynamic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    15308 2022-06-26 15:39:47.000000 lark_dynamic-1.0.4/lark_dynamic.py
--rw-rw-rw-   0        0        0       42 2022-06-26 15:47:33.109653 lark_dynamic-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      932 2022-06-26 15:47:03.000000 lark_dynamic-1.0.4/setup.py
+-rw-r--r--   0        0        0     1068 2023-05-16 13:43:39.024142 lark_dynamic-1.1.0/LICENSE
+-rw-r--r--   0        0        0      767 2023-05-16 13:43:39.024142 lark_dynamic-1.1.0/lark_dynamic/__init__.py
+-rw-r--r--   0        0        0     3471 2023-05-16 13:43:39.024142 lark_dynamic-1.1.0/lark_dynamic/atoms.py
+-rw-r--r--   0        0        0     4751 2023-05-16 13:43:39.024142 lark_dynamic-1.1.0/lark_dynamic/combinators.py
+-rw-r--r--   0        0        0       60 2023-05-16 13:43:39.024142 lark_dynamic-1.1.0/lark_dynamic/constants.py
+-rw-r--r--   0        0        0     3347 2023-05-16 13:43:39.024142 lark_dynamic-1.1.0/lark_dynamic/definitions.py
+-rw-r--r--   0        0        0     6216 2023-05-16 13:43:39.024142 lark_dynamic-1.1.0/lark_dynamic/grammar.py
+-rw-r--r--   0        0        0      578 2023-05-16 13:43:39.024142 lark_dynamic-1.1.0/lark_dynamic/modifier.py
+-rw-r--r--   0        0        0        0 2023-05-16 13:43:39.024142 lark_dynamic-1.1.0/lark_dynamic/py.typed
+-rw-r--r--   0        0        0     1239 2023-05-16 13:43:39.024142 lark_dynamic-1.1.0/lark_dynamic/token.py
+-rw-r--r--   0        0        0      513 2023-05-16 13:43:39.024142 lark_dynamic-1.1.0/lark_dynamic/utils.py
+-rw-r--r--   0        0        0      913 2023-05-16 13:43:39.024142 lark_dynamic-1.1.0/lark_dynamic/variable.py
+-rw-r--r--   0        0        0      372 2023-05-16 13:43:39.024142 lark_dynamic-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 lark_dynamic-1.1.0/PKG-INFO
```

