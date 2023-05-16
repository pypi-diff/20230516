# Comparing `tmp/customdataclass-0.1.1.2.tar.gz` & `tmp/customdataclass-0.1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "customdataclass-0.1.1.2.tar", last modified: Tue May  2 08:46:04 2023, max compression
+gzip compressed data, was "customdataclass-0.1.1.3.tar", last modified: Tue May 16 12:20:33 2023, max compression
```

## Comparing `customdataclass-0.1.1.2.tar` & `customdataclass-0.1.1.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)        0 2023-05-02 08:46:04.333408 customdataclass-0.1.1.2/
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     1074 2023-04-27 13:55:41.000000 customdataclass-0.1.1.2/LICENSE.md
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     4572 2023-05-02 08:46:04.333408 customdataclass-0.1.1.2/PKG-INFO
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     4009 2023-04-27 15:41:41.000000 customdataclass-0.1.1.2/README.md
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)      685 2023-05-02 08:42:29.000000 customdataclass-0.1.1.2/pyproject.toml
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       38 2023-05-02 08:46:04.333408 customdataclass-0.1.1.2/setup.cfg
-drwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)        0 2023-05-02 08:46:04.330075 customdataclass-0.1.1.2/src/
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       48 2023-04-27 16:09:58.000000 customdataclass-0.1.1.2/src/__init__.py
-drwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)        0 2023-05-02 08:46:04.330075 customdataclass-0.1.1.2/src/customdataclass.egg-info/
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     4572 2023-05-02 08:46:04.000000 customdataclass-0.1.1.2/src/customdataclass.egg-info/PKG-INFO
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)      579 2023-05-02 08:46:04.000000 customdataclass-0.1.1.2/src/customdataclass.egg-info/SOURCES.txt
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)        1 2023-05-02 08:46:04.000000 customdataclass-0.1.1.2/src/customdataclass.egg-info/dependency_links.txt
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       25 2023-05-02 08:46:04.000000 customdataclass-0.1.1.2/src/customdataclass.egg-info/requires.txt
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       25 2023-05-02 08:46:04.000000 customdataclass-0.1.1.2/src/customdataclass.egg-info/top_level.txt
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)    15562 2023-05-02 08:28:28.000000 customdataclass-0.1.1.2/src/customdataclass.py
-drwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)        0 2023-05-02 08:46:04.330075 customdataclass-0.1.1.2/tests/
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     2223 2023-04-27 15:56:13.000000 customdataclass-0.1.1.2/tests/test_complex_dataclass.py
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     3893 2023-04-27 15:56:25.000000 customdataclass-0.1.1.2/tests/test_dataclass.py
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     2116 2023-05-01 13:46:55.000000 customdataclass-0.1.1.2/tests/test_dataclass_list.py
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)      756 2023-04-27 15:56:26.000000 customdataclass-0.1.1.2/tests/test_default_value_dataclass.py
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     1459 2023-04-27 15:56:27.000000 customdataclass-0.1.1.2/tests/test_incomplete_typing_dataclass.py
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     1469 2023-04-27 15:56:31.000000 customdataclass-0.1.1.2/tests/test_mutable_dataclass.py
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     5043 2023-04-27 16:09:06.000000 customdataclass-0.1.1.2/tests/test_nested_dataclass.py
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     2766 2023-04-27 15:56:38.000000 customdataclass-0.1.1.2/tests/test_partial_dataclass.py
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     1131 2023-04-27 15:56:43.000000 customdataclass-0.1.1.2/tests/test_random_dataclass.py
+drwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)        0 2023-05-16 12:20:33.759563 customdataclass-0.1.1.3/
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     1074 2023-04-27 13:55:41.000000 customdataclass-0.1.1.3/LICENSE.md
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     4760 2023-05-16 12:20:33.759563 customdataclass-0.1.1.3/PKG-INFO
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     4197 2023-05-02 11:45:36.000000 customdataclass-0.1.1.3/README.md
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)      685 2023-05-16 12:20:09.000000 customdataclass-0.1.1.3/pyproject.toml
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       38 2023-05-16 12:20:33.759563 customdataclass-0.1.1.3/setup.cfg
+drwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)        0 2023-05-16 12:20:33.756230 customdataclass-0.1.1.3/src/
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       48 2023-05-16 12:20:11.000000 customdataclass-0.1.1.3/src/__init__.py
+drwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)        0 2023-05-16 12:20:33.759563 customdataclass-0.1.1.3/src/customdataclass.egg-info/
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     4760 2023-05-16 12:20:33.000000 customdataclass-0.1.1.3/src/customdataclass.egg-info/PKG-INFO
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)      579 2023-05-16 12:20:33.000000 customdataclass-0.1.1.3/src/customdataclass.egg-info/SOURCES.txt
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)        1 2023-05-16 12:20:33.000000 customdataclass-0.1.1.3/src/customdataclass.egg-info/dependency_links.txt
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       25 2023-05-16 12:20:33.000000 customdataclass-0.1.1.3/src/customdataclass.egg-info/requires.txt
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       25 2023-05-16 12:20:33.000000 customdataclass-0.1.1.3/src/customdataclass.egg-info/top_level.txt
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)    15892 2023-05-16 12:19:18.000000 customdataclass-0.1.1.3/src/customdataclass.py
+drwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)        0 2023-05-16 12:20:33.759563 customdataclass-0.1.1.3/tests/
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     2223 2023-04-27 15:56:13.000000 customdataclass-0.1.1.3/tests/test_complex_dataclass.py
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     4377 2023-05-02 11:45:36.000000 customdataclass-0.1.1.3/tests/test_dataclass.py
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     2116 2023-05-01 13:46:55.000000 customdataclass-0.1.1.3/tests/test_dataclass_list.py
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)      756 2023-04-27 15:56:26.000000 customdataclass-0.1.1.3/tests/test_default_value_dataclass.py
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     1459 2023-05-02 10:17:05.000000 customdataclass-0.1.1.3/tests/test_incomplete_typing_dataclass.py
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     1698 2023-05-16 12:10:28.000000 customdataclass-0.1.1.3/tests/test_mutable_dataclass.py
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     5043 2023-04-27 16:09:06.000000 customdataclass-0.1.1.3/tests/test_nested_dataclass.py
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     2766 2023-04-27 15:56:38.000000 customdataclass-0.1.1.3/tests/test_partial_dataclass.py
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     1131 2023-04-27 15:56:43.000000 customdataclass-0.1.1.3/tests/test_random_dataclass.py
```

### Comparing `customdataclass-0.1.1.2/LICENSE.md` & `customdataclass-0.1.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `customdataclass-0.1.1.2/PKG-INFO` & `customdataclass-0.1.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 Metadata-Version: 2.1
 Name: customdataclass
-Version: 0.1.1.2
+Version: 0.1.1.3
 Summary: A custom dataclass implementation
 Author-email: Lorenzo Rossi <pypi@lorenzoros.si>
 License: MIT
 Project-URL: Homepage, https://github.com/lorossi/customdataclass
 Project-URL: Bug Tracker, https://github.com/lorossi/customdataclass/issues
 Project-URL: documentation, https://lorossi.github.io/customdataclass/
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # Customdataclass
 
-![coverage](https://img.shields.io/badge/dynamic/json?color=informational&label=code%20coverage&query=totals.percent_covered_display&suffix=%25&url=https%3A%2F%2Fraw.githubusercontent.com%2Florossi%2Fcustomdataclass%2Fmain%2Fcoverage.json)
-![issues](https://img.shields.io/github/issues-raw/lorossi/customdataclass)
-![license](https://img.shields.io/pypi/l/customdataclass)
-![python-version](https://img.shields.io/pypi/pyversions/customdataclass)
-![version](https://img.shields.io/pypi/v/customdataclass)
+<p align="center">
+<img src=https://img.shields.io/github/issues-raw/lorossi/customdataclass></img>
+<img src=https://img.shields.io/pypi/l/customdataclass></img>
+<img src=https://img.shields.io/pypi/pyversions/customdataclass></img>
+<img src=https://img.shields.io/pypi/v/customdataclass></img>
+<img src=https://img.shields.io/pypi/format/customdataclass></img>
+<img src=https://img.shields.io/badge/dynamic/json?color=informational&label=code%20coverage&query=totals.percent_covered_display&suffix=%25&url=https%3A%2F%2Fraw.githubusercontent.com%2Florossi%2Fcustomdataclass%2Fmain%2Fcoverage.json></img>
+<img src=https://img.shields.io/github/languages/top/lorossi/customdataclass></img>
+</p>
 
 Custom implementation of the `dataclass` module from the standard Python library as a base class for other dataclasses.
 The documentation is available [here](https://lorossi.github.io/customdataclass).
 
 ## Details
 
 A while back I was working on a project *(now lost in a dusty corner of my GitHub profile)* that required me to create a lot of data structures *(variables used only to hold complex data)* and I quickly realised that using dictionaries *(or named dictionaries)* was slowly becoming messy because:
```

