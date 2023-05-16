# Comparing `tmp/dexie_rewards-0.0.6.tar.gz` & `tmp/dexie_rewards-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dexie_rewards-0.0.6.tar", max compression
+gzip compressed data, was "dexie_rewards-0.0.7.tar", max compression
```

## Comparing `dexie_rewards-0.0.6.tar` & `dexie_rewards-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    11357 2023-05-02 08:44:23.355168 dexie_rewards-0.0.6/LICENSE
--rw-r--r--   0        0        0    12145 2023-05-13 02:37:26.609073 dexie_rewards-0.0.6/README.md
--rw-r--r--   0        0        0      768 2023-05-13 04:22:25.624481 dexie_rewards-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      219 2023-05-04 04:23:21.607369 dexie_rewards-0.0.6/src/dexie_rewards/__init__.py
--rw-r--r--   0        0        0     1126 2023-05-13 02:26:45.947358 dexie_rewards-0.0.6/src/dexie_rewards/config.py
--rw-r--r--   0        0        0      822 2023-05-12 12:18:23.796037 dexie_rewards-0.0.6/src/dexie_rewards/decorators/with_db_connection.py
--rw-r--r--   0        0        0     1207 2023-05-11 04:12:56.210275 dexie_rewards-0.0.6/src/dexie_rewards/decorators/with_wallet_rpc_client.py
--rw-r--r--   0        0        0      234 2023-05-08 10:51:08.009870 dexie_rewards-0.0.6/src/dexie_rewards/main.py
--rw-r--r--   0        0        0     3505 2023-05-13 03:54:19.525074 dexie_rewards-0.0.6/src/dexie_rewards/rewards/claim.py
--rw-r--r--   0        0        0     1921 2023-05-13 03:55:02.188725 dexie_rewards-0.0.6/src/dexie_rewards/rewards/list.py
--rw-r--r--   0        0        0      272 2023-05-08 10:18:31.545940 dexie_rewards-0.0.6/src/dexie_rewards/rewards/main.py
--rw-r--r--   0        0        0     4797 2023-05-13 04:16:40.726557 dexie_rewards-0.0.6/src/dexie_rewards/rewards/utils.py
--rw-r--r--   0        0        0     2292 2023-05-09 13:07:18.656197 dexie_rewards-0.0.6/src/dexie_rewards/services/dexie_api.py
--rw-r--r--   0        0        0     3756 2023-05-13 03:51:52.828154 dexie_rewards-0.0.6/src/dexie_rewards/services/dexie_db.py
--rw-r--r--   0        0        0     1713 2023-05-11 04:36:56.173403 dexie_rewards-0.0.6/src/dexie_rewards/services/wallet_rpc_client.py
--rw-r--r--   0        0        0      911 2023-05-09 07:34:28.541774 dexie_rewards-0.0.6/src/dexie_rewards/types/offer_reward.py
--rw-r--r--   0        0        0      229 2023-05-09 11:06:14.984159 dexie_rewards-0.0.6/src/dexie_rewards/types/utils.py
--rw-r--r--   0        0        0     1851 2023-05-12 13:28:19.018840 dexie_rewards-0.0.6/src/dexie_rewards/utils.py
--rw-r--r--   0        0        0    12900 1970-01-01 00:00:00.000000 dexie_rewards-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-02 08:44:23.355168 dexie_rewards-0.0.7/LICENSE
+-rw-r--r--   0        0        0    12037 2023-05-16 00:41:25.101677 dexie_rewards-0.0.7/README.md
+-rw-r--r--   0        0        0      768 2023-05-16 01:44:16.901401 dexie_rewards-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      219 2023-05-04 04:23:21.607369 dexie_rewards-0.0.7/src/dexie_rewards/__init__.py
+-rw-r--r--   0        0        0     1126 2023-05-13 02:26:45.947358 dexie_rewards-0.0.7/src/dexie_rewards/config.py
+-rw-r--r--   0        0        0      822 2023-05-12 12:18:23.796037 dexie_rewards-0.0.7/src/dexie_rewards/decorators/with_db_connection.py
+-rw-r--r--   0        0        0     1207 2023-05-11 04:12:56.210275 dexie_rewards-0.0.7/src/dexie_rewards/decorators/with_wallet_rpc_client.py
+-rw-r--r--   0        0        0      234 2023-05-08 10:51:08.009870 dexie_rewards-0.0.7/src/dexie_rewards/main.py
+-rw-r--r--   0        0        0     3505 2023-05-13 03:54:19.525074 dexie_rewards-0.0.7/src/dexie_rewards/rewards/claim.py
+-rw-r--r--   0        0        0     1921 2023-05-13 03:55:02.188725 dexie_rewards-0.0.7/src/dexie_rewards/rewards/list.py
+-rw-r--r--   0        0        0      272 2023-05-08 10:18:31.545940 dexie_rewards-0.0.7/src/dexie_rewards/rewards/main.py
+-rw-r--r--   0        0        0     4839 2023-05-16 01:41:53.653083 dexie_rewards-0.0.7/src/dexie_rewards/rewards/utils.py
+-rw-r--r--   0        0        0     2293 2023-05-16 00:50:15.508487 dexie_rewards-0.0.7/src/dexie_rewards/services/dexie_api.py
+-rw-r--r--   0        0        0     3756 2023-05-13 03:51:52.828154 dexie_rewards-0.0.7/src/dexie_rewards/services/dexie_db.py
+-rw-r--r--   0        0        0     1713 2023-05-11 04:36:56.173403 dexie_rewards-0.0.7/src/dexie_rewards/services/wallet_rpc_client.py
+-rw-r--r--   0        0        0      801 2023-05-16 00:41:08.479451 dexie_rewards-0.0.7/src/dexie_rewards/types/offer_reward.py
+-rw-r--r--   0        0        0      229 2023-05-09 11:06:14.984159 dexie_rewards-0.0.7/src/dexie_rewards/types/utils.py
+-rw-r--r--   0        0        0     1851 2023-05-12 13:28:19.018840 dexie_rewards-0.0.7/src/dexie_rewards/utils.py
+-rw-r--r--   0        0        0    12792 1970-01-01 00:00:00.000000 dexie_rewards-0.0.7/PKG-INFO
```

### Comparing `dexie_rewards-0.0.6/LICENSE` & `dexie_rewards-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dexie_rewards-0.0.6/README.md` & `dexie_rewards-0.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -134,23 +134,21 @@
 
 ❯ dexie rewards list -f 2149823282 --json | jq
 [
   {
     "id": "Hj7KL4YjEyM8Sa4svzJe9SzunuGBT8wSUjDjXjPxoyDs",
     "status": 0,
     "date_found": "2023-05-12T07:31:43.086Z",
-    "date_rewards_since": "2023-05-12T12:35:44.370Z",
     "maker_puzzle_hash": "0x1aa36967f74dfc0b85996e9adbe2e646c507b34644c1e17501d790b3838dbdd4",
     "claimable_rewards": 0.068
   },
   {
     "id": "2dUtWAAsEbyGEY8G5NtNBsXWNCkZTuyRNjiZxb64Pmzd",
     "status": 0,
     "date_found": "2023-05-12T08:31:17.874Z",
-    "date_rewards_since": "2023-05-12T12:35:44.364Z",
     "maker_puzzle_hash": "0x1aa36967f74dfc0b85996e9adbe2e646c507b34644c1e17501d790b3838dbdd4",
     "claimable_rewards": 0.064
   }
 ]
 ```
 
 #### claim
```

