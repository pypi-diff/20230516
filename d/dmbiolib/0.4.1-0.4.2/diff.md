# Comparing `tmp/dmbiolib-0.4.1.tar.gz` & `tmp/dmbiolib-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dmbiolib-0.4.1.tar", last modified: Tue May 16 06:53:06 2023, max compression
+gzip compressed data, was "dmbiolib-0.4.2.tar", last modified: Tue May 16 08:31:04 2023, max compression
```

## Comparing `dmbiolib-0.4.1.tar` & `dmbiolib-0.4.2.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxrwxrwx   0 daming    (1000) daming    (1000)        0 2023-05-16 06:53:03.113356 dmbiolib-0.4.1/
--rwxrwxrwx   0 daming    (1000) daming    (1000)    35802 2022-04-11 07:19:36.000000 dmbiolib-0.4.1/LICENSE
--rwxrwxrwx   0 daming    (1000) daming    (1000)     1224 2023-05-16 06:53:03.110356 dmbiolib-0.4.1/PKG-INFO
--rwxrwxrwx   0 daming    (1000) daming    (1000)      649 2023-02-08 06:46:06.000000 dmbiolib-0.4.1/README.md
-drwxrwxrwx   0 daming    (1000) daming    (1000)        0 2023-05-16 06:53:03.012354 dmbiolib-0.4.1/dmbiolib/
-drwxrwxrwx   0 daming    (1000) daming    (1000)        0 2023-05-16 06:53:03.089354 dmbiolib-0.4.1/dmbiolib/dmbiolib.egg-info/
--rwxrwxrwx   0 daming    (1000) daming    (1000)     1224 2023-05-16 06:53:02.000000 dmbiolib-0.4.1/dmbiolib/dmbiolib.egg-info/PKG-INFO
--rwxrwxrwx   0 daming    (1000) daming    (1000)      211 2023-05-16 06:53:02.000000 dmbiolib-0.4.1/dmbiolib/dmbiolib.egg-info/SOURCES.txt
--rwxrwxrwx   0 daming    (1000) daming    (1000)        1 2023-05-16 06:53:02.000000 dmbiolib-0.4.1/dmbiolib/dmbiolib.egg-info/dependency_links.txt
--rwxrwxrwx   0 daming    (1000) daming    (1000)        9 2023-05-16 06:53:02.000000 dmbiolib-0.4.1/dmbiolib/dmbiolib.egg-info/top_level.txt
--rwxrwxrwx   0 daming    (1000) daming    (1000)    23179 2023-05-16 06:50:38.000000 dmbiolib-0.4.1/dmbiolib/dmbiolib.py
--rwxrwxrwx   0 daming    (1000) daming    (1000)       38 2023-05-16 06:53:03.114356 dmbiolib-0.4.1/setup.cfg
--rwxrwxrwx   0 daming    (1000) daming    (1000)      928 2023-05-16 06:51:05.000000 dmbiolib-0.4.1/setup.py
+drwxrwxrwx   0 daming    (1000) daming    (1000)        0 2023-05-16 08:31:01.321851 dmbiolib-0.4.2/
+-rwxrwxrwx   0 daming    (1000) daming    (1000)    35802 2022-04-11 07:19:36.000000 dmbiolib-0.4.2/LICENSE
+-rwxrwxrwx   0 daming    (1000) daming    (1000)     1224 2023-05-16 08:31:01.318850 dmbiolib-0.4.2/PKG-INFO
+-rwxrwxrwx   0 daming    (1000) daming    (1000)      649 2023-02-08 06:46:06.000000 dmbiolib-0.4.2/README.md
+drwxrwxrwx   0 daming    (1000) daming    (1000)        0 2023-05-16 08:31:01.229849 dmbiolib-0.4.2/dmbiolib/
+drwxrwxrwx   0 daming    (1000) daming    (1000)        0 2023-05-16 08:31:01.293850 dmbiolib-0.4.2/dmbiolib/dmbiolib.egg-info/
+-rwxrwxrwx   0 daming    (1000) daming    (1000)     1224 2023-05-16 08:31:01.000000 dmbiolib-0.4.2/dmbiolib/dmbiolib.egg-info/PKG-INFO
+-rwxrwxrwx   0 daming    (1000) daming    (1000)      226 2023-05-16 08:31:01.000000 dmbiolib-0.4.2/dmbiolib/dmbiolib.egg-info/SOURCES.txt
+-rwxrwxrwx   0 daming    (1000) daming    (1000)        1 2023-05-16 08:31:01.000000 dmbiolib-0.4.2/dmbiolib/dmbiolib.egg-info/dependency_links.txt
+-rwxrwxrwx   0 daming    (1000) daming    (1000)        9 2023-05-16 08:31:01.000000 dmbiolib-0.4.2/dmbiolib/dmbiolib.egg-info/top_level.txt
+-rwxrwxrwx   0 daming    (1000) daming    (1000)    23172 2023-05-16 08:29:58.000000 dmbiolib-0.4.2/dmbiolib/dmbiolib.py
+-rwxrwxrwx   0 daming    (1000) daming    (1000)       38 2023-05-16 08:31:01.322849 dmbiolib-0.4.2/setup.cfg
+-rwxrwxrwx   0 daming    (1000) daming    (1000)      928 2023-05-16 08:30:19.000000 dmbiolib-0.4.2/setup.py
+drwxrwxrwx   0 daming    (1000) daming    (1000)        0 2023-05-16 08:31:01.306852 dmbiolib-0.4.2/tests/
+-rwxrwxrwx   0 daming    (1000) daming    (1000)     1584 2023-01-19 17:46:58.000000 dmbiolib-0.4.2/tests/test_.py
```

### Comparing `dmbiolib-0.4.1/LICENSE` & `dmbiolib-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dmbiolib-0.4.1/PKG-INFO` & `dmbiolib-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmbiolib
-Version: 0.4.1
+Version: 0.4.2
 Summary: Library of Python functions used in other projects
 Home-page: https://github.com/damienmarsic/dmbiolib
 Author: Damien Marsic
 Author-email: damien.marsic@aliyun.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `dmbiolib-0.4.1/README.md` & `dmbiolib-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `dmbiolib-0.4.1/dmbiolib/dmbiolib.egg-info/PKG-INFO` & `dmbiolib-0.4.2/dmbiolib/dmbiolib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmbiolib
