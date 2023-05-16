# Comparing `tmp/anyjsonthing-0.3.1.tar.gz` & `tmp/anyjsonthing-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anyjsonthing-0.3.1.tar", last modified: Mon Apr 24 09:14:19 2023, max compression
+gzip compressed data, was "anyjsonthing-0.4.0.tar", last modified: Tue May 16 19:20:40 2023, max compression
```

## Comparing `anyjsonthing-0.3.1.tar` & `anyjsonthing-0.4.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:19.009360 anyjsonthing-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-24 09:13:19.000000 anyjsonthing-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-04-24 09:14:19.009360 anyjsonthing-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-04-24 09:13:19.000000 anyjsonthing-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-04-24 09:13:19.000000 anyjsonthing-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-24 09:14:19.013360 anyjsonthing-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:19.005360 anyjsonthing-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:19.009360 anyjsonthing-0.3.1/src/main/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:19.009360 anyjsonthing-0.3.1/src/main/anyjsonthing/
--rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-04-24 09:13:19.000000 anyjsonthing-0.3.1/src/main/anyjsonthing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-04-24 09:13:19.000000 anyjsonthing-0.3.1/src/main/anyjsonthing/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    21999 2023-04-24 09:13:19.000000 anyjsonthing-0.3.1/src/main/anyjsonthing/serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8395 2023-04-24 09:13:19.000000 anyjsonthing-0.3.1/src/main/anyjsonthing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:19.009360 anyjsonthing-0.3.1/src/main/anyjsonthing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-04-24 09:14:18.000000 anyjsonthing-0.3.1/src/main/anyjsonthing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-24 09:14:19.000000 anyjsonthing-0.3.1/src/main/anyjsonthing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 09:14:18.000000 anyjsonthing-0.3.1/src/main/anyjsonthing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-24 09:14:18.000000 anyjsonthing-0.3.1/src/main/anyjsonthing.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:20:40.881385 anyjsonthing-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-16 19:19:53.000000 anyjsonthing-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-05-16 19:20:40.881385 anyjsonthing-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-05-16 19:19:53.000000 anyjsonthing-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-16 19:19:53.000000 anyjsonthing-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-16 19:20:40.881385 anyjsonthing-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:20:40.877384 anyjsonthing-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:20:40.877384 anyjsonthing-0.4.0/src/main/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:20:40.877384 anyjsonthing-0.4.0/src/main/anyjsonthing/
+-rw-r--r--   0 runner    (1001) docker     (123)     8817 2023-05-16 19:19:53.000000 anyjsonthing-0.4.0/src/main/anyjsonthing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6183 2023-05-16 19:19:53.000000 anyjsonthing-0.4.0/src/main/anyjsonthing/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24705 2023-05-16 19:19:53.000000 anyjsonthing-0.4.0/src/main/anyjsonthing/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8395 2023-05-16 19:19:53.000000 anyjsonthing-0.4.0/src/main/anyjsonthing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:20:40.877384 anyjsonthing-0.4.0/src/main/anyjsonthing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-05-16 19:20:40.000000 anyjsonthing-0.4.0/src/main/anyjsonthing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-16 19:20:40.000000 anyjsonthing-0.4.0/src/main/anyjsonthing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 19:20:40.000000 anyjsonthing-0.4.0/src/main/anyjsonthing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-16 19:20:40.000000 anyjsonthing-0.4.0/src/main/anyjsonthing.egg-info/top_level.txt
```

### Comparing `anyjsonthing-0.3.1/LICENSE` & `anyjsonthing-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `anyjsonthing-0.3.1/PKG-INFO` & `anyjsonthing-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anyjsonthing
-Version: 0.3.1
+Version: 0.4.0
 Summary: A library that implements serialization of simple data objects as JSON data.
 Home-page: https://github.com/phohenecker/anyjsonthing
 Author: Patrick Hohenecker
 Author-email: patrick.hohenecker@gmx.at
 License: Simplified BSD License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `anyjsonthing-0.3.1/README.md` & `anyjsonthing-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `anyjsonthing-0.3.1/pyproject.toml` & `anyjsonthing-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `anyjsonthing-0.3.1/setup.cfg` & `anyjsonthing-0.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `anyjsonthing-0.3.1/src/main/anyjsonthing/__init__.py` & `anyjsonthing-0.4.0/src/main/anyjsonthing/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -119,14 +119,34 @@
    assert json_data == {"a": "A", "b": "B"}
 
    # Step 2: deserialize the JSON data
    reconstructed = anyjsonthing.Serializer.from_json(AnotherDataClass, json_data)
    assert str(reconstructed) != str(some_instance)
    assert str(reconstructed) == str(AnotherDataClass("A", "B"))
 
+Another issue that we frequently encounter in practice is that JSON data which needs to be deserialized contains
+additional object properties that do not exist in the target dataclass or normal class, respectively. To handle this
+specific use case, the :meth:`~anyjsonthing.serializer.Serializer.from_json` method has an optional parameter
+``ignore_unknown_props``, which allows for specifying that such additional properties should simply be ignored. This is
+illustrated in the following example:
+
+.. code-block:: python
+
+   import anyjsonthing
+   from dataclasses import dataclass
+
+   @dataclass
+   class MyDataClass:
+       a: str
+
+   deserialized = anyjsonthing.Serializer.from_json(MyDataClass, {"a": "A", "b": "B"})  # -> ERROR!
+   deserialized = anyjsonthing.Serializer.from_json(MyDataClass, {"a": "A", "b": "B"}, ignore_unknown_props=True)
+   assert deserialized == MyDataClass("A")
+
+
 Finally, the :mod:`anyjsonthing` library provides the class :class:`~anyjsonthing.io.IO`, which combines the
 functionality implemented by the :class:`~anyjsonthing.serializer.Serializer` with read/write operations. This allows
 for directly serializing data objects to the disk, and thus covers the main use case targeted by :mod:`anyjsonthing`.
 The following example illustrates how to use the :class:`~anyjsonthing.io.IO` class (for additional details on all
 available I/O methods, please have a look at the API docs of :class:`~anyjsonthing.io.IO`):
 
 .. code-block:: python
```

