# Comparing `tmp/smplotlib-0.0.6.tar.gz` & `tmp/smplotlib-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/jiaxuanli/Dropbox (Princeton)/Research/Packages/smplotlib/dist/.tmp-j3lyd1s5/smplotlib-0.0.6.tar", last modified: Tue Apr 18 01:19:12 2023, max compression
+gzip compressed data, was "/Users/jiaxuanli/Dropbox (Princeton)/Research/Packages/smplotlib/dist/.tmp-3a10clzx/smplotlib-0.0.7.tar", last modified: Tue May 16 20:53:47 2023, max compression
```

## Comparing `smplotlib-0.0.6.tar` & `smplotlib-0.0.7.tar`

### file list

```diff
@@ -1,39 +1,38 @@
-drwxr-xr-x   0 jiaxuanli   (501) staff       (20)        0 2023-04-18 01:19:12.000000 smplotlib-0.0.6/
--rw-r--r--   0 jiaxuanli   (501) staff       (20)     1067 2023-04-14 01:14:04.000000 smplotlib-0.0.6/LICENSE
--rw-r--r--   0 jiaxuanli   (501) staff       (20)       70 2023-04-14 03:22:16.000000 smplotlib-0.0.6/MANIFEST.in
--rw-r--r--   0 jiaxuanli   (501) staff       (20)     2057 2023-04-18 01:19:12.000000 smplotlib-0.0.6/PKG-INFO
--rw-r--r--   0 jiaxuanli   (501) staff       (20)     1531 2023-04-14 03:48:18.000000 smplotlib-0.0.6/README.md
--rw-r--r--   0 jiaxuanli   (501) staff       (20)      652 2023-04-18 01:18:55.000000 smplotlib-0.0.6/pyproject.toml
--rw-r--r--   0 jiaxuanli   (501) staff       (20)       38 2023-04-18 01:19:12.000000 smplotlib-0.0.6/setup.cfg
-drwxr-xr-x   0 jiaxuanli   (501) staff       (20)        0 2023-04-18 01:19:12.000000 smplotlib-0.0.6/src/
-drwxr-xr-x   0 jiaxuanli   (501) staff       (20)        0 2023-04-18 01:19:12.000000 smplotlib-0.0.6/src/smplotlib/
--rw-r--r--   0 jiaxuanli   (501) staff       (20)     3225 2023-04-15 23:05:56.000000 smplotlib-0.0.6/src/smplotlib/__init__.py
--rw-r--r--   0 jiaxuanli   (501) staff       (20)     2275 2023-04-14 03:14:00.000000 smplotlib-0.0.6/src/smplotlib/demo.py
--rw-r--r--   0 jiaxuanli   (501) staff       (20)    40688 2023-04-15 23:05:11.000000 smplotlib-0.0.6/src/smplotlib/smplot.mplstyle
-drwxr-xr-x   0 jiaxuanli   (501) staff       (20)        0 2023-04-18 01:19:12.000000 smplotlib-0.0.6/src/smplotlib/test_data/
--rw-r--r--   0 jiaxuanli   (501) staff       (20)    16128 2023-04-14 03:09:55.000000 smplotlib-0.0.6/src/smplotlib/test_data/test_array.npy
-drwxr-xr-x   0 jiaxuanli   (501) staff       (20)        0 2023-04-18 01:19:12.000000 smplotlib-0.0.6/src/smplotlib/ttf/
--rw-r--r--   0 jiaxuanli   (501) staff       (20)    70276 2023-04-14 03:09:55.000000 smplotlib-0.0.6/src/smplotlib/ttf/AVHersheyComplexHeavy.ttf
--rw-r--r--   0 jiaxuanli   (501) staff       (20)    68936 2023-04-14 03:09:55.000000 smplotlib-0.0.6/src/smplotlib/ttf/AVHersheyComplexHeavyItalic.ttf
--rw-r--r--   0 jiaxuanli   (501) staff       (20)    88976 2023-04-14 03:09:55.000000 smplotlib-0.0.6/src/smplotlib/ttf/AVHersheyComplexLight.ttf
--rw-r--r--   0 jiaxuanli   (501) staff       (20)    79800 2023-04-14 03:09:55.000000 smplotlib-0.0.6/src/smplotlib/ttf/AVHersheyComplexLightItalic.ttf
--rw-r--r--   0 jiaxuanli   (501) staff       (20)   131412 2023-04-14 03:09:55.000000 smplotlib-0.0.6/src/smplotlib/ttf/AVHersheyComplexMedium.ttf
--rw-r--r--   0 jiaxuanli   (501) staff       (20)   122572 2023-04-14 03:09:55.000000 smplotlib-0.0.6/src/smplotlib/ttf/AVHersheyComplexMediumItalic.ttf
--rw-r--r--   0 jiaxuanli   (501) staff       (20)    24356 2023-04-14 03:09:55.000000 smplotlib-0.0.6/src/smplotlib/ttf/AVHersheyDuplexHeavy.ttf
--rw-r--r--   0 jiaxuanli   (501) staff       (20)    22544 2023-04-14 03:09:55.000000 smplotlib-0.0.6/src/smplotlib/ttf/AVHersheyDuplexHeavyItalic.ttf
--rw-r--r--   0 jiaxuanli   (501) staff       (20)    44468 2023-04-14 03:09:55.000000 smplotlib-0.0.6/src/smplotlib/ttf/AVHersheyDuplexLight.ttf
--rw-r--r--   0 jiaxuanli   (501) staff       (20)    39724 2023-04-14 03:09:55.000000 smplotlib-0.0.6/src/smplotlib/ttf/AVHersheyDuplexLightItalic.ttf
--rw-r--r--   0 jiaxuanli   (501) staff       (20)    25640 2023-04-14 03:09:55.000000 smplotlib-0.0.6/src/smplotlib/ttf/AVHersheyDuplexMedium.ttf
--rw-r--r--   0 jiaxuanli   (501) staff       (20)    23516 2023-04-14 03:09:55.000000 smplotlib-0.0.6/src/smplotlib/ttf/AVHersheyDuplexMediumItalic.ttf
--rw-r--r--   0 jiaxuanli   (501) staff       (20)    28444 2023-04-14 03:09:55.000000 smplotlib-0.0.6/src/smplotlib/ttf/AVHersheySimplexHeavy.ttf
--rw-r--r--   0 jiaxuanli   (501) staff       (20)    25056 2023-04-14 03:09:55.000000 smplotlib-0.0.6/src/smplotlib/ttf/AVHersheySimplexHeavyItalic.ttf
--rw-r--r--   0 jiaxuanli   (501) staff       (20)    60092 2023-04-14 03:09:55.000000 smplotlib-0.0.6/src/smplotlib/ttf/AVHersheySimplexLight.ttf
--rw-r--r--   0 jiaxuanli   (501) staff       (20)    52776 2023-04-14 03:09:55.000000 smplotlib-0.0.6/src/smplotlib/ttf/AVHersheySimplexLightItalic.ttf
--rw-r--r--   0 jiaxuanli   (501) staff       (20)    28256 2023-04-14 03:09:55.000000 smplotlib-0.0.6/src/smplotlib/ttf/AVHersheySimplexMedium.ttf
--rw-r--r--   0 jiaxuanli   (501) staff       (20)    25140 2023-04-14 03:09:55.000000 smplotlib-0.0.6/src/smplotlib/ttf/AVHersheySimplexMediumItalic.ttf
-drwxr-xr-x   0 jiaxuanli   (501) staff       (20)        0 2023-04-18 01:19:12.000000 smplotlib-0.0.6/src/smplotlib.egg-info/
--rw-r--r--   0 jiaxuanli   (501) staff       (20)     2057 2023-04-18 01:19:12.000000 smplotlib-0.0.6/src/smplotlib.egg-info/PKG-INFO
--rw-r--r--   0 jiaxuanli   (501) staff       (20)     1169 2023-04-18 01:19:12.000000 smplotlib-0.0.6/src/smplotlib.egg-info/SOURCES.txt
--rw-r--r--   0 jiaxuanli   (501) staff       (20)        1 2023-04-18 01:19:12.000000 smplotlib-0.0.6/src/smplotlib.egg-info/dependency_links.txt
--rw-r--r--   0 jiaxuanli   (501) staff       (20)       10 2023-04-18 01:19:12.000000 smplotlib-0.0.6/src/smplotlib.egg-info/top_level.txt
--rw-r--r--   0 jiaxuanli   (501) staff       (20)    45260 2023-04-14 03:09:55.000000 smplotlib-0.0.6/two_phase.png
+drwxr-xr-x   0 jiaxuanli   (501) staff       (20)        0 2023-05-16 20:53:47.000000 smplotlib-0.0.7/
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)     1067 2023-04-19 19:05:25.000000 smplotlib-0.0.7/LICENSE
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)       70 2023-04-19 19:05:25.000000 smplotlib-0.0.7/MANIFEST.in
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)     2663 2023-05-16 20:53:47.000000 smplotlib-0.0.7/PKG-INFO
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)     2137 2023-05-09 17:28:53.000000 smplotlib-0.0.7/README.md
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)      652 2023-04-19 19:06:59.000000 smplotlib-0.0.7/pyproject.toml
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)       38 2023-05-16 20:53:47.000000 smplotlib-0.0.7/setup.cfg
+drwxr-xr-x   0 jiaxuanli   (501) staff       (20)        0 2023-05-16 20:53:47.000000 smplotlib-0.0.7/src/
+drwxr-xr-x   0 jiaxuanli   (501) staff       (20)        0 2023-05-16 20:53:47.000000 smplotlib-0.0.7/src/smplotlib/
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)     3225 2023-04-19 19:05:25.000000 smplotlib-0.0.7/src/smplotlib/__init__.py
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)     2275 2023-04-19 19:05:25.000000 smplotlib-0.0.7/src/smplotlib/demo.py
+drwxr-xr-x   0 jiaxuanli   (501) staff       (20)        0 2023-05-16 20:53:47.000000 smplotlib-0.0.7/src/smplotlib/test_data/
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)    16128 2023-04-19 19:05:25.000000 smplotlib-0.0.7/src/smplotlib/test_data/test_array.npy
+drwxr-xr-x   0 jiaxuanli   (501) staff       (20)        0 2023-05-16 20:53:47.000000 smplotlib-0.0.7/src/smplotlib/ttf/
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)    70276 2023-04-19 19:05:25.000000 smplotlib-0.0.7/src/smplotlib/ttf/AVHersheyComplexHeavy.ttf
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)    68936 2023-04-19 19:05:25.000000 smplotlib-0.0.7/src/smplotlib/ttf/AVHersheyComplexHeavyItalic.ttf
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)    88976 2023-04-19 19:05:25.000000 smplotlib-0.0.7/src/smplotlib/ttf/AVHersheyComplexLight.ttf
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)    79800 2023-04-19 19:05:25.000000 smplotlib-0.0.7/src/smplotlib/ttf/AVHersheyComplexLightItalic.ttf
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)   131412 2023-04-19 19:05:25.000000 smplotlib-0.0.7/src/smplotlib/ttf/AVHersheyComplexMedium.ttf
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)   122572 2023-04-19 19:05:25.000000 smplotlib-0.0.7/src/smplotlib/ttf/AVHersheyComplexMediumItalic.ttf
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)    24356 2023-04-19 19:05:25.000000 smplotlib-0.0.7/src/smplotlib/ttf/AVHersheyDuplexHeavy.ttf
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)    22544 2023-04-19 19:05:25.000000 smplotlib-0.0.7/src/smplotlib/ttf/AVHersheyDuplexHeavyItalic.ttf
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)    44468 2023-04-19 19:05:25.000000 smplotlib-0.0.7/src/smplotlib/ttf/AVHersheyDuplexLight.ttf
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)    39724 2023-04-19 19:05:25.000000 smplotlib-0.0.7/src/smplotlib/ttf/AVHersheyDuplexLightItalic.ttf
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)    25640 2023-04-19 19:05:25.000000 smplotlib-0.0.7/src/smplotlib/ttf/AVHersheyDuplexMedium.ttf
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)    23516 2023-04-19 19:05:25.000000 smplotlib-0.0.7/src/smplotlib/ttf/AVHersheyDuplexMediumItalic.ttf
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)    28444 2023-04-19 19:05:25.000000 smplotlib-0.0.7/src/smplotlib/ttf/AVHersheySimplexHeavy.ttf
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)    25056 2023-04-19 19:05:25.000000 smplotlib-0.0.7/src/smplotlib/ttf/AVHersheySimplexHeavyItalic.ttf
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)    60092 2023-04-19 19:05:25.000000 smplotlib-0.0.7/src/smplotlib/ttf/AVHersheySimplexLight.ttf
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)    52776 2023-04-19 19:05:25.000000 smplotlib-0.0.7/src/smplotlib/ttf/AVHersheySimplexLightItalic.ttf
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)    28256 2023-04-19 19:05:25.000000 smplotlib-0.0.7/src/smplotlib/ttf/AVHersheySimplexMedium.ttf
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)    25140 2023-04-19 19:05:25.000000 smplotlib-0.0.7/src/smplotlib/ttf/AVHersheySimplexMediumItalic.ttf
+drwxr-xr-x   0 jiaxuanli   (501) staff       (20)        0 2023-05-16 20:53:47.000000 smplotlib-0.0.7/src/smplotlib.egg-info/
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)     2663 2023-05-16 20:53:47.000000 smplotlib-0.0.7/src/smplotlib.egg-info/PKG-INFO
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)     1139 2023-05-16 20:53:47.000000 smplotlib-0.0.7/src/smplotlib.egg-info/SOURCES.txt
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)        1 2023-05-16 20:53:47.000000 smplotlib-0.0.7/src/smplotlib.egg-info/dependency_links.txt
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)       10 2023-05-16 20:53:47.000000 smplotlib-0.0.7/src/smplotlib.egg-info/top_level.txt
+-rw-r--r--   0 jiaxuanli   (501) staff       (20)    45260 2023-04-19 19:05:25.000000 smplotlib-0.0.7/two_phase.png
```

### Comparing `smplotlib-0.0.6/LICENSE` & `smplotlib-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.6/PKG-INFO` & `smplotlib-0.0.7/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: smplotlib
-Version: 0.0.6
+Version: 0.0.7
 Summary: Matplotlib template for SuperMongo style
 Author-email: Jiaxuan Li <jiaxuanl@princeton.edu>
 Project-URL: Homepage, https://github.com/AstroJacobLi/smplotlib
 Project-URL: Bug Tracker, https://github.com/AstroJacobLi/smplotlib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # smplotlib
