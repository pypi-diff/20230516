# Comparing `tmp/typegraph-0.1.7.tar.gz` & `tmp/typegraph-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typegraph-0.1.7.tar", max compression
+gzip compressed data, was "typegraph-0.1.8.tar", max compression
```

## Comparing `typegraph-0.1.7.tar` & `typegraph-0.1.8.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     5254 2023-05-02 08:12:21.968983 typegraph-0.1.7/LICENSE.md
--rw-r--r--   0        0        0     1445 2023-05-02 08:12:21.968983 typegraph-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      225 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/__init__.py
--rw-r--r--   0        0        0      904 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/effects.py
--rw-r--r--   0        0        0     3323 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/graph/auth/__init__.py
--rw-r--r--   0        0        0      377 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/graph/auth/oauth2.py
--rw-r--r--   0        0        0     1868 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/graph/builder.py
--rw-r--r--   0        0        0     3066 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/graph/models.py
--rw-r--r--   0        0        0     1953 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/graph/nodes.py
--rw-r--r--   0        0        0     5774 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/graph/typegraph.py
--rw-r--r--   0        0        0     7955 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/importers/base/importer.py
--rw-r--r--   0        0        0     3667 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/importers/base/typify.py
--rw-r--r--   0        0        0     7499 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/importers/google_discovery.py
--rw-r--r--   0        0        0     4236 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/importers/graphql.py
--rw-r--r--   0        0        0     8909 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/importers/openapi.py
--rw-r--r--   0        0        0     3904 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/injection.py
--rw-r--r--   0        0        0     4338 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/policies.py
--rw-r--r--   0        0        0     1675 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/providers/aws/runtimes/s3.py
--rw-r--r--   0        0        0    28490 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/providers/prisma/relations.py
--rw-r--r--   0        0        0    22924 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/providers/prisma/runtimes/prisma.py
--rw-r--r--   0        0        0     6601 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/providers/prisma/schema.py
--rw-r--r--   0        0        0    15008 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/providers/prisma/type_generator.py
--rw-r--r--   0        0        0     2373 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/providers/prisma/utils.py
--rw-r--r--   0        0        0     2209 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/providers/temporal/runtimes/temporal.py
--rw-r--r--   0        0        0     1351 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/runtimes/base.py
--rw-r--r--   0        0        0     5234 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/runtimes/deno.py
--rw-r--r--   0        0        0     1403 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/runtimes/graphql.py
--rw-r--r--   0        0        0     2789 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/runtimes/http.py
--rw-r--r--   0        0        0     1352 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/runtimes/python_wasi.py
--rw-r--r--   0        0        0     2880 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/runtimes/random.py
--rw-r--r--   0        0        0     2053 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/runtimes/typegate.py
--rw-r--r--   0        0        0     1169 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/runtimes/wasmedge.py
--rw-r--r--   0        0        0    20388 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/types.py
--rw-r--r--   0        0        0      487 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/utils/__init__.py
--rw-r--r--   0        0        0      644 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/utils/attrs.py
--rw-r--r--   0        0        0     1977 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/utils/jsonschema.py
--rw-r--r--   0        0        0     2198 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/utils/loaders.py
--rw-r--r--   0        0        0      185 2023-05-02 08:12:21.972983 typegraph-0.1.7/typegraph/utils/sanitizers.py
--rw-r--r--   0        0        0     1484 1970-01-01 00:00:00.000000 typegraph-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     5254 2023-05-16 07:53:50.765317 typegraph-0.1.8/LICENSE.md
+-rw-r--r--   0        0        0     1446 2023-05-16 07:53:50.765317 typegraph-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      225 2023-05-16 07:53:50.769317 typegraph-0.1.8/typegraph/__init__.py
+-rw-r--r--   0        0        0      904 2023-05-16 07:53:50.769317 typegraph-0.1.8/typegraph/effects.py
+-rw-r--r--   0        0        0     3323 2023-05-16 07:53:50.769317 typegraph-0.1.8/typegraph/graph/auth/__init__.py
+-rw-r--r--   0        0        0      377 2023-05-16 07:53:50.769317 typegraph-0.1.8/typegraph/graph/auth/oauth2.py
+-rw-r--r--   0        0        0     1868 2023-05-16 07:53:50.769317 typegraph-0.1.8/typegraph/graph/builder.py
+-rw-r--r--   0        0        0     3066 2023-05-16 07:53:50.769317 typegraph-0.1.8/typegraph/graph/models.py
+-rw-r--r--   0        0        0     1953 2023-05-16 07:53:50.769317 typegraph-0.1.8/typegraph/graph/nodes.py
+-rw-r--r--   0        0        0     5774 2023-05-16 07:53:50.769317 typegraph-0.1.8/typegraph/graph/typegraph.py
+-rw-r--r--   0        0        0     9347 2023-05-16 07:53:50.769317 typegraph-0.1.8/typegraph/importers/base/importer.py
+-rw-r--r--   0        0        0     3667 2023-05-16 07:53:50.769317 typegraph-0.1.8/typegraph/importers/base/typify.py
+-rw-r--r--   0        0        0     7421 2023-05-16 07:53:50.769317 typegraph-0.1.8/typegraph/importers/google_discovery.py
+-rw-r--r--   0        0        0     4236 2023-05-16 07:53:50.769317 typegraph-0.1.8/typegraph/importers/graphql.py
+-rw-r--r--   0        0        0     8909 2023-05-16 07:53:50.769317 typegraph-0.1.8/typegraph/importers/openapi.py
+-rw-r--r--   0        0        0     3904 2023-05-16 07:53:50.769317 typegraph-0.1.8/typegraph/injection.py
+-rw-r--r--   0        0        0     4338 2023-05-16 07:53:50.769317 typegraph-0.1.8/typegraph/policies.py
+-rw-r--r--   0        0        0     1761 2023-05-16 07:53:50.769317 typegraph-0.1.8/typegraph/providers/aws/runtimes/s3.py
+-rw-r--r--   0        0        0    28490 2023-05-16 07:53:50.769317 typegraph-0.1.8/typegraph/providers/prisma/relations.py
+-rw-r--r--   0        0        0    17565 2023-05-16 07:53:50.769317 typegraph-0.1.8/typegraph/providers/prisma/runtimes/prisma.py
+-rw-r--r--   0        0        0     6601 2023-05-16 07:53:50.769317 typegraph-0.1.8/typegraph/providers/prisma/schema.py
+-rw-r--r--   0        0        0    15008 2023-05-16 07:53:50.769317 typegraph-0.1.8/typegraph/providers/prisma/type_generator.py
+-rw-r--r--   0        0        0     2373 2023-05-16 07:53:50.769317 typegraph-0.1.8/typegraph/providers/prisma/utils.py
+-rw-r--r--   0        0        0     2185 2023-05-16 07:53:50.769317 typegraph-0.1.8/typegraph/providers/temporal/runtimes/temporal.py
+-rw-r--r--   0        0        0     1351 2023-05-16 07:53:50.773317 typegraph-0.1.8/typegraph/runtimes/base.py
+-rw-r--r--   0        0        0     5322 2023-05-16 07:53:50.773317 typegraph-0.1.8/typegraph/runtimes/deno.py
+-rw-r--r--   0        0        0     1494 2023-05-16 07:53:50.773317 typegraph-0.1.8/typegraph/runtimes/graphql.py
+-rw-r--r--   0        0        0     2598 2023-05-16 07:53:50.773317 typegraph-0.1.8/typegraph/runtimes/http.py
+-rw-r--r--   0        0        0     1431 2023-05-16 07:53:50.773317 typegraph-0.1.8/typegraph/runtimes/python.py
+-rw-r--r--   0        0        0     2949 2023-05-16 07:53:50.773317 typegraph-0.1.8/typegraph/runtimes/random.py
+-rw-r--r--   0        0        0     2053 2023-05-16 07:53:50.773317 typegraph-0.1.8/typegraph/runtimes/typegate.py
+-rw-r--r--   0        0        0     1178 2023-05-16 07:53:50.773317 typegraph-0.1.8/typegraph/runtimes/wasmedge.py
+-rw-r--r--   0        0        0    22574 2023-05-16 07:53:50.773317 typegraph-0.1.8/typegraph/types.py
+-rw-r--r--   0        0        0      487 2023-05-16 07:53:50.773317 typegraph-0.1.8/typegraph/utils/__init__.py
+-rw-r--r--   0        0        0      644 2023-05-16 07:53:50.773317 typegraph-0.1.8/typegraph/utils/attrs.py
+-rw-r--r--   0        0        0     1977 2023-05-16 07:53:50.773317 typegraph-0.1.8/typegraph/utils/jsonschema.py
+-rw-r--r--   0        0        0     2198 2023-05-16 07:53:50.773317 typegraph-0.1.8/typegraph/utils/loaders.py
+-rw-r--r--   0        0        0      185 2023-05-16 07:53:50.773317 typegraph-0.1.8/typegraph/utils/sanitizers.py
+-rw-r--r--   0        0        0     1485 1970-01-01 00:00:00.000000 typegraph-0.1.8/PKG-INFO
```

### Comparing `typegraph-0.1.7/LICENSE.md` & `typegraph-0.1.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.7/pyproject.toml` & `typegraph-0.1.8/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "typegraph"
-version = "0.1.7"
-description = "Compose your data, anywhere, and build iterative API blocks with zero-trust and serverless deployment, no matter where and how your (legacy) systems are."
+version = "0.1.8"
+description = "The low-code API platform for developers. Build modular APIs with zero-trust and serverless deployment, no matter where and how your (legacy) systems are."
 authors = ["Metatype Contributors <support@metatype.dev>"]
 license = "ELv2"
 homepage = "https://metatype.dev"
 repository = "https://github.com/metatypedev/metatype"
 include = ["typegraph/**/*", "LICENSE.md"]
 keywords = ["api", "composition", "typesystem", "graphql", "ecosystem"]
 classifiers = [
```

### Comparing `typegraph-0.1.7/typegraph/effects.py` & `typegraph-0.1.8/typegraph/effects.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.7/typegraph/graph/auth/__init__.py` & `typegraph-0.1.8/typegraph/graph/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.7/typegraph/graph/builder.py` & `typegraph-0.1.8/typegraph/graph/builder.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.7/typegraph/graph/models.py` & `typegraph-0.1.8/typegraph/graph/models.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.7/typegraph/graph/nodes.py` & `typegraph-0.1.8/typegraph/graph/nodes.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.7/typegraph/graph/typegraph.py` & `typegraph-0.1.8/typegraph/graph/typegraph.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.7/typegraph/importers/base/importer.py` & `typegraph-0.1.8/typegraph/importers/base/importer.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,36 +5,51 @@
 import re
 import sys
 from ast import literal_eval
 from typing import Dict, List, Optional, Set, Tuple
 
 import black
 from attrs import define, field, frozen
+from box import Box
 from redbaron import AtomtrailersNode, NameNode, RedBaron
 
 from typegraph import TypeGraph, t
 from typegraph.importers.base.typify import Typify
 from typegraph.types import reserved_types
 
 # TODO: detect indentation size/character from file
 
 
 @define
 class Codegen:
     indent: str = field(default=" " * 4)
     indent_level: int = field(default=1)
+    indent_level_pyi: int = field(default=0)
     res: str = field(default="", init=False)
+    res_hint: str = field(default="", init=False)
 
     def line(self, line: str = "", indent_level=0):
         indent = self.indent * (self.indent_level + indent_level)
         if line == "":
             self.res += "\n"
         else:
             self.res += f"{indent}{line}\n"
 
+    def hint_line(self, line: str = "", indent_level=0):
+        indent = self.indent * (self.indent_level_pyi + indent_level)
+        if line == "":
+            self.res_hint += "\n"
+        else:
+            self.res_hint += f"{indent}{line}\n"
+
+
+# Some Type Name => Some_Type_Name
+def as_attr(name: str):
+    return re.sub(r"\s+", "_", name)
+
 
 class Importer:
     """Base importer class"""
 
     imports: Set[Tuple[str, str]]
     headers: List[str]  # codegen header lines
     name: str
@@ -73,14 +88,15 @@
             )
         self.renames.update({name: name for name in keep_names})
         reserved = [name for name in self.renames.values() if name in reserved_types]
         if len(reserved) > 0:
             raise Exception(f"Cannot use reserved types: {', '.join(reserved)}")
 
         self.tg = TypeGraph(name="__importer__")
