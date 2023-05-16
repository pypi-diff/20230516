# Comparing `tmp/createai-0.1.0.tar.gz` & `tmp/createai-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "createai-0.1.0.tar", last modified: Sun May 14 12:12:38 2023, max compression
+gzip compressed data, was "createai-0.1.1.tar", last modified: Tue May 16 10:14:33 2023, max compression
```

## Comparing `createai-0.1.0.tar` & `createai-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 12:12:38.730952 createai-0.1.0/
--rw-rw-rw-   0        0        0     1095 2023-05-14 12:09:53.000000 createai-0.1.0/LICENCE
--rw-rw-rw-   0        0        0       48 2023-05-14 12:12:38.000000 createai-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1848 2023-05-14 12:12:38.730952 createai-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1403 2023-05-14 12:06:51.000000 createai-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-14 12:12:38.729932 createai-0.1.0/createai.egg-info/
--rw-rw-rw-   0        0        0     1848 2023-05-14 12:12:38.000000 createai-0.1.0/createai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      276 2023-05-14 12:12:38.000000 createai-0.1.0/createai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 12:12:38.000000 createai-0.1.0/createai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-05-14 12:12:38.000000 createai-0.1.0/createai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-14 12:12:38.731952 createai-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      671 2023-05-14 12:12:38.000000 createai-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 10:14:33.701328 createai-0.1.1/
+-rw-rw-rw-   0        0        0     1095 2023-05-14 12:09:53.000000 createai-0.1.1/LICENCE
+-rw-rw-rw-   0        0        0       48 2023-05-16 10:14:33.000000 createai-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1803 2023-05-16 10:14:33.701328 createai-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1358 2023-05-16 10:13:14.000000 createai-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-16 10:14:33.699327 createai-0.1.1/createai.egg-info/
+-rw-rw-rw-   0        0        0     1803 2023-05-16 10:14:33.000000 createai-0.1.1/createai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-05-16 10:14:33.000000 createai-0.1.1/createai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 10:14:33.000000 createai-0.1.1/createai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-05-16 10:14:33.000000 createai-0.1.1/createai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-16 10:14:33.703327 createai-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      671 2023-05-16 10:14:33.000000 createai-0.1.1/setup.py
```

### Comparing `createai-0.1.0/LICENCE` & `createai-0.1.1/LICENCE`

 * *Files identical despite different names*

### Comparing `createai-0.1.0/PKG-INFO` & `createai-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: createai
-Version: 0.1.0
+Version: 0.1.1
 Summary: Easy tool for creating AI in python
 Home-page: https://github.com/R0fael/CreateAI
 Author: R0fael
 Author-email: roslobodchikov@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 
-# CreateAI v0.1.0
+# CreateAI v0.1.1
 It's easy tool to create ai in python easy and fast.
 You can edit source code of CreateAI on [Create AI's github](https://github.com/R0fael/CreateAI)
 
 ## Dependencies
  - numpy
  - knowledge of python
  - our documentation
@@ -35,55 +35,53 @@
 
 ## Installation
 
 Installing project with pip
 
 Windows:
 ```bash
-pip install СreateAI
+pip install createai
 ```
 
 MacOS:
 ```bash
-pip3 install СreateAI
+pip3 install createai
 ```
 
 Linux:
 ```bash
-sudo pip install СreateAI
+sudo pip install createai
 ```
 
 Or if you don't have pip :
 download sourse code and editing examples files
 
 ## Example
 ```python
-from CreateAI import *
-"""
-inputs - create inputs
-outputs - create outputs
-"""
 # importing CreateAI
-from CreateAI import *
+from createai import *
 
 n = Neuron(weights(3, 1), inputs([
     [0, 0, 1],
     [1, 1, 1],
     [1, 0, 1],
     [0, 1, 1]
-]), outputs([[0, 1, 1, 0]]),save_path="my_save.nws")  # Neuron creating with saving
-#.nws -> file extension -> neuron weight save
+]), outputs([[0, 1, 1, 0]]),save_path="my_save.cns")  # Neuron creating with saving
+#.cns -> file extension -> neuron weight save
 
 n.learn(20_000)  # Neuron learning
 
 print(n.process([1, 1, 0]))  # Neuron test
 print(n.process([0, 1, 0]))  # Neuron test
 ```
 
 ## Change log
 
 -0.1.0 - first version
-## Plans
 
--0.1.1 - Multi neurons update
+-0.1.1 - speed up and little bug fix
+
+## Plans
 
 -0.1.2 - More metods of learning
+
+-0.1.3 - Multi neurons update
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `createai-0.1.0/README.md` & `createai-0.1.1/createai.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,23 @@
+Metadata-Version: 2.1
+Name: createai
+Version: 0.1.1
+Summary: Easy tool for creating AI in python
+Home-page: https://github.com/R0fael/CreateAI
+Author: R0fael
+Author-email: roslobodchikov@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENCE
 
-# CreateAI v0.1.0
+
+# CreateAI v0.1.1
 It's easy tool to create ai in python easy and fast.
 You can edit source code of CreateAI on [Create AI's github](https://github.com/R0fael/CreateAI)
 
 ## Dependencies
  - numpy
  - knowledge of python
  - our documentation
@@ -21,55 +35,53 @@
 
 ## Installation
 
 Installing project with pip
 
 Windows:
 ```bash
-pip install СreateAI
+pip install createai
 ```
 
 MacOS:
 ```bash
-pip3 install СreateAI
+pip3 install createai
 ```
 
 Linux:
 ```bash
-sudo pip install СreateAI
+sudo pip install createai
 ```
 
 Or if you don't have pip :
 download sourse code and editing examples files
 
 ## Example
 ```python
-from CreateAI import *
-"""
-inputs - create inputs
-outputs - create outputs
-"""
 # importing CreateAI
-from CreateAI import *
+from createai import *
 
 n = Neuron(weights(3, 1), inputs([
     [0, 0, 1],
     [1, 1, 1],
     [1, 0, 1],
     [0, 1, 1]
-]), outputs([[0, 1, 1, 0]]),save_path="my_save.nws")  # Neuron creating with saving
-#.nws -> file extension -> neuron weight save
+]), outputs([[0, 1, 1, 0]]),save_path="my_save.cns")  # Neuron creating with saving
+#.cns -> file extension -> neuron weight save
 
 n.learn(20_000)  # Neuron learning
 
 print(n.process([1, 1, 0]))  # Neuron test
 print(n.process([0, 1, 0]))  # Neuron test
 ```
 
 ## Change log
 
 -0.1.0 - first version
+
+-0.1.1 - speed up and little bug fix
+
 ## Plans
 
--0.1.1 - Multi neurons update
+-0.1.2 - More metods of learning
 
--0.1.2 - More metods of learning
+-0.1.3 - Multi neurons update
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `createai-0.1.0/setup.py` & `createai-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 with open(r'C:\MyUse\code\python\EasyPack\README.md', 'r', encoding='utf-8') as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name='createai',
-	version='0.1.0',
+	version='0.1.1',
 	author='R0fael',
 	author_email='roslobodchikov@gmail.com',
 	description='Easy tool for creating AI in python',
 	long_description=long_description,
 	long_description_content_type='text/markdown',
 	url='https://github.com/R0fael/CreateAI',
 	packages=['C:\MyUse\code\python\EasyPack\createai'],
```

