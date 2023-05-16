# Comparing `tmp/ethhelper-0.3.6.tar.gz` & `tmp/ethhelper-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ethhelper-0.3.6.tar", max compression
+gzip compressed data, was "ethhelper-0.4.0.tar", max compression
```

## Comparing `ethhelper-0.3.6.tar` & `ethhelper-0.4.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0    11357 2023-05-09 05:07:50.736843 ethhelper-0.3.6/LICENSE
--rw-r--r--   0        0        0     1708 2023-05-09 05:07:50.736843 ethhelper-0.3.6/README.md
--rw-r--r--   0        0        0     2155 2023-05-09 05:07:50.740844 ethhelper-0.3.6/pyproject.toml
--rw-r--r--   0        0        0      156 2023-05-09 05:07:50.740844 ethhelper-0.3.6/src/ethhelper/__init__.py
--rw-r--r--   0        0        0        0 2023-05-09 05:07:50.740844 ethhelper-0.3.6/src/ethhelper/connectors/__init__.py
--rw-r--r--   0        0        0     1565 2023-05-09 05:07:50.740844 ethhelper-0.3.6/src/ethhelper/connectors/http/__init__.py
--rw-r--r--   0        0        0    13216 2023-05-09 05:07:50.740844 ethhelper-0.3.6/src/ethhelper/connectors/http/base.py
--rw-r--r--   0        0        0     7712 2023-05-09 05:07:50.740844 ethhelper-0.3.6/src/ethhelper/connectors/http/custom.py
--rw-r--r--   0        0        0    16281 2023-05-09 05:07:50.740844 ethhelper-0.3.6/src/ethhelper/connectors/http/eth.py
--rw-r--r--   0        0        0     1743 2023-05-09 05:07:50.740844 ethhelper-0.3.6/src/ethhelper/connectors/http/net.py
--rw-r--r--   0        0        0     3958 2023-05-09 05:07:50.740844 ethhelper-0.3.6/src/ethhelper/connectors/http/txpool.py
--rw-r--r--   0        0        0      159 2023-05-09 05:07:50.740844 ethhelper-0.3.6/src/ethhelper/connectors/ws/__init__.py
--rw-r--r--   0        0        0     5912 2023-05-09 05:07:50.740844 ethhelper-0.3.6/src/ethhelper/connectors/ws/base.py
--rw-r--r--   0        0        0     3505 2023-05-09 05:07:50.740844 ethhelper-0.3.6/src/ethhelper/connectors/ws/block.py
--rw-r--r--   0        0        0        0 2023-05-09 05:07:50.740844 ethhelper-0.3.6/src/ethhelper/datatypes/__init__.py
--rw-r--r--   0        0        0     7579 2023-05-09 05:07:50.740844 ethhelper-0.3.6/src/ethhelper/datatypes/base.py
--rw-r--r--   0        0        0    17501 2023-05-09 05:07:50.740844 ethhelper-0.3.6/src/ethhelper/datatypes/eth.py
--rw-r--r--   0        0        0     6824 2023-05-09 05:07:50.740844 ethhelper-0.3.6/src/ethhelper/datatypes/geth.py
--rw-r--r--   0        0        0     5135 2023-05-09 05:07:50.740844 ethhelper-0.3.6/src/ethhelper/datatypes/txpool.py
--rw-r--r--   0        0        0        0 2023-05-09 05:07:50.740844 ethhelper-0.3.6/src/ethhelper/py.typed
--rw-r--r--   0        0        0     1387 2023-05-09 05:07:50.740844 ethhelper-0.3.6/src/ethhelper/types.py
--rw-r--r--   0        0        0        0 2023-05-09 05:07:50.740844 ethhelper-0.3.6/src/ethhelper/utils/__init__.py
--rw-r--r--   0        0        0      927 2023-05-09 05:07:50.740844 ethhelper-0.3.6/src/ethhelper/utils/convert.py
--rw-r--r--   0        0        0      498 2023-05-09 05:07:50.740844 ethhelper-0.3.6/src/ethhelper/utils/json.py
--rw-r--r--   0        0        0     2851 1970-01-01 00:00:00.000000 ethhelper-0.3.6/setup.py
--rw-r--r--   0        0        0     2679 1970-01-01 00:00:00.000000 ethhelper-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-16 10:10:44.942273 ethhelper-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1708 2023-05-16 10:10:44.942273 ethhelper-0.4.0/README.md
+-rw-r--r--   0        0        0     2155 2023-05-16 10:10:44.946274 ethhelper-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      174 2023-05-16 10:10:44.946274 ethhelper-0.4.0/src/ethhelper/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-16 10:10:44.946274 ethhelper-0.4.0/src/ethhelper/connectors/__init__.py
+-rw-r--r--   0        0        0     1966 2023-05-16 10:10:44.946274 ethhelper-0.4.0/src/ethhelper/connectors/http/__init__.py
+-rw-r--r--   0        0        0    13216 2023-05-16 10:10:44.946274 ethhelper-0.4.0/src/ethhelper/connectors/http/base.py
+-rw-r--r--   0        0        0     9327 2023-05-16 10:10:44.946274 ethhelper-0.4.0/src/ethhelper/connectors/http/custom.py
+-rw-r--r--   0        0        0    16281 2023-05-16 10:10:44.946274 ethhelper-0.4.0/src/ethhelper/connectors/http/eth.py
+-rw-r--r--   0        0        0     5175 2023-05-16 10:10:44.946274 ethhelper-0.4.0/src/ethhelper/connectors/http/graphql.py
+-rw-r--r--   0        0        0     1743 2023-05-16 10:10:44.946274 ethhelper-0.4.0/src/ethhelper/connectors/http/net.py
+-rw-r--r--   0        0        0     3958 2023-05-16 10:10:44.946274 ethhelper-0.4.0/src/ethhelper/connectors/http/txpool.py
+-rw-r--r--   0        0        0      159 2023-05-16 10:10:44.946274 ethhelper-0.4.0/src/ethhelper/connectors/ws/__init__.py
+-rw-r--r--   0        0        0     5912 2023-05-16 10:10:44.946274 ethhelper-0.4.0/src/ethhelper/connectors/ws/base.py
+-rw-r--r--   0        0        0     3505 2023-05-16 10:10:44.946274 ethhelper-0.4.0/src/ethhelper/connectors/ws/block.py
+-rw-r--r--   0        0        0        0 2023-05-16 10:10:44.946274 ethhelper-0.4.0/src/ethhelper/datatypes/__init__.py
+-rw-r--r--   0        0        0     7579 2023-05-16 10:10:44.946274 ethhelper-0.4.0/src/ethhelper/datatypes/base.py
+-rw-r--r--   0        0        0    17501 2023-05-16 10:10:44.946274 ethhelper-0.4.0/src/ethhelper/datatypes/eth.py
+-rw-r--r--   0        0        0     7167 2023-05-16 10:10:44.946274 ethhelper-0.4.0/src/ethhelper/datatypes/geth.py
+-rw-r--r--   0        0        0     5135 2023-05-16 10:10:44.946274 ethhelper-0.4.0/src/ethhelper/datatypes/txpool.py
+-rw-r--r--   0        0        0        0 2023-05-16 10:10:44.946274 ethhelper-0.4.0/src/ethhelper/py.typed
+-rw-r--r--   0        0        0     1387 2023-05-16 10:10:44.946274 ethhelper-0.4.0/src/ethhelper/types.py
+-rw-r--r--   0        0        0        0 2023-05-16 10:10:44.946274 ethhelper-0.4.0/src/ethhelper/utils/__init__.py
+-rw-r--r--   0        0        0      927 2023-05-16 10:10:44.946274 ethhelper-0.4.0/src/ethhelper/utils/convert.py
+-rw-r--r--   0        0        0      498 2023-05-16 10:10:44.946274 ethhelper-0.4.0/src/ethhelper/utils/json.py
+-rw-r--r--   0        0        0     2851 1970-01-01 00:00:00.000000 ethhelper-0.4.0/setup.py
+-rw-r--r--   0        0        0     2679 1970-01-01 00:00:00.000000 ethhelper-0.4.0/PKG-INFO
```

### Comparing `ethhelper-0.3.6/LICENSE` & `ethhelper-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ethhelper-0.3.6/README.md` & `ethhelper-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `ethhelper-0.3.6/pyproject.toml` & `ethhelper-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "ethhelper"
-version = "0.3.6"
+version = "0.4.0"
 description = "Asynchronous Geth node connection encapsulation based on httpx, websockets and web3.py. Geth node and Ethereum type extension based on pydantic."
 authors = ["XiaoHuiHui233 <1025184872@qq.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/XiaoHuiHui233/ETHHelper"
 keywords = ["ethereum", "asyncio", "geth", "pydantic"]
 
 [tool.poetry.dependencies]
 eth-typing = "^3.3.0"
 httpx = "^0.23.3"
 orjson = "^3.8.12"
 pydantic = "^1.10.7"
 python = "^3.10"
-web3 = "^6.3.0"
+web3 = "^6.4.0"
 websockets = "^10.4"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 isort = "^5.12.0"
 mypy = "^1.2.0"
 pytest = "^7.3.1"
```

