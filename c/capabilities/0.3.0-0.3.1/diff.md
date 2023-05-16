# Comparing `tmp/capabilities-0.3.0.tar.gz` & `tmp/capabilities-0.3.1.tar.gz`

## Comparing `capabilities-0.3.0.tar` & `capabilities-0.3.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 capabilities-0.3.0/setup.py
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 capabilities-0.3.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 capabilities-0.3.0/capabilities/__about__.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 capabilities-0.3.0/capabilities/__init__.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 capabilities-0.3.0/capabilities/__main__.py
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 capabilities-0.3.0/capabilities/cli.py
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 capabilities-0.3.0/capabilities/config.py
--rw-r--r--   0        0        0    16630 2020-02-02 00:00:00.000000 capabilities-0.3.0/capabilities/core.py
--rw-r--r--   0        0        0     6785 2020-02-02 00:00:00.000000 capabilities-0.3.0/capabilities/dec.py
--rw-r--r--   0        0        0    15089 2020-02-02 00:00:00.000000 capabilities-0.3.0/capabilities/example.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 capabilities-0.3.0/capabilities/search/__init__.py
--rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 capabilities-0.3.0/capabilities/search/hf.py
--rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 capabilities-0.3.0/capabilities/search/loader.py
--rw-r--r--   0        0        0     6082 2020-02-02 00:00:00.000000 capabilities-0.3.0/capabilities/search/nomic_index.py
--rw-r--r--   0        0        0     6286 2020-02-02 00:00:00.000000 capabilities-0.3.0/capabilities/search/oai.py
--rw-r--r--   0        0        0    12426 2020-02-02 00:00:00.000000 capabilities-0.3.0/capabilities/search/search_index.py
--rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 capabilities-0.3.0/capabilities/search/simple_vector_index.py
--rw-r--r--   0        0        0     7076 2020-02-02 00:00:00.000000 capabilities-0.3.0/capabilities/search/types.py
--rw-r--r--   0        0        0     5233 2020-02-02 00:00:00.000000 capabilities-0.3.0/capabilities/search/util.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 capabilities-0.3.0/capabilities/util/__init__.py
--rw-r--r--   0        0        0     8767 2020-02-02 00:00:00.000000 capabilities-0.3.0/capabilities/util/config.py
--rw-r--r--   0        0        0     6628 2020-02-02 00:00:00.000000 capabilities-0.3.0/capabilities/util/misc.py
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 capabilities-0.3.0/examples/cheese.py
--rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 capabilities-0.3.0/examples/leansearch.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 capabilities-0.3.0/examples/readme.txt
--rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 capabilities-0.3.0/examples/tesla10k.py
--rw-r--r--   0        0        0   840980 2020-02-02 00:00:00.000000 capabilities-0.3.0/examples/data/apple10k.pdf
--rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 capabilities-0.3.0/examples/data/sample.md
--rw-r--r--   0        0        0     7945 2020-02-02 00:00:00.000000 capabilities-0.3.0/examples/data/sample.pdf
--rw-r--r--   0        0        0   157134 2020-02-02 00:00:00.000000 capabilities-0.3.0/examples/data/tesla10k.txt
--rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 capabilities-0.3.0/tests/test_dec.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 capabilities-0.3.0/tests/test_document_loader.py
--rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 capabilities-0.3.0/tests/test_search.py
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 capabilities-0.3.0/tests/test_search_util.py
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 capabilities-0.3.0/tests/test_tutorial1.py
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 capabilities-0.3.0/tests/test_vector_idx.py
--rw-r--r--   0        0        0   353564 2020-02-02 00:00:00.000000 capabilities-0.3.0/tests/snapshots/test_search/test_search_e2e/NomicIndex-openai/r0.txt
--rw-r--r--   0        0        0   353563 2020-02-02 00:00:00.000000 capabilities-0.3.0/tests/snapshots/test_search/test_search_e2e/NomicIndex-sentence-transformersall-MiniLM-L6-v2/r0.txt
--rw-r--r--   0        0        0   353563 2020-02-02 00:00:00.000000 capabilities-0.3.0/tests/snapshots/test_search/test_search_e2e/SearchIndex-openai/r0.txt
--rw-r--r--   0        0        0   353565 2020-02-02 00:00:00.000000 capabilities-0.3.0/tests/snapshots/test_search/test_search_e2e/SearchIndex-sentence-transformersall-MiniLM-L6-v2/r0.txt
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 capabilities-0.3.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 capabilities-0.3.0/LICENSE
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 capabilities-0.3.0/README.md
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 capabilities-0.3.0/pyproject.toml
--rw-r--r--   0        0        0    14266 2020-02-02 00:00:00.000000 capabilities-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 capabilities-0.3.1/setup.py
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 capabilities-0.3.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 capabilities-0.3.1/capabilities/__about__.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 capabilities-0.3.1/capabilities/__init__.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 capabilities-0.3.1/capabilities/__main__.py
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 capabilities-0.3.1/capabilities/cli.py
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 capabilities-0.3.1/capabilities/config.py
+-rw-r--r--   0        0        0    16987 2020-02-02 00:00:00.000000 capabilities-0.3.1/capabilities/core.py
+-rw-r--r--   0        0        0     8071 2020-02-02 00:00:00.000000 capabilities-0.3.1/capabilities/dec.py
+-rw-r--r--   0        0        0    15162 2020-02-02 00:00:00.000000 capabilities-0.3.1/capabilities/example.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 capabilities-0.3.1/capabilities/search/__init__.py
+-rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 capabilities-0.3.1/capabilities/search/hf.py
+-rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 capabilities-0.3.1/capabilities/search/loader.py
+-rw-r--r--   0        0        0     6082 2020-02-02 00:00:00.000000 capabilities-0.3.1/capabilities/search/nomic_index.py
+-rw-r--r--   0        0        0     6286 2020-02-02 00:00:00.000000 capabilities-0.3.1/capabilities/search/oai.py
+-rw-r--r--   0        0        0    12426 2020-02-02 00:00:00.000000 capabilities-0.3.1/capabilities/search/search_index.py
+-rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 capabilities-0.3.1/capabilities/search/simple_vector_index.py
+-rw-r--r--   0        0        0     7076 2020-02-02 00:00:00.000000 capabilities-0.3.1/capabilities/search/types.py
+-rw-r--r--   0        0        0     5313 2020-02-02 00:00:00.000000 capabilities-0.3.1/capabilities/search/util.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 capabilities-0.3.1/capabilities/util/__init__.py
+-rw-r--r--   0        0        0     8767 2020-02-02 00:00:00.000000 capabilities-0.3.1/capabilities/util/config.py
+-rw-r--r--   0        0        0     6628 2020-02-02 00:00:00.000000 capabilities-0.3.1/capabilities/util/misc.py
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 capabilities-0.3.1/examples/cheese.py
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 capabilities-0.3.1/examples/leansearch.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 capabilities-0.3.1/examples/readme.txt
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 capabilities-0.3.1/examples/tesla10k.py
+-rw-r--r--   0        0        0   840980 2020-02-02 00:00:00.000000 capabilities-0.3.1/examples/data/apple10k.pdf
+-rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 capabilities-0.3.1/examples/data/sample.md
+-rw-r--r--   0        0        0     7945 2020-02-02 00:00:00.000000 capabilities-0.3.1/examples/data/sample.pdf
+-rw-r--r--   0        0        0   157134 2020-02-02 00:00:00.000000 capabilities-0.3.1/examples/data/tesla10k.txt
+-rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 capabilities-0.3.1/tests/test_dec.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 capabilities-0.3.1/tests/test_document_loader.py
+-rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 capabilities-0.3.1/tests/test_search.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 capabilities-0.3.1/tests/test_search_util.py
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 capabilities-0.3.1/tests/test_tutorial1.py
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 capabilities-0.3.1/tests/test_vector_idx.py
+-rw-r--r--   0        0        0   353564 2020-02-02 00:00:00.000000 capabilities-0.3.1/tests/snapshots/test_search/test_search_e2e/NomicIndex-openai/r0.txt
+-rw-r--r--   0        0        0   353563 2020-02-02 00:00:00.000000 capabilities-0.3.1/tests/snapshots/test_search/test_search_e2e/NomicIndex-sentence-transformersall-MiniLM-L6-v2/r0.txt
+-rw-r--r--   0        0        0   353563 2020-02-02 00:00:00.000000 capabilities-0.3.1/tests/snapshots/test_search/test_search_e2e/SearchIndex-openai/r0.txt
+-rw-r--r--   0        0        0   353565 2020-02-02 00:00:00.000000 capabilities-0.3.1/tests/snapshots/test_search/test_search_e2e/SearchIndex-sentence-transformersall-MiniLM-L6-v2/r0.txt
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 capabilities-0.3.1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 capabilities-0.3.1/LICENSE
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 capabilities-0.3.1/README.md
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 capabilities-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0    14287 2020-02-02 00:00:00.000000 capabilities-0.3.1/PKG-INFO
```

### Comparing `capabilities-0.3.0/.github/workflows/python-publish.yml` & `capabilities-0.3.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.0/capabilities/cli.py` & `capabilities-0.3.1/capabilities/cli.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.0/capabilities/config.py` & `capabilities-0.3.1/capabilities/config.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.0/capabilities/core.py` & `capabilities-0.3.1/capabilities/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import os
 import dataclasses
 import typing
 import dacite
 from dataclasses import dataclass, field, is_dataclass
