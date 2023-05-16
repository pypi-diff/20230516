# Comparing `tmp/fparse-1.20.0.tar.gz` & `tmp/fparse-1.20.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fparse-1.20.0.tar", last modified: Tue May 16 02:30:53 2023, max compression
+gzip compressed data, was "fparse-1.20.1.tar", last modified: Tue May 16 02:38:07 2023, max compression
```

## Comparing `fparse-1.20.0.tar` & `fparse-1.20.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 bendichter   (502) staff       (20)        0 2023-05-16 02:30:53.149285 fparse-1.20.0/
--rw-r--r--   0 bendichter   (502) staff       (20)     1085 2023-05-15 16:57:19.000000 fparse-1.20.0/LICENSE
--rw-r--r--   0 bendichter   (502) staff       (20)       40 2023-05-15 16:57:19.000000 fparse-1.20.0/MANIFEST.in
--rw-r--r--   0 bendichter   (502) staff       (20)    19747 2023-05-16 02:30:53.149105 fparse-1.20.0/PKG-INFO
--rw-r--r--   0 bendichter   (502) staff       (20)    18975 2023-05-16 02:30:53.000000 fparse-1.20.0/README.rst
-drwxr-xr-x   0 bendichter   (502) staff       (20)        0 2023-05-16 02:30:53.148920 fparse-1.20.0/fparse.egg-info/
--rw-r--r--   0 bendichter   (502) staff       (20)    19747 2023-05-16 02:30:53.000000 fparse-1.20.0/fparse.egg-info/PKG-INFO
--rw-r--r--   0 bendichter   (502) staff       (20)      184 2023-05-16 02:30:53.000000 fparse-1.20.0/fparse.egg-info/SOURCES.txt
--rw-r--r--   0 bendichter   (502) staff       (20)        1 2023-05-16 02:30:53.000000 fparse-1.20.0/fparse.egg-info/dependency_links.txt
--rw-r--r--   0 bendichter   (502) staff       (20)        7 2023-05-16 02:30:53.000000 fparse-1.20.0/fparse.egg-info/top_level.txt
--rw-r--r--   0 bendichter   (502) staff       (20)    53944 2023-05-16 02:25:39.000000 fparse-1.20.0/fparse.py
--rw-r--r--   0 bendichter   (502) staff       (20)       38 2023-05-16 02:30:53.149331 fparse-1.20.0/setup.cfg
--rwxr-xr-x   0 bendichter   (502) staff       (20)     1107 2023-05-16 02:26:03.000000 fparse-1.20.0/setup.py
--rwxr-xr-x   0 bendichter   (502) staff       (20)    44517 2023-05-15 16:57:19.000000 fparse-1.20.0/test_fparse.py
+drwxr-xr-x   0 bendichter   (502) staff       (20)        0 2023-05-16 02:38:07.792762 fparse-1.20.1/
+-rw-r--r--   0 bendichter   (502) staff       (20)     1085 2023-05-15 16:57:19.000000 fparse-1.20.1/LICENSE
+-rw-r--r--   0 bendichter   (502) staff       (20)       40 2023-05-15 16:57:19.000000 fparse-1.20.1/MANIFEST.in
+-rw-r--r--   0 bendichter   (502) staff       (20)    19899 2023-05-16 02:38:07.792579 fparse-1.20.1/PKG-INFO
+-rw-r--r--   0 bendichter   (502) staff       (20)    19125 2023-05-16 02:38:07.000000 fparse-1.20.1/README.rst
+drwxr-xr-x   0 bendichter   (502) staff       (20)        0 2023-05-16 02:38:07.792381 fparse-1.20.1/fparse.egg-info/
+-rw-r--r--   0 bendichter   (502) staff       (20)    19899 2023-05-16 02:38:07.000000 fparse-1.20.1/fparse.egg-info/PKG-INFO
+-rw-r--r--   0 bendichter   (502) staff       (20)      184 2023-05-16 02:38:07.000000 fparse-1.20.1/fparse.egg-info/SOURCES.txt
+-rw-r--r--   0 bendichter   (502) staff       (20)        1 2023-05-16 02:38:07.000000 fparse-1.20.1/fparse.egg-info/dependency_links.txt
+-rw-r--r--   0 bendichter   (502) staff       (20)        7 2023-05-16 02:38:07.000000 fparse-1.20.1/fparse.egg-info/top_level.txt
+-rw-r--r--   0 bendichter   (502) staff       (20)    54096 2023-05-16 02:37:25.000000 fparse-1.20.1/fparse.py
+-rw-r--r--   0 bendichter   (502) staff       (20)       38 2023-05-16 02:38:07.792803 fparse-1.20.1/setup.cfg
+-rwxr-xr-x   0 bendichter   (502) staff       (20)     1109 2023-05-16 02:34:17.000000 fparse-1.20.1/setup.py
+-rwxr-xr-x   0 bendichter   (502) staff       (20)    44517 2023-05-15 16:57:19.000000 fparse-1.20.1/test_fparse.py
```

### Comparing `fparse-1.20.0/LICENSE` & `fparse-1.20.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fparse-1.20.0/PKG-INFO` & `fparse-1.20.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: fparse
-Version: 1.20.0
+Version: 1.20.1
 Summary: parse() is the opposite of format()