### Comparing `anyjsonthing-0.3.1/src/main/anyjsonthing/io.py` & `anyjsonthing-0.4.0/src/main/anyjsonthing/io.py`

 * *Files 20% similar despite different names*

```diff
@@ -84,37 +84,44 @@
                 [serializer.Serializer.to_json(x) for x in anything]
         )
 
         target_path = pathlib.Path(path)
         target_path.write_text(json_data)
 
     @staticmethod
-    def load(cls: type[_T], path: os.PathLike) -> _T:
+    def load(cls: type[_T], path: os.PathLike, ignore_unknown_props: bool = False) -> _T:
         """Loads and deserialized the JSON representation a single instance of ``cls`` from the specified ``path``.
 
         Args:
             cls: The :class:`type` of the deserialized instance.
             path: The path that the deserialized JSON representation is loaded from.
+            ignore_unknown_props: Indicates whether superfluous JSON object properties encountered during
+                deserialization of the loaded JSON data should be ignored as opposed to raising an error.
 
         Returns:
             The created instance of the specified ``cls``.
         """
 
         source_path = pathlib.Path(path)
         json_data = json.loads(source_path.read_text())
-        return serializer.Serializer.from_json(cls, json_data)
+        return serializer.Serializer.from_json(cls, json_data, ignore_unknown_props=ignore_unknown_props)
 
     @staticmethod
-    def load_all(cls: type[_T], path: os.PathLike) -> list[_T]:
+    def load_all(cls: type[_T], path: os.PathLike, ignore_unknown_props: bool = False) -> list[_T]:
         """Loads and deserialized the JSON representation of multiple instances of ``cls`` from the specified ``path``.
 
         Args:
             cls: The :class:`type` of the deserialized instance.
             path: The path that the deserialized JSON representation is loaded from.
+            ignore_unknown_props: Indicates whether superfluous JSON object properties encountered during
+                deserialization of the loaded JSON data should be ignored as opposed to raising an error.
 
         Returns:
             A :class:`list` of all created instances of the specified ``cls``.
         """
 
         source_path = pathlib.Path(path)
         json_data = json.loads(source_path.read_text())
-        return [serializer.Serializer.from_json(cls, x) for x in json_data]
+        return [
+                serializer.Serializer.from_json(cls, x, ignore_unknown_props=ignore_unknown_props)
+                for x in json_data
+        ]
```

