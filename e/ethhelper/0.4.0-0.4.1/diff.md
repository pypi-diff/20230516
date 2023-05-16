# Comparing `tmp/ethhelper-0.4.0.tar.gz` & `tmp/ethhelper-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ethhelper-0.4.0.tar", max compression
+gzip compressed data, was "ethhelper-0.4.1.tar", max compression
```

## Comparing `ethhelper-0.4.0.tar` & `ethhelper-0.4.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    11357 2023-05-16 10:10:44.942273 ethhelper-0.4.0/LICENSE
--rw-r--r--   0        0        0     1708 2023-05-16 10:10:44.942273 ethhelper-0.4.0/README.md
--rw-r--r--   0        0        0     2155 2023-05-16 10:10:44.946274 ethhelper-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      174 2023-05-16 10:10:44.946274 ethhelper-0.4.0/src/ethhelper/__init__.py
--rw-r--r--   0        0        0        0 2023-05-16 10:10:44.946274 ethhelper-0.4.0/src/ethhelper/connectors/__init__.py
--rw-r--r--   0        0        0     1966 2023-05-16 10:10:44.946274 ethhelper-0.4.0/src/ethhelper/connectors/http/__init__.py
--rw-r--r--   0        0        0    13216 2023-05-16 10:10:44.946274 ethhelper-0.4.0/src/ethhelper/connectors/http/base.py
--rw-r--r--   0        0        0     9327 2023-05-16 10:10:44.946274 ethhelper-0.4.0/src/ethhelper/connectors/http/custom.py
--rw-r--r--   0        0        0    16281 2023-05-16 10:10:44.946274 ethhelper-0.4.0/src/ethhelper/connectors/http/eth.py
--rw-r--r--   0        0        0     5175 2023-05-16 10:10:44.946274 ethhelper-0.4.0/src/ethhelper/connectors/http/graphql.py
--rw-r--r--   0        0        0     1743 2023-05-16 10:10:44.946274 ethhelper-0.4.0/src/ethhelper/connectors/http/net.py
--rw-r--r--   0        0        0     3958 2023-05-16 10:10:44.946274 ethhelper-0.4.0/src/ethhelper/connectors/http/txpool.py
--rw-r--r--   0        0        0      159 2023-05-16 10:10:44.946274 ethhelper-0.4.0/src/ethhelper/connectors/ws/__init__.py
--rw-r--r--   0        0        0     5912 2023-05-16 10:10:44.946274 ethhelper-0.4.0/src/ethhelper/connectors/ws/base.py
--rw-r--r--   0        0        0     3505 2023-05-16 10:10:44.946274 ethhelper-0.4.0/src/ethhelper/connectors/ws/block.py
--rw-r--r--   0        0        0        0 2023-05-16 10:10:44.946274 ethhelper-0.4.0/src/ethhelper/datatypes/__init__.py
--rw-r--r--   0        0        0     7579 2023-05-16 10:10:44.946274 ethhelper-0.4.0/src/ethhelper/datatypes/base.py
--rw-r--r--   0        0        0    17501 2023-05-16 10:10:44.946274 ethhelper-0.4.0/src/ethhelper/datatypes/eth.py
--rw-r--r--   0        0        0     7167 2023-05-16 10:10:44.946274 ethhelper-0.4.0/src/ethhelper/datatypes/geth.py
--rw-r--r--   0        0        0     5135 2023-05-16 10:10:44.946274 ethhelper-0.4.0/src/ethhelper/datatypes/txpool.py
--rw-r--r--   0        0        0        0 2023-05-16 10:10:44.946274 ethhelper-0.4.0/src/ethhelper/py.typed
--rw-r--r--   0        0        0     1387 2023-05-16 10:10:44.946274 ethhelper-0.4.0/src/ethhelper/types.py
--rw-r--r--   0        0        0        0 2023-05-16 10:10:44.946274 ethhelper-0.4.0/src/ethhelper/utils/__init__.py
--rw-r--r--   0        0        0      927 2023-05-16 10:10:44.946274 ethhelper-0.4.0/src/ethhelper/utils/convert.py
--rw-r--r--   0        0        0      498 2023-05-16 10:10:44.946274 ethhelper-0.4.0/src/ethhelper/utils/json.py
--rw-r--r--   0        0        0     2851 1970-01-01 00:00:00.000000 ethhelper-0.4.0/setup.py
--rw-r--r--   0        0        0     2679 1970-01-01 00:00:00.000000 ethhelper-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-16 15:58:36.193240 ethhelper-0.4.1/LICENSE
+-rw-r--r--   0        0        0     1708 2023-05-16 15:58:36.193240 ethhelper-0.4.1/README.md
+-rw-r--r--   0        0        0     2155 2023-05-16 15:58:36.197240 ethhelper-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      174 2023-05-16 15:58:36.197240 ethhelper-0.4.1/src/ethhelper/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-16 15:58:36.197240 ethhelper-0.4.1/src/ethhelper/connectors/__init__.py
+-rw-r--r--   0        0        0     1966 2023-05-16 15:58:36.197240 ethhelper-0.4.1/src/ethhelper/connectors/http/__init__.py
+-rw-r--r--   0        0        0    13216 2023-05-16 15:58:36.197240 ethhelper-0.4.1/src/ethhelper/connectors/http/base.py
+-rw-r--r--   0        0        0     8944 2023-05-16 15:58:36.197240 ethhelper-0.4.1/src/ethhelper/connectors/http/custom.py
+-rw-r--r--   0        0        0    16281 2023-05-16 15:58:36.197240 ethhelper-0.4.1/src/ethhelper/connectors/http/eth.py
+-rw-r--r--   0        0        0     5175 2023-05-16 15:58:36.197240 ethhelper-0.4.1/src/ethhelper/connectors/http/graphql.py
+-rw-r--r--   0        0        0     1743 2023-05-16 15:58:36.197240 ethhelper-0.4.1/src/ethhelper/connectors/http/net.py
+-rw-r--r--   0        0        0     3958 2023-05-16 15:58:36.197240 ethhelper-0.4.1/src/ethhelper/connectors/http/txpool.py
+-rw-r--r--   0        0        0      159 2023-05-16 15:58:36.197240 ethhelper-0.4.1/src/ethhelper/connectors/ws/__init__.py
+-rw-r--r--   0        0        0     5912 2023-05-16 15:58:36.197240 ethhelper-0.4.1/src/ethhelper/connectors/ws/base.py
+-rw-r--r--   0        0        0     3505 2023-05-16 15:58:36.197240 ethhelper-0.4.1/src/ethhelper/connectors/ws/block.py
+-rw-r--r--   0        0        0        0 2023-05-16 15:58:36.197240 ethhelper-0.4.1/src/ethhelper/datatypes/__init__.py
+-rw-r--r--   0        0        0     7579 2023-05-16 15:58:36.197240 ethhelper-0.4.1/src/ethhelper/datatypes/base.py
+-rw-r--r--   0        0        0    17501 2023-05-16 15:58:36.197240 ethhelper-0.4.1/src/ethhelper/datatypes/eth.py
+-rw-r--r--   0        0        0     7167 2023-05-16 15:58:36.197240 ethhelper-0.4.1/src/ethhelper/datatypes/geth.py
+-rw-r--r--   0        0        0     5135 2023-05-16 15:58:36.197240 ethhelper-0.4.1/src/ethhelper/datatypes/txpool.py
+-rw-r--r--   0        0        0        0 2023-05-16 15:58:36.197240 ethhelper-0.4.1/src/ethhelper/py.typed
+-rw-r--r--   0        0        0     1433 2023-05-16 15:58:36.197240 ethhelper-0.4.1/src/ethhelper/types.py
+-rw-r--r--   0        0        0        0 2023-05-16 15:58:36.197240 ethhelper-0.4.1/src/ethhelper/utils/__init__.py
+-rw-r--r--   0        0        0      927 2023-05-16 15:58:36.197240 ethhelper-0.4.1/src/ethhelper/utils/convert.py
+-rw-r--r--   0        0        0      498 2023-05-16 15:58:36.197240 ethhelper-0.4.1/src/ethhelper/utils/json.py
+-rw-r--r--   0        0        0     2851 1970-01-01 00:00:00.000000 ethhelper-0.4.1/setup.py
+-rw-r--r--   0        0        0     2679 1970-01-01 00:00:00.000000 ethhelper-0.4.1/PKG-INFO
```

### Comparing `ethhelper-0.4.0/LICENSE` & `ethhelper-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ethhelper-0.4.0/README.md` & `ethhelper-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `ethhelper-0.4.0/pyproject.toml` & `ethhelper-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "ethhelper"
-version = "0.4.0"
+version = "0.4.1"
 description = "Asynchronous Geth node connection encapsulation based on httpx, websockets and web3.py. Geth node and Ethereum type extension based on pydantic."
 authors = ["XiaoHuiHui233 <1025184872@qq.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/XiaoHuiHui233/ETHHelper"
 keywords = ["ethereum", "asyncio", "geth", "pydantic"]
```