+        self.type_hint = []
 
     def __enter__(self):
         ImporterContext.push(self)
         self.tg.__enter__()
         return self
 
     def __exit__(self, exc_type, exc_value, exc_tb):
@@ -116,58 +132,72 @@
         renames = {name: f"_{self.name}_{next(counter)}_{name}" for name in self.types}
         renames.update(self.renames)
 
         cg.line(f"renames = {repr(renames)}")
         cg.line()
 
         cg.line("types = {}")
+        cg.hint_line("from typegraph import t")
+        cg.hint_line("class TypeList:")
 
         if len(self.types) > 0:
             for name, tpe in self.types.items():
                 cg.line(f"types[{repr(name)}] = {typify(tpe, name)}")
+                cg.hint_line(f"{as_attr(name)}: t.typedef = ...", 1)
 
             cg.line()
 
         cg.line("functions = {}")
+        cg.hint_line("class FuncList:")
         for name, fn in self.exposed.items():
             cg.line(f"functions[{repr(name)}] = {typify(fn)}")
+            cg.hint_line(f"{as_attr(name)}: t.func = ...", 1)
         cg.line()
 
+        cg.hint_line("class Import:")
+        cg.hint_line("types: TypeList = ...", 1)
+        cg.hint_line("functions: FuncList = ...", 1)
+        cg.hint_line(f"def {self.get_def_name()}() -> Import: ...")
+
+        self.imports.add(("box", "Box"))
         self.imports.add(("typegraph.importers.base.importer", "Import"))
         cg.line(
-            f"return Import(importer={repr(self.name)}, renames=renames, types=types, functions=functions)"
+            f"return Import(importer={repr(self.name)}, renames=renames, types=Box(types), functions=Box(functions))"
         )
 
         return cg
 
