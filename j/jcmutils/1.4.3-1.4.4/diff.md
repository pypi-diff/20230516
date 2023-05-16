# Comparing `tmp/jcmutils-1.4.3.tar.gz` & `tmp/jcmutils-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jcmutils-1.4.3.tar", last modified: Tue May 16 07:28:09 2023, max compression
+gzip compressed data, was "jcmutils-1.4.4.tar", last modified: Tue May 16 10:56:29 2023, max compression
```

## Comparing `jcmutils-1.4.3.tar` & `jcmutils-1.4.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-05-16 07:28:09.165178 jcmutils-1.4.3/
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     1073 2023-04-15 12:55:54.000000 jcmutils-1.4.3/LICENSE
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-05-16 07:28:09.165178 jcmutils-1.4.3/PKG-INFO
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     3044 2023-04-15 12:55:54.000000 jcmutils-1.4.3/README.md
-drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-05-16 07:28:09.165178 jcmutils-1.4.3/jcmutils/
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      165 2023-04-18 07:48:21.000000 jcmutils-1.4.3/jcmutils/__init__.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     6777 2023-05-16 07:27:18.000000 jcmutils-1.4.3/jcmutils/dataset_utils.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     2151 2023-04-15 12:55:54.000000 jcmutils-1.4.3/jcmutils/gen_sources.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     1496 2023-04-15 12:55:54.000000 jcmutils-1.4.3/jcmutils/logger.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     8780 2023-05-11 10:05:05.000000 jcmutils-1.4.3/jcmutils/solver.py
-drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-05-16 07:28:09.165178 jcmutils-1.4.3/jcmutils.egg-info/
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-05-16 07:28:09.000000 jcmutils-1.4.3/jcmutils.egg-info/PKG-INFO
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      294 2023-05-16 07:28:09.000000 jcmutils-1.4.3/jcmutils.egg-info/SOURCES.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)        1 2023-05-16 07:28:09.000000 jcmutils-1.4.3/jcmutils.egg-info/dependency_links.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-05-16 07:28:09.000000 jcmutils-1.4.3/jcmutils.egg-info/requires.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)        9 2023-05-16 07:28:09.000000 jcmutils-1.4.3/jcmutils.egg-info/top_level.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-05-16 07:28:09.165178 jcmutils-1.4.3/setup.cfg
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      539 2023-05-16 07:27:37.000000 jcmutils-1.4.3/setup.py
+drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-05-16 10:56:29.145059 jcmutils-1.4.4/
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     1073 2023-04-15 12:55:54.000000 jcmutils-1.4.4/LICENSE
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-05-16 10:56:29.145059 jcmutils-1.4.4/PKG-INFO
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     3044 2023-04-15 12:55:54.000000 jcmutils-1.4.4/README.md
+drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-05-16 10:56:29.145059 jcmutils-1.4.4/jcmutils/
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      165 2023-04-18 07:48:21.000000 jcmutils-1.4.4/jcmutils/__init__.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     6783 2023-05-16 10:56:06.000000 jcmutils-1.4.4/jcmutils/dataset_utils.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     2151 2023-04-15 12:55:54.000000 jcmutils-1.4.4/jcmutils/gen_sources.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     1496 2023-04-15 12:55:54.000000 jcmutils-1.4.4/jcmutils/logger.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     8780 2023-05-11 10:05:05.000000 jcmutils-1.4.4/jcmutils/solver.py
+drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-05-16 10:56:29.145059 jcmutils-1.4.4/jcmutils.egg-info/
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-05-16 10:56:29.000000 jcmutils-1.4.4/jcmutils.egg-info/PKG-INFO
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      294 2023-05-16 10:56:29.000000 jcmutils-1.4.4/jcmutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)        1 2023-05-16 10:56:29.000000 jcmutils-1.4.4/jcmutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-05-16 10:56:29.000000 jcmutils-1.4.4/jcmutils.egg-info/requires.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)        9 2023-05-16 10:56:29.000000 jcmutils-1.4.4/jcmutils.egg-info/top_level.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-05-16 10:56:29.145059 jcmutils-1.4.4/setup.cfg
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      539 2023-05-16 10:56:12.000000 jcmutils-1.4.4/setup.py
```

### Comparing `jcmutils-1.4.3/LICENSE` & `jcmutils-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jcmutils-1.4.3/README.md` & `jcmutils-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `jcmutils-1.4.3/jcmutils/dataset_utils.py` & `jcmutils-1.4.4/jcmutils/dataset_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,16 +77,16 @@
         
         # 合并最终结果
         vmaxa = np.max(total_results) if vmax is None else vmax
         afield = (total_results/ vmaxa)*235
         afield = np.rot90(afield)
 
         # 确定缺陷在原始图像中的位置
-        xpos = self.keys['defectpos'][0] * 1.0/( origin_size['x'][1] - origin_size['x'][0]) * origin_image_size[0]
-        ypos = origin_image_size-(self.keys['defectpos'][1] * 1.0/(origin_size['y'][1] - origin_size['y'][0]) * origin_image_size[1])
+        xpos = self.keys[0]['defectpos'][0] * 1.0/( origin_size['x'][1] - origin_size['x'][0]) * origin_image_size[0]
+        ypos = origin_image_size-(self.keys[0]['defectpos'][1] * 1.0/(origin_size['y'][1] - origin_size['y'][0]) * origin_image_size[1])
         roi = np.ceil([xpos - defect_size*1.0/source_density,xpos + defect_size*1.0/source_density,ypos - defect_size*1.0/source_density,ypos+defect_size*1.0/source_density])
 
         # 保存
         defect_image = afield
         output_image = template_image
         output_image[roi[0]:roi[1],roi[2]:roi[3]] = defect_image[roi[0]:roi[1],roi[2]:roi[3]]
         label_name = target_filename + ".txt"
```

### Comparing `jcmutils-1.4.3/jcmutils/gen_sources.py` & `jcmutils-1.4.4/jcmutils/gen_sources.py`

 * *Files identical despite different names*

### Comparing `jcmutils-1.4.3/jcmutils/logger.py` & `jcmutils-1.4.4/jcmutils/logger.py`

 * *Files identical despite different names*

### Comparing `jcmutils-1.4.3/jcmutils/solver.py` & `jcmutils-1.4.4/jcmutils/solver.py`

 * *Files identical despite different names*

### Comparing `jcmutils-1.4.3/setup.py` & `jcmutils-1.4.4/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup,find_packages
 
-VERSION = '1.4.3'
+VERSION = '1.4.4'
 DESCRIPTION = "A general utils for jcmsuite"
 
 setup(
     name="jcmutils",
     version=VERSION,
     author="crafter-z",
     author_email="crafterz@163.com",
```