### Comparing `ethhelper-0.4.0/src/ethhelper/connectors/http/__init__.py` & `ethhelper-0.4.1/src/ethhelper/connectors/http/__init__.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.4.0/src/ethhelper/connectors/http/base.py` & `ethhelper-0.4.1/src/ethhelper/connectors/http/base.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.4.0/src/ethhelper/connectors/http/custom.py` & `ethhelper-0.4.1/src/ethhelper/connectors/http/custom.py`

 * *Files 3% similar despite different names*

```diff
@@ -124,22 +124,21 @@
         if end_height - start_height > step:
             results: list[Log] = []
             self.logger.info(
                 f"Try to get logs from {start_height} to {end_height}, "
                 f"call per {step} blocks"
             )
             for i in range(start_height, end_height + 1, step + 1):
-                if i + step > end_height:
-                    results += await self.get_logs_by_blocks(
-                        BlockNumber(i), end_height, address, topics
-                    )
-                else:
-                    results += await self.get_logs_by_blocks(
-                        BlockNumber(i), BlockNumber(i + step), address, topics
-                    )
+                results += await self.get_logs_by_blocks(
+                    BlockNumber(i),
+                    BlockNumber(min(end_height, i + step)),
+                    address,
+                    topics,
+                    step
+                )
             return results
         else:
             self.logger.info(f"Get logs from {start_height} to {end_height}")
             fliter_params = FilterParams(  # type: ignore
                 address = address,
                 from_block = start_height,  # type: ignore
                 to_block = end_height,  # type: ignore
@@ -216,27 +215,21 @@
         """
         if len(numbers) > step:
             results: list[Block] = []
             self.logger.info(
                 f"Try to get {len(numbers)} blocks, call per {step} blocks"
             )
             for i in range(0, len(numbers), step):
-                if i + step > len(numbers):
-                    results += await self.get_blocks_by_numbers(
-                        numbers[i:]
-                    )
-                    self.logger.info("Get blocks process: 100 %")
-                else:
-                    results += await self.get_blocks_by_numbers(
-                        numbers[i:i+step]
-                    )
-                    self.logger.info(
-                        "Get blocks process: "
-                        f"{((i + step)/len(numbers)*100):.2f} %"
-                    )
+                results += await self.get_blocks_by_numbers(
+                    numbers[i:min(i+step, len(numbers))], step
+                )
+                self.logger.info(
+                    "Get blocks process: "
+                    f"{((i + step)/len(numbers)*100):.2f} %"
+                )
             return results
         else:
             requests: list[tuple[str, list[Any] | None]] = []
             for number in numbers:
                 requests.append(("eth_getBlockByNumber", [hex(number), False]))
             success, errors = await self.send_multiple(requests)
             if len(errors) != 0:
```

