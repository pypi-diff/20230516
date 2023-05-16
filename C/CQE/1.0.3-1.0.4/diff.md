# Comparing `tmp/CQE-1.0.3.tar.gz` & `tmp/CQE-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CQE-1.0.3.tar", last modified: Tue May 16 12:08:17 2023, max compression
+gzip compressed data, was "CQE-1.0.4.tar", last modified: Tue May 16 12:50:06 2023, max compression
```

## Comparing `CQE-1.0.3.tar` & `CQE-1.0.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 satyaalmasian   (501) staff       (20)        0 2023-05-16 12:08:17.319309 CQE-1.0.3/
-drwxr-xr-x   0 satyaalmasian   (501) staff       (20)        0 2023-05-16 12:08:17.314786 CQE-1.0.3/CQE/
--rw-r--r--   0 satyaalmasian   (501) staff       (20)   106799 2023-05-16 11:51:34.000000 CQE-1.0.3/CQE/CQE.py
--rw-r--r--   0 satyaalmasian   (501) staff       (20)    17260 2023-05-16 11:51:34.000000 CQE-1.0.3/CQE/NumberNormalizer.py
--rw-r--r--   0 satyaalmasian   (501) staff       (20)        0 2023-05-10 11:20:18.000000 CQE-1.0.3/CQE/__init__.py
--rw-r--r--   0 satyaalmasian   (501) staff       (20)    12489 2023-05-15 13:17:03.000000 CQE-1.0.3/CQE/classes.py
--rw-r--r--   0 satyaalmasian   (501) staff       (20)     7901 2023-05-14 12:56:44.000000 CQE-1.0.3/CQE/number_lookup.py
--rw-r--r--   0 satyaalmasian   (501) staff       (20)    43173 2023-05-15 15:19:41.000000 CQE-1.0.3/CQE/rules.py
--rw-r--r--   0 satyaalmasian   (501) staff       (20)   148308 2023-05-10 11:20:18.000000 CQE-1.0.3/CQE/unit.json
-drwxr-xr-x   0 satyaalmasian   (501) staff       (20)        0 2023-05-16 12:08:17.318641 CQE-1.0.3/CQE/unit_classifier/
--rw-r--r--   0 satyaalmasian   (501) staff       (20)        0 2023-05-10 11:20:18.000000 CQE-1.0.3/CQE/unit_classifier/__init__.py
--rw-r--r--   0 satyaalmasian   (501) staff       (20)      559 2023-05-10 11:20:18.000000 CQE-1.0.3/CQE/unit_classifier/sample_usage.py
--rw-r--r--   0 satyaalmasian   (501) staff       (20)     7024 2023-05-11 07:08:00.000000 CQE-1.0.3/CQE/unit_classifier/train_classifier_bert.py
--rw-r--r--   0 satyaalmasian   (501) staff       (20)     1570 2023-05-11 11:07:05.000000 CQE-1.0.3/CQE/unit_classifier/unit_disambiguator.py
--rw-r--r--   0 satyaalmasian   (501) staff       (20)  1481390 2023-05-11 11:08:19.000000 CQE-1.0.3/CQE/unit_models.zip
-drwxr-xr-x   0 satyaalmasian   (501) staff       (20)        0 2023-05-16 12:08:17.317843 CQE-1.0.3/CQE.egg-info/
--rw-r--r--   0 satyaalmasian   (501) staff       (20)    10300 2023-05-16 12:08:17.000000 CQE-1.0.3/CQE.egg-info/PKG-INFO
--rw-r--r--   0 satyaalmasian   (501) staff       (20)      452 2023-05-16 12:08:17.000000 CQE-1.0.3/CQE.egg-info/SOURCES.txt
--rw-r--r--   0 satyaalmasian   (501) staff       (20)        1 2023-05-16 12:08:17.000000 CQE-1.0.3/CQE.egg-info/dependency_links.txt
--rw-r--r--   0 satyaalmasian   (501) staff       (20)       30 2023-05-16 12:08:17.000000 CQE-1.0.3/CQE.egg-info/requires.txt
--rw-r--r--   0 satyaalmasian   (501) staff       (20)        4 2023-05-16 12:08:17.000000 CQE-1.0.3/CQE.egg-info/top_level.txt
--rw-r--r--   0 satyaalmasian   (501) staff       (20)    34957 2023-05-12 10:54:06.000000 CQE-1.0.3/LICENSE.md
--rw-r--r--   0 satyaalmasian   (501) staff       (20)    10300 2023-05-16 12:08:17.319043 CQE-1.0.3/PKG-INFO
--rw-r--r--   0 satyaalmasian   (501) staff       (20)    10037 2023-05-16 11:51:34.000000 CQE-1.0.3/README.md
--rw-r--r--   0 satyaalmasian   (501) staff       (20)       38 2023-05-16 12:08:17.319362 CQE-1.0.3/setup.cfg
--rw-r--r--   0 satyaalmasian   (501) staff       (20)      670 2023-05-16 12:08:16.000000 CQE-1.0.3/setup.py
+drwxr-xr-x   0 satyaalmasian   (501) staff       (20)        0 2023-05-16 12:50:06.705724 CQE-1.0.4/
+drwxr-xr-x   0 satyaalmasian   (501) staff       (20)        0 2023-05-16 12:50:06.701716 CQE-1.0.4/CQE/
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)   106799 2023-05-16 11:51:34.000000 CQE-1.0.4/CQE/CQE.py
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)    17260 2023-05-16 11:51:34.000000 CQE-1.0.4/CQE/NumberNormalizer.py
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)        0 2023-05-10 11:20:18.000000 CQE-1.0.4/CQE/__init__.py
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)    12489 2023-05-15 13:17:03.000000 CQE-1.0.4/CQE/classes.py
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)     7901 2023-05-14 12:56:44.000000 CQE-1.0.4/CQE/number_lookup.py
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)    43173 2023-05-15 15:19:41.000000 CQE-1.0.4/CQE/rules.py
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)   148308 2023-05-10 11:20:18.000000 CQE-1.0.4/CQE/unit.json
+drwxr-xr-x   0 satyaalmasian   (501) staff       (20)        0 2023-05-16 12:50:06.705154 CQE-1.0.4/CQE/unit_classifier/
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)        0 2023-05-10 11:20:18.000000 CQE-1.0.4/CQE/unit_classifier/__init__.py
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)      559 2023-05-10 11:20:18.000000 CQE-1.0.4/CQE/unit_classifier/sample_usage.py
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)     7024 2023-05-11 07:08:00.000000 CQE-1.0.4/CQE/unit_classifier/train_classifier_bert.py
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)     1570 2023-05-11 11:07:05.000000 CQE-1.0.4/CQE/unit_classifier/unit_disambiguator.py
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)  1481390 2023-05-11 11:08:19.000000 CQE-1.0.4/CQE/unit_models.zip
+drwxr-xr-x   0 satyaalmasian   (501) staff       (20)        0 2023-05-16 12:50:06.704330 CQE-1.0.4/CQE.egg-info/
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)    10300 2023-05-16 12:50:06.000000 CQE-1.0.4/CQE.egg-info/PKG-INFO
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)      452 2023-05-16 12:50:06.000000 CQE-1.0.4/CQE.egg-info/SOURCES.txt
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)        1 2023-05-16 12:50:06.000000 CQE-1.0.4/CQE.egg-info/dependency_links.txt
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)      467 2023-05-16 12:50:06.000000 CQE-1.0.4/CQE.egg-info/requires.txt
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)        4 2023-05-16 12:50:06.000000 CQE-1.0.4/CQE.egg-info/top_level.txt
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)    34957 2023-05-12 10:54:06.000000 CQE-1.0.4/LICENSE.md
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)    10300 2023-05-16 12:50:06.705486 CQE-1.0.4/PKG-INFO
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)    10037 2023-05-16 11:51:34.000000 CQE-1.0.4/README.md
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)       38 2023-05-16 12:50:06.705766 CQE-1.0.4/setup.cfg
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)     1232 2023-05-16 12:46:46.000000 CQE-1.0.4/setup.py
```

### Comparing `CQE-1.0.3/CQE/CQE.py` & `CQE-1.0.4/CQE/CQE.py`

 * *Files identical despite different names*

### Comparing `CQE-1.0.3/CQE/NumberNormalizer.py` & `CQE-1.0.4/CQE/NumberNormalizer.py`

 * *Files identical despite different names*

### Comparing `CQE-1.0.3/CQE/classes.py` & `CQE-1.0.4/CQE/classes.py`

 * *Files identical despite different names*

### Comparing `CQE-1.0.3/CQE/number_lookup.py` & `CQE-1.0.4/CQE/number_lookup.py`

 * *Files identical despite different names*

### Comparing `CQE-1.0.3/CQE/rules.py` & `CQE-1.0.4/CQE/rules.py`

 * *Files identical despite different names*

### Comparing `CQE-1.0.3/CQE/unit.json` & `CQE-1.0.4/CQE/unit.json`

 * *Files identical despite different names*

### Comparing `CQE-1.0.3/CQE/unit_classifier/sample_usage.py` & `CQE-1.0.4/CQE/unit_classifier/sample_usage.py`

 * *Files identical despite different names*

### Comparing `CQE-1.0.3/CQE/unit_classifier/train_classifier_bert.py` & `CQE-1.0.4/CQE/unit_classifier/train_classifier_bert.py`

 * *Files identical despite different names*

### Comparing `CQE-1.0.3/CQE/unit_classifier/unit_disambiguator.py` & `CQE-1.0.4/CQE/unit_classifier/unit_disambiguator.py`

 * *Files identical despite different names*

### Comparing `CQE-1.0.3/CQE/unit_models.zip` & `CQE-1.0.4/CQE/unit_models.zip`

 * *Files identical despite different names*

### Comparing `CQE-1.0.3/CQE.egg-info/PKG-INFO` & `CQE-1.0.4/CQE.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CQE
-Version: 1.0.3
+Version: 1.0.4
 Summary: quantity extractor
 Home-page: https://github.com/vivkaz/CQE
 Author: satyaalmasian and vivian kazakova
 Author-email: satya.almasian@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `CQE-1.0.3/LICENSE.md` & `CQE-1.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `CQE-1.0.3/PKG-INFO` & `CQE-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CQE
-Version: 1.0.3
+Version: 1.0.4
 Summary: quantity extractor
 Home-page: https://github.com/vivkaz/CQE
 Author: satyaalmasian and vivian kazakova
 Author-email: satya.almasian@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `CQE-1.0.3/README.md` & `CQE-1.0.4/README.md`

 * *Files identical despite different names*

