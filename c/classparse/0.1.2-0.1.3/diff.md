# Comparing `tmp/classparse-0.1.2.tar.gz` & `tmp/classparse-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "classparse-0.1.2.tar", last modified: Mon May 15 23:24:54 2023, max compression
+gzip compressed data, was "classparse-0.1.3.tar", last modified: Mon May 15 23:43:28 2023, max compression
```

## Comparing `classparse-0.1.2.tar` & `classparse-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 liran     (1000) liran     (1000)        0 2023-05-15 23:24:54.088829 classparse-0.1.2/
--rw-rw-r--   0 liran     (1000) liran     (1000)     5224 2023-05-09 12:28:19.000000 classparse-0.1.2/CODE_OF_CONDUCT.md
--rw-rw-r--   0 liran     (1000) liran     (1000)     1501 2023-05-15 23:23:55.000000 classparse-0.1.2/LICENSE
--rw-rw-r--   0 liran     (1000) liran     (1000)       78 2023-05-09 12:28:19.000000 classparse-0.1.2/MANIFEST.in
--rw-rw-r--   0 liran     (1000) liran     (1000)    16361 2023-05-15 23:24:54.088829 classparse-0.1.2/PKG-INFO
--rwxrwxr-x   0 liran     (1000) liran     (1000)    15694 2023-05-15 23:23:55.000000 classparse-0.1.2/README.md
-drwxrwxr-x   0 liran     (1000) liran     (1000)        0 2023-05-15 23:24:54.088829 classparse-0.1.2/classparse/
--rw-rw-r--   0 liran     (1000) liran     (1000)    12692 2023-05-15 23:23:55.000000 classparse-0.1.2/classparse/__init__.py
--rw-rw-r--   0 liran     (1000) liran     (1000)     3140 2023-05-15 23:23:55.000000 classparse-0.1.2/classparse/docs.py
--rw-rw-r--   0 liran     (1000) liran     (1000)     9041 2023-05-15 23:23:55.000000 classparse-0.1.2/classparse/types.py
-drwxrwxr-x   0 liran     (1000) liran     (1000)        0 2023-05-15 23:24:54.088829 classparse-0.1.2/classparse.egg-info/
--rw-rw-r--   0 liran     (1000) liran     (1000)    16361 2023-05-15 23:24:54.000000 classparse-0.1.2/classparse.egg-info/PKG-INFO
--rw-rw-r--   0 liran     (1000) liran     (1000)      294 2023-05-15 23:24:54.000000 classparse-0.1.2/classparse.egg-info/SOURCES.txt
--rw-rw-r--   0 liran     (1000) liran     (1000)        1 2023-05-15 23:24:54.000000 classparse-0.1.2/classparse.egg-info/dependency_links.txt
--rw-rw-r--   0 liran     (1000) liran     (1000)       73 2023-05-15 23:24:54.000000 classparse-0.1.2/classparse.egg-info/requires.txt
--rw-rw-r--   0 liran     (1000) liran     (1000)       11 2023-05-15 23:24:54.000000 classparse-0.1.2/classparse.egg-info/top_level.txt
--rw-rw-r--   0 liran     (1000) liran     (1000)     3134 2023-05-15 23:23:55.000000 classparse-0.1.2/pyproject.toml
--rw-rw-r--   0 liran     (1000) liran     (1000)       38 2023-05-15 23:24:54.088829 classparse-0.1.2/setup.cfg
+drwxrwxr-x   0 liran     (1000) liran     (1000)        0 2023-05-15 23:43:28.732604 classparse-0.1.3/
+-rw-rw-r--   0 liran     (1000) liran     (1000)     5224 2023-05-09 12:28:19.000000 classparse-0.1.3/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 liran     (1000) liran     (1000)     1501 2023-05-15 23:42:57.000000 classparse-0.1.3/LICENSE
+-rw-rw-r--   0 liran     (1000) liran     (1000)       78 2023-05-09 12:28:19.000000 classparse-0.1.3/MANIFEST.in
+-rw-rw-r--   0 liran     (1000) liran     (1000)    16331 2023-05-15 23:43:28.732604 classparse-0.1.3/PKG-INFO
+-rwxrwxr-x   0 liran     (1000) liran     (1000)    15664 2023-05-15 23:42:57.000000 classparse-0.1.3/README.md
+drwxrwxr-x   0 liran     (1000) liran     (1000)        0 2023-05-15 23:43:28.732604 classparse-0.1.3/classparse/
+-rw-rw-r--   0 liran     (1000) liran     (1000)    12692 2023-05-15 23:42:57.000000 classparse-0.1.3/classparse/__init__.py
+-rw-rw-r--   0 liran     (1000) liran     (1000)     3140 2023-05-15 23:42:57.000000 classparse-0.1.3/classparse/docs.py
+-rw-rw-r--   0 liran     (1000) liran     (1000)     9238 2023-05-15 23:42:57.000000 classparse-0.1.3/classparse/types.py
+drwxrwxr-x   0 liran     (1000) liran     (1000)        0 2023-05-15 23:43:28.732604 classparse-0.1.3/classparse.egg-info/
+-rw-rw-r--   0 liran     (1000) liran     (1000)    16331 2023-05-15 23:43:28.000000 classparse-0.1.3/classparse.egg-info/PKG-INFO
+-rw-rw-r--   0 liran     (1000) liran     (1000)      294 2023-05-15 23:43:28.000000 classparse-0.1.3/classparse.egg-info/SOURCES.txt
+-rw-rw-r--   0 liran     (1000) liran     (1000)        1 2023-05-15 23:43:28.000000 classparse-0.1.3/classparse.egg-info/dependency_links.txt
+-rw-rw-r--   0 liran     (1000) liran     (1000)       73 2023-05-15 23:43:28.000000 classparse-0.1.3/classparse.egg-info/requires.txt
+-rw-rw-r--   0 liran     (1000) liran     (1000)       11 2023-05-15 23:43:28.000000 classparse-0.1.3/classparse.egg-info/top_level.txt
+-rw-rw-r--   0 liran     (1000) liran     (1000)     3134 2023-05-15 23:42:57.000000 classparse-0.1.3/pyproject.toml
+-rw-rw-r--   0 liran     (1000) liran     (1000)       38 2023-05-15 23:43:28.732604 classparse-0.1.3/setup.cfg
```

### Comparing `classparse-0.1.2/CODE_OF_CONDUCT.md` & `classparse-0.1.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `classparse-0.1.2/LICENSE` & `classparse-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `classparse-0.1.2/PKG-INFO` & `classparse-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: classparse
-Version: 0.1.2
+Version: 0.1.3
 Summary: Declarative `ArgumentParser` definition with `dataclass` notation.
 Author-email: Liran Funaro <liran.funaro@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/liran-funaro/classparse
 Keywords: argparse,dataclass
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -50,15 +50,15 @@
 
 Declarative `ArgumentParser` definition with `dataclass` notation.
  - No `ArgumentParser` boilerplate code
  - IDE autocompletion and type hints
 
 # Install
 ```bash
-pip install classparse==0.1.2
+pip install classparse==0.1.3
 ```
 
 # Simple Example
 This is a simple example of the most basic usage of this library.
 <!-- embed: examples/simple.py -->
 ```python
 # examples/simple.py
@@ -198,26 +198,26 @@
 <!-- execute: python examples/usage.py --help -->
 ```text
 $ python examples/usage.py --help
 usage: my_program.py [-h] [--int-arg INT_ARG]
                      [--str-enum-choice-arg {Initialize/init,Execute/exec}]
                      [--int-enum-choice-arg {Cat/1,Dog/2}]
                      [--literal-arg {a,b,c}] [--literal-int-arg {1,2,3}]
