# Comparing `tmp/gpterminal-0.1.2.tar.gz` & `tmp/gpterminal-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpterminal-0.1.2.tar", last modified: Tue May 16 08:45:50 2023, max compression
+gzip compressed data, was "gpterminal-0.1.3.tar", last modified: Tue May 16 08:50:50 2023, max compression
```

## Comparing `gpterminal-0.1.2.tar` & `gpterminal-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-16 08:45:50.023433 gpterminal-0.1.2/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2902 2023-05-16 08:45:50.023012 gpterminal-0.1.2/PKG-INFO
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2148 2023-05-15 16:21:20.000000 gpterminal-0.1.2/README.md
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-16 08:45:50.018466 gpterminal-0.1.2/cli/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     7902 2023-05-16 08:04:08.000000 gpterminal-0.1.2/cli/ChatGPT.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-05-16 03:14:58.000000 gpterminal-0.1.2/cli/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     6906 2023-05-16 08:30:54.000000 gpterminal-0.1.2/cli/cli.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     8176 2023-05-15 15:21:27.000000 gpterminal-0.1.2/cli/code_execution.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      854 2023-05-15 15:21:12.000000 gpterminal-0.1.2/cli/utils.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-16 08:45:50.022480 gpterminal-0.1.2/gpterminal.egg-info/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2902 2023-05-16 08:45:49.000000 gpterminal-0.1.2/gpterminal.egg-info/PKG-INFO
--rw-r--r--   0 luzhipeng   (501) staff       (20)      301 2023-05-16 08:45:50.000000 gpterminal-0.1.2/gpterminal.egg-info/SOURCES.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)        1 2023-05-16 08:45:49.000000 gpterminal-0.1.2/gpterminal.egg-info/dependency_links.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)       50 2023-05-16 08:45:49.000000 gpterminal-0.1.2/gpterminal.egg-info/entry_points.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)       97 2023-05-16 08:45:49.000000 gpterminal-0.1.2/gpterminal.egg-info/requires.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)        4 2023-05-16 08:45:50.000000 gpterminal-0.1.2/gpterminal.egg-info/top_level.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)       38 2023-05-16 08:45:50.023577 gpterminal-0.1.2/setup.cfg
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1259 2023-05-16 08:45:42.000000 gpterminal-0.1.2/setup.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-16 08:50:50.674251 gpterminal-0.1.3/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2902 2023-05-16 08:50:50.673171 gpterminal-0.1.3/PKG-INFO
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2148 2023-05-15 16:21:20.000000 gpterminal-0.1.3/README.md
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-16 08:50:50.668262 gpterminal-0.1.3/cli/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     7902 2023-05-16 08:04:08.000000 gpterminal-0.1.3/cli/ChatGPT.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-05-16 03:14:58.000000 gpterminal-0.1.3/cli/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     6906 2023-05-16 08:30:54.000000 gpterminal-0.1.3/cli/cli.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     8176 2023-05-15 15:21:27.000000 gpterminal-0.1.3/cli/code_execution.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      854 2023-05-15 15:21:12.000000 gpterminal-0.1.3/cli/utils.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-16 08:50:50.672409 gpterminal-0.1.3/gpterminal.egg-info/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2902 2023-05-16 08:50:50.000000 gpterminal-0.1.3/gpterminal.egg-info/PKG-INFO
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      301 2023-05-16 08:50:50.000000 gpterminal-0.1.3/gpterminal.egg-info/SOURCES.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        1 2023-05-16 08:50:50.000000 gpterminal-0.1.3/gpterminal.egg-info/dependency_links.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       50 2023-05-16 08:50:50.000000 gpterminal-0.1.3/gpterminal.egg-info/entry_points.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       97 2023-05-16 08:50:50.000000 gpterminal-0.1.3/gpterminal.egg-info/requires.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        4 2023-05-16 08:50:50.000000 gpterminal-0.1.3/gpterminal.egg-info/top_level.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       38 2023-05-16 08:50:50.674903 gpterminal-0.1.3/setup.cfg
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1322 2023-05-16 08:50:31.000000 gpterminal-0.1.3/setup.py
```

### Comparing `gpterminal-0.1.2/PKG-INFO` & `gpterminal-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpterminal
-Version: 0.1.2
+Version: 0.1.3
 Summary: A CLI tool to interact with GPT-3/GPT-4, answer Git questions, and execute commands
 Home-page: https://github.com/yourusername/gpterminal
 Author: Your Name
 Author-email: your.email@example.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gpterminal-0.1.2/README.md` & `gpterminal-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `gpterminal-0.1.2/cli/ChatGPT.py` & `gpterminal-0.1.3/cli/ChatGPT.py`

 * *Files identical despite different names*

### Comparing `gpterminal-0.1.2/cli/cli.py` & `gpterminal-0.1.3/cli/cli.py`

 * *Files identical despite different names*

### Comparing `gpterminal-0.1.2/cli/code_execution.py` & `gpterminal-0.1.3/cli/code_execution.py`

 * *Files identical despite different names*

### Comparing `gpterminal-0.1.2/cli/utils.py` & `gpterminal-0.1.3/cli/utils.py`

 * *Files identical despite different names*

### Comparing `gpterminal-0.1.2/gpterminal.egg-info/PKG-INFO` & `gpterminal-0.1.3/gpterminal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpterminal
-Version: 0.1.2
+Version: 0.1.3
 Summary: A CLI tool to interact with GPT-3/GPT-4, answer Git questions, and execute commands
 Home-page: https://github.com/yourusername/gpterminal
 Author: Your Name
 Author-email: your.email@example.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

