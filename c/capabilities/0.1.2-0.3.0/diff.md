# Comparing `tmp/capabilities-0.1.2.tar.gz` & `tmp/capabilities-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "capabilities-0.1.2.tar", last modified: Fri May 12 04:31:03 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `capabilities-0.1.2.tar` & `capabilities-0.3.0.tar`

### file list

```diff
@@ -1,30 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 04:31:03.283925 capabilities-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-12 04:30:41.000000 capabilities-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13514 2023-05-12 04:31:03.283925 capabilities-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-12 04:30:41.000000 capabilities-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 04:31:03.279925 capabilities-0.1.2/capabilities/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-12 04:30:41.000000 capabilities-0.1.2/capabilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-12 04:30:41.000000 capabilities-0.1.2/capabilities/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    15365 2023-05-12 04:30:41.000000 capabilities-0.1.2/capabilities/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-05-12 04:30:41.000000 capabilities-0.1.2/capabilities/dec.py
--rw-r--r--   0 runner    (1001) docker     (123)    12771 2023-05-12 04:30:41.000000 capabilities-0.1.2/capabilities/example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 04:31:03.283925 capabilities-0.1.2/capabilities/search/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-12 04:30:41.000000 capabilities-0.1.2/capabilities/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-05-12 04:30:41.000000 capabilities-0.1.2/capabilities/search/hf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-12 04:30:41.000000 capabilities-0.1.2/capabilities/search/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-05-12 04:30:41.000000 capabilities-0.1.2/capabilities/search/nomic_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-05-12 04:30:41.000000 capabilities-0.1.2/capabilities/search/oai.py
--rw-r--r--   0 runner    (1001) docker     (123)    12083 2023-05-12 04:30:41.000000 capabilities-0.1.2/capabilities/search/search_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-12 04:30:41.000000 capabilities-0.1.2/capabilities/search/simple_vector_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-05-12 04:30:41.000000 capabilities-0.1.2/capabilities/search/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-05-12 04:30:41.000000 capabilities-0.1.2/capabilities/search/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-05-12 04:30:41.000000 capabilities-0.1.2/capabilities/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 04:31:03.279925 capabilities-0.1.2/capabilities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13514 2023-05-12 04:31:03.000000 capabilities-0.1.2/capabilities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-12 04:31:03.000000 capabilities-0.1.2/capabilities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 04:31:03.000000 capabilities-0.1.2/capabilities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-12 04:31:03.000000 capabilities-0.1.2/capabilities.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-12 04:31:03.000000 capabilities-0.1.2/capabilities.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-12 04:30:41.000000 capabilities-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 04:31:03.283925 capabilities-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-12 04:30:41.000000 capabilities-0.1.2/setup.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 capabilities-0.3.0/setup.py
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 capabilities-0.3.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 capabilities-0.3.0/capabilities/__about__.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 capabilities-0.3.0/capabilities/__init__.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 capabilities-0.3.0/capabilities/__main__.py
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 capabilities-0.3.0/capabilities/cli.py
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 capabilities-0.3.0/capabilities/config.py
+-rw-r--r--   0        0        0    16630 2020-02-02 00:00:00.000000 capabilities-0.3.0/capabilities/core.py
+-rw-r--r--   0        0        0     6785 2020-02-02 00:00:00.000000 capabilities-0.3.0/capabilities/dec.py
+-rw-r--r--   0        0        0    15089 2020-02-02 00:00:00.000000 capabilities-0.3.0/capabilities/example.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 capabilities-0.3.0/capabilities/search/__init__.py
+-rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 capabilities-0.3.0/capabilities/search/hf.py
+-rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 capabilities-0.3.0/capabilities/search/loader.py
+-rw-r--r--   0        0        0     6082 2020-02-02 00:00:00.000000 capabilities-0.3.0/capabilities/search/nomic_index.py
+-rw-r--r--   0        0        0     6286 2020-02-02 00:00:00.000000 capabilities-0.3.0/capabilities/search/oai.py
+-rw-r--r--   0        0        0    12426 2020-02-02 00:00:00.000000 capabilities-0.3.0/capabilities/search/search_index.py
+-rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 capabilities-0.3.0/capabilities/search/simple_vector_index.py
+-rw-r--r--   0        0        0     7076 2020-02-02 00:00:00.000000 capabilities-0.3.0/capabilities/search/types.py
+-rw-r--r--   0        0        0     5233 2020-02-02 00:00:00.000000 capabilities-0.3.0/capabilities/search/util.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 capabilities-0.3.0/capabilities/util/__init__.py
+-rw-r--r--   0        0        0     8767 2020-02-02 00:00:00.000000 capabilities-0.3.0/capabilities/util/config.py
+-rw-r--r--   0        0        0     6628 2020-02-02 00:00:00.000000 capabilities-0.3.0/capabilities/util/misc.py
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 capabilities-0.3.0/examples/cheese.py
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 capabilities-0.3.0/examples/leansearch.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 capabilities-0.3.0/examples/readme.txt
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 capabilities-0.3.0/examples/tesla10k.py
+-rw-r--r--   0        0        0   840980 2020-02-02 00:00:00.000000 capabilities-0.3.0/examples/data/apple10k.pdf
+-rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 capabilities-0.3.0/examples/data/sample.md
+-rw-r--r--   0        0        0     7945 2020-02-02 00:00:00.000000 capabilities-0.3.0/examples/data/sample.pdf
+-rw-r--r--   0        0        0   157134 2020-02-02 00:00:00.000000 capabilities-0.3.0/examples/data/tesla10k.txt
+-rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 capabilities-0.3.0/tests/test_dec.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 capabilities-0.3.0/tests/test_document_loader.py
+-rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 capabilities-0.3.0/tests/test_search.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 capabilities-0.3.0/tests/test_search_util.py
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 capabilities-0.3.0/tests/test_tutorial1.py
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 capabilities-0.3.0/tests/test_vector_idx.py
+-rw-r--r--   0        0        0   353564 2020-02-02 00:00:00.000000 capabilities-0.3.0/tests/snapshots/test_search/test_search_e2e/NomicIndex-openai/r0.txt
+-rw-r--r--   0        0        0   353563 2020-02-02 00:00:00.000000 capabilities-0.3.0/tests/snapshots/test_search/test_search_e2e/NomicIndex-sentence-transformersall-MiniLM-L6-v2/r0.txt
+-rw-r--r--   0        0        0   353563 2020-02-02 00:00:00.000000 capabilities-0.3.0/tests/snapshots/test_search/test_search_e2e/SearchIndex-openai/r0.txt
+-rw-r--r--   0        0        0   353565 2020-02-02 00:00:00.000000 capabilities-0.3.0/tests/snapshots/test_search/test_search_e2e/SearchIndex-sentence-transformersall-MiniLM-L6-v2/r0.txt
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 capabilities-0.3.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 capabilities-0.3.0/LICENSE
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 capabilities-0.3.0/README.md
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 capabilities-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    14266 2020-02-02 00:00:00.000000 capabilities-0.3.0/PKG-INFO
```

