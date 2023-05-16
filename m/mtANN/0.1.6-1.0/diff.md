# Comparing `tmp/mtANN-0.1.6.tar.gz` & `tmp/mtANN-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mtANN-0.1.6.tar", last modified: Mon May 15 12:12:36 2023, max compression
+gzip compressed data, was "dist/mtANN-1.0.tar", last modified: Tue May 16 08:11:15 2023, max compression
```

## Comparing `mtANN-0.1.6.tar` & `mtANN-1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 xyxuan     (501) staff       (20)        0 2023-05-15 12:12:36.000000 mtANN-0.1.6/
--rw-r--r--   0 xyxuan     (501) staff       (20)     2979 2023-05-15 12:12:36.000000 mtANN-0.1.6/PKG-INFO
--rw-r--r--   0 xyxuan     (501) staff       (20)     2686 2023-05-15 11:31:58.000000 mtANN-0.1.6/README.md
-drwxr-xr-x   0 xyxuan     (501) staff       (20)        0 2023-05-15 12:12:36.000000 mtANN-0.1.6/mtANN/
--rw-r--r--   0 xyxuan     (501) staff       (20)       40 2023-05-15 11:34:42.000000 mtANN-0.1.6/mtANN/__init__.py
--rw-r--r--   0 xyxuan     (501) staff       (20)    15650 2023-05-15 12:11:34.000000 mtANN-0.1.6/mtANN/model.py
--rw-r--r--   0 xyxuan     (501) staff       (20)     3183 2023-05-11 10:26:48.000000 mtANN-0.1.6/mtANN/utils.py
-drwxr-xr-x   0 xyxuan     (501) staff       (20)        0 2023-05-15 12:12:36.000000 mtANN-0.1.6/mtANN.egg-info/
--rw-r--r--   0 xyxuan     (501) staff       (20)     2979 2023-05-15 12:12:36.000000 mtANN-0.1.6/mtANN.egg-info/PKG-INFO
--rw-r--r--   0 xyxuan     (501) staff       (20)      210 2023-05-15 12:12:36.000000 mtANN-0.1.6/mtANN.egg-info/SOURCES.txt
--rw-r--r--   0 xyxuan     (501) staff       (20)        1 2023-05-15 12:12:36.000000 mtANN-0.1.6/mtANN.egg-info/dependency_links.txt
--rw-r--r--   0 xyxuan     (501) staff       (20)       61 2023-05-15 12:12:36.000000 mtANN-0.1.6/mtANN.egg-info/requires.txt
--rw-r--r--   0 xyxuan     (501) staff       (20)        6 2023-05-15 12:12:36.000000 mtANN-0.1.6/mtANN.egg-info/top_level.txt
--rw-r--r--   0 xyxuan     (501) staff       (20)       38 2023-05-15 12:12:36.000000 mtANN-0.1.6/setup.cfg
--rw-r--r--   0 xyxuan     (501) staff       (20)      678 2023-05-15 12:12:01.000000 mtANN-0.1.6/setup.py
+drwxr-xr-x   0 xyxuan     (501) staff       (20)        0 2023-05-16 08:11:15.000000 mtANN-1.0/
+-rw-r--r--   0 xyxuan     (501) staff       (20)     3179 2023-05-16 08:11:15.000000 mtANN-1.0/PKG-INFO
+-rwxrwxrwx   0 xyxuan     (501) staff       (20)     2888 2023-05-16 08:10:59.000000 mtANN-1.0/README.md
+drwxr-xr-x   0 xyxuan     (501) staff       (20)        0 2023-05-16 08:11:15.000000 mtANN-1.0/mtANN/
+-rwxrwxrwx   0 xyxuan     (501) staff       (20)       40 2023-05-15 11:34:42.000000 mtANN-1.0/mtANN/__init__.py
+-rwxrwxrwx   0 xyxuan     (501) staff       (20)    15650 2023-05-15 12:11:34.000000 mtANN-1.0/mtANN/model.py
+-rwxrwxrwx   0 xyxuan     (501) staff       (20)     3183 2023-05-11 10:26:48.000000 mtANN-1.0/mtANN/utils.py
+drwxr-xr-x   0 xyxuan     (501) staff       (20)        0 2023-05-16 08:11:15.000000 mtANN-1.0/mtANN.egg-info/
+-rw-r--r--   0 xyxuan     (501) staff       (20)     3179 2023-05-16 08:11:15.000000 mtANN-1.0/mtANN.egg-info/PKG-INFO
+-rw-r--r--   0 xyxuan     (501) staff       (20)      210 2023-05-16 08:11:15.000000 mtANN-1.0/mtANN.egg-info/SOURCES.txt
+-rw-r--r--   0 xyxuan     (501) staff       (20)        1 2023-05-16 08:11:15.000000 mtANN-1.0/mtANN.egg-info/dependency_links.txt
+-rw-r--r--   0 xyxuan     (501) staff       (20)       61 2023-05-16 08:11:15.000000 mtANN-1.0/mtANN.egg-info/requires.txt
+-rw-r--r--   0 xyxuan     (501) staff       (20)        6 2023-05-16 08:11:15.000000 mtANN-1.0/mtANN.egg-info/top_level.txt
+-rw-r--r--   0 xyxuan     (501) staff       (20)       38 2023-05-16 08:11:15.000000 mtANN-1.0/setup.cfg
+-rwxrwxrwx   0 xyxuan     (501) staff       (20)      619 2023-05-16 08:10:43.000000 mtANN-1.0/setup.py
```

### Comparing `mtANN-0.1.6/PKG-INFO` & `mtANN-1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: mtANN
-Version: 0.1.6
-Summary: Ensemble Multiple References for Single-cell RNA Seuquencing Data Annotation and Unseen Cells Identification
-Author: Yi-Xuan Xiong
-Author-email: xyxuana@mails.ccnu.edu.cn
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
 # Ensemble of multiple references for single-cell RNA sequencing data annotation and unseen cell-type identification
 
 mtANN is a novel cell-type annotation framework
 that integrates ensemble learning and deep learning
 simultaneously, to annotate cells in a new query dataset with the help of multiple well-labeled reference datasets. It takes multiple well-labeled reference datasets and a query dataset that needs to be annotated as input. It begins with generating a series of subsets for each reference dataset by adopting various gene selection methods. Next, for each reference subset, a base classification model is trained based on neural networks. Then, mtANN annotates the cells in the query dataset by integrating the prediction results from all the base classification models. Finally, it identifies cells that may belong to cell types not observed in the reference datasets according to the uncertainty of the predictions.
 
 ![Figure1](Figure1.png)
