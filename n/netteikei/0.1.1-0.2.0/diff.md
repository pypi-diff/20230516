# Comparing `tmp/netteikei-0.1.1-py3-none-any.whl.zip` & `tmp/netteikei-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 6519 bytes, number of entries: 12
--rw-------  2.0 unx       64 b- defN 23-May-08 13:50 netteikei/__init__.py
--rw-------  2.0 unx     2801 b- defN 23-May-08 13:39 netteikei/core.py
+Zip file size: 6607 bytes, number of entries: 12
+-rw-------  2.0 unx      131 b- defN 23-May-16 19:25 netteikei/__init__.py
+-rw-------  2.0 unx     2679 b- defN 23-May-14 16:14 netteikei/core.py
 -rw-------  2.0 unx        0 b- defN 23-May-07 09:41 netteikei/py.typed
--rw-------  2.0 unx     1055 b- defN 23-May-08 13:39 netteikei/typedefs.py
+-rw-------  2.0 unx     1297 b- defN 23-May-14 16:14 netteikei/typedefs.py
 -rw-------  2.0 unx        0 b- defN 23-May-07 13:53 netteikei/contrib/__init__.py
--rw-------  2.0 unx     2487 b- defN 23-May-08 13:39 netteikei/contrib/download.py
--rw-------  2.0 unx     1144 b- defN 23-May-08 13:39 netteikei/contrib/utils.py
--rw-------  2.0 unx     1068 b- defN 23-May-08 13:58 netteikei-0.1.1.dist-info/LICENSE
--rw-------  2.0 unx     1325 b- defN 23-May-08 13:58 netteikei-0.1.1.dist-info/METADATA
--rw-------  2.0 unx       92 b- defN 23-May-08 13:58 netteikei-0.1.1.dist-info/WHEEL
--rw-------  2.0 unx       10 b- defN 23-May-08 13:58 netteikei-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      948 b- defN 23-May-08 13:58 netteikei-0.1.1.dist-info/RECORD
-12 files, 10994 bytes uncompressed, 4925 bytes compressed:  55.2%
+-rw-------  2.0 unx     2435 b- defN 23-May-14 16:48 netteikei/contrib/download.py
+-rw-------  2.0 unx     1158 b- defN 23-May-14 17:10 netteikei/contrib/utils.py
+-rw-------  2.0 unx     1068 b- defN 23-May-16 19:27 netteikei-0.2.0.dist-info/LICENSE
+-rw-------  2.0 unx     1325 b- defN 23-May-16 19:27 netteikei-0.2.0.dist-info/METADATA
+-rw-------  2.0 unx       92 b- defN 23-May-16 19:27 netteikei-0.2.0.dist-info/WHEEL
+-rw-------  2.0 unx       10 b- defN 23-May-16 19:27 netteikei-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      949 b- defN 23-May-16 19:27 netteikei-0.2.0.dist-info/RECORD
+12 files, 11144 bytes uncompressed, 5013 bytes compressed:  55.0%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: netteikei/contrib/download.py
 Comment: 
 
 Filename: netteikei/contrib/utils.py
 Comment: 
 
-Filename: netteikei-0.1.1.dist-info/LICENSE
+Filename: netteikei-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: netteikei-0.1.1.dist-info/METADATA
+Filename: netteikei-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: netteikei-0.1.1.dist-info/WHEEL
+Filename: netteikei-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: netteikei-0.1.1.dist-info/top_level.txt
+Filename: netteikei-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: netteikei-0.1.1.dist-info/RECORD
+Filename: netteikei-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## netteikei/__init__.py

```diff
@@ -1,3 +1,6 @@
-__version__ = "0.1.1"
+from .core import Client, Handler
+from .typedefs import Request
 
-from .core import Client, RequestHandler
+
+__version__ = "0.2.0"
+__all__ = ["Client", "Handler", "Request"]
```

## netteikei/core.py

