# Comparing `tmp/mslex-0.3.0.tar.gz` & `tmp/mslex-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mslex-0.3.0.tar", last modified: Sun Oct  6 21:56:48 2019, max compression
+gzip compressed data, was "mslex-1.0.0.tar", last modified: Mon May 15 20:30:08 2023, max compression
```

## Comparing `mslex-0.3.0.tar` & `mslex-1.0.0.tar`

### file list

```diff
@@ -1,38 +1,32 @@
-drwxr-xr-x   0 lawrence_danna (941817330) admin       (80)        0 2019-10-06 21:56:48.000000 mslex-0.3.0/
--rw-r--r--   0 lawrence_danna (941817330) admin       (80)     2921 2019-10-06 21:56:48.000000 mslex-0.3.0/PKG-INFO
--rw-r--r--   0 lawrence_danna (941817330) admin       (80)      587 2019-10-06 07:06:25.000000 mslex-0.3.0/LICENSE
--rw-r--r--   0 lawrence_danna (941817330) admin       (80)     3497 2019-10-06 07:06:25.000000 mslex-0.3.0/CONTRIBUTING.rst
-drwxr-xr-x   0 lawrence_danna (941817330) admin       (80)        0 2019-10-06 21:56:48.000000 mslex-0.3.0/mslex.egg-info/
--rw-r--r--   0 lawrence_danna (941817330) admin       (80)     2921 2019-10-06 21:56:47.000000 mslex-0.3.0/mslex.egg-info/PKG-INFO
--rw-r--r--   0 lawrence_danna (941817330) admin       (80)        1 2019-10-03 04:23:25.000000 mslex-0.3.0/mslex.egg-info/not-zip-safe
--rw-r--r--   0 lawrence_danna (941817330) admin       (80)      581 2019-10-06 21:56:47.000000 mslex-0.3.0/mslex.egg-info/SOURCES.txt
--rw-r--r--   0 lawrence_danna (941817330) admin       (80)       49 2019-10-06 21:56:47.000000 mslex-0.3.0/mslex.egg-info/entry_points.txt
--rw-r--r--   0 lawrence_danna (941817330) admin       (80)        6 2019-10-06 21:56:47.000000 mslex-0.3.0/mslex.egg-info/top_level.txt
--rw-r--r--   0 lawrence_danna (941817330) admin       (80)        1 2019-10-06 21:56:47.000000 mslex-0.3.0/mslex.egg-info/dependency_links.txt
-drwxr-xr-x   0 lawrence_danna (941817330) admin       (80)        0 2019-10-06 21:56:48.000000 mslex-0.3.0/tests/
--rw-r--r--   0 lawrence_danna (941817330) admin       (80)       60 2019-10-06 07:06:25.000000 mslex-0.3.0/tests/__init__.py
--rw-r--r--   0 lawrence_danna (941817330) admin       (80)    12030 2019-10-06 21:52:52.000000 mslex-0.3.0/tests/test_mslex.py
--rw-r--r--   0 lawrence_danna (941817330) admin       (80)      262 2019-10-06 07:06:25.000000 mslex-0.3.0/MANIFEST.in
-drwxr-xr-x   0 lawrence_danna (941817330) admin       (80)        0 2019-10-06 21:56:48.000000 mslex-0.3.0/docs/
--rw-r--r--   0 lawrence_danna (941817330) admin       (80)      302 2019-10-06 07:06:25.000000 mslex-0.3.0/docs/index.rst
--rw-r--r--   0 lawrence_danna (941817330) admin       (80)       33 2019-10-06 07:06:25.000000 mslex-0.3.0/docs/contributing.rst
--rw-r--r--   0 lawrence_danna (941817330) admin       (80)      607 2019-10-06 07:06:25.000000 mslex-0.3.0/docs/Makefile
--rwxr-xr-x   0 lawrence_danna (941817330) admin       (80)     4793 2019-10-06 07:06:25.000000 mslex-0.3.0/docs/conf.py
--rw-r--r--   0 lawrence_danna (941817330) admin       (80)       65 2019-10-06 07:06:25.000000 mslex-0.3.0/docs/usage.rst
--rw-r--r--   0 lawrence_danna (941817330) admin       (80)      767 2019-10-06 07:06:25.000000 mslex-0.3.0/docs/make.bat
-drwxr-xr-x   0 lawrence_danna (941817330) admin       (80)        0 2019-10-06 21:56:48.000000 mslex-0.3.0/docs/_build/
-drwxr-xr-x   0 lawrence_danna (941817330) admin       (80)        0 2019-10-06 21:56:48.000000 mslex-0.3.0/docs/_build/html/
-drwxr-xr-x   0 lawrence_danna (941817330) admin       (80)        0 2019-10-06 21:56:48.000000 mslex-0.3.0/docs/_build/html/_static/
--rw-r--r--   0 lawrence_danna (941817330) admin       (80)       90 2019-10-03 05:23:34.000000 mslex-0.3.0/docs/_build/html/_static/plus.png
--rw-r--r--   0 lawrence_danna (941817330) admin       (80)      286 2019-10-03 05:23:34.000000 mslex-0.3.0/docs/_build/html/_static/file.png
--rw-r--r--   0 lawrence_danna (941817330) admin       (80)       90 2019-10-03 05:23:34.000000 mslex-0.3.0/docs/_build/html/_static/minus.png
--rw-r--r--   0 lawrence_danna (941817330) admin       (80)       28 2019-10-06 07:06:25.000000 mslex-0.3.0/docs/history.rst
--rw-r--r--   0 lawrence_danna (941817330) admin       (80)     1094 2019-10-06 07:06:25.000000 mslex-0.3.0/docs/installation.rst
--rw-r--r--   0 lawrence_danna (941817330) admin       (80)       28 2019-10-06 07:06:25.000000 mslex-0.3.0/docs/authors.rst
--rw-r--r--   0 lawrence_danna (941817330) admin       (80)       27 2019-10-06 07:06:25.000000 mslex-0.3.0/docs/readme.rst
--rw-r--r--   0 lawrence_danna (941817330) admin       (80)     1411 2019-10-06 21:54:49.000000 mslex-0.3.0/setup.py
--rw-r--r--   0 lawrence_danna (941817330) admin       (80)       89 2019-10-06 07:06:25.000000 mslex-0.3.0/HISTORY.rst
--rw-r--r--   0 lawrence_danna (941817330) admin       (80)      161 2019-10-06 07:06:25.000000 mslex-0.3.0/AUTHORS.rst
--rw-r--r--   0 lawrence_danna (941817330) admin       (80)      379 2019-10-06 21:56:48.000000 mslex-0.3.0/setup.cfg
--rw-r--r--   0 lawrence_danna (941817330) admin       (80)     1678 2019-10-06 07:06:25.000000 mslex-0.3.0/README.rst
--rw-r--r--   0 lawrence_danna (941817330) admin       (80)     5089 2019-10-06 21:54:49.000000 mslex-0.3.0/mslex.py
+drwxr-xr-x   0 larry      (502) staff       (20)        0 2023-05-15 20:30:08.272588 mslex-1.0.0/
+-rw-r--r--   0 larry      (502) staff       (20)      161 2023-03-22 17:56:02.000000 mslex-1.0.0/AUTHORS.rst
+-rw-r--r--   0 larry      (502) staff       (20)     3497 2023-03-22 17:56:02.000000 mslex-1.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 larry      (502) staff       (20)       89 2023-03-22 17:56:02.000000 mslex-1.0.0/HISTORY.rst
+-rw-r--r--   0 larry      (502) staff       (20)      587 2023-03-22 17:56:02.000000 mslex-1.0.0/LICENSE
+-rw-r--r--   0 larry      (502) staff       (20)      262 2023-03-22 17:56:02.000000 mslex-1.0.0/MANIFEST.in
+-rw-r--r--   0 larry      (502) staff       (20)     2769 2023-05-15 20:30:08.272642 mslex-1.0.0/PKG-INFO
+-rw-r--r--   0 larry      (502) staff       (20)     1973 2023-05-15 20:22:39.000000 mslex-1.0.0/README.rst
+drwxr-xr-x   0 larry      (502) staff       (20)        0 2023-05-15 20:30:08.271451 mslex-1.0.0/docs/
+-rw-r--r--   0 larry      (502) staff       (20)      607 2023-03-22 17:56:02.000000 mslex-1.0.0/docs/Makefile
+-rw-r--r--   0 larry      (502) staff       (20)       28 2023-03-22 17:56:02.000000 mslex-1.0.0/docs/authors.rst
+-rwxr-xr-x   0 larry      (502) staff       (20)     4793 2023-03-22 17:56:02.000000 mslex-1.0.0/docs/conf.py
+-rw-r--r--   0 larry      (502) staff       (20)       33 2023-03-22 17:56:02.000000 mslex-1.0.0/docs/contributing.rst
+-rw-r--r--   0 larry      (502) staff       (20)       28 2023-03-22 17:56:02.000000 mslex-1.0.0/docs/history.rst
+-rw-r--r--   0 larry      (502) staff       (20)      302 2023-03-22 17:56:02.000000 mslex-1.0.0/docs/index.rst
+-rw-r--r--   0 larry      (502) staff       (20)     1094 2023-03-22 17:56:02.000000 mslex-1.0.0/docs/installation.rst
+-rw-r--r--   0 larry      (502) staff       (20)      767 2023-03-22 17:56:02.000000 mslex-1.0.0/docs/make.bat
+-rw-r--r--   0 larry      (502) staff       (20)       27 2023-03-22 17:56:02.000000 mslex-1.0.0/docs/readme.rst
+-rw-r--r--   0 larry      (502) staff       (20)       65 2023-03-22 17:56:02.000000 mslex-1.0.0/docs/usage.rst
+drwxr-xr-x   0 larry      (502) staff       (20)        0 2023-05-15 20:30:08.272233 mslex-1.0.0/mslex.egg-info/
+-rw-r--r--   0 larry      (502) staff       (20)     2769 2023-05-15 20:30:08.000000 mslex-1.0.0/mslex.egg-info/PKG-INFO
+-rw-r--r--   0 larry      (502) staff       (20)      478 2023-05-15 20:30:08.000000 mslex-1.0.0/mslex.egg-info/SOURCES.txt
+-rw-r--r--   0 larry      (502) staff       (20)        1 2023-05-15 20:30:08.000000 mslex-1.0.0/mslex.egg-info/dependency_links.txt
+-rw-r--r--   0 larry      (502) staff       (20)       48 2023-05-15 20:30:08.000000 mslex-1.0.0/mslex.egg-info/entry_points.txt
+-rw-r--r--   0 larry      (502) staff       (20)        1 2023-05-15 20:22:02.000000 mslex-1.0.0/mslex.egg-info/not-zip-safe
+-rw-r--r--   0 larry      (502) staff       (20)        6 2023-05-15 20:30:08.000000 mslex-1.0.0/mslex.egg-info/top_level.txt
+-rw-r--r--   0 larry      (502) staff       (20)     5089 2023-05-15 20:19:16.000000 mslex-1.0.0/mslex.py
+-rw-r--r--   0 larry      (502) staff       (20)      379 2023-05-15 20:30:08.272902 mslex-1.0.0/setup.cfg
+-rw-r--r--   0 larry      (502) staff       (20)     1419 2023-05-15 20:26:51.000000 mslex-1.0.0/setup.py
+drwxr-xr-x   0 larry      (502) staff       (20)        0 2023-05-15 20:30:08.272485 mslex-1.0.0/tests/
+-rw-r--r--   0 larry      (502) staff       (20)       60 2023-03-22 17:56:02.000000 mslex-1.0.0/tests/__init__.py
+-rw-r--r--   0 larry      (502) staff       (20)    12080 2023-05-15 20:19:16.000000 mslex-1.0.0/tests/test_mslex.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `mslex-0.3.0/PKG-INFO` & `mslex-1.0.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,79 +1,85 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: mslex
-Version: 0.3.0
+Version: 1.0.0
 Summary: shlex for windows
 Home-page: https://github.com/smoofra/mslex
 Author: Lawrence D'Anna
 Author-email: larry@elder-gods.org
 License: Apache Software License 2.0
-Description: =====
-        mslex
-        =====
-        
-        
-        .. image:: https://img.shields.io/pypi/v/mslex.svg
-                :target: https://pypi.python.org/pypi/mslex
-        
-        .. image:: https://img.shields.io/travis/smoofra/mslex.svg
-                :target: https://travis-ci.org/smoofra/mslex
-        
-        .. image:: https://readthedocs.org/projects/mslex/badge/?version=latest
-                :target: https://mslex.readthedocs.io/en/latest/?badge=latest
-                :alt: Documentation Status
-        
-        
-        shlex for windows
-        
-        * Free software: Apache Software License 2.0
-        * Documentation: https://mslex.readthedocs.io.
-        
-        Features
-        --------
-        
-        This is the missing shlex package for windows shell quoting.   It provides two
-        functions -- split and quote -- just like shlex.
-        
-        
-        Credits
-        -------
-        
-        These are excellent articles to read if you really want to face the
-        sanity-melting reality buried under the surface of how windows passes command
-        line arguments to your programs.   I recommend you read something else.
-        
-        * `How a Windows Program Splits Its Command Line Into Individual Arguments`_
-        
-        * `Everyone quotes command line arguments the wrong way`_
-        
-        .. _`How a Windows Program Splits Its Command Line Into Individual Arguments`:
-          http://www.windowsinspired.com/how-a-windows-programs-splits-its-command-line-into-individual-arguments/
-        
-        .. _`Everyone quotes command line arguments the wrong way`:
-          https://blogs.msdn.microsoft.com/twistylittlepassagesallalike/2011/04/23/everyone-quotes-command-line-arguments-the-wrong-way/
-        
-        This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
-        
-        .. _Cookiecutter: https://github.com/audreyr/cookiecutter
-        .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
-        
-        
-        =======
-        History
-        =======
-        
-        0.1.0 (2019-10-02)
-        ------------------
-        
-        * First release on PyPI.
-        
 Keywords: mslex
-Platform: UNKNOWN
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.5
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+=====
+mslex
+=====
+
+
+.. image:: https://img.shields.io/pypi/v/mslex.svg
+        :target: https://pypi.python.org/pypi/mslex
+
+.. image:: https://img.shields.io/travis/smoofra/mslex.svg
+        :target: https://travis-ci.org/smoofra/mslex
+
+.. image:: https://readthedocs.org/projects/mslex/badge/?version=latest
+        :target: https://mslex.readthedocs.io/en/latest/?badge=latest
+        :alt: Documentation Status
+
+
+shlex for windows
+
+* Free software: Apache Software License 2.0
+* Documentation: https://mslex.readthedocs.io.
+
+Features
+--------
+
+This is the missing shlex package for windows shell quoting.   It provides two
+functions -- split and quote -- just like shlex.
+
+
+Credits
+-------
+
+These are excellent articles to read if you really want to face the
+sanity-melting reality buried under the surface of how windows passes command
+line arguments to your programs.   I recommend you read something else.
+
+* `How a Windows Program Splits Its Command Line Into Individual Arguments`_
+
+  * The original URL is now dead, but fortunately the article is `backed up on the Internet Archive`_
+
+* `Everyone quotes command line arguments the wrong way`_
+
+.. _`How a Windows Program Splits Its Command Line Into Individual Arguments`:
+  http://www.windowsinspired.com/how-a-windows-programs-splits-its-command-line-into-individual-arguments/
+
+.. _`backed up on the Internet Archive`:
+  https://web.archive.org/web/20220629212422/http://www.windowsinspired.com/how-a-windows-programs-splits-its-command-line-into-individual-arguments/
+
+.. _`Everyone quotes command line arguments the wrong way`:
+  https://blogs.msdn.microsoft.com/twistylittlepassagesallalike/2011/04/23/everyone-quotes-command-line-arguments-the-wrong-way/
+
+This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
+
+.. _Cookiecutter: https://github.com/audreyr/cookiecutter
+.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
+
+
+=======
+History
+=======
+
+0.1.0 (2019-10-02)
+------------------
+
+* First release on PyPI.
```

