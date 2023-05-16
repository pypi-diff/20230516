# Comparing `tmp/nyoibo-0.4.1.tar.gz` & `tmp/nyoibo-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nyoibo-0.4.1.tar", last modified: Wed Mar  2 02:12:18 2022, max compression
+gzip compressed data, was "nyoibo-0.5.0.tar", last modified: Tue May 16 02:09:42 2023, max compression
```

## Comparing `nyoibo-0.4.1.tar` & `nyoibo-0.5.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 pity      (1000) pity      (1000)        0 2022-03-02 02:12:18.302881 nyoibo-0.4.1/
--rw-r--r--   0 pity      (1000) pity      (1000)     5707 2022-03-02 02:12:18.302881 nyoibo-0.4.1/PKG-INFO
--rw-r--r--   0 pity      (1000) pity      (1000)     3614 2022-03-02 02:01:30.000000 nyoibo-0.4.1/README.rst
-drwxr-xr-x   0 pity      (1000) pity      (1000)        0 2022-03-02 02:12:18.294881 nyoibo-0.4.1/nyoibo/
--rw-r--r--   0 pity      (1000) pity      (1000)       67 2022-03-02 02:09:47.000000 nyoibo-0.4.1/nyoibo/__init__.py
-drwxr-xr-x   0 pity      (1000) pity      (1000)        0 2022-03-02 02:12:18.298881 nyoibo-0.4.1/nyoibo/entities/
--rw-r--r--   0 pity      (1000) pity      (1000)       41 2020-07-03 03:22:00.000000 nyoibo-0.4.1/nyoibo/entities/__init__.py
--rw-r--r--   0 pity      (1000) pity      (1000)   218033 2022-02-21 02:38:07.000000 nyoibo-0.4.1/nyoibo/entities/entity.c
--rw-r--r--   0 pity      (1000) pity      (1000)     1752 2022-02-21 00:21:17.000000 nyoibo-0.4.1/nyoibo/entities/meta_entity.py
--rw-r--r--   0 pity      (1000) pity      (1000)      344 2022-02-21 02:23:48.000000 nyoibo-0.4.1/nyoibo/exceptions.py
--rw-r--r--   0 pity      (1000) pity      (1000)   763755 2022-02-25 03:37:01.000000 nyoibo-0.4.1/nyoibo/fields.c
-drwxr-xr-x   0 pity      (1000) pity      (1000)        0 2022-03-02 02:12:18.298881 nyoibo-0.4.1/nyoibo.egg-info/
--rw-r--r--   0 pity      (1000) pity      (1000)     5707 2022-03-02 02:12:18.000000 nyoibo-0.4.1/nyoibo.egg-info/PKG-INFO
--rw-r--r--   0 pity      (1000) pity      (1000)      399 2022-03-02 02:12:18.000000 nyoibo-0.4.1/nyoibo.egg-info/SOURCES.txt
--rw-r--r--   0 pity      (1000) pity      (1000)        1 2022-03-02 02:12:18.000000 nyoibo-0.4.1/nyoibo.egg-info/dependency_links.txt
--rw-r--r--   0 pity      (1000) pity      (1000)       13 2022-03-02 02:12:18.000000 nyoibo-0.4.1/nyoibo.egg-info/top_level.txt
--rw-r--r--   0 pity      (1000) pity      (1000)       38 2022-03-02 02:12:18.302881 nyoibo-0.4.1/setup.cfg
--rw-r--r--   0 pity      (1000) pity      (1000)     2019 2022-02-22 03:56:18.000000 nyoibo-0.4.1/setup.py
-drwxr-xr-x   0 pity      (1000) pity      (1000)        0 2022-03-02 02:12:18.298881 nyoibo-0.4.1/tests/
--rw-r--r--   0 pity      (1000) pity      (1000)        0 2020-07-03 01:20:54.000000 nyoibo-0.4.1/tests/__init__.py
--rw-r--r--   0 pity      (1000) pity      (1000)     7026 2022-02-21 00:24:35.000000 nyoibo-0.4.1/tests/test_entity.py
--rw-r--r--   0 pity      (1000) pity      (1000)     1556 2022-02-21 00:26:05.000000 nyoibo-0.4.1/tests/test_extend_entity.py
--rw-r--r--   0 pity      (1000) pity      (1000)      290 2022-01-26 02:48:15.000000 nyoibo-0.4.1/tests/test_field_validations.py
--rw-r--r--   0 pity      (1000) pity      (1000)     7639 2022-02-23 02:03:12.000000 nyoibo-0.4.1/tests/test_fields.py
+drwxr-xr-x   0 pity      (1000) pity      (1000)        0 2023-05-16 02:09:42.326228 nyoibo-0.5.0/
+-rw-r--r--   0 pity      (1000) pity      (1000)     7652 2021-02-09 03:18:30.000000 nyoibo-0.5.0/LICENSE
+-rw-r--r--   0 pity      (1000) pity      (1000)     4469 2023-05-16 02:09:42.326228 nyoibo-0.5.0/PKG-INFO
+-rw-r--r--   0 pity      (1000) pity      (1000)     3615 2023-05-16 01:48:14.000000 nyoibo-0.5.0/README.rst
+drwxr-xr-x   0 pity      (1000) pity      (1000)        0 2023-05-16 02:09:42.322229 nyoibo-0.5.0/nyoibo/
+-rw-r--r--   0 pity      (1000) pity      (1000)       67 2023-05-16 02:03:02.000000 nyoibo-0.5.0/nyoibo/__init__.py
+drwxr-xr-x   0 pity      (1000) pity      (1000)        0 2023-05-16 02:09:42.326228 nyoibo-0.5.0/nyoibo/entities/
+-rw-r--r--   0 pity      (1000) pity      (1000)       41 2020-07-03 03:22:00.000000 nyoibo-0.5.0/nyoibo/entities/__init__.py
+-rw-r--r--   0 pity      (1000) pity      (1000)   223043 2023-05-16 01:07:10.000000 nyoibo-0.5.0/nyoibo/entities/entity.c
+-rw-r--r--   0 pity      (1000) pity      (1000)     1752 2022-02-21 00:21:17.000000 nyoibo-0.5.0/nyoibo/entities/meta_entity.py
+-rw-r--r--   0 pity      (1000) pity      (1000)      344 2022-02-21 02:23:48.000000 nyoibo-0.5.0/nyoibo/exceptions.py
+-rw-r--r--   0 pity      (1000) pity      (1000)   777394 2023-05-16 01:07:11.000000 nyoibo-0.5.0/nyoibo/fields.c
+drwxr-xr-x   0 pity      (1000) pity      (1000)        0 2023-05-16 02:09:42.326228 nyoibo-0.5.0/nyoibo.egg-info/
+-rw-r--r--   0 pity      (1000) pity      (1000)     4469 2023-05-16 02:09:42.000000 nyoibo-0.5.0/nyoibo.egg-info/PKG-INFO
+-rw-r--r--   0 pity      (1000) pity      (1000)      407 2023-05-16 02:09:42.000000 nyoibo-0.5.0/nyoibo.egg-info/SOURCES.txt
+-rw-r--r--   0 pity      (1000) pity      (1000)        1 2023-05-16 02:09:42.000000 nyoibo-0.5.0/nyoibo.egg-info/dependency_links.txt
+-rw-r--r--   0 pity      (1000) pity      (1000)       13 2023-05-16 02:09:42.000000 nyoibo-0.5.0/nyoibo.egg-info/top_level.txt
+-rw-r--r--   0 pity      (1000) pity      (1000)       38 2023-05-16 02:09:42.326228 nyoibo-0.5.0/setup.cfg
+-rw-r--r--   0 pity      (1000) pity      (1000)     1984 2023-05-16 01:53:28.000000 nyoibo-0.5.0/setup.py
+drwxr-xr-x   0 pity      (1000) pity      (1000)        0 2023-05-16 02:09:42.326228 nyoibo-0.5.0/tests/
+-rw-r--r--   0 pity      (1000) pity      (1000)        0 2020-07-03 01:20:54.000000 nyoibo-0.5.0/tests/__init__.py
+-rw-r--r--   0 pity      (1000) pity      (1000)     7026 2022-02-21 00:24:35.000000 nyoibo-0.5.0/tests/test_entity.py
+-rw-r--r--   0 pity      (1000) pity      (1000)     1556 2022-02-21 00:26:05.000000 nyoibo-0.5.0/tests/test_extend_entity.py
+-rw-r--r--   0 pity      (1000) pity      (1000)      290 2022-01-26 02:48:15.000000 nyoibo-0.5.0/tests/test_field_validations.py
+-rw-r--r--   0 pity      (1000) pity      (1000)     7639 2022-02-23 02:03:12.000000 nyoibo-0.5.0/tests/test_fields.py
```

### Comparing `nyoibo-0.4.1/PKG-INFO` & `nyoibo-0.5.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,172 +1,170 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: nyoibo
-Version: 0.4.1
+Version: 0.5.0
 Summary: Implement attributes accessors in an easy way
 Home-page: https://github.com/pity7736/nyoibo
 Author: Julián Cortés
-Author-email: pity7736@gmail.com
-License: UNKNOWN
-Description: Nyoibo
-        ======
-        
-        .. image:: https://readthedocs.org/projects/nyoibo/badge/?version=latest
-            :target: https://nyoibo.readthedocs.io/en/latest/?badge=latest
-            :alt: Documentation Status
-        
-        .. image:: https://circleci.com/gh/pity7736/nyoibo.svg?style=shield
-            :target: https://circleci.com/gh/pity7736/nyoibo
-        
-        Nyoibo is an easy way to avoid repetitive code with "private" attributes in
-        Python.
-        
-        `See full documentation <https://nyoibo.readthedocs.io/en/latest/>`_
-        
-        
-        Installation
-        ------------
-        
-        You can install nyoibo with pip. Nyoibo requires python 3.7 or higer.
-        
-        ``pip install nyoibo``
-        
-        
-        What does "nyoibo" mean?
-        ------------------------
-        
-        Nyoibo is a mystical staff given to Son Goku by his grandfather Son Gohan.
-        
-        .. image:: ./nyoibo.png
-           :width: 300px
-           :height: 300px
-           :alt: nyoibo
-        
-        
-        Usage
-        -----
-        
-        Instead of doing this:
-        
-        .. code-block:: python
-        
-            class Example:
-        
-                def __init__(self, value=None, other_value=None, default='hello')
-                    self._value = value
-                    self._other_value = other_value
-                    self._default = default
-        
-                def get_value(self):
-                    return self._value
-        
-                value = property(get_value)
-        
-                def get_other_value(self):
-                    return self._other_value
-        
-                def set_other_value(self, value):
-                    self._other_value = value
-        
-                other_value = property(get_other_value, set_other_value)
-        
-                def do_something(self):
-                    return f'{self._default} world'
-        
-        
-        You can do this:
-        
-        .. code-block:: python
-        
-            from nyoibo import Entity, fields
-        
-        
-            class Example(Entity):
-                _value = fields.StrField()
-                _other_value = fields.IntField(mutable=True)
-                _default = fields.StrField(private=True, default_value='hello')
-        
-                def do_something(self):
-                    return f'{self._default} world'
-        
-        In both cases you could use this code like this:
-        
-        .. code-block:: python
-        
-            example = Example(value='some value', other_value=10)
-        
-            assert example.value == 'some value'
-            assert example.get_value() == 'some value'
-            assert example.get_other_value() == 10
-            example.other_value = 15
-            assert example.get_other_value() == 15
-            assert example.do_something() == 'hello world'
-        
-        
-        Why not use dataclass decorator?
-        --------------------------------
-        
-        ``@dataclass`` decorator helps to avoid to write the ``__init__`` method but if you
-        want to use this approach (information hiding and encapsulation), you need to
-        write getters and setters anyway. Furthermore, with ``nyoibo`` you get extra
-        features like casting to right value (due to static typing), validations, override ``__init__`` method and so on.
-        
-        Above example with ``dataclass`` decorator:
-        
-        .. code-block:: python
-        
-            from dataclasses import dataclass
-        
-        
-            @dataclass
-            class Example:
-                _value: str
-                _other_value: int
-                _default: str = 'hello'
-        
-                def get_value(self):
-                    return self._value
-        
-                value = property(get_value)
-        
-                def get_other_value(self):
-                    return self._other_value
-        
-                def set_other_value(self, value):
-                    self._other_value = value
-        
-                other_value = property(get_other_value, set_other_value)
-        
-                def do_something(self):
-                    return f'{self._default} world'
-        
-        Even this code doesn't work because ``__init__`` method has ``_value``,
-        ``_other_value`` and ``_default`` arguments. Therefore the instantiation will be:
-        
-        .. code-block:: python
-        
-            example = Example(_value='some value', _other_value=10)
-        
-        
-        
-        License
-        -------
-        
-        Distributed under the terms of the LGPLv3 license.
-        
-        See `license <https://github.com/pity7736/nyoibo/blob/master/LICENSE>`_.
-        
+Author-email: julian.cortes77@protonmail.com
 Keywords: accessors private
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Requires-Python: >=3.9
+License-File: LICENSE
+
+Nyoibo
+======
+
+.. image:: https://readthedocs.org/projects/nyoibo/badge/?version=latest
+    :target: https://nyoibo.readthedocs.io/en/latest/?badge=latest
+    :alt: Documentation Status
+
+.. image:: https://circleci.com/gh/pity7736/nyoibo.svg?style=shield
+    :target: https://circleci.com/gh/pity7736/nyoibo
+
+Nyoibo is an easy way to avoid repetitive code with "private" attributes in
+Python.
+
+`See full documentation <https://nyoibo.readthedocs.io/en/latest/>`_
+
+
+Installation
+------------
+
+You can install nyoibo with pip. Nyoibo requires python 3.9 or higher.
+
+``pip install nyoibo``
+
+
+What does "nyoibo" mean?
+------------------------
+
+Nyoibo is a mystical staff given to Son Goku by his grandfather Son Gohan.
+
+.. image:: ./nyoibo.png
+   :width: 300px
+   :height: 300px
+   :alt: nyoibo
+
+
+Usage
+-----
+
+Instead of doing this:
+
+.. code-block:: python
+
+    class Example:
+
+        def __init__(self, value=None, other_value=None, default='hello')
+            self._value = value
+            self._other_value = other_value
+            self._default = default
+
+        def get_value(self):
+            return self._value
+
+        value = property(get_value)
+
+        def get_other_value(self):
+            return self._other_value
+
+        def set_other_value(self, value):
+            self._other_value = value
+
+        other_value = property(get_other_value, set_other_value)
+
+        def do_something(self):
+            return f'{self._default} world'
+
+
+You can do this:
+
+.. code-block:: python
+
+    from nyoibo import Entity, fields
+
+
+    class Example(Entity):
+        _value = fields.StrField()
+        _other_value = fields.IntField(mutable=True)
+        _default = fields.StrField(private=True, default_value='hello')
+
+        def do_something(self):
+            return f'{self._default} world'
+
+In both cases you could use this code like this:
+
+.. code-block:: python
+
+    example = Example(value='some value', other_value=10)
+
+    assert example.value == 'some value'
+    assert example.get_value() == 'some value'
+    assert example.get_other_value() == 10
+    example.other_value = 15
+    assert example.get_other_value() == 15
+    assert example.do_something() == 'hello world'
+
+
+Why not use dataclass decorator?
+--------------------------------
+
+``@dataclass`` decorator helps to avoid to write the ``__init__`` method but if you
+want to use this approach (information hiding and encapsulation), you need to
+write getters and setters anyway. Furthermore, with ``nyoibo`` you get extra
+features like casting to right value (due to static typing), validations, override ``__init__`` method and so on.
+
+Above example with ``dataclass`` decorator:
+
+.. code-block:: python
+
+    from dataclasses import dataclass
+
+
+    @dataclass
+    class Example:
+        _value: str
+        _other_value: int
+        _default: str = 'hello'
+
+        def get_value(self):
+            return self._value
+
+        value = property(get_value)
+
+        def get_other_value(self):
+            return self._other_value
+
+        def set_other_value(self, value):
+            self._other_value = value
+
+        other_value = property(get_other_value, set_other_value)
+
+        def do_something(self):
+            return f'{self._default} world'
+
+Even this code doesn't work because ``__init__`` method has ``_value``,
+``_other_value`` and ``_default`` arguments. Therefore the instantiation will be:
+
+.. code-block:: python
+
+    example = Example(_value='some value', _other_value=10)
+
+
+
+License
+-------
+
+Distributed under the terms of the LGPLv3 license.
+
+See `license <https://github.com/pity7736/nyoibo/blob/master/LICENSE>`_.
```

### Comparing `nyoibo-0.4.1/README.rst` & `nyoibo-0.5.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 `See full documentation <https://nyoibo.readthedocs.io/en/latest/>`_
 
 
 Installation
 ------------
 
