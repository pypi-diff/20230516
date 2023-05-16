# Comparing `tmp/cvxportfolio-0.3.0.tar.gz` & `tmp/cvxportfolio-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxportfolio-0.3.0.tar", last modified: Fri May 12 05:21:23 2023, max compression
+gzip compressed data, was "cvxportfolio-0.3.1.tar", last modified: Tue May 16 17:39:56 2023, max compression
```

## Comparing `cvxportfolio-0.3.0.tar` & `cvxportfolio-0.3.1.tar`

### file list

```diff
@@ -1,39 +1,41 @@
-drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-05-12 05:21:23.927908 cvxportfolio-0.3.0/
--rw-r--r--   0 enzo       (501) staff       (20)      199 2023-04-08 05:48:25.000000 cvxportfolio-0.3.0/AUTHORS
--rw-r--r--   0 enzo       (501) staff       (20)      599 2023-04-08 05:48:25.000000 cvxportfolio-0.3.0/LICENSE
--rw-r--r--   0 enzo       (501) staff       (20)      329 2023-05-12 05:21:23.927585 cvxportfolio-0.3.0/PKG-INFO
--rw-r--r--   0 enzo       (501) staff       (20)     3487 2023-05-12 03:58:00.000000 cvxportfolio-0.3.0/README.md
-drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-05-12 05:21:23.910446 cvxportfolio-0.3.0/cvxportfolio/
--rw-r--r--   0 enzo       (501) staff       (20)      888 2023-05-12 05:21:20.000000 cvxportfolio-0.3.0/cvxportfolio/__init__.py
--rw-r--r--   0 enzo       (501) staff       (20)     6972 2023-05-12 04:06:18.000000 cvxportfolio-0.3.0/cvxportfolio/constraints.py
--rw-r--r--   0 enzo       (501) staff       (20)     9746 2023-05-12 05:19:45.000000 cvxportfolio-0.3.0/cvxportfolio/costs.py
--rw-r--r--   0 enzo       (501) staff       (20)    19217 2023-05-11 16:35:10.000000 cvxportfolio-0.3.0/cvxportfolio/data.py
--rw-r--r--   0 enzo       (501) staff       (20)     1004 2023-05-11 16:35:10.000000 cvxportfolio-0.3.0/cvxportfolio/errors.py
--rw-r--r--   0 enzo       (501) staff       (20)    10204 2023-05-11 16:35:10.000000 cvxportfolio-0.3.0/cvxportfolio/estimator.py
--rw-r--r--   0 enzo       (501) staff       (20)    19854 2023-05-11 19:03:54.000000 cvxportfolio-0.3.0/cvxportfolio/policies.py
--rw-r--r--   0 enzo       (501) staff       (20)     5909 2023-05-12 05:13:01.000000 cvxportfolio-0.3.0/cvxportfolio/result.py
--rw-r--r--   0 enzo       (501) staff       (20)    10807 2023-05-12 05:05:30.000000 cvxportfolio-0.3.0/cvxportfolio/returns.py
--rw-r--r--   0 enzo       (501) staff       (20)    18691 2023-05-12 05:01:19.000000 cvxportfolio-0.3.0/cvxportfolio/risks.py
--rw-r--r--   0 enzo       (501) staff       (20)    24580 2023-05-12 04:34:39.000000 cvxportfolio-0.3.0/cvxportfolio/simulator.py
-drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-05-12 05:21:23.926979 cvxportfolio-0.3.0/cvxportfolio/tests/
--rw-r--r--   0 enzo       (501) staff       (20)        0 2023-05-12 05:21:20.000000 cvxportfolio-0.3.0/cvxportfolio/tests/__init__.py
--rw-r--r--   0 enzo       (501) staff       (20)     1626 2023-05-11 16:35:10.000000 cvxportfolio-0.3.0/cvxportfolio/tests/base.py
--rw-r--r--   0 enzo       (501) staff       (20)   156730 2023-05-11 16:35:10.000000 cvxportfolio-0.3.0/cvxportfolio/tests/returns.csv
--rw-r--r--   0 enzo       (501) staff       (20)   149356 2023-05-11 16:35:10.000000 cvxportfolio-0.3.0/cvxportfolio/tests/sigmas.csv
--rw-r--r--   0 enzo       (501) staff       (20)     8855 2023-05-11 16:35:10.000000 cvxportfolio-0.3.0/cvxportfolio/tests/test_constraints.py
--rw-r--r--   0 enzo       (501) staff       (20)     8306 2023-05-11 19:06:55.000000 cvxportfolio-0.3.0/cvxportfolio/tests/test_costs.py
--rw-r--r--   0 enzo       (501) staff       (20)    10329 2023-05-11 16:35:10.000000 cvxportfolio-0.3.0/cvxportfolio/tests/test_data.py
--rw-r--r--   0 enzo       (501) staff       (20)     6657 2023-05-11 16:35:10.000000 cvxportfolio-0.3.0/cvxportfolio/tests/test_estimator.py
--rw-r--r--   0 enzo       (501) staff       (20)    21796 2023-05-11 19:07:12.000000 cvxportfolio-0.3.0/cvxportfolio/tests/test_policies.py
--rw-r--r--   0 enzo       (501) staff       (20)     4349 2023-05-11 19:07:22.000000 cvxportfolio-0.3.0/cvxportfolio/tests/test_returns.py
--rw-r--r--   0 enzo       (501) staff       (20)     8964 2023-05-11 19:07:41.000000 cvxportfolio-0.3.0/cvxportfolio/tests/test_risks.py
--rw-r--r--   0 enzo       (501) staff       (20)    10577 2023-05-11 16:35:10.000000 cvxportfolio-0.3.0/cvxportfolio/tests/test_simulator.py
--rw-r--r--   0 enzo       (501) staff       (20)   116620 2023-05-11 16:35:10.000000 cvxportfolio-0.3.0/cvxportfolio/tests/volumes.csv
-drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-05-12 05:21:23.913031 cvxportfolio-0.3.0/cvxportfolio.egg-info/
--rw-r--r--   0 enzo       (501) staff       (20)      329 2023-05-12 05:21:23.000000 cvxportfolio-0.3.0/cvxportfolio.egg-info/PKG-INFO
--rw-r--r--   0 enzo       (501) staff       (20)      910 2023-05-12 05:21:23.000000 cvxportfolio-0.3.0/cvxportfolio.egg-info/SOURCES.txt
--rw-r--r--   0 enzo       (501) staff       (20)        1 2023-05-12 05:21:23.000000 cvxportfolio-0.3.0/cvxportfolio.egg-info/dependency_links.txt
--rw-r--r--   0 enzo       (501) staff       (20)       64 2023-05-12 05:21:23.000000 cvxportfolio-0.3.0/cvxportfolio.egg-info/requires.txt
--rw-r--r--   0 enzo       (501) staff       (20)       13 2023-05-12 05:21:23.000000 cvxportfolio-0.3.0/cvxportfolio.egg-info/top_level.txt
--rw-r--r--   0 enzo       (501) staff       (20)       38 2023-05-12 05:21:23.927992 cvxportfolio-0.3.0/setup.cfg
--rw-r--r--   0 enzo       (501) staff       (20)      788 2023-05-12 05:21:20.000000 cvxportfolio-0.3.0/setup.py
+drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-05-16 17:39:56.418780 cvxportfolio-0.3.1/
+-rw-r--r--   0 enzo       (501) staff       (20)      199 2023-04-08 05:48:25.000000 cvxportfolio-0.3.1/AUTHORS
+-rw-r--r--   0 enzo       (501) staff       (20)      599 2023-04-08 05:48:25.000000 cvxportfolio-0.3.1/LICENSE
+-rw-r--r--   0 enzo       (501) staff       (20)      329 2023-05-16 17:39:56.418449 cvxportfolio-0.3.1/PKG-INFO
+-rw-r--r--   0 enzo       (501) staff       (20)     3650 2023-05-13 03:51:33.000000 cvxportfolio-0.3.1/README.md
+drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-05-16 17:39:56.396634 cvxportfolio-0.3.1/cvxportfolio/
+-rw-r--r--   0 enzo       (501) staff       (20)      888 2023-05-16 17:39:49.000000 cvxportfolio-0.3.1/cvxportfolio/__init__.py
+-rw-r--r--   0 enzo       (501) staff       (20)     6972 2023-05-12 04:06:18.000000 cvxportfolio-0.3.1/cvxportfolio/constraints.py
+-rw-r--r--   0 enzo       (501) staff       (20)     9746 2023-05-12 05:19:45.000000 cvxportfolio-0.3.1/cvxportfolio/costs.py
+-rw-r--r--   0 enzo       (501) staff       (20)    19617 2023-05-16 16:47:47.000000 cvxportfolio-0.3.1/cvxportfolio/data.py
+-rw-r--r--   0 enzo       (501) staff       (20)     1004 2023-05-11 16:35:10.000000 cvxportfolio-0.3.1/cvxportfolio/errors.py
+-rw-r--r--   0 enzo       (501) staff       (20)    10412 2023-05-16 16:47:47.000000 cvxportfolio-0.3.1/cvxportfolio/estimator.py
+-rw-r--r--   0 enzo       (501) staff       (20)     7597 2023-05-16 17:30:00.000000 cvxportfolio-0.3.1/cvxportfolio/forecast.py
+-rw-r--r--   0 enzo       (501) staff       (20)    19854 2023-05-11 19:03:54.000000 cvxportfolio-0.3.1/cvxportfolio/policies.py
+-rw-r--r--   0 enzo       (501) staff       (20)     6959 2023-05-16 16:47:47.000000 cvxportfolio-0.3.1/cvxportfolio/result.py
+-rw-r--r--   0 enzo       (501) staff       (20)    11140 2023-05-16 16:47:47.000000 cvxportfolio-0.3.1/cvxportfolio/returns.py
+-rw-r--r--   0 enzo       (501) staff       (20)    20012 2023-05-16 16:47:47.000000 cvxportfolio-0.3.1/cvxportfolio/risks.py
+-rw-r--r--   0 enzo       (501) staff       (20)    25533 2023-05-16 16:47:47.000000 cvxportfolio-0.3.1/cvxportfolio/simulator.py
+drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-05-16 17:39:56.416552 cvxportfolio-0.3.1/cvxportfolio/tests/
+-rw-r--r--   0 enzo       (501) staff       (20)        0 2023-05-16 17:39:49.000000 cvxportfolio-0.3.1/cvxportfolio/tests/__init__.py
+-rw-r--r--   0 enzo       (501) staff       (20)     1626 2023-05-11 16:35:10.000000 cvxportfolio-0.3.1/cvxportfolio/tests/base.py
+-rw-r--r--   0 enzo       (501) staff       (20)   156730 2023-05-11 16:35:10.000000 cvxportfolio-0.3.1/cvxportfolio/tests/returns.csv
+-rw-r--r--   0 enzo       (501) staff       (20)   149356 2023-05-11 16:35:10.000000 cvxportfolio-0.3.1/cvxportfolio/tests/sigmas.csv
+-rw-r--r--   0 enzo       (501) staff       (20)     8855 2023-05-11 16:35:10.000000 cvxportfolio-0.3.1/cvxportfolio/tests/test_constraints.py
+-rw-r--r--   0 enzo       (501) staff       (20)     8310 2023-05-16 16:47:47.000000 cvxportfolio-0.3.1/cvxportfolio/tests/test_costs.py
+-rw-r--r--   0 enzo       (501) staff       (20)    10329 2023-05-11 16:35:10.000000 cvxportfolio-0.3.1/cvxportfolio/tests/test_data.py
+-rw-r--r--   0 enzo       (501) staff       (20)     6718 2023-05-16 16:47:47.000000 cvxportfolio-0.3.1/cvxportfolio/tests/test_estimator.py
+-rw-r--r--   0 enzo       (501) staff       (20)     6567 2023-05-16 16:47:47.000000 cvxportfolio-0.3.1/cvxportfolio/tests/test_forecast.py
+-rw-r--r--   0 enzo       (501) staff       (20)    21909 2023-05-16 16:47:47.000000 cvxportfolio-0.3.1/cvxportfolio/tests/test_policies.py
+-rw-r--r--   0 enzo       (501) staff       (20)     4381 2023-05-16 16:47:47.000000 cvxportfolio-0.3.1/cvxportfolio/tests/test_returns.py
+-rw-r--r--   0 enzo       (501) staff       (20)     9070 2023-05-16 16:47:47.000000 cvxportfolio-0.3.1/cvxportfolio/tests/test_risks.py
+-rw-r--r--   0 enzo       (501) staff       (20)    10591 2023-05-16 16:47:47.000000 cvxportfolio-0.3.1/cvxportfolio/tests/test_simulator.py
+-rw-r--r--   0 enzo       (501) staff       (20)   116620 2023-05-11 16:35:10.000000 cvxportfolio-0.3.1/cvxportfolio/tests/volumes.csv
+drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-05-16 17:39:56.399470 cvxportfolio-0.3.1/cvxportfolio.egg-info/
+-rw-r--r--   0 enzo       (501) staff       (20)      329 2023-05-16 17:39:56.000000 cvxportfolio-0.3.1/cvxportfolio.egg-info/PKG-INFO
+-rw-r--r--   0 enzo       (501) staff       (20)      971 2023-05-16 17:39:56.000000 cvxportfolio-0.3.1/cvxportfolio.egg-info/SOURCES.txt
+-rw-r--r--   0 enzo       (501) staff       (20)        1 2023-05-16 17:39:56.000000 cvxportfolio-0.3.1/cvxportfolio.egg-info/dependency_links.txt
+-rw-r--r--   0 enzo       (501) staff       (20)       64 2023-05-16 17:39:56.000000 cvxportfolio-0.3.1/cvxportfolio.egg-info/requires.txt
+-rw-r--r--   0 enzo       (501) staff       (20)       13 2023-05-16 17:39:56.000000 cvxportfolio-0.3.1/cvxportfolio.egg-info/top_level.txt
+-rw-r--r--   0 enzo       (501) staff       (20)       38 2023-05-16 17:39:56.418868 cvxportfolio-0.3.1/setup.cfg
+-rw-r--r--   0 enzo       (501) staff       (20)      788 2023-05-16 17:39:49.000000 cvxportfolio-0.3.1/setup.py
```

### Comparing `cvxportfolio-0.3.0/LICENSE` & `cvxportfolio-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.0/README.md` & `cvxportfolio-0.3.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Cvxportfolio
 
 [![CVXportfolio on PyPI](https://img.shields.io/pypi/v/cvxportfolio.svg)](https://pypi.org/project/cvxportfolio/)
 [![Downloads](https://static.pepy.tech/personalized-badge/cvxportfolio?period=month&units=international_system&left_color=black&right_color=orange&left_text=PyPI%20downloads%20per%20month)](https://pepy.tech/project/cvxportfolio)
 [![Documentation Status](https://readthedocs.org/projects/cvxportfolio/badge/?version=latest)](https://cvxportfolio.readthedocs.io/en/latest/?badge=latest)
+[![Coverage Status](https://coveralls.io/repos/github/cvxgrp/cvxportfolio/badge.svg?branch=master)](https://coveralls.io/github/cvxgrp/cvxportfolio?branch=master)
 
 
 **WORK IN PROGRESS. Cvxportfolio is currently under development. We will freeze the user interface by end of 2023Q2 and release the first stable version by end of 2023Q3.**
 
 
 `cvxportfolio` is a python library for portfolio optimization and simulation
 based on the book [Multi-Period Trading via Convex Optimization](https://web.stanford.edu/~boyd/papers/pdf/cvx_portfolio.pdf)
```

### Comparing `cvxportfolio-0.3.0/cvxportfolio/__init__.py` & `cvxportfolio-0.3.1/cvxportfolio/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.3.0"
+__version__ = "0.3.1"
 from .data import *
 from .simulator import *
 from .result import *
 from .policies import *
 from .constraints import *
 from .costs import *
 from .returns import *
```

### Comparing `cvxportfolio-0.3.0/cvxportfolio/constraints.py` & `cvxportfolio-0.3.1/cvxportfolio/constraints.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.0/cvxportfolio/costs.py` & `cvxportfolio-0.3.1/cvxportfolio/costs.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.0/cvxportfolio/data.py` & `cvxportfolio-0.3.1/cvxportfolio/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,24 +112,34 @@
 
     This should not be used directly unless you know what you're doing.
     """
 
     @staticmethod
     def internal_process(data):
         """Manipulate yfinance data for better storing."""
+        
+        # nan-out nonpositive prices
+        data.loc[data["Open"] <= 0, 'Open'] = np.nan
+        data.loc[data["Close"] <= 0, "Close"] = np.nan
+        data.loc[data["High"] <= 0, "High"] = np.nan
+        data.loc[data["Low"] <= 0, "Low"] = np.nan
+        data.loc[data["Adj Close"] <= 0, "Adj Close"] = np.nan
+        
+        # nan-out negative volumes
+        data.loc[data["Volume"] < 0, 'Volume'] = np.nan
+        
         intraday_logreturn = np.log(data["Close"]) - np.log(data["Open"])
         close_to_close_logreturn = np.log(data["Adj Close"]).diff().shift(-1)
         open_to_open_logreturn = (
             close_to_close_logreturn + intraday_logreturn - intraday_logreturn.shift(-1)
         )
         data["Return"] = np.exp(open_to_open_logreturn) - 1
         del data["Adj Close"]
         # eliminate intraday data
-        data.loc[data.index[-1], ["High", "Low",
-                                  "Close", "Return", "Volume"]] = np.nan
+        data.loc[data.index[-1], ["High", "Low", "Close", "Return", "Volume"]] = np.nan
         return data
 
     @classmethod
     def download(cls, symbol, current=None, overlap=5, **kwargs):
         """Download single stock from Yahoo Finance.
 
         If data was already downloaded we only download
@@ -166,16 +176,16 @@
         on the day.
         """
         data["ValueVolume"] = data["Volume"] * data["Open"]
         del data["Volume"]
         # remove infty values
         data.iloc[:, :] = np.nan_to_num(data.values, copy=True, nan=np.nan, posinf=np.nan, neginf=np.nan)
         # remove extreme values
-        data.loc[data["Return"] < -.99, "Return"] = np.nan
-        data.loc[data["Return"] > .99, "Return"] = np.nan
+        # data.loc[data["Return"] < -.99, "Return"] = np.nan
+        # data.loc[data["Return"] > .99, "Return"] = np.nan
         return data
 
 
 class BaseDataStore(BaseData):
     """Base class for data storage systems.
 
     Attributes:
```

### Comparing `cvxportfolio-0.3.0/cvxportfolio/errors.py` & `cvxportfolio-0.3.1/cvxportfolio/errors.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.0/cvxportfolio/estimator.py` & `cvxportfolio-0.3.1/cvxportfolio/estimator.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,17 +140,18 @@
                     f"{self.__class__.__name__}.values_in_time result is a np.nan scalar."
                 )
             else:
                 return result
 
         if isinstance(result, np.ndarray):
             if np.any(np.isnan(result)) and not self.allow_nans:
-                raise MissingValuesError(
-                    f"{self.__class__.__name__}.values_in_time result is an array with np.nan's."
-                )
+                message = f"{self.__class__.__name__}.values_in_time result is an array with np.nan's."
+                if hasattr(self.data, 'columns') and len(self.data.columns) == len(result):
+                    message += "Specifically, the problem is with symbol(s)", list(self.data.columns[np.isnan(result)])
+                raise MissingValuesError(message)
             else:
                 return result
 
         raise DataError(
             f"{self.__class__.__name__}.values_in_time result is not a scalar or array."
         )
```

### Comparing `cvxportfolio-0.3.0/cvxportfolio/policies.py` & `cvxportfolio-0.3.1/cvxportfolio/policies.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.0/cvxportfolio/result.py` & `cvxportfolio-0.3.1/cvxportfolio/result.py`

 * *Files 14% similar despite different names*

```diff
@@ -35,22 +35,24 @@
     """Holds the data from a Backtest and producs metrics and plots."""
     
     # Periods per year.
     # When we generalize to intra- or multi-day 
     # trading we won't have this constant.
     PPY = 252
     
-    def __init__(self, h, u, z, tcost, hcost_stocks, hcost_cash, cash_returns):
+    def __init__(self, h, u, z, tcost, hcost_stocks, hcost_cash, cash_returns, policy_times, simulator_times):
         self.h = h
         self.u = u
         self.z = z
         self.tcost = tcost
         self.hcost_stocks = hcost_stocks
         self.hcost_cash = hcost_cash
         self.cash_returns = cash_returns
+        self.policy_times = policy_times
+        self.simulator_times = simulator_times
 
     @property
     def v(self):
         """The value of the portfolio over time."""
         return self.h.sum(axis=1)
 
     @property
@@ -62,15 +64,15 @@
     def w(self):
         """The weights of the portfolio over time."""
         return (self.h.T / self.v).T
 
     @property
     def leverage(self):
         """Portfolio leverage"""
-        return np.abs(self.w).sum(1)
+        return np.abs(self.w.iloc[:, :-1]).sum(1)
 
     @property
     def volatility(self):
         """The annualized, realized portfolio volatility."""
         return np.sqrt(self.PPY) * np.std(self.returns)
 
     @property
@@ -138,27 +140,31 @@
         """Turnover ||u_t||_1/v_t"""
         return np.abs(self.u.iloc[:,:-1]).sum(axis=1) / self.v.loc[self.u.index]
 
     @property
     def trading_days(self):
         """The fraction of days with nonzero turnover."""
         return (self.turnover.values > 0).sum() / self.turnover.size
-
+        
     @property
-    def max_drawdown(self):
-        """The maximum peak to trough drawdown in percent."""
-        val_arr = self.v.values
-        max_dd_so_far = 0
-        cur_max = val_arr[0]
-        for val in val_arr[1:]:
-            if val >= cur_max:
-                cur_max = val
-            elif 100 * (cur_max - val) / cur_max > max_dd_so_far:
-                max_dd_so_far = 100 * (cur_max - val) / cur_max
-        return max_dd_so_far
+    def drawdown(self):
+        return (1 - (self.v / self.v.cummax()))
+
+    # @property
+    # def max_drawdown(self):
+    #     """The maximum peak to trough drawdown in percent."""
+    #     val_arr = self.v.values
+    #     max_dd_so_far = 0
+    #     cur_max = val_arr[0]
+    #     for val in val_arr[1:]:
+    #         if val >= cur_max:
+    #             cur_max = val
+    #         elif 100 * (cur_max - val) / cur_max > max_dd_so_far:
+    #             max_dd_so_far = 100 * (cur_max - val) / cur_max
+    #     return max_dd_so_far
         
     @property
     def excess_returns(self):
         return self.returns - self.cash_returns
 
 
     def __repr__(self):
@@ -167,17 +173,32 @@
             "Initial timestamp": self.h.index[0],
             "Final timestamp": self.h.index[-1],
             "Total profit (PnL)": self.profit,
             "Annualized portfolio return (%)": self.returns.mean() * 100 * self.PPY,
             "Annualized excess return (%)": self.excess_returns.mean() * 100 * self.PPY,
             "Annualized excess risk (%)": self.excess_returns.std() * 100 * np.sqrt(self.PPY),
             "Sharpe ratio": self.sharpe_ratio,
-            "Max. drawdown (%)": self.max_drawdown,
+            "Max. drawdown (%)": self.drawdown.max() * 100,
+            "Average drawdown (%)": self.drawdown.mean() * 100,
+            "Daily Turnover (%)": self.turnover.mean() * 100,
             "Annualized Turnover (%)": self.turnover.mean() * 100 * self.PPY,
-            #"Average policy time (sec)": self.policy_time.mean(),
-            #"Average simulator time (sec)": self.simulation_time.mean(),
+            
+            "Average leverage (%)": self.leverage.mean() * 100,
+            "Max leverage (%)": self.leverage.max() * 100,
+            
+            "Average daily tcost (bp)": (self.tcost / self.v).mean()*1E4,
+            "Average daily tcost ($)": (self.tcost).mean(),
+            "Average daily stock borrow cost (bp)": (self.hcost_stocks / self.v).mean()*1E4,
+            "Average daily stock borrow cost ($)": (self.hcost_stocks).mean(),
+            "Average daily cash return or cost (bp)": (self.hcost_cash / self.v).mean()*1E4,
+            "Average daily cash return or cost ($)": (self.hcost_cash).mean(),
+            
+            "Average policy time (sec)": self.policy_times.mean(),
+            "Average simulator time (sec)": self.simulator_times.mean(),
+            
+            
             })
 
         return 'Backtest Result:\n' + pd.Series(data=data).to_string(float_format="{:,.3f}".format)
```

### Comparing `cvxportfolio-0.3.0/cvxportfolio/returns.py` & `cvxportfolio-0.3.1/cvxportfolio/returns.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 import numpy as np
 import pandas as pd
 
 
 from .costs import BaseCost, CombinedCosts
 from .risks import BaseRiskModel
 from .estimator import DataEstimator, ParameterEstimator
+from .forecast import HistoricalMeanReturn, HistoricalMeanError
 
 __all__ = [
     "ReturnsForecast",
     "ReturnsForecastError",
 ]
 
 
@@ -143,53 +144,55 @@
     def __init__(self, r_hat=None, #rolling=None, halflife=None, 
                 lastforcash=True, 
                 subtractshorts=True):
         
         if not r_hat is None:
             self.r_hat = DataEstimator(r_hat)
         else:
-            self.r_hat = None
+            self.r_hat = HistoricalMeanReturn(lastforcash=lastforcash)
             
-        self.lastforcash = True
+        # self.lastforcash = True
         self.subtractshorts = subtractshorts
         
         if self.subtractshorts:
             self.cash_return = cvx.Parameter(nonneg=True)
         
        
-    @classmethod # we make it a classmethod so that also covariances can use it
-    def update_full_mean(cls, past_returns, last_estimation, last_counts, last_time):
-
-        if last_time is None: # full estimation
-            estimation = past_returns.sum()
-            counts = past_returns.count()
-        else:
-            assert last_time == past_returns.index[-2]
-            estimation = last_estimation * last_counts + past_returns.iloc[-1].fillna(0.)
-            counts = last_counts + past_returns.iloc[-1:].count()
-
-        return estimation/counts, counts, past_returns.index[-1]
+    # @classmethod # we make it a classmethod so that also covariances can use it
+    # def update_full_mean(cls, past_returns, last_estimation, last_counts, last_time):
+    #
+    #     if last_time is None: # full estimation
+    #         estimation = past_returns.sum()
+    #         counts = past_returns.count()
+    #     else:
+    #         assert last_time == past_returns.index[-2]
+    #         estimation = last_estimation * last_counts + past_returns.iloc[-1].fillna(0.)
+    #         counts = last_counts + past_returns.iloc[-1:].count()
+    #
+    #     return estimation/counts, counts, past_returns.index[-1]
             
         
     def pre_evaluation(self, universe, backtest_times):
         
         self.r_hat_parameter = cvx.Parameter(len(universe))
         
     
     def values_in_time(self, t, past_returns, **kwargs):
         
         super().values_in_time(t=t, past_returns=past_returns, **kwargs)
         
-        if self.r_hat is None:
-            tmp = past_returns.mean()
-            if self.lastforcash:
-                tmp.iloc[-1] = past_returns.iloc[-1, -1]
-            self.r_hat_parameter.value = tmp.values
-        else:
-            self.r_hat_parameter.value = self.r_hat.current_value
+        # if self.r_hat is None:
+        #     tmp = past_returns.mean()
+        #     if self.lastforcash:
+        #         tmp.iloc[-1] = past_returns.iloc[-1, -1]
+        #     self.r_hat_parameter.value = tmp.values
+        # else:
+        #     self.r_hat_parameter.value = self.r_hat.current_value
+        
+        self.r_hat_parameter.value = self.r_hat.current_value
             
         if self.subtractshorts:
             self.cash_return.value = self.r_hat_parameter.value[-1]
 
         
     def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         if self.subtractshorts:
@@ -217,41 +220,41 @@
         errors on the returns forecasts (if Series),
         or varying in time (if DataFrame), 
         or fitted from the data as the standard deviation
         of the historical mean estimator 
     :type deltas_errors: pd.DataFrame or pd.Series or None
     """
 
-    def __init__(self, deltas=None, zeroforcash=True, # rolling=None, halflife=None
-        ):
+    def __init__(self, deltas=None):#, zeroforcash=True, # rolling=None, halflife=None
         
         if not deltas is None:
             self.deltas = DataEstimator(deltas)
         else:
-            self.deltas = None
-        self.zeroforcash = zeroforcash
+            self.deltas = HistoricalMeanError()#zeroforcash)
+        # self.zeroforcash = zeroforcash
 
             
     def pre_evaluation(self, universe, backtest_times):
         super().pre_evaluation(universe=universe, backtest_times=backtest_times)
-        self.deltas_parameter = cvx.Parameter(len(universe), nonneg=True)
+        self.deltas_parameter = cvx.Parameter(len(universe)-1, nonneg=True)
 
 
     def values_in_time(self, t, past_returns, **kwargs):
         super().values_in_time(t=t, past_returns=past_returns, **kwargs)
-        if self.deltas is None:
-            # if self.mode == 'full':
-            tmp = (past_returns.iloc[:,:].std() / np.sqrt(past_returns.iloc[:,:].count())).values
-            if self.zeroforcash:
-                tmp[-1] = 0.
-            self.deltas_parameter.value = tmp
-        else:
-            self.deltas_parameter.value = self.deltas.current_value
+        # if self.deltas is None:
+        #     # if self.mode == 'full':
+        #     tmp = (past_returns.iloc[:,:].std() / np.sqrt(past_returns.iloc[:,:].count())).values
+        #     if self.zeroforcash:
+        #         tmp[-1] = 0.
+        #     self.deltas_parameter.value = tmp
+        # else:
+        #     self.deltas_parameter.value = self.deltas.current_value
+        self.deltas_parameter.value = self.deltas.current_value
 
 
     def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         """Compile to cvxpy expression."""
-        return cvx.abs(w_plus_minus_w_bm).T @ self.deltas_parameter
+        return cvx.abs(w_plus_minus_w_bm[:-1]).T @ self.deltas_parameter
```

### Comparing `cvxportfolio-0.3.0/cvxportfolio/risks.py` & `cvxportfolio-0.3.1/cvxportfolio/risks.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 import cvxpy as cvx
 import numpy as np
 import pandas as pd
 
 from .costs import BaseCost
 from .errors import ForeCastError
+from .forecast import HistoricalVariance, HistoricalFactorizedCovariance
 
 logger = logging.getLogger(__name__)
 
 
 __all__ = [
     "FullCovariance",
     "DiagonalCovariance",
@@ -127,25 +128,29 @@
     # :type addmean: bool
     # """
 
     def __init__(self, Sigma=None, addmean=True):
 
         if not Sigma is None:
             self.Sigma = DataEstimator(Sigma)
+            self.alreadyfactorized = False
         else:
-            self.Sigma = Sigma
-        self.zeroforcash = True
-        self.addmean = addmean
+            self.Sigma = HistoricalFactorizedCovariance(# zeroforcash=True, 
+                addmean=addmean) #Sigma
+            self.alreadyfactorized = True
+            
+        # self.zeroforcash = True
+        # self.addmean = addmean
 
 
     def pre_evaluation(self, universe, backtest_times):
         super().pre_evaluation(universe, backtest_times)
         
         
-        self.Sigma_sqrt = cvx.Parameter((len(universe), len(universe)))#+self.addmean))
+        self.Sigma_sqrt = cvx.Parameter((len(universe)-1, len(universe)-1))#+self.addmean))
 
         #super().pre_evaluation(returns, volumes, start_time, end_time, **kwargs)
         
     # @classmethod
     # def get_count_matrix(cls, past_returns):
     #     """We obtain the matrix of non-null joint counts."""
     #     tmp = ~past_returns.isnull()
@@ -165,35 +170,36 @@
     #
     #     return estimation, counts, past_returns.index[-1]
 
     def values_in_time(self, t, past_returns, **kwargs):
         """Update forecast error risk here, and take square root of Sigma."""
         super().values_in_time(t=t, past_returns=past_returns, **kwargs)
         
-        if self.Sigma is None:
-            Sigma = past_returns.cov(ddof=0)
-            if self.addmean:
-                mean = past_returns.mean()
-                Sigma += np.outer(mean, mean)
-            if self.zeroforcash:
-                Sigma.iloc[:, -1] = 0
-                Sigma.iloc[-1, :] = 0
+        # if self.Sigma is None:
+        #     Sigma = past_returns.cov(ddof=0)
+        #     if self.addmean:
+        #         mean = past_returns.mean()
+        #         Sigma += np.outer(mean, mean)
+        #     if self.zeroforcash:
+        #         Sigma.iloc[:, -1] = 0
+        #         Sigma.iloc[-1, :] = 0
+        # else:
+        #     Sigma = self.Sigma.current_value
+
+        if self.alreadyfactorized:
+            self.Sigma_sqrt.value = self.Sigma.current_value
         else:
             Sigma = self.Sigma.current_value
-
-            
-        eigval, eigvec = np.linalg.eigh(Sigma)
-
-        eigval = np.maximum(eigval, 0.)
-        
-        self.Sigma_sqrt.value = eigvec @ np.diag(np.sqrt(eigval))
+            eigval, eigvec = np.linalg.eigh(Sigma)
+            eigval = np.maximum(eigval, 0.)
+            self.Sigma_sqrt.value = eigvec @ np.diag(np.sqrt(eigval))
 
     def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         # TODO change benchmark weights passing
-        self.cvxpy_expression = cvx.sum_squares(self.Sigma_sqrt.T @ w_plus_minus_w_bm)
+        self.cvxpy_expression = cvx.sum_squares(self.Sigma_sqrt.T @ w_plus_minus_w_bm[:-1])
     
         return self.cvxpy_expression
 
 class RiskForecastError(BaseRiskModel):
     """Risk forecast error. 
     
     Implements the model defined in page 31 of the book. Takes same arguments
@@ -202,45 +208,47 @@
     :param sigma_squares: per-stock variances, indexed by time if DataFrame.
         If None it will be fitted on past data.
     :type sigma_squares: pd.DataFrame or pd.Series or None
     """
 
     def __init__(self, sigma_squares=None):
         if sigma_squares is None:
-            self.sigma_squares = None
+            self.sigma_squares = HistoricalVariance(addmean=True) #None None
         else:
             self.sigma_squares = DataEstimator(sigma_squares)
         # self.standard_deviations = ParameterEstimator(standard_deviations)
-        self.zeroforcash=True
-        self.addmean=True
+        # self.zeroforcash=True
+        # self.addmean=True
         
     def pre_evaluation(self, universe, backtest_times):
         super().pre_evaluation(universe, backtest_times)
-        self.sigmas_parameter = cvx.Parameter(len(universe), nonneg=True)#+self.addmean))
+        self.sigmas_parameter = cvx.Parameter(len(universe)-1, nonneg=True)#+self.addmean))
 
     def values_in_time(self, t, past_returns, **kwargs):
         """Update forecast error risk here, and take square root of Sigma."""
         super().values_in_time(t=t, past_returns=past_returns)
         
-        if self.sigma_squares is None:
-            sigma_squares = past_returns.var(ddof=0)
-            if self.addmean:
-                mean = past_returns.mean()
-                sigma_squares += mean**2
-            if self.zeroforcash:
-                sigma_squares.iloc[-1] = 0.
-            sigma_squares = sigma_squares.values
-        else:
-            sigma_squares = self.sigma_squares.current_value
+        # if self.sigma_squares is None:
+        #     sigma_squares = past_returns.var(ddof=0)
+        #     if self.addmean:
+        #         mean = past_returns.mean()
+        #         sigma_squares += mean**2
+        #     if self.zeroforcash:
+        #         sigma_squares.iloc[-1] = 0.
+        #     sigma_squares = sigma_squares.values
+        # else:
+        #     sigma_squares = self.sigma_squares.current_value
+            
+        sigma_squares = self.sigma_squares.current_value
         
         self.sigmas_parameter.value = np.sqrt(sigma_squares)
 
     def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
 
-        return cvx.square(cvx.abs(w_plus_minus_w_bm).T @ self.sigmas_parameter)
+        return cvx.square(cvx.abs(w_plus_minus_w_bm[:-1]).T @ self.sigmas_parameter)
                 
                 
 
 
 class DiagonalCovariance(BaseRiskModel):
     """Diagonal covariance matrix, user-provided or fit from data.
 
@@ -249,44 +257,46 @@
     :type sigma_squares: pd.DataFrame or pd.Series or None 
     """
 
     def __init__(self, sigma_squares=None):
         if not sigma_squares is None:
             self.sigma_squares = DataEstimator(sigma_squares)
         else:
-            self.sigma_squares = None
-        self.zeroforcash = True
-        self.addmean = True
+            self.sigma_squares = HistoricalVariance(addmean=True) #None
+        #self.zeroforcash = True
+        #self.addmean = True
         # self.standard_deviations = ParameterEstimator(standard_deviations)
         
     def pre_evaluation(self, universe, backtest_times):
         super().pre_evaluation(universe, backtest_times)
-        self.sigmas_parameter = cvx.Parameter(len(universe)) #+self.addmean))
+        self.sigmas_parameter = cvx.Parameter(len(universe)-1) #+self.addmean))
 
     def values_in_time(self, t, past_returns, **kwargs):
         """Update forecast error risk here, and take square root of Sigma."""
         #super().values_in_time(t, current_weights, current_portfolio_value, past_returns, past_volumes, **kwargs)
         super().values_in_time(t=t, past_returns=past_returns, **kwargs)
         
-        if self.sigma_squares is None:
-            sigma_squares = past_returns.var(ddof=0)
-            if self.addmean:
-                mean = past_returns.mean()       
-                sigma_squares += mean**2
-            if self.zeroforcash:
-                sigma_squares[-1] = 0.
-            sigma_squares = sigma_squares.values
-        else:
-            sigma_squares = self.sigma_squares.current_value
+        # if self.sigma_squares is None:
+        #     sigma_squares = past_returns.var(ddof=0)
+        #     if self.addmean:
+        #         mean = past_returns.mean()
+        #         sigma_squares += mean**2
+        #     if self.zeroforcash:
+        #         sigma_squares[-1] = 0.
+        #     sigma_squares = sigma_squares.values
+        # else:
+        #     sigma_squares = self.sigma_squares.current_value
+        
+        sigma_squares = self.sigma_squares.current_value
 
         self.sigmas_parameter.value = np.sqrt(sigma_squares)
 
     def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
 
-        return cvx.sum_squares(cvx.multiply(w_plus_minus_w_bm, self.sigmas_parameter))
+        return cvx.sum_squares(cvx.multiply(w_plus_minus_w_bm[:-1], self.sigmas_parameter))
 
 
 class FactorModelCovariance(BaseRiskModel):
     """Factor model covariance, either user-provided or fitted from the data.
     
     It has the structure
     
@@ -317,91 +327,102 @@
     #     forecast_error_kappa (float or pd.Series): uncertainty on the
     #         assets' correlations. See the paper, pages 32-33.
 
     # """
 
     factor_Sigma = None
 
-    def __init__(self, F=None, d=None, num_factors=1, normalize=False):
+    def __init__(self, F=None, d=None, num_factors=1):#, normalize=False):
         self.F = F if F is None else ParameterEstimator(F) 
         self.d = d if d is None else DataEstimator(d) 
-        self.num_factors = num_factors
-        self.addmean = True
-        self.zeroforcash = True
-        self.normalize = normalize
-
-    @staticmethod
-    def build_low_rank_model(rets, num_factors=10, iters=10, normalize=True, shrink=True):
-        r"""Build a low rank risk model from past returns that include NaNs.
-    
-        This is an experimental procedure that may work well on past returns
-        matrices with few NaN values (say, below 20% of the total entries). 
-        If there are (many) NaNs, one should probably also use a rather 
-        large risk forecast error.
-        """
-        # rets = past_returns.iloc[:,:-1] # drop cash
-        nan_fraction = rets.isnull().sum().sum() / np.prod(rets.shape)
-        normalizer = np.sqrt((rets**2).mean()) 
-        if normalize:
-            normalized = rets/(normalizer + 1E-8)
-        else:
-            normalized = rets
-        if nan_fraction:
-            if nan_fraction > 0.1 and not shrink:
-                warnings.warn("Low rank model estimation on past returns with many NaNs should use the `shrink` option")
-            nan_implicit_imputation = pd.DataFrame(0., columns=normalized.columns, index = normalized.index)
-            for i in range(iters):
-                u, s, v = np.linalg.svd(normalized.fillna(nan_implicit_imputation), full_matrices=False)
-                nan_implicit_imputation = pd.DataFrame(
-                    (u[:, :num_factors] * (s[:num_factors] - s[num_factors] * shrink)) @ v[:num_factors], 
-                    columns = normalized.columns, index = normalized.index) 
+        if (self.F is None) or (self.d is None):
+            self.fit = True
+            self.Sigma = HistoricalFactorizedCovariance(addmean=True) #Sigma
         else:
-            u, s, v = np.linalg.svd(normalized, full_matrices=False)
-        F = v[:num_factors].T * s[:num_factors] / np.sqrt(len(rets))
-        if normalize:
-            F = pd.DataFrame(F.T * (normalizer.values + 1E-8), columns=normalizer.index)
-        else:
-            F = pd.DataFrame(F.T, columns=normalizer.index)
-        idyosyncratic = normalizer**2 - (F**2).sum(0)
-        if not np.all(idyosyncratic >= 0.):
-            raise ForeCastError("Low rank risk estimation with iterative SVD did not work.")
-        return F, idyosyncratic
+            self.fit = False
+        self.num_factors = num_factors
+        # self.addmean = True
+        # self.zeroforcash = True
+        # self.normalize = normalize
+
+    # @staticmethod
+    # def build_low_rank_model(rets, num_factors=10, iters=10, normalize=True, shrink=True):
+    #     r"""Build a low rank risk model from past returns that include NaNs.
+    #
+    #     This is an experimental procedure that may work well on past returns
+    #     matrices with few NaN values (say, below 20% of the total entries).
+    #     If there are (many) NaNs, one should probably also use a rather
+    #     large risk forecast error.
+    #     """
+    #     # rets = past_returns.iloc[:,:-1] # drop cash
+    #     nan_fraction = rets.isnull().sum().sum() / np.prod(rets.shape)
+    #     normalizer = np.sqrt((rets**2).mean())
+    #     if normalize:
+    #         normalized = rets/(normalizer + 1E-8)
+    #     else:
+    #         normalized = rets
+    #     if nan_fraction:
+    #         if nan_fraction > 0.1 and not shrink:
+    #             warnings.warn("Low rank model estimation on past returns with many NaNs should use the `shrink` option")
+    #         nan_implicit_imputation = pd.DataFrame(0., columns=normalized.columns, index = normalized.index)
+    #         for i in range(iters):
+    #             u, s, v = np.linalg.svd(normalized.fillna(nan_implicit_imputation), full_matrices=False)
+    #             nan_implicit_imputation = pd.DataFrame(
+    #                 (u[:, :num_factors] * (s[:num_factors] - s[num_factors] * shrink)) @ v[:num_factors],
+    #                 columns = normalized.columns, index = normalized.index)
+    #     else:
+    #         u, s, v = np.linalg.svd(normalized, full_matrices=False)
+    #     F = v[:num_factors].T * s[:num_factors] / np.sqrt(len(rets))
+    #     if normalize:
+    #         F = pd.DataFrame(F.T * (normalizer.values + 1E-8), columns=normalizer.index)
+    #     else:
+    #         F = pd.DataFrame(F.T, columns=normalizer.index)
+    #     idyosyncratic = normalizer**2 - (F**2).sum(0)
+    #     if not np.all(idyosyncratic >= 0.):
+    #         raise ForeCastError("Low rank risk estimation with iterative SVD did not work.")
+    #     return F, idyosyncratic
 
     def pre_evaluation(self, universe, backtest_times):
         super().pre_evaluation(universe, backtest_times)
         # super().pre_evaluation(returns, volumes, start_time, end_time, **kwargs)
-        self.idyosync_sqrt_parameter = cvx.Parameter(len(universe))
-        self.F_parameter = cvx.Parameter((self.num_factors, len(universe))) if self.F is None else self.F
+        self.idyosync_sqrt_parameter = cvx.Parameter(len(universe)-1)
+        self.F_parameter = cvx.Parameter((self.num_factors, len(universe)-1)) if self.F is None else self.F
         # if not (self.factor_Sigma is None):
         #     self.factor_Sigma_sqrt = cvx.Parameter(self.factor_Sigma.shape, PSD=True)
         # self.forecast_error_penalizer = cvx.Parameter(returns.shape[1], nonneg=True)
 
     def values_in_time(self, t, past_returns, **kwargs):
         super().values_in_time(t=t, past_returns=past_returns, **kwargs)
         
-        if self.F is None:
-            if not self.addmean:
-                past_returns = past_returns - past_returns.mean()
-            if self.zeroforcash:
-                past_returns = pd.DataFrame(past_returns, copy=True)
-                past_returns.iloc[:, -1] = 0.
-            F, d = self.build_low_rank_model(past_returns, num_factors=self.num_factors, normalize=self.normalize)
-            self.F_parameter.value = F.values
-            d = d.values
+        # if self.F is None:
+        #     if not self.addmean:
+        #         past_returns = past_returns - past_returns.mean()
+        #     if self.zeroforcash:
+        #         past_returns = pd.DataFrame(past_returns, copy=True)
+        #         past_returns.iloc[:, -1] = 0.
+        #     F, d = self.build_low_rank_model(past_returns, num_factors=self.num_factors, normalize=self.normalize)
+        #     self.F_parameter.value = F.values
+        #     d = d.values
+        # else:
+        #     d = self.d.current_value
+        if self.fit:
+            Sigmasqrt = self.Sigma.current_value
+            # numpy eigendecomposition has largest eigenvalues last
+            self.F_parameter.value = Sigmasqrt[:, -self.num_factors:].T
+            d = (Sigmasqrt[:, :-self.num_factors]**2).sum(1)
         else:
             d = self.d.current_value
-    
         self.idyosync_sqrt_parameter.value = np.sqrt(d)
 
 
     def compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
-        self.expression = cvx.sum_squares(cvx.multiply(self.idyosync_sqrt_parameter, w_plus_minus_w_bm))
+        self.expression = cvx.sum_squares(cvx.multiply(self.idyosync_sqrt_parameter, w_plus_minus_w_bm[:-1]))
         assert self.expression.is_dcp(dpp=True)
 
-        self.expression += cvx.sum_squares(self.F_parameter @ w_plus_minus_w_bm)
+        self.expression += cvx.sum_squares(self.F_parameter @ w_plus_minus_w_bm[:-1])
         assert self.expression.is_dcp(dpp=True)
 
         return self.expression
         
 
 class WorstCaseRisk(BaseRiskModel):
     """Select the most restrictive risk model for each value of the allocation vector.
```

### Comparing `cvxportfolio-0.3.0/cvxportfolio/simulator.py` & `cvxportfolio-0.3.1/cvxportfolio/simulator.py`

 * *Files 4% similar despite different names*

```diff
@@ -143,14 +143,15 @@
             transaction_cost_exponent=1.5,
             window_sigma_estimate=252,
             spread_on_borrowing_stocks_percent=.5,
             spread_on_long_positions_percent=None,
             dividends=0.,
             spread_on_lending_cash_percent=.5,
             spread_on_borrowing_cash_percent=.5,
+            min_history_for_inclusion=250,
             cash_key="USDOLLAR",
             base_location=BASE_LOCATION):
         """Initialize the Simulator and download data if necessary."""
         if not len(universe):
             if costs is None: # we allow old simulator syntax for the time being
                 if ((returns is None) or (volumes is None)):
                     raise SyntaxError(
@@ -186,14 +187,15 @@
         self.transaction_cost_coefficient_b = transaction_cost_coefficient_b
         self.transaction_cost_exponent = transaction_cost_exponent
         self.window_sigma_estimate = window_sigma_estimate
         self.spread_on_borrowing_stocks_percent = spread_on_borrowing_stocks_percent
         self.spread_on_long_positions_percent = spread_on_long_positions_percent
         self.spread_on_lending_cash_percent = spread_on_lending_cash_percent
         self.spread_on_borrowing_cash_percent = spread_on_borrowing_cash_percent
+        self.min_history_for_inclusion = min_history_for_inclusion
 
         # compute my DataEstimator(s)
         self.sigma_estimate = DataEstimator(
             self.returns.data.iloc[:, :-1].rolling(window=self.window_sigma_estimate, min_periods=1).std().shift(1))
 
     def prepare_data(self):
         """Build data from data storage and download interfaces.
@@ -225,15 +227,15 @@
         self.volumes = pd.DataFrame(
             {stock: self.database_accesses[stock].data['ValueVolume'] for stock in self.universe})
         
 
         # build prices
         self.prices = pd.DataFrame(
             {stock: self.database_accesses[stock].data['Open'] for stock in self.universe})
-        
+            
         
         # yfinance has some issues with most recent data; we patch it here but this
         # logic should go in .data
         if self.prices.iloc[-5:].isnull().any().any():
             drop_at = self.prices.iloc[-5:].isnull().any(axis=1).idxmax()
             self.prices = self.prices.loc[self.prices.index<drop_at]
             self.returns = self.returns.loc[self.returns.index<drop_at]
@@ -341,23 +343,30 @@
         
         # translate to weights
         current_portfolio_value = sum(h)
         current_weights = h / current_portfolio_value
         # print(t, current_portfolio_value)
 
         # get view of past data
-        past_returns = self.returns.data.loc[self.returns.data.index < t]
-        past_volumes = self.volumes.data.loc[self.volumes.data.index < t]
+        tidx = self.returns.data.index.get_loc(t)
+        # past_returns = self.returns.data.loc[self.returns.data.index < t]
+        #assert np.all(past_returns.fillna(0.) == self.returns.data.iloc[:tidx].fillna(0.))
+        past_returns = self.returns.data.iloc[:tidx]
+        #past_volumes = self.volumes.data.loc[self.volumes.data.index < t]
+        #assert np.all(past_volumes.fillna(0.) == self.volumes.data.iloc[:tidx].fillna(0.))
+        past_volumes = self.volumes.data.iloc[:tidx]
 
         # update internal estimators (spreads, dividends, volumes, ..., )
         super().values_in_time(t=t)
 
         # evaluate the policy
+        s = time.time()
         z = policy.values_in_time(t=t, current_weights=current_weights, current_portfolio_value=current_portfolio_value, 
             past_returns=past_returns, past_volumes=past_volumes, current_prices=self.prices.current_value, **kwargs)
+        policy_time = time.time() - s
         
         # for safety recompute cash
         z[-1] = -sum(z[:-1])
         assert sum(z) == 0.
         
         # trades in dollars
         u = z * current_portfolio_value
@@ -386,15 +395,15 @@
         # multiply positions by market returns (only non-cash)
         h_next = pd.Series(h_plus, copy=True)
         h_next[:-1] *= (1 + self.returns.current_value[:-1])
         
         # credit costs to cash (includes cash return)
         h_next[-1] = h_plus[-1] + (transaction_costs + holding_costs + cash_holding_costs)
             
-        return h_next, z, u, transaction_costs, holding_costs, cash_holding_costs, 
+        return h_next, z, u, transaction_costs, holding_costs, cash_holding_costs, policy_time
         
     def initialize_policy(self, policy, start_time, end_time):
         """Initialize the policy object.
         """
         policy.pre_evaluation(universe = self.returns.data.columns, 
                              backtest_times = self.returns.data.index[(self.returns.data.index<end_time) & 
                                  (self.returns.data.index>=start_time)])
@@ -406,24 +415,30 @@
         
         h_df = pd.DataFrame(columns=self.returns.data.columns)
         u = pd.DataFrame(columns=self.returns.data.columns)
         z = pd.DataFrame(columns=self.returns.data.columns)
         tcost = pd.Series(dtype=float)
         hcost_stocks = pd.Series(dtype=float)
         hcost_cash = pd.Series(dtype=float)
+        policy_times = pd.Series(dtype=float)
+        simulator_times = pd.Series(dtype=float)
         
         for t in self.returns.data.index[(self.returns.data.index >= start_time) & (self.returns.data.index < end_time)]:
             h_df.loc[t] = h
-            h, z.loc[t], u.loc[t], tcost.loc[t], hcost_stocks.loc[t], hcost_cash.loc[t] = \
+            s = time.time()
+            h, z.loc[t], u.loc[t], tcost.loc[t], hcost_stocks.loc[t], hcost_cash.loc[t], policy_times.loc[t] = \
                 self.simulate(t=t, h=h, policy=policy)
+            simulator_times.loc[t] = time.time() - s - policy_times.loc[t]
         
         h_df.loc[pd.Timestamp(end_time)] = h  
         
+        
         return BacktestResult(h=h_df, u=u, z=z, tcost=tcost, hcost_stocks=hcost_stocks, hcost_cash=hcost_cash, 
-            cash_returns=self.returns.data[self.cash_key].loc[u.index])
+            cash_returns=self.returns.data[self.cash_key].loc[u.index], 
+                policy_times=policy_times, simulator_times=simulator_times)
         
                   
                                  
     def backtest(self, policy, start_time, end_time=None, initial_value = 1E6, h=None, parallel=True):
         """Backtest one or more trading policy.
         
         If runnning in parallel you must be careful at how you use this method. If 
@@ -459,43 +474,44 @@
         """
         
         # turn policy and h into lists
         if not hasattr(policy, '__len__'):
             policy = [policy]
         
         if not hasattr(h, '__len__'):
-            h = [h]*len(policy)
+            h = [h] * len(policy)
             
         if not (len(policy) == len(h)):
             raise SyntaxError("If passing lists of policies and initial portfolios they must have the same length.")
         
         # discover start and end times
         start_time = pd.Series(self.returns.data.index >= start_time, self.returns.data.index).idxmax()
         if end_time is None:
             end_time  = self.returns.data.index[-1]
         else:
             end_time = self.returns.data.index[self.returns.data.index <= end_time][-1]
+            
+        # discard names that don't meet the min_history_for_inclusion
+        # history = (~self.returns.data.loc[self.returns.data.index < start_time].isnull()).sum()
         
         # initialize policies and get initial portfolios
         for i in range(len(policy)):
             self.initialize_policy(policy[i], start_time, end_time)
         
             if h[i] is None:
                 h[i] = pd.Series(0., self.returns.data.columns)
                 h[i][-1] = initial_value
                 
-        def parallel_runner(zipped):
+        def nonparallel_runner(zipped):
             return self._single_backtest(zipped[0], start_time, end_time, zipped[1])
-            
-        # parallel_worker(policy, simulator, start_time, end_time, h)
-        
+                    
         
         # decide if run in parallel or not
         if (not parallel) or len(policy) == 1:
-            result = list(map(parallel_runner, zip(policy, h)))
+            result = list(map(nonparallel_runner, zip(policy, h)))
         else:
             with Pool() as p:
                 # if not __name__ == '__main__':
                 #     raise SyntaxError('When executing parallel backtests, the Simulator should be instantiated ')
                 result = p.starmap(parallel_worker, zip(policy, [self] * len(policy), [start_time] * len(policy), [end_time] * len(policy), h))
                 
         if len(result) == 1:
```

### Comparing `cvxportfolio-0.3.0/cvxportfolio/tests/base.py` & `cvxportfolio-0.3.1/cvxportfolio/tests/base.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.0/cvxportfolio/tests/returns.csv` & `cvxportfolio-0.3.1/cvxportfolio/tests/returns.csv`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.0/cvxportfolio/tests/sigmas.csv` & `cvxportfolio-0.3.1/cvxportfolio/tests/sigmas.csv`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.0/cvxportfolio/tests/test_constraints.py` & `cvxportfolio-0.3.1/cvxportfolio/tests/test_constraints.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.0/cvxportfolio/tests/test_costs.py` & `cvxportfolio-0.3.1/cvxportfolio/tests/test_costs.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         # n = len(self.returns.columns)
         # wplus = cvx.Variable(n)
         self.w_plus_minus_w_bm.value = np.random.uniform(size=self.N)
         self.w_plus_minus_w_bm.value /= sum(self.w_plus_minus_w_bm.value)
         t = self.returns.index[1]
 
         cost1 = DiagonalCovariance()
-        cost2 = FullCovariance(self.returns.iloc[:, :].T @ self.returns.iloc[:, :] / len(self.returns))
+        cost2 = FullCovariance(self.returns.iloc[:, :-1].T @ self.returns.iloc[:, :-1] / len(self.returns))
         cost3 = cost1 + cost2
 
         cost3.pre_evaluation(universe=self.returns.columns, backtest_times=self.returns.index)
         expr3 = cost3.compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
         expr1 = cost1.compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
         expr2 = cost2.compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
         cost3.values_in_time(t=t, past_returns=self.returns.loc[self.returns.index < t])
```

### Comparing `cvxportfolio-0.3.0/cvxportfolio/tests/test_data.py` & `cvxportfolio-0.3.1/cvxportfolio/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.0/cvxportfolio/tests/test_estimator.py` & `cvxportfolio-0.3.1/cvxportfolio/tests/test_estimator.py`

 * *Files 0% similar despite different names*

```diff
@@ -166,7 +166,11 @@
         estimator = ParameterEstimator(data)
         self.assertTrue( not hasattr(estimator, "value"))
         estimator.pre_evaluation(universe=None, backtest_times=timeindex)
         # assert hasattr(estimator, 'parameter')
         self.assertTrue( hasattr(estimator, "value"))
         estimator.values_in_time("2022-01-05")
         self.assertTrue( np.all(estimator.value == data.loc["2022-01-05"]))
+        
+if __name__ == '__main__':
+    unittest.main()
+
```

### Comparing `cvxportfolio-0.3.0/cvxportfolio/tests/test_policies.py` & `cvxportfolio-0.3.1/cvxportfolio/tests/test_policies.py`

 * *Files 1% similar despite different names*

```diff
@@ -301,17 +301,19 @@
         cvxportfolio_result = pd.Series(result, self.returns.columns)
 
         print(cvxportfolio_result)
         
         # print(np.linalg.eigh(self.returns.iloc[:121, :-1].cov().values)[0])
 
         # REPLICATE WITH CVXPY
+        
+        COV = self.returns.iloc[:121, :-1].cov(ddof=0).values #+ np.outer(self.returns.iloc[:121, :-1].mean(), self.returns.iloc[:121, :-1].mean())
         w = cvx.Variable(self.N)
         cvx.Problem(cvx.Maximize(w.T @ self.returns.iloc[:121].mean().values -
-                                 2 * cvx.quad_form(w[:-1], self.returns.iloc[:121, :-1].cov(ddof=0).values) -
+                                 2 * cvx.quad_form(w[:-1], COV) -
                                  5 * 1E-4 * cvx.sum(cvx.abs(w - curw)[:-1])
                                  ),
                     [w >= 0, w <= 1, sum(w) == 1]
                     ).solve(solver='ECOS')
 
         cvxpy_result = pd.Series(w.value - curw, self.returns.columns)
```

### Comparing `cvxportfolio-0.3.0/cvxportfolio/tests/test_returns.py` & `cvxportfolio-0.3.1/cvxportfolio/tests/test_returns.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,36 +67,36 @@
         self.w_plus.value /= sum(self.w_plus.value)
         myforecast = self.returns.loc[self.returns.index < t].mean()
         myforecast.iloc[-1] = self.returns.iloc[122, -1]
         self.assertTrue(np.isclose(cvxpy_expression.value, self.w_plus.value @ myforecast))
         
     def test_returns_forecast_error(self):
 
-        delta = self.returns.std() / np.sqrt(len(self.returns))
-        delta.iloc[-1] = 0
+        delta = self.returns.iloc[:, :-1].std(ddof=0) / np.sqrt(len(self.returns))
+        # delta.iloc[-1] = 0
 
         error_risk = ReturnsForecastError(delta)
         cvxpy_expression = self.boilerplate(error_risk)
         error_risk.values_in_time(t='ciao', past_returns='hello')
 
         self.w_plus_minus_w_bm.value = np.random.randn(self.N)
-        self.assertTrue(np.isclose(cvxpy_expression.value, np.abs(self.w_plus_minus_w_bm.value) @ delta))
+        self.assertTrue(np.isclose(cvxpy_expression.value, np.abs(self.w_plus_minus_w_bm.value[:-1]) @ delta))
 
 
     def test_full_returns_forecast_error(self):
 
         error_risk = ReturnsForecastError()
         cvxpy_expression = self.boilerplate(error_risk)
         t = self.returns.index[123]
         past_returns = self.returns.loc[self.returns.index < t]
         
         error_risk.values_in_time(t=t, past_returns = past_returns)
         self.w_plus_minus_w_bm.value = np.random.randn(self.N)
         
-        delta = past_returns.std() / np.sqrt(past_returns.count())
+        delta = past_returns.std(ddof=0) / np.sqrt(past_returns.count())
 
         print(cvxpy_expression.value)
         print(np.abs(self.w_plus_minus_w_bm.value[:-1]) @ delta[:-1])
         self.assertTrue(np.isclose(cvxpy_expression.value, np.abs(self.w_plus_minus_w_bm.value[:-1]) @ delta[:-1]))
```

### Comparing `cvxportfolio-0.3.0/cvxportfolio/tests/test_risks.py` & `cvxportfolio-0.3.1/cvxportfolio/tests/test_risks.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,28 +38,28 @@
         
     def boilerplate(self, model):
         model.pre_evaluation(universe=self.returns.columns, backtest_times=self.returns.index)
         return model.compile_to_cvxpy(self.w_plus, self.z, self.w_plus_minus_w_bm)
 
 
     def test_full_sigma(self):
-        historical_covariances = self.returns.rolling(50).cov(ddof=0).dropna()
+        historical_covariances = self.returns.iloc[:, :-1].rolling(50).cov(ddof=0).dropna()
         risk_model = FullCovariance(historical_covariances)
         
         cvxpy_expression = self.boilerplate(risk_model)
 
         self.assertTrue(cvxpy_expression.is_convex())
 
         t = historical_covariances.index[123][0]
         self.w_plus_minus_w_bm.value = np.random.randn(self.N)
 
         risk_model.values_in_time(t=t, past_returns='Hello!')
 
-        self.assertTrue(np.isclose(cvxpy_expression.value, self.w_plus_minus_w_bm.value @
-                          historical_covariances.loc[t] @ self.w_plus_minus_w_bm.value))
+        self.assertTrue(np.isclose(cvxpy_expression.value, self.w_plus_minus_w_bm.value[:-1] @
+                          historical_covariances.loc[t] @ self.w_plus_minus_w_bm.value[:-1]))
                                
     def test_full_estimated_sigma(self):
 
         risk_model = FullCovariance()
         
         cvxpy_expression = self.boilerplate(risk_model)
         self.assertTrue(cvxpy_expression.is_convex())
@@ -87,26 +87,26 @@
                           self.w_plus_minus_w_bm.value[:-1] @ should_be @ self.w_plus_minus_w_bm.value[:-1]))
                           
     def test_diagonal_covariance(self):
 
         # N = returns.shape[1]
         # returns.iloc[:, -1] = 0.
 
-        historical_variances = self.returns.rolling(50).var().shift(1).dropna()
+        historical_variances = self.returns.iloc[:,:-1].rolling(50).var().shift(1).dropna()
         risk_model = DiagonalCovariance(historical_variances)
         cvxpy_expression = self.boilerplate(risk_model)
         self.assertTrue(cvxpy_expression.is_convex())
 
         t = historical_variances.index[123]
         self.w_plus_minus_w_bm.value = np.random.randn(self.N) 
 
         risk_model.values_in_time(t, past_returns='hello')
 
-        self.assertTrue(np.isclose(cvxpy_expression.value, self.w_plus_minus_w_bm.value @
-                          np.diag(historical_variances.loc[t]) @ self.w_plus_minus_w_bm.value))
+        self.assertTrue(np.isclose(cvxpy_expression.value, self.w_plus_minus_w_bm.value[:-1] @
+                          np.diag(historical_variances.loc[t]) @ self.w_plus_minus_w_bm.value[:-1]))
 
     def test_full_diagonal_covariance(self):
 
         risk_model = DiagonalCovariance()
         cvxpy_expression = self.boilerplate(risk_model)
         self.assertTrue(cvxpy_expression.is_convex())
 
@@ -120,32 +120,32 @@
         
         self.assertTrue(np.isclose(cvxpy_expression.value, self.w_plus_minus_w_bm.value @
                           np.diag(should_be) @ self.w_plus_minus_w_bm.value))
 
 
     def test_forecast_error(self):
 
-        historical_variances = (self.returns**2).rolling(50).mean().shift(1).dropna()
+        historical_variances = (self.returns.iloc[:, :-1]**2).rolling(50).mean().shift(1).dropna()
         
         risk_model = RiskForecastError(historical_variances)
         cvxpy_expression = self.boilerplate(risk_model)
         
         self.assertTrue(cvxpy_expression.is_convex())
 
         t = historical_variances.index[123]
         
         self.w_plus_minus_w_bm.value = np.random.randn(self.N) 
 
         risk_model.values_in_time(t, past_returns='hello')
 
         print(cvxpy_expression.value)
-        print((np.abs(self.w_plus_minus_w_bm.value) @ np.sqrt(historical_variances.loc[t]))**2)
+        print((np.abs(self.w_plus_minus_w_bm.value[:-1]) @ np.sqrt(historical_variances.loc[t]))**2)
         self.assertTrue(np.isclose(cvxpy_expression.value, 
         
-        (np.abs(self.w_plus_minus_w_bm.value) @ np.sqrt(historical_variances.loc[t]))**2
+        (np.abs(self.w_plus_minus_w_bm.value[:-1]) @ np.sqrt(historical_variances.loc[t]))**2
         
         ))
 
     def test_full_forecast_error(self):
 
         risk_model = RiskForecastError()
         cvxpy_expression = self.boilerplate(risk_model)
@@ -164,31 +164,31 @@
         
         (np.abs(self.w_plus_minus_w_bm.value) @ np.sqrt(should_be))**2
         
         ))
         
     def test_low_rank_covariance(self):
         
-        F = pd.DataFrame(np.random.randn(2, self.N), columns=self.returns.columns)
-        d = pd.Series(np.random.uniform(self.N), self.returns.columns)
+        F = pd.DataFrame(np.random.randn(2, self.N-1), columns=self.returns.columns[:-1])
+        d = pd.Series(np.random.uniform(size=(self.N-1)), self.returns.columns[:-1])
         risk_model = FactorModelCovariance(F=F, d=d)
         
         cvxpy_expression = self.boilerplate(risk_model)
         self.assertTrue(cvxpy_expression.is_convex())
         
         risk_model.values_in_time(t=self.returns.index[12], past_returns='hello')
         self.w_plus_minus_w_bm.value = np.random.randn(self.N)
         
         self.assertTrue(np.isclose(cvxpy_expression.value, 
-            self.w_plus_minus_w_bm.value @ np.diag(d) @ self.w_plus_minus_w_bm.value + \
-                ((F @ self.w_plus_minus_w_bm.value)**2).sum()))
+            self.w_plus_minus_w_bm.value[:-1] @ np.diag(d) @ self.w_plus_minus_w_bm.value[:-1] + \
+                ((F @ self.w_plus_minus_w_bm.value[:-1])**2).sum()))
                 
     def test_estimated_low_rank_covariance(self):
         
