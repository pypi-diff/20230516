# Comparing `tmp/classparse-0.1.1.tar.gz` & `tmp/classparse-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "classparse-0.1.1.tar", last modified: Sun May 14 15:09:42 2023, max compression
+gzip compressed data, was "classparse-0.1.2.tar", last modified: Mon May 15 23:24:54 2023, max compression
```

## Comparing `classparse-0.1.1.tar` & `classparse-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 liran     (1000) liran     (1000)        0 2023-05-14 15:09:42.025274 classparse-0.1.1/
--rw-rw-r--   0 liran     (1000) liran     (1000)     5224 2023-05-09 12:28:19.000000 classparse-0.1.1/CODE_OF_CONDUCT.md
--rw-rw-r--   0 liran     (1000) liran     (1000)     1501 2023-05-14 15:07:13.000000 classparse-0.1.1/LICENSE
--rw-rw-r--   0 liran     (1000) liran     (1000)       78 2023-05-09 12:28:19.000000 classparse-0.1.1/MANIFEST.in
--rw-rw-r--   0 liran     (1000) liran     (1000)    15873 2023-05-14 15:09:42.025274 classparse-0.1.1/PKG-INFO
--rwxrwxr-x   0 liran     (1000) liran     (1000)    15206 2023-05-14 15:07:13.000000 classparse-0.1.1/README.md
-drwxrwxr-x   0 liran     (1000) liran     (1000)        0 2023-05-14 15:09:42.025274 classparse-0.1.1/classparse/
--rw-rw-r--   0 liran     (1000) liran     (1000)    12772 2023-05-14 15:07:13.000000 classparse-0.1.1/classparse/__init__.py
--rw-rw-r--   0 liran     (1000) liran     (1000)     3140 2023-05-14 15:07:13.000000 classparse-0.1.1/classparse/docs.py
--rw-rw-r--   0 liran     (1000) liran     (1000)     8197 2023-05-14 15:07:13.000000 classparse-0.1.1/classparse/types.py
-drwxrwxr-x   0 liran     (1000) liran     (1000)        0 2023-05-14 15:09:42.025274 classparse-0.1.1/classparse.egg-info/
--rw-rw-r--   0 liran     (1000) liran     (1000)    15873 2023-05-14 15:09:41.000000 classparse-0.1.1/classparse.egg-info/PKG-INFO
--rw-rw-r--   0 liran     (1000) liran     (1000)      294 2023-05-14 15:09:41.000000 classparse-0.1.1/classparse.egg-info/SOURCES.txt
--rw-rw-r--   0 liran     (1000) liran     (1000)        1 2023-05-14 15:09:41.000000 classparse-0.1.1/classparse.egg-info/dependency_links.txt
--rw-rw-r--   0 liran     (1000) liran     (1000)       73 2023-05-14 15:09:41.000000 classparse-0.1.1/classparse.egg-info/requires.txt
--rw-rw-r--   0 liran     (1000) liran     (1000)       11 2023-05-14 15:09:41.000000 classparse-0.1.1/classparse.egg-info/top_level.txt
--rw-rw-r--   0 liran     (1000) liran     (1000)     3133 2023-05-14 15:07:13.000000 classparse-0.1.1/pyproject.toml
--rw-rw-r--   0 liran     (1000) liran     (1000)       38 2023-05-14 15:09:42.025274 classparse-0.1.1/setup.cfg
+drwxrwxr-x   0 liran     (1000) liran     (1000)        0 2023-05-15 23:24:54.088829 classparse-0.1.2/
+-rw-rw-r--   0 liran     (1000) liran     (1000)     5224 2023-05-09 12:28:19.000000 classparse-0.1.2/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 liran     (1000) liran     (1000)     1501 2023-05-15 23:23:55.000000 classparse-0.1.2/LICENSE
+-rw-rw-r--   0 liran     (1000) liran     (1000)       78 2023-05-09 12:28:19.000000 classparse-0.1.2/MANIFEST.in
+-rw-rw-r--   0 liran     (1000) liran     (1000)    16361 2023-05-15 23:24:54.088829 classparse-0.1.2/PKG-INFO
+-rwxrwxr-x   0 liran     (1000) liran     (1000)    15694 2023-05-15 23:23:55.000000 classparse-0.1.2/README.md
+drwxrwxr-x   0 liran     (1000) liran     (1000)        0 2023-05-15 23:24:54.088829 classparse-0.1.2/classparse/
+-rw-rw-r--   0 liran     (1000) liran     (1000)    12692 2023-05-15 23:23:55.000000 classparse-0.1.2/classparse/__init__.py
+-rw-rw-r--   0 liran     (1000) liran     (1000)     3140 2023-05-15 23:23:55.000000 classparse-0.1.2/classparse/docs.py
+-rw-rw-r--   0 liran     (1000) liran     (1000)     9041 2023-05-15 23:23:55.000000 classparse-0.1.2/classparse/types.py
+drwxrwxr-x   0 liran     (1000) liran     (1000)        0 2023-05-15 23:24:54.088829 classparse-0.1.2/classparse.egg-info/
+-rw-rw-r--   0 liran     (1000) liran     (1000)    16361 2023-05-15 23:24:54.000000 classparse-0.1.2/classparse.egg-info/PKG-INFO
+-rw-rw-r--   0 liran     (1000) liran     (1000)      294 2023-05-15 23:24:54.000000 classparse-0.1.2/classparse.egg-info/SOURCES.txt
+-rw-rw-r--   0 liran     (1000) liran     (1000)        1 2023-05-15 23:24:54.000000 classparse-0.1.2/classparse.egg-info/dependency_links.txt
+-rw-rw-r--   0 liran     (1000) liran     (1000)       73 2023-05-15 23:24:54.000000 classparse-0.1.2/classparse.egg-info/requires.txt
+-rw-rw-r--   0 liran     (1000) liran     (1000)       11 2023-05-15 23:24:54.000000 classparse-0.1.2/classparse.egg-info/top_level.txt
+-rw-rw-r--   0 liran     (1000) liran     (1000)     3134 2023-05-15 23:23:55.000000 classparse-0.1.2/pyproject.toml
+-rw-rw-r--   0 liran     (1000) liran     (1000)       38 2023-05-15 23:24:54.088829 classparse-0.1.2/setup.cfg
```

### Comparing `classparse-0.1.1/CODE_OF_CONDUCT.md` & `classparse-0.1.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `classparse-0.1.1/LICENSE` & `classparse-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `classparse-0.1.1/PKG-INFO` & `classparse-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: classparse
-Version: 0.1.1
-Summary: Declarative `ArgumentParser` definition with `dataclass` notation.
-Author-email: Liran Funaro <liran.funaro@gmail.com>
-License: BSD-3-Clause
-Project-URL: Homepage, https://github.com/liran-funaro/classparse
-Keywords: argparse,dataclass
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 <!---
 Copyright (c) 2023-2023, Liran Funaro.
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 1. Redistributions of source code must retain the above copyright
@@ -50,15 +32,15 @@
 
 Declarative `ArgumentParser` definition with `dataclass` notation.
  - No `ArgumentParser` boilerplate code
  - IDE autocompletion and type hints
 
 # Install
 ```bash
-pip install git+https://github.com/liran-funaro/classparse@0.1.1
+pip install classparse==0.1.2
 ```
 
 # Simple Example
 This is a simple example of the most basic usage of this library.
 <!-- embed: examples/simple.py -->
 ```python
 # examples/simple.py
@@ -122,15 +104,15 @@
     prog="my_program.py",  # Keyword arguments are passed to the parser init.
     default_argument_args=dict(help="(type: %(type)s)"),  # Set default arguments for each call of add_argument().
 )
 @dataclass(frozen=True)
 class AllOptions:
     """
     Class doc string ==> parser description.
-    The fields' inline comment ==> argument's help.
+    The fields' inline/above comment ==> argument's help.
     """
 
     pos_arg_1: str  # Field with no explicit default ==> positional arguments (default=%(default)s)
     pos_arg_2: int = pos_arg(
         5,
         nargs="?",
         help=(
@@ -140,15 +122,15 @@
         ),
     )  # When the help field is specified explicitly, the inline comment is ignored
     int_arg: int = 1  # Field's type and default are applied to the parser (type=%(type)s, default=%(default)s)
     str_enum_choice_arg: Action = Action.Initialize  # StrEnum ==> choice argument (type=%(type)s, default=%(default)s)
     int_enum_choice_arg: Animal = Animal.Cat  # IntEnum ==> choice argument (type=%(type)s, default=%(default)s)
     literal_arg: Literal["a", "b", "c"] = None  # Literal ==> choice argument (type=%(type)s, default=%(default)s)
     literal_int_arg: Literal[1, 2, 3] = None  # Literal's type is automatically inferred (type=%(type)s)
-    mixed_literal: Literal[1, 2, "3", "4", True] = None  # We can mix multiple literal types (type=%(type)s)
+    mixed_literal: Literal[1, 2, "3", "4", True, Animal.Cat] = None  # We can mix multiple literal types (type=%(type)s)
     optional_arg: Optional[int] = None  # Optional can be used for type hinting (type=%(type)s)
     just_optional_arg: Optional = None  # Bare optional also works (type=%(type)s)
     optional_choice_arg: Optional[Action] = None  # Nested types are supported (type=%(type)s)
     union_arg: Union[int, float, bool] = None  # Tries to convert to type in order until first success (type=%(type)s)
     path_arg: Path = None
     flag_arg: int = arg(
         "-f",
@@ -162,16 +144,17 @@
     required_arg: float = arg("-r", required=True)  # E.g., required=%(required)s
     metavar_arg: str = arg(metavar="M")  # E.g., metavar=%(metavar)s
     int_list: List[int] = (1,)  # List type hint ==> nargs="+" (type=%(type)s)
     int_2_list: Tuple[int, int] = (1, 2)  # Tuple type hint ==> nargs=<tuple length> (nargs=%(nargs)s, type=%(type)s)
     multi_type_tuple: Tuple[int, float, str] = (1, 1e-3, "a")  # We can use multiple types (type=%(type)s)
     actions: List[Action] = ()  # List[Enum] ==> choices with nargs="+" (nargs=%(nargs)s, type=%(type)s)
     animals: List[Animal] = ()  # List[Enum] ==> choices with nargs="+" (nargs=%(nargs)s, type=%(type)s)
-    literal_list: List[Literal["aa", "bb"]] = ("aa",)  # List[Literal] ==> choices with nargs="+"
+    literal_list: List[Literal["aa", "bb", 11, 22, Animal.Cat]] = ("aa",)  # List[Literal] ==> choices with nargs="+"
     union_list: List[Union[int, float, str, bool]] = ()
+    union_with_literal: List[Union[Literal["a", "b", 1, 2], float, bool]] = ()
     typeless_list: list = ()  # If list type is unspecified, then it uses argparse default (type=%(type)s)
     typeless_typing_list: List = ()  # typing.List or list are supported
     none_bool_arg: bool = None  # boolean args ==> argparse.BooleanOptionalAction (type=%(type)s)
     true_bool_arg: bool = True  # We can set any default value
     false_bool_arg: bool = False
     complex_arg: complex = complex(1, -1)
 
@@ -197,36 +180,37 @@
 <!-- execute: python examples/usage.py --help -->
 ```text
 $ python examples/usage.py --help
 usage: my_program.py [-h] [--int-arg INT_ARG]
                      [--str-enum-choice-arg {Initialize/init,Execute/exec}]
                      [--int-enum-choice-arg {Cat/1,Dog/2}]
                      [--literal-arg {a,b,c}] [--literal-int-arg {1,2,3}]