### Comparing `capabilities-0.1.2/LICENSE` & `capabilities-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `capabilities-0.1.2/PKG-INFO` & `capabilities-0.3.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capabilities
-Version: 0.1.2
+Version: 0.3.0
 Summary: Build trusted, faster, and more powerful applications with the Blazon Capabilities API.
 Author-email: Blazon AI <support@blazon.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -200,25 +200,50 @@
                http://www.apache.org/licenses/LICENSE-2.0
         
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
-        
+License-File: LICENSE
 Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: search
+Requires-Dist: aiohttp
+Requires-Dist: asyncio
+Requires-Dist: backoff
+Requires-Dist: blobfile
+Requires-Dist: dacite
+Requires-Dist: diskcache
+Requires-Dist: fire
+Requires-Dist: google
+Requires-Dist: openai
+Requires-Dist: pdfminer-six
+Requires-Dist: pydantic
+Requires-Dist: pydantic[dotenv]
+Requires-Dist: requests
+Requires-Dist: rich
+Requires-Dist: textual
+Requires-Dist: tiktoken
+Requires-Dist: typer
+Provides-Extra: agent
+Requires-Dist: google; extra == 'agent'
 Provides-Extra: nomic
+Requires-Dist: nomic; extra == 'nomic'
+Provides-Extra: search
+Requires-Dist: bs4; extra == 'search'
+Requires-Dist: pyllamacpp; extra == 'search'
+Requires-Dist: python-magic; extra == 'search'
 Provides-Extra: sentence-transformers
-License-File: LICENSE
+Requires-Dist: sentence-transformers; extra == 'sentence-transformers'
+Description-Content-Type: text/markdown
 
 # capabilities
 
 Blazon Capabilities SDK
 
