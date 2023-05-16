# Comparing `tmp/adaptive-cards-py-0.0.5.tar.gz` & `tmp/adaptive-cards-py-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adaptive-cards-py-0.0.5.tar", last modified: Thu Apr 27 18:28:36 2023, max compression
+gzip compressed data, was "adaptive-cards-py-0.0.6.tar", last modified: Tue May 16 18:53:12 2023, max compression
```

## Comparing `adaptive-cards-py-0.0.5.tar` & `adaptive-cards-py-0.0.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 dennis    (1000) dennis    (1000)        0 2023-04-27 18:28:36.935849 adaptive-cards-py-0.0.5/
--rw-r--r--   0 dennis    (1000) dennis    (1000)     1068 2023-04-24 18:32:53.000000 adaptive-cards-py-0.0.5/LICENSE
--rw-r--r--   0 dennis    (1000) dennis    (1000)       41 2023-04-27 18:12:27.000000 adaptive-cards-py-0.0.5/MANIFEST.in
--rw-r--r--   0 dennis    (1000) dennis    (1000)     8520 2023-04-27 18:28:36.935849 adaptive-cards-py-0.0.5/PKG-INFO
--rw-r--r--   0 dennis    (1000) dennis    (1000)     6785 2023-04-27 18:28:26.000000 adaptive-cards-py-0.0.5/README.md
-drwxr-xr-x   0 dennis    (1000) dennis    (1000)        0 2023-04-27 18:28:36.935849 adaptive-cards-py-0.0.5/adaptive_cards/
--rw-r--r--   0 dennis    (1000) dennis    (1000)        0 2023-04-27 18:12:27.000000 adaptive-cards-py-0.0.5/adaptive_cards/__init__.py
--rw-r--r--   0 dennis    (1000) dennis    (1000)     3602 2023-04-25 16:45:04.000000 adaptive-cards-py-0.0.5/adaptive_cards/actions.py
--rw-r--r--   0 dennis    (1000) dennis    (1000)     5615 2023-04-27 18:19:30.000000 adaptive-cards-py-0.0.5/adaptive_cards/card.py
--rw-r--r--   0 dennis    (1000) dennis    (1000)     4592 2023-04-27 18:12:27.000000 adaptive-cards-py-0.0.5/adaptive_cards/card_types.py
--rw-r--r--   0 dennis    (1000) dennis    (1000)     8375 2023-04-25 16:45:04.000000 adaptive-cards-py-0.0.5/adaptive_cards/containers.py
--rw-r--r--   0 dennis    (1000) dennis    (1000)     6013 2023-04-25 16:45:04.000000 adaptive-cards-py-0.0.5/adaptive_cards/elements.py
--rw-r--r--   0 dennis    (1000) dennis    (1000)     5753 2023-04-25 16:45:04.000000 adaptive-cards-py-0.0.5/adaptive_cards/inputs.py
--rw-r--r--   0 dennis    (1000) dennis    (1000)      216 2023-04-25 16:45:04.000000 adaptive-cards-py-0.0.5/adaptive_cards/utils.py
--rw-r--r--   0 dennis    (1000) dennis    (1000)     3140 2023-04-26 17:52:15.000000 adaptive-cards-py-0.0.5/adaptive_cards/validation.py
-drwxr-xr-x   0 dennis    (1000) dennis    (1000)        0 2023-04-27 18:28:36.935849 adaptive-cards-py-0.0.5/adaptive_cards_py.egg-info/
--rw-r--r--   0 dennis    (1000) dennis    (1000)     8520 2023-04-27 18:28:36.000000 adaptive-cards-py-0.0.5/adaptive_cards_py.egg-info/PKG-INFO
--rw-r--r--   0 dennis    (1000) dennis    (1000)      563 2023-04-27 18:28:36.000000 adaptive-cards-py-0.0.5/adaptive_cards_py.egg-info/SOURCES.txt
--rw-r--r--   0 dennis    (1000) dennis    (1000)        1 2023-04-27 18:28:36.000000 adaptive-cards-py-0.0.5/adaptive_cards_py.egg-info/dependency_links.txt
--rw-r--r--   0 dennis    (1000) dennis    (1000)       25 2023-04-27 18:28:36.000000 adaptive-cards-py-0.0.5/adaptive_cards_py.egg-info/requires.txt
--rw-r--r--   0 dennis    (1000) dennis    (1000)       15 2023-04-27 18:28:36.000000 adaptive-cards-py-0.0.5/adaptive_cards_py.egg-info/top_level.txt
-drwxr-xr-x   0 dennis    (1000) dennis    (1000)        0 2023-04-27 18:28:36.935849 adaptive-cards-py-0.0.5/examples/
-drwxr-xr-x   0 dennis    (1000) dennis    (1000)        0 2023-04-27 18:28:36.935849 adaptive-cards-py-0.0.5/examples/simple_card/
--rw-r--r--   0 dennis    (1000) dennis    (1000)     7670 2023-04-26 17:52:15.000000 adaptive-cards-py-0.0.5/examples/simple_card/simple_card.jpg
--rw-r--r--   0 dennis    (1000) dennis    (1000)    20672 2023-04-26 17:52:15.000000 adaptive-cards-py-0.0.5/examples/simple_card/simple_card_2.jpg
--rw-r--r--   0 dennis    (1000) dennis    (1000)      711 2023-04-27 18:27:46.000000 adaptive-cards-py-0.0.5/pyproject.toml
--rw-r--r--   0 dennis    (1000) dennis    (1000)       38 2023-04-27 18:28:36.935849 adaptive-cards-py-0.0.5/setup.cfg
+drwxr-xr-x   0 dennis    (1000) dennis    (1000)        0 2023-05-16 18:53:12.629420 adaptive-cards-py-0.0.6/
+-rw-r--r--   0 dennis    (1000) dennis    (1000)     1068 2023-04-24 18:32:53.000000 adaptive-cards-py-0.0.6/LICENSE
+-rw-r--r--   0 dennis    (1000) dennis    (1000)       41 2023-04-27 18:12:27.000000 adaptive-cards-py-0.0.6/MANIFEST.in
+-rw-r--r--   0 dennis    (1000) dennis    (1000)    23576 2023-05-16 18:53:12.629420 adaptive-cards-py-0.0.6/PKG-INFO
+-rw-r--r--   0 dennis    (1000) dennis    (1000)    21841 2023-05-16 18:48:35.000000 adaptive-cards-py-0.0.6/README.md
+drwxr-xr-x   0 dennis    (1000) dennis    (1000)        0 2023-05-16 18:53:12.619420 adaptive-cards-py-0.0.6/adaptive_cards/
+-rw-r--r--   0 dennis    (1000) dennis    (1000)        0 2023-04-27 18:12:27.000000 adaptive-cards-py-0.0.6/adaptive_cards/__init__.py
+-rw-r--r--   0 dennis    (1000) dennis    (1000)     3602 2023-05-16 18:07:56.000000 adaptive-cards-py-0.0.6/adaptive_cards/actions.py
+-rw-r--r--   0 dennis    (1000) dennis    (1000)     5615 2023-05-16 18:07:56.000000 adaptive-cards-py-0.0.6/adaptive_cards/card.py
+-rw-r--r--   0 dennis    (1000) dennis    (1000)     4592 2023-05-16 18:07:56.000000 adaptive-cards-py-0.0.6/adaptive_cards/card_types.py
+-rw-r--r--   0 dennis    (1000) dennis    (1000)     8375 2023-05-16 18:07:56.000000 adaptive-cards-py-0.0.6/adaptive_cards/containers.py
+-rw-r--r--   0 dennis    (1000) dennis    (1000)     6013 2023-05-16 18:07:56.000000 adaptive-cards-py-0.0.6/adaptive_cards/elements.py
+-rw-r--r--   0 dennis    (1000) dennis    (1000)     5753 2023-05-16 18:07:56.000000 adaptive-cards-py-0.0.6/adaptive_cards/inputs.py
+-rw-r--r--   0 dennis    (1000) dennis    (1000)      216 2023-05-16 18:07:56.000000 adaptive-cards-py-0.0.6/adaptive_cards/utils.py
+-rw-r--r--   0 dennis    (1000) dennis    (1000)     3140 2023-05-16 18:07:56.000000 adaptive-cards-py-0.0.6/adaptive_cards/validation.py
+drwxr-xr-x   0 dennis    (1000) dennis    (1000)        0 2023-05-16 18:53:12.619420 adaptive-cards-py-0.0.6/adaptive_cards_py.egg-info/
+-rw-r--r--   0 dennis    (1000) dennis    (1000)    23576 2023-05-16 18:53:12.000000 adaptive-cards-py-0.0.6/adaptive_cards_py.egg-info/PKG-INFO
+-rw-r--r--   0 dennis    (1000) dennis    (1000)      563 2023-05-16 18:53:12.000000 adaptive-cards-py-0.0.6/adaptive_cards_py.egg-info/SOURCES.txt
+-rw-r--r--   0 dennis    (1000) dennis    (1000)        1 2023-05-16 18:53:12.000000 adaptive-cards-py-0.0.6/adaptive_cards_py.egg-info/dependency_links.txt
+-rw-r--r--   0 dennis    (1000) dennis    (1000)       25 2023-05-16 18:53:12.000000 adaptive-cards-py-0.0.6/adaptive_cards_py.egg-info/requires.txt
+-rw-r--r--   0 dennis    (1000) dennis    (1000)       15 2023-05-16 18:53:12.000000 adaptive-cards-py-0.0.6/adaptive_cards_py.egg-info/top_level.txt
+drwxr-xr-x   0 dennis    (1000) dennis    (1000)        0 2023-05-16 18:53:12.619420 adaptive-cards-py-0.0.6/examples/
+drwxr-xr-x   0 dennis    (1000) dennis    (1000)        0 2023-05-16 18:53:12.619420 adaptive-cards-py-0.0.6/examples/simple_card/
+-rw-r--r--   0 dennis    (1000) dennis    (1000)     7670 2023-04-26 17:52:15.000000 adaptive-cards-py-0.0.6/examples/simple_card/simple_card.jpg
+-rw-r--r--   0 dennis    (1000) dennis    (1000)    20672 2023-04-26 17:52:15.000000 adaptive-cards-py-0.0.6/examples/simple_card/simple_card_2.jpg
+-rw-r--r--   0 dennis    (1000) dennis    (1000)      711 2023-05-16 18:53:00.000000 adaptive-cards-py-0.0.6/pyproject.toml
+-rw-r--r--   0 dennis    (1000) dennis    (1000)       38 2023-05-16 18:53:12.629420 adaptive-cards-py-0.0.6/setup.cfg
```

### Comparing `adaptive-cards-py-0.0.5/LICENSE` & `adaptive-cards-py-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `adaptive-cards-py-0.0.5/adaptive_cards/actions.py` & `adaptive-cards-py-0.0.6/adaptive_cards/actions.py`

 * *Files identical despite different names*

