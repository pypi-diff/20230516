# Comparing `tmp/denmune-1.16.2.tar.gz` & `tmp/denmune-1.16.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "denmune-1.16.2.tar", last modified: Mon May  1 19:38:54 2023, max compression
+gzip compressed data, was "denmune-1.16.3.tar", last modified: Tue May 16 13:52:20 2023, max compression
```

## Comparing `denmune-1.16.2.tar` & `denmune-1.16.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 19:38:54.192114 denmune-1.16.2/
--rw-rw-rw-   0        0        0     1498 2021-12-31 23:30:13.000000 denmune-1.16.2/LICENSE
--rw-rw-rw-   0        0        0       47 2021-12-27 21:52:58.000000 denmune-1.16.2/MANIFEST.in
--rw-rw-rw-   0        0        0    31656 2023-05-01 19:38:54.193118 denmune-1.16.2/PKG-INFO
--rw-rw-rw-   0        0        0    30985 2023-05-01 19:30:28.000000 denmune-1.16.2/README.md
--rw-rw-rw-   0        0        0      108 2021-12-23 20:19:35.000000 denmune-1.16.2/pyproject.toml
--rw-rw-rw-   0        0        0      810 2023-05-01 19:38:54.195117 denmune-1.16.2/setup.cfg
--rw-rw-rw-   0        0        0      257 2023-05-01 00:42:54.000000 denmune-1.16.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-01 19:38:54.137658 denmune-1.16.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-01 19:38:54.167116 denmune-1.16.2/src/denmune/
--rw-rw-rw-   0        0        0       28 2022-05-12 02:48:25.000000 denmune-1.16.2/src/denmune/__init__.py
--rw-rw-rw-   0        0        0    39240 2023-04-30 00:20:12.000000 denmune-1.16.2/src/denmune/denmune.py
-drwxrwxrwx   0        0        0        0 2023-05-01 19:38:54.186484 denmune-1.16.2/src/denmune.egg-info/
--rw-rw-rw-   0        0        0    31656 2023-05-01 19:38:54.000000 denmune-1.16.2/src/denmune.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2023-05-01 19:38:54.000000 denmune-1.16.2/src/denmune.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 19:38:54.000000 denmune-1.16.2/src/denmune.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      123 2023-05-01 19:38:54.000000 denmune-1.16.2/src/denmune.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-01 19:38:54.000000 denmune-1.16.2/src/denmune.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 13:52:20.308588 denmune-1.16.3/
+-rw-rw-rw-   0        0        0     1498 2021-12-31 23:30:13.000000 denmune-1.16.3/LICENSE
+-rw-rw-rw-   0        0        0       47 2021-12-27 21:52:58.000000 denmune-1.16.3/MANIFEST.in
+-rw-rw-rw-   0        0        0    29848 2023-05-16 13:52:20.310590 denmune-1.16.3/PKG-INFO
+-rw-rw-rw-   0        0        0    29177 2023-05-16 13:50:19.000000 denmune-1.16.3/README.md
+-rw-rw-rw-   0        0        0      108 2021-12-23 20:19:35.000000 denmune-1.16.3/pyproject.toml
+-rw-rw-rw-   0        0        0      810 2023-05-16 13:52:20.314794 denmune-1.16.3/setup.cfg
+-rw-rw-rw-   0        0        0      257 2023-05-16 13:50:59.000000 denmune-1.16.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 13:52:20.223706 denmune-1.16.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-16 13:52:20.277095 denmune-1.16.3/src/denmune/
+-rw-rw-rw-   0        0        0       28 2022-05-12 02:48:25.000000 denmune-1.16.3/src/denmune/__init__.py
+-rw-rw-rw-   0        0        0    39240 2023-04-30 00:20:12.000000 denmune-1.16.3/src/denmune/denmune.py
+drwxrwxrwx   0        0        0        0 2023-05-16 13:52:20.305583 denmune-1.16.3/src/denmune.egg-info/
+-rw-rw-rw-   0        0        0    29848 2023-05-16 13:52:20.000000 denmune-1.16.3/src/denmune.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2023-05-16 13:52:20.000000 denmune-1.16.3/src/denmune.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 13:52:20.000000 denmune-1.16.3/src/denmune.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      123 2023-05-16 13:52:20.000000 denmune-1.16.3/src/denmune.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-16 13:52:20.000000 denmune-1.16.3/src/denmune.egg-info/top_level.txt
```

### Comparing `denmune-1.16.2/LICENSE` & `denmune-1.16.3/LICENSE`

 * *Files identical despite different names*

### Comparing `denmune-1.16.2/PKG-INFO` & `denmune-1.16.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denmune
-Version: 1.16.2
+Version: 1.16.3
 Summary: This is the package for DenMune Clustering Algorithm published in paper https://doi.org/10.1016/j.patcog.2020.107589
 Home-page: https://github.com/scikit-learn-contrib/denmune-clustering-algorithm
 Author: Dr. Mohamed Ali Abbas & Prof. Amin  Shoukry
 Author-email: mohamed.alyabbas@outlook.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
@@ -12,99 +12,88 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # DenMune: A density-peak clustering algorithm
 DenMune is a clustering algorithm that can find clusters of arbitrary size, shapes and densities in two-dimensions. Higher dimensions are first reduced to 2-D using the t-sne. The algorithm relies on a single parameter K (the number of nearest neighbors). The results show the superiority of the algorithm. Enjoy the simplicity but the power of DenMune.
 
-
-
-Collaborative Test Drive (New)
-------------------------------
-
+## Reproducibility & Test Drives
 Now you can reproduce all the research experiments, and even share the results and collaborate to the algorithm using our capsule on CodeOcean. Each Capsule is a self-contained computational experiment with computing environment, code, data, version history, and results. 
 
-| Capsule URL                                   | Description                                     |
-| --------------------------------------------- | ----------------------------------------------- |
-| https://codeocean.com/capsule/3560333/tree/v1 | importing DenmUne from source code files        |
-| https://codeocean.com/capsule/3560333/tree/v2 | importing DenmUne after installing it using pip |
-
-
-
+also, you may use our repo2docker offered by mybinder.org, which encapsulate the algorithm and all required data in one virtual machine instance. All Jupyter notebooks examples found in this repository will be also available to you in action to practice in this respo2docer. Thanks mybinder.org, you made it possible!
 