-Version: 0.4.1
+Version: 0.4.2
 Summary: Library of Python functions used in other projects
 Home-page: https://github.com/damienmarsic/dmbiolib
 Author: Damien Marsic
 Author-email: damien.marsic@aliyun.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `dmbiolib-0.4.1/dmbiolib/dmbiolib.py` & `dmbiolib-0.4.2/dmbiolib/dmbiolib.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python
-__version__='0.4.1'
+__version__='0.4.2'
 last_update='2023-05-16'
 author='Damien Marsic, damien.marsic@aliyun.com'
 license='GNU General Public v3 (GPLv3)'
 docs='https://dmbiolib.readthedocs.io'
 
 import sys,os,gzip,time,math
 from glob import glob
@@ -398,15 +398,15 @@
         a,b='',''
     y=[n.replace(a,'*') for n in rfiles if a and a in n]+[n for n in rfiles if (a not in n and b not in n) or not a]
     z=prefix(y)
     for i in range(len(y)):
         x=y[i]
         if a and '*' in x:
             x=y[i].replace('*',a)+' '+y[i].replace('*',b)
-        y[i]=y[i][:z[i]]+' '+x
+        y[i]=z[i]+' '+x
     return sortfiles(y,' ')
 
 def findall(probe,seq,start,end,overlap=False):
     i=seq.find(probe,start,end)
     while i!=-1:
         yield i
         if overlap:
```

### Comparing `dmbiolib-0.4.1/setup.py` & `dmbiolib-0.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="dmbiolib", # Replace with your own username
-    version="0.4.1",
+    version="0.4.2",
     author="Damien Marsic",
     author_email="damien.marsic@aliyun.com",
     description="Library of Python functions used in other projects",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/damienmarsic/dmbiolib",
     package_dir={'': 'dmbiolib'},
```

