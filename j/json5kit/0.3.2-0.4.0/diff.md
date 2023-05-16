# Comparing `tmp/json5kit-0.3.2.tar.gz` & `tmp/json5kit-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json5kit-0.3.2.tar", last modified: Sun Apr 16 15:01:46 2023, max compression
+gzip compressed data, was "json5kit-0.4.0.tar", last modified: Tue May 16 20:46:45 2023, max compression
```

## Comparing `json5kit-0.3.2.tar` & `json5kit-0.4.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2023-04-16 15:01:46.781928 json5kit-0.3.2/
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1072 2023-04-13 16:58:14.000000 json5kit-0.3.2/LICENSE
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     2273 2023-04-16 15:01:46.782038 json5kit-0.3.2/PKG-INFO
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1415 2023-04-13 21:46:23.000000 json5kit-0.3.2/README.md
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1213 2023-04-16 15:01:46.782484 json5kit-0.3.2/setup.cfg
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)       38 2023-04-13 16:58:14.000000 json5kit-0.3.2/setup.py
-drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2023-04-16 15:01:46.779127 json5kit-0.3.2/src/
-drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2023-04-16 15:01:46.780733 json5kit-0.3.2/src/json5kit/
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)    11877 2023-04-14 13:21:37.000000 json5kit-0.3.2/src/json5kit/__init__.py
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     7422 2023-04-16 15:01:38.000000 json5kit-0.3.2/src/json5kit/nodes.py
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     3629 2023-04-13 21:44:53.000000 json5kit-0.3.2/src/json5kit/visitor.py
-drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2023-04-16 15:01:46.781777 json5kit-0.3.2/src/json5kit.egg-info/
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     2273 2023-04-16 15:01:46.000000 json5kit-0.3.2/src/json5kit.egg-info/PKG-INFO
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)      286 2023-04-16 15:01:46.000000 json5kit-0.3.2/src/json5kit.egg-info/SOURCES.txt
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)        1 2023-04-16 15:01:46.000000 json5kit-0.3.2/src/json5kit.egg-info/dependency_links.txt
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)       77 2023-04-16 15:01:46.000000 json5kit-0.3.2/src/json5kit.egg-info/requires.txt
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)        9 2023-04-16 15:01:46.000000 json5kit-0.3.2/src/json5kit.egg-info/top_level.txt
+drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2023-05-16 20:46:45.624875 json5kit-0.4.0/
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1072 2023-04-13 16:58:14.000000 json5kit-0.4.0/LICENSE
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     2381 2023-05-16 20:46:45.624951 json5kit-0.4.0/PKG-INFO
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1523 2023-05-16 20:46:05.000000 json5kit-0.4.0/README.md
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1218 2023-05-16 20:46:45.625251 json5kit-0.4.0/setup.cfg
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)       38 2023-04-13 16:58:14.000000 json5kit-0.4.0/setup.py
+drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2023-05-16 20:46:45.623003 json5kit-0.4.0/src/
+drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2023-05-16 20:46:45.624144 json5kit-0.4.0/src/json5kit/
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)    12403 2023-05-16 20:46:05.000000 json5kit-0.4.0/src/json5kit/__init__.py
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     7951 2023-05-16 20:46:05.000000 json5kit-0.4.0/src/json5kit/nodes.py
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     3629 2023-04-13 21:44:53.000000 json5kit-0.4.0/src/json5kit/visitor.py
+drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2023-05-16 20:46:45.624778 json5kit-0.4.0/src/json5kit.egg-info/
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     2381 2023-05-16 20:46:45.000000 json5kit-0.4.0/src/json5kit.egg-info/PKG-INFO
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)      286 2023-05-16 20:46:45.000000 json5kit-0.4.0/src/json5kit.egg-info/SOURCES.txt
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)        1 2023-05-16 20:46:45.000000 json5kit-0.4.0/src/json5kit.egg-info/dependency_links.txt
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)       81 2023-05-16 20:46:45.000000 json5kit-0.4.0/src/json5kit.egg-info/requires.txt
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)        9 2023-05-16 20:46:45.000000 json5kit-0.4.0/src/json5kit.egg-info/top_level.txt
```

### Comparing `json5kit-0.3.2/LICENSE` & `json5kit-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `json5kit-0.3.2/PKG-INFO` & `json5kit-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json5kit
-Version: 0.3.2
+Version: 0.4.0
 Summary: A Roundtrip parser and CST for JSON, JSONC and JSON5.
 Home-page: https://github.com/tusharsadhwani/json5kit
 Author: Tushar Sadhwani
 Author-email: tushar.sadhwani000@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,55 +21,57 @@
 Provides-Extra: dev
 License-File: LICENSE
 
 # json5kit
 
 A Roundtrip parser and CST for JSON, JSONC and JSON5.
 
-> Currently a work in progress
+[JSON5](https://json5.org) is a superset of JSON, that allows trailing commas,
+comments, unquoted and single-quoted object keys, and a lot more.
 
-Currently supports parsing all of JSON syntax, and converting it back to source.
+Currently supports parsing most JSON5 syntax, and converting it back to source.
 Also supports single line `// comments`.
 
 ## Installation
 
 ```bash
 pip install json5kit
 ```
 
 ## Usage
 
 ```python
 >>> source = """
 ... {
-...   "items": [1, 2, 4],  // change this to 3
+...   items: [1, 2, 4],  // change this to 3
 ... }
 ... """
 >>> import json5kit
 >>> tree = json5kit.parse(source)
 >>> print(tree.to_source())
 
 {
-  "items": [1, 2, 4],  // change this to 3
+  items: [1, 2, 4],  // change this to 3
 }
 
 >>> print(tree.to_json())
 {"items":[1,2,4]}
+
 >>> # Let's replace the `4` with `3` now:
 >>> class ReplaceFourWithThree(json5kit.Json5Transformer):
 ...     def visit_Number(self, node):
 ...         if node.value == 4:
 ...             return node.replace(value=3)
 ...         return node
 ...
 >>> ReplaceFourWithThree().visit(tree)
 >>> print(tree.to_source())
 
 {
-  "items": [1, 2, 3],  // change this to 3
+  items: [1, 2, 3],  // change this to 3
 }
 >>> print(tree.to_json())
 {"items":[1,2,3]}
 ```
 
 ## Development / Testing