-Home-page: https://github.com/r1chardj0n3s/parse
+Home-page: https://github.com/catalystneuro/fparse
 Author: Richard Jones & Ben Dichter
 Author-email: ben.dichter@catalystneuro.com
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: BSD License
 License-File: LICENSE
 
+This is a fork of the `parse library`_ that adds the ability to parse datetime formats.
+
 Parse strings using a specification based on the Python format() syntax.
 
    ``parse()`` is the opposite of ``format()``
 
 The module is set up to only export ``parse()``, ``search()``, ``findall()``,
 and ``with_pattern()`` when ``import \*`` is used:
 
@@ -292,15 +294,16 @@
 
 .. _`Format String Syntax`:
   http://docs.python.org/library/string.html#format-string-syntax
 .. _`Format Specification Mini-Language`:
   http://docs.python.org/library/string.html#format-specification-mini-language
 .. _`1989 C standard format codes`:
   https://docs.python.org/3/library/datetime.html#strftime-and-strptime-format-codes
-
+.. _`parse library`:
+  https://github.com/r1chardj0n3s/parse
 
 Result and Match Objects
 ------------------------
 
 The result of a ``parse()`` and ``search()`` operation is either ``None`` (no match), a
 ``Result`` instance or a ``Match`` instance if ``evaluate_result`` is False.
 
@@ -357,15 +360,15 @@
     >>> assert _ is None, "MISMATCH"
 
 You can also use the ``with_pattern(pattern)`` decorator to add this
 information to a type converter function:
 
 .. code-block:: pycon
 
-    >>> from parse import with_pattern
+    >>> from fparse import with_pattern
     >>> @with_pattern(r'\d+')
     ... def parse_number(text):
     ...    return int(text)
     >>> parse('Answer: {number:Number}', 'Answer: 42', dict(Number=parse_number))
     <Result () {'number': 42}>
 
 A more complete example of a custom type might be:
```

### Comparing `fparse-1.20.0/README.rst` & `fparse-1.20.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+This is a fork of the `parse library`_ that adds the ability to parse datetime formats.
+
 Parse strings using a specification based on the Python format() syntax.
 
    ``parse()`` is the opposite of ``format()``
 
 The module is set up to only export ``parse()``, ``search()``, ``findall()``,
 and ``with_pattern()`` when ``import \*`` is used:
 
@@ -273,15 +275,16 @@
 
 .. _`Format String Syntax`:
   http://docs.python.org/library/string.html#format-string-syntax
 .. _`Format Specification Mini-Language`:
   http://docs.python.org/library/string.html#format-specification-mini-language
 .. _`1989 C standard format codes`:
   https://docs.python.org/3/library/datetime.html#strftime-and-strptime-format-codes
-
+.. _`parse library`:
+  https://github.com/r1chardj0n3s/parse
 
 Result and Match Objects
 ------------------------
 
 The result of a ``parse()`` and ``search()`` operation is either ``None`` (no match), a
 ``Result`` instance or a ``Match`` instance if ``evaluate_result`` is False.
 
@@ -338,15 +341,15 @@
     >>> assert _ is None, "MISMATCH"
 
 You can also use the ``with_pattern(pattern)`` decorator to add this
 information to a type converter function:
 
 .. code-block:: pycon
 
-    >>> from parse import with_pattern
+    >>> from fparse import with_pattern
     >>> @with_pattern(r'\d+')
     ... def parse_number(text):
     ...    return int(text)
     >>> parse('Answer: {number:Number}', 'Answer: 42', dict(Number=parse_number))
     <Result () {'number': 42}>
 
 A more complete example of a custom type might be:
```

### Comparing `fparse-1.20.0/fparse.egg-info/PKG-INFO` & `fparse-1.20.1/fparse.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: fparse
-Version: 1.20.0
+Version: 1.20.1
 Summary: parse() is the opposite of format()
-Home-page: https://github.com/r1chardj0n3s/parse
+Home-page: https://github.com/catalystneuro/fparse
 Author: Richard Jones & Ben Dichter
 Author-email: ben.dichter@catalystneuro.com
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: BSD License
 License-File: LICENSE
 
+This is a fork of the `parse library`_ that adds the ability to parse datetime formats.
+
 Parse strings using a specification based on the Python format() syntax.
 
    ``parse()`` is the opposite of ``format()``
 
 The module is set up to only export ``parse()``, ``search()``, ``findall()``,
 and ``with_pattern()`` when ``import \*`` is used:
 