### Comparing `adaptive-cards-py-0.0.5/adaptive_cards/card.py` & `adaptive-cards-py-0.0.6/adaptive_cards/card.py`

 * *Files identical despite different names*

### Comparing `adaptive-cards-py-0.0.5/adaptive_cards/card_types.py` & `adaptive-cards-py-0.0.6/adaptive_cards/card_types.py`

 * *Files identical despite different names*

### Comparing `adaptive-cards-py-0.0.5/adaptive_cards/containers.py` & `adaptive-cards-py-0.0.6/adaptive_cards/containers.py`

 * *Files identical despite different names*

### Comparing `adaptive-cards-py-0.0.5/adaptive_cards/elements.py` & `adaptive-cards-py-0.0.6/adaptive_cards/elements.py`

 * *Files identical despite different names*

### Comparing `adaptive-cards-py-0.0.5/adaptive_cards/inputs.py` & `adaptive-cards-py-0.0.6/adaptive_cards/inputs.py`

 * *Files identical despite different names*

### Comparing `adaptive-cards-py-0.0.5/adaptive_cards/validation.py` & `adaptive-cards-py-0.0.6/adaptive_cards/validation.py`

 * *Files identical despite different names*

### Comparing `adaptive-cards-py-0.0.5/adaptive_cards_py.egg-info/SOURCES.txt` & `adaptive-cards-py-0.0.6/adaptive_cards_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adaptive-cards-py-0.0.5/examples/simple_card/simple_card.jpg` & `adaptive-cards-py-0.0.6/examples/simple_card/simple_card.jpg`

 * *Files identical despite different names*

### Comparing `adaptive-cards-py-0.0.5/examples/simple_card/simple_card_2.jpg` & `adaptive-cards-py-0.0.6/examples/simple_card/simple_card_2.jpg`

 * *Files identical despite different names*

### Comparing `adaptive-cards-py-0.0.5/pyproject.toml` & `adaptive-cards-py-0.0.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "adaptive-cards-py"
-version = "0.0.5"
+version = "0.0.6"
 description = "Python wrapper library for building beautiful adaptive cards"
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 readme = "README.md"
```