+    def get_def_name(self):
+        return f"import_{self.name}"
+
     def imp(self, gen: bool):
         if not gen:
             return
 
         file = inspect.stack()[1].filename
 
         with open(file) as f:
             code = RedBaron(f.read())
 
         gen_arg = self.find_generate_arg(code)
         if not gen_arg:
             raise Exception("Expected to find generate argument import node")
         gen_arg.value = "False"
 
-        cg = self.codegen(Codegen()).res
+        source = self.codegen(Codegen())
 
         for frm, imp in self.imports:
             if not code.find(
                 "from_import",
                 value=lambda x: x.dumps() == frm,
                 targets=lambda x: x.dumps() == imp,
             ):
                 code.insert(0, f"from {frm} import {imp}\n")
 
-        name = f"import_{self.name}"
+        name = self.get_def_name()
         target_node = code.find("def", lambda node: node.name == name)
         wth = code.find("with")
 
         comment = f"# Function generated by {type(self).__name__}. Do not change."
 
         if target_node is not None:
             comment_node = next(
@@ -178,24 +208,29 @@
                 ),
                 None,
             )
             if comment_node.type != "comment":
                 target_node.insert_before(comment)
             else:
                 comment_node.value = comment
-            target_node.value = cg
+            target_node.value = source.res
         else:
             wth.insert_before(comment)