-                     [--mixed-literal {1,2,3,4,True,Animal.Cat}]
+                     [--mixed-literal {1,2,3,4,True,Cat/1}]
                      [--optional-arg OPTIONAL_ARG]
                      [--just-optional-arg JUST_OPTIONAL_ARG]
                      [--optional-choice-arg {Initialize/init,Execute/exec}]
                      [--union-arg UNION_ARG] [--path-arg PATH_ARG]
                      [-f FLAG_ARG] -r REQUIRED_ARG [--metavar-arg M]
                      [--int-list INT_LIST [INT_LIST ...]]
                      [--int-2-list INT_2_LIST INT_2_LIST]
                      [--multi-type-tuple MULTI_TYPE_TUPLE MULTI_TYPE_TUPLE MULTI_TYPE_TUPLE]
                      [--actions {Initialize/init,Execute/exec} [{Initialize/init,Execute/exec} ...]]
                      [--animals {Cat/1,Dog/2} [{Cat/1,Dog/2} ...]]
-                     [--literal-list {aa,bb,11,22,Animal.Cat} [{aa,bb,11,22,Animal.Cat} ...]]
+                     [--literal-list {aa,bb,11,22,Cat/1} [{aa,bb,11,22,Cat/1} ...]]
                      [--union-list UNION_LIST [UNION_LIST ...]]
                      [--union-with-literal UNION_WITH_LITERAL [UNION_WITH_LITERAL ...]]
                      [--typeless-list TYPELESS_LIST [TYPELESS_LIST ...]]
                      [--typeless-typing-list TYPELESS_TYPING_LIST [TYPELESS_TYPING_LIST ...]]
                      [--none-bool-arg | --no-none-bool-arg]
                      [--true-bool-arg | --no-true-bool-arg]
                      [--false-bool-arg | --no-false-bool-arg]