### Comparing `dexie_rewards-0.0.6/pyproject.toml` & `dexie_rewards-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dexie-rewards"
-version = "0.0.6"
+version = "0.0.7"
 description = "An open source Python tool which runs locally and will automatically claim rewards for all your created offers on dexie."
 authors = ["Dexie Contributors <pypi@dexie.space>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{ include = "dexie_rewards", from = "src" }]
 
 [tool.poetry.dependencies]
```

### Comparing `dexie_rewards-0.0.6/src/dexie_rewards/config.py` & `dexie_rewards-0.0.7/src/dexie_rewards/config.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-0.0.6/src/dexie_rewards/decorators/with_db_connection.py` & `dexie_rewards-0.0.7/src/dexie_rewards/decorators/with_db_connection.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-0.0.6/src/dexie_rewards/decorators/with_wallet_rpc_client.py` & `dexie_rewards-0.0.7/src/dexie_rewards/decorators/with_wallet_rpc_client.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-0.0.6/src/dexie_rewards/rewards/claim.py` & `dexie_rewards-0.0.7/src/dexie_rewards/rewards/claim.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-0.0.6/src/dexie_rewards/rewards/list.py` & `dexie_rewards-0.0.7/src/dexie_rewards/rewards/list.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-0.0.6/src/dexie_rewards/rewards/utils.py` & `dexie_rewards-0.0.7/src/dexie_rewards/rewards/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,47 @@
 from rich import box
 from rich.console import Console
 from rich.table import Table
 from rich.text import Text
 from typing import Any, Dict, List, Tuple
+import datetime
+import json
 import traceback
 
 from chia.types.blockchain_format.sized_bytes import bytes32
 from chia.wallet.trading.offer import Offer
 
 from ..config import dexie_api_url, dexie_blue, dexie_url
 from ..services import wallet_rpc_client as wallet_rpc_client
 from ..services.dexie_api import Api, get_dexie_bs58_offer_hash
 from ..services import dexie_db as dexie_db
 from ..types.offer_reward import OfferReward
 from ..types.utils import from_datetime
 
 
 async def create_claims(offers_rewards: List[OfferReward]) -> List[Any]:
+    date = from_datetime(datetime.datetime.now())
     claims = []
     for offer_reward in offers_rewards:
         (
             public_key,
             signature,
             signing_mode,
         ) = await sign_claim(
             offer_reward.offer_id,
-            from_datetime(offer_reward.date_rewards_since),
+            date,
             offer_reward.maker_puzzle_hash,
         )
 
         # return offer hash, signature, pk, and puzzle hash
         claim_info = {
             "offer_id": offer_reward.offer_id,
             "signature": signature,
             "public_key": public_key,
+            "date": date,
         }
         claims.append(claim_info)
     return claims
 
 
 async def get_offers_with_claimable_rewards(
     synced_fingerprint: int, console: Console = Console()
@@ -87,17 +91,17 @@
         traceback_string = traceback.format_exc()
         console.print(traceback_string)
         console.print(e)
         return []
 
 
 async def sign_claim(
-    offer_id: str, date_rewards_since: str, maker_puzzle_hash: bytes32
+    offer_id: str, date: str, maker_puzzle_hash: bytes32
 ) -> Tuple[str, str, str]:
-    message = f"Claim liquidity rewards for {offer_id} since {date_rewards_since}"
+    message = f"Claim dexie liquidity rewards for offer {offer_id} ({date})"
     return await wallet_rpc_client.sign_message_by_puzzle_hash(
         maker_puzzle_hash, message
     )
 
 
 async def claim_rewards(claims_payload: Any) -> Dict[str, Any]:
     result = await Api(dexie_api_url).claim_rewards(claims_payload)
```

### Comparing `dexie_rewards-0.0.6/src/dexie_rewards/services/dexie_api.py` & `dexie_rewards-0.0.7/src/dexie_rewards/services/dexie_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,12 +61,12 @@
                 raise RuntimeError(rep.reason)
             return await rep.json()
 
     # claim rewards
     async def claim_rewards(self, claims_payload: Dict[str, Any]) -> Dict[str, Any]:
         async with (
             aiohttp.ClientSession() as session,
-            session.post(f"{self.base_url}/claimRewards", json=claims_payload) as rep,
+            session.post(f"{self.base_url}/rewards/claim", json=claims_payload) as rep,
         ):
             if not rep.ok:
                 raise RuntimeError(rep.reason)
             return await rep.json()
```

### Comparing `dexie_rewards-0.0.6/src/dexie_rewards/services/dexie_db.py` & `dexie_rewards-0.0.7/src/dexie_rewards/services/dexie_db.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-0.0.6/src/dexie_rewards/services/wallet_rpc_client.py` & `dexie_rewards-0.0.7/src/dexie_rewards/services/wallet_rpc_client.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-0.0.6/src/dexie_rewards/types/offer_reward.py` & `dexie_rewards-0.0.7/src/dexie_rewards/types/offer_reward.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,20 +9,18 @@
 
 @dataclass
 class OfferReward:
     offer_id: str
     is_active: bool
     claimable_rewards: float
     date_found: datetime
-    date_rewards_since: datetime
     maker_puzzle_hash: bytes32
 
     @classmethod
     def from_json_dict(cls, json_dict: Dict[str, Any]) -> "OfferReward":
         return cls(
             offer_id=json_dict["id"],
             is_active=True if json_dict["status"] == 0 else False,
             claimable_rewards=round(float(json_dict["claimable_rewards"]), 3),
             date_found=to_datetime(json_dict["date_found"]),
-            date_rewards_since=to_datetime(json_dict["date_rewards_since"]),
             maker_puzzle_hash=bytes32.from_hexstr(json_dict["maker_puzzle_hash"]),
         )
```

### Comparing `dexie_rewards-0.0.6/src/dexie_rewards/utils.py` & `dexie_rewards-0.0.7/src/dexie_rewards/utils.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-0.0.6/PKG-INFO` & `dexie_rewards-0.0.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dexie-rewards
-Version: 0.0.6
+Version: 0.0.7
 Summary: An open source Python tool which runs locally and will automatically claim rewards for all your created offers on dexie.
 License: Apache-2.0
 Author: Dexie Contributors
 Author-email: pypi@dexie.space
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -153,23 +153,21 @@
 
 ❯ dexie rewards list -f 2149823282 --json | jq
 [
   {
     "id": "Hj7KL4YjEyM8Sa4svzJe9SzunuGBT8wSUjDjXjPxoyDs",
     "status": 0,
     "date_found": "2023-05-12T07:31:43.086Z",
-    "date_rewards_since": "2023-05-12T12:35:44.370Z",
     "maker_puzzle_hash": "0x1aa36967f74dfc0b85996e9adbe2e646c507b34644c1e17501d790b3838dbdd4",
     "claimable_rewards": 0.068
   },
   {
     "id": "2dUtWAAsEbyGEY8G5NtNBsXWNCkZTuyRNjiZxb64Pmzd",
     "status": 0,
     "date_found": "2023-05-12T08:31:17.874Z",
-    "date_rewards_since": "2023-05-12T12:35:44.364Z",
     "maker_puzzle_hash": "0x1aa36967f74dfc0b85996e9adbe2e646c507b34644c1e17501d790b3838dbdd4",
     "claimable_rewards": 0.064
   }
 ]
 ```
 
 #### claim
```

