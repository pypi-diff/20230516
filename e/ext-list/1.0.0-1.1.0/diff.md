# Comparing `tmp/ext-list-1.0.0.tar.gz` & `tmp/ext-list-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ext-list-1.0.0.tar", last modified: Sun Apr  2 16:07:36 2023, max compression
+gzip compressed data, was "ext-list-1.1.0.tar", last modified: Tue May 16 13:56:29 2023, max compression
```

## Comparing `ext-list-1.0.0.tar` & `ext-list-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 16:07:36.320143 ext-list-1.0.0/
--rw-r--r--   0 root         (0) root         (0)     1082 2023-03-28 13:29:21.000000 ext-list-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4679 2023-04-02 16:07:36.318127 ext-list-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3544 2023-04-02 15:46:27.000000 ext-list-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 16:07:36.307211 ext-list-1.0.0/ext_list.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4679 2023-04-02 16:07:36.000000 ext-list-1.0.0/ext_list.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      197 2023-04-02 16:07:36.000000 ext-list-1.0.0/ext_list.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-02 16:07:36.000000 ext-list-1.0.0/ext_list.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-04-02 16:07:36.000000 ext-list-1.0.0/ext_list.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-02 16:07:36.000000 ext-list-1.0.0/ext_list.egg-info/top_level.txt
--rwxr-xr-x   0 root         (0) root         (0)    25702 2023-04-02 15:38:12.000000 ext-list-1.0.0/ext_list.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-02 16:07:36.320143 ext-list-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1470 2023-04-02 16:05:48.000000 ext-list-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 13:56:29.431176 ext-list-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)     1082 2023-03-28 13:29:21.000000 ext-list-1.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4448 2023-05-16 13:56:29.429622 ext-list-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3326 2023-05-16 13:02:45.000000 ext-list-1.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 13:56:29.378283 ext-list-1.1.0/ext_list/
+-rwxr-xr-x   0 root         (0) root         (0)    33491 2023-05-16 13:02:45.000000 ext-list-1.1.0/ext_list/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1461 2023-05-16 11:17:41.000000 ext-list-1.1.0/ext_list/base.py
+-rw-r--r--   0 root         (0) root         (0)     6545 2023-05-16 13:02:45.000000 ext-list-1.1.0/ext_list/dict_operations.py
+-rw-r--r--   0 root         (0) root         (0)     1420 2023-05-15 19:44:30.000000 ext-list-1.1.0/ext_list/list_operations.py
+-rw-r--r--   0 root         (0) root         (0)     3323 2023-05-15 19:44:30.000000 ext-list-1.1.0/ext_list/operator_operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 13:56:29.420782 ext-list-1.1.0/ext_list.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4448 2023-05-16 13:56:29.000000 ext-list-1.1.0/ext_list.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      311 2023-05-16 13:56:29.000000 ext-list-1.1.0/ext_list.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 13:56:29.000000 ext-list-1.1.0/ext_list.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-16 13:56:29.000000 ext-list-1.1.0/ext_list.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-16 13:56:29.000000 ext-list-1.1.0/ext_list.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-16 13:56:29.431176 ext-list-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1464 2023-05-16 13:44:42.000000 ext-list-1.1.0/setup.py
```

### Comparing `ext-list-1.0.0/LICENSE` & `ext-list-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ext-list-1.0.0/PKG-INFO` & `ext-list-1.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: ext-list
-Version: 1.0.0
+Version: 1.1.0
 Summary: This is a utility library that extends Python's list operations.
 Home-page: https://github.com/sk-guritech/ext-list
 Author: Sakaguchi Ryo
 Author-email: sakaguchi@sk-techfirm.com
 Project-URL: Bug Tracker, https://github.com/sk-guritech/ext-list/issues
 Keywords: list,comprehension,iterable,code quality
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -30,16 +30,15 @@
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ext-list)
 ![GitHub](https://img.shields.io/github/license/sk-guritech/ext-list)
 
 This library was created to improve the quality of code through list operations. It allows commonly written list comprehension operations to be called as methods and enables lists to be treated more abstractly than the built-in `list`.
 
 Using this library reduces the number of times list comprehensions need to be written, resulting in improved overall code readability and searchability.
 
-Additionally, `ExtList` ensures that it is an `Iterable` object of a **single type**, which imposes a constraint to only use lists of a single type. This constraint ultimately leads to a simpler program structure.
-
+More information -> **[Docs: ExtList](https://sk-guritech.github.io/ext-list/)**
 
 ## Installation
 ```
 pip install ext-list
 ```
 
 ## Examples
@@ -119,17 +118,15 @@
     ```
     >>> persons = ExtList([Person('Alice', 25), Person('Bob', 30)])
     >>> persons.to_dict_with_complex_keys([Person.name, Person.age])
     {('Alice', 25): Person('Alice', 30),
     ('Bob', 30): Person('Bob', 25)}
     ```
 
-See the docs for more examples. (under constructed ...)
-
-_**If you want to see more examples immediately, please check out the Examples section in each method docstring.**_
+See the **[Docs: ExtList](https://sk-guritech.github.io/ext-list/)** for more examples !
 
 ## requirements
 ```
 typing_extensions
 ```
 
 ## License
```

### Comparing `ext-list-1.0.0/README.md` & `ext-list-1.1.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ext-list)
 ![GitHub](https://img.shields.io/github/license/sk-guritech/ext-list)
 
 This library was created to improve the quality of code through list operations. It allows commonly written list comprehension operations to be called as methods and enables lists to be treated more abstractly than the built-in `list`.
 
 Using this library reduces the number of times list comprehensions need to be written, resulting in improved overall code readability and searchability.
 
-Additionally, `ExtList` ensures that it is an `Iterable` object of a **single type**, which imposes a constraint to only use lists of a single type. This constraint ultimately leads to a simpler program structure.
-
+More information -> **[Docs: ExtList](https://sk-guritech.github.io/ext-list/)**
 
 ## Installation
 ```
 pip install ext-list
 ```
 
 ## Examples
@@ -92,17 +91,15 @@
     ```
     >>> persons = ExtList([Person('Alice', 25), Person('Bob', 30)])
     >>> persons.to_dict_with_complex_keys([Person.name, Person.age])
     {('Alice', 25): Person('Alice', 30),
     ('Bob', 30): Person('Bob', 25)}
     ```
 
-See the docs for more examples. (under constructed ...)
-
-_**If you want to see more examples immediately, please check out the Examples section in each method docstring.**_
+See the **[Docs: ExtList](https://sk-guritech.github.io/ext-list/)** for more examples !
 
 ## requirements
 ```
 typing_extensions
 ```
 
 ## License
```

### Comparing `ext-list-1.0.0/ext_list.egg-info/PKG-INFO` & `ext-list-1.1.0/ext_list.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: ext-list
-Version: 1.0.0
+Version: 1.1.0
 Summary: This is a utility library that extends Python's list operations.
 Home-page: https://github.com/sk-guritech/ext-list
 Author: Sakaguchi Ryo
 Author-email: sakaguchi@sk-techfirm.com
 Project-URL: Bug Tracker, https://github.com/sk-guritech/ext-list/issues
 Keywords: list,comprehension,iterable,code quality
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -30,16 +30,15 @@
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ext-list)
 ![GitHub](https://img.shields.io/github/license/sk-guritech/ext-list)
 
 This library was created to improve the quality of code through list operations. It allows commonly written list comprehension operations to be called as methods and enables lists to be treated more abstractly than the built-in `list`.
 
 Using this library reduces the number of times list comprehensions need to be written, resulting in improved overall code readability and searchability.
 
-Additionally, `ExtList` ensures that it is an `Iterable` object of a **single type**, which imposes a constraint to only use lists of a single type. This constraint ultimately leads to a simpler program structure.
-
+More information -> **[Docs: ExtList](https://sk-guritech.github.io/ext-list/)**
 
 ## Installation
 ```
 pip install ext-list
 ```
 
 ## Examples
@@ -119,17 +118,15 @@
     ```
     >>> persons = ExtList([Person('Alice', 25), Person('Bob', 30)])
     >>> persons.to_dict_with_complex_keys([Person.name, Person.age])
     {('Alice', 25): Person('Alice', 30),
     ('Bob', 30): Person('Bob', 25)}
     ```
 
-See the docs for more examples. (under constructed ...)
-
-_**If you want to see more examples immediately, please check out the Examples section in each method docstring.**_
+See the **[Docs: ExtList](https://sk-guritech.github.io/ext-list/)** for more examples !
 
 ## requirements
 ```
 typing_extensions
 ```
 
 ## License
```

### Comparing `ext-list-1.0.0/ext_list.py` & `ext-list-1.1.0/ext_list/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from __future__ import annotations
 
-import copy
 from types import FunctionType
-from types import GetSetDescriptorType
-from types import MethodDescriptorType
 from typing import Any
 from typing import Callable
 from typing import Hashable
-from typing import List
 from typing import TypeVar
 
 from typing_extensions import override
+from typing_extensions import SupportsIndex  # type: ignore
+
+from ext_list.dict_operations import _DictOperation  # type: ignore
+from ext_list.list_operations import _ListOperation  # type: ignore
+from ext_list.operator_operations import _OperatorOperation  # type: ignore
 
 T = TypeVar('T')
 TI = TypeVar('TI', bound=type)
 
 
-class ExtList(List[T]):
+class ExtList(_ListOperation[T], _OperatorOperation[T], _DictOperation[T]):
     """
     Note:
         The following class is used to describe each method of ExtList:
 
             >>> class Person:
             ...     def __init__(self, name, age):
             ...         self.__name = name
@@ -41,162 +42,91 @@
             ...         return self.__age
             ...
             ...     def __repr__(self):
             ...         return f'Person(\'{self.name}\', {self.age})'
     """
 
     def __init__(self, iterable: list[T] = []) -> None:
-        ExtList.__validate_all_elements_are_same_type(iterable)
         super().__init__(iterable)
 
     @staticmethod
-    def __validate_all_elements_are_same_type(iterable: list[Any]) -> None:
-        if not iterable:
-            return
-
-        allowed_type: Any = type(iterable[0])
-
-        if not all(isinstance(element, allowed_type) for element in iterable):
-            raise TypeError(
-                'Expected all elements to be of the same type.',
-            )
-
-    @staticmethod
     def __validate_ext_list(iterable: Any) -> None:
         if not isinstance(iterable, ExtList):
             raise TypeError(f'Expected <class \'ExtList\'> but got {type(iterable)}')
 
-    def __validate_same_type_element(self, element: T) -> None:
-        if not isinstance(element, type(self[0])):
-            raise TypeError(
-                f'Expected {type(self[0])} but got {type(element)}.',
-            )
-
-    def __validate_same_type_ext_list(self, other: ExtList[T]):
-        if not isinstance(self[0], type(other[0])):  # type: ignore[index]
-            raise TypeError(
-                f'Expected ExtList[{type(self[0])}] but got ExtList[{type(other[0])}].',  # type: ignore[index]
-            )
-
-    def __is_indexable(self) -> bool:
-        return hasattr(self[0], '__getitem__')
-
-    @staticmethod
-    def __get_value_by_function(element: T, func: FunctionType, *args: Any) -> Any:
-        return func(element, *args)
-
-    @staticmethod
-    def __get_value_by_index(element: T, index: Hashable | Hashable) -> Any:
-        return element[index]  # type: ignore
-
-    @staticmethod
-    def __get_value_by_property(element: T, prop: property) -> Any:
-        return prop.__get__(element)  # type: ignore[misc]
-
-    @staticmethod
-    def __get_value_by_attr_name(element: T, attr_name: str, *args: Any) -> Any:
-        object = getattr(element, attr_name)
-
-        if callable(object):
-            return object(*args)
-
-        return object
-
-    def __determine_get_value_method(self, key: FunctionType | property | str | Hashable) -> Callable[[T, Any], Any]:
-        if self.__is_indexable():
-            return ExtList.__get_value_by_index
-
-        if isinstance(key, FunctionType) or isinstance(key, MethodDescriptorType):
-            return ExtList.__get_value_by_function
-
-        if isinstance(key, property) or isinstance(key, GetSetDescriptorType):
-            return ExtList.__get_value_by_property
-
-        return ExtList.__get_value_by_attr_name
-
     @ override
     def __add__(self, other: ExtList[T]) -> ExtList[T]:  # type: ignore[override]
         self.__validate_ext_list(other)
 
         if not self:
             return other
 
         if not other:
             return self
 
-        self.__validate_same_type_ext_list(other)
-
         return ExtList(super().__add__(other))
 
     @ override
     def __iadd__(self, other: ExtList[T]) -> ExtList[T]:  # type: ignore[override]
         self.__validate_ext_list(other)
 
         if not self:
             super().__iadd__(other)
             return other
 
         if not other:
             super().__iadd__(other)
             return self
 
-        self.__validate_same_type_ext_list(other)
-
         super().__iadd__(other)
 
         return self
 
     @ override
     def append(self, element: T) -> None:
         if not self:
             super().append(element)
             return
 
-        self.__validate_same_type_element(element)
-
         super().append(element)
 
     @ override
     def extend(self, other: ExtList[T]) -> None:  # type: ignore[override]
         if not isinstance(other, ExtList):  # type: ignore
             raise TypeError(f'Expected ExtList but got {type(other)}')
 
         if not self:
             super().extend(other)
             return
 
         if not other:
             return
 
-        self.__validate_same_type_ext_list(other)
-
         super().extend(other)
 
     @ override
-    def insert(self, index: Hashable, element: T) -> None:
+    def insert(self, index: SupportsIndex, element: T) -> None:
         if not self:
             super().insert(index, element)
             return
 
-        self.__validate_same_type_element(element)
-
         super().insert(index, element)
 
+    @ override
     def extract(self, key: FunctionType | property | str | Hashable, *args: Any) -> ExtList[Any]:
         """
         Extracts and returns a list of values associated with the given key from the objects.
 
         Args:
             key (FunctionType | property | str | Hashable): The key to extract values for. If the key is function,
                 the callable will be executed and its result will be returned.
-            *args Any: If key is a function, the arguments will be passed to the function.
+            *args (Any): If key is a function, the arguments will be passed to the function.
 
         Returns:
-            ExtList: A list of values associated with the given key. If no values are found or the object
-                is empty, an empty ExtList is returned.
+            ExtList[Any]: A list of values associated with the given key.
 
         Examples:
             The following example demonstrates how to use the 'extract' method.
 
             >>> ext_list_1 = ExtList([{'a': 1}, {'a': 2}, {'a': 3}])
             >>> ext_list_1.extract('a')
             [1, 2, 3]
@@ -210,34 +140,148 @@
             ['Alice', 'Bob', 'Charlie']
 
             >>> ext_list_3.extract(Person.introduce)
             ['Alice is 25 years old.', 'Bob is 30 years old.', 'Charlie is 35 years old.']
 
             >>> ext_list_3.extract(Person.get_age_n_years_ago, 5)
             [20, 25, 30]
+
+        Overrides :meth:`_ListOperation.extract`.
         """
-        if not self:
-            return ExtList()
+        return self.__class__(super().extract(key, *args))
+
+    @ override
+    def extract_duplicates(self, other: ExtList[T]) -> ExtList[T]:  # type: ignore
+        """
+        Returns a list of objects that are in both the current object and the given object.
+
+        Args:
+            compare_ext_list (ExtList[T]): The object to compare the current object to.
+
+        Returns:
+            ExtList[T]: A list of objects that are in both the current object and the given object. If no objects are found
+            or the object is empty, an empty ExtList is returned.
+
+        Examples:
+            The following example demonstrates how to use the `extract_duplicates` method.
+
+            >>> ext_list_1 = ExtList([{'name': 'Alice', 'age': 25}, {'name': 'Bob', 'age': 30}])
+            >>> ext_list_2 = ExtList([{'name': 'Bob', 'age': 30}, {'name': 'Charlie', 'age': 35}])
+            >>> ext_list_1.extract_duplicates(ext_list_2)
+            [{'name': 'Bob', 'age': 30}]
+
+        Overrides :meth:`_ListOperation.extract_duplicates`.
+        """
+        return self.__class__(super().extract_duplicates(other))
+
+    @override
+    def is_duplicate(self) -> bool:
+        """
+        Returns `True` if there are any duplicates in the current object, `False` otherwise.
+
+        Returns:
+            bool: `True` if there are any duplicates in the current object, `False` otherwise.
+
+        Examples:
+            The following example demonstrates how to use the `is_duplicate` method.
+
+            >>> ext_list_1 = ExtList([{'name': 'Alice', 'age': 25}, {'name': 'Bob', 'age': 30}, {'name': 'Alice', 'age': 25}])
+            >>> ext_list_1.is_duplicate()
+            True
+
+            >>> ext_list_2 = ExtList([{'name': 'Alice', 'age': 25}, {'name': 'Bob', 'age': 30}, {'name': 'Charlie', 'age': 35}])
+            >>> ext_list_2.is_duplicate()
+            False
+
+        Overrides :meth:`_ListOperation.is_duplicate`.
+        """
+        return super().is_duplicate()
+
+    def one(self) -> T | None:
+        """
+        Returns the first object in the current object. If the object is empty, `None` is returned.
+
+        Returns:
+            T or None: The first object in the current object, or `None` if the object is empty.
+
+        Examples:
+            The following example demonstrates how to use the `one` method to return the first object in an ExtList:
+
+            >>> ext_list_1 = ExtList([1, 2, 3])
+            >>> ext_list_1.one()
+            1
+
+            The following example demonstrates how to use the `one` method to return `None` when the object is empty:
+
+            >>> ext_list_2 = ExtList([])
+            >>> ext_list_2.one()
+            None
+
+        Overrides :meth:`_ListOperation.one`.
+        """
+        return super().one()
+
+    def first(self) -> T:
+        """
+        Returns the first object in the current object.
+
+        Returns:
+            T: The first object in the current object.
+
+        Raises:
+            IndexError: If the object is empty.
+
+        Examples:
+            The following example demonstrates how to use the `first` method to return the first object in an ExtList:
+
+            >>> ext_list_1 = ExtList([1, 2, 3])
+            >>> ext_list_1.first()
+            1
+
+        Overrides :meth:`_ListOperation.first`.
+        """
+        return super().first()
+
+    @override
+    def map(self, function: FunctionType | type, *args: Any) -> ExtList[Any]:
+        """
+        Apply a function or constructor to each element.
+
+        Args:
+            function (FunctionType | type): The function or type to apply to each element.
+            *args (Any): Additional arguments to pass to the function or type.
+
+        Returns:
+            ExtList[Any]: A new ExtList containing the mapped values.
+
+        Examples:
+            The following example demonstrates how to use the `map` method.
 
-        get_value_method: Callable[[T, Any], Any] = self.__determine_get_value_method(key)
+            >>> ext_list_1 = ExtList([1, 2, 3])
+            >>> ext_list_1.map(float)
+            [1.0, 2.0, 3.0]
 
-        return ExtList([get_value_method(element, key, *args) for element in self])  # type: ignore[arg-type]
+        Overrides :meth:`_ListOperation.map`.
+        """
+        return self.__class__(super().map(function, *args))
 
-    def equals(self, key: FunctionType | property | str | Hashable, compare_target: Any, *args: Any) -> ExtList[T]:
+    @override
+    def equal(self, key: FunctionType | property | str | Hashable, compare_target: Any, *args: Any) -> ExtList[T]:
         """
         Returns a list of objects that have the given key set to the given value.
 
         Args:
-            key (FunctionType | property | str | Hashable): The key to search for.
+            key (FunctionType | property | str | Hashable): The key to compare values for. If the key is function,
+                the callable will be executed and its result will be returned.
             compare_target (Any): The value to compare the objects' values to.
-            *args Any: If key is a function, the arguments will be passed to the function.
+            *args (Any): If key is a function, the arguments will be passed to the function.
 
         Returns:
-            ExtList: A list of objects that have the given key set to the given value. If no objects are found or the object
-                is empty, an empty ExtList is returned.
+            ExtList[T]: A list of objects that have the given key set to the given value. If no objects are found or the object
+            is empty, an empty ExtList is returned.
 
         Examples:
             The following example demonstrates how to use the `equals` method.
 
             >>> ext_list_1 = ExtList([{'name': 'Alice', 'age': 25}, {'name': 'Bob', 'age': 30}, {'name': 'Charlie', 'age': 35}])
             >>> ext_list_1.equals('age', 25)
             [{'name': 'Alice', 'age': 25}]
@@ -251,37 +295,35 @@
             [, Person('Bob', 30), Person('David', 30)]
 
             >>> ext_list_3.equals(Person.introduce, 'Alice is 25 years old.')
             [Person('Alice', 25)]
 
             >>> ext_list_3.equals(Person.get_age_n_years_ago, 20, 5)
             [Person('Alice', 25)]
-        """
-        if not self:
-            return ExtList()
-
-        get_value_method: Callable[[T, Any], Any] = self.__determine_get_value_method(key)
 
-        if compare_target in {None, False, True}:
-            return ExtList([element for element in self if get_value_method(element, key, *args) is compare_target])  # type: ignore[arg-type]
-
-        return ExtList([element for element in self if get_value_method(element, key, *args) == compare_target])  # type: ignore[arg-type]
+        Overrides :meth:`_OperatorOperation.equal`.
+        """
+        return self.__class__(super().equal(key, compare_target, *args))
 
-    def not_equals(self, key: FunctionType | property | Hashable, compare_target: Any, *args: Any) -> ExtList[T]:
+    @override
+    def not_equal(self, key: FunctionType | property | Hashable, compare_target: Any, *args: Any) -> ExtList[T]:
         """
         Returns a list of objects that do not have the given key set to the given value.
 
         Args:
-            key (FunctionType | property | str | Hashable): The key to search for.
+            key (FunctionType | property | str | Hashable): The key to compare values for. If the key is function,
+                the callable will be executed and its result will be returned.
+
             compare_target (Any): The value to compare the objects' values to.
-            *args Any: If key is a function, the arguments will be passed to the function.
+
+            *args (Any): If key is a function, the arguments will be passed to the function.
 
         Returns:
-            ExtList: A list of objects that do not have the given key set to the given value. If no objects are found or the
-                object is empty, an empty ExtList is returned.
+            ExtList[T]: A list of objects that do not have the given key set to the given value.
+            If no objects are found or the object is empty, an empty ExtList is returned.
 
         Examples:
             The following example demonstrates how to use the `not_equals` method.
 
             >>> ext_list_1 = ExtList([{'name': 'Alice', 'age': 25}, {'name': 'Bob', 'age': 30}, {'name': 'Charlie', 'age': 35}])
             >>> ext_list_1.not_equals('age', 25)
             [{'name': 'Bob', 'age': 30}, {'name': 'Charlie', 'age': 35}]
@@ -295,336 +337,431 @@
             [Person('Alice', 25), Person('Charlie', 35)]
 
             >>> ext_list_3.not_equals(Person.introduce, 'Alice is 25 years old.')
             [Person('Bob', 30), Person('Charlie', 35), Person('David', 30)]
 
             >>> ext_list_3.not_equals(Person.get_age_n_years_ago, 20, 5)
             [Person('Bob', 30), Person('Charlie', 35), Person('David', 30)]
-        """
-        if not self:
-            return ExtList()
-
-        get_value_method: Callable[[T, Any], Any] = self.__determine_get_value_method(key)
 
-        if compare_target in {None, False, True}:
-            return ExtList([element for element in self if get_value_method(element, key, *args) is not compare_target])  # type: ignore[arg-type]
-
-        return ExtList([element for element in self if get_value_method(element, key, *args) != compare_target])  # type: ignore[arg-type]
+        Overrides :meth:`_OperatorOperation.not_equal`.
+        """
+        return self.__class__(super().not_equal(key, compare_target, *args))
 
-    def in_(self, key: FunctionType | property | str | Hashable, compare_targets: list[Any], *args: Any) -> ExtList[T]:
+    @override
+    def greater(self, key: FunctionType | property | Hashable, compare_target: Any, *args: Any) -> ExtList[T]:
         """
-        Returns a list of objects that have the given key set to one of the given values.
+        Return a list of objects that are greater than the specified compare_target, when the
+        object is passed through the provided key function, property or hashable key.
 
         Args:
-            key (FunctionType | property | str | Hashable): The key to search for.
-            compare_targets (list): A list of values to compare the objects' values to.
-            *args Any: If key is a function, the arguments will be passed to the function.
+            key (Union[FunctionType, property, Hashable]): The key to compare values for. If the key is function,
+                the callable will be executed and its result will be returned.
+            compare_target (Any): The value to compare against.
+            *args (Any): If key is a function, the arguments will be passed to the function.
 
         Returns:
-            ExtList: A list of objects that have the given key set to one of the given values. If no objects are found or
-                the object is empty, an empty ExtList is returned.
+            List[T]: A list of objects that are greater than the compare_target, when the
+            object is passed through the provided key.
 
         Examples:
-            The following example demonstrates how to use the `in_` method.
+            The following example demonstrates how to use the `greater` method.
 
             >>> ext_list_1 = ExtList([{'name': 'Alice', 'age': 25}, {'name': 'Bob', 'age': 30}, {'name': 'Charlie', 'age': 35}])
-            >>> ext_list_1.in_('age', [25, 30])
-            [{'name': 'Alice', 'age': 25}, {'name': 'Bob', 'age': 30}]
-
-            >>> ext_list_2 = ExtList([{'name': 'Alice', 'graduated': None}, {'name': 'Bob', 'graduated': False}, {'name': 'Charlie', 'graduated': True}])
-            >>> ext_list_2.in_('graduated', [False, True])
-            [{'name': 'Bob', 'graduated': False}, {'name': 'Charlie', 'graduated': True}]
+            >>> ext_list_1.greater('age', 30)
+            [{'name': 'Charlie', 'age': 35}]
 
-            >>> ext_list_3 = ExtList([Person('Alice', 25), Person('Bob', 30), Person('Charlie', 35)])
-            >>> ext_list_3.in_(Person.age, [25, 35])
-            [Person(Alice, 25), Person(Charlie, 35)]
+            >>> ext_list_2 = ExtList([Person('Alice', 25), Person('Bob', 30), Person('Charlie', 35), Person('David', 30)])
+            >>> ext_list_2.greater(Person.age, 30)
+            [Person('Charlie', 35)]
 
-            >>> ext_list_3.in_(Person.introduce, ['Alice is 25 years old.', 'Charlie is 35 years old.'])
-            [Person('Alice', 25), Person('Charlie', 35)]
+            >>> ext_list_2.greater(Person.get_age_n_years_ago, 25, 5)
+            [Person('Charlie', 35)]
 
-            >>> ext_list_3.in_(Person.get_age_n_years_ago, [20, 30], 5)
-            [Person('Alice', 25), Person('Charlie', 35)]
+        Overrides :meth:`_OperatorOperation.greater`.
         """
-        if not self:
-            return ExtList()
-
-        get_value_method: Callable[[T, Any], Any] = self.__determine_get_value_method(key)
-
-        return ExtList([element for element in self if get_value_method(element, key, *args) in compare_targets])  # type: ignore[arg-type]
+        return self.__class__(super().greater(key, compare_target, *args))
 
-    def not_in_(self, key: FunctionType | property | str | Hashable, compare_targets: list[Any], *args: Any) -> ExtList[T]:
+    @override
+    def greater_or_equal(self, key: FunctionType | property | Hashable, compare_target: Any, *args: Any) -> ExtList[T]:
         """
-        Returns a list of objects that do not have the given key set to any of the given values.
+        Return a list of objects that are greater than or equal the specified compare_target, when the
+        object is passed through the provided key function, property or hashable key.
 
         Args:
-            key (FunctionType | property | str | Hashable): The key to search for.
-            compare_targets (list): A list of values to compare the objects' values to.
-            *args Any: If key is a function, the arguments will be passed to the function.
+            key (Union[FunctionType, property, Hashable]): The key to compare values for. If the key is function,
+                the callable will be executed and its result will be returned.
+            compare_target (Any): The value to compare against.
+            *args (Any): Additional arguments to be passed to the key function.
 
         Returns:
-            ExtList: A list of objects that do not have the given key set to any of the given values. If no objects are
-                found or the object is empty, an empty ExtList is returned.
+            List[T]: A list of objects that are greater than or equal the compare_target, when the
+            object is passed through the provided key.
 
         Examples:
-            The following example demonstrates how to use the `not_in_` method:
+            The following example demonstrates how to use the `greater_or_equal` method.
 
             >>> ext_list_1 = ExtList([{'name': 'Alice', 'age': 25}, {'name': 'Bob', 'age': 30}, {'name': 'Charlie', 'age': 35}])
-            >>> ext_list_1.not_in_('age', [25, 30])
-            [{'name': 'Charlie', 'age': 35}]
-
-            >>> ext_list_2 = ExtList([{'name': 'Alice', 'graduated': None}, {'name': 'Bob', 'graduated': False}, {'name': 'Charlie', 'graduated': True}])
-            >>> ext_list_2.not_in_('graduated', [False, True])
-            [{'name': 'Alice', 'graduated': None}]
+            >>> ext_list_1.greater_or_equal('age', 30)
+            [{'name': 'Bob', 'age': 30}, {'name': 'Charlie', 'age': 35}]
 
-            >>> ext_list_3 = ExtList([Person('Alice', 25), Person('Bob', 30), Person('Charlie', 35)])
-            >>> ext_list_3.not_in_(Person.age, [25, 35])
-            [Person(Bob, 30)]
+            >>> ext_list_2 = ExtList([Person('Alice', 25), Person('Bob', 30), Person('Charlie', 35), Person('David', 30)])
+            >>> ext_list_2.greater_or_equal(Person.age, 30)
+            [Person('Bob', 30), Person('Charlie', 35), Person('David', 30)]
 
-            >>> ext_list_3.not_in_(Person.introduce, ['Alice is 25 years old.', 'Charlie is 35 years old.'])
-            [Person('Bob', 30)]
+            >>> ext_list_2.greater_or_equal(Person.get_age_n_years_ago, 25, 5)
+            [Person('Bob', 30), Person('Charlie', 35), Person('David', 30)]
 
-            >>> ext_list_3.not_in_(Person.get_age_n_years_ago, [20, 30], 5)
-            [Person('Bob', 30)]
+        Overrides :meth:`_OperatorOperation.greater_or_equal`.
         """
-        if not self:
-            return ExtList()
-
-        get_value_method: Callable[[T, Any], Any] = self.__determine_get_value_method(key)
-
-        return ExtList([element for element in self if get_value_method(element, key, *args) not in compare_targets])  # type: ignore[arg-type]
+        return self.__class__(super().greater_or_equal(key, compare_target, *args))
 
-    def extract_duplicates(self, other: ExtList[T]) -> ExtList[T]:
+    @override
+    def less(self, key: FunctionType | property | Hashable, compare_target: Any, *args: Any) -> ExtList[T]:
         """
-        Returns a list of objects that are in both the current object and the given object.
+        Return a list of objects that are less than the specified compare_target, when the
+        object is passed through the provided key function, property or hashable key.
 
         Args:
-            compare_ext_list (ExtList): The object to compare the current object to.
+            key (Union[FunctionType, property, Hashable]): The key to compare values for. If the key is function,
+                the callable will be executed and its result will be returned.
+            compare_target (Any): The value to compare against.
+            *args (Any): Additional arguments to be passed to the key function.
 
         Returns:
-            ExtList: A list of objects that are in both the current object and the given object. If no objects are found
-                or the object is empty, an empty ExtList is returned.
+            List[T]: A list of objects that are less than the compare_target, when the
+            object is passed through the provided key.
 
         Examples:
-            The following example demonstrates how to use the `extract_duplicates` method.
+            The following example demonstrates how to use the `less` method.
 
-            >>> ext_list_1 = ExtList([{'name': 'Alice', 'age': 25}, {'name': 'Bob', 'age': 30}])
-            >>> ext_list_2 = ExtList([{'name': 'Bob', 'age': 30}, {'name': 'Charlie', 'age': 35}])
-            >>> ext_list_1.extract_duplicates(ext_list_2)
-            [{'name': 'Bob', 'age': 30}]
+            >>> ext_list_1 = ExtList([{'name': 'Alice', 'age': 25}, {'name': 'Bob', 'age': 30}, {'name': 'Charlie', 'age': 35}])
+            >>> ext_list_1.less('age', 30)
+            [{'name': 'Alice', 'age': 25}]
+
+            >>> ext_list_2 = ExtList([Person('Alice', 25), Person('Bob', 30), Person('Charlie', 35), Person('David', 30)])
+            >>> ext_list_2.less(Person.age, 30)
+            [Person('Alice', 25)]
+
+            >>> ext_list_2.less(Person.get_age_n_years_ago, 25, 5)
+            [Person('Alice', 25)]
+
+        Overrides :meth:`_OperatorOperation.less`.
         """
-        return ExtList([element for element in self if element in other])
+        return self.__class__(super().less(key, compare_target, *args))
 
-    def is_duplicate(self) -> bool:
+    @override
+    def less_or_equal(self, key: FunctionType | property | Hashable, compare_target: Any, *args: Any) -> ExtList[T]:
         """
-        Returns `True` if there are any duplicates in the current object, `False` otherwise.
+        Return a list of objects that are less than or equal the specified compare_target, when the
+        object is passed through the provided key function, property or hashable key.
+
+        Args:
+            key (Union[FunctionType, property, Hashable]): The key to compare values for. If the key is function,
+                the callable will be executed and its result will be returned.
+            compare_target (Any): The value to compare against.
+            *args (Any): Additional arguments to be passed to the key function.
 
         Returns:
-            bool: `True` if there are any duplicates in the current object, `False` otherwise.
+            List[T]: A list of objects that are less than or equal the compare_target, when the
+            object is passed through the provided key.
 
         Examples:
-            The following example demonstrates how to use the `is_duplicate` method.
-
-            >>> ext_list_1 = ExtList([{'name': 'Alice', 'age': 25}, {'name': 'Bob', 'age': 30}, {'name': 'Alice', 'age': 25}])
-            >>> ext_list_1.is_duplicate()
-            True
+            The following example demonstrates how to use the `less_or_equal` method.
 
-            >>> ext_list_2 = ExtList([{'name': 'Alice', 'age': 25}, {'name': 'Bob', 'age': 30}, {'name': 'Charlie', 'age': 35}])
-            >>> ext_list_2.is_duplicate()
-            False
-        """
-        if not self:
-            return False
+            >>> ext_list_1 = ExtList([{'name': 'Alice', 'age': 25}, {'name': 'Bob', 'age': 30}, {'name': 'Charlie', 'age': 35}])
+            >>> ext_list_1.less_or_equal('age', 30)
+            [{'name': 'Alice', 'age': 25}, {'name': 'Bob', 'age': 30}]
 
-        tmp_ext_list: ExtList[T] = copy.deepcopy(self)
+            >>> ext_list_2 = ExtList([Person('Alice', 25), Person('Bob', 30), Person('Charlie', 35), Person('David', 30)])
+            >>> ext_list_2.less_or_equal(Person.age, 30)
+            [Person('Alice', 25), Person('Bob', 30), Person('David', 30)]
 
-        for _ in range(len(tmp_ext_list)):
-            if tmp_ext_list.pop() in tmp_ext_list:
-                return True
+            >>> ext_list_2.less_or_equal(Person.get_age_n_years_ago, 25, 5)
+            [Person('Alice', 25), Person('Bob', 30), Person('David', 30)]
 
-        return False
+        Overrides :meth:`_OperatorOperation.less_or_equal`.
+        """
+        return self.__class__(super().less_or_equal(key, compare_target, *args))
 
-    def one(self) -> T | None:
+    @override
+    def in_(self, key: FunctionType | property | str | Hashable, compare_target: list[Any], *args: Any) -> ExtList[T]:
         """
-        Returns the first object in the current object. If the object is empty, `None` is returned.
+        Returns a list of objects that have the given key set to one of the given values.
+
+        Args:
+            key (FunctionType | property | str | Hashable): The key to compare values for. If the key is function,
+                the callable will be executed and its result will be returned.
+            compare_targets (list): A list of values to compare the objects' values to.
+            *args Any: If key is a function, the arguments will be passed to the function.
 
         Returns:
-            T or None: The first object in the current object, or `None` if the object is empty.
+            ExtList[T]: A list of objects that have the given key set to one of the given values. If no objects are found or
+            the object is empty, an empty ExtList is returned.
 
         Examples:
-            The following example demonstrates how to use the `one` method to return the first object in an ExtList:
+            The following example demonstrates how to use the `in_` method.
 
-            >>> ext_list_1 = ExtList([1, 2, 3])
-            >>> ext_list_1.one()
-            1
+            >>> ext_list_1 = ExtList([{'name': 'Alice', 'age': 25}, {'name': 'Bob', 'age': 30}, {'name': 'Charlie', 'age': 35}])
+            >>> ext_list_1.in_('age', [25, 30])
+            [{'name': 'Alice', 'age': 25}, {'name': 'Bob', 'age': 30}]
 
-            The following example demonstrates how to use the `one` method to return `None` when the object is empty:
+            >>> ext_list_2 = ExtList([{'name': 'Alice', 'graduated': None}, {'name': 'Bob', 'graduated': False}, {'name': 'Charlie', 'graduated': True}])
+            >>> ext_list_2.in_('graduated', [False, True])
+            [{'name': 'Bob', 'graduated': False}, {'name': 'Charlie', 'graduated': True}]
 
-            >>> ext_list_2 = ExtList([])
-            >>> ext_list_2.one()
-            None
+            >>> ext_list_3 = ExtList([Person('Alice', 25), Person('Bob', 30), Person('Charlie', 35)])
+            >>> ext_list_3.in_(Person.age, [25, 35])
+            [Person(Alice, 25), Person(Charlie, 35)]
+
+            >>> ext_list_3.in_(Person.introduce, ['Alice is 25 years old.', 'Charlie is 35 years old.'])
+            [Person('Alice', 25), Person('Charlie', 35)]
+
+            >>> ext_list_3.in_(Person.get_age_n_years_ago, [20, 30], 5)
+            [Person('Alice', 25), Person('Charlie', 35)]
+
+        Overrides :meth:`_OperatorOperation.in_`.
         """
-        try:
-            return self[0]
-        except IndexError:
-            return None
+        return self.__class__(super().in_(key, compare_target, *args))
 
-    def first(self) -> T:
+    @override
+    def not_in_(self, key: FunctionType | property | str | Hashable, compare_target: list[Any], *args: Any) -> ExtList[T]:
         """
-        Returns the first object in the current object.
+        Returns a list of objects that do not have the given key set to any of the given values.
 
-        Returns:
-            T: The first object in the current object.
+        Args:
+            key (FunctionType | property | str | Hashable): The key to compare values for. If the key is function,
+                the callable will be executed and its result will be returned.
+            compare_targets (list): A list of values to compare the objects' values to.
+            *args (Any): If key is a function, the arguments will be passed to the function.
 
-        Raises:
-            IndexError: If the object is empty.
+        Returns:
+            ExtList[T]: A list of objects that do not have the given key set to any of the given values. If no objects are
+            found or the object is empty, an empty ExtList is returned.
 
         Examples:
-            The following example demonstrates how to use the `first` method to return the first object in an ExtList:
+            The following example demonstrates how to use the `not_in_` method:
 
-            >>> ext_list_1 = ExtList([1, 2, 3])
-            >>> ext_list_1.first()
-            1
+            >>> ext_list_1 = ExtList([{'name': 'Alice', 'age': 25}, {'name': 'Bob', 'age': 30}, {'name': 'Charlie', 'age': 35}])
+            >>> ext_list_1.not_in_('age', [25, 30])
+            [{'name': 'Charlie', 'age': 35}]
+
+            >>> ext_list_2 = ExtList([{'name': 'Alice', 'graduated': None}, {'name': 'Bob', 'graduated': False}, {'name': 'Charlie', 'graduated': True}])
+            >>> ext_list_2.not_in_('graduated', [False, True])
+            [{'name': 'Alice', 'graduated': None}]
 
+            >>> ext_list_3 = ExtList([Person('Alice', 25), Person('Bob', 30), Person('Charlie', 35)])
+            >>> ext_list_3.not_in_(Person.age, [25, 35])
+            [Person(Bob, 30)]
+
+            >>> ext_list_3.not_in_(Person.introduce, ['Alice is 25 years old.', 'Charlie is 35 years old.'])
+            [Person('Bob', 30)]
+
+            >>> ext_list_3.not_in_(Person.get_age_n_years_ago, [20, 30], 5)
+            [Person('Bob', 30)]
+
+        Overrides :meth:`_OperatorOperation.not_in_`.
         """
-        return self[0]
+        return self.__class__(super().not_in_(key, compare_target, *args))
 
+    @override
     def to_dict(self, key: FunctionType | property | str | Hashable, *args: Any) -> dict[Hashable, T]:
         """
         Converts the current object to a dictionary, using the given key as the dictionary key.
 
         Args:
-            key (FunctionType | property | str | Hashable): The key to use as the dictionary key.
+            key (FunctionType | property | str | Hashable): The key to use as the dictionary key. If the key is function,
+                the callable will be executed and its result will be returned.
             *args Any: If key is a function, the arguments will be passed to the function.
 
         Returns:
-            dict: A dictionary of objects, using the given key as the dictionary key.
+            dict[Hashable, T]: A dictionary of objects, using the given key as the dictionary key.
 
         Examples:
-            The following example demonstrates how to use the `to_dict` method to convert an ExtList of dictionaries to a
-            dictionary:
+            The following example demonstrates how to use the `to_dict` method.
 
             >>> ext_list_1 = ExtList([{'name': 'Alice', 'age': 25}, {'name': 'Bob', 'age': 30}])
             >>> ext_list_1.to_dict('name')
             {'Alice': {'name': 'Alice', 'age': 25}, 'Bob': {'name': 'Bob', 'age': 30}}
 
-            The following example demonstrates how to use the `to_dict` method to convert an ExtList of lists to a
-            dictionary:
-
             >>> ext_list_2 = ExtList([['Alice', 25], ['Bob', 30]])
             >>> ext_list_2.to_dict(0)
             {'Alice': ['Alice', 25], 'Bob': ['Bob', 30]}
 
-            The following example demonstrates how to use the `to_dict` method to convert an ExtList of objects to a
-            dictionary:
-
             >>> ext_list_3 = ExtList([Person('Alice', 25), Person('Bob', 30)])
             >>> ext_list_3.to_dict(Person.name)
             {'Alice': Person('Alice', 25), 'Bob': Person('Bob', 30)}
 
             >>> ext_list_3.to_dict(Person.get_age_n_years_ago, 5)
             {20: Person('Alice', 25), 25: Person('Bob', 30)}
+
+        Overrides :meth:`_DictOperation.to_dict`.
         """
-        if not self:
-            return {}
+        return super().to_dict(key, *args)
+
+    @override
+    def to_dict_list(self, keys: list[FunctionType | property | str | Hashable], arg_tuples: list[tuple[Any, ...]] = []) -> ExtList[dict[str | Hashable, Any]]:
+        """
+        Converts the objects into a list of dictionaries, where each dictionary contains the specified keys
+        and their corresponding values from the object.
+
+        Args:
+            keys (list[FunctionType | property | str | Hashable]): A list of keys to include in the dictionaries. Each key can
+                be a function, property, string, or hashable object.
+            arg_tuples (list[tuple[Any, ...]], optional): A list of argument tuples. Each tuple contains the arguments to be
+                passed to the corresponding key function or property. Defaults to an empty list.
+
+        Returns:
+            ExtList[dict[str | Hashable, Any]]: A list of dictionaries, where each dictionary represents an element and contains
+            the specified keys and their corresponding values.
+
+        Examples:
+            The following example demonstrates how to use the `to_dict_list` method.
+
+            >>> ext_list_1 = ExtList([{'name': 'Alice', 'age': 25}, {'name': 'Bob', 'age': 30}])
+            >>> ext_list_1.to_dict_list(['name'])
+            [{'name': 'Alice'}, {'name': 'Bob'}]
+
+            >>> ext_list_2 = ExtList([['Alice', 25], ['Bob', 30]])
+            >>> ext_list_2.to_dict_list([0])
+            [{0: 'Alice'}, {0: 'Bob'}]
 
-        get_value_method: Callable[[T, Any], Any] = self.__determine_get_value_method(key)
+            >>> ext_list_3 = ExtList([Person('Alice', 25), Person('Bob', 30)])
+            >>> ext_list_3.to_dict_list([Person.name, Person.get_age_n_years_ago], [(), (5,)])
+            [{'name': 'Alice', 'get_age_n_years_ago': 20}, {'name': 'Bob', 'get_age_n_years_ago': 25}]
 
-        return {get_value_method(element, key, *args): element for element in self}  # type: ignore[arg-type]
+        Overrides :meth:`_DictOperation.to_dict_list`.
+        """
+        return self.__class__(super().to_dict_list(keys, arg_tuples))
 
-    def to_dict_with_complex_keys(self, keys: list[FunctionType | property | str] | list[Hashable], arg_tuples: tuple[tuple[Any, ...], ...] = tuple()) -> dict[tuple[Any, ...], T]:
+    @override
+    def to_dict_with_complex_keys(self, keys: list[FunctionType | property | str] | list[Hashable], arg_tuples: list[tuple[Any, ...]] = []) -> dict[tuple[Any, ...], T]:
         """
-        Returns a dictionary of the elements in the `ExtList` with complex keys.
+        Returns a dictionary of the objects in the `ExtList` with complex keys.
 
         Args:
             keys (List[FunctionType | property | str] | List[Hashable]): A list of the keys for the dictionary.
             arg_tuples (Tuple[Tuple[Any,...],...]): A list of tuples of the arguments. If key is a function, the arguments will be passed to the function.
 
         Returns:
-            Dict[Tuple[Any, ...], T]: A dictionary of the elements in the `ExtList` with complex keys.
+            Dict[Tuple[Any, ...], T]: A dictionary of the objects in the `ExtList` with complex keys.
 
         Examples:
             The following example demonstrates how to use the `to_dict_with_complex_keys` method.
 
             >>> ext_list_1 = ExtList([Person('Alice', 25), Person('Bob', 30), Person('Charlie', 35), Person('David', 30)])
             >>> ext_list_1.to_dict_with_complex_keys([Person.name, Person.age])
             {('Alice', 25): Person('Alice', 25),
              ('Bob', 30): Person('Bob', 30),
              ('Charlie', 35): Person('Charlie', 35),
              ('David', 30): Person('David', 30)}
 
-            >>> ext_list_1.to_dict_with_complex_keys(['name', Person.introduce, Person.get_age_n_years_ago], ((), (), (5,)))
+            >>> ext_list_1.to_dict_with_complex_keys(['name', Person.introduce, Person.get_age_n_years_ago], [(), (), (5,)])
             {('Alice', 'Alice is 25 years old.', 20): Person('Alice', 25),
              ('Bob', 'Bob is 30 years old.', 25): Person('Bob', 30),
              ('Charlie', 'Charlie is 35 years old.', 30): Person('Charlie', 35),
              ('David', 'David is 30 years old.', 25): Person('David', 30)}
+
+        Overrides :meth:`_DictOperation.to_dict_with_complex_keys`.
         """
+        return super().to_dict_with_complex_keys(keys, arg_tuples)
 
-        if not self:
-            return {}
+    @override
+    def dicts_to_instances(self, type_: TI) -> ExtList[TI]:  # type: ignore[override]
+        """
+        Convert a list of dictionaries to a list of instances of the given class.
 
-        if self.__is_indexable():
-            return self.__to_dict_with_complex_keys_from_indexable_object(keys)  # type: ignore[arg-type]
+        Args:
+            type_ (Type[TI]): The type of the instances to create.
 
-        return self.__to_dict_with_complex_keys_from_others(keys, arg_tuples)  # type: ignore[arg-type]
+        Returns:
+            ExtList[TI]: A new ExtList containing the instances.
 
-    def __to_dict_with_complex_keys_from_indexable_object(self, keys: list[Hashable]) -> dict[tuple[Any, ...], T]:
-        return {tuple(element[key] for key in keys): element for element in self}  # type: ignore[index]
+        Examples:
+            The following example demonstrates how to use the `dicts_to_instances` method.
 
-    def __to_dict_with_complex_keys_from_others(self, keys: list[FunctionType | property | str], arg_tuples: tuple[tuple[Any, ...]]) -> dict[tuple[Any, ...], T]:
-        result: dict[tuple[Any, ...], T] = {}
+            >>> ext_list_1 = ExtList([{'name': 'alice', 'age': 25}, {'name': 'bob', 'age': 30}, {'name': 'charlie', 'age': 35}])
+            >>> ext_list_1.dicts_to_instances(Person)
+            [Person('alice', 25), Person('bob', 30), Person('charlie', 35)]
 
-        if not arg_tuples:
-            arg_tuples = tuple(tuple() for _ in range(len(keys)))
+        Overrides :meth:`_DictOperation.dicts_to_instances`.
+        """
+        return self.__class__(super().dicts_to_instances(type_))
 
-        for element in self:
-            tupled_key: tuple[Any, ...] = self.__generate_tupled_key(keys, element, arg_tuples)
-            result[tupled_key] = element
+    @override
+    def group_by_key(self, key: FunctionType | property | str | Hashable, *args: Any) -> dict[Hashable, ExtList[T]]:  # type: ignore[override]
+        """Groups the objects of the list by a specified key.
 
-        return result
+        Args:
+            key (FunctionType | property | str | Hashable): The key to group the objects by. This can be
+                a function, property, string, or hashable object.
+            *args (Any): Additional arguments to pass to the key function or property.
 
-    def __generate_tupled_key(self, keys: list[FunctionType | property | str], element: T, arg_tuples: tuple[Any]) -> tuple[Any, ...]:
-        tupled_key: tuple[Any, ...] = tuple()
+        Returns:
+            dict[Hashable, ExtList[T]]: A dictionary of lists, where the keys are the result of applying the
+            key function or property to the objects of the list, and the values are lists of objects
+            with the same key.
 
-        for key, arg_tuple in zip(keys, arg_tuples):
-            get_value_method = self.__determine_get_value_method(key)
-            tupled_key += (get_value_method(element, key, *arg_tuple),)
+        Examples:
+            The following example demonstrates how to use the `dicts_to_instances` method.
 
-        return tupled_key
+            >>> ext_list_1 = ExtList([{'name': 'alice', 'age': 25}, {'name': 'bob', 'age': 30}, {'name': 'charlie', 'age': 35}, {'name': 'david', 'age': 30}])
+            >>> ext_list_1.group_by_key('age')
+            {25: [{'name': 'alice', 'age': 25}], 30: [{'name': 'bob', 'age': 30}, {'name': 'david', 'age': 30}], 35: [{'name': 'charlie', 'age': 35}]}
 
-    def map(self, function: FunctionType | type, *args: Any) -> ExtList[Any]:
+        Overrides :meth:`_DictOperation.group_by_key`.
         """
-        Apply a function or constructor to each element.
+        return super().group_by_key(key, *args)  # type: ignore[assignment]
+
+    @override
+    def rename_keys(self, rename_keys: dict[Hashable, Hashable]) -> ExtList[T]:
+        """
+        Renames the keys in the objects based on the provided mapping dictionary.
 
         Args:
-            function (FunctionType | type): The function to apply to each element.
-            *args (Any): Additional arguments to pass to the function.
+            rename_keys (dict[Hashable, Hashable]): A dictionary that maps the keys to be renamed. The keys in the dictionary
+                represent the original keys, while the corresponding values represent the new keys.
 
         Returns:
-            ExtList[Any]: A new ExtList containing the mapped values.
+            ExtList[T]: A list of objects with the renamed keys.
+
+        Raises:
+            TypeError: If the object is not indexable.
 
         Examples:
-            The following example demonstrates how to use the `map` method.
+            >>> ext_list = ExtList([{'name': 'alice', 'age': 25}, {'name': 'bob', 'age': 30}])
+            >>> ext_list.rename_keys({'name': 'Name', 'age': 'Age'})
+            [{'Name': 'alice', 'Age': 25}, {'Name': 'bob', 'Age': 30}]
 
-            >>> ext_list_1 = ExtList([1, 2, 3])
-            >>> ext_list_1.map(float)
-            [1.0, 2.0, 3.0]
+        Overrides :meth:`_DictOperation.rename_keys`.
         """
-        return ExtList([function(element, *args) for element in self])
+        return self.__class__(super().rename_keys(rename_keys))
 
-    def dicts_to_instances(self: ExtList[dict[str, Any]], type_: TI) -> ExtList[TI]:
+    @override
+    def map_for_keys(self, keys: list[Hashable], function: Callable[[Any], Any] | type, *args: Any) -> ExtList[dict[Any, Any]]:
         """
-        Convert a list of dictionaries to a list of instances of the given class.
+        Applies a function to specific keys of each element in the dictionary.
 
         Args:
-            type_ (Type[TI]): The type of the instances to create.
+            keys (list[Hashable]): A list of hashable keys to apply the function to.
+            function (Callable[[Any], Any] | type): The function or type to apply to the keys.
+                It should accept the value of each key as the first argument, followed by optional args.
+            *args (Any): Optional arguments to be passed to the function along with each key's value.
 
         Returns:
-            ExtList[TI]: A new ExtList containing the instances.
+            An instance of ExtList containing the modified dictionaries.
 
-        Examples:
-            The following example demonstrates how to use the `dicts_to_instances` method.
+        Raises:
+            TypeError: If the dictionary is not indexable.
 
-            >>> ext_list_1 = ExtList([{'name': 'alice', 'age': 25}, {'name': 'bob', 'age': 30}, {'name': 'charlie', 'age': 35}])
-            >>> ext_list_1.dicts_to_instances(Person)
-            [Person('alice', 25), Person('bob', 30), Person('charlie', 35)]
+        Example:
+            The following example demonstrates how to use the `map_for_keys` method.
+
+            >>> ext_list = ExtList([{'a': 1, 'b': 2, 'c': 3}])
+            >>> keys = ['a', 'b']
+            >>> function = lambda x, y: x + y
+            >>> args = (10,)
+            >>> ext_list.map_for_keys(keys, function, *args)
+            {'a': 11, 'b': 12, 'c': 3}
+
+        Overrides :meth:`_DictOperation.map_for_keys`.
         """
-        return ExtList([type_(**element) for element in self])
+        return ExtList(super().map_for_keys(keys, function, *args))
```

### Comparing `ext-list-1.0.0/setup.py` & `ext-list-1.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,38 +3,38 @@
 from setuptools import setup
 
 with open('README.md', encoding='utf-8') as readme_md:
     long_description = readme_md.read()
 
 setup(
     name='ext-list',
-    version='1.0.0',
+    version='1.1.0',
     author='Sakaguchi Ryo',
     author_email='sakaguchi@sk-techfirm.com',
     description='This is a utility library that extends Python\'s list operations.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/sk-guritech/ext-list',
     project_urls={
         'Bug Tracker': 'https://github.com/sk-guritech/ext-list/issues',
     },
     classifiers=[
         'Topic :: Software Development :: Libraries :: Python Modules',
-        'Development Status :: 5 - Production/Stable',
+        'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Typing :: Typed',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12',
     ],
     keywords=['list', 'comprehension', 'iterable', 'code quality'],
-    packages=['.'],
+    packages=['ext_list'],
     python_requires='>=3.7',
     install_requires=['typing_extensions'],
 )
```

