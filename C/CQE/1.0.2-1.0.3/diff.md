# Comparing `tmp/CQE-1.0.2.tar.gz` & `tmp/CQE-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CQE-1.0.2.tar", last modified: Tue May 16 11:29:56 2023, max compression
+gzip compressed data, was "CQE-1.0.3.tar", last modified: Tue May 16 12:08:17 2023, max compression
```

## Comparing `CQE-1.0.2.tar` & `CQE-1.0.3.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxr-xr-x   0 satyaalmasian   (501) staff       (20)        0 2023-05-16 11:29:56.569381 CQE-1.0.2/
-drwxr-xr-x   0 satyaalmasian   (501) staff       (20)        0 2023-05-16 11:29:56.564696 CQE-1.0.2/CQE/
--rw-r--r--   0 satyaalmasian   (501) staff       (20)   106834 2023-05-15 13:17:03.000000 CQE-1.0.2/CQE/NumParser.py
--rw-r--r--   0 satyaalmasian   (501) staff       (20)    17278 2023-05-14 12:56:44.000000 CQE-1.0.2/CQE/NumberNormalizer.py
--rw-r--r--   0 satyaalmasian   (501) staff       (20)        0 2023-05-10 11:20:18.000000 CQE-1.0.2/CQE/__init__.py
--rw-r--r--   0 satyaalmasian   (501) staff       (20)    12489 2023-05-15 13:17:03.000000 CQE-1.0.2/CQE/classes.py
--rw-r--r--   0 satyaalmasian   (501) staff       (20)      992 2023-05-15 13:22:43.000000 CQE-1.0.2/CQE/example.py
--rw-r--r--   0 satyaalmasian   (501) staff       (20)     7901 2023-05-14 12:56:44.000000 CQE-1.0.2/CQE/number_lookup.py
--rw-r--r--   0 satyaalmasian   (501) staff       (20)    43173 2023-05-15 15:19:41.000000 CQE-1.0.2/CQE/rules.py
--rw-r--r--   0 satyaalmasian   (501) staff       (20)   148308 2023-05-10 11:20:18.000000 CQE-1.0.2/CQE/unit.json
-drwxr-xr-x   0 satyaalmasian   (501) staff       (20)        0 2023-05-16 11:29:56.568738 CQE-1.0.2/CQE/unit_classifier/
--rw-r--r--   0 satyaalmasian   (501) staff       (20)        0 2023-05-10 11:20:18.000000 CQE-1.0.2/CQE/unit_classifier/__init__.py
--rw-r--r--   0 satyaalmasian   (501) staff       (20)      559 2023-05-10 11:20:18.000000 CQE-1.0.2/CQE/unit_classifier/sample_usage.py
--rw-r--r--   0 satyaalmasian   (501) staff       (20)     7024 2023-05-11 07:08:00.000000 CQE-1.0.2/CQE/unit_classifier/train_classifier_bert.py
--rw-r--r--   0 satyaalmasian   (501) staff       (20)     1570 2023-05-11 11:07:05.000000 CQE-1.0.2/CQE/unit_classifier/unit_disambiguator.py
--rw-r--r--   0 satyaalmasian   (501) staff       (20)  1481390 2023-05-11 11:08:19.000000 CQE-1.0.2/CQE/unit_models.zip
-drwxr-xr-x   0 satyaalmasian   (501) staff       (20)        0 2023-05-16 11:29:56.567885 CQE-1.0.2/CQE.egg-info/
--rw-r--r--   0 satyaalmasian   (501) staff       (20)    10352 2023-05-16 11:29:56.000000 CQE-1.0.2/CQE.egg-info/PKG-INFO
--rw-r--r--   0 satyaalmasian   (501) staff       (20)      473 2023-05-16 11:29:56.000000 CQE-1.0.2/CQE.egg-info/SOURCES.txt
--rw-r--r--   0 satyaalmasian   (501) staff       (20)        1 2023-05-16 11:29:56.000000 CQE-1.0.2/CQE.egg-info/dependency_links.txt
--rw-r--r--   0 satyaalmasian   (501) staff       (20)       30 2023-05-16 11:29:56.000000 CQE-1.0.2/CQE.egg-info/requires.txt
--rw-r--r--   0 satyaalmasian   (501) staff       (20)        4 2023-05-16 11:29:56.000000 CQE-1.0.2/CQE.egg-info/top_level.txt
--rw-r--r--   0 satyaalmasian   (501) staff       (20)    34957 2023-05-12 10:54:06.000000 CQE-1.0.2/LICENSE.md
--rw-r--r--   0 satyaalmasian   (501) staff       (20)    10352 2023-05-16 11:29:56.569104 CQE-1.0.2/PKG-INFO
--rw-r--r--   0 satyaalmasian   (501) staff       (20)    10089 2023-05-16 11:17:07.000000 CQE-1.0.2/README.md
--rw-r--r--   0 satyaalmasian   (501) staff       (20)       38 2023-05-16 11:29:56.569440 CQE-1.0.2/setup.cfg
--rw-r--r--   0 satyaalmasian   (501) staff       (20)      670 2023-05-16 11:29:19.000000 CQE-1.0.2/setup.py
+drwxr-xr-x   0 satyaalmasian   (501) staff       (20)        0 2023-05-16 12:08:17.319309 CQE-1.0.3/
+drwxr-xr-x   0 satyaalmasian   (501) staff       (20)        0 2023-05-16 12:08:17.314786 CQE-1.0.3/CQE/
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)   106799 2023-05-16 11:51:34.000000 CQE-1.0.3/CQE/CQE.py
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)    17260 2023-05-16 11:51:34.000000 CQE-1.0.3/CQE/NumberNormalizer.py
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)        0 2023-05-10 11:20:18.000000 CQE-1.0.3/CQE/__init__.py
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)    12489 2023-05-15 13:17:03.000000 CQE-1.0.3/CQE/classes.py
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)     7901 2023-05-14 12:56:44.000000 CQE-1.0.3/CQE/number_lookup.py
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)    43173 2023-05-15 15:19:41.000000 CQE-1.0.3/CQE/rules.py
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)   148308 2023-05-10 11:20:18.000000 CQE-1.0.3/CQE/unit.json
+drwxr-xr-x   0 satyaalmasian   (501) staff       (20)        0 2023-05-16 12:08:17.318641 CQE-1.0.3/CQE/unit_classifier/
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)        0 2023-05-10 11:20:18.000000 CQE-1.0.3/CQE/unit_classifier/__init__.py
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)      559 2023-05-10 11:20:18.000000 CQE-1.0.3/CQE/unit_classifier/sample_usage.py
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)     7024 2023-05-11 07:08:00.000000 CQE-1.0.3/CQE/unit_classifier/train_classifier_bert.py
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)     1570 2023-05-11 11:07:05.000000 CQE-1.0.3/CQE/unit_classifier/unit_disambiguator.py
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)  1481390 2023-05-11 11:08:19.000000 CQE-1.0.3/CQE/unit_models.zip
+drwxr-xr-x   0 satyaalmasian   (501) staff       (20)        0 2023-05-16 12:08:17.317843 CQE-1.0.3/CQE.egg-info/
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)    10300 2023-05-16 12:08:17.000000 CQE-1.0.3/CQE.egg-info/PKG-INFO
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)      452 2023-05-16 12:08:17.000000 CQE-1.0.3/CQE.egg-info/SOURCES.txt
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)        1 2023-05-16 12:08:17.000000 CQE-1.0.3/CQE.egg-info/dependency_links.txt
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)       30 2023-05-16 12:08:17.000000 CQE-1.0.3/CQE.egg-info/requires.txt
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)        4 2023-05-16 12:08:17.000000 CQE-1.0.3/CQE.egg-info/top_level.txt
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)    34957 2023-05-12 10:54:06.000000 CQE-1.0.3/LICENSE.md
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)    10300 2023-05-16 12:08:17.319043 CQE-1.0.3/PKG-INFO
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)    10037 2023-05-16 11:51:34.000000 CQE-1.0.3/README.md
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)       38 2023-05-16 12:08:17.319362 CQE-1.0.3/setup.cfg
+-rw-r--r--   0 satyaalmasian   (501) staff       (20)      670 2023-05-16 12:08:16.000000 CQE-1.0.3/setup.py
```

### Comparing `CQE-1.0.2/CQE/NumParser.py` & `CQE-1.0.3/CQE/CQE.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 from spacy.lang.lex_attrs import like_num as sp_like_num
 from spacy.lang.char_classes import ALPHA, ALPHA_LOWER, ALPHA_UPPER, HYPHENS
 from spacy.lang.char_classes import CONCAT_QUOTES, LIST_ELLIPSES, LIST_ICONS
 from spacy.util import compile_infix_regex
 
 from fuzzywuzzy import fuzz
 
