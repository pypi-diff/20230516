# Comparing `tmp/KMMTR-0.0.6.tar.gz` & `tmp/KMMTR-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KMMTR-0.0.6.tar", last modified: Mon May 15 11:33:23 2023, max compression
+gzip compressed data, was "KMMTR-0.0.7.tar", last modified: Tue May 16 11:12:33 2023, max compression
```

## Comparing `KMMTR-0.0.6.tar` & `KMMTR-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-15 11:33:23.785771 KMMTR-0.0.6/
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-15 11:33:23.784884 KMMTR-0.0.6/KMMTR/
--rwxr-xr-x   0 jacob      (501) staff       (20)     6643 2023-05-15 11:31:46.000000 KMMTR-0.0.6/KMMTR/KMM.py
--rwxr-xr-x   0 jacob      (501) staff       (20)     6510 2023-05-15 11:32:03.000000 KMMTR-0.0.6/KMMTR/KMMTR.py
--rwxr-xr-x   0 jacob      (501) staff       (20)      386 2023-04-19 10:18:26.000000 KMMTR-0.0.6/KMMTR/__init__.py
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-15 11:33:23.785473 KMMTR-0.0.6/KMMTR.egg-info/
--rw-r--r--   0 jacob      (501) staff       (20)     1453 2023-05-15 11:33:23.000000 KMMTR-0.0.6/KMMTR.egg-info/PKG-INFO
--rw-r--r--   0 jacob      (501) staff       (20)      208 2023-05-15 11:33:23.000000 KMMTR-0.0.6/KMMTR.egg-info/SOURCES.txt
--rw-r--r--   0 jacob      (501) staff       (20)        1 2023-05-15 11:33:23.000000 KMMTR-0.0.6/KMMTR.egg-info/dependency_links.txt
--rw-r--r--   0 jacob      (501) staff       (20)       33 2023-05-15 11:33:23.000000 KMMTR-0.0.6/KMMTR.egg-info/requires.txt
--rw-r--r--   0 jacob      (501) staff       (20)        6 2023-05-15 11:33:23.000000 KMMTR-0.0.6/KMMTR.egg-info/top_level.txt
--rw-r--r--   0 jacob      (501) staff       (20)     1453 2023-05-15 11:33:23.785638 KMMTR-0.0.6/PKG-INFO
--rw-r--r--   0 jacob      (501) staff       (20)      859 2023-04-20 09:04:07.000000 KMMTR-0.0.6/README.md
--rw-r--r--   0 jacob      (501) staff       (20)       38 2023-05-15 11:33:23.785813 KMMTR-0.0.6/setup.cfg
--rw-r--r--   0 jacob      (501) staff       (20)     1381 2023-05-15 11:33:11.000000 KMMTR-0.0.6/setup.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-16 11:12:33.309531 KMMTR-0.0.7/
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-16 11:12:33.308691 KMMTR-0.0.7/KMMTR/
+-rwxr-xr-x   0 jacob      (501) staff       (20)     6687 2023-05-16 11:11:25.000000 KMMTR-0.0.7/KMMTR/KMM.py
+-rwxr-xr-x   0 jacob      (501) staff       (20)     6510 2023-05-16 11:11:43.000000 KMMTR-0.0.7/KMMTR/KMMTR.py
+-rwxr-xr-x   0 jacob      (501) staff       (20)      386 2023-04-19 10:18:26.000000 KMMTR-0.0.7/KMMTR/__init__.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-16 11:12:33.309250 KMMTR-0.0.7/KMMTR.egg-info/
+-rw-r--r--   0 jacob      (501) staff       (20)     1453 2023-05-16 11:12:33.000000 KMMTR-0.0.7/KMMTR.egg-info/PKG-INFO
+-rw-r--r--   0 jacob      (501) staff       (20)      208 2023-05-16 11:12:33.000000 KMMTR-0.0.7/KMMTR.egg-info/SOURCES.txt
+-rw-r--r--   0 jacob      (501) staff       (20)        1 2023-05-16 11:12:33.000000 KMMTR-0.0.7/KMMTR.egg-info/dependency_links.txt
+-rw-r--r--   0 jacob      (501) staff       (20)       33 2023-05-16 11:12:33.000000 KMMTR-0.0.7/KMMTR.egg-info/requires.txt
+-rw-r--r--   0 jacob      (501) staff       (20)        6 2023-05-16 11:12:33.000000 KMMTR-0.0.7/KMMTR.egg-info/top_level.txt
+-rw-r--r--   0 jacob      (501) staff       (20)     1453 2023-05-16 11:12:33.309405 KMMTR-0.0.7/PKG-INFO
+-rw-r--r--   0 jacob      (501) staff       (20)      859 2023-04-20 09:04:07.000000 KMMTR-0.0.7/README.md
+-rw-r--r--   0 jacob      (501) staff       (20)       38 2023-05-16 11:12:33.309569 KMMTR-0.0.7/setup.cfg
+-rw-r--r--   0 jacob      (501) staff       (20)     1381 2023-05-16 11:11:58.000000 KMMTR-0.0.7/setup.py
```

### Comparing `KMMTR-0.0.6/KMMTR/KMM.py` & `KMMTR-0.0.7/KMMTR/KMM.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,29 +70,30 @@
         
         Returns:
             An instantiated kernel function object.
         """
         Xtrain = np.array(self.target_data)
         Ytrain = np.array(self.target_response)
         ker = self.call_kernel()
-        noise_ker = WhiteKernel(noise_level_bounds=(0.01,0.5))
+        noise_ker = WhiteKernel(noise_level_bounds=(0.01,0.1))
         # cal the data nosie by maximazing the likelihood 
         GPr = GPR(kernel=ker+noise_ker,normalize_y=True).fit(Xtrain,Ytrain)
         noise_level = np.exp(GPr.kernel_.theta[1])
         print('Trained noise is %f' % noise_level)
 
         GPr_fit = GPR(kernel=ker, alpha = noise_level,normalize_y=True).fit(Xtrain,Ytrain)
         print('Trained Kernel Function :', GPr_fit.kernel_)
         para = np.exp(GPr_fit.kernel_.theta)
+        print('Trained length scale :', para)
 
         Inst_kernel = self.call_kernel(para)
         return Inst_kernel
 
 
-    def cal_beta(self, B=1,tao = None):
+    def cal_beta(self, B,tao = None):
         """
         Helper function to calculate the beta values that balance the source and target data distributions.
         
         Args:
             B (float): Bound on the beta values. Defaults to 1.
         
         Returns:
```

### Comparing `KMMTR-0.0.6/KMMTR/KMMTR.py` & `KMMTR-0.0.7/KMMTR/KMMTR.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
     Methods
     -------
     fit(source_dataset,target_dataset,test_data)
         Fit the transfer learning regression model to the source dataset and target dataset, and predict the target variable
         on the test dataset.
     """
-    def __init__(self, Regressor='RF',UpBound=1,kernel = 'RBF', Targets = 1):
+    def __init__(self, Regressor='RF',UpBound=2,kernel = 'RBF', Targets = 1):
         """
         Initialize KMMTransferReg model.
 
         Parameters
         ----------
         Regressor : str or object, default='RF'
             A regression model used to fit the mapped data. If a string is passed, it should be one of {'RF', 'LR'}
```

### Comparing `KMMTR-0.0.6/KMMTR.egg-info/PKG-INFO` & `KMMTR-0.0.7/KMMTR.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KMMTR
-Version: 0.0.6
+Version: 0.0.7
 Summary: a transfer learning regression model based on Kernel Mean Matching (KMM) algorithm
 Home-page: https://github.com/Bin-Cao/KMMTransferRegressor
 Author: CaoBin
 Author-email: bcao@shu.edu.com
 Maintainer: CaoBin
 Maintainer-email: binjacobcao@gmail.com
 License: MIT License
```

### Comparing `KMMTR-0.0.6/PKG-INFO` & `KMMTR-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KMMTR
-Version: 0.0.6
+Version: 0.0.7
 Summary: a transfer learning regression model based on Kernel Mean Matching (KMM) algorithm
 Home-page: https://github.com/Bin-Cao/KMMTransferRegressor
 Author: CaoBin
 Author-email: bcao@shu.edu.com
 Maintainer: CaoBin
 Maintainer-email: binjacobcao@gmail.com
 License: MIT License
```

### Comparing `KMMTR-0.0.6/README.md` & `KMMTR-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `KMMTR-0.0.6/setup.py` & `KMMTR-0.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name='KMMTR',  # 包名
-    version='0.0.6',  # 版本
+    version='0.0.7',  # 版本
     description="a transfer learning regression model based on Kernel Mean Matching (KMM) algorithm",  # 包简介
     long_description=open('README.md',encoding='utf-8').read(),  # 读取文件中介绍包的详细内容
     include_package_data=True,  # 是否允许上传资源文件
     author='CaoBin',  # 作者
     author_email='bcao@shu.edu.com',  # 作者邮件
     maintainer='CaoBin',  # 维护者
     maintainer_email='binjacobcao@gmail.com',  # 维护者邮件
```