-                     [--mixed-literal {1,2,3,4,True}]
+                     [--mixed-literal {1,2,3,4,True,Animal.Cat}]
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
-                     [--literal-list {aa,bb} [{aa,bb} ...]]
+                     [--literal-list {aa,bb,11,22,Animal.Cat} [{aa,bb,11,22,Animal.Cat} ...]]
                      [--union-list UNION_LIST [UNION_LIST ...]]
+                     [--union-with-literal UNION_WITH_LITERAL [UNION_WITH_LITERAL ...]]
                      [--typeless-list TYPELESS_LIST [TYPELESS_LIST ...]]
                      [--typeless-typing-list TYPELESS_TYPING_LIST [TYPELESS_TYPING_LIST ...]]
                      [--none-bool-arg | --no-none-bool-arg]
                      [--true-bool-arg | --no-true-bool-arg]
                      [--false-bool-arg | --no-false-bool-arg]
                      [--complex-arg COMPLEX_ARG] [-s SHOW [SHOW ...]]
                      pos-arg-1 [pos-arg-2]
 
-Class doc string ==> parser description. The fields' inline comment ==>
+Class doc string ==> parser description. The fields' inline/above comment ==>
 argument's help.
 
 positional arguments:
   pos-arg-1             Field with no explicit default ==> positional
                         arguments (default=None)
   pos-arg-2             pos_arg() is a wrapper around dataclasses.field().The
                         first argument (optional) is the argument default
