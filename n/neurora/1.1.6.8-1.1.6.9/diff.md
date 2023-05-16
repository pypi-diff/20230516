# Comparing `tmp/neurora-1.1.6.8.tar.gz` & `tmp/neurora-1.1.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neurora-1.1.6.8.tar", last modified: Sun Sep 11 06:34:51 2022, max compression
+gzip compressed data, was "neurora-1.1.6.9.tar", last modified: Sun Nov 20 03:25:07 2022, max compression
```

## Comparing `neurora-1.1.6.8.tar` & `neurora-1.1.6.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 zitonglu   (501) staff       (20)        0 2022-09-11 06:34:51.703897 neurora-1.1.6.8/
--rwxr-xr-x   0 zitonglu   (501) staff       (20)     1066 2020-12-21 17:20:54.000000 neurora-1.1.6.8/LICENSE
--rw-r--r--   0 zitonglu   (501) staff       (20)     5151 2022-09-11 06:34:51.703189 neurora-1.1.6.8/PKG-INFO
--rwxr-xr-x   0 zitonglu   (501) staff       (20)     4398 2021-12-25 02:14:38.000000 neurora-1.1.6.8/README.md
-drwxr-xr-x   0 zitonglu   (501) staff       (20)        0 2022-09-11 06:34:51.684082 neurora-1.1.6.8/neurora/
--rwxr-xr-x   0 zitonglu   (501) staff       (20)        0 2020-02-04 21:54:44.000000 neurora-1.1.6.8/neurora/__init__.py
--rwxr-xr-x   0 zitonglu   (501) staff       (20)    39334 2021-06-02 08:24:21.000000 neurora-1.1.6.8/neurora/corr_cal.py
--rwxr-xr-x   0 zitonglu   (501) staff       (20)    12071 2021-06-02 08:24:21.000000 neurora-1.1.6.8/neurora/corr_cal_by_rdm.py
--rw-r--r--   0 zitonglu   (501) staff       (20)    24987 2021-12-24 02:09:13.000000 neurora-1.1.6.8/neurora/ctcorr_cal.py
--rw-r--r--   0 zitonglu   (501) staff       (20)     4853 2021-12-24 00:50:55.000000 neurora-1.1.6.8/neurora/ctrdm_cal.py
--rw-r--r--   0 zitonglu   (501) staff       (20)     7218 2021-12-24 01:08:29.000000 neurora-1.1.6.8/neurora/ctrdm_corr.py
--rw-r--r--   0 zitonglu   (501) staff       (20)    81694 2022-08-14 05:04:27.000000 neurora-1.1.6.8/neurora/decoding.py
--rw-r--r--   0 zitonglu   (501) staff       (20)    10345 2021-08-04 19:18:15.000000 neurora-1.1.6.8/neurora/isc_cal.py
--rwxr-xr-x   0 zitonglu   (501) staff       (20)    16613 2021-06-27 07:28:55.000000 neurora-1.1.6.8/neurora/nii_save.py
--rw-r--r--   0 zitonglu   (501) staff       (20)     9782 2021-08-04 19:18:15.000000 neurora-1.1.6.8/neurora/nps_cal.py
--rwxr-xr-x   0 zitonglu   (501) staff       (20)    32727 2022-09-05 15:20:42.000000 neurora-1.1.6.8/neurora/rdm_cal.py
--rwxr-xr-x   0 zitonglu   (501) staff       (20)    15632 2022-08-09 01:20:46.000000 neurora-1.1.6.8/neurora/rdm_corr.py
--rwxr-xr-x   0 zitonglu   (501) staff       (20)    82301 2022-09-11 06:12:59.000000 neurora-1.1.6.8/neurora/rsa_plot.py
--rw-r--r--   0 zitonglu   (501) staff       (20)    17216 2021-08-04 19:36:34.000000 neurora-1.1.6.8/neurora/stats_cal.py
--rw-r--r--   0 zitonglu   (501) staff       (20)    21324 2021-06-02 08:30:50.000000 neurora-1.1.6.8/neurora/stps_cal.py
--rwxr-xr-x   0 zitonglu   (501) staff       (20)    69257 2022-07-17 05:47:44.000000 neurora-1.1.6.8/neurora/stuff.py
-drwxr-xr-x   0 zitonglu   (501) staff       (20)        0 2022-09-11 06:34:51.697230 neurora-1.1.6.8/neurora/template/
--rw-r--r--   0 zitonglu   (501) staff       (20)   171107 2014-03-04 17:20:33.000000 neurora-1.1.6.8/neurora/template/HarvardOxford-cort-maxprob-thr0-1mm.nii.gz
--rwxr-xr-x   0 zitonglu   (501) staff       (20)  3510359 2006-03-07 10:02:04.000000 neurora-1.1.6.8/neurora/template/ch2.nii.gz
--rwxr-xr-x   0 zitonglu   (501) staff       (20)  1329166 2006-03-07 10:00:14.000000 neurora-1.1.6.8/neurora/template/ch2bet.nii.gz
-drwxr-xr-x   0 zitonglu   (501) staff       (20)        0 2022-09-11 06:34:51.687457 neurora-1.1.6.8/neurora.egg-info/
--rw-r--r--   0 zitonglu   (501) staff       (20)     5151 2022-09-11 06:34:50.000000 neurora-1.1.6.8/neurora.egg-info/PKG-INFO
--rw-r--r--   0 zitonglu   (501) staff       (20)      626 2022-09-11 06:34:51.000000 neurora-1.1.6.8/neurora.egg-info/SOURCES.txt
--rw-r--r--   0 zitonglu   (501) staff       (20)        1 2022-09-11 06:34:50.000000 neurora-1.1.6.8/neurora.egg-info/dependency_links.txt
--rw-r--r--   0 zitonglu   (501) staff       (20)       76 2022-09-11 06:34:51.000000 neurora-1.1.6.8/neurora.egg-info/requires.txt
--rw-r--r--   0 zitonglu   (501) staff       (20)        8 2022-09-11 06:34:51.000000 neurora-1.1.6.8/neurora.egg-info/top_level.txt
--rw-r--r--   0 zitonglu   (501) staff       (20)       38 2022-09-11 06:34:51.704157 neurora-1.1.6.8/setup.cfg
--rwxr-xr-x   0 zitonglu   (501) staff       (20)     1172 2022-09-11 06:15:05.000000 neurora-1.1.6.8/setup.py
+drwxr-xr-x   0 zitonglu   (501) staff       (20)        0 2022-11-20 03:25:07.251881 neurora-1.1.6.9/
+-rwxr-xr-x   0 zitonglu   (501) staff       (20)     1066 2020-12-21 17:20:54.000000 neurora-1.1.6.9/LICENSE
+-rw-r--r--   0 zitonglu   (501) staff       (20)     5149 2022-11-20 03:25:07.250959 neurora-1.1.6.9/PKG-INFO
+-rwxr-xr-x   0 zitonglu   (501) staff       (20)     4398 2021-12-25 02:14:38.000000 neurora-1.1.6.9/README.md
+drwxr-xr-x   0 zitonglu   (501) staff       (20)        0 2022-11-20 03:25:07.149422 neurora-1.1.6.9/neurora/
+-rwxr-xr-x   0 zitonglu   (501) staff       (20)        0 2020-02-04 21:54:44.000000 neurora-1.1.6.9/neurora/__init__.py
+-rwxr-xr-x   0 zitonglu   (501) staff       (20)    39334 2021-06-02 08:24:21.000000 neurora-1.1.6.9/neurora/corr_cal.py
+-rwxr-xr-x   0 zitonglu   (501) staff       (20)    12071 2021-06-02 08:24:21.000000 neurora-1.1.6.9/neurora/corr_cal_by_rdm.py
+-rw-r--r--   0 zitonglu   (501) staff       (20)    24987 2021-12-24 02:09:13.000000 neurora-1.1.6.9/neurora/ctcorr_cal.py
+-rw-r--r--   0 zitonglu   (501) staff       (20)     4853 2021-12-24 00:50:55.000000 neurora-1.1.6.9/neurora/ctrdm_cal.py
+-rw-r--r--   0 zitonglu   (501) staff       (20)     7218 2021-12-24 01:08:29.000000 neurora-1.1.6.9/neurora/ctrdm_corr.py
+-rw-r--r--   0 zitonglu   (501) staff       (20)    81694 2022-08-14 05:04:27.000000 neurora-1.1.6.9/neurora/decoding.py
+-rw-r--r--   0 zitonglu   (501) staff       (20)    10345 2021-08-04 19:18:15.000000 neurora-1.1.6.9/neurora/isc_cal.py
+-rwxr-xr-x   0 zitonglu   (501) staff       (20)    16613 2021-06-27 07:28:55.000000 neurora-1.1.6.9/neurora/nii_save.py
+-rw-r--r--   0 zitonglu   (501) staff       (20)     9782 2021-08-04 19:18:15.000000 neurora-1.1.6.9/neurora/nps_cal.py
+-rwxr-xr-x   0 zitonglu   (501) staff       (20)    32738 2022-11-20 03:18:51.000000 neurora-1.1.6.9/neurora/rdm_cal.py
+-rwxr-xr-x   0 zitonglu   (501) staff       (20)    15632 2022-08-09 01:20:46.000000 neurora-1.1.6.9/neurora/rdm_corr.py
+-rwxr-xr-x   0 zitonglu   (501) staff       (20)    82301 2022-09-11 06:12:59.000000 neurora-1.1.6.9/neurora/rsa_plot.py
+-rw-r--r--   0 zitonglu   (501) staff       (20)    17216 2021-08-04 19:36:34.000000 neurora-1.1.6.9/neurora/stats_cal.py
+-rw-r--r--   0 zitonglu   (501) staff       (20)    21324 2021-06-02 08:30:50.000000 neurora-1.1.6.9/neurora/stps_cal.py
+-rwxr-xr-x   0 zitonglu   (501) staff       (20)    69257 2022-07-17 05:47:44.000000 neurora-1.1.6.9/neurora/stuff.py
+drwxr-xr-x   0 zitonglu   (501) staff       (20)        0 2022-11-20 03:25:07.208834 neurora-1.1.6.9/neurora/template/
+-rw-r--r--   0 zitonglu   (501) staff       (20)   171107 2014-03-04 17:20:33.000000 neurora-1.1.6.9/neurora/template/HarvardOxford-cort-maxprob-thr0-1mm.nii.gz
+-rwxr-xr-x   0 zitonglu   (501) staff       (20)  3510359 2006-03-07 10:02:04.000000 neurora-1.1.6.9/neurora/template/ch2.nii.gz
+-rwxr-xr-x   0 zitonglu   (501) staff       (20)  1329166 2006-03-07 10:00:14.000000 neurora-1.1.6.9/neurora/template/ch2bet.nii.gz
+drwxr-xr-x   0 zitonglu   (501) staff       (20)        0 2022-11-20 03:25:07.160746 neurora-1.1.6.9/neurora.egg-info/
+-rw-r--r--   0 zitonglu   (501) staff       (20)     5149 2022-11-20 03:25:06.000000 neurora-1.1.6.9/neurora.egg-info/PKG-INFO
+-rw-r--r--   0 zitonglu   (501) staff       (20)      626 2022-11-20 03:25:06.000000 neurora-1.1.6.9/neurora.egg-info/SOURCES.txt
+-rw-r--r--   0 zitonglu   (501) staff       (20)        1 2022-11-20 03:25:06.000000 neurora-1.1.6.9/neurora.egg-info/dependency_links.txt
+-rw-r--r--   0 zitonglu   (501) staff       (20)       76 2022-11-20 03:25:06.000000 neurora-1.1.6.9/neurora.egg-info/requires.txt
+-rw-r--r--   0 zitonglu   (501) staff       (20)        8 2022-11-20 03:25:06.000000 neurora-1.1.6.9/neurora.egg-info/top_level.txt
+-rw-r--r--   0 zitonglu   (501) staff       (20)       38 2022-11-20 03:25:07.252065 neurora-1.1.6.9/setup.cfg
+-rwxr-xr-x   0 zitonglu   (501) staff       (20)     1172 2022-11-20 03:19:23.000000 neurora-1.1.6.9/setup.py
```

### Comparing `neurora-1.1.6.8/LICENSE` & `neurora-1.1.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `neurora-1.1.6.8/PKG-INFO` & `neurora-1.1.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurora
-Version: 1.1.6.8
+Version: 1.1.6.9
 Summary: A Python Toolbox for Multimodal Neural Data Representation Analysis
 Home-page: https://github.com/ZitongLu1996/NeuroRA
 Author: Zitong Lu
 Author-email: zitonglu1996@gmail.com
 Maintainer: Zitong Lu
 Maintainer-email: zitonglu1996@gmail.com
 License: MIT License
@@ -92,9 +92,7 @@
 **Noteworthily**, this toolbox is currently only a **test version**. 
 If you have any question, find some bugs or have some useful suggestions while using, you can email me and I will be happy and thankful to know.
 >My email address: 
 >zitonglu1996@gmail.com / zitonglu@outlook.com
 
 >My personal homepage:
 >https://zitonglu1996.github.io
-
-
```

