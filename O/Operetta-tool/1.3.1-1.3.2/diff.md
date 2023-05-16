# Comparing `tmp/Operetta_tool-1.3.1.tar.gz` & `tmp/Operetta_tool-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Operetta_tool-1.3.1.tar", last modified: Mon May 15 20:49:43 2023, max compression
+gzip compressed data, was "Operetta_tool-1.3.2.tar", last modified: Tue May 16 08:59:42 2023, max compression
```

## Comparing `Operetta_tool-1.3.1.tar` & `Operetta_tool-1.3.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 20:49:43.933744 Operetta_tool-1.3.1/
--rw-rw-rw-   0        0        0     1104 2022-01-09 13:54:52.000000 Operetta_tool-1.3.1/LICENSE
--rw-rw-rw-   0        0        0       28 2023-03-16 18:37:03.000000 Operetta_tool-1.3.1/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-05-15 20:49:43.933744 Operetta_tool-1.3.1/Operetta_tool.egg-info/
--rw-rw-rw-   0        0        0      725 2023-05-15 20:49:43.000000 Operetta_tool-1.3.1/Operetta_tool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2023-05-15 20:49:43.000000 Operetta_tool-1.3.1/Operetta_tool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 20:49:43.000000 Operetta_tool-1.3.1/Operetta_tool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      108 2023-05-15 20:49:43.000000 Operetta_tool-1.3.1/Operetta_tool.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-15 20:49:43.000000 Operetta_tool-1.3.1/Operetta_tool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      725 2023-05-15 20:49:43.933744 Operetta_tool-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0    11126 2023-03-20 21:02:31.000000 Operetta_tool-1.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 20:49:43.933744 Operetta_tool-1.3.1/operetta/
--rw-rw-rw-   0        0        0      153 2023-05-15 20:49:11.000000 Operetta_tool-1.3.1/operetta/__init__.py
--rw-rw-rw-   0        0        0   261950 2023-03-14 17:41:39.000000 Operetta_tool-1.3.1/operetta/jbsicon.ico
--rw-rw-rw-   0        0        0    47619 2023-05-15 20:48:35.000000 Operetta_tool-1.3.1/operetta/operetta_annotation.py
--rw-rw-rw-   0        0        0       42 2023-05-15 20:49:43.933744 Operetta_tool-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1276 2023-05-15 20:49:18.000000 Operetta_tool-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 08:59:42.812489 Operetta_tool-1.3.2/
+-rw-rw-rw-   0        0        0     1104 2022-01-09 13:54:52.000000 Operetta_tool-1.3.2/LICENSE
+-rw-rw-rw-   0        0        0       28 2023-03-16 18:37:03.000000 Operetta_tool-1.3.2/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-05-16 08:59:42.807466 Operetta_tool-1.3.2/Operetta_tool.egg-info/
+-rw-rw-rw-   0        0        0      725 2023-05-16 08:59:42.000000 Operetta_tool-1.3.2/Operetta_tool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2023-05-16 08:59:42.000000 Operetta_tool-1.3.2/Operetta_tool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 08:59:42.000000 Operetta_tool-1.3.2/Operetta_tool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2023-05-16 08:59:42.000000 Operetta_tool-1.3.2/Operetta_tool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-16 08:59:42.000000 Operetta_tool-1.3.2/Operetta_tool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      725 2023-05-16 08:59:42.811491 Operetta_tool-1.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0    11126 2023-03-20 21:02:31.000000 Operetta_tool-1.3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-16 08:59:42.810477 Operetta_tool-1.3.2/operetta/
+-rw-rw-rw-   0        0        0      153 2023-05-16 08:58:53.000000 Operetta_tool-1.3.2/operetta/__init__.py
+-rw-rw-rw-   0        0        0   261950 2023-03-14 17:41:39.000000 Operetta_tool-1.3.2/operetta/jbsicon.ico
+-rw-rw-rw-   0        0        0    48388 2023-05-16 08:50:32.000000 Operetta_tool-1.3.2/operetta/operetta_annotation.py
+-rw-rw-rw-   0        0        0       42 2023-05-16 08:59:42.812489 Operetta_tool-1.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     1276 2023-05-16 08:58:51.000000 Operetta_tool-1.3.2/setup.py
```

### Comparing `Operetta_tool-1.3.1/LICENSE` & `Operetta_tool-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Operetta_tool-1.3.1/Operetta_tool.egg-info/PKG-INFO` & `Operetta_tool-1.3.2/Operetta_tool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Operetta-tool
-Version: 1.3.1
+Version: 1.3.2
 Summary: operetta_tool
 Author: Jakub Kubis
 Author-email: jbiosystem@gmail.com
 License: MIT
 Keywords: python,opera,images,annotation,AI,cv,perkin
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Operetta_tool-1.3.1/PKG-INFO` & `Operetta_tool-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Operetta_tool
-Version: 1.3.1
+Version: 1.3.2
 Summary: operetta_tool
 Author: Jakub Kubis
 Author-email: jbiosystem@gmail.com
 License: MIT
 Keywords: python,opera,images,annotation,AI,cv,perkin
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Operetta_tool-1.3.1/README.md` & `Operetta_tool-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `Operetta_tool-1.3.1/operetta/jbsicon.ico` & `Operetta_tool-1.3.2/operetta/jbsicon.ico`

 * *Files identical despite different names*

