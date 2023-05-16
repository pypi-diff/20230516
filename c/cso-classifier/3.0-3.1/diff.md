# Comparing `tmp/cso-classifier-3.0.tar.gz` & `tmp/cso-classifier-3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/aas358/Development/CSO Classifier Versioning/going to version 3.0/to_publish/cso-classifier/dist/tmpyii9wvd9/cso-classif", last modified: Tue Jul 13 16:31:58 2021, max compression
+gzip compressed data, was "/data/user-data/aas358/test_cso/cso-classifier/dist/.tmp-hc1mgb5a/cso-classifier-3.1.tar", last modified: Tue May 16 11:50:42 2023, max compression
```

## Comparing `cso-classifier-3.0.tar` & `cso-classifier-3.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 aas358   (1141393362) OPEN-UNIVERSITY\Domain Users (1182653967)        0 2021-07-13 16:31:58.000000 cso-classifier-3.0/
--rw-r--r--   0 aas358   (1141393362) OPEN-UNIVERSITY\Domain Users (1182653967)    11385 2021-07-13 16:00:10.000000 cso-classifier-3.0/LICENSE
--rw-r--r--   0 aas358   (1141393362) OPEN-UNIVERSITY\Domain Users (1182653967)       42 2021-07-13 16:00:10.000000 cso-classifier-3.0/MANIFEST.in
--rw-r--r--   0 aas358   (1141393362) OPEN-UNIVERSITY\Domain Users (1182653967)    41377 2021-07-13 16:31:58.000000 cso-classifier-3.0/PKG-INFO
--rw-r--r--   0 aas358   (1141393362) OPEN-UNIVERSITY\Domain Users (1182653967)    40755 2021-07-13 16:00:10.000000 cso-classifier-3.0/README.md
-drwxr-xr-x   0 aas358   (1141393362) OPEN-UNIVERSITY\Domain Users (1182653967)        0 2021-07-13 16:31:58.000000 cso-classifier-3.0/cso_classifier/
--rw-r--r--   0 aas358   (1141393362) OPEN-UNIVERSITY\Domain Users (1182653967)      462 2021-07-13 16:00:10.000000 cso-classifier-3.0/cso_classifier/__init__.py
-drwxr-xr-x   0 aas358   (1141393362) OPEN-UNIVERSITY\Domain Users (1182653967)        0 2021-07-13 16:31:58.000000 cso-classifier-3.0/cso_classifier/assets/
--rw-r--r--   0 aas358   (1141393362) OPEN-UNIVERSITY\Domain Users (1182653967)     1845 2021-07-13 16:00:10.000000 cso-classifier-3.0/cso_classifier/assets/README.md
--rw-r--r--   0 aas358   (1141393362) OPEN-UNIVERSITY\Domain Users (1182653967)    12906 2021-07-13 16:00:10.000000 cso-classifier-3.0/cso_classifier/classifier.py
--rw-r--r--   0 aas358   (1141393362) OPEN-UNIVERSITY\Domain Users (1182653967)      574 2021-07-13 16:00:10.000000 cso-classifier-3.0/cso_classifier/config.ini
--rw-r--r--   0 aas358   (1141393362) OPEN-UNIVERSITY\Domain Users (1182653967)     3755 2021-07-13 16:00:10.000000 cso-classifier-3.0/cso_classifier/config.py
--rw-r--r--   0 aas358   (1141393362) OPEN-UNIVERSITY\Domain Users (1182653967)     2327 2021-07-13 16:00:10.000000 cso-classifier-3.0/cso_classifier/misc.py
--rw-r--r--   0 aas358   (1141393362) OPEN-UNIVERSITY\Domain Users (1182653967)     8700 2021-07-13 16:00:10.000000 cso-classifier-3.0/cso_classifier/model.py
--rw-r--r--   0 aas358   (1141393362) OPEN-UNIVERSITY\Domain Users (1182653967)    19219 2021-07-13 16:00:10.000000 cso-classifier-3.0/cso_classifier/ontology.py
--rw-r--r--   0 aas358   (1141393362) OPEN-UNIVERSITY\Domain Users (1182653967)     7084 2021-07-13 16:00:10.000000 cso-classifier-3.0/cso_classifier/paper.py
--rw-r--r--   0 aas358   (1141393362) OPEN-UNIVERSITY\Domain Users (1182653967)    10045 2021-07-13 16:00:10.000000 cso-classifier-3.0/cso_classifier/postprocmodule.py
--rw-r--r--   0 aas358   (1141393362) OPEN-UNIVERSITY\Domain Users (1182653967)     3202 2021-07-13 16:00:10.000000 cso-classifier-3.0/cso_classifier/result.py
--rw-r--r--   0 aas358   (1141393362) OPEN-UNIVERSITY\Domain Users (1182653967)    12660 2021-07-13 16:00:10.000000 cso-classifier-3.0/cso_classifier/semanticmodule.py
--rw-r--r--   0 aas358   (1141393362) OPEN-UNIVERSITY\Domain Users (1182653967)     6674 2021-07-13 16:00:10.000000 cso-classifier-3.0/cso_classifier/syntacticmodule.py
--rw-r--r--   0 aas358   (1141393362) OPEN-UNIVERSITY\Domain Users (1182653967)     5103 2021-07-13 16:00:10.000000 cso-classifier-3.0/cso_classifier/test.py
--rw-r--r--   0 aas358   (1141393362) OPEN-UNIVERSITY\Domain Users (1182653967)       88 2021-07-13 16:00:10.000000 cso-classifier-3.0/cso_classifier/version.py
-drwxr-xr-x   0 aas358   (1141393362) OPEN-UNIVERSITY\Domain Users (1182653967)        0 2021-07-13 16:31:58.000000 cso-classifier-3.0/cso_classifier.egg-info/
--rw-r--r--   0 aas358   (1141393362) OPEN-UNIVERSITY\Domain Users (1182653967)    41377 2021-07-13 16:31:58.000000 cso-classifier-3.0/cso_classifier.egg-info/PKG-INFO
--rw-r--r--   0 aas358   (1141393362) OPEN-UNIVERSITY\Domain Users (1182653967)      638 2021-07-13 16:31:58.000000 cso-classifier-3.0/cso_classifier.egg-info/SOURCES.txt
--rw-r--r--   0 aas358   (1141393362) OPEN-UNIVERSITY\Domain Users (1182653967)        1 2021-07-13 16:31:58.000000 cso-classifier-3.0/cso_classifier.egg-info/dependency_links.txt
--rw-r--r--   0 aas358   (1141393362) OPEN-UNIVERSITY\Domain Users (1182653967)      203 2021-07-13 16:31:58.000000 cso-classifier-3.0/cso_classifier.egg-info/requires.txt
--rw-r--r--   0 aas358   (1141393362) OPEN-UNIVERSITY\Domain Users (1182653967)       15 2021-07-13 16:31:58.000000 cso-classifier-3.0/cso_classifier.egg-info/top_level.txt
--rw-r--r--   0 aas358   (1141393362) OPEN-UNIVERSITY\Domain Users (1182653967)       38 2021-07-13 16:31:58.000000 cso-classifier-3.0/setup.cfg
--rw-r--r--   0 aas358   (1141393362) OPEN-UNIVERSITY\Domain Users (1182653967)     1428 2021-07-13 16:00:10.000000 cso-classifier-3.0/setup.py
+drwxr-xr-x   0 aas358   (311234) kmi      (100513)        0 2023-05-16 11:50:42.000000 cso-classifier-3.1/
+-rw-r--r--   0 aas358   (311234) kmi      (100513)    11385 2023-05-16 11:48:48.000000 cso-classifier-3.1/LICENSE
+-rw-r--r--   0 aas358   (311234) kmi      (100513)       42 2023-05-16 11:48:48.000000 cso-classifier-3.1/MANIFEST.in
+-rw-r--r--   0 aas358   (311234) kmi      (100513)    42642 2023-05-16 11:50:42.000000 cso-classifier-3.1/PKG-INFO
+-rw-r--r--   0 aas358   (311234) kmi      (100513)    42057 2023-05-16 11:48:48.000000 cso-classifier-3.1/README.md
+drwxr-xr-x   0 aas358   (311234) kmi      (100513)        0 2023-05-16 11:50:42.000000 cso-classifier-3.1/cso_classifier/
+-rw-r--r--   0 aas358   (311234) kmi      (100513)      462 2023-05-16 11:48:48.000000 cso-classifier-3.1/cso_classifier/__init__.py
+drwxr-xr-x   0 aas358   (311234) kmi      (100513)        0 2023-05-16 11:50:42.000000 cso-classifier-3.1/cso_classifier/assets/
+-rw-r--r--   0 aas358   (311234) kmi      (100513)     1845 2023-05-16 11:48:48.000000 cso-classifier-3.1/cso_classifier/assets/README.md
+-rw-r--r--   0 aas358   (311234) kmi      (100513)    12906 2023-05-16 11:48:48.000000 cso-classifier-3.1/cso_classifier/classifier.py
+-rw-r--r--   0 aas358   (311234) kmi      (100513)      574 2023-05-16 11:48:48.000000 cso-classifier-3.1/cso_classifier/config.ini
+-rw-r--r--   0 aas358   (311234) kmi      (100513)     3755 2023-05-16 11:48:48.000000 cso-classifier-3.1/cso_classifier/config.py
+-rw-r--r--   0 aas358   (311234) kmi      (100513)     2327 2023-05-16 11:48:48.000000 cso-classifier-3.1/cso_classifier/misc.py
+-rw-r--r--   0 aas358   (311234) kmi      (100513)     8700 2023-05-16 11:48:48.000000 cso-classifier-3.1/cso_classifier/model.py
+-rw-r--r--   0 aas358   (311234) kmi      (100513)    19219 2023-05-16 11:48:48.000000 cso-classifier-3.1/cso_classifier/ontology.py
+-rw-r--r--   0 aas358   (311234) kmi      (100513)     7084 2023-05-16 11:48:48.000000 cso-classifier-3.1/cso_classifier/paper.py
+-rw-r--r--   0 aas358   (311234) kmi      (100513)    10045 2023-05-16 11:48:48.000000 cso-classifier-3.1/cso_classifier/postprocmodule.py
+-rw-r--r--   0 aas358   (311234) kmi      (100513)     3202 2023-05-16 11:48:48.000000 cso-classifier-3.1/cso_classifier/result.py
+-rw-r--r--   0 aas358   (311234) kmi      (100513)    12667 2023-05-16 11:48:48.000000 cso-classifier-3.1/cso_classifier/semanticmodule.py
+-rw-r--r--   0 aas358   (311234) kmi      (100513)     6671 2023-05-16 11:48:48.000000 cso-classifier-3.1/cso_classifier/syntacticmodule.py
+-rw-r--r--   0 aas358   (311234) kmi      (100513)     5103 2023-05-16 11:48:48.000000 cso-classifier-3.1/cso_classifier/test.py
+-rw-r--r--   0 aas358   (311234) kmi      (100513)       88 2023-05-16 11:48:48.000000 cso-classifier-3.1/cso_classifier/version.py
+drwxr-xr-x   0 aas358   (311234) kmi      (100513)        0 2023-05-16 11:50:42.000000 cso-classifier-3.1/cso_classifier.egg-info/
+-rw-r--r--   0 aas358   (311234) kmi      (100513)    42642 2023-05-16 11:50:42.000000 cso-classifier-3.1/cso_classifier.egg-info/PKG-INFO
+-rw-r--r--   0 aas358   (311234) kmi      (100513)      638 2023-05-16 11:50:42.000000 cso-classifier-3.1/cso_classifier.egg-info/SOURCES.txt
+-rw-r--r--   0 aas358   (311234) kmi      (100513)        1 2023-05-16 11:50:42.000000 cso-classifier-3.1/cso_classifier.egg-info/dependency_links.txt
+-rw-r--r--   0 aas358   (311234) kmi      (100513)      264 2023-05-16 11:50:42.000000 cso-classifier-3.1/cso_classifier.egg-info/requires.txt
+-rw-r--r--   0 aas358   (311234) kmi      (100513)       15 2023-05-16 11:50:42.000000 cso-classifier-3.1/cso_classifier.egg-info/top_level.txt
+-rw-r--r--   0 aas358   (311234) kmi      (100513)       38 2023-05-16 11:50:42.000000 cso-classifier-3.1/setup.cfg
+-rw-r--r--   0 aas358   (311234) kmi      (100513)     1484 2023-05-16 11:48:48.000000 cso-classifier-3.1/setup.py
```

### Comparing `cso-classifier-3.0/LICENSE` & `cso-classifier-3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cso-classifier-3.0/PKG-INFO` & `cso-classifier-3.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,68 +1,65 @@
-Metadata-Version: 2.1
-Name: cso-classifier
-Version: 3.0
-Summary: A light-weight Python app for classifying scientific documents with the topics from the Computer Science Ontology (https://cso.kmi.open.ac.uk/home).
-Home-page: https://github.com/angelosalatino/cso-classifier
-Author: Angelo Salatino
-Author-email: angelo.salatino@open.ac.uk
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # CSO-Classifier
 
 [![PyPI version](https://badge.fury.io/py/cso-classifier.svg)](https://badge.fury.io/py/cso-classifier) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.2660819.svg)](https://doi.org/10.5281/zenodo.2660819)
 [![Python 3.6+](https://img.shields.io/badge/python-3.6+-blue.svg)](https://www.python.org/downloads/release/python-360/)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 ## Abstract
 
 Classifying research papers according to their research topics is an important task to improve their retrievability, assist the creation of smart analytics, and support a variety of approaches for analysing and making sense of the research environment. In this repository, we present the CSO Classifier, a new unsupervised approach for automatically classifying research papers according to the [Computer Science Ontology (CSO)](https://cso.kmi.open.ac.uk), a comprehensive ontology of research areas in the field of Computer Science. The CSO Classifier takes as input the metadata associated with a research paper (title, abstract, keywords) and returns a selection of research concepts drawn from the ontology. The approach was evaluated on a gold standard of manually annotated articles yielding a significant improvement over alternative methods.
 
+Read more: [https://skm.kmi.open.ac.uk/cso-classifier/](https://skm.kmi.open.ac.uk/cso-classifier/)
+
 ## Table of contents
 
 <!--ts-->
-* [Abstract](#abstract)
-* [Table of contents](#table-of-contents)
-* [About](#about)
-* [Getting started](#getting-started)
-  * [Installation using PIP](#installation-using-pip)
-  * [Installation using Github](#installation-using-github)
-  * [Troubleshooting](#troubleshooting)
-  * [Setup](#setup)
-  * [Update](#update)
-  * [Version](#version)
-  * [Test](#test)
-* [Usage examples](#usage-examples)
-  * [Classifying a single paper (SP)](#classifying-a-single-paper-sp)
-  * [Classifying in batch mode (BM)](#classifying-in-batch-mode-bm)
-  * [Parameters](#parameters)
-* [Releases](#releases)
-  * [v3.0](#v30)
-  * [v2.3.2](#v232)
-  * [v2.3.1](#v231)
-  * [v2.3](#v23)
-  * [v2.2](#v22)
-  * [v2.1](#v21)
-  * [v2.0](#v20)
-  * [v1.0](#v10)
-* [List of Files](#list-of-files)
-* [Word2vec model and token-to-cso-combined file generation](#word2vec-model-and-token-to-cso-combined-file-generation)
-  * [Word Embedding generation](#word-embedding-generation)
-  * [token-to-cso-combined file](#token-to-cso-combined-file)
-* [Use the CSO Classifier in other domains of Science](#use-the-cso-classifier-in-other-domains-of-science)
-* [How to Cite CSO Classifier](#how-to-cite-cso-classifier)
-* [License](#license)
-* [References](#references)
+- [CSO-Classifier](#cso-classifier)
+  - [Abstract](#abstract)
+  - [Table of contents](#table-of-contents)
+  - [About](#about)
+  - [Getting started](#getting-started)
+    - [Installation using PIP](#installation-using-pip)
+    - [Installation using Github](#installation-using-github)
+    - [Troubleshooting](#troubleshooting)
+      - [Unable to install requirements](#unable-to-install-requirements)
+      - [Unable to install python-Levenshtein](#unable-to-install-python-levenshtein)
+      - ["python setup.py egg\_info" failed](#python-setuppy-egg_info-failed)
+    - [Setup](#setup)
+    - [Update](#update)
+    - [Version](#version)
+    - [Test](#test)
+  - [Usage examples](#usage-examples)
+    - [Classifying a single paper (SP)](#classifying-a-single-paper-sp)
+      - [Sample Input (SP)](#sample-input-sp)
+      - [Run (SP)](#run-sp)
+      - [Sample Output (SP)](#sample-output-sp)
+    - [Classifying in batch mode (BM)](#classifying-in-batch-mode-bm)
+      - [Sample Input (BM)](#sample-input-bm)
+      - [Run (BM)](#run-bm)
+      - [Sample Output (BM)](#sample-output-bm)
+    - [Parameters](#parameters)
+  - [Releases](#releases)
+    - [v3.1](#v31)
+    - [v3.0](#v30)
+    - [v2.3.2](#v232)
+    - [v2.3.1](#v231)
+    - [v2.3](#v23)
+    - [v2.2](#v22)
+    - [v2.1](#v21)
+    - [v2.0](#v20)
+    - [v1.0](#v10)
+  - [List of Files](#list-of-files)
+  - [Word2vec model and token-to-cso-combined file generation](#word2vec-model-and-token-to-cso-combined-file-generation)
+    - [Word Embedding generation](#word-embedding-generation)
+    - [token-to-cso-combined file](#token-to-cso-combined-file)
+  - [Use the CSO Classifier in other domains of Science](#use-the-cso-classifier-in-other-domains-of-science)
+  - [How to Cite CSO Classifier](#how-to-cite-cso-classifier)
+  - [License](#license)
+  - [References](#references)
 <!--te-->
 
 ## About
 
 The CSO Classifier is a novel application that takes as input the text from the abstract, title, and keywords of a research paper and outputs a list of relevant concepts from CSO. It consists of three main components: (i) the syntactic module, (ii) the semantic module and (iii) the post-processing module. Figure 1 depicts its architecture. The syntactic module parses the input documents and identifies CSO concepts that are explicitly referred to in the document. The semantic module uses part-of-speech tagging to identify promising terms and then exploits word embeddings to infer semantically related topics. Finally, the post-processing module combines the results of these two modules, removes outliers, and enhances them by including relevant super-areas.
 
 ![Framework of CSO Classifier](https://github.com/angelosalatino/cso-classifier/raw/master/images/Workflow.png "Framework of CSO Classifier")
@@ -218,15 +215,15 @@
 
 Even if you are running multiple classifications, the current implementation of the CSO Classifier will load the CSO and the model only once, saving computational time.
 
 #### Sample Output (SP)
 
 As output, the classifier returns a dictionary with five components: (i) syntactic, (ii) semantic, (iii) union, (iv) enhanced, and (v) explanation. The latter field is available only if the **explanation** flag is set to True.
 
-Below you can find an example. The keys syntactic and semantic respectively contain the topics returned by the syntacic and semantic module. Union contains the unique topics found by the previous two modules. In ehancement you can find the relevant super-areas. *Please be aware that the results may change according to the version of Computer Science Ontology.*
+Below you can find an example. The keys syntactic and semantic respectively contain the topics returned by the syntactic and semantic module. Union contains the unique topics found by the previous two modules. In enhanced you can find the relevant super-areas. *Please be aware that the results may change according to the version of Computer Science Ontology.*
 
 ```json
 {
    "syntactic":[
       "network topology",
       "online social networks",
       "real-world networks",
@@ -433,14 +430,23 @@
 **Table 1**: Parameters availability when using CSO Classifier
 
 
 ## Releases
 
 Here we list the available releases for the CSO Classifier. These releases are available for download both from [Github](https://github.com/angelosalatino/cso-classifier/releases) and [Zenodo](10.5281/zenodo.2660819).
 
+### v3.1
+
+This release brings in two main changes. The first change is related to the library (and the code) to perform the Levenshtein similarity. Before we relied on ```python-Levenshtein``` which required ```python3-devel```. This new version uses ```rapidfuzz``` which as fast as the previous library and it is much easier to install on the various systems.
+The second change is related to an updated list of dependencies. We updated some libraries including ```igraph```.
+
+Download from:
+
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7940877.svg)](https://doi.org/10.5281/zenodo.7940877)
+
 ### v3.0
 
 This release welcomes some improvements under the hood. In particular:
 * we refactored the code, reorganising scripts into more elegant classes
 * we added functionalities to automatically setup and update the classifier to the latest version of CSO
 * we added the *explanation* feature, which returns chunks of text that allowed the classifier to infer a given topic
 * the syntactic module takes now advantage of Spacy POS tagger (as previously done only by semantic module)
@@ -602,9 +608,7 @@
 ## References
 
 [1] Osborne, F., Salatino, A., Birukou, A. and Motta, E. 2016. Automatic Classification of Springer Nature Proceedings with Smart Topic Miner. The Semantic Web -- ISWC 2016. 9982 LNCS, (2016), 383–399. DOI:https://doi.org/10.1007/978-3-319-46547-0_33
 
 [2] Mikolov, T., Chen, K., Corrado, G. and Dean, J. 2013. Efficient Estimation of Word Representations in Vector Space. (Jan. 2013).
 
 [3] Mikolov, T., Chen, K., Corrado, G. and Dean, J. 2013. Distributed Representations of Words and Phrases and their Compositionality. Advances in neural information processing systems. 3111–3119.
-
-
```

### Comparing `cso-classifier-3.0/README.md` & `cso-classifier-3.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,52 +1,79 @@
+Metadata-Version: 2.1
+Name: cso-classifier
+Version: 3.1
+Summary: A light-weight Python app for classifying scientific documents with the topics from the Computer Science Ontology (https://cso.kmi.open.ac.uk/home).
+Home-page: https://github.com/angelosalatino/cso-classifier
+Author: Angelo Salatino
+Author-email: angelo.salatino@open.ac.uk
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # CSO-Classifier
 
 [![PyPI version](https://badge.fury.io/py/cso-classifier.svg)](https://badge.fury.io/py/cso-classifier) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.2660819.svg)](https://doi.org/10.5281/zenodo.2660819)
 [![Python 3.6+](https://img.shields.io/badge/python-3.6+-blue.svg)](https://www.python.org/downloads/release/python-360/)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 ## Abstract
 
 Classifying research papers according to their research topics is an important task to improve their retrievability, assist the creation of smart analytics, and support a variety of approaches for analysing and making sense of the research environment. In this repository, we present the CSO Classifier, a new unsupervised approach for automatically classifying research papers according to the [Computer Science Ontology (CSO)](https://cso.kmi.open.ac.uk), a comprehensive ontology of research areas in the field of Computer Science. The CSO Classifier takes as input the metadata associated with a research paper (title, abstract, keywords) and returns a selection of research concepts drawn from the ontology. The approach was evaluated on a gold standard of manually annotated articles yielding a significant improvement over alternative methods.
 
+Read more: [https://skm.kmi.open.ac.uk/cso-classifier/](https://skm.kmi.open.ac.uk/cso-classifier/)
+
 ## Table of contents
 
 <!--ts-->
-* [Abstract](#abstract)
-* [Table of contents](#table-of-contents)
-* [About](#about)
-* [Getting started](#getting-started)
-  * [Installation using PIP](#installation-using-pip)
-  * [Installation using Github](#installation-using-github)
-  * [Troubleshooting](#troubleshooting)
-  * [Setup](#setup)
-  * [Update](#update)
-  * [Version](#version)
-  * [Test](#test)
-* [Usage examples](#usage-examples)
-  * [Classifying a single paper (SP)](#classifying-a-single-paper-sp)
-  * [Classifying in batch mode (BM)](#classifying-in-batch-mode-bm)
-  * [Parameters](#parameters)
-* [Releases](#releases)
-  * [v3.0](#v30)
-  * [v2.3.2](#v232)
-  * [v2.3.1](#v231)
-  * [v2.3](#v23)
-  * [v2.2](#v22)
-  * [v2.1](#v21)
-  * [v2.0](#v20)
-  * [v1.0](#v10)
-* [List of Files](#list-of-files)
-* [Word2vec model and token-to-cso-combined file generation](#word2vec-model-and-token-to-cso-combined-file-generation)
-  * [Word Embedding generation](#word-embedding-generation)
-  * [token-to-cso-combined file](#token-to-cso-combined-file)
-* [Use the CSO Classifier in other domains of Science](#use-the-cso-classifier-in-other-domains-of-science)
-* [How to Cite CSO Classifier](#how-to-cite-cso-classifier)
-* [License](#license)
-* [References](#references)
+- [CSO-Classifier](#cso-classifier)
+  - [Abstract](#abstract)
+  - [Table of contents](#table-of-contents)
+  - [About](#about)
+  - [Getting started](#getting-started)
+    - [Installation using PIP](#installation-using-pip)
+    - [Installation using Github](#installation-using-github)
+    - [Troubleshooting](#troubleshooting)
+      - [Unable to install requirements](#unable-to-install-requirements)
+      - [Unable to install python-Levenshtein](#unable-to-install-python-levenshtein)
+      - ["python setup.py egg\_info" failed](#python-setuppy-egg_info-failed)
+    - [Setup](#setup)
+    - [Update](#update)
+    - [Version](#version)
+    - [Test](#test)
+  - [Usage examples](#usage-examples)
+    - [Classifying a single paper (SP)](#classifying-a-single-paper-sp)
+      - [Sample Input (SP)](#sample-input-sp)
+      - [Run (SP)](#run-sp)
+      - [Sample Output (SP)](#sample-output-sp)
+    - [Classifying in batch mode (BM)](#classifying-in-batch-mode-bm)
+      - [Sample Input (BM)](#sample-input-bm)
+      - [Run (BM)](#run-bm)
+      - [Sample Output (BM)](#sample-output-bm)
+    - [Parameters](#parameters)
+  - [Releases](#releases)
+    - [v3.1](#v31)
+    - [v3.0](#v30)
+    - [v2.3.2](#v232)
+    - [v2.3.1](#v231)
+    - [v2.3](#v23)
+    - [v2.2](#v22)
+    - [v2.1](#v21)
+    - [v2.0](#v20)
+    - [v1.0](#v10)
+  - [List of Files](#list-of-files)
+  - [Word2vec model and token-to-cso-combined file generation](#word2vec-model-and-token-to-cso-combined-file-generation)
+    - [Word Embedding generation](#word-embedding-generation)
+    - [token-to-cso-combined file](#token-to-cso-combined-file)
+  - [Use the CSO Classifier in other domains of Science](#use-the-cso-classifier-in-other-domains-of-science)
+  - [How to Cite CSO Classifier](#how-to-cite-cso-classifier)
+  - [License](#license)
+  - [References](#references)
 <!--te-->
 
 ## About
 
 The CSO Classifier is a novel application that takes as input the text from the abstract, title, and keywords of a research paper and outputs a list of relevant concepts from CSO. It consists of three main components: (i) the syntactic module, (ii) the semantic module and (iii) the post-processing module. Figure 1 depicts its architecture. The syntactic module parses the input documents and identifies CSO concepts that are explicitly referred to in the document. The semantic module uses part-of-speech tagging to identify promising terms and then exploits word embeddings to infer semantically related topics. Finally, the post-processing module combines the results of these two modules, removes outliers, and enhances them by including relevant super-areas.
 
 ![Framework of CSO Classifier](https://github.com/angelosalatino/cso-classifier/raw/master/images/Workflow.png "Framework of CSO Classifier")
@@ -202,15 +229,15 @@
 
 Even if you are running multiple classifications, the current implementation of the CSO Classifier will load the CSO and the model only once, saving computational time.
 
 #### Sample Output (SP)
 
 As output, the classifier returns a dictionary with five components: (i) syntactic, (ii) semantic, (iii) union, (iv) enhanced, and (v) explanation. The latter field is available only if the **explanation** flag is set to True.
 
-Below you can find an example. The keys syntactic and semantic respectively contain the topics returned by the syntacic and semantic module. Union contains the unique topics found by the previous two modules. In ehancement you can find the relevant super-areas. *Please be aware that the results may change according to the version of Computer Science Ontology.*
+Below you can find an example. The keys syntactic and semantic respectively contain the topics returned by the syntactic and semantic module. Union contains the unique topics found by the previous two modules. In enhanced you can find the relevant super-areas. *Please be aware that the results may change according to the version of Computer Science Ontology.*
 
 ```json
 {
    "syntactic":[
       "network topology",
       "online social networks",
       "real-world networks",
@@ -417,14 +444,23 @@
 **Table 1**: Parameters availability when using CSO Classifier
 
 
 ## Releases
 
 Here we list the available releases for the CSO Classifier. These releases are available for download both from [Github](https://github.com/angelosalatino/cso-classifier/releases) and [Zenodo](10.5281/zenodo.2660819).
 
+### v3.1
+
+This release brings in two main changes. The first change is related to the library (and the code) to perform the Levenshtein similarity. Before we relied on ```python-Levenshtein``` which required ```python3-devel```. This new version uses ```rapidfuzz``` which as fast as the previous library and it is much easier to install on the various systems.
+The second change is related to an updated list of dependencies. We updated some libraries including ```igraph```.
+
+Download from:
+
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7940877.svg)](https://doi.org/10.5281/zenodo.7940877)
+
 ### v3.0
 
 This release welcomes some improvements under the hood. In particular:
 * we refactored the code, reorganising scripts into more elegant classes
 * we added functionalities to automatically setup and update the classifier to the latest version of CSO
 * we added the *explanation* feature, which returns chunks of text that allowed the classifier to infer a given topic
 * the syntactic module takes now advantage of Spacy POS tagger (as previously done only by semantic module)
```

### Comparing `cso-classifier-3.0/cso_classifier/assets/README.md` & `cso-classifier-3.1/cso_classifier/assets/README.md`

 * *Files identical despite different names*

### Comparing `cso-classifier-3.0/cso_classifier/classifier.py` & `cso-classifier-3.1/cso_classifier/classifier.py`

 * *Files identical despite different names*

### Comparing `cso-classifier-3.0/cso_classifier/config.ini` & `cso-classifier-3.1/cso_classifier/config.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [classifier]
-classifier_version = 3.0
+classifier_version = 3.1
 package_name = cso-classifier
 
 [ontology]
 cso_path = assets/cso.csv
 cso_pickle_path = assets/cso.p
 cso_graph_path = assets/cso_graph.p
 cso_remote_url = https://cso.kmi.open.ac.uk/download
```

### Comparing `cso-classifier-3.0/cso_classifier/config.py` & `cso-classifier-3.1/cso_classifier/config.py`

 * *Files identical despite different names*

### Comparing `cso-classifier-3.0/cso_classifier/misc.py` & `cso-classifier-3.1/cso_classifier/misc.py`

 * *Files identical despite different names*

### Comparing `cso-classifier-3.0/cso_classifier/model.py` & `cso-classifier-3.1/cso_classifier/model.py`

 * *Files identical despite different names*

### Comparing `cso-classifier-3.0/cso_classifier/ontology.py` & `cso-classifier-3.1/cso_classifier/ontology.py`

 * *Files identical despite different names*

### Comparing `cso-classifier-3.0/cso_classifier/paper.py` & `cso-classifier-3.1/cso_classifier/paper.py`

 * *Files identical despite different names*

### Comparing `cso-classifier-3.0/cso_classifier/postprocmodule.py` & `cso-classifier-3.1/cso_classifier/postprocmodule.py`

 * *Files identical despite different names*

### Comparing `cso-classifier-3.0/cso_classifier/result.py` & `cso-classifier-3.1/cso_classifier/result.py`

 * *Files identical despite different names*

### Comparing `cso-classifier-3.0/cso_classifier/semanticmodule.py` & `cso-classifier-3.1/cso_classifier/semanticmodule.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import warnings
 from kneed import KneeLocator
-import Levenshtein.StringMatcher as ls
+from rapidfuzz.distance import Levenshtein
 from nltk import everygrams
 
 class Semantic:
     """ A simple abstraction layer for using the Semantic module of the CSO classifier """
 
     def __init__(self, model = None, cso = None, fast_classification = True, paper = None):
         """Function that initialises an object of class CSOClassifierSemantic and all its members.
@@ -13,15 +13,15 @@
             model (dictionary): word2vec model.
             cso (dictionary): Computer Science Ontology
             paper (dictionary): paper{"title":"...","abstract":"...","keywords":"..."} the paper.
         """
         self.cso = cso                  #Stores the CSO Ontology
         self.paper = paper              #Paper to analyse
         self.model = model              #contains the cached model
-        self.min_similarity = 0.94      #Initialises the min_similarity
+        self.min_similarity = 0.90      #Initialises the min_similarity
         self.fast_classification = fast_classification # if will use the full model or not
         self.explanation = dict()
 
 
     def set_paper(self, paper):
         """Function that initializes the paper variable in the class.
 
@@ -241,15 +241,15 @@
         Returns:
             list_of_matched_topics (list): containing of all found topics
         """
         identified_topics = list()
         for word, sim in similar_words:
             topics = self.cso.find_closest_matches(word)
             for topic in topics:
-                str_sim = ls.StringMatcher(None, topic, word).ratio() #topic is from cso, wet is from word embedding
+                str_sim = Levenshtein.normalized_similarity(topic, word) #topic is from cso, wet is from word embedding
                 if str_sim >= self.min_similarity:
                     identified_topics.append({"topic":topic,"sim_t":str_sim,"wet":word,"sim_w":sim})
         return identified_topics
 
 
     def __rank_topics(self, found_topics, explanation):
         """ Function that ranks the list of found topics. It also cleans the explanation accordingly
```

### Comparing `cso-classifier-3.0/cso_classifier/syntacticmodule.py` & `cso-classifier-3.1/cso_classifier/syntacticmodule.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from nltk import ngrams
 from nltk.tokenize import word_tokenize
-from Levenshtein.StringMatcher import StringMatcher
+from rapidfuzz.distance import Levenshtein
 
 
 class Syntactic:
     """ A simple abstraction layer for using the Syntactic module of the CSO classifier """
 
     def __init__(self, cso = None, paper = None):
         """Function that initialises an object of class CSOClassifierSyntactic and all its members.
@@ -12,15 +12,15 @@
         Args:
             cso (Ontology class): Computer Science Ontology
             paper (Paper class): object containing the paper.
 
         """
         # Initialise variables to store CSO data - loads into memory
         self.cso = cso                  # the ontologo object
-        self.min_similarity = 0.94      # Value of minimum similarity
+        self.min_similarity = 0.90      # Value of minimum similarity
         self.paper = paper              # the paper object
         self.explanation = dict()       # the explanation dictionary
 
 
     def set_paper(self, paper):
         """Function that initializes the paper variable in the class.
 
@@ -107,15 +107,15 @@
                     # if there isn't an exact match on the first 4 characters of the ngram and a topic, move on
                     #topic_block = [key for key, _ in self.cso.topics.items() if key.startswith(gram[:4])]
                     topic_block = self.cso.topic_stems[gram[:4]]
                 except KeyError:
                     continue
                 for topic in topic_block:
                     # otherwise look for an inexact match
-                    match_ratio = StringMatcher(None, topic, gram).ratio()
+                    match_ratio = Levenshtein.normalized_similarity(topic, gram)
                     if match_ratio >= self.min_similarity:
                         try:
                             # if a 'primary label' exists for the current topic, use it instead of the matched topic
                             topic = self.cso.primary_labels[topic]
                         except KeyError:
                             pass
                         # note the tokens that matched the topic and how closely
```

### Comparing `cso-classifier-3.0/cso_classifier/test.py` & `cso-classifier-3.1/cso_classifier/test.py`

 * *Files identical despite different names*

### Comparing `cso-classifier-3.0/cso_classifier.egg-info/PKG-INFO` & `cso-classifier-3.1/cso_classifier.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: cso-classifier
-Version: 3.0
+Version: 3.1
 Summary: A light-weight Python app for classifying scientific documents with the topics from the Computer Science Ontology (https://cso.kmi.open.ac.uk/home).
 Home-page: https://github.com/angelosalatino/cso-classifier
 Author: Angelo Salatino
 Author-email: angelo.salatino@open.ac.uk
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -20,49 +18,62 @@
 [![Python 3.6+](https://img.shields.io/badge/python-3.6+-blue.svg)](https://www.python.org/downloads/release/python-360/)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 ## Abstract
 
 Classifying research papers according to their research topics is an important task to improve their retrievability, assist the creation of smart analytics, and support a variety of approaches for analysing and making sense of the research environment. In this repository, we present the CSO Classifier, a new unsupervised approach for automatically classifying research papers according to the [Computer Science Ontology (CSO)](https://cso.kmi.open.ac.uk), a comprehensive ontology of research areas in the field of Computer Science. The CSO Classifier takes as input the metadata associated with a research paper (title, abstract, keywords) and returns a selection of research concepts drawn from the ontology. The approach was evaluated on a gold standard of manually annotated articles yielding a significant improvement over alternative methods.
 
+Read more: [https://skm.kmi.open.ac.uk/cso-classifier/](https://skm.kmi.open.ac.uk/cso-classifier/)
+
 ## Table of contents
 
 <!--ts-->
-* [Abstract](#abstract)
-* [Table of contents](#table-of-contents)
-* [About](#about)
-* [Getting started](#getting-started)
-  * [Installation using PIP](#installation-using-pip)
-  * [Installation using Github](#installation-using-github)
-  * [Troubleshooting](#troubleshooting)
-  * [Setup](#setup)
-  * [Update](#update)
-  * [Version](#version)
-  * [Test](#test)
-* [Usage examples](#usage-examples)
-  * [Classifying a single paper (SP)](#classifying-a-single-paper-sp)
-  * [Classifying in batch mode (BM)](#classifying-in-batch-mode-bm)
-  * [Parameters](#parameters)
-* [Releases](#releases)
-  * [v3.0](#v30)
-  * [v2.3.2](#v232)
-  * [v2.3.1](#v231)
-  * [v2.3](#v23)
-  * [v2.2](#v22)
-  * [v2.1](#v21)
-  * [v2.0](#v20)
-  * [v1.0](#v10)
-* [List of Files](#list-of-files)
-* [Word2vec model and token-to-cso-combined file generation](#word2vec-model-and-token-to-cso-combined-file-generation)
-  * [Word Embedding generation](#word-embedding-generation)
-  * [token-to-cso-combined file](#token-to-cso-combined-file)
-* [Use the CSO Classifier in other domains of Science](#use-the-cso-classifier-in-other-domains-of-science)
-* [How to Cite CSO Classifier](#how-to-cite-cso-classifier)
-* [License](#license)
-* [References](#references)
+- [CSO-Classifier](#cso-classifier)
+  - [Abstract](#abstract)
+  - [Table of contents](#table-of-contents)
+  - [About](#about)
+  - [Getting started](#getting-started)
+    - [Installation using PIP](#installation-using-pip)
+    - [Installation using Github](#installation-using-github)
+    - [Troubleshooting](#troubleshooting)
+      - [Unable to install requirements](#unable-to-install-requirements)
+      - [Unable to install python-Levenshtein](#unable-to-install-python-levenshtein)
+      - ["python setup.py egg\_info" failed](#python-setuppy-egg_info-failed)
+    - [Setup](#setup)
+    - [Update](#update)
+    - [Version](#version)
+    - [Test](#test)
+  - [Usage examples](#usage-examples)
+    - [Classifying a single paper (SP)](#classifying-a-single-paper-sp)
+      - [Sample Input (SP)](#sample-input-sp)
+      - [Run (SP)](#run-sp)
+      - [Sample Output (SP)](#sample-output-sp)
+    - [Classifying in batch mode (BM)](#classifying-in-batch-mode-bm)
+      - [Sample Input (BM)](#sample-input-bm)
+      - [Run (BM)](#run-bm)
+      - [Sample Output (BM)](#sample-output-bm)
+    - [Parameters](#parameters)
+  - [Releases](#releases)
+    - [v3.1](#v31)
+    - [v3.0](#v30)
+    - [v2.3.2](#v232)
+    - [v2.3.1](#v231)
+    - [v2.3](#v23)
+    - [v2.2](#v22)
+    - [v2.1](#v21)
+    - [v2.0](#v20)
+    - [v1.0](#v10)
+  - [List of Files](#list-of-files)
+  - [Word2vec model and token-to-cso-combined file generation](#word2vec-model-and-token-to-cso-combined-file-generation)
+    - [Word Embedding generation](#word-embedding-generation)
+    - [token-to-cso-combined file](#token-to-cso-combined-file)
+  - [Use the CSO Classifier in other domains of Science](#use-the-cso-classifier-in-other-domains-of-science)
+  - [How to Cite CSO Classifier](#how-to-cite-cso-classifier)
+  - [License](#license)
+  - [References](#references)
 <!--te-->
 
 ## About
 
 The CSO Classifier is a novel application that takes as input the text from the abstract, title, and keywords of a research paper and outputs a list of relevant concepts from CSO. It consists of three main components: (i) the syntactic module, (ii) the semantic module and (iii) the post-processing module. Figure 1 depicts its architecture. The syntactic module parses the input documents and identifies CSO concepts that are explicitly referred to in the document. The semantic module uses part-of-speech tagging to identify promising terms and then exploits word embeddings to infer semantically related topics. Finally, the post-processing module combines the results of these two modules, removes outliers, and enhances them by including relevant super-areas.
 
 ![Framework of CSO Classifier](https://github.com/angelosalatino/cso-classifier/raw/master/images/Workflow.png "Framework of CSO Classifier")
@@ -218,15 +229,15 @@
 
 Even if you are running multiple classifications, the current implementation of the CSO Classifier will load the CSO and the model only once, saving computational time.
 
 #### Sample Output (SP)
 
 As output, the classifier returns a dictionary with five components: (i) syntactic, (ii) semantic, (iii) union, (iv) enhanced, and (v) explanation. The latter field is available only if the **explanation** flag is set to True.
 
-Below you can find an example. The keys syntactic and semantic respectively contain the topics returned by the syntacic and semantic module. Union contains the unique topics found by the previous two modules. In ehancement you can find the relevant super-areas. *Please be aware that the results may change according to the version of Computer Science Ontology.*
+Below you can find an example. The keys syntactic and semantic respectively contain the topics returned by the syntactic and semantic module. Union contains the unique topics found by the previous two modules. In enhanced you can find the relevant super-areas. *Please be aware that the results may change according to the version of Computer Science Ontology.*
 
 ```json
 {
    "syntactic":[
       "network topology",
       "online social networks",
       "real-world networks",
@@ -433,14 +444,23 @@
 **Table 1**: Parameters availability when using CSO Classifier
 
 
 ## Releases
 
 Here we list the available releases for the CSO Classifier. These releases are available for download both from [Github](https://github.com/angelosalatino/cso-classifier/releases) and [Zenodo](10.5281/zenodo.2660819).
 
+### v3.1
+
+This release brings in two main changes. The first change is related to the library (and the code) to perform the Levenshtein similarity. Before we relied on ```python-Levenshtein``` which required ```python3-devel```. This new version uses ```rapidfuzz``` which as fast as the previous library and it is much easier to install on the various systems.
+The second change is related to an updated list of dependencies. We updated some libraries including ```igraph```.
+
+Download from:
+
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7940877.svg)](https://doi.org/10.5281/zenodo.7940877)
+
 ### v3.0
 
 This release welcomes some improvements under the hood. In particular:
 * we refactored the code, reorganising scripts into more elegant classes
 * we added functionalities to automatically setup and update the classifier to the latest version of CSO
 * we added the *explanation* feature, which returns chunks of text that allowed the classifier to infer a given topic
 * the syntactic module takes now advantage of Spacy POS tagger (as previously done only by semantic module)
@@ -602,9 +622,7 @@
 ## References
 
 [1] Osborne, F., Salatino, A., Birukou, A. and Motta, E. 2016. Automatic Classification of Springer Nature Proceedings with Smart Topic Miner. The Semantic Web -- ISWC 2016. 9982 LNCS, (2016), 383–399. DOI:https://doi.org/10.1007/978-3-319-46547-0_33
 
 [2] Mikolov, T., Chen, K., Corrado, G. and Dean, J. 2013. Efficient Estimation of Word Representations in Vector Space. (Jan. 2013).
 
 [3] Mikolov, T., Chen, K., Corrado, G. and Dean, J. 2013. Distributed Representations of Words and Phrases and their Compositionality. Advances in neural information processing systems. 3111–3119.
-
-
```

### Comparing `cso-classifier-3.0/cso_classifier.egg-info/SOURCES.txt` & `cso-classifier-3.1/cso_classifier.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cso-classifier-3.0/setup.py` & `cso-classifier-3.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 import configparser
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 requirements_to_install = [
+    'igraph==0.10.4;python_version>="3.7"',
+    'python-igraph==0.9.1;python_version<"3.7"',
+    'gensim==3.8.3',
     'click==7.1.2',
-    'gensim==3.8.1',
     'hurry.filesize==0.9',
     'kneed==0.3.1',
     'nltk==3.6.2',
-    'python-igraph==0.9.1',
-    'python-Levenshtein==0.12.2',
+    'rapidfuzz==2.11.1',
     'numpy>=1.19.5',
     'requests==2.25.1',
     'spacy==3.0.5',
     'strsimpy==0.2.0',
     'update-checker==0.18.0'
 ]
```

