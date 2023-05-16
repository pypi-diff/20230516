# Comparing `tmp/kirzner_serializer-0.0.1.tar.gz` & `tmp/kirzner_serializer-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kirzner_serializer-0.0.1.tar", last modified: Sun May 14 21:13:19 2023, max compression
+gzip compressed data, was "kirzner_serializer-0.0.2.tar", last modified: Tue May 16 16:23:46 2023, max compression
```

## Comparing `kirzner_serializer-0.0.1.tar` & `kirzner_serializer-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 21:13:19.862726 kirzner_serializer-0.0.1/
--rw-rw-rw-   0        0        0      905 2023-05-14 21:13:19.862726 kirzner_serializer-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      468 2023-05-14 20:16:00.000000 kirzner_serializer-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-14 21:13:19.847103 kirzner_serializer-0.0.1/kirznerSerializer/
--rw-rw-rw-   0        0        0        0 2023-05-14 19:58:02.000000 kirzner_serializer-0.0.1/kirznerSerializer/__init__.py
--rw-rw-rw-   0        0        0     5802 2023-05-14 20:04:46.000000 kirzner_serializer-0.0.1/kirznerSerializer/base_serializer.py
--rw-rw-rw-   0        0        0     3939 2023-05-14 19:51:30.000000 kirzner_serializer-0.0.1/kirznerSerializer/constants.py
--rw-rw-rw-   0        0        0    10663 2023-05-14 20:55:06.000000 kirzner_serializer-0.0.1/kirznerSerializer/json_serializer.py
--rw-rw-rw-   0        0        0     7825 2023-05-14 20:51:08.000000 kirzner_serializer-0.0.1/kirznerSerializer/xml_serializer.py
-drwxrwxrwx   0        0        0        0 2023-05-14 21:13:19.847103 kirzner_serializer-0.0.1/kirzner_serializer.egg-info/
--rw-rw-rw-   0        0        0      905 2023-05-14 21:13:19.000000 kirzner_serializer-0.0.1/kirzner_serializer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      459 2023-05-14 21:13:19.000000 kirzner_serializer-0.0.1/kirzner_serializer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 21:13:19.000000 kirzner_serializer-0.0.1/kirzner_serializer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-14 21:13:19.000000 kirzner_serializer-0.0.1/kirzner_serializer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-05-14 21:13:19.000000 kirzner_serializer-0.0.1/kirzner_serializer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-14 21:13:19.862726 kirzner_serializer-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      869 2023-05-14 21:09:56.000000 kirzner_serializer-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-14 21:13:19.862726 kirzner_serializer-0.0.1/tests/
--rw-rw-rw-   0        0        0     5850 2023-05-14 14:50:03.000000 kirzner_serializer-0.0.1/tests/test_constants.py
--rw-rw-rw-   0        0        0    13015 2023-05-14 20:04:46.000000 kirzner_serializer-0.0.1/tests/test_json.py
--rw-rw-rw-   0        0        0    12822 2023-05-14 20:04:46.000000 kirzner_serializer-0.0.1/tests/test_xml.py
+drwxrwxrwx   0        0        0        0 2023-05-16 16:23:46.498547 kirzner_serializer-0.0.2/
+-rw-rw-rw-   0        0        0      905 2023-05-16 16:23:46.498547 kirzner_serializer-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      468 2023-05-14 20:16:00.000000 kirzner_serializer-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-16 16:23:46.408598 kirzner_serializer-0.0.2/kirznerSerializer/
+-rw-rw-rw-   0        0        0        0 2023-05-14 19:58:02.000000 kirzner_serializer-0.0.2/kirznerSerializer/__init__.py
+-rw-rw-rw-   0        0        0     5947 2023-05-16 15:18:34.000000 kirzner_serializer-0.0.2/kirznerSerializer/base_serializer.py
+-rw-rw-rw-   0        0        0     3972 2023-05-16 15:18:34.000000 kirzner_serializer-0.0.2/kirznerSerializer/constants.py
+-rw-rw-rw-   0        0        0    12493 2023-05-16 15:18:34.000000 kirzner_serializer-0.0.2/kirznerSerializer/json_serializer.py
+-rw-rw-rw-   0        0        0     9795 2023-05-16 15:18:34.000000 kirzner_serializer-0.0.2/kirznerSerializer/xml_serializer.py
+drwxrwxrwx   0        0        0        0 2023-05-16 16:23:46.427230 kirzner_serializer-0.0.2/kirzner_serializer.egg-info/
+-rw-rw-rw-   0        0        0      905 2023-05-16 16:23:46.000000 kirzner_serializer-0.0.2/kirzner_serializer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      459 2023-05-16 16:23:46.000000 kirzner_serializer-0.0.2/kirzner_serializer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 16:23:46.000000 kirzner_serializer-0.0.2/kirzner_serializer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-16 16:23:46.000000 kirzner_serializer-0.0.2/kirzner_serializer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-16 16:23:46.000000 kirzner_serializer-0.0.2/kirzner_serializer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-16 16:23:46.500973 kirzner_serializer-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      869 2023-05-16 16:21:24.000000 kirzner_serializer-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 16:23:46.427230 kirzner_serializer-0.0.2/tests/
+-rw-rw-rw-   0        0        0     5850 2023-05-16 16:14:11.000000 kirzner_serializer-0.0.2/tests/test_constants.py
+-rw-rw-rw-   0        0        0    13636 2023-05-16 16:15:06.000000 kirzner_serializer-0.0.2/tests/test_json.py
+-rw-rw-rw-   0        0        0    13434 2023-05-16 16:15:06.000000 kirzner_serializer-0.0.2/tests/test_xml.py
```

### Comparing `kirzner_serializer-0.0.1/PKG-INFO` & `kirzner_serializer-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kirzner_serializer
-Version: 0.0.1
+Version: 0.0.2
 Summary: Module for json and xml serialization
 Author: Nastya Kirzner
 Author-email: kirznernasta@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `kirzner_serializer-0.0.1/kirznerSerializer/base_serializer.py` & `kirzner_serializer-0.0.2/kirznerSerializer/base_serializer.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,14 +42,18 @@
 
     @classmethod
     @abstractmethod
     def loads(cls, s: str):
         pass
 
     @classmethod
+    def is_iterator(cls, obj):
+        return hasattr(obj, '__iter__') and hasattr(obj, '__next__') and callable(obj.__iter__)
+
+    @classmethod
     def serialize_code(cls, obj: CODE_TYPE):
         source = {}
         for (key, value) in inspect.getmembers(obj):
             if key in CODE_ATTRIBUTES:
                 source[key] = value
         source_json = cls.dumps(source)
 
@@ -143,19 +147,17 @@
             function.__globals__.update({function.__name__: function})
 
         return function
 
     @classmethod
     def deserialize_type(cls, value):
         source = cls.loads(value)
-
         name = source[NAME_KEY]
         bases = source[BASES_KEY]
         dictionary = source[DICT_KEY]
-
         result = type(name, bases, dictionary)
 
         for attribute in result.__dict__.values():
             if inspect.isroutine(attribute):
 
                 if type(attribute) in (STATIC_METHOD_TYPE, CLASS_METHOD_TYPE):
                     function_globals = attribute.__func__.__globals__
```