```

### Comparing `json5kit-0.3.2/README.md` & `json5kit-0.4.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,52 +1,54 @@
 # json5kit
 
 A Roundtrip parser and CST for JSON, JSONC and JSON5.
 
-> Currently a work in progress
+[JSON5](https://json5.org) is a superset of JSON, that allows trailing commas,
+comments, unquoted and single-quoted object keys, and a lot more.
 
-Currently supports parsing all of JSON syntax, and converting it back to source.
+Currently supports parsing most JSON5 syntax, and converting it back to source.
 Also supports single line `// comments`.
 
 ## Installation
 
 ```bash
 pip install json5kit
 ```
 
 ## Usage
 
 ```python
 >>> source = """
 ... {
-...   "items": [1, 2, 4],  // change this to 3
+...   items: [1, 2, 4],  // change this to 3
 ... }
 ... """
 >>> import json5kit
 >>> tree = json5kit.parse(source)
 >>> print(tree.to_source())
 
 {
-  "items": [1, 2, 4],  // change this to 3
+  items: [1, 2, 4],  // change this to 3
 }
 
 >>> print(tree.to_json())
 {"items":[1,2,4]}
+
 >>> # Let's replace the `4` with `3` now:
 >>> class ReplaceFourWithThree(json5kit.Json5Transformer):
 ...     def visit_Number(self, node):
 ...         if node.value == 4:
 ...             return node.replace(value=3)
 ...         return node
 ...
 >>> ReplaceFourWithThree().visit(tree)
 >>> print(tree.to_source())
 
 {
-  "items": [1, 2, 3],  // change this to 3
+  items: [1, 2, 3],  // change this to 3
 }
 >>> print(tree.to_json())
 {"items":[1,2,3]}
 ```
 
 ## Development / Testing
```

### Comparing `json5kit-0.3.2/setup.cfg` & `json5kit-0.4.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = json5kit
-version = 0.3.2
+version = 0.4.0
 description = A Roundtrip parser and CST for JSON, JSONC and JSON5.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tusharsadhwani/json5kit
 author = Tushar Sadhwani
 author_email = tushar.sadhwani000@gmail.com
 license = MIT
@@ -27,14 +27,15 @@
 package_dir = =src
 
 [options.packages.find]
 where = ./src
 
 [options.extras_require]
 dev = 
+	tox
 	black
 	mypy
 	pytest-cov
 	typing_extensions; python_version < "3.8"
 
 [tool:pytest]
 addopts = --cov --cov-report=term-missing
```

### Comparing `json5kit-0.3.2/src/json5kit/__init__.py` & `json5kit-0.4.0/src/json5kit/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 from json5kit.nodes import (
     Json5Array,
     Json5Boolean,
     Json5Comma,
     Json5Comment,
     Json5File,
+    Json5Identifier,
     Json5Key,
     Json5Newline,
     Json5Node,
     Json5Null,
     Json5Number,
     Json5Object,
     Json5Primitive,
@@ -193,19 +194,26 @@
         else:
             raise NotImplementedError(self.source[self.current])
 
         trailing_trivia_nodes = self.parse_trivia()
         node.trailing_trivia_nodes = trailing_trivia_nodes
         return node
 
-    # def parse_identifier(self) -> Json5Key:
-    #     """Scans keywords and variable names."""
-    #     # TODO: not full ECMA syntax
-    #     while not self.scanned and (self.peek().isalnum() or self.peek() == "_"):
-    #         self.advance()
+    def parse_identifier(self) -> str:
+        """
+        Scans keywords and variable names.
+        It doesn't check for the first letter being a non-number because the call-site
+        already confirms that.
+        """
+        # TODO: not full ECMA syntax
+        start_index = self.current
+        while not self.scanned and (self.peek().isalnum() or self.peek() == "_"):
+            self.advance()
+        identifier = self.source[start_index : self.current]
+        return identifier
 
     def parse_string(self, quote_char: Literal["'", '"']) -> tuple[str, str]:
         # TODO: this is probably not all escapes
         start_index = self.current
         unescaped_chars = []
         while not self.scanned and self.peek() != quote_char:
             char = self.read_char()
@@ -285,26 +293,33 @@
         while not self.scanned and not self.match_next("]"):
             items.append(self.parse_array_member())
 
         trailing_trivia_nodes = self.parse_trivia()
         return Json5Array(items, leading_trivia_nodes, trailing_trivia_nodes)
 
     def parse_object_entry(self) -> tuple[Json5Key, Json5Node]:
-        # TODO: identifier support
-        if not self.match_next(('"', "'")):
-            raise Json5ParseError(f"Expected to find identifier", index=self.current)
+        key_value_node: Json5String | Json5Identifier
+
+        if self.peek().isalpha() or self.peek() == "_":
+            source = self.parse_identifier()
+            trailing_trivia = self.parse_trivia()
+            key_value_node = Json5Identifier(source, trailing_trivia)
 
-        quote_char = cast(Literal['"', "'"], self.previous())
-        source, value = self.parse_string(quote_char)
-        string_trailing_trivia = self.parse_trivia()
-        string_node = Json5String(source, value, string_trailing_trivia)
+        elif self.match_next(('"', "'")):
+            quote_char = cast(Literal['"', "'"], self.previous())
+            source, value = self.parse_string(quote_char)
+            trailing_trivia = self.parse_trivia()
+            key_value_node = Json5String(source, value, trailing_trivia)
+
+        else:
+            raise Json5ParseError(f"Expected to find identifier", index=self.current)
 
         self.consume(":")
         trivia_after_colon = self.parse_trivia()
-        key_node = Json5Key(string_node, trivia_after_colon)
+        key_node = Json5Key(key_value_node, trivia_after_colon)
 
         value_node = self.parse_node()
         if self.peek() == "}":
             # Trailing comma not necessary for last element
             pass
         else:
             self.consume(",")
```

### Comparing `json5kit-0.3.2/src/json5kit/nodes.py` & `json5kit-0.4.0/src/json5kit/nodes.py`

 * *Files 12% similar despite different names*

```diff
@@ -96,19 +96,41 @@
         self,
         source: str,
         value: str,
         trailing_trivia_nodes: list[Json5Trivia],
     ) -> None:
         super().__init__(source, value, trailing_trivia_nodes)
 
+    def to_json(self) -> str:
+        if self.source.startswith("'"):
+            unquoted_source = self.source[1:-1]
+            return f'"{unquoted_source}"'
+
+        return self.source
+
+
+class Json5Identifier(Json5Primitive):
+    value: str
+
+    def __init__(
+        self,
+        source: str,
+        trailing_trivia_nodes: list[Json5Trivia],
+    ) -> None:
+        # the value is the same as the source
+        super().__init__(source, source, trailing_trivia_nodes)
+
+    def to_json(self) -> str:
+        return f'"{self.source}"'
+
 
 class Json5Key:
     def __init__(
         self,
-        value: Json5String,  # TODO: identifier support
+        value: Json5String | Json5Identifier,
         trailing_trivia_nodes: list[Json5Trivia],
     ) -> None:
         self.value = value
         self.trailing_trivia_nodes = trailing_trivia_nodes
 
     def to_source(self) -> str:
         return (
```

### Comparing `json5kit-0.3.2/src/json5kit/visitor.py` & `json5kit-0.4.0/src/json5kit/visitor.py`

 * *Files identical despite different names*

### Comparing `json5kit-0.3.2/src/json5kit.egg-info/PKG-INFO` & `json5kit-0.4.0/src/json5kit.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json5kit
-Version: 0.3.2
+Version: 0.4.0
 Summary: A Roundtrip parser and CST for JSON, JSONC and JSON5.
 Home-page: https://github.com/tusharsadhwani/json5kit
 Author: Tushar Sadhwani
 Author-email: tushar.sadhwani000@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,55 +21,57 @@
 Provides-Extra: dev
 License-File: LICENSE
 
 # json5kit
 
 A Roundtrip parser and CST for JSON, JSONC and JSON5.
 
-> Currently a work in progress
+[JSON5](https://json5.org) is a superset of JSON, that allows trailing commas,
+comments, unquoted and single-quoted object keys, and a lot more.
 
-Currently supports parsing all of JSON syntax, and converting it back to source.
+Currently supports parsing most JSON5 syntax, and converting it back to source.
 Also supports single line `// comments`.
 
 ## Installation
 
 ```bash
 pip install json5kit
 ```
 
 ## Usage
 
 ```python
 >>> source = """
 ... {
-...   "items": [1, 2, 4],  // change this to 3
+...   items: [1, 2, 4],  // change this to 3
 ... }
 ... """
 >>> import json5kit
 >>> tree = json5kit.parse(source)
 >>> print(tree.to_source())
 
 {
-  "items": [1, 2, 4],  // change this to 3
+  items: [1, 2, 4],  // change this to 3
 }
 
 >>> print(tree.to_json())
 {"items":[1,2,4]}
+
 >>> # Let's replace the `4` with `3` now:
 >>> class ReplaceFourWithThree(json5kit.Json5Transformer):
 ...     def visit_Number(self, node):
 ...         if node.value == 4:
 ...             return node.replace(value=3)
 ...         return node
 ...
 >>> ReplaceFourWithThree().visit(tree)
 >>> print(tree.to_source())
 
 {
-  "items": [1, 2, 3],  // change this to 3
+  items: [1, 2, 3],  // change this to 3
 }
 >>> print(tree.to_json())
 {"items":[1,2,3]}
 ```
 
 ## Development / Testing
```