-You can install nyoibo with pip. Nyoibo requires python 3.7 or higer.
+You can install nyoibo with pip. Nyoibo requires python 3.9 or higher.
 
 ``pip install nyoibo``
 
 
 What does "nyoibo" mean?
 ------------------------
```

### Comparing `nyoibo-0.4.1/nyoibo/entities/entity.c` & `nyoibo-0.5.0/nyoibo/entities/entity.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.26 */
+/* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "name": "nyoibo.entities.entity",
         "sources": [
             "nyoibo/entities/entity.pyx"
@@ -17,16 +17,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_26"
-#define CYTHON_HEX_VERSION 0x001D1AF0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -57,14 +57,15 @@
 #ifndef Py_HUGE_VAL
   #define Py_HUGE_VAL HUGE_VAL
 #endif
 #ifdef PYPY_VERSION
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
   #define CYTHON_USE_TYPE_SLOTS 0
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #if PY_VERSION_HEX < 0x03050000
     #undef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 0
@@ -93,18 +94,22 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #undef CYTHON_USE_ASYNC_SLOTS
   #define CYTHON_USE_ASYNC_SLOTS 0
@@ -134,18 +139,67 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
+#elif defined(PY_NOGIL)
+  #define CYTHON_COMPILING_IN_PYPY 0
+  #define CYTHON_COMPILING_IN_PYSTON 0
+  #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 1
+  #ifndef CYTHON_USE_TYPE_SLOTS
+    #define CYTHON_USE_TYPE_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYTYPE_LOOKUP
+  #define CYTHON_USE_PYTYPE_LOOKUP 0
+  #ifndef CYTHON_USE_ASYNC_SLOTS
+    #define CYTHON_USE_ASYNC_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYLIST_INTERNALS
+  #define CYTHON_USE_PYLIST_INTERNALS 0
+  #ifndef CYTHON_USE_UNICODE_INTERNALS
+    #define CYTHON_USE_UNICODE_INTERNALS 1
+  #endif
+  #undef CYTHON_USE_UNICODE_WRITER
+  #define CYTHON_USE_UNICODE_WRITER 0
+  #undef CYTHON_USE_PYLONG_INTERNALS
+  #define CYTHON_USE_PYLONG_INTERNALS 0
+  #ifndef CYTHON_AVOID_BORROWED_REFS
+    #define CYTHON_AVOID_BORROWED_REFS 0
+  #endif
+  #ifndef CYTHON_ASSUME_SAFE_MACROS
+    #define CYTHON_ASSUME_SAFE_MACROS 1
+  #endif
+  #ifndef CYTHON_UNPACK_METHODS
+    #define CYTHON_UNPACK_METHODS 1
+  #endif
+  #undef CYTHON_FAST_THREAD_STATE
+  #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_PYCALL
+  #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
+  #ifndef CYTHON_USE_TP_FINALIZE
+    #define CYTHON_USE_TP_FINALIZE 1
+  #endif
+  #undef CYTHON_USE_DICT_VERSIONS
+  #define CYTHON_USE_DICT_VERSIONS 0
+  #undef CYTHON_USE_EXC_INFO_STACK
+  #define CYTHON_USE_EXC_INFO_STACK 0
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYTYPE_LOOKUP
     #define CYTHON_USE_PYTYPE_LOOKUP 0
   #elif !defined(CYTHON_USE_PYTYPE_LOOKUP)
@@ -157,15 +211,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -180,32 +234,41 @@
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
-  #ifndef CYTHON_FAST_THREAD_STATE
+  #if PY_VERSION_HEX >= 0x030B00A4
+    #undef CYTHON_FAST_THREAD_STATE
+    #define CYTHON_FAST_THREAD_STATE 0
+  #elif !defined(CYTHON_FAST_THREAD_STATE)
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
   #ifndef CYTHON_FAST_PYCALL
-    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030B00A1)
+    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030A0000)
   #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
-  #ifndef CYTHON_USE_EXC_INFO_STACK
+  #if PY_VERSION_HEX >= 0x030B00A4
+    #undef CYTHON_USE_EXC_INFO_STACK
+    #define CYTHON_USE_EXC_INFO_STACK 0
+  #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if CYTHON_USE_PYLONG_INTERNALS
   #if PY_MAJOR_VERSION < 3
     #include "longintrepr.h"
@@ -497,35 +560,35 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
   #else
-  #define __Pyx_PyUnicode_READY(op)       (0)
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
-  #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
@@ -649,16 +712,18 @@
     typedef struct {
         unaryfunc am_await;
         unaryfunc am_aiter;
         unaryfunc am_anext;
     } __Pyx_PyAsyncMethodsStruct;
 #endif
 
-#if defined(WIN32) || defined(MS_WINDOWS)
-  #define _USE_MATH_DEFINES
+#if defined(_WIN32) || defined(WIN32) || defined(MS_WINDOWS)
+  #if !defined(_USE_MATH_DEFINES)
+    #define _USE_MATH_DEFINES
+  #endif
 #endif
 #include <math.h>
 #ifdef NAN
 #define __PYX_NAN() ((float) NAN)
 #else
 static CYTHON_INLINE float __PYX_NAN() {
   float value;
@@ -1110,14 +1175,20 @@
     (sizeof(char [1 - 2*!(cond)]) - 1)
 #ifndef Py_MEMBER_SIZE
 #define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
 #endif
 #if CYTHON_FAST_PYCALL
   static size_t __pyx_pyframe_localsplus_offset = 0;
   #include "frameobject.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
   #define __Pxy_PyFrame_Initialize_Offsets()\
     ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
      (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
   #define __Pyx_PyFrame_GetLocalsplus(frame)\
     (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
 #endif // CYTHON_FAST_PYCALL
 #endif
@@ -1233,20 +1304,28 @@
 
 /* GetAttr.proto */
 static CYTHON_INLINE PyObject *__Pyx_GetAttr(PyObject *, PyObject *);
 
 /* TypeImport.proto */
 #ifndef __PYX_HAVE_RT_ImportType_proto
 #define __PYX_HAVE_RT_ImportType_proto
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#endif
 enum __Pyx_ImportType_CheckSize {
    __Pyx_ImportType_CheckSize_Error = 0,
    __Pyx_ImportType_CheckSize_Warn = 1,
    __Pyx_ImportType_CheckSize_Ignore = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
 #endif
 
 /* GetVTable.proto */
 static void* __Pyx_GetVtable(PyObject *dict);
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
@@ -1281,26 +1360,26 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
@@ -1686,15 +1765,15 @@
   __pyx_t_6 = 0;
   while (1) {
     __pyx_t_7 = __Pyx_dict_iter_next(__pyx_t_1, __pyx_t_3, &__pyx_t_2, &__pyx_t_6, &__pyx_t_5, NULL, __pyx_t_4);
     if (unlikely(__pyx_t_7 == 0)) break;
     if (unlikely(__pyx_t_7 == -1)) __PYX_ERR(0, 24, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_GOTREF(__pyx_t_5);
-    if (!(likely(PyUnicode_CheckExact(__pyx_t_6))||((__pyx_t_6) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_6)->tp_name), 0))) __PYX_ERR(0, 24, __pyx_L1_error)
+    if (!(likely(PyUnicode_CheckExact(__pyx_t_6))||((__pyx_t_6) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_6)->tp_name), 0))) __PYX_ERR(0, 24, __pyx_L1_error)
     if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_6nyoibo_6fields_Field))))) __PYX_ERR(0, 24, __pyx_L1_error)
     __Pyx_XDECREF_SET(__pyx_v_key, ((PyObject*)__pyx_t_6));
     __pyx_t_6 = 0;
     __Pyx_XDECREF_SET(__pyx_v_field, ((struct __pyx_obj_6nyoibo_6fields_Field *)__pyx_t_5));
     __pyx_t_5 = 0;
 
     /* "nyoibo/entities/entity.pyx":25
@@ -2209,15 +2288,15 @@
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
   __pyx_umethod_PyDict_Type_get.type = (PyObject*)&PyDict_Type;
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_modinit_global_init_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_variable_export_code(void); /*proto*/
@@ -2265,24 +2344,28 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule("nyoibo.fields"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_6nyoibo_6fields_Field = __Pyx_ImportType(__pyx_t_1, "nyoibo.fields", "Field", sizeof(struct __pyx_obj_6nyoibo_6fields_Field), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_6nyoibo_6fields_Field = __Pyx_ImportType(__pyx_t_1, "nyoibo.fields", "Field", sizeof(struct __pyx_obj_6nyoibo_6fields_Field), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_6nyoibo_6fields_Field),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_6nyoibo_6fields_Field) __PYX_ERR(1, 2, __pyx_L1_error)
   __pyx_vtabptr_6nyoibo_6fields_Field = (struct __pyx_vtabstruct_6nyoibo_6fields_Field*)__Pyx_GetVtable(__pyx_ptype_6nyoibo_6fields_Field->tp_dict); if (unlikely(!__pyx_vtabptr_6nyoibo_6fields_Field)) __PYX_ERR(1, 2, __pyx_L1_error)
-  __pyx_ptype_6nyoibo_6fields_StrField = __Pyx_ImportType(__pyx_t_1, "nyoibo.fields", "StrField", sizeof(struct __pyx_obj_6nyoibo_6fields_StrField), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_6nyoibo_6fields_StrField = __Pyx_ImportType(__pyx_t_1, "nyoibo.fields", "StrField", sizeof(struct __pyx_obj_6nyoibo_6fields_StrField), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_6nyoibo_6fields_StrField),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_6nyoibo_6fields_StrField) __PYX_ERR(1, 12, __pyx_L1_error)
   __pyx_vtabptr_6nyoibo_6fields_StrField = (struct __pyx_vtabstruct_6nyoibo_6fields_StrField*)__Pyx_GetVtable(__pyx_ptype_6nyoibo_6fields_StrField->tp_dict); if (unlikely(!__pyx_vtabptr_6nyoibo_6fields_StrField)) __PYX_ERR(1, 12, __pyx_L1_error)
-  __pyx_ptype_6nyoibo_6fields_IntField = __Pyx_ImportType(__pyx_t_1, "nyoibo.fields", "IntField", sizeof(struct __pyx_obj_6nyoibo_6fields_IntField), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_6nyoibo_6fields_IntField = __Pyx_ImportType(__pyx_t_1, "nyoibo.fields", "IntField", sizeof(struct __pyx_obj_6nyoibo_6fields_IntField), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_6nyoibo_6fields_IntField),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_6nyoibo_6fields_IntField) __PYX_ERR(1, 16, __pyx_L1_error)
   __pyx_vtabptr_6nyoibo_6fields_IntField = (struct __pyx_vtabstruct_6nyoibo_6fields_IntField*)__Pyx_GetVtable(__pyx_ptype_6nyoibo_6fields_IntField->tp_dict); if (unlikely(!__pyx_vtabptr_6nyoibo_6fields_IntField)) __PYX_ERR(1, 16, __pyx_L1_error)
-  __pyx_ptype_6nyoibo_6fields_LinkField = __Pyx_ImportType(__pyx_t_1, "nyoibo.fields", "LinkField", sizeof(struct __pyx_obj_6nyoibo_6fields_LinkField), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_6nyoibo_6fields_LinkField = __Pyx_ImportType(__pyx_t_1, "nyoibo.fields", "LinkField", sizeof(struct __pyx_obj_6nyoibo_6fields_LinkField), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_6nyoibo_6fields_LinkField),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_6nyoibo_6fields_LinkField) __PYX_ERR(1, 21, __pyx_L1_error)
   __pyx_vtabptr_6nyoibo_6fields_LinkField = (struct __pyx_vtabstruct_6nyoibo_6fields_LinkField*)__Pyx_GetVtable(__pyx_ptype_6nyoibo_6fields_LinkField->tp_dict); if (unlikely(!__pyx_vtabptr_6nyoibo_6fields_LinkField)) __PYX_ERR(1, 21, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
@@ -2471,15 +2554,15 @@
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_nyoibo__entities__entity) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -2977,15 +3060,15 @@
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
 #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(func)) {
         return __Pyx_PyFunction_FastCall(func, NULL, 0);
     }
 #endif
-#ifdef __Pyx_CyFunction_USED
+#if defined(__Pyx_CyFunction_USED) && defined(NDEBUG)
     if (likely(PyCFunction_Check(func) || __Pyx_CyFunction_Check(func)))
 #else
     if (likely(PyCFunction_Check(func)))
 #endif
     {
         if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
             return __Pyx_PyObject_CallMethO(func, NULL);
@@ -3199,18 +3282,16 @@
 
 /* UnpackItemEndCheck */
 static int __Pyx_IternextUnpackEndCheck(PyObject *retval, Py_ssize_t expected) {
     if (unlikely(retval)) {
         Py_DECREF(retval);
         __Pyx_RaiseTooManyValuesError(expected);
         return -1;
-    } else {
-        return __Pyx_IterFinish();
     }
-    return 0;
+    return __Pyx_IterFinish();
 }
 
 /* RaiseNoneIterError */
 static CYTHON_INLINE void __Pyx_RaiseNoneNotIterableError(void) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
 }
 
@@ -3427,19 +3508,19 @@
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_CallUnboundCMethod1(__Pyx_CachedCFunction* cfunc, PyObject* self, PyObject* arg) {
     if (likely(cfunc->func)) {
         int flag = cfunc->flag;
         if (flag == METH_O) {
             return (*(cfunc->func))(self, arg);
         } else if (PY_VERSION_HEX >= 0x030600B1 && flag == METH_FASTCALL) {
-            if (PY_VERSION_HEX >= 0x030700A0) {
+            #if PY_VERSION_HEX >= 0x030700A0
                 return (*(__Pyx_PyCFunctionFast)(void*)(PyCFunction)cfunc->func)(self, &arg, 1);
-            } else {
+            #else
                 return (*(__Pyx_PyCFunctionFastWithKeywords)(void*)(PyCFunction)cfunc->func)(self, &arg, 1, NULL);
-            }
+            #endif
         } else if (PY_VERSION_HEX >= 0x030700A0 && flag == (METH_FASTCALL | METH_KEYWORDS)) {
             return (*(__Pyx_PyCFunctionFastWithKeywords)(void*)(PyCFunction)cfunc->func)(self, &arg, 1, NULL);
         }
     }
     return __Pyx__CallUnboundCMethod1(cfunc, self, arg);
 }
 #endif
@@ -3581,44 +3662,62 @@
     return PyObject_GetAttr(o, n);
 }
 
 /* TypeImport */
 #ifndef __PYX_HAVE_RT_ImportType
 #define __PYX_HAVE_RT_ImportType
 static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
     if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