### Comparing `neurora-1.1.6.8/README.md` & `neurora-1.1.6.9/README.md`

 * *Files identical despite different names*

### Comparing `neurora-1.1.6.8/neurora/corr_cal.py` & `neurora-1.1.6.9/neurora/corr_cal.py`

 * *Files identical despite different names*

### Comparing `neurora-1.1.6.8/neurora/corr_cal_by_rdm.py` & `neurora-1.1.6.9/neurora/corr_cal_by_rdm.py`

 * *Files identical despite different names*

### Comparing `neurora-1.1.6.8/neurora/ctcorr_cal.py` & `neurora-1.1.6.9/neurora/ctcorr_cal.py`

 * *Files identical despite different names*

### Comparing `neurora-1.1.6.8/neurora/ctrdm_cal.py` & `neurora-1.1.6.9/neurora/ctrdm_cal.py`

 * *Files identical despite different names*

### Comparing `neurora-1.1.6.8/neurora/ctrdm_corr.py` & `neurora-1.1.6.9/neurora/ctrdm_corr.py`

 * *Files identical despite different names*

### Comparing `neurora-1.1.6.8/neurora/decoding.py` & `neurora-1.1.6.9/neurora/decoding.py`

 * *Files identical despite different names*

### Comparing `neurora-1.1.6.8/neurora/isc_cal.py` & `neurora-1.1.6.9/neurora/isc_cal.py`

 * *Files identical despite different names*

