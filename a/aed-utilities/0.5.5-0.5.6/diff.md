# Comparing `tmp/aed_utilities-0.5.5.tar.gz` & `tmp/aed_utilities-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aed_utilities-0.5.5.tar", last modified: Wed Jun  1 14:24:46 2022, max compression
+gzip compressed data, was "aed_utilities-0.5.6.tar", last modified: Tue May 16 16:38:31 2023, max compression
```

## Comparing `aed_utilities-0.5.5.tar` & `aed_utilities-0.5.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
-drwxrwxrwx   0        0        0        0 2022-06-01 14:24:46.584132 aed_utilities-0.5.5/
--rw-rw-rw-   0        0        0      842 2022-06-01 14:24:46.584132 aed_utilities-0.5.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-06-01 14:24:46.584132 aed_utilities-0.5.5/aed_utilities/
--rw-rw-rw-   0        0        0       41 2021-02-26 12:47:42.041774 aed_utilities-0.5.5/aed_utilities/__init__.py
--rw-rw-rw-   0        0        0    12381 2022-06-01 13:58:44.325940 aed_utilities-0.5.5/aed_utilities/visualizacion.py
--rw-rw-rw-   0        0        0       61 2021-01-21 20:47:51.168849 aed_utilities-0.5.5/setup.cfg
--rw-rw-rw-   0        0        0     1758 2022-06-01 14:14:11.931784 aed_utilities-0.5.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 16:38:31.034361 aed_utilities-0.5.6/
+-rw-rw-rw-   0        0        0      842 2023-05-16 16:38:31.034361 aed_utilities-0.5.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-16 16:38:31.034361 aed_utilities-0.5.6/aed_utilities/
+-rw-rw-rw-   0        0        0       41 2021-02-26 12:47:42.041774 aed_utilities-0.5.6/aed_utilities/__init__.py
+-rw-rw-rw-   0        0        0    12388 2023-05-16 16:33:27.404940 aed_utilities-0.5.6/aed_utilities/visualizacion.py
+-rw-rw-rw-   0        0        0       61 2021-01-21 20:47:51.168849 aed_utilities-0.5.6/setup.cfg
+-rw-rw-rw-   0        0        0     1758 2023-05-16 16:34:35.481351 aed_utilities-0.5.6/setup.py
```

### Comparing `aed_utilities-0.5.5/PKG-INFO` & `aed_utilities-0.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: aed_utilities
-Version: 0.5.5
+Version: 0.5.6
 Summary: Herramientas basicas de dibujo de estructuras de datos
 Home-page: https://github.com/ivansipiran/aed_utilities
 Author: Profesores del Curso
 Author-email: isipiran@dcc.uchile.cl
 License: MIT
-Download-URL: https://github.com/ivansipiran/aed-utilities/archive/refs/tags/v0.5.5.tar.gz
+Download-URL: https://github.com/ivansipiran/aed-utilities/archive/refs/tags/v0.5.6.tar.gz
 Description: UNKNOWN
 Keywords: estructuras de datos,algoritmos
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aed_utilities-0.5.5/aed_utilities/visualizacion.py` & `aed_utilities-0.5.6/aed_utilities/visualizacion.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
     code = "node" + str(self.counterNodes)
     self.counterNodes = self.counterNodes + 1
     return code
 
   def copy_tree(self, node):
     if self.classNone is not None:
       if isinstance(node, self.classNone):
-        if not hasattr(node, "info"):
+        if not hasattr(node, self.nameInfo):
           if not self.drawNull:
             return None
           else:
             newNode = PositionNode(None, "", None, "square", "null" + str(self.counterNull))
             self.counterNull = self.counterNull + 1
             return newNode
         else:
```

### Comparing `aed_utilities-0.5.5/setup.py` & `aed_utilities-0.5.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from distutils.core import setup
 setup(
   name = 'aed_utilities',         # How you named your package folder (MyLib)
   packages = ['aed_utilities'],   # Chose the same as "name"
-  version = '0.5.5',      # Start with a small number and increase it with every change you make
+  version = '0.5.6',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'Herramientas basicas de dibujo de estructuras de datos',   # Give a short description about your library
   author = 'Profesores del Curso',                   # Type in your name
   author_email = 'isipiran@dcc.uchile.cl',      # Type in your E-Mail
   url = 'https://github.com/ivansipiran/aed_utilities',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/ivansipiran/aed-utilities/archive/refs/tags/v0.5.5.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/ivansipiran/aed-utilities/archive/refs/tags/v0.5.6.tar.gz',    # I explain this later on
   keywords = ['estructuras de datos', 'algoritmos'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'validators',
           'beautifulsoup4',
       ],
   classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
```

