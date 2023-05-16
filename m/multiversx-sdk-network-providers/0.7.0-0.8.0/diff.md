# Comparing `tmp/multiversx_sdk_network_providers-0.7.0.tar.gz` & `tmp/multiversx_sdk_network_providers-0.8.0.tar.gz`

## Comparing `multiversx_sdk_network_providers-0.7.0.tar` & `multiversx_sdk_network_providers-0.8.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/.flake8
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/py.typed
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/pyrightconfig.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/requirements-dev.txt
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/requirements.txt
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/.github/workflows/linter-flake8.yml
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/.github/workflows/linter-pyright.yml
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/__init__.py
--rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/accounts.py
--rw-r--r--   0        0        0     9538 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/api_network_provider.py
--rw-r--r--   0        0        0     7290 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/api_network_provider_test.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/config.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/constants.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/contract_query_requests.py
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/contract_query_response.py
--rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/contract_results.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/errors.py
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/interface.py
--rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/network_config.py
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/network_general_statistics.py
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/network_stake.py
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/network_status.py
--rw-r--r--   0        0        0    10488 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/proxy_network_provider.py
--rw-r--r--   0        0        0     8854 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/proxy_network_provider_test.py
--rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/resources.py
--rw-r--r--   0        0        0     5831 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/token_definitions.py
--rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/tokens.py
--rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/transaction_completion_strategy.py
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/transaction_events.py
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/transaction_logs.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/transaction_receipt.py
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/transaction_status.py
--rw-r--r--   0        0        0     4974 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/transactions.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/utils.py
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/LICENSE
--rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/README.md
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/.flake8
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/py.typed
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/pyrightconfig.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/requirements-dev.txt
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/requirements.txt
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/.github/workflows/linter-flake8.yml
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/.github/workflows/linter-pyright.yml
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/__init__.py
+-rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/accounts.py
+-rw-r--r--   0        0        0    10897 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/api_network_provider.py
+-rw-r--r--   0        0        0     8294 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/api_network_provider_test.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/config.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/constants.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/contract_query_requests.py
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/contract_query_response.py
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/contract_results.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/errors.py
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/interface.py
+-rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/network_config.py
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/network_general_statistics.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/network_stake.py
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/network_status.py
+-rw-r--r--   0        0        0    10656 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/proxy_network_provider.py
+-rw-r--r--   0        0        0     9195 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/proxy_network_provider_test.py
+-rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/resources.py
+-rw-r--r--   0        0        0     5831 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/token_definitions.py
+-rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/tokens.py
+-rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/transaction_completion_strategy.py
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/transaction_events.py
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/transaction_logs.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/transaction_receipt.py
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/transaction_status.py
+-rw-r--r--   0        0        0     6604 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/transactions.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/utils.py
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/LICENSE
+-rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/README.md
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 multiversx_sdk_network_providers-0.8.0/PKG-INFO
```

### Comparing `multiversx_sdk_network_providers-0.7.0/.github/workflows/linter-flake8.yml` & `multiversx_sdk_network_providers-0.8.0/.github/workflows/linter-flake8.yml`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.7.0/.github/workflows/linter-pyright.yml` & `multiversx_sdk_network_providers-0.8.0/.github/workflows/linter-pyright.yml`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.7.0/.github/workflows/python-publish.yml` & `multiversx_sdk_network_providers-0.8.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.7.0/.github/workflows/test.yml` & `multiversx_sdk_network_providers-0.8.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/accounts.py` & `multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/accounts.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/api_network_provider.py` & `multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/api_network_provider.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,27 +17,31 @@
 from multiversx_sdk_network_providers.network_status import NetworkStatus
 from multiversx_sdk_network_providers.proxy_network_provider import ProxyNetworkProvider
 from multiversx_sdk_network_providers.token_definitions import (
     DefinitionOfFungibleTokenOnNetwork, DefinitionOfTokenCollectionOnNetwork)
 from multiversx_sdk_network_providers.tokens import (FungibleTokenOfAccountOnNetwork,
                                                      NonFungibleTokenOfAccountOnNetwork)
 from multiversx_sdk_network_providers.transaction_status import TransactionStatus
-from multiversx_sdk_network_providers.transactions import TransactionOnNetwork
+from multiversx_sdk_network_providers.transactions import TransactionOnNetwork, TransactionInMempool
 from multiversx_sdk_network_providers.utils import decimal_to_padded_hex
 
 
 class ApiNetworkProvider:
-    def __init__(self, url: str, auth: Union[AuthBase, None] = None, address_hrp: str = DEFAULT_ADDRESS_HRP):
+    def __init__(self, url: str, auth: Union[AuthBase, None] = None, address_hrp: str = DEFAULT_ADDRESS_HRP) -> None:
         self.url = url
         self.backing_proxy = ProxyNetworkProvider(url, auth, address_hrp)
         self.auth = auth
 
     def get_network_config(self) -> NetworkConfig:
         return self.backing_proxy.get_network_config()
 