-from typing import Dict, Any, List, Type, TypeAlias, TypeVar, Union, Literal
+from typing import Dict, Any, List, Type, TypeVar, Union, Literal
 from typing import Optional
+try:
+    from typing import TypeAlias
+except:
+    from typing_extensions import TypeAlias
 import requests
 import aiohttp
 import asyncio
 import time
 
 import aiohttp
 import dacite
@@ -27,32 +31,34 @@
 
 
 @dataclass
 class CapabilityBase:
     ...
 
 
+from termcolor import colored
+
 @dataclass
 class Capability(CapabilityBase):
     uri: str
     _capability: Optional[CapabilityBase] = None
 
     def __call__(self, *args, **kwargs):
+        print(colored("[  ✓  ]", "green"), f"Capability({self.uri}) running with {len(args) + len(kwargs)} arguments")
         return self._capability(*args, **kwargs)
 
     async def run_async(self, *args, **kwargs):
+        print(colored("[  ✓  ]", "green"), f"Capability({self.uri}) running async with {len(args) + len(kwargs)} arguments")
         return await self._capability.run_async(*args, **kwargs)
 
     def __post_init__(self):
         try:
             self._capability = _CAPABILITIES[self.uri]
         except KeyError as e:
-            print(
-                f"KeyError={e}\nCapability lookup failed for uri={self.uri}.\nValid URIs are:"
-            )
+            print(colored("[  ✗  ]", "red"), f"KeyError={e}\nCapability lookup failed for uri={self.uri}.\nValid URIs are:")
             for k in _CAPABILITIES.keys():
                 print(f"  {k}")
 
 
 from functools import wraps
 import inspect
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `capabilities-0.3.0/capabilities/dec.py` & `capabilities-0.3.1/capabilities/dec.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import sys
+from termcolor import colored
 import functools
 import ast
 import inspect
 import importlib
 from typing import Callable, Generic, ParamSpec, TypeVar, overload
 import warnings
 
@@ -53,14 +55,15 @@
         self.signature = inspect.signature(func)
         self.input_spec = {
             k: _flatten_param(p, path=[k]) for k, p in self.signature.parameters.items()
         }
         self.output_spec = flatten_model(self.signature.return_annotation)
 
     def __call__(self, *args: P.args, **kwargs: P.kwargs):
+        print(f"[llm] running with {len(args) + len(kwargs)} arguments")
         binding = self.signature.bind(*args, **kwargs)
         binding.apply_defaults()
         input_dict = {k: to_dict(v) for k, v in binding.arguments.items()}
         # [todo](ed) currently endpoint can't handle having root spec not be a dictionary.
         wrap_output = not isinstance(self.output_spec, dict)
         if wrap_output:
             output_spec = {"output": self.output_spec}
@@ -138,21 +141,39 @@
         if not regenerate:  # no-op if `regenerate==False`
             return func
 
         lines, start_lineno = inspect.getsourcelines(func)
         code_before, code_after = get_llm_inline_context(func)
 
         for _ in range(num_tries):  # Try `num_tries` times
+            print("[llm_inline] generating code")
             completed = complete_code("\n".join(lines[1:]), code_before, code_after)
 
             # Try to parse out the function body, but if unsuccessful, fall back to the original completion.
+            print("[llm_inline] postprocessing")            
             processed = postprocess(completed, func.__name__)
             completed = processed if processed else completed
+            print("[llm_inline] postprocessing complete")                        
             new_decorator = f"@llm_inline(regenerate=False)"
-            if input(f"The following code will be written to your file: \n{completed}\nContinue? (y/n)") == "y":
+            # if input(f"The following code will be written to your file: \n{completed}\nContinue? (y/n) ") == "y":
+            #     with open(inspect.getfile(func), "w") as f:
+            #         f.write(f"{code_before}\n{new_decorator}\n{completed}\n{code_after}")
+
+            #     # Reload the module and the functions
+            #     # todo: reload the script itself could result in ModuleNotFoundError: spec not found for the module '__main__'.
+            #     #       Trying an dirty way but may need to explore best-practice later.
+            #     try:
+            #         module = inspect.getmodule(func)
+            #         importlib.reload(module)
+            #         globals().update(vars(module))
+            #         return getattr(module, func.__name__)
+            #     except:
+            #         exec(completed, globals())
+            #         return globals()[func.__name__]
+            if input(colored("The following code will be written to your file: \n", "green") + colored(f"{completed}\n", "blue") + colored("Continue? (y/n) ", "green")) == "y":
                 with open(inspect.getfile(func), "w") as f:
                     f.write(f"{code_before}\n{new_decorator}\n{completed}\n{code_after}")
 
                 # Reload the module and the functions
                 # todo: reload the script itself could result in ModuleNotFoundError: spec not found for the module '__main__'.
                 #       Trying an dirty way but may need to explore best-practice later.
                 try:
```

