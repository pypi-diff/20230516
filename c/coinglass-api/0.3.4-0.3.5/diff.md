# Comparing `tmp/coinglass_api-0.3.4.tar.gz` & `tmp/coinglass_api-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coinglass_api-0.3.4.tar", max compression
+gzip compressed data, was "coinglass_api-0.3.5.tar", max compression
```

## Comparing `coinglass_api-0.3.4.tar` & `coinglass_api-0.3.5.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1069 2023-01-15 20:06:02.595582 coinglass_api-0.3.4/LICENSE.md
--rw-r--r--   0        0        0     4054 2023-03-03 10:15:21.547762 coinglass_api-0.3.4/README.md
--rw-r--r--   0        0        0       57 2023-01-15 18:42:45.746707 coinglass_api-0.3.4/coinglass_api/__init__.py
--rw-r--r--   0        0        0    11044 2023-02-18 20:50:23.647057 coinglass_api-0.3.4/coinglass_api/api.py
--rw-r--r--   0        0        0      699 2023-03-05 21:18:03.581294 coinglass_api-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     4874 1970-01-01 00:00:00.000000 coinglass_api-0.3.4/setup.py
--rw-r--r--   0        0        0     4763 1970-01-01 00:00:00.000000 coinglass_api-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-01-15 20:06:02.595582 coinglass_api-0.3.5/LICENSE.md
+-rw-r--r--   0        0        0     4218 2023-05-16 13:11:00.550496 coinglass_api-0.3.5/README.md
+-rw-r--r--   0        0        0       57 2023-01-15 18:42:45.746707 coinglass_api-0.3.5/coinglass_api/__init__.py
+-rw-r--r--   0        0        0    11089 2023-05-16 12:46:14.173931 coinglass_api-0.3.5/coinglass_api/api.py
+-rw-r--r--   0        0        0      809 2023-05-16 12:44:05.063649 coinglass_api-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     4962 1970-01-01 00:00:00.000000 coinglass_api-0.3.5/PKG-INFO
```

### Comparing `coinglass_api-0.3.4/LICENSE.md` & `coinglass_api-0.3.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `coinglass_api-0.3.4/README.md` & `coinglass_api-0.3.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Coinglass API
 [![PyPi version](https://img.shields.io/pypi/v/coinglass-api)](https://pypi.python.org/pypi/coinglass-api/)
 [![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-3100//)
 [![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)](https://www.python.org/downloads/release/python-3110//)
+[![codecov](https://codecov.io/gh/dineshpinto/coinglass-api/branch/main/graph/badge.svg?token=XTJRRU2W1T)](https://codecov.io/gh/dineshpinto/coinglass-api)
 
 ## Unofficial Python client for Coinglass API
 
 Wrapper around the [Coinglass API](https://coinglass.com/pricing) to fetch data about the crypto markets.
 All data is output in pandas DataFrames (single or multi-index) and all time series data uses a DateTimeIndex.
 
 **Note**: This is work in progress. Currently only supports the `indicator` API endpoint.
@@ -22,19 +23,18 @@
 
 ```bash
 poetry add coinglass-api
 ```
 
 ## Usage
 
-
 ```python
 from coinglass_api import CoinglassAPI
 
-cg = CoinglassAPI(api_key="abcd1234")
+cg = CoinglassAPI(coinglass_secret="abcd1234")
 
 # Funding rate of ETH on dYdX
 fr_btc_dydx = cg.funding(ex="dYdX", pair="ETH-USD", interval="h8")
 
 # Get average funding for BTC
 fr_avg_btc = cg.funding_average(symbol="BTC", interval="h4")
```

### Comparing `coinglass_api-0.3.4/coinglass_api/api.py` & `coinglass_api-0.3.5/coinglass_api/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import pandas as pd
 import requests
 
 
 class CoinglassAPI:
     """ Unofficial Python client for Coinglass API """
 
-    def __init__(self, api_key: str):
+    def __init__(self, coinglass_secret: str):
         """
         Args:
-            api_key: key from Coinglass, get one at https://www.coinglass.com/pricing
+            coinglass_secret: key from Coinglass, get one at https://www.coinglass.com/pricing
         """