@@ -244,15 +244,15 @@
                         default=Initialize)
   --int-enum-choice-arg {Cat/1,Dog/2}
                         IntEnum ==> choice argument (type=Animal, default=Cat)
   --literal-arg {a,b,c}
                         Literal ==> choice argument (type=str, default=None)
   --literal-int-arg {1,2,3}
                         Literal's type is automatically inferred (type=int)
-  --mixed-literal {1,2,3,4,True,Animal.Cat}
+  --mixed-literal {1,2,3,4,True,Cat/1}
                         We can mix multiple literal types
                         (type=typing.Literal[1, 2, '3', '4', True,
                         <Animal.Cat: 1>])
   --optional-arg OPTIONAL_ARG
                         Optional can be used for type hinting (type=int)
   --just-optional-arg JUST_OPTIONAL_ARG
                         Bare optional also works (type=None)
@@ -280,15 +280,15 @@
                         float, str])
   --actions {Initialize/init,Execute/exec} [{Initialize/init,Execute/exec} ...]
                         List[Enum] ==> choices with nargs="+" (nargs=+,
                         type=Action)
   --animals {Cat/1,Dog/2} [{Cat/1,Dog/2} ...]
                         List[Enum] ==> choices with nargs="+" (nargs=+,
                         type=Animal)
-  --literal-list {aa,bb,11,22,Animal.Cat} [{aa,bb,11,22,Animal.Cat} ...]
+  --literal-list {aa,bb,11,22,Cat/1} [{aa,bb,11,22,Cat/1} ...]
                         List[Literal] ==> choices with nargs="+"
   --union-list UNION_LIST [UNION_LIST ...]
                         (type: typing.Union[int, float, str, bool])
   --union-with-literal UNION_WITH_LITERAL [UNION_WITH_LITERAL ...]
                         (type: typing.Union[typing.Literal['a', 'b', 1, 2],
                         float, bool])
   --typeless-list TYPELESS_LIST [TYPELESS_LIST ...]
```

### Comparing `classparse-0.1.2/README.md` & `classparse-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 Declarative `ArgumentParser` definition with `dataclass` notation.
  - No `ArgumentParser` boilerplate code
  - IDE autocompletion and type hints
 
 # Install
 ```bash
-pip install classparse==0.1.2
+pip install classparse==0.1.3
 ```
 
 # Simple Example
 This is a simple example of the most basic usage of this library.
 <!-- embed: examples/simple.py -->
 ```python
 # examples/simple.py
@@ -180,26 +180,26 @@
 <!-- execute: python examples/usage.py --help -->
 ```text
 $ python examples/usage.py --help
 usage: my_program.py [-h] [--int-arg INT_ARG]
                      [--str-enum-choice-arg {Initialize/init,Execute/exec}]
                      [--int-enum-choice-arg {Cat/1,Dog/2}]
                      [--literal-arg {a,b,c}] [--literal-int-arg {1,2,3}]