### Comparing `ethhelper-0.4.0/src/ethhelper/connectors/http/eth.py` & `ethhelper-0.4.1/src/ethhelper/connectors/http/eth.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.4.0/src/ethhelper/connectors/http/graphql.py` & `ethhelper-0.4.1/src/ethhelper/connectors/http/graphql.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.4.0/src/ethhelper/connectors/http/net.py` & `ethhelper-0.4.1/src/ethhelper/connectors/http/net.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.4.0/src/ethhelper/connectors/http/txpool.py` & `ethhelper-0.4.1/src/ethhelper/connectors/http/txpool.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.4.0/src/ethhelper/connectors/ws/base.py` & `ethhelper-0.4.1/src/ethhelper/connectors/ws/base.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.4.0/src/ethhelper/connectors/ws/block.py` & `ethhelper-0.4.1/src/ethhelper/connectors/ws/block.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.4.0/src/ethhelper/datatypes/base.py` & `ethhelper-0.4.1/src/ethhelper/datatypes/base.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.4.0/src/ethhelper/datatypes/eth.py` & `ethhelper-0.4.1/src/ethhelper/datatypes/eth.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.4.0/src/ethhelper/datatypes/geth.py` & `ethhelper-0.4.1/src/ethhelper/datatypes/geth.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.4.0/src/ethhelper/datatypes/txpool.py` & `ethhelper-0.4.1/src/ethhelper/datatypes/txpool.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.4.0/src/ethhelper/types.py` & `ethhelper-0.4.1/src/ethhelper/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 )
 from .datatypes.geth import (
     CallOverride,
     CallOverrideParams,
     GethError,
     GethErrorDetail,
     GethErrorResponse,
+    GethGraphQLError,
     GethIsDead,
     GethRequest,
     GethResponse,
     GethSuccessResponse,
     GethWSItem,
     GethWSResponse,
     IdNotMatch,
@@ -61,14 +62,15 @@
     "Receipt",
     "FilterParams",
     "CallOverride",
     "CallOverrideParams",
     "GethError",
     "GethErrorDetail",
     "GethErrorResponse",
+    "GethGraphQLError",
     "GethIsDead",
     "GethRequest",
     "GethResponse",
     "GethSuccessResponse",
     "GethWSItem",
     "GethWSResponse",
     "IdNotMatch",
```

### Comparing `ethhelper-0.4.0/src/ethhelper/utils/convert.py` & `ethhelper-0.4.1/src/ethhelper/utils/convert.py`

 * *Files identical despite different names*

### Comparing `ethhelper-0.4.0/setup.py` & `ethhelper-0.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
  'orjson>=3.8.12,<4.0.0',
  'pydantic>=1.10.7,<2.0.0',
  'web3>=6.4.0,<7.0.0',
  'websockets>=10.4,<11.0']
 
 setup_kwargs = {
     'name': 'ethhelper',
-    'version': '0.4.0',
+    'version': '0.4.1',
     'description': 'Asynchronous Geth node connection encapsulation based on httpx, websockets and web3.py. Geth node and Ethereum type extension based on pydantic.',
     'long_description': "# ETHHelper\n\n[![Build Status](https://img.shields.io/github/actions/workflow/status/XiaoHuiHui233/ETHHelper/publish.yml)](https://github.com/XiaoHuiHui233/ETHHelper/actions)\n[![Documentation Status](https://readthedocs.org/projects/ethhelper/badge/?version=latest)](https://ethhelper.readthedocs.io/en/latest/?badge=latest)\n![Python Version](https://img.shields.io/pypi/pyversions/ethhelper)\n![Wheel Status](https://img.shields.io/pypi/wheel/ethhelper)\n[![Latest Version](https://img.shields.io/github/v/release/XiaoHuiHui233/ETHHelper)](https://github.com/XiaoHuiHui233/ETHHelper/releases)\n[![License](https://img.shields.io/github/license/XiaoHuiHui233/ETHHelper)](https://github.com/XiaoHuiHui233/ETHHelper/blob/main/LICENSE)\n\nAsynchronous Geth node connection encapsulation based on httpx, websockets and web3.py. Geth node and Ethereum type extension based on pydantic.\n\nQuickstart see [this](https://ethhelper.readthedocs.io/en/latest/quickstart.html).\n\n[中文](docs/README_cn.md) | English\n\n## Usage\n\n### pypi\n\nIf you prefer to use pypi to install this package, you can just run the following command:\n\n```bash\npip install ethhelper\n```\n\n### git\n\nThe project is managed by poetry. If you prefer to use git to install this package, you can use poetry to directly add a reference to the project's build package through git.\n\nThe command is as follow:\n\n```bash\npoetry add git+ssh://git@github.com:XiaoHuiHui233/ETHHelper.git\n```\n\n## Build\n\nYou can use poetry's tools to generate a build of this project (pure Python).\n\nThe command is as follow:\n\n```bash\npoetry build\n```\n\n## Author and License\n\nETHHelper was written by [XiaoHuiHui233](https://github.com/XiaoHuiHui233/), licensed under the Apache 2.0.\n",
     'author': 'XiaoHuiHui233',
     'author_email': '1025184872@qq.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/XiaoHuiHui233/ETHHelper',
```

### Comparing `ethhelper-0.4.0/PKG-INFO` & `ethhelper-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ethhelper
-Version: 0.4.0
+Version: 0.4.1
 Summary: Asynchronous Geth node connection encapsulation based on httpx, websockets and web3.py. Geth node and Ethereum type extension based on pydantic.
 Home-page: https://github.com/XiaoHuiHui233/ETHHelper
 License: Apache-2.0
 Keywords: ethereum,asyncio,geth,pydantic
 Author: XiaoHuiHui233
 Author-email: 1025184872@qq.com
 Requires-Python: >=3.10,<4.0
```

