# Comparing `tmp/nubia-cli-0.2.3.tar.gz` & `tmp/nubia_cli-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nubia-cli-0.2.3.tar", max compression
+gzip compressed data, was "nubia_cli-0.2.4.tar", max compression
```

## Comparing `nubia-cli-0.2.3.tar` & `nubia_cli-0.2.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1539 2022-04-16 06:23:56.277051 nubia-cli-0.2.3/LICENSE
--rw-r--r--   0        0        0      908 2022-12-05 20:14:27.777677 nubia-cli-0.2.3/nubia/__init__.py
--rw-r--r--   0        0        0      232 2022-04-16 06:23:56.277051 nubia-cli-0.2.3/nubia/internal/__init__.py
--rw-r--r--   0        0        0      570 2022-04-16 06:23:56.277051 nubia-cli-0.2.3/nubia/internal/blackcmd.py
--rw-r--r--   0        0        0    20321 2022-10-29 19:48:54.572808 nubia-cli-0.2.3/nubia/internal/cmdbase.py
--rw-r--r--   0        0        0     1427 2022-04-16 06:23:56.277051 nubia-cli-0.2.3/nubia/internal/cmdloader.py
--rw-r--r--   0        0        0      232 2022-04-16 06:23:56.277051 nubia-cli-0.2.3/nubia/internal/commands/__init__.py
--rw-r--r--   0        0        0     2167 2022-04-16 06:23:56.277051 nubia-cli-0.2.3/nubia/internal/commands/builtin.py
--rw-r--r--   0        0        0     2326 2022-04-16 06:23:56.277051 nubia-cli-0.2.3/nubia/internal/commands/help.py
--rw-r--r--   0        0        0    12489 2022-12-05 20:14:27.777677 nubia-cli-0.2.3/nubia/internal/completion.py
--rw-r--r--   0        0        0      293 2022-04-16 06:23:56.277051 nubia-cli-0.2.3/nubia/internal/constants.py
--rw-r--r--   0        0        0     2871 2022-04-16 06:23:56.277051 nubia-cli-0.2.3/nubia/internal/context.py
--rw-r--r--   0        0        0     1419 2022-04-16 06:23:56.277051 nubia-cli-0.2.3/nubia/internal/deprecation.py
--rw-r--r--   0        0        0      417 2022-04-16 06:23:56.277051 nubia-cli-0.2.3/nubia/internal/exceptions.py
--rw-r--r--   0        0        0     6941 2022-04-16 06:23:56.277051 nubia-cli-0.2.3/nubia/internal/helpers.py
--rw-r--r--   0        0        0     7784 2022-04-16 06:23:56.277051 nubia-cli-0.2.3/nubia/internal/interactive.py
--rw-r--r--   0        0        0      232 2022-04-16 06:23:56.277051 nubia-cli-0.2.3/nubia/internal/io/__init__.py
--rw-r--r--   0        0        0      919 2022-04-16 06:23:56.277051 nubia-cli-0.2.3/nubia/internal/io/eventbus.py
--rw-r--r--   0        0        0     1617 2022-04-16 06:23:56.277051 nubia-cli-0.2.3/nubia/internal/io/logger.py
--rw-r--r--   0        0        0     1754 2022-04-16 06:23:56.277051 nubia-cli-0.2.3/nubia/internal/io/session_logger.py
--rw-r--r--   0        0        0     1870 2022-04-16 06:23:56.277051 nubia-cli-0.2.3/nubia/internal/ipython.py
--rw-r--r--   0        0        0    12114 2022-04-16 08:03:37.550418 nubia-cli-0.2.3/nubia/internal/nubia.py
--rw-r--r--   0        0        0     1346 2022-12-05 20:14:27.777677 nubia-cli-0.2.3/nubia/internal/options.py
--rw-r--r--   0        0        0     3609 2022-12-05 20:14:27.777677 nubia-cli-0.2.3/nubia/internal/parser.py
--rw-r--r--   0        0        0     5084 2022-04-16 06:23:56.277051 nubia-cli-0.2.3/nubia/internal/plugin_interface.py
--rw-r--r--   0        0        0     4194 2022-04-16 06:23:56.277051 nubia-cli-0.2.3/nubia/internal/registry.py
--rw-r--r--   0        0        0     4034 2022-10-29 19:48:54.572808 nubia-cli-0.2.3/nubia/internal/registry_tools.py
--rw-r--r--   0        0        0    13996 2022-04-16 06:23:56.277051 nubia-cli-0.2.3/nubia/internal/typing/__init__.py
--rw-r--r--   0        0        0    12512 2022-08-02 02:16:46.055147 nubia-cli-0.2.3/nubia/internal/typing/argparse.py
--rw-r--r--   0        0        0     5983 2022-04-16 06:23:56.277051 nubia-cli-0.2.3/nubia/internal/typing/builder.py
--rw-r--r--   0        0        0     1726 2022-10-29 19:47:44.132076 nubia-cli-0.2.3/nubia/internal/typing/inspect.py
--rw-r--r--   0        0        0      232 2022-04-16 06:23:56.281051 nubia-cli-0.2.3/nubia/internal/ui/__init__.py
--rw-r--r--   0        0        0      720 2022-04-16 06:23:56.281051 nubia-cli-0.2.3/nubia/internal/ui/ipython.py
--rw-r--r--   0        0        0     9874 2022-04-16 06:23:56.281051 nubia-cli-0.2.3/nubia/internal/ui/lexer.py
--rw-r--r--   0        0        0      705 2022-04-16 06:23:56.281051 nubia-cli-0.2.3/nubia/internal/ui/statusbar.py
--rw-r--r--   0        0        0     2329 2022-04-16 06:23:56.281051 nubia-cli-0.2.3/nubia/internal/ui/style.py
--rw-r--r--   0        0        0     1067 2022-04-16 06:23:56.281051 nubia-cli-0.2.3/nubia/internal/usage_logger_interface.py
--rw-r--r--   0        0        0     1511 2022-12-05 20:20:26.209640 nubia-cli-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      972 2022-12-05 20:23:27.942551 nubia-cli-0.2.3/setup.py
--rw-r--r--   0        0        0      765 2022-12-05 20:23:27.942718 nubia-cli-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1539 2022-04-16 06:23:56.277051 nubia_cli-0.2.4/LICENSE
+-rw-r--r--   0        0        0      908 2023-05-16 10:40:54.852223 nubia_cli-0.2.4/nubia/__init__.py
+-rw-r--r--   0        0        0      232 2022-04-16 06:23:56.277051 nubia_cli-0.2.4/nubia/internal/__init__.py
+-rw-r--r--   0        0        0      570 2022-04-16 06:23:56.277051 nubia_cli-0.2.4/nubia/internal/blackcmd.py
+-rw-r--r--   0        0        0    20321 2022-10-29 19:48:54.572808 nubia_cli-0.2.4/nubia/internal/cmdbase.py
+-rw-r--r--   0        0        0     1435 2023-05-16 10:40:54.852223 nubia_cli-0.2.4/nubia/internal/cmdloader.py
+-rw-r--r--   0        0        0      232 2022-04-16 06:23:56.277051 nubia_cli-0.2.4/nubia/internal/commands/__init__.py
+-rw-r--r--   0        0        0     2167 2022-04-16 06:23:56.277051 nubia_cli-0.2.4/nubia/internal/commands/builtin.py
+-rw-r--r--   0        0        0     2326 2022-04-16 06:23:56.277051 nubia_cli-0.2.4/nubia/internal/commands/help.py
+-rw-r--r--   0        0        0    12485 2023-05-16 10:40:54.852223 nubia_cli-0.2.4/nubia/internal/completion.py
+-rw-r--r--   0        0        0      293 2022-04-16 06:23:56.277051 nubia_cli-0.2.4/nubia/internal/constants.py
+-rw-r--r--   0        0        0     2871 2022-04-16 06:23:56.277051 nubia_cli-0.2.4/nubia/internal/context.py
+-rw-r--r--   0        0        0     1419 2022-04-16 06:23:56.277051 nubia_cli-0.2.4/nubia/internal/deprecation.py
+-rw-r--r--   0        0        0      417 2022-04-16 06:23:56.277051 nubia_cli-0.2.4/nubia/internal/exceptions.py
+-rw-r--r--   0        0        0     6941 2022-04-16 06:23:56.277051 nubia_cli-0.2.4/nubia/internal/helpers.py
+-rw-r--r--   0        0        0     7784 2022-04-16 06:23:56.277051 nubia_cli-0.2.4/nubia/internal/interactive.py
+-rw-r--r--   0        0        0      232 2022-04-16 06:23:56.277051 nubia_cli-0.2.4/nubia/internal/io/__init__.py
+-rw-r--r--   0        0        0      919 2022-04-16 06:23:56.277051 nubia_cli-0.2.4/nubia/internal/io/eventbus.py
+-rw-r--r--   0        0        0     1617 2022-04-16 06:23:56.277051 nubia_cli-0.2.4/nubia/internal/io/logger.py
+-rw-r--r--   0        0        0     1754 2022-04-16 06:23:56.277051 nubia_cli-0.2.4/nubia/internal/io/session_logger.py
+-rw-r--r--   0        0        0     1870 2022-04-16 06:23:56.277051 nubia_cli-0.2.4/nubia/internal/ipython.py
+-rw-r--r--   0        0        0    12114 2022-04-16 08:03:37.550418 nubia_cli-0.2.4/nubia/internal/nubia.py
+-rw-r--r--   0        0        0     1346 2022-12-05 20:14:27.777677 nubia_cli-0.2.4/nubia/internal/options.py
+-rw-r--r--   0        0        0     3609 2022-12-05 20:14:27.777677 nubia_cli-0.2.4/nubia/internal/parser.py
+-rw-r--r--   0        0        0     5084 2022-04-16 06:23:56.277051 nubia_cli-0.2.4/nubia/internal/plugin_interface.py
+-rw-r--r--   0        0        0     4194 2022-04-16 06:23:56.277051 nubia_cli-0.2.4/nubia/internal/registry.py
+-rw-r--r--   0        0        0     4034 2022-10-29 19:48:54.572808 nubia_cli-0.2.4/nubia/internal/registry_tools.py
+-rw-r--r--   0        0        0    13996 2022-04-16 06:23:56.277051 nubia_cli-0.2.4/nubia/internal/typing/__init__.py
+-rw-r--r--   0        0        0    12512 2022-08-02 02:16:46.055147 nubia_cli-0.2.4/nubia/internal/typing/argparse.py
+-rw-r--r--   0        0        0     6116 2023-05-16 10:40:54.852223 nubia_cli-0.2.4/nubia/internal/typing/builder.py
+-rw-r--r--   0        0        0     1999 2023-05-16 10:40:54.852223 nubia_cli-0.2.4/nubia/internal/typing/inspect.py
+-rw-r--r--   0        0        0      232 2022-04-16 06:23:56.281051 nubia_cli-0.2.4/nubia/internal/ui/__init__.py
+-rw-r--r--   0        0        0      720 2022-04-16 06:23:56.281051 nubia_cli-0.2.4/nubia/internal/ui/ipython.py
+-rw-r--r--   0        0        0     9874 2022-04-16 06:23:56.281051 nubia_cli-0.2.4/nubia/internal/ui/lexer.py
+-rw-r--r--   0        0        0      705 2022-04-16 06:23:56.281051 nubia_cli-0.2.4/nubia/internal/ui/statusbar.py
+-rw-r--r--   0        0        0     2329 2022-04-16 06:23:56.281051 nubia_cli-0.2.4/nubia/internal/ui/style.py
+-rw-r--r--   0        0        0     1067 2022-04-16 06:23:56.281051 nubia_cli-0.2.4/nubia/internal/usage_logger_interface.py
+-rw-r--r--   0        0        0     1510 2023-05-16 10:40:54.852223 nubia_cli-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      978 1970-01-01 00:00:00.000000 nubia_cli-0.2.4/setup.py
+-rw-r--r--   0        0        0      865 1970-01-01 00:00:00.000000 nubia_cli-0.2.4/PKG-INFO
```

### Comparing `nubia-cli-0.2.3/LICENSE` & `nubia_cli-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nubia-cli-0.2.3/nubia/__init__.py` & `nubia_cli-0.2.4/nubia/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,8 +30,8 @@
     "context",
     "deprecated",
     "eventbus",
     "exceptions",
     "statusbar",
 ]
 
