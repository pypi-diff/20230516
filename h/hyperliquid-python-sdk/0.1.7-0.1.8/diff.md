# Comparing `tmp/hyperliquid_python_sdk-0.1.7.tar.gz` & `tmp/hyperliquid_python_sdk-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperliquid_python_sdk-0.1.7.tar", max compression
+gzip compressed data, was "hyperliquid_python_sdk-0.1.8.tar", max compression
```

## Comparing `hyperliquid_python_sdk-0.1.7.tar` & `hyperliquid_python_sdk-0.1.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1083 2023-04-14 18:01:14.091628 hyperliquid_python_sdk-0.1.7/LICENSE.md
--rw-r--r--   0        0        0     5727 2023-04-14 18:01:14.101353 hyperliquid_python_sdk-0.1.7/README.md
--rw-r--r--   0        0        0        0 2023-04-14 18:01:14.086502 hyperliquid_python_sdk-0.1.7/hyperliquid/__init__.py
--rw-r--r--   0        0        0     1677 2023-04-14 18:01:14.090826 hyperliquid_python_sdk-0.1.7/hyperliquid/api.py
--rw-r--r--   0        0        0     3148 2023-04-14 18:01:14.086377 hyperliquid_python_sdk-0.1.7/hyperliquid/exchange.py
--rw-r--r--   0        0        0     4938 2023-04-14 18:01:14.091061 hyperliquid_python_sdk-0.1.7/hyperliquid/info.py
--rw-r--r--   0        0        0        0 2023-04-14 18:01:14.087711 hyperliquid_python_sdk-0.1.7/hyperliquid/utils/__init__.py
--rw-r--r--   0        0        0      144 2023-04-14 18:01:14.087641 hyperliquid_python_sdk-0.1.7/hyperliquid/utils/constants.py
--rw-r--r--   0        0        0      479 2023-04-14 18:01:14.087371 hyperliquid_python_sdk-0.1.7/hyperliquid/utils/error.py
--rw-r--r--   0        0        0     4927 2023-04-14 18:01:14.087022 hyperliquid_python_sdk-0.1.7/hyperliquid/utils/signing.py
--rw-r--r--   0        0        0     2174 2023-04-14 18:01:14.087870 hyperliquid_python_sdk-0.1.7/hyperliquid/utils/types.py
--rw-r--r--   0        0        0     4690 2023-04-14 18:01:14.091374 hyperliquid_python_sdk-0.1.7/hyperliquid/websocket_manager.py
--rw-r--r--   0        0        0     3838 2023-04-14 18:04:41.692184 hyperliquid_python_sdk-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     7315 1970-01-01 00:00:00.000000 hyperliquid_python_sdk-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-05-16 01:06:14.480083 hyperliquid_python_sdk-0.1.8/LICENSE.md
+-rw-r--r--   0        0        0     5741 2023-05-16 01:06:14.495874 hyperliquid_python_sdk-0.1.8/README.md
+-rw-r--r--   0        0        0        0 2023-05-16 01:06:14.471293 hyperliquid_python_sdk-0.1.8/hyperliquid/__init__.py
+-rw-r--r--   0        0        0     1677 2023-05-16 01:06:14.479107 hyperliquid_python_sdk-0.1.8/hyperliquid/api.py
+-rw-r--r--   0        0        0     4557 2023-05-16 01:06:14.471030 hyperliquid_python_sdk-0.1.8/hyperliquid/exchange.py
+-rw-r--r--   0        0        0     4938 2023-05-16 01:06:14.479409 hyperliquid_python_sdk-0.1.8/hyperliquid/info.py
+-rw-r--r--   0        0        0        0 2023-05-16 01:06:14.473421 hyperliquid_python_sdk-0.1.8/hyperliquid/utils/__init__.py
+-rw-r--r--   0        0        0      144 2023-05-16 01:06:14.473252 hyperliquid_python_sdk-0.1.8/hyperliquid/utils/constants.py
+-rw-r--r--   0        0        0      479 2023-05-16 01:06:14.472868 hyperliquid_python_sdk-0.1.8/hyperliquid/utils/error.py
+-rw-r--r--   0        0        0     5070 2023-05-16 01:06:14.472421 hyperliquid_python_sdk-0.1.8/hyperliquid/utils/signing.py
+-rw-r--r--   0        0        0     2174 2023-05-16 01:06:14.473857 hyperliquid_python_sdk-0.1.8/hyperliquid/utils/types.py
+-rw-r--r--   0        0        0     4691 2023-05-16 01:06:14.479757 hyperliquid_python_sdk-0.1.8/hyperliquid/websocket_manager.py
+-rw-r--r--   0        0        0     3859 2023-05-16 01:06:14.490743 hyperliquid_python_sdk-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     7371 1970-01-01 00:00:00.000000 hyperliquid_python_sdk-0.1.8/PKG-INFO
```

### Comparing `hyperliquid_python_sdk-0.1.7/LICENSE.md` & `hyperliquid_python_sdk-0.1.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hyperliquid_python_sdk-0.1.7/README.md` & `hyperliquid_python_sdk-0.1.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 See [examples](examples) for more complete examples. You can also checkout the repo and run any of the examples after configuring your private key e.g. 
 ```bash
 cp examples/config.json.example examples/config.json
 vim examples/config.json
 python examples/basic_order.py
 ```
 