@@ -242,17 +226,18 @@
                         default=Initialize)
   --int-enum-choice-arg {Cat/1,Dog/2}
                         IntEnum ==> choice argument (type=Animal, default=Cat)
   --literal-arg {a,b,c}
                         Literal ==> choice argument (type=str, default=None)
   --literal-int-arg {1,2,3}
                         Literal's type is automatically inferred (type=int)
-  --mixed-literal {1,2,3,4,True}
+  --mixed-literal {1,2,3,4,True,Animal.Cat}
                         We can mix multiple literal types
-                        (type=typing.Literal[1, 2, '3', '4', True])
+                        (type=typing.Literal[1, 2, '3', '4', True,
+                        <Animal.Cat: 1>])
   --optional-arg OPTIONAL_ARG
                         Optional can be used for type hinting (type=int)
   --just-optional-arg JUST_OPTIONAL_ARG
                         Bare optional also works (type=None)
   --optional-choice-arg {Initialize/init,Execute/exec}
                         Nested types are supported (type=Action)
   --union-arg UNION_ARG
@@ -277,18 +262,21 @@
                         float, str])
   --actions {Initialize/init,Execute/exec} [{Initialize/init,Execute/exec} ...]
                         List[Enum] ==> choices with nargs="+" (nargs=+,
                         type=Action)
   --animals {Cat/1,Dog/2} [{Cat/1,Dog/2} ...]
                         List[Enum] ==> choices with nargs="+" (nargs=+,
                         type=Animal)
-  --literal-list {aa,bb} [{aa,bb} ...]
+  --literal-list {aa,bb,11,22,Animal.Cat} [{aa,bb,11,22,Animal.Cat} ...]
                         List[Literal] ==> choices with nargs="+"
   --union-list UNION_LIST [UNION_LIST ...]
                         (type: typing.Union[int, float, str, bool])
+  --union-with-literal UNION_WITH_LITERAL [UNION_WITH_LITERAL ...]
+                        (type: typing.Union[typing.Literal['a', 'b', 1, 2],
+                        float, bool])
   --typeless-list TYPELESS_LIST [TYPELESS_LIST ...]
                         If list type is unspecified, then it uses argparse
                         default (type=None)
   --typeless-typing-list TYPELESS_TYPING_LIST [TYPELESS_TYPING_LIST ...]
                         typing.List or list are supported
   --none-bool-arg, --no-none-bool-arg
                         boolean args ==> argparse.BooleanOptionalAction