-                     [--mixed-literal {1,2,3,4,True,Animal.Cat}]
+                     [--mixed-literal {1,2,3,4,True,Cat/1}]
                      [--optional-arg OPTIONAL_ARG]
                      [--just-optional-arg JUST_OPTIONAL_ARG]
                      [--optional-choice-arg {Initialize/init,Execute/exec}]
                      [--union-arg UNION_ARG] [--path-arg PATH_ARG]
                      [-f FLAG_ARG] -r REQUIRED_ARG [--metavar-arg M]
                      [--int-list INT_LIST [INT_LIST ...]]
                      [--int-2-list INT_2_LIST INT_2_LIST]
                      [--multi-type-tuple MULTI_TYPE_TUPLE MULTI_TYPE_TUPLE MULTI_TYPE_TUPLE]
                      [--actions {Initialize/init,Execute/exec} [{Initialize/init,Execute/exec} ...]]
                      [--animals {Cat/1,Dog/2} [{Cat/1,Dog/2} ...]]
-                     [--literal-list {aa,bb,11,22,Animal.Cat} [{aa,bb,11,22,Animal.Cat} ...]]
+                     [--literal-list {aa,bb,11,22,Cat/1} [{aa,bb,11,22,Cat/1} ...]]
                      [--union-list UNION_LIST [UNION_LIST ...]]
                      [--union-with-literal UNION_WITH_LITERAL [UNION_WITH_LITERAL ...]]
                      [--typeless-list TYPELESS_LIST [TYPELESS_LIST ...]]
                      [--typeless-typing-list TYPELESS_TYPING_LIST [TYPELESS_TYPING_LIST ...]]
                      [--none-bool-arg | --no-none-bool-arg]
                      [--true-bool-arg | --no-true-bool-arg]
                      [--false-bool-arg | --no-false-bool-arg]
@@ -226,15 +226,15 @@
                         default=Initialize)
   --int-enum-choice-arg {Cat/1,Dog/2}
                         IntEnum ==> choice argument (type=Animal, default=Cat)
   --literal-arg {a,b,c}
                         Literal ==> choice argument (type=str, default=None)
   --literal-int-arg {1,2,3}
                         Literal's type is automatically inferred (type=int)
-  --mixed-literal {1,2,3,4,True,Animal.Cat}
+  --mixed-literal {1,2,3,4,True,Cat/1}
                         We can mix multiple literal types
                         (type=typing.Literal[1, 2, '3', '4', True,
                         <Animal.Cat: 1>])
   --optional-arg OPTIONAL_ARG
                         Optional can be used for type hinting (type=int)
   --just-optional-arg JUST_OPTIONAL_ARG
                         Bare optional also works (type=None)
@@ -262,15 +262,15 @@
                         float, str])
   --actions {Initialize/init,Execute/exec} [{Initialize/init,Execute/exec} ...]
                         List[Enum] ==> choices with nargs="+" (nargs=+,
                         type=Action)
   --animals {Cat/1,Dog/2} [{Cat/1,Dog/2} ...]
                         List[Enum] ==> choices with nargs="+" (nargs=+,
                         type=Animal)
-  --literal-list {aa,bb,11,22,Animal.Cat} [{aa,bb,11,22,Animal.Cat} ...]
+  --literal-list {aa,bb,11,22,Cat/1} [{aa,bb,11,22,Cat/1} ...]
                         List[Literal] ==> choices with nargs="+"
   --union-list UNION_LIST [UNION_LIST ...]
                         (type: typing.Union[int, float, str, bool])
   --union-with-literal UNION_WITH_LITERAL [UNION_WITH_LITERAL ...]
                         (type: typing.Union[typing.Literal['a', 'b', 1, 2],
                         float, bool])
   --typeless-list TYPELESS_LIST [TYPELESS_LIST ...]