### Comparing `mslex-0.3.0/LICENSE` & `mslex-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mslex-0.3.0/CONTRIBUTING.rst` & `mslex-1.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `mslex-0.3.0/mslex.egg-info/PKG-INFO` & `mslex-1.0.0/mslex.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,79 +1,85 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: mslex
-Version: 0.3.0
+Version: 1.0.0
 Summary: shlex for windows
 Home-page: https://github.com/smoofra/mslex
 Author: Lawrence D'Anna
 Author-email: larry@elder-gods.org
 License: Apache Software License 2.0
-Description: =====
-        mslex
-        =====
-        
-        
-        .. image:: https://img.shields.io/pypi/v/mslex.svg
-                :target: https://pypi.python.org/pypi/mslex
-        
-        .. image:: https://img.shields.io/travis/smoofra/mslex.svg
-                :target: https://travis-ci.org/smoofra/mslex
-        
-        .. image:: https://readthedocs.org/projects/mslex/badge/?version=latest
-                :target: https://mslex.readthedocs.io/en/latest/?badge=latest
-                :alt: Documentation Status
-        
-        
-        shlex for windows
-        
-        * Free software: Apache Software License 2.0
-        * Documentation: https://mslex.readthedocs.io.
-        
-        Features
-        --------
-        
-        This is the missing shlex package for windows shell quoting.   It provides two
-        functions -- split and quote -- just like shlex.
-        
-        
-        Credits
-        -------
-        
-        These are excellent articles to read if you really want to face the
-        sanity-melting reality buried under the surface of how windows passes command
-        line arguments to your programs.   I recommend you read something else.
-        
-        * `How a Windows Program Splits Its Command Line Into Individual Arguments`_
-        
-        * `Everyone quotes command line arguments the wrong way`_
-        
-        .. _`How a Windows Program Splits Its Command Line Into Individual Arguments`:
-          http://www.windowsinspired.com/how-a-windows-programs-splits-its-command-line-into-individual-arguments/
-        
-        .. _`Everyone quotes command line arguments the wrong way`:
-          https://blogs.msdn.microsoft.com/twistylittlepassagesallalike/2011/04/23/everyone-quotes-command-line-arguments-the-wrong-way/
-        
-        This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
-        
-        .. _Cookiecutter: https://github.com/audreyr/cookiecutter
-        .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
-        
-        
-        =======
-        History
-        =======
-        
-        0.1.0 (2019-10-02)
-        ------------------
-        
-        * First release on PyPI.
-        
 Keywords: mslex
