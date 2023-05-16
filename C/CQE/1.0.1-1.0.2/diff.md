# Comparing `tmp/CQE-1.0.1.tar.gz` & `tmp/CQE-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CQE-1.0.1.tar", last modified: Tue May 16 11:15:22 2023, max compression
+gzip compressed data, was "CQE-1.0.2.tar", last modified: Tue May 16 11:29:56 2023, max compression
```

## Comparing `CQE-1.0.1.tar` & `CQE-1.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 satyaalmasian   (501) staff       (20)        0 2023-05-16 11:15:22.101512 CQE-1.0.1/
-drwxr-xr-x   0 satyaalmasian   (501) staff       (20)        0 2023-05-16 11:15:22.096695 CQE-1.0.1/CQE/
--rw-r--r--   0 satyaalmasian   (501) staff       (20)   106834 2023-05-15 13:17:03.000000 CQE-1.0.1/CQE/NumParser.py
--rw-r--r--   0 satyaalmasian   (501) staff       (20)    17278 2023-05-14 12:56:44.000000 CQE-1.0.1/CQE/NumberNormalizer.py
--rw-r--r--   0 satyaalmasian   (501) staff       (20)        0 2023-05-10 11:20:18.000000 CQE-1.0.1/CQE/__init__.py
--rw-r--r--   0 satyaalmasian   (501) staff       (20)    12489 2023-05-15 13:17:03.000000 CQE-1.0.1/CQE/classes.py
--rw-r--r--   0 satyaalmasian   (501) staff       (20)      992 2023-05-15 13:22:43.000000 CQE-1.0.1/CQE/example.py
--rw-r--r--   0 satyaalmasian   (501) staff       (20)     7901 2023-05-14 12:56:44.000000 CQE-1.0.1/CQE/number_lookup.py
--rw-r--r--   0 satyaalmasian   (501) staff       (20)    43173 2023-05-15 15:19:41.000000 CQE-1.0.1/CQE/rules.py
--rw-r--r--   0 satyaalmasian   (501) staff       (20)   148308 2023-05-10 11:20:18.000000 CQE-1.0.1/CQE/unit.json
-drwxr-xr-x   0 satyaalmasian   (501) staff       (20)        0 2023-05-16 11:15:22.100711 CQE-1.0.1/CQE/unit_classifier/
--rw-r--r--   0 satyaalmasian   (501) staff       (20)        0 2023-05-10 11:20:18.000000 CQE-1.0.1/CQE/unit_classifier/__init__.py
--rw-r--r--   0 satyaalmasian   (501) staff       (20)      559 2023-05-10 11:20:18.000000 CQE-1.0.1/CQE/unit_classifier/sample_usage.py
--rw-r--r--   0 satyaalmasian   (501) staff       (20)     7024 2023-05-11 07:08:00.000000 CQE-1.0.1/CQE/unit_classifier/train_classifier_bert.py
--rw-r--r--   0 satyaalmasian   (501) staff       (20)     1570 2023-05-11 11:07:05.000000 CQE-1.0.1/CQE/unit_classifier/unit_disambiguator.py
--rw-r--r--   0 satyaalmasian   (501) staff       (20)  1481390 2023-05-11 11:08:19.000000 CQE-1.0.1/CQE/unit_models.zip
-drwxr-xr-x   0 satyaalmasian   (501) staff       (20)        0 2023-05-16 11:15:22.099712 CQE-1.0.1/CQE.egg-info/
--rw-r--r--   0 satyaalmasian   (501) staff       (20)      193 2023-05-16 11:15:22.000000 CQE-1.0.1/CQE.egg-info/PKG-INFO
--rw-r--r--   0 satyaalmasian   (501) staff       (20)      473 2023-05-16 11:15:22.000000 CQE-1.0.1/CQE.egg-info/SOURCES.txt
--rw-r--r--   0 satyaalmasian   (501) staff       (20)        1 2023-05-16 11:15:22.000000 CQE-1.0.1/CQE.egg-info/dependency_links.txt
--rw-r--r--   0 satyaalmasian   (501) staff       (20)       30 2023-05-16 11:15:22.000000 CQE-1.0.1/CQE.egg-info/requires.txt
--rw-r--r--   0 satyaalmasian   (501) staff       (20)        4 2023-05-16 11:15:22.000000 CQE-1.0.1/CQE.egg-info/top_level.txt
--rw-r--r--   0 satyaalmasian   (501) staff       (20)    34957 2023-05-12 10:54:06.000000 CQE-1.0.1/LICENSE.md
--rw-r--r--   0 satyaalmasian   (501) staff       (20)      193 2023-05-16 11:15:22.101168 CQE-1.0.1/PKG-INFO
--rw-r--r--   0 satyaalmasian   (501) staff       (20)    10043 2023-05-16 11:08:15.000000 CQE-1.0.1/README.md
--rw-r--r--   0 satyaalmasian   (501) staff       (20)       38 2023-05-16 11:15:22.101561 CQE-1.0.1/setup.cfg
--rw-r--r--   0 satyaalmasian   (501) staff       (20)      425 2023-05-11 09:47:02.000000 CQE-1.0.1/setup.py
+drwxr-xr-x   0 satyaalmasian   (501) staff       (20)        0 2023-05-16 11:29:56.569381 CQE-1.0.2/
+drwxr-xr-x   0 satyaalmasian   (501) staff       (20)        0 2023-05-16 11:29:56.564696 CQE-1.0.2/CQE/
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)   106834 2023-05-15 13:17:03.000000 CQE-1.0.2/CQE/NumParser.py
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)    17278 2023-05-14 12:56:44.000000 CQE-1.0.2/CQE/NumberNormalizer.py
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)        0 2023-05-10 11:20:18.000000 CQE-1.0.2/CQE/__init__.py
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)    12489 2023-05-15 13:17:03.000000 CQE-1.0.2/CQE/classes.py
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)      992 2023-05-15 13:22:43.000000 CQE-1.0.2/CQE/example.py
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)     7901 2023-05-14 12:56:44.000000 CQE-1.0.2/CQE/number_lookup.py
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)    43173 2023-05-15 15:19:41.000000 CQE-1.0.2/CQE/rules.py
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)   148308 2023-05-10 11:20:18.000000 CQE-1.0.2/CQE/unit.json
+drwxr-xr-x   0 satyaalmasian   (501) staff       (20)        0 2023-05-16 11:29:56.568738 CQE-1.0.2/CQE/unit_classifier/
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)        0 2023-05-10 11:20:18.000000 CQE-1.0.2/CQE/unit_classifier/__init__.py
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)      559 2023-05-10 11:20:18.000000 CQE-1.0.2/CQE/unit_classifier/sample_usage.py
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)     7024 2023-05-11 07:08:00.000000 CQE-1.0.2/CQE/unit_classifier/train_classifier_bert.py
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)     1570 2023-05-11 11:07:05.000000 CQE-1.0.2/CQE/unit_classifier/unit_disambiguator.py
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)  1481390 2023-05-11 11:08:19.000000 CQE-1.0.2/CQE/unit_models.zip
+drwxr-xr-x   0 satyaalmasian   (501) staff       (20)        0 2023-05-16 11:29:56.567885 CQE-1.0.2/CQE.egg-info/
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)    10352 2023-05-16 11:29:56.000000 CQE-1.0.2/CQE.egg-info/PKG-INFO
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)      473 2023-05-16 11:29:56.000000 CQE-1.0.2/CQE.egg-info/SOURCES.txt
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)        1 2023-05-16 11:29:56.000000 CQE-1.0.2/CQE.egg-info/dependency_links.txt
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)       30 2023-05-16 11:29:56.000000 CQE-1.0.2/CQE.egg-info/requires.txt
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)        4 2023-05-16 11:29:56.000000 CQE-1.0.2/CQE.egg-info/top_level.txt
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)    34957 2023-05-12 10:54:06.000000 CQE-1.0.2/LICENSE.md
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)    10352 2023-05-16 11:29:56.569104 CQE-1.0.2/PKG-INFO
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)    10089 2023-05-16 11:17:07.000000 CQE-1.0.2/README.md
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)       38 2023-05-16 11:29:56.569440 CQE-1.0.2/setup.cfg
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)      670 2023-05-16 11:29:19.000000 CQE-1.0.2/setup.py
```

### Comparing `CQE-1.0.1/CQE/NumParser.py` & `CQE-1.0.2/CQE/NumParser.py`

 * *Files identical despite different names*

### Comparing `CQE-1.0.1/CQE/NumberNormalizer.py` & `CQE-1.0.2/CQE/NumberNormalizer.py`

 * *Files identical despite different names*

### Comparing `CQE-1.0.1/CQE/classes.py` & `CQE-1.0.2/CQE/classes.py`

 * *Files identical despite different names*

### Comparing `CQE-1.0.1/CQE/example.py` & `CQE-1.0.2/CQE/example.py`

 * *Files identical despite different names*

### Comparing `CQE-1.0.1/CQE/number_lookup.py` & `CQE-1.0.2/CQE/number_lookup.py`

 * *Files identical despite different names*

### Comparing `CQE-1.0.1/CQE/rules.py` & `CQE-1.0.2/CQE/rules.py`

 * *Files identical despite different names*

### Comparing `CQE-1.0.1/CQE/unit.json` & `CQE-1.0.2/CQE/unit.json`

 * *Files identical despite different names*

### Comparing `CQE-1.0.1/CQE/unit_classifier/sample_usage.py` & `CQE-1.0.2/CQE/unit_classifier/sample_usage.py`

 * *Files identical despite different names*

### Comparing `CQE-1.0.1/CQE/unit_classifier/train_classifier_bert.py` & `CQE-1.0.2/CQE/unit_classifier/train_classifier_bert.py`

 * *Files identical despite different names*

### Comparing `CQE-1.0.1/CQE/unit_classifier/unit_disambiguator.py` & `CQE-1.0.2/CQE/unit_classifier/unit_disambiguator.py`

 * *Files identical despite different names*

### Comparing `CQE-1.0.1/CQE/unit_models.zip` & `CQE-1.0.2/CQE/unit_models.zip`

 * *Files identical despite different names*

### Comparing `CQE-1.0.1/LICENSE.md` & `CQE-1.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `CQE-1.0.1/README.md` & `CQE-1.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # CQE
-##Evaultion and data in [CQE_Evaluation](https://github.com/satya77/CQE_Evaluation).
+## Evaultion and data in [CQE_Evaluation](https://github.com/satya77/CQE_Evaluation).
 
 A Framework for Comprehensive Quantity Extraction. This repository contains code for the paper:
 
 [CQE: A Framework for Comprehensive Quantity Extraction
 ](https://arxiv.org/pdf/2305.08853v1.pdf)
 
 Satya Almasian*, Vivian Kazakova*, Philipp Göldner, Michael Gertz  
@@ -22,14 +22,19 @@
 }
 ```
 ### Prerequisites
 you can also install the package using on the root directory of the package.
 ```
 pip install .
 ```
