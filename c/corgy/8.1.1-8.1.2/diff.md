# Comparing `tmp/corgy-8.1.1.tar.gz` & `tmp/corgy-8.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corgy-8.1.1.tar", max compression
+gzip compressed data, was "corgy-8.1.2.tar", max compression
```

## Comparing `corgy-8.1.1.tar` & `corgy-8.1.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0    30358 2023-04-15 15:50:54.074604 corgy-8.1.1/CHANGELOG.md
--rw-r--r--   0        0        0     1072 2023-04-15 15:50:54.074604 corgy-8.1.1/LICENSE
--rw-r--r--   0        0        0     4196 2023-04-15 15:50:54.074604 corgy-8.1.1/README.md
--rw-r--r--   0        0        0      468 2023-04-15 15:50:54.074604 corgy-8.1.1/corgy/__init__.py
--rw-r--r--   0        0        0     2329 2023-04-15 15:50:54.074604 corgy-8.1.1/corgy/_actions.py
--rw-r--r--   0        0        0      505 2023-04-15 15:50:54.074604 corgy-8.1.1/corgy/_annotations.py
--rw-r--r--   0        0        0    49762 2023-04-15 15:50:54.074604 corgy-8.1.1/corgy/_corgy.py
--rw-r--r--   0        0        0     3202 2023-04-15 15:50:54.074604 corgy-8.1.1/corgy/_corgychecker.py
--rw-r--r--   0        0        0     6237 2023-04-15 15:50:54.074604 corgy-8.1.1/corgy/_corgyparser.py
--rw-r--r--   0        0        0    36993 2023-04-15 15:50:54.078604 corgy-8.1.1/corgy/_helpfmt.py
--rw-r--r--   0        0        0    18067 2023-04-15 15:50:54.078604 corgy-8.1.1/corgy/_meta.py
--rw-r--r--   0        0        0       64 2023-04-15 15:51:34.074688 corgy-8.1.1/corgy/_version.py
--rw-r--r--   0        0        0        0 2023-04-15 15:50:54.078604 corgy-8.1.1/corgy/py.typed
--rw-r--r--   0        0        0     1598 2023-04-15 15:50:54.078604 corgy-8.1.1/corgy/types/__init__.py
--rw-r--r--   0        0        0     2382 2023-04-15 15:50:54.078604 corgy-8.1.1/corgy/types/_expand.py
--rw-r--r--   0        0        0     3413 2023-04-15 15:50:54.078604 corgy-8.1.1/corgy/types/_initargs.py
--rw-r--r--   0        0        0     2777 2023-04-15 15:50:54.078604 corgy-8.1.1/corgy/types/_inputfile.py
--rw-r--r--   0        0        0     5464 2023-04-15 15:50:54.078604 corgy-8.1.1/corgy/types/_keyvaluepairs.py
--rw-r--r--   0        0        0     5271 2023-04-15 15:50:54.078604 corgy-8.1.1/corgy/types/_outputfile.py
--rw-r--r--   0        0        0     9846 2023-04-15 15:50:54.078604 corgy-8.1.1/corgy/types/_subclass.py
--rw-r--r--   0        0        0    35296 2023-04-15 15:50:54.078604 corgy-8.1.1/docs/corgy.md
--rw-r--r--   0        0        0    11884 2023-04-15 15:50:54.078604 corgy-8.1.1/docs/corgy.types.md
--rw-r--r--   0        0        0      132 2023-04-15 15:50:54.078604 corgy-8.1.1/docs/index.md
--rw-r--r--   0        0        0     2679 2023-04-15 15:51:34.074688 corgy-8.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-15 15:50:54.078604 corgy-8.1.1/tests/__init__.py
--rw-r--r--   0        0        0    89079 2023-04-15 15:50:54.078604 corgy-8.1.1/tests/test_corgy.py
--rw-r--r--   0        0        0     4240 2023-04-15 15:50:54.078604 corgy-8.1.1/tests/test_corgychecker.py
--rw-r--r--   0        0        0    16681 2023-04-15 15:50:54.078604 corgy-8.1.1/tests/test_corgyparser.py
--rw-r--r--   0        0        0      800 2023-04-15 15:50:54.078604 corgy-8.1.1/tests/test_doctests.py
--rw-r--r--   0        0        0    47095 2023-04-15 15:50:54.078604 corgy-8.1.1/tests/test_helpfmt.py
--rw-r--r--   0        0        0        0 2023-04-15 15:50:54.078604 corgy-8.1.1/tests/types/__init__.py
--rw-r--r--   0        0        0      328 2023-04-15 15:50:54.078604 corgy-8.1.1/tests/types/_pklclasses.py
--rw-r--r--   0        0        0     2002 2023-04-15 15:50:54.078604 corgy-8.1.1/tests/types/_specialtmps.py
--rw-r--r--   0        0        0     3356 2023-04-15 15:50:54.078604 corgy-8.1.1/tests/types/_test_file.py
--rw-r--r--   0        0        0     2678 2023-04-15 15:50:54.078604 corgy-8.1.1/tests/types/test_initargs.py
--rw-r--r--   0        0        0     2496 2023-04-15 15:50:54.078604 corgy-8.1.1/tests/types/test_inputfiles.py
--rw-r--r--   0        0        0     5443 2023-04-15 15:50:54.078604 corgy-8.1.1/tests/types/test_keyvaluepairs.py
--rw-r--r--   0        0        0     5122 2023-04-15 15:50:54.078604 corgy-8.1.1/tests/types/test_outputfiles.py
--rw-r--r--   0        0        0     7082 2023-04-15 15:50:54.078604 corgy-8.1.1/tests/types/test_subclass.py
--rw-r--r--   0        0        0     5497 1970-01-01 00:00:00.000000 corgy-8.1.1/PKG-INFO
+-rw-r--r--   0        0        0    30621 2023-05-16 00:52:41.060122 corgy-8.1.2/CHANGELOG.md
+-rw-r--r--   0        0        0     1072 2023-05-16 00:52:41.060122 corgy-8.1.2/LICENSE
+-rw-r--r--   0        0        0     4196 2023-05-16 00:52:41.060122 corgy-8.1.2/README.md
+-rw-r--r--   0        0        0      468 2023-05-16 00:52:41.060122 corgy-8.1.2/corgy/__init__.py
+-rw-r--r--   0        0        0     2329 2023-05-16 00:52:41.060122 corgy-8.1.2/corgy/_actions.py
+-rw-r--r--   0        0        0      505 2023-05-16 00:52:41.060122 corgy-8.1.2/corgy/_annotations.py
+-rw-r--r--   0        0        0    49762 2023-05-16 00:52:41.060122 corgy-8.1.2/corgy/_corgy.py
+-rw-r--r--   0        0        0     3202 2023-05-16 00:52:41.060122 corgy-8.1.2/corgy/_corgychecker.py
+-rw-r--r--   0        0        0     6237 2023-05-16 00:52:41.060122 corgy-8.1.2/corgy/_corgyparser.py
+-rw-r--r--   0        0        0    36993 2023-05-16 00:52:41.060122 corgy-8.1.2/corgy/_helpfmt.py
+-rw-r--r--   0        0        0    18742 2023-05-16 00:52:41.060122 corgy-8.1.2/corgy/_meta.py
+-rw-r--r--   0        0        0       64 2023-05-16 00:53:17.388231 corgy-8.1.2/corgy/_version.py
+-rw-r--r--   0        0        0        0 2023-05-16 00:52:41.060122 corgy-8.1.2/corgy/py.typed
+-rw-r--r--   0        0        0     1598 2023-05-16 00:52:41.060122 corgy-8.1.2/corgy/types/__init__.py
+-rw-r--r--   0        0        0     2382 2023-05-16 00:52:41.060122 corgy-8.1.2/corgy/types/_expand.py
+-rw-r--r--   0        0        0     3413 2023-05-16 00:52:41.060122 corgy-8.1.2/corgy/types/_initargs.py
+-rw-r--r--   0        0        0     2777 2023-05-16 00:52:41.060122 corgy-8.1.2/corgy/types/_inputfile.py
+-rw-r--r--   0        0        0     5464 2023-05-16 00:52:41.060122 corgy-8.1.2/corgy/types/_keyvaluepairs.py
+-rw-r--r--   0        0        0     5271 2023-05-16 00:52:41.060122 corgy-8.1.2/corgy/types/_outputfile.py
+-rw-r--r--   0        0        0     9846 2023-05-16 00:52:41.060122 corgy-8.1.2/corgy/types/_subclass.py
+-rw-r--r--   0        0        0    35296 2023-05-16 00:52:41.064122 corgy-8.1.2/docs/corgy.md
+-rw-r--r--   0        0        0    11884 2023-05-16 00:52:41.064122 corgy-8.1.2/docs/corgy.types.md
+-rw-r--r--   0        0        0      132 2023-05-16 00:52:41.064122 corgy-8.1.2/docs/index.md
+-rw-r--r--   0        0        0     2679 2023-05-16 00:53:17.384231 corgy-8.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-16 00:52:41.064122 corgy-8.1.2/tests/__init__.py
+-rw-r--r--   0        0        0    90410 2023-05-16 00:52:41.064122 corgy-8.1.2/tests/test_corgy.py
+-rw-r--r--   0        0        0     4240 2023-05-16 00:52:41.064122 corgy-8.1.2/tests/test_corgychecker.py
+-rw-r--r--   0        0        0    16681 2023-05-16 00:52:41.064122 corgy-8.1.2/tests/test_corgyparser.py
+-rw-r--r--   0        0        0      800 2023-05-16 00:52:41.064122 corgy-8.1.2/tests/test_doctests.py
+-rw-r--r--   0        0        0    47095 2023-05-16 00:52:41.064122 corgy-8.1.2/tests/test_helpfmt.py
+-rw-r--r--   0        0        0        0 2023-05-16 00:52:41.064122 corgy-8.1.2/tests/types/__init__.py
+-rw-r--r--   0        0        0      328 2023-05-16 00:52:41.064122 corgy-8.1.2/tests/types/_pklclasses.py
+-rw-r--r--   0        0        0     2002 2023-05-16 00:52:41.064122 corgy-8.1.2/tests/types/_specialtmps.py
+-rw-r--r--   0        0        0     3356 2023-05-16 00:52:41.064122 corgy-8.1.2/tests/types/_test_file.py
+-rw-r--r--   0        0        0     2678 2023-05-16 00:52:41.064122 corgy-8.1.2/tests/types/test_initargs.py
+-rw-r--r--   0        0        0     2496 2023-05-16 00:52:41.064122 corgy-8.1.2/tests/types/test_inputfiles.py
+-rw-r--r--   0        0        0     5443 2023-05-16 00:52:41.064122 corgy-8.1.2/tests/types/test_keyvaluepairs.py
+-rw-r--r--   0        0        0     5122 2023-05-16 00:52:41.064122 corgy-8.1.2/tests/types/test_outputfiles.py
+-rw-r--r--   0        0        0     7082 2023-05-16 00:52:41.064122 corgy-8.1.2/tests/types/test_subclass.py
+-rw-r--r--   0        0        0     5497 1970-01-01 00:00:00.000000 corgy-8.1.2/PKG-INFO
```

### Comparing `corgy-8.1.1/CHANGELOG.md` & `corgy-8.1.2/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # Changelog
 
 All notable changes to this project will be documented in this file. See [standard-version](https://github.com/conventional-changelog/standard-version) for commit guidelines.
 
+### [8.1.2](https://github.com/jayanthkoushik/corgy/compare/v8.1.1...v8.1.2) (2023-05-16)
+
+
+### Bug Fixes
+
+* inherit `corgy_` parameters for `Corgy` sub-classes ([9e87e4d](https://github.com/jayanthkoushik/corgy/commit/9e87e4d5fb0a58c63d0c2e7cd4aaff33ecf47aef))
+
 ### [8.1.1](https://github.com/jayanthkoushik/corgy/compare/v8.1.0...v8.1.1) (2023-04-15)
 
 
 ### Bug Fixes
 
 * fix annotation for `corgy.corgychecker` ([1bf5dba](https://github.com/jayanthkoushik/corgy/commit/1bf5dba17c19ccc7bb3c9c1d76225c1d57dcfd98))
```

### Comparing `corgy-8.1.1/LICENSE` & `corgy-8.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `corgy-8.1.1/README.md` & `corgy-8.1.2/README.md`

 * *Files identical despite different names*

### Comparing `corgy-8.1.1/corgy/_actions.py` & `corgy-8.1.2/corgy/_actions.py`

 * *Files identical despite different names*

### Comparing `corgy-8.1.1/corgy/_corgy.py` & `corgy-8.1.2/corgy/_corgy.py`

 * *Files identical despite different names*

### Comparing `corgy-8.1.1/corgy/_corgychecker.py` & `corgy-8.1.2/corgy/_corgychecker.py`

 * *Files identical despite different names*

### Comparing `corgy-8.1.1/corgy/_corgyparser.py` & `corgy-8.1.2/corgy/_corgyparser.py`

 * *Files identical despite different names*

### Comparing `corgy-8.1.1/corgy/_helpfmt.py` & `corgy-8.1.2/corgy/_helpfmt.py`

 * *Files identical despite different names*

### Comparing `corgy-8.1.1/corgy/_meta.py` & `corgy-8.1.2/corgy/_meta.py`

 * *Files 4% similar despite different names*

```diff
@@ -176,49 +176,27 @@
     and required attributes are stored in `__required`. Attribute value checkers, if
     present, are stored in `__checkers`.
     """
 
     __slots__ = ()
 
     def __new__(cls, name, bases, namespace, **kwds) -> CorgyMeta:
-        try:
-            _make_slots = kwds.pop("corgy_make_slots")
-        except KeyError:
-            _make_slots = True
-
-        if _make_slots:
-            if "__slots__" not in namespace:
-                namespace["__slots__"] = []
-            else:
-                namespace["__slots__"] = list(namespace["__slots__"])
-            namespace["__slots__"].append("__frozen")
-        elif "__slots__" in namespace:
-            raise TypeError(
-                "`__slots__` cannot be defined if `corgy_make_slots` is `False`"
-            )
-
         cls_annotations = namespace.get("__annotations__", {})
         namespace["__annotations__"] = {}
         namespace["__defaults"] = {}
         namespace["__flags"] = {}
         namespace["__parsers"] = {}
         namespace["__helps"] = {}
         namespace["__checkers"] = {}
         namespace["__required"] = set()
 
         # Temp set of not required attributes--to handle inheritance from
         # non-`Corgy` classes.
         _not_required = set()
 
-        # Extract `corgy_freeze_after_init` (default `False`).
-        try:
-            namespace["__freeze_after_init"] = kwds.pop("corgy_freeze_after_init")
-        except KeyError:
-            namespace["__freeze_after_init"] = False
-
         # See if `corgy_track_bases` is specified (default `True`).
         try:
             _track_bases = kwds.pop("corgy_track_bases")
         except KeyError:
             _track_bases = True
         if _track_bases:
             for base in bases:
@@ -228,14 +206,21 @@
                     # `base` is also a `Corgy` class.
                     namespace["__defaults"].update(getattr(base, "__defaults"))
                     namespace["__flags"].update(getattr(base, "__flags"))
                     namespace["__parsers"].update(getattr(base, "__parsers"))
                     namespace["__helps"].update(getattr(base, "__helps"))
                     namespace["__checkers"].update(getattr(base, "__checkers"))
                     namespace["__required"].update(getattr(base, "__required"))
+                    namespace["__make_slots"] = getattr(base, "__make_slots")
+                    namespace["__freeze_after_init"] = getattr(
+                        base, "__freeze_after_init"
+                    )
+                    namespace["__required_by_default"] = getattr(
+                        base, "__required_by_default"
+                    )
                     # Add not required attributes to temp set.
                     _base_required = getattr(base, "__required")
                     for _var_name in _base_annotations:
                         if _var_name not in _base_required:
                             _not_required.add(_var_name)
                 else:
                     # Fetch default values directly from the base.
@@ -246,19 +231,45 @@
                             )
                         except AttributeError:
                             pass
 
         # Add current annotations last, so that they override base values.
         namespace["__annotations__"].update(cls_annotations)
 
-        # See if `corgy_required_by_default` is specified (default `False`).
-        try:
-            _required_by_default = kwds.pop("corgy_required_by_default")
-        except KeyError:
-            _required_by_default = False
+        # Extract `corgy_` class parameters. Values set in `kwds` take preference,
+        # followed by base class values (in reverse order), and finally the parameter
+        # default.
+
+        # Extract `corgy_make_slots` (default `True`)
+        namespace["__make_slots"] = kwds.pop(
+            "corgy_make_slots", namespace.get("__make_slots", True)
+        )
+        _make_slots = namespace["__make_slots"]
+
+        if _make_slots:
+            if "__slots__" not in namespace:
+                namespace["__slots__"] = []
+            else:
+                namespace["__slots__"] = list(namespace["__slots__"])
+            namespace["__slots__"].append("__frozen")
+        elif "__slots__" in namespace:
+            raise TypeError(
+                "`__slots__` cannot be defined if `corgy_make_slots` is `False`"
+            )
+
+        # Extract `corgy_freeze_after_init` (default `False`).
+        namespace["__freeze_after_init"] = kwds.pop(
+            "corgy_freeze_after_init", namespace.get("__freeze_after_init", False)
+        )
+
+        # Extract `corgy_required_by_default` (default `False`).
+        namespace["__required_by_default"] = kwds.pop(
+            "corgy_required_by_default", namespace.get("__required_by_default", False)
+        )
+        _required_by_default = namespace["__required_by_default"]
 
         tempnew = super().__new__(cls, name, bases, namespace)
         type_hints = get_type_hints(tempnew, include_extras=True)
 
         if not type_hints:
             return tempnew
```

### Comparing `corgy-8.1.1/corgy/types/__init__.py` & `corgy-8.1.2/corgy/types/__init__.py`

 * *Files identical despite different names*

### Comparing `corgy-8.1.1/corgy/types/_expand.py` & `corgy-8.1.2/corgy/types/_expand.py`

 * *Files identical despite different names*

### Comparing `corgy-8.1.1/corgy/types/_initargs.py` & `corgy-8.1.2/corgy/types/_initargs.py`

 * *Files identical despite different names*

### Comparing `corgy-8.1.1/corgy/types/_inputfile.py` & `corgy-8.1.2/corgy/types/_inputfile.py`

 * *Files identical despite different names*

### Comparing `corgy-8.1.1/corgy/types/_keyvaluepairs.py` & `corgy-8.1.2/corgy/types/_keyvaluepairs.py`

 * *Files identical despite different names*

### Comparing `corgy-8.1.1/corgy/types/_outputfile.py` & `corgy-8.1.2/corgy/types/_outputfile.py`

 * *Files identical despite different names*

### Comparing `corgy-8.1.1/corgy/types/_subclass.py` & `corgy-8.1.2/corgy/types/_subclass.py`

 * *Files identical despite different names*

### Comparing `corgy-8.1.1/docs/corgy.md` & `corgy-8.1.2/docs/corgy.md`

 * *Files identical despite different names*

### Comparing `corgy-8.1.1/docs/corgy.types.md` & `corgy-8.1.2/docs/corgy.types.md`

 * *Files identical despite different names*

### Comparing `corgy-8.1.1/pyproject.toml` & `corgy-8.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "corgy"
-version = "8.1.1"  # managed by `poetry-dynamic-versioning`
+version = "8.1.2"  # managed by `poetry-dynamic-versioning`
 description = "Elegant data classes"
 authors = ["Jayanth Koushik <mail@jkoushik.me>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/jayanthkoushik/corgy"
 packages = [
   { include = "corgy" },
```

### Comparing `corgy-8.1.1/tests/test_corgy.py` & `corgy-8.1.2/tests/test_corgy.py`

 * *Files 1% similar despite different names*

```diff
@@ -624,14 +624,63 @@
 
         class D3(C, Corgy):
             x: NotRequired[int]
             y: Required[int]
 
         self.assertSetEqual(getattr(D3, "__required"), {"y"})
 
+    def test_corgy_cls_inherits_make_slots(self):
+        class C(Corgy, corgy_make_slots=False):
+            ...
+
+        class D1(C):
+            ...
+
+        class D2(Corgy):
+            ...
+
+        self.assertEqual(getattr(D1, "__make_slots"), False)
+        self.assertEqual(getattr(D2, "__make_slots"), True)
+        self.assertIs(D1.__slots__, Corgy.__slots__)
+        self.assertIsNot(D2.__slots__, Corgy.__slots__)
+
+    def test_corgy_cls_inherits_required_by_default(self):
+        class C(Corgy, corgy_required_by_default=True):
+            ...
+
+        class D1(C):
+            x: int
+
+        class D2(Corgy):
+            x: int
+
+        self.assertEqual(getattr(D1, "__required_by_default"), True)
+        self.assertEqual(getattr(D2, "__required_by_default"), False)
+        with self.assertRaises(ValueError):
+            D1()
+        D2()
+
+    def test_corgy_cls_inherits_freeze_after_init(self):
+        class C(Corgy, corgy_freeze_after_init=True):
+            ...
+
+        class D1(C):
+            x: int
+
+        class D2(Corgy):
+            x: int
+
+        self.assertEqual(getattr(D1, "__freeze_after_init"), True)
+        self.assertEqual(getattr(D2, "__freeze_after_init"), False)
+        d1 = D1(x=1)
+        with self.assertRaises(TypeError):
+            d1.x = 2
+        d2 = D2(x=1)
+        d2.x = 2
+
 
 class TestCorgyTypeChecking(TestCase):
     def test_corgy_cls_type_checks_during_init(self):
         class C(Corgy):
             x: int
 
         with self.assertRaises(ValueError):
```

### Comparing `corgy-8.1.1/tests/test_corgychecker.py` & `corgy-8.1.2/tests/test_corgychecker.py`

 * *Files identical despite different names*

### Comparing `corgy-8.1.1/tests/test_corgyparser.py` & `corgy-8.1.2/tests/test_corgyparser.py`

 * *Files identical despite different names*

### Comparing `corgy-8.1.1/tests/test_doctests.py` & `corgy-8.1.2/tests/test_doctests.py`

 * *Files identical despite different names*

### Comparing `corgy-8.1.1/tests/test_helpfmt.py` & `corgy-8.1.2/tests/test_helpfmt.py`

 * *Files identical despite different names*

### Comparing `corgy-8.1.1/tests/types/_specialtmps.py` & `corgy-8.1.2/tests/types/_specialtmps.py`

 * *Files identical despite different names*

### Comparing `corgy-8.1.1/tests/types/_test_file.py` & `corgy-8.1.2/tests/types/_test_file.py`

 * *Files identical despite different names*

### Comparing `corgy-8.1.1/tests/types/test_initargs.py` & `corgy-8.1.2/tests/types/test_initargs.py`

 * *Files identical despite different names*

### Comparing `corgy-8.1.1/tests/types/test_inputfiles.py` & `corgy-8.1.2/tests/types/test_inputfiles.py`

 * *Files identical despite different names*

### Comparing `corgy-8.1.1/tests/types/test_keyvaluepairs.py` & `corgy-8.1.2/tests/types/test_keyvaluepairs.py`

 * *Files identical despite different names*

### Comparing `corgy-8.1.1/tests/types/test_outputfiles.py` & `corgy-8.1.2/tests/types/test_outputfiles.py`

 * *Files identical despite different names*

### Comparing `corgy-8.1.1/tests/types/test_subclass.py` & `corgy-8.1.2/tests/types/test_subclass.py`

 * *Files identical despite different names*

### Comparing `corgy-8.1.1/PKG-INFO` & `corgy-8.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corgy
-Version: 8.1.1
+Version: 8.1.2
 Summary: Elegant data classes
 Home-page: https://github.com/jayanthkoushik/corgy
 License: MIT
 Keywords: data classes,argparse,argument parsing,command line parsing,cli
 Author: Jayanth Koushik
 Author-email: mail@jkoushik.me
 Requires-Python: >=3.7,<4.0
```