### Comparing `capabilities-0.3.0/capabilities/example.py` & `capabilities-0.3.1/capabilities/example.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,16 @@
     class SupportedBulletPoint(BaseModel):
         """
         A class representing a supported bullet point in a document summary.
         A supported bullet point has a bullet point summarizing a passage from the text,
         as well as the supporting text itself, which is a passage of text extracted verbatim from the document.
         """
 
-        bullet_point: str
-        supporting_text: str
+        bullet_point: str # claim
+        supporting_text: str # verbatim passage fom the original document
 
     class DocumentSummary(BaseModel):
         """
         A class representing a summary of a document, consisting of a list of supported bullet points.
         """
 
         supportedBulletPoints: List[SupportedBulletPoint]
@@ -57,17 +57,16 @@
 
     for x in document_summary.supportedBulletPoints:
         print(f"claim: {x.bullet_point}")
         print(f'    support: """{x.supporting_text}"""\n')
 
 
 def example_document_qa():
-    c = Capability("blazon/document_qa")
     question = "Who formed the Carborundum Company?"
-    answer = c(EXAMPLE_PASSAGE, question)
+    answer = Capability("blazon/document_qa")(EXAMPLE_PASSAGE, question)
     print("Result: ", answer)
     print(
         "Formatted result: ",
         "- " + "\n- ".join(bp["bullet_point"] for bp in answer["answer"]["claims"]),
     )
 
 