-Platform: UNKNOWN
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.5
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+=====
+mslex
+=====
+
+
+.. image:: https://img.shields.io/pypi/v/mslex.svg
+        :target: https://pypi.python.org/pypi/mslex
+
+.. image:: https://img.shields.io/travis/smoofra/mslex.svg
+        :target: https://travis-ci.org/smoofra/mslex
+
+.. image:: https://readthedocs.org/projects/mslex/badge/?version=latest
+        :target: https://mslex.readthedocs.io/en/latest/?badge=latest
+        :alt: Documentation Status
+
+
+shlex for windows
+
+* Free software: Apache Software License 2.0
+* Documentation: https://mslex.readthedocs.io.
+
+Features
+--------
+
+This is the missing shlex package for windows shell quoting.   It provides two
+functions -- split and quote -- just like shlex.
+
+
+Credits
+-------
+
+These are excellent articles to read if you really want to face the
+sanity-melting reality buried under the surface of how windows passes command
+line arguments to your programs.   I recommend you read something else.
+
+* `How a Windows Program Splits Its Command Line Into Individual Arguments`_
+
+  * The original URL is now dead, but fortunately the article is `backed up on the Internet Archive`_
+
+* `Everyone quotes command line arguments the wrong way`_
+
+.. _`How a Windows Program Splits Its Command Line Into Individual Arguments`:
+  http://www.windowsinspired.com/how-a-windows-programs-splits-its-command-line-into-individual-arguments/
+
+.. _`backed up on the Internet Archive`:
+  https://web.archive.org/web/20220629212422/http://www.windowsinspired.com/how-a-windows-programs-splits-its-command-line-into-individual-arguments/
+
+.. _`Everyone quotes command line arguments the wrong way`:
+  https://blogs.msdn.microsoft.com/twistylittlepassagesallalike/2011/04/23/everyone-quotes-command-line-arguments-the-wrong-way/
+
+This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
+
+.. _Cookiecutter: https://github.com/audreyr/cookiecutter
+.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
+
+
+=======
+History
+=======
+
+0.1.0 (2019-10-02)
+------------------
+
+* First release on PyPI.
```

### Comparing `mslex-0.3.0/tests/test_mslex.py` & `mslex-1.0.0/tests/test_mslex.py`

 * *Files 1% similar despite different names*

```diff
@@ -223,26 +223,26 @@
     def case(self, s, ans, cmd):
         try:
             if ans is not None:
                 self.assertEqual(split(s, like_cmd=cmd), ans)
             if sys.platform == 'win32' and not cmd:
                 self.assertEqual(split(s), ctypes_split(s))
         except AssertionError:
-            print(f"in: «{s}»")
+            print("in: «{}»".format(s))
             print()
             for x in split(s, like_cmd=cmd):
-                print(f"out: «{x}»")
+                print("out: «{}»".format(x))
             print()
             if ans is not None:
                 for x in ans:
-                    print(f"ans: «{x}»")
+                    print("ans: «{}»".format(x))
                 print()
             if sys.platform == 'win32':
                 for x in ctypes_split(s):
-                    print(f"win: «{x}»")
+                    print("win: «{}»".format(x))
                 print()
             raise
 
 
     def setUp(self):
         """Set up test fixtures, if any."""
 
@@ -306,29 +306,29 @@
             prod = itertools.product(*itertools.repeat(chars, 8))
             for x in prod:
                 yield ''.join(x)
 
         for s in every_string():
             q = quote(s, for_cmd=False)
             self.assertEqual([s], split(q, like_cmd=False))
-            self.assertEqual([s, s], split(f'{q} {q}', like_cmd=False))
+            self.assertEqual([s, s], split('{} {}'.format(q,q), like_cmd=False))
 
 
     def test_quote_every_string_for_cmd(self):
 
         def every_string():
             chars = [' ', 'x', '"', '\\', '^', '&', '!']
             prod = itertools.product(*itertools.repeat(chars, 6))
             for x in prod:
                 yield ''.join(x)
 
         for s in every_string():
             q = quote(s)
             self.assertEqual([s], split(q))
