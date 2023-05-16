# Comparing `tmp/styles-0.1.9.tar.gz` & `tmp/styles-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "styles-0.1.9.tar", last modified: Tue May 16 08:16:13 2023, max compression
+gzip compressed data, was "styles-0.2.0.tar", last modified: Tue May 16 08:21:16 2023, max compression
```

## Comparing `styles-0.1.9.tar` & `styles-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 08:16:13.567116 styles-0.1.9/
--rw-rw-rw-   0        0        0      593 2023-05-16 08:16:13.566133 styles-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0      437 2022-11-21 13:37:43.000000 styles-0.1.9/README.md
--rw-rw-rw-   0        0        0       42 2023-05-16 08:16:13.567116 styles-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0      737 2023-05-16 08:16:07.000000 styles-0.1.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-16 08:16:13.542601 styles-0.1.9/styles/
--rw-rw-rw-   0        0        0     9823 2023-05-16 07:19:25.000000 styles-0.1.9/styles/Style.py
--rw-rw-rw-   0        0        0      346 2023-05-16 07:22:06.000000 styles-0.1.9/styles/__init__.py
--rw-rw-rw-   0        0        0     1889 2022-12-06 08:06:09.000000 styles-0.1.9/styles/figures.py
--rw-rw-rw-   0        0        0     2302 2022-12-06 08:09:20.000000 styles-0.1.9/styles/osInfo.py
-drwxrwxrwx   0        0        0        0 2023-05-16 08:16:13.563138 styles-0.1.9/styles.egg-info/
--rw-rw-rw-   0        0        0      593 2023-05-16 08:16:13.000000 styles-0.1.9/styles.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      208 2023-05-16 08:16:13.000000 styles-0.1.9/styles.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 08:16:13.000000 styles-0.1.9/styles.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-16 08:16:13.000000 styles-0.1.9/styles.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 08:21:16.771448 styles-0.2.0/
+-rw-rw-rw-   0        0        0     1019 2023-05-16 08:21:16.771448 styles-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      437 2022-11-21 13:37:43.000000 styles-0.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-16 08:21:16.772448 styles-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      874 2023-05-16 08:21:12.000000 styles-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 08:21:16.753448 styles-0.2.0/styles/
+-rw-rw-rw-   0        0        0     9823 2023-05-16 07:19:25.000000 styles-0.2.0/styles/Style.py
+-rw-rw-rw-   0        0        0      346 2023-05-16 07:22:06.000000 styles-0.2.0/styles/__init__.py
+-rw-rw-rw-   0        0        0     1889 2022-12-06 08:06:09.000000 styles-0.2.0/styles/figures.py
+-rw-rw-rw-   0        0        0     2302 2022-12-06 08:09:20.000000 styles-0.2.0/styles/osInfo.py
+drwxrwxrwx   0        0        0        0 2023-05-16 08:21:16.769448 styles-0.2.0/styles.egg-info/
+-rw-rw-rw-   0        0        0     1019 2023-05-16 08:21:16.000000 styles-0.2.0/styles.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      208 2023-05-16 08:21:16.000000 styles-0.2.0/styles.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 08:21:16.000000 styles-0.2.0/styles.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-16 08:21:16.000000 styles-0.2.0/styles.egg-info/top_level.txt
```

### Comparing `styles-0.1.9/setup.py` & `styles-0.2.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,28 @@
 from setuptools import setup
 
+
+# Description
+long_description = ""
+with open("README.md", "r", encoding="utf-8") as fh:
+    long_description = fh.read()
+
+
+
 setup(
     name='styles',
-    version='0.1.9',
+    version='0.2.0',
     description='A Style pack for python',
     url='https://github.com/Xtarii/PythonStylePack',
     author='Lord Alvin Hansen',
     author_email='alvin.hansen@elev.ga.ntig.se',
     license='BSD 2-clause',
     packages=['styles'],
 
-    long_description="./README.md",
+    long_description=long_description,
     long_description_content_type="text/markdown",
 
     classifiers=[
         'Development Status :: 1 - Planning',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: BSD License',
         'Operating System :: POSIX :: Linux',
```

### Comparing `styles-0.1.9/styles/Style.py` & `styles-0.2.0/styles/Style.py`

 * *Files identical despite different names*

### Comparing `styles-0.1.9/styles/figures.py` & `styles-0.2.0/styles/figures.py`

 * *Files identical despite different names*

### Comparing `styles-0.1.9/styles/osInfo.py` & `styles-0.2.0/styles/osInfo.py`

 * *Files identical despite different names*