@@ -83,29 +82,29 @@
 
     class ParsedTable(BaseModel):
         rows: List[ParsedRow]
 
     instructions: str = """\
     Given the following `unstructured_table` ASCII representation of a table, parse it into a list of rows where each row is a list of cells, consisting of the contents of each cell of the `unstructured_table` with all trailing and leading whitespace stripped."""
 
-    c = Capability("blazon/structured")
+    from capabilities import Capability
 
     unstructured_table = """\
 |mathqa        |      0|acc     |  0.2500|_  | 0.0435|
 |              |       |acc_norm|  0.2300|_  | 0.0423|
 |lambada_openai|      0|ppl     |145.0963|_  |53.1010|
 |              |       |acc     |  0.2400|_  | 0.0429|
 |boolq         |      1|acc     |  0.6000|_  | 0.0492|
 |hellaswag     |      0|acc     |  0.3000|_  | 0.0461||
               |       |acc_norm|  0.3600|_  | 0.0482|
 |triviaqa      |      1|acc     |  0.0000|_  | 0.0000|
 |winogrande    |      0|acc     |  0.4000|_  | 0.0492|
 |race          |      1|acc     |  0.2900|_  | 0.0456|"""
 
-    parsed_table = c(
+    parsed_table = Capability("blazon/structured")(
         UnstructuredTable,
         ParsedTable,
         instructions,
         UnstructuredTable(unstructured_table=unstructured_table),
     )
 
     for row in parsed_table.rows:
```

### Comparing `capabilities-0.3.0/capabilities/search/hf.py` & `capabilities-0.3.1/capabilities/search/hf.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.0/capabilities/search/loader.py` & `capabilities-0.3.1/capabilities/search/loader.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,25 +9,25 @@
 from dataclasses import dataclass
 from capabilities.search.util import digest
 
 
 from typing import Hashable, Optional, Union
 
 from .types import TextItem
+import mimetypes
 
 try:
     from pdfminer.high_level import extract_text
-    import magic
     from bs4 import BeautifulSoup
 except ImportError:
     raise ImportError(
         "To use search capabilities, you need to install additional dependencies. "
         "You can do this by running\n"
         'pip install "capabilities[search]"\n'
-    ) from None
+    )
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
 class Document(TextItem):
     text: str