-from numparser import NumberNormalizer
-from numparser.rules import rules
-from numparser.number_lookup import maps, suffixes
-from numparser.classes import Change, Value, Range, Unit, Quantity
+from . import NumberNormalizer
+from .rules import rules
+from .number_lookup import maps, suffixes
+from .classes import Change, Value, Range, Unit, Quantity
 from pathlib import Path
 
 def get_project_root() -> Path:
     return Path(__file__).parent
 
 # Add a debug option to the numparser, so that we can disable the warnings
 parser = argparse.ArgumentParser()
```

### Comparing `CQE-1.0.2/CQE/NumberNormalizer.py` & `CQE-1.0.3/CQE/NumberNormalizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 import json
 import os
 from ordered_set import OrderedSet
 
 from spacy.lang.lex_attrs import is_digit, like_num
 from spacy.tokens import Token
 
-from numparser.number_lookup import maps, prefixes
-from numparser.unit_classifier.unit_disambiguator import unit_disambiguator
+from .number_lookup import maps, prefixes
+from .unit_classifier.unit_disambiguator import unit_disambiguator
 
 locale.setlocale(locale.LC_ALL, 'en_US.UTF-8')
 
 from pathlib import Path
 def get_project_root() -> Path:
     return Path(__file__).parent
```

### Comparing `CQE-1.0.2/CQE/classes.py` & `CQE-1.0.3/CQE/classes.py`

 * *Files identical despite different names*

### Comparing `CQE-1.0.2/CQE/number_lookup.py` & `CQE-1.0.3/CQE/number_lookup.py`

 * *Files identical despite different names*

### Comparing `CQE-1.0.2/CQE/rules.py` & `CQE-1.0.3/CQE/rules.py`

 * *Files identical despite different names*

### Comparing `CQE-1.0.2/CQE/unit.json` & `CQE-1.0.3/CQE/unit.json`

 * *Files identical despite different names*

### Comparing `CQE-1.0.2/CQE/unit_classifier/sample_usage.py` & `CQE-1.0.3/CQE/unit_classifier/sample_usage.py`

 * *Files identical despite different names*

### Comparing `CQE-1.0.2/CQE/unit_classifier/train_classifier_bert.py` & `CQE-1.0.3/CQE/unit_classifier/train_classifier_bert.py`

 * *Files identical despite different names*

### Comparing `CQE-1.0.2/CQE/unit_classifier/unit_disambiguator.py` & `CQE-1.0.3/CQE/unit_classifier/unit_disambiguator.py`

 * *Files identical despite different names*

### Comparing `CQE-1.0.2/CQE/unit_models.zip` & `CQE-1.0.3/CQE/unit_models.zip`

 * *Files identical despite different names*

### Comparing `CQE-1.0.2/CQE.egg-info/PKG-INFO` & `CQE-1.0.3/CQE.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CQE
-Version: 1.0.2
+Version: 1.0.3
 Summary: quantity extractor
 Home-page: https://github.com/vivkaz/CQE
 Author: satyaalmasian and vivian kazakova
 Author-email: satya.almasian@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