### Comparing `ethhelper-0.3.6/src/ethhelper/connectors/http/__init__.py` & `ethhelper-0.4.0/src/ethhelper/connectors/http/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,23 +10,26 @@
 )
 from .custom import (
     GethCustomHttp,
 )
 from .eth import (
     GethEthHttp,
 )
+from .graphql import (
+    GethGraphQL,
+)
 from .net import (
     GethNetHttp,
 )
 from .txpool import (
     GethTxpoolHttp,
 )
 
 
-class GethHttpConnector(GethCustomHttp):
+class GethHttpConnector(GethGraphQL, GethCustomHttp):
     """``GethHttpConnector`` is an asynchronous wrapper for all HTTP interfaces
     supported by ETHHelper.
 
     Due to the flat design style, all interfaces use a simple naming structure
     as the member methods of this class.
 
     The ``url`` is used to indicate the path of the HTTP service of the Geth
@@ -35,24 +38,35 @@
 
     The ``logger`` is used to assign a logger of the Python logging module to
     this class. Explicitly assigning a logger can be used to control the output
     location of the logger, which is convenient for debugging. If this
     parameter is not provided or ``None`` is giving, this class will
     automatically call ``logging.getLogger("GethHttpConnector")`` to generate a
     default logger.
+
+    The ``graphql_url`` is used to specify the URL for the GraphQL interface of
+    the Geth node, usually in the form of ``http://host:port/graphql``. If not
+    provided, it will generate from ``url`` by appending ``/graphql``.
     """