@@ -62,16 +62,24 @@
         byte_content = response.read()
     elif os.path.isfile(location):
         with open(location, "rb") as f:
             byte_content = f.read()
     else:
         raise ValueError(f"{location} is neither a local file nor a valid url")
 
-    mime = magic.Magic(mime=True)
-    filetype = mime.from_buffer(byte_content)
+    try:
+        import magic
+        mime = magic.Magic(mime=True)
+        filetype = mime.from_buffer(byte_content)
+    except ImportError:
+        if os.path.isfile(location):
+            mime, enc = mimetypes.guess_type(str(location))
+            filetype = mime or ""
+        else:
+            raise ImportError('Please install https://pypi.org/project/python-magic/')
 
     if "application/pdf" in filetype:
         text = extract_text(io.BytesIO(byte_content))
     elif "html" in filetype:
         soup = BeautifulSoup(byte_content.decode(), "lxml")
         text = soup.get_text()
     else:
```

### Comparing `capabilities-0.3.0/capabilities/search/nomic_index.py` & `capabilities-0.3.1/capabilities/search/nomic_index.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.0/capabilities/search/oai.py` & `capabilities-0.3.1/capabilities/search/oai.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.0/capabilities/search/search_index.py` & `capabilities-0.3.1/capabilities/search/search_index.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.0/capabilities/search/simple_vector_index.py` & `capabilities-0.3.1/capabilities/search/simple_vector_index.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.0/capabilities/search/types.py` & `capabilities-0.3.1/capabilities/search/types.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.0/capabilities/search/util.py` & `capabilities-0.3.1/capabilities/search/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,19 +7,23 @@
 from typing import (
     Any,
     Callable,
     Iterable,
     Optional,
     Sequence,
     Tuple,
-    TypeAlias,
     Union,
     overload,
     TypeVar,
 )
+try:
+    from typing import TypeAlias
+except:
+    from typing_extensions import TypeAlias
+    
 from hashlib import blake2b
 from diskcache import Cache
 
 K = TypeVar("K")
 T = TypeVar("T")
 U = TypeVar("U")
 V = TypeVar("V")