@@ -4348,14 +4447,22 @@
         argc = PyTuple_GET_SIZE(args);
         new_args = PyTuple_GetSlice(args, 1, argc);
         if (unlikely(!new_args))
             return NULL;
         self = PyTuple_GetItem(args, 0);
         if (unlikely(!self)) {
             Py_DECREF(new_args);
+#if PY_MAJOR_VERSION > 2
+            PyErr_Format(PyExc_TypeError,
+                         "unbound method %.200S() needs an argument",
+                         cyfunc->func_qualname);
+#else
+            PyErr_SetString(PyExc_TypeError,
+                            "unbound method needs an argument");
+#endif
             return NULL;
         }
         result = __Pyx_CyFunction_CallMethod(func, self, new_args, kw);
         Py_DECREF(new_args);
     } else {
         result = __Pyx_CyFunction_Call(func, args, kw);
     }
@@ -4416,21 +4523,21 @@
     0,
     0,
     0,
     0,
 #if PY_VERSION_HEX >= 0x030400a1
     0,
 #endif
-#if PY_VERSION_HEX >= 0x030800b1
+#if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PYPY_VERSION_NUM+0 >= 0x06000000
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
     0,
 #endif
 };
 static int __pyx_CyFunction_init(void) {
     __pyx_CyFunctionType = __Pyx_FetchCommonType(&__pyx_CyFunctionType_type);
     if (unlikely(__pyx_CyFunctionType == NULL)) {
         return -1;
@@ -4604,15 +4711,15 @@
     tstate->curexc_value = 0;
     tstate->curexc_traceback = 0;
 }
 #endif
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
@@ -4728,14 +4835,20 @@
     Py_INCREF(code_object);
 }
 
 /* AddTraceback */
 #include "compile.h"
 #include "frameobject.h"
 #include "traceback.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
 static PyCodeObject* __Pyx_CreateCodeObjectForTraceback(
             const char *funcname, int c_line,
             int py_line, const char *filename) {
     PyCodeObject *py_code = NULL;
     PyObject *py_funcname = NULL;
     #if PY_MAJOR_VERSION < 3
     PyObject *py_srcfile = NULL;
@@ -4791,22 +4904,32 @@
     return NULL;
 }
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename) {
     PyCodeObject *py_code = 0;
     PyFrameObject *py_frame = 0;
     PyThreadState *tstate = __Pyx_PyThreadState_Current;
+    PyObject *ptype, *pvalue, *ptraceback;
     if (c_line) {
         c_line = __Pyx_CLineForTraceback(tstate, c_line);
     }
     py_code = __pyx_find_code_object(c_line ? -c_line : py_line);
     if (!py_code) {
+        __Pyx_ErrFetchInState(tstate, &ptype, &pvalue, &ptraceback);
         py_code = __Pyx_CreateCodeObjectForTraceback(
             funcname, c_line, py_line, filename);
-        if (!py_code) goto bad;
+        if (!py_code) {
+            /* If the code object creation fails, then we should clear the
+               fetched exception references and propagate the new exception */
+            Py_XDECREF(ptype);
+            Py_XDECREF(pvalue);
+            Py_XDECREF(ptraceback);
+            goto bad;
+        }
+        __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
         __pyx_insert_code_object(c_line ? -c_line : py_line, py_code);
     }
     py_frame = PyFrame_New(
         tstate,            /*PyThreadState *tstate,*/
         py_code,           /*PyCodeObject *code,*/
         __pyx_d,    /*PyObject *globals,*/
         0                  /*PyObject *locals*/
@@ -5369,19 +5492,41 @@
     }
     return (PyErr_GivenExceptionMatches(err, exc_type1) || PyErr_GivenExceptionMatches(err, exc_type2));
 }
 #endif
 
 /* CheckBinaryVersion */
 static int __Pyx_check_binary_version(void) {
-    char ctversion[4], rtversion[4];
-    PyOS_snprintf(ctversion, 4, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
-    PyOS_snprintf(rtversion, 4, "%s", Py_GetVersion());
-    if (ctversion[0] != rtversion[0] || ctversion[2] != rtversion[2]) {
+    char ctversion[5];
+    int same=1, i, found_dot;
+    const char* rt_from_call = Py_GetVersion();
+    PyOS_snprintf(ctversion, 5, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
+    found_dot = 0;
+    for (i = 0; i < 4; i++) {
+        if (!ctversion[i]) {
+            same = (rt_from_call[i] < '0' || rt_from_call[i] > '9');
+            break;
+        }
+        if (rt_from_call[i] != ctversion[i]) {
+            same = 0;
+            break;
+        }
+    }
+    if (!same) {
+        char rtversion[5] = {'\0'};
         char message[200];
+        for (i=0; i<4; ++i) {
+            if (rt_from_call[i] == '.') {
+                if (found_dot) break;
+                found_dot = 1;
+            } else if (rt_from_call[i] < '0' || rt_from_call[i] > '9') {
+                break;
+            }
+            rtversion[i] = rt_from_call[i];
+        }
         PyOS_snprintf(message, sizeof(message),
                       "compiletime version %s of module '%.100s' "
                       "does not match runtime version %s",
                       ctversion, __Pyx_MODULE_NAME, rtversion);
         return PyErr_WarnEx(NULL, message, 1);
     }
     return 0;
```

### Comparing `nyoibo-0.4.1/nyoibo/entities/meta_entity.py` & `nyoibo-0.5.0/nyoibo/entities/meta_entity.py`

 * *Files identical despite different names*

### Comparing `nyoibo-0.4.1/nyoibo/fields.c` & `nyoibo-0.5.0/nyoibo/fields.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.26 */
+/* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "name": "nyoibo.fields",
         "sources": [
             "nyoibo/fields.pyx"
@@ -17,16 +17,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_26"
-#define CYTHON_HEX_VERSION 0x001D1AF0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -57,14 +57,15 @@
 #ifndef Py_HUGE_VAL
   #define Py_HUGE_VAL HUGE_VAL
 #endif
 #ifdef PYPY_VERSION
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
   #define CYTHON_USE_TYPE_SLOTS 0
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #if PY_VERSION_HEX < 0x03050000
     #undef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 0
@@ -93,18 +94,22 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #undef CYTHON_USE_ASYNC_SLOTS
   #define CYTHON_USE_ASYNC_SLOTS 0
@@ -134,18 +139,67 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
+#elif defined(PY_NOGIL)
+  #define CYTHON_COMPILING_IN_PYPY 0
+  #define CYTHON_COMPILING_IN_PYSTON 0
+  #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 1
+  #ifndef CYTHON_USE_TYPE_SLOTS
+    #define CYTHON_USE_TYPE_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYTYPE_LOOKUP
+  #define CYTHON_USE_PYTYPE_LOOKUP 0
+  #ifndef CYTHON_USE_ASYNC_SLOTS
+    #define CYTHON_USE_ASYNC_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYLIST_INTERNALS
+  #define CYTHON_USE_PYLIST_INTERNALS 0
+  #ifndef CYTHON_USE_UNICODE_INTERNALS
+    #define CYTHON_USE_UNICODE_INTERNALS 1
+  #endif
+  #undef CYTHON_USE_UNICODE_WRITER
+  #define CYTHON_USE_UNICODE_WRITER 0
+  #undef CYTHON_USE_PYLONG_INTERNALS
+  #define CYTHON_USE_PYLONG_INTERNALS 0
+  #ifndef CYTHON_AVOID_BORROWED_REFS
+    #define CYTHON_AVOID_BORROWED_REFS 0
+  #endif
+  #ifndef CYTHON_ASSUME_SAFE_MACROS
+    #define CYTHON_ASSUME_SAFE_MACROS 1
+  #endif
+  #ifndef CYTHON_UNPACK_METHODS
+    #define CYTHON_UNPACK_METHODS 1
+  #endif
+  #undef CYTHON_FAST_THREAD_STATE
+  #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_PYCALL
+  #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
+  #ifndef CYTHON_USE_TP_FINALIZE
+    #define CYTHON_USE_TP_FINALIZE 1
+  #endif
+  #undef CYTHON_USE_DICT_VERSIONS
+  #define CYTHON_USE_DICT_VERSIONS 0
+  #undef CYTHON_USE_EXC_INFO_STACK
+  #define CYTHON_USE_EXC_INFO_STACK 0
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYTYPE_LOOKUP
     #define CYTHON_USE_PYTYPE_LOOKUP 0
   #elif !defined(CYTHON_USE_PYTYPE_LOOKUP)
@@ -157,15 +211,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -180,32 +234,41 @@
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
-  #ifndef CYTHON_FAST_THREAD_STATE
+  #if PY_VERSION_HEX >= 0x030B00A4
+    #undef CYTHON_FAST_THREAD_STATE
+    #define CYTHON_FAST_THREAD_STATE 0
+  #elif !defined(CYTHON_FAST_THREAD_STATE)
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
   #ifndef CYTHON_FAST_PYCALL
-    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030B00A1)
+    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030A0000)
   #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
-  #ifndef CYTHON_USE_EXC_INFO_STACK
+  #if PY_VERSION_HEX >= 0x030B00A4
+    #undef CYTHON_USE_EXC_INFO_STACK
+    #define CYTHON_USE_EXC_INFO_STACK 0
+  #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if CYTHON_USE_PYLONG_INTERNALS
   #if PY_MAJOR_VERSION < 3
     #include "longintrepr.h"
@@ -497,35 +560,35 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
   #else
-  #define __Pyx_PyUnicode_READY(op)       (0)
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
-  #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
@@ -649,16 +712,18 @@
     typedef struct {
         unaryfunc am_await;
         unaryfunc am_aiter;
         unaryfunc am_anext;
     } __Pyx_PyAsyncMethodsStruct;
 #endif
 
-#if defined(WIN32) || defined(MS_WINDOWS)
-  #define _USE_MATH_DEFINES
+#if defined(_WIN32) || defined(WIN32) || defined(MS_WINDOWS)
+  #if !defined(_USE_MATH_DEFINES)
+    #define _USE_MATH_DEFINES
+  #endif
 #endif
 #include <math.h>
 #ifdef NAN
 #define __PYX_NAN() ((float) NAN)
 #else
 static CYTHON_INLINE float __PYX_NAN() {
   float value;
@@ -1287,14 +1352,20 @@
     (sizeof(char [1 - 2*!(cond)]) - 1)
 #ifndef Py_MEMBER_SIZE
 #define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
 #endif
 #if CYTHON_FAST_PYCALL
   static size_t __pyx_pyframe_localsplus_offset = 0;
   #include "frameobject.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
   #define __Pxy_PyFrame_Initialize_Offsets()\
     ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
      (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
   #define __Pyx_PyFrame_GetLocalsplus(frame)\
     (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
 #endif // CYTHON_FAST_PYCALL
 #endif
@@ -1315,26 +1386,26 @@
 #endif
 
 /* PyObjectCallOneArg.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg);
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
@@ -1487,14 +1558,20 @@
     Py_DECREF(none);
     return 0;
 #else
     return PyList_SetSlice(L, PY_SSIZE_T_MAX, PY_SSIZE_T_MAX, v);
 #endif
 }
 
+/* PySequenceContains.proto */
+static CYTHON_INLINE int __Pyx_PySequence_ContainsTF(PyObject* item, PyObject* seq, int eq) {
+    int result = PySequence_Contains(seq, item);
+    return unlikely(result < 0) ? result : (result == (eq == Py_EQ));
+}
+
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* ImportFrom.proto */
 static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
 
 /* GetItemInt.proto */
@@ -1814,18 +1891,18 @@
 static const char __pyx_k_is_greater_than_max_value[] = ") is greater than max_value (";
 static const char __pyx_k_pyx_unpickle_DecimalField[] = "__pyx_unpickle_DecimalField";
 static const char __pyx_k_pyx_unpickle_DatetimeField[] = "__pyx_unpickle_DatetimeField";
 static const char __pyx_k_nyoibo_entities_meta_entity[] = "nyoibo.entities.meta_entity";
 static const char __pyx_k_max_value_must_be_an_integer[] = "max_value must be an integer";
 static const char __pyx_k_min_value_must_be_an_integer[] = "min_value must be an integer";
 static const char __pyx_k_to_must_be_an_Entity_subclass[] = "to must be an Entity subclass";
-static const char __pyx_k_Incompatible_checksums_s_vs_0x37[] = "Incompatible checksums (%s vs 0x37df068 = (choices, default_value, mutable, private, required, to))";
-static const char __pyx_k_Incompatible_checksums_s_vs_0x87[] = "Incompatible checksums (%s vs 0x87ffd98 = (choices, default_value, max_length, mutable, private, required))";
-static const char __pyx_k_Incompatible_checksums_s_vs_0xd4[] = "Incompatible checksums (%s vs 0xd43e024 = (choices, default_value, max_value, min_value, mutable, private, required))";
-static const char __pyx_k_Incompatible_checksums_s_vs_0xe4[] = "Incompatible checksums (%s vs 0xe41db34 = (choices, default_value, mutable, private, required))";
+static const char __pyx_k_Incompatible_checksums_0x_x_vs_0[] = "Incompatible checksums (0x%x vs (0xe41db34, 0x22cbad7, 0xa0145de) = (choices, default_value, mutable, private, required))";
+static const char __pyx_k_Incompatible_checksums_0x_x_vs_0_2[] = "Incompatible checksums (0x%x vs (0x87ffd98, 0x223c4c1, 0x5d84c1f) = (choices, default_value, max_length, mutable, private, required))";
+static const char __pyx_k_Incompatible_checksums_0x_x_vs_0_3[] = "Incompatible checksums (0x%x vs (0xd43e024, 0xd116a37, 0xd2e28da) = (choices, default_value, max_value, min_value, mutable, private, required))";
+static const char __pyx_k_Incompatible_checksums_0x_x_vs_0_4[] = "Incompatible checksums (0x%x vs (0x37df068, 0x13e4e4a, 0x17f2992) = (choices, default_value, mutable, private, required, to))";
 static PyObject *__pyx_kp_u_;
 static PyObject *__pyx_n_s_BoolField;
 static PyObject *__pyx_n_s_DateField;
 static PyObject *__pyx_n_s_DatetimeField;
 static PyObject *__pyx_n_s_Decimal;
 static PyObject *__pyx_n_s_DecimalField;
 static PyObject *__pyx_n_s_DictField;
@@ -1833,18 +1910,18 @@
 static PyObject *__pyx_n_s_Field;
 static PyObject *__pyx_n_s_FieldValueError;
 static PyObject *__pyx_kp_s_Field_for_dict_values;
 static PyObject *__pyx_kp_s_Field_for_json_values;
 static PyObject *__pyx_kp_s_Field_for_list_values;
 static PyObject *__pyx_kp_s_Field_for_tuple_values;
 static PyObject *__pyx_n_s_FloatField;
-static PyObject *__pyx_kp_s_Incompatible_checksums_s_vs_0x37;
-static PyObject *__pyx_kp_s_Incompatible_checksums_s_vs_0x87;
-static PyObject *__pyx_kp_s_Incompatible_checksums_s_vs_0xd4;
-static PyObject *__pyx_kp_s_Incompatible_checksums_s_vs_0xe4;
+static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0;
+static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_2;
+static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_3;
+static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_4;
 static PyObject *__pyx_n_s_IntField;
 static PyObject *__pyx_n_s_IntMaxValueError;
 static PyObject *__pyx_n_s_IntMinValueError;
 static PyObject *__pyx_n_s_InvalidOperation;
 static PyObject *__pyx_n_s_JSONField;
 static PyObject *__pyx_n_s_JSONField_parse;
 static PyObject *__pyx_n_s_LinkField;
@@ -1980,40 +2057,52 @@
 static PyObject *__pyx_tp_new_6nyoibo_6fields_IntField(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_6nyoibo_6fields_LinkField(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_6nyoibo_6fields_BoolField(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_6nyoibo_6fields_DateField(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_6nyoibo_6fields_DatetimeField(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_6nyoibo_6fields_FloatField(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_6nyoibo_6fields_DecimalField(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
+static PyObject *__pyx_int_20860490;
+static PyObject *__pyx_int_25110930;
+static PyObject *__pyx_int_35898561;
+static PyObject *__pyx_int_36485847;
 static PyObject *__pyx_int_58585192;
+static PyObject *__pyx_int_98061343;
 static PyObject *__pyx_int_142605720;
+static PyObject *__pyx_int_167855582;
+static PyObject *__pyx_int_219245111;
+static PyObject *__pyx_int_221128922;
 static PyObject *__pyx_int_222552100;
 static PyObject *__pyx_int_239196980;
 static PyObject *__pyx_tuple__2;
 static PyObject *__pyx_tuple__3;
 static PyObject *__pyx_tuple__4;
+static PyObject *__pyx_tuple__5;
 static PyObject *__pyx_tuple__6;
+static PyObject *__pyx_tuple__7;
 static PyObject *__pyx_tuple__8;
 static PyObject *__pyx_tuple__10;
 static PyObject *__pyx_tuple__12;
 static PyObject *__pyx_tuple__14;
 static PyObject *__pyx_tuple__16;
 static PyObject *__pyx_tuple__18;
 static PyObject *__pyx_tuple__20;
 static PyObject *__pyx_tuple__22;
-static PyObject *__pyx_codeobj__5;
-static PyObject *__pyx_codeobj__7;
+static PyObject *__pyx_tuple__24;
+static PyObject *__pyx_tuple__26;
 static PyObject *__pyx_codeobj__9;
 static PyObject *__pyx_codeobj__11;
 static PyObject *__pyx_codeobj__13;
 static PyObject *__pyx_codeobj__15;
 static PyObject *__pyx_codeobj__17;
 static PyObject *__pyx_codeobj__19;
 static PyObject *__pyx_codeobj__21;
 static PyObject *__pyx_codeobj__23;
+static PyObject *__pyx_codeobj__25;
+static PyObject *__pyx_codeobj__27;
 /* Late includes */
 
 /* "nyoibo/fields.pyx":34
  *     _exceptions = (TypeError, ValueError)
  * 
  *     def __init__(self, private=False, mutable=False, default_value=None,             # <<<<<<<<<<<<<<
  *                  choices=None, bint required=False):
@@ -3228,15 +3317,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":17
  *         return __pyx_unpickle_Field, (type(self), 0xe41db34, state)
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle_Field__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
-  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
+  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
   __pyx_t_1 = __pyx_f_6nyoibo_6fields___pyx_unpickle_Field__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_Field, (type(self), 0xe41db34, state)
@@ -3888,15 +3977,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":17
  *         return __pyx_unpickle_StrField, (type(self), 0x87ffd98, state)
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle_StrField__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
-  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
+  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
   __pyx_t_1 = __pyx_f_6nyoibo_6fields___pyx_unpickle_StrField__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_StrField, (type(self), 0x87ffd98, state)
@@ -4938,15 +5027,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":17
  *         return __pyx_unpickle_IntField, (type(self), 0xd43e024, state)
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle_IntField__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
-  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
+  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
   __pyx_t_1 = __pyx_f_6nyoibo_6fields___pyx_unpickle_IntField__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_IntField, (type(self), 0xd43e024, state)
@@ -5363,15 +5452,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":17
  *         return __pyx_unpickle_BoolField, (type(self), 0xe41db34, state)
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle_BoolField__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
-  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
+  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
   __pyx_t_1 = __pyx_f_6nyoibo_6fields___pyx_unpickle_BoolField__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_BoolField, (type(self), 0xe41db34, state)
@@ -5804,15 +5893,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":17
  *         return __pyx_unpickle_DateField, (type(self), 0xe41db34, state)
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle_DateField__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
-  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
+  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
   __pyx_t_1 = __pyx_f_6nyoibo_6fields___pyx_unpickle_DateField__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_DateField, (type(self), 0xe41db34, state)
@@ -6245,15 +6334,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":17
  *         return __pyx_unpickle_DatetimeField, (type(self), 0xe41db34, state)
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle_DatetimeField__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
-  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
+  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
   __pyx_t_1 = __pyx_f_6nyoibo_6fields___pyx_unpickle_DatetimeField__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_DatetimeField, (type(self), 0xe41db34, state)
@@ -6577,15 +6666,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":17
  *         return __pyx_unpickle_FloatField, (type(self), 0xe41db34, state)
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle_FloatField__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
-  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
+  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
   __pyx_t_1 = __pyx_f_6nyoibo_6fields___pyx_unpickle_FloatField__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_FloatField, (type(self), 0xe41db34, state)
@@ -6909,15 +6998,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":17
  *         return __pyx_unpickle_DecimalField, (type(self), 0xe41db34, state)
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle_DecimalField__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
-  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
+  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
   __pyx_t_1 = __pyx_f_6nyoibo_6fields___pyx_unpickle_DecimalField__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_DecimalField, (type(self), 0xe41db34, state)
@@ -7826,15 +7915,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":17
  *         return __pyx_unpickle_LinkField, (type(self), 0x37df068, state)
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle_LinkField__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
-  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
+  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
   __pyx_t_1 = __pyx_f_6nyoibo_6fields___pyx_unpickle_LinkField__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_LinkField, (type(self), 0x37df068, state)
@@ -8213,151 +8302,155 @@
 }
 
 static PyObject *__pyx_pf_6nyoibo_6fields___pyx_unpickle_Field(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
+  PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_Field", 0);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xe41db34:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0xe41db34, 0x22cbad7, 0xa0145de):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe41db34 = (choices, default_value, mutable, private, required))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe41db34, 0x22cbad7, 0xa0145de) = (choices, default_value, mutable, private, required))" % __pyx_checksum)
  */
-  __pyx_t_1 = ((__pyx_v___pyx_checksum != 0xe41db34) != 0);
-  if (__pyx_t_1) {
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__3, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xe41db34:
+ *     if __pyx_checksum not in (0xe41db34, 0x22cbad7, 0xa0145de):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe41db34 = (choices, default_value, mutable, private, required))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe41db34, 0x22cbad7, 0xa0145de) = (choices, default_value, mutable, private, required))" % __pyx_checksum)
  *     __pyx_result = Field.__new__(__pyx_type)
  */
-    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
-    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PickleError);
-    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_2, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_INCREF(__pyx_t_2);
-    __pyx_v___pyx_PickleError = __pyx_t_2;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
+    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_v___pyx_PickleError = __pyx_t_1;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":6
- *     if __pyx_checksum != 0xe41db34:
+ *     if __pyx_checksum not in (0xe41db34, 0x22cbad7, 0xa0145de):
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe41db34 = (choices, default_value, mutable, private, required))" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe41db34, 0x22cbad7, 0xa0145de) = (choices, default_value, mutable, private, required))" % __pyx_checksum)             # <<<<<<<<<<<<<<
  *     __pyx_result = Field.__new__(__pyx_type)
  *     if __pyx_state is not None:
  */
-    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_s_vs_0xe4, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_INCREF(__pyx_v___pyx_PickleError);
-    __pyx_t_2 = __pyx_v___pyx_PickleError; __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_5);
+    __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 6, __pyx_L1_error)
 
     /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xe41db34:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0xe41db34, 0x22cbad7, 0xa0145de):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe41db34 = (choices, default_value, mutable, private, required))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe41db34, 0x22cbad7, 0xa0145de) = (choices, default_value, mutable, private, required))" % __pyx_checksum)
  */
   }
 
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe41db34 = (choices, default_value, mutable, private, required))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe41db34, 0x22cbad7, 0xa0145de) = (choices, default_value, mutable, private, required))" % __pyx_checksum)
  *     __pyx_result = Field.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_Field__set_state(<Field> __pyx_result, __pyx_state)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_6nyoibo_6fields_Field), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_6nyoibo_6fields_Field), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v___pyx_type);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v___pyx_result = __pyx_t_3;
