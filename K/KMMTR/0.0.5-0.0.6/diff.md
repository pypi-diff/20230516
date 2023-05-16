# Comparing `tmp/KMMTR-0.0.5.tar.gz` & `tmp/KMMTR-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KMMTR-0.0.5.tar", last modified: Mon May 15 09:10:49 2023, max compression
+gzip compressed data, was "KMMTR-0.0.6.tar", last modified: Mon May 15 11:33:23 2023, max compression
```

## Comparing `KMMTR-0.0.5.tar` & `KMMTR-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-15 09:10:49.884701 KMMTR-0.0.5/
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-15 09:10:49.883771 KMMTR-0.0.5/KMMTR/
--rwxr-xr-x   0 jacob      (501) staff       (20)     6612 2023-05-15 09:10:13.000000 KMMTR-0.0.5/KMMTR/KMM.py
--rwxr-xr-x   0 jacob      (501) staff       (20)     6511 2023-05-03 02:58:16.000000 KMMTR-0.0.5/KMMTR/KMMTR.py
--rwxr-xr-x   0 jacob      (501) staff       (20)      386 2023-04-19 10:18:26.000000 KMMTR-0.0.5/KMMTR/__init__.py
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-15 09:10:49.884402 KMMTR-0.0.5/KMMTR.egg-info/
--rw-r--r--   0 jacob      (501) staff       (20)     1453 2023-05-15 09:10:49.000000 KMMTR-0.0.5/KMMTR.egg-info/PKG-INFO
--rw-r--r--   0 jacob      (501) staff       (20)      208 2023-05-15 09:10:49.000000 KMMTR-0.0.5/KMMTR.egg-info/SOURCES.txt
--rw-r--r--   0 jacob      (501) staff       (20)        1 2023-05-15 09:10:49.000000 KMMTR-0.0.5/KMMTR.egg-info/dependency_links.txt
--rw-r--r--   0 jacob      (501) staff       (20)       33 2023-05-15 09:10:49.000000 KMMTR-0.0.5/KMMTR.egg-info/requires.txt
--rw-r--r--   0 jacob      (501) staff       (20)        6 2023-05-15 09:10:49.000000 KMMTR-0.0.5/KMMTR.egg-info/top_level.txt
--rw-r--r--   0 jacob      (501) staff       (20)     1453 2023-05-15 09:10:49.884565 KMMTR-0.0.5/PKG-INFO
--rw-r--r--   0 jacob      (501) staff       (20)      859 2023-04-20 09:04:07.000000 KMMTR-0.0.5/README.md
--rw-r--r--   0 jacob      (501) staff       (20)       38 2023-05-15 09:10:49.884739 KMMTR-0.0.5/setup.cfg
--rw-r--r--   0 jacob      (501) staff       (20)     1381 2023-05-15 09:10:37.000000 KMMTR-0.0.5/setup.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-15 11:33:23.785771 KMMTR-0.0.6/
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-15 11:33:23.784884 KMMTR-0.0.6/KMMTR/
+-rwxr-xr-x   0 jacob      (501) staff       (20)     6643 2023-05-15 11:31:46.000000 KMMTR-0.0.6/KMMTR/KMM.py
+-rwxr-xr-x   0 jacob      (501) staff       (20)     6510 2023-05-15 11:32:03.000000 KMMTR-0.0.6/KMMTR/KMMTR.py
+-rwxr-xr-x   0 jacob      (501) staff       (20)      386 2023-04-19 10:18:26.000000 KMMTR-0.0.6/KMMTR/__init__.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-15 11:33:23.785473 KMMTR-0.0.6/KMMTR.egg-info/
+-rw-r--r--   0 jacob      (501) staff       (20)     1453 2023-05-15 11:33:23.000000 KMMTR-0.0.6/KMMTR.egg-info/PKG-INFO
+-rw-r--r--   0 jacob      (501) staff       (20)      208 2023-05-15 11:33:23.000000 KMMTR-0.0.6/KMMTR.egg-info/SOURCES.txt
+-rw-r--r--   0 jacob      (501) staff       (20)        1 2023-05-15 11:33:23.000000 KMMTR-0.0.6/KMMTR.egg-info/dependency_links.txt
+-rw-r--r--   0 jacob      (501) staff       (20)       33 2023-05-15 11:33:23.000000 KMMTR-0.0.6/KMMTR.egg-info/requires.txt
+-rw-r--r--   0 jacob      (501) staff       (20)        6 2023-05-15 11:33:23.000000 KMMTR-0.0.6/KMMTR.egg-info/top_level.txt
+-rw-r--r--   0 jacob      (501) staff       (20)     1453 2023-05-15 11:33:23.785638 KMMTR-0.0.6/PKG-INFO
+-rw-r--r--   0 jacob      (501) staff       (20)      859 2023-04-20 09:04:07.000000 KMMTR-0.0.6/README.md
+-rw-r--r--   0 jacob      (501) staff       (20)       38 2023-05-15 11:33:23.785813 KMMTR-0.0.6/setup.cfg
+-rw-r--r--   0 jacob      (501) staff       (20)     1381 2023-05-15 11:33:11.000000 KMMTR-0.0.6/setup.py
```

### Comparing `KMMTR-0.0.5/KMMTR/KMM.py` & `KMMTR-0.0.6/KMMTR/KMM.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,20 +70,21 @@
         
         Returns:
             An instantiated kernel function object.
         """
         Xtrain = np.array(self.target_data)
         Ytrain = np.array(self.target_response)
         ker = self.call_kernel()
-        noise_ker = WhiteKernel(noise_level_bounds=(0.01,1))
+        noise_ker = WhiteKernel(noise_level_bounds=(0.01,0.5))
         # cal the data nosie by maximazing the likelihood 
-        GPr = GPR(kernel=ker+noise_ker).fit(Xtrain[:-int(0.8*len(Xtrain)),:],Ytrain[:-int(0.8*len(Xtrain)),:])
+        GPr = GPR(kernel=ker+noise_ker,normalize_y=True).fit(Xtrain,Ytrain)
         noise_level = np.exp(GPr.kernel_.theta[1])
+        print('Trained noise is %f' % noise_level)
 
-        GPr_fit = GPR(kernel=ker, alpha = noise_level).fit(Xtrain,Ytrain)
+        GPr_fit = GPR(kernel=ker, alpha = noise_level,normalize_y=True).fit(Xtrain,Ytrain)
         print('Trained Kernel Function :', GPr_fit.kernel_)
         para = np.exp(GPr_fit.kernel_.theta)
 
         Inst_kernel = self.call_kernel(para)
         return Inst_kernel
 
 
@@ -156,17 +157,15 @@
         M_G1_U = copy.deepcopy(matrix(M_G1))
         M_G2_U = copy.deepcopy(matrix(M_G2))
         M_A1 = matrix(M_A1)
         M_A2 = matrix(M_A2)
         V_h1_U = copy.deepcopy(matrix(V_h1))
         V_h2_U = copy.deepcopy(matrix(V_h2))
         M_G = matrix(np.r_[M_G1_U, M_G2_U,M_A1,M_A2])
-        h1 = matrix(1+tao)
-        h2 = matrix(tao-1)
+        h1 = matrix(0.99+tao)
+        h2 = matrix(tao-0.99)
         h = matrix(np.r_[V_h1_U, V_h2_U,h1,h2])
 
-        
-
         solvers.options['show_progress'] = True
         sol = solvers.qp(M_P,V_q,M_G,h)
         beta = sol['x']
         return np.array(beta)
```

### Comparing `KMMTR-0.0.5/KMMTR/KMMTR.py` & `KMMTR-0.0.6/KMMTR/KMMTR.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,14 @@
         check_weight(self.Regressor.fit)
 
         data_weight = np.concatenate(
             (beta,np.ones(
                 (len(target_data),1)
                         )))
 
-
         return self.Regressor.fit(X,Y, sample_weight = data_weight.flatten()).predict(test_data), beta.flatten()
 
 
 def check_attributes(estimator, attribute_list):
     for attribute in attribute_list:
         if hasattr(estimator, attribute) :
             print(f"The estimator has a {attribute} attribute.")
```

### Comparing `KMMTR-0.0.5/KMMTR.egg-info/PKG-INFO` & `KMMTR-0.0.6/KMMTR.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KMMTR
-Version: 0.0.5
+Version: 0.0.6
 Summary: a transfer learning regression model based on Kernel Mean Matching (KMM) algorithm
 Home-page: https://github.com/Bin-Cao/KMMTransferRegressor
 Author: CaoBin
 Author-email: bcao@shu.edu.com
 Maintainer: CaoBin
 Maintainer-email: binjacobcao@gmail.com
 License: MIT License
```

### Comparing `KMMTR-0.0.5/PKG-INFO` & `KMMTR-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KMMTR
-Version: 0.0.5
+Version: 0.0.6
 Summary: a transfer learning regression model based on Kernel Mean Matching (KMM) algorithm
 Home-page: https://github.com/Bin-Cao/KMMTransferRegressor
 Author: CaoBin
 Author-email: bcao@shu.edu.com
 Maintainer: CaoBin
 Maintainer-email: binjacobcao@gmail.com
 License: MIT License
```

### Comparing `KMMTR-0.0.5/README.md` & `KMMTR-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `KMMTR-0.0.5/setup.py` & `KMMTR-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name='KMMTR',  # 包名
-    version='0.0.5',  # 版本
+    version='0.0.6',  # 版本
     description="a transfer learning regression model based on Kernel Mean Matching (KMM) algorithm",  # 包简介
     long_description=open('README.md',encoding='utf-8').read(),  # 读取文件中介绍包的详细内容
     include_package_data=True,  # 是否允许上传资源文件
     author='CaoBin',  # 作者
     author_email='bcao@shu.edu.com',  # 作者邮件
     maintainer='CaoBin',  # 维护者
     maintainer_email='binjacobcao@gmail.com',  # 维护者邮件
```

