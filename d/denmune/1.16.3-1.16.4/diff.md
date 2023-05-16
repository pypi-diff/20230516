# Comparing `tmp/denmune-1.16.3.tar.gz` & `tmp/denmune-1.16.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "denmune-1.16.3.tar", last modified: Tue May 16 13:52:20 2023, max compression
+gzip compressed data, was "denmune-1.16.4.tar", last modified: Tue May 16 14:32:08 2023, max compression
```

## Comparing `denmune-1.16.3.tar` & `denmune-1.16.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 13:52:20.308588 denmune-1.16.3/
--rw-rw-rw-   0        0        0     1498 2021-12-31 23:30:13.000000 denmune-1.16.3/LICENSE
--rw-rw-rw-   0        0        0       47 2021-12-27 21:52:58.000000 denmune-1.16.3/MANIFEST.in
--rw-rw-rw-   0        0        0    29848 2023-05-16 13:52:20.310590 denmune-1.16.3/PKG-INFO
--rw-rw-rw-   0        0        0    29177 2023-05-16 13:50:19.000000 denmune-1.16.3/README.md
--rw-rw-rw-   0        0        0      108 2021-12-23 20:19:35.000000 denmune-1.16.3/pyproject.toml
--rw-rw-rw-   0        0        0      810 2023-05-16 13:52:20.314794 denmune-1.16.3/setup.cfg
--rw-rw-rw-   0        0        0      257 2023-05-16 13:50:59.000000 denmune-1.16.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-16 13:52:20.223706 denmune-1.16.3/src/
-drwxrwxrwx   0        0        0        0 2023-05-16 13:52:20.277095 denmune-1.16.3/src/denmune/
--rw-rw-rw-   0        0        0       28 2022-05-12 02:48:25.000000 denmune-1.16.3/src/denmune/__init__.py
--rw-rw-rw-   0        0        0    39240 2023-04-30 00:20:12.000000 denmune-1.16.3/src/denmune/denmune.py
-drwxrwxrwx   0        0        0        0 2023-05-16 13:52:20.305583 denmune-1.16.3/src/denmune.egg-info/
--rw-rw-rw-   0        0        0    29848 2023-05-16 13:52:20.000000 denmune-1.16.3/src/denmune.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2023-05-16 13:52:20.000000 denmune-1.16.3/src/denmune.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 13:52:20.000000 denmune-1.16.3/src/denmune.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      123 2023-05-16 13:52:20.000000 denmune-1.16.3/src/denmune.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-16 13:52:20.000000 denmune-1.16.3/src/denmune.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 14:32:08.660427 denmune-1.16.4/
+-rw-rw-rw-   0        0        0     1498 2021-12-31 23:30:13.000000 denmune-1.16.4/LICENSE
+-rw-rw-rw-   0        0        0       47 2021-12-27 21:52:58.000000 denmune-1.16.4/MANIFEST.in
+-rw-rw-rw-   0        0        0    29731 2023-05-16 14:32:08.661540 denmune-1.16.4/PKG-INFO
+-rw-rw-rw-   0        0        0    29060 2023-05-16 14:30:55.000000 denmune-1.16.4/README.md
+-rw-rw-rw-   0        0        0      108 2021-12-23 20:19:35.000000 denmune-1.16.4/pyproject.toml
+-rw-rw-rw-   0        0        0      810 2023-05-16 14:32:08.664940 denmune-1.16.4/setup.cfg
+-rw-rw-rw-   0        0        0      257 2023-05-16 13:50:59.000000 denmune-1.16.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:32:08.584559 denmune-1.16.4/src/
+drwxrwxrwx   0        0        0        0 2023-05-16 14:32:08.624353 denmune-1.16.4/src/denmune/
+-rw-rw-rw-   0        0        0       28 2022-05-12 02:48:25.000000 denmune-1.16.4/src/denmune/__init__.py
+-rw-rw-rw-   0        0        0    39240 2023-04-30 00:20:12.000000 denmune-1.16.4/src/denmune/denmune.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:32:08.657396 denmune-1.16.4/src/denmune.egg-info/
+-rw-rw-rw-   0        0        0    29731 2023-05-16 14:32:08.000000 denmune-1.16.4/src/denmune.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2023-05-16 14:32:08.000000 denmune-1.16.4/src/denmune.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 14:32:08.000000 denmune-1.16.4/src/denmune.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      123 2023-05-16 14:32:08.000000 denmune-1.16.4/src/denmune.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-16 14:32:08.000000 denmune-1.16.4/src/denmune.egg-info/top_level.txt
```

### Comparing `denmune-1.16.3/LICENSE` & `denmune-1.16.4/LICENSE`

 * *Files identical despite different names*

### Comparing `denmune-1.16.3/PKG-INFO` & `denmune-1.16.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denmune
-Version: 1.16.3
+Version: 1.16.4
 Summary: This is the package for DenMune Clustering Algorithm published in paper https://doi.org/10.1016/j.patcog.2020.107589
 Home-page: https://github.com/scikit-learn-contrib/denmune-clustering-algorithm
 Author: Dr. Mohamed Ali Abbas & Prof. Amin  Shoukry
 Author-email: mohamed.alyabbas@outlook.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