-        self.__api_key = api_key
+        self.__coinglass_secret = coinglass_secret
         self._base_url = "https://open-api.coinglass.com/public/v2/indicator/"
         self._session = requests.Session()
 
     def _get(self, endpoint: str, params: dict = None) -> dict:
         headers = {
             "accept": "application/json",
-            "coinglassSecret": self.__api_key
+            "coinglassSecret": self.__coinglass_secret
         }
         url = self._base_url + endpoint
         return self._session.request('GET', url, params=params, headers=headers, timeout=30).json()
 
     @staticmethod
     def _create_dataframe(data: list[dict], time_col: str) -> pd.DataFrame:
         """ Create pandas DataFrame from list of dicts """
```

### Comparing `coinglass_api-0.3.4/pyproject.toml` & `coinglass_api-0.3.5/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 [tool.poetry]
 name = "coinglass-api"
-version = "0.3.4"
+version = "0.3.5"
 repository = "https://github.com/dineshpinto/coinglass-api"
 homepage = "https://github.com/dineshpinto/coinglass-api"
 license = "MIT"
-keywords = ["coinglass", "api", "crypto", "cryptocurrency"]
+keywords = ["coinglass", "api", "crypto", "cryptocurrency", "bitcoin", "ethereum", "binance", "dydx", "okex"]
 description = "Unofficial Python client for Coinglass API"
 authors = ["dineshpinto <annual.fallout_0z@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "coinglass_api" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-pandas = "^1.5.2"
+pandas = "^2.0.0"
 requests = "^2.28.2"
 
 [tool.poetry.group.dev.dependencies]
 jupyterlab = "^3.5.2"
 matplotlib = "^3.5.2"
 seaborn = "^0.11.2"
 
+
+[tool.poetry.group.test.dependencies]
+coverage = "^7.2.5"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `coinglass_api-0.3.4/setup.py` & `coinglass_api-0.3.5/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,122 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: coinglass-api
+Version: 0.3.5
+Summary: Unofficial Python client for Coinglass API
+Home-page: https://github.com/dineshpinto/coinglass-api
+License: MIT
+Keywords: coinglass,api,crypto,cryptocurrency,bitcoin,ethereum,binance,dydx,okex
+Author: dineshpinto
+Author-email: annual.fallout_0z@gmail.com
+Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pandas (>=2.0.0,<3.0.0)
+Requires-Dist: requests (>=2.28.2,<3.0.0)
+Project-URL: Repository, https://github.com/dineshpinto/coinglass-api
+Description-Content-Type: text/markdown
+
+# Coinglass API
+[![PyPi version](https://img.shields.io/pypi/v/coinglass-api)](https://pypi.python.org/pypi/coinglass-api/)
+[![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-3100//)
+[![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)](https://www.python.org/downloads/release/python-3110//)
+[![codecov](https://codecov.io/gh/dineshpinto/coinglass-api/branch/main/graph/badge.svg?token=XTJRRU2W1T)](https://codecov.io/gh/dineshpinto/coinglass-api)
+
+## Unofficial Python client for Coinglass API
+
+Wrapper around the [Coinglass API](https://coinglass.com/pricing) to fetch data about the crypto markets.
+All data is output in pandas DataFrames (single or multi-index) and all time series data uses a DateTimeIndex.
+
+**Note**: This is work in progress. Currently only supports the `indicator` API endpoint.
+
+![Example Plot](https://github.com/dineshpinto/coinglass-api/blob/main/examples/example_plot.jpg?raw=true)
+
+## Installation
+
+```bash
+pip install coinglass-api
+```
+
+### or with poetry 
+
+```bash
+poetry add coinglass-api
+```
+
+## Usage
+
+```python
+from coinglass_api import CoinglassAPI
+
+cg = CoinglassAPI(coinglass_secret="abcd1234")
+
+# Funding rate of ETH on dYdX
+fr_btc_dydx = cg.funding(ex="dYdX", pair="ETH-USD", interval="h8")
+
+# Get average funding for BTC
+fr_avg_btc = cg.funding_average(symbol="BTC", interval="h4")
+
+# Get funding OHLC for ETHUSDT on Binance
+fr_ohlc_eth_binance = cg.funding_ohlc(ex="Binance", pair="ETHUSDT", interval="h4")
+
+# Get aggregated OI OHLC data for BTC
+oi_agg_eth = cg.open_interest_aggregated_ohlc(symbol="ETH", interval="h4")
+
+# Get OHLC liquidations data for ETHUSDT on dYdX
+liq_ohlc_eth_dydx = cg.liquidation_pair(ex="dYdX", pair="ETH-USD", interval="h4")
+
+# Get liquidation data for BTC
+liq_btc = cg.liquidation_symbol(symbol="BTC", interval="h4")
+
+# Get long/short ratios for BTC
+lsr_btc = cg.long_short_symbol(symbol="BTC", interval="h4")
+```
+
+## Examples
+
+```
+>>> cg.funding(ex="dYdX", pair="ETH-USD", interval="h8").head()
+```
+
+| <br/>time           | exchangeName<br/> | symbol<br/> | quoteCurrency<br/> | fundingRate<br/> |
+|:--------------------|:------------------|:------------|:-------------------|:-----------------|
+| 2022-08-22 08:00:00 | dYdX              | ETH         | USD                | -0.001151        |
+| 2022-08-22 16:00:00 | dYdX              | ETH         | USD                | 0.001678         |
+| 2022-08-23 00:00:00 | dYdX              | ETH         | USD                | 0.003743         |
+| 2022-08-23 08:00:00 | dYdX              | ETH         | USD                | 0.003561         |
+| 2022-08-23 16:00:00 | dYdX              | ETH         | USD                | 0.000658         |
+
+```
+>>> cg.funding(ex="dYdX", pair="ETH-USD", interval="h8").info()
+```
+
+```
+<class 'pandas.core.frame.DataFrame'>
+DatetimeIndex: 500 entries, 2022-08-22 08:00:00 to 2023-02-04 16:00:00
+Data columns (total 4 columns):
+ #   Column         Non-Null Count  Dtype  
+---  ------         --------------  -----  
+ 0   exchangeName   500 non-null    object 
+ 1   symbol         500 non-null    object 
+ 2   quoteCurrency  500 non-null    object 
+ 3   fundingRate    500 non-null    float64
+dtypes: float64(1), object(3)
+memory usage: 19.5+ KB
+```
+
+```
+>>> cg.funding(ex="dYdX", pair="ETH-USD", interval="h8").plot(y="fundingRate")
+```
+![funding_rate](https://github.com/dineshpinto/coinglass-api/blob/main/examples/funding_rate.jpg?raw=true)
+
+## Disclaimer
+
+This project is for educational purposes only. You should not construe any such information or other material as legal,
+tax, investment, financial, or other advice. Nothing contained here constitutes a solicitation, recommendation,
+endorsement, or offer by me or any third party service provider to buy or sell any securities or other financial
+instruments in this or in any other jurisdiction in which such solicitation or offer would be unlawful under the
+securities laws of such jurisdiction.
 
-packages = \
-['coinglass_api']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['pandas>=1.5.2,<2.0.0', 'requests>=2.28.2,<3.0.0']
-
-setup_kwargs = {
-    'name': 'coinglass-api',
-    'version': '0.3.4',
-    'description': 'Unofficial Python client for Coinglass API',
-    'long_description': '# Coinglass API\n[![PyPi version](https://img.shields.io/pypi/v/coinglass-api)](https://pypi.python.org/pypi/coinglass-api/)\n[![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-3100//)\n[![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)](https://www.python.org/downloads/release/python-3110//)\n\n## Unofficial Python client for Coinglass API\n\nWrapper around the [Coinglass API](https://coinglass.com/pricing) to fetch data about the crypto markets.\nAll data is output in pandas DataFrames (single or multi-index) and all time series data uses a DateTimeIndex.\n\n**Note**: This is work in progress. Currently only supports the `indicator` API endpoint.\n\n![Example Plot](https://github.com/dineshpinto/coinglass-api/blob/main/examples/example_plot.jpg?raw=true)\n\n## Installation\n\n```bash\npip install coinglass-api\n```\n\n### or with poetry \n\n```bash\npoetry add coinglass-api\n```\n\n## Usage\n\n\n```python\nfrom coinglass_api import CoinglassAPI\n\ncg = CoinglassAPI(api_key="abcd1234")\n\n# Funding rate of ETH on dYdX\nfr_btc_dydx = cg.funding(ex="dYdX", pair="ETH-USD", interval="h8")\n\n# Get average funding for BTC\nfr_avg_btc = cg.funding_average(symbol="BTC", interval="h4")\n\n# Get funding OHLC for ETHUSDT on Binance\nfr_ohlc_eth_binance = cg.funding_ohlc(ex="Binance", pair="ETHUSDT", interval="h4")\n\n# Get aggregated OI OHLC data for BTC\noi_agg_eth = cg.open_interest_aggregated_ohlc(symbol="ETH", interval="h4")\n\n# Get OHLC liquidations data for ETHUSDT on dYdX\nliq_ohlc_eth_dydx = cg.liquidation_pair(ex="dYdX", pair="ETH-USD", interval="h4")\n\n# Get liquidation data for BTC\nliq_btc = cg.liquidation_symbol(symbol="BTC", interval="h4")\n\n# Get long/short ratios for BTC\nlsr_btc = cg.long_short_symbol(symbol="BTC", interval="h4")\n```\n\n## Examples\n\n```\n>>> cg.funding(ex="dYdX", pair="ETH-USD", interval="h8").head()\n```\n\n| <br/>time           | exchangeName<br/> | symbol<br/> | quoteCurrency<br/> | fundingRate<br/> |\n|:--------------------|:------------------|:------------|:-------------------|:-----------------|\n| 2022-08-22 08:00:00 | dYdX              | ETH         | USD                | -0.001151        |\n| 2022-08-22 16:00:00 | dYdX              | ETH         | USD                | 0.001678         |\n| 2022-08-23 00:00:00 | dYdX              | ETH         | USD                | 0.003743         |\n| 2022-08-23 08:00:00 | dYdX              | ETH         | USD                | 0.003561         |\n| 2022-08-23 16:00:00 | dYdX              | ETH         | USD                | 0.000658         |\n\n```\n>>> cg.funding(ex="dYdX", pair="ETH-USD", interval="h8").info()\n```\n\n```\n<class \'pandas.core.frame.DataFrame\'>\nDatetimeIndex: 500 entries, 2022-08-22 08:00:00 to 2023-02-04 16:00:00\nData columns (total 4 columns):\n #   Column         Non-Null Count  Dtype  \n---  ------         --------------  -----  \n 0   exchangeName   500 non-null    object \n 1   symbol         500 non-null    object \n 2   quoteCurrency  500 non-null    object \n 3   fundingRate    500 non-null    float64\ndtypes: float64(1), object(3)\nmemory usage: 19.5+ KB\n```\n\n```\n>>> cg.funding(ex="dYdX", pair="ETH-USD", interval="h8").plot(y="fundingRate")\n```\n![funding_rate](https://github.com/dineshpinto/coinglass-api/blob/main/examples/funding_rate.jpg?raw=true)\n\n## Disclaimer\n\nThis project is for educational purposes only. You should not construe any such information or other material as legal,\ntax, investment, financial, or other advice. Nothing contained here constitutes a solicitation, recommendation,\nendorsement, or offer by me or any third party service provider to buy or sell any securities or other financial\ninstruments in this or in any other jurisdiction in which such solicitation or offer would be unlawful under the\nsecurities laws of such jurisdiction.\n\nUnder no circumstances will I be held responsible or liable in any way for any claims, damages, losses, expenses, costs,\nor liabilities whatsoever, including, without limitation, any direct or indirect damages for loss of profits.',
-    'author': 'dineshpinto',
-    'author_email': 'annual.fallout_0z@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/dineshpinto/coinglass-api',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.10,<4.0',
-}
-
-
-setup(**setup_kwargs)
+Under no circumstances will I be held responsible or liable in any way for any claims, damages, losses, expenses, costs,
+or liabilities whatsoever, including, without limitation, any direct or indirect damages for loss of profits.
```