-  __pyx_t_3 = 0;
+  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result = __pyx_t_4;
+  __pyx_t_4 = 0;
 
   /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe41db34 = (choices, default_value, mutable, private, required))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe41db34, 0x22cbad7, 0xa0145de) = (choices, default_value, mutable, private, required))" % __pyx_checksum)
  *     __pyx_result = Field.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_Field__set_state(<Field> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
-  __pyx_t_1 = (__pyx_v___pyx_state != Py_None);
-  __pyx_t_6 = (__pyx_t_1 != 0);
-  if (__pyx_t_6) {
+  __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_2 = (__pyx_t_3 != 0);
+  if (__pyx_t_2) {
 
     /* "(tree fragment)":9
  *     __pyx_result = Field.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_Field__set_state(<Field> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_Field__set_state(Field __pyx_result, tuple __pyx_state):
  */
-    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
-    __pyx_t_3 = __pyx_f_6nyoibo_6fields___pyx_unpickle_Field__set_state(((struct __pyx_obj_6nyoibo_6fields_Field *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 9, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
+    __pyx_t_4 = __pyx_f_6nyoibo_6fields___pyx_unpickle_Field__set_state(((struct __pyx_obj_6nyoibo_6fields_Field *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe41db34 = (choices, default_value, mutable, private, required))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe41db34, 0x22cbad7, 0xa0145de) = (choices, default_value, mutable, private, required))" % __pyx_checksum)
  *     __pyx_result = Field.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_Field__set_state(<Field> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   }
 
@@ -8377,18 +8470,18 @@
  * def __pyx_unpickle_Field(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("nyoibo.fields.__pyx_unpickle_Field", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -8652,151 +8745,155 @@
 }
 
 static PyObject *__pyx_pf_6nyoibo_6fields_2__pyx_unpickle_StrField(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
+  PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_StrField", 0);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x87ffd98:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0x87ffd98, 0x223c4c1, 0x5d84c1f):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x87ffd98 = (choices, default_value, max_length, mutable, private, required))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x87ffd98, 0x223c4c1, 0x5d84c1f) = (choices, default_value, max_length, mutable, private, required))" % __pyx_checksum)
  */
-  __pyx_t_1 = ((__pyx_v___pyx_checksum != 0x87ffd98) != 0);
-  if (__pyx_t_1) {
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__4, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x87ffd98:
+ *     if __pyx_checksum not in (0x87ffd98, 0x223c4c1, 0x5d84c1f):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x87ffd98 = (choices, default_value, max_length, mutable, private, required))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x87ffd98, 0x223c4c1, 0x5d84c1f) = (choices, default_value, max_length, mutable, private, required))" % __pyx_checksum)
  *     __pyx_result = StrField.__new__(__pyx_type)
  */
-    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
-    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PickleError);
-    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_2, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_INCREF(__pyx_t_2);
-    __pyx_v___pyx_PickleError = __pyx_t_2;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
+    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_v___pyx_PickleError = __pyx_t_1;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":6
- *     if __pyx_checksum != 0x87ffd98:
+ *     if __pyx_checksum not in (0x87ffd98, 0x223c4c1, 0x5d84c1f):
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x87ffd98 = (choices, default_value, max_length, mutable, private, required))" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x87ffd98, 0x223c4c1, 0x5d84c1f) = (choices, default_value, max_length, mutable, private, required))" % __pyx_checksum)             # <<<<<<<<<<<<<<
  *     __pyx_result = StrField.__new__(__pyx_type)
  *     if __pyx_state is not None:
  */
-    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_s_vs_0x87, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_2, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_INCREF(__pyx_v___pyx_PickleError);
-    __pyx_t_2 = __pyx_v___pyx_PickleError; __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_5);
+    __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 6, __pyx_L1_error)
 
     /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x87ffd98:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0x87ffd98, 0x223c4c1, 0x5d84c1f):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x87ffd98 = (choices, default_value, max_length, mutable, private, required))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x87ffd98, 0x223c4c1, 0x5d84c1f) = (choices, default_value, max_length, mutable, private, required))" % __pyx_checksum)
  */
   }
 
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x87ffd98 = (choices, default_value, max_length, mutable, private, required))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x87ffd98, 0x223c4c1, 0x5d84c1f) = (choices, default_value, max_length, mutable, private, required))" % __pyx_checksum)
  *     __pyx_result = StrField.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_StrField__set_state(<StrField> __pyx_result, __pyx_state)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_6nyoibo_6fields_StrField), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_6nyoibo_6fields_StrField), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v___pyx_type);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v___pyx_result = __pyx_t_3;
-  __pyx_t_3 = 0;
+  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result = __pyx_t_4;
+  __pyx_t_4 = 0;
 
   /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x87ffd98 = (choices, default_value, max_length, mutable, private, required))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x87ffd98, 0x223c4c1, 0x5d84c1f) = (choices, default_value, max_length, mutable, private, required))" % __pyx_checksum)
  *     __pyx_result = StrField.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_StrField__set_state(<StrField> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
-  __pyx_t_1 = (__pyx_v___pyx_state != Py_None);
-  __pyx_t_6 = (__pyx_t_1 != 0);
-  if (__pyx_t_6) {
+  __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_2 = (__pyx_t_3 != 0);
+  if (__pyx_t_2) {
 
     /* "(tree fragment)":9
  *     __pyx_result = StrField.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_StrField__set_state(<StrField> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_StrField__set_state(StrField __pyx_result, tuple __pyx_state):
  */
-    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
-    __pyx_t_3 = __pyx_f_6nyoibo_6fields___pyx_unpickle_StrField__set_state(((struct __pyx_obj_6nyoibo_6fields_StrField *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 9, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
+    __pyx_t_4 = __pyx_f_6nyoibo_6fields___pyx_unpickle_StrField__set_state(((struct __pyx_obj_6nyoibo_6fields_StrField *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x87ffd98 = (choices, default_value, max_length, mutable, private, required))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x87ffd98, 0x223c4c1, 0x5d84c1f) = (choices, default_value, max_length, mutable, private, required))" % __pyx_checksum)
  *     __pyx_result = StrField.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_StrField__set_state(<StrField> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   }
 
@@ -8816,18 +8913,18 @@
  * def __pyx_unpickle_StrField(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("nyoibo.fields.__pyx_unpickle_StrField", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -9101,151 +9198,155 @@
 }
 
 static PyObject *__pyx_pf_6nyoibo_6fields_4__pyx_unpickle_IntField(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
+  PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_IntField", 0);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xd43e024:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0xd43e024, 0xd116a37, 0xd2e28da):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xd43e024 = (choices, default_value, max_value, min_value, mutable, private, required))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd43e024, 0xd116a37, 0xd2e28da) = (choices, default_value, max_value, min_value, mutable, private, required))" % __pyx_checksum)
  */
-  __pyx_t_1 = ((__pyx_v___pyx_checksum != 0xd43e024) != 0);
-  if (__pyx_t_1) {
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__5, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xd43e024:
+ *     if __pyx_checksum not in (0xd43e024, 0xd116a37, 0xd2e28da):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xd43e024 = (choices, default_value, max_value, min_value, mutable, private, required))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd43e024, 0xd116a37, 0xd2e28da) = (choices, default_value, max_value, min_value, mutable, private, required))" % __pyx_checksum)
  *     __pyx_result = IntField.__new__(__pyx_type)
  */
-    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
-    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PickleError);
-    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_2, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_INCREF(__pyx_t_2);
-    __pyx_v___pyx_PickleError = __pyx_t_2;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
+    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_v___pyx_PickleError = __pyx_t_1;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":6
- *     if __pyx_checksum != 0xd43e024:
+ *     if __pyx_checksum not in (0xd43e024, 0xd116a37, 0xd2e28da):
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xd43e024 = (choices, default_value, max_value, min_value, mutable, private, required))" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd43e024, 0xd116a37, 0xd2e28da) = (choices, default_value, max_value, min_value, mutable, private, required))" % __pyx_checksum)             # <<<<<<<<<<<<<<
  *     __pyx_result = IntField.__new__(__pyx_type)
  *     if __pyx_state is not None:
  */
-    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_s_vs_0xd4, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_3, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_INCREF(__pyx_v___pyx_PickleError);
-    __pyx_t_2 = __pyx_v___pyx_PickleError; __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_5);
+    __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 6, __pyx_L1_error)
 
     /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xd43e024:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0xd43e024, 0xd116a37, 0xd2e28da):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xd43e024 = (choices, default_value, max_value, min_value, mutable, private, required))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd43e024, 0xd116a37, 0xd2e28da) = (choices, default_value, max_value, min_value, mutable, private, required))" % __pyx_checksum)
  */
   }
 
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xd43e024 = (choices, default_value, max_value, min_value, mutable, private, required))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd43e024, 0xd116a37, 0xd2e28da) = (choices, default_value, max_value, min_value, mutable, private, required))" % __pyx_checksum)
  *     __pyx_result = IntField.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_IntField__set_state(<IntField> __pyx_result, __pyx_state)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_6nyoibo_6fields_IntField), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_6nyoibo_6fields_IntField), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v___pyx_type);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v___pyx_result = __pyx_t_3;
