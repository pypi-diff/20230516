# Comparing `tmp/tetun_lid-1.0.1.tar.gz` & `tmp/tetun_lid-1.0.2.tar.gz`

## Comparing `tetun_lid-1.0.1.tar` & `tetun_lid-1.0.2.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tetun_lid-1.0.1/.DS_Store
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 tetun_lid-1.0.1/Pipfile
--rw-r--r--   0        0        0     8238 2020-02-02 00:00:00.000000 tetun_lid-1.0.1/Pipfile.lock
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tetun_lid-1.0.1/tetunlid/__init__.py
--rw-r--r--   0        0        0     2846 2020-02-02 00:00:00.000000 tetun_lid-1.0.1/tetunlid/lid.py
--rw-r--r--   0        0        0 20889678 2020-02-02 00:00:00.000000 tetun_lid-1.0.1/tetunlid/model/tetun_lid_model.pkl
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 tetun_lid-1.0.1/LICENSE
--rw-r--r--   0        0        0     6123 2020-02-02 00:00:00.000000 tetun_lid-1.0.1/README.md
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 tetun_lid-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     6515 2020-02-02 00:00:00.000000 tetun_lid-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tetun_lid-1.0.2/.DS_Store
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 tetun_lid-1.0.2/Pipfile
+-rw-r--r--   0        0        0     8238 2020-02-02 00:00:00.000000 tetun_lid-1.0.2/Pipfile.lock
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 tetun_lid-1.0.2/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tetun_lid-1.0.2/tetunlid/__init__.py
+-rw-r--r--   0        0        0     2803 2020-02-02 00:00:00.000000 tetun_lid-1.0.2/tetunlid/lid.py
+-rw-r--r--   0        0        0 16769278 2020-02-02 00:00:00.000000 tetun_lid-1.0.2/tetunlid/model/tetun_lid_model.pkl
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 tetun_lid-1.0.2/LICENSE
+-rw-r--r--   0        0        0     6089 2020-02-02 00:00:00.000000 tetun_lid-1.0.2/README.md
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 tetun_lid-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     6481 2020-02-02 00:00:00.000000 tetun_lid-1.0.2/PKG-INFO
```

### Comparing `tetun_lid-1.0.1/Pipfile.lock` & `tetun_lid-1.0.2/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `tetun_lid-1.0.1/tetunlid/lid.py` & `tetun_lid-1.0.2/tetunlid/lid.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,14 @@
     * Tetun
     * Portuguese
     * English
     * Indonesian
 """
 import joblib
 from pathlib import Path
-from unidecode import unidecode
 from typing import List
 
 
 def load_model() -> object:
     """ Load Tetun language identification model """
     module_path = Path(__file__).parent
     model_path = module_path/'model'/'tetun_lid_model.pkl'
@@ -33,15 +32,15 @@
     :param input: a string.
     :return: a language name.
     """
     if not type(input) is str:
         return "Your input is not a string."
 
     model = load_model()
-    pred_probs = model.predict_proba([unidecode(input)])
+    pred_probs = model.predict_proba([input])
 
     for probs in pred_probs:
         max_lang = model.classes_[probs.argmax()]
         if max_lang == 'tet':
             prediction = "Tetun"
         if max_lang == 'pt':
             prediction = "Portuguese"
```

### Comparing `tetun_lid-1.0.1/LICENSE` & `tetun_lid-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tetun_lid-1.0.1/README.md` & `tetun_lid-1.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -14,22 +14,20 @@
 
 ### Dependecies
 
 Tetun LID depends on the following packages:
 
 * joblib
 * scikit-learn
-* Unidecode
 
 To install the dependencies packages, run these commands in your console:
 
 ```
 pip install joblib
 pip install scikit-learn
-pip install Unidecode
 ```
 
 ### Usage
 
 To use Tetun LID, from the `tetunlid` package, import the `lid` module, and then call a function.
 
 1. In case you want to `predict the language` of an input text, use the `predict_language()` function.
```

### Comparing `tetun_lid-1.0.1/PKG-INFO` & `tetun_lid-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tetun_lid
-Version: 1.0.1
+Version: 1.0.2
 Summary: Tetun Language Identification Model
 Author-email: Gabriel de Jesus <gabriel.dejesus@timornews.tl>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -26,22 +26,20 @@
 
 ### Dependecies
 
 Tetun LID depends on the following packages:
 
 * joblib
 * scikit-learn
-* Unidecode
 
 To install the dependencies packages, run these commands in your console:
 
 ```
 pip install joblib
 pip install scikit-learn
-pip install Unidecode
 ```
 
 ### Usage
 
 To use Tetun LID, from the `tetunlid` package, import the `lid` module, and then call a function.
 
 1. In case you want to `predict the language` of an input text, use the `predict_language()` function.
```