```

### Comparing `classparse-0.1.2/classparse/__init__.py` & `classparse-0.1.3/classparse/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     Type,
     Union,
 )
 
 from classparse import docs
 from classparse.types import _update_field_type, _obj_to_yaml_dict, _yaml_dict_to_obj
 
-__version__ = "0.1.2"
+__version__ = "0.1.3"
 NO_ARG = "__no_arg__"
 POS_ARG = "__pos_arg__"
 
 
 def arg(flag=None, default=None, **metadata):
     """
     Allow adding parameters to a named argument.
```

### Comparing `classparse-0.1.2/classparse/docs.py` & `classparse-0.1.3/classparse/docs.py`

 * *Files identical despite different names*

### Comparing `classparse-0.1.2/classparse/types.py` & `classparse-0.1.3/classparse/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,34 +197,43 @@
         a.args["type"] = Union[tuple(a.type_args)]
         return True
     else:
         del a.args["type"]
         return False
 
 
+def _make_metavar(o: Any) -> str:
+    if isinstance(o, enum.Enum):
+        return f"{o.name}/{o.value}"
+    else:
+        return str(o)
+
+
 def _update_enum(a: Argument) -> bool:
     """Enum type is used to define a typed choice argument"""
     assert issubclass(a.type, enum.Enum)
     choices = list(a.type)
     a.args["choices"] = choices
-    a.args["metavar"] = "{%s}" % ",".join([f"{c.name}/{c.value}" for c in choices])
+    a.args["metavar"] = "{%s}" % ",".join(map(_make_metavar, choices))
     cur_default = a.args.get("default", None)
     if isinstance(cur_default, enum.Enum):
         a.args["default"] = cur_default.name
     a.args["type"] = __make_enum_parser(a.type)
     return False
 
 
 def _update_literal(a: Argument) -> bool:
     """Literal type is used to define an untyped choice argument"""
     choices = list(a.type_args)
     assert len(choices) > 0, "'Literal' must have at least one parameter."
     choices_types = set(map(type, a.type_args))
 
     a.args["choices"] = choices
+    a.args["metavar"] = "{%s}" % ",".join(map(_make_metavar, choices))
+
     if len(choices_types) == 1:
         a.args["type"] = list(choices_types)[0]
         return True
     else:
         a.args["type"] = __make_literal_parser(a.type, raise_error=False)
         return False
```

### Comparing `classparse-0.1.2/classparse.egg-info/PKG-INFO` & `classparse-0.1.3/classparse.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: classparse
-Version: 0.1.2
+Version: 0.1.3
 Summary: Declarative `ArgumentParser` definition with `dataclass` notation.
 Author-email: Liran Funaro <liran.funaro@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/liran-funaro/classparse
 Keywords: argparse,dataclass
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -50,15 +50,15 @@
 
 Declarative `ArgumentParser` definition with `dataclass` notation.
  - No `ArgumentParser` boilerplate code
  - IDE autocompletion and type hints
 
 # Install
 ```bash
-pip install classparse==0.1.2
+pip install classparse==0.1.3
 ```
 
 # Simple Example
 This is a simple example of the most basic usage of this library.
 <!-- embed: examples/simple.py -->
 ```python
 # examples/simple.py
@@ -198,26 +198,26 @@
 <!-- execute: python examples/usage.py --help -->
 ```text
 $ python examples/usage.py --help
 usage: my_program.py [-h] [--int-arg INT_ARG]
                      [--str-enum-choice-arg {Initialize/init,Execute/exec}]
                      [--int-enum-choice-arg {Cat/1,Dog/2}]
                      [--literal-arg {a,b,c}] [--literal-int-arg {1,2,3}]
-                     [--mixed-literal {1,2,3,4,True,Animal.Cat}]
+                     [--mixed-literal {1,2,3,4,True,Cat/1}]
                      [--optional-arg OPTIONAL_ARG]
                      [--just-optional-arg JUST_OPTIONAL_ARG]
                      [--optional-choice-arg {Initialize/init,Execute/exec}]
                      [--union-arg UNION_ARG] [--path-arg PATH_ARG]
                      [-f FLAG_ARG] -r REQUIRED_ARG [--metavar-arg M]
                      [--int-list INT_LIST [INT_LIST ...]]
                      [--int-2-list INT_2_LIST INT_2_LIST]
                      [--multi-type-tuple MULTI_TYPE_TUPLE MULTI_TYPE_TUPLE MULTI_TYPE_TUPLE]
                      [--actions {Initialize/init,Execute/exec} [{Initialize/init,Execute/exec} ...]]
                      [--animals {Cat/1,Dog/2} [{Cat/1,Dog/2} ...]]
-                     [--literal-list {aa,bb,11,22,Animal.Cat} [{aa,bb,11,22,Animal.Cat} ...]]
+                     [--literal-list {aa,bb,11,22,Cat/1} [{aa,bb,11,22,Cat/1} ...]]
                      [--union-list UNION_LIST [UNION_LIST ...]]
                      [--union-with-literal UNION_WITH_LITERAL [UNION_WITH_LITERAL ...]]
                      [--typeless-list TYPELESS_LIST [TYPELESS_LIST ...]]
                      [--typeless-typing-list TYPELESS_TYPING_LIST [TYPELESS_TYPING_LIST ...]]
                      [--none-bool-arg | --no-none-bool-arg]
                      [--true-bool-arg | --no-true-bool-arg]
                      [--false-bool-arg | --no-false-bool-arg]
@@ -244,15 +244,15 @@
                         default=Initialize)
   --int-enum-choice-arg {Cat/1,Dog/2}
                         IntEnum ==> choice argument (type=Animal, default=Cat)
   --literal-arg {a,b,c}
                         Literal ==> choice argument (type=str, default=None)
   --literal-int-arg {1,2,3}
                         Literal's type is automatically inferred (type=int)
-  --mixed-literal {1,2,3,4,True,Animal.Cat}
+  --mixed-literal {1,2,3,4,True,Cat/1}
                         We can mix multiple literal types
                         (type=typing.Literal[1, 2, '3', '4', True,
                         <Animal.Cat: 1>])
   --optional-arg OPTIONAL_ARG
                         Optional can be used for type hinting (type=int)
   --just-optional-arg JUST_OPTIONAL_ARG
                         Bare optional also works (type=None)
@@ -280,15 +280,15 @@
                         float, str])
   --actions {Initialize/init,Execute/exec} [{Initialize/init,Execute/exec} ...]
                         List[Enum] ==> choices with nargs="+" (nargs=+,
                         type=Action)
   --animals {Cat/1,Dog/2} [{Cat/1,Dog/2} ...]
                         List[Enum] ==> choices with nargs="+" (nargs=+,
                         type=Animal)
-  --literal-list {aa,bb,11,22,Animal.Cat} [{aa,bb,11,22,Animal.Cat} ...]
+  --literal-list {aa,bb,11,22,Cat/1} [{aa,bb,11,22,Cat/1} ...]
                         List[Literal] ==> choices with nargs="+"
   --union-list UNION_LIST [UNION_LIST ...]
                         (type: typing.Union[int, float, str, bool])
   --union-with-literal UNION_WITH_LITERAL [UNION_WITH_LITERAL ...]
                         (type: typing.Union[typing.Literal['a', 'b', 1, 2],
                         float, bool])
   --typeless-list TYPELESS_LIST [TYPELESS_LIST ...]
```

### Comparing `classparse-0.1.2/pyproject.toml` & `classparse-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "classparse"
-version = "0.1.2"
+version = "0.1.3"
 description = "Declarative `ArgumentParser` definition with `dataclass` notation."
 readme = "README.md"
 authors = [{ name = "Liran Funaro", email = "liran.funaro@gmail.com" }]
 license = { text = "BSD-3-Clause" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
@@ -51,15 +51,15 @@
 [project.optional-dependencies]
 dev = ["bumpver", "black", "flake8", "pip-tools", "pytest", "pytest-cov", "coveralls"]
 
 [project.urls]
 Homepage = "https://github.com/liran-funaro/classparse"
 
 [tool.bumpver]
-current_version = "0.1.2"
+current_version = "0.1.3"
 version_pattern = "MAJOR.MINOR.PATCH[-TAG]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

