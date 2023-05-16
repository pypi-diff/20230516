# Comparing `tmp/gpterminal-0.1.3.tar.gz` & `tmp/gpterminal-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpterminal-0.1.3.tar", last modified: Tue May 16 08:50:50 2023, max compression
+gzip compressed data, was "gpterminal-0.1.4.tar", last modified: Tue May 16 09:05:11 2023, max compression
```

## Comparing `gpterminal-0.1.3.tar` & `gpterminal-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-16 08:50:50.674251 gpterminal-0.1.3/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2902 2023-05-16 08:50:50.673171 gpterminal-0.1.3/PKG-INFO
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2148 2023-05-15 16:21:20.000000 gpterminal-0.1.3/README.md
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-16 08:50:50.668262 gpterminal-0.1.3/cli/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     7902 2023-05-16 08:04:08.000000 gpterminal-0.1.3/cli/ChatGPT.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-05-16 03:14:58.000000 gpterminal-0.1.3/cli/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     6906 2023-05-16 08:30:54.000000 gpterminal-0.1.3/cli/cli.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     8176 2023-05-15 15:21:27.000000 gpterminal-0.1.3/cli/code_execution.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      854 2023-05-15 15:21:12.000000 gpterminal-0.1.3/cli/utils.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-16 08:50:50.672409 gpterminal-0.1.3/gpterminal.egg-info/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2902 2023-05-16 08:50:50.000000 gpterminal-0.1.3/gpterminal.egg-info/PKG-INFO
--rw-r--r--   0 luzhipeng   (501) staff       (20)      301 2023-05-16 08:50:50.000000 gpterminal-0.1.3/gpterminal.egg-info/SOURCES.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)        1 2023-05-16 08:50:50.000000 gpterminal-0.1.3/gpterminal.egg-info/dependency_links.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)       50 2023-05-16 08:50:50.000000 gpterminal-0.1.3/gpterminal.egg-info/entry_points.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)       97 2023-05-16 08:50:50.000000 gpterminal-0.1.3/gpterminal.egg-info/requires.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)        4 2023-05-16 08:50:50.000000 gpterminal-0.1.3/gpterminal.egg-info/top_level.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)       38 2023-05-16 08:50:50.674903 gpterminal-0.1.3/setup.cfg
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1322 2023-05-16 08:50:31.000000 gpterminal-0.1.3/setup.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-16 09:05:11.540603 gpterminal-0.1.4/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2902 2023-05-16 09:05:11.540154 gpterminal-0.1.4/PKG-INFO
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2148 2023-05-15 16:21:20.000000 gpterminal-0.1.4/README.md
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-16 09:05:11.534660 gpterminal-0.1.4/cli/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     7902 2023-05-16 08:04:08.000000 gpterminal-0.1.4/cli/ChatGPT.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-05-16 03:14:58.000000 gpterminal-0.1.4/cli/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     6906 2023-05-16 08:30:54.000000 gpterminal-0.1.4/cli/cli.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     8176 2023-05-15 15:21:27.000000 gpterminal-0.1.4/cli/code_execution.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      854 2023-05-15 15:21:12.000000 gpterminal-0.1.4/cli/utils.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-16 09:05:11.539492 gpterminal-0.1.4/gpterminal.egg-info/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2902 2023-05-16 09:05:11.000000 gpterminal-0.1.4/gpterminal.egg-info/PKG-INFO
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      301 2023-05-16 09:05:11.000000 gpterminal-0.1.4/gpterminal.egg-info/SOURCES.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        1 2023-05-16 09:05:11.000000 gpterminal-0.1.4/gpterminal.egg-info/dependency_links.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       50 2023-05-16 09:05:11.000000 gpterminal-0.1.4/gpterminal.egg-info/entry_points.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       59 2023-05-16 09:05:11.000000 gpterminal-0.1.4/gpterminal.egg-info/requires.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        4 2023-05-16 09:05:11.000000 gpterminal-0.1.4/gpterminal.egg-info/top_level.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       38 2023-05-16 09:05:11.540803 gpterminal-0.1.4/setup.cfg
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1284 2023-05-16 09:00:53.000000 gpterminal-0.1.4/setup.py
```

### Comparing `gpterminal-0.1.3/PKG-INFO` & `gpterminal-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpterminal
-Version: 0.1.3
+Version: 0.1.4
 Summary: A CLI tool to interact with GPT-3/GPT-4, answer Git questions, and execute commands
 Home-page: https://github.com/yourusername/gpterminal
 Author: Your Name
 Author-email: your.email@example.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gpterminal-0.1.3/README.md` & `gpterminal-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `gpterminal-0.1.3/cli/ChatGPT.py` & `gpterminal-0.1.4/cli/ChatGPT.py`

 * *Files identical despite different names*

### Comparing `gpterminal-0.1.3/cli/cli.py` & `gpterminal-0.1.4/cli/cli.py`

 * *Files identical despite different names*

### Comparing `gpterminal-0.1.3/cli/code_execution.py` & `gpterminal-0.1.4/cli/code_execution.py`

 * *Files identical despite different names*

### Comparing `gpterminal-0.1.3/cli/utils.py` & `gpterminal-0.1.4/cli/utils.py`

 * *Files identical despite different names*

### Comparing `gpterminal-0.1.3/gpterminal.egg-info/PKG-INFO` & `gpterminal-0.1.4/gpterminal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpterminal
-Version: 0.1.3
+Version: 0.1.4
 Summary: A CLI tool to interact with GPT-3/GPT-4, answer Git questions, and execute commands
 Home-page: https://github.com/yourusername/gpterminal
 Author: Your Name
 Author-email: your.email@example.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gpterminal-0.1.3/setup.py` & `gpterminal-0.1.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="gpterminal",
-    version="0.1.3",
+    version="0.1.4",
     author="Your Name",
     author_email="your.email@example.com",
     description="A CLI tool to interact with GPT-3/GPT-4, answer Git questions, and execute commands",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/yourusername/gpterminal",
     packages=find_packages(),
     install_requires=[
-        'click==8.0.1',
-        'requests==2.26.0',
-        'rich==10.3.0',
-        'pathlib==1.0.1',
+        'click',
+        'requests',
+        'rich',
+        'pathlib',
         'openai',
         'tiktoken',
-        'prompt_toolkit==3.0.20'
+        'prompt_toolkit'
     ],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
```