-  __pyx_t_3 = 0;
+  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result = __pyx_t_4;
+  __pyx_t_4 = 0;
 
   /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xd43e024 = (choices, default_value, max_value, min_value, mutable, private, required))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd43e024, 0xd116a37, 0xd2e28da) = (choices, default_value, max_value, min_value, mutable, private, required))" % __pyx_checksum)
  *     __pyx_result = IntField.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_IntField__set_state(<IntField> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
-  __pyx_t_1 = (__pyx_v___pyx_state != Py_None);
-  __pyx_t_6 = (__pyx_t_1 != 0);
-  if (__pyx_t_6) {
+  __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_2 = (__pyx_t_3 != 0);
+  if (__pyx_t_2) {
 
     /* "(tree fragment)":9
  *     __pyx_result = IntField.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_IntField__set_state(<IntField> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_IntField__set_state(IntField __pyx_result, tuple __pyx_state):
  */
-    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
-    __pyx_t_3 = __pyx_f_6nyoibo_6fields___pyx_unpickle_IntField__set_state(((struct __pyx_obj_6nyoibo_6fields_IntField *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 9, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
+    __pyx_t_4 = __pyx_f_6nyoibo_6fields___pyx_unpickle_IntField__set_state(((struct __pyx_obj_6nyoibo_6fields_IntField *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xd43e024 = (choices, default_value, max_value, min_value, mutable, private, required))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xd43e024, 0xd116a37, 0xd2e28da) = (choices, default_value, max_value, min_value, mutable, private, required))" % __pyx_checksum)
  *     __pyx_result = IntField.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_IntField__set_state(<IntField> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   }
 
@@ -9265,18 +9366,18 @@
  * def __pyx_unpickle_IntField(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("nyoibo.fields.__pyx_unpickle_IntField", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -9562,151 +9663,155 @@
 }
 
 static PyObject *__pyx_pf_6nyoibo_6fields_6__pyx_unpickle_BoolField(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
+  PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_BoolField", 0);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xe41db34:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0xe41db34, 0x22cbad7, 0xa0145de):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe41db34 = (choices, default_value, mutable, private, required))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe41db34, 0x22cbad7, 0xa0145de) = (choices, default_value, mutable, private, required))" % __pyx_checksum)
  */
-  __pyx_t_1 = ((__pyx_v___pyx_checksum != 0xe41db34) != 0);
-  if (__pyx_t_1) {
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__3, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xe41db34:
+ *     if __pyx_checksum not in (0xe41db34, 0x22cbad7, 0xa0145de):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe41db34 = (choices, default_value, mutable, private, required))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe41db34, 0x22cbad7, 0xa0145de) = (choices, default_value, mutable, private, required))" % __pyx_checksum)
  *     __pyx_result = BoolField.__new__(__pyx_type)
  */
-    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
-    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PickleError);
-    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_2, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_INCREF(__pyx_t_2);
-    __pyx_v___pyx_PickleError = __pyx_t_2;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
+    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_v___pyx_PickleError = __pyx_t_1;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":6
- *     if __pyx_checksum != 0xe41db34:
+ *     if __pyx_checksum not in (0xe41db34, 0x22cbad7, 0xa0145de):
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe41db34 = (choices, default_value, mutable, private, required))" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe41db34, 0x22cbad7, 0xa0145de) = (choices, default_value, mutable, private, required))" % __pyx_checksum)             # <<<<<<<<<<<<<<
  *     __pyx_result = BoolField.__new__(__pyx_type)
  *     if __pyx_state is not None:
  */
-    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_s_vs_0xe4, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_INCREF(__pyx_v___pyx_PickleError);
-    __pyx_t_2 = __pyx_v___pyx_PickleError; __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_5);
+    __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 6, __pyx_L1_error)
 
     /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xe41db34:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0xe41db34, 0x22cbad7, 0xa0145de):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe41db34 = (choices, default_value, mutable, private, required))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe41db34, 0x22cbad7, 0xa0145de) = (choices, default_value, mutable, private, required))" % __pyx_checksum)
  */
   }
 
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe41db34 = (choices, default_value, mutable, private, required))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe41db34, 0x22cbad7, 0xa0145de) = (choices, default_value, mutable, private, required))" % __pyx_checksum)
  *     __pyx_result = BoolField.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_BoolField__set_state(<BoolField> __pyx_result, __pyx_state)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_6nyoibo_6fields_BoolField), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_6nyoibo_6fields_BoolField), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v___pyx_type);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v___pyx_result = __pyx_t_3;
-  __pyx_t_3 = 0;
+  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result = __pyx_t_4;
+  __pyx_t_4 = 0;
 
   /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe41db34 = (choices, default_value, mutable, private, required))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe41db34, 0x22cbad7, 0xa0145de) = (choices, default_value, mutable, private, required))" % __pyx_checksum)
  *     __pyx_result = BoolField.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_BoolField__set_state(<BoolField> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
-  __pyx_t_1 = (__pyx_v___pyx_state != Py_None);
-  __pyx_t_6 = (__pyx_t_1 != 0);
-  if (__pyx_t_6) {
+  __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_2 = (__pyx_t_3 != 0);
+  if (__pyx_t_2) {
 
     /* "(tree fragment)":9
  *     __pyx_result = BoolField.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_BoolField__set_state(<BoolField> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_BoolField__set_state(BoolField __pyx_result, tuple __pyx_state):
  */
-    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
-    __pyx_t_3 = __pyx_f_6nyoibo_6fields___pyx_unpickle_BoolField__set_state(((struct __pyx_obj_6nyoibo_6fields_BoolField *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 9, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
+    __pyx_t_4 = __pyx_f_6nyoibo_6fields___pyx_unpickle_BoolField__set_state(((struct __pyx_obj_6nyoibo_6fields_BoolField *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe41db34 = (choices, default_value, mutable, private, required))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe41db34, 0x22cbad7, 0xa0145de) = (choices, default_value, mutable, private, required))" % __pyx_checksum)
  *     __pyx_result = BoolField.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_BoolField__set_state(<BoolField> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   }
 
@@ -9726,18 +9831,18 @@
  * def __pyx_unpickle_BoolField(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("nyoibo.fields.__pyx_unpickle_BoolField", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -10001,151 +10106,155 @@
 }
 
 static PyObject *__pyx_pf_6nyoibo_6fields_8__pyx_unpickle_DateField(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
+  PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_DateField", 0);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xe41db34:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0xe41db34, 0x22cbad7, 0xa0145de):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe41db34 = (choices, default_value, mutable, private, required))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe41db34, 0x22cbad7, 0xa0145de) = (choices, default_value, mutable, private, required))" % __pyx_checksum)
  */
-  __pyx_t_1 = ((__pyx_v___pyx_checksum != 0xe41db34) != 0);
-  if (__pyx_t_1) {
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__3, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xe41db34:
+ *     if __pyx_checksum not in (0xe41db34, 0x22cbad7, 0xa0145de):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe41db34 = (choices, default_value, mutable, private, required))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe41db34, 0x22cbad7, 0xa0145de) = (choices, default_value, mutable, private, required))" % __pyx_checksum)
  *     __pyx_result = DateField.__new__(__pyx_type)
  */
-    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
-    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PickleError);
-    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_2, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_INCREF(__pyx_t_2);
-    __pyx_v___pyx_PickleError = __pyx_t_2;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
+    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_v___pyx_PickleError = __pyx_t_1;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":6
- *     if __pyx_checksum != 0xe41db34:
+ *     if __pyx_checksum not in (0xe41db34, 0x22cbad7, 0xa0145de):
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe41db34 = (choices, default_value, mutable, private, required))" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe41db34, 0x22cbad7, 0xa0145de) = (choices, default_value, mutable, private, required))" % __pyx_checksum)             # <<<<<<<<<<<<<<
  *     __pyx_result = DateField.__new__(__pyx_type)
  *     if __pyx_state is not None:
  */
-    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_s_vs_0xe4, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_INCREF(__pyx_v___pyx_PickleError);
-    __pyx_t_2 = __pyx_v___pyx_PickleError; __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_5);
+    __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 6, __pyx_L1_error)
 
     /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xe41db34:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0xe41db34, 0x22cbad7, 0xa0145de):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe41db34 = (choices, default_value, mutable, private, required))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe41db34, 0x22cbad7, 0xa0145de) = (choices, default_value, mutable, private, required))" % __pyx_checksum)
  */
   }
 
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe41db34 = (choices, default_value, mutable, private, required))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe41db34, 0x22cbad7, 0xa0145de) = (choices, default_value, mutable, private, required))" % __pyx_checksum)
  *     __pyx_result = DateField.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_DateField__set_state(<DateField> __pyx_result, __pyx_state)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_6nyoibo_6fields_DateField), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_6nyoibo_6fields_DateField), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v___pyx_type);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v___pyx_result = __pyx_t_3;
-  __pyx_t_3 = 0;
+  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result = __pyx_t_4;
+  __pyx_t_4 = 0;
 
   /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe41db34 = (choices, default_value, mutable, private, required))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe41db34, 0x22cbad7, 0xa0145de) = (choices, default_value, mutable, private, required))" % __pyx_checksum)
  *     __pyx_result = DateField.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_DateField__set_state(<DateField> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
-  __pyx_t_1 = (__pyx_v___pyx_state != Py_None);
-  __pyx_t_6 = (__pyx_t_1 != 0);
-  if (__pyx_t_6) {
+  __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_2 = (__pyx_t_3 != 0);
+  if (__pyx_t_2) {
 
     /* "(tree fragment)":9
  *     __pyx_result = DateField.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_DateField__set_state(<DateField> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_DateField__set_state(DateField __pyx_result, tuple __pyx_state):
  */
-    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
-    __pyx_t_3 = __pyx_f_6nyoibo_6fields___pyx_unpickle_DateField__set_state(((struct __pyx_obj_6nyoibo_6fields_DateField *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 9, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
+    __pyx_t_4 = __pyx_f_6nyoibo_6fields___pyx_unpickle_DateField__set_state(((struct __pyx_obj_6nyoibo_6fields_DateField *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe41db34 = (choices, default_value, mutable, private, required))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe41db34, 0x22cbad7, 0xa0145de) = (choices, default_value, mutable, private, required))" % __pyx_checksum)
  *     __pyx_result = DateField.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_DateField__set_state(<DateField> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   }
 
@@ -10165,18 +10274,18 @@
  * def __pyx_unpickle_DateField(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("nyoibo.fields.__pyx_unpickle_DateField", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -10440,151 +10549,155 @@
 }
 
 static PyObject *__pyx_pf_6nyoibo_6fields_10__pyx_unpickle_DatetimeField(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
+  PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_DatetimeField", 0);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xe41db34:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0xe41db34, 0x22cbad7, 0xa0145de):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe41db34 = (choices, default_value, mutable, private, required))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe41db34, 0x22cbad7, 0xa0145de) = (choices, default_value, mutable, private, required))" % __pyx_checksum)
  */
-  __pyx_t_1 = ((__pyx_v___pyx_checksum != 0xe41db34) != 0);
-  if (__pyx_t_1) {
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__3, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xe41db34:
+ *     if __pyx_checksum not in (0xe41db34, 0x22cbad7, 0xa0145de):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe41db34 = (choices, default_value, mutable, private, required))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe41db34, 0x22cbad7, 0xa0145de) = (choices, default_value, mutable, private, required))" % __pyx_checksum)
  *     __pyx_result = DatetimeField.__new__(__pyx_type)
  */
-    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
-    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PickleError);
-    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_2, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_INCREF(__pyx_t_2);
-    __pyx_v___pyx_PickleError = __pyx_t_2;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
+    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_v___pyx_PickleError = __pyx_t_1;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":6
- *     if __pyx_checksum != 0xe41db34:
+ *     if __pyx_checksum not in (0xe41db34, 0x22cbad7, 0xa0145de):
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe41db34 = (choices, default_value, mutable, private, required))" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe41db34, 0x22cbad7, 0xa0145de) = (choices, default_value, mutable, private, required))" % __pyx_checksum)             # <<<<<<<<<<<<<<
  *     __pyx_result = DatetimeField.__new__(__pyx_type)
  *     if __pyx_state is not None:
  */
-    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_s_vs_0xe4, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_INCREF(__pyx_v___pyx_PickleError);
-    __pyx_t_2 = __pyx_v___pyx_PickleError; __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_5);
+    __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 6, __pyx_L1_error)
 
     /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xe41db34:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0xe41db34, 0x22cbad7, 0xa0145de):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe41db34 = (choices, default_value, mutable, private, required))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe41db34, 0x22cbad7, 0xa0145de) = (choices, default_value, mutable, private, required))" % __pyx_checksum)
  */
   }
 
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe41db34 = (choices, default_value, mutable, private, required))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe41db34, 0x22cbad7, 0xa0145de) = (choices, default_value, mutable, private, required))" % __pyx_checksum)
  *     __pyx_result = DatetimeField.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_DatetimeField__set_state(<DatetimeField> __pyx_result, __pyx_state)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_6nyoibo_6fields_DatetimeField), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_6nyoibo_6fields_DatetimeField), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v___pyx_type);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v___pyx_result = __pyx_t_3;