```

### Comparing `classparse-0.1.1/README.md` & `classparse-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: classparse
+Version: 0.1.2
+Summary: Declarative `ArgumentParser` definition with `dataclass` notation.
+Author-email: Liran Funaro <liran.funaro@gmail.com>
+License: BSD-3-Clause
+Project-URL: Homepage, https://github.com/liran-funaro/classparse
+Keywords: argparse,dataclass
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 <!---
 Copyright (c) 2023-2023, Liran Funaro.
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 1. Redistributions of source code must retain the above copyright
@@ -32,15 +50,15 @@
 
 Declarative `ArgumentParser` definition with `dataclass` notation.
  - No `ArgumentParser` boilerplate code
  - IDE autocompletion and type hints
 
 # Install
 ```bash
-pip install git+https://github.com/liran-funaro/classparse@0.1.1
+pip install classparse==0.1.2
 ```
 
 # Simple Example
 This is a simple example of the most basic usage of this library.
 <!-- embed: examples/simple.py -->
 ```python
 # examples/simple.py
@@ -104,15 +122,15 @@
     prog="my_program.py",  # Keyword arguments are passed to the parser init.
     default_argument_args=dict(help="(type: %(type)s)"),  # Set default arguments for each call of add_argument().
 )
 @dataclass(frozen=True)
 class AllOptions:
     """
     Class doc string ==> parser description.
-    The fields' inline comment ==> argument's help.
+    The fields' inline/above comment ==> argument's help.
     """
 
     pos_arg_1: str  # Field with no explicit default ==> positional arguments (default=%(default)s)
     pos_arg_2: int = pos_arg(
         5,
         nargs="?",
         help=(
@@ -122,15 +140,15 @@
         ),
     )  # When the help field is specified explicitly, the inline comment is ignored
     int_arg: int = 1  # Field's type and default are applied to the parser (type=%(type)s, default=%(default)s)
     str_enum_choice_arg: Action = Action.Initialize  # StrEnum ==> choice argument (type=%(type)s, default=%(default)s)
     int_enum_choice_arg: Animal = Animal.Cat  # IntEnum ==> choice argument (type=%(type)s, default=%(default)s)
     literal_arg: Literal["a", "b", "c"] = None  # Literal ==> choice argument (type=%(type)s, default=%(default)s)
     literal_int_arg: Literal[1, 2, 3] = None  # Literal's type is automatically inferred (type=%(type)s)
-    mixed_literal: Literal[1, 2, "3", "4", True] = None  # We can mix multiple literal types (type=%(type)s)
+    mixed_literal: Literal[1, 2, "3", "4", True, Animal.Cat] = None  # We can mix multiple literal types (type=%(type)s)
     optional_arg: Optional[int] = None  # Optional can be used for type hinting (type=%(type)s)
     just_optional_arg: Optional = None  # Bare optional also works (type=%(type)s)
     optional_choice_arg: Optional[Action] = None  # Nested types are supported (type=%(type)s)
     union_arg: Union[int, float, bool] = None  # Tries to convert to type in order until first success (type=%(type)s)
     path_arg: Path = None
     flag_arg: int = arg(
         "-f",
@@ -144,16 +162,17 @@
     required_arg: float = arg("-r", required=True)  # E.g., required=%(required)s
     metavar_arg: str = arg(metavar="M")  # E.g., metavar=%(metavar)s
     int_list: List[int] = (1,)  # List type hint ==> nargs="+" (type=%(type)s)
     int_2_list: Tuple[int, int] = (1, 2)  # Tuple type hint ==> nargs=<tuple length> (nargs=%(nargs)s, type=%(type)s)
     multi_type_tuple: Tuple[int, float, str] = (1, 1e-3, "a")  # We can use multiple types (type=%(type)s)
     actions: List[Action] = ()  # List[Enum] ==> choices with nargs="+" (nargs=%(nargs)s, type=%(type)s)
     animals: List[Animal] = ()  # List[Enum] ==> choices with nargs="+" (nargs=%(nargs)s, type=%(type)s)
-    literal_list: List[Literal["aa", "bb"]] = ("aa",)  # List[Literal] ==> choices with nargs="+"
+    literal_list: List[Literal["aa", "bb", 11, 22, Animal.Cat]] = ("aa",)  # List[Literal] ==> choices with nargs="+"
     union_list: List[Union[int, float, str, bool]] = ()
+    union_with_literal: List[Union[Literal["a", "b", 1, 2], float, bool]] = ()
     typeless_list: list = ()  # If list type is unspecified, then it uses argparse default (type=%(type)s)
     typeless_typing_list: List = ()  # typing.List or list are supported
     none_bool_arg: bool = None  # boolean args ==> argparse.BooleanOptionalAction (type=%(type)s)
     true_bool_arg: bool = True  # We can set any default value
     false_bool_arg: bool = False
     complex_arg: complex = complex(1, -1)
 
@@ -179,36 +198,37 @@
 <!-- execute: python examples/usage.py --help -->
 ```text
 $ python examples/usage.py --help
 usage: my_program.py [-h] [--int-arg INT_ARG]
                      [--str-enum-choice-arg {Initialize/init,Execute/exec}]
                      [--int-enum-choice-arg {Cat/1,Dog/2}]
                      [--literal-arg {a,b,c}] [--literal-int-arg {1,2,3}]
-                     [--mixed-literal {1,2,3,4,True}]
+                     [--mixed-literal {1,2,3,4,True,Animal.Cat}]
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
-                     [--literal-list {aa,bb} [{aa,bb} ...]]
+                     [--literal-list {aa,bb,11,22,Animal.Cat} [{aa,bb,11,22,Animal.Cat} ...]]
                      [--union-list UNION_LIST [UNION_LIST ...]]
+                     [--union-with-literal UNION_WITH_LITERAL [UNION_WITH_LITERAL ...]]
                      [--typeless-list TYPELESS_LIST [TYPELESS_LIST ...]]
                      [--typeless-typing-list TYPELESS_TYPING_LIST [TYPELESS_TYPING_LIST ...]]
                      [--none-bool-arg | --no-none-bool-arg]
                      [--true-bool-arg | --no-true-bool-arg]
                      [--false-bool-arg | --no-false-bool-arg]
                      [--complex-arg COMPLEX_ARG] [-s SHOW [SHOW ...]]
                      pos-arg-1 [pos-arg-2]
 
-Class doc string ==> parser description. The fields' inline comment ==>
+Class doc string ==> parser description. The fields' inline/above comment ==>
 argument's help.
 
 positional arguments:
   pos-arg-1             Field with no explicit default ==> positional
                         arguments (default=None)
   pos-arg-2             pos_arg() is a wrapper around dataclasses.field().The
                         first argument (optional) is the argument default
