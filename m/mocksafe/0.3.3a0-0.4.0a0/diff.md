# Comparing `tmp/mocksafe-0.3.3a0.tar.gz` & `tmp/mocksafe-0.4.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mocksafe-0.3.3a0.tar", last modified: Sun May 14 19:37:25 2023, max compression
+gzip compressed data, was "mocksafe-0.4.0a0.tar", last modified: Tue May 16 18:35:00 2023, max compression
```

## Comparing `mocksafe-0.3.3a0.tar` & `mocksafe-0.4.0a0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 danielmayo   (501) staff       (20)        0 2023-05-14 19:37:25.191592 mocksafe-0.3.3a0/
--rw-r--r--   0 danielmayo   (501) staff       (20)     1068 2023-05-08 16:33:22.000000 mocksafe-0.3.3a0/LICENSE
--rw-r--r--   0 danielmayo   (501) staff       (20)     3425 2023-05-14 19:37:25.191378 mocksafe-0.3.3a0/PKG-INFO
--rw-r--r--   0 danielmayo   (501) staff       (20)      820 2023-05-14 19:30:06.000000 mocksafe-0.3.3a0/README.rst
-drwxr-xr-x   0 danielmayo   (501) staff       (20)        0 2023-05-14 19:37:25.182524 mocksafe-0.3.3a0/mocksafe/
--rw-r--r--   0 danielmayo   (501) staff       (20)      400 2023-05-14 19:28:21.000000 mocksafe-0.3.3a0/mocksafe/__init__.py
--rw-r--r--   0 danielmayo   (501) staff       (20)      987 2023-05-08 16:37:20.000000 mocksafe-0.3.3a0/mocksafe/call_matchers.py
--rw-r--r--   0 danielmayo   (501) staff       (20)     3616 2023-05-14 14:51:07.000000 mocksafe-0.3.3a0/mocksafe/call_type_validator.py
--rw-r--r--   0 danielmayo   (501) staff       (20)      119 2023-05-08 16:37:10.000000 mocksafe-0.3.3a0/mocksafe/custom_types.py
--rw-r--r--   0 danielmayo   (501) staff       (20)     5261 2023-05-14 14:51:07.000000 mocksafe-0.3.3a0/mocksafe/mock.py
--rw-r--r--   0 danielmayo   (501) staff       (20)     1583 2023-05-14 14:52:32.000000 mocksafe-0.3.3a0/mocksafe/spy.py
--rw-r--r--   0 danielmayo   (501) staff       (20)     3075 2023-05-14 15:05:34.000000 mocksafe-0.3.3a0/mocksafe/stub.py
--rw-r--r--   0 danielmayo   (501) staff       (20)     3944 2023-05-08 16:37:45.000000 mocksafe-0.3.3a0/mocksafe/that.py
--rw-r--r--   0 danielmayo   (501) staff       (20)     5485 2023-05-08 16:37:45.000000 mocksafe-0.3.3a0/mocksafe/when_then.py
-drwxr-xr-x   0 danielmayo   (501) staff       (20)        0 2023-05-14 19:37:25.190899 mocksafe-0.3.3a0/mocksafe.egg-info/
--rw-r--r--   0 danielmayo   (501) staff       (20)     3425 2023-05-14 19:37:25.000000 mocksafe-0.3.3a0/mocksafe.egg-info/PKG-INFO
--rw-r--r--   0 danielmayo   (501) staff       (20)      377 2023-05-14 19:37:25.000000 mocksafe-0.3.3a0/mocksafe.egg-info/SOURCES.txt
--rw-r--r--   0 danielmayo   (501) staff       (20)        1 2023-05-14 19:37:25.000000 mocksafe-0.3.3a0/mocksafe.egg-info/dependency_links.txt
--rw-r--r--   0 danielmayo   (501) staff       (20)        9 2023-05-14 19:37:25.000000 mocksafe-0.3.3a0/mocksafe.egg-info/top_level.txt
--rw-r--r--   0 danielmayo   (501) staff       (20)     1825 2023-05-14 19:29:45.000000 mocksafe-0.3.3a0/pyproject.toml
--rw-r--r--   0 danielmayo   (501) staff       (20)       38 2023-05-14 19:37:25.191644 mocksafe-0.3.3a0/setup.cfg
-drwxr-xr-x   0 danielmayo   (501) staff       (20)        0 2023-05-14 19:37:25.191134 mocksafe-0.3.3a0/tests/
--rw-r--r--   0 danielmayo   (501) staff       (20)     6086 2023-05-14 15:00:39.000000 mocksafe-0.3.3a0/tests/test_mocksafe.py
+drwxr-xr-x   0 danielmayo   (501) staff       (20)        0 2023-05-16 18:35:00.295553 mocksafe-0.4.0a0/
+-rw-r--r--   0 danielmayo   (501) staff       (20)     1068 2023-05-08 16:33:22.000000 mocksafe-0.4.0a0/LICENSE
+-rw-r--r--   0 danielmayo   (501) staff       (20)     3474 2023-05-16 18:35:00.295278 mocksafe-0.4.0a0/PKG-INFO
+-rw-r--r--   0 danielmayo   (501) staff       (20)      820 2023-05-16 17:23:30.000000 mocksafe-0.4.0a0/README.rst
+drwxr-xr-x   0 danielmayo   (501) staff       (20)        0 2023-05-16 18:35:00.285380 mocksafe-0.4.0a0/mocksafe/
+-rw-r--r--   0 danielmayo   (501) staff       (20)      400 2023-05-16 17:23:30.000000 mocksafe-0.4.0a0/mocksafe/__init__.py
+-rw-r--r--   0 danielmayo   (501) staff       (20)      987 2023-05-08 16:37:20.000000 mocksafe-0.4.0a0/mocksafe/call_matchers.py
+-rw-r--r--   0 danielmayo   (501) staff       (20)     4198 2023-05-16 17:23:30.000000 mocksafe-0.4.0a0/mocksafe/call_type_validator.py
+-rw-r--r--   0 danielmayo   (501) staff       (20)      119 2023-05-16 16:52:33.000000 mocksafe-0.4.0a0/mocksafe/custom_types.py
+-rw-r--r--   0 danielmayo   (501) staff       (20)     5316 2023-05-16 17:23:30.000000 mocksafe-0.4.0a0/mocksafe/mock.py
+-rw-r--r--   0 danielmayo   (501) staff       (20)     1583 2023-05-14 14:52:32.000000 mocksafe-0.4.0a0/mocksafe/spy.py
+-rw-r--r--   0 danielmayo   (501) staff       (20)     3162 2023-05-16 17:23:30.000000 mocksafe-0.4.0a0/mocksafe/stub.py
+-rw-r--r--   0 danielmayo   (501) staff       (20)     3981 2023-05-16 17:23:30.000000 mocksafe-0.4.0a0/mocksafe/that.py
+-rw-r--r--   0 danielmayo   (501) staff       (20)     5504 2023-05-16 17:23:30.000000 mocksafe-0.4.0a0/mocksafe/when_then.py
+drwxr-xr-x   0 danielmayo   (501) staff       (20)        0 2023-05-16 18:35:00.294577 mocksafe-0.4.0a0/mocksafe.egg-info/
+-rw-r--r--   0 danielmayo   (501) staff       (20)     3474 2023-05-16 18:35:00.000000 mocksafe-0.4.0a0/mocksafe.egg-info/PKG-INFO
+-rw-r--r--   0 danielmayo   (501) staff       (20)      377 2023-05-16 18:35:00.000000 mocksafe-0.4.0a0/mocksafe.egg-info/SOURCES.txt
+-rw-r--r--   0 danielmayo   (501) staff       (20)        1 2023-05-16 18:35:00.000000 mocksafe-0.4.0a0/mocksafe.egg-info/dependency_links.txt
+-rw-r--r--   0 danielmayo   (501) staff       (20)        9 2023-05-16 18:35:00.000000 mocksafe-0.4.0a0/mocksafe.egg-info/top_level.txt
+-rw-r--r--   0 danielmayo   (501) staff       (20)     1869 2023-05-16 17:23:30.000000 mocksafe-0.4.0a0/pyproject.toml
+-rw-r--r--   0 danielmayo   (501) staff       (20)       38 2023-05-16 18:35:00.295623 mocksafe-0.4.0a0/setup.cfg
+drwxr-xr-x   0 danielmayo   (501) staff       (20)        0 2023-05-16 18:35:00.294929 mocksafe-0.4.0a0/tests/
+-rw-r--r--   0 danielmayo   (501) staff       (20)     6117 2023-05-16 17:23:30.000000 mocksafe-0.4.0a0/tests/test_mocksafe.py
```

### Comparing `mocksafe-0.3.3a0/LICENSE` & `mocksafe-0.4.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `mocksafe-0.3.3a0/PKG-INFO` & `mocksafe-0.4.0a0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mocksafe
-Version: 0.3.3a0
+Version: 0.4.0a0
 Summary: A mocking library developed to enable static and runtime type checking of your mocks to keep them in sync with production code.
 License: MIT License
         
         Copyright (c) 2023 Daniel Mayo
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -31,33 +31,34 @@
 Classifier: Natural Language :: English
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Testing :: Mocking
 Classifier: Topic :: Software Development :: Testing :: Unit
 Classifier: Framework :: Pytest
 Classifier: Typing :: Typed
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 .. image:: https://readthedocs.org/projects/mocksafe/badge/?version=latest
     :target: https://mocksafe.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
-MockSafe v0.3.3-alpha
+MockSafe v0.4.0-alpha
 ---------------------
 
 A mocking library developed to enable static and runtime type checking of your mocks to help keep them up-to-date with your production code.
 
 It has a simple, fluent API and is designed to be used with Python's `assert` statement.
 
 Checkout the docs link below for more information.
```