### Comparing `kirzner_serializer-0.0.1/kirznerSerializer/constants.py` & `kirzner_serializer-0.0.2/kirznerSerializer/constants.py`

 * *Files 11% similar despite different names*

```diff
@@ -38,15 +38,14 @@
 TRUE_VALUE = 'true'
 FALSE_VALUE = 'false'
 
 BOOL_ERROR = 'Invalid bool value!'
 NULL_ERROR = 'Invalid null value!'
 JSON_ERROR = 'Invalid json value!'
 XMl_ERROR = 'Invalid xml value!'
-BUILT_IN_ERROR = 'Built-in function cannot be serialized!'
 UNKNOWN_TYPE_ERROR = 'Type cannot be serialized: '
 
 
 class BoolException(BaseException):
     message = BOOL_ERROR
 
     def __init__(self, *args):
@@ -56,21 +55,14 @@
 class NullException(BaseException):
     message = NULL_ERROR
 
     def __init__(self, *args):
         super().__init__(self.message, *args)
 
 
-class BuiltInException(BaseException):
-    message = BUILT_IN_ERROR
-
-    def __init__(self, *args):
-        super().__init__(self.message, *args)
-
-
 class InvalidJsonException(BaseException):
     message = JSON_ERROR
 
     def __init__(self, *args):
         super().__init__(self.message, *args)
 
 
@@ -89,18 +81,30 @@
 
 
 NAME_KEY = '__name__'
 CODE_KEY = '__code__'
 DICT_KEY = '__dict__'
 CLASS_KEY = '__class__'
 BASES_KEY = '__bases__'
+MODULE_KEY = '__module__'
 GLOBALS_KEY = '__globals__'
 CLOSURE_KEY = '__closure__'
 DEFAULTS_KEY = '__defaults__'
 
+
+SOURCE_KEY = 'source'
+
+GETTER_KEY = 'getter'
+SETTER_KEY = 'setter'
+DELETER_KEY = 'deleter'
+
+MAP_KEY = 'map'
+ITER_KEY = 'iter'
+FILTER_KEY: str = 'filter'
+
 FUNCTION_ATTRIBUTES = (CODE_KEY, GLOBALS_KEY, NAME_KEY, DEFAULTS_KEY, CLOSURE_KEY)
 
 CODE_ATTRIBUTES = [CodeType.co_argcount.__name__,
                    CodeType.co_posonlyargcount.__name__,
                    CodeType.co_kwonlyargcount.__name__,
                    CodeType.co_nlocals.__name__,
                    CodeType.co_stacksize.__name__,
@@ -123,13 +127,14 @@
 
 UNIQUE_TYPES = (MappingProxyType, WrapperDescriptorType, MethodDescriptorType, GetSetDescriptorType, BuiltinMethodType)
 
 CODE_TYPE_NAME = CODE_TYPE.__name__
 CELL_TYPE_NAME = CELL_TYPE.__name__
 MODULE_TYPE_NAME = MODULE_TYPE.__name__
 FUNCTION_TYPE_NAME = FUNCTION_TYPE.__name__
+BUILD_IN_FUNCTION_NAME = 'builtin_function_or_method'
 
 PROPERTY_TYPE = property
 CLASS_METHOD_TYPE = classmethod
 STATIC_METHOD_TYPE = staticmethod
 
 CLASS_OR_STATIC_METHOD_TYPE = (CLASS_METHOD_TYPE, STATIC_METHOD_TYPE)
```