@@ -224,17 +244,18 @@
                         default=Initialize)
   --int-enum-choice-arg {Cat/1,Dog/2}
                         IntEnum ==> choice argument (type=Animal, default=Cat)
   --literal-arg {a,b,c}
                         Literal ==> choice argument (type=str, default=None)
   --literal-int-arg {1,2,3}
                         Literal's type is automatically inferred (type=int)
-  --mixed-literal {1,2,3,4,True}
+  --mixed-literal {1,2,3,4,True,Animal.Cat}
                         We can mix multiple literal types
-                        (type=typing.Literal[1, 2, '3', '4', True])
+                        (type=typing.Literal[1, 2, '3', '4', True,
+                        <Animal.Cat: 1>])
   --optional-arg OPTIONAL_ARG
                         Optional can be used for type hinting (type=int)
   --just-optional-arg JUST_OPTIONAL_ARG
                         Bare optional also works (type=None)
   --optional-choice-arg {Initialize/init,Execute/exec}
                         Nested types are supported (type=Action)
   --union-arg UNION_ARG
@@ -259,18 +280,21 @@
                         float, str])
   --actions {Initialize/init,Execute/exec} [{Initialize/init,Execute/exec} ...]
                         List[Enum] ==> choices with nargs="+" (nargs=+,
                         type=Action)
   --animals {Cat/1,Dog/2} [{Cat/1,Dog/2} ...]
                         List[Enum] ==> choices with nargs="+" (nargs=+,
                         type=Animal)
-  --literal-list {aa,bb} [{aa,bb} ...]
+  --literal-list {aa,bb,11,22,Animal.Cat} [{aa,bb,11,22,Animal.Cat} ...]
                         List[Literal] ==> choices with nargs="+"
   --union-list UNION_LIST [UNION_LIST ...]
                         (type: typing.Union[int, float, str, bool])
+  --union-with-literal UNION_WITH_LITERAL [UNION_WITH_LITERAL ...]
+                        (type: typing.Union[typing.Literal['a', 'b', 1, 2],
+                        float, bool])
   --typeless-list TYPELESS_LIST [TYPELESS_LIST ...]
                         If list type is unspecified, then it uses argparse
                         default (type=None)
   --typeless-typing-list TYPELESS_TYPING_LIST [TYPELESS_TYPING_LIST ...]
                         typing.List or list are supported
   --none-bool-arg, --no-none-bool-arg
                         boolean args ==> argparse.BooleanOptionalAction
```

### Comparing `classparse-0.1.1/classparse/__init__.py` & `classparse-0.1.2/classparse/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,41 +25,37 @@
 CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
 SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
 INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
 CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 POSSIBILITY OF SUCH DAMAGE.
 """
+import yaml
 import argparse
 import dataclasses
-import enum
 import functools
 import typing
 from dataclasses import dataclass
 from types import MethodType
 from typing import (
     Any,
-    Callable,
     Dict,
     Iterable,
     List,
     Optional,
     Sequence,
     Tuple,
     Type,
     Union,
 )
 
-import yaml
-
 from classparse import docs
-from classparse.types import _update_field_type
-
-__version__ = "0.1.1"
+from classparse.types import _update_field_type, _obj_to_yaml_dict, _yaml_dict_to_obj
 
+__version__ = "0.1.2"
 NO_ARG = "__no_arg__"
 POS_ARG = "__pos_arg__"
 
 
 def arg(flag=None, default=None, **metadata):
     """
     Allow adding parameters to a named argument.
@@ -99,48 +95,28 @@
     arg_name = to_arg_name(arg_name)
     if positional:
         assert flag is None, "Flag is not supported for positional argument"
         return [arg_name]
     return filter(None, [flag, f"--{arg_name}"])
 
 
-def _obj_to_yaml_dict(o):
-    if isinstance(o, dict):
-        return {k: _obj_to_yaml_dict(v) for k, v in o.items()}
-    if isinstance(o, (tuple, list)):
-        return [_obj_to_yaml_dict(v) for v in o]
-    if isinstance(o, enum.Enum):
-        return o.name
-    elif isinstance(o, (int, float, bool)) or o is None:
-        return o
-    return str(o)
-
-
-def _yaml_dict_to_obj(o, value_type: Union[Callable, Dict[str, Callable]]):
-    if isinstance(o, dict):
-        return {k: _yaml_dict_to_obj(v, value_type.get(k, None)) for k, v in o.items()}
-    if isinstance(o, (tuple, list)):
-        return [_yaml_dict_to_obj(v, value_type) for v in o]
-
-    if callable(value_type) and isinstance(o, str):
-        return value_type(o)
-    else:
-        return o
-
-
 class DataclassParser(typing.Protocol):  # pragma: no cover
     @classmethod
     def get_vars(cls) -> Dict[str, Any]:
         ...
 
     @classmethod
     def asdict(cls) -> Dict[str, Any]:
         ...
 
     @classmethod
+    def from_dict(cls, namespace: Dict[str, Any]) -> "DataclassParser":
+        ...
+
+    @classmethod
     def dump_yaml(cls, stream=None, **kwargs) -> str:
         ...
 
     @classmethod
     def load_yaml(cls, stream) -> "DataclassParser":
         ...
 
@@ -198,21 +174,24 @@
         parser_args.setdefault("description", cls.__doc__)
         self.parser_args = parser_args
 
         self.docs = docs.get_argument_docs(cls)
         self.args = []
 
         for field in dataclasses.fields(cls):
-            self.add_argument_from_field(field)
+            self._add_argument_from_field(field)
 
