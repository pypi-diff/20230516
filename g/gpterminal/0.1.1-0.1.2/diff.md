# Comparing `tmp/GPTerminal-0.1.1.tar.gz` & `tmp/gpterminal-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GPTerminal-0.1.1.tar", last modified: Mon May 15 16:30:20 2023, max compression
+gzip compressed data, was "gpterminal-0.1.2.tar", last modified: Tue May 16 08:45:50 2023, max compression
```

## Comparing `GPTerminal-0.1.1.tar` & `gpterminal-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,18 @@
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-15 16:30:20.754740 GPTerminal-0.1.1/
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-15 16:30:20.752739 GPTerminal-0.1.1/GPTerminal.egg-info/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2892 2023-05-15 16:30:20.000000 GPTerminal-0.1.1/GPTerminal.egg-info/PKG-INFO
--rw-r--r--   0 luzhipeng   (501) staff       (20)      224 2023-05-15 16:30:20.000000 GPTerminal-0.1.1/GPTerminal.egg-info/SOURCES.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)        1 2023-05-15 16:30:20.000000 GPTerminal-0.1.1/GPTerminal.egg-info/dependency_links.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)       35 2023-05-15 16:30:20.000000 GPTerminal-0.1.1/GPTerminal.egg-info/entry_points.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)       82 2023-05-15 16:30:20.000000 GPTerminal-0.1.1/GPTerminal.egg-info/requires.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)        1 2023-05-15 16:30:20.000000 GPTerminal-0.1.1/GPTerminal.egg-info/top_level.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2892 2023-05-15 16:30:20.753986 GPTerminal-0.1.1/PKG-INFO
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2148 2023-05-15 16:21:20.000000 GPTerminal-0.1.1/README.md
--rw-r--r--   0 luzhipeng   (501) staff       (20)       38 2023-05-15 16:30:20.754912 GPTerminal-0.1.1/setup.cfg
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1269 2023-05-15 16:29:50.000000 GPTerminal-0.1.1/setup.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-16 08:45:50.023433 gpterminal-0.1.2/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2902 2023-05-16 08:45:50.023012 gpterminal-0.1.2/PKG-INFO
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2148 2023-05-15 16:21:20.000000 gpterminal-0.1.2/README.md
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-16 08:45:50.018466 gpterminal-0.1.2/cli/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     7902 2023-05-16 08:04:08.000000 gpterminal-0.1.2/cli/ChatGPT.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-05-16 03:14:58.000000 gpterminal-0.1.2/cli/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     6906 2023-05-16 08:30:54.000000 gpterminal-0.1.2/cli/cli.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     8176 2023-05-15 15:21:27.000000 gpterminal-0.1.2/cli/code_execution.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      854 2023-05-15 15:21:12.000000 gpterminal-0.1.2/cli/utils.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-16 08:45:50.022480 gpterminal-0.1.2/gpterminal.egg-info/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2902 2023-05-16 08:45:49.000000 gpterminal-0.1.2/gpterminal.egg-info/PKG-INFO
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      301 2023-05-16 08:45:50.000000 gpterminal-0.1.2/gpterminal.egg-info/SOURCES.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        1 2023-05-16 08:45:49.000000 gpterminal-0.1.2/gpterminal.egg-info/dependency_links.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       50 2023-05-16 08:45:49.000000 gpterminal-0.1.2/gpterminal.egg-info/entry_points.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       97 2023-05-16 08:45:49.000000 gpterminal-0.1.2/gpterminal.egg-info/requires.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        4 2023-05-16 08:45:50.000000 gpterminal-0.1.2/gpterminal.egg-info/top_level.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       38 2023-05-16 08:45:50.023577 gpterminal-0.1.2/setup.cfg
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1259 2023-05-16 08:45:42.000000 gpterminal-0.1.2/setup.py
```

### Comparing `GPTerminal-0.1.1/GPTerminal.egg-info/PKG-INFO` & `gpterminal-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
-Name: GPTerminal
-Version: 0.1.1
-Summary: A command line tool that utilizes GPT models to assist with various tasks
-Home-page: https://github.com/yourusername/GPTerminal
+Name: gpterminal
+Version: 0.1.2
+Summary: A CLI tool to interact with GPT-3/GPT-4, answer Git questions, and execute commands
+Home-page: https://github.com/yourusername/gpterminal
 Author: Your Name
 Author-email: your.email@example.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `GPTerminal-0.1.1/PKG-INFO` & `gpterminal-0.1.2/gpterminal.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
-Name: GPTerminal
-Version: 0.1.1
-Summary: A command line tool that utilizes GPT models to assist with various tasks
-Home-page: https://github.com/yourusername/GPTerminal
+Name: gpterminal
+Version: 0.1.2
+Summary: A CLI tool to interact with GPT-3/GPT-4, answer Git questions, and execute commands
+Home-page: https://github.com/yourusername/gpterminal
 Author: Your Name
 Author-email: your.email@example.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `GPTerminal-0.1.1/README.md` & `gpterminal-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `GPTerminal-0.1.1/setup.py` & `gpterminal-0.1.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,37 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
+with open("requirements.txt", "r", encoding="utf-8") as req:
+    requirements = req.read().splitlines()
+
 setup(
-    name="GPTerminal",
-    version="0.1.1",
+    name="gpterminal",
+    version="0.1.2",
     author="Your Name",
     author_email="your.email@example.com",
-    description="A command line tool that utilizes GPT models to assist with various tasks",
+    description="A CLI tool to interact with GPT-3/GPT-4, answer Git questions, and execute commands",
     long_description=long_description,
- long_description_content_type="text/markdown",
-    url="https://github.com/yourusername/GPTerminal",
+    long_description_content_type="text/markdown",
+    url="https://github.com/yourusername/gpterminal",
     packages=find_packages(),
+    install_requires=requirements,
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
     ],
     python_requires=">=3.6",
-    install_requires=[
-        "click",
-        "requests>=2.25.0",
-        "rich>=10.0.0",
-        "openai>=0.10.2",
-        "tiktoken",
-        "prompt_toolkit>=3.0.0",
-    ],
     entry_points={
         "console_scripts": [
-            "gpterminal=cli",
+            "gpterminal=cli.cli:gpterminal",
         ],
     },
 )
```