+Read our [Getting Started Guide](https://docs.blazon.ai).
+
 # Install and run example
 
 ```bash
 pip install -e . # installs `capabilities`
 python -m capabilities.example example_structured
 ```
```

### Comparing `capabilities-0.1.2/capabilities/core.py` & `capabilities-0.3.0/capabilities/core.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,29 +5,96 @@
 from dataclasses import dataclass, field, is_dataclass
 from typing import Dict, Any, List, Type, TypeAlias, TypeVar, Union, Literal
 from typing import Optional
 import requests
 import aiohttp
 import asyncio
 import time
-from capabilities.config import CONFIG
+
+import aiohttp
+import dacite
+import requests
+from dataclasses import dataclass, field, is_dataclass, asdict
 from pydantic import BaseModel
 from pydantic.fields import ModelField
 from pydantic.main import ModelMetaclass
 import logging
 
 logger = logging.getLogger("capabilities")
+from typing import Any, Callable, Dict, List, Literal, Optional, Union
+from capabilities.config import CONFIG
+
+_CAPABILITIES = {}
 
 
 @dataclass
 class CapabilityBase:
     ...
 
 
 @dataclass
+class Capability(CapabilityBase):
+    uri: str
+    _capability: Optional[CapabilityBase] = None
+
+    def __call__(self, *args, **kwargs):
+        return self._capability(*args, **kwargs)
+
+    async def run_async(self, *args, **kwargs):
+        return await self._capability.run_async(*args, **kwargs)
+
+    def __post_init__(self):
+        try:
+            self._capability = _CAPABILITIES[self.uri]
+        except KeyError as e:
+            print(
+                f"KeyError={e}\nCapability lookup failed for uri={self.uri}.\nValid URIs are:"
+            )
+            for k in _CAPABILITIES.keys():
+                print(f"  {k}")
+
+
+from functools import wraps
+import inspect
+
+
+def register(uri: str) -> Callable:
+    """
+    A decorator that registers an instance of the decorated class
+    under the given URI in _CAPABILITIES.
+
+    Args:
+        uri (str): The URI to register the instance of the decorated class.
+
+    Returns:
+        Callable: The decorator function
+        that receives the decorated class and returns it unmodified.
+    """
+
+    def wrapper(cls):
+        async def async_run(sync_func, *args, **kwargs):
+            loop = asyncio.get_event_loop()
+            return await loop.run_in_executor(None, sync_func, *args, **kwargs)
+
+        _CAPABILITIES[uri] = cls() if inspect.isclass(cls) else cls
+        call_method = getattr(cls, "__call__")
+        if not hasattr(cls, "run_async"):
+
+            @wraps(call_method)
+            async def run_async(*args, **kwargs):
+                return await async_run(call_method, *args, **kwargs)
+
+            cls.run_async = run_async
+        return cls
+
+    return wrapper
+
+
+@register("blazon/document_qa")
+@dataclass
 class DocumentQA(CapabilityBase):
     """
     DocumentQA capability that sends the given query to DocumentQA service for answering based on the provided document.
 
     Attributes:
         None
 
@@ -59,18 +126,18 @@
         print(
             f"[DocumentQA] running query against document with {len(document)} characters"
         )
         patience = 8
         count = 0
         while count < patience:
             try:
-                url = "https://api.blazon.ai/blazon/documentqa"
+                url = f"{CONFIG.api_url}/blazon/documentqa"
                 headers = {
                     "Content-type": "application/json",
-                    "api-key": CONFIG.api_key,
+                    "api-key": CONFIG.get_api_key(),
                 }
                 payload = {
                     "document": document,
                     "query": query,
                 }
                 resp = requests.post(url=url, headers=headers, json=payload)
                 return resp.json()
@@ -85,25 +152,25 @@
         print(
             f"[DocumentQA] running query against document with {len(document)} characters"
         )
         patience = 8
         count = 0
         while count < patience:
             try:
-                url = "https://api.blazon.ai/blazon/documentqa"
+                url = f"{CONFIG.api_url}/blazon/documentqa"
                 if session is None:
                     async with aiohttp.ClientSession(
                         connector=aiohttp.TCPConnector(ssl=False)
                     ) as session:
                         return await self.run_async(
                             document=document, query=query, session=session
                         )
                 headers = {
                     "Content-type": "application/json",
-                    "api-key": CONFIG.api_key,
+                    "api-key": CONFIG.get_api_key(),
                 }
                 payload = {
                     "document": document,
                     "query": query,
                 }
                 async with session.post(url, headers=headers, json=payload) as resp:
                     response = await resp.json()
@@ -117,14 +184,15 @@
                 sleep_duration = 2.0**count
                 print(f"retrying after sleeping for {sleep_duration:.2f}")
                 count += 1
                 time.sleep(sleep_duration)
         raise Exception("[DocumentQA] failed after hitting max retries")
 
 
+@register("blazon/summarize")
 @dataclass
 class Summarize(CapabilityBase):
     """
     Class for summarizing text using an API call to https://api.blazon.ai/blazon/summarize.
 
     Args:
         CapabilityBase (class): Base class for all capabilities.
@@ -149,18 +217,18 @@
     """
 
     def __call__(self, document: str):
         patience = 8
         count = 0
         while count < patience:
             try:
-                url = "https://api.blazon.ai/blazon/summarize"
+                url = f"{CONFIG.api_url}/blazon/summarize"
                 headers = {
                     "Content-type": "application/json",
-                    "api-key": CONFIG.api_key,
+                    "api-key": CONFIG.get_api_key(),
                 }
                 payload = {
                     "document": document,
                 }
                 print(
                     f"[Summarize] running query against document with {len(document)} characters"
                 )
@@ -174,23 +242,23 @@
         raise Exception("[Summarize] failed after hitting max retries")
 
     async def run_async(self, document: str, session=None):
         patience = 8
         count = 0
         while count < patience:
             try:
-                url = "https://api.blazon.ai/blazon/summarize"
+                url = f"{CONFIG.api_url}/blazon/summarize"
                 if session is None:
                     async with aiohttp.ClientSession(
                         connector=aiohttp.TCPConnector(ssl=False)
                     ) as session:
                         return await self.run_async(document=document, session=session)
                 headers = {
                     "Content-type": "application/json",
-                    "api-key": CONFIG.api_key,
+                    "api-key": CONFIG.get_api_key(),
                 }
                 payload = {
                     "document": document,
                 }
                 print(
                     f"[Summarize] running query against document with {len(document)} characters"
                 )
@@ -230,15 +298,15 @@
             raise TypeError(
                 f"can't deduce list type arg for {m} at {p}, please provide a type annotation to list.",
                 path,
             )
         t = flatten_model(args[0])
         return [t]
     elif isinstance(m, ModelMetaclass):
-        fields: dict[str, ModelField] = m.__fields__ # type: ignore
+        fields: dict[str, ModelField] = m.__fields__  # type: ignore
         return {
             k: flatten_model(f.annotation, path=path + [k]) for k, f in fields.items()
         }
     elif is_dataclass(m):
         return {
             f.name: flatten_model(f.type, path=path + [f.name])
             for f in dataclasses.fields(m)
@@ -282,30 +350,39 @@
         return t.parse_obj(d)
     elif is_dataclass(t):
         assert isinstance(d, dict)
         return dacite.from_dict(t, d)  # type: ignore
     elif t == list or typing.get_origin(t) == list:
         assert isinstance(d, list)
         args = typing.get_args(t)
-        if len(args)!= 1:
-            return d # type: ignore
+        if len(args) != 1:
+            return d  # type: ignore
         (arg,) = args
         return [of_dict(arg, o) for o in d]  # type: ignore
     elif t == dict:
         (kt, vt) = typing.get_args(t)
         assert isinstance(d, dict)
         assert kt in [str, int]
         return {of_dict(kt, k): of_dict(vt, v) for k, v in d.items()}  # type: ignore
     elif t in [str, int, float, bool]:
         assert isinstance(d, t)
         return d
     else:
         raise TypeError(f"unsupported datatype={t}")
 
 
+def unflatten_model(output_spec, result):
+    return (
+        output_spec.parse_obj(result)
+        if isinstance(output_spec, ModelMetaclass)
+        else dacite.from_dict(output_spec, result)
+    )
+
+
+@register("blazon/structured")
 @dataclass
 class Structured(CapabilityBase):
     """
     `Structured` class allows making requests to the multi API for structured tasks. The class extends CapabilityBase which provides required functionality to interact with multi API. Structured tasks are tasks with specific input and output specs with a natural language instruction.
 
     Attributes:
         headers (Dict[Any, Any]): HTTP headers to use in requests. It includes the Content-type and API Key parameters.
@@ -313,21 +390,19 @@
 
     Methods:
         __call__(self, input_spec: ModelMetaclass, output_spec: ModelMetaclass, instructions: str, input: BaseModel) -> Union[output_spec, BaseModel]: Calls the API by sending a payload within a request object. Returns output_spec object if output_spec is ModelMetaclass or if it is an instance of a BaseModel.
 
         async run_async(self, input_spec: ModelMetaclass, output_spec: ModelMetaclass, instructions: str, input: BaseModel, session=None) -> Union[output_spec, BaseModel]: Calls the API asynchronously. Returns output_spec object if output_spec is ModelMetaclass or if it is an instance of a BaseModel.
     """
 
-    headers: dict = field(
-        default_factory=lambda: {
-            "Content-type": "application/json",
-            "api-key": CONFIG.api_key,
-        }
-    )
-    url: str = "https://api.blazon.ai/blazon/structured"
+    url: str = f"{CONFIG.api_url}/blazon/structured"
+
+    @property
+    def headers(self):
+        return {"Content-type": "application/json", "api-key": CONFIG.get_api_key()}
 
     def __call__(
         self,
         input_spec: ModelMetaclass,
         output_spec: ModelMetaclass,
         instructions: str,
         input: Any,
@@ -370,37 +445,7 @@
                     return of_dict(output_spec, result)
         else:
             async with session.post(
                 self.url, headers=self.headers, json=payload
             ) as resp:
                 result = (await resp.json())["output"]
                 return of_dict(output_spec, result)
-
-
-_CAPABILITIES = {
-    "multi/structured": Structured(),
-    "multi/document_qa": DocumentQA(),
-    "multi/summarize": Summarize(),
-    "blazon/structured": Structured(),
-    "blazon/document_qa": DocumentQA(),
-    "blazon/summarize": Summarize(),
-}
-
-
-@dataclass
-class Capability(CapabilityBase):
-    uri: str
-    _capability: Optional[CapabilityBase] = None
-
-    def __call__(self, *args, **kwargs):
-        return self._capability(*args, **kwargs)
-
-    async def run_async(self, *args, **kwargs):
-        return await self._capability.run_async(*args, **kwargs)
-
-    def __post_init__(self):
-        try:
-            self._capability = _CAPABILITIES[self.uri]
-        except KeyError as e:
-            print(f"Capability lookup failed for uri={self.uri}.\nValid URIs are:")
-            for k in _CAPABILITIES.keys():
-                print(f"  {k}")
```

### Comparing `capabilities-0.1.2/capabilities/example.py` & `capabilities-0.3.0/capabilities/example.py`

 * *Files 13% similar despite different names*

```diff
@@ -56,26 +56,14 @@
     )
 
     for x in document_summary.supportedBulletPoints:
         print(f"claim: {x.bullet_point}")
         print(f'    support: """{x.supporting_text}"""\n')
 
 
-# def example_document_qa():
-#     c = Capability("blazon/document_qa")
-#     question = "Who formed the Carborundum Company?"
-#     answer = c(EXAMPLE_PASSAGE, question)
-#     print(dict(question=question))
-#     print(answer)
-#     question = "What colors were emitted by the first LED crystal?"
-#     answer = c(EXAMPLE_PASSAGE, question)
-#     print(dict(question=question))
-#     print(answer)
-
-
 def example_document_qa():
     c = Capability("blazon/document_qa")
     question = "Who formed the Carborundum Company?"
     answer = c(EXAMPLE_PASSAGE, question)
     print("Result: ", answer)
     print(
         "Formatted result: ",
@@ -160,14 +148,15 @@
 def structured_chain_of_thought():
     class Input(BaseModel):
         input: str
 
     class ChainOfThought(BaseModel):
         thoughts: List[List[str]]
         conclusion: str
+
         meta_conclusion: str
 
     class CombinedInputOutput(BaseModel):
         input: Input
         cot: ChainOfThought
 
     class Output(BaseModel):
@@ -223,17 +212,15 @@
         text="Understand: I'll slip quietly away through twilit meadows with only this one dream - you come too."
     )
 
     # provide some instructions
     instructions = "Given the input `text`, produce a `french_translation` which translates the `text` into French. Also produce a word-level translation called `word_translations`, which is a list of (english word, french transliteration) pairs."
 
     # print the task to console
-    result = Capability("blazon/structured")(
-        InputText, TranslationOutput, instructions, inp
-    )
+    result = Capability("blazon/structured")(InputText, TranslationOutput, instructions, inp)
     import json
 
     print(json.dumps(result.dict(), indent=2))
 
 
 def example_summarize():
     print(Capability("blazon/summarize")(EXAMPLE_PASSAGE))
@@ -312,12 +299,68 @@
         BulletPoints,
         Summary,
         "Combine the `bullet_points` into a paragraph-length summary. Use only information which is in the `bullet_points`. Ensure the final `summary` is crisp, professional, and flows well.",
         BulletPoints(bullet_points=bullet_points),
     ).summary
 
 
+def synth_app(instructions: str):
+    class Instruction(BaseModel):
+        instruction: str
+
+    class PartialWebsiteElement(BaseModel):
+        html_tag: str
+        parameters: List[str]
+        instruction: str
+
+    class Plan(BaseModel):
+        top_level_description: str  # model-generated description of what the end result should look like
+        partial_elements: List[PartialWebsiteElement]
+
+    instruction = """\
+    Given the user `instruction` for a website to build in HTML, write a plan with a paragraph-length `top_level_description` for the overall structure and look and feel of the website, and a comprehensive list of `partial_elements`, each of which contains an `html_tag` for that element, `parameters` to be passed as arguments to the tag, and an `instruction` specifying that element of the final HTML document. Phrase the `instruction` as an instruction to a software engineer who will fully implement the element. The `partial_elements` should include headers, footers, and should use inline tailwind CSS styling. Use Javascript as necessary. Do not create SVG elements.
+    """
+
+    input = Instruction(instruction=instructions)
+    output = Capability("blazon/structured")(Instruction, Plan, instruction, input)
+
+    print("top-level: ", output.top_level_description)
+    for pe in output.partial_elements:
+        print(pe)
+
+    from concurrent import futures
+
+    def generate_html_element(p1: Plan, p2: PartialWebsiteElement):
+        instruction = "Given the `plan`, implement the `partial_website_element` as a `complete_html_element`. Implement the `instruction`. Fully implement the `instruction` and do not leave placeholders or comments. Do not repeat the `instruction`. Fill in all missing content and add code for e.g. Javascript, connecting to external APIs, and databases as necessary. Link to nonexistent website, social media profiles, and make up contact information and legal disclaimers as needed."
+
+        class Plan2(BaseModel):
+            plan: Plan
+            partial_website_element: PartialWebsiteElement
+
+        class HTMLElement(BaseModel):
+            html_element: str
+
+        return Capability("blazon/structured")(
+            Plan2, HTMLElement, instruction, Plan2(plan=p1, partial_website_element=p2)
+        )
+
+    with futures.ThreadPoolExecutor(8) as pool:
+        html_elements = pool.map(
+            lambda p: generate_html_element(output, p), output.partial_elements
+        )
+
+    final_document = "\n".join(x.html_element for x in html_elements)
+
+    with open("test2.html", "w") as f:
+        f.write(final_document)
+
+    return final_document
+
+
+# from multisearch.trace_flow import if_json_spec_async
+# synthesize a plan / chain of thought using GPT4
+
 # example usage: python -m capabilities.example example_translation
 if __name__ == "__main__":
     import sys
 
     fire.Fire(component=locals()[sys.argv[1]], command=sys.argv[2:])
```

### Comparing `capabilities-0.1.2/capabilities/search/hf.py` & `capabilities-0.3.0/capabilities/search/hf.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
 from typing import Sequence
 from .types import EmbeddingModel
 from hashlib import blake2b
 from .util import batched, cache
+from tqdm import tqdm
 
 try:
     from sentence_transformers import SentenceTransformer
 except ModuleNotFoundError:
     raise ModuleNotFoundError(
         "In order to use sentence-transformer modules, please run `pip install sentence-transformers`"
     )
@@ -52,15 +53,15 @@
 
     def encode_no_cache(self, texts: list[str], show_progress_bar=True):
         return self.model.encode(list(texts), show_progress_bar=show_progress_bar)
 
     def encode(self, sentences: list[str], show_progress_bar=True):
         h = blake2b()
         h.update(self.name.encode())
-        for sentence in sentences:
+        for sentence in tqdm(sentences):
             h.update(sentence.encode())
         digest = h.hexdigest()
         result = cache.get(digest)
         if result is not None:
             logger.debug(f"Using cached encoding")
             return result
         result = self.encode_no_cache(sentences, show_progress_bar=show_progress_bar)
```

### Comparing `capabilities-0.1.2/capabilities/search/loader.py` & `capabilities-0.3.0/capabilities/search/loader.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,32 +3,41 @@
 import io
 from pathlib import Path
 
 from urllib.parse import urlparse
 from urllib import request
 
 from dataclasses import dataclass
-from pdfminer.high_level import extract_text
 from capabilities.search.util import digest
-import magic
-from bs4 import BeautifulSoup
+
 
 from typing import Hashable, Optional, Union
 
 from .types import TextItem
 
+try:
+    from pdfminer.high_level import extract_text
+    import magic
+    from bs4 import BeautifulSoup
+except ImportError:
+    raise ImportError(
+        "To use search capabilities, you need to install additional dependencies. "
+        "You can do this by running\n"
+        'pip install "capabilities[search]"\n'
+    ) from None
+
 logger = logging.getLogger(__name__)
 
 
 @dataclass
 class Document(TextItem):
     text: str
     doc_id: str
-    location : str
-    digest : str
+    location: str
+    digest: str
 
     @property
     def id(self):
         return str(self.doc_id)
 
     def get_text(self) -> str:
         return self.text
@@ -70,8 +79,8 @@
             text = byte_content.decode()
         except UnicodeDecodeError:
             logger.exception(
                 f"{location} does not appear to be a pdf document, an html document, or contain valid text."
             )
             raise
 
-    return Document(text=text, doc_id=doc_id, location=location, digest = digest(text))
+    return Document(text=text, doc_id=doc_id, location=location, digest=digest(text))
```

### Comparing `capabilities-0.1.2/capabilities/search/nomic_index.py` & `capabilities-0.3.0/capabilities/search/nomic_index.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,33 +88,29 @@
     @property
     def index(self):
         if len(self.chunks) < 20:
             raise RuntimeError(
                 "Nomic does not yet have enough data to index. Please make sure there are at least 20 datapoints."
             )
         if len(self.project.indices) == 0:
-            return self.project.create_index(
-                name="main-index", colorable_fields=["item_id"]
-            )
+            return self.project.create_index(name="main-index", colorable_fields=["item_id"])
         else:
             return self.project.indices[0].projections[0]  # idk
 
     def update(self, items: Iterable[T]):
         items = list(items)
         for item in items:
             if item.id in self.items:
                 raise RuntimeError(f"Item {item.id} already exists in the index.")
             self.items[item.id] = item
         if self.embedding_model is not None:
             chunks = list(get_chunks(items, self.embedding_model))
             for chunk in chunks:
                 if chunk.unique_id in self.chunks:
-                    raise RuntimeError(
-                        f"Chunk {chunk.unique_id} already exists in the index."
-                    )
+                    raise RuntimeError(f"Chunk {chunk.unique_id} already exists in the index.")
                 self.chunks[chunk.unique_id] = chunk
             texts = [chunk.text for chunk in chunks]
             embeddings = self.embedding_model.encode(texts)
             assert isinstance(embeddings, np.ndarray)
             assert len(embeddings.shape) == 2
             self.project.add_embeddings(
                 data=[c.dict() for c in chunks],
@@ -148,13 +144,11 @@
                         substring_range=chunk.substring_range,
                     )
 
                 items = [mk(id, score) for id, score in zip(ids[0], distances[0])]
                 return items
 
         else:
-            raise NotImplementedError(
-                "search on a text-mode Nomic index is not yet implemented."
-            )
+            raise NotImplementedError("search on a text-mode Nomic index is not yet implemented.")
 
     def __len__(self):
         raise NotImplementedError("todo")
```

### Comparing `capabilities-0.1.2/capabilities/search/oai.py` & `capabilities-0.3.0/capabilities/search/oai.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 """ Open AI API client. """
-
+import time
+import logging
+from capabilities.util import parallel_map
+from tqdm import tqdm
 from datetime import datetime
 import json
 from typing import Literal, Optional, Union
 import numpy as np
 from pydantic import BaseModel, BaseSettings, Field, SecretStr
 import tiktoken
 from .types import EmbeddingModel
@@ -114,15 +117,15 @@
 
 # [todo] throttling, retries
 @cache.memoize()
 def embeddings(params: EmbeddingRequest) -> EmbeddingResponse:
     resp = OpenAISettings().post("/v1/embeddings", json=params.dict(exclude_none=True))  # type: ignore
     j = resp.json()
     if resp.status_code // 100 == 4:
-        raise requests.HTTPError(f"{resp.status_code}: {json.dumps(j, indent=2)}", response = resp)
+        raise requests.HTTPError(f"{resp.status_code}: {json.dumps(j, indent=2)}", response=resp)
     resp.raise_for_status()
     r = EmbeddingResponse.parse_obj(j)
     return r
 
 
 @cache.memoize()
 def chat_completions(params: CompletionRequest) -> CompletionResponse:
@@ -132,27 +135,28 @@
     r = CompletionResponse.parse_obj(j)
     return r
 
 
 class OpenAIEmbeddingModel(EmbeddingModel):
     model_name = "text-embedding-ada-002"
     tokenizer_name = "cl100k_base"
+    chunk_size: int = 511
 
     def __init__(self):
         self.tokenizer = tiktoken.get_encoding(self.tokenizer_name)
 
     def __setstate__(self, state):
         self.__init__()
 
     def __getstate__(self):
         return {}
 
     @property
     def max_tokens_per_item(self) -> int:
-        return 8191
+        return self.chunk_size
 
     @property
     def dim(self) -> int:
         return 1536
 
     def count_tokens(self, text: str):
         num_tokens = len(self.tokenizer.encode(text))
@@ -177,22 +181,32 @@
         return starts, ends
 
     def encode(self, texts: list[str]):
         lengths = [self.count_tokens(text) for text in texts]
         N = self.max_tokens_per_item
         for i, l in enumerate(lengths):
             if l > N:
-                raise ValueError(
-                    f"{i}th text {texts[i]} is too long, please chunk it first"
-                )
+                raise ValueError(f"{i}th text {texts[i]} is too long, please chunk it first")
         batches = argbatch(lengths, N)
         es = []
-        its = track(batches) if len(batches) > 100 else batches
-        for batch in its:
+        # its = track(batches) if len(batches) > 100 else batches
+        its = batches
+
+        def process_batch(batch, texts, embeddings, model_name):
             ts = texts[batch.start : batch.stop]
-            responses = embeddings(EmbeddingRequest(model=self.model_name, input=ts))
+            responses = embeddings(EmbeddingRequest(model=model_name, input=ts))
             new_es = np.array([r.embedding for r in responses.data])
             assert len(new_es) == len(ts)
+            return new_es
+
+        ARGS = [(batch, texts, embeddings, self.model_name) for batch in its]
+        its = parallel_map(
+            lambda x: process_batch(*x), ARGS, parallelism=8, ignore_exceptions=False
+        )
+        if len(batches) > 100:
+            its = track(its, total=len(ARGS), description="Generating embedding(s)...")
+        for new_es in its:
             es.append(new_es)
+
         es = np.concatenate(es, axis=0)
         assert len(es) == len(texts)
         return es
```

### Comparing `capabilities-0.1.2/capabilities/search/search_index.py` & `capabilities-0.3.0/capabilities/search/search_index.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,14 +13,16 @@
     EmbeddingModel,
     TextItem,
     VectorIndex,
     get_text,
 )
 from .util import Bijection, argwindow, unzip
 import numpy as np
+from tqdm import tqdm
+from ..util import parallel_map
 
 T = TypeVar("T", bound=TextItem)
 
 logger = logging.getLogger("capabilities.search")
 
 
 def simple_chunker(
@@ -40,17 +42,15 @@
     text = get_text(item)
     tokens = model.tokenize(text)
     if len(tokens) < N:
         yield Chunk.total(item)
         return
     # [todo] maybe support a model.n_tokens_offset(n_tokens) -> offset method?
     ERROR_MARGIN = 10
-    assert (
-        ERROR_MARGIN < N
-    ), f"max_tokens_per_chunk {N} should be larger than {ERROR_MARGIN}"
+    assert ERROR_MARGIN < N, f"max_tokens_per_chunk {N} should be larger than {ERROR_MARGIN}"
     windows = list(argwindow(len(tokens), N - ERROR_MARGIN, 0.5))
 
     for window_start, window_end in windows:
         chunk_text = model.detokenize(tokens[window_start:window_end])
         pre_chunk_text = model.detokenize(tokens[:window_start])
         offset_start = len(pre_chunk_text)
         offset_end = len(pre_chunk_text) + len(chunk_text)
@@ -70,17 +70,15 @@
 class ChunkMap:
     """Keeps track of the mappings between chunk_ids, ids, indexes."""
 
     def __init__(self):
         self._idx_of_id: Dict[str, dict[Optional[str], int]] = defaultdict(dict)
         self._id_of_idx: Dict[int, str] = {}
         self._chunk_id_of_idx: Dict[int, Optional[str]] = {}
-        self._chunk_range_of_chunk_id: dict[
-            tuple[str, Optional[str]], Optional[range]
-        ] = {}
+        self._chunk_range_of_chunk_id: dict[tuple[str, Optional[str]], Optional[range]] = {}
 
     def __len__(self):
         return len(self._id_of_idx)
 
     def add(self, chunk: Chunk):
         index = len(self)
         idx_of_chunk_id = self._idx_of_id[chunk.item_id]
@@ -119,38 +117,40 @@
 
 
 T = TypeVar("T", bound=TextItem)
 
 
 @dataclass
 class SearchResult(Generic[T]):
-    """Result of calling SearchIndex.search."""
+    """Result of calling SearchIndex.search.
 
-    item: T
-    """ The TextItem that was found.
+    Attributes:
+        item: The TextItem that was found. Note that the item may have been chunked, in which case the chunk_id will
+            be non-None. You can use item.get_text() to get the chunk text.
+        chunk_id: If the original text-item was too long and got chunked, we also pass an identifier for the chunk.
+        score: Value between 0.0 and 1.0 representing the score of the item, higher is closer to the query.
+        substring_range: Optional range specifying the substring range in the original text where the match occurred.
+        id: Property that gets the item_id of the found item.
+    """
 
-    Note that the item may have been chunked, in which case the chunk_id will be non-None.
-    You can use item.get_text() to get the chunk text."""
+    item: T
     chunk_id: Optional[str]
-    """ If the original text-item was too long and got chunked, we also pass an identifier for the chunk. """
     score: float
-    """ Value between 0.0 and 1.0 representing the score of the item, higher is closer to the query. """
-    substring_range: Optional[range] = field(default=None)
+    substring_range: Optional[range] = None
 
     @property
-    def id(self):
+    def id(self) -> str:
         """Gets the item_id of the found item."""
         return self.item.id
 
     def get_text(self) -> str:
-        """Gets the chunk text of the found item."""
+        """Gets the chunk text or full text of the found item depending on the presence of substring_range."""
         fulltext = self.item.get_text()
         if self.substring_range is not None:
-            r = self.substring_range
-            return fulltext[r.start : r.stop]
+            return fulltext[self.substring_range.start : self.substring_range.stop]
         else:
             return fulltext
 
 
 class AbstractSearchIndex(Generic[T], ABC):
     @abstractmethod
     def update(self, items: Iterable[T]):
@@ -168,17 +168,15 @@
         raise NotImplementedError()
 
     def get_item(self, item_id: str) -> T:
         """Get the item for the given id. Raises KeyError if not found."""
         raise NotImplementedError()
 
 
-def chunk_item(
-    item: TextItem, max_chunk_size: int, model: EmbeddingModel
-) -> Iterable[Chunk]:
+def chunk_item(item: TextItem, max_chunk_size: int, model: EmbeddingModel) -> Iterable[Chunk]:
     """Run item.chunk or fallback to simple_chunker.
 
     Also performs some validation that the chunks are constructed correctly.
     """
     chunks = item.chunk(max_chunk_size, model)
     if chunks is NotImplemented:
         chunks = simple_chunker(item, max_chunk_size, model)
@@ -258,29 +256,31 @@
         The default algorithm is `simple_chunker`.
 
         Args:
             items (Iterable[TextItem]): The items to add to the index.
         Raises:
             NotImplementedError: If updating items that already exist in the index. (we are working on it)
         """
-        items = list(items)
-        for item in items:
+        iterated_items = []
+
+        for item in tqdm(items):
             if item.id in self.items:
                 # [todo]
                 raise NotImplementedError(
                     "Updating items that already exist in the index is not currently supported."
                 )
             self.items[item.id] = item
-        texts = list(self._cmap.extend(get_chunks(items, self.embedding_model)))
+            iterated_items.append(item)
+        texts = list(self._cmap.extend(get_chunks(iterated_items, self.embedding_model)))
         embeddings: np.ndarray = self.embedding_model.encode(texts)
         assert len(texts) == len(embeddings)
         self.vector_index.add(embeddings)
         assert len(self.vector_index) == len(self._cmap)
         logger.debug(
-            f"Added {len(items)} items ({len(texts)} chunks) to the search index."
+            f"Added {len(iterated_items)} items ({len(texts)} chunks) to the search index."
         )
 
     def search(self, query: str, limit=5) -> Iterable[SearchResult]:
         """Finds a set of nearest results for the given query.
 
         The exact algorithm used is determined by the choice of self.vector_index.
         The resulting SearchResult objects can be used to identify the documents and chunks of documents that match the query.
```

### Comparing `capabilities-0.1.2/capabilities/search/simple_vector_index.py` & `capabilities-0.3.0/capabilities/search/simple_vector_index.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         d = self.rows.shape[1]
         if d == 0:
             return None
         else:
             return d
 
     def add(self, arr):
-        assert len(arr.shape) == 2
+        assert len(arr.shape) == 2, f"arr.shape={arr.shape}"
         norm = np.linalg.norm(arr, axis=1)
         if np.any(norm == 0):
             raise ValueError("vector with norm 0 detected")
         arr /= norm[:, np.newaxis]
         if len(self) == 0:
             self.rows = arr
         else:
```

### Comparing `capabilities-0.1.2/capabilities/search/types.py` & `capabilities-0.3.0/capabilities/search/types.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.1.2/capabilities/search/util.py` & `capabilities-0.3.0/capabilities/search/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,17 +36,15 @@
     return x[1]
 
 
 def argmin(a):
     return min(range(len(a)), key=lambda x: a[x])
 
 
-def partition(
-    pred: Callable[[T], bool], iterable: Iterable[T]
-) -> tuple[Iterable[T], Iterable[T]]:
+def partition(pred: Callable[[T], bool], iterable: Iterable[T]) -> tuple[Iterable[T], Iterable[T]]:
     """Use a predicate to partition entries into false entries and true entries
 
     origin: https://docs.python.org/3/library/itertools.html#itertools-recipes
     """
     # partition(is_odd, range(10)) --> 0 2 4 6 8   and  1 3 5 7 9
     t1, t2 = itertools.tee(iterable)
     return itertools.filterfalse(pred, t1), filter(pred, t2)
@@ -197,13 +195,13 @@
         assert isinstance(d, dict)
         self._forward = d
         self._inverse = {v: k for k, v in self._forward.items()}
         assert len(self._forward) == len(self._inverse), "not a bijection"
 
 
 def digest(item: Union[str, bytes]):
-    """ Computes the blake2b digest of a given item. """
+    """Computes the blake2b digest of a given item."""
     h = blake2b()
     if isinstance(item, str):
         item = item.encode("utf-8")
     h.update(item)
     return h.hexdigest()
```

### Comparing `capabilities-0.1.2/capabilities/util.py` & `capabilities-0.3.0/capabilities/util/misc.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,20 @@
+from dataclasses import dataclass
 import time
 import aiohttp
 import fire
 import os
 import requests
 import openai
 import random
 import tiktoken
+import concurrent.futures
+from typing import Callable, List, Any, TypeVar, Iterable, Optional
+import time
+from threading import Thread
 
 ENCODER = tiktoken.get_encoding("p50k_base")
 
 
 def tokenize(contents):
     return ENCODER.encode(contents)
 
@@ -18,15 +23,18 @@
     return ENCODER.decode(tokens)
 
 
 def get_chunks_tokenized(contents: str, max_len: int = 256, stride=None):
     if stride is None:
         stride = max_len
     tokens = tokenize(contents)
-    return [tokens[stride * i : stride * i + max_len] for i in range(len(tokens) // stride + 1)]
+    return [
+        tokens[stride * i : stride * i + max_len]
+        for i in range(len(tokens) // stride + 1)
+    ]
 
 
 def get_tokenized_length(contents: str):
     return len(tokenize(contents))
 
 
 def get_chunks_core(contents, max_len, stride=None):
@@ -56,15 +64,17 @@
             # Retry on specified errors
             except errors as e:
                 # Increment retries
                 num_retries += 1
 
                 # Check if max retries has been reached
                 if num_retries > max_retries:
-                    raise Exception(f"Maximum number of retries ({max_retries}) exceeded.")
+                    raise Exception(
+                        f"Maximum number of retries ({max_retries}) exceeded."
+                    )
                 print(
                     f"[retry_with_exponential_backoff] retrying, num_retries={num_retries} max_retries={max_retries}"
                 )
 
                 # Increment the delay
                 delay *= exponential_base * (1 + jitter * random.random())
 
@@ -101,15 +111,17 @@
             # Retry on specified errors
             except errors as e:
                 # Increment retries
                 num_retries += 1
 
                 # Check if max retries has been reached
                 if num_retries > max_retries:
-                    raise Exception(f"Maximum number of retries ({max_retries}) exceeded.")
+                    raise Exception(
+                        f"Maximum number of retries ({max_retries}) exceeded."
+                    )
                 print(
                     f"[retry_with_exponential_backoff] retrying, num_retries={num_retries} max_retries={max_retries}"
                 )
 
                 # Increment the delay
                 delay *= exponential_base * (1 + jitter * random.random())
 
@@ -149,9 +161,60 @@
 @retry_with_exponential_backoff
 def text_embed(prompt):
     headers = {
         "Content-Type": "application/json",
         "Authorization": f"Bearer {os.environ.get('OPENAI_API_KEY_EMBED')}",
     }
     payload = {"input": prompt, "model": "text-embedding-ada-002"}
-    r = requests.post("https://api.openai.com/v1/embeddings", headers=headers, json=payload)
+    r = requests.post(
+        "https://api.openai.com/v1/embeddings", headers=headers, json=payload
+    )
     return r.json()["data"][0]["embedding"]
+
+
+T = TypeVar("T")
+
+
+def parallel_map(
+    fn: Callable, xs: List[T], parallelism: int = 8, ignore_exceptions: bool = False
+) -> Iterable[T]:
+    results = [None] * len(xs)  # initialize with None
+    current_index = 0
+
+    @dataclass
+    class IgnoreException:
+        exception: Optional[Any] = None
+
+    if ignore_exceptions:
+
+        def wrapper_fn(*args, **kwargs):
+            try:
+                return fn(*args, **kwargs)
+            except Exception as e:
+                return IgnoreException(exception=e)
+
+    fn2 = wrapper_fn if ignore_exceptions else fn
+
+    def get_results():
+        with concurrent.futures.ThreadPoolExecutor(parallelism) as executor:
+            futures = [executor.submit(fn2, x) for x in xs]
+
+            for future in concurrent.futures.as_completed(futures):
+                idx = futures.index(future)  # get index of current future
+                result = future.result()  # get result of current future
+                results[idx] = result  # insert result into proper index
+
+    t = Thread(target=get_results)
+    t.start()
+    while current_index < len(results):
+        if results[current_index] is not None:
+            if not ignore_exceptions:
+                yield results[current_index]
+                current_index += 1
+            else:
+                if not isinstance(results[current_index], IgnoreException):
+                    yield results[current_index]
+                    current_index += 1
+                else:
+                    print("Got an exception!", results[current_index])
+                    current_index += 1
+    t.join()
```

### Comparing `capabilities-0.1.2/pyproject.toml` & `capabilities-0.3.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["setuptools==63.4.1"]
-build-backend = "setuptools.build_meta"
+requires = ["hatchling"]
+build-backend = "hatchling.build"
 
 [project]
 name = "capabilities"
-version = "0.1.2"
+dynamic = ["version"]
 authors = [
   { name="Blazon AI", email="support@blazon.ai" },
 ]
 description = "Build trusted, faster, and more powerful applications with the Blazon Capabilities API."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
@@ -19,31 +19,45 @@
   "asyncio",
   "aiohttp",
   "pdfminer.six",
   "tiktoken",
   "blobfile",
   "pydantic",
   "pydantic[dotenv]",
-  "termcolor",
   "rich",
+  "typer",
+  "openai",
+  "backoff",
+  "diskcache",
+  "google",
+  "openai",
+  "textual",
 ]
 
+[project.scripts]
+capabilities = "capabilities.cli:app"
+
+[tool.hatch.version]
+path = "capabilities/__about__.py"
+
 [project.optional-dependencies]
 search = [
   "pyllamacpp",
   "python-magic",
   "bs4",
-  "diskcache",
 ]
 nomic = [
   "nomic",
 ]
 sentence-transformers = [
   "sentence-transformers"
 ]
+agent = [
+    "google"
+]
 
 [tool.hatch.envs.default]
 dependencies = [
   "coverage[toml]>=6.5",
   "pytest",
   "pytest-snapshot",
   "hypothesis",
@@ -54,15 +68,15 @@
   "requests",
   "dacite",
   "aiohttp",
   "tiktoken",
   "pyllamacpp",
   "python-magic",
   "bs4",
-  "diskcache",
+  "google"
 ]
 [tool.hatch.envs.default.scripts]
 test = "pytest {args:tests}"
 test-cov = "coverage run -m pytest {args:tests}"
 cov-report = [
   "- coverage combine",
   "coverage report",
```

