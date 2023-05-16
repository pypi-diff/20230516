# Comparing `tmp/lealnumeros-0.0.4.tar.gz` & `tmp/lealnumeros-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lealnumeros-0.0.4.tar", last modified: Tue May 16 05:08:21 2023, max compression
+gzip compressed data, was "lealnumeros-0.0.5.tar", last modified: Tue May 16 22:21:31 2023, max compression
```

## Comparing `lealnumeros-0.0.4.tar` & `lealnumeros-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 05:08:21.289503 lealnumeros-0.0.4/
--rw-rw-rw-   0        0        0     1098 2023-05-14 20:25:14.000000 lealnumeros-0.0.4/LICENCE
--rw-rw-rw-   0        0        0     1431 2023-05-16 05:08:21.287505 lealnumeros-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1081 2023-05-16 05:05:38.000000 lealnumeros-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-16 05:08:21.256523 lealnumeros-0.0.4/lealNumeros/
--rw-rw-rw-   0        0        0       32 2023-05-14 20:13:46.000000 lealnumeros-0.0.4/lealNumeros/__init__.py
--rw-rw-rw-   0        0        0     2452 2023-05-16 04:59:56.000000 lealnumeros-0.0.4/lealNumeros/main.py
-drwxrwxrwx   0        0        0        0 2023-05-16 05:08:21.284506 lealnumeros-0.0.4/lealnumeros.egg-info/
--rw-rw-rw-   0        0        0     1431 2023-05-16 05:08:21.000000 lealnumeros-0.0.4/lealnumeros.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-05-16 05:08:21.000000 lealnumeros-0.0.4/lealnumeros.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 05:08:21.000000 lealnumeros-0.0.4/lealnumeros.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-16 05:08:21.000000 lealnumeros-0.0.4/lealnumeros.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-16 05:08:21.000000 lealnumeros-0.0.4/lealnumeros.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-16 05:08:21.289503 lealnumeros-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      517 2023-05-16 05:08:02.000000 lealnumeros-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 22:21:31.305223 lealnumeros-0.0.5/
+-rw-rw-rw-   0        0        0     1098 2023-05-14 20:25:14.000000 lealnumeros-0.0.5/LICENCE
+-rw-rw-rw-   0        0        0     1431 2023-05-16 22:21:31.304223 lealnumeros-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1081 2023-05-16 05:05:38.000000 lealnumeros-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-16 22:21:31.261248 lealnumeros-0.0.5/lealNumeros/
+-rw-rw-rw-   0        0        0       32 2023-05-14 20:13:46.000000 lealnumeros-0.0.5/lealNumeros/__init__.py
+-rw-rw-rw-   0        0        0     4021 2023-05-16 22:19:27.000000 lealnumeros-0.0.5/lealNumeros/main.py
+drwxrwxrwx   0        0        0        0 2023-05-16 22:21:31.302224 lealnumeros-0.0.5/lealnumeros.egg-info/
+-rw-rw-rw-   0        0        0     1431 2023-05-16 22:21:31.000000 lealnumeros-0.0.5/lealnumeros.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-05-16 22:21:31.000000 lealnumeros-0.0.5/lealnumeros.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 22:21:31.000000 lealnumeros-0.0.5/lealnumeros.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-16 22:21:31.000000 lealnumeros-0.0.5/lealnumeros.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-16 22:21:31.000000 lealnumeros-0.0.5/lealnumeros.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-16 22:21:31.305223 lealnumeros-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      517 2023-05-16 22:20:54.000000 lealnumeros-0.0.5/setup.py
```

### Comparing `lealnumeros-0.0.4/LICENCE` & `lealnumeros-0.0.5/LICENCE`

 * *Files identical despite different names*

### Comparing `lealnumeros-0.0.4/PKG-INFO` & `lealnumeros-0.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lealnumeros
-Version: 0.0.4
+Version: 0.0.5
 Summary: Trabalhe com formatação de números de uma maneira rápido e fácil.
 Author: José Rodolfo
 Author-email: silvaleal.ctt@gmail.com
 License: MIT License
 Keywords: lealnumeros
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `lealnumeros-0.0.4/README.md` & `lealnumeros-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `lealnumeros-0.0.4/lealnumeros.egg-info/PKG-INFO` & `lealnumeros-0.0.5/lealnumeros.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lealnumeros
-Version: 0.0.4
+Version: 0.0.5
 Summary: Trabalhe com formatação de números de uma maneira rápido e fácil.
 Author: José Rodolfo
 Author-email: silvaleal.ctt@gmail.com
 License: MIT License
 Keywords: lealnumeros
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `lealnumeros-0.0.4/setup.py` & `lealnumeros-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open("README.md", "r") as arq:
     readme = arq.read()
 
 setup(name='lealnumeros',
-    version='0.0.4',
+    version='0.0.5',
     license='MIT License',
     author='José Rodolfo',
     long_description=readme,
     long_description_content_type="text/markdown",
     author_email='silvaleal.ctt@gmail.com',
     keywords='lealnumeros',
     description=u'Trabalhe com formatação de números de uma maneira rápido e fácil.',
```

