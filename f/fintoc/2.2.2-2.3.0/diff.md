# Comparing `tmp/fintoc-2.2.2.tar.gz` & `tmp/fintoc-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fintoc-2.2.2.tar", max compression
+gzip compressed data, was "fintoc-2.3.0.tar", max compression
```

## Comparing `fintoc-2.2.2.tar` & `fintoc-2.3.0.tar`

### file list

```diff
@@ -1,48 +1,52 @@
--rw-r--r--   0        0        0     1492 2022-01-04 13:44:43.755433 fintoc-2.2.2/LICENSE.md
--rw-r--r--   0        0        0    14987 2022-01-04 13:44:43.755433 fintoc-2.2.2/README.md
--rw-r--r--   0        0        0      116 2022-01-04 13:44:43.755433 fintoc-2.2.2/fintoc/__init__.py
--rw-r--r--   0        0        0     1940 2022-01-04 13:44:43.755433 fintoc-2.2.2/fintoc/client.py
--rw-r--r--   0        0        0      209 2022-01-04 13:44:43.755433 fintoc-2.2.2/fintoc/constants.py
--rw-r--r--   0        0        0      844 2022-01-04 13:44:43.755433 fintoc-2.2.2/fintoc/core.py
--rw-r--r--   0        0        0     1259 2022-01-04 13:44:43.755433 fintoc-2.2.2/fintoc/errors.py
--rw-r--r--   0        0        0      520 2022-01-04 13:44:43.755433 fintoc-2.2.2/fintoc/managers/__init__.py
--rw-r--r--   0        0        0      220 2022-01-04 13:44:43.755433 fintoc-2.2.2/fintoc/managers/accounts_manager.py
--rw-r--r--   0        0        0      213 2022-01-04 13:44:43.755433 fintoc-2.2.2/fintoc/managers/invoices_manager.py
--rw-r--r--   0        0        0      734 2022-01-04 13:44:43.755433 fintoc-2.2.2/fintoc/managers/links_manager.py
--rw-r--r--   0        0        0      223 2022-01-04 13:44:43.755433 fintoc-2.2.2/fintoc/managers/movements_manager.py
--rw-r--r--   0        0        0      256 2022-01-04 13:44:43.755433 fintoc-2.2.2/fintoc/managers/payment_intents_manager.py
--rw-r--r--   0        0        0      256 2022-01-04 13:44:43.755433 fintoc-2.2.2/fintoc/managers/refresh_intents_manager.py
--rw-r--r--   0        0        0      239 2022-01-04 13:44:43.755433 fintoc-2.2.2/fintoc/managers/subscriptions_manager.py
--rw-r--r--   0        0        0      229 2022-01-04 13:44:43.755433 fintoc-2.2.2/fintoc/managers/tax_returns_manager.py
--rw-r--r--   0        0        0      284 2022-01-04 13:44:43.755433 fintoc-2.2.2/fintoc/managers/webhook_endpoints_manager.py
--rw-r--r--   0        0        0      133 2022-01-04 13:44:43.755433 fintoc-2.2.2/fintoc/mixins/__init__.py
--rw-r--r--   0        0        0     5172 2022-01-04 13:44:43.755433 fintoc-2.2.2/fintoc/mixins/manager_mixin.py
--rw-r--r--   0        0        0     2873 2022-01-04 13:44:43.755433 fintoc-2.2.2/fintoc/mixins/resource_mixin.py
--rw-r--r--   0        0        0     1772 2022-01-04 13:44:43.755433 fintoc-2.2.2/fintoc/paginator.py
--rw-r--r--   0        0        0     1892 2022-01-04 13:44:43.755433 fintoc-2.2.2/fintoc/resource_handlers.py
--rw-r--r--   0        0        0      829 2022-01-04 13:44:43.755433 fintoc-2.2.2/fintoc/resources/__init__.py
--rw-r--r--   0        0        0      838 2022-01-04 13:44:43.755433 fintoc-2.2.2/fintoc/resources/account.py
--rw-r--r--   0        0        0      155 2022-01-04 13:44:43.755433 fintoc-2.2.2/fintoc/resources/balance.py
--rw-r--r--   0        0        0      176 2022-01-04 13:44:43.755433 fintoc-2.2.2/fintoc/resources/generic_fintoc_resource.py
--rw-r--r--   0        0        0      152 2022-01-04 13:44:43.755433 fintoc-2.2.2/fintoc/resources/income.py
--rw-r--r--   0        0        0      167 2022-01-04 13:44:43.755433 fintoc-2.2.2/fintoc/resources/institution.py
--rw-r--r--   0        0        0      189 2022-01-04 13:44:43.755433 fintoc-2.2.2/fintoc/resources/institution_invoice.py
--rw-r--r--   0        0        0      196 2022-01-04 13:44:43.755433 fintoc-2.2.2/fintoc/resources/institution_tax_return.py
--rw-r--r--   0        0        0      242 2022-01-04 13:44:43.755433 fintoc-2.2.2/fintoc/resources/invoice.py
--rw-r--r--   0        0        0     2865 2022-01-04 13:44:43.755433 fintoc-2.2.2/fintoc/resources/link.py
--rw-r--r--   0        0        0      278 2022-01-04 13:44:43.755433 fintoc-2.2.2/fintoc/resources/movement.py
--rw-r--r--   0        0        0      165 2022-01-04 13:44:43.755433 fintoc-2.2.2/fintoc/resources/other_taxes.py
--rw-r--r--   0        0        0      294 2022-01-04 13:44:43.755433 fintoc-2.2.2/fintoc/resources/payment_intent.py
--rw-r--r--   0        0        0      174 2022-01-04 13:44:43.755433 fintoc-2.2.2/fintoc/resources/refresh_intent.py
--rw-r--r--   0        0        0      180 2022-01-04 13:44:43.755433 fintoc-2.2.2/fintoc/resources/services_invoice.py
--rw-r--r--   0        0        0      170 2022-01-04 13:44:43.755433 fintoc-2.2.2/fintoc/resources/subscription.py
--rw-r--r--   0        0        0      162 2022-01-04 13:44:43.755433 fintoc-2.2.2/fintoc/resources/tax_return.py
--rw-r--r--   0        0        0      158 2022-01-04 13:44:43.755433 fintoc-2.2.2/fintoc/resources/taxpayer.py
--rw-r--r--   0        0        0      171 2022-01-04 13:44:43.755433 fintoc-2.2.2/fintoc/resources/tobacco_taxes.py
--rw-r--r--   0        0        0      180 2022-01-04 13:44:43.755433 fintoc-2.2.2/fintoc/resources/transfer_account.py
--rw-r--r--   0        0        0      180 2022-01-04 13:44:43.755433 fintoc-2.2.2/fintoc/resources/webhook_endpoint.py
--rw-r--r--   0        0        0     3353 2022-01-04 13:44:43.755433 fintoc-2.2.2/fintoc/utils.py
--rw-r--r--   0        0        0      125 2022-01-04 13:44:43.755433 fintoc-2.2.2/fintoc/version.py
--rw-r--r--   0        0        0      800 2022-01-04 13:44:43.755433 fintoc-2.2.2/pyproject.toml
--rw-r--r--   0        0        0    16121 2022-01-04 13:44:51.832159 fintoc-2.2.2/setup.py
--rw-r--r--   0        0        0    15861 2022-01-04 13:44:51.832845 fintoc-2.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1492 2023-05-16 19:25:32.957477 fintoc-2.3.0/LICENSE.md
+-rw-r--r--   0        0        0    15310 2023-05-16 19:25:32.957477 fintoc-2.3.0/README.md
+-rw-r--r--   0        0        0      116 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/__init__.py
+-rw-r--r--   0        0        0     1940 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/client.py
+-rw-r--r--   0        0        0      209 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/constants.py
+-rw-r--r--   0        0        0     1209 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/core.py
+-rw-r--r--   0        0        0     1259 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/errors.py
+-rw-r--r--   0        0        0      633 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/managers/__init__.py
+-rw-r--r--   0        0        0      220 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/managers/accounts_manager.py
+-rw-r--r--   0        0        0      225 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/managers/charges_manager.py
+-rw-r--r--   0        0        0      213 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/managers/invoices_manager.py
+-rw-r--r--   0        0        0      734 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/managers/links_manager.py
+-rw-r--r--   0        0        0      223 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/managers/movements_manager.py
+-rw-r--r--   0        0        0      256 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/managers/payment_intents_manager.py
+-rw-r--r--   0        0        0      256 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/managers/refresh_intents_manager.py
+-rw-r--r--   0        0        0      276 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/managers/subscription_intents_manager.py
+-rw-r--r--   0        0        0      239 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/managers/subscriptions_manager.py
+-rw-r--r--   0        0        0      229 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/managers/tax_returns_manager.py
+-rw-r--r--   0        0        0      284 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/managers/webhook_endpoints_manager.py
+-rw-r--r--   0        0        0      133 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/mixins/__init__.py
+-rw-r--r--   0        0        0     5172 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/mixins/manager_mixin.py
+-rw-r--r--   0        0        0     2873 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/mixins/resource_mixin.py
+-rw-r--r--   0        0        0     1772 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/paginator.py
+-rw-r--r--   0        0        0     1892 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/resource_handlers.py
+-rw-r--r--   0        0        0      908 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/resources/__init__.py
+-rw-r--r--   0        0        0      838 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/resources/account.py
+-rw-r--r--   0        0        0      155 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/resources/balance.py
+-rw-r--r--   0        0        0      152 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/resources/charge.py
+-rw-r--r--   0        0        0      176 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/resources/generic_fintoc_resource.py
+-rw-r--r--   0        0        0      152 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/resources/income.py
+-rw-r--r--   0        0        0      167 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/resources/institution.py
+-rw-r--r--   0        0        0      189 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/resources/institution_invoice.py
+-rw-r--r--   0        0        0      196 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/resources/institution_tax_return.py
+-rw-r--r--   0        0        0      242 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/resources/invoice.py
+-rw-r--r--   0        0        0     2865 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/resources/link.py
+-rw-r--r--   0        0        0      278 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/resources/movement.py
+-rw-r--r--   0        0        0      165 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/resources/other_taxes.py
+-rw-r--r--   0        0        0      294 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/resources/payment_intent.py
+-rw-r--r--   0        0        0      174 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/resources/refresh_intent.py
+-rw-r--r--   0        0        0      180 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/resources/services_invoice.py
+-rw-r--r--   0        0        0      170 2023-05-16 19:25:32.957477 fintoc-2.3.0/fintoc/resources/subscription.py
+-rw-r--r--   0        0        0      189 2023-05-16 19:25:32.961477 fintoc-2.3.0/fintoc/resources/subscription_intent.py
+-rw-r--r--   0        0        0      162 2023-05-16 19:25:32.961477 fintoc-2.3.0/fintoc/resources/tax_return.py
+-rw-r--r--   0        0        0      158 2023-05-16 19:25:32.961477 fintoc-2.3.0/fintoc/resources/taxpayer.py
+-rw-r--r--   0        0        0      171 2023-05-16 19:25:32.961477 fintoc-2.3.0/fintoc/resources/tobacco_taxes.py
+-rw-r--r--   0        0        0      180 2023-05-16 19:25:32.961477 fintoc-2.3.0/fintoc/resources/transfer_account.py
+-rw-r--r--   0        0        0      180 2023-05-16 19:25:32.961477 fintoc-2.3.0/fintoc/resources/webhook_endpoint.py
+-rw-r--r--   0        0        0     3353 2023-05-16 19:25:32.961477 fintoc-2.3.0/fintoc/utils.py
+-rw-r--r--   0        0        0      125 2023-05-16 19:25:32.961477 fintoc-2.3.0/fintoc/version.py
+-rw-r--r--   0        0        0      801 2023-05-16 19:25:32.961477 fintoc-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0    16469 1970-01-01 00:00:00.000000 fintoc-2.3.0/setup.py
+-rw-r--r--   0        0        0    16134 1970-01-01 00:00:00.000000 fintoc-2.3.0/PKG-INFO
```

### Comparing `fintoc-2.2.2/LICENSE.md` & `fintoc-2.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fintoc-2.2.2/README.md` & `fintoc-2.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: fintoc
+Version: 2.3.0
+Summary: The official Python client for the Fintoc API.
+Home-page: https://fintoc.com/
+License: BSD-3-Clause
+Author: Daniel Leal
+Author-email: daniel@fintoc.com
+Maintainer: Daniel Leal
+Maintainer-email: daniel@fintoc.com
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Dist: httpx (>=0.16,<1.0)
+Project-URL: Issue Tracker, https://github.com/fintoc-com/fintoc-python/issues
+Project-URL: Repository, https://github.com/fintoc-com/fintoc-python
+Description-Content-Type: text/markdown
+
 <h1 align="center">Fintoc meets Python 🐍</h1>
 
 <p align="center">
     <em>
         You have just found the Python-flavored client of <a href="https://fintoc.com/" target="_blank">Fintoc</a>.
     </em>
 </p>