-  __pyx_t_3 = 0;
+  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result = __pyx_t_4;
+  __pyx_t_4 = 0;
 
   /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe41db34 = (choices, default_value, mutable, private, required))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe41db34, 0x22cbad7, 0xa0145de) = (choices, default_value, mutable, private, required))" % __pyx_checksum)
  *     __pyx_result = DatetimeField.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_DatetimeField__set_state(<DatetimeField> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
-  __pyx_t_1 = (__pyx_v___pyx_state != Py_None);
-  __pyx_t_6 = (__pyx_t_1 != 0);
-  if (__pyx_t_6) {
+  __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_2 = (__pyx_t_3 != 0);
+  if (__pyx_t_2) {
 
     /* "(tree fragment)":9
  *     __pyx_result = DatetimeField.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_DatetimeField__set_state(<DatetimeField> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_DatetimeField__set_state(DatetimeField __pyx_result, tuple __pyx_state):
  */
-    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
-    __pyx_t_3 = __pyx_f_6nyoibo_6fields___pyx_unpickle_DatetimeField__set_state(((struct __pyx_obj_6nyoibo_6fields_DatetimeField *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 9, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
+    __pyx_t_4 = __pyx_f_6nyoibo_6fields___pyx_unpickle_DatetimeField__set_state(((struct __pyx_obj_6nyoibo_6fields_DatetimeField *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe41db34 = (choices, default_value, mutable, private, required))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe41db34, 0x22cbad7, 0xa0145de) = (choices, default_value, mutable, private, required))" % __pyx_checksum)
  *     __pyx_result = DatetimeField.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_DatetimeField__set_state(<DatetimeField> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   }
 
@@ -10604,18 +10717,18 @@
  * def __pyx_unpickle_DatetimeField(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("nyoibo.fields.__pyx_unpickle_DatetimeField", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -10879,151 +10992,155 @@
 }
 
 static PyObject *__pyx_pf_6nyoibo_6fields_12__pyx_unpickle_FloatField(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
+  PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_FloatField", 0);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xe41db34:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0xe41db34, 0x22cbad7, 0xa0145de):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe41db34 = (choices, default_value, mutable, private, required))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe41db34, 0x22cbad7, 0xa0145de) = (choices, default_value, mutable, private, required))" % __pyx_checksum)
  */
-  __pyx_t_1 = ((__pyx_v___pyx_checksum != 0xe41db34) != 0);
-  if (__pyx_t_1) {
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__3, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xe41db34:
+ *     if __pyx_checksum not in (0xe41db34, 0x22cbad7, 0xa0145de):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe41db34 = (choices, default_value, mutable, private, required))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe41db34, 0x22cbad7, 0xa0145de) = (choices, default_value, mutable, private, required))" % __pyx_checksum)
  *     __pyx_result = FloatField.__new__(__pyx_type)
  */
-    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
-    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PickleError);
-    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_2, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_INCREF(__pyx_t_2);
-    __pyx_v___pyx_PickleError = __pyx_t_2;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
+    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_v___pyx_PickleError = __pyx_t_1;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":6
- *     if __pyx_checksum != 0xe41db34:
+ *     if __pyx_checksum not in (0xe41db34, 0x22cbad7, 0xa0145de):
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe41db34 = (choices, default_value, mutable, private, required))" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe41db34, 0x22cbad7, 0xa0145de) = (choices, default_value, mutable, private, required))" % __pyx_checksum)             # <<<<<<<<<<<<<<
  *     __pyx_result = FloatField.__new__(__pyx_type)
  *     if __pyx_state is not None:
  */
-    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_s_vs_0xe4, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_INCREF(__pyx_v___pyx_PickleError);
-    __pyx_t_2 = __pyx_v___pyx_PickleError; __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_5);
+    __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 6, __pyx_L1_error)
 
     /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xe41db34:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0xe41db34, 0x22cbad7, 0xa0145de):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe41db34 = (choices, default_value, mutable, private, required))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe41db34, 0x22cbad7, 0xa0145de) = (choices, default_value, mutable, private, required))" % __pyx_checksum)
  */
   }
 
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe41db34 = (choices, default_value, mutable, private, required))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe41db34, 0x22cbad7, 0xa0145de) = (choices, default_value, mutable, private, required))" % __pyx_checksum)
  *     __pyx_result = FloatField.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_FloatField__set_state(<FloatField> __pyx_result, __pyx_state)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_6nyoibo_6fields_FloatField), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_6nyoibo_6fields_FloatField), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v___pyx_type);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v___pyx_result = __pyx_t_3;
-  __pyx_t_3 = 0;
+  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result = __pyx_t_4;
+  __pyx_t_4 = 0;
 
   /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe41db34 = (choices, default_value, mutable, private, required))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe41db34, 0x22cbad7, 0xa0145de) = (choices, default_value, mutable, private, required))" % __pyx_checksum)
  *     __pyx_result = FloatField.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_FloatField__set_state(<FloatField> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
-  __pyx_t_1 = (__pyx_v___pyx_state != Py_None);
-  __pyx_t_6 = (__pyx_t_1 != 0);
-  if (__pyx_t_6) {
+  __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_2 = (__pyx_t_3 != 0);
+  if (__pyx_t_2) {
 
     /* "(tree fragment)":9
  *     __pyx_result = FloatField.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_FloatField__set_state(<FloatField> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_FloatField__set_state(FloatField __pyx_result, tuple __pyx_state):
  */
-    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
-    __pyx_t_3 = __pyx_f_6nyoibo_6fields___pyx_unpickle_FloatField__set_state(((struct __pyx_obj_6nyoibo_6fields_FloatField *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 9, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
+    __pyx_t_4 = __pyx_f_6nyoibo_6fields___pyx_unpickle_FloatField__set_state(((struct __pyx_obj_6nyoibo_6fields_FloatField *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe41db34 = (choices, default_value, mutable, private, required))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe41db34, 0x22cbad7, 0xa0145de) = (choices, default_value, mutable, private, required))" % __pyx_checksum)
  *     __pyx_result = FloatField.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_FloatField__set_state(<FloatField> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   }
 
@@ -11043,18 +11160,18 @@
  * def __pyx_unpickle_FloatField(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("nyoibo.fields.__pyx_unpickle_FloatField", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -11318,151 +11435,155 @@
 }
 
 static PyObject *__pyx_pf_6nyoibo_6fields_14__pyx_unpickle_DecimalField(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
+  PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_DecimalField", 0);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xe41db34:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0xe41db34, 0x22cbad7, 0xa0145de):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe41db34 = (choices, default_value, mutable, private, required))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe41db34, 0x22cbad7, 0xa0145de) = (choices, default_value, mutable, private, required))" % __pyx_checksum)
  */
-  __pyx_t_1 = ((__pyx_v___pyx_checksum != 0xe41db34) != 0);
-  if (__pyx_t_1) {
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__3, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xe41db34:
+ *     if __pyx_checksum not in (0xe41db34, 0x22cbad7, 0xa0145de):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe41db34 = (choices, default_value, mutable, private, required))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe41db34, 0x22cbad7, 0xa0145de) = (choices, default_value, mutable, private, required))" % __pyx_checksum)
  *     __pyx_result = DecimalField.__new__(__pyx_type)
  */
-    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
-    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PickleError);
-    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_2, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_INCREF(__pyx_t_2);
-    __pyx_v___pyx_PickleError = __pyx_t_2;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
+    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_v___pyx_PickleError = __pyx_t_1;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":6
- *     if __pyx_checksum != 0xe41db34:
+ *     if __pyx_checksum not in (0xe41db34, 0x22cbad7, 0xa0145de):
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe41db34 = (choices, default_value, mutable, private, required))" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe41db34, 0x22cbad7, 0xa0145de) = (choices, default_value, mutable, private, required))" % __pyx_checksum)             # <<<<<<<<<<<<<<
  *     __pyx_result = DecimalField.__new__(__pyx_type)
  *     if __pyx_state is not None:
  */
-    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_s_vs_0xe4, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_INCREF(__pyx_v___pyx_PickleError);
-    __pyx_t_2 = __pyx_v___pyx_PickleError; __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_5);
+    __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 6, __pyx_L1_error)
 
     /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0xe41db34:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0xe41db34, 0x22cbad7, 0xa0145de):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe41db34 = (choices, default_value, mutable, private, required))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe41db34, 0x22cbad7, 0xa0145de) = (choices, default_value, mutable, private, required))" % __pyx_checksum)
  */
   }
 
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe41db34 = (choices, default_value, mutable, private, required))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe41db34, 0x22cbad7, 0xa0145de) = (choices, default_value, mutable, private, required))" % __pyx_checksum)
  *     __pyx_result = DecimalField.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_DecimalField__set_state(<DecimalField> __pyx_result, __pyx_state)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_6nyoibo_6fields_DecimalField), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_6nyoibo_6fields_DecimalField), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v___pyx_type);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v___pyx_result = __pyx_t_3;
-  __pyx_t_3 = 0;
+  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result = __pyx_t_4;
+  __pyx_t_4 = 0;
 
   /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe41db34 = (choices, default_value, mutable, private, required))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe41db34, 0x22cbad7, 0xa0145de) = (choices, default_value, mutable, private, required))" % __pyx_checksum)
  *     __pyx_result = DecimalField.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_DecimalField__set_state(<DecimalField> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
-  __pyx_t_1 = (__pyx_v___pyx_state != Py_None);
-  __pyx_t_6 = (__pyx_t_1 != 0);
-  if (__pyx_t_6) {
+  __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_2 = (__pyx_t_3 != 0);
+  if (__pyx_t_2) {
 
     /* "(tree fragment)":9
  *     __pyx_result = DecimalField.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_DecimalField__set_state(<DecimalField> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_DecimalField__set_state(DecimalField __pyx_result, tuple __pyx_state):
  */
-    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
-    __pyx_t_3 = __pyx_f_6nyoibo_6fields___pyx_unpickle_DecimalField__set_state(((struct __pyx_obj_6nyoibo_6fields_DecimalField *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 9, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
+    __pyx_t_4 = __pyx_f_6nyoibo_6fields___pyx_unpickle_DecimalField__set_state(((struct __pyx_obj_6nyoibo_6fields_DecimalField *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xe41db34 = (choices, default_value, mutable, private, required))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe41db34, 0x22cbad7, 0xa0145de) = (choices, default_value, mutable, private, required))" % __pyx_checksum)
  *     __pyx_result = DecimalField.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_DecimalField__set_state(<DecimalField> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   }
 
@@ -11482,18 +11603,18 @@
  * def __pyx_unpickle_DecimalField(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("nyoibo.fields.__pyx_unpickle_DecimalField", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -11757,151 +11878,155 @@
 }
 
 static PyObject *__pyx_pf_6nyoibo_6fields_16__pyx_unpickle_LinkField(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
+  PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_LinkField", 0);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x37df068:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0x37df068, 0x13e4e4a, 0x17f2992):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x37df068 = (choices, default_value, mutable, private, required, to))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x37df068, 0x13e4e4a, 0x17f2992) = (choices, default_value, mutable, private, required, to))" % __pyx_checksum)
  */
-  __pyx_t_1 = ((__pyx_v___pyx_checksum != 0x37df068) != 0);
-  if (__pyx_t_1) {
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__6, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x37df068:
+ *     if __pyx_checksum not in (0x37df068, 0x13e4e4a, 0x17f2992):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x37df068 = (choices, default_value, mutable, private, required, to))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x37df068, 0x13e4e4a, 0x17f2992) = (choices, default_value, mutable, private, required, to))" % __pyx_checksum)
  *     __pyx_result = LinkField.__new__(__pyx_type)
  */
-    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
-    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PickleError);
-    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_2, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_INCREF(__pyx_t_2);
-    __pyx_v___pyx_PickleError = __pyx_t_2;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
+    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_v___pyx_PickleError = __pyx_t_1;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":6
- *     if __pyx_checksum != 0x37df068:
+ *     if __pyx_checksum not in (0x37df068, 0x13e4e4a, 0x17f2992):
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x37df068 = (choices, default_value, mutable, private, required, to))" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x37df068, 0x13e4e4a, 0x17f2992) = (choices, default_value, mutable, private, required, to))" % __pyx_checksum)             # <<<<<<<<<<<<<<
  *     __pyx_result = LinkField.__new__(__pyx_type)
  *     if __pyx_state is not None:
  */
-    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_s_vs_0x37, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_4, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_INCREF(__pyx_v___pyx_PickleError);
-    __pyx_t_2 = __pyx_v___pyx_PickleError; __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_5);
+    __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 6, __pyx_L1_error)
 
     /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x37df068:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0x37df068, 0x13e4e4a, 0x17f2992):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x37df068 = (choices, default_value, mutable, private, required, to))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x37df068, 0x13e4e4a, 0x17f2992) = (choices, default_value, mutable, private, required, to))" % __pyx_checksum)
  */
   }
 
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x37df068 = (choices, default_value, mutable, private, required, to))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x37df068, 0x13e4e4a, 0x17f2992) = (choices, default_value, mutable, private, required, to))" % __pyx_checksum)
  *     __pyx_result = LinkField.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_LinkField__set_state(<LinkField> __pyx_result, __pyx_state)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_6nyoibo_6fields_LinkField), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_6nyoibo_6fields_LinkField), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v___pyx_type);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v___pyx_result = __pyx_t_3;
