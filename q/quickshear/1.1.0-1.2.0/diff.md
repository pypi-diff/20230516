# Comparing `tmp/quickshear-1.1.0.tar.gz` & `tmp/quickshear-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/quickshear-1.1.0.tar", last modified: Tue May 23 20:39:25 2017, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `quickshear-1.1.0.tar` & `quickshear-1.2.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxr-x   0 cjmarkie  (1002) cjmarkie  (1002)        0 2017-05-23 20:39:25.000000 quickshear-1.1.0/
-drwxrwxr-x   0 cjmarkie  (1002) cjmarkie  (1002)        0 2017-05-23 20:39:25.000000 quickshear-1.1.0/quickshear.egg-info/
--rw-rw-r--   0 cjmarkie  (1002) cjmarkie  (1002)       48 2017-05-23 20:39:25.000000 quickshear-1.1.0/quickshear.egg-info/entry_points.txt
--rw-rw-r--   0 cjmarkie  (1002) cjmarkie  (1002)     1883 2017-05-23 20:39:25.000000 quickshear-1.1.0/quickshear.egg-info/PKG-INFO
--rw-rw-r--   0 cjmarkie  (1002) cjmarkie  (1002)       14 2017-05-23 20:39:25.000000 quickshear-1.1.0/quickshear.egg-info/requires.txt
--rw-rw-r--   0 cjmarkie  (1002) cjmarkie  (1002)        1 2017-05-23 20:39:25.000000 quickshear-1.1.0/quickshear.egg-info/dependency_links.txt
--rw-rw-r--   0 cjmarkie  (1002) cjmarkie  (1002)       11 2017-05-23 20:39:25.000000 quickshear-1.1.0/quickshear.egg-info/top_level.txt
--rw-rw-r--   0 cjmarkie  (1002) cjmarkie  (1002)      239 2017-05-23 20:39:25.000000 quickshear-1.1.0/quickshear.egg-info/SOURCES.txt
--rw-rw-r--   0 cjmarkie  (1002) cjmarkie  (1002)       38 2017-05-23 20:39:25.000000 quickshear-1.1.0/setup.cfg
--rw-rw-r--   0 cjmarkie  (1002) cjmarkie  (1002)     1883 2017-05-23 20:39:25.000000 quickshear-1.1.0/PKG-INFO
--rw-rw-r--   0 cjmarkie  (1002) cjmarkie  (1002)     2899 2017-05-16 15:01:43.000000 quickshear-1.1.0/setup.py
--rwxrwxr-x   0 cjmarkie  (1002) cjmarkie  (1002)     7303 2017-05-22 19:28:24.000000 quickshear-1.1.0/quickshear.py
--rw-rw-r--   0 cjmarkie  (1002) cjmarkie  (1002)      878 2017-03-07 16:15:08.000000 quickshear-1.1.0/README.rst
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 quickshear-1.2.0/CHANGES
+-rw-r--r--   0        0        0   510510 2020-02-02 00:00:00.000000 quickshear-1.2.0/quickshear.pdf
+-rwxr-xr-x   0        0        0     6317 2020-02-02 00:00:00.000000 quickshear-1.2.0/quickshear.py
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 quickshear-1.2.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 quickshear-1.2.0/.mypy_cache/.gitignore
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 quickshear-1.2.0/.mypy_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 quickshear-1.2.0/.mypy_cache/3.10/@plugins_snapshot.json
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 quickshear-1.2.0/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 quickshear-1.2.0/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 quickshear-1.2.0/.ruff_cache/content/258253175ce71916
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 quickshear-1.2.0/LICENSE
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 quickshear-1.2.0/README.rst
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 quickshear-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3577 2020-02-02 00:00:00.000000 quickshear-1.2.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `quickshear-1.1.0/README.rst` & `quickshear-1.2.0/README.rst`

 * *Files identical despite different names*