### Comparing `anyjsonthing-0.3.1/src/main/anyjsonthing/serializer.py` & `anyjsonthing-0.4.0/src/main/anyjsonthing/serializer.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 #   NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS                #
 #   SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.                      #
 #                                                                                     #
 # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
 
 import collections
+import copy
 import itertools
 import types
 import typing
 
 import anyjsonthing.utils as utils
 
 from typing import Any
@@ -128,30 +129,33 @@
                 return False
 
         # If we arrive at this point, we successfully confirmed that there are attributes/properties for all args needed
         # to reconstruct anything.
         return True
 
     @staticmethod
-    def from_json(cls: type[_T], json: dict[str, Any]) -> _T:
+    def from_json(cls: type[_T], json: dict[str, Any], ignore_unknown_props: bool = False) -> _T:
         """Deserializes the provided ``json`` data into an instance of the specified ``cls``.
 
         Args:
             cls: The :class:`type` of the instance that is described by the provided ``json`` data.
             json: The JSON representation of the instance that is deserialized.
+            ignore_unknown_props: Indicates whether superfluous object properties in the given ``json`` data (which do
+                not exist in the ``cls``) should be ignored as opposed to raising an error.
 
         Returns:
             The deserialized instance of ``cls``.
 
         Raises:
             ValueError: If the ``json`` data is missing a required arg of the ``__init__`` method of the target ``cls``
-                or if it specifies properties that are unknown to the latter.
+                (or any nested type) or if ``ignore_unknown_props`` is ``False`` and it specifies properties that are
+                unknown to the latter.
         """
 
-        return Serializer._dejsonify(json, cls)
+        return Serializer._dejsonify(json, type_annotation=cls, ignore_unknown_props=ignore_unknown_props)
 
     @classmethod
     def to_json(cls, anything: Any, strict: bool = True) -> Any:
         """Serializes ``anything``, creating a JSON representation of the same.
 
         Args:
             anything: The data object that is serialized as JSON data.
@@ -172,21 +176,24 @@
 
         return cls._jsonify(anything)
 
     @classmethod
     def _dejsonify(
             cls,
             anything: Any,
-            type_annotation: Union[None, type, types.GenericAlias, typing._GenericAlias] = None
+            type_annotation: Union[None, type, types.GenericAlias, typing._GenericAlias] = None,
+            ignore_unknown_props: bool = False
     ) -> Any:
         """Maps ``anything`` describing JSON data to the according representation described by the ``type_annotation``.
 
         Args:
             anything: The JSON data that is mapped to the corresponding Python representation.
             type_annotation: Describes the target Python object to map ``anything`` to.
+            ignore_unknown_props: Indicates whether superfluous JSON object properties encountered during processing of
+                ``anything`` should be ignored as opposed to raising an error.
 
         Returns:
             The created Python representation of ``anything``.
 
         Raises:
             ValueError: If ``anything`` could not be mapped for some reason (e.g., due to ``anything`` not being valid
                 JSON data).
@@ -197,70 +204,93 @@
 
         if anything is None or isinstance(anything, (str, int, float, bool)):
 
             return anything
 
         elif isinstance(anything, list):
 
-            return cls._dejsonify_array(anything, type_annotation=type_annotation)
+            return cls._dejsonify_array(
+                    anything,
+                    type_annotation=type_annotation,
+                    ignore_unknown_props=ignore_unknown_props
+            )
 
         elif isinstance(anything, dict):
 
             # For dicts, we have to distinguish between those that should be mapped to Python dicts and those that
             # should be mapped to other class instances. To that end, we consider the type annotation, which may
             # provided additional information. If no type annotation is provided, then we always map to dicts.
 
             if type_annotation is None:  # -> No type annotation was provided.
 
-                return cls._dejsonify_dict(anything)
+                return cls._dejsonify_dict(anything, ignore_unknown_props=ignore_unknown_props)
 
             elif (
                     isinstance(type_annotation, types.GenericAlias) and
                     type_annotation.__origin__ == dict
             ):  # -> The type annotation is a generic type alias dict[_, _].
 