```

### Comparing `capabilities-0.3.0/capabilities/util/config.py` & `capabilities-0.3.1/capabilities/util/config.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.0/capabilities/util/misc.py` & `capabilities-0.3.1/capabilities/util/misc.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.0/examples/cheese.py` & `capabilities-0.3.1/examples/cheese.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.0/examples/leansearch.py` & `capabilities-0.3.1/examples/leansearch.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.0/examples/tesla10k.py` & `capabilities-0.3.1/examples/tesla10k.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.0/examples/data/apple10k.pdf` & `capabilities-0.3.1/examples/data/apple10k.pdf`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.0/examples/data/sample.md` & `capabilities-0.3.1/examples/data/sample.md`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.0/examples/data/sample.pdf` & `capabilities-0.3.1/examples/data/sample.pdf`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.0/examples/data/tesla10k.txt` & `capabilities-0.3.1/examples/data/tesla10k.txt`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.0/tests/test_dec.py` & `capabilities-0.3.1/tests/test_dec.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.0/tests/test_document_loader.py` & `capabilities-0.3.1/tests/test_document_loader.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.0/tests/test_search.py` & `capabilities-0.3.1/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.0/tests/test_search_util.py` & `capabilities-0.3.1/tests/test_search_util.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.0/tests/test_tutorial1.py` & `capabilities-0.3.1/tests/test_tutorial1.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.0/tests/test_vector_idx.py` & `capabilities-0.3.1/tests/test_vector_idx.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.0/tests/snapshots/test_search/test_search_e2e/NomicIndex-openai/r0.txt` & `capabilities-0.3.1/tests/snapshots/test_search/test_search_e2e/NomicIndex-openai/r0.txt`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.0/tests/snapshots/test_search/test_search_e2e/NomicIndex-sentence-transformersall-MiniLM-L6-v2/r0.txt` & `capabilities-0.3.1/tests/snapshots/test_search/test_search_e2e/NomicIndex-sentence-transformersall-MiniLM-L6-v2/r0.txt`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.0/tests/snapshots/test_search/test_search_e2e/SearchIndex-openai/r0.txt` & `capabilities-0.3.1/tests/snapshots/test_search/test_search_e2e/SearchIndex-openai/r0.txt`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.0/tests/snapshots/test_search/test_search_e2e/SearchIndex-sentence-transformersall-MiniLM-L6-v2/r0.txt` & `capabilities-0.3.1/tests/snapshots/test_search/test_search_e2e/SearchIndex-sentence-transformersall-MiniLM-L6-v2/r0.txt`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.0/.gitignore` & `capabilities-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.0/LICENSE` & `capabilities-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.0/pyproject.toml` & `capabilities-0.3.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -27,14 +27,15 @@
   "typer",
   "openai",
   "backoff",
   "diskcache",
   "google",
   "openai",
   "textual",
+  "numpy",
 ]
 
 [project.scripts]
 capabilities = "capabilities.cli:app"
 
 [tool.hatch.version]
 path = "capabilities/__about__.py"
@@ -68,15 +69,16 @@
   "requests",
   "dacite",
   "aiohttp",
   "tiktoken",
   "pyllamacpp",
   "python-magic",
   "bs4",
-  "google"
+  "google",
+  "typing_extensions",
 ]
 [tool.hatch.envs.default.scripts]
 test = "pytest {args:tests}"
 test-cov = "coverage run -m pytest {args:tests}"
 cov-report = [
   "- coverage combine",
   "coverage report",
```

### Comparing `capabilities-0.3.0/PKG-INFO` & `capabilities-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capabilities
-Version: 0.3.0
+Version: 0.3.1
 Summary: Build trusted, faster, and more powerful applications with the Blazon Capabilities API.
 Author-email: Blazon AI <support@blazon.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -210,14 +210,15 @@
 Requires-Dist: asyncio
 Requires-Dist: backoff
 Requires-Dist: blobfile
 Requires-Dist: dacite
 Requires-Dist: diskcache
 Requires-Dist: fire
 Requires-Dist: google
+Requires-Dist: numpy
 Requires-Dist: openai
 Requires-Dist: pdfminer-six
 Requires-Dist: pydantic
 Requires-Dist: pydantic[dotenv]
 Requires-Dist: requests
 Requires-Dist: rich
 Requires-Dist: textual
```