### Comparing `neurora-1.1.6.8/neurora/nii_save.py` & `neurora-1.1.6.9/neurora/nii_save.py`

 * *Files identical despite different names*

### Comparing `neurora-1.1.6.8/neurora/nps_cal.py` & `neurora-1.1.6.9/neurora/nps_cal.py`

 * *Files identical despite different names*

### Comparing `neurora-1.1.6.8/neurora/rdm_cal.py` & `neurora-1.1.6.9/neurora/rdm_cal.py`

 * *Files 1% similar despite different names*

```diff
@@ -560,15 +560,15 @@
                 print(data.shape)
                 labels = np.zeros([subs, 2*trials])
                 labels[:, trials:] = 1
                 print(labels.shape)
                 rdms[:, :, con1, con2] = tbyt_decoding_kfold(data, labels, n=2, navg=navg, time_opt=time_opt,
                                                              time_win=time_win, time_step=time_step, nfolds=nfolds,
                                                              nrepeats=nrepeats, normalization=normalization,
-                                                             smooth=True)
+                                                             pca=False, smooth=True)
                 rdms[:, :, con2, con1] = rdms[:, :, con1, con2]
 
     if sub_opt == 0:
 
         return np.average(rdms, axis=0)
 
     else:
```

### Comparing `neurora-1.1.6.8/neurora/rdm_corr.py` & `neurora-1.1.6.9/neurora/rdm_corr.py`

 * *Files identical despite different names*

