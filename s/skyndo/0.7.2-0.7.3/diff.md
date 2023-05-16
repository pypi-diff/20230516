# Comparing `tmp/skyndo-0.7.2.tar.gz` & `tmp/skyndo-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skyndo-0.7.2.tar", last modified: Tue May 16 03:07:23 2023, max compression
+gzip compressed data, was "skyndo-0.7.3.tar", last modified: Tue May 16 04:34:40 2023, max compression
```

## Comparing `skyndo-0.7.2.tar` & `skyndo-0.7.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 03:07:23.550303 skyndo-0.7.2/
--rw-rw-rw-   0        0        0      378 2023-05-16 03:07:23.550303 skyndo-0.7.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-16 03:07:23.551301 skyndo-0.7.2/setup.cfg
--rw-rw-rw-   0        0        0      508 2023-05-16 03:06:55.000000 skyndo-0.7.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-16 03:07:23.425638 skyndo-0.7.2/skyndo/
--rw-rw-rw-   0        0        0        0 2023-03-31 15:55:53.000000 skyndo-0.7.2/skyndo/_init_.py
--rw-rw-rw-   0        0        0     2250 2023-05-16 03:05:31.000000 skyndo-0.7.2/skyndo/predict.py
-drwxrwxrwx   0        0        0        0 2023-05-16 03:07:23.548310 skyndo-0.7.2/skyndo.egg-info/
--rw-rw-rw-   0        0        0      378 2023-05-16 03:07:22.000000 skyndo-0.7.2/skyndo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2023-05-16 03:07:23.000000 skyndo-0.7.2/skyndo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 03:07:22.000000 skyndo-0.7.2/skyndo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-05-16 03:07:22.000000 skyndo-0.7.2/skyndo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-16 03:07:22.000000 skyndo-0.7.2/skyndo.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 04:34:40.403088 skyndo-0.7.3/
+-rw-rw-rw-   0        0        0      378 2023-05-16 04:34:40.400095 skyndo-0.7.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-16 04:34:40.403751 skyndo-0.7.3/setup.cfg
+-rw-rw-rw-   0        0        0      508 2023-05-16 04:34:27.000000 skyndo-0.7.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 04:34:40.331278 skyndo-0.7.3/skyndo/
+-rw-rw-rw-   0        0        0        0 2023-03-31 15:55:53.000000 skyndo-0.7.3/skyndo/_init_.py
+-rw-rw-rw-   0        0        0     2175 2023-05-16 04:33:41.000000 skyndo-0.7.3/skyndo/predict.py
+drwxrwxrwx   0        0        0        0 2023-05-16 04:34:40.399100 skyndo-0.7.3/skyndo.egg-info/
+-rw-rw-rw-   0        0        0      378 2023-05-16 04:34:40.000000 skyndo-0.7.3/skyndo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2023-05-16 04:34:40.000000 skyndo-0.7.3/skyndo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 04:34:40.000000 skyndo-0.7.3/skyndo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-05-16 04:34:40.000000 skyndo-0.7.3/skyndo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-16 04:34:40.000000 skyndo-0.7.3/skyndo.egg-info/top_level.txt
```

### Comparing `skyndo-0.7.2/skyndo/predict.py` & `skyndo-0.7.3/skyndo/predict.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import pandas as pd
 import seaborn as sns
 import matplotlib.pyplot as plt
 
 
 def predictor(alpha, delta, u, g, i, r, z, redshift): # To predict the class of the astronomical objet for given features.
     # Load the trained model
-    with open('https://github.com/NishanD21/Astronomical-Objects-Classification/blob/main/model.pkl', 'rb') as f:
+    with open('model.pkl', 'rb') as f:
         model = pickle.load(f)
     
     # Make the prediction
     x = np.array([[alpha, delta, u, g, i, r, z, redshift]])
     prediction = model.predict(x)[0]
     
     # Map the predicted value to the desired class
```