@@ -28,32 +19,30 @@
 - Python: 3.8.8
 - Python packages: pandas = 1.2.3, numpy = 1.19,2, scanpy=1.9.0, scipy = 1.6.1, sklearn = 0.24.1, torch = 1.9.1, giniclust3 = 1.1.0, rpy2 = 3.5.2
 - R: 3.6.1
 - R packages: limma = 3.42.2, Seurat = 3.1.1, parallel = 3.6.1
 
 ### Environment 2
 - System: Windows 10
-- Python: 3.8.15
-- Python packages: pandas = 2.0.0, numpy = 1.23.5, scanpy=1.9.3, scipy = 1.10.1, sklearn = 1.1.3, torch = 1.10.0, giniclust3 = 1.1.2, rpy2 = 3.4.1
+- Python: 3.7.6
+- Python packages: pandas = 1.3.5, numpy = 1.21.6, scanpy=1.9.3, scipy = 1.7.3, scikit-learn = 1.0.2, torch = 1.13.0, giniclust3 = 1.1.2, rpy2 = 3.5.11
 - R: 4.1.2
 - R packages: limma = 3.50.3, Seurat = 4.2.0, parallel = 4.1.2
 
 # Installation
 
-`pip install mtANN==0.1.3`
+`pip install mtANN==1.0`
+
+To successfully use mtANN, please ensure that R is correctly installed and added to the environment variables. Additionally, you need to add a new user variable named `R_USER` that points to the installation path of the Python package `rpy2`.
 
 # Useage
 The mtANN repository includes the mtANN code files in the `mtANN` folder and provides a usage example `example` which specifically shows the format of the input data and the usage of the main function. The data used in the example can be downloaded at [https://doi.org/10.5281/zenodo.7922657](https://doi.org/10.5281/zenodo.7922657). 
 
 The input data considered by the current version of mtANN is in `csv` format, where rows are samples and columns are features. In addition, its cell type information is stored in another csv file, and its naming format is the name of the dataset + `_label`.
 
-# Installation
-
-`pip install mtANN==0.1.0`
-
  
 # Contact
 
 Please do not hesitate to contact Miss Yi-Xuan Xiong ([xyxuana@mails.ccnu.edu.cn](xyxuana@mails.ccnu.edu.cn)) or Dr. Xiao-Fei Zhang ([zhangxf@ccnu.edu.cn](zhangxf@ccnu.edu.cn)) to seek any clarifications regarding any contents or operation of the archive.
```

### Comparing `mtANN-0.1.6/README.md` & `mtANN-1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+Metadata-Version: 2.1
+Name: mtANN
+Version: 1.0
+Summary: Ensemble Multiple References for Single-cell RNA Seuquencing Data Annotation and Unseen Cells Identification
+Author: Yi-Xuan Xiong
+Author-email: xyxuana@mails.ccnu.edu.cn
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+
 # Ensemble of multiple references for single-cell RNA sequencing data annotation and unseen cell-type identification
 
 mtANN is a novel cell-type annotation framework
 that integrates ensemble learning and deep learning
 simultaneously, to annotate cells in a new query dataset with the help of multiple well-labeled reference datasets. It takes multiple well-labeled reference datasets and a query dataset that needs to be annotated as input. It begins with generating a series of subsets for each reference dataset by adopting various gene selection methods. Next, for each reference subset, a base classification model is trained based on neural networks. Then, mtANN annotates the cells in the query dataset by integrating the prediction results from all the base classification models. Finally, it identifies cells that may belong to cell types not observed in the reference datasets according to the uncertainty of the predictions.
 
 ![Figure1](Figure1.png)
@@ -19,32 +28,30 @@
 - Python: 3.8.8
 - Python packages: pandas = 1.2.3, numpy = 1.19,2, scanpy=1.9.0, scipy = 1.6.1, sklearn = 0.24.1, torch = 1.9.1, giniclust3 = 1.1.0, rpy2 = 3.5.2
 - R: 3.6.1
 - R packages: limma = 3.42.2, Seurat = 3.1.1, parallel = 3.6.1
 
 ### Environment 2
 - System: Windows 10
-- Python: 3.8.15
-- Python packages: pandas = 2.0.0, numpy = 1.23.5, scanpy=1.9.3, scipy = 1.10.1, sklearn = 1.1.3, torch = 1.10.0, giniclust3 = 1.1.2, rpy2 = 3.4.1
+- Python: 3.7.6
+- Python packages: pandas = 1.3.5, numpy = 1.21.6, scanpy=1.9.3, scipy = 1.7.3, scikit-learn = 1.0.2, torch = 1.13.0, giniclust3 = 1.1.2, rpy2 = 3.5.11
 - R: 4.1.2
 - R packages: limma = 3.50.3, Seurat = 4.2.0, parallel = 4.1.2
 
 # Installation
 
-`pip install mtANN==0.1.3`
+`pip install mtANN==1.0`
+
+To successfully use mtANN, please ensure that R is correctly installed and added to the environment variables. Additionally, you need to add a new user variable named `R_USER` that points to the installation path of the Python package `rpy2`.
 
 # Useage
 The mtANN repository includes the mtANN code files in the `mtANN` folder and provides a usage example `example` which specifically shows the format of the input data and the usage of the main function. The data used in the example can be downloaded at [https://doi.org/10.5281/zenodo.7922657](https://doi.org/10.5281/zenodo.7922657). 
 
 The input data considered by the current version of mtANN is in `csv` format, where rows are samples and columns are features. In addition, its cell type information is stored in another csv file, and its naming format is the name of the dataset + `_label`.
 
-# Installation
-
-`pip install mtANN==0.1.0`
-
  
 # Contact
 
 Please do not hesitate to contact Miss Yi-Xuan Xiong ([xyxuana@mails.ccnu.edu.cn](xyxuana@mails.ccnu.edu.cn)) or Dr. Xiao-Fei Zhang ([zhangxf@ccnu.edu.cn](zhangxf@ccnu.edu.cn)) to seek any clarifications regarding any contents or operation of the archive.
```

### Comparing `mtANN-0.1.6/mtANN/model.py` & `mtANN-1.0/mtANN/model.py`

 * *Files identical despite different names*

### Comparing `mtANN-0.1.6/mtANN/utils.py` & `mtANN-1.0/mtANN/utils.py`

 * *Files identical despite different names*

### Comparing `mtANN-0.1.6/mtANN.egg-info/PKG-INFO` & `mtANN-1.0/mtANN.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtANN
-Version: 0.1.6
+Version: 1.0
 Summary: Ensemble Multiple References for Single-cell RNA Seuquencing Data Annotation and Unseen Cells Identification
 Author: Yi-Xuan Xiong
 Author-email: xyxuana@mails.ccnu.edu.cn
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Ensemble of multiple references for single-cell RNA sequencing data annotation and unseen cell-type identification
@@ -28,32 +28,30 @@
 - Python: 3.8.8
 - Python packages: pandas = 1.2.3, numpy = 1.19,2, scanpy=1.9.0, scipy = 1.6.1, sklearn = 0.24.1, torch = 1.9.1, giniclust3 = 1.1.0, rpy2 = 3.5.2
 - R: 3.6.1
 - R packages: limma = 3.42.2, Seurat = 3.1.1, parallel = 3.6.1
 
 ### Environment 2
 - System: Windows 10
-- Python: 3.8.15
-- Python packages: pandas = 2.0.0, numpy = 1.23.5, scanpy=1.9.3, scipy = 1.10.1, sklearn = 1.1.3, torch = 1.10.0, giniclust3 = 1.1.2, rpy2 = 3.4.1
+- Python: 3.7.6
+- Python packages: pandas = 1.3.5, numpy = 1.21.6, scanpy=1.9.3, scipy = 1.7.3, scikit-learn = 1.0.2, torch = 1.13.0, giniclust3 = 1.1.2, rpy2 = 3.5.11
 - R: 4.1.2
 - R packages: limma = 3.50.3, Seurat = 4.2.0, parallel = 4.1.2
 
 # Installation
 
-`pip install mtANN==0.1.3`
+`pip install mtANN==1.0`
+
+To successfully use mtANN, please ensure that R is correctly installed and added to the environment variables. Additionally, you need to add a new user variable named `R_USER` that points to the installation path of the Python package `rpy2`.
 
 # Useage
 The mtANN repository includes the mtANN code files in the `mtANN` folder and provides a usage example `example` which specifically shows the format of the input data and the usage of the main function. The data used in the example can be downloaded at [https://doi.org/10.5281/zenodo.7922657](https://doi.org/10.5281/zenodo.7922657). 
 
 The input data considered by the current version of mtANN is in `csv` format, where rows are samples and columns are features. In addition, its cell type information is stored in another csv file, and its naming format is the name of the dataset + `_label`.
 
-# Installation
-
-`pip install mtANN==0.1.0`
-
  
 # Contact
 
 Please do not hesitate to contact Miss Yi-Xuan Xiong ([xyxuana@mails.ccnu.edu.cn](xyxuana@mails.ccnu.edu.cn)) or Dr. Xiao-Fei Zhang ([zhangxf@ccnu.edu.cn](zhangxf@ccnu.edu.cn)) to seek any clarifications regarding any contents or operation of the archive.
```