-            self.assertEqual([s, s], split(f'{q} {q}'))
+            self.assertEqual([s, s], split('{} {}'.format(q,q)))
 
 
     @unittest.skipUnless(sys.platform == "win32", "requires Windows")
     def test_quote_every_string_using_cmd(self):
         def every_string():
             chars = [' ', 'x', '"', '\\', '^', '&']
             prod = itertools.product(*itertools.repeat(chars, 4))
```

### Comparing `mslex-0.3.0/docs/Makefile` & `mslex-1.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mslex-0.3.0/docs/conf.py` & `mslex-1.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mslex-0.3.0/docs/make.bat` & `mslex-1.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mslex-0.3.0/docs/installation.rst` & `mslex-1.0.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `mslex-0.3.0/setup.py` & `mslex-1.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 test_requirements = [ ]
 
 setup(
     author="Lawrence D'Anna",
     author_email='larry@elder-gods.org',
     python_requires='>=3.5',
     classifiers=[
-        'Development Status :: 2 - Pre-Alpha',
+        'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
@@ -44,10 +44,10 @@
     keywords='mslex',
     name='mslex',
     py_modules=['mslex'],
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/smoofra/mslex',
-    version='0.3.0',
+    version='1.0.0',
     zip_safe=False,
 )
```

### Comparing `mslex-0.3.0/README.rst` & `mslex-1.0.0/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -31,19 +31,24 @@
 
 These are excellent articles to read if you really want to face the
 sanity-melting reality buried under the surface of how windows passes command
 line arguments to your programs.   I recommend you read something else.
 
 * `How a Windows Program Splits Its Command Line Into Individual Arguments`_
 