```diff
@@ -1,101 +1,99 @@
 from abc import ABC, abstractmethod
 import asyncio
 from contextvars import ContextVar
 from typing import Generic, TypeVar, final
 
 from aiohttp import ClientResponse, ClientSession
 
-from .typedefs import RequestParams
+from .typedefs import Request
 
 
-T = TypeVar("T")
-U = TypeVar("U")
+_T = TypeVar("_T")
+_R = TypeVar("_R")
 
 
-class RequestHandler(ABC, Generic[T, U]):
-    """
-    Base class designed as a template for making concurrent HTTP requests.
+class Handler(ABC, Generic[_T, _R]):
+    """Base class designed for making requests.
 
     Attributes
     ----------
     ctx
         Context variable possessing relevant data for making requests.
-        Its value is set automatically for each request.
+        The value is automatically set for each request.
 
     Methods
     -------
-    generate_params()
-        Returns the HTTP method, URL and options for the request.
-        These options override the options set in the underlying
-        `aiohttp.ClientSession` instance. This method is automatically
-        called before making each request.
-
+    create_request()
+        Returns the request URL and options to override the options set
+        in the underlying `aiohttp.ClientSession` instance. This method
+        is called before making each request.
     process_response(resp)
         Processes the `aiohttp.ClientResponse` instance received as its
-        only argument into the relevant result. This method is called
-        automatically after a request has been made.
+        only argument into relevant data. This method is called after a
+        request has been made.
     """
 
-    ctx: ContextVar[T] = ContextVar("ctx")
+    ctx: ContextVar[_T] = ContextVar("ctx")
 
     @abstractmethod
-    async def generate_params(self) -> RequestParams:
+    async def create_request(self) -> Request:
         ...
 
     @abstractmethod
-    async def process_response(self, resp: ClientResponse) -> U:
+    async def process_response(self, res: ClientResponse) -> _R:
         ...
 
 
 @final
-class Client(Generic[T, U]):
+class Client(Generic[_T, _R]):
     """
     Utility for making concurrent HTTP requests.
 
     Parameters
     ----------
     session
         An instance of `aiohttp.ClientSession`.
     handler
-        Instance of a `RequestHandler` implementation.
+        Instance of a `Handler` implementation.
     max_workers, default 5
         Number of request workers that can run concurrently.
 
     See Also
     --------
-    netteikei.RequestHandler : Abstract base class for making requests.
+    Handler : Abstract base class for making requests.
     """
 
     def __init__(
         self,
         session: ClientSession,
-        handler: RequestHandler[T, U],
+        handler: Handler[_T, _R],
         max_workers: int = 5
     ) -> None:
         self._session = session
         self._handler = handler
         self._sem = asyncio.Semaphore(max_workers)
     
-    async def _request(self, obj: T) -> U:
+    async def _request(self, obj: _T) -> _R:
         async with self._sem:
             self._handler.ctx.set(obj)
-            method, url, opts = await self._handler.generate_params()
-            async with self._session.request(method, url, **opts) as resp:
-                return await self._handler.process_response(resp)
+            method, url, opts = await self._handler.create_request()
+            async with self._session.request(method, url, **opts) as res:
+                return await self._handler.process_response(res)
 
-    async def gather(self, *args: T) -> list[U]:
-        """
-        Processes data into relevant results using the `RequestHandler`
-        implementation provided by the user.
+    async def gather(self, *objs: _T) -> list[_R]:
+        """Make multiple concurrent HTTP requests.
+
+        Processes the given objects into relevant data using the provided
+        `Handler` implementation.
 
         Parameters
         ----------
-        *args
+        obj
             Data required for making requests.
 
         Returns
         -------
         list
             Results processed from the given data.
         """
-        return await asyncio.gather(*(self._request(obj) for obj in args))
+        return await asyncio.gather(*(self._request(obj) for obj in objs))
```

## netteikei/typedefs.py

```diff
@@ -1,13 +1,9 @@
-from collections.abc import (
-    Callable,
-    Iterable,
-    Mapping
-)
-from typing import Any, Literal, TypedDict
+from collections.abc import Callable, Iterable, Mapping
+from typing import Any, Literal, NamedTuple, Self, TypedDict, Unpack
 
 from aiohttp import (
     BaseConnector,
     BasicAuth,
     ClientTimeout,
     HttpVersion,
     TraceConfig
@@ -37,8 +33,21 @@
     auto_decompress: bool
     read_bufsize: int
     trust_env: bool
     requote_redirect_url: bool
     trace_configs: list[TraceConfig] | None
 
 
-RequestParams = tuple[Method, StrOrURL, SessionOpts]
+class Request(NamedTuple):
+    method: Method
+    url: StrOrURL
+    opts: SessionOpts
+
+    @classmethod
+    def new(
+        cls,
+        *,
+        method: Method = "GET",
+        url: StrOrURL,
+        **opts: Unpack[SessionOpts]
+    ) -> Self:
+        return cls(method, url, opts)
```

