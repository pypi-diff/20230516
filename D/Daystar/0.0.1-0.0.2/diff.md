# Comparing `tmp/Daystar-0.0.1.tar.gz` & `tmp/Daystar-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Daystar-0.0.1.tar", last modified: Tue May 16 03:22:12 2023, max compression
+gzip compressed data, was "Daystar-0.0.2.tar", last modified: Tue May 16 03:28:59 2023, max compression
```

## Comparing `Daystar-0.0.1.tar` & `Daystar-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-16 03:22:12.066861 Daystar-0.0.1/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-16 03:22:12.066861 Daystar-0.0.1/Daystar/
--rw-r--r--   0 runner    (1000) runner    (1000)      339 2023-05-16 03:16:27.000000 Daystar-0.0.1/Daystar/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-16 03:22:12.066861 Daystar-0.0.1/Daystar.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)      402 2023-05-16 03:22:11.000000 Daystar-0.0.1/Daystar.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      215 2023-05-16 03:22:11.000000 Daystar-0.0.1/Daystar.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-05-16 03:22:11.000000 Daystar-0.0.1/Daystar.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       11 2023-05-16 03:22:11.000000 Daystar-0.0.1/Daystar.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        8 2023-05-16 03:22:11.000000 Daystar-0.0.1/Daystar.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     1069 2023-05-16 03:18:05.000000 Daystar-0.0.1/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)      402 2023-05-16 03:22:12.066861 Daystar-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2023-05-16 03:17:36.000000 Daystar-0.0.1/README.md
--rw-r--r--   0 runner    (1000) runner    (1000)      473 2023-01-20 17:56:39.000000 Daystar-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-05-16 03:22:12.066861 Daystar-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      697 2023-05-16 03:19:59.000000 Daystar-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-16 03:28:59.262423 Daystar-0.0.2/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-16 03:28:59.258423 Daystar-0.0.2/Daystar/
+-rw-r--r--   0 runner    (1000) runner    (1000)      646 2023-05-16 03:28:40.000000 Daystar-0.0.2/Daystar/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-16 03:28:59.262423 Daystar-0.0.2/Daystar.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)      402 2023-05-16 03:28:59.000000 Daystar-0.0.2/Daystar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      215 2023-05-16 03:28:59.000000 Daystar-0.0.2/Daystar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-05-16 03:28:59.000000 Daystar-0.0.2/Daystar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       11 2023-05-16 03:28:59.000000 Daystar-0.0.2/Daystar.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        8 2023-05-16 03:28:59.000000 Daystar-0.0.2/Daystar.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     1069 2023-05-16 03:18:05.000000 Daystar-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)      402 2023-05-16 03:28:59.262423 Daystar-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2023-05-16 03:17:36.000000 Daystar-0.0.2/README.md
+-rw-r--r--   0 runner    (1000) runner    (1000)      473 2023-01-20 17:56:39.000000 Daystar-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-05-16 03:28:59.262423 Daystar-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      658 2023-05-16 03:28:46.000000 Daystar-0.0.2/setup.py
```

### Comparing `Daystar-0.0.1/LICENSE` & `Daystar-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Daystar-0.0.1/setup.py` & `Daystar-0.0.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import setuptools
 with open("README.md", "r") as fh:
-    long_description = fh.read()
+  long_description = fh.read()
 setuptools.setup(
-    name="Daystar",
-    version="0.0.1",
-    author="Siddhu Pendyala",
-    author_email="siddhu.pendyala@outlook.com",
-    description="Sun calculation class from Solarflare module",
-    long_description=long_description, # don't touch this, this is your README.md
-    long_description_content_type="text/markdown",
-    packages=setuptools.find_packages(),
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-    ],
-    python_requires='>=3.6',
-    install_requires = ["Solarflare"]
-)
+  name="Daystar",
+  version="0.0.2",
+  author="Siddhu Pendyala",
+  author_email="siddhu.pendyala@outlook.com",
+  description="Sun calculation class from Solarflare module",
+  long_description=long_description,  # don't touch this, this is your README.md
+  long_description_content_type="text/markdown",
+  packages=setuptools.find_packages(),
+  classifiers=[
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+  ],
+  python_requires='>=3.6',
+  install_requires=["Solarflare"])
```