-        self.all_types = {name: kwargs.get("type", None) for name, _, kwargs in self.args}
-        self.all_defaults = {name: kwargs.get("default", None) for name, _, kwargs in self.args}
+        self.all_types = self._get_all_kwarg("type")
+        self.all_defaults = self._get_all_kwarg("default")
         self.main_parser = self.make()
 
-    def add_argument_from_field(self, field: dataclasses.Field):
+    def _get_all_kwarg(self, arg_name):
+        return {name: kwargs.get(arg_name, None) for name, _, kwargs in self.args}
+
+    def _add_argument_from_field(self, field: dataclasses.Field):
         # Arguments precedence: field.metadata, default_argument_args
         kwargs = dict(self.default_argument_args)
         kwargs.update(field.metadata)
         is_no_arg = kwargs.pop(NO_ARG, False)
         if is_no_arg:
             return
 
@@ -252,25 +231,36 @@
             if name in default_values:
                 kwargs = dict(kwargs, default=default_values[name])
             parser.add_argument(*args, **kwargs)
 
         return parser
 
     def cast_to_class(self, namespace) -> dataclass:
-        return self.cls(**{to_var_name(k): v for k, v in vars(namespace).items()})
+        if not isinstance(namespace, dict):
+            namespace = vars(namespace)
+        return self.cls(**{to_var_name(k): v for k, v in namespace.items()})
 
     def get_vars(self, instance_or_cls) -> Dict[str, Any]:
         if isinstance(instance_or_cls, type):
             return dict(self.all_defaults)
         else:
             return dataclasses.asdict(instance_or_cls)
 
     def asdict(self, instance_or_cls) -> Dict[str, Any]:
         return {to_arg_name(k): v for k, v in self.get_vars(instance_or_cls).items()}
 
+    def from_dict(self, instance_or_cls, namespace: Union[Any, Dict[str, Any]]) -> DataclassParser:
+        if not isinstance(namespace, dict):
+            namespace = vars(namespace)
+
+        defaults = self.get_vars(instance_or_cls)
+        iter_namespace = ((to_var_name(k), v) for k, v in namespace.items())
+        defaults.update({k: v for k, v in iter_namespace if k in defaults})
+        return self.cast_to_class(defaults)
+
     def dump_yaml(self, instance_or_cls, stream=None, **kwargs) -> str:
         cur_vars = self.get_vars(instance_or_cls)
         cur_vars = _obj_to_yaml_dict(cur_vars)
         return yaml.safe_dump(cur_vars, stream=stream, **kwargs)
 
     def load_yaml(self, instance_or_cls, stream) -> DataclassParser:
         cur_vars = self.get_vars(instance_or_cls)
```

### Comparing `classparse-0.1.1/classparse/docs.py` & `classparse-0.1.2/classparse/docs.py`

 * *Files identical despite different names*

### Comparing `classparse-0.1.1/classparse/types.py` & `classparse-0.1.2/classparse/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 POSSIBILITY OF SUCH DAMAGE.
 """
 import argparse
 import enum
 import functools
 import itertools
 import typing
-from typing import Any, Dict, List, Literal, Optional, Tuple, Type, Union
+from typing import Any, Dict, List, Literal, Optional, Tuple, Type, Union, Callable
 
 _TYPE_RECURSION_LIMIT = 1024
 
 
 @functools.wraps(bool)
 def __parse_bool(x):
     _x = str(x).lower().strip()
@@ -105,14 +105,18 @@
     return _is_type(t, bool)
 
 
 def _is_str_type(t):
     return _is_type(t, str)
 
 
+def _is_none_type(t):
+    return t is None or _is_type(t, type(None))
+
+
 def _is_literal_type(t):
     return typing.get_origin(t) is Literal
 
 
 def __get_type_parser(t):
     if _is_bool_type(t):
         return __parse_bool
@@ -168,15 +172,15 @@
     """Optional annotation without a type"""
     del a.args["type"]
     return False
 
 
 def _update_union(a: Argument) -> bool:
     """Optional annotation with a type (interpreted as a Union), Union"""
-    arg_set = [v for v in a.type_args if not issubclass(v, type(None)) and v is not None]
+    arg_set = [t for t in a.type_args if not _is_none_type(t)]
     if len(arg_set) == 1:
         # For union of one type (other than None), we support further inspection of the type
         a.args["type"] = a.type_args[0]
         return True
     else:
         a.args["type"] = __wrap_union(a.type, arg_set)
         return False
@@ -209,29 +213,28 @@
     a.args["type"] = __make_enum_parser(a.type)
     return False
 
 
 def _update_literal(a: Argument) -> bool:
     """Literal type is used to define an untyped choice argument"""
     choices = list(a.type_args)
+    assert len(choices) > 0, "'Literal' must have at least one parameter."
     choices_types = set(map(type, a.type_args))
 
     a.args["choices"] = choices
     if len(choices_types) == 1:
         a.args["type"] = list(choices_types)[0]
         return True
-    elif len(choices_types) == 0:
-        del a.args["type"]
     else:
         a.args["type"] = __make_literal_parser(a.type, raise_error=False)
         return False
 
 
 def _update_bool(a: Argument) -> bool:
-    """bool type is used to define a store_true argument"""
+    """bool type is used to define a BooleanOptionalAction argument"""
     if hasattr(argparse, "BooleanOptionalAction"):
         a.args["action"] = argparse.BooleanOptionalAction
     else:
         a.args["action"] = "store_true"
         del a.args["type"]
     return False
 
@@ -261,7 +264,31 @@
 
 def _update_field_type(argument_args: Dict[str, Any]):
     a = Argument(argument_args)
     iter_count = itertools.count()
     # Some types are recursive, so we iterate until no special type is matched
     while _update_field_type_internal(a) and next(iter_count) < _TYPE_RECURSION_LIMIT:
         a.update_type()
+
+
+def _obj_to_yaml_dict(o):
+    if isinstance(o, dict):
+        return {k: _obj_to_yaml_dict(v) for k, v in o.items()}
+    if isinstance(o, (tuple, list)):
+        return [_obj_to_yaml_dict(v) for v in o]
+    if isinstance(o, enum.Enum):
+        return o.name
+    if isinstance(o, (int, float, bool)) or o is None:
+        return o
+    else:
+        return str(o)
+
+
+def _yaml_dict_to_obj(o, value_type: Union[Callable, Dict[str, Callable]]):
+    if isinstance(o, dict):
+        return {k: _yaml_dict_to_obj(v, value_type.get(k, None)) for k, v in o.items()}
+    if isinstance(o, (tuple, list)):
+        return [_yaml_dict_to_obj(v, value_type) for v in o]
+    if callable(value_type) and isinstance(o, str):
+        return value_type(o)
+    else:
+        return o
```

### Comparing `classparse-0.1.1/classparse.egg-info/PKG-INFO` & `classparse-0.1.2/classparse.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: classparse
-Version: 0.1.1
+Version: 0.1.2
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
-pip install git+https://github.com/liran-funaro/classparse@0.1.1
+pip install classparse==0.1.2
 ```
 
 # Simple Example
 This is a simple example of the most basic usage of this library.
 <!-- embed: examples/simple.py -->
 ```python
 # examples/simple.py
@@ -122,15 +122,15 @@
     prog="my_program.py",  # Keyword arguments are passed to the parser init.
     default_argument_args=dict(help="(type: %(type)s)"),  # Set default arguments for each call of add_argument().
 )
 @dataclass(frozen=True)
 class AllOptions:
     """
     Class doc string ==> parser description.
