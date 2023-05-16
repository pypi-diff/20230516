# Comparing `tmp/fedinesia-2.5.0.tar.gz` & `tmp/fedinesia-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedinesia-2.5.0.tar", last modified: Sun Mar 12 01:57:53 2023, max compression
+gzip compressed data, was "fedinesia-2.5.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fedinesia-2.5.0.tar` & `fedinesia-2.5.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     3495 2023-03-12 01:57:02.079373 fedinesia-2.5.0/README.rst
--rw-r--r--   0        0        0     3716 2023-03-12 01:57:02.079373 fedinesia-2.5.0/pyproject.toml
--rw-r--r--   0        0        0      471 2023-03-12 01:57:02.079373 fedinesia-2.5.0/src/fedinesia/__init__.py
--rw-r--r--   0        0        0    13741 2023-03-12 01:57:02.079373 fedinesia-2.5.0/src/fedinesia/amnesia.py
--rw-r--r--   0        0        0    16703 2023-03-12 01:57:02.079373 fedinesia-2.5.0/src/fedinesia/config.py
--rw-r--r--   0        0        0     9042 2023-03-12 01:57:02.079373 fedinesia-2.5.0/src/fedinesia/util.py
--rw-r--r--   0        0        0     5317 1970-01-01 00:00:00.000000 fedinesia-2.5.0/PKG-INFO
+-rw-r--r--   0        0        0     3481 2023-05-16 02:01:42.571817 fedinesia-2.5.1/README.rst
+-rw-r--r--   0        0        0     3716 2023-05-16 02:01:42.571817 fedinesia-2.5.1/pyproject.toml
+-rw-r--r--   0        0        0      471 2023-05-16 02:01:42.571817 fedinesia-2.5.1/src/fedinesia/__init__.py
+-rw-r--r--   0        0        0    13741 2023-05-16 02:01:42.571817 fedinesia-2.5.1/src/fedinesia/amnesia.py
+-rw-r--r--   0        0        0    16703 2023-05-16 02:01:42.571817 fedinesia-2.5.1/src/fedinesia/config.py
+-rw-r--r--   0        0        0     9042 2023-05-16 02:01:42.571817 fedinesia-2.5.1/src/fedinesia/util.py
+-rw-r--r--   0        0        0     5303 1970-01-01 00:00:00.000000 fedinesia-2.5.1/PKG-INFO
```

### Comparing `fedinesia-2.5.0/README.rst` & `fedinesia-2.5.1/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -28,21 +28,21 @@
 Install and run from `Source <https://codeberg.org/MarvinsMastodonTools/fedinesia>`_
 ==============================================================================================
 
 Alternatively you can run Fedinesia from source by cloning the repository using the following command line::
 
     git clone https://codeberg.org/MarvinsMastodonTools/fedinesia.git
 
-Fedinesia uses `Poetry <https://python-poetry.org/>`_ for dependency control, please install Poetry before proceeding further.
+Fedinesia uses `PDM <https://pdm.fming.dev/latest/>`_ for dependency control, please install PDM before proceeding further.
 
-Before running, make sure you have all required python modules installed. With Poetry this is as easy as::
+Before running, make sure you have all required python modules installed. With PDM this is as easy as::
 
-    poetry install --only main
+    pdm sync --group :all
 
-Run Fedinesia with the command `poetry run fedinesia`
+Run Fedinesia with the command `pdm run fedinesia`
 
 Configuration / First Run
 =========================
 
 Fedinesia will ask for all necessary parameters when run for the first time and store them in ```config.json``
 file in the current directory.
```

### Comparing `fedinesia-2.5.0/pyproject.toml` & `fedinesia-2.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fedinesia-2.5.0/src/fedinesia/amnesia.py` & `fedinesia-2.5.1/src/fedinesia/amnesia.py`

 * *Files identical despite different names*

### Comparing `fedinesia-2.5.0/src/fedinesia/config.py` & `fedinesia-2.5.1/src/fedinesia/config.py`

 * *Files identical despite different names*

### Comparing `fedinesia-2.5.0/src/fedinesia/util.py` & `fedinesia-2.5.1/src/fedinesia/util.py`

 * *Files identical despite different names*

### Comparing `fedinesia-2.5.0/PKG-INFO` & `fedinesia-2.5.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedinesia
-Version: 2.5.0
+Version: 2.5.1
 Summary: Deletes old posts from fediverse accounts. Confirmed working with Mastodon and Pleroma (and Forks)
 Author-email: marvin8 <marvin8@tuta.io>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
@@ -68,21 +68,21 @@
 Install and run from `Source <https://codeberg.org/MarvinsMastodonTools/fedinesia>`_
 ==============================================================================================
 
 Alternatively you can run Fedinesia from source by cloning the repository using the following command line::
 
     git clone https://codeberg.org/MarvinsMastodonTools/fedinesia.git
 
-Fedinesia uses `Poetry <https://python-poetry.org/>`_ for dependency control, please install Poetry before proceeding further.
+Fedinesia uses `PDM <https://pdm.fming.dev/latest/>`_ for dependency control, please install PDM before proceeding further.
 
-Before running, make sure you have all required python modules installed. With Poetry this is as easy as::
+Before running, make sure you have all required python modules installed. With PDM this is as easy as::
 
-    poetry install --only main
+    pdm sync --group :all
 
-Run Fedinesia with the command `poetry run fedinesia`
+Run Fedinesia with the command `pdm run fedinesia`
 
 Configuration / First Run
 =========================
 
 Fedinesia will ask for all necessary parameters when run for the first time and store them in ```config.json``
 file in the current directory.
```