-## Getting started with development
+## Getting started with contributing to this repo
 
 1. Download `Poetry`: https://python-poetry.org/. Note that in the install script you might have to set `symlinks=True` in `venv.EnvBuilder`.
 
 2. Point poetry to correct version of python. For development we require python 3.10 exactly. Some dependencies have issues on 3.11, while older versions don't have correct typing support.
 `brew install python@3.10 && poetry env use /opt/homebrew/Cellar/python@3.10/3.10.10_1/bin/python3.10`
 
 3. Install dependencies:
```

### Comparing `hyperliquid_python_sdk-0.1.7/hyperliquid/api.py` & `hyperliquid_python_sdk-0.1.8/hyperliquid/api.py`

 * *Files identical despite different names*

### Comparing `hyperliquid_python_sdk-0.1.7/hyperliquid/exchange.py` & `hyperliquid_python_sdk-0.1.8/hyperliquid/exchange.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import logging
 
 from eth_account.signers.local import LocalAccount
 
 from hyperliquid.api import API
 from hyperliquid.info import Info
 from hyperliquid.utils.signing import (
-    OrderSpec,
-    order_spec_preprocessing,
-    order_grouping_to_number,
-    sign_l1_action,
     ZERO_ADDRESS,
+    OrderSpec,
     OrderType,
-    order_spec_to_order_wire,
+    float_to_usd_int,
     get_timestamp_ms,
+    order_grouping_to_number,
+    order_spec_preprocessing,
+    order_spec_to_order_wire,
+    sign_l1_action,
 )