-        risk_model = FactorModelCovariance(normalize=False)
+        risk_model = FactorModelCovariance()#normalize=False)
         
         cvxpy_expression = self.boilerplate(risk_model)
         self.assertTrue(cvxpy_expression.is_convex())
         
         t = pd.Timestamp('2014-06-02')
         
         past = self.returns.loc[self.returns.index < t]
```

### Comparing `cvxportfolio-0.3.0/cvxportfolio/tests/test_simulator.py` & `cvxportfolio-0.3.1/cvxportfolio/tests/test_simulator.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,15 +174,15 @@
             h = np.random.randn(3)*10000
             h[-1] = 10000 - sum(h[:-1])
             h0 = pd.Series(h, simulator.returns.data.columns)
             h = pd.Series(h0, copy=True)
             simulator.initialize_policy(policy, start_time, end_time)
             for t in simulator.returns.data.index[(simulator.returns.data.index >= start_time) & (simulator.returns.data.index <= end_time)]:
                 oldcash = h[-1]
-                h, z, u, tcost, stock_hcost, cash_hcost = simulator.simulate(t=t, h=h, policy=policy)
+                h, z, u, tcost, stock_hcost, cash_hcost, timer = simulator.simulate(t=t, h=h, policy=policy)
                 assert tcost == 0.
                 if np.all(h0[:2] > 0):
                     assert stock_hcost == 0.
                 assert np.isclose(oldcash + stock_hcost + cash_hcost, h[-1])
             
             simh = h0[:-1] * simulator.prices.data.loc[pd.Timestamp(end_time) + pd.Timedelta('1d')] / simulator.prices.data.loc[start_time]
             self.assertTrue(np.allclose(simh, h[:-1]))