-            wth.insert_before(f"def {name}():\n{cg}")
+            wth.insert_before(f"def {name}():\n{source.res}")
 
         new_code = black.format_str(code.dumps(), mode=black.FileMode())
+        new_hint_code = black.format_str(source.res_hint, mode=black.FileMode())
 
         with open(file, "w") as f:
             f.write(new_code)
 
+        filename_pyi = re.sub(r"\.py$", ".pyi", file)
+        with open(filename_pyi, "w") as f:
+            f.write(new_hint_code)
+
         print(f"File updated: {file}", file=sys.stderr)
         exit(0)
 
     def find_generate_arg(self, code: RedBaron) -> Optional[NameNode]:
         for node in code.find_all("atomtrailers"):
             found = self.find_generate_arg_in(node)
             if found:
@@ -249,23 +284,26 @@
         return cls.importer
 
 
 @frozen
 class Import:
     importer: str
     renames: Dict[str, str]
-    types: Dict[str, t.typedef]
-    functions: Dict[str, t.func]
+    types: Box  # Dict[str, t.typedef]
+    functions: Box  # Dict[str, t.func]
 
     def type(self, name: str):
-        typ = self.types.get(name)
-        if typ is None:
+        try:
+            typ = getattr(self.types, name)
+            return typ
+        except Exception:
             raise Exception(f"Type '{name}' not found in import '{self.importer}")
 
     def func(self, name: str):