### Comparing `kirzner_serializer-0.0.1/kirznerSerializer/json_serializer.py` & `kirzner_serializer-0.0.2/kirznerSerializer/json_serializer.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,14 @@
                                          InvalidJsonException,
                                          UnknownTypeException,
                                          CLOSE_SQUARE_BRACKET,
                                          OPEN_SQUARE_BRACKET,
                                          FUNCTION_TYPE_NAME,
                                          STATIC_METHOD_TYPE,
                                          CLASS_METHOD_TYPE,
-                                         BuiltInException,
                                          LIST_TUPLE_BYTES,
                                          MODULE_TYPE_NAME,
                                          COMMON_JSON_REG,
                                          CODE_TYPE_NAME,
                                          CELL_TYPE_NAME,
                                          PROPERTY_TYPE,
                                          UNIQUE_TYPES,
@@ -25,15 +24,16 @@
                                          VALUE_KEY,
                                          BASES_KEY,
                                          TYPE_KEY,
                                          NAME_KEY,
                                          DICT_KEY,
                                          COLON,
                                          COMMA,
-                                         NUM)
+                                         NUM, GETTER_KEY, SETTER_KEY, DELETER_KEY, MODULE_KEY, BUILD_IN_FUNCTION_NAME,
+                                         CLASS_KEY, SOURCE_KEY, ITER_KEY, MAP_KEY, FILTER_KEY)
 
 
 class JsonSerializer(BaseSerializer):
 
     @classmethod
     def dumps(cls, obj) -> str:
         return cls.__to_json(obj)
@@ -75,23 +75,38 @@
 
         elif isinstance(obj, CELL_TYPE):
             json_string += cls.__to_json(obj.cell_contents)
 
         elif type(obj) in CLASS_OR_STATIC_METHOD_TYPE:
             json_string += cls.__to_json(obj.__func__, is_inner_function=is_inner_function)
 
