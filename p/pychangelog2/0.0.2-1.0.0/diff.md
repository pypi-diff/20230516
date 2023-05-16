# Comparing `tmp/pychangelog2-0.0.2.tar.gz` & `tmp/pychangelog2-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pychangelog2-0.0.2.tar", last modified: Thu Nov 24 11:34:31 2022, max compression
+gzip compressed data, was "pychangelog2-1.0.0.tar", last modified: Tue May 16 08:04:03 2023, max compression
```

## Comparing `pychangelog2-0.0.2.tar` & `pychangelog2-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 11:34:31.443594 pychangelog2-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (122)    35147 2022-11-24 11:34:23.000000 pychangelog2-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     1312 2022-11-24 11:34:31.443594 pychangelog2-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      761 2022-11-24 11:34:23.000000 pychangelog2-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 11:34:31.443594 pychangelog2-0.0.2/pychangelog2/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-24 11:34:23.000000 pychangelog2-0.0.2/pychangelog2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      891 2022-11-24 11:34:23.000000 pychangelog2-0.0.2/pychangelog2/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 11:34:31.443594 pychangelog2-0.0.2/pychangelog2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1312 2022-11-24 11:34:31.000000 pychangelog2-0.0.2/pychangelog2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      294 2022-11-24 11:34:31.000000 pychangelog2-0.0.2/pychangelog2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-24 11:34:31.000000 pychangelog2-0.0.2/pychangelog2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       59 2022-11-24 11:34:31.000000 pychangelog2-0.0.2/pychangelog2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       16 2022-11-24 11:34:31.000000 pychangelog2-0.0.2/pychangelog2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2022-11-24 11:34:31.000000 pychangelog2-0.0.2/pychangelog2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-24 11:34:31.443594 pychangelog2-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1671 2022-11-24 11:34:23.000000 pychangelog2-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:04:03.496966 pychangelog2-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-16 08:03:47.000000 pychangelog2-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    42285 2023-05-16 08:04:03.496966 pychangelog2-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-16 08:03:47.000000 pychangelog2-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:04:03.496966 pychangelog2-1.0.0/pychangelog2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 08:03:47.000000 pychangelog2-1.0.0/pychangelog2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-16 08:03:47.000000 pychangelog2-1.0.0/pychangelog2/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:04:03.496966 pychangelog2-1.0.0/pychangelog2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    42285 2023-05-16 08:04:03.000000 pychangelog2-1.0.0/pychangelog2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-16 08:04:03.000000 pychangelog2-1.0.0/pychangelog2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 08:04:03.000000 pychangelog2-1.0.0/pychangelog2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-16 08:04:03.000000 pychangelog2-1.0.0/pychangelog2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-16 08:04:03.000000 pychangelog2-1.0.0/pychangelog2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-16 08:04:03.000000 pychangelog2-1.0.0/pychangelog2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-16 08:03:47.000000 pychangelog2-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-16 08:03:47.000000 pychangelog2-1.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 08:04:03.496966 pychangelog2-1.0.0/setup.cfg
```

### Comparing `pychangelog2-0.0.2/LICENSE` & `pychangelog2-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pychangelog2-0.0.2/README.md` & `pychangelog2-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pychangelog2-0.0.2/pychangelog2/__main__.py` & `pychangelog2-1.0.0/pychangelog2/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     for tag in repo.tags:
         if tag.commit.authored_date > last_authored_date:
             last_authored_date = tag.commit.authored_date
             last_tag = tag
 
     commits = []
     for commit in repo.iter_commits():
-        if commit.message.startswith('Merge pull request'):
+        if commit.message.startswith('Merge '):
             # skip merge requests
             continue
         if commit == last_tag.commit:
             # reaches last tag
             break
         commits.append(commit)
```