+[![DOI](https://zenodo.org/badge/627675650.svg)](https://zenodo.org/badge/latestdoi/627675650) [![Downloads](https://static.pepy.tech/badge/smplotlib)](https://pepy.tech/project/smplotlib) [![PyPI version](https://badge.fury.io/py/smplotlib.svg)](https://badge.fury.io/py/smplotlib) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+
 Matplotlib template for [SuperMongo (SM)](https://www.astro.princeton.edu/~rhl/sm/) style. Make your plots stylish and professional (and old-school) by one line of code.
 
 ## Installation
 
 ```bash
 pip install smplotlib
 ```
@@ -35,7 +37,10 @@
 
 ![example](two_phase.png)
 
 ## Hershey font
 SuperMongo uses [Hershey fonts](https://www.astro.princeton.edu/~rhl/sm/sm.html#TOC73). The [``ttf`` files](https://github.com/yangcht/Hershey_font_TTF) are from a compilation by astronomer [`yangcht`](https://github.com/yangcht). Thanks for the great work! 
 
 There have been many [efforts](https://retrocomputingforum.com/t/hershey-fonts-the-original-vector-fonts/1852) on translating the [original](http://paulbourke.net/dataformats/hershey/) Hershey font to modern formats, also see [this](https://github.com/Dener-Silva/Hershey-TTF) and [this](https://github.com/scruss/AVHershey-OTF). The font files in this repo still lack some characters, and the support for LaTeX and light weight fonts are not satisfying. If you have any suggestions, please feel free to open an issue or pull request.
+
+## Citation
+If you find this package entertaining or useful, please consider citing it following the instructions in [![DOI](https://zenodo.org/badge/627675650.svg)](https://zenodo.org/badge/latestdoi/627675650).
```

### Comparing `smplotlib-0.0.6/README.md` & `smplotlib-0.0.7/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # smplotlib
+[![DOI](https://zenodo.org/badge/627675650.svg)](https://zenodo.org/badge/latestdoi/627675650) [![Downloads](https://static.pepy.tech/badge/smplotlib)](https://pepy.tech/project/smplotlib) [![PyPI version](https://badge.fury.io/py/smplotlib.svg)](https://badge.fury.io/py/smplotlib) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+
 Matplotlib template for [SuperMongo (SM)](https://www.astro.princeton.edu/~rhl/sm/) style. Make your plots stylish and professional (and old-school) by one line of code.
 
 ## Installation
 
 ```bash
 pip install smplotlib
 ```
@@ -20,8 +22,11 @@
 Then just use `matplotlib.pyplot` as usual. For a quick start, you can use `smplotlib.demo_plot()` to generate a figure with the default settings. This figure is inspired by the two-phase ISM figure in Prof. Bruce Draine's [book](https://www.astro.princeton.edu/~draine/book/index.html), but the cooling curve doesn't correspond to the actual CR rates and ISRF.
 
 ![example](two_phase.png)
 
 ## Hershey font
 SuperMongo uses [Hershey fonts](https://www.astro.princeton.edu/~rhl/sm/sm.html#TOC73). The [``ttf`` files](https://github.com/yangcht/Hershey_font_TTF) are from a compilation by astronomer [`yangcht`](https://github.com/yangcht). Thanks for the great work! 
 
-There have been many [efforts](https://retrocomputingforum.com/t/hershey-fonts-the-original-vector-fonts/1852) on translating the [original](http://paulbourke.net/dataformats/hershey/) Hershey font to modern formats, also see [this](https://github.com/Dener-Silva/Hershey-TTF) and [this](https://github.com/scruss/AVHershey-OTF). The font files in this repo still lack some characters, and the support for LaTeX and light weight fonts are not satisfying. If you have any suggestions, please feel free to open an issue or pull request.
+There have been many [efforts](https://retrocomputingforum.com/t/hershey-fonts-the-original-vector-fonts/1852) on translating the [original](http://paulbourke.net/dataformats/hershey/) Hershey font to modern formats, also see [this](https://github.com/Dener-Silva/Hershey-TTF) and [this](https://github.com/scruss/AVHershey-OTF). The font files in this repo still lack some characters, and the support for LaTeX and light weight fonts are not satisfying. If you have any suggestions, please feel free to open an issue or pull request.
+
+## Citation
+If you find this package entertaining or useful, please consider citing it following the instructions in [![DOI](https://zenodo.org/badge/627675650.svg)](https://zenodo.org/badge/latestdoi/627675650).
```

### Comparing `smplotlib-0.0.6/pyproject.toml` & `smplotlib-0.0.7/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "smplotlib"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Jiaxuan Li", email="jiaxuanl@princeton.edu" },
 ]
 description = "Matplotlib template for SuperMongo style"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `smplotlib-0.0.6/src/smplotlib/__init__.py` & `smplotlib-0.0.7/src/smplotlib/__init__.py`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.6/src/smplotlib/demo.py` & `smplotlib-0.0.7/src/smplotlib/demo.py`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.6/src/smplotlib/test_data/test_array.npy` & `smplotlib-0.0.7/src/smplotlib/test_data/test_array.npy`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.6/src/smplotlib/ttf/AVHersheyComplexHeavy.ttf` & `smplotlib-0.0.7/src/smplotlib/ttf/AVHersheyComplexHeavy.ttf`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.6/src/smplotlib/ttf/AVHersheyComplexHeavyItalic.ttf` & `smplotlib-0.0.7/src/smplotlib/ttf/AVHersheyComplexHeavyItalic.ttf`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.6/src/smplotlib/ttf/AVHersheyComplexLight.ttf` & `smplotlib-0.0.7/src/smplotlib/ttf/AVHersheyComplexLight.ttf`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.6/src/smplotlib/ttf/AVHersheyComplexLightItalic.ttf` & `smplotlib-0.0.7/src/smplotlib/ttf/AVHersheyComplexLightItalic.ttf`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.6/src/smplotlib/ttf/AVHersheyComplexMedium.ttf` & `smplotlib-0.0.7/src/smplotlib/ttf/AVHersheyComplexMedium.ttf`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.6/src/smplotlib/ttf/AVHersheyComplexMediumItalic.ttf` & `smplotlib-0.0.7/src/smplotlib/ttf/AVHersheyComplexMediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.6/src/smplotlib/ttf/AVHersheyDuplexHeavy.ttf` & `smplotlib-0.0.7/src/smplotlib/ttf/AVHersheyDuplexHeavy.ttf`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.6/src/smplotlib/ttf/AVHersheyDuplexHeavyItalic.ttf` & `smplotlib-0.0.7/src/smplotlib/ttf/AVHersheyDuplexHeavyItalic.ttf`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.6/src/smplotlib/ttf/AVHersheyDuplexLight.ttf` & `smplotlib-0.0.7/src/smplotlib/ttf/AVHersheyDuplexLight.ttf`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.6/src/smplotlib/ttf/AVHersheyDuplexLightItalic.ttf` & `smplotlib-0.0.7/src/smplotlib/ttf/AVHersheyDuplexLightItalic.ttf`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.6/src/smplotlib/ttf/AVHersheyDuplexMedium.ttf` & `smplotlib-0.0.7/src/smplotlib/ttf/AVHersheyDuplexMedium.ttf`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.6/src/smplotlib/ttf/AVHersheyDuplexMediumItalic.ttf` & `smplotlib-0.0.7/src/smplotlib/ttf/AVHersheyDuplexMediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.6/src/smplotlib/ttf/AVHersheySimplexHeavy.ttf` & `smplotlib-0.0.7/src/smplotlib/ttf/AVHersheySimplexHeavy.ttf`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.6/src/smplotlib/ttf/AVHersheySimplexHeavyItalic.ttf` & `smplotlib-0.0.7/src/smplotlib/ttf/AVHersheySimplexHeavyItalic.ttf`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.6/src/smplotlib/ttf/AVHersheySimplexLight.ttf` & `smplotlib-0.0.7/src/smplotlib/ttf/AVHersheySimplexLight.ttf`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.6/src/smplotlib/ttf/AVHersheySimplexLightItalic.ttf` & `smplotlib-0.0.7/src/smplotlib/ttf/AVHersheySimplexLightItalic.ttf`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.6/src/smplotlib/ttf/AVHersheySimplexMedium.ttf` & `smplotlib-0.0.7/src/smplotlib/ttf/AVHersheySimplexMedium.ttf`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.6/src/smplotlib/ttf/AVHersheySimplexMediumItalic.ttf` & `smplotlib-0.0.7/src/smplotlib/ttf/AVHersheySimplexMediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `smplotlib-0.0.6/src/smplotlib.egg-info/PKG-INFO` & `smplotlib-0.0.7/src/smplotlib.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: smplotlib
-Version: 0.0.6
+Version: 0.0.7
 Summary: Matplotlib template for SuperMongo style
 Author-email: Jiaxuan Li <jiaxuanl@princeton.edu>
 Project-URL: Homepage, https://github.com/AstroJacobLi/smplotlib
 Project-URL: Bug Tracker, https://github.com/AstroJacobLi/smplotlib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # smplotlib
+[![DOI](https://zenodo.org/badge/627675650.svg)](https://zenodo.org/badge/latestdoi/627675650) [![Downloads](https://static.pepy.tech/badge/smplotlib)](https://pepy.tech/project/smplotlib) [![PyPI version](https://badge.fury.io/py/smplotlib.svg)](https://badge.fury.io/py/smplotlib) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+
 Matplotlib template for [SuperMongo (SM)](https://www.astro.princeton.edu/~rhl/sm/) style. Make your plots stylish and professional (and old-school) by one line of code.
 
 ## Installation
 
 ```bash
 pip install smplotlib
 ```
@@ -35,7 +37,10 @@
 
 ![example](two_phase.png)
 
 ## Hershey font
 SuperMongo uses [Hershey fonts](https://www.astro.princeton.edu/~rhl/sm/sm.html#TOC73). The [``ttf`` files](https://github.com/yangcht/Hershey_font_TTF) are from a compilation by astronomer [`yangcht`](https://github.com/yangcht). Thanks for the great work! 
 
 There have been many [efforts](https://retrocomputingforum.com/t/hershey-fonts-the-original-vector-fonts/1852) on translating the [original](http://paulbourke.net/dataformats/hershey/) Hershey font to modern formats, also see [this](https://github.com/Dener-Silva/Hershey-TTF) and [this](https://github.com/scruss/AVHershey-OTF). The font files in this repo still lack some characters, and the support for LaTeX and light weight fonts are not satisfying. If you have any suggestions, please feel free to open an issue or pull request.
+
+## Citation
+If you find this package entertaining or useful, please consider citing it following the instructions in [![DOI](https://zenodo.org/badge/627675650.svg)](https://zenodo.org/badge/latestdoi/627675650).
```

### Comparing `smplotlib-0.0.6/src/smplotlib.egg-info/SOURCES.txt` & `smplotlib-0.0.7/src/smplotlib.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 two_phase.png
 src/smplotlib/__init__.py
 src/smplotlib/demo.py
-src/smplotlib/smplot.mplstyle
 src/smplotlib.egg-info/PKG-INFO
 src/smplotlib.egg-info/SOURCES.txt
 src/smplotlib.egg-info/dependency_links.txt
 src/smplotlib.egg-info/top_level.txt
 src/smplotlib/test_data/test_array.npy
 src/smplotlib/ttf/AVHersheyComplexHeavy.ttf
 src/smplotlib/ttf/AVHersheyComplexHeavyItalic.ttf
```

### Comparing `smplotlib-0.0.6/two_phase.png` & `smplotlib-0.0.7/two_phase.png`

 * *Files identical despite different names*