### Comparing `neurora-1.1.6.8/neurora/rsa_plot.py` & `neurora-1.1.6.9/neurora/rsa_plot.py`

 * *Files identical despite different names*

### Comparing `neurora-1.1.6.8/neurora/stats_cal.py` & `neurora-1.1.6.9/neurora/stats_cal.py`

 * *Files identical despite different names*

### Comparing `neurora-1.1.6.8/neurora/stps_cal.py` & `neurora-1.1.6.9/neurora/stps_cal.py`

 * *Files identical despite different names*

### Comparing `neurora-1.1.6.8/neurora/stuff.py` & `neurora-1.1.6.9/neurora/stuff.py`

 * *Files identical despite different names*

### Comparing `neurora-1.1.6.8/neurora/template/HarvardOxford-cort-maxprob-thr0-1mm.nii.gz` & `neurora-1.1.6.9/neurora/template/HarvardOxford-cort-maxprob-thr0-1mm.nii.gz`

 * *Files identical despite different names*

### Comparing `neurora-1.1.6.8/neurora/template/ch2.nii.gz` & `neurora-1.1.6.9/neurora/template/ch2.nii.gz`

 * *Files identical despite different names*

### Comparing `neurora-1.1.6.8/neurora/template/ch2bet.nii.gz` & `neurora-1.1.6.9/neurora/template/ch2bet.nii.gz`

 * *Files identical despite different names*

### Comparing `neurora-1.1.6.8/neurora.egg-info/PKG-INFO` & `neurora-1.1.6.9/neurora.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurora
-Version: 1.1.6.8
+Version: 1.1.6.9
 Summary: A Python Toolbox for Multimodal Neural Data Representation Analysis
 Home-page: https://github.com/ZitongLu1996/NeuroRA
 Author: Zitong Lu
 Author-email: zitonglu1996@gmail.com
 Maintainer: Zitong Lu
 Maintainer-email: zitonglu1996@gmail.com
 License: MIT License
@@ -92,9 +92,7 @@
 **Noteworthily**, this toolbox is currently only a **test version**. 
 If you have any question, find some bugs or have some useful suggestions while using, you can email me and I will be happy and thankful to know.
 >My email address: 
 >zitonglu1996@gmail.com / zitonglu@outlook.com
 
 >My personal homepage:
 >https://zitonglu1996.github.io
-
-
```

### Comparing `neurora-1.1.6.8/neurora.egg-info/SOURCES.txt` & `neurora-1.1.6.9/neurora.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neurora-1.1.6.8/setup.py` & `neurora-1.1.6.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='neurora',
-    version='1.1.6.8',
+    version='1.1.6.9',
     description=(
         'A Python Toolbox for Multimodal Neural Data Representation Analysis'
     ),
     long_description=open('README.md').read(),
     author='Zitong Lu',
     author_email='zitonglu1996@gmail.com',
     maintainer='Zitong Lu',
```