### Comparing `customdataclass-0.1.1.2/README.md` & `customdataclass-0.1.1.3/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 # Customdataclass
 
-![coverage](https://img.shields.io/badge/dynamic/json?color=informational&label=code%20coverage&query=totals.percent_covered_display&suffix=%25&url=https%3A%2F%2Fraw.githubusercontent.com%2Florossi%2Fcustomdataclass%2Fmain%2Fcoverage.json)
-![issues](https://img.shields.io/github/issues-raw/lorossi/customdataclass)
-![license](https://img.shields.io/pypi/l/customdataclass)
-![python-version](https://img.shields.io/pypi/pyversions/customdataclass)
-![version](https://img.shields.io/pypi/v/customdataclass)
+<p align="center">
+<img src=https://img.shields.io/github/issues-raw/lorossi/customdataclass></img>
+<img src=https://img.shields.io/pypi/l/customdataclass></img>
+<img src=https://img.shields.io/pypi/pyversions/customdataclass></img>
+<img src=https://img.shields.io/pypi/v/customdataclass></img>
+<img src=https://img.shields.io/pypi/format/customdataclass></img>
+<img src=https://img.shields.io/badge/dynamic/json?color=informational&label=code%20coverage&query=totals.percent_covered_display&suffix=%25&url=https%3A%2F%2Fraw.githubusercontent.com%2Florossi%2Fcustomdataclass%2Fmain%2Fcoverage.json></img>
+<img src=https://img.shields.io/github/languages/top/lorossi/customdataclass></img>
+</p>
 
 Custom implementation of the `dataclass` module from the standard Python library as a base class for other dataclasses.
 The documentation is available [here](https://lorossi.github.io/customdataclass).
 
 ## Details
 
 A while back I was working on a project *(now lost in a dusty corner of my GitHub profile)* that required me to create a lot of data structures *(variables used only to hold complex data)* and I quickly realised that using dictionaries *(or named dictionaries)* was slowly becoming messy because:
```

### Comparing `customdataclass-0.1.1.2/pyproject.toml` & `customdataclass-0.1.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "customdataclass"
-version = "0.1.1.2"
+version = "0.1.1.3"
 authors = [{ name = "Lorenzo Rossi", email = "pypi@lorenzoros.si" }]
 description = "A custom dataclass implementation"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
   "Programming Language :: Python :: 3",
   "Operating System :: OS Independent",
```

### Comparing `customdataclass-0.1.1.2/src/customdataclass.egg-info/PKG-INFO` & `customdataclass-0.1.1.3/src/customdataclass.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 Metadata-Version: 2.1
 Name: customdataclass
-Version: 0.1.1.2
+Version: 0.1.1.3
 Summary: A custom dataclass implementation
 Author-email: Lorenzo Rossi <pypi@lorenzoros.si>
 License: MIT
 Project-URL: Homepage, https://github.com/lorossi/customdataclass
 Project-URL: Bug Tracker, https://github.com/lorossi/customdataclass/issues
 Project-URL: documentation, https://lorossi.github.io/customdataclass/
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # Customdataclass
 
-![coverage](https://img.shields.io/badge/dynamic/json?color=informational&label=code%20coverage&query=totals.percent_covered_display&suffix=%25&url=https%3A%2F%2Fraw.githubusercontent.com%2Florossi%2Fcustomdataclass%2Fmain%2Fcoverage.json)
-![issues](https://img.shields.io/github/issues-raw/lorossi/customdataclass)
-![license](https://img.shields.io/pypi/l/customdataclass)
-![python-version](https://img.shields.io/pypi/pyversions/customdataclass)
-![version](https://img.shields.io/pypi/v/customdataclass)
+<p align="center">
+<img src=https://img.shields.io/github/issues-raw/lorossi/customdataclass></img>
+<img src=https://img.shields.io/pypi/l/customdataclass></img>
+<img src=https://img.shields.io/pypi/pyversions/customdataclass></img>
+<img src=https://img.shields.io/pypi/v/customdataclass></img>
+<img src=https://img.shields.io/pypi/format/customdataclass></img>
+<img src=https://img.shields.io/badge/dynamic/json?color=informational&label=code%20coverage&query=totals.percent_covered_display&suffix=%25&url=https%3A%2F%2Fraw.githubusercontent.com%2Florossi%2Fcustomdataclass%2Fmain%2Fcoverage.json></img>
+<img src=https://img.shields.io/github/languages/top/lorossi/customdataclass></img>
+</p>
 
 Custom implementation of the `dataclass` module from the standard Python library as a base class for other dataclasses.
 The documentation is available [here](https://lorossi.github.io/customdataclass).
 
 ## Details
 
 A while back I was working on a project *(now lost in a dusty corner of my GitHub profile)* that required me to create a lot of data structures *(variables used only to hold complex data)* and I quickly realised that using dictionaries *(or named dictionaries)* was slowly becoming messy because:
```

### Comparing `customdataclass-0.1.1.2/src/customdataclass.egg-info/SOURCES.txt` & `customdataclass-0.1.1.3/src/customdataclass.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `customdataclass-0.1.1.2/src/customdataclass.py` & `customdataclass-0.1.1.3/src/customdataclass.py`

 * *Files 5% similar despite different names*

```diff
@@ -93,14 +93,24 @@
             setattr(self, k, kwargs.get(k, None))
 
         # freeze the class
         self._frozen = self._frozen_after_init
         # unset the deserialized flag
         self._deserialized = False
 
+    def freeze(
+        self,
+    ) -> None:
+        """Freeze the class.
+
+        After this, attributes cannot be changed.
+        The action cannot be undone.
+        """
+        self._frozen = True
+
     def _checkAttributesValid(self, kwargs: dict) -> bool:
         """Check if all the attributes are valid (as specified in the class \
             definition).
 
         Args:
             kwargs (dict): kwargs to check
 
@@ -423,14 +433,19 @@
             else:
                 # simple types
                 d[k] = v
 
         return d
 
     @property
+    def frozen(self) -> bool:
+        """Return the frozen status of the object."""
+        return self._frozen
+
+    @property
     @_importDecorator
     def to_json(self) -> str:
         """
         Return a json representation of the object. \
         Attributes are recursively converted to json.
 
         Returns:
```

### Comparing `customdataclass-0.1.1.2/tests/test_complex_dataclass.py` & `customdataclass-0.1.1.3/tests/test_complex_dataclass.py`

 * *Files identical despite different names*

### Comparing `customdataclass-0.1.1.2/tests/test_dataclass.py` & `customdataclass-0.1.1.3/tests/test_dataclass.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import unittest
+from typing import Any
 
 from src.customdataclass import Dataclass
 
 
 class SampleClass(Dataclass):
     """Test class."""
 
@@ -130,7 +131,28 @@
     def testCreation(self):
         s = EmptyClass()
         self.assertEqual(s.attributes, [])
 
     def testRepresentation(self):
         s = EmptyClass()
         self.assertEqual(repr(s), "EmptyClass()")
+
+
+class AnyClass(Dataclass):
+    """Test class."""
+
+    any_var: Any
+
+
+class TestAnyClass(unittest.TestCase):
+    def testCreation(self):
+        s = AnyClass(any_var=1)
+        self.assertEqual(s.any_var, 1)
+
+    def testEquality(self):
+        s1 = AnyClass(any_var=1)
+        s2 = AnyClass(any_var=1)
+        self.assertEqual(s1, s2)
+
+    def testRepresentation(self):
+        s = AnyClass(any_var=1)
+        self.assertEqual(repr(s), "AnyClass(any_var=1)")
```

### Comparing `customdataclass-0.1.1.2/tests/test_dataclass_list.py` & `customdataclass-0.1.1.3/tests/test_dataclass_list.py`

 * *Files identical despite different names*

### Comparing `customdataclass-0.1.1.2/tests/test_default_value_dataclass.py` & `customdataclass-0.1.1.3/tests/test_default_value_dataclass.py`

 * *Files identical despite different names*

### Comparing `customdataclass-0.1.1.2/tests/test_incomplete_typing_dataclass.py` & `customdataclass-0.1.1.3/tests/test_incomplete_typing_dataclass.py`

 * *Files identical despite different names*

### Comparing `customdataclass-0.1.1.2/tests/test_mutable_dataclass.py` & `customdataclass-0.1.1.3/tests/test_mutable_dataclass.py`

 * *Files 18% similar despite different names*

```diff
@@ -27,14 +27,16 @@
         self.assertEqual(s.bool_var, True)
 
         self.assertIsInstance(s.int_var, int)
         self.assertIsInstance(s.float_var, float)
         self.assertIsInstance(s.str_var, str)
         self.assertIsInstance(s.bool_var, bool)
 
+        self.assertFalse(s.frozen)
+
     def testEquality(self):
         s1, _ = self._createDataclass()
         s2, _ = self._createDataclass()
         self.assertEqual(s1, s2)
 
     def testMutation(self):
         s1, s2 = self._createDataclass()
@@ -45,7 +47,14 @@
 
         self.assertEqual(s1.int_var, 2)
         self.assertEqual(s1.float_var, 2.0)
         self.assertEqual(s1.str_var, "2")
         self.assertEqual(s1.bool_var, False)
 
         self.assertEqual(s1, s2)
+
+    def testFreeze(self):
+        s, _ = self._createDataclass()
+        s.freeze()
+        self.assertTrue(s.frozen)
+        with self.assertRaises(AttributeError):
+            s.int_var = 2
```

### Comparing `customdataclass-0.1.1.2/tests/test_nested_dataclass.py` & `customdataclass-0.1.1.3/tests/test_nested_dataclass.py`

 * *Files identical despite different names*

### Comparing `customdataclass-0.1.1.2/tests/test_partial_dataclass.py` & `customdataclass-0.1.1.3/tests/test_partial_dataclass.py`

 * *Files identical despite different names*

### Comparing `customdataclass-0.1.1.2/tests/test_random_dataclass.py` & `customdataclass-0.1.1.3/tests/test_random_dataclass.py`

 * *Files identical despite different names*