-        elif inspect.isbuiltin(obj) or type(obj) is PROPERTY_TYPE:
-            raise BuiltInException()
+        elif type(obj) is PROPERTY_TYPE:
+            json_string = f'{{{TYPE_KEY}"{property.__name__}",{VALUE_KEY}'
+            json_string += cls.__to_json({GETTER_KEY: obj.fget, SETTER_KEY: obj.fset, DELETER_KEY: obj.fdel})
+
+        elif inspect.isbuiltin(obj):
+            json_string += cls.__to_json({MODULE_KEY: obj.__module__, NAME_KEY: obj.__name__})
+
+        elif cls.is_iterator(obj):
+            if not isinstance(obj, (map, filter)):
+                json_string = f'{{{TYPE_KEY}"{ITER_KEY}",{VALUE_KEY}'
+
+            data = list(map(cls.__to_json, obj))
+            json_string += cls.__to_json(data, serialize_value=False)
 
         elif inspect.isroutine(obj):
             json_string += cls.serialize_routine(obj, is_inner_function)
 
         elif inspect.isclass(obj):
             json_string += cls.__serialize_class(obj)
 
+        elif isinstance(obj, object):
+            source = {CLASS_KEY: cls.__to_json(obj.__class__), SOURCE_KEY: cls.__get_dict(obj)}
+            json_string += cls.__to_json(source, serialize_value=False)
+
         else:
             raise UnknownTypeException(type(obj).__name__)
 
         json_string += CLOSE_BRACE
 
         if comma:
             json_string += COMMA
@@ -216,28 +231,52 @@
 
             elif type_name == CODE_TYPE_NAME:
                 return cls.deserialize_code(value)
 
             elif type_name == CELL_TYPE_NAME:
                 return cls.deserialize_cell(value)
 
+            elif type_name == MAP_KEY:
+                source = cls.__from_json(value)
+                return map(lambda x: x, source)
+
+            elif type_name == FILTER_KEY:
+                source = cls.__from_json(value)
+                return filter(lambda x: x, source)
+
+            elif type_name == ITER_KEY:
+                source = cls.__from_json(value)
+                return iter(source)
+
+            elif type_name == property.__name__:
+                source = cls.__from_json(value)
+                return property(source[GETTER_KEY], source[SETTER_KEY], source[DELETER_KEY])
+
             elif type_name == STATIC_METHOD_TYPE.__name__:
                 return staticmethod(cls.__from_json(value))
 
             elif type_name == CLASS_METHOD_TYPE.__name__:
                 return classmethod(cls.__from_json(value))
 
+            elif type_name == BUILD_IN_FUNCTION_NAME:
+                source = cls.__from_json(value)
+                module = __import__(source[MODULE_KEY])
+                return getattr(module, source[NAME_KEY])
+
             elif type_name == FUNCTION_TYPE_NAME:
                 return cls.deserialize_function(value)
 
             elif type_name == type.__name__:
                 return cls.deserialize_type(value)
 
             else:
-                raise InvalidJsonException()
+                value = cls.__from_json(value)
+                obj = object.__new__(value[CLASS_KEY])
+                obj.__dict__ = value[SOURCE_KEY]
+                return obj
 
     @classmethod
     def __unescape_string(cls, value: str):
         result = value.replace('\\\\', '\\').replace('\\"', '\"')
         return result
 
     @classmethod
```

### Comparing `kirzner_serializer-0.0.1/kirznerSerializer/xml_serializer.py` & `kirzner_serializer-0.0.2/kirznerSerializer/xml_serializer.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,26 +10,26 @@
                                          LIST_TUPLE_BYTES_SET,
                                          InvalidXmlException,
                                          STATIC_METHOD_TYPE,
                                          FUNCTION_TYPE_NAME,
                                          CLASS_METHOD_TYPE,
                                          VALUE_GROUP_NAME,
                                          MODULE_TYPE_NAME,
-                                         BuiltInException,
                                          COMMON_XML_REG,
                                          CODE_TYPE_NAME,
                                          CELL_TYPE_NAME,
                                          PROPERTY_TYPE,
                                          UNIQUE_TYPES,
                                          NULL_VALUE,
                                          CELL_TYPE,
                                          BASES_KEY,
                                          DICT_KEY,
                                          NAME_KEY,
-                                         NUM)
+                                         NUM, MODULE_KEY, CLASS_KEY, SOURCE_KEY, GETTER_KEY, SETTER_KEY, DELETER_KEY,
+                                         BUILD_IN_FUNCTION_NAME, MAP_KEY, FILTER_KEY, ITER_KEY)
 
 
 class XmlSerializer(BaseSerializer):
 
     @classmethod
     def dumps(cls, obj):
         return cls.__to_xml(obj)