+  * The original URL is now dead, but fortunately the article is `backed up on the Internet Archive`_
+
 * `Everyone quotes command line arguments the wrong way`_
 
 .. _`How a Windows Program Splits Its Command Line Into Individual Arguments`:
   http://www.windowsinspired.com/how-a-windows-programs-splits-its-command-line-into-individual-arguments/
 
+.. _`backed up on the Internet Archive`:
+  https://web.archive.org/web/20220629212422/http://www.windowsinspired.com/how-a-windows-programs-splits-its-command-line-into-individual-arguments/
+
 .. _`Everyone quotes command line arguments the wrong way`:
   https://blogs.msdn.microsoft.com/twistylittlepassagesallalike/2011/04/23/everyone-quotes-command-line-arguments-the-wrong-way/
 
 This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
 
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
```

### Comparing `mslex-0.3.0/mslex.py` & `mslex-1.0.0/mslex.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
                     yield '"'
                     quote_mode = not quote_mode
                 else:
                     yield text
                     if check:
                         meta = cmd_meta_inside_quotes if quote_mode else cmd_meta
                         if re.search(meta, text):
-                            raise ValueError(f"unquoted cmd metacharacters in string: {repr(s)}")
+                            raise ValueError("unquoted cmd metacharacters in string: " + repr(s))
         s = ''.join(i())
     return list(iter_args(s))
 
 
 
 def quote(s, for_cmd=True):
     """
```