-                return cls._dejsonify_dict(anything, type_annotation=type_annotation)
+                return cls._dejsonify_dict(
+                        anything,
+                        type_annotation=type_annotation,
+                        ignore_unknown_props=ignore_unknown_props
+                )
 
             elif isinstance(type_annotation, typing._GenericAlias):  # -> The TA is a custom generic class.
 
-                return cls._dejsonify_object(anything, type_annotation.__origin__)
+                return cls._dejsonify_object(
+                        anything,
+                        target_type=type_annotation.__origin__,
+                        ignore_unknown_props=ignore_unknown_props
+                )
 
             else:  # -> The type annotation is not a generic type annotation, but an actual type.
 
                 if type_annotation == dict:
 
-                    return cls._dejsonify_dict(anything, type_annotation=type_annotation)
+                    return cls._dejsonify_dict(
+                            anything,
+                            type_annotation=type_annotation,
+                            ignore_unknown_props=ignore_unknown_props
+                    )
 
                 else:
-                    return cls._dejsonify_object(anything, type_annotation)
+                    return cls._dejsonify_object(
+                            anything,
+                            target_type=type_annotation,
+                            ignore_unknown_props=ignore_unknown_props
+                    )
 
         else:
 
             raise ValueError(
                     "The provided <anything> could not be mapped to an equivalent Python object. "
                     "Are you sure it is valid JSON data?"
             )
 
     @classmethod
     def _dejsonify_array(
             cls,
             json_array: list,
-            type_annotation: Union[None, type, types.GenericAlias] = None
+            type_annotation: Union[None, type, types.GenericAlias] = None,
+            ignore_unknown_props: bool = False
     ) -> Union[list, tuple]:
         """Maps the provided ``json_array`` to the according :class:`list` or :class:`tuple`.
 
         If no ``type_annotation`` is provided, then the ``json_array`` is always mapped to a :class:`list`.
         Technically, the ``json_array`` is of course already a :class:`list`. However, the optional arg
         ``type_annotation`` allows for specifying the exact target :class:`list` or :class:`tuple`, which in turn incurs
         required parsing of elements. An example of a such a ``type_annotation`` could look
         like this: ``list[MyClass]`` or ``tuple[dict[str, MyClass], ...]``.
 
         Args:
             json_array: The JSON array that is mapped to a :class:`list` or :class:`tuple`.
             type_annotation: A type annotation that describes the target :class:`type`.
+            ignore_unknown_props: Indicates whether superfluous JSON object properties encountered during processing of
+                the ``json_array`` should be ignored as opposed to raising an error.
 
         Returns:
             The created :class:`list` or :class:`tuple`.
 
         Raises:
             ValueError: If the ``type_annotation`` is specified (i.e., not ``None`` and not ``Any``), but
                 is neither :class:`list`, nor `class:`tuple`, nor a generic type alias of these two :class:`type`\ s.
@@ -299,32 +329,38 @@
 
         # Next, we recursively parse the elements of the array, and combine them into a single list/tuple.
         element_type_annotation = (
                 type_annotation.__args__[0]  # -> NOTICE: This also removes the "..." from tuples.
                 if isinstance(type_annotation, types.GenericAlias) else
                 None
         )
-        return array_type(cls._dejsonify(x, type_annotation=element_type_annotation) for x in json_array)
+        return array_type(
+                cls._dejsonify(x, type_annotation=element_type_annotation, ignore_unknown_props=ignore_unknown_props)
+                for x in json_array
+        )
 
     @classmethod
     def _dejsonify_dict(
             cls,
             json_object: dict,
-            type_annotation: Optional[types.GenericAlias] = None
+            type_annotation: Optional[types.GenericAlias] = None,
+            ignore_unknown_props: bool = False
     ) -> dict:
         """Maps the provided ``json_object`` to the according :class:`dict`.
 
         Technically, the ``json_object`` is of course already a :class:`dict`. However, the optional arg
         ``type_annotation`` allows for specifying types of the keys of target :class:`dict` (e.g., as instances of a
         specific class), which in turn incurs required parsing. An example of a such a ``type_annotation`` could look
         like this: ``dict[str, list[MyClass]]``.
 
         Args:
             json_object: The JSON object that is mapped to a :class:`dict`.
             type_annotation: A type annotation that describes the target :class:`dict`.