@@ -32,34 +32,29 @@
 }
 ```
 ### Prerequisites
 you can also install the package using on the root directory of the package.
 ```
 pip install .
 ```
-or simply via pip:
-```
-pip install CQE
-```
-
 ### Usage
 Create a `NumParser` and parse some text or sentence.
 ```python
-from CQE.NumParser import NumParser
+from CQE import CQE
 
-parser = NumParser()
+parser = CQE.NumParser()
 text = "The sp 500 was down 2.1% and nasdaq fell 2.5%."
 result = parser.parse(text)
 print(result)
 
 >>> [(=,2.1,[%],percentage,[sp, 500]), (=,2.5,[%],percentage,[nasdaq])]
 ```
 Use the overload option for additional functionality. The NumParser will compute the span indices of the Quantity, the normalized input sentence, the long and the simplified scientific notation of the Value, whether the unit is scientific or noun based and the unit surface forms.
 ```python
-parser = NumParser(overload=True)
+parser = CQE.NumParser(overload=True)
 text = "The sp 500 was down 2.1% and nasdaq fell 2.5%."
 result = parser.parse(text)
 
 for res in result:
     print(f"""
 	Quantity: {res}
 	=====
```

### Comparing `CQE-1.0.2/LICENSE.md` & `CQE-1.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `CQE-1.0.2/PKG-INFO` & `CQE-1.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CQE
-Version: 1.0.2
+Version: 1.0.3
 Summary: quantity extractor
 Home-page: https://github.com/vivkaz/CQE
 Author: satyaalmasian and vivian kazakova
 Author-email: satya.almasian@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
@@ -32,34 +32,29 @@
 }
 ```
 ### Prerequisites
 you can also install the package using on the root directory of the package.
 ```
 pip install .
 ```
-or simply via pip:
-```
-pip install CQE
-```
-
 ### Usage
 Create a `NumParser` and parse some text or sentence.
 ```python
-from CQE.NumParser import NumParser
+from CQE import CQE
 
-parser = NumParser()
+parser = CQE.NumParser()
 text = "The sp 500 was down 2.1% and nasdaq fell 2.5%."
 result = parser.parse(text)
 print(result)
 
 >>> [(=,2.1,[%],percentage,[sp, 500]), (=,2.5,[%],percentage,[nasdaq])]
 ```
 Use the overload option for additional functionality. The NumParser will compute the span indices of the Quantity, the normalized input sentence, the long and the simplified scientific notation of the Value, whether the unit is scientific or noun based and the unit surface forms.
 ```python
-parser = NumParser(overload=True)
+parser = CQE.NumParser(overload=True)
 text = "The sp 500 was down 2.1% and nasdaq fell 2.5%."
 result = parser.parse(text)
 
 for res in result:
     print(f"""
 	Quantity: {res}
 	=====
```

### Comparing `CQE-1.0.2/README.md` & `CQE-1.0.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -22,34 +22,29 @@
 }
 ```
 ### Prerequisites
 you can also install the package using on the root directory of the package.
 ```
 pip install .
 ```
-or simply via pip:
-```
-pip install CQE
-```
-
 ### Usage
 Create a `NumParser` and parse some text or sentence.
 ```python