-from hyperliquid.utils.types import Meta, Any, Literal, Optional
+from hyperliquid.utils.types import Any, Literal, Meta, Optional
 
 
 class Exchange(API):
     def __init__(
         self,
         wallet: LocalAccount,
         base_url: Optional[str] = None,
@@ -31,14 +32,24 @@
         if meta is None:
             info = Info(base_url, skip_ws=True)
             self.meta = info.meta()
         else:
             self.meta = meta
         self.coin_to_asset = {asset_info["name"]: asset for (asset, asset_info) in enumerate(self.meta["universe"])}
 
+    def _post_action(self, action, signature, nonce):
+        payload = {
+            "action": action,
+            "nonce": nonce,
+            "signature": signature,
+            "vaultAddress": self.vault_address,
+        }
+        logging.debug(payload)
+        return self.post("/exchange", payload)
+
     def order(
         self, coin: str, is_buy: bool, sz: float, limit_px: float, order_type: OrderType, reduce_only: bool = False
     ) -> Any:
         order_spec: OrderSpec = {
             "order": {
                 "asset": self.coin_to_asset[coin],
                 "isBuy": is_buy,
@@ -54,47 +65,84 @@
         signature = sign_l1_action(
             self.wallet,
             ["(uint32,bool,uint64,uint64,bool,uint8,uint64)[]", "uint8"],
             [[order_spec_preprocessing(order_spec)], order_grouping_to_number(grouping)],
             ZERO_ADDRESS if self.vault_address is None else self.vault_address,
             timestamp,
         )
-        payload = {
-            "action": {
+
+        return self._post_action(
+            {
                 "type": "order",
                 "grouping": grouping,
                 "orders": [order_spec_to_order_wire(order_spec)],
             },
-            "nonce": timestamp,
-            "signature": signature,
-            "vaultAddress": self.vault_address,
-        }
-        logging.debug(payload)
-        return self.post("/exchange", payload)
+            signature,
+            timestamp,
+        )
 
     def cancel(self, coin: str, oid: int) -> Any:
         timestamp = get_timestamp_ms()
         asset = self.coin_to_asset[coin]
         signature = sign_l1_action(
             self.wallet,
             ["(uint32,uint64)[]"],
             [[(asset, oid)]],
             ZERO_ADDRESS if self.vault_address is None else self.vault_address,
             timestamp,
         )
-        return self.post(
-            "/exchange",
+        return self._post_action(
+            {
+                "type": "cancel",
+                "cancels": [
+                    {
+                        "asset": asset,
+                        "oid": oid,
+                    }
+                ],
+            },
+            signature,
+            timestamp,
+        )
+
+    def update_leverage(self, leverage: int, coin: str, is_cross: bool = True) -> Any:
+        timestamp = get_timestamp_ms()
+        asset = self.coin_to_asset[coin]
+        signature = sign_l1_action(
+            self.wallet,
+            ["uint32", "bool", "uint32"],
+            [asset, is_cross, leverage],
+            ZERO_ADDRESS if self.vault_address is None else self.vault_address,
+            timestamp,
+        )
+        return self._post_action(
             {
-                "action": {
-                    "type": "cancel",
-                    "cancels": [
-                        {
-                            "asset": asset,
-                            "oid": oid,
-                        }
-                    ],
-                },
-                "nonce": timestamp,
-                "signature": signature,
-                "vaultAddress": self.vault_address,
+                "type": "updateLeverage",
+                "asset": asset,
+                "isCross": is_cross,
+                "leverage": leverage,
             },
+            signature,
+            timestamp,
+        )
+
+    def update_isolated_margin(self, amount: float, coin: str) -> Any:
+        timestamp = get_timestamp_ms()
+        asset = self.coin_to_asset[coin]
+        amount = float_to_usd_int(amount)
+        signature = sign_l1_action(
+            self.wallet,
+            ["uint32", "bool", "int64"],
+            [asset, True, amount],
+            ZERO_ADDRESS if self.vault_address is None else self.vault_address,
+            timestamp,
+        )
+        return self._post_action(
+            {
+                "type": "updateIsolatedMargin",
+                "asset": asset,
+                "isBuy": True,
+                "ntli": amount,
+            },
+            signature,
+            timestamp,
         )
```

### Comparing `hyperliquid_python_sdk-0.1.7/hyperliquid/info.py` & `hyperliquid_python_sdk-0.1.8/hyperliquid/info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from hyperliquid.api import API
-from hyperliquid.utils.types import Meta, Subscription, Any, cast, Callable
+from hyperliquid.utils.types import Any, Callable, Meta, Subscription, cast
 from hyperliquid.websocket_manager import WebsocketManager
 
 
 class Info(API):
     def __init__(self, base_url=None, skip_ws=False):
         super().__init__(base_url)
         if not skip_ws:
```

### Comparing `hyperliquid_python_sdk-0.1.7/hyperliquid/utils/signing.py` & `hyperliquid_python_sdk-0.1.8/hyperliquid/utils/signing.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import time
+
 from eth_abi import encode
 from eth_account.messages import encode_structured_data
 from eth_utils import keccak, to_hex
 
-from hyperliquid.utils.types import TypedDict, Literal, Union, Any, Tuple
+from hyperliquid.utils.types import Any, Literal, Tuple, TypedDict, Union
 
 ZERO_ADDRESS = "0x0000000000000000000000000000000000000000"
 
 Tif = Union[Literal["Alo"], Literal["Ioc"], Literal["Gtc"]]
 Tpsl = Union[Literal["tp"], Literal["sl"]]
 LimitOrderType = TypedDict("LimitOrderType", {"tif": Tif})
 TriggerOrderType = TypedDict("TriggerOrderType", {"triggerPx": int, "isMarket": bool, "tpsl": Tpsl})
@@ -133,15 +134,23 @@
     rounded = "{:.8f}".format(x)
     if abs(float(rounded) - x) >= 1e-12:
         raise ValueError("float_to_wire causes rounding", x)
     return rounded
 
 
 def float_to_int_for_hashing(x: float) -> int:
-    with_decimals = x * 10**8
+    return float_to_int(x, 8)
+
+
+def float_to_usd_int(x: float) -> int:
+    return float_to_int(x, 6)
+
+
+def float_to_int(x: float, power: int) -> int:
+    with_decimals = x * 10**power
     if abs(round(with_decimals) - with_decimals) >= 1e-4:
-        raise ValueError("float_to_int_for_hashing causes rounding", x)
+        raise ValueError("float_to_int causes rounding", x)
     return round(with_decimals)
 
 
 def get_timestamp_ms() -> int:
     return int(time.time() * 1000)
```

### Comparing `hyperliquid_python_sdk-0.1.7/hyperliquid/utils/types.py` & `hyperliquid_python_sdk-0.1.8/hyperliquid/utils/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sys
 
 if sys.version_info >= (3, 8):
-    from typing import TypedDict, Literal
+    from typing import Literal, TypedDict
 else:
     from typing_extensions import TypedDict, Literal
 
-from typing import List, Union, Dict, Tuple, Any, Optional, cast, Callable, NamedTuple
+from typing import Any, Callable, Dict, List, NamedTuple, Optional, Tuple, Union, cast
 
 Any = Any
 Option = Optional
 cast = cast
 Callable = Callable
 NamedTuple = NamedTuple
```

### Comparing `hyperliquid_python_sdk-0.1.7/hyperliquid/websocket_manager.py` & `hyperliquid_python_sdk-0.1.8/hyperliquid/websocket_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-import logging
-from collections import defaultdict
 import json
+import logging
 import threading
+from collections import defaultdict
+
 import websocket
 
-from hyperliquid.utils.types import Subscription, WsMsg, Callable, Any, NamedTuple, Optional, List, Tuple, Dict
+from hyperliquid.utils.types import Any, Callable, Dict, List, NamedTuple, Optional, Subscription, Tuple, WsMsg
 
 ActiveSubscription = NamedTuple("ActiveSubscription", [("callback", Callable[[Any], None]), ("subscription_id", int)])
 
 
 def subscription_to_identifier(subscription: Subscription) -> str:
     if subscription["type"] == "allMids":
         return "allMids"
```

### Comparing `hyperliquid_python_sdk-0.1.7/pyproject.toml` & `hyperliquid_python_sdk-0.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "hyperliquid-python-sdk"
-version = "0.1.7"
+version = "0.1.8"
 description = "SDK for Hyperliquid API trading with Python."
 readme = "README.md"
 authors = ["Hyperliquid <hello@hyperliquid.xyz>"]
 license = "MIT"
 repository = "https://github.com/hyperliquid-dex/hyperliquid-python-sdk"
 homepage = "https://github.com/hyperliquid-dex/hyperliquid-python-sdk"
 packages = [
@@ -43,14 +43,15 @@
 rich = "^10.14.0"
 pytest-vcr = "^1.0.2"
 pytest-cov = "^4.0.0"
 eth-utils = "^2.1.0"
 eth-abi = "^3.0.1"
 eth-account = "^0.8.0"
 websocket-client = "^1.5.1"
+requests = "^2.28.2"
 
 [tool.poetry.dev-dependencies]
 python = "3.10.10"
 bandit = "^1.7.1"
 black = "^22.3.0"
 darglint = "^1.8.1"
 isort = {extras = ["colors"], version = "^5.10.1"}
```

### Comparing `hyperliquid_python_sdk-0.1.7/PKG-INFO` & `hyperliquid_python_sdk-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperliquid-python-sdk
-Version: 0.1.7
+Version: 0.1.8
 Summary: SDK for Hyperliquid API trading with Python.
 Home-page: https://github.com/hyperliquid-dex/hyperliquid-python-sdk
 License: MIT
 Author: Hyperliquid
 Author-email: hello@hyperliquid.xyz
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -24,14 +24,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: eth-abi (>=3.0.1,<4.0.0)
 Requires-Dist: eth-account (>=0.8.0,<0.9.0)
 Requires-Dist: eth-utils (>=2.1.0,<3.0.0)
 Requires-Dist: importlib_metadata (>=4.5.0,<5.0.0) ; python_version < "3.8"
 Requires-Dist: pytest-cov (>=4.0.0,<5.0.0)
 Requires-Dist: pytest-vcr (>=1.0.2,<2.0.0)
+Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: rich (>=10.14.0,<11.0.0)
 Requires-Dist: typer[all] (>=0.4.0,<0.5.0)
 Requires-Dist: websocket-client (>=1.5.1,<2.0.0)
 Project-URL: Repository, https://github.com/hyperliquid-dex/hyperliquid-python-sdk
 Description-Content-Type: text/markdown
 
 # hyperliquid-python-sdk
@@ -67,15 +68,15 @@
 See [examples](examples) for more complete examples. You can also checkout the repo and run any of the examples after configuring your private key e.g. 
 ```bash
 cp examples/config.json.example examples/config.json
 vim examples/config.json
 python examples/basic_order.py
 ```
 
-## Getting started with development
+## Getting started with contributing to this repo
 
 1. Download `Poetry`: https://python-poetry.org/. Note that in the install script you might have to set `symlinks=True` in `venv.EnvBuilder`.
 
 2. Point poetry to correct version of python. For development we require python 3.10 exactly. Some dependencies have issues on 3.11, while older versions don't have correct typing support.
 `brew install python@3.10 && poetry env use /opt/homebrew/Cellar/python@3.10/3.10.10_1/bin/python3.10`
 
 3. Install dependencies:
```