-        fn = self.functions.get(name)
-        if fn is None:
+        try:
+            fn = getattr(self.functions, name)
+            return fn
+        except Exception:
             raise Exception(f"Function '{name}' not found in import '{self.importer}'")
-        return fn
 
     def all(self):
         return self.functions
```

### Comparing `typegraph-0.1.7/typegraph/importers/base/typify.py` & `typegraph-0.1.8/typegraph/importers/base/typify.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.7/typegraph/importers/google_discovery.py` & `typegraph-0.1.8/typegraph/importers/google_discovery.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,16 +36,14 @@
         file: Optional[str] = None,
         renames: Dict[str, str] = {},
         keep_names: List[str] = [],
     ):
         super().__init__(name, renames=renames, keep_names=keep_names)
         self.imports = {
             ("typegraph", "t"),
-            ("typegraph", "TypeGraph"),
-            ("typegraph", "effects"),
             ("typegraph.runtimes.http", "HTTPRuntime"),
         }
 
         if file is None:
             self.specification = Box(httpx.get(url).json())
         else:
             with open(file) as f:
```

### Comparing `typegraph-0.1.7/typegraph/importers/graphql.py` & `typegraph-0.1.8/typegraph/importers/graphql.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.7/typegraph/importers/openapi.py` & `typegraph-0.1.8/typegraph/importers/openapi.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.7/typegraph/injection.py` & `typegraph-0.1.8/typegraph/injection.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.7/typegraph/policies.py` & `typegraph-0.1.8/typegraph/policies.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.7/typegraph/providers/aws/runtimes/s3.py` & `typegraph-0.1.8/typegraph/providers/aws/runtimes/s3.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 from typegraph.effects import Effect
 from typegraph.runtimes.base import Materializer, Runtime
 from typegraph.utils.attrs import always
 
 
 @frozen
 class S3Runtime(Runtime):
+    """
+    [Documentation](https://metatype.dev/docs/reference/runtimes/s3)
+    """
+
     host: str
     region: str
     access_key_secret: str
     secret_key_secret: str
     runtime_name: str = always("s3")
 
     def data(self, collector):
```

### Comparing `typegraph-0.1.7/typegraph/providers/prisma/relations.py` & `typegraph-0.1.8/typegraph/providers/prisma/relations.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.7/typegraph/providers/prisma/schema.py` & `typegraph-0.1.8/typegraph/providers/prisma/schema.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.7/typegraph/providers/prisma/type_generator.py` & `typegraph-0.1.8/typegraph/providers/prisma/type_generator.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.7/typegraph/providers/prisma/utils.py` & `typegraph-0.1.8/typegraph/providers/prisma/utils.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.7/typegraph/providers/temporal/runtimes/temporal.py` & `typegraph-0.1.8/typegraph/providers/temporal/runtimes/temporal.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,17 +5,16 @@
 from typegraph import types as t
 from typegraph.runtimes.base import Materializer, Runtime
 from typegraph.utils.attrs import always
 
 
 @frozen
 class TemporalRuntime(Runtime):
