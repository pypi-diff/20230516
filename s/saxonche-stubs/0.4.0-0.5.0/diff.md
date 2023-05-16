# Comparing `tmp/saxonche_stubs-0.4.0.tar.gz` & `tmp/saxonche_stubs-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saxonche_stubs-0.4.0.tar", max compression
+gzip compressed data, was "saxonche_stubs-0.5.0.tar", max compression
```

## Comparing `saxonche_stubs-0.4.0.tar` & `saxonche_stubs-0.5.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      490 2023-04-21 15:06:15.152853 saxonche_stubs-0.4.0/README.md
--rw-r--r--   0        0        0     1572 2023-04-27 14:19:13.462861 saxonche_stubs-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     9838 2023-04-27 14:19:07.274991 saxonche_stubs-0.4.0/saxonche-stubs/__init__.pyi
--rw-r--r--   0        0        0     1127 1970-01-01 00:00:00.000000 saxonche_stubs-0.4.0/setup.py
--rw-r--r--   0        0        0     1991 1970-01-01 00:00:00.000000 saxonche_stubs-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      490 2023-04-21 15:06:15.152853 saxonche_stubs-0.5.0/README.md
+-rw-r--r--   0        0        0     1572 2023-05-16 17:34:34.747572 saxonche_stubs-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0    11580 2023-05-16 17:33:26.788581 saxonche_stubs-0.5.0/saxonche-stubs/__init__.pyi
+-rw-r--r--   0        0        0     1127 1970-01-01 00:00:00.000000 saxonche_stubs-0.5.0/setup.py
+-rw-r--r--   0        0        0     1991 1970-01-01 00:00:00.000000 saxonche_stubs-0.5.0/PKG-INFO
```

### Comparing `saxonche_stubs-0.4.0/pyproject.toml` & `saxonche_stubs-0.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "saxonche-stubs"
-version = "0.4.0"
+version = "0.5.0"
 description = "Type stubs for saxonche"
 authors = ["Bpolitycki <bastian.politycki@unisg.ch>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 packages = [{include = "saxonche-stubs"}]
 
 classifiers = [
```

### Comparing `saxonche_stubs-0.4.0/saxonche-stubs/__init__.pyi` & `saxonche_stubs-0.5.0/saxonche-stubs/__init__.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -14,14 +14,24 @@
         exc_type: Any,
         exc_val: Any,
         exc_tb: Any,
     ) -> None: ...
     def clear_configuration_properties(self) -> None:
         """Clear all configuration properties that have been set"""
         ...
+    def exception_clear(self) -> None:
+        """Clear any exception that has been raised"""
+        ...
+    def exception_occurred(self) -> bool:
+        """Check whether an exception has been raised internally within Saxon/C.
+
+        Returns:
+            bool: True if an exception has been raised, False otherwise
+        """
+        ...
     def new_xpath_processor(self) -> PyXPathProcessor:
         """Creates a new XPath processor, which used to evaluate XPath expressions."""
         ...
     def new_xquery_processor(self) -> PyXQueryProcessor:
         """Creates a new XQuery processor, which used to evaluate XQuery expressions."""
         ...
     def new_xslt30_processor(self) -> PyXslt30Processor: ...
@@ -76,35 +86,78 @@
         """Declare a namespace prefix for use in XPath expressions.
 
         Args:
             prefix (str): The namespace prefix
             uri (str): The namespace uri
         """
         ...
-    def evaluate(self, xpath: str) -> PyXdmValue:
+    def effective_boolean_value(self, xpath_str: str) -> bool:
+        """Evaluate an XPath expression and return the effective boolean value of the result.
+
+        Args:
+            xpath (str): The XPath expression
+
+        Returns:
+            bool: The effective boolean value of the result
+        """
+        ...
+    def evaluate(self, xpath_str: str) -> PyXdmValue | None:
         """Evaluate an XPath expression and return the result as a sequence.
 
         Args:
             xpath (str): The XPath expression
 
         Returns:
-            PyXdmValue: A sequence of Xdm Values is returned.
+            PyXdmValue: A sequence of Xdm Values is returned. Return None if the expression returns an empty sequence.
         """
         ...
-    def evaluate_single(self, xpath: str) -> PyXdmItem | None:
+    def evaluate_single(self, xpath_str: str) -> PyXdmItem | None:
         """Evaluate an XPath expression and return the result as a single item.
 
         Args:
             xpath (str): The XPath expression
 
         Returns:
-            PyXdmValue: A single Xdm Item is returned. return None if the expression returns an empty sequence.
+            PyXdmValue: A single Xdm Item is returned. Return None if the expression returns an empty sequence.
             If the expression returns a sequence of more than one item, any items after the first are ignored.
         """
         ...
+    def exception_clear(self) -> None:
+        """Clear any exception that has been raised"""
+        ...
+    def exception_count(self) -> int:
+        """Get the number of errors and warnings that have been reported.
+
+        Returns:
+            int: The number of errors and warnings that have been reported
+        """
+        ...
+    def exception_occured(self) -> bool:
+        """Check whether an exception has been raised internally within Saxon/C.
+
+        Returns:
+            bool: True if an exception has been raised, False otherwise
+        """
+        ...
+    @overload
+    def set_context(self, file_name: str) -> None:
+        """Set the context item from a file.
+
+        Args:
+            file_name (str): The file name of the context item
+        """
+        ...
+    @overload
+    def set_context(self, xdm_item: PyXdmItem) -> None:
+        """Set the context item from an XdmItem.
+
+        Args:
+            xdm_item (PyXdmItem): The XdmItem of the context item
+        """
+        ...
 
 class PyXQueryProcessor:
     def __init__(self) -> None:
         """An PyXQueryProcessor object represents factory to compile, load and execute queries."""
     ...
 
 class PyXslt30Processor:
```

### Comparing `saxonche_stubs-0.4.0/setup.py` & `saxonche_stubs-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['saxonche>=12.1.0,<13.0.0']
 
 setup_kwargs = {
     'name': 'saxonche-stubs',
-    'version': '0.4.0',
+    'version': '0.5.0',
     'description': 'Type stubs for saxonche',
     'long_description': '# saxonche-stubs\n\nType stubs for the [saxonche](https://pypi.org/project/saxonche/) python package. This package has no functionality itself, but is merely an addition to the completion within IDEs. The basis for type annotations and comments is the documentation of [the Saxon Python API](https://www.saxonica.com/saxon-c/doc11/html/saxonc.html).\n\nAt the moment not all APIs are fully typed.\n\n## Author / Contact\n\n- [Bastian Politycki](https://github.com/Bpolitycki) – Swiss Law Sources\n',
     'author': 'Bpolitycki',
     'author_email': 'bastian.politycki@unisg.ch',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `saxonche_stubs-0.4.0/PKG-INFO` & `saxonche_stubs-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saxonche-stubs
-Version: 0.4.0
+Version: 0.5.0
 Summary: Type stubs for saxonche
 License: GPL-3.0-or-later
 Author: Bpolitycki
 Author-email: bastian.politycki@unisg.ch
 Requires-Python: >=3.8
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