-Scientific Work
----------------------
+| Test-drive                               | URL                                                          |
+| ---------------------------------------- | ------------------------------------------------------------ |
+| Reproduce our code capsule on Code Ocean | [![Open in Code Ocean](https://codeocean.com/codeocean-assets/badge/open-in-code-ocean.svg)](https://denmune.egy1st.org/codeocean-capsule) |
+| Use our test-drive on MyBinder           | [![Launch notebook examples in Binder](https://static.mybinder.org/badge_logo.svg)](https://denmune.egy1st.org/mybinder-repo2docker) |
 
+## Scientific Work
 | Paper                                                        | Journal                                                      | Data                                                         | ResearchGate stats                                           |
 | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
-| [![Elsevier, journal's article publisher ](https://img.shields.io/badge/elsevier-published-orange)](https://www.sciencedirect.com/science/article/abs/pii/S0031320320303927) | [![scimagojr](https://www.scimagojr.com/journal_img.php?id=24823)](https://www.scimagojr.com/journalsearch.php?q=24823&tip=sid&clean=0) | [![Research datasets at  Mendeley ](https://img.shields.io/badge/mendeley-data-bluegreen)](https://data.mendeley.com/datasets/b73cw5n43r/4) | ![Researchgate Stats](https://raw.githubusercontent.com/egy1st/images/main/clustering/researshgate.png) |
-
-Coding, Security & Maintenance
------------------------
+| [![Elsevier, journal's article publisher ](https://img.shields.io/badge/elsevier-published-orange)](https://denmune.egy1st.org/research-paper) | [![scimagojr](https://www.scimagojr.com/journal_img.php?id=24823)](https://www.scimagojr.com/journalsearch.php?q=24823&tip=sid&clean=0) | [![Research datasets at  Mendeley ](https://img.shields.io/badge/mendeley-data-bluegreen)]( https://denmune.egy1st.org/mendeley-data) | ![Researchgate Stats](https://raw.githubusercontent.com/egy1st/images/main/clustering/researshgate.png) |
 
+## Coding, Security & Maintenance
 | Code Style                                                   | Installation                                                 | CI Workflow                                                  | Code Coverage                                                | Code Scanning                                                |
 | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
 | ![Code Style: Black](https://img.shields.io/badge/code%20style-black-black) | [![PyPI Version](https://img.shields.io/pypi/v/denmune.svg)]( https://pypi.org/project/denmune/) | [![CircleCI, continuous integration](https://circleci.com/gh/egy1st/denmune-clustering-algorithm/tree/main.svg?style=shield)](https://circleci.com/gh/egy1st/denmune-clustering-algorithm/tree/main) | [![codecov](https://codecov.io/gh/egy1st/denmune-clustering-algorithm/branch/main/graph/badge.svg?token=QCbRdRtzYE)](https://codecov.io/gh/egy1st/denmune-clustering-algorithm) | [![CodeQL](https://github.com/adrinjalali/denmune-clustering-algorithm/actions/workflows/codeql.yml/badge.svg)](https://github.com/adrinjalali/denmune-clustering-algorithm/actions/workflows/codeql.yml) |
 
-Docs & Tutorials
-----------------------------
-
-| Read the Docs                                                | Repo2Docker                                                  | Colab                                                        | kaggle                                                       |
+## Tutorials
+| Reproducible Capsule                                         | Repo2Docker                                                  | Colab                                                        | kaggle                                                       |
 | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
-| [![Documentation Status](https://readthedocs.org/projects/denmune/badge/?version=latest)](https://denmune.readthedocs.io/en/latest/?badge=latest) | [![Launch notebook examples in Binder](https://static.mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/egy1st/denmune-clustering-algorithm/HEAD) | [![Launch notebook examples in Colaboratory, Google Research]( https://colab.research.google.com/assets/colab-badge.svg)](#colab) | [![Launch notebook examples in Kaggle, the workspace where data scientist meet](https://kaggle.com/static/images/open-in-kaggle.svg)](#kaggle) |
-
-Downloads Stats
---------------------
+| [![Open in Code Ocean](https://codeocean.com/codeocean-assets/badge/open-in-code-ocean.svg)](https://denmune.egy1st.org/codeocean-capsule) | [![Launch notebook examples in Binder](https://static.mybinder.org/badge_logo.svg)](https://denmune.egy1st.org/mybinder-repo2docker) | [![Launch notebook examples in Colaboratory, Google Research]( https://colab.research.google.com/assets/colab-badge.svg)](#colab) | [![Launch notebook examples in Kaggle, the workspace where data scientist meet](https://kaggle.com/static/images/open-in-kaggle.svg)](#kaggle) |
 
+## Downloads Stats
 | download/week                                                | download/month                                               | Total downloads                                              |
 | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
 | [![Downloads](https://static.pepy.tech/personalized-badge/denmune?period=week&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/denmune) | [![Downloads](https://static.pepy.tech/personalized-badge/denmune?period=month&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/denmune) | [![Downloads](https://static.pepy.tech/personalized-badge/denmune?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/denmune) |
 
-Based on the paper
--------------------
-
+## Based on the paper
 |Paper|
 |-------------------------------------------------------------------------------------------
 |Mohamed Abbas, Adel El-Zoghabi, Amin Shoukry,                                                                       
 |*DenMune: Density peak based clustering using mutual nearest neighbors*                                           
 |In: Journal of Pattern Recognition, Elsevier,                                                                 
 |volume 109, number 107589, January 2021                                                                      
 |DOI: https://doi.org/10.1016/j.patcog.2020.107589                                                 
 
-Documentation:
----------------
-
+## Documentation:
 Documentation, including tutorials, are available on:
    -  [![read the docs](https://img.shields.io/badge/read_the-docs-orange)](https://denmune.readthedocs.io/en/latest/?badge=latest)
-   -  [https://docs.zerobytes.one/](https://docs.zerobytes.one)
+   -  [![Read my docs](https://img.shields.io/badge/read_my-docs-green)](https://docs.egy1st.org)
 
 
-Watch it in action
--------------------
+
+## Watch it in action
 
 This 30 seconds will tell you how a density-based algorithm, DenMune propagates:
 
   [![interact with the propagation](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1o-tP3uvDGjxBOGYkir1lnbr74sZ06e0U?usp=sharing)
 
   [![Propagation in DenMune](https://raw.githubusercontent.com/egy1st/denmune-clustering-algorithm/main/images/propagation.gif)]()
 
+## Still interested?
+Watch this ***10-min*** illustrative video on Vimeo (no ads). Thank you Vimeo for making it possible without any distraction (No ads. We hate ads).
+
+- [![watch on Vimeo](https://img.shields.io/badge/watch_on-vimeo-green?style=for-the-badge)](https://player.vimeo.com/video/827209757)
+- [![YouTube Video Views](https://img.shields.io/youtube/views/o77raaasuOM?style=for-the-badge)](https://www.youtube.com/watch?v=o77raaasuOM) on Youtube
+
 
 
-When less means more
---------------------
+## When less means more
 
 Most classic clustering algorithms fail in detecting complex clusters where clusters are of different size, shape, density, and being exist in noisy data.
   Recently, a density-based algorithm named DenMune showed great ability in detecting complex shapes even in noisy data. it can detect number of clusters automatically, detect both pre-identified-noise and post-identified-noise automatically and removing them.
 
   It can achieve accuracy reach 100% in some classic pattern problems, achieve 97% in MNIST dataset. A great advantage of this algorithm is being single-parameter algorithm. All you need is to set number of k-nearest neighbor and the algorithm will care about the rest. Being Non-sensitive to changes in k, make it robust and stable.
 
   Keep in mind, the algorithm reduce any N-D dataset to only 2-D dataset initially, so it is a good benefit of this algorithm is being always to plot your data and explore it which make this algorithm a good candidate for data exploration. Finally, the algorithm comes with neat package for visualizing data, validating it and analyze the whole clustering process.
 
-How to install DenMune
-------------------------
+
+
+## How to install DenMune
 
 Simply install DenMune clustering algorithm using pip command from the official Python repository
 
   [![PyPI Version](https://img.shields.io/pypi/v/denmune.svg)]( https://pypi.org/project/denmune/)
 
   From the shell run the command
 
@@ -116,30 +105,27 @@
 
   ```ipython3
 !pip install denmune
   ```
 
 
 
-How to use  DenMune
---------------------
+## How to use  DenMune
 
 Once DenMune is installed, you just need to import it 
 
   ```python
 from denmune import DenMune
   ```
 
-  ###### Please note that first denmune (the package) in small letters, while the other one(the class itself) has D and M in capital case.
-
+*<u>Please note that first denmune (the package) in small letters, while the other one(the class itself) has D and M in capital case</u>.*
 
 
 
-Read data
------------
+## Read data
 
 There are four possible cases of data:
 
   - only train data without labels
   - only labeled train data
   - labeled train data in addition to test data without labels
   - labeled train data in addition to labeled test data
@@ -232,18 +218,18 @@
   ![pendigits train](https://raw.githubusercontent.com/egy1st/images/main/clustering/pendigits_50.png)
 
 test data as predicted by DenMune on training the dataset at k=50
 
   ![pendigits test](https://raw.githubusercontent.com/egy1st/images/main/clustering/pendigits_test_50.png)
 
 
-Algorithm's Parameters
------------------------
 
-    1. Parameters used within the initialization of the DenMune class
+## Algorithm's Parameters
+
+1. **Parameters used within the initialization of the DenMune class**
 
   ```python
 def __init__ (self,
                   train_data=None, test_data=None,
                   train_truth=None, test_truth=None, 
                   file_2d =None, k_nearest=None, 
                   rgn_tsne=False, prop_step=0,
@@ -286,18 +272,19 @@
     - default: None
 
   - prop_step:
 
     - size of increment used in showing the clustering propagation.
     - leave this parameter set to 0, the default value, unless you are willing intentionally to enter the propagation mode.
     - default: 0
+    
+    
 
-     
 
-    2. Parameters used within the fit_predict function:
+2. **Parameters used within the fit_predict function:**
 
   ```python
  def fit_predict(self,
                     validate=True,
                     show_plots=True,
                     show_noise=True, 
                     show_analyzer=True
@@ -316,27 +303,28 @@
     - show/hide noise and outlier
     - default: True
 
   - show_analyzer:
     - show/hide the analyzer
     - default: True
     
-    
 
-The Analyzer
--------------
+
+
+## The Analyzer
 
 The algorithm provide an exploratory tool called analyzer, once called it will provide you with in-depth analysis on how your clustering results perform.
 
   ![DenMune Analyzer](https://raw.githubusercontent.com/egy1st/images/main/clustering/analyzer.png)
 
-Noise Detection
-----------------
 
-  DenMune detects noise and outlier automatically, no need to any further work from your side.
+
+## Noise Detection
+
+DenMune detects noise and outlier automatically, no need to any further work from your side.
 
   - It plots pre-identified noise in black
   - It plots post-identified noise in light grey
 
   You can set show_noise parameter to False.
 
 
@@ -355,18 +343,18 @@
   ```
 
 | noisy data                                                   | clean data                                                   |
 | ------------------------------------------------------------ | ------------------------------------------------------------ |
 | ![noisy data](https://raw.githubusercontent.com/egy1st/images/main/clustering/noisy_data.png) | ![clean data](https://raw.githubusercontent.com/egy1st/images/main/clustering/clean_data.png) |
 
 
-Validation
---------------
 
-  You can get your validation results using 3 methods
+## Validation
+
+You can get your validation results using 3 methods
 
   - by showing the Analyzer
   - extract values from the validity returned list from fit_predict function
   - extract values from the Analyzer dictionary
     -
       There are  five validity measures built-in the algorithm, which are:
 
@@ -374,24 +362,25 @@
   - F1 score
   - NMI index (Normalized Mutual Information)
   - AMI index (Adjusted Mutual Information)
   - ARI index (Adjusted Rand Index)
 
   ![Validation snapshot](https://raw.githubusercontent.com/egy1st/images/main/clustering/validation.png) 
 
-K-nearest Evolution
--------------------
+
+
+## K-nearest Evolution
 
 The following chart shows the evolution of pre and post identified noise in correspondence to increase of number of knn. Also, detected number of clusters is analyzed in the same chart in relation with both types of identified  noise.
 
   ![knn evolution chart](https://raw.githubusercontent.com/egy1st/images/main/clustering/knn_vs_noise.png)
 
 
-The Scalability
-----------------
+
+## The Scalability
 
 | data size          | time                   |
 | ------------------ | ---------------------- |
 | data  size: 5000   | time: 2.3139 seconds   |
 | data  size: 10000  | time: 5.8752 seconds   |
 | data  size: 15000  | time: 12.4535 seconds  |
 | data  size: 20000  | time: 18.8466 seconds  |
@@ -406,27 +395,25 @@
 | data  size: 65000  | time: 149.1858 seconds |
 | data  size: 70000  | time: 177.4184 seconds |
 | data  size: 75000  | time: 204.0712 seconds |
 | data  size: 80000  | time: 220.502 seconds  |
 | data  size: 85000  | time: 251.7625 seconds |
 | data  size: 100000 | time: 257.563 seconds  |
 
-  | ![noisy data chart](https://raw.githubusercontent.com/egy1st/images/main/clustering/scalability.png)
-
+  |![noisy data chart](https://raw.githubusercontent.com/egy1st/images/main/clustering/scalability.png)
 
-The Stability
---------------
 
+## The Stability
   The algorithm is only single-parameter, even more it not sensitive to changes in that parameter, k. You may guess that from the following chart yourself. This is of great benefit for you as a data exploration analyst. You can simply explore the dataset using an arbitrary k. Being Non-sensitive to changes in k, make it robust and stable.
 
   ![DenMune Stability chart](https://raw.githubusercontent.com/egy1st/images/main/clustering/stability.png)
 
 
-Reveal the propagation
------------------------
+
+## Reveal the propagation
 
 one of the top performing feature in this algorithm is enabling you to watch how your clusters propagate to construct the final output clusters. just use the parameter 'prop_step' as in the following example:
 
   ```python
 dataset = "t7.10k" #
 data_path = 'datasets/denmune/chameleon/' 
 
@@ -449,92 +436,65 @@
     clear_output(wait=True)
     dm = DenMune(train_data=X_train, k_nearest=knn, rgn_tsne=False, prop_step=snapshot)
     labels, validity = dm.fit_predict(show_analyzer=False, show_noise=False)  
   ```
 
   [![Propagation in DenMune](https://raw.githubusercontent.com/egy1st/denmune-clustering-algorithm/main/images/propagation.gif)]()
 
-Interact with the algorithm
----------------------------
-
-  [![chameleon datasets](https://raw.githubusercontent.com/egy1st/denmune-clustering-algorithm/main/images/chameleon_detection.png)](https://colab.research.google.com/drive/1EUROd6TRwxW3A_XD3KTxL8miL2ias4Ue?usp=sharing)
-
-  This notebook allows you interact with the algorithm in many aspects:
-
-  - you can choose which dataset to cluster (among 4 chameleon datasets)
-  - you can decide which number of k-nearest neighbor to use 
-  - show noise on/off; thus you can invesetigate noise detected by the algorithm
-  - show analyzer on/off
 
 
-How to run and test
---------------------
+## Interact with the algorithm
 
-  1. Launch Examples in Repo2Docker Binder
+[![chameleon datasets](https://raw.githubusercontent.com/egy1st/denmune-clustering-algorithm/main/images/chameleon_detection.png)](https://colab.research.google.com/drive/1EUROd6TRwxW3A_XD3KTxL8miL2ias4Ue?usp=sharing)
 
-     Simply use our repo2docker offered by mybinder.org, which encapsulate the algorithm and all required data in one virtual machine instance. All Jupyter notebooks examples found in this repository will be also available to you in action to practice in this respo2docer. Thanks mybinder.org, you made it possible!
+*click image to interact* 
 
-     [![Launch notebook examples in Binder](https://static.mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/egy1st/denmune-clustering-algorithm/HEAD)
 
 
+ This notebook allows you interact with the algorithm in many aspects:
 
-  2. Launch each Example in Google Research, CoLab
-         
-     Need to test examples one by one, then here another option. Use colab offered by google research to test each example individually.
+  - you can choose which dataset to cluster (among 4 chameleon datasets)
+  - you can decide which number of k-nearest neighbor to use 
+  - show noise on/off; thus you can invesetigate noise detected by the algorithm
+  - show analyzer on/off
 
-     Here is a list of Google CoLab URL to use the algorithm interactively
-     ----------------------------------------------------------------------
 
 
-| Dataset                                          | CoLab URL                                                    |
-| ------------------------------------------------ | ------------------------------------------------------------ |
-| How to use it - colab                            | [![How to use it - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://colab.research.google.com/drive/1J_uKdhZ3z1KeY0-wJ7Ruw2PZSY1orKQm) |
-| Chameleon datasets - colab                       | [![Chameleon datasets - colab]( https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1EUROd6TRwxW3A_XD3KTxL8miL2ias4Ue?usp=sharing) |
-| 2D Shape datasets - colab                        | [![2D Shape datasets - colab]( https://colab.research.google.com/assets/colab-badge.svg)]( https://colab.research.google.com/drive/1EaqTPCRHSuTKB-qEbnWHpGKFj6XytMIk?usp=sharing) |
-| MNIST dataset - colab                            | [![MNIST dataset - colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1a9FGHRA6IPc5jhLOV46iEbpUeQXptSJp?usp=sharing) |
-| iris dataset - colab                             | [![iris dataset - colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1nKql57Xh7xVVu6NpTbg3vRdRg42R7hjm?usp=sharing) |
-| Get 97% by training MNIST dataset - colab        | [![Get 97% by training MNIST dataset - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://colab.research.google.com/drive/1NeOtXEQY94oD98Ufbh3IhTHnnYwIA659) |
-| Non-groundtruth datasets - colab                 | [![Non-groundtruth datasets - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://colab.research.google.com/drive/1d17ejQ83aUy0CZIeQ7bHTugSC9AjJ2mU?usp=sharing) |
-| Noise detection - colab                          | [![Noise detection - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://colab.research.google.com/drive/1Bp3c-cJfjLWxupmrBJ_6Q4-nqIfZcII4) |
-| Validation - colab                               | [![Validation - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://colab.research.google.com/drive/13_EVaQOv_QiNmQiMWJAcFFHPJHGCrQLe) |
-| How it propagates - colab                        | [![How it propagates - colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1o-tP3uvDGjxBOGYkir1lnbr74sZ06e0U?usp=sharing) |
-| Snapshots of propagation - colab                 | [![snapshots of the propagation - colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1vPXNKa8Rf3TnqDHSD3YSWl3g1iNSqjl2?usp=sharing) |
-| Scalability - colab                              | [![Scalability - colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1d55wkBndLLapO7Yx1ePHhE8mL61j9-TH?usp=sharing) |
-| Stability vs number of nearest neighbors - colab | [![Stability vs number of nearest neighbors - colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/17VgVRMFBWvkSIH1yA3tMl6UQ7Eu68K2l?usp=sharing) |
-| k-nearest-evolution - colab                      | [![k-nearest-evolution - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://colab.research.google.com/drive/1DZ-CQPV3WwJSiaV3-rjwPwmXw4RUh8Qj) |
+## We love Jupyter Notebooks
 
+Need to test examples one by one, then here other two options
 
+-  Use colab offered by google research to test each example individually.
+-  If you are a kaggler like me, then Kaggle, the best workspace where data scientist meet, should fit you to test the algorithm with great experience. 
 
-  3. Launch each Example in Kaggle workspace
 
-     If you are a kaggler like me, then Kaggle, the best workspace where data scientist meet, should fit you to test the algorithm with great experience. 
 
+Here is a list of Google CoLab & Kaggle notebooks  to practice the use of  the algorithm interactively.
 
-     | Dataset                                  | Kaggle URL                                                   |
-     | ---------------------------------------- | ------------------------------------------------------------ |
-     | When less means more - kaggle            | [![When less means more - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)]( https://www.kaggle.com/egyfirst/when-less-means-more) |
-     | Non-groundtruth datasets - kaggle        | [![Non-groundtruth datasets](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/egyfirst/detecting-non-groundtruth-datasets) |
-     | 2D Shape datasets - kaggle               | [![2D Shape datasets - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/egyfirst/detection-of-2d-shape-datasets) |
-     | MNIST dataset kaggle                     | [![MNIST dataset - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/egyfirst/get-97-using-simple-yet-one-parameter-algorithm) |
-     | Iris dataset kaggle                      | [![iris dataset - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/egyfirst/denmune-clustering-iris-dataset) |
-     | Training MNIST to get 97%                | [![Training MNIST to get 97%](https://kaggle.com/static/images/open-in-kaggle.svg)](  https://www.kaggle.com/egyfirst/training-mnist-dataset-to-get-97) |
-     | Noise detection - kaggle                 | [![Noise detection - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)]( https://www.kaggle.com/egyfirst/noise-detection) |
-     | Validation - kaggle                      | [![Validation - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/egyfirst/validate-in-5-built-in-validity-insexes) |
-     | The beauty of propagation - kaggle       | [![The beauty of propagation - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/egyfirst/the-beauty-of-clusters-propagation) |
-     | The beauty of propagation part2 - kaggle | [![The beauty of propagation part 2 - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/egyfirst/the-beauty-of-propagation-part2) |
-     | Snapshots of propagation -kaggle         | [![The beauty of propagation - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/egyfirst/beauty-of-propagation-part3) |
-     | Scalability kaggle                       | [![Scalability - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/egyfirst/scalability-vs-speed) |
-     | Stability - kaggle                       | [![Stability - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/egyfirst/stability-vs-number-of-nearest-neighbor) |
-     | k-nearest-evolution - kaggle             | [![k-nearest-evolution - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/egyfirst/k-nearest-evolution) |
 
+| Dataset                       | CoLab notebook                                               | Kaggle notebook                                              |
+| ----------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
+| How to use it?                | [![How to use it - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/how-to-use) | [![When less means more - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/how-to-use) |
+| Chameleon datasets            | [![Chameleon datasets - colab]( https://colab.research.google.com/assets/colab-badge.svg)](https://denmune.egy1st.org/colab/chameleon) | [![Non-groundtruth datasets](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/chameleon) |
+| 2D Shape datasets             | [![2D Shape datasets - colab]( https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/2d-shapes) | [![2D Shape datasets - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/2d-shapes) |
+| MNIST dataset                 | [![MNIST dataset - colab](https://colab.research.google.com/assets/colab-badge.svg)](https://denmune.egy1st.org/colab/mnist-dataset) | [![MNIST dataset - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/mnist-dataset) |
+| iris dataset                  | [![iris dataset - colab](https://colab.research.google.com/assets/colab-badge.svg)](https://denmune.egy1st.org/colab/iris-dataset) | [![iris dataset - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/iris-dataset) |
+| Scoring 97% on MNIST dataset  | [![Get 97% by training MNIST dataset - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/score-97-mnist) | [![Training MNIST to get 97%](https://kaggle.com/static/images/open-in-kaggle.svg)]( https://denmune.egy1st.org/kaggle/score-97-mnist) |
+| Clustering unlabeled datasets | [![Non-groundtruth datasets - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/unlabeled-data) | [![Non-groundtruth datasets](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/unlabeled-data) |
+| Noise detection               | [![Noise detection - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/noise-detection ) | [![Noise detection - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)]( https://denmune.egy1st.org/kaggle/noise-detection) |
+| Validation                    | [![Validation - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/how-to-validate ) | [![Validation - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)]( https://denmune.egy1st.org/kaggle/how-to-validate) |
+| How does it propagate?        | [![How it propagates - colab](https://colab.research.google.com/assets/colab-badge.svg)](https://denmune.egy1st.org/colab/how-propagate ) | [![The beauty of propagation - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)]( https://denmune.egy1st.org/kaggle/how-propagate) <br />[![The beauty of propagation part 2 - kaggle]( https://kaggle.com/static/images/open-in-kaggle.svg)]( https://denmune.egy1st.org/kaggle/how-propagate-2) |
+| Snapshots of propagation      | [![snapshots of the propagation - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/propagation-shots ) | [![The beauty of propagation - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)]( https://denmune.egy1st.org/kaggle/propagation-shots ) |
+| Scalability                   | [![Scalability - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/scalability ) | [![Scalability - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/scalability) |
+| Stability                     | [![Stability vs number of nearest neighbors - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/stability) | [![Stability - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/stability) |
+| k-nearest-evolution           | [![k-nearest-evolution - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/knn-evolution) | [![k-nearest-evolution - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)]( https://denmune.egy1st.org/kaggle/knn-evolution ) |
 
 
-How to cite
-------------
 
+## How to cite
 If you have used this codebase in a scientific publication and wish to cite it, please use the [Journal of Pattern Recognition article](https://www.sciencedirect.com/science/article/abs/pii/S0031320320303927)
 
       Mohamed Abbas McInnes, Adel El-Zoghaby, Amin Ahoukry, *DenMune: Density peak based clustering using mutual nearest neighbors*
       In: Journal of Pattern Recognition, Elsevier, volume 109, number 107589.
       January 2021
 
 
@@ -552,32 +512,28 @@
 keywords = {Clustering, Mutual neighbors, Dimensionality reduction, Arbitrary shapes, Pattern recognition, Nearest neighbors, Density peak},
 abstract = {Many clustering algorithms fail when clusters are of arbitrary shapes, of varying densities, or the data classes are unbalanced and close to each other, even in two dimensions. A novel clustering algorithm “DenMune” is presented to meet this challenge. It is based on identifying dense regions using mutual nearest neighborhoods of size K, where K is the only parameter required from the user, besides obeying the mutual nearest neighbor consistency principle. The algorithm is stable for a wide range of values of K. Moreover, it is able to automatically detect and remove noise from the clustering process as well as detecting the target clusters. It produces robust results on various low and high dimensional datasets relative to several known state of the art clustering algorithms.}
 }
   ```
 
 
 
-Licensing
-------------
-
+## Licensing
 The DenMune algorithm is 3-clause BSD licensed. Enjoy.
 
  [![BSD 3-Clause “New” or “Revised” License" ](https://img.shields.io/badge/license-BSD-green)](https://choosealicense.com/licenses/bsd-3-clause/)
 
 
 
-Task List
-------------
-
+## Task List
   - [x] Update Github with the DenMune sourcecode
   - [x] create repo2docker repository
   - [x] Create pip Package
   - [x] create CoLab shared examples
   - [x] create documentation
   - [x] create Kaggle shared examples
   - [x] PEP8 compliant
   - [x] Continuous integration
   - [x] scikit-learn compatible
   - [x] creating unit tests (coverage: 100%)
   - [x] generating API documentation
   - [x] create reproducible capsule on codeocean
-  - [ ] create conda package
+  - [ ] create conda package (*postponed untill NGT has conda installation*)
```

### Comparing `denmune-1.16.2/README.md` & `denmune-1.16.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,95 +1,84 @@
 # DenMune: A density-peak clustering algorithm
 DenMune is a clustering algorithm that can find clusters of arbitrary size, shapes and densities in two-dimensions. Higher dimensions are first reduced to 2-D using the t-sne. The algorithm relies on a single parameter K (the number of nearest neighbors). The results show the superiority of the algorithm. Enjoy the simplicity but the power of DenMune.
 
-
-
-Collaborative Test Drive (New)
-------------------------------
-
+## Reproducibility & Test Drives
 Now you can reproduce all the research experiments, and even share the results and collaborate to the algorithm using our capsule on CodeOcean. Each Capsule is a self-contained computational experiment with computing environment, code, data, version history, and results. 
 
-| Capsule URL                                   | Description                                     |
-| --------------------------------------------- | ----------------------------------------------- |
-| https://codeocean.com/capsule/3560333/tree/v1 | importing DenmUne from source code files        |
-| https://codeocean.com/capsule/3560333/tree/v2 | importing DenmUne after installing it using pip |
-
-
-
+also, you may use our repo2docker offered by mybinder.org, which encapsulate the algorithm and all required data in one virtual machine instance. All Jupyter notebooks examples found in this repository will be also available to you in action to practice in this respo2docer. Thanks mybinder.org, you made it possible!
 
-Scientific Work
----------------------
+| Test-drive                               | URL                                                          |
+| ---------------------------------------- | ------------------------------------------------------------ |
+| Reproduce our code capsule on Code Ocean | [![Open in Code Ocean](https://codeocean.com/codeocean-assets/badge/open-in-code-ocean.svg)](https://denmune.egy1st.org/codeocean-capsule) |
+| Use our test-drive on MyBinder           | [![Launch notebook examples in Binder](https://static.mybinder.org/badge_logo.svg)](https://denmune.egy1st.org/mybinder-repo2docker) |
 
+## Scientific Work
 | Paper                                                        | Journal                                                      | Data                                                         | ResearchGate stats                                           |
 | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
-| [![Elsevier, journal's article publisher ](https://img.shields.io/badge/elsevier-published-orange)](https://www.sciencedirect.com/science/article/abs/pii/S0031320320303927) | [![scimagojr](https://www.scimagojr.com/journal_img.php?id=24823)](https://www.scimagojr.com/journalsearch.php?q=24823&tip=sid&clean=0) | [![Research datasets at  Mendeley ](https://img.shields.io/badge/mendeley-data-bluegreen)](https://data.mendeley.com/datasets/b73cw5n43r/4) | ![Researchgate Stats](https://raw.githubusercontent.com/egy1st/images/main/clustering/researshgate.png) |
-
-Coding, Security & Maintenance
------------------------
+| [![Elsevier, journal's article publisher ](https://img.shields.io/badge/elsevier-published-orange)](https://denmune.egy1st.org/research-paper) | [![scimagojr](https://www.scimagojr.com/journal_img.php?id=24823)](https://www.scimagojr.com/journalsearch.php?q=24823&tip=sid&clean=0) | [![Research datasets at  Mendeley ](https://img.shields.io/badge/mendeley-data-bluegreen)]( https://denmune.egy1st.org/mendeley-data) | ![Researchgate Stats](https://raw.githubusercontent.com/egy1st/images/main/clustering/researshgate.png) |
 
+## Coding, Security & Maintenance
 | Code Style                                                   | Installation                                                 | CI Workflow                                                  | Code Coverage                                                | Code Scanning                                                |
 | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
 | ![Code Style: Black](https://img.shields.io/badge/code%20style-black-black) | [![PyPI Version](https://img.shields.io/pypi/v/denmune.svg)]( https://pypi.org/project/denmune/) | [![CircleCI, continuous integration](https://circleci.com/gh/egy1st/denmune-clustering-algorithm/tree/main.svg?style=shield)](https://circleci.com/gh/egy1st/denmune-clustering-algorithm/tree/main) | [![codecov](https://codecov.io/gh/egy1st/denmune-clustering-algorithm/branch/main/graph/badge.svg?token=QCbRdRtzYE)](https://codecov.io/gh/egy1st/denmune-clustering-algorithm) | [![CodeQL](https://github.com/adrinjalali/denmune-clustering-algorithm/actions/workflows/codeql.yml/badge.svg)](https://github.com/adrinjalali/denmune-clustering-algorithm/actions/workflows/codeql.yml) |
 
-Docs & Tutorials
-----------------------------
-
-| Read the Docs                                                | Repo2Docker                                                  | Colab                                                        | kaggle                                                       |
+## Tutorials
+| Reproducible Capsule                                         | Repo2Docker                                                  | Colab                                                        | kaggle                                                       |
 | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
-| [![Documentation Status](https://readthedocs.org/projects/denmune/badge/?version=latest)](https://denmune.readthedocs.io/en/latest/?badge=latest) | [![Launch notebook examples in Binder](https://static.mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/egy1st/denmune-clustering-algorithm/HEAD) | [![Launch notebook examples in Colaboratory, Google Research]( https://colab.research.google.com/assets/colab-badge.svg)](#colab) | [![Launch notebook examples in Kaggle, the workspace where data scientist meet](https://kaggle.com/static/images/open-in-kaggle.svg)](#kaggle) |
-
-Downloads Stats
---------------------
+| [![Open in Code Ocean](https://codeocean.com/codeocean-assets/badge/open-in-code-ocean.svg)](https://denmune.egy1st.org/codeocean-capsule) | [![Launch notebook examples in Binder](https://static.mybinder.org/badge_logo.svg)](https://denmune.egy1st.org/mybinder-repo2docker) | [![Launch notebook examples in Colaboratory, Google Research]( https://colab.research.google.com/assets/colab-badge.svg)](#colab) | [![Launch notebook examples in Kaggle, the workspace where data scientist meet](https://kaggle.com/static/images/open-in-kaggle.svg)](#kaggle) |
 
+## Downloads Stats
 | download/week                                                | download/month                                               | Total downloads                                              |
 | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
 | [![Downloads](https://static.pepy.tech/personalized-badge/denmune?period=week&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/denmune) | [![Downloads](https://static.pepy.tech/personalized-badge/denmune?period=month&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/denmune) | [![Downloads](https://static.pepy.tech/personalized-badge/denmune?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/denmune) |
 
-Based on the paper
--------------------
-
+## Based on the paper
 |Paper|
 |-------------------------------------------------------------------------------------------
 |Mohamed Abbas, Adel El-Zoghabi, Amin Shoukry,                                                                       
 |*DenMune: Density peak based clustering using mutual nearest neighbors*                                           
 |In: Journal of Pattern Recognition, Elsevier,                                                                 
 |volume 109, number 107589, January 2021                                                                      
 |DOI: https://doi.org/10.1016/j.patcog.2020.107589                                                 
 
-Documentation:
----------------
-
+## Documentation:
 Documentation, including tutorials, are available on:
    -  [![read the docs](https://img.shields.io/badge/read_the-docs-orange)](https://denmune.readthedocs.io/en/latest/?badge=latest)
-   -  [https://docs.zerobytes.one/](https://docs.zerobytes.one)
+   -  [![Read my docs](https://img.shields.io/badge/read_my-docs-green)](https://docs.egy1st.org)
 
 
-Watch it in action
--------------------
+
+## Watch it in action
 
 This 30 seconds will tell you how a density-based algorithm, DenMune propagates:
 
   [![interact with the propagation](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1o-tP3uvDGjxBOGYkir1lnbr74sZ06e0U?usp=sharing)
 
   [![Propagation in DenMune](https://raw.githubusercontent.com/egy1st/denmune-clustering-algorithm/main/images/propagation.gif)]()
 
+## Still interested?
+Watch this ***10-min*** illustrative video on Vimeo (no ads). Thank you Vimeo for making it possible without any distraction (No ads. We hate ads).
+
+- [![watch on Vimeo](https://img.shields.io/badge/watch_on-vimeo-green?style=for-the-badge)](https://player.vimeo.com/video/827209757)
+- [![YouTube Video Views](https://img.shields.io/youtube/views/o77raaasuOM?style=for-the-badge)](https://www.youtube.com/watch?v=o77raaasuOM) on Youtube
+
 
 
-When less means more
---------------------
+## When less means more
 
 Most classic clustering algorithms fail in detecting complex clusters where clusters are of different size, shape, density, and being exist in noisy data.
   Recently, a density-based algorithm named DenMune showed great ability in detecting complex shapes even in noisy data. it can detect number of clusters automatically, detect both pre-identified-noise and post-identified-noise automatically and removing them.
 
   It can achieve accuracy reach 100% in some classic pattern problems, achieve 97% in MNIST dataset. A great advantage of this algorithm is being single-parameter algorithm. All you need is to set number of k-nearest neighbor and the algorithm will care about the rest. Being Non-sensitive to changes in k, make it robust and stable.
 
   Keep in mind, the algorithm reduce any N-D dataset to only 2-D dataset initially, so it is a good benefit of this algorithm is being always to plot your data and explore it which make this algorithm a good candidate for data exploration. Finally, the algorithm comes with neat package for visualizing data, validating it and analyze the whole clustering process.
 
-How to install DenMune
-------------------------
+
+
+## How to install DenMune
 
 Simply install DenMune clustering algorithm using pip command from the official Python repository
 
   [![PyPI Version](https://img.shields.io/pypi/v/denmune.svg)]( https://pypi.org/project/denmune/)
 
   From the shell run the command
 
@@ -101,30 +90,27 @@
 
   ```ipython3
 !pip install denmune
   ```
 
 
 
-How to use  DenMune
---------------------
+## How to use  DenMune
 
 Once DenMune is installed, you just need to import it 
 
   ```python
 from denmune import DenMune
   ```
 
-  ###### Please note that first denmune (the package) in small letters, while the other one(the class itself) has D and M in capital case.
-
+*<u>Please note that first denmune (the package) in small letters, while the other one(the class itself) has D and M in capital case</u>.*
 
 
 
-Read data
------------
+## Read data
 
 There are four possible cases of data:
 
   - only train data without labels
   - only labeled train data
   - labeled train data in addition to test data without labels
   - labeled train data in addition to labeled test data
@@ -217,18 +203,18 @@
   ![pendigits train](https://raw.githubusercontent.com/egy1st/images/main/clustering/pendigits_50.png)
 
 test data as predicted by DenMune on training the dataset at k=50
 
   ![pendigits test](https://raw.githubusercontent.com/egy1st/images/main/clustering/pendigits_test_50.png)
 
 
-Algorithm's Parameters
------------------------
 
-    1. Parameters used within the initialization of the DenMune class
+## Algorithm's Parameters
+
+1. **Parameters used within the initialization of the DenMune class**
 
   ```python
 def __init__ (self,
                   train_data=None, test_data=None,
                   train_truth=None, test_truth=None, 
                   file_2d =None, k_nearest=None, 
                   rgn_tsne=False, prop_step=0,
@@ -271,18 +257,19 @@
     - default: None
 
   - prop_step:
 
     - size of increment used in showing the clustering propagation.
     - leave this parameter set to 0, the default value, unless you are willing intentionally to enter the propagation mode.
     - default: 0
+    
+    
 
-     
 
-    2. Parameters used within the fit_predict function:
+2. **Parameters used within the fit_predict function:**
 
   ```python
  def fit_predict(self,
                     validate=True,
                     show_plots=True,
                     show_noise=True, 
                     show_analyzer=True
@@ -301,27 +288,28 @@
     - show/hide noise and outlier
     - default: True
 
   - show_analyzer:
     - show/hide the analyzer
     - default: True
     
-    
 
-The Analyzer
--------------
+
+
+## The Analyzer
 
 The algorithm provide an exploratory tool called analyzer, once called it will provide you with in-depth analysis on how your clustering results perform.
 
   ![DenMune Analyzer](https://raw.githubusercontent.com/egy1st/images/main/clustering/analyzer.png)
 
-Noise Detection
-----------------
 
-  DenMune detects noise and outlier automatically, no need to any further work from your side.
+
+## Noise Detection
+
+DenMune detects noise and outlier automatically, no need to any further work from your side.
 
   - It plots pre-identified noise in black
   - It plots post-identified noise in light grey
 
   You can set show_noise parameter to False.
 
 
@@ -340,18 +328,18 @@
   ```
 
 | noisy data                                                   | clean data                                                   |
 | ------------------------------------------------------------ | ------------------------------------------------------------ |
 | ![noisy data](https://raw.githubusercontent.com/egy1st/images/main/clustering/noisy_data.png) | ![clean data](https://raw.githubusercontent.com/egy1st/images/main/clustering/clean_data.png) |
 
 
-Validation
---------------
 
-  You can get your validation results using 3 methods
+## Validation
+
+You can get your validation results using 3 methods
 
   - by showing the Analyzer
   - extract values from the validity returned list from fit_predict function
   - extract values from the Analyzer dictionary
     -
       There are  five validity measures built-in the algorithm, which are:
 
@@ -359,24 +347,25 @@
   - F1 score
   - NMI index (Normalized Mutual Information)
   - AMI index (Adjusted Mutual Information)
   - ARI index (Adjusted Rand Index)
 
   ![Validation snapshot](https://raw.githubusercontent.com/egy1st/images/main/clustering/validation.png) 
 
-K-nearest Evolution
--------------------
+
+
+## K-nearest Evolution
 
 The following chart shows the evolution of pre and post identified noise in correspondence to increase of number of knn. Also, detected number of clusters is analyzed in the same chart in relation with both types of identified  noise.
 
   ![knn evolution chart](https://raw.githubusercontent.com/egy1st/images/main/clustering/knn_vs_noise.png)
 
 
-The Scalability
-----------------
+
+## The Scalability
 
 | data size          | time                   |
 | ------------------ | ---------------------- |
 | data  size: 5000   | time: 2.3139 seconds   |
 | data  size: 10000  | time: 5.8752 seconds   |
 | data  size: 15000  | time: 12.4535 seconds  |
 | data  size: 20000  | time: 18.8466 seconds  |
@@ -391,27 +380,25 @@
 | data  size: 65000  | time: 149.1858 seconds |
 | data  size: 70000  | time: 177.4184 seconds |
 | data  size: 75000  | time: 204.0712 seconds |
 | data  size: 80000  | time: 220.502 seconds  |
 | data  size: 85000  | time: 251.7625 seconds |
 | data  size: 100000 | time: 257.563 seconds  |
 
-  | ![noisy data chart](https://raw.githubusercontent.com/egy1st/images/main/clustering/scalability.png)
-
+  |![noisy data chart](https://raw.githubusercontent.com/egy1st/images/main/clustering/scalability.png)
 
-The Stability
---------------
 
+## The Stability
   The algorithm is only single-parameter, even more it not sensitive to changes in that parameter, k. You may guess that from the following chart yourself. This is of great benefit for you as a data exploration analyst. You can simply explore the dataset using an arbitrary k. Being Non-sensitive to changes in k, make it robust and stable.
 
   ![DenMune Stability chart](https://raw.githubusercontent.com/egy1st/images/main/clustering/stability.png)
 
 
-Reveal the propagation
------------------------
+
+## Reveal the propagation
 
 one of the top performing feature in this algorithm is enabling you to watch how your clusters propagate to construct the final output clusters. just use the parameter 'prop_step' as in the following example:
 
   ```python
 dataset = "t7.10k" #
 data_path = 'datasets/denmune/chameleon/' 
 
@@ -434,92 +421,65 @@
     clear_output(wait=True)
     dm = DenMune(train_data=X_train, k_nearest=knn, rgn_tsne=False, prop_step=snapshot)
     labels, validity = dm.fit_predict(show_analyzer=False, show_noise=False)  
   ```
 
   [![Propagation in DenMune](https://raw.githubusercontent.com/egy1st/denmune-clustering-algorithm/main/images/propagation.gif)]()
 
-Interact with the algorithm
----------------------------
-
-  [![chameleon datasets](https://raw.githubusercontent.com/egy1st/denmune-clustering-algorithm/main/images/chameleon_detection.png)](https://colab.research.google.com/drive/1EUROd6TRwxW3A_XD3KTxL8miL2ias4Ue?usp=sharing)
-
-  This notebook allows you interact with the algorithm in many aspects:
-
-  - you can choose which dataset to cluster (among 4 chameleon datasets)
-  - you can decide which number of k-nearest neighbor to use 
-  - show noise on/off; thus you can invesetigate noise detected by the algorithm
-  - show analyzer on/off
 
 
-How to run and test
---------------------
+## Interact with the algorithm
 
-  1. Launch Examples in Repo2Docker Binder
+[![chameleon datasets](https://raw.githubusercontent.com/egy1st/denmune-clustering-algorithm/main/images/chameleon_detection.png)](https://colab.research.google.com/drive/1EUROd6TRwxW3A_XD3KTxL8miL2ias4Ue?usp=sharing)
 
-     Simply use our repo2docker offered by mybinder.org, which encapsulate the algorithm and all required data in one virtual machine instance. All Jupyter notebooks examples found in this repository will be also available to you in action to practice in this respo2docer. Thanks mybinder.org, you made it possible!
+*click image to interact* 
 
-     [![Launch notebook examples in Binder](https://static.mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/egy1st/denmune-clustering-algorithm/HEAD)
 
 
+ This notebook allows you interact with the algorithm in many aspects:
 
-  2. Launch each Example in Google Research, CoLab
-         
-     Need to test examples one by one, then here another option. Use colab offered by google research to test each example individually.
+  - you can choose which dataset to cluster (among 4 chameleon datasets)
+  - you can decide which number of k-nearest neighbor to use 
+  - show noise on/off; thus you can invesetigate noise detected by the algorithm
+  - show analyzer on/off
 
-     Here is a list of Google CoLab URL to use the algorithm interactively
-     ----------------------------------------------------------------------
 
 
-| Dataset                                          | CoLab URL                                                    |
-| ------------------------------------------------ | ------------------------------------------------------------ |
-| How to use it - colab                            | [![How to use it - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://colab.research.google.com/drive/1J_uKdhZ3z1KeY0-wJ7Ruw2PZSY1orKQm) |
-| Chameleon datasets - colab                       | [![Chameleon datasets - colab]( https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1EUROd6TRwxW3A_XD3KTxL8miL2ias4Ue?usp=sharing) |
-| 2D Shape datasets - colab                        | [![2D Shape datasets - colab]( https://colab.research.google.com/assets/colab-badge.svg)]( https://colab.research.google.com/drive/1EaqTPCRHSuTKB-qEbnWHpGKFj6XytMIk?usp=sharing) |
-| MNIST dataset - colab                            | [![MNIST dataset - colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1a9FGHRA6IPc5jhLOV46iEbpUeQXptSJp?usp=sharing) |
-| iris dataset - colab                             | [![iris dataset - colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1nKql57Xh7xVVu6NpTbg3vRdRg42R7hjm?usp=sharing) |
-| Get 97% by training MNIST dataset - colab        | [![Get 97% by training MNIST dataset - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://colab.research.google.com/drive/1NeOtXEQY94oD98Ufbh3IhTHnnYwIA659) |
-| Non-groundtruth datasets - colab                 | [![Non-groundtruth datasets - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://colab.research.google.com/drive/1d17ejQ83aUy0CZIeQ7bHTugSC9AjJ2mU?usp=sharing) |
-| Noise detection - colab                          | [![Noise detection - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://colab.research.google.com/drive/1Bp3c-cJfjLWxupmrBJ_6Q4-nqIfZcII4) |
-| Validation - colab                               | [![Validation - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://colab.research.google.com/drive/13_EVaQOv_QiNmQiMWJAcFFHPJHGCrQLe) |
-| How it propagates - colab                        | [![How it propagates - colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1o-tP3uvDGjxBOGYkir1lnbr74sZ06e0U?usp=sharing) |
-| Snapshots of propagation - colab                 | [![snapshots of the propagation - colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1vPXNKa8Rf3TnqDHSD3YSWl3g1iNSqjl2?usp=sharing) |
-| Scalability - colab                              | [![Scalability - colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1d55wkBndLLapO7Yx1ePHhE8mL61j9-TH?usp=sharing) |
-| Stability vs number of nearest neighbors - colab | [![Stability vs number of nearest neighbors - colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/17VgVRMFBWvkSIH1yA3tMl6UQ7Eu68K2l?usp=sharing) |
-| k-nearest-evolution - colab                      | [![k-nearest-evolution - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://colab.research.google.com/drive/1DZ-CQPV3WwJSiaV3-rjwPwmXw4RUh8Qj) |
+## We love Jupyter Notebooks
 
+Need to test examples one by one, then here other two options
 
+-  Use colab offered by google research to test each example individually.
+-  If you are a kaggler like me, then Kaggle, the best workspace where data scientist meet, should fit you to test the algorithm with great experience. 
 
-  3. Launch each Example in Kaggle workspace
 
-     If you are a kaggler like me, then Kaggle, the best workspace where data scientist meet, should fit you to test the algorithm with great experience. 
 
+Here is a list of Google CoLab & Kaggle notebooks  to practice the use of  the algorithm interactively.
 
-     | Dataset                                  | Kaggle URL                                                   |
-     | ---------------------------------------- | ------------------------------------------------------------ |
-     | When less means more - kaggle            | [![When less means more - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)]( https://www.kaggle.com/egyfirst/when-less-means-more) |
-     | Non-groundtruth datasets - kaggle        | [![Non-groundtruth datasets](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/egyfirst/detecting-non-groundtruth-datasets) |
-     | 2D Shape datasets - kaggle               | [![2D Shape datasets - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/egyfirst/detection-of-2d-shape-datasets) |
-     | MNIST dataset kaggle                     | [![MNIST dataset - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/egyfirst/get-97-using-simple-yet-one-parameter-algorithm) |
-     | Iris dataset kaggle                      | [![iris dataset - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/egyfirst/denmune-clustering-iris-dataset) |
-     | Training MNIST to get 97%                | [![Training MNIST to get 97%](https://kaggle.com/static/images/open-in-kaggle.svg)](  https://www.kaggle.com/egyfirst/training-mnist-dataset-to-get-97) |
-     | Noise detection - kaggle                 | [![Noise detection - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)]( https://www.kaggle.com/egyfirst/noise-detection) |
-     | Validation - kaggle                      | [![Validation - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/egyfirst/validate-in-5-built-in-validity-insexes) |
-     | The beauty of propagation - kaggle       | [![The beauty of propagation - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/egyfirst/the-beauty-of-clusters-propagation) |
-     | The beauty of propagation part2 - kaggle | [![The beauty of propagation part 2 - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/egyfirst/the-beauty-of-propagation-part2) |
-     | Snapshots of propagation -kaggle         | [![The beauty of propagation - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/egyfirst/beauty-of-propagation-part3) |
-     | Scalability kaggle                       | [![Scalability - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/egyfirst/scalability-vs-speed) |
-     | Stability - kaggle                       | [![Stability - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/egyfirst/stability-vs-number-of-nearest-neighbor) |
-     | k-nearest-evolution - kaggle             | [![k-nearest-evolution - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/egyfirst/k-nearest-evolution) |
 
+| Dataset                       | CoLab notebook                                               | Kaggle notebook                                              |
+| ----------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
+| How to use it?                | [![How to use it - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/how-to-use) | [![When less means more - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/how-to-use) |
+| Chameleon datasets            | [![Chameleon datasets - colab]( https://colab.research.google.com/assets/colab-badge.svg)](https://denmune.egy1st.org/colab/chameleon) | [![Non-groundtruth datasets](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/chameleon) |
+| 2D Shape datasets             | [![2D Shape datasets - colab]( https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/2d-shapes) | [![2D Shape datasets - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/2d-shapes) |
+| MNIST dataset                 | [![MNIST dataset - colab](https://colab.research.google.com/assets/colab-badge.svg)](https://denmune.egy1st.org/colab/mnist-dataset) | [![MNIST dataset - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/mnist-dataset) |
+| iris dataset                  | [![iris dataset - colab](https://colab.research.google.com/assets/colab-badge.svg)](https://denmune.egy1st.org/colab/iris-dataset) | [![iris dataset - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/iris-dataset) |
+| Scoring 97% on MNIST dataset  | [![Get 97% by training MNIST dataset - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/score-97-mnist) | [![Training MNIST to get 97%](https://kaggle.com/static/images/open-in-kaggle.svg)]( https://denmune.egy1st.org/kaggle/score-97-mnist) |
+| Clustering unlabeled datasets | [![Non-groundtruth datasets - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/unlabeled-data) | [![Non-groundtruth datasets](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/unlabeled-data) |
+| Noise detection               | [![Noise detection - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/noise-detection ) | [![Noise detection - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)]( https://denmune.egy1st.org/kaggle/noise-detection) |
+| Validation                    | [![Validation - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/how-to-validate ) | [![Validation - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)]( https://denmune.egy1st.org/kaggle/how-to-validate) |
+| How does it propagate?        | [![How it propagates - colab](https://colab.research.google.com/assets/colab-badge.svg)](https://denmune.egy1st.org/colab/how-propagate ) | [![The beauty of propagation - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)]( https://denmune.egy1st.org/kaggle/how-propagate) <br />[![The beauty of propagation part 2 - kaggle]( https://kaggle.com/static/images/open-in-kaggle.svg)]( https://denmune.egy1st.org/kaggle/how-propagate-2) |
+| Snapshots of propagation      | [![snapshots of the propagation - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/propagation-shots ) | [![The beauty of propagation - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)]( https://denmune.egy1st.org/kaggle/propagation-shots ) |
+| Scalability                   | [![Scalability - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/scalability ) | [![Scalability - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/scalability) |
+| Stability                     | [![Stability vs number of nearest neighbors - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/stability) | [![Stability - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/stability) |
+| k-nearest-evolution           | [![k-nearest-evolution - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/knn-evolution) | [![k-nearest-evolution - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)]( https://denmune.egy1st.org/kaggle/knn-evolution ) |
 
 
-How to cite
-------------
 
+## How to cite
 If you have used this codebase in a scientific publication and wish to cite it, please use the [Journal of Pattern Recognition article](https://www.sciencedirect.com/science/article/abs/pii/S0031320320303927)
 
       Mohamed Abbas McInnes, Adel El-Zoghaby, Amin Ahoukry, *DenMune: Density peak based clustering using mutual nearest neighbors*
       In: Journal of Pattern Recognition, Elsevier, volume 109, number 107589.
       January 2021
 
 
@@ -537,32 +497,28 @@
 keywords = {Clustering, Mutual neighbors, Dimensionality reduction, Arbitrary shapes, Pattern recognition, Nearest neighbors, Density peak},
 abstract = {Many clustering algorithms fail when clusters are of arbitrary shapes, of varying densities, or the data classes are unbalanced and close to each other, even in two dimensions. A novel clustering algorithm “DenMune” is presented to meet this challenge. It is based on identifying dense regions using mutual nearest neighborhoods of size K, where K is the only parameter required from the user, besides obeying the mutual nearest neighbor consistency principle. The algorithm is stable for a wide range of values of K. Moreover, it is able to automatically detect and remove noise from the clustering process as well as detecting the target clusters. It produces robust results on various low and high dimensional datasets relative to several known state of the art clustering algorithms.}
 }
   ```
 
 
 
-Licensing
-------------
-
+## Licensing
 The DenMune algorithm is 3-clause BSD licensed. Enjoy.
 
  [![BSD 3-Clause “New” or “Revised” License" ](https://img.shields.io/badge/license-BSD-green)](https://choosealicense.com/licenses/bsd-3-clause/)
 
 
 
-Task List
-------------
-
+## Task List
   - [x] Update Github with the DenMune sourcecode
   - [x] create repo2docker repository
   - [x] Create pip Package
   - [x] create CoLab shared examples
   - [x] create documentation
   - [x] create Kaggle shared examples
   - [x] PEP8 compliant
   - [x] Continuous integration
   - [x] scikit-learn compatible
   - [x] creating unit tests (coverage: 100%)
   - [x] generating API documentation
   - [x] create reproducible capsule on codeocean
-  - [ ] create conda package
+  - [ ] create conda package (*postponed untill NGT has conda installation*)
```

### Comparing `denmune-1.16.2/setup.cfg` & `denmune-1.16.3/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 656e 6d75 6e65 0d0a 7665 7273   = denmune..vers
-00000020: 696f 6e20 3d20 312e 3136 2e32 0d0a 6175  ion = 1.16.2..au
+00000020: 696f 6e20 3d20 312e 3136 2e33 0d0a 6175  ion = 1.16.3..au
 00000030: 7468 6f72 203d 2044 722e 204d 6f68 616d  thor = Dr. Moham
 00000040: 6564 2041 6c69 2041 6262 6173 2026 2050  ed Ali Abbas & P
 00000050: 726f 662e 2041 6d69 6e20 2053 686f 756b  rof. Amin  Shouk
 00000060: 7279 0d0a 6175 7468 6f72 5f65 6d61 696c  ry..author_email
 00000070: 203d 206d 6f68 616d 6564 2e61 6c79 6162   = mohamed.alyab
 00000080: 6261 7340 6f75 746c 6f6f 6b2e 636f 6d0d  bas@outlook.com.
 00000090: 0a64 6573 6372 6970 7469 6f6e 203d 2054  .description = T
```

### Comparing `denmune-1.16.2/src/denmune/denmune.py` & `denmune-1.16.3/src/denmune/denmune.py`

 * *Files identical despite different names*

### Comparing `denmune-1.16.2/src/denmune.egg-info/PKG-INFO` & `denmune-1.16.3/src/denmune.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denmune
-Version: 1.16.2
+Version: 1.16.3
 Summary: This is the package for DenMune Clustering Algorithm published in paper https://doi.org/10.1016/j.patcog.2020.107589
 Home-page: https://github.com/scikit-learn-contrib/denmune-clustering-algorithm
 Author: Dr. Mohamed Ali Abbas & Prof. Amin  Shoukry
 Author-email: mohamed.alyabbas@outlook.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
@@ -12,99 +12,88 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # DenMune: A density-peak clustering algorithm
 DenMune is a clustering algorithm that can find clusters of arbitrary size, shapes and densities in two-dimensions. Higher dimensions are first reduced to 2-D using the t-sne. The algorithm relies on a single parameter K (the number of nearest neighbors). The results show the superiority of the algorithm. Enjoy the simplicity but the power of DenMune.
 
-
-
-Collaborative Test Drive (New)
-------------------------------
-
+## Reproducibility & Test Drives
 Now you can reproduce all the research experiments, and even share the results and collaborate to the algorithm using our capsule on CodeOcean. Each Capsule is a self-contained computational experiment with computing environment, code, data, version history, and results. 
 
-| Capsule URL                                   | Description                                     |
-| --------------------------------------------- | ----------------------------------------------- |
-| https://codeocean.com/capsule/3560333/tree/v1 | importing DenmUne from source code files        |
-| https://codeocean.com/capsule/3560333/tree/v2 | importing DenmUne after installing it using pip |
-
-
-
+also, you may use our repo2docker offered by mybinder.org, which encapsulate the algorithm and all required data in one virtual machine instance. All Jupyter notebooks examples found in this repository will be also available to you in action to practice in this respo2docer. Thanks mybinder.org, you made it possible!
 
-Scientific Work
----------------------
+| Test-drive                               | URL                                                          |
+| ---------------------------------------- | ------------------------------------------------------------ |
+| Reproduce our code capsule on Code Ocean | [![Open in Code Ocean](https://codeocean.com/codeocean-assets/badge/open-in-code-ocean.svg)](https://denmune.egy1st.org/codeocean-capsule) |
+| Use our test-drive on MyBinder           | [![Launch notebook examples in Binder](https://static.mybinder.org/badge_logo.svg)](https://denmune.egy1st.org/mybinder-repo2docker) |
 
+## Scientific Work
 | Paper                                                        | Journal                                                      | Data                                                         | ResearchGate stats                                           |
 | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
-| [![Elsevier, journal's article publisher ](https://img.shields.io/badge/elsevier-published-orange)](https://www.sciencedirect.com/science/article/abs/pii/S0031320320303927) | [![scimagojr](https://www.scimagojr.com/journal_img.php?id=24823)](https://www.scimagojr.com/journalsearch.php?q=24823&tip=sid&clean=0) | [![Research datasets at  Mendeley ](https://img.shields.io/badge/mendeley-data-bluegreen)](https://data.mendeley.com/datasets/b73cw5n43r/4) | ![Researchgate Stats](https://raw.githubusercontent.com/egy1st/images/main/clustering/researshgate.png) |
-
-Coding, Security & Maintenance
------------------------
+| [![Elsevier, journal's article publisher ](https://img.shields.io/badge/elsevier-published-orange)](https://denmune.egy1st.org/research-paper) | [![scimagojr](https://www.scimagojr.com/journal_img.php?id=24823)](https://www.scimagojr.com/journalsearch.php?q=24823&tip=sid&clean=0) | [![Research datasets at  Mendeley ](https://img.shields.io/badge/mendeley-data-bluegreen)]( https://denmune.egy1st.org/mendeley-data) | ![Researchgate Stats](https://raw.githubusercontent.com/egy1st/images/main/clustering/researshgate.png) |
 
+## Coding, Security & Maintenance
 | Code Style                                                   | Installation                                                 | CI Workflow                                                  | Code Coverage                                                | Code Scanning                                                |
 | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
 | ![Code Style: Black](https://img.shields.io/badge/code%20style-black-black) | [![PyPI Version](https://img.shields.io/pypi/v/denmune.svg)]( https://pypi.org/project/denmune/) | [![CircleCI, continuous integration](https://circleci.com/gh/egy1st/denmune-clustering-algorithm/tree/main.svg?style=shield)](https://circleci.com/gh/egy1st/denmune-clustering-algorithm/tree/main) | [![codecov](https://codecov.io/gh/egy1st/denmune-clustering-algorithm/branch/main/graph/badge.svg?token=QCbRdRtzYE)](https://codecov.io/gh/egy1st/denmune-clustering-algorithm) | [![CodeQL](https://github.com/adrinjalali/denmune-clustering-algorithm/actions/workflows/codeql.yml/badge.svg)](https://github.com/adrinjalali/denmune-clustering-algorithm/actions/workflows/codeql.yml) |
 
-Docs & Tutorials
-----------------------------
-
-| Read the Docs                                                | Repo2Docker                                                  | Colab                                                        | kaggle                                                       |
+## Tutorials
+| Reproducible Capsule                                         | Repo2Docker                                                  | Colab                                                        | kaggle                                                       |
 | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
-| [![Documentation Status](https://readthedocs.org/projects/denmune/badge/?version=latest)](https://denmune.readthedocs.io/en/latest/?badge=latest) | [![Launch notebook examples in Binder](https://static.mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/egy1st/denmune-clustering-algorithm/HEAD) | [![Launch notebook examples in Colaboratory, Google Research]( https://colab.research.google.com/assets/colab-badge.svg)](#colab) | [![Launch notebook examples in Kaggle, the workspace where data scientist meet](https://kaggle.com/static/images/open-in-kaggle.svg)](#kaggle) |
-
-Downloads Stats
---------------------
+| [![Open in Code Ocean](https://codeocean.com/codeocean-assets/badge/open-in-code-ocean.svg)](https://denmune.egy1st.org/codeocean-capsule) | [![Launch notebook examples in Binder](https://static.mybinder.org/badge_logo.svg)](https://denmune.egy1st.org/mybinder-repo2docker) | [![Launch notebook examples in Colaboratory, Google Research]( https://colab.research.google.com/assets/colab-badge.svg)](#colab) | [![Launch notebook examples in Kaggle, the workspace where data scientist meet](https://kaggle.com/static/images/open-in-kaggle.svg)](#kaggle) |
 
+## Downloads Stats
 | download/week                                                | download/month                                               | Total downloads                                              |
 | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
 | [![Downloads](https://static.pepy.tech/personalized-badge/denmune?period=week&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/denmune) | [![Downloads](https://static.pepy.tech/personalized-badge/denmune?period=month&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/denmune) | [![Downloads](https://static.pepy.tech/personalized-badge/denmune?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/denmune) |
 
-Based on the paper
--------------------
-
+## Based on the paper
 |Paper|
 |-------------------------------------------------------------------------------------------
 |Mohamed Abbas, Adel El-Zoghabi, Amin Shoukry,                                                                       
 |*DenMune: Density peak based clustering using mutual nearest neighbors*                                           
 |In: Journal of Pattern Recognition, Elsevier,                                                                 
 |volume 109, number 107589, January 2021                                                                      
 |DOI: https://doi.org/10.1016/j.patcog.2020.107589                                                 
 
-Documentation:
----------------
-
+## Documentation:
 Documentation, including tutorials, are available on:
    -  [![read the docs](https://img.shields.io/badge/read_the-docs-orange)](https://denmune.readthedocs.io/en/latest/?badge=latest)
-   -  [https://docs.zerobytes.one/](https://docs.zerobytes.one)
+   -  [![Read my docs](https://img.shields.io/badge/read_my-docs-green)](https://docs.egy1st.org)
 
 
-Watch it in action
--------------------
+
+## Watch it in action
 
 This 30 seconds will tell you how a density-based algorithm, DenMune propagates:
 
   [![interact with the propagation](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1o-tP3uvDGjxBOGYkir1lnbr74sZ06e0U?usp=sharing)
 
   [![Propagation in DenMune](https://raw.githubusercontent.com/egy1st/denmune-clustering-algorithm/main/images/propagation.gif)]()
 
+## Still interested?
+Watch this ***10-min*** illustrative video on Vimeo (no ads). Thank you Vimeo for making it possible without any distraction (No ads. We hate ads).
+
+- [![watch on Vimeo](https://img.shields.io/badge/watch_on-vimeo-green?style=for-the-badge)](https://player.vimeo.com/video/827209757)
+- [![YouTube Video Views](https://img.shields.io/youtube/views/o77raaasuOM?style=for-the-badge)](https://www.youtube.com/watch?v=o77raaasuOM) on Youtube
+
 
 
-When less means more
---------------------
+## When less means more
 
 Most classic clustering algorithms fail in detecting complex clusters where clusters are of different size, shape, density, and being exist in noisy data.
   Recently, a density-based algorithm named DenMune showed great ability in detecting complex shapes even in noisy data. it can detect number of clusters automatically, detect both pre-identified-noise and post-identified-noise automatically and removing them.
 
   It can achieve accuracy reach 100% in some classic pattern problems, achieve 97% in MNIST dataset. A great advantage of this algorithm is being single-parameter algorithm. All you need is to set number of k-nearest neighbor and the algorithm will care about the rest. Being Non-sensitive to changes in k, make it robust and stable.
 
   Keep in mind, the algorithm reduce any N-D dataset to only 2-D dataset initially, so it is a good benefit of this algorithm is being always to plot your data and explore it which make this algorithm a good candidate for data exploration. Finally, the algorithm comes with neat package for visualizing data, validating it and analyze the whole clustering process.
 
-How to install DenMune
-------------------------
+
+
+## How to install DenMune
 
 Simply install DenMune clustering algorithm using pip command from the official Python repository
 
   [![PyPI Version](https://img.shields.io/pypi/v/denmune.svg)]( https://pypi.org/project/denmune/)
 
   From the shell run the command
 
@@ -116,30 +105,27 @@
 
   ```ipython3
 !pip install denmune
   ```
 
 
 
-How to use  DenMune
---------------------
+## How to use  DenMune
 
 Once DenMune is installed, you just need to import it 
 
   ```python
 from denmune import DenMune
   ```
 
-  ###### Please note that first denmune (the package) in small letters, while the other one(the class itself) has D and M in capital case.
-
+*<u>Please note that first denmune (the package) in small letters, while the other one(the class itself) has D and M in capital case</u>.*
 
 
 
-Read data
------------
+## Read data
 
 There are four possible cases of data:
 
   - only train data without labels
   - only labeled train data
   - labeled train data in addition to test data without labels
   - labeled train data in addition to labeled test data
@@ -232,18 +218,18 @@
   ![pendigits train](https://raw.githubusercontent.com/egy1st/images/main/clustering/pendigits_50.png)
 
 test data as predicted by DenMune on training the dataset at k=50
 
   ![pendigits test](https://raw.githubusercontent.com/egy1st/images/main/clustering/pendigits_test_50.png)
 
 
-Algorithm's Parameters
------------------------
 
-    1. Parameters used within the initialization of the DenMune class
+## Algorithm's Parameters
+
+1. **Parameters used within the initialization of the DenMune class**
 
   ```python
 def __init__ (self,
                   train_data=None, test_data=None,
                   train_truth=None, test_truth=None, 
                   file_2d =None, k_nearest=None, 
                   rgn_tsne=False, prop_step=0,
@@ -286,18 +272,19 @@
     - default: None
 
   - prop_step:
 
     - size of increment used in showing the clustering propagation.
     - leave this parameter set to 0, the default value, unless you are willing intentionally to enter the propagation mode.
     - default: 0
+    
+    
 
-     
 
-    2. Parameters used within the fit_predict function:
+2. **Parameters used within the fit_predict function:**
 
   ```python
  def fit_predict(self,
                     validate=True,
                     show_plots=True,
                     show_noise=True, 
                     show_analyzer=True
@@ -316,27 +303,28 @@
     - show/hide noise and outlier
     - default: True
 
   - show_analyzer:
     - show/hide the analyzer
     - default: True
     
-    
 
-The Analyzer
--------------
+
+
+## The Analyzer
 
 The algorithm provide an exploratory tool called analyzer, once called it will provide you with in-depth analysis on how your clustering results perform.
 
   ![DenMune Analyzer](https://raw.githubusercontent.com/egy1st/images/main/clustering/analyzer.png)
 
-Noise Detection
-----------------
 
-  DenMune detects noise and outlier automatically, no need to any further work from your side.
+
+## Noise Detection
+
+DenMune detects noise and outlier automatically, no need to any further work from your side.
 
   - It plots pre-identified noise in black
   - It plots post-identified noise in light grey
 
   You can set show_noise parameter to False.
 
 
@@ -355,18 +343,18 @@
   ```
 
 | noisy data                                                   | clean data                                                   |
 | ------------------------------------------------------------ | ------------------------------------------------------------ |
 | ![noisy data](https://raw.githubusercontent.com/egy1st/images/main/clustering/noisy_data.png) | ![clean data](https://raw.githubusercontent.com/egy1st/images/main/clustering/clean_data.png) |
 
 
-Validation
---------------
 
-  You can get your validation results using 3 methods
+## Validation
+
+You can get your validation results using 3 methods
 
   - by showing the Analyzer
   - extract values from the validity returned list from fit_predict function
   - extract values from the Analyzer dictionary
     -
       There are  five validity measures built-in the algorithm, which are:
 
@@ -374,24 +362,25 @@
   - F1 score
   - NMI index (Normalized Mutual Information)
   - AMI index (Adjusted Mutual Information)
   - ARI index (Adjusted Rand Index)
 
   ![Validation snapshot](https://raw.githubusercontent.com/egy1st/images/main/clustering/validation.png) 
 
-K-nearest Evolution
--------------------
+
+
+## K-nearest Evolution
 
 The following chart shows the evolution of pre and post identified noise in correspondence to increase of number of knn. Also, detected number of clusters is analyzed in the same chart in relation with both types of identified  noise.
 
   ![knn evolution chart](https://raw.githubusercontent.com/egy1st/images/main/clustering/knn_vs_noise.png)
 
 
-The Scalability
-----------------
+
+## The Scalability
 
 | data size          | time                   |
 | ------------------ | ---------------------- |
 | data  size: 5000   | time: 2.3139 seconds   |
 | data  size: 10000  | time: 5.8752 seconds   |
 | data  size: 15000  | time: 12.4535 seconds  |
 | data  size: 20000  | time: 18.8466 seconds  |
@@ -406,27 +395,25 @@
 | data  size: 65000  | time: 149.1858 seconds |
 | data  size: 70000  | time: 177.4184 seconds |
 | data  size: 75000  | time: 204.0712 seconds |
 | data  size: 80000  | time: 220.502 seconds  |
 | data  size: 85000  | time: 251.7625 seconds |
 | data  size: 100000 | time: 257.563 seconds  |
 
-  | ![noisy data chart](https://raw.githubusercontent.com/egy1st/images/main/clustering/scalability.png)
-
+  |![noisy data chart](https://raw.githubusercontent.com/egy1st/images/main/clustering/scalability.png)
 
-The Stability
---------------
 
+## The Stability
   The algorithm is only single-parameter, even more it not sensitive to changes in that parameter, k. You may guess that from the following chart yourself. This is of great benefit for you as a data exploration analyst. You can simply explore the dataset using an arbitrary k. Being Non-sensitive to changes in k, make it robust and stable.
 
   ![DenMune Stability chart](https://raw.githubusercontent.com/egy1st/images/main/clustering/stability.png)
 
 
-Reveal the propagation
------------------------
+
+## Reveal the propagation
 
 one of the top performing feature in this algorithm is enabling you to watch how your clusters propagate to construct the final output clusters. just use the parameter 'prop_step' as in the following example:
 
   ```python
 dataset = "t7.10k" #
 data_path = 'datasets/denmune/chameleon/' 
 
@@ -449,92 +436,65 @@
     clear_output(wait=True)
     dm = DenMune(train_data=X_train, k_nearest=knn, rgn_tsne=False, prop_step=snapshot)
     labels, validity = dm.fit_predict(show_analyzer=False, show_noise=False)  
   ```
 
   [![Propagation in DenMune](https://raw.githubusercontent.com/egy1st/denmune-clustering-algorithm/main/images/propagation.gif)]()
 
-Interact with the algorithm
----------------------------
-
-  [![chameleon datasets](https://raw.githubusercontent.com/egy1st/denmune-clustering-algorithm/main/images/chameleon_detection.png)](https://colab.research.google.com/drive/1EUROd6TRwxW3A_XD3KTxL8miL2ias4Ue?usp=sharing)
-
-  This notebook allows you interact with the algorithm in many aspects:
-
-  - you can choose which dataset to cluster (among 4 chameleon datasets)
-  - you can decide which number of k-nearest neighbor to use 
-  - show noise on/off; thus you can invesetigate noise detected by the algorithm
-  - show analyzer on/off
 
 
-How to run and test
---------------------
+## Interact with the algorithm
 
-  1. Launch Examples in Repo2Docker Binder
+[![chameleon datasets](https://raw.githubusercontent.com/egy1st/denmune-clustering-algorithm/main/images/chameleon_detection.png)](https://colab.research.google.com/drive/1EUROd6TRwxW3A_XD3KTxL8miL2ias4Ue?usp=sharing)
 
-     Simply use our repo2docker offered by mybinder.org, which encapsulate the algorithm and all required data in one virtual machine instance. All Jupyter notebooks examples found in this repository will be also available to you in action to practice in this respo2docer. Thanks mybinder.org, you made it possible!
+*click image to interact* 
 
-     [![Launch notebook examples in Binder](https://static.mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/egy1st/denmune-clustering-algorithm/HEAD)
 
 
+ This notebook allows you interact with the algorithm in many aspects:
 
-  2. Launch each Example in Google Research, CoLab
-         
-     Need to test examples one by one, then here another option. Use colab offered by google research to test each example individually.
+  - you can choose which dataset to cluster (among 4 chameleon datasets)
+  - you can decide which number of k-nearest neighbor to use 
+  - show noise on/off; thus you can invesetigate noise detected by the algorithm
+  - show analyzer on/off
 
-     Here is a list of Google CoLab URL to use the algorithm interactively
-     ----------------------------------------------------------------------
 
 
-| Dataset                                          | CoLab URL                                                    |
-| ------------------------------------------------ | ------------------------------------------------------------ |
-| How to use it - colab                            | [![How to use it - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://colab.research.google.com/drive/1J_uKdhZ3z1KeY0-wJ7Ruw2PZSY1orKQm) |
-| Chameleon datasets - colab                       | [![Chameleon datasets - colab]( https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1EUROd6TRwxW3A_XD3KTxL8miL2ias4Ue?usp=sharing) |
-| 2D Shape datasets - colab                        | [![2D Shape datasets - colab]( https://colab.research.google.com/assets/colab-badge.svg)]( https://colab.research.google.com/drive/1EaqTPCRHSuTKB-qEbnWHpGKFj6XytMIk?usp=sharing) |
-| MNIST dataset - colab                            | [![MNIST dataset - colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1a9FGHRA6IPc5jhLOV46iEbpUeQXptSJp?usp=sharing) |
-| iris dataset - colab                             | [![iris dataset - colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1nKql57Xh7xVVu6NpTbg3vRdRg42R7hjm?usp=sharing) |
-| Get 97% by training MNIST dataset - colab        | [![Get 97% by training MNIST dataset - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://colab.research.google.com/drive/1NeOtXEQY94oD98Ufbh3IhTHnnYwIA659) |
-| Non-groundtruth datasets - colab                 | [![Non-groundtruth datasets - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://colab.research.google.com/drive/1d17ejQ83aUy0CZIeQ7bHTugSC9AjJ2mU?usp=sharing) |
-| Noise detection - colab                          | [![Noise detection - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://colab.research.google.com/drive/1Bp3c-cJfjLWxupmrBJ_6Q4-nqIfZcII4) |
-| Validation - colab                               | [![Validation - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://colab.research.google.com/drive/13_EVaQOv_QiNmQiMWJAcFFHPJHGCrQLe) |
-| How it propagates - colab                        | [![How it propagates - colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1o-tP3uvDGjxBOGYkir1lnbr74sZ06e0U?usp=sharing) |
-| Snapshots of propagation - colab                 | [![snapshots of the propagation - colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1vPXNKa8Rf3TnqDHSD3YSWl3g1iNSqjl2?usp=sharing) |
-| Scalability - colab                              | [![Scalability - colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1d55wkBndLLapO7Yx1ePHhE8mL61j9-TH?usp=sharing) |
-| Stability vs number of nearest neighbors - colab | [![Stability vs number of nearest neighbors - colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/17VgVRMFBWvkSIH1yA3tMl6UQ7Eu68K2l?usp=sharing) |
-| k-nearest-evolution - colab                      | [![k-nearest-evolution - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://colab.research.google.com/drive/1DZ-CQPV3WwJSiaV3-rjwPwmXw4RUh8Qj) |
+## We love Jupyter Notebooks
 
+Need to test examples one by one, then here other two options
 
+-  Use colab offered by google research to test each example individually.
+-  If you are a kaggler like me, then Kaggle, the best workspace where data scientist meet, should fit you to test the algorithm with great experience. 
 
-  3. Launch each Example in Kaggle workspace
 
-     If you are a kaggler like me, then Kaggle, the best workspace where data scientist meet, should fit you to test the algorithm with great experience. 
 
+Here is a list of Google CoLab & Kaggle notebooks  to practice the use of  the algorithm interactively.
 
-     | Dataset                                  | Kaggle URL                                                   |
-     | ---------------------------------------- | ------------------------------------------------------------ |
-     | When less means more - kaggle            | [![When less means more - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)]( https://www.kaggle.com/egyfirst/when-less-means-more) |
-     | Non-groundtruth datasets - kaggle        | [![Non-groundtruth datasets](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/egyfirst/detecting-non-groundtruth-datasets) |
-     | 2D Shape datasets - kaggle               | [![2D Shape datasets - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/egyfirst/detection-of-2d-shape-datasets) |
-     | MNIST dataset kaggle                     | [![MNIST dataset - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/egyfirst/get-97-using-simple-yet-one-parameter-algorithm) |
-     | Iris dataset kaggle                      | [![iris dataset - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/egyfirst/denmune-clustering-iris-dataset) |
-     | Training MNIST to get 97%                | [![Training MNIST to get 97%](https://kaggle.com/static/images/open-in-kaggle.svg)](  https://www.kaggle.com/egyfirst/training-mnist-dataset-to-get-97) |
-     | Noise detection - kaggle                 | [![Noise detection - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)]( https://www.kaggle.com/egyfirst/noise-detection) |
-     | Validation - kaggle                      | [![Validation - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/egyfirst/validate-in-5-built-in-validity-insexes) |
-     | The beauty of propagation - kaggle       | [![The beauty of propagation - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/egyfirst/the-beauty-of-clusters-propagation) |
-     | The beauty of propagation part2 - kaggle | [![The beauty of propagation part 2 - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/egyfirst/the-beauty-of-propagation-part2) |
-     | Snapshots of propagation -kaggle         | [![The beauty of propagation - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/egyfirst/beauty-of-propagation-part3) |
-     | Scalability kaggle                       | [![Scalability - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/egyfirst/scalability-vs-speed) |
-     | Stability - kaggle                       | [![Stability - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/egyfirst/stability-vs-number-of-nearest-neighbor) |
-     | k-nearest-evolution - kaggle             | [![k-nearest-evolution - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/egyfirst/k-nearest-evolution) |
 
+| Dataset                       | CoLab notebook                                               | Kaggle notebook                                              |
+| ----------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
+| How to use it?                | [![How to use it - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/how-to-use) | [![When less means more - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/how-to-use) |
+| Chameleon datasets            | [![Chameleon datasets - colab]( https://colab.research.google.com/assets/colab-badge.svg)](https://denmune.egy1st.org/colab/chameleon) | [![Non-groundtruth datasets](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/chameleon) |
+| 2D Shape datasets             | [![2D Shape datasets - colab]( https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/2d-shapes) | [![2D Shape datasets - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/2d-shapes) |
+| MNIST dataset                 | [![MNIST dataset - colab](https://colab.research.google.com/assets/colab-badge.svg)](https://denmune.egy1st.org/colab/mnist-dataset) | [![MNIST dataset - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/mnist-dataset) |
+| iris dataset                  | [![iris dataset - colab](https://colab.research.google.com/assets/colab-badge.svg)](https://denmune.egy1st.org/colab/iris-dataset) | [![iris dataset - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/iris-dataset) |
+| Scoring 97% on MNIST dataset  | [![Get 97% by training MNIST dataset - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/score-97-mnist) | [![Training MNIST to get 97%](https://kaggle.com/static/images/open-in-kaggle.svg)]( https://denmune.egy1st.org/kaggle/score-97-mnist) |
+| Clustering unlabeled datasets | [![Non-groundtruth datasets - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/unlabeled-data) | [![Non-groundtruth datasets](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/unlabeled-data) |
+| Noise detection               | [![Noise detection - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/noise-detection ) | [![Noise detection - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)]( https://denmune.egy1st.org/kaggle/noise-detection) |
+| Validation                    | [![Validation - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/how-to-validate ) | [![Validation - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)]( https://denmune.egy1st.org/kaggle/how-to-validate) |
+| How does it propagate?        | [![How it propagates - colab](https://colab.research.google.com/assets/colab-badge.svg)](https://denmune.egy1st.org/colab/how-propagate ) | [![The beauty of propagation - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)]( https://denmune.egy1st.org/kaggle/how-propagate) <br />[![The beauty of propagation part 2 - kaggle]( https://kaggle.com/static/images/open-in-kaggle.svg)]( https://denmune.egy1st.org/kaggle/how-propagate-2) |
+| Snapshots of propagation      | [![snapshots of the propagation - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/propagation-shots ) | [![The beauty of propagation - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)]( https://denmune.egy1st.org/kaggle/propagation-shots ) |
+| Scalability                   | [![Scalability - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/scalability ) | [![Scalability - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/scalability) |
+| Stability                     | [![Stability vs number of nearest neighbors - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/stability) | [![Stability - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://denmune.egy1st.org/kaggle/stability) |
+| k-nearest-evolution           | [![k-nearest-evolution - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://denmune.egy1st.org/colab/knn-evolution) | [![k-nearest-evolution - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)]( https://denmune.egy1st.org/kaggle/knn-evolution ) |
 
 
-How to cite
-------------
 
+## How to cite
 If you have used this codebase in a scientific publication and wish to cite it, please use the [Journal of Pattern Recognition article](https://www.sciencedirect.com/science/article/abs/pii/S0031320320303927)
 
       Mohamed Abbas McInnes, Adel El-Zoghaby, Amin Ahoukry, *DenMune: Density peak based clustering using mutual nearest neighbors*
       In: Journal of Pattern Recognition, Elsevier, volume 109, number 107589.
       January 2021
 
 
@@ -552,32 +512,28 @@
 keywords = {Clustering, Mutual neighbors, Dimensionality reduction, Arbitrary shapes, Pattern recognition, Nearest neighbors, Density peak},
 abstract = {Many clustering algorithms fail when clusters are of arbitrary shapes, of varying densities, or the data classes are unbalanced and close to each other, even in two dimensions. A novel clustering algorithm “DenMune” is presented to meet this challenge. It is based on identifying dense regions using mutual nearest neighborhoods of size K, where K is the only parameter required from the user, besides obeying the mutual nearest neighbor consistency principle. The algorithm is stable for a wide range of values of K. Moreover, it is able to automatically detect and remove noise from the clustering process as well as detecting the target clusters. It produces robust results on various low and high dimensional datasets relative to several known state of the art clustering algorithms.}
 }
   ```
 
 
 
-Licensing
-------------
-
+## Licensing
 The DenMune algorithm is 3-clause BSD licensed. Enjoy.
 
  [![BSD 3-Clause “New” or “Revised” License" ](https://img.shields.io/badge/license-BSD-green)](https://choosealicense.com/licenses/bsd-3-clause/)
 
 
 
-Task List
-------------
-
+## Task List
   - [x] Update Github with the DenMune sourcecode
   - [x] create repo2docker repository
   - [x] Create pip Package
   - [x] create CoLab shared examples
   - [x] create documentation
   - [x] create Kaggle shared examples
   - [x] PEP8 compliant
   - [x] Continuous integration
   - [x] scikit-learn compatible
   - [x] creating unit tests (coverage: 100%)
   - [x] generating API documentation
   - [x] create reproducible capsule on codeocean
-  - [ ] create conda package
+  - [ ] create conda package (*postponed untill NGT has conda installation*)
```