@@ -67,15 +67,15 @@
 This 30 seconds will tell you how a density-based algorithm, DenMune propagates:
 
   [![interact with the propagation](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1o-tP3uvDGjxBOGYkir1lnbr74sZ06e0U?usp=sharing)
 
   [![Propagation in DenMune](https://raw.githubusercontent.com/egy1st/denmune-clustering-algorithm/main/images/propagation.gif)]()
 
 ## Still interested?
-Watch this ***10-min*** illustrative video on Vimeo (no ads). Thank you Vimeo for making it possible without any distraction (No ads. We hate ads).
+Watch this ***10-min*** illustrative video on:
 
 - [![watch on Vimeo](https://img.shields.io/badge/watch_on-vimeo-green?style=for-the-badge)](https://player.vimeo.com/video/827209757)
 - [![YouTube Video Views](https://img.shields.io/youtube/views/o77raaasuOM?style=for-the-badge)](https://www.youtube.com/watch?v=o77raaasuOM) on Youtube
 
 
 
 ## When less means more
@@ -467,30 +467,30 @@
 -  If you are a kaggler like me, then Kaggle, the best workspace where data scientist meet, should fit you to test the algorithm with great experience. 
 
 
 
 Here is a list of Google CoLab & Kaggle notebooks  to practice the use of  the algorithm interactively.
 
 
-| Dataset                       | CoLab notebook                                               | Kaggle notebook                                              |
-| ----------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
-| How to use it?                | [![How to use it - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/how-to-use) | [![When less means more - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/how-to-use) |
-| Chameleon datasets            | [![Chameleon datasets - colab]( https://colab.research.google.com/assets/colab-badge.svg)](https://denmune.egy1st.org/colab/chameleon) | [![Non-groundtruth datasets](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/chameleon) |
-| 2D Shape datasets             | [![2D Shape datasets - colab]( https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/2d-shapes) | [![2D Shape datasets - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/2d-shapes) |
-| MNIST dataset                 | [![MNIST dataset - colab](https://colab.research.google.com/assets/colab-badge.svg)](https://denmune.egy1st.org/colab/mnist-dataset) | [![MNIST dataset - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/mnist-dataset) |
-| iris dataset                  | [![iris dataset - colab](https://colab.research.google.com/assets/colab-badge.svg)](https://denmune.egy1st.org/colab/iris-dataset) | [![iris dataset - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/iris-dataset) |
-| Scoring 97% on MNIST dataset  | [![Get 97% by training MNIST dataset - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/score-97-mnist) | [![Training MNIST to get 97%](https://kaggle.com/static/images/open-in-kaggle.svg)]( https://denmune.egy1st.org/kaggle/score-97-mnist) |
-| Clustering unlabeled datasets | [![Non-groundtruth datasets - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/unlabeled-data) | [![Non-groundtruth datasets](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/unlabeled-data) |
-| Noise detection               | [![Noise detection - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/noise-detection ) | [![Noise detection - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)]( https://denmune.egy1st.org/kaggle/noise-detection) |
-| Validation                    | [![Validation - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/how-to-validate ) | [![Validation - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)]( https://denmune.egy1st.org/kaggle/how-to-validate) |
-| How does it propagate?        | [![How it propagates - colab](https://colab.research.google.com/assets/colab-badge.svg)](https://denmune.egy1st.org/colab/how-propagate ) | [![The beauty of propagation - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)]( https://denmune.egy1st.org/kaggle/how-propagate) <br />[![The beauty of propagation part 2 - kaggle]( https://kaggle.com/static/images/open-in-kaggle.svg)]( https://denmune.egy1st.org/kaggle/how-propagate-2) |
-| Snapshots of propagation      | [![snapshots of the propagation - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/propagation-shots ) | [![The beauty of propagation - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)]( https://denmune.egy1st.org/kaggle/propagation-shots ) |
-| Scalability                   | [![Scalability - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/scalability ) | [![Scalability - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/scalability) |
-| Stability                     | [![Stability vs number of nearest neighbors - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/stability) | [![Stability - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/stability) |
-| k-nearest-evolution           | [![k-nearest-evolution - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/knn-evolution) | [![k-nearest-evolution - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)]( https://denmune.egy1st.org/kaggle/knn-evolution ) |
+| Dataset                      | CoLab notebook                                               | Kaggle notebook                                              |
+| ---------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
+| How to use it?               | [![How to use it - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/how-to-use) | [![When less means more - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/how-to-use) |
+| Chameleon datasets           | [![Chameleon datasets - colab]( https://colab.research.google.com/assets/colab-badge.svg)](https://denmune.egy1st.org/colab/chameleon) | [![Non-groundtruth datasets](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/chameleon) |
+| 2D Shape datasets            | [![2D Shape datasets - colab]( https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/2d-shapes) | [![2D Shape datasets - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/2d-shapes) |
+| Clustering unlabeled data    | [![Non-groundtruth datasets - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/unlabeled-data) | [![Non-groundtruth datasets](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/unlabeled-data) |
+| iris dataset                 | [![iris dataset - colab](https://colab.research.google.com/assets/colab-badge.svg)](https://denmune.egy1st.org/colab/iris-dataset) | [![iris dataset - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/iris-dataset) |
+| MNIST dataset                | [![MNIST dataset - colab](https://colab.research.google.com/assets/colab-badge.svg)](https://denmune.egy1st.org/colab/mnist-dataset) | [![MNIST dataset - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/mnist-dataset) |
+| Scoring 97% on MNIST dataset | [![Get 97% by training MNIST dataset - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/score-97-mnist) | [![Training MNIST to get 97%](https://kaggle.com/static/images/open-in-kaggle.svg)]( https://denmune.egy1st.org/kaggle/score-97-mnist) |
+| Noise detection              | [![Noise detection - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/noise-detection ) | [![Noise detection - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)]( https://denmune.egy1st.org/kaggle/noise-detection) |
+| Validation                   | [![Validation - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/how-to-validate ) | [![Validation - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)]( https://denmune.egy1st.org/kaggle/how-to-validate) |
+| How does it propagate?       | [![How it propagates - colab](https://colab.research.google.com/assets/colab-badge.svg)](https://denmune.egy1st.org/colab/how-propagate ) | [![The beauty of propagation - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)]( https://denmune.egy1st.org/kaggle/how-propagate) <br />[![The beauty of propagation part 2 - kaggle]( https://kaggle.com/static/images/open-in-kaggle.svg)]( https://denmune.egy1st.org/kaggle/how-propagate-2) |
+| Snapshots of propagation     | [![snapshots of the propagation - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/propagation-shots ) | [![The beauty of propagation - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)]( https://denmune.egy1st.org/kaggle/propagation-shots ) |
+| Scalability                  | [![Scalability - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/scalability ) | [![Scalability - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/scalability) |
+| Stability                    | [![Stability vs number of nearest neighbors - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/stability) | [![Stability - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/stability) |
+| k-nearest-evolution          | [![k-nearest-evolution - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/knn-evolution) | [![k-nearest-evolution - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)]( https://denmune.egy1st.org/kaggle/knn-evolution ) |
 
 
 
 ## How to cite
 If you have used this codebase in a scientific publication and wish to cite it, please use the [Journal of Pattern Recognition article](https://www.sciencedirect.com/science/article/abs/pii/S0031320320303927)
 
       Mohamed Abbas McInnes, Adel El-Zoghaby, Amin Ahoukry, *DenMune: Density peak based clustering using mutual nearest neighbors*
```

### Comparing `denmune-1.16.3/README.md` & `denmune-1.16.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 This 30 seconds will tell you how a density-based algorithm, DenMune propagates:
 
   [![interact with the propagation](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1o-tP3uvDGjxBOGYkir1lnbr74sZ06e0U?usp=sharing)
 
   [![Propagation in DenMune](https://raw.githubusercontent.com/egy1st/denmune-clustering-algorithm/main/images/propagation.gif)]()
 
 ## Still interested?
-Watch this ***10-min*** illustrative video on Vimeo (no ads). Thank you Vimeo for making it possible without any distraction (No ads. We hate ads).
+Watch this ***10-min*** illustrative video on:
 
 - [![watch on Vimeo](https://img.shields.io/badge/watch_on-vimeo-green?style=for-the-badge)](https://player.vimeo.com/video/827209757)
 - [![YouTube Video Views](https://img.shields.io/youtube/views/o77raaasuOM?style=for-the-badge)](https://www.youtube.com/watch?v=o77raaasuOM) on Youtube
 
 
 
 ## When less means more
@@ -452,30 +452,30 @@
 -  If you are a kaggler like me, then Kaggle, the best workspace where data scientist meet, should fit you to test the algorithm with great experience. 
 
 
 
 Here is a list of Google CoLab & Kaggle notebooks  to practice the use of  the algorithm interactively.
 
 
-| Dataset                       | CoLab notebook                                               | Kaggle notebook                                              |
-| ----------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
-| How to use it?                | [![How to use it - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/how-to-use) | [![When less means more - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/how-to-use) |
-| Chameleon datasets            | [![Chameleon datasets - colab]( https://colab.research.google.com/assets/colab-badge.svg)](https://denmune.egy1st.org/colab/chameleon) | [![Non-groundtruth datasets](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/chameleon) |
-| 2D Shape datasets             | [![2D Shape datasets - colab]( https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/2d-shapes) | [![2D Shape datasets - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/2d-shapes) |
-| MNIST dataset                 | [![MNIST dataset - colab](https://colab.research.google.com/assets/colab-badge.svg)](https://denmune.egy1st.org/colab/mnist-dataset) | [![MNIST dataset - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/mnist-dataset) |
-| iris dataset                  | [![iris dataset - colab](https://colab.research.google.com/assets/colab-badge.svg)](https://denmune.egy1st.org/colab/iris-dataset) | [![iris dataset - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/iris-dataset) |
-| Scoring 97% on MNIST dataset  | [![Get 97% by training MNIST dataset - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/score-97-mnist) | [![Training MNIST to get 97%](https://kaggle.com/static/images/open-in-kaggle.svg)]( https://denmune.egy1st.org/kaggle/score-97-mnist) |
-| Clustering unlabeled datasets | [![Non-groundtruth datasets - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/unlabeled-data) | [![Non-groundtruth datasets](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/unlabeled-data) |
-| Noise detection               | [![Noise detection - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/noise-detection ) | [![Noise detection - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)]( https://denmune.egy1st.org/kaggle/noise-detection) |
-| Validation                    | [![Validation - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/how-to-validate ) | [![Validation - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)]( https://denmune.egy1st.org/kaggle/how-to-validate) |
-| How does it propagate?        | [![How it propagates - colab](https://colab.research.google.com/assets/colab-badge.svg)](https://denmune.egy1st.org/colab/how-propagate ) | [![The beauty of propagation - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)]( https://denmune.egy1st.org/kaggle/how-propagate) <br />[![The beauty of propagation part 2 - kaggle]( https://kaggle.com/static/images/open-in-kaggle.svg)]( https://denmune.egy1st.org/kaggle/how-propagate-2) |
-| Snapshots of propagation      | [![snapshots of the propagation - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/propagation-shots ) | [![The beauty of propagation - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)]( https://denmune.egy1st.org/kaggle/propagation-shots ) |
-| Scalability                   | [![Scalability - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/scalability ) | [![Scalability - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/scalability) |
-| Stability                     | [![Stability vs number of nearest neighbors - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/stability) | [![Stability - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/stability) |
-| k-nearest-evolution           | [![k-nearest-evolution - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/knn-evolution) | [![k-nearest-evolution - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)]( https://denmune.egy1st.org/kaggle/knn-evolution ) |
+| Dataset                      | CoLab notebook                                               | Kaggle notebook                                              |
+| ---------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
+| How to use it?               | [![How to use it - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/how-to-use) | [![When less means more - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/how-to-use) |
+| Chameleon datasets           | [![Chameleon datasets - colab]( https://colab.research.google.com/assets/colab-badge.svg)](https://denmune.egy1st.org/colab/chameleon) | [![Non-groundtruth datasets](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/chameleon) |
+| 2D Shape datasets            | [![2D Shape datasets - colab]( https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/2d-shapes) | [![2D Shape datasets - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/2d-shapes) |
+| Clustering unlabeled data    | [![Non-groundtruth datasets - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/unlabeled-data) | [![Non-groundtruth datasets](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/unlabeled-data) |
+| iris dataset                 | [![iris dataset - colab](https://colab.research.google.com/assets/colab-badge.svg)](https://denmune.egy1st.org/colab/iris-dataset) | [![iris dataset - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/iris-dataset) |
+| MNIST dataset                | [![MNIST dataset - colab](https://colab.research.google.com/assets/colab-badge.svg)](https://denmune.egy1st.org/colab/mnist-dataset) | [![MNIST dataset - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/mnist-dataset) |
+| Scoring 97% on MNIST dataset | [![Get 97% by training MNIST dataset - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/score-97-mnist) | [![Training MNIST to get 97%](https://kaggle.com/static/images/open-in-kaggle.svg)]( https://denmune.egy1st.org/kaggle/score-97-mnist) |
+| Noise detection              | [![Noise detection - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/noise-detection ) | [![Noise detection - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)]( https://denmune.egy1st.org/kaggle/noise-detection) |
+| Validation                   | [![Validation - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/how-to-validate ) | [![Validation - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)]( https://denmune.egy1st.org/kaggle/how-to-validate) |
+| How does it propagate?       | [![How it propagates - colab](https://colab.research.google.com/assets/colab-badge.svg)](https://denmune.egy1st.org/colab/how-propagate ) | [![The beauty of propagation - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)]( https://denmune.egy1st.org/kaggle/how-propagate) <br />[![The beauty of propagation part 2 - kaggle]( https://kaggle.com/static/images/open-in-kaggle.svg)]( https://denmune.egy1st.org/kaggle/how-propagate-2) |
+| Snapshots of propagation     | [![snapshots of the propagation - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/propagation-shots ) | [![The beauty of propagation - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)]( https://denmune.egy1st.org/kaggle/propagation-shots ) |
+| Scalability                  | [![Scalability - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/scalability ) | [![Scalability - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/scalability) |
+| Stability                    | [![Stability vs number of nearest neighbors - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/stability) | [![Stability - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/stability) |
+| k-nearest-evolution          | [![k-nearest-evolution - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/knn-evolution) | [![k-nearest-evolution - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)]( https://denmune.egy1st.org/kaggle/knn-evolution ) |
 
 
 
 ## How to cite
 If you have used this codebase in a scientific publication and wish to cite it, please use the [Journal of Pattern Recognition article](https://www.sciencedirect.com/science/article/abs/pii/S0031320320303927)
 
       Mohamed Abbas McInnes, Adel El-Zoghaby, Amin Ahoukry, *DenMune: Density peak based clustering using mutual nearest neighbors*
```

### Comparing `denmune-1.16.3/setup.cfg` & `denmune-1.16.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 656e 6d75 6e65 0d0a 7665 7273   = denmune..vers
-00000020: 696f 6e20 3d20 312e 3136 2e33 0d0a 6175  ion = 1.16.3..au
+00000020: 696f 6e20 3d20 312e 3136 2e34 0d0a 6175  ion = 1.16.4..au
 00000030: 7468 6f72 203d 2044 722e 204d 6f68 616d  thor = Dr. Moham
 00000040: 6564 2041 6c69 2041 6262 6173 2026 2050  ed Ali Abbas & P
 00000050: 726f 662e 2041 6d69 6e20 2053 686f 756b  rof. Amin  Shouk
 00000060: 7279 0d0a 6175 7468 6f72 5f65 6d61 696c  ry..author_email
 00000070: 203d 206d 6f68 616d 6564 2e61 6c79 6162   = mohamed.alyab
 00000080: 6261 7340 6f75 746c 6f6f 6b2e 636f 6d0d  bas@outlook.com.
 00000090: 0a64 6573 6372 6970 7469 6f6e 203d 2054  .description = T
```

### Comparing `denmune-1.16.3/src/denmune/denmune.py` & `denmune-1.16.4/src/denmune/denmune.py`

 * *Files identical despite different names*

### Comparing `denmune-1.16.3/src/denmune.egg-info/PKG-INFO` & `denmune-1.16.4/src/denmune.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denmune
-Version: 1.16.3
+Version: 1.16.4
 Summary: This is the package for DenMune Clustering Algorithm published in paper https://doi.org/10.1016/j.patcog.2020.107589
 Home-page: https://github.com/scikit-learn-contrib/denmune-clustering-algorithm
 Author: Dr. Mohamed Ali Abbas & Prof. Amin  Shoukry
 Author-email: mohamed.alyabbas@outlook.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
@@ -67,15 +67,15 @@
 This 30 seconds will tell you how a density-based algorithm, DenMune propagates:
 
   [![interact with the propagation](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1o-tP3uvDGjxBOGYkir1lnbr74sZ06e0U?usp=sharing)
 
   [![Propagation in DenMune](https://raw.githubusercontent.com/egy1st/denmune-clustering-algorithm/main/images/propagation.gif)]()
 
 ## Still interested?
-Watch this ***10-min*** illustrative video on Vimeo (no ads). Thank you Vimeo for making it possible without any distraction (No ads. We hate ads).
+Watch this ***10-min*** illustrative video on:
 
 - [![watch on Vimeo](https://img.shields.io/badge/watch_on-vimeo-green?style=for-the-badge)](https://player.vimeo.com/video/827209757)
 - [![YouTube Video Views](https://img.shields.io/youtube/views/o77raaasuOM?style=for-the-badge)](https://www.youtube.com/watch?v=o77raaasuOM) on Youtube
 
 
 
 ## When less means more
@@ -467,30 +467,30 @@
 -  If you are a kaggler like me, then Kaggle, the best workspace where data scientist meet, should fit you to test the algorithm with great experience. 
 
 
 
 Here is a list of Google CoLab & Kaggle notebooks  to practice the use of  the algorithm interactively.
 
 
-| Dataset                       | CoLab notebook                                               | Kaggle notebook                                              |
-| ----------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
-| How to use it?                | [![How to use it - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/how-to-use) | [![When less means more - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/how-to-use) |
-| Chameleon datasets            | [![Chameleon datasets - colab]( https://colab.research.google.com/assets/colab-badge.svg)](https://denmune.egy1st.org/colab/chameleon) | [![Non-groundtruth datasets](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/chameleon) |
-| 2D Shape datasets             | [![2D Shape datasets - colab]( https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/2d-shapes) | [![2D Shape datasets - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/2d-shapes) |
-| MNIST dataset                 | [![MNIST dataset - colab](https://colab.research.google.com/assets/colab-badge.svg)](https://denmune.egy1st.org/colab/mnist-dataset) | [![MNIST dataset - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/mnist-dataset) |
-| iris dataset                  | [![iris dataset - colab](https://colab.research.google.com/assets/colab-badge.svg)](https://denmune.egy1st.org/colab/iris-dataset) | [![iris dataset - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/iris-dataset) |
-| Scoring 97% on MNIST dataset  | [![Get 97% by training MNIST dataset - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/score-97-mnist) | [![Training MNIST to get 97%](https://kaggle.com/static/images/open-in-kaggle.svg)]( https://denmune.egy1st.org/kaggle/score-97-mnist) |
-| Clustering unlabeled datasets | [![Non-groundtruth datasets - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/unlabeled-data) | [![Non-groundtruth datasets](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/unlabeled-data) |
-| Noise detection               | [![Noise detection - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/noise-detection ) | [![Noise detection - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)]( https://denmune.egy1st.org/kaggle/noise-detection) |
-| Validation                    | [![Validation - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/how-to-validate ) | [![Validation - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)]( https://denmune.egy1st.org/kaggle/how-to-validate) |
-| How does it propagate?        | [![How it propagates - colab](https://colab.research.google.com/assets/colab-badge.svg)](https://denmune.egy1st.org/colab/how-propagate ) | [![The beauty of propagation - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)]( https://denmune.egy1st.org/kaggle/how-propagate) <br />[![The beauty of propagation part 2 - kaggle]( https://kaggle.com/static/images/open-in-kaggle.svg)]( https://denmune.egy1st.org/kaggle/how-propagate-2) |
-| Snapshots of propagation      | [![snapshots of the propagation - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/propagation-shots ) | [![The beauty of propagation - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)]( https://denmune.egy1st.org/kaggle/propagation-shots ) |
-| Scalability                   | [![Scalability - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/scalability ) | [![Scalability - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/scalability) |
-| Stability                     | [![Stability vs number of nearest neighbors - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/stability) | [![Stability - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/stability) |
-| k-nearest-evolution           | [![k-nearest-evolution - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/knn-evolution) | [![k-nearest-evolution - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)]( https://denmune.egy1st.org/kaggle/knn-evolution ) |
+| Dataset                      | CoLab notebook                                               | Kaggle notebook                                              |
+| ---------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
+| How to use it?               | [![How to use it - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/how-to-use) | [![When less means more - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/how-to-use) |
+| Chameleon datasets           | [![Chameleon datasets - colab]( https://colab.research.google.com/assets/colab-badge.svg)](https://denmune.egy1st.org/colab/chameleon) | [![Non-groundtruth datasets](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/chameleon) |
+| 2D Shape datasets            | [![2D Shape datasets - colab]( https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/2d-shapes) | [![2D Shape datasets - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/2d-shapes) |
+| Clustering unlabeled data    | [![Non-groundtruth datasets - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/unlabeled-data) | [![Non-groundtruth datasets](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/unlabeled-data) |
+| iris dataset                 | [![iris dataset - colab](https://colab.research.google.com/assets/colab-badge.svg)](https://denmune.egy1st.org/colab/iris-dataset) | [![iris dataset - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/iris-dataset) |
+| MNIST dataset                | [![MNIST dataset - colab](https://colab.research.google.com/assets/colab-badge.svg)](https://denmune.egy1st.org/colab/mnist-dataset) | [![MNIST dataset - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/mnist-dataset) |
+| Scoring 97% on MNIST dataset | [![Get 97% by training MNIST dataset - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/score-97-mnist) | [![Training MNIST to get 97%](https://kaggle.com/static/images/open-in-kaggle.svg)]( https://denmune.egy1st.org/kaggle/score-97-mnist) |
+| Noise detection              | [![Noise detection - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/noise-detection ) | [![Noise detection - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)]( https://denmune.egy1st.org/kaggle/noise-detection) |
+| Validation                   | [![Validation - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/how-to-validate ) | [![Validation - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)]( https://denmune.egy1st.org/kaggle/how-to-validate) |
+| How does it propagate?       | [![How it propagates - colab](https://colab.research.google.com/assets/colab-badge.svg)](https://denmune.egy1st.org/colab/how-propagate ) | [![The beauty of propagation - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)]( https://denmune.egy1st.org/kaggle/how-propagate) <br />[![The beauty of propagation part 2 - kaggle]( https://kaggle.com/static/images/open-in-kaggle.svg)]( https://denmune.egy1st.org/kaggle/how-propagate-2) |
+| Snapshots of propagation     | [![snapshots of the propagation - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/propagation-shots ) | [![The beauty of propagation - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)]( https://denmune.egy1st.org/kaggle/propagation-shots ) |
+| Scalability                  | [![Scalability - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/scalability ) | [![Scalability - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/scalability) |
+| Stability                    | [![Stability vs number of nearest neighbors - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/stability) | [![Stability - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/stability) |
+| k-nearest-evolution          | [![k-nearest-evolution - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/knn-evolution) | [![k-nearest-evolution - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)]( https://denmune.egy1st.org/kaggle/knn-evolution ) |
 
 
 
 ## How to cite
 If you have used this codebase in a scientific publication and wish to cite it, please use the [Journal of Pattern Recognition article](https://www.sciencedirect.com/science/article/abs/pii/S0031320320303927)
 
       Mohamed Abbas McInnes, Adel El-Zoghaby, Amin Ahoukry, *DenMune: Density peak based clustering using mutual nearest neighbors*
```