-__version__ = "0.2.3"
+__version__ = "0.2.4"
```

### Comparing `nubia-cli-0.2.3/nubia/internal/blackcmd.py` & `nubia_cli-0.2.4/nubia/internal/blackcmd.py`

 * *Files identical despite different names*

### Comparing `nubia-cli-0.2.3/nubia/internal/cmdbase.py` & `nubia_cli-0.2.4/nubia/internal/cmdbase.py`

 * *Files identical despite different names*

### Comparing `nubia-cli-0.2.3/nubia/internal/cmdloader.py` & `nubia_cli-0.2.4/nubia/internal/cmdloader.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 # Copyright (c) Facebook, Inc. and its affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 #
+from importlib import import_module
 import pkgutil
 import types
 import typing as t
 
 
 def _walk_module(module: types.ModuleType):
     for attr_name in dir(module):
@@ -19,15 +20,15 @@
             if hasattr(member, "__command"):
                 yield member
 
 
 def _walk_package(name, path) -> t.List[types.FunctionType]:
     packages = pkgutil.walk_packages(path, prefix=f"{name}.")
     for importer, modname, ispkg in packages:
-        loaded = importer.find_module(modname).load_module(modname)
+        loaded = import_module(modname)
         if not ispkg:
             yield from _walk_module(loaded)
 
 
 def load_commands(base_package) -> None:
     """
     Loads all commands defined in a loaded python package object. This function
```

### Comparing `nubia-cli-0.2.3/nubia/internal/commands/builtin.py` & `nubia_cli-0.2.4/nubia/internal/commands/builtin.py`

 * *Files identical despite different names*

### Comparing `nubia-cli-0.2.3/nubia/internal/commands/help.py` & `nubia_cli-0.2.4/nubia/internal/commands/help.py`

 * *Files identical despite different names*

### Comparing `nubia-cli-0.2.3/nubia/internal/completion.py` & `nubia_cli-0.2.4/nubia/internal/completion.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,17 +48,17 @@
         if delim == "=":
             self._is_argument = True
             self._key = key
         else:
             # This is positional, the value is the key
             value = self._key
             assert len(value) == 0
+        value = value.strip()
         if len(value) > 0:
             # Let's parse the value, is it a single, list, dict?
-            value = value.strip()
             if value[0] == "[":
                 self._is_list = True
                 value = value.strip("[")
                 list_values = value.rpartition(",")
                 self._last_value = list_values[len(list_values) - 1].lstrip()
             elif value[0] == "{":
                 self._is_dict = True
```

### Comparing `nubia-cli-0.2.3/nubia/internal/context.py` & `nubia_cli-0.2.4/nubia/internal/context.py`

 * *Files identical despite different names*

### Comparing `nubia-cli-0.2.3/nubia/internal/deprecation.py` & `nubia_cli-0.2.4/nubia/internal/deprecation.py`

 * *Files identical despite different names*

### Comparing `nubia-cli-0.2.3/nubia/internal/helpers.py` & `nubia_cli-0.2.4/nubia/internal/helpers.py`

 * *Files identical despite different names*

### Comparing `nubia-cli-0.2.3/nubia/internal/interactive.py` & `nubia_cli-0.2.4/nubia/internal/interactive.py`

 * *Files identical despite different names*

### Comparing `nubia-cli-0.2.3/nubia/internal/io/eventbus.py` & `nubia_cli-0.2.4/nubia/internal/io/eventbus.py`

 * *Files identical despite different names*

### Comparing `nubia-cli-0.2.3/nubia/internal/io/logger.py` & `nubia_cli-0.2.4/nubia/internal/io/logger.py`

 * *Files identical despite different names*

### Comparing `nubia-cli-0.2.3/nubia/internal/io/session_logger.py` & `nubia_cli-0.2.4/nubia/internal/io/session_logger.py`

 * *Files identical despite different names*

### Comparing `nubia-cli-0.2.3/nubia/internal/ipython.py` & `nubia_cli-0.2.4/nubia/internal/ipython.py`

 * *Files identical despite different names*

### Comparing `nubia-cli-0.2.3/nubia/internal/nubia.py` & `nubia_cli-0.2.4/nubia/internal/nubia.py`

 * *Files identical despite different names*

### Comparing `nubia-cli-0.2.3/nubia/internal/options.py` & `nubia_cli-0.2.4/nubia/internal/options.py`

 * *Files identical despite different names*

### Comparing `nubia-cli-0.2.3/nubia/internal/parser.py` & `nubia_cli-0.2.4/nubia/internal/parser.py`

 * *Files identical despite different names*

### Comparing `nubia-cli-0.2.3/nubia/internal/plugin_interface.py` & `nubia_cli-0.2.4/nubia/internal/plugin_interface.py`

 * *Files identical despite different names*

### Comparing `nubia-cli-0.2.3/nubia/internal/registry.py` & `nubia_cli-0.2.4/nubia/internal/registry.py`

 * *Files identical despite different names*

### Comparing `nubia-cli-0.2.3/nubia/internal/registry_tools.py` & `nubia_cli-0.2.4/nubia/internal/registry_tools.py`

 * *Files identical despite different names*

### Comparing `nubia-cli-0.2.3/nubia/internal/typing/__init__.py` & `nubia_cli-0.2.4/nubia/internal/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `nubia-cli-0.2.3/nubia/internal/typing/argparse.py` & `nubia_cli-0.2.4/nubia/internal/typing/argparse.py`

 * *Files identical despite different names*

### Comparing `nubia-cli-0.2.3/nubia/internal/typing/builder.py` & `nubia_cli-0.2.4/nubia/internal/typing/builder.py`

 * *Files 5% similar despite different names*

```diff
@@ -150,14 +150,19 @@
         return string
 
 
 def _apply_dict_type(value, key_type=None, value_type=None):
     if not key_type and not value_type:
         return dict(value)
 
+    if not isinstance(value, dict):
+        raise ValueError(
+            "Cannot convert {} to dictionary".format(value)
+        )
+
     key_type = key_type or _identity_function
     value_type = value_type or _identity_function
     return {key_type(key): value_type(value) for key, value in value.items()}
 
 
 def _apply_tuple_type(value, *types):
     if not types:
```

### Comparing `nubia-cli-0.2.3/nubia/internal/typing/inspect.py` & `nubia_cli-0.2.4/nubia/internal/typing/inspect.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,19 +13,26 @@
 # This is re-exported, add more if you need more from typing_inspect elsewhere.
 from typing_inspect import is_optional_type  # noqa
 from typing_inspect import NEW_TYPING, is_tuple_type, is_typevar, is_union_type
 
 from nubia.internal.helpers import issubclass_
 
 if NEW_TYPING:
-    from typing import _GenericAlias
+    # from python 3.9 List, Dict are _SpecialGenericAlias type, which with
+    # _GenericAlias is subclass of _BaseGenericAlias
+    try:
+        from typing import _BaseGenericAlias
+        GENERIC_TYPE = _BaseGenericAlias
+    except ImportError:
+        from typing import _GenericAlias
+        GENERIC_TYPE = _GenericAlias
 
 
 def _is_generic_alias_of(this, that) -> bool:
-    return isinstance(this, _GenericAlias) and issubclass_(this.__origin__, that)
+    return isinstance(this, GENERIC_TYPE) and issubclass_(this.__origin__, that)
 
 
 def is_none_type(tp) -> bool:
     """Checks whether a type is a `None' type."""
     return tp is type(None)  # noqa E721
 
 
@@ -35,15 +42,15 @@
         return tp is Mapping or _is_generic_alias_of(tp, collections.abc.Mapping)
     return issubclass_(tp, collections.abc.Mapping)
 
 
 def is_iterable_type(tp) -> bool:
     """Checks whether a type is an iterable type."""
     if NEW_TYPING:
-        return tp is Iterable or tp is List or _is_generic_alias_of(tp, collections.abc.Iterable)
+        return tp is Iterable or _is_generic_alias_of(tp, collections.abc.Iterable)
     return issubclass_(tp, list)
 
 
 def get_first_type_argument(tp):
     """Returns first type argument, e.g. `int' for `List[int]'."""
     assert hasattr(tp, "__args__") and len(tp.__args__) > 0
     return tp.__args__[0]
```

### Comparing `nubia-cli-0.2.3/nubia/internal/ui/ipython.py` & `nubia_cli-0.2.4/nubia/internal/ui/ipython.py`

 * *Files identical despite different names*

### Comparing `nubia-cli-0.2.3/nubia/internal/ui/lexer.py` & `nubia_cli-0.2.4/nubia/internal/ui/lexer.py`

 * *Files identical despite different names*

### Comparing `nubia-cli-0.2.3/nubia/internal/ui/statusbar.py` & `nubia_cli-0.2.4/nubia/internal/ui/statusbar.py`

 * *Files identical despite different names*

### Comparing `nubia-cli-0.2.3/nubia/internal/ui/style.py` & `nubia_cli-0.2.4/nubia/internal/ui/style.py`

 * *Files identical despite different names*

### Comparing `nubia-cli-0.2.3/nubia/internal/usage_logger_interface.py` & `nubia_cli-0.2.4/nubia/internal/usage_logger_interface.py`

 * *Files identical despite different names*

### Comparing `nubia-cli-0.2.3/pyproject.toml` & `nubia_cli-0.2.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -24,27 +24,27 @@
   | build
   | dist
 )/
 '''
 
 [tool.poetry]
 name = "nubia-cli"
-version = "0.2.3"
+version = "0.2.4"
 description = "A fork of Meta's nubia, a framework for building beautiful shells."
 authors = ["Ahmed Soliman <asoli@fb.com>", "Andreas Backx <andreasbackx@fb.com>",
            "Stardust Systems Dev Team"]
 license = "BSD"
 packages = [
   { include = "nubia" }
 ]
 include = ["LICENSE"]
 
 [tool.poetry.dependencies]
-python = ">3.7.2,<3.10"
-jellyfish = "^0.8.9"
+python = ">3.7.2,<3.12"
+jellyfish = "~0.11"
 prettytable = "^2.4.0"
 prompt-toolkit = "^3.0.23"
 Pygments = "^2.10.0"
 pyparsing = "^2.4.7"
 termcolor = "^1.1.0"
 typing-inspect = "^0.7.1"
 wcwidth = "^0.2.5"
```

### Comparing `nubia-cli-0.2.3/setup.py` & `nubia_cli-0.2.4/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,33 +10,33 @@
  'nubia.internal.ui']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['Pygments>=2.10.0,<3.0.0',
- 'jellyfish>=0.8.9,<0.9.0',
+ 'jellyfish>=0.11,<0.12',
  'prettytable>=2.4.0,<3.0.0',
  'prompt-toolkit>=3.0.23,<4.0.0',
  'pyparsing>=2.4.7,<3.0.0',
  'termcolor>=1.1.0,<2.0.0',
  'typing-inspect>=0.7.1,<0.8.0',
  'wcwidth>=0.2.5,<0.3.0']
 
 setup_kwargs = {
     'name': 'nubia-cli',
-    'version': '0.2.3',
+    'version': '0.2.4',
     'description': "A fork of Meta's nubia, a framework for building beautiful shells.",
-    'long_description': None,
+    'long_description': 'None',
     'author': 'Ahmed Soliman',
     'author_email': 'asoli@fb.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>3.7.2,<3.10',
+    'python_requires': '>3.7.2,<3.12',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `nubia-cli-0.2.3/PKG-INFO` & `nubia_cli-0.2.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: nubia-cli
-Version: 0.2.3
+Version: 0.2.4
 Summary: A fork of Meta's nubia, a framework for building beautiful shells.
 License: BSD
 Author: Ahmed Soliman
 Author-email: asoli@fb.com
-Requires-Python: >3.7.2,<3.10
+Requires-Python: >3.7.2,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Pygments (>=2.10.0,<3.0.0)
-Requires-Dist: jellyfish (>=0.8.9,<0.9.0)
+Requires-Dist: jellyfish (>=0.11,<0.12)
 Requires-Dist: prettytable (>=2.4.0,<3.0.0)
 Requires-Dist: prompt-toolkit (>=3.0.23,<4.0.0)
 Requires-Dist: pyparsing (>=2.4.7,<3.0.0)
 Requires-Dist: termcolor (>=1.1.0,<2.0.0)
 Requires-Dist: typing-inspect (>=0.7.1,<0.8.0)
 Requires-Dist: wcwidth (>=0.2.5,<0.3.0)
```