### Comparing `Operetta_tool-1.3.1/operetta/operetta_annotation.py` & `Operetta_tool-1.3.2/operetta/operetta_annotation.py`

 * *Files 2% similar despite different names*

```diff
@@ -456,15 +456,16 @@
             images_tmp2.close()
             
             del data
             
             os.remove(os.path.join(path_to_images, 'images2.h5'))
             
     except:
-        print("Something went wrong. Check the function input data and try again!")
+        print("Something went wrong. Check the function input data and try again! \nCheck that the number of channels you want to assemble matches the number of data channels!")
+
 
 
 
 
 def z_projection(path_to_tiff:str, stack_check:str):
 
     if not os.path.exists(path_to_tiff):
@@ -508,15 +509,15 @@
         
             # calculate the z-score for each pixel
             z_score = abs(stack - mean_zstack) / std_zstack
             
             del mean_zstack, std_zstack
         
             # identify pixels with z-scores above the threshold
-            stack[(z_score > 2.5) | (z_score < -2.5)] = np.nan
+            stack[(z_score > 2.5) | (z_score < -2.5)] = -999
             
             del z_score
         
         stack = stack.astype(np.uint64)  
         
         for n, d in enumerate(stack):   
             stack[n] = (stack[n] / np.mean(stack[n])) * (((2**16)-1) /  np.log(np.mean(stack[n])))
@@ -640,23 +641,38 @@
         
         def active_changes():
                 
                
                 global img_gamma
                 
                 if projections_type.get() == 'avg':
-                    img = np.nanmean(stack, axis=0).astype(np.uint16)      
+                    mask = stack == -999  
+                    img = np.ma.masked_array(stack, mask=mask)  
+                    img = np.mean(img, axis=0).astype(np.uint16) 
+                    del mask
                 elif projections_type.get() == 'max':
-                    img = np.max(stack, axis=0).astype(np.uint16)    
+                    mask = stack == -999  
+                    img = np.ma.masked_array(stack, mask=mask)  
+                    img = np.max(img, axis=0).astype(np.uint16)  
+                    del mask
                 elif projections_type.get() == 'min':
-                    img = np.min(stack, axis=0).astype(np.uint16)    
+                    mask = stack == -999  
+                    img = np.ma.masked_array(stack, mask=mask)  
+                    img = np.min(img, axis=0).astype(np.uint16)
+                    del mask
                 elif projections_type.get() == 'std':
-                    img = np.std(stack, axis=0).astype(np.uint16)    
+                    mask = stack == -999  
+                    img = np.ma.masked_array(stack, mask=mask)  
+                    img = np.std(img, axis=0).astype(np.uint16) 
+                    del mask
                 elif projections_type.get() == 'median':
-                    img = np.median(stack, axis=0).astype(np.uint16)    
+                    mask = stack == -999  
+                    img = np.ma.masked_array(stack, mask=mask)  
+                    img = np.median(img, axis=0).astype(np.uint16)    
+                    del mask
                
                 
                 img = img.astype(np.int64)
                 
                 color = combobox.get()
                 
     
@@ -810,14 +826,15 @@
         return img_gamma
 
 
 
 
 
 
+
 def merge_images(image_list:list):
     
     try:
     
         intensity_factors = []
         for bt in range(len(image_list)):
             intensity_factors.append(1)
```

### Comparing `Operetta_tool-1.3.1/setup.py` & `Operetta_tool-1.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.3.1' 
+VERSION = '1.3.2' 
 DESCRIPTION = 'operetta_tool'
 LONG_DESCRIPTION = 'The Operetta_tool is a python library created for handling and annotation images from the Opera Phenix platform used for ML / AI applications. Instructions for use on github [https://github.com/jkubis96/Operetta_tool] '
 
 # Setting up
 setup(
         name="Operetta_tool", 
         version=VERSION,
```