@@ -20,22 +42,14 @@
 </a>
 
 <a href="https://github.com/fintoc-com/fintoc-python/actions?query=workflow%3Alinters" target="_blank">
     <img src="https://img.shields.io/github/workflow/status/fintoc-com/fintoc-python/linters?label=linters&logo=github" alt="Linters">
 </a>
 </p>
 
-## Why?
-
-You can think of [Fintoc API](https://fintoc.com/docs) as a piscola.
-And the key ingredient to a properly made piscola are the ice cubes.
-Sure, you can still have a [piscola without ice cubes](https://curl.haxx.se/).
-But hey… that’s not enjoyable -- why would you do that?
-Do yourself a favor: go grab some ice cubes by installing this refreshing library.
-
 ## Installation
 
 Install using pip!
 
 ```sh
 pip install fintoc
 ```
@@ -319,25 +333,14 @@
 Once you have a Link, you can use the `tax_returns` manager to get all the tax returns associated to a link!
 
 ```python
 for tax_return in link.tax_returns.all():
     print(tax_return.id)
 ```
 
-#### The `subscriptions` manager
-
-Available methods: `all`, `get`.
-
-Once you have a Link, you can use the `subscriptions` manager to get all the subscriptions associated to a link!
-
-```python
-for subscription in link.subscriptions.all():
-    print(subscription.id)
-```
-
 #### The `refresh_intents` manager
 
 Available methods: `all`, `get`, `create`.
 
 Refresh intents allow you to control how an account gets refreshed on Fintoc! Once you have a Link, you can use the `refresh_intents` manager to create a new refresh intent:
 
 ```python
@@ -388,14 +391,52 @@
 Once you have an Account, you can use the `movements` manager to get all the movements associated to that account!
 
 ```python
 for movement in account.movements.all():
     print(movement.id)
 ```
 
+#### The `subscription_intents` manager
+
+Available methods: `all`, `get`, `create`
+
+Subscription intents allow you to start a subscription using Fintoc!:
+
+```python
+subscription_intent = fintoc_client.subscription_intents.create()
+
+print(subscription_intent.id)            # si_BO381oEATXonG6bj
+print(subscription_intent.widget_token)  # si_BO381oEATXonG6bj_sec_a4xK32BanKWYn
+```
+
+#### The `subscriptions` manager
+
+Available methods: `all`, `get`
+
+You can check the status of the created subscription with the `subscriptions` manager
+
+```python
+subscription = fintoc_client.subscriptions.get('<subscription_id>')
+print(subscription.status)
+```
+
+#### The `charges` manager
+
+Available methods: `all`, `get`, `create`
+
+Once you have active subscriptions, you can use the `charges` manager to create charges to thosse subscriptions
+
+```python
+charge = fintoc_client.charges.create(
+    currency='CLP',
+    amount=1250,
+    subscription_id='<subscription_id>',
+)
+```
+
 ### Serialization
 
 Any resource of the SDK can be serialized! To get the serialized resource, just call the `serialize` method!
 
 ```python
 account = link.accounts.all(lazy=False)[0]
 
@@ -405,7 +446,8 @@
 The serialization corresponds to a dictionary with only simple types, that can be JSON-serialized.
 
 ## Acknowledgements
 
 The first version of this SDK was originally designed and handcrafted by [**@nebil**](https://github.com/nebil),
 [ad](https://en.wikipedia.org/wiki/Ad_honorem) [piscolem](https://en.wiktionary.org/wiki/piscola).
 He built it with the help of Gianni Roberto’s [Picchi 2](https://www.youtube.com/watch?v=WqjUlmkYr2g).
+
```

#### html2text {}

```diff
@@ -1,35 +1,41 @@
+Metadata-Version: 2.1 Name: fintoc Version: 2.3.0 Summary: The official Python
+client for the Fintoc API. Home-page: https://fintoc.com/ License: BSD-3-Clause
+Author: Daniel Leal Author-email: daniel@fintoc.com Maintainer: Daniel Leal
+Maintainer-email: daniel@fintoc.com Requires-Python: >=3.7,<4.0 Classifier:
+License :: OSI Approved :: BSD License Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Requires-Dist:
+httpx (>=0.16,<1.0) Project-URL: Issue Tracker, https://github.com/fintoc-com/
+fintoc-python/issues Project-URL: Repository, https://github.com/fintoc-com/
+fintoc-python Description-Content-Type: text/markdown
                     ****** Fintoc meets Python ð ******
            You have just found the Python-flavored client of Fintoc.
                  [PyPI_-_Version] [Tests] [Coverage] [Linters]
-## Why? You can think of [Fintoc API](https://fintoc.com/docs) as a piscola.
-And the key ingredient to a properly made piscola are the ice cubes. Sure, you
-can still have a [piscola without ice cubes](https://curl.haxx.se/). But heyâ¦
-thatâs not enjoyable -- why would you do that? Do yourself a favor: go grab
-some ice cubes by installing this refreshing library. ## Installation Install
-using pip! ```sh pip install fintoc ``` **Note:** This SDK requires [**Python
-3.6+**](https://docs.python.org/3/whatsnew/3.6.html). ## Usage The idea behind
-this SDK is to stick to the API design as much as possible, so that it feels
-ridiculously natural to use even while only reading the raw API documentation.
-### Quickstart To be able to use this SDK, you first need to have a [Fintoc]
-(https://app.fintoc.com/login) account. You will need to get your secret API
-key from the dashboard to be able to use the SDK. Once you have your API key,
-all you need to do is initialize a `Fintoc` object with it and you're ready to
-start enjoying Fintoc! ```python from fintoc import Fintoc fintoc_client =
-Fintoc("your_api_key") ``` Now you can start using the SDK! ### Managers To
-make the usage of the SDK feel natural, resources are managed by **managers**
-(_wow_). These **managers** correspond to objects with some methods that allow
-you to get the resources that you want. Each manager is _attached_ to another
-resource, following the API structure. For example, the `Fintoc` object has
-`links` and `webhook_endpoints` managers, while `Link` objects have an
-`accounts` manager (we will see more examples soon). Notice that **not every
-manager has all of the methods**, as they correspond to the API capabilities.
-The methods of the managers are the following (we will use the
-`webhook_endpoints` manager as an example): #### `all` You can use the `all`
-method of the managers as follows: ```python webhook_endpoints =
+## Installation Install using pip! ```sh pip install fintoc ``` **Note:** This
+SDK requires [**Python 3.6+**](https://docs.python.org/3/whatsnew/3.6.html). ##
+Usage The idea behind this SDK is to stick to the API design as much as
+possible, so that it feels ridiculously natural to use even while only reading
+the raw API documentation. ### Quickstart To be able to use this SDK, you first
+need to have a [Fintoc](https://app.fintoc.com/login) account. You will need to
+get your secret API key from the dashboard to be able to use the SDK. Once you
+have your API key, all you need to do is initialize a `Fintoc` object with it
+and you're ready to start enjoying Fintoc! ```python from fintoc import Fintoc
+fintoc_client = Fintoc("your_api_key") ``` Now you can start using the SDK! ###
+Managers To make the usage of the SDK feel natural, resources are managed by
+**managers** (_wow_). These **managers** correspond to objects with some
+methods that allow you to get the resources that you want. Each manager is
+_attached_ to another resource, following the API structure. For example, the
+`Fintoc` object has `links` and `webhook_endpoints` managers, while `Link`
+objects have an `accounts` manager (we will see more examples soon). Notice
+that **not every manager has all of the methods**, as they correspond to the
+API capabilities. The methods of the managers are the following (we will use
+the `webhook_endpoints` manager as an example): #### `all` You can use the
+`all` method of the managers as follows: ```python webhook_endpoints =
 fintoc_client.webhook_endpoints.all() ``` The `all` method of the managers
 returns **a generator** with all the instances of the resource. This method can
 also receive `kwargs`! The arguments that can be passed are the arguments that
 the API receives for that specific resource! For example, the `Movement`
 resource can be filtered using `since` and `until`, so if you wanted to get a
 range of `movements` from an `account`, all you need to do is to pass the
 parameters to the method! ```python movements = account.movements.all
@@ -145,40 +151,49 @@
 link.refresh_intents.all() # Refresh Intents accounts = link.accounts.all() #
 Accounts ``` #### The `invoices` manager Available methods: `all`. Once you
 have a Link, you can use the `invoices` manager to get all the invoices
 associated to a link! ```python for invoice in link.invoices.all(): print
 (invoice.id) ``` #### The `tax_returns` manager Available methods: `all`,
 `get`. Once you have a Link, you can use the `tax_returns` manager to get all
 the tax returns associated to a link! ```python for tax_return in
-link.tax_returns.all(): print(tax_return.id) ``` #### The `subscriptions`
-manager Available methods: `all`, `get`. Once you have a Link, you can use the
-`subscriptions` manager to get all the subscriptions associated to a link!
-```python for subscription in link.subscriptions.all(): print(subscription.id)
-``` #### The `refresh_intents` manager Available methods: `all`, `get`,
-`create`. Refresh intents allow you to control how an account gets refreshed on
-Fintoc! Once you have a Link, you can use the `refresh_intents` manager to
-create a new refresh intent: ```python refresh_intent =
-link.refresh_intents.create() print(refresh_intent.id) # ri_5A94DVCJ7xNM3MEo
-``` Notice that the success of this refresh intent will be notified through a
-Webhook. Now, let's list every refresh intent we have: ```python for
-refresh_intent in link.refresh_intents.all(): print(refresh_intent.id) ``` If
-you see a refresh intent you want to use, just use the `get` method! ```python
-refresh_intent = link.refresh_intents.get("ri_5A94DVCJ7xNM3MEo") print
-(refresh_intent.id) # ri_5A94DVCJ7xNM3MEo print(refresh_intent.status) #
-succeeded ``` #### The `accounts` manager Available methods: `all`, `get`. Once
-you have a Link, you can use the `accounts` manager to get all the accounts
-associated to a link! ```python for account in link.accounts.all(): print
-(account.id) ``` Notice that accounts also have a `movements` manager, to get
-all of the movements of an account: ```python account = link.accounts.all
-(lazy=False)[0] movements = account.movements.all(lazy=False) ``` #### The
-`movements` manager Available methods: `all`, `get`. Once you have an Account,
-you can use the `movements` manager to get all the movements associated to that
-account! ```python for movement in account.movements.all(): print(movement.id)
-``` ### Serialization Any resource of the SDK can be serialized! To get the
-serialized resource, just call the `serialize` method! ```python account =
-link.accounts.all(lazy=False)[0] serialization = account.serialize() ``` The
-serialization corresponds to a dictionary with only simple types, that can be
-JSON-serialized. ## Acknowledgements The first version of this SDK was
-originally designed and handcrafted by [**@nebil**](https://github.com/nebil),
-[ad](https://en.wikipedia.org/wiki/Ad_honorem) [piscolem](https://
-en.wiktionary.org/wiki/piscola). He built it with the help of Gianni
-Robertoâs [Picchi 2](https://www.youtube.com/watch?v=WqjUlmkYr2g).
+link.tax_returns.all(): print(tax_return.id) ``` #### The `refresh_intents`
+manager Available methods: `all`, `get`, `create`. Refresh intents allow you to
+control how an account gets refreshed on Fintoc! Once you have a Link, you can
+use the `refresh_intents` manager to create a new refresh intent: ```python
+refresh_intent = link.refresh_intents.create() print(refresh_intent.id) #
+ri_5A94DVCJ7xNM3MEo ``` Notice that the success of this refresh intent will be
+notified through a Webhook. Now, let's list every refresh intent we have:
+```python for refresh_intent in link.refresh_intents.all(): print
+(refresh_intent.id) ``` If you see a refresh intent you want to use, just use
+the `get` method! ```python refresh_intent = link.refresh_intents.get
+("ri_5A94DVCJ7xNM3MEo") print(refresh_intent.id) # ri_5A94DVCJ7xNM3MEo print
+(refresh_intent.status) # succeeded ``` #### The `accounts` manager Available
+methods: `all`, `get`. Once you have a Link, you can use the `accounts` manager
+to get all the accounts associated to a link! ```python for account in
+link.accounts.all(): print(account.id) ``` Notice that accounts also have a
+`movements` manager, to get all of the movements of an account: ```python
+account = link.accounts.all(lazy=False)[0] movements = account.movements.all
+(lazy=False) ``` #### The `movements` manager Available methods: `all`, `get`.
+Once you have an Account, you can use the `movements` manager to get all the
+movements associated to that account! ```python for movement in
+account.movements.all(): print(movement.id) ``` #### The `subscription_intents`
+manager Available methods: `all`, `get`, `create` Subscription intents allow
+you to start a subscription using Fintoc!: ```python subscription_intent =
+fintoc_client.subscription_intents.create() print(subscription_intent.id) #
+si_BO381oEATXonG6bj print(subscription_intent.widget_token) #
+si_BO381oEATXonG6bj_sec_a4xK32BanKWYn ``` #### The `subscriptions` manager
+Available methods: `all`, `get` You can check the status of the created
+subscription with the `subscriptions` manager ```python subscription =
+fintoc_client.subscriptions.get('') print(subscription.status) ``` #### The
+`charges` manager Available methods: `all`, `get`, `create` Once you have
+active subscriptions, you can use the `charges` manager to create charges to
+thosse subscriptions ```python charge = fintoc_client.charges.create
+( currency='CLP', amount=1250, subscription_id='', ) ``` ### Serialization Any
+resource of the SDK can be serialized! To get the serialized resource, just
+call the `serialize` method! ```python account = link.accounts.all(lazy=False)
+[0] serialization = account.serialize() ``` The serialization corresponds to a
+dictionary with only simple types, that can be JSON-serialized. ##
+Acknowledgements The first version of this SDK was originally designed and
+handcrafted by [**@nebil**](https://github.com/nebil), [ad](https://
+en.wikipedia.org/wiki/Ad_honorem) [piscolem](https://en.wiktionary.org/wiki/
+piscola). He built it with the help of Gianni Robertoâs [Picchi 2](https://
+www.youtube.com/watch?v=WqjUlmkYr2g).
```

### Comparing `fintoc-2.2.2/fintoc/client.py` & `fintoc-2.3.0/fintoc/client.py`

 * *Files identical despite different names*

### Comparing `fintoc-2.2.2/fintoc/errors.py` & `fintoc-2.3.0/fintoc/errors.py`

 * *Files identical despite different names*

### Comparing `fintoc-2.2.2/fintoc/managers/__init__.py` & `fintoc-2.3.0/fintoc/managers/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """Init file for the managers module of the SDK."""
 
 from .accounts_manager import AccountsManager
+from .charges_manager import ChargesManager
 from .invoices_manager import InvoicesManager
 from .links_manager import LinksManager
 from .movements_manager import MovementsManager
 from .payment_intents_manager import PaymentIntentsManager
 from .refresh_intents_manager import RefreshIntentsManager
+from .subscription_intents_manager import SubscriptionIntentsManager
 from .subscriptions_manager import SubscriptionsManager
 from .tax_returns_manager import TaxRetunsManager
 from .webhook_endpoints_manager import WebhookEndpointsManager
```

### Comparing `fintoc-2.2.2/fintoc/managers/links_manager.py` & `fintoc-2.3.0/fintoc/managers/links_manager.py`

 * *Files identical despite different names*

### Comparing `fintoc-2.2.2/fintoc/mixins/manager_mixin.py` & `fintoc-2.3.0/fintoc/mixins/manager_mixin.py`

 * *Files identical despite different names*

### Comparing `fintoc-2.2.2/fintoc/mixins/resource_mixin.py` & `fintoc-2.3.0/fintoc/mixins/resource_mixin.py`

 * *Files identical despite different names*

### Comparing `fintoc-2.2.2/fintoc/paginator.py` & `fintoc-2.3.0/fintoc/paginator.py`

 * *Files identical despite different names*

### Comparing `fintoc-2.2.2/fintoc/resource_handlers.py` & `fintoc-2.3.0/fintoc/resource_handlers.py`

 * *Files identical despite different names*

### Comparing `fintoc-2.2.2/fintoc/resources/__init__.py` & `fintoc-2.3.0/fintoc/resources/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 """Init file for the resources module of the SDK."""
 
 from .account import Account
 from .balance import Balance
+from .charge import Charge
 from .generic_fintoc_resource import GenericFintocResource
 from .income import Income
 from .institution import Institution
 from .institution_invoice import InstitutionInvoice
 from .institution_tax_return import InstitutionTaxReturn
 from .invoice import Invoice
 from .link import Link
 from .movement import Movement
 from .other_taxes import OtherTaxes
 from .payment_intent import PaymentIntent
 from .refresh_intent import RefreshIntent
 from .services_invoice import ServicesInvoice
 from .subscription import Subscription
+from .subscription_intent import SubscriptionIntent
 from .tax_return import TaxReturn
 from .taxpayer import Taxpayer
 from .tobacco_taxes import TobaccoTaxes
 from .transfer_account import TransferAccount
 from .webhook_endpoint import WebhookEndpoint
```

### Comparing `fintoc-2.2.2/fintoc/resources/account.py` & `fintoc-2.3.0/fintoc/resources/account.py`

 * *Files identical despite different names*

### Comparing `fintoc-2.2.2/fintoc/resources/link.py` & `fintoc-2.3.0/fintoc/resources/link.py`

 * *Files identical despite different names*

### Comparing `fintoc-2.2.2/fintoc/utils.py` & `fintoc-2.3.0/fintoc/utils.py`

 * *Files identical despite different names*

### Comparing `fintoc-2.2.2/pyproject.toml` & `fintoc-2.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fintoc"
-version = "2.2.2"
+version = "2.3.0"
 description = "The official Python client for the Fintoc API."
 authors = ["Daniel Leal <daniel@fintoc.com>", "Nebil Kawas <nebil@uc.cl>"]
 maintainers = ["Daniel Leal <daniel@fintoc.com>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://fintoc.com/"
 repository = "https://github.com/fintoc-com/fintoc-python"
@@ -15,19 +15,19 @@
     ".pylintrc",
     "Makefile",
     "scripts",
     "tests"
 ]
 
 [tool.poetry.dependencies]
-python = "^3.6"
+python = "^3.7"
 httpx = ">=0.16, < 1.0"
 
 [tool.poetry.dev-dependencies]
-black = "^20.8b1"
+black = "^22.10.0"
 flake8 = "^3.8.4"
 isort = "^5.6.4"
 pylint = "^2.6.0"
 pytest = "^6.1.1"
 pytest-cov = "^2.12.1"
 
 [tool.poetry.urls]
```

### Comparing `fintoc-2.2.2/setup.py` & `fintoc-2.3.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 {'': ['*']}
 
 install_requires = \
 ['httpx>=0.16,<1.0']
 
 setup_kwargs = {
     'name': 'fintoc',
-    'version': '2.2.2',
+    'version': '2.3.0',
     'description': 'The official Python client for the Fintoc API.',
-    'long_description': '<h1 align="center">Fintoc meets Python 🐍</h1>\n\n<p align="center">\n    <em>\n        You have just found the Python-flavored client of <a href="https://fintoc.com/" target="_blank">Fintoc</a>.\n    </em>\n</p>\n\n<p align="center">\n<a href="https://pypi.org/project/fintoc" target="_blank">\n    <img src="https://img.shields.io/pypi/v/fintoc?label=version&logo=python&logoColor=%23fff&color=306998" alt="PyPI - Version">\n</a>\n\n<a href="https://github.com/fintoc-com/fintoc-python/actions?query=workflow%3Atests" target="_blank">\n    <img src="https://img.shields.io/github/workflow/status/fintoc-com/fintoc-python/tests?label=tests&logo=python&logoColor=%23fff" alt="Tests">\n</a>\n\n<a href="https://codecov.io/gh/fintoc-com/fintoc-python" target="_blank">\n    <img src="https://img.shields.io/codecov/c/gh/fintoc-com/fintoc-python?label=coverage&logo=codecov&logoColor=ffffff" alt="Coverage">\n</a>\n\n<a href="https://github.com/fintoc-com/fintoc-python/actions?query=workflow%3Alinters" target="_blank">\n    <img src="https://img.shields.io/github/workflow/status/fintoc-com/fintoc-python/linters?label=linters&logo=github" alt="Linters">\n</a>\n</p>\n\n## Why?\n\nYou can think of [Fintoc API](https://fintoc.com/docs) as a piscola.\nAnd the key ingredient to a properly made piscola are the ice cubes.\nSure, you can still have a [piscola without ice cubes](https://curl.haxx.se/).\nBut hey… that’s not enjoyable -- why would you do that?\nDo yourself a favor: go grab some ice cubes by installing this refreshing library.\n\n## Installation\n\nInstall using pip!\n\n```sh\npip install fintoc\n```\n\n**Note:** This SDK requires [**Python 3.6+**](https://docs.python.org/3/whatsnew/3.6.html).\n\n## Usage\n\nThe idea behind this SDK is to stick to the API design as much as possible, so that it feels ridiculously natural to use even while only reading the raw API documentation.\n\n### Quickstart\n\nTo be able to use this SDK, you first need to have a [Fintoc](https://app.fintoc.com/login) account. You will need to get your secret API key from the dashboard to be able to use the SDK. Once you have your API key, all you need to do is initialize a `Fintoc` object with it and you\'re ready to start enjoying Fintoc!\n\n```python\nfrom fintoc import Fintoc\n\nfintoc_client = Fintoc("your_api_key")\n```\n\nNow you can start using the SDK!\n\n### Managers\n\nTo make the usage of the SDK feel natural, resources are managed by **managers** (_wow_). These **managers** correspond to objects with some methods that allow you to get the resources that you want. Each manager is _attached_ to another resource, following the API structure. For example, the `Fintoc` object has `links` and `webhook_endpoints` managers, while `Link` objects have an `accounts` manager (we will see more examples soon). Notice that **not every manager has all of the methods**, as they correspond to the API capabilities. The methods of the managers are the following (we will use the `webhook_endpoints` manager as an example):\n\n#### `all`\n\nYou can use the `all` method of the managers as follows:\n\n```python\nwebhook_endpoints = fintoc_client.webhook_endpoints.all()\n```\n\nThe `all` method of the managers returns **a generator** with all the instances of the resource. This method can also receive `kwargs`! The arguments that can be passed are the arguments that the API receives for that specific resource! For example, the `Movement` resource can be filtered using `since` and `until`, so if you wanted to get a range of `movements` from an `account`, all you need to do is to pass the parameters to the method!\n\n```python\nmovements = account.movements.all(since="2019-07-24", until="2021-05-12")\n```\n\nYou can also pass the `lazy=False` parameter to the method to force the SDK to return a list of all the instances of the resource instead of the generator. **Beware**: this could take **very long**, depending on the amount of instances that exist of said resource:\n\n```python\nwebhook_endpoints = fintoc_client.webhook_endpoints.all(lazy=False)\n\nisinstance(webhook_endpoints, list)  # True\n```\n\n#### `get`\n\nYou can use the `get` method of the managers as follows:\n\n```python\nwebhook_endpoint = fintoc_client.webhook_endpoints.get("we_8anqVLlBC8ROodem")\n```\n\nThe `get` method of the managers returns an existing instance of the resource using its identifier to find it.\n\n#### `create`\n\nYou can use the `create` method of the managers as follows:\n\n```python\nwebhook_endpoint = fintoc_client.webhook_endpoints.create(\n    url="https://webhook.site/58gfb429-c33c-20c7-584b-d5ew3y3202a0",\n    enabled_events=["link.credentials_changed"],\n    description="Fantasting webhook endpoint",\n)\n```\n\nThe `create` method of the managers creates and returns a new instance of the resource. The attributes of the created object are passed as `kwargs`, and correspond to the parameters specified by the API documentation for the creation of said resource.\n\n#### `update`\n\nYou can use the `update` method of the managers as follows:\n\n```python\nwebhook_endpoint = fintoc_client.webhook_endpoints.update(\n    "we_8anqVLlBC8ROodem",\n    enabled_events=["account.refresh_intent.succeeded"],\n    disabled=True,\n)\n```\n\nThe `update` method of the managers updates and returns an existing instance of the resource using its identifier to find it. The first parameter of the method corresponds to the identifier being used to find the existing instance of the resource. The attributes to be modified are passed as `kwargs`, and correspond to the parameters specified by the API documentation for the update action of said resource.\n\nNotice that using the manager to update an instance of a resource is equivalent (in terms of outcome) to calling the `update` directly on the object itself:\n\n\n```python\n# Using the manager\nwebhook_endpoint = fintoc_client.webhook_endpoints.update(\n    "we_8anqVLlBC8ROodem",\n    enabled_events=["account.refresh_intent.succeeded"],\n    disabled=True,\n)\n\n# Using the object\nwebhook_endpoint = fintoc_client.webhook_endpoints.get("we_8anqVLlBC8ROodem")\nwebhook_endpoint.update(\n    enabled_events=["account.refresh_intent.succeeded"],\n    disabled=True,\n)\n```\n\nWhen using the SDK, you will probably almost always want to use the object directly to update, just because it is way less verbose if you already have the object itself. Also, using the `update` method from the manager first needs to `get` the resource and then updates it, so it translates to 2 API calls. If you already have the object to update, using the `update` method directly from the object just updates it, so it translates to just 1 API call.\n\n#### `delete`\n\nYou can use the `delete` method of the managers as follows:\n\n```python\ndeleted_identifier = fintoc_client.webhook_endpoints.delete("we_8anqVLlBC8ROodem")\n```\n\nThe `delete` method of the managers deletes an existing instance of the resource using its identifier to find it and returns the identifier.\n\nNotice that using the manager to delete an instance of a resource is equivalent (in terms of outcome) to calling the `delete` directly on the object itself:\n\n\n```python\n# Using the manager\ndeleted_identifier = fintoc_client.webhook_endpoints.delete("we_8anqVLlBC8ROodem")\n\n# Using the object\nwebhook_endpoint = fintoc_client.webhook_endpoints.get("we_8anqVLlBC8ROodem")\ndeleted_identifier = webhook_endpoint.delete()\n```\n\nWhen using the SDK, you will probably almost always want to use the object directly to delete, just because it is way less verbose if you already have the object itself. Also, using the `delete` method from the manager first needs to `get` the resource and then deletes it, so it translates to 2 API calls. If you already have the object to delete, using the `delete` method directly from the object just deletes it, so it translates to just 1 API call.\n\n### The shape of the SDK\n\nFor complete information about the API, head to [the docs](https://fintoc.com/docs). You will notice that the shape of the SDK is very similar to the shape of the API. Let\'s start with the `Fintoc` object.\n\n#### The `Fintoc` object\n\nTo create a `Fintoc` object, instantiate it using your secret API key:\n\n```python\nfrom fintoc import Fintoc\n\nfintoc_client = Fintoc("your_api_key")\n```\n\nThis gives us access to a bunch of operations already. The object created using this _snippet_ contains three [managers](#managers): `links`, `payment_intents` and `webhook_endpoints`.\n\n#### The `webhook_endpoints` manager\n\nAvailable methods: `all`, `get`, `create`, `update`, `delete`.\n\nFrom the Fintoc client, you can manage your webhook endpoints swiftly! Start by creating a new Webhook Endpoint!\n\n```python\nwebhook_endpoint = fintoc_client.webhook_endpoints.create(\n    url="https://webhook.site/58gfb429-c33c-20c7-584b-d5ew3y3202a0",\n    enabled_events=["account.refresh_intent.succeeded"],\n    disabled=True,\n)\n\nprint(webhook_endpoint.id)  # we_8anqVLlBC8ROodem\n```\n\nYou can update this webhook endpoint any time you want! Just run the following command:\n\n```python\nwebhook_endpoint = fintoc_client.webhook_endpoints.update(\n    "we_8anqVLlBC8ROodem",\n    enabled_events=["link.credentials_changed"],\n    description="Fantasting webhook endpoint",\n)\n\nprint(webhook_endpoint.status)  # disabled\n```\n\nMaybe you no longer want this webhook endpoint. Let\'s delete it!\n\n```python\nfintoc_client.webhook_endpoints.delete("we_8anqVLlBC8ROodem")\n```\n\nNow, let\'s list every webhook endpoint we have:\n\n```python\nfor webhook_endpoint in fintoc_client.webhook_endpoints.all():\n    print(webhook_endpoint.id)\n```\n\nIf you see a webhook endpoint you want to use, just use the `get` method!\n\n```python\nwebhook_endpoint = fintoc_client.webhook_endpoints.get("we_8anqVLlBC8ROodem")\n\nprint(webhook_endpoint.id)  # we_8anqVLlBC8ROodem\n```\n\n#### The `payment_intents` manager\n\nAvailable methods: `all`, `get`, `create`.\n\nPayment intents allow you to start a payment using Fintoc! Start by creating a new payment intent:\n\n```python\npayment_intent = fintoc_client.payment_intents.create(\n    currency="CLP",\n    amount=5990,\n    recipient_account={\n        "holder_id": "111111111",\n        "number": "123123123",\n        "type": "checking_account",\n        "institution_id": "cl_banco_de_chile",\n    }\n)\n\nprint(payment_intent.id)            # pi_BO381oEATXonG6bj\nprint(payment_intent.widget_token)  # pi_BO381oEATXonG6bj_sec_a4xK32BanKWYn\n```\n\nNotice that the success of this payment intent will be notified through a Webhook. Now, let\'s list every payment intent we have:\n\n```python\nfor payment_intent in fintoc_client.payment_intents.all():\n    print(payment_intent.id)\n```\n\nIf you see a payment intent you want to use, just use the `get` method!\n\n```python\npayment_intent = fintoc_client.payment_intents.get("pi_BO381oEATXonG6bj")\n\nprint(payment_intent.id)      # pi_BO381oEATXonG6bj\nprint(payment_intent.status)  # succeeded\n```\n\n#### The `links` manager\n\nAvailable methods: `all`, `get`, `update`, `delete`.\n\nLinks are probably the most importat resource. Let\'s list them!\n\n```python\nprint(len(fintoc_client.links.all(lazy=False)))  # 3\n\nfor link in fintoc_client.links.all():\n    print(link.id)\n```\n\nLinks are a bit different than the rest of the resources, because their identifier is not really their `id`, but their `link_token`. This means that, in order to `get`, `update` or `delete` a link, you need to pass the `link_token`!\n\n```python\nlink = fintoc_client.links.get("link_Y75EXAKiIVj7w489_token_NCqjwRVoTX3cmnx8pnbpqd11")\n```\n\nNotice that the Link objects generated from the `all` method will won\'t be able to execute `update` or `delete` operations, while any Link object generated from `get` or `update` will have permission to `update` or `delete` (given that the link token is necessary to `get` or `update` in the first place).\n\nThe Link resource has a lot of **managers**!\n\n```python\ninvoices = link.invoices.all()  # Invoices\ntax_returns = link.tax_returns.all()  # Tax Returns\nsubscriptions = link.subscriptions.all()  # Subscriptions\nrefresh_intents = link.refresh_intents.all()  # Refresh Intents\naccounts = link.accounts.all()  # Accounts\n```\n\n#### The `invoices` manager\n\nAvailable methods: `all`.\n\nOnce you have a Link, you can use the `invoices` manager to get all the invoices associated to a link!\n\n```python\nfor invoice in link.invoices.all():\n    print(invoice.id)\n```\n\n#### The `tax_returns` manager\n\nAvailable methods: `all`, `get`.\n\nOnce you have a Link, you can use the `tax_returns` manager to get all the tax returns associated to a link!\n\n```python\nfor tax_return in link.tax_returns.all():\n    print(tax_return.id)\n```\n\n#### The `subscriptions` manager\n\nAvailable methods: `all`, `get`.\n\nOnce you have a Link, you can use the `subscriptions` manager to get all the subscriptions associated to a link!\n\n```python\nfor subscription in link.subscriptions.all():\n    print(subscription.id)\n```\n\n#### The `refresh_intents` manager\n\nAvailable methods: `all`, `get`, `create`.\n\nRefresh intents allow you to control how an account gets refreshed on Fintoc! Once you have a Link, you can use the `refresh_intents` manager to create a new refresh intent:\n\n```python\nrefresh_intent = link.refresh_intents.create()\n\nprint(refresh_intent.id)  # ri_5A94DVCJ7xNM3MEo\n```\n\nNotice that the success of this refresh intent will be notified through a Webhook. Now, let\'s list every refresh intent we have:\n\n```python\nfor refresh_intent in link.refresh_intents.all():\n    print(refresh_intent.id)\n```\n\nIf you see a refresh intent you want to use, just use the `get` method!\n\n```python\nrefresh_intent = link.refresh_intents.get("ri_5A94DVCJ7xNM3MEo")\n\nprint(refresh_intent.id)      # ri_5A94DVCJ7xNM3MEo\nprint(refresh_intent.status)  # succeeded\n```\n\n#### The `accounts` manager\n\nAvailable methods: `all`, `get`.\n\nOnce you have a Link, you can use the `accounts` manager to get all the accounts associated to a link!\n\n```python\nfor account in link.accounts.all():\n    print(account.id)\n```\n\nNotice that accounts also have a `movements` manager, to get all of the movements of an account:\n\n```python\naccount = link.accounts.all(lazy=False)[0]\n\nmovements = account.movements.all(lazy=False)\n```\n\n#### The `movements` manager\n\nAvailable methods: `all`, `get`.\n\nOnce you have an Account, you can use the `movements` manager to get all the movements associated to that account!\n\n```python\nfor movement in account.movements.all():\n    print(movement.id)\n```\n\n### Serialization\n\nAny resource of the SDK can be serialized! To get the serialized resource, just call the `serialize` method!\n\n```python\naccount = link.accounts.all(lazy=False)[0]\n\nserialization = account.serialize()\n```\n\nThe serialization corresponds to a dictionary with only simple types, that can be JSON-serialized.\n\n## Acknowledgements\n\nThe first version of this SDK was originally designed and handcrafted by [**@nebil**](https://github.com/nebil),\n[ad](https://en.wikipedia.org/wiki/Ad_honorem) [piscolem](https://en.wiktionary.org/wiki/piscola).\nHe built it with the help of Gianni Roberto’s [Picchi 2](https://www.youtube.com/watch?v=WqjUlmkYr2g).\n',
+    'long_description': '<h1 align="center">Fintoc meets Python 🐍</h1>\n\n<p align="center">\n    <em>\n        You have just found the Python-flavored client of <a href="https://fintoc.com/" target="_blank">Fintoc</a>.\n    </em>\n</p>\n\n<p align="center">\n<a href="https://pypi.org/project/fintoc" target="_blank">\n    <img src="https://img.shields.io/pypi/v/fintoc?label=version&logo=python&logoColor=%23fff&color=306998" alt="PyPI - Version">\n</a>\n\n<a href="https://github.com/fintoc-com/fintoc-python/actions?query=workflow%3Atests" target="_blank">\n    <img src="https://img.shields.io/github/workflow/status/fintoc-com/fintoc-python/tests?label=tests&logo=python&logoColor=%23fff" alt="Tests">\n</a>\n\n<a href="https://codecov.io/gh/fintoc-com/fintoc-python" target="_blank">\n    <img src="https://img.shields.io/codecov/c/gh/fintoc-com/fintoc-python?label=coverage&logo=codecov&logoColor=ffffff" alt="Coverage">\n</a>\n\n<a href="https://github.com/fintoc-com/fintoc-python/actions?query=workflow%3Alinters" target="_blank">\n    <img src="https://img.shields.io/github/workflow/status/fintoc-com/fintoc-python/linters?label=linters&logo=github" alt="Linters">\n</a>\n</p>\n\n## Installation\n\nInstall using pip!\n\n```sh\npip install fintoc\n```\n\n**Note:** This SDK requires [**Python 3.6+**](https://docs.python.org/3/whatsnew/3.6.html).\n\n## Usage\n\nThe idea behind this SDK is to stick to the API design as much as possible, so that it feels ridiculously natural to use even while only reading the raw API documentation.\n\n### Quickstart\n\nTo be able to use this SDK, you first need to have a [Fintoc](https://app.fintoc.com/login) account. You will need to get your secret API key from the dashboard to be able to use the SDK. Once you have your API key, all you need to do is initialize a `Fintoc` object with it and you\'re ready to start enjoying Fintoc!\n\n```python\nfrom fintoc import Fintoc\n\nfintoc_client = Fintoc("your_api_key")\n```\n\nNow you can start using the SDK!\n\n### Managers\n\nTo make the usage of the SDK feel natural, resources are managed by **managers** (_wow_). These **managers** correspond to objects with some methods that allow you to get the resources that you want. Each manager is _attached_ to another resource, following the API structure. For example, the `Fintoc` object has `links` and `webhook_endpoints` managers, while `Link` objects have an `accounts` manager (we will see more examples soon). Notice that **not every manager has all of the methods**, as they correspond to the API capabilities. The methods of the managers are the following (we will use the `webhook_endpoints` manager as an example):\n\n#### `all`\n\nYou can use the `all` method of the managers as follows:\n\n```python\nwebhook_endpoints = fintoc_client.webhook_endpoints.all()\n```\n\nThe `all` method of the managers returns **a generator** with all the instances of the resource. This method can also receive `kwargs`! The arguments that can be passed are the arguments that the API receives for that specific resource! For example, the `Movement` resource can be filtered using `since` and `until`, so if you wanted to get a range of `movements` from an `account`, all you need to do is to pass the parameters to the method!\n\n```python\nmovements = account.movements.all(since="2019-07-24", until="2021-05-12")\n```\n\nYou can also pass the `lazy=False` parameter to the method to force the SDK to return a list of all the instances of the resource instead of the generator. **Beware**: this could take **very long**, depending on the amount of instances that exist of said resource:\n\n```python\nwebhook_endpoints = fintoc_client.webhook_endpoints.all(lazy=False)\n\nisinstance(webhook_endpoints, list)  # True\n```\n\n#### `get`\n\nYou can use the `get` method of the managers as follows:\n\n```python\nwebhook_endpoint = fintoc_client.webhook_endpoints.get("we_8anqVLlBC8ROodem")\n```\n\nThe `get` method of the managers returns an existing instance of the resource using its identifier to find it.\n\n#### `create`\n\nYou can use the `create` method of the managers as follows:\n\n```python\nwebhook_endpoint = fintoc_client.webhook_endpoints.create(\n    url="https://webhook.site/58gfb429-c33c-20c7-584b-d5ew3y3202a0",\n    enabled_events=["link.credentials_changed"],\n    description="Fantasting webhook endpoint",\n)\n```\n\nThe `create` method of the managers creates and returns a new instance of the resource. The attributes of the created object are passed as `kwargs`, and correspond to the parameters specified by the API documentation for the creation of said resource.\n\n#### `update`\n\nYou can use the `update` method of the managers as follows:\n\n```python\nwebhook_endpoint = fintoc_client.webhook_endpoints.update(\n    "we_8anqVLlBC8ROodem",\n    enabled_events=["account.refresh_intent.succeeded"],\n    disabled=True,\n)\n```\n\nThe `update` method of the managers updates and returns an existing instance of the resource using its identifier to find it. The first parameter of the method corresponds to the identifier being used to find the existing instance of the resource. The attributes to be modified are passed as `kwargs`, and correspond to the parameters specified by the API documentation for the update action of said resource.\n\nNotice that using the manager to update an instance of a resource is equivalent (in terms of outcome) to calling the `update` directly on the object itself:\n\n\n```python\n# Using the manager\nwebhook_endpoint = fintoc_client.webhook_endpoints.update(\n    "we_8anqVLlBC8ROodem",\n    enabled_events=["account.refresh_intent.succeeded"],\n    disabled=True,\n)\n\n# Using the object\nwebhook_endpoint = fintoc_client.webhook_endpoints.get("we_8anqVLlBC8ROodem")\nwebhook_endpoint.update(\n    enabled_events=["account.refresh_intent.succeeded"],\n    disabled=True,\n)\n```\n\nWhen using the SDK, you will probably almost always want to use the object directly to update, just because it is way less verbose if you already have the object itself. Also, using the `update` method from the manager first needs to `get` the resource and then updates it, so it translates to 2 API calls. If you already have the object to update, using the `update` method directly from the object just updates it, so it translates to just 1 API call.\n\n#### `delete`\n\nYou can use the `delete` method of the managers as follows:\n\n```python\ndeleted_identifier = fintoc_client.webhook_endpoints.delete("we_8anqVLlBC8ROodem")\n```\n\nThe `delete` method of the managers deletes an existing instance of the resource using its identifier to find it and returns the identifier.\n\nNotice that using the manager to delete an instance of a resource is equivalent (in terms of outcome) to calling the `delete` directly on the object itself:\n\n\n```python\n# Using the manager\ndeleted_identifier = fintoc_client.webhook_endpoints.delete("we_8anqVLlBC8ROodem")\n\n# Using the object\nwebhook_endpoint = fintoc_client.webhook_endpoints.get("we_8anqVLlBC8ROodem")\ndeleted_identifier = webhook_endpoint.delete()\n```\n\nWhen using the SDK, you will probably almost always want to use the object directly to delete, just because it is way less verbose if you already have the object itself. Also, using the `delete` method from the manager first needs to `get` the resource and then deletes it, so it translates to 2 API calls. If you already have the object to delete, using the `delete` method directly from the object just deletes it, so it translates to just 1 API call.\n\n### The shape of the SDK\n\nFor complete information about the API, head to [the docs](https://fintoc.com/docs). You will notice that the shape of the SDK is very similar to the shape of the API. Let\'s start with the `Fintoc` object.\n\n#### The `Fintoc` object\n\nTo create a `Fintoc` object, instantiate it using your secret API key:\n\n```python\nfrom fintoc import Fintoc\n\nfintoc_client = Fintoc("your_api_key")\n```\n\nThis gives us access to a bunch of operations already. The object created using this _snippet_ contains three [managers](#managers): `links`, `payment_intents` and `webhook_endpoints`.\n\n#### The `webhook_endpoints` manager\n\nAvailable methods: `all`, `get`, `create`, `update`, `delete`.\n\nFrom the Fintoc client, you can manage your webhook endpoints swiftly! Start by creating a new Webhook Endpoint!\n\n```python\nwebhook_endpoint = fintoc_client.webhook_endpoints.create(\n    url="https://webhook.site/58gfb429-c33c-20c7-584b-d5ew3y3202a0",\n    enabled_events=["account.refresh_intent.succeeded"],\n    disabled=True,\n)\n\nprint(webhook_endpoint.id)  # we_8anqVLlBC8ROodem\n```\n\nYou can update this webhook endpoint any time you want! Just run the following command:\n\n```python\nwebhook_endpoint = fintoc_client.webhook_endpoints.update(\n    "we_8anqVLlBC8ROodem",\n    enabled_events=["link.credentials_changed"],\n    description="Fantasting webhook endpoint",\n)\n\nprint(webhook_endpoint.status)  # disabled\n```\n\nMaybe you no longer want this webhook endpoint. Let\'s delete it!\n\n```python\nfintoc_client.webhook_endpoints.delete("we_8anqVLlBC8ROodem")\n```\n\nNow, let\'s list every webhook endpoint we have:\n\n```python\nfor webhook_endpoint in fintoc_client.webhook_endpoints.all():\n    print(webhook_endpoint.id)\n```\n\nIf you see a webhook endpoint you want to use, just use the `get` method!\n\n```python\nwebhook_endpoint = fintoc_client.webhook_endpoints.get("we_8anqVLlBC8ROodem")\n\nprint(webhook_endpoint.id)  # we_8anqVLlBC8ROodem\n```\n\n#### The `payment_intents` manager\n\nAvailable methods: `all`, `get`, `create`.\n\nPayment intents allow you to start a payment using Fintoc! Start by creating a new payment intent:\n\n```python\npayment_intent = fintoc_client.payment_intents.create(\n    currency="CLP",\n    amount=5990,\n    recipient_account={\n        "holder_id": "111111111",\n        "number": "123123123",\n        "type": "checking_account",\n        "institution_id": "cl_banco_de_chile",\n    }\n)\n\nprint(payment_intent.id)            # pi_BO381oEATXonG6bj\nprint(payment_intent.widget_token)  # pi_BO381oEATXonG6bj_sec_a4xK32BanKWYn\n```\n\nNotice that the success of this payment intent will be notified through a Webhook. Now, let\'s list every payment intent we have:\n\n```python\nfor payment_intent in fintoc_client.payment_intents.all():\n    print(payment_intent.id)\n```\n\nIf you see a payment intent you want to use, just use the `get` method!\n\n```python\npayment_intent = fintoc_client.payment_intents.get("pi_BO381oEATXonG6bj")\n\nprint(payment_intent.id)      # pi_BO381oEATXonG6bj\nprint(payment_intent.status)  # succeeded\n```\n\n#### The `links` manager\n\nAvailable methods: `all`, `get`, `update`, `delete`.\n\nLinks are probably the most importat resource. Let\'s list them!\n\n```python\nprint(len(fintoc_client.links.all(lazy=False)))  # 3\n\nfor link in fintoc_client.links.all():\n    print(link.id)\n```\n\nLinks are a bit different than the rest of the resources, because their identifier is not really their `id`, but their `link_token`. This means that, in order to `get`, `update` or `delete` a link, you need to pass the `link_token`!\n\n```python\nlink = fintoc_client.links.get("link_Y75EXAKiIVj7w489_token_NCqjwRVoTX3cmnx8pnbpqd11")\n```\n\nNotice that the Link objects generated from the `all` method will won\'t be able to execute `update` or `delete` operations, while any Link object generated from `get` or `update` will have permission to `update` or `delete` (given that the link token is necessary to `get` or `update` in the first place).\n\nThe Link resource has a lot of **managers**!\n\n```python\ninvoices = link.invoices.all()  # Invoices\ntax_returns = link.tax_returns.all()  # Tax Returns\nsubscriptions = link.subscriptions.all()  # Subscriptions\nrefresh_intents = link.refresh_intents.all()  # Refresh Intents\naccounts = link.accounts.all()  # Accounts\n```\n\n#### The `invoices` manager\n\nAvailable methods: `all`.\n\nOnce you have a Link, you can use the `invoices` manager to get all the invoices associated to a link!\n\n```python\nfor invoice in link.invoices.all():\n    print(invoice.id)\n```\n\n#### The `tax_returns` manager\n\nAvailable methods: `all`, `get`.\n\nOnce you have a Link, you can use the `tax_returns` manager to get all the tax returns associated to a link!\n\n```python\nfor tax_return in link.tax_returns.all():\n    print(tax_return.id)\n```\n\n#### The `refresh_intents` manager\n\nAvailable methods: `all`, `get`, `create`.\n\nRefresh intents allow you to control how an account gets refreshed on Fintoc! Once you have a Link, you can use the `refresh_intents` manager to create a new refresh intent:\n\n```python\nrefresh_intent = link.refresh_intents.create()\n\nprint(refresh_intent.id)  # ri_5A94DVCJ7xNM3MEo\n```\n\nNotice that the success of this refresh intent will be notified through a Webhook. Now, let\'s list every refresh intent we have:\n\n```python\nfor refresh_intent in link.refresh_intents.all():\n    print(refresh_intent.id)\n```\n\nIf you see a refresh intent you want to use, just use the `get` method!\n\n```python\nrefresh_intent = link.refresh_intents.get("ri_5A94DVCJ7xNM3MEo")\n\nprint(refresh_intent.id)      # ri_5A94DVCJ7xNM3MEo\nprint(refresh_intent.status)  # succeeded\n```\n\n#### The `accounts` manager\n\nAvailable methods: `all`, `get`.\n\nOnce you have a Link, you can use the `accounts` manager to get all the accounts associated to a link!\n\n```python\nfor account in link.accounts.all():\n    print(account.id)\n```\n\nNotice that accounts also have a `movements` manager, to get all of the movements of an account:\n\n```python\naccount = link.accounts.all(lazy=False)[0]\n\nmovements = account.movements.all(lazy=False)\n```\n\n#### The `movements` manager\n\nAvailable methods: `all`, `get`.\n\nOnce you have an Account, you can use the `movements` manager to get all the movements associated to that account!\n\n```python\nfor movement in account.movements.all():\n    print(movement.id)\n```\n\n#### The `subscription_intents` manager\n\nAvailable methods: `all`, `get`, `create`\n\nSubscription intents allow you to start a subscription using Fintoc!:\n\n```python\nsubscription_intent = fintoc_client.subscription_intents.create()\n\nprint(subscription_intent.id)            # si_BO381oEATXonG6bj\nprint(subscription_intent.widget_token)  # si_BO381oEATXonG6bj_sec_a4xK32BanKWYn\n```\n\n#### The `subscriptions` manager\n\nAvailable methods: `all`, `get`\n\nYou can check the status of the created subscription with the `subscriptions` manager\n\n```python\nsubscription = fintoc_client.subscriptions.get(\'<subscription_id>\')\nprint(subscription.status)\n```\n\n#### The `charges` manager\n\nAvailable methods: `all`, `get`, `create`\n\nOnce you have active subscriptions, you can use the `charges` manager to create charges to thosse subscriptions\n\n```python\ncharge = fintoc_client.charges.create(\n    currency=\'CLP\',\n    amount=1250,\n    subscription_id=\'<subscription_id>\',\n)\n```\n\n### Serialization\n\nAny resource of the SDK can be serialized! To get the serialized resource, just call the `serialize` method!\n\n```python\naccount = link.accounts.all(lazy=False)[0]\n\nserialization = account.serialize()\n```\n\nThe serialization corresponds to a dictionary with only simple types, that can be JSON-serialized.\n\n## Acknowledgements\n\nThe first version of this SDK was originally designed and handcrafted by [**@nebil**](https://github.com/nebil),\n[ad](https://en.wikipedia.org/wiki/Ad_honorem) [piscolem](https://en.wiktionary.org/wiki/piscola).\nHe built it with the help of Gianni Roberto’s [Picchi 2](https://www.youtube.com/watch?v=WqjUlmkYr2g).\n',
     'author': 'Daniel Leal',
     'author_email': 'daniel@fintoc.com',
     'maintainer': 'Daniel Leal',
     'maintainer_email': 'daniel@fintoc.com',
     'url': 'https://fintoc.com/',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.6,<4.0',
+    'python_requires': '>=3.7,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,24 +1,19 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['fintoc',
 'fintoc.managers', 'fintoc.mixins', 'fintoc.resources'] package_data = \ {'':
 ['*']} install_requires = \ ['httpx>=0.16,<1.0'] setup_kwargs = { 'name':
-'fintoc', 'version': '2.2.2', 'description': 'The official Python client for
+'fintoc', 'version': '2.3.0', 'description': 'The official Python client for
 the Fintoc API.', 'long_description': '
                     ****** Fintoc meets Python ð ******
 \n\n
       \n \n You have just found the Python-flavored client of Fintoc.\n\n
 \n\n
 \n\n_[PyPI_-_Version]\n\n\n\n_[Tests]\n\n\n\n_[Coverage]\n\n\n\n_[Linters]\n\n
-\n\n## Why?\n\nYou can think of [Fintoc API](https://fintoc.com/docs) as a
-piscola.\nAnd the key ingredient to a properly made piscola are the ice
-cubes.\nSure, you can still have a [piscola without ice cubes](https://
-curl.haxx.se/).\nBut heyâ¦ thatâs not enjoyable -- why would you do
-that?\nDo yourself a favor: go grab some ice cubes by installing this
-refreshing library.\n\n## Installation\n\nInstall using pip!\n\n```sh\npip
-install fintoc\n```\n\n**Note:** This SDK requires [**Python 3.6+**](https://
+\n\n## Installation\n\nInstall using pip!\n\n```sh\npip install
+fintoc\n```\n\n**Note:** This SDK requires [**Python 3.6+**](https://
 docs.python.org/3/whatsnew/3.6.html).\n\n## Usage\n\nThe idea behind this SDK
 is to stick to the API design as much as possible, so that it feels
 ridiculously natural to use even while only reading the raw API
 documentation.\n\n### Quickstart\n\nTo be able to use this SDK, you first need
 to have a [Fintoc](https://app.fintoc.com/login) account. You will need to get
 your secret API key from the dashboard to be able to use the SDK. Once you have
 your API key, all you need to do is initialize a `Fintoc` object with it and
@@ -162,48 +157,58 @@
 Intents\naccounts = link.accounts.all() # Accounts\n```\n\n#### The `invoices`
 manager\n\nAvailable methods: `all`.\n\nOnce you have a Link, you can use the
 `invoices` manager to get all the invoices associated to a
 link!\n\n```python\nfor invoice in link.invoices.all():\n print
 (invoice.id)\n```\n\n#### The `tax_returns` manager\n\nAvailable methods:
 `all`, `get`.\n\nOnce you have a Link, you can use the `tax_returns` manager to
 get all the tax returns associated to a link!\n\n```python\nfor tax_return in
-link.tax_returns.all():\n print(tax_return.id)\n```\n\n#### The `subscriptions`
-manager\n\nAvailable methods: `all`, `get`.\n\nOnce you have a Link, you can
-use the `subscriptions` manager to get all the subscriptions associated to a
-link!\n\n```python\nfor subscription in link.subscriptions.all():\n print
-(subscription.id)\n```\n\n#### The `refresh_intents` manager\n\nAvailable
-methods: `all`, `get`, `create`.\n\nRefresh intents allow you to control how an
-account gets refreshed on Fintoc! Once you have a Link, you can use the
-`refresh_intents` manager to create a new refresh intent:
-\n\n```python\nrefresh_intent = link.refresh_intents.create()\n\nprint
-(refresh_intent.id) # ri_5A94DVCJ7xNM3MEo\n```\n\nNotice that the success of
-this refresh intent will be notified through a Webhook. Now, let\'s list every
-refresh intent we have:\n\n```python\nfor refresh_intent in
-link.refresh_intents.all():\n print(refresh_intent.id)\n```\n\nIf you see a
-refresh intent you want to use, just use the `get`
-method!\n\n```python\nrefresh_intent = link.refresh_intents.get
+link.tax_returns.all():\n print(tax_return.id)\n```\n\n#### The
+`refresh_intents` manager\n\nAvailable methods: `all`, `get`,
+`create`.\n\nRefresh intents allow you to control how an account gets refreshed
+on Fintoc! Once you have a Link, you can use the `refresh_intents` manager to
+create a new refresh intent:\n\n```python\nrefresh_intent =
+link.refresh_intents.create()\n\nprint(refresh_intent.id) #
+ri_5A94DVCJ7xNM3MEo\n```\n\nNotice that the success of this refresh intent will
+be notified through a Webhook. Now, let\'s list every refresh intent we have:
+\n\n```python\nfor refresh_intent in link.refresh_intents.all():\n print
+(refresh_intent.id)\n```\n\nIf you see a refresh intent you want to use, just
+use the `get` method!\n\n```python\nrefresh_intent = link.refresh_intents.get
 ("ri_5A94DVCJ7xNM3MEo")\n\nprint(refresh_intent.id) #
 ri_5A94DVCJ7xNM3MEo\nprint(refresh_intent.status) # succeeded\n```\n\n#### The
 `accounts` manager\n\nAvailable methods: `all`, `get`.\n\nOnce you have a Link,
 you can use the `accounts` manager to get all the accounts associated to a
 link!\n\n```python\nfor account in link.accounts.all():\n print
 (account.id)\n```\n\nNotice that accounts also have a `movements` manager, to
 get all of the movements of an account:\n\n```python\naccount =
 link.accounts.all(lazy=False)[0]\n\nmovements = account.movements.all
 (lazy=False)\n```\n\n#### The `movements` manager\n\nAvailable methods: `all`,
 `get`.\n\nOnce you have an Account, you can use the `movements` manager to get
 all the movements associated to that account!\n\n```python\nfor movement in
-account.movements.all():\n print(movement.id)\n```\n\n### Serialization\n\nAny
-resource of the SDK can be serialized! To get the serialized resource, just
-call the `serialize` method!\n\n```python\naccount = link.accounts.all
-(lazy=False)[0]\n\nserialization = account.serialize()\n```\n\nThe
-serialization corresponds to a dictionary with only simple types, that can be
-JSON-serialized.\n\n## Acknowledgements\n\nThe first version of this SDK was
-originally designed and handcrafted by [**@nebil**](https://github.com/
-nebil),\n[ad](https://en.wikipedia.org/wiki/Ad_honorem) [piscolem](https://
-en.wiktionary.org/wiki/piscola).\nHe built it with the help of Gianni
+account.movements.all():\n print(movement.id)\n```\n\n#### The
+`subscription_intents` manager\n\nAvailable methods: `all`, `get`,
+`create`\n\nSubscription intents allow you to start a subscription using
+Fintoc!:\n\n```python\nsubscription_intent =
+fintoc_client.subscription_intents.create()\n\nprint(subscription_intent.id) #
+si_BO381oEATXonG6bj\nprint(subscription_intent.widget_token) #
+si_BO381oEATXonG6bj_sec_a4xK32BanKWYn\n```\n\n#### The `subscriptions`
+manager\n\nAvailable methods: `all`, `get`\n\nYou can check the status of the
+created subscription with the `subscriptions`
+manager\n\n```python\nsubscription = fintoc_client.subscriptions.get
+(\'\')\nprint(subscription.status)\n```\n\n#### The `charges`
+manager\n\nAvailable methods: `all`, `get`, `create`\n\nOnce you have active
+subscriptions, you can use the `charges` manager to create charges to thosse
+subscriptions\n\n```python\ncharge = fintoc_client.charges.create(\n
+currency=\'CLP\',\n amount=1250,\n subscription_id=\'\',\n)\n```\n\n###
+Serialization\n\nAny resource of the SDK can be serialized! To get the
+serialized resource, just call the `serialize` method!\n\n```python\naccount =
+link.accounts.all(lazy=False)[0]\n\nserialization = account.serialize
+()\n```\n\nThe serialization corresponds to a dictionary with only simple
+types, that can be JSON-serialized.\n\n## Acknowledgements\n\nThe first version
+of this SDK was originally designed and handcrafted by [**@nebil**](https://
+github.com/nebil),\n[ad](https://en.wikipedia.org/wiki/Ad_honorem) [piscolem]
+(https://en.wiktionary.org/wiki/piscola).\nHe built it with the help of Gianni
 Robertoâs [Picchi 2](https://www.youtube.com/watch?v=WqjUlmkYr2g).\n',
 'author': 'Daniel Leal', 'author_email': 'daniel@fintoc.com', 'maintainer':
 'Daniel Leal', 'maintainer_email': 'daniel@fintoc.com', 'url': 'https://
 fintoc.com/', 'packages': packages, 'package_data': package_data,
-'install_requires': install_requires, 'python_requires': '>=3.6,<4.0', } setup
+'install_requires': install_requires, 'python_requires': '>=3.7,<4.0', } setup
 (**setup_kwargs)
```

### Comparing `fintoc-2.2.2/PKG-INFO` & `fintoc-2.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: fintoc
-Version: 2.2.2
-Summary: The official Python client for the Fintoc API.
-Home-page: https://fintoc.com/
-License: BSD-3-Clause
-Author: Daniel Leal
-Author-email: daniel@fintoc.com
-Maintainer: Daniel Leal
-Maintainer-email: daniel@fintoc.com
-Requires-Python: >=3.6,<4.0
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: httpx (>=0.16,<1.0)
-Project-URL: Issue Tracker, https://github.com/fintoc-com/fintoc-python/issues
-Project-URL: Repository, https://github.com/fintoc-com/fintoc-python
-Description-Content-Type: text/markdown
-
 <h1 align="center">Fintoc meets Python 🐍</h1>
 
 <p align="center">
     <em>
         You have just found the Python-flavored client of <a href="https://fintoc.com/" target="_blank">Fintoc</a>.
     </em>
 </p>
@@ -43,22 +20,14 @@
 </a>
 
 <a href="https://github.com/fintoc-com/fintoc-python/actions?query=workflow%3Alinters" target="_blank">
     <img src="https://img.shields.io/github/workflow/status/fintoc-com/fintoc-python/linters?label=linters&logo=github" alt="Linters">
 </a>
 </p>
 
-## Why?
-
-You can think of [Fintoc API](https://fintoc.com/docs) as a piscola.
-And the key ingredient to a properly made piscola are the ice cubes.
-Sure, you can still have a [piscola without ice cubes](https://curl.haxx.se/).
-But hey… that’s not enjoyable -- why would you do that?
-Do yourself a favor: go grab some ice cubes by installing this refreshing library.
-
 ## Installation
 
 Install using pip!
 
 ```sh
 pip install fintoc
 ```
@@ -342,25 +311,14 @@
 Once you have a Link, you can use the `tax_returns` manager to get all the tax returns associated to a link!
 
 ```python
 for tax_return in link.tax_returns.all():
     print(tax_return.id)
 ```
 
-#### The `subscriptions` manager
-
-Available methods: `all`, `get`.
-
-Once you have a Link, you can use the `subscriptions` manager to get all the subscriptions associated to a link!
-
-```python
-for subscription in link.subscriptions.all():
-    print(subscription.id)
-```
-
 #### The `refresh_intents` manager
 
 Available methods: `all`, `get`, `create`.
 
 Refresh intents allow you to control how an account gets refreshed on Fintoc! Once you have a Link, you can use the `refresh_intents` manager to create a new refresh intent:
 
 ```python
@@ -411,14 +369,52 @@
 Once you have an Account, you can use the `movements` manager to get all the movements associated to that account!
 
 ```python
 for movement in account.movements.all():
     print(movement.id)
 ```
 
+#### The `subscription_intents` manager
+
+Available methods: `all`, `get`, `create`
+
+Subscription intents allow you to start a subscription using Fintoc!:
+
+```python
+subscription_intent = fintoc_client.subscription_intents.create()
+
+print(subscription_intent.id)            # si_BO381oEATXonG6bj
+print(subscription_intent.widget_token)  # si_BO381oEATXonG6bj_sec_a4xK32BanKWYn
+```
+
+#### The `subscriptions` manager
+
+Available methods: `all`, `get`
+
+You can check the status of the created subscription with the `subscriptions` manager
+
+```python
+subscription = fintoc_client.subscriptions.get('<subscription_id>')
+print(subscription.status)
+```
+
+#### The `charges` manager
+
+Available methods: `all`, `get`, `create`
+
+Once you have active subscriptions, you can use the `charges` manager to create charges to thosse subscriptions
+
+```python
+charge = fintoc_client.charges.create(
+    currency='CLP',
+    amount=1250,
+    subscription_id='<subscription_id>',
+)
+```
+
 ### Serialization
 
 Any resource of the SDK can be serialized! To get the serialized resource, just call the `serialize` method!
 
 ```python
 account = link.accounts.all(lazy=False)[0]
 
@@ -428,8 +424,7 @@
 The serialization corresponds to a dictionary with only simple types, that can be JSON-serialized.
 
 ## Acknowledgements
 
 The first version of this SDK was originally designed and handcrafted by [**@nebil**](https://github.com/nebil),
 [ad](https://en.wikipedia.org/wiki/Ad_honorem) [piscolem](https://en.wiktionary.org/wiki/piscola).
 He built it with the help of Gianni Roberto’s [Picchi 2](https://www.youtube.com/watch?v=WqjUlmkYr2g).
-
```

#### html2text {}

```diff
@@ -1,47 +1,30 @@
-Metadata-Version: 2.1 Name: fintoc Version: 2.2.2 Summary: The official Python
-client for the Fintoc API. Home-page: https://fintoc.com/ License: BSD-3-Clause
-Author: Daniel Leal Author-email: daniel@fintoc.com Maintainer: Daniel Leal
-Maintainer-email: daniel@fintoc.com Requires-Python: >=3.6,<4.0 Classifier:
-License :: OSI Approved :: BSD License Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.6 Classifier: Programming Language ::
-Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Requires-Dist: httpx (>=0.16,<1.0)
-Project-URL: Issue Tracker, https://github.com/fintoc-com/fintoc-python/issues
-Project-URL: Repository, https://github.com/fintoc-com/fintoc-python
-Description-Content-Type: text/markdown
                     ****** Fintoc meets Python ð ******
            You have just found the Python-flavored client of Fintoc.
                  [PyPI_-_Version] [Tests] [Coverage] [Linters]
-## Why? You can think of [Fintoc API](https://fintoc.com/docs) as a piscola.
-And the key ingredient to a properly made piscola are the ice cubes. Sure, you
-can still have a [piscola without ice cubes](https://curl.haxx.se/). But heyâ¦
-thatâs not enjoyable -- why would you do that? Do yourself a favor: go grab
-some ice cubes by installing this refreshing library. ## Installation Install
-using pip! ```sh pip install fintoc ``` **Note:** This SDK requires [**Python
-3.6+**](https://docs.python.org/3/whatsnew/3.6.html). ## Usage The idea behind
-this SDK is to stick to the API design as much as possible, so that it feels
-ridiculously natural to use even while only reading the raw API documentation.
-### Quickstart To be able to use this SDK, you first need to have a [Fintoc]
-(https://app.fintoc.com/login) account. You will need to get your secret API
-key from the dashboard to be able to use the SDK. Once you have your API key,
-all you need to do is initialize a `Fintoc` object with it and you're ready to
-start enjoying Fintoc! ```python from fintoc import Fintoc fintoc_client =
-Fintoc("your_api_key") ``` Now you can start using the SDK! ### Managers To
-make the usage of the SDK feel natural, resources are managed by **managers**
-(_wow_). These **managers** correspond to objects with some methods that allow
-you to get the resources that you want. Each manager is _attached_ to another
-resource, following the API structure. For example, the `Fintoc` object has
-`links` and `webhook_endpoints` managers, while `Link` objects have an
-`accounts` manager (we will see more examples soon). Notice that **not every
-manager has all of the methods**, as they correspond to the API capabilities.
-The methods of the managers are the following (we will use the
-`webhook_endpoints` manager as an example): #### `all` You can use the `all`
-method of the managers as follows: ```python webhook_endpoints =
+## Installation Install using pip! ```sh pip install fintoc ``` **Note:** This
+SDK requires [**Python 3.6+**](https://docs.python.org/3/whatsnew/3.6.html). ##
+Usage The idea behind this SDK is to stick to the API design as much as
+possible, so that it feels ridiculously natural to use even while only reading
+the raw API documentation. ### Quickstart To be able to use this SDK, you first
+need to have a [Fintoc](https://app.fintoc.com/login) account. You will need to
+get your secret API key from the dashboard to be able to use the SDK. Once you
+have your API key, all you need to do is initialize a `Fintoc` object with it
+and you're ready to start enjoying Fintoc! ```python from fintoc import Fintoc
+fintoc_client = Fintoc("your_api_key") ``` Now you can start using the SDK! ###
+Managers To make the usage of the SDK feel natural, resources are managed by
+**managers** (_wow_). These **managers** correspond to objects with some
+methods that allow you to get the resources that you want. Each manager is
+_attached_ to another resource, following the API structure. For example, the
+`Fintoc` object has `links` and `webhook_endpoints` managers, while `Link`
+objects have an `accounts` manager (we will see more examples soon). Notice
+that **not every manager has all of the methods**, as they correspond to the
+API capabilities. The methods of the managers are the following (we will use
+the `webhook_endpoints` manager as an example): #### `all` You can use the
+`all` method of the managers as follows: ```python webhook_endpoints =
 fintoc_client.webhook_endpoints.all() ``` The `all` method of the managers
 returns **a generator** with all the instances of the resource. This method can
 also receive `kwargs`! The arguments that can be passed are the arguments that
 the API receives for that specific resource! For example, the `Movement`
 resource can be filtered using `since` and `until`, so if you wanted to get a
 range of `movements` from an `account`, all you need to do is to pass the
 parameters to the method! ```python movements = account.movements.all
@@ -157,40 +140,49 @@
 link.refresh_intents.all() # Refresh Intents accounts = link.accounts.all() #
 Accounts ``` #### The `invoices` manager Available methods: `all`. Once you
 have a Link, you can use the `invoices` manager to get all the invoices
 associated to a link! ```python for invoice in link.invoices.all(): print
 (invoice.id) ``` #### The `tax_returns` manager Available methods: `all`,
 `get`. Once you have a Link, you can use the `tax_returns` manager to get all
 the tax returns associated to a link! ```python for tax_return in
-link.tax_returns.all(): print(tax_return.id) ``` #### The `subscriptions`
-manager Available methods: `all`, `get`. Once you have a Link, you can use the
-`subscriptions` manager to get all the subscriptions associated to a link!
-```python for subscription in link.subscriptions.all(): print(subscription.id)
-``` #### The `refresh_intents` manager Available methods: `all`, `get`,
-`create`. Refresh intents allow you to control how an account gets refreshed on
-Fintoc! Once you have a Link, you can use the `refresh_intents` manager to
-create a new refresh intent: ```python refresh_intent =
-link.refresh_intents.create() print(refresh_intent.id) # ri_5A94DVCJ7xNM3MEo
-``` Notice that the success of this refresh intent will be notified through a
-Webhook. Now, let's list every refresh intent we have: ```python for
-refresh_intent in link.refresh_intents.all(): print(refresh_intent.id) ``` If
-you see a refresh intent you want to use, just use the `get` method! ```python
-refresh_intent = link.refresh_intents.get("ri_5A94DVCJ7xNM3MEo") print
-(refresh_intent.id) # ri_5A94DVCJ7xNM3MEo print(refresh_intent.status) #
-succeeded ``` #### The `accounts` manager Available methods: `all`, `get`. Once
-you have a Link, you can use the `accounts` manager to get all the accounts
-associated to a link! ```python for account in link.accounts.all(): print
-(account.id) ``` Notice that accounts also have a `movements` manager, to get
-all of the movements of an account: ```python account = link.accounts.all
-(lazy=False)[0] movements = account.movements.all(lazy=False) ``` #### The
-`movements` manager Available methods: `all`, `get`. Once you have an Account,
-you can use the `movements` manager to get all the movements associated to that
-account! ```python for movement in account.movements.all(): print(movement.id)
-``` ### Serialization Any resource of the SDK can be serialized! To get the
-serialized resource, just call the `serialize` method! ```python account =
-link.accounts.all(lazy=False)[0] serialization = account.serialize() ``` The
-serialization corresponds to a dictionary with only simple types, that can be
-JSON-serialized. ## Acknowledgements The first version of this SDK was
-originally designed and handcrafted by [**@nebil**](https://github.com/nebil),
-[ad](https://en.wikipedia.org/wiki/Ad_honorem) [piscolem](https://
-en.wiktionary.org/wiki/piscola). He built it with the help of Gianni
-Robertoâs [Picchi 2](https://www.youtube.com/watch?v=WqjUlmkYr2g).
+link.tax_returns.all(): print(tax_return.id) ``` #### The `refresh_intents`
+manager Available methods: `all`, `get`, `create`. Refresh intents allow you to
+control how an account gets refreshed on Fintoc! Once you have a Link, you can
+use the `refresh_intents` manager to create a new refresh intent: ```python
+refresh_intent = link.refresh_intents.create() print(refresh_intent.id) #
+ri_5A94DVCJ7xNM3MEo ``` Notice that the success of this refresh intent will be
+notified through a Webhook. Now, let's list every refresh intent we have:
+```python for refresh_intent in link.refresh_intents.all(): print
+(refresh_intent.id) ``` If you see a refresh intent you want to use, just use
+the `get` method! ```python refresh_intent = link.refresh_intents.get
+("ri_5A94DVCJ7xNM3MEo") print(refresh_intent.id) # ri_5A94DVCJ7xNM3MEo print
+(refresh_intent.status) # succeeded ``` #### The `accounts` manager Available
+methods: `all`, `get`. Once you have a Link, you can use the `accounts` manager
+to get all the accounts associated to a link! ```python for account in
+link.accounts.all(): print(account.id) ``` Notice that accounts also have a
+`movements` manager, to get all of the movements of an account: ```python
+account = link.accounts.all(lazy=False)[0] movements = account.movements.all
+(lazy=False) ``` #### The `movements` manager Available methods: `all`, `get`.
+Once you have an Account, you can use the `movements` manager to get all the
+movements associated to that account! ```python for movement in
+account.movements.all(): print(movement.id) ``` #### The `subscription_intents`
+manager Available methods: `all`, `get`, `create` Subscription intents allow
+you to start a subscription using Fintoc!: ```python subscription_intent =
+fintoc_client.subscription_intents.create() print(subscription_intent.id) #
+si_BO381oEATXonG6bj print(subscription_intent.widget_token) #
+si_BO381oEATXonG6bj_sec_a4xK32BanKWYn ``` #### The `subscriptions` manager
+Available methods: `all`, `get` You can check the status of the created
+subscription with the `subscriptions` manager ```python subscription =
+fintoc_client.subscriptions.get('') print(subscription.status) ``` #### The
+`charges` manager Available methods: `all`, `get`, `create` Once you have
+active subscriptions, you can use the `charges` manager to create charges to
+thosse subscriptions ```python charge = fintoc_client.charges.create
+( currency='CLP', amount=1250, subscription_id='', ) ``` ### Serialization Any
+resource of the SDK can be serialized! To get the serialized resource, just
+call the `serialize` method! ```python account = link.accounts.all(lazy=False)
+[0] serialization = account.serialize() ``` The serialization corresponds to a
+dictionary with only simple types, that can be JSON-serialized. ##
+Acknowledgements The first version of this SDK was originally designed and
+handcrafted by [**@nebil**](https://github.com/nebil), [ad](https://
+en.wikipedia.org/wiki/Ad_honorem) [piscolem](https://en.wiktionary.org/wiki/
+piscola). He built it with the help of Gianni Robertoâs [Picchi 2](https://
+www.youtube.com/watch?v=WqjUlmkYr2g).
```

