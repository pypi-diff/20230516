# Comparing `tmp/arcangelai-2.0.5.tar.gz` & `tmp/arcangelai-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcangelai-2.0.5.tar", last modified: Sun Apr 30 01:09:27 2023, max compression
+gzip compressed data, was "arcangelai-2.0.6.tar", last modified: Tue May 16 02:43:39 2023, max compression
```

## Comparing `arcangelai-2.0.5.tar` & `arcangelai-2.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 william    (506) staff       (20)        0 2023-04-30 01:09:27.861576 arcangelai-2.0.5/
--rw-r--r--   0 william    (506) staff       (20)       77 2023-04-29 21:40:13.000000 arcangelai-2.0.5/CHANGELOG.txt
--rw-r--r--   0 william    (506) staff       (20)     1067 2023-04-29 21:25:13.000000 arcangelai-2.0.5/LICENSE
--rw-r--r--   0 william    (506) staff       (20)       25 2023-04-29 21:53:13.000000 arcangelai-2.0.5/MANIFEST.in
--rw-r--r--   0 william    (506) staff       (20)      554 2023-04-30 01:09:27.860310 arcangelai-2.0.5/PKG-INFO
--rw-r--r--   0 william    (506) staff       (20)       36 2023-04-29 22:47:34.000000 arcangelai-2.0.5/README.md
-drwxr-xr-x   0 william    (506) staff       (20)        0 2023-04-30 01:09:27.854112 arcangelai-2.0.5/arcangelai/
--rw-r--r--   0 william    (506) staff       (20)      951 2023-04-30 01:09:09.000000 arcangelai-2.0.5/arcangelai/__init__.py
-drwxr-xr-x   0 william    (506) staff       (20)        0 2023-04-30 01:09:27.859696 arcangelai-2.0.5/arcangelai.egg-info/
--rw-r--r--   0 william    (506) staff       (20)      554 2023-04-30 01:09:27.000000 arcangelai-2.0.5/arcangelai.egg-info/PKG-INFO
--rw-r--r--   0 william    (506) staff       (20)      211 2023-04-30 01:09:27.000000 arcangelai-2.0.5/arcangelai.egg-info/SOURCES.txt
--rw-r--r--   0 william    (506) staff       (20)        1 2023-04-30 01:09:27.000000 arcangelai-2.0.5/arcangelai.egg-info/dependency_links.txt
--rw-r--r--   0 william    (506) staff       (20)       11 2023-04-30 01:09:27.000000 arcangelai-2.0.5/arcangelai.egg-info/top_level.txt
--rw-r--r--   0 william    (506) staff       (20)       38 2023-04-30 01:09:27.861712 arcangelai-2.0.5/setup.cfg
--rw-r--r--   0 william    (506) staff       (20)      646 2023-04-30 01:09:18.000000 arcangelai-2.0.5/setup.py
+drwxr-xr-x   0 william    (506) staff       (20)        0 2023-05-16 02:43:39.211030 arcangelai-2.0.6/
+-rw-r--r--   0 william    (506) staff       (20)       77 2023-04-29 21:40:13.000000 arcangelai-2.0.6/CHANGELOG.txt
+-rw-r--r--   0 william    (506) staff       (20)     1067 2023-04-29 21:25:13.000000 arcangelai-2.0.6/LICENSE
+-rw-r--r--   0 william    (506) staff       (20)       25 2023-04-29 21:53:13.000000 arcangelai-2.0.6/MANIFEST.in
+-rw-r--r--   0 william    (506) staff       (20)      552 2023-05-16 02:43:39.208143 arcangelai-2.0.6/PKG-INFO
+-rw-r--r--   0 william    (506) staff       (20)       36 2023-04-29 22:47:34.000000 arcangelai-2.0.6/README.md
+drwxr-xr-x   0 william    (506) staff       (20)        0 2023-05-16 02:43:39.201303 arcangelai-2.0.6/arcangelai/
+-rw-r--r--   0 william    (506) staff       (20)     1071 2023-05-16 02:41:15.000000 arcangelai-2.0.6/arcangelai/__init__.py
+drwxr-xr-x   0 william    (506) staff       (20)        0 2023-05-16 02:43:39.206894 arcangelai-2.0.6/arcangelai.egg-info/
+-rw-r--r--   0 william    (506) staff       (20)      552 2023-05-16 02:43:39.000000 arcangelai-2.0.6/arcangelai.egg-info/PKG-INFO
+-rw-r--r--   0 william    (506) staff       (20)      211 2023-05-16 02:43:39.000000 arcangelai-2.0.6/arcangelai.egg-info/SOURCES.txt
+-rw-r--r--   0 william    (506) staff       (20)        1 2023-05-16 02:43:39.000000 arcangelai-2.0.6/arcangelai.egg-info/dependency_links.txt
+-rw-r--r--   0 william    (506) staff       (20)       11 2023-05-16 02:43:39.000000 arcangelai-2.0.6/arcangelai.egg-info/top_level.txt
+-rw-r--r--   0 william    (506) staff       (20)       38 2023-05-16 02:43:39.211221 arcangelai-2.0.6/setup.cfg
+-rw-r--r--   0 william    (506) staff       (20)      644 2023-05-16 02:39:35.000000 arcangelai-2.0.6/setup.py
```

### Comparing `arcangelai-2.0.5/LICENSE` & `arcangelai-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `arcangelai-2.0.5/PKG-INFO` & `arcangelai-2.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: arcangelai
-Version: 2.0.5
+Version: 2.0.6
 Summary: Autonomous AI
 Home-page: 
 Author: Arc Angel Ai
-Author-email: arcangelgpt@gmail.com
+Author-email: info@arcangelai.com
 License: MIT
 Keywords: autonomous
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
```

### Comparing `arcangelai-2.0.5/arcangelai.egg-info/PKG-INFO` & `arcangelai-2.0.6/arcangelai.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: arcangelai
-Version: 2.0.5
+Version: 2.0.6
 Summary: Autonomous AI
 Home-page: 
 Author: Arc Angel Ai
-Author-email: arcangelgpt@gmail.com
+Author-email: info@arcangelai.com
 License: MIT
 Keywords: autonomous
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
```

### Comparing `arcangelai-2.0.5/setup.py` & `arcangelai-2.0.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,20 +5,20 @@
   'Intended Audience :: Education',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='arcangelai',
-  version='2.0.5',
+  version='2.0.6',
   description='Autonomous AI',
   long_description_content_type='text/x-rst',
   long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
   url='',  
   author='Arc Angel Ai',
-  author_email='arcangelgpt@gmail.com',
+  author_email='info@arcangelai.com',
   license='MIT', 
   classifiers=classifiers,
   keywords='autonomous', 
   packages=find_packages(),
   install_requires=[''] 
 )
```