+    def get_network_gas_configs(self) -> Dict[str, Any]:
+        response = self.do_get_generic("network/gas-configs")
+        return response["data"]
+
     def get_network_status(self) -> NetworkStatus:
         return self.backing_proxy.get_network_status()
 
     def get_guardian_data(self, address: IAddress) -> GuardianData:
         return self.backing_proxy.get_guardian_data(address)
 
     def get_network_stake_statistics(self) -> NetworkStake:
@@ -114,22 +118,50 @@
 
     def get_transaction(self, tx_hash: str) -> TransactionOnNetwork:
         response = self.do_get_generic(f'transactions/{tx_hash}')
         transaction = TransactionOnNetwork.from_api_http_response(tx_hash, response)
 
         return transaction
 
-    def get_transactions(self, address: IAddress, pagination: IPagination = DefaultPagination()) -> List[TransactionOnNetwork]:
+    def get_account_transactions(self, address: IAddress, pagination: IPagination = DefaultPagination()) -> List[TransactionOnNetwork]:
         url = f"accounts/{address.bech32()}/transactions?{self._build_pagination_params(pagination)}"
         response = self.do_get_generic_collection(url)
 
         transactions = [TransactionOnNetwork.from_api_http_response(tx.get("txHash", ""), tx) for tx in response]
 
         return transactions
 
+    def get_bunch_of_transactions(self, tx_hashes: List[str], with_block_info: bool = True, with_results: bool = True) -> List[TransactionOnNetwork]:
+        hashes = ",".join(tx_hashes)
+
+        url = f"transactions?hashes={hashes}"
+
+        if with_block_info:
+            url += "&withBlockInfo=true"
+
+        if with_results:
+            url += "&withResults=true"
+
+        result = self.do_get_generic_collection(url)
+
+        transactions = [TransactionOnNetwork.from_api_http_response(transaction["txHash"], transaction) for transaction in result]
+        return transactions
+
+    def get_transactions_in_mempool_for_account(self, address: IAddress) -> List[TransactionInMempool]:
+        url = f"transaction/pool?by-sender={address.bech32()}&fields=sender,receiver,gaslimit,gasprice,value,nonce,data"
+        response = self.do_get_generic(url)
+        tx_pool = response["data"]["txPool"]
+        mempool_transactions = tx_pool.get("transactions", [])
+
+        if not mempool_transactions:
+            return []
+
+        transactions = [TransactionInMempool.from_http_response(transaction) for transaction in mempool_transactions]
+        return transactions
+
     def get_transaction_status(self, tx_hash: str) -> TransactionStatus:
         response = self.do_get_generic(f'transactions/{tx_hash}?fields=status')
         status = TransactionStatus(response.get('status', ''))
 
         return status
 
     def send_transaction(self, transaction: ITransaction) -> str:
```

### Comparing `multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/api_network_provider_test.py` & `multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/api_network_provider_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,14 +37,22 @@
         assert result.rounds_per_epoch == 1200
         assert result.refresh_rate == 6000
         assert result.epoch >= 2864
         assert result.rounds_passed >= 0
         assert result.transactions >= 4330650
         assert result.accounts >= 92270
 
+    def test_get_network_gas_configs(self):
+        result = self.api.get_network_gas_configs()
+        built_in_cost = result["gasConfigs"]["builtInCost"]
+        meta_system_sc_cost = result["gasConfigs"]["metaSystemSCCost"]
+
+        assert built_in_cost["ESDTTransfer"] == 200000
+        assert meta_system_sc_cost["Stake"] == 5000000
+
     def test_get_account(self):
         address = Address.from_bech32('erd1testnlersh4z0wsv8kjx39me4rmnvjkwu8dsaea7ukdvvc9z396qykv7z7')
         result = self.api.get_account(address)
 
         assert result.address.bech32() == 'erd1testnlersh4z0wsv8kjx39me4rmnvjkwu8dsaea7ukdvvc9z396qykv7z7'
         assert result.username == ''
 
@@ -85,22 +93,36 @@
         assert result.hash == '2cb813be9d5e5040abb2522da75fa5c8d94f72caa510ff51d7525659f398298b'
         assert result.nonce == 828
         assert result.is_completed
         assert result.sender.bech32() == 'erd1testnlersh4z0wsv8kjx39me4rmnvjkwu8dsaea7ukdvvc9z396qykv7z7'
         assert result.receiver.bech32() == 'erd1c8tnzykaj7lhrd5cy6jap533afr4dqu7uqcdm6qv4wuwly9lcsqqm9ll4f'
         assert result.value == '10000000000000000000'
 