+            ignore_unknown_props: Indicates whether superfluous JSON object properties encountered during processing of
+                the ``json_object`` should be ignored as opposed to raising an error.
 
         Returns:
             The created :class:`dict`.
 
         Raises:
             ValueError: If the ``type_annotation`` is specified (i.e., not ``None`` and not ``Any``), but does not
                 describe a :class:`dict`.
@@ -346,28 +382,35 @@
         # Next, we recursively dejsonify the values of the dict.
         value_type_annotation = (
                 None
                 if type_annotation is None else
                 type_annotation.__args__[1]  # -> That is the type hint for the values. ([0] describes keys.)
         )
         return {
-                k: cls._dejsonify(v, type_annotation=value_type_annotation)
+                k: cls._dejsonify(v, type_annotation=value_type_annotation, ignore_unknown_props=ignore_unknown_props)
                 for k, v in json_object.items()
         }
 
     @classmethod
-    def _dejsonify_object(cls, json_object: dict[str, Any], target_type: type[_T]) -> _T:
+    def _dejsonify_object(
+            cls,
+            json_object: dict[str, Any],
+            target_type: type[_T],
+            ignore_unknown_props: bool = False
+    ) -> _T:
         """Maps the provided ``json_object`` to the according instance of the ``target_type``.
 
         Notice that this method is **not** supposed to be used for JSON objects that should be mapped to
         :class:`dict`\ s, which is implemented by the method :meth:`~._dejsonify_dict`.
 
         Args:
             json_object: The JSON object that is mapped to an instance of the ``target_type``.
             target_type: The :class:`type` that the ``json_object`` describes an instance of.
+            ignore_unknown_props: Indicates whether superfluous JSON object properties encountered during processing of
+                the ``json_object`` should be ignored as opposed to raising an error.
 
         Returns:
             The created instance of the ``target_type``.
         """
 
         # To be able to sanitize the provided JSON data, we first retrieve all args of the constructor of the given
         # type together with their type annotations.
@@ -381,24 +424,32 @@
         # Now, we first ensure that all required args are specified.
         for some_arg in required_args:
 
             if some_arg not in json_object:
 
                 raise ValueError(f"Missing required arg <{some_arg}> in the given <json_object>")
 
-        # Next, we ensure that no unknown args are provided.
-        for some_arg in json_object.keys():
+        # Next, we handle unknown args. If unknown args are ignored, then we remove them from considered JSON object.
+        # Otherwise, we raise an error.
+        json_object = copy.deepcopy(json_object)  # -> Ensures that deleting keys doesn't corrupt the original instance.
+        for some_arg in list(json_object.keys()):
 
             if some_arg not in all_args:
 
-                raise ValueError(f"Encountered unknown arg <{some_arg}> in the given <json_object>")
+                if ignore_unknown_props:
+
+                    del json_object[some_arg]
+
+                else:
+
+                    raise ValueError(f"Encountered unknown arg <{some_arg}> in the given <json_object>")
 
         # Finally, we are ready to parse the args and create the needed instance.
         parsed_args = {
-                k: cls._dejsonify(v, type_annotation=type_annotations[k])
+                k: cls._dejsonify(v, type_annotation=type_annotations[k], ignore_unknown_props=ignore_unknown_props)
                 for k, v in json_object.items()
         }
         return target_type(**parsed_args)
 
     @classmethod
     def _jsonify(cls, anything: Any) -> Any:
         """Maps ``anything`` to the according JSON representation.
```

### Comparing `anyjsonthing-0.3.1/src/main/anyjsonthing/utils.py` & `anyjsonthing-0.4.0/src/main/anyjsonthing/utils.py`

 * *Files identical despite different names*

### Comparing `anyjsonthing-0.3.1/src/main/anyjsonthing.egg-info/PKG-INFO` & `anyjsonthing-0.4.0/src/main/anyjsonthing.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anyjsonthing
-Version: 0.3.1
+Version: 0.4.0
 Summary: A library that implements serialization of simple data objects as JSON data.
 Home-page: https://github.com/phohenecker/anyjsonthing
 Author: Patrick Hohenecker
 Author-email: patrick.hohenecker@gmx.at
 License: Simplified BSD License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