## netteikei/contrib/download.py

```diff
@@ -3,37 +3,29 @@
 from pathlib import Path
 from typing import NamedTuple, Self, Unpack
 
 import aiofiles
 from aiohttp import ClientResponse, ClientSession
 import tqdm
 
-from .. import Client, RequestHandler
-from ..typedefs import (
-    RequestParams,
-    SessionOpts,
-    StrOrURL
-)
-from .utils import (
-    parse_name,
-    parse_length,
-    get_start_byte
-)
+from .. import Client, Handler
+from ..typedefs import Request, SessionOpts, StrOrURL
+from .utils import isfile, parse_name, parse_length, get_start_byte
 
 
 _DIR: ContextVar[Path] = ContextVar("dir")
 
 
 class DownloadAlreadyExists(Exception):
     
-    def __init__(self, name: str) -> None:
-        self.name = name
+    def __init__(self, path: Path) -> None:
+        self.path = path
 
     def __str__(self) -> str:
-        return f"'{self.name}' alredy exists"
+        return f"'{self.path}' alredy exists"
 
 
 class Download(NamedTuple):
     url: StrOrURL
     path: Path
     length: int | None
     start: int
@@ -41,24 +33,27 @@
     @classmethod
     async def new(cls, session: ClientSession, url: StrOrURL, /) -> Self:
         async with session.head(url) as resp:
             name = parse_name(resp, "untitled")
             length = parse_length(resp.headers)
             path = _DIR.get() / name
             start = await get_start_byte(resp.headers, path)
-            if start == length:
-                raise DownloadAlreadyExists(name)
+            if await isfile(path) and start == length:
+                raise DownloadAlreadyExists(path)
             return cls(url, path, length, start)
 
 
-class DownloadHandler(RequestHandler[Download, None]):
+class Downloader(Handler[Download, None]):
 
-    async def generate_params(self) -> RequestParams:
+    async def create_request(self) -> Request:
         dl = self.ctx.get()
-        return "GET", dl.url, {"headers": {"Range": f"bytes={dl.start}-"}}
+        return Request.new(
+            url=dl.url,
+            headers={"Range": f"bytes={dl.start}-"}
+        )
 
     async def process_response(self, resp: ClientResponse) -> None:
         dl = self.ctx.get()
         async with resp, aiofiles.open(dl.path, "wb") as f:
             with tqdm.tqdm(
                 total=dl.length,
                 initial=dl.start,
@@ -73,21 +68,18 @@
                     pbar.update(len(chunk))
 
 
 async def download(
     dir: Path,
     /,
     *urls: StrOrURL,
-    concurrent_limit: int = 3,
+    limit: int = 3,
     **kwargs: Unpack[SessionOpts]
 ) -> None:
-    _DIR.set(dir)
+    token = _DIR.set(dir)
     async with ClientSession(**kwargs) as session:
         dls = await asyncio.gather(
             *(Download.new(session, url) for url in urls)
         )
-        client = Client(
-            session=session,
-            handler=DownloadHandler(),
-            max_workers=concurrent_limit
-        )
+        client = Client(session, Downloader(), max_workers=limit)
         await client.gather(*dls)
+    _DIR.reset(token)
```

## netteikei/contrib/utils.py

```diff
@@ -6,35 +6,41 @@
 from typing import ParamSpec, TypeVar
 
 from aiohttp import ClientResponse
 import pyrfc6266
 
 from ..typedefs import Headers
 
-P = ParamSpec("P")
-T = TypeVar("T")
 
-def _wrap(fn: Callable[P, T]) -> Callable[P, Awaitable[T]]:
+_P = ParamSpec("_P")
+_R = TypeVar("_R")
+
+
+def wrap(fn: Callable[_P, _R]) -> Callable[_P, Awaitable[_R]]:
     @functools.wraps(fn)
-    async def inner(*args: P.args, **kwargs: P.kwargs) -> T:
+    async def inner(*args: _P.args, **kwargs: _P.kwargs) -> _R:
         return await asyncio.to_thread(fn, *args, **kwargs)
     return inner
 
-getsize = _wrap(os.path.getsize)
-isfile = _wrap(os.path.isfile)
+
+getsize = wrap(os.path.getsize)
+isfile = wrap(os.path.isfile)
+
 
 def parse_name(resp: ClientResponse, default: str) -> str:
     if (s := resp.headers.get("Content-Disposition")) is None:
         return resp.url.name
     else:
         if (name := pyrfc6266.parse_filename(s)) is None:
             return default
         return name
 
+
 def parse_length(headers: Headers) -> int | None:
     if (s := headers.get("Content-Length")) is not None:
         return int(s)
 
+
 async def get_start_byte(headers: Headers, file: Path) -> int:
     if headers.get("Accept-Ranges") == "bytes" and await isfile(file):
         return await getsize(file)
     return 0
```