@@ -292,15 +294,16 @@
 
 .. _`Format String Syntax`:
   http://docs.python.org/library/string.html#format-string-syntax
 .. _`Format Specification Mini-Language`:
   http://docs.python.org/library/string.html#format-specification-mini-language
 .. _`1989 C standard format codes`:
   https://docs.python.org/3/library/datetime.html#strftime-and-strptime-format-codes
-
+.. _`parse library`:
+  https://github.com/r1chardj0n3s/parse
 
 Result and Match Objects
 ------------------------
 
 The result of a ``parse()`` and ``search()`` operation is either ``None`` (no match), a
 ``Result`` instance or a ``Match`` instance if ``evaluate_result`` is False.
 
@@ -357,15 +360,15 @@
     >>> assert _ is None, "MISMATCH"
 
 You can also use the ``with_pattern(pattern)`` decorator to add this
 information to a type converter function:
 
 .. code-block:: pycon
 
-    >>> from parse import with_pattern
+    >>> from fparse import with_pattern
     >>> @with_pattern(r'\d+')
     ... def parse_number(text):
     ...    return int(text)
     >>> parse('Answer: {number:Number}', 'Answer: 42', dict(Number=parse_number))
     <Result () {'number': 42}>
 
 A more complete example of a custom type might be:
```

### Comparing `fparse-1.20.0/fparse.py` & `fparse-1.20.1/fparse.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-r'''Parse strings using a specification based on the Python format() syntax.
+r'''This is a fork of the `parse library`_ that adds the ability to parse datetime formats.
+
+Parse strings using a specification based on the Python format() syntax.
 
    ``parse()`` is the opposite of ``format()``
 
 The module is set up to only export ``parse()``, ``search()``, ``findall()``,
 and ``with_pattern()`` when ``import \*`` is used:
 
 >>> from fparse import *
@@ -273,15 +275,16 @@
 
 .. _`Format String Syntax`:
   http://docs.python.org/library/string.html#format-string-syntax
 .. _`Format Specification Mini-Language`:
   http://docs.python.org/library/string.html#format-specification-mini-language
 .. _`1989 C standard format codes`:
   https://docs.python.org/3/library/datetime.html#strftime-and-strptime-format-codes
-
+.. _`parse library`:
+  https://github.com/r1chardj0n3s/parse
 
 Result and Match Objects
 ------------------------
 
 The result of a ``parse()`` and ``search()`` operation is either ``None`` (no match), a
 ``Result`` instance or a ``Match`` instance if ``evaluate_result`` is False.
 
@@ -338,15 +341,15 @@
     >>> assert _ is None, "MISMATCH"
 
 You can also use the ``with_pattern(pattern)`` decorator to add this
 information to a type converter function:
 
 .. code-block:: pycon
 
-    >>> from parse import with_pattern
+    >>> from fparse import with_pattern
     >>> @with_pattern(r'\d+')
     ... def parse_number(text):
     ...    return int(text)
     >>> parse('Answer: {number:Number}', 'Answer: 42', dict(Number=parse_number))
     <Result () {'number': 42}>
 
 A more complete example of a custom type might be:
@@ -479,15 +482,15 @@
 
 This code is copyright 2012-2021 Richard Jones <richard@python.org>
 See the end of the source file for the license of use.
 '''
 
 from __future__ import absolute_import
 
-__version__ = '1.20.0'
+__version__ = '1.20.1'
 
 # yes, I now have two problems
 import re
 import sys
 from copy import copy
 from datetime import datetime, time, tzinfo, timedelta
 from decimal import Decimal
@@ -502,16 +505,16 @@
 def with_pattern(pattern, regex_group_count=None):
     r"""Attach a regular expression pattern matcher to a custom type converter
     function.
 
     This annotates the type converter with the :attr:`pattern` attribute.
 
     EXAMPLE:
-        >>> import parse
-        >>> @parse.with_pattern(r"\d+")
+        >>> import fparse
+        >>> @fparse.with_pattern(r"\d+")
         ... def parse_number(text):
         ...     return int(text)
 
     is equivalent to:
 
         >>> def parse_number(text):
         ...     return int(text)
```

### Comparing `fparse-1.20.0/setup.py` & `fparse-1.20.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     name="fparse",
     version=__version__,
     description="parse() is the opposite of format()",
     long_description=__doc__,
     author="Richard Jones & Ben Dichter",
     author_email="ben.dichter@catalystneuro.com",
     py_modules=['fparse'],
-    url='https://github.com/r1chardj0n3s/parse',
+    url='https://github.com/catalystneuro/fparse',
     classifiers=[
         'Environment :: Web Environment',
         'Intended Audience :: Developers',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
```

### Comparing `fparse-1.20.0/test_fparse.py` & `fparse-1.20.1/test_fparse.py`

 * *Files identical despite different names*