-    def __init__(self, url: str, logger: Logger | None = None) -> None:
+    def __init__(
+        self,
+        url: str,
+        logger: Logger | None = None,
+        graphql_url: str | None = None
+    ) -> None:
         if logger is None:
             logger = logging.getLogger("GethHttpConnector")
-        super().__init__(url, logger)
+        super().__init__(url, logger, graphql_url=graphql_url)
+
 
 
 __all__ = [
     "GethHttpAbstract",
     "GethHttpCustomized",
     "GethHttpWeb3",
     "GethCustomHttp",
     "GethEthHttp",
     "GethNetHttp",
     "GethTxpoolHttp",
-    "GethHttpConnector"
+    "GethHttpConnector",
+    "GethGraphQL"
 ]
```

### Comparing `ethhelper-0.3.6/src/ethhelper/connectors/http/base.py` & `ethhelper-0.4.0/src/ethhelper/connectors/http/base.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.3.6/src/ethhelper/connectors/http/custom.py` & `ethhelper-0.4.0/src/ethhelper/connectors/http/custom.py`

 * *Files 14% similar despite different names*

```diff
@@ -94,47 +94,55 @@
         return [Log.parse_obj(log) for log in logs]
 
     async def get_logs_by_blocks(
         self,
         start_height: BlockNumber,
         end_height: BlockNumber,
         address: Address | list[Address] | None = None,
-        topics: Sequence[Hash32 | Sequence[Hash32]] | None = None
+        topics: Sequence[Hash32 | Sequence[Hash32]] | None = None,
+        step: int = 200
     ) -> list[Log]:
         """Retrieve a list of logs within a range of blocks specified by block
         heights.
 
         Args:
             start_height: The block height to start retrieving logs from.
             end_height: The block height to stop retrieving logs from.
             address: An address or list of addresses to filter the logs by.
             topics: A list of topics or nested lists of topics to filter the
                 logs by.
+            step: The maximum number of blocks per request, preventing a single
+                request from requiring too much memory and taking too long.
 
         Returns:
             A list of Log objects parsed from the logs returned by the Geth
             node.
 
         Raises:
             ethhelper.types.GethError: Raised when the Geth node returns an
                 error.
         """