-    def test_get_transactions(self):
+    def test_get_account_transactions(self):
         address = Address.from_bech32('erd1testnlersh4z0wsv8kjx39me4rmnvjkwu8dsaea7ukdvvc9z396qykv7z7')
         pagination = Pagination(0, 2)
 
-        result = self.api.get_transactions(address, pagination)
+        result = self.api.get_account_transactions(address, pagination)
 
         assert len(result) == 2
 
+    def test_get_trasactions(self):
+        hashes = ["19de07b20873c6b9c77d3666eab532329f16f55a62b9fc961e52e4e0d57835d6", "8e43a0fb73bb97d1cacbca7de6d90ffacd9b7e10773f4ba37c6b8adbad6461dc"]
+        result = self.api.get_bunch_of_transactions(hashes)
+
+        assert len(result) == 2
+        assert result[0].status.is_failed()
+        assert result[1].status.is_successful()
+
+    def test_get_transactions_in_mempool_for_account(self):
+        address = Address.from_bech32("erd1testnlersh4z0wsv8kjx39me4rmnvjkwu8dsaea7ukdvvc9z396qykv7z7")
+        result = self.api.get_transactions_in_mempool_for_account(address)
+
+        assert len(result) == 0
+
     def test_get_sc_invoking_tx(self):
         result = self.api.get_transaction('cd2da63a51fd422c8b69a1b5ebcb9edbbf0eb9750c3fe8e199d39ed5d82000e9')
 
         assert result.is_completed == True
         assert len(result.contract_results.items) > 0
         assert result.data == 'issue@54455354@54455354@03e8@00@63616e4d696e74@74727565@63616e4275726e@74727565@63616e4368616e67654f776e6572@74727565@63616e55706772616465@74727565'
```

### Comparing `multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/contract_query_requests.py` & `multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/contract_query_requests.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/contract_query_response.py` & `multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/contract_query_response.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/contract_results.py` & `multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/contract_results.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/interface.py` & `multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/interface.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/network_config.py` & `multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/network_config.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/network_general_statistics.py` & `multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/network_general_statistics.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/network_stake.py` & `multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/network_stake.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/network_status.py` & `multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/network_status.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/proxy_network_provider.py` & `multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/proxy_network_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,25 +18,29 @@
 from multiversx_sdk_network_providers.tokens import (FungibleTokenOfAccountOnNetwork,
                                                      NonFungibleTokenOfAccountOnNetwork)
 from multiversx_sdk_network_providers.transaction_status import TransactionStatus
 from multiversx_sdk_network_providers.transactions import TransactionOnNetwork
 
 
 class ProxyNetworkProvider:
-    def __init__(self, url: str, auth: Union[AuthBase, None] = None, address_hrp: str = DEFAULT_ADDRESS_HRP):
+    def __init__(self, url: str, auth: Union[AuthBase, None] = None, address_hrp: str = DEFAULT_ADDRESS_HRP) -> None:
         self.url = url
         self.auth = auth
         self.address_hrp = address_hrp
 
     def get_network_config(self) -> NetworkConfig:
         response = self.do_get_generic('network/config')
         network_config = NetworkConfig.from_http_response(response.get('config', ''))
 
         return network_config
 
+    def get_network_gas_configs(self) -> Dict[str, Any]:
+        response = self.do_get_generic("network/gas-configs").to_dictionary()
+        return response
+
     def get_network_status(self, shard: Optional[int] = METACHAIN_ID) -> NetworkStatus:
         response = self.do_get_generic(f'network/status/{shard}')
         network_status = NetworkStatus.from_http_response(response.get('status', ''))
 
         return network_status
 
     def get_account(self, address: IAddress) -> AccountOnNetwork:
```

### Comparing `multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/proxy_network_provider_test.py` & `multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/proxy_network_provider_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,14 +33,22 @@
         assert result.round_at_epoch_start >= 3471351
         assert result.rounds_passed_in_current_epcoch > 0
         assert result.nonces_passed_in_current_epoch > 0
         assert result.highest_final_nonce >= 3436531
         assert result.nonce_at_epoch_start >= 3435637
         assert result.rounds_per_epoch == 1200
 
