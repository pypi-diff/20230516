# Comparing `tmp/styles-0.1.7.tar.gz` & `tmp/styles-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "styles-0.1.7.tar", last modified: Tue May 16 07:28:57 2023, max compression
+gzip compressed data, was "styles-0.1.8.tar", last modified: Tue May 16 08:12:48 2023, max compression
```

## Comparing `styles-0.1.7.tar` & `styles-0.1.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 07:28:57.919157 styles-0.1.7/
--rw-rw-rw-   0        0        0      537 2023-05-16 07:28:57.917140 styles-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0      437 2022-11-21 13:37:43.000000 styles-0.1.7/README.rst
--rw-rw-rw-   0        0        0       42 2023-05-16 07:28:57.920141 styles-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      646 2023-05-16 07:28:26.000000 styles-0.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-16 07:28:57.890141 styles-0.1.7/styles/
--rw-rw-rw-   0        0        0     9823 2023-05-16 07:19:25.000000 styles-0.1.7/styles/Style.py
--rw-rw-rw-   0        0        0      346 2023-05-16 07:22:06.000000 styles-0.1.7/styles/__init__.py
--rw-rw-rw-   0        0        0     1889 2022-12-06 08:06:09.000000 styles-0.1.7/styles/figures.py
--rw-rw-rw-   0        0        0     2302 2022-12-06 08:09:20.000000 styles-0.1.7/styles/osInfo.py
-drwxrwxrwx   0        0        0        0 2023-05-16 07:28:57.914138 styles-0.1.7/styles.egg-info/
--rw-rw-rw-   0        0        0      537 2023-05-16 07:28:57.000000 styles-0.1.7/styles.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      209 2023-05-16 07:28:57.000000 styles-0.1.7/styles.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 07:28:57.000000 styles-0.1.7/styles.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-16 07:28:57.000000 styles-0.1.7/styles.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 08:12:48.479587 styles-0.1.8/
+-rw-rw-rw-   0        0        0      591 2023-05-16 08:12:48.478587 styles-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0      437 2022-11-21 13:37:43.000000 styles-0.1.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-16 08:12:48.479587 styles-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      735 2023-05-16 08:12:42.000000 styles-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 08:12:48.458602 styles-0.1.8/styles/
+-rw-rw-rw-   0        0        0     9823 2023-05-16 07:19:25.000000 styles-0.1.8/styles/Style.py
+-rw-rw-rw-   0        0        0      346 2023-05-16 07:22:06.000000 styles-0.1.8/styles/__init__.py
+-rw-rw-rw-   0        0        0     1889 2022-12-06 08:06:09.000000 styles-0.1.8/styles/figures.py
+-rw-rw-rw-   0        0        0     2302 2022-12-06 08:09:20.000000 styles-0.1.8/styles/osInfo.py
+drwxrwxrwx   0        0        0        0 2023-05-16 08:12:48.477588 styles-0.1.8/styles.egg-info/
+-rw-rw-rw-   0        0        0      591 2023-05-16 08:12:48.000000 styles-0.1.8/styles.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      208 2023-05-16 08:12:48.000000 styles-0.1.8/styles.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 08:12:48.000000 styles-0.1.8/styles.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-16 08:12:48.000000 styles-0.1.8/styles.egg-info/top_level.txt
```

### Comparing `styles-0.1.7/PKG-INFO` & `styles-0.1.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 Metadata-Version: 2.1
 Name: styles
-Version: 0.1.7
+Version: 0.1.8
 Summary: A Style pack for python
 Home-page: https://github.com/Xtarii/PythonStylePack
 Author: Lord Alvin Hansen
 Author-email: alvin.hansen@elev.ga.ntig.se
 License: BSD 2-clause
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+
+README.md
```

### Comparing `styles-0.1.7/setup.py` & `styles-0.1.8/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 from setuptools import setup
 
 setup(
     name='styles',
-    version='0.1.7',
+    version='0.1.8',
     description='A Style pack for python',
     url='https://github.com/Xtarii/PythonStylePack',
     author='Lord Alvin Hansen',
     author_email='alvin.hansen@elev.ga.ntig.se',
     license='BSD 2-clause',
     packages=['styles'],
 
+    long_description="README.md",
+    long_description_content_type="text/markdown",
+
     classifiers=[
         'Development Status :: 1 - Planning',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: BSD License',
         'Operating System :: POSIX :: Linux',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.11',
```

### Comparing `styles-0.1.7/styles/Style.py` & `styles-0.1.8/styles/Style.py`

 * *Files identical despite different names*

### Comparing `styles-0.1.7/styles/figures.py` & `styles-0.1.8/styles/figures.py`

 * *Files identical despite different names*

### Comparing `styles-0.1.7/styles/osInfo.py` & `styles-0.1.8/styles/osInfo.py`

 * *Files identical despite different names*

### Comparing `styles-0.1.7/styles.egg-info/PKG-INFO` & `styles-0.1.8/styles.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 Metadata-Version: 2.1
 Name: styles
-Version: 0.1.7
+Version: 0.1.8
 Summary: A Style pack for python
 Home-page: https://github.com/Xtarii/PythonStylePack
 Author: Lord Alvin Hansen
 Author-email: alvin.hansen@elev.ga.ntig.se
 License: BSD 2-clause
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+
+README.md
```