-  __pyx_t_3 = 0;
+  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result = __pyx_t_4;
+  __pyx_t_4 = 0;
 
   /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x37df068 = (choices, default_value, mutable, private, required, to))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x37df068, 0x13e4e4a, 0x17f2992) = (choices, default_value, mutable, private, required, to))" % __pyx_checksum)
  *     __pyx_result = LinkField.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_LinkField__set_state(<LinkField> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
-  __pyx_t_1 = (__pyx_v___pyx_state != Py_None);
-  __pyx_t_6 = (__pyx_t_1 != 0);
-  if (__pyx_t_6) {
+  __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_2 = (__pyx_t_3 != 0);
+  if (__pyx_t_2) {
 
     /* "(tree fragment)":9
  *     __pyx_result = LinkField.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_LinkField__set_state(<LinkField> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_LinkField__set_state(LinkField __pyx_result, tuple __pyx_state):
  */
-    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
-    __pyx_t_3 = __pyx_f_6nyoibo_6fields___pyx_unpickle_LinkField__set_state(((struct __pyx_obj_6nyoibo_6fields_LinkField *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 9, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
+    __pyx_t_4 = __pyx_f_6nyoibo_6fields___pyx_unpickle_LinkField__set_state(((struct __pyx_obj_6nyoibo_6fields_LinkField *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x37df068 = (choices, default_value, mutable, private, required, to))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x37df068, 0x13e4e4a, 0x17f2992) = (choices, default_value, mutable, private, required, to))" % __pyx_checksum)
  *     __pyx_result = LinkField.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_LinkField__set_state(<LinkField> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   }
 
@@ -11921,18 +12046,18 @@
  * def __pyx_unpickle_LinkField(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("nyoibo.fields.__pyx_unpickle_LinkField", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -12282,21 +12407,21 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1
+  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PYPY_VERSION_NUM+0 >= 0x06000000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_6nyoibo_6fields_StrField __pyx_vtable_6nyoibo_6fields_StrField;
 
 static PyObject *__pyx_tp_new_6nyoibo_6fields_StrField(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_6nyoibo_6fields_StrField *p;
@@ -12370,21 +12495,21 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1
+  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PYPY_VERSION_NUM+0 >= 0x06000000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_6nyoibo_6fields_IntField __pyx_vtable_6nyoibo_6fields_IntField;
 
 static PyObject *__pyx_tp_new_6nyoibo_6fields_IntField(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_6nyoibo_6fields_IntField *p;
@@ -12501,21 +12626,21 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1
+  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PYPY_VERSION_NUM+0 >= 0x06000000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_6nyoibo_6fields_LinkField __pyx_vtable_6nyoibo_6fields_LinkField;
 
 static PyObject *__pyx_tp_new_6nyoibo_6fields_LinkField(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_6nyoibo_6fields_LinkField *p;
@@ -12633,21 +12758,21 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1
+  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PYPY_VERSION_NUM+0 >= 0x06000000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_6nyoibo_6fields_BoolField __pyx_vtable_6nyoibo_6fields_BoolField;
 
 static PyObject *__pyx_tp_new_6nyoibo_6fields_BoolField(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_6nyoibo_6fields_BoolField *p;
@@ -12725,21 +12850,21 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1
+  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PYPY_VERSION_NUM+0 >= 0x06000000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_6nyoibo_6fields_DateField __pyx_vtable_6nyoibo_6fields_DateField;
 
 static PyObject *__pyx_tp_new_6nyoibo_6fields_DateField(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_6nyoibo_6fields_DateField *p;
@@ -12817,21 +12942,21 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1
+  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PYPY_VERSION_NUM+0 >= 0x06000000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_6nyoibo_6fields_DatetimeField __pyx_vtable_6nyoibo_6fields_DatetimeField;
 
 static PyObject *__pyx_tp_new_6nyoibo_6fields_DatetimeField(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_6nyoibo_6fields_DatetimeField *p;
@@ -12909,21 +13034,21 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1
+  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PYPY_VERSION_NUM+0 >= 0x06000000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_6nyoibo_6fields_FloatField __pyx_vtable_6nyoibo_6fields_FloatField;
 
 static PyObject *__pyx_tp_new_6nyoibo_6fields_FloatField(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_6nyoibo_6fields_FloatField *p;
@@ -13001,21 +13126,21 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1
+  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PYPY_VERSION_NUM+0 >= 0x06000000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_6nyoibo_6fields_DecimalField __pyx_vtable_6nyoibo_6fields_DecimalField;
 
 static PyObject *__pyx_tp_new_6nyoibo_6fields_DecimalField(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_6nyoibo_6fields_DecimalField *p;
@@ -13093,21 +13218,21 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1
+  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PYPY_VERSION_NUM+0 >= 0x06000000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
@@ -13165,18 +13290,18 @@
   {&__pyx_n_s_Field, __pyx_k_Field, sizeof(__pyx_k_Field), 0, 0, 1, 1},
   {&__pyx_n_s_FieldValueError, __pyx_k_FieldValueError, sizeof(__pyx_k_FieldValueError), 0, 0, 1, 1},
   {&__pyx_kp_s_Field_for_dict_values, __pyx_k_Field_for_dict_values, sizeof(__pyx_k_Field_for_dict_values), 0, 0, 1, 0},
   {&__pyx_kp_s_Field_for_json_values, __pyx_k_Field_for_json_values, sizeof(__pyx_k_Field_for_json_values), 0, 0, 1, 0},
   {&__pyx_kp_s_Field_for_list_values, __pyx_k_Field_for_list_values, sizeof(__pyx_k_Field_for_list_values), 0, 0, 1, 0},
   {&__pyx_kp_s_Field_for_tuple_values, __pyx_k_Field_for_tuple_values, sizeof(__pyx_k_Field_for_tuple_values), 0, 0, 1, 0},
   {&__pyx_n_s_FloatField, __pyx_k_FloatField, sizeof(__pyx_k_FloatField), 0, 0, 1, 1},
-  {&__pyx_kp_s_Incompatible_checksums_s_vs_0x37, __pyx_k_Incompatible_checksums_s_vs_0x37, sizeof(__pyx_k_Incompatible_checksums_s_vs_0x37), 0, 0, 1, 0},
-  {&__pyx_kp_s_Incompatible_checksums_s_vs_0x87, __pyx_k_Incompatible_checksums_s_vs_0x87, sizeof(__pyx_k_Incompatible_checksums_s_vs_0x87), 0, 0, 1, 0},
-  {&__pyx_kp_s_Incompatible_checksums_s_vs_0xd4, __pyx_k_Incompatible_checksums_s_vs_0xd4, sizeof(__pyx_k_Incompatible_checksums_s_vs_0xd4), 0, 0, 1, 0},
-  {&__pyx_kp_s_Incompatible_checksums_s_vs_0xe4, __pyx_k_Incompatible_checksums_s_vs_0xe4, sizeof(__pyx_k_Incompatible_checksums_s_vs_0xe4), 0, 0, 1, 0},
+  {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_k_Incompatible_checksums_0x_x_vs_0, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0), 0, 0, 1, 0},
+  {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_2, __pyx_k_Incompatible_checksums_0x_x_vs_0_2, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0_2), 0, 0, 1, 0},
+  {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_3, __pyx_k_Incompatible_checksums_0x_x_vs_0_3, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0_3), 0, 0, 1, 0},
+  {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_4, __pyx_k_Incompatible_checksums_0x_x_vs_0_4, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0_4), 0, 0, 1, 0},
   {&__pyx_n_s_IntField, __pyx_k_IntField, sizeof(__pyx_k_IntField), 0, 0, 1, 1},
   {&__pyx_n_s_IntMaxValueError, __pyx_k_IntMaxValueError, sizeof(__pyx_k_IntMaxValueError), 0, 0, 1, 1},
   {&__pyx_n_s_IntMinValueError, __pyx_k_IntMinValueError, sizeof(__pyx_k_IntMinValueError), 0, 0, 1, 1},
   {&__pyx_n_s_InvalidOperation, __pyx_k_InvalidOperation, sizeof(__pyx_k_InvalidOperation), 0, 0, 1, 1},
   {&__pyx_n_s_JSONField, __pyx_k_JSONField, sizeof(__pyx_k_JSONField), 0, 0, 1, 1},
   {&__pyx_n_s_JSONField_parse, __pyx_k_JSONField_parse, sizeof(__pyx_k_JSONField_parse), 0, 0, 1, 1},
   {&__pyx_n_s_LinkField, __pyx_k_LinkField, sizeof(__pyx_k_LinkField), 0, 0, 1, 1},
@@ -13289,89 +13414,117 @@
  *         super(LinkField, self).__init__(*args, **kwargs)
  *         self.to = to
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_to_must_be_an_Entity_subclass); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 240, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
+  /* "(tree fragment)":4
+ *     cdef object __pyx_PickleError
+ *     cdef object __pyx_result
+ *     if __pyx_checksum not in (0xe41db34, 0x22cbad7, 0xa0145de):             # <<<<<<<<<<<<<<
+ *         from pickle import PickleError as __pyx_PickleError
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xe41db34, 0x22cbad7, 0xa0145de) = (choices, default_value, mutable, private, required))" % __pyx_checksum)
+ */
+  __pyx_tuple__3 = PyTuple_Pack(3, __pyx_int_239196980, __pyx_int_36485847, __pyx_int_167855582); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__3);
+  __Pyx_GIVEREF(__pyx_tuple__3);
+  __pyx_tuple__4 = PyTuple_Pack(3, __pyx_int_142605720, __pyx_int_35898561, __pyx_int_98061343); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__4);
+  __Pyx_GIVEREF(__pyx_tuple__4);
+  __pyx_tuple__5 = PyTuple_Pack(3, __pyx_int_222552100, __pyx_int_219245111, __pyx_int_221128922); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__5);
+  __Pyx_GIVEREF(__pyx_tuple__5);
+  __pyx_tuple__6 = PyTuple_Pack(3, __pyx_int_58585192, __pyx_int_20860490, __pyx_int_25110930); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__6);
+  __Pyx_GIVEREF(__pyx_tuple__6);
+
   /* "nyoibo/fields.pyx":32
  * 
  *     _internal_type = None
  *     _exceptions = (TypeError, ValueError)             # <<<<<<<<<<<<<<
  * 
  *     def __init__(self, private=False, mutable=False, default_value=None,
  */
-  __pyx_tuple__3 = PyTuple_Pack(2, __pyx_builtin_TypeError, __pyx_builtin_ValueError); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 32, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__3);
-  __Pyx_GIVEREF(__pyx_tuple__3);
+  __pyx_tuple__7 = PyTuple_Pack(2, __pyx_builtin_TypeError, __pyx_builtin_ValueError); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 32, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__7);
+  __Pyx_GIVEREF(__pyx_tuple__7);
 
   /* "nyoibo/fields.pyx":268
  *     _internal_type = str
  * 
  *     def parse(self, value):             # <<<<<<<<<<<<<<
  *         try:
  *             return json.dumps(value)
  */
-  __pyx_tuple__4 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_value_2); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 268, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__4);
-  __Pyx_GIVEREF(__pyx_tuple__4);
-  __pyx_codeobj__5 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__4, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nyoibo_fields_pyx, __pyx_n_s_parse, 268, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__5)) __PYX_ERR(0, 268, __pyx_L1_error)
+  __pyx_tuple__8 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_value_2); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 268, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__8);
+  __Pyx_GIVEREF(__pyx_tuple__8);
+  __pyx_codeobj__9 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__8, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nyoibo_fields_pyx, __pyx_n_s_parse, 268, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__9)) __PYX_ERR(0, 268, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_Field(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_tuple__6 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__6);
-  __Pyx_GIVEREF(__pyx_tuple__6);
-  __pyx_codeobj__7 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Field, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__7)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __pyx_tuple__8 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__8);
-  __Pyx_GIVEREF(__pyx_tuple__8);
-  __pyx_codeobj__9 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__8, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_StrField, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__9)) __PYX_ERR(1, 1, __pyx_L1_error)
   __pyx_tuple__10 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__10);
   __Pyx_GIVEREF(__pyx_tuple__10);
-  __pyx_codeobj__11 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__10, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_IntField, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__11)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_codeobj__11 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__10, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Field, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__11)) __PYX_ERR(1, 1, __pyx_L1_error)
   __pyx_tuple__12 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__12);
   __Pyx_GIVEREF(__pyx_tuple__12);
-  __pyx_codeobj__13 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__12, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_BoolField, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__13)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_codeobj__13 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__12, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_StrField, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__13)) __PYX_ERR(1, 1, __pyx_L1_error)
   __pyx_tuple__14 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__14);
   __Pyx_GIVEREF(__pyx_tuple__14);
-  __pyx_codeobj__15 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__14, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_DateField, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__15)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_codeobj__15 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__14, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_IntField, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__15)) __PYX_ERR(1, 1, __pyx_L1_error)
   __pyx_tuple__16 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__16);
   __Pyx_GIVEREF(__pyx_tuple__16);
-  __pyx_codeobj__17 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__16, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_DatetimeField, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__17)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_codeobj__17 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__16, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_BoolField, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__17)) __PYX_ERR(1, 1, __pyx_L1_error)
   __pyx_tuple__18 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__18);
   __Pyx_GIVEREF(__pyx_tuple__18);
-  __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__18, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_FloatField, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__18, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_DateField, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(1, 1, __pyx_L1_error)
   __pyx_tuple__20 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__20);
   __Pyx_GIVEREF(__pyx_tuple__20);
-  __pyx_codeobj__21 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__20, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_DecimalField, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__21)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_codeobj__21 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__20, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_DatetimeField, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__21)) __PYX_ERR(1, 1, __pyx_L1_error)
   __pyx_tuple__22 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__22);
   __Pyx_GIVEREF(__pyx_tuple__22);