## Comparing `netteikei-0.1.1.dist-info/LICENSE` & `netteikei-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `netteikei-0.1.1.dist-info/METADATA` & `netteikei-0.2.0.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netteikei
-Version: 0.1.1
+Version: 0.2.0
 Summary: Utility library for making concurrent HTTP requests using aiohttp
 Home-page: https://github.com/fernofsigma/netteikei
 Author: FernOfSigma
 Author-email: fernofsigma@tuta.io
 License: MIT
 Project-URL: GitHub: issues, https://github.com/fernofsigma/netteikei/issues
 Project-URL: GitHub: repo, https://github.com/fernofsigma/netteikei
```

## Comparing `netteikei-0.1.1.dist-info/RECORD` & `netteikei-0.2.0.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-netteikei/__init__.py,sha256=Q5RWyjANksYTANd5T034RArj6BC9pTRauz-ud9U5VjY,64
-netteikei/core.py,sha256=et2XxAkQhs4QSkbBEfH811BJ7QqakxbLwiO_1qJnCcw,2801
+netteikei/__init__.py,sha256=4OoJPt3pWzJhk4t7p68Lh81uzeBbt_-ZehOm210C_vU,131
+netteikei/core.py,sha256=_iwcs1T3j8ZjN46x02f8rP0SlClnpeD-Q8Codq3Oz4Q,2679
 netteikei/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-netteikei/typedefs.py,sha256=UjwEfJvuwJ0693C5OQ8Eg-bivCQbWwwJ5cB0I-ULYXI,1055
+netteikei/typedefs.py,sha256=WG1_PMtZVnXJTfOTTOUY9nSQ5TDID1URux9GwGJWVNA,1297
 netteikei/contrib/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-netteikei/contrib/download.py,sha256=l2GEBdBCWBqfgVPQ41fF94nKSGU91wT44ZYXlxVgFTk,2487
-netteikei/contrib/utils.py,sha256=JDqp5rH9fb1nBejde0_0sNQpRsK1BoqMeV46371-zCI,1144
-netteikei-0.1.1.dist-info/LICENSE,sha256=37AgUwjy1RqDbLVahc_zXbHKIRzTEKjlDpKfzB6a-6g,1068
-netteikei-0.1.1.dist-info/METADATA,sha256=JaE51vox1d1QfsBCrQdJcwdtfoEDsxCI1KzhSL6Kmbo,1325
-netteikei-0.1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-netteikei-0.1.1.dist-info/top_level.txt,sha256=1TkkZh-n9Ys0kU95kW0keVBeiiY87lC-pR-FF7FFGB0,10
-netteikei-0.1.1.dist-info/RECORD,,
+netteikei/contrib/download.py,sha256=gCRn4cVUPiVziPRK2ioJmcX_9eGIs3c13c6jttdDT8k,2435
+netteikei/contrib/utils.py,sha256=tWW73FXdlUGyhZKJoLU1lSb7u_OciKpcZPBXWFkwfyE,1158
+netteikei-0.2.0.dist-info/LICENSE,sha256=37AgUwjy1RqDbLVahc_zXbHKIRzTEKjlDpKfzB6a-6g,1068
+netteikei-0.2.0.dist-info/METADATA,sha256=Gntz48i9k8sdbgMQU5zxRv-IBzNCQ5GRFV2624ie-RI,1325
+netteikei-0.2.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+netteikei-0.2.0.dist-info/top_level.txt,sha256=1TkkZh-n9Ys0kU95kW0keVBeiiY87lC-pR-FF7FFGB0,10
+netteikei-0.2.0.dist-info/RECORD,,
```

