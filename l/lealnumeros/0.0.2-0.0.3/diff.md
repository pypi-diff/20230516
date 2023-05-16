# Comparing `tmp/lealnumeros-0.0.2.tar.gz` & `tmp/lealnumeros-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lealnumeros-0.0.2.tar", last modified: Mon May 15 00:14:16 2023, max compression
+gzip compressed data, was "lealnumeros-0.0.3.tar", last modified: Tue May 16 05:02:27 2023, max compression
```

## Comparing `lealnumeros-0.0.2.tar` & `lealnumeros-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 00:14:16.303334 lealnumeros-0.0.2/
--rw-rw-rw-   0        0        0     1098 2023-05-14 20:25:14.000000 lealnumeros-0.0.2/LICENCE
--rw-rw-rw-   0        0        0     1278 2023-05-15 00:14:16.301335 lealnumeros-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      932 2023-05-14 23:53:56.000000 lealnumeros-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 00:14:16.264356 lealnumeros-0.0.2/lealNumeros/
--rw-rw-rw-   0        0        0       32 2023-05-14 20:13:46.000000 lealnumeros-0.0.2/lealNumeros/__init__.py
--rw-rw-rw-   0        0        0     2018 2023-05-14 20:12:56.000000 lealnumeros-0.0.2/lealNumeros/main.py
-drwxrwxrwx   0        0        0        0 2023-05-15 00:14:16.300335 lealnumeros-0.0.2/lealnumeros.egg-info/
--rw-rw-rw-   0        0        0     1278 2023-05-15 00:14:16.000000 lealnumeros-0.0.2/lealnumeros.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-05-15 00:14:16.000000 lealnumeros-0.0.2/lealnumeros.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 00:14:16.000000 lealnumeros-0.0.2/lealnumeros.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-15 00:14:16.000000 lealnumeros-0.0.2/lealnumeros.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-15 00:14:16.000000 lealnumeros-0.0.2/lealnumeros.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-15 00:14:16.303334 lealnumeros-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      517 2023-05-15 00:05:12.000000 lealnumeros-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 05:02:26.996460 lealnumeros-0.0.3/
+-rw-rw-rw-   0        0        0     1098 2023-05-14 20:25:14.000000 lealnumeros-0.0.3/LICENCE
+-rw-rw-rw-   0        0        0     1278 2023-05-16 05:02:26.995450 lealnumeros-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      932 2023-05-14 23:53:56.000000 lealnumeros-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-16 05:02:26.959481 lealnumeros-0.0.3/lealNumeros/
+-rw-rw-rw-   0        0        0       32 2023-05-14 20:13:46.000000 lealnumeros-0.0.3/lealNumeros/__init__.py
+-rw-rw-rw-   0        0        0     2452 2023-05-16 04:59:56.000000 lealnumeros-0.0.3/lealNumeros/main.py
+drwxrwxrwx   0        0        0        0 2023-05-16 05:02:26.993462 lealnumeros-0.0.3/lealnumeros.egg-info/
+-rw-rw-rw-   0        0        0     1278 2023-05-16 05:02:26.000000 lealnumeros-0.0.3/lealnumeros.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-05-16 05:02:26.000000 lealnumeros-0.0.3/lealnumeros.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 05:02:26.000000 lealnumeros-0.0.3/lealnumeros.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-16 05:02:26.000000 lealnumeros-0.0.3/lealnumeros.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-16 05:02:26.000000 lealnumeros-0.0.3/lealnumeros.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-16 05:02:26.997449 lealnumeros-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      517 2023-05-16 05:01:32.000000 lealnumeros-0.0.3/setup.py
```

### Comparing `lealnumeros-0.0.2/LICENCE` & `lealnumeros-0.0.3/LICENCE`

 * *Files identical despite different names*

### Comparing `lealnumeros-0.0.2/PKG-INFO` & `lealnumeros-0.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lealnumeros
-Version: 0.0.2
+Version: 0.0.3
 Summary: Trabalhe com formatação de números de uma maneira rápido e fácil.
 Author: José Rodolfo
 Author-email: silvaleal.ctt@gmail.com
 License: MIT License
 Keywords: lealnumeros
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `lealnumeros-0.0.2/README.md` & `lealnumeros-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `lealnumeros-0.0.2/lealnumeros.egg-info/PKG-INFO` & `lealnumeros-0.0.3/lealnumeros.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lealnumeros
-Version: 0.0.2
+Version: 0.0.3
 Summary: Trabalhe com formatação de números de uma maneira rápido e fácil.
 Author: José Rodolfo
 Author-email: silvaleal.ctt@gmail.com
 License: MIT License
 Keywords: lealnumeros
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `lealnumeros-0.0.2/setup.py` & `lealnumeros-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open("README.md", "r") as arq:
     readme = arq.read()
 
 setup(name='lealnumeros',
-    version='0.0.2',
+    version='0.0.3',
     license='MIT License',
     author='José Rodolfo',
     long_description=readme,
     long_description_content_type="text/markdown",
     author_email='silvaleal.ctt@gmail.com',
     keywords='lealnumeros',
     description=u'Trabalhe com formatação de números de uma maneira rápido e fácil.',
```