+or simply via pip:
+```
+pip install CQE
+```
+
 ### Usage
 Create a `NumParser` and parse some text or sentence.
 ```python
 from CQE.NumParser import NumParser
 
 parser = NumParser()
 text = "The sp 500 was down 2.1% and nasdaq fell 2.5%."
@@ -171,8 +176,8 @@
 LONELY_NUM [2.24]
 
 Candidates: [[US$, 58.24, per, barrel, 10], [US$, 2.24, per, mmBTU, 25], [19, cents, 6], [10.4, cents, 21]]
 Quadruples: [([], [58.24], [US$, per, barrel], 10), ([], [2.24], [US$, per, mmBTU], 25), ([], [19], [cents], 6), ([], [10.4], [cents], 21)]
 
 Output: [(=,58.24,[US$, per, barrel],united states dollar / barrel,[September, crude, contract]), (=,2.24,[US$, per, mmBTU],united states dollar / mmBTU,[September, natural, gas, contract]), (=,19.0,[cents],cent,[September, crude, contract]), (=,10.4,[cents],cent,[September, natural, gas, contract])]
 ```
-_Note that the numbers 6, 10, 21 and 25 indicate the position of the quantity in the text._
+_Note that the numbers 6, 10, 21 and 25 indicate the position of the quantity in the text._
```