@@ -75,23 +75,41 @@
 
         elif isinstance(obj, CELL_TYPE):
             xml_string += cls.__to_xml(obj.cell_contents)
 
         elif type(obj) in CLASS_OR_STATIC_METHOD_TYPE:
             xml_string += cls.__to_xml(obj.__func__, is_inner_function=is_inner_function)
 
-        elif inspect.isbuiltin(obj) or type(obj) is PROPERTY_TYPE:
-            raise BuiltInException()
+        elif type(obj) is PROPERTY_TYPE:
+            type_name = property.__name__
+            xml_string = f'<{type_name}>'
+            xml_string += cls.__to_xml({GETTER_KEY: obj.fget, SETTER_KEY: obj.fset, DELETER_KEY: obj.fdel})
+
+        elif cls.is_iterator(obj):
+            if not isinstance(obj, (map, filter)):
+                type_name = ITER_KEY
+                xml_string = f'<{type_name}>'
+
+            data = list(map(cls.__to_xml, obj))
+            xml_string += cls.__to_xml(data, serialize_value=False)
+
+        elif inspect.isbuiltin(obj):
+            xml_string += cls.__to_xml({MODULE_KEY: obj.__module__, NAME_KEY: obj.__name__})
 
         elif inspect.isroutine(obj):
             xml_string += cls.serialize_routine(obj, is_inner_function)
 
         elif inspect.isclass(obj):
             xml_string += cls.__serialize_class(obj)
 
+        elif isinstance(obj, object):
+            source = {CLASS_KEY: cls.__to_xml(obj.__class__),
+                      SOURCE_KEY: cls.__to_xml(cls.__get_dict(obj), serialize_value=False)}
+            xml_string += cls.__to_xml(source, serialize_value=False)
+
         else:
             raise UnknownTypeException(type(obj).__name__)
 
         xml_string += f'</{type_name}>'
 
         return xml_string
 
@@ -179,27 +197,51 @@
 
                 elif open_tag == CODE_TYPE_NAME:
                     return cls.deserialize_code(value)
 
                 elif open_tag == CELL_TYPE_NAME:
                     return cls.deserialize_cell(value)
 
+                elif open_tag == MAP_KEY:
+                    source = cls.__from_xml(value)
+                    return map(lambda x: x, source)
+
+                elif open_tag == FILTER_KEY:
+                    source = cls.__from_xml(value)
+                    return filter(lambda x: x, source)
+
+                elif open_tag == ITER_KEY:
+                    source = cls.__from_xml(value)
+                    return iter(source)
+
+                elif open_tag == property.__name__:
+                    source = cls.__from_xml(value)
+                    return property(source[GETTER_KEY], source[SETTER_KEY], source[DELETER_KEY])
+
                 elif open_tag == STATIC_METHOD_TYPE.__name__:
                     return staticmethod(cls.__from_xml(value))
 
                 elif open_tag == CLASS_METHOD_TYPE.__name__:
                     return classmethod(cls.__from_xml(value))
 
+                elif open_tag == BUILD_IN_FUNCTION_NAME:
+                    source = cls.__from_xml(value)
+                    module = __import__(source[MODULE_KEY])
+                    return getattr(module, source[NAME_KEY])
+
                 elif open_tag == FUNCTION_TYPE_NAME:
                     return cls.deserialize_function(value)
 
                 elif open_tag == type.__name__:
                     return cls.deserialize_type(value)
 
                 else:
-                    raise InvalidXmlException()
+                    value = cls.__from_xml(value)
+                    obj = object.__new__(value[CLASS_KEY])
+                    obj.__dict__ = value[SOURCE_KEY]
+                    return obj
 
     @classmethod
     def __unescape_string(cls, s: str):
         s = s.replace('&amp;', '&').replace('&lt;', '<').replace('&gt;', '>')
         s = s.replace('&quot;', '"').replace('&apos;', "'")
         return s
```

### Comparing `kirzner_serializer-0.0.1/kirzner_serializer.egg-info/PKG-INFO` & `kirzner_serializer-0.0.2/kirzner_serializer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kirzner-serializer
-Version: 0.0.1
+Version: 0.0.2
 Summary: Module for json and xml serialization
 Author: Nastya Kirzner
 Author-email: kirznernasta@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `kirzner_serializer-0.0.1/setup.py` & `kirzner_serializer-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 HERE = path.abspath(path.dirname(__file__))
 
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="kirzner_serializer",
-    version="0.0.1",
+    version="0.0.2",
     description="Module for json and xml serialization",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Nastya Kirzner",
     author_email="kirznernasta@gmail.com",
     license="MIT",
     classifiers=[
```