-    """Interacts with Temporal server.
-
-    This runtime is *experimental* state and is subject to change.
+    """
+    [Documentation](https://metatype.dev/docs/reference/runtimes/temporal)
     """
 
     host: str
     name: str
     runtime_name: str = always("temporal")
 
     def data(self, collector):
```

### Comparing `typegraph-0.1.7/typegraph/runtimes/base.py` & `typegraph-0.1.8/typegraph/runtimes/base.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.7/typegraph/runtimes/deno.py` & `typegraph-0.1.8/typegraph/runtimes/deno.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,18 @@
 from typegraph.graph.nodes import Node
 from typegraph.runtimes.base import Materializer, Runtime
 from typegraph.utils.attrs import SKIP, always
 
 
 @frozen
 class DenoRuntime(Runtime):
+    """
+    [Documentation](https://metatype.dev/docs/reference/runtimes/deno)
+    """
+
     worker: str = field(kw_only=True, default="default")
     allow_net: Tuple[str, ...] = field(
         kw_only=True, factory=tuple, metadata={SKIP: True}
     )
     permissions: Dict[str, Any] = field(factory=frozendict, init=False)
     runtime_name: str = always("deno")
```

### Comparing `typegraph-0.1.7/typegraph/runtimes/graphql.py` & `typegraph-0.1.8/typegraph/runtimes/graphql.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 from typegraph.effects import Effect
 from typegraph.runtimes.base import Materializer, Runtime
 from typegraph.utils.attrs import always, required
 
 
 @frozen
 class GraphQLRuntime(Runtime):
+    """
+    [Documentation](https://metatype.dev/docs/reference/runtimes/graphql)
+    """
+
     endpoint: str
     runtime_name: str = always("graphql")
 
     def query(
         self, inp: t.struct, out: t.typedef, *, path: Optional[Tuple[str, ...]] = None
     ):
         if path is not None and len(path) == 0:
```

### Comparing `typegraph-0.1.7/typegraph/runtimes/http.py` & `typegraph-0.1.8/typegraph/runtimes/http.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,27 +10,16 @@
 from typegraph.effects import Effect
 from typegraph.runtimes.base import Materializer, Runtime
 from typegraph.utils.attrs import always, required
 
 
 @frozen
 class HTTPRuntime(Runtime):
-    """Runs HTTP requests.
-
-    Example:
-    ```python
-    from typegraph.runtime.http import HTTPRuntime
-
-    remote = HTTPRuntime('https://dev.to/api')
-    remote.get(
-        '/test',
-        t.struct({}),
-        t.array(t.struct({'a': t.integer()})),
-    )
-    ```
+    """
+    [Documentation](https://metatype.dev/docs/reference/runtimes/http)
     """
 
     endpoint: str
     cert_secret: Optional[str] = None
     basic_auth_secret: Optional[str] = None
     runtime_name: str = always("http")
```

### Comparing `typegraph-0.1.7/typegraph/runtimes/python_wasi.py` & `typegraph-0.1.8/typegraph/runtimes/python.py`

 * *Files 20% similar despite different names*

```diff
@@ -28,15 +28,19 @@
         self.lambdas = []
 
     def visit_Lambda(self, node):
         self.lambdas.append(unparse(node).strip())
 
 
 @frozen
-class PythonWasiRuntime(Runtime):
+class Python(Runtime):
+    """
+    [Documentation](https://metatype.dev/docs/reference/runtimes/python)
+    """
+
     runtime_name: str = always("python_wasi")
 
     def from_lambda(self, function):
         lambdas = LambdaCollector.collect(function)
         assert len(lambdas) == 1
         fn = str(lambdas[0])
         m = hashlib.sha256()
```

### Comparing `typegraph-0.1.7/typegraph/runtimes/random.py` & `typegraph-0.1.8/typegraph/runtimes/random.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 # Copyright Metatype OÜ under the Elastic License 2.0 (ELv2). See LICENSE.md for usage.
 
 from typing import Callable, Dict, List, Optional
 
 from attrs import field, frozen
 
-from typegraph import effects
+from typegraph import effects, utils
 from typegraph import types as t
-from typegraph import utils
 from typegraph.effects import Effect
 from typegraph.runtimes.base import Materializer, Runtime
 from typegraph.utils.attrs import always
 
 
 def pick(d: Dict, *largs) -> Dict:
     return utils.drop_nones(utils.pick(d, *largs))
 
 
 @frozen
 class RandomRuntime(Runtime):
+    """
+    [Documentation](https://metatype.dev/docs/reference/runtimes/random)
+    """
+
     runtime_name: str = always("random")
     seed: Optional[int] = field(kw_only=True, default=None)
     reset: str = field(kw_only=True, default="")
 
     def get_type_config(self, tpe: "t.typedef") -> Dict:
         base = tpe.runtime_config
```

### Comparing `typegraph-0.1.7/typegraph/runtimes/typegate.py` & `typegraph-0.1.8/typegraph/runtimes/typegate.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.7/typegraph/runtimes/wasmedge.py` & `typegraph-0.1.8/typegraph/runtimes/wasmedge.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,17 +10,16 @@
 from typegraph.effects import Effect
 from typegraph.runtimes.base import Materializer, Runtime
 from typegraph.utils.attrs import always, required
 
 
 @frozen
 class WasmEdgeRuntime(Runtime):
-    """Runs Wasm functions on the WasmEdge runtime.
-
-    **Experimental**
+    """
+    [Documentation](https://metatype.dev/docs/reference/runtimes/wasmedge)
     """
 
     runtime_name: str = always("wasmedge")
 
     def data(self, collector):
         return {
             **super().data(collector),
```

### Comparing `typegraph-0.1.7/typegraph/types.py` & `typegraph-0.1.8/typegraph/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,24 +113,27 @@
     policies: Tuple[Policy, ...] = field(kw_only=True, factory=tuple)
     # runtime_config: Dict[str, Any] = field(
     #     kw_only=True, factory=dict, hash=False, metadata={SKIP: True}
     # )
     runtime_config: Dict[str, Any] = field(
         kw_only=True, factory=frozendict, hash=False, metadata={SKIP: True}
     )
-    _enum: Optional[Tuple[Any]] = optional_field()
+    _enum: Optional[Tuple[str]] = optional_field()
 
     collector_target: Optional[str] = always(Collector.types)
 
     def __attrs_post_init__(self):
         if self.graph is None:
             raise Exception("No typegraph context")
         if self.name == "":
             object.__setattr__(self, "name", f"{self.type}_{self.graph.next_type_id()}")
 
+    def overwrite_name(self, name: str):
+        object.__setattr__(self, "name", name)
+
     def replace(self, **changes) -> Self:
         return evolve(self, **changes)
 
     @property
     def type(self):
         return type(self).__name__
 
@@ -202,15 +205,14 @@
 
         for e in self.edges:
             if isinstance(e, typedef):
                 e._propagate_runtime(self.runtime, visited)
             if isinstance(e, NodeProxy):
                 e.get()._propagate_runtime(self.runtime, visited)
 
-    # TODO @overload
     @overload
     def inject(self, injection: Injection) -> Self:
         pass
 
     @overload
     def inject(self, injection: Dict[Optional[EffectType], Injection]) -> Self:
         pass
@@ -247,15 +249,17 @@
         d = dict()
         d.update(self.runtime_config)
         d.update(kwargs)
         d.update({f: True for f in flags})
         return self.replace(runtime_config=frozendict(d))
 
     def enum(self, variants: List[Any]) -> Self:
-        return self.replace(enum=tuple(variants))
+        import json
+
+        return self.replace(enum=tuple(json.dumps(variant) for variant in variants))
 
     def data(self, collector) -> dict:
         if self.runtime is None:
             raise Exception("Expected Runtime, got None")
 
         ret = remove_none_values(asdict(self))
         ret["type"] = self.type
@@ -483,15 +487,14 @@
 
 
 def date() -> string:
     return string().format("date")
 
 
 def phone() -> string:
-    # TODO replace with the phone number pattern when typechecking
     return string().format("phone")
 
 
 def enum(variants: List[str]) -> string:
     return string().enum(variants)
 
 
@@ -510,14 +513,57 @@
         validator=[validate_struct_props], factory=frozendict, converter=frozendict
     )
     additional_props: Optional[Union[bool, TypeNode]] = None
     _min: Optional[int] = constraint("minProperties")
     _max: Optional[int] = constraint("maxProperties")
     # _dependentRequired
 
+    def __attrs_post_init__(self):
+        super().__attrs_post_init__()
+        if self.__class__ != struct:
+            # TODO implement recursive props resolution for parent class
+            # https://en.wikipedia.org/wiki/C3_linearization
+            if len(self.__class__.__bases__) > 1:
+                raise Exception("multiple inheritance is currently not supported")
+            (base,) = self.__class__.__bases__
+            child_cls = self.__class__
+            child_attr = set([i for i in vars(child_cls) if not i.startswith("__")])
+            parent_attr = set([i for i in vars(base) if not i.startswith("__")])
+
+            # reserved field check
+            reserved_attr = set(vars(struct)).union(vars(typedef))
+            common = sorted(reserved_attr.intersection(child_attr))
+            if len(common) > 0:
+                err_msg = ", ".join(common)
+                if len(common) == 1:
+                    err_msg += " is a reserved field"
+                else:
+                    err_msg += " are reserved fields"
+                raise Exception(err_msg)
+            self_attr = child_attr
+            if base != struct:
+                # child.props should inherit parent.props
+                curr_base = base
+                while curr_base != struct:
+                    if len(curr_base.__bases__) > 1:
+                        raise Exception(
+                            "multiple inheritance is currently not supported"
+                        )
+                    (curr_base,) = curr_base.__bases__
+                    fields = set([i for i in vars(curr_base) if not i.startswith("__")])
+                    parent_attr = parent_attr.union(fields)
+                self_attr = self_attr.union(parent_attr)
+            props = {}
+            for attr in sorted(self_attr):
+                value = getattr(self, attr)
+                if isinstance(value, typedef):
+                    props[attr] = value
+            # self.overwrite_name(self.__class__.__name__)
+            object.__setattr__(self, "props", frozendict(props))
+
     def additional(self, t: Union[bool, TypeNode]):
         return self.replace(additional_props=t)
 
     # creates a duplicate type with no runtime
     def detach(self):
         return self.replace(
             name=f"{self.type}_{self.graph.next_type_id()}", runtime=None
@@ -528,21 +574,21 @@
         new_props.update(props)
         return self.replace(
             props=frozendict(new_props), name=f"{self.type}_{self.graph.next_type_id()}"
         )
 
     def __getattr__(self, attr):
         try:
+            if attr == "props":
+                return self.props
             return super().__getattr__(attr)
         except AttributeError:
             pass
-
         if attr in self.props:
             return self.props[attr]
-
         raise Exception(f'no prop named "{attr}" in type {self}')
 
     @property
     def type(self):
         return "object"
 
     @property
```

### Comparing `typegraph-0.1.7/typegraph/utils/attrs.py` & `typegraph-0.1.8/typegraph/utils/attrs.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.7/typegraph/utils/jsonschema.py` & `typegraph-0.1.8/typegraph/utils/jsonschema.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.7/typegraph/utils/loaders.py` & `typegraph-0.1.8/typegraph/utils/loaders.py`

 * *Files identical despite different names*

### Comparing `typegraph-0.1.7/PKG-INFO` & `typegraph-0.1.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: typegraph
-Version: 0.1.7
-Summary: Compose your data, anywhere, and build iterative API blocks with zero-trust and serverless deployment, no matter where and how your (legacy) systems are.
+Version: 0.1.8
+Summary: The low-code API platform for developers. Build modular APIs with zero-trust and serverless deployment, no matter where and how your (legacy) systems are.
 Home-page: https://metatype.dev
 License: ELv2
 Keywords: api,composition,typesystem,graphql,ecosystem
 Author: Metatype Contributors
 Author-email: support@metatype.dev
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
```