-    The fields' inline comment ==> argument's help.
+    The fields' inline/above comment ==> argument's help.
     """
 
     pos_arg_1: str  # Field with no explicit default ==> positional arguments (default=%(default)s)
     pos_arg_2: int = pos_arg(
         5,
         nargs="?",
         help=(
@@ -140,15 +140,15 @@
         ),
     )  # When the help field is specified explicitly, the inline comment is ignored
     int_arg: int = 1  # Field's type and default are applied to the parser (type=%(type)s, default=%(default)s)
     str_enum_choice_arg: Action = Action.Initialize  # StrEnum ==> choice argument (type=%(type)s, default=%(default)s)
     int_enum_choice_arg: Animal = Animal.Cat  # IntEnum ==> choice argument (type=%(type)s, default=%(default)s)
     literal_arg: Literal["a", "b", "c"] = None  # Literal ==> choice argument (type=%(type)s, default=%(default)s)
     literal_int_arg: Literal[1, 2, 3] = None  # Literal's type is automatically inferred (type=%(type)s)
-    mixed_literal: Literal[1, 2, "3", "4", True] = None  # We can mix multiple literal types (type=%(type)s)
+    mixed_literal: Literal[1, 2, "3", "4", True, Animal.Cat] = None  # We can mix multiple literal types (type=%(type)s)
     optional_arg: Optional[int] = None  # Optional can be used for type hinting (type=%(type)s)
     just_optional_arg: Optional = None  # Bare optional also works (type=%(type)s)
     optional_choice_arg: Optional[Action] = None  # Nested types are supported (type=%(type)s)
     union_arg: Union[int, float, bool] = None  # Tries to convert to type in order until first success (type=%(type)s)
     path_arg: Path = None
     flag_arg: int = arg(
         "-f",
@@ -162,16 +162,17 @@
     required_arg: float = arg("-r", required=True)  # E.g., required=%(required)s
     metavar_arg: str = arg(metavar="M")  # E.g., metavar=%(metavar)s
     int_list: List[int] = (1,)  # List type hint ==> nargs="+" (type=%(type)s)
     int_2_list: Tuple[int, int] = (1, 2)  # Tuple type hint ==> nargs=<tuple length> (nargs=%(nargs)s, type=%(type)s)
     multi_type_tuple: Tuple[int, float, str] = (1, 1e-3, "a")  # We can use multiple types (type=%(type)s)
     actions: List[Action] = ()  # List[Enum] ==> choices with nargs="+" (nargs=%(nargs)s, type=%(type)s)
     animals: List[Animal] = ()  # List[Enum] ==> choices with nargs="+" (nargs=%(nargs)s, type=%(type)s)
-    literal_list: List[Literal["aa", "bb"]] = ("aa",)  # List[Literal] ==> choices with nargs="+"
+    literal_list: List[Literal["aa", "bb", 11, 22, Animal.Cat]] = ("aa",)  # List[Literal] ==> choices with nargs="+"
     union_list: List[Union[int, float, str, bool]] = ()
+    union_with_literal: List[Union[Literal["a", "b", 1, 2], float, bool]] = ()
     typeless_list: list = ()  # If list type is unspecified, then it uses argparse default (type=%(type)s)
     typeless_typing_list: List = ()  # typing.List or list are supported
     none_bool_arg: bool = None  # boolean args ==> argparse.BooleanOptionalAction (type=%(type)s)
     true_bool_arg: bool = True  # We can set any default value
     false_bool_arg: bool = False
     complex_arg: complex = complex(1, -1)
 
@@ -197,36 +198,37 @@
 <!-- execute: python examples/usage.py --help -->
 ```text
 $ python examples/usage.py --help
 usage: my_program.py [-h] [--int-arg INT_ARG]
                      [--str-enum-choice-arg {Initialize/init,Execute/exec}]
                      [--int-enum-choice-arg {Cat/1,Dog/2}]
                      [--literal-arg {a,b,c}] [--literal-int-arg {1,2,3}]
-                     [--mixed-literal {1,2,3,4,True}]
+                     [--mixed-literal {1,2,3,4,True,Animal.Cat}]
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
-                     [--literal-list {aa,bb} [{aa,bb} ...]]
+                     [--literal-list {aa,bb,11,22,Animal.Cat} [{aa,bb,11,22,Animal.Cat} ...]]
                      [--union-list UNION_LIST [UNION_LIST ...]]
+                     [--union-with-literal UNION_WITH_LITERAL [UNION_WITH_LITERAL ...]]
                      [--typeless-list TYPELESS_LIST [TYPELESS_LIST ...]]
                      [--typeless-typing-list TYPELESS_TYPING_LIST [TYPELESS_TYPING_LIST ...]]
                      [--none-bool-arg | --no-none-bool-arg]
                      [--true-bool-arg | --no-true-bool-arg]
                      [--false-bool-arg | --no-false-bool-arg]
                      [--complex-arg COMPLEX_ARG] [-s SHOW [SHOW ...]]
                      pos-arg-1 [pos-arg-2]
 
-Class doc string ==> parser description. The fields' inline comment ==>
+Class doc string ==> parser description. The fields' inline/above comment ==>
 argument's help.
 
 positional arguments:
   pos-arg-1             Field with no explicit default ==> positional
                         arguments (default=None)
   pos-arg-2             pos_arg() is a wrapper around dataclasses.field().The
                         first argument (optional) is the argument default
@@ -242,17 +244,18 @@
                         default=Initialize)
   --int-enum-choice-arg {Cat/1,Dog/2}
                         IntEnum ==> choice argument (type=Animal, default=Cat)
   --literal-arg {a,b,c}
                         Literal ==> choice argument (type=str, default=None)
   --literal-int-arg {1,2,3}
                         Literal's type is automatically inferred (type=int)
-  --mixed-literal {1,2,3,4,True}
+  --mixed-literal {1,2,3,4,True,Animal.Cat}
                         We can mix multiple literal types
-                        (type=typing.Literal[1, 2, '3', '4', True])
+                        (type=typing.Literal[1, 2, '3', '4', True,
+                        <Animal.Cat: 1>])
   --optional-arg OPTIONAL_ARG
                         Optional can be used for type hinting (type=int)
   --just-optional-arg JUST_OPTIONAL_ARG
                         Bare optional also works (type=None)
   --optional-choice-arg {Initialize/init,Execute/exec}
                         Nested types are supported (type=Action)
   --union-arg UNION_ARG
@@ -277,18 +280,21 @@
                         float, str])
   --actions {Initialize/init,Execute/exec} [{Initialize/init,Execute/exec} ...]
                         List[Enum] ==> choices with nargs="+" (nargs=+,
                         type=Action)
   --animals {Cat/1,Dog/2} [{Cat/1,Dog/2} ...]
                         List[Enum] ==> choices with nargs="+" (nargs=+,
                         type=Animal)
-  --literal-list {aa,bb} [{aa,bb} ...]
+  --literal-list {aa,bb,11,22,Animal.Cat} [{aa,bb,11,22,Animal.Cat} ...]
                         List[Literal] ==> choices with nargs="+"
   --union-list UNION_LIST [UNION_LIST ...]
                         (type: typing.Union[int, float, str, bool])
+  --union-with-literal UNION_WITH_LITERAL [UNION_WITH_LITERAL ...]
+                        (type: typing.Union[typing.Literal['a', 'b', 1, 2],
+                        float, bool])
   --typeless-list TYPELESS_LIST [TYPELESS_LIST ...]
                         If list type is unspecified, then it uses argparse
                         default (type=None)
   --typeless-typing-list TYPELESS_TYPING_LIST [TYPELESS_TYPING_LIST ...]
                         typing.List or list are supported
   --none-bool-arg, --no-none-bool-arg
                         boolean args ==> argparse.BooleanOptionalAction
```

### Comparing `classparse-0.1.1/pyproject.toml` & `classparse-0.1.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "classparse"
-version = "0.1.1"
+version = "0.1.2"
 description = "Declarative `ArgumentParser` definition with `dataclass` notation."
 readme = "README.md"
 authors = [{ name = "Liran Funaro", email = "liran.funaro@gmail.com" }]
 license = { text = "BSD-3-Clause" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
@@ -51,29 +51,29 @@
 [project.optional-dependencies]
 dev = ["bumpver", "black", "flake8", "pip-tools", "pytest", "pytest-cov", "coveralls"]
 
 [project.urls]
 Homepage = "https://github.com/liran-funaro/classparse"
 
 [tool.bumpver]
-current_version = "0.1.1"
+current_version = "0.1.2"
 version_pattern = "MAJOR.MINOR.PATCH[-TAG]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
     "current_version = \"{version}\"",
     "version = \"{version}\"",
     "Copyright (c) 2023-YYYY, Liran Funaro.",
 ]
 "README.md" = [
-    "classparse@{version}",
+    "classparse=={version}",
     "Copyright (c) 2023-YYYY, Liran Funaro.",
 ]
 "LICENSE" = [
     "Copyright (c) 2023-YYYY, Liran Funaro.",
 ]
 "*/*.py" = [
     "Copyright (c) 2023-YYYY, Liran Funaro.",
```