-        if end_height - start_height > 200:
+        if end_height - start_height > step:
             results: list[Log] = []
-            for i in range(start_height, end_height + 1, 201):
-                if i + 200 > end_height:
+            self.logger.info(
+                f"Try to get logs from {start_height} to {end_height}, "
+                f"call per {step} blocks"
+            )
+            for i in range(start_height, end_height + 1, step + 1):
+                if i + step > end_height:
                     results += await self.get_logs_by_blocks(
                         BlockNumber(i), end_height, address, topics
                     )
                 else:
                     results += await self.get_logs_by_blocks(
-                        BlockNumber(i), BlockNumber(i + 200), address, topics
+                        BlockNumber(i), BlockNumber(i + step), address, topics
                     )
             return results
         else:
+            self.logger.info(f"Get logs from {start_height} to {end_height}")
             fliter_params = FilterParams(  # type: ignore
                 address = address,
                 from_block = start_height,  # type: ignore
                 to_block = end_height,  # type: ignore
                 topics = topics
             )
             return await self.get_logs(fliter_params)
@@ -186,42 +194,71 @@
         ts_now = int(datetime.now().timestamp())
         td = ts_now - timestamp
         pos_lower = height_now - (td // 12) - 5
         pos_upper = height_now - (td // 24) + 5
         return await self._binary_search(
             BlockNumber(pos_lower), BlockNumber(pos_upper), timestamp
         )
-    
+
     async def get_blocks_by_numbers(
-        self, start: BlockNumber, end: BlockNumber
+        self, numbers: list[BlockNumber], step: int = 200
     ) -> list[Block]:
         """
         Get the blocks with the given block numbers.
 
         Args:
-            start: The start block number.
-            end: The end block number.
+            numbers: The block numbers.
+            step: The maximum number of blocks per request, preventing a single
+                request from requiring too much memory and taking too long.
 
         Returns:
             A list of ``Block`` instances that represent the blocks with the
             given block numbers.
         """
-        if end - start > 200:
+        if len(numbers) > step:
             results: list[Block] = []
-            for i in range(start, end + 1, 201):
-                if i + 200 > end:
+            self.logger.info(
+                f"Try to get {len(numbers)} blocks, call per {step} blocks"
+            )
+            for i in range(0, len(numbers), step):
+                if i + step > len(numbers):
                     results += await self.get_blocks_by_numbers(
-                        BlockNumber(i), end
+                        numbers[i:]
                     )
+                    self.logger.info("Get blocks process: 100 %")
                 else:
                     results += await self.get_blocks_by_numbers(
-                        BlockNumber(i), BlockNumber(i + 200)
+                        numbers[i:i+step]
+                    )
+                    self.logger.info(
+                        "Get blocks process: "
+                        f"{((i + step)/len(numbers)*100):.2f} %"
                     )
             return results
         else:
             requests: list[tuple[str, list[Any] | None]] = []
-            for i in range(start, end + 1):
-                requests.append(("eth_getBlockByNumber", [hex(i), False]))
+            for number in numbers:
+                requests.append(("eth_getBlockByNumber", [hex(number), False]))
             success, errors = await self.send_multiple(requests)
             if len(errors) != 0:
                 raise GethError(error=[err.error for err in errors])
             return [Block.parse_obj(suc.result) for suc in success]
+
+    async def get_blocks_by_numbers_range(
+        self, start: BlockNumber, end: BlockNumber, step: int = 200
+    ) -> list[Block]:
+        """
+        Get the blocks with the given block numbers range.
+
+        Args:
+            start: The start block number.
+            end: The end block number.
+            step: The maximum number of blocks per request, preventing a single
+                request from requiring too much memory and taking too long.
+
+        Returns:
+            A list of ``Block`` instances that represent the blocks with the
+            given block numbers range.
+        """
+        return await self.get_blocks_by_numbers(
+            [BlockNumber(i) for i in range(start, end + 1, 1)], step
+        )
```

### Comparing `ethhelper-0.3.6/src/ethhelper/connectors/http/eth.py` & `ethhelper-0.4.0/src/ethhelper/connectors/http/eth.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.3.6/src/ethhelper/connectors/http/net.py` & `ethhelper-0.4.0/src/ethhelper/connectors/http/net.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.3.6/src/ethhelper/connectors/http/txpool.py` & `ethhelper-0.4.0/src/ethhelper/connectors/http/txpool.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.3.6/src/ethhelper/connectors/ws/base.py` & `ethhelper-0.4.0/src/ethhelper/connectors/ws/base.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.3.6/src/ethhelper/connectors/ws/block.py` & `ethhelper-0.4.0/src/ethhelper/connectors/ws/block.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.3.6/src/ethhelper/datatypes/base.py` & `ethhelper-0.4.0/src/ethhelper/datatypes/base.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.3.6/src/ethhelper/datatypes/eth.py` & `ethhelper-0.4.0/src/ethhelper/datatypes/eth.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.3.6/src/ethhelper/datatypes/geth.py` & `ethhelper-0.4.0/src/ethhelper/datatypes/geth.py`

 * *Files 4% similar despite different names*

```diff
@@ -112,14 +112,23 @@
             self.code = error.code
             """The error code."""
             self.msg = error.message
             """A description of the error."""
             super().__init__(f"{error.code}: {error.message}")
 
 
+class GethGraphQLError(Exception):
+    """An exception representing an error response from the Geth graphql."""
+    def __init__(self, msgs: list[str], data: dict[str, Any]) -> None:
+        self.msgs = msgs
+        """The error messages."""
+        self.data = data
+        """The data received."""
+        super().__init__("\n".join(msgs))
+
 class GethErrorResponse(BaseModel):
     """A class representing an error response from the Geth client."""
     jsonrpc: str = "2.0"
     """The version of the JSON-RPC protocol."""
     id: int | None
     """The ID of the response, or None if it is a notification."""
     error: GethErrorDetail
```

### Comparing `ethhelper-0.3.6/src/ethhelper/datatypes/txpool.py` & `ethhelper-0.4.0/src/ethhelper/datatypes/txpool.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.3.6/src/ethhelper/types.py` & `ethhelper-0.4.0/src/ethhelper/types.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.3.6/src/ethhelper/utils/convert.py` & `ethhelper-0.4.0/src/ethhelper/utils/convert.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.3.6/setup.py` & `ethhelper-0.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,20 +16,20 @@
 {'': ['*']}
 
 install_requires = \
 ['eth-typing>=3.3.0,<4.0.0',
  'httpx>=0.23.3,<0.24.0',
  'orjson>=3.8.12,<4.0.0',
  'pydantic>=1.10.7,<2.0.0',
- 'web3>=6.3.0,<7.0.0',
+ 'web3>=6.4.0,<7.0.0',
  'websockets>=10.4,<11.0']
 
 setup_kwargs = {
     'name': 'ethhelper',
-    'version': '0.3.6',
+    'version': '0.4.0',
     'description': 'Asynchronous Geth node connection encapsulation based on httpx, websockets and web3.py. Geth node and Ethereum type extension based on pydantic.',
     'long_description': "# ETHHelper\n\n[![Build Status](https://img.shields.io/github/actions/workflow/status/XiaoHuiHui233/ETHHelper/publish.yml)](https://github.com/XiaoHuiHui233/ETHHelper/actions)\n[![Documentation Status](https://readthedocs.org/projects/ethhelper/badge/?version=latest)](https://ethhelper.readthedocs.io/en/latest/?badge=latest)\n![Python Version](https://img.shields.io/pypi/pyversions/ethhelper)\n![Wheel Status](https://img.shields.io/pypi/wheel/ethhelper)\n[![Latest Version](https://img.shields.io/github/v/release/XiaoHuiHui233/ETHHelper)](https://github.com/XiaoHuiHui233/ETHHelper/releases)\n[![License](https://img.shields.io/github/license/XiaoHuiHui233/ETHHelper)](https://github.com/XiaoHuiHui233/ETHHelper/blob/main/LICENSE)\n\nAsynchronous Geth node connection encapsulation based on httpx, websockets and web3.py. Geth node and Ethereum type extension based on pydantic.\n\nQuickstart see [this](https://ethhelper.readthedocs.io/en/latest/quickstart.html).\n\n[中文](docs/README_cn.md) | English\n\n## Usage\n\n### pypi\n\nIf you prefer to use pypi to install this package, you can just run the following command:\n\n```bash\npip install ethhelper\n```\n\n### git\n\nThe project is managed by poetry. If you prefer to use git to install this package, you can use poetry to directly add a reference to the project's build package through git.\n\nThe command is as follow:\n\n```bash\npoetry add git+ssh://git@github.com:XiaoHuiHui233/ETHHelper.git\n```\n\n## Build\n\nYou can use poetry's tools to generate a build of this project (pure Python).\n\nThe command is as follow:\n\n```bash\npoetry build\n```\n\n## Author and License\n\nETHHelper was written by [XiaoHuiHui233](https://github.com/XiaoHuiHui233/), licensed under the Apache 2.0.\n",
     'author': 'XiaoHuiHui233',
     'author_email': '1025184872@qq.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/XiaoHuiHui233/ETHHelper',
```

### Comparing `ethhelper-0.3.6/PKG-INFO` & `ethhelper-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ethhelper
-Version: 0.3.6
+Version: 0.4.0
 Summary: Asynchronous Geth node connection encapsulation based on httpx, websockets and web3.py. Geth node and Ethereum type extension based on pydantic.
 Home-page: https://github.com/XiaoHuiHui233/ETHHelper
 License: Apache-2.0
 Keywords: ethereum,asyncio,geth,pydantic
 Author: XiaoHuiHui233
 Author-email: 1025184872@qq.com
 Requires-Python: >=3.10,<4.0
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: eth-typing (>=3.3.0,<4.0.0)
 Requires-Dist: httpx (>=0.23.3,<0.24.0)
 Requires-Dist: orjson (>=3.8.12,<4.0.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
-Requires-Dist: web3 (>=6.3.0,<7.0.0)
+Requires-Dist: web3 (>=6.4.0,<7.0.0)
 Requires-Dist: websockets (>=10.4,<11.0)
 Project-URL: Repository, https://github.com/XiaoHuiHui233/ETHHelper
 Description-Content-Type: text/markdown
 
 # ETHHelper
 
 [![Build Status](https://img.shields.io/github/actions/workflow/status/XiaoHuiHui233/ETHHelper/publish.yml)](https://github.com/XiaoHuiHui233/ETHHelper/actions)
```