-from CQE.NumParser import NumParser
+from CQE import CQE
 
-parser = NumParser()
+parser = CQE.NumParser()
 text = "The sp 500 was down 2.1% and nasdaq fell 2.5%."
 result = parser.parse(text)
 print(result)
 
 >>> [(=,2.1,[%],percentage,[sp, 500]), (=,2.5,[%],percentage,[nasdaq])]
 ```
 Use the overload option for additional functionality. The NumParser will compute the span indices of the Quantity, the normalized input sentence, the long and the simplified scientific notation of the Value, whether the unit is scientific or noun based and the unit surface forms.
 ```python
-parser = NumParser(overload=True)
+parser = CQE.NumParser(overload=True)
 text = "The sp 500 was down 2.1% and nasdaq fell 2.5%."
 result = parser.parse(text)
 
 for res in result:
     print(f"""
 	Quantity: {res}
 	=====
```

### Comparing `CQE-1.0.2/setup.py` & `CQE-1.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='CQE',
-    version='1.0.2',
+    version='1.0.3',
     packages=['CQE','CQE.unit_classifier'],
     package_data={'': ['unit.json'],'': ['unit_models.zip']},# both has to be empty
     url='https://github.com/vivkaz/CQE',
     license='',
     long_description_content_type="text/markdown",
     long_description=long_description,
     author='satyaalmasian and vivian kazakova',
```