@@ -196,15 +196,15 @@
             h = np.random.randn(3)*10000
             h[-1] = 10000 - sum(h[:-1])
             h0 = pd.Series(h, simulator.returns.data.columns)
             h = pd.Series(h0, copy=True)
             simulator.initialize_policy(policy, start_time, end_time)
             for t in simulator.returns.data.index[(simulator.returns.data.index >= start_time) & (simulator.returns.data.index <= end_time)]:
                 oldcash = h[-1]
-                h, z, u, tcost, stock_hcost, cash_hcost = simulator.simulate(t=t, h=h, policy=policy)
+                h, z, u, tcost, stock_hcost, cash_hcost, timer = simulator.simulate(t=t, h=h, policy=policy)
                 print(h)
                 print(tcost, stock_hcost, cash_hcost)
             
             self.assertTrue(np.all(np.abs(h[:-1]) < simulator.prices.data.loc[end_time]))
             
     def test_backtest(self):
         pol = cp.SinglePeriodOptimization(cp.ReturnsForecast() -
```

### Comparing `cvxportfolio-0.3.0/cvxportfolio/tests/volumes.csv` & `cvxportfolio-0.3.1/cvxportfolio/tests/volumes.csv`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.3.0/cvxportfolio.egg-info/SOURCES.txt` & `cvxportfolio-0.3.1/cvxportfolio.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 setup.py
 cvxportfolio/__init__.py
 cvxportfolio/constraints.py
 cvxportfolio/costs.py
 cvxportfolio/data.py
 cvxportfolio/errors.py
 cvxportfolio/estimator.py
+cvxportfolio/forecast.py
 cvxportfolio/policies.py
 cvxportfolio/result.py
 cvxportfolio/returns.py
 cvxportfolio/risks.py
 cvxportfolio/simulator.py
 cvxportfolio.egg-info/PKG-INFO
 cvxportfolio.egg-info/SOURCES.txt
@@ -22,12 +23,13 @@
 cvxportfolio/tests/base.py
 cvxportfolio/tests/returns.csv
 cvxportfolio/tests/sigmas.csv
 cvxportfolio/tests/test_constraints.py
 cvxportfolio/tests/test_costs.py
 cvxportfolio/tests/test_data.py
 cvxportfolio/tests/test_estimator.py
+cvxportfolio/tests/test_forecast.py
 cvxportfolio/tests/test_policies.py
 cvxportfolio/tests/test_returns.py
 cvxportfolio/tests/test_risks.py
 cvxportfolio/tests/test_simulator.py
 cvxportfolio/tests/volumes.csv
```

### Comparing `cvxportfolio-0.3.0/setup.py` & `cvxportfolio-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='cvxportfolio',
-    version='0.3.0',
+    version='0.3.1',
     author='Enzo Busseti, Stephen Boyd, Steven Diamond, BlackRock Inc.',
     maintainer='Enzo Busseti',
     author_email='enzo.busseti@gmail.com',
     packages=['cvxportfolio',
               'cvxportfolio.tests'],
     package_dir={'cvxportfolio': 'cvxportfolio'},
     package_data={'cvxportfolio': [
```