### Comparing `kirzner_serializer-0.0.1/tests/test_constants.py` & `kirzner_serializer-0.0.2/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `kirzner_serializer-0.0.1/tests/test_json.py` & `kirzner_serializer-0.0.2/tests/test_json.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import unittest
 
 from kirznerSerializer.json_serializer import JsonSerializer
 
 from kirznerSerializer.constants import (InvalidJsonException,
-                                         BuiltInException,
                                          BoolException)
 
 from tests.test_constants import (SPECIAL_STRING_VARIABLE, FILE_FOR_SPECIAL_STRING_JSON, EXPECTED_SPECIAL_STRING_JSON,
                                   QUOTES_STRING_VARIABLE, FILE_FOR_QUOTES_STRING_JSON, EXPECTED_QUOTES_STRING_JSON,
                                   NESTED_LIST_VARIABLE, FILE_FOR_NESTED_LIST_JSON, EXPECTED_NESTED_LIST_JSON,
                                   DICTIONARY_VARIABLE, FILE_FOR_DICTIONARY_JSON, EXPECTED_DICTIONARY_JSON,
                                   STRING_VARIABLE, FILE_FOR_STRING_JSON, EXPECTED_STRING_JSON,
@@ -182,15 +181,17 @@
 class JSONFunctionsTestCase(unittest.TestCase):
     def test_function(self):
         json = JsonSerializer.dumps(FUNCTION_VARIABLE)
         obj = JsonSerializer.loads(json)
         self.assertEqual(FUNCTION_VARIABLE(), obj())
 
     def test_built_in_function(self):
-        self.assertRaises(BuiltInException, JsonSerializer.dumps, BUILT_IN_FUNCTION)
+        json = JsonSerializer.dumps(BUILT_IN_FUNCTION)
+        obj = JsonSerializer.loads(json)
+        self.assertEqual(BUILT_IN_FUNCTION, obj)
 
     def test_lambda(self):
         json = JsonSerializer.dumps(LAMBDA_VARIABLE)
         obj = JsonSerializer.loads(json)
         self.assertEqual(LAMBDA_VARIABLE(STRING_VARIABLE), obj(STRING_VARIABLE))
 
     def test_wrapper(self):
@@ -218,16 +219,16 @@
         obj = JsonSerializer.loads(json)
         self.assertEqual(FUNCTION_WITH_GLOBALS_REFERENCE(0), obj(0))
 
 
 class JSONClassesTestCase(unittest.TestCase):
     def test_object(self):
         expected_object = CLASS_REFERENCE()
-        json = JsonSerializer.dumps(CLASS_REFERENCE)
-        obj = JsonSerializer.loads(json)()
+        json = JsonSerializer.dumps(expected_object)
+        obj = JsonSerializer.loads(json)
         self.assertEqual(expected_object.hi(), obj.hi())
 
     def test_class_with_inheritance(self):
         expected_object = CLASS_WITH_INHERITANCE()
         json = JsonSerializer.dumps(CLASS_WITH_INHERITANCE)
         obj = JsonSerializer.loads(json)()
         self.assertEqual(expected_object.hi(), obj.hi())
@@ -273,10 +274,25 @@
         self.assertEqual(0, obj.sin(0))
 
     def test_code(self):
         json = JsonSerializer.dumps(CODE_VARIABLE)
         obj = JsonSerializer.loads(json)
         self.assertEqual(CODE_VARIABLE, obj)
 
+    def test_map(self):
+        json = JsonSerializer.dumps(map(lambda x: x + 1, [1, 2, 3]))
+        obj = JsonSerializer.loads(json)
+        self.assertEqual(list(map(lambda x: x + 1, [1, 2, 3])), list(obj))
+
+    def test_filter(self):
+        json = JsonSerializer.dumps(filter(lambda x: x > 2, [1, 2, 3]))
+        obj = JsonSerializer.loads(json)
+        self.assertEqual(list(filter(lambda x: x > 2, [1, 2, 3])), list(obj))
+
+    def test_iter(self):
+        json = JsonSerializer.dumps(iter('string'))
+        obj = JsonSerializer.loads(json)
+        self.assertEqual(next(iter('string')), next(obj))
+
 
 if __name__ == '__main__':
     unittest.TextTestRunner().run(JSONTests())
```

### Comparing `kirzner_serializer-0.0.1/tests/test_xml.py` & `kirzner_serializer-0.0.2/tests/test_xml.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import unittest
 
 from kirznerSerializer.xml_serializer import XmlSerializer
 
 from kirznerSerializer.constants import (InvalidXmlException,
-                                         BuiltInException,
                                          BoolException)
 
 from tests.test_constants import (SPECIAL_STRING_VARIABLE, FILE_FOR_SPECIAL_STRING_XML, EXPECTED_SPECIAL_STRING_XML,
                                   QUOTES_STRING_VARIABLE, FILE_FOR_QUOTES_STRING_XML, EXPECTED_QUOTES_STRING_XML,
                                   NESTED_LIST_VARIABLE, FILE_FOR_NESTED_LIST_XML, EXPECTED_NESTED_LIST_XML,
                                   DICTIONARY_VARIABLE, FILE_FOR_DICTIONARY_XML, EXPECTED_DICTIONARY_XML,
                                   STRING_VARIABLE, FILE_FOR_STRING_XML, EXPECTED_STRING_XML,
@@ -182,15 +181,17 @@
 class XMLFunctionsTestCase(unittest.TestCase):
     def test_function(self):
         xml = XmlSerializer.dumps(FUNCTION_VARIABLE)
         obj = XmlSerializer.loads(xml)
         self.assertEqual(FUNCTION_VARIABLE(), obj())
 
     def test_built_in_function(self):
-        self.assertRaises(BuiltInException, XmlSerializer.dumps, BUILT_IN_FUNCTION)
+        xml = XmlSerializer.dumps(BUILT_IN_FUNCTION)
+        obj = XmlSerializer.loads(xml)
+        self.assertEqual(BUILT_IN_FUNCTION, obj)
 
     def test_lambda(self):
         xml = XmlSerializer.dumps(LAMBDA_VARIABLE)
         obj = XmlSerializer.loads(xml)
         self.assertEqual(LAMBDA_VARIABLE(STRING_VARIABLE), obj(STRING_VARIABLE))
 
     def test_wrapper(self):
@@ -218,16 +219,16 @@
         obj = XmlSerializer.loads(xml)
         self.assertEqual(FUNCTION_WITH_GLOBALS_REFERENCE(0), obj(0))
 
 
 class XMLClassesTestCase(unittest.TestCase):
     def test_object(self):
         expected_object = CLASS_REFERENCE()
-        xml = XmlSerializer.dumps(CLASS_REFERENCE)
-        obj = XmlSerializer.loads(xml)()
+        xml = XmlSerializer.dumps(expected_object)
+        obj = XmlSerializer.loads(xml)
         self.assertEqual(expected_object.hi(), obj.hi())
 
     def test_class_with_inheritance(self):
         expected_object = CLASS_WITH_INHERITANCE()
         xml = XmlSerializer.dumps(CLASS_WITH_INHERITANCE)
         obj = XmlSerializer.loads(xml)()
         self.assertEqual(expected_object.hi(), obj.hi())
@@ -273,10 +274,25 @@
         self.assertEqual(0, obj.sin(0))
 
     def test_code(self):
         xml = XmlSerializer.dumps(CODE_VARIABLE)
         obj = XmlSerializer.loads(xml)
         self.assertEqual(CODE_VARIABLE, obj)
 
+    def test_map(self):
+        json = XmlSerializer.dumps(map(lambda x: x + 1, [1, 2, 3]))
+        obj = XmlSerializer.loads(json)
+        self.assertEqual(list(map(lambda x: x + 1, [1, 2, 3])), list(obj))
+
+    def test_filter(self):
+        json = XmlSerializer.dumps(filter(lambda x: x > 2, [1, 2, 3]))
+        obj = XmlSerializer.loads(json)
+        self.assertEqual(list(filter(lambda x: x > 2, [1, 2, 3])), list(obj))
+
+    def test_iter(self):
+        json = XmlSerializer.dumps(iter('string'))
+        obj = XmlSerializer.loads(json)
+        self.assertEqual(next(iter('string')), next(obj))
+
 
 if __name__ == '__main__':
     unittest.TextTestRunner().run(XMLTests())
```