### Comparing `mocksafe-0.3.3a0/README.rst` & `mocksafe-0.4.0a0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 .. image:: https://readthedocs.org/projects/mocksafe/badge/?version=latest
     :target: https://mocksafe.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
-MockSafe v0.3.3-alpha
+MockSafe v0.4.0-alpha
 ---------------------
 
 A mocking library developed to enable static and runtime type checking of your mocks to help keep them up-to-date with your production code.
 
 It has a simple, fluent API and is designed to be used with Python's `assert` statement.
 
 Checkout the docs link below for more information.
```

### Comparing `mocksafe-0.3.3a0/mocksafe/call_matchers.py` & `mocksafe-0.4.0a0/mocksafe/call_matchers.py`

 * *Files identical despite different names*

### Comparing `mocksafe-0.3.3a0/mocksafe/call_type_validator.py` & `mocksafe-0.4.0a0/mocksafe/call_type_validator.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from inspect import Parameter
-from types import GenericAlias, UnionType, MappingProxyType
-from typing import cast
+from types import GenericAlias, MappingProxyType
+from typing import Union, cast
 from mocksafe.custom_types import MethodName
 
 
 class CallTypeValidator:
     def __init__(
         self,
         method_name: MethodName,
@@ -62,15 +62,15 @@
     def _param_match_kwarg(self, name: str, param: Parameter) -> bool:
         if param.kind not in [Parameter.KEYWORD_ONLY, Parameter.POSITIONAL_OR_KEYWORD]:
             return False
 
         return name in self._kwargs or param.default != Parameter.empty
 
     def _validate_type(self, param, arg):
-        if param.annotation != Parameter.empty and not _type_match(
+        if param.annotation != Parameter.empty and not type_match(
             arg, param.annotation
         ):
             raise TypeError(
                 f"Invalid type passed to mocked method {self._method_name}() for parameter: '{param}'. Actual argument passed was: {arg} ({type(arg)})."
             )
 
     def _check_extra_positional_args(self):
@@ -82,24 +82,46 @@
     def _check_extra_keyword_args(self):
         if self._kwargs:
             raise TypeError(
                 f"Mocked method {self._method_name}() was passed unexpected keyword argument(s): {self._kwargs}."
             )
 
 
-def _type_match(arg, expected_type: type) -> bool:
+def type_match(arg, expected_type: type) -> bool:
+    if _is_union(expected_type):
+        generic_type: GenericAlias = cast(GenericAlias, expected_type)
+
+        union: tuple = generic_type.__args__
+
+        # Recursively match any type in the union
+        return any(type_match(arg, t) for t in union)
+
     try:
-        # Handle generic type by checking just the base type
+        # Handle other generic types by checking just the base type
         # E.g. for dict[str, str] just check isinstance(arg, type(dict))
-        origin_type = cast(GenericAlias, expected_type).__origin__
-        return isinstance(arg, origin_type)
+        generic_type = cast(GenericAlias, expected_type)
+        return isinstance(arg, generic_type.__origin__)
     except AttributeError:
         pass
 
+    return isinstance(arg, expected_type)
+
+
+def _is_union(t: type) -> bool:
+    # 1. Check for types.UnionType
+
+    # This type is not supported in Python 3.9
+    # So we check for it at runtime in this hacky way
+    if t.__class__.__name__ == "UnionType":
+        return True
+
+    # 2. Check for typing.Union / typing.Optional
+    # Both are equivalent under the covers
     try:
-        # Handle union type: recursively match any type in the union
-        union: tuple = cast(UnionType, expected_type).__args__
-        return any(_type_match(arg, t) for t in union)
+        generic_type: GenericAlias = cast(GenericAlias, t)
+
+        # typing.Union cannot be used with isinstance()
+        return generic_type.__origin__ == Union
     except AttributeError:
         pass
 
-    return isinstance(arg, expected_type)
+    return False
```

### Comparing `mocksafe-0.3.3a0/mocksafe/mock.py` & `mocksafe-0.4.0a0/mocksafe/mock.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from __future__ import annotations
 import inspect
 from itertools import count
-from typing import Generic, TypeVar, Any, cast
+from typing import Generic, TypeVar, Optional, Union, Any, cast
 from collections.abc import Callable
 from mocksafe.custom_types import MethodName, CallMatcher, Call
 from mocksafe.spy import MethodSpy
 from mocksafe.stub import MethodStub, ResultsProvider
 from mocksafe.call_matchers import ExactCallMatcher
 
 
 T = TypeVar("T")
 
 MOCK_NUMBER = count()
 
 
-def mock(class_type: type[T], name: str | None = None) -> T:
+def mock(class_type: type[T], name: Optional[str] = None) -> T:
     """
     Creates a mock of the given ``class_type``.
 
     :param class_type: the class to be mocked of generic type ``T``
     :type class_type: type[T]
 
     :param name: optional custom name to help identify the
@@ -58,15 +58,15 @@
 
 
 def call_equal_to(exact: Call) -> CallMatcher:
     return ExactCallMatcher(exact)
 
 
 class SafeMock(Generic[T]):
-    def __init__(self, class_type: type[T], name: str | None = None):
+    def __init__(self, class_type: type[T], name: Optional[str] = None):
         self._class_type = class_type
         self._mocks: dict[MethodName, MethodMock] = {}
         self._name = name or next(MOCK_NUMBER)
 
     @property
     def mocked_methods(self) -> dict[MethodName, MethodMock]:
         return self._mocks.copy()
@@ -76,15 +76,15 @@
     @property  # type: ignore
     def __class__(self):
         return self._class_type
 
     def __repr__(self) -> str:
         return f"SafeMock[{self._class_type.__name__}#{self._name}]"
 
-    def __getattr__(self, attr_name: str) -> MethodMock | Any:
+    def __getattr__(self, attr_name: str) -> Union[MethodMock, Any]:
         if attr_mock := self._mocks.get(attr_name):
             return attr_mock
 
         if attr_name in getattr(self._class_type, "__attrs__", []):
             # Field attribute defined on the original class
             raise AttributeError(f"{self}.{attr_name} attribute value not set.")
 
@@ -137,18 +137,20 @@
     def full_name(self) -> str:
         return f"{self._class_type.__name__}.{self.name}"
 
     @property
     def name(self) -> MethodName:
         return self._stub.name
 
-    def add_stub(self, matcher: CallMatcher, effects: list[T | BaseException]) -> None:
+    def add_stub(
+        self, matcher: CallMatcher, effects: list[Union[T, BaseException]]
+    ) -> None:
         self._stub.add(matcher, effects)
 
-    def stub_last_call(self, effects: list[T | BaseException]) -> None:
+    def stub_last_call(self, effects: list[Union[T, BaseException]]) -> None:
         matcher = call_equal_to(self._spy.pop_call())
         self._stub.add(matcher, effects)
 
     def custom_result_for_last_call(self, custom: ResultsProvider) -> None:
         matcher = call_equal_to(self._spy.pop_call())
         self.custom_result(matcher, custom)
```

### Comparing `mocksafe-0.3.3a0/mocksafe/spy.py` & `mocksafe-0.4.0a0/mocksafe/spy.py`

 * *Files identical despite different names*

### Comparing `mocksafe-0.3.3a0/mocksafe/stub.py` & `mocksafe-0.4.0a0/mocksafe/stub.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from inspect import Signature, isclass
-from typing import Generic, TypeVar
+from typing import Generic, TypeVar, Optional, Union
 from collections.abc import Callable
 from mocksafe.custom_types import MethodName, CallMatcher
+from mocksafe.call_type_validator import type_match
 
 
 T = TypeVar("T")
 ResultsProvider = Callable[..., T]
 
 
 # Stub default values for these simple built-in types
@@ -14,24 +15,24 @@
 
 class MethodStub(Generic[T]):
     def __init__(self, name: MethodName, result_type: type):
         self._name = name
         self._stubs: list[tuple[CallMatcher, ResultsProvider]] = []
         self._result_type = result_type
 
-    def __call__(self, *args, **kwargs) -> T | None:
+    def __call__(self, *args, **kwargs) -> Optional[T]:
         call = (tuple(args), kwargs)
         for matcher, results in self._stubs:
             if matcher(call):
                 return results(*args, **kwargs)
 
         # No default return value has been stubbed, try to determine
         # something sensible to return
 
-        default_value: T | None
+        default_value: Optional[T]
         result_type: type = self._result_type
 
         if result_type == type(None):
             default_value = None  # type: ignore
         elif result_type == Signature.empty:
             # There are no type annotations to infer type from.
             # Fall back to None.
@@ -49,31 +50,31 @@
             reps.append(f"{matcher} -> {results}")
         return "; ".join(reps)
 
     @property
     def name(self) -> MethodName:
         return self._name
 
-    def add(self, matcher: CallMatcher, effects: list[T | BaseException]) -> None:
+    def add(self, matcher: CallMatcher, effects: list[Union[T, BaseException]]) -> None:
         self._validate_effects(effects)
         self.add_effect(matcher, CannedEffects(effects))
 
     def add_effect(self, matcher: CallMatcher, effect: ResultsProvider) -> None:
         self._stubs.insert(0, (matcher, effect))
 
-    def _validate_effects(self, effects: list[T | BaseException]):
+    def _validate_effects(self, effects: list[Union[T, BaseException]]):
         # Runtime check in case static type checking allows an incompatible type
         # to slip through
         if self._result_type == Signature.empty:
             return  # Nothing we can check
 
         for e in effects:
             if isinstance(e, BaseException):
                 continue
-            if not isinstance(e, self._result_type):
+            if not type_match(e, self._result_type):
                 raise TypeError(
                     f"Cannot use stub result {e} ({type(e)}) with the mocked method {self._name}(), the expected return type is: {self._result_type}."
                 )
 
 
 class CannedEffects(Generic[T]):
     def __init__(self, effects: list[T]):
```

### Comparing `mocksafe-0.3.3a0/mocksafe/that.py` & `mocksafe-0.4.0a0/mocksafe/that.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from __future__ import annotations
+from typing import Union
 from collections.abc import Callable
 from mocksafe.custom_types import Call
 from mocksafe.mock import MethodMock
 
 
 Args = tuple
 
@@ -121,19 +122,19 @@
 
     @property
     def num_calls(self) -> int:
         """Returns the number of calls made to the mocked method."""
         return len(self._method_mock.calls)
 
     @property
-    def last_call(self) -> Args | Call:
+    def last_call(self) -> Union[Args, Call]:
         """Returns details of the last call made to the mocked method."""
         return self.nth_call(-1)
 
-    def nth_call(self, n: int) -> Args | Call:
+    def nth_call(self, n: int) -> Union[Args, Call]:
         """Returns details of the Nth call made to the mocked method."""
         call = self._method_mock.nth_call(n)
 
         args, kwargs = call
 
         if kwargs:
             return call
```

### Comparing `mocksafe-0.3.3a0/mocksafe/when_then.py` & `mocksafe-0.4.0a0/mocksafe/when_then.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from __future__ import annotations
-from typing import Generic, TypeVar
+from typing import Generic, Union, TypeVar
 from collections.abc import Callable
 from mocksafe.custom_types import CallMatcher
 from mocksafe.mock import MethodMock, ResultsProvider
 from mocksafe.call_matchers import AnyCallMatcher, CustomCallMatcher
 
 
 T = TypeVar("T")
@@ -120,15 +120,15 @@
 
     def then(self, result: ResultsProvider) -> None:
         """
         Use a custom lambda to produce stubbed results.
         """
         self._method_mock.custom_result(self._matcher, result)
 
-    def use_side_effects(self, *side_effects: T | BaseException) -> None:
+    def use_side_effects(self, *side_effects: Union[T, BaseException]) -> None:
         """
         Specify an ordered sequence of results and/or exceptions to be returned/raised.
         """
         self._method_mock.add_stub(self._matcher, list(side_effects))
 
 
 class LastCallStubber(Generic[T]):
@@ -160,14 +160,14 @@
 
     def then_raise(self, error: BaseException) -> None:
         self.use_side_effects(error)
 
     def then(self, result: ResultsProvider) -> None:
         self._method_mock.custom_result_for_last_call(result)
 
-    def use_side_effects(self, *side_effects: T | BaseException) -> None:
+    def use_side_effects(self, *side_effects: Union[T, BaseException]) -> None:
         if not self._method_mock.calls:
             raise ValueError(
                 f"Mocked methods do not match: when({self._method_mock.full_name}).called_with(<different_method>)"
             )
 
         self._method_mock.stub_last_call(list(side_effects))
```

### Comparing `mocksafe-0.3.3a0/mocksafe.egg-info/PKG-INFO` & `mocksafe-0.4.0a0/mocksafe.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mocksafe
-Version: 0.3.3a0
+Version: 0.4.0a0
 Summary: A mocking library developed to enable static and runtime type checking of your mocks to keep them in sync with production code.
 License: MIT License
         
         Copyright (c) 2023 Daniel Mayo
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -31,33 +31,34 @@
 Classifier: Natural Language :: English
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Testing :: Mocking
 Classifier: Topic :: Software Development :: Testing :: Unit
 Classifier: Framework :: Pytest
 Classifier: Typing :: Typed
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 .. image:: https://readthedocs.org/projects/mocksafe/badge/?version=latest
     :target: https://mocksafe.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
-MockSafe v0.3.3-alpha
+MockSafe v0.4.0-alpha
 ---------------------
 
 A mocking library developed to enable static and runtime type checking of your mocks to help keep them up-to-date with your production code.
 
 It has a simple, fluent API and is designed to be used with Python's `assert` statement.
 
 Checkout the docs link below for more information.
```

### Comparing `mocksafe-0.3.3a0/pyproject.toml` & `mocksafe-0.4.0a0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 [project]
 name = "mocksafe"
-version = "0.3.3-alpha"
+version = "0.4.0-alpha"
 
 description = "A mocking library developed to enable static and runtime type checking of your mocks to keep them in sync with production code."
 
-requires-python = ">= 3.10"
+requires-python = ">= 3.9"
 readme = "README.rst"
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Natural Language :: English",
     "Environment :: Console",
     "Operating System :: OS Independent",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Testing",
     "Topic :: Software Development :: Testing :: Mocking",
@@ -35,15 +36,15 @@
 Source = "https://github.com/dmayo3/mocksafe"
 
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools", "wheel"]
 
 [tool.bumpver]
-current_version = "0.3.3-alpha"
+current_version = "0.4.0-alpha"
 version_pattern = "MAJOR.MINOR.PATCH[-TAG]"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `mocksafe-0.3.3a0/tests/test_mocksafe.py` & `mocksafe-0.4.0a0/tests/test_mocksafe.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from random import Random
+from typing import Optional
 import pytest
 from mocksafe import mock, when, that, spy
 
 
 class MyClass:
     def foo(self, bar: str, baz: int = 123) -> int:
         return baz + len(bar)
 
-    def quux(self) -> str | None:
+    def quux(self) -> Optional[str]:
         return "something"
 
 
 def test_mock_isinstance_of_mocked_class():
     mock_object: MyClass = mock(MyClass)
 
     assert isinstance(mock_object, MyClass)
```