+    def test_get_network_gas_configs(self):
+        result = self.proxy.get_network_gas_configs()
+        built_in_cost = result["gasConfigs"]["builtInCost"]
+        meta_system_sc_cost = result["gasConfigs"]["metaSystemSCCost"]
+
+        assert built_in_cost["ESDTTransfer"] == 200000
+        assert meta_system_sc_cost["Stake"] == 5000000
+
     def test_get_account(self):
         address = Address.from_bech32(
             "erd1testnlersh4z0wsv8kjx39me4rmnvjkwu8dsaea7ukdvvc9z396qykv7z7"
         )
         result = self.proxy.get_account(address)
 
         assert (
```

### Comparing `multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/resources.py` & `multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/resources.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/token_definitions.py` & `multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/token_definitions.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/tokens.py` & `multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/tokens.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/transaction_completion_strategy.py` & `multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/transaction_completion_strategy.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/transaction_events.py` & `multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/transaction_events.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/transaction_logs.py` & `multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/transaction_logs.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/transaction_receipt.py` & `multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/transaction_receipt.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/transaction_status.py` & `multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/transaction_status.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.7.0/multiversx_sdk_network_providers/transactions.py` & `multiversx_sdk_network_providers-0.8.0/multiversx_sdk_network_providers/transactions.py`

 * *Files 23% similar despite different names*

```diff
@@ -36,14 +36,15 @@
         self.block_nonce: int = 0
         self.hyperblock_nonce: int = 0
         self.hyperblock_hash: str = ""
 
         self.receipt: TransactionReceipt = TransactionReceipt()
         self.contract_results: ContractResults = ContractResults([])
         self.logs: TransactionLogs = TransactionLogs()
+        self.raw_response: Dict[str, Any] = {}
 
     def get_status(self) -> TransactionStatus:
         return self.status
 
     @staticmethod
     def from_api_http_response(
         tx_hash: str, response: Dict[str, Any]
@@ -103,14 +104,15 @@
         result.hyperblock_nonce = response.get("hyperblockNonce", 0)
         result.hyperblock_hash = response.get("hyperblockHash", "")
 
         result.receipt = TransactionReceipt.from_http_response(
             response.get("receipt", {})
         )
         result.logs = TransactionLogs.from_http_response(response.get("logs", {}))
+        result.raw_response = response
 
         return result
 
     def to_dictionary(self) -> Dict[str, Any]:
         return {
             "isCompleted": self.is_completed,
             "hash": self.hash,
@@ -129,7 +131,54 @@
             "timestamp": self.timestamp,
             "blockNonce": self.block_nonce,
             "hyperblockNonce": self.hyperblock_nonce,
             "hyperblockHash": self.hyperblock_hash,
             "smartContractResults": [item.to_dictionary() for item in self.contract_results.items],
             "logs": self.logs.to_dictionary(),
         }
+
+
+class TransactionInMempool:
+    def __init__(self) -> None:
+        self.hash: str = ""
+        self.receiver: IAddress = EmptyAddress()
+        self.sender: IAddress = EmptyAddress()
+        self.gas_limit: int = 0
+        self.gas_price: int = 0
+        self.data: str = ""
+        self.nonce: int = 0
+        self.value: int = 0
+
+    @staticmethod
+    def from_http_response(data: Dict[str, Any]) -> "TransactionInMempool":
+        data = data["txFields"]
+        transaction = TransactionInMempool()
+
+        transaction.hash = data.get("hash", "")
+        sender = data.get("sender", "")
+        transaction.sender = Address.from_bech32(sender) if sender else EmptyAddress()
+
+        receiver = data.get("receiver", "")
+        transaction.receiver = Address.from_bech32(receiver) if receiver else EmptyAddress()
+
+        transaction.gas_price = data.get("gasPrice", 0)
+        transaction.gas_limit = data.get("gasLimit", 0)
+
+        transaction.nonce = data.get("nonce", 0)
+        transaction.value = data.get("value", 0)
+
+        data_field = data.get("data", "")
+        transaction.data = base64.b64decode(data_field).decode()
+
+        return transaction
+
+    def to_dictionary(self) -> Dict[str, Any]:
+        return {
+            "txHash": self.hash,
+            "sender": self.sender.bech32(),
+            "receiver": self.receiver.bech32(),
+            "nonce": self.nonce,
+            "value": self.value,
+            "gasLimit": self.gas_limit,
+            "gasPrice": self.gas_price,
+            "data": self.data
+        }
```

### Comparing `multiversx_sdk_network_providers-0.7.0/.gitignore` & `multiversx_sdk_network_providers-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.7.0/LICENSE` & `multiversx_sdk_network_providers-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.7.0/README.md` & `multiversx_sdk_network_providers-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_network_providers-0.7.0/pyproject.toml` & `multiversx_sdk_network_providers-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [project]
 name = "multiversx-sdk-network-providers"
-version = "0.7.0"
+version = "0.8.0"
 authors = [
   { name="MultiversX" },
 ]
 license = "MIT"
 description = "Network providers for MultiversX Python SDK."
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `multiversx_sdk_network_providers-0.7.0/PKG-INFO` & `multiversx_sdk_network_providers-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiversx-sdk-network-providers
-Version: 0.7.0
+Version: 0.8.0
 Summary: Network providers for MultiversX Python SDK.
 Project-URL: Homepage, https://github.com/multiversx/mx-sdk-py-network-providers
 Author: MultiversX
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