-  __pyx_codeobj__23 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_LinkField, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__23)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_codeobj__23 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_FloatField, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__23)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__24 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__24);
+  __Pyx_GIVEREF(__pyx_tuple__24);
+  __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__24, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_DecimalField, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__26 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__26);
+  __Pyx_GIVEREF(__pyx_tuple__26);
+  __pyx_codeobj__27 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__26, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_LinkField, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__27)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_20860490 = PyInt_FromLong(20860490L); if (unlikely(!__pyx_int_20860490)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_25110930 = PyInt_FromLong(25110930L); if (unlikely(!__pyx_int_25110930)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_35898561 = PyInt_FromLong(35898561L); if (unlikely(!__pyx_int_35898561)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_36485847 = PyInt_FromLong(36485847L); if (unlikely(!__pyx_int_36485847)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_58585192 = PyInt_FromLong(58585192L); if (unlikely(!__pyx_int_58585192)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_98061343 = PyInt_FromLong(98061343L); if (unlikely(!__pyx_int_98061343)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_142605720 = PyInt_FromLong(142605720L); if (unlikely(!__pyx_int_142605720)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_167855582 = PyInt_FromLong(167855582L); if (unlikely(!__pyx_int_167855582)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_219245111 = PyInt_FromLong(219245111L); if (unlikely(!__pyx_int_219245111)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_221128922 = PyInt_FromLong(221128922L); if (unlikely(!__pyx_int_221128922)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_222552100 = PyInt_FromLong(222552100L); if (unlikely(!__pyx_int_222552100)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_239196980 = PyInt_FromLong(239196980L); if (unlikely(!__pyx_int_239196980)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
@@ -13743,15 +13896,15 @@
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_nyoibo__fields) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -13913,15 +14066,15 @@
   /* "nyoibo/fields.pyx":32
  * 
  *     _internal_type = None
  *     _exceptions = (TypeError, ValueError)             # <<<<<<<<<<<<<<
  * 
  *     def __init__(self, private=False, mutable=False, default_value=None,
  */
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_6nyoibo_6fields_Field->tp_dict, __pyx_n_s_exceptions, __pyx_tuple__3) < 0) __PYX_ERR(0, 32, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_6nyoibo_6fields_Field->tp_dict, __pyx_n_s_exceptions, __pyx_tuple__7) < 0) __PYX_ERR(0, 32, __pyx_L1_error)
   PyType_Modified(__pyx_ptype_6nyoibo_6fields_Field);
 
   /* "nyoibo/fields.pyx":97
  *     """
  * 
  *     _internal_type = str             # <<<<<<<<<<<<<<
  * 
@@ -14106,15 +14259,15 @@
   /* "nyoibo/fields.pyx":268
  *     _internal_type = str
  * 
  *     def parse(self, value):             # <<<<<<<<<<<<<<
  *         try:
  *             return json.dumps(value)
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6nyoibo_6fields_9JSONField_1parse, 0, __pyx_n_s_JSONField_parse, NULL, __pyx_n_s_nyoibo_fields, __pyx_d, ((PyObject *)__pyx_codeobj__5)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 268, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_6nyoibo_6fields_9JSONField_1parse, 0, __pyx_n_s_JSONField_parse, NULL, __pyx_n_s_nyoibo_fields, __pyx_d, ((PyObject *)__pyx_codeobj__9)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 268, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_parse, __pyx_t_4) < 0) __PYX_ERR(0, 268, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "nyoibo/fields.pyx":262
  * 
  * 
@@ -15002,28 +15155,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -15438,15 +15591,15 @@
         uval = NULL;
         if (uoffset > 0) {
             prepend_sign = !!prepend_sign;
             if (uoffset > prepend_sign) {
                 padding = PyUnicode_FromOrdinal(padding_char);
                 if (likely(padding) && uoffset > prepend_sign + 1) {
                     PyObject *tmp;
-                    PyObject *repeat = PyInt_FromSize_t(uoffset - prepend_sign);
+                    PyObject *repeat = PyInt_FromSsize_t(uoffset - prepend_sign);
                     if (unlikely(!repeat)) goto done_or_error;
                     tmp = PyNumber_Multiply(padding, repeat);
                     Py_DECREF(repeat);
                     Py_DECREF(padding);
                     padding = tmp;
                 }
                 if (unlikely(!padding)) goto done_or_error;
@@ -15641,15 +15794,15 @@
         ps2 = PyBytes_AS_STRING(s2);
         if (ps1[0] != ps2[0]) {
             return (equals == Py_NE);
         } else if (length == 1) {
             return (equals == Py_EQ);
         } else {
             int result;
-#if CYTHON_USE_UNICODE_INTERNALS
+#if CYTHON_USE_UNICODE_INTERNALS && (PY_VERSION_HEX < 0x030B0000)
             Py_hash_t hash1, hash2;
             hash1 = ((PyBytesObject*)s1)->ob_shash;
             hash2 = ((PyBytesObject*)s2)->ob_shash;
             if (hash1 != hash2 && hash1 != -1 && hash2 != -1) {
                 return (equals == Py_NE);
             }
 #endif
@@ -16064,25 +16217,43 @@
   }
   Py_XDECREF(name_attr);
   return ret;
 }
 static int __Pyx_setup_reduce(PyObject* type_obj) {
     int ret = 0;
     PyObject *object_reduce = NULL;
+    PyObject *object_getstate = NULL;
     PyObject *object_reduce_ex = NULL;
     PyObject *reduce = NULL;
     PyObject *reduce_ex = NULL;
     PyObject *reduce_cython = NULL;
     PyObject *setstate = NULL;
     PyObject *setstate_cython = NULL;
+    PyObject *getstate = NULL;
 #if CYTHON_USE_PYTYPE_LOOKUP
-    if (_PyType_Lookup((PyTypeObject*)type_obj, __pyx_n_s_getstate)) goto __PYX_GOOD;
+    getstate = _PyType_Lookup((PyTypeObject*)type_obj, __pyx_n_s_getstate);
 #else
-    if (PyObject_HasAttr(type_obj, __pyx_n_s_getstate)) goto __PYX_GOOD;
+    getstate = __Pyx_PyObject_GetAttrStrNoError(type_obj, __pyx_n_s_getstate);
+    if (!getstate && PyErr_Occurred()) {
+        goto __PYX_BAD;
+    }
+#endif
+    if (getstate) {
+#if CYTHON_USE_PYTYPE_LOOKUP
+        object_getstate = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_getstate);
+#else
+        object_getstate = __Pyx_PyObject_GetAttrStrNoError((PyObject*)&PyBaseObject_Type, __pyx_n_s_getstate);
+        if (!object_getstate && PyErr_Occurred()) {
+            goto __PYX_BAD;
+        }
 #endif
+        if (object_getstate != getstate) {
+            goto __PYX_GOOD;
+        }
+    }
 #if CYTHON_USE_PYTYPE_LOOKUP
     object_reduce_ex = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
 #else
     object_reduce_ex = __Pyx_PyObject_GetAttrStr((PyObject*)&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
 #endif
     reduce_ex = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_reduce_ex); if (unlikely(!reduce_ex)) goto __PYX_BAD;
     if (reduce_ex == object_reduce_ex) {
@@ -16119,14 +16290,16 @@
     if (!PyErr_Occurred())
         PyErr_Format(PyExc_RuntimeError, "Unable to initialize pickling for %s", ((PyTypeObject*)type_obj)->tp_name);
     ret = -1;
 __PYX_GOOD:
 #if !CYTHON_USE_PYTYPE_LOOKUP
     Py_XDECREF(object_reduce);
     Py_XDECREF(object_reduce_ex);
+    Py_XDECREF(object_getstate);
+    Py_XDECREF(getstate);
 #endif
     Py_XDECREF(reduce);
     Py_XDECREF(reduce_ex);
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
@@ -16770,14 +16943,22 @@
         argc = PyTuple_GET_SIZE(args);
         new_args = PyTuple_GetSlice(args, 1, argc);
         if (unlikely(!new_args))
             return NULL;
         self = PyTuple_GetItem(args, 0);
         if (unlikely(!self)) {
             Py_DECREF(new_args);
+#if PY_MAJOR_VERSION > 2
+            PyErr_Format(PyExc_TypeError,
+                         "unbound method %.200S() needs an argument",
+                         cyfunc->func_qualname);
+#else
+            PyErr_SetString(PyExc_TypeError,
+                            "unbound method needs an argument");
+#endif
             return NULL;
         }
         result = __Pyx_CyFunction_CallMethod(func, self, new_args, kw);
         Py_DECREF(new_args);
     } else {
         result = __Pyx_CyFunction_Call(func, args, kw);
     }
@@ -16838,21 +17019,21 @@
     0,
     0,
     0,
     0,
 #if PY_VERSION_HEX >= 0x030400a1
     0,
 #endif
-#if PY_VERSION_HEX >= 0x030800b1
+#if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PYPY_VERSION_NUM+0 >= 0x06000000
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
     0,
 #endif
 };
 static int __pyx_CyFunction_init(void) {
     __pyx_CyFunctionType = __Pyx_FetchCommonType(&__pyx_CyFunctionType_type);
     if (unlikely(__pyx_CyFunctionType == NULL)) {
         return -1;
@@ -16896,15 +17077,15 @@
         PyObject_GC_Track(op);
     }
     return op;
 }
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
@@ -17020,14 +17201,20 @@
     Py_INCREF(code_object);
 }
 
 /* AddTraceback */
 #include "compile.h"
 #include "frameobject.h"
 #include "traceback.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
 static PyCodeObject* __Pyx_CreateCodeObjectForTraceback(
             const char *funcname, int c_line,
             int py_line, const char *filename) {
     PyCodeObject *py_code = NULL;
     PyObject *py_funcname = NULL;
     #if PY_MAJOR_VERSION < 3
     PyObject *py_srcfile = NULL;
@@ -17083,22 +17270,32 @@
     return NULL;
 }
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename) {
     PyCodeObject *py_code = 0;
     PyFrameObject *py_frame = 0;
     PyThreadState *tstate = __Pyx_PyThreadState_Current;
+    PyObject *ptype, *pvalue, *ptraceback;
     if (c_line) {
         c_line = __Pyx_CLineForTraceback(tstate, c_line);
     }
     py_code = __pyx_find_code_object(c_line ? -c_line : py_line);
     if (!py_code) {
+        __Pyx_ErrFetchInState(tstate, &ptype, &pvalue, &ptraceback);
         py_code = __Pyx_CreateCodeObjectForTraceback(
             funcname, c_line, py_line, filename);
-        if (!py_code) goto bad;
+        if (!py_code) {
+            /* If the code object creation fails, then we should clear the
+               fetched exception references and propagate the new exception */
+            Py_XDECREF(ptype);
+            Py_XDECREF(pvalue);
+            Py_XDECREF(ptraceback);
+            goto bad;
+        }
+        __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
         __pyx_insert_code_object(c_line ? -c_line : py_line, py_code);
     }
     py_frame = PyFrame_New(
         tstate,            /*PyThreadState *tstate,*/
         py_code,           /*PyCodeObject *code,*/
         __pyx_d,    /*PyObject *globals,*/
         0                  /*PyObject *locals*/
@@ -17599,19 +17796,41 @@
         return _PyLong_FromByteArray(bytes, sizeof(long),
                                      little, !is_unsigned);
     }
 }
 
 /* CheckBinaryVersion */
 static int __Pyx_check_binary_version(void) {
-    char ctversion[4], rtversion[4];
-    PyOS_snprintf(ctversion, 4, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
-    PyOS_snprintf(rtversion, 4, "%s", Py_GetVersion());
-    if (ctversion[0] != rtversion[0] || ctversion[2] != rtversion[2]) {
+    char ctversion[5];
+    int same=1, i, found_dot;
+    const char* rt_from_call = Py_GetVersion();
+    PyOS_snprintf(ctversion, 5, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
+    found_dot = 0;
+    for (i = 0; i < 4; i++) {
+        if (!ctversion[i]) {
+            same = (rt_from_call[i] < '0' || rt_from_call[i] > '9');
+            break;
+        }
+        if (rt_from_call[i] != ctversion[i]) {
+            same = 0;
+            break;
+        }
+    }
+    if (!same) {
+        char rtversion[5] = {'\0'};
         char message[200];
+        for (i=0; i<4; ++i) {
+            if (rt_from_call[i] == '.') {
+                if (found_dot) break;
+                found_dot = 1;
+            } else if (rt_from_call[i] < '0' || rt_from_call[i] > '9') {
+                break;
+            }
+            rtversion[i] = rt_from_call[i];
+        }
         PyOS_snprintf(message, sizeof(message),
                       "compiletime version %s of module '%.100s' "
                       "does not match runtime version %s",
                       ctversion, __Pyx_MODULE_NAME, rtversion);
         return PyErr_WarnEx(NULL, message, 1);
     }
     return 0;
```

### Comparing `nyoibo-0.4.1/nyoibo.egg-info/PKG-INFO` & `nyoibo-0.5.0/nyoibo.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,172 +1,170 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: nyoibo
-Version: 0.4.1
+Version: 0.5.0
 Summary: Implement attributes accessors in an easy way
 Home-page: https://github.com/pity7736/nyoibo
 Author: Julián Cortés
-Author-email: pity7736@gmail.com
-License: UNKNOWN
-Description: Nyoibo
-        ======
-        
-        .. image:: https://readthedocs.org/projects/nyoibo/badge/?version=latest
-            :target: https://nyoibo.readthedocs.io/en/latest/?badge=latest
-            :alt: Documentation Status
-        
-        .. image:: https://circleci.com/gh/pity7736/nyoibo.svg?style=shield
-            :target: https://circleci.com/gh/pity7736/nyoibo
-        
-        Nyoibo is an easy way to avoid repetitive code with "private" attributes in
-        Python.
-        
-        `See full documentation <https://nyoibo.readthedocs.io/en/latest/>`_
-        
-        
-        Installation
-        ------------
-        
-        You can install nyoibo with pip. Nyoibo requires python 3.7 or higer.
-        
-        ``pip install nyoibo``
-        
-        
-        What does "nyoibo" mean?
-        ------------------------
-        
-        Nyoibo is a mystical staff given to Son Goku by his grandfather Son Gohan.
-        
-        .. image:: ./nyoibo.png
-           :width: 300px
-           :height: 300px
-           :alt: nyoibo
-        
-        
-        Usage
-        -----
-        
-        Instead of doing this:
-        
-        .. code-block:: python
-        
-            class Example:
-        
-                def __init__(self, value=None, other_value=None, default='hello')
-                    self._value = value
-                    self._other_value = other_value
-                    self._default = default
-        
-                def get_value(self):
-                    return self._value
-        
-                value = property(get_value)
-        
-                def get_other_value(self):
-                    return self._other_value
-        
-                def set_other_value(self, value):
-                    self._other_value = value
-        
-                other_value = property(get_other_value, set_other_value)
-        
-                def do_something(self):
-                    return f'{self._default} world'
-        
-        
-        You can do this:
-        
-        .. code-block:: python
-        
-            from nyoibo import Entity, fields
-        
-        
-            class Example(Entity):
-                _value = fields.StrField()
-                _other_value = fields.IntField(mutable=True)
-                _default = fields.StrField(private=True, default_value='hello')
-        
-                def do_something(self):
-                    return f'{self._default} world'
-        
-        In both cases you could use this code like this:
-        
-        .. code-block:: python
-        
-            example = Example(value='some value', other_value=10)
-        
-            assert example.value == 'some value'
-            assert example.get_value() == 'some value'
-            assert example.get_other_value() == 10
-            example.other_value = 15
-            assert example.get_other_value() == 15
-            assert example.do_something() == 'hello world'
-        
-        
-        Why not use dataclass decorator?
-        --------------------------------
-        
-        ``@dataclass`` decorator helps to avoid to write the ``__init__`` method but if you
-        want to use this approach (information hiding and encapsulation), you need to
-        write getters and setters anyway. Furthermore, with ``nyoibo`` you get extra
-        features like casting to right value (due to static typing), validations, override ``__init__`` method and so on.
-        
-        Above example with ``dataclass`` decorator:
-        
-        .. code-block:: python
-        
-            from dataclasses import dataclass
-        
-        
-            @dataclass
-            class Example:
-                _value: str
-                _other_value: int
-                _default: str = 'hello'
-        
-                def get_value(self):
-                    return self._value
-        
-                value = property(get_value)
-        
-                def get_other_value(self):
-                    return self._other_value
-        
-                def set_other_value(self, value):
-                    self._other_value = value
-        
-                other_value = property(get_other_value, set_other_value)
-        
-                def do_something(self):
-                    return f'{self._default} world'
-        
-        Even this code doesn't work because ``__init__`` method has ``_value``,
-        ``_other_value`` and ``_default`` arguments. Therefore the instantiation will be:
-        
-        .. code-block:: python
-        
-            example = Example(_value='some value', _other_value=10)
-        
-        
-        
-        License
-        -------
-        
-        Distributed under the terms of the LGPLv3 license.
-        
-        See `license <https://github.com/pity7736/nyoibo/blob/master/LICENSE>`_.
-        
+Author-email: julian.cortes77@protonmail.com
 Keywords: accessors private
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Requires-Python: >=3.9
+License-File: LICENSE
+
+Nyoibo
+======
+
+.. image:: https://readthedocs.org/projects/nyoibo/badge/?version=latest
+    :target: https://nyoibo.readthedocs.io/en/latest/?badge=latest
+    :alt: Documentation Status
+
+.. image:: https://circleci.com/gh/pity7736/nyoibo.svg?style=shield
+    :target: https://circleci.com/gh/pity7736/nyoibo
+
+Nyoibo is an easy way to avoid repetitive code with "private" attributes in
+Python.
+
+`See full documentation <https://nyoibo.readthedocs.io/en/latest/>`_
+
+
+Installation
+------------
+
+You can install nyoibo with pip. Nyoibo requires python 3.9 or higher.
+
+``pip install nyoibo``
+
+
+What does "nyoibo" mean?
+------------------------
+
+Nyoibo is a mystical staff given to Son Goku by his grandfather Son Gohan.
+
+.. image:: ./nyoibo.png
+   :width: 300px
+   :height: 300px
+   :alt: nyoibo
+
+
+Usage
+-----
+
+Instead of doing this:
+
+.. code-block:: python
+
+    class Example:
+
+        def __init__(self, value=None, other_value=None, default='hello')
+            self._value = value
+            self._other_value = other_value
+            self._default = default
+
+        def get_value(self):
+            return self._value
+
+        value = property(get_value)
+
+        def get_other_value(self):
+            return self._other_value
+
+        def set_other_value(self, value):
+            self._other_value = value
+
+        other_value = property(get_other_value, set_other_value)
+
+        def do_something(self):
+            return f'{self._default} world'
+
+
+You can do this:
+
+.. code-block:: python
+
+    from nyoibo import Entity, fields
+
+
+    class Example(Entity):
+        _value = fields.StrField()
+        _other_value = fields.IntField(mutable=True)
+        _default = fields.StrField(private=True, default_value='hello')
+
+        def do_something(self):
+            return f'{self._default} world'
+
+In both cases you could use this code like this:
+
+.. code-block:: python
+
+    example = Example(value='some value', other_value=10)
+
+    assert example.value == 'some value'
+    assert example.get_value() == 'some value'
+    assert example.get_other_value() == 10
+    example.other_value = 15
+    assert example.get_other_value() == 15
+    assert example.do_something() == 'hello world'
+
+
+Why not use dataclass decorator?
+--------------------------------
+
+``@dataclass`` decorator helps to avoid to write the ``__init__`` method but if you
+want to use this approach (information hiding and encapsulation), you need to
+write getters and setters anyway. Furthermore, with ``nyoibo`` you get extra
+features like casting to right value (due to static typing), validations, override ``__init__`` method and so on.
+
+Above example with ``dataclass`` decorator:
+
+.. code-block:: python
+
+    from dataclasses import dataclass
+
+
+    @dataclass
+    class Example:
+        _value: str
+        _other_value: int
+        _default: str = 'hello'
+
+        def get_value(self):
+            return self._value
+
+        value = property(get_value)
+
+        def get_other_value(self):
+            return self._other_value
+
+        def set_other_value(self, value):
+            self._other_value = value
+
+        other_value = property(get_other_value, set_other_value)
+
+        def do_something(self):
+            return f'{self._default} world'
+
+Even this code doesn't work because ``__init__`` method has ``_value``,
+``_other_value`` and ``_default`` arguments. Therefore the instantiation will be:
+
+.. code-block:: python
+
+    example = Example(_value='some value', _other_value=10)
+
+
+
+License
+-------
+
+Distributed under the terms of the LGPLv3 license.
+
+See `license <https://github.com/pity7736/nyoibo/blob/master/LICENSE>`_.
```

### Comparing `nyoibo-0.4.1/setup.py` & `nyoibo-0.5.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,16 +26,16 @@
             VERSION = version.strip(" \n'\"")
             break
 
 with open('README.rst') as f:
     readme = f.read()
 
 tests_require = [
-    'pytest==6.2.5'
-    'pytest-cov==3.0.0'
+    'pytest~=7.0.0',
+    'pytest-cov~=3.0.0'
 ]
 
 extensions = [
     Extension('nyoibo.fields', [f'nyoibo/fields.{ext}']),
     Extension('nyoibo.entities.entity', [f'nyoibo/entities/entity.{ext}'])
 ]
 
@@ -50,31 +50,30 @@
     )
 
 setup(
     name='nyoibo',
     version=VERSION,
     packages=find_packages(),
     author='Julián Cortés',
-    author_email='pity7736@gmail.com',
+    author_email='julian.cortes77@protonmail.com',
     description='Implement attributes accessors in an easy way',
     long_description=readme,
     keywords='accessors private',
     ext_modules=extensions,
     url='https://github.com/pity7736/nyoibo',
     tests_require=tests_require,
-    python_requires='>=3.7',
+    python_requires='>=3.9',
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Natural Language :: English',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3 :: Only',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Software Development',
         'Topic :: Utilities',
         'Typing :: Typed'
     ]
 )
```

### Comparing `nyoibo-0.4.1/tests/test_entity.py` & `nyoibo-0.5.0/tests/test_entity.py`

 * *Files identical despite different names*

### Comparing `nyoibo-0.4.1/tests/test_extend_entity.py` & `nyoibo-0.5.0/tests/test_extend_entity.py`

 * *Files identical despite different names*

### Comparing `nyoibo-0.4.1/tests/test_fields.py` & `nyoibo-0.5.0/tests/test_fields.py`

 * *Files identical despite different names*

