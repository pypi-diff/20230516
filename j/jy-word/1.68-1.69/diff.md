# Comparing `tmp/jy-word-1.68.tar.gz` & `tmp/jy-word-1.69.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\jy-word-1.68.tar", last modified: Tue Nov  2 09:23:39 2021, max compression
+gzip compressed data, was "dist\jy-word-1.69.tar", last modified: Tue May 16 03:36:59 2023, max compression
```

## Comparing `jy-word-1.68.tar` & `jy-word-1.69.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2021-11-02 09:23:39.298371 jy-word-1.68/
-drwxrwxrwx   0        0        0        0 2021-11-02 09:23:39.263582 jy-word-1.68/HPPTESTPYTHONPROJECT/
--rw-rw-rw-   0        0        0     3895 2019-08-06 06:28:10.000000 jy-word-1.68/HPPTESTPYTHONPROJECT/TCM_template.py
--rw-rw-rw-   0        0        0     4418 2019-09-29 02:28:23.000000 jy-word-1.68/HPPTESTPYTHONPROJECT/TCM_template_new.py
--rw-rw-rw-   0        0        0      145 2019-03-07 07:22:32.000000 jy-word-1.68/HPPTESTPYTHONPROJECT/__init__.py
--rw-rw-rw-   0        0        0     2224 2019-01-25 05:57:09.000000 jy-word-1.68/HPPTESTPYTHONPROJECT/aip_test.py
--rw-rw-rw-   0        0        0      449 2018-08-14 00:22:40.000000 jy-word-1.68/HPPTESTPYTHONPROJECT/crop_img.py
--rw-rw-rw-   0        0        0     3539 2018-08-14 00:22:40.000000 jy-word-1.68/HPPTESTPYTHONPROJECT/csv2json.py
--rw-rw-rw-   0        0        0     4016 2018-08-24 03:21:16.000000 jy-word-1.68/HPPTESTPYTHONPROJECT/genes.py
--rw-rw-rw-   0        0        0      771 2018-08-14 00:22:40.000000 jy-word-1.68/HPPTESTPYTHONPROJECT/get_pc.py
--rw-rw-rw-   0        0        0     1302 2018-10-17 04:34:58.000000 jy-word-1.68/HPPTESTPYTHONPROJECT/html2img.py
--rw-rw-rw-   0        0        0      956 2019-06-20 09:27:03.000000 jy-word-1.68/HPPTESTPYTHONPROJECT/huankuan.py
--rw-rw-rw-   0        0        0     8163 2019-03-07 07:40:11.000000 jy-word-1.68/HPPTESTPYTHONPROJECT/jy_alipay.py
--rw-rw-rw-   0        0        0     3408 2019-02-15 02:36:10.000000 jy-word-1.68/HPPTESTPYTHONPROJECT/jy_alipay_requests.py
--rw-rw-rw-   0        0        0     3082 2019-03-07 07:38:15.000000 jy-word-1.68/HPPTESTPYTHONPROJECT/jy_paypal.py
--rw-rw-rw-   0        0        0     2797 2019-03-19 09:44:14.000000 jy-word-1.68/HPPTESTPYTHONPROJECT/kuakua.py
--rw-rw-rw-   0        0        0     1889 2019-11-29 08:34:50.000000 jy-word-1.68/HPPTESTPYTHONPROJECT/pdf2img.py
--rw-rw-rw-   0        0        0      997 2019-11-29 08:56:46.000000 jy-word-1.68/HPPTESTPYTHONPROJECT/pdf_test.py
--rw-rw-rw-   0        0        0     9337 2019-11-29 08:54:45.000000 jy-word-1.68/HPPTESTPYTHONPROJECT/pdf_test2.py
--rw-rw-rw-   0        0        0      481 2018-08-14 00:22:40.000000 jy-word-1.68/HPPTESTPYTHONPROJECT/rename_imgs.py
--rw-rw-rw-   0        0        0    34486 2019-06-26 09:27:48.000000 jy-word-1.68/HPPTESTPYTHONPROJECT/tcm_code.py
--rw-rw-rw-   0        0        0    14647 2019-11-20 07:35:05.000000 jy-word-1.68/HPPTESTPYTHONPROJECT/test.py
--rw-rw-rw-   0        0        0      441 2018-09-05 03:54:09.000000 jy-word-1.68/HPPTESTPYTHONPROJECT/test_a.py
--rw-rw-rw-   0        0        0      539 2018-10-11 09:20:34.000000 jy-word-1.68/HPPTESTPYTHONPROJECT/test_barcode.py
--rw-rw-rw-   0        0        0      546 2018-08-22 02:36:34.000000 jy-word-1.68/HPPTESTPYTHONPROJECT/test_maf.py
--rw-rw-rw-   0        0        0      450 2019-11-29 08:58:37.000000 jy-word-1.68/HPPTESTPYTHONPROJECT/test_pdf2img.py
--rw-rw-rw-   0        0        0      948 2018-08-14 00:22:40.000000 jy-word-1.68/HPPTESTPYTHONPROJECT/test_pool.py
--rw-rw-rw-   0        0        0     3339 2020-05-25 02:21:46.000000 jy-word-1.68/HPPTESTPYTHONPROJECT/translate.py
--rw-rw-rw-   0        0        0      583 2019-05-23 03:40:56.000000 jy-word-1.68/HPPTESTPYTHONPROJECT/vern_test.py
--rw-rw-rw-   0        0        0      302 2018-08-14 00:22:40.000000 jy-word-1.68/HPPTESTPYTHONPROJECT/xls_text.py
--rw-rw-rw-   0        0        0      263 2021-11-02 09:23:39.297371 jy-word-1.68/PKG-INFO
-drwxrwxrwx   0        0        0        0 2021-11-02 09:23:39.283371 jy-word-1.68/jy_word/
--rw-rw-rw-   0        0        0     6695 2021-11-02 09:23:36.000000 jy-word-1.68/jy_word/File.py
--rw-rw-rw-   0        0        0     7604 2019-04-01 04:11:45.000000 jy-word-1.68/jy_word/JYFlaskApp.py
--rw-rw-rw-   0        0        0    12693 2019-03-15 05:35:17.000000 jy-word-1.68/jy_word/JYPAY.py
--rw-rw-rw-   0        0        0    44506 2019-12-19 09:41:55.000000 jy-word-1.68/jy_word/Word.py
--rw-rw-rw-   0        0        0      224 2018-08-23 06:36:30.000000 jy-word-1.68/jy_word/__init__.py
--rw-rw-rw-   0        0        0   303631 2019-12-10 06:29:24.000000 jy-word-1.68/jy_word/demo_xml.py
--rw-rw-rw-   0        0        0     2869 2019-11-29 09:25:00.000000 jy-word-1.68/jy_word/pdf2img.py
--rw-rw-rw-   0        0        0    12537 2020-08-12 06:14:24.000000 jy-word-1.68/jy_word/web_tool.py
-drwxrwxrwx   0        0        0        0 2021-11-02 09:23:39.295372 jy-word-1.68/jy_word.egg-info/
--rw-rw-rw-   0        0        0      263 2021-11-02 09:23:38.000000 jy-word-1.68/jy_word.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1261 2021-11-02 09:23:38.000000 jy-word-1.68/jy_word.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-11-02 09:23:38.000000 jy-word-1.68/jy_word.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2021-11-02 09:23:38.000000 jy-word-1.68/jy_word.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2021-11-02 09:23:38.000000 jy-word-1.68/jy_word.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-11-02 09:23:39.300375 jy-word-1.68/setup.cfg
--rw-rw-rw-   0        0        0      596 2021-11-02 09:23:37.000000 jy-word-1.68/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 03:36:59.892235 jy-word-1.69/
+drwxrwxrwx   0        0        0        0 2023-05-16 03:36:59.832195 jy-word-1.69/HPPTESTPYTHONPROJECT/
+-rw-rw-rw-   0        0        0     3895 2019-08-06 06:28:10.000000 jy-word-1.69/HPPTESTPYTHONPROJECT/TCM_template.py
+-rw-rw-rw-   0        0        0     4418 2019-09-29 02:28:23.000000 jy-word-1.69/HPPTESTPYTHONPROJECT/TCM_template_new.py
+-rw-rw-rw-   0        0        0      145 2019-03-07 07:22:32.000000 jy-word-1.69/HPPTESTPYTHONPROJECT/__init__.py
+-rw-rw-rw-   0        0        0     2224 2019-01-25 05:57:09.000000 jy-word-1.69/HPPTESTPYTHONPROJECT/aip_test.py
+-rw-rw-rw-   0        0        0      449 2018-08-14 00:22:40.000000 jy-word-1.69/HPPTESTPYTHONPROJECT/crop_img.py
+-rw-rw-rw-   0        0        0     3539 2018-08-14 00:22:40.000000 jy-word-1.69/HPPTESTPYTHONPROJECT/csv2json.py
+-rw-rw-rw-   0        0        0     4016 2018-08-24 03:21:16.000000 jy-word-1.69/HPPTESTPYTHONPROJECT/genes.py
+-rw-rw-rw-   0        0        0      771 2018-08-14 00:22:40.000000 jy-word-1.69/HPPTESTPYTHONPROJECT/get_pc.py
+-rw-rw-rw-   0        0        0     1302 2018-10-17 04:34:58.000000 jy-word-1.69/HPPTESTPYTHONPROJECT/html2img.py
+-rw-rw-rw-   0        0        0      956 2019-06-20 09:27:03.000000 jy-word-1.69/HPPTESTPYTHONPROJECT/huankuan.py
+-rw-rw-rw-   0        0        0     8163 2019-03-07 07:40:11.000000 jy-word-1.69/HPPTESTPYTHONPROJECT/jy_alipay.py
+-rw-rw-rw-   0        0        0     3408 2019-02-15 02:36:10.000000 jy-word-1.69/HPPTESTPYTHONPROJECT/jy_alipay_requests.py
+-rw-rw-rw-   0        0        0     3082 2019-03-07 07:38:15.000000 jy-word-1.69/HPPTESTPYTHONPROJECT/jy_paypal.py
+-rw-rw-rw-   0        0        0     2797 2019-03-19 09:44:14.000000 jy-word-1.69/HPPTESTPYTHONPROJECT/kuakua.py
+-rw-rw-rw-   0        0        0     1889 2019-11-29 08:34:50.000000 jy-word-1.69/HPPTESTPYTHONPROJECT/pdf2img.py
+-rw-rw-rw-   0        0        0      997 2019-11-29 08:56:46.000000 jy-word-1.69/HPPTESTPYTHONPROJECT/pdf_test.py
+-rw-rw-rw-   0        0        0     9337 2019-11-29 08:54:45.000000 jy-word-1.69/HPPTESTPYTHONPROJECT/pdf_test2.py
+-rw-rw-rw-   0        0        0      481 2018-08-14 00:22:40.000000 jy-word-1.69/HPPTESTPYTHONPROJECT/rename_imgs.py
+-rw-rw-rw-   0        0        0    34486 2019-06-26 09:27:48.000000 jy-word-1.69/HPPTESTPYTHONPROJECT/tcm_code.py
+-rw-rw-rw-   0        0        0    14647 2019-11-20 07:35:05.000000 jy-word-1.69/HPPTESTPYTHONPROJECT/test.py
+-rw-rw-rw-   0        0        0      441 2018-09-05 03:54:09.000000 jy-word-1.69/HPPTESTPYTHONPROJECT/test_a.py
+-rw-rw-rw-   0        0        0      539 2018-10-11 09:20:34.000000 jy-word-1.69/HPPTESTPYTHONPROJECT/test_barcode.py
+-rw-rw-rw-   0        0        0      546 2018-08-22 02:36:34.000000 jy-word-1.69/HPPTESTPYTHONPROJECT/test_maf.py
+-rw-rw-rw-   0        0        0      450 2019-11-29 08:58:37.000000 jy-word-1.69/HPPTESTPYTHONPROJECT/test_pdf2img.py
+-rw-rw-rw-   0        0        0      948 2018-08-14 00:22:40.000000 jy-word-1.69/HPPTESTPYTHONPROJECT/test_pool.py
+-rw-rw-rw-   0        0        0     3339 2020-05-25 02:21:46.000000 jy-word-1.69/HPPTESTPYTHONPROJECT/translate.py
+-rw-rw-rw-   0        0        0      583 2019-05-23 03:40:56.000000 jy-word-1.69/HPPTESTPYTHONPROJECT/vern_test.py
+-rw-rw-rw-   0        0        0      302 2018-08-14 00:22:40.000000 jy-word-1.69/HPPTESTPYTHONPROJECT/xls_text.py
+-rw-rw-rw-   0        0        0      263 2023-05-16 03:36:59.891234 jy-word-1.69/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-16 03:36:59.867200 jy-word-1.69/jy_word/
+-rw-rw-rw-   0        0        0     6695 2021-11-02 09:23:36.000000 jy-word-1.69/jy_word/File.py
+-rw-rw-rw-   0        0        0     7604 2019-04-01 04:11:45.000000 jy-word-1.69/jy_word/JYFlaskApp.py
+-rw-rw-rw-   0        0        0    12693 2019-03-15 05:35:17.000000 jy-word-1.69/jy_word/JYPAY.py
+-rw-rw-rw-   0        0        0    44506 2019-12-19 09:41:55.000000 jy-word-1.69/jy_word/Word.py
+-rw-rw-rw-   0        0        0      224 2018-08-23 06:36:30.000000 jy-word-1.69/jy_word/__init__.py
+-rw-rw-rw-   0        0        0   303631 2019-12-10 06:29:24.000000 jy-word-1.69/jy_word/demo_xml.py
+-rw-rw-rw-   0        0        0     2869 2019-11-29 09:25:00.000000 jy-word-1.69/jy_word/pdf2img.py
+-rw-rw-rw-   0        0        0    12799 2023-05-16 03:36:37.000000 jy-word-1.69/jy_word/web_tool.py
+drwxrwxrwx   0        0        0        0 2023-05-16 03:36:59.886203 jy-word-1.69/jy_word.egg-info/
+-rw-rw-rw-   0        0        0      263 2023-05-16 03:36:59.000000 jy-word-1.69/jy_word.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1261 2023-05-16 03:36:59.000000 jy-word-1.69/jy_word.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 03:36:59.000000 jy-word-1.69/jy_word.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-16 03:36:59.000000 jy-word-1.69/jy_word.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2023-05-16 03:36:59.000000 jy-word-1.69/jy_word.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-16 03:36:59.894234 jy-word-1.69/setup.cfg
+-rw-rw-rw-   0        0        0      596 2023-05-16 03:36:54.000000 jy-word-1.69/setup.py
```

### Comparing `jy-word-1.68/HPPTESTPYTHONPROJECT/TCM_template.py` & `jy-word-1.69/HPPTESTPYTHONPROJECT/TCM_template.py`

 * *Files identical despite different names*

### Comparing `jy-word-1.68/HPPTESTPYTHONPROJECT/TCM_template_new.py` & `jy-word-1.69/HPPTESTPYTHONPROJECT/TCM_template_new.py`

 * *Files identical despite different names*

### Comparing `jy-word-1.68/HPPTESTPYTHONPROJECT/aip_test.py` & `jy-word-1.69/HPPTESTPYTHONPROJECT/aip_test.py`

 * *Files identical despite different names*

### Comparing `jy-word-1.68/HPPTESTPYTHONPROJECT/csv2json.py` & `jy-word-1.69/HPPTESTPYTHONPROJECT/csv2json.py`

 * *Files identical despite different names*

### Comparing `jy-word-1.68/HPPTESTPYTHONPROJECT/genes.py` & `jy-word-1.69/HPPTESTPYTHONPROJECT/genes.py`

 * *Files identical despite different names*

### Comparing `jy-word-1.68/HPPTESTPYTHONPROJECT/get_pc.py` & `jy-word-1.69/HPPTESTPYTHONPROJECT/get_pc.py`

 * *Files identical despite different names*

### Comparing `jy-word-1.68/HPPTESTPYTHONPROJECT/html2img.py` & `jy-word-1.69/HPPTESTPYTHONPROJECT/html2img.py`

 * *Files identical despite different names*

### Comparing `jy-word-1.68/HPPTESTPYTHONPROJECT/huankuan.py` & `jy-word-1.69/HPPTESTPYTHONPROJECT/huankuan.py`

 * *Files identical despite different names*

### Comparing `jy-word-1.68/HPPTESTPYTHONPROJECT/jy_alipay.py` & `jy-word-1.69/HPPTESTPYTHONPROJECT/jy_alipay.py`

 * *Files identical despite different names*

### Comparing `jy-word-1.68/HPPTESTPYTHONPROJECT/jy_alipay_requests.py` & `jy-word-1.69/HPPTESTPYTHONPROJECT/jy_alipay_requests.py`

 * *Files identical despite different names*

### Comparing `jy-word-1.68/HPPTESTPYTHONPROJECT/jy_paypal.py` & `jy-word-1.69/HPPTESTPYTHONPROJECT/jy_paypal.py`

 * *Files identical despite different names*

### Comparing `jy-word-1.68/HPPTESTPYTHONPROJECT/kuakua.py` & `jy-word-1.69/HPPTESTPYTHONPROJECT/kuakua.py`

 * *Files identical despite different names*

### Comparing `jy-word-1.68/HPPTESTPYTHONPROJECT/pdf2img.py` & `jy-word-1.69/HPPTESTPYTHONPROJECT/pdf2img.py`

 * *Files identical despite different names*

### Comparing `jy-word-1.68/HPPTESTPYTHONPROJECT/pdf_test.py` & `jy-word-1.69/HPPTESTPYTHONPROJECT/pdf_test.py`

 * *Files identical despite different names*

### Comparing `jy-word-1.68/HPPTESTPYTHONPROJECT/pdf_test2.py` & `jy-word-1.69/HPPTESTPYTHONPROJECT/pdf_test2.py`

 * *Files identical despite different names*

### Comparing `jy-word-1.68/HPPTESTPYTHONPROJECT/tcm_code.py` & `jy-word-1.69/HPPTESTPYTHONPROJECT/tcm_code.py`

 * *Files identical despite different names*

### Comparing `jy-word-1.68/HPPTESTPYTHONPROJECT/test.py` & `jy-word-1.69/HPPTESTPYTHONPROJECT/test.py`

 * *Files identical despite different names*

### Comparing `jy-word-1.68/HPPTESTPYTHONPROJECT/test_barcode.py` & `jy-word-1.69/HPPTESTPYTHONPROJECT/test_barcode.py`

 * *Files identical despite different names*

### Comparing `jy-word-1.68/HPPTESTPYTHONPROJECT/test_maf.py` & `jy-word-1.69/HPPTESTPYTHONPROJECT/test_maf.py`

 * *Files identical despite different names*

### Comparing `jy-word-1.68/HPPTESTPYTHONPROJECT/test_pool.py` & `jy-word-1.69/HPPTESTPYTHONPROJECT/test_pool.py`

 * *Files identical despite different names*

### Comparing `jy-word-1.68/HPPTESTPYTHONPROJECT/translate.py` & `jy-word-1.69/HPPTESTPYTHONPROJECT/translate.py`

 * *Files identical despite different names*

### Comparing `jy-word-1.68/HPPTESTPYTHONPROJECT/vern_test.py` & `jy-word-1.69/HPPTESTPYTHONPROJECT/vern_test.py`

 * *Files identical despite different names*

### Comparing `jy-word-1.68/jy_word/File.py` & `jy-word-1.69/jy_word/File.py`

 * *Files identical despite different names*

### Comparing `jy-word-1.68/jy_word/JYFlaskApp.py` & `jy-word-1.69/jy_word/JYFlaskApp.py`

 * *Files identical despite different names*

### Comparing `jy-word-1.68/jy_word/JYPAY.py` & `jy-word-1.69/jy_word/JYPAY.py`

 * *Files identical despite different names*

### Comparing `jy-word-1.68/jy_word/Word.py` & `jy-word-1.69/jy_word/Word.py`

 * *Files identical despite different names*

### Comparing `jy-word-1.68/jy_word/demo_xml.py` & `jy-word-1.69/jy_word/demo_xml.py`

 * *Files identical despite different names*

### Comparing `jy-word-1.68/jy_word/pdf2img.py` & `jy-word-1.69/jy_word/pdf2img.py`

 * *Files identical despite different names*

### Comparing `jy-word-1.68/jy_word/web_tool.py` & `jy-word-1.69/jy_word/web_tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,21 @@
     #Get file(s) to zip ...
     if os.path.isfile(dirname):
         file_list.append(dirname)
         dirname = os.path.dirname(dirname)
     elif os.path.isdir(dirname):
         #get all file in directory
         for filename in os.listdir(dirname):
-            file_list.append(os.path.join(dirname, filename))
+            path = os.path.join(dirname, filename)
+            if os.path.isfile(path):
+                file_list.append(path)
+            elif os.path.isdir(path):
+                for filename1 in os.listdir(path):
+                    path1 = os.path.join(path, filename1)
+                    file_list.append(path1)
 
     #Start to zip file ...
     destZip = zipfile.ZipFile(fullzipfilename, "w")
     i = 0
     for eachfile in file_list:
         destfile = eachfile[len(dirname):]
         print "Zip file %s..." % destfile
```

### Comparing `jy-word-1.68/jy_word.egg-info/SOURCES.txt` & `jy-word-1.69/jy_word.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jy-word-1.68/setup.py` & `jy-word-1.69/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # !/usr/bin/python
 # Create Date 2018/6/4 0004
 __author__ = 'huohuo'
 from setuptools import setup, find_packages
 
 setup(
     name='jy-word',
-    version='1.68',
+    version='1.69',
     keywords=('word', 'test'),
     description='generate word',
     license='MIT License',
     author='hp910219',
     author_email='hp910219@126.com',
     url='https://github.com/hp910219/jy-word.git',
     packages=find_packages(exclude=['test']),
```

