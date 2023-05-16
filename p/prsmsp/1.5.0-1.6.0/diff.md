# Comparing `tmp/prsmsp-1.5.0.tar.gz` & `tmp/prsmsp-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prsmsp-1.5.0.tar", last modified: Sat May  6 18:52:46 2023, max compression
+gzip compressed data, was "prsmsp-1.6.0.tar", last modified: Tue May 16 18:59:47 2023, max compression
```

## Comparing `prsmsp-1.5.0.tar` & `prsmsp-1.6.0.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:52:46.213863 prsmsp-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-05-06 18:52:46.213863 prsmsp-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-06 18:52:35.000000 prsmsp-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:52:46.209863 prsmsp-1.5.0/prsmsp/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-06 18:52:35.000000 prsmsp-1.5.0/prsmsp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:52:46.209863 prsmsp-1.5.0/prsmsp/abstracts/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-06 18:52:35.000000 prsmsp-1.5.0/prsmsp/abstracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-06 18:52:35.000000 prsmsp-1.5.0/prsmsp/abstracts/abcpanel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:52:46.209863 prsmsp-1.5.0/prsmsp/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 18:52:35.000000 prsmsp-1.5.0/prsmsp/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 18:52:35.000000 prsmsp-1.5.0/prsmsp/exceptions/abstracts.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-06 18:52:35.000000 prsmsp-1.5.0/prsmsp/exceptions/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 18:52:35.000000 prsmsp-1.5.0/prsmsp/exceptions/panels.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:52:46.209863 prsmsp-1.5.0/prsmsp/factories/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-06 18:52:35.000000 prsmsp-1.5.0/prsmsp/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-06 18:52:35.000000 prsmsp-1.5.0/prsmsp/factories/auth_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:52:46.209863 prsmsp-1.5.0/prsmsp/models/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-06 18:52:35.000000 prsmsp-1.5.0/prsmsp/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-06 18:52:35.000000 prsmsp-1.5.0/prsmsp/models/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-06 18:52:35.000000 prsmsp-1.5.0/prsmsp/models/response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:52:46.209863 prsmsp-1.5.0/prsmsp/panels/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-06 18:52:35.000000 prsmsp-1.5.0/prsmsp/panels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-05-06 18:52:35.000000 prsmsp-1.5.0/prsmsp/panels/farazsms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-06 18:52:35.000000 prsmsp-1.5.0/prsmsp/panels/ghasedaksms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-05-06 18:52:35.000000 prsmsp-1.5.0/prsmsp/panels/kavenegar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-06 18:52:35.000000 prsmsp-1.5.0/prsmsp/panels/mediana.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-06 18:52:35.000000 prsmsp-1.5.0/prsmsp/panels/melipayamak.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-05-06 18:52:35.000000 prsmsp-1.5.0/prsmsp/panels/niksms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-05-06 18:52:35.000000 prsmsp-1.5.0/prsmsp/panels/smsdotir.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-06 18:52:35.000000 prsmsp-1.5.0/prsmsp/panels/smsone.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-05-06 18:52:35.000000 prsmsp-1.5.0/prsmsp/panels/webonesms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:52:46.209863 prsmsp-1.5.0/prsmsp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-05-06 18:52:46.000000 prsmsp-1.5.0/prsmsp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-06 18:52:46.000000 prsmsp-1.5.0/prsmsp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 18:52:46.000000 prsmsp-1.5.0/prsmsp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 18:52:46.000000 prsmsp-1.5.0/prsmsp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-06 18:52:46.000000 prsmsp-1.5.0/prsmsp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-06 18:52:46.000000 prsmsp-1.5.0/prsmsp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-06 18:52:46.213863 prsmsp-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-06 18:52:35.000000 prsmsp-1.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:52:46.213863 prsmsp-1.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 18:52:35.000000 prsmsp-1.5.0/tests/test_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:59:47.344678 prsmsp-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-05-16 18:59:47.344678 prsmsp-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-05-16 18:59:36.000000 prsmsp-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:59:47.340678 prsmsp-1.6.0/prsmsp/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-16 18:59:36.000000 prsmsp-1.6.0/prsmsp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:59:47.340678 prsmsp-1.6.0/prsmsp/abstracts/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-16 18:59:36.000000 prsmsp-1.6.0/prsmsp/abstracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-16 18:59:36.000000 prsmsp-1.6.0/prsmsp/abstracts/abcpanel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:59:47.340678 prsmsp-1.6.0/prsmsp/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:59:36.000000 prsmsp-1.6.0/prsmsp/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:59:36.000000 prsmsp-1.6.0/prsmsp/exceptions/abstracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-16 18:59:36.000000 prsmsp-1.6.0/prsmsp/exceptions/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:59:36.000000 prsmsp-1.6.0/prsmsp/exceptions/panels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:59:47.340678 prsmsp-1.6.0/prsmsp/factories/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-16 18:59:36.000000 prsmsp-1.6.0/prsmsp/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-16 18:59:36.000000 prsmsp-1.6.0/prsmsp/factories/auth_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:59:47.340678 prsmsp-1.6.0/prsmsp/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-16 18:59:36.000000 prsmsp-1.6.0/prsmsp/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-16 18:59:36.000000 prsmsp-1.6.0/prsmsp/models/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-16 18:59:36.000000 prsmsp-1.6.0/prsmsp/models/response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:59:47.344678 prsmsp-1.6.0/prsmsp/panels/
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-16 18:59:36.000000 prsmsp-1.6.0/prsmsp/panels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-05-16 18:59:36.000000 prsmsp-1.6.0/prsmsp/panels/farazsms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-16 18:59:36.000000 prsmsp-1.6.0/prsmsp/panels/ghasedaksms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-05-16 18:59:36.000000 prsmsp-1.6.0/prsmsp/panels/kavenegar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-16 18:59:36.000000 prsmsp-1.6.0/prsmsp/panels/mediana.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-16 18:59:36.000000 prsmsp-1.6.0/prsmsp/panels/melipayamak.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-05-16 18:59:36.000000 prsmsp-1.6.0/prsmsp/panels/niksms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-16 18:59:36.000000 prsmsp-1.6.0/prsmsp/panels/sapak.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-05-16 18:59:36.000000 prsmsp-1.6.0/prsmsp/panels/smsdotir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-16 18:59:36.000000 prsmsp-1.6.0/prsmsp/panels/smsone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-05-16 18:59:36.000000 prsmsp-1.6.0/prsmsp/panels/webonesms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:59:47.340678 prsmsp-1.6.0/prsmsp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-05-16 18:59:47.000000 prsmsp-1.6.0/prsmsp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-16 18:59:47.000000 prsmsp-1.6.0/prsmsp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 18:59:47.000000 prsmsp-1.6.0/prsmsp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 18:59:47.000000 prsmsp-1.6.0/prsmsp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-16 18:59:47.000000 prsmsp-1.6.0/prsmsp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-16 18:59:47.000000 prsmsp-1.6.0/prsmsp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-16 18:59:47.344678 prsmsp-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-16 18:59:36.000000 prsmsp-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:59:47.344678 prsmsp-1.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:59:36.000000 prsmsp-1.6.0/tests/test_app.py
```

### Comparing `prsmsp-1.5.0/PKG-INFO` & `prsmsp-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prsmsp
-Version: 1.5.0
+Version: 1.6.0
 Summary: Package to work with sms panels
 Home-page: https://github.com/parsariyahi/prsmsp
 Author: Parsa Riyahi
 Author-email: pany.parsariyahi@gmail.com
 License: MIT License
 Project-URL: Homepage, https://github.com/parsariyahi/prsmsp
 Project-URL: Documentation, https://prsmsp.readthedocs.io/en/latest/
@@ -51,14 +51,15 @@
 * [Web one](http://webone-sms.ir)
 * [Meli Payamak](https://www.melipayamak.com)
 * [Mediana](https://mediana.ir)
 * [Ghasedak Sms](https://ghasedak.me)
 * [Faraz Sms](https://farazsms.com/)
 * [Nik Sms](https://niksms.com/)
 * [Sms1](https://sms1.ir/)
+* [Sapak](https://sapak.me/)
 
 <br>
 
 # How to use?
 First lets install the package
 ```shell
 pip install prsmsp
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: prsmsp Version: 1.5.0 Summary: Package to work with
+Metadata-Version: 2.1 Name: prsmsp Version: 1.6.0 Summary: Package to work with
 sms panels Home-page: https://github.com/parsariyahi/prsmsp Author: Parsa
 Riyahi Author-email: pany.parsariyahi@gmail.com License: MIT License Project-
 URL: Homepage, https://github.com/parsariyahi/prsmsp Project-URL:
 Documentation, https://prsmsp.readthedocs.io/en/latest/ Project-URL: Source,
 https://github.com/parsariyahi/prsmsp Project-URL: Tracker, https://github.com/
 parsariyahi/prsmsp/issues Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python Classifier: Programming Language ::
@@ -23,15 +23,15 @@
   You have all the famous and well designed SMS panels ready to go. - You can
  have several SMS panels at the same time. - Don't need to build the wheel of
    your bicycle each time âº. - Fast and Small - Easy to implement and use
    # Supported panels * [Kavenegar](http://kavenegar.com) * [Sms.ir](http://
       sms.ir) * [Web one](http://webone-sms.ir) * [Meli Payamak](https://
 www.melipayamak.com) * [Mediana](https://mediana.ir) * [Ghasedak Sms](https://
     ghasedak.me) * [Faraz Sms](https://farazsms.com/) * [Nik Sms](https://
-                   niksms.com/) * [Sms1](https://sms1.ir/)
+     niksms.com/) * [Sms1](https://sms1.ir/) * [Sapak](https://sapak.me/)
  # How to use? First lets install the package ```shell pip install prsmsp ```
  This block of code is for **kavenegar** sms panel. Each of sms panels has its
   own parameters. Please read their docs first. ```python from prsmsp.panels
   import Kavenegar api_key = "your api key" panel = Kavenegar(api_key) # auth
  receptor = "your receptor" msg = "your message" panel.send_sms(receptor, msg)
  ``` #### [Docs](https://prsmsp.readthedocs.io/en/latest/panels/panels.html)
  # How to support this project? for this project to be better and bigger than
```

### Comparing `prsmsp-1.5.0/README.md` & `prsmsp-1.6.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 * [Web one](http://webone-sms.ir)
 * [Meli Payamak](https://www.melipayamak.com)
 * [Mediana](https://mediana.ir)
 * [Ghasedak Sms](https://ghasedak.me)
 * [Faraz Sms](https://farazsms.com/)
 * [Nik Sms](https://niksms.com/)
 * [Sms1](https://sms1.ir/)
+* [Sapak](https://sapak.me/)
 
 <br>
 
 # How to use?
 First lets install the package
 ```shell
 pip install prsmsp
```

#### html2text {}

```diff
@@ -12,15 +12,15 @@
   You have all the famous and well designed SMS panels ready to go. - You can
  have several SMS panels at the same time. - Don't need to build the wheel of
    your bicycle each time âº. - Fast and Small - Easy to implement and use
    # Supported panels * [Kavenegar](http://kavenegar.com) * [Sms.ir](http://
       sms.ir) * [Web one](http://webone-sms.ir) * [Meli Payamak](https://
 www.melipayamak.com) * [Mediana](https://mediana.ir) * [Ghasedak Sms](https://
     ghasedak.me) * [Faraz Sms](https://farazsms.com/) * [Nik Sms](https://
-                   niksms.com/) * [Sms1](https://sms1.ir/)
+     niksms.com/) * [Sms1](https://sms1.ir/) * [Sapak](https://sapak.me/)
  # How to use? First lets install the package ```shell pip install prsmsp ```
  This block of code is for **kavenegar** sms panel. Each of sms panels has its
   own parameters. Please read their docs first. ```python from prsmsp.panels
   import Kavenegar api_key = "your api key" panel = Kavenegar(api_key) # auth
  receptor = "your receptor" msg = "your message" panel.send_sms(receptor, msg)
  ``` #### [Docs](https://prsmsp.readthedocs.io/en/latest/panels/panels.html)
  # How to support this project? for this project to be better and bigger than
```

### Comparing `prsmsp-1.5.0/prsmsp/factories/auth_factory.py` & `prsmsp-1.6.0/prsmsp/factories/auth_factory.py`

 * *Files identical despite different names*

### Comparing `prsmsp-1.5.0/prsmsp/models/response.py` & `prsmsp-1.6.0/prsmsp/models/response.py`

 * *Files identical despite different names*

### Comparing `prsmsp-1.5.0/prsmsp/panels/farazsms.py` & `prsmsp-1.6.0/prsmsp/panels/farazsms.py`

 * *Files identical despite different names*

### Comparing `prsmsp-1.5.0/prsmsp/panels/ghasedaksms.py` & `prsmsp-1.6.0/prsmsp/panels/ghasedaksms.py`

 * *Files identical despite different names*

### Comparing `prsmsp-1.5.0/prsmsp/panels/kavenegar.py` & `prsmsp-1.6.0/prsmsp/panels/kavenegar.py`

 * *Files identical despite different names*

### Comparing `prsmsp-1.5.0/prsmsp/panels/mediana.py` & `prsmsp-1.6.0/prsmsp/panels/mediana.py`

 * *Files identical despite different names*

### Comparing `prsmsp-1.5.0/prsmsp/panels/melipayamak.py` & `prsmsp-1.6.0/prsmsp/panels/melipayamak.py`

 * *Files identical despite different names*

### Comparing `prsmsp-1.5.0/prsmsp/panels/niksms.py` & `prsmsp-1.6.0/prsmsp/panels/niksms.py`

 * *Files identical despite different names*

### Comparing `prsmsp-1.5.0/prsmsp/panels/smsdotir.py` & `prsmsp-1.6.0/prsmsp/panels/smsdotir.py`

 * *Files identical despite different names*

### Comparing `prsmsp-1.5.0/prsmsp/panels/smsone.py` & `prsmsp-1.6.0/prsmsp/panels/smsone.py`

 * *Files identical despite different names*

### Comparing `prsmsp-1.5.0/prsmsp/panels/webonesms.py` & `prsmsp-1.6.0/prsmsp/panels/webonesms.py`

 * *Files identical despite different names*

### Comparing `prsmsp-1.5.0/prsmsp.egg-info/PKG-INFO` & `prsmsp-1.6.0/prsmsp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prsmsp
-Version: 1.5.0
+Version: 1.6.0
 Summary: Package to work with sms panels
 Home-page: https://github.com/parsariyahi/prsmsp
 Author: Parsa Riyahi
 Author-email: pany.parsariyahi@gmail.com
 License: MIT License
 Project-URL: Homepage, https://github.com/parsariyahi/prsmsp
 Project-URL: Documentation, https://prsmsp.readthedocs.io/en/latest/
@@ -51,14 +51,15 @@
 * [Web one](http://webone-sms.ir)
 * [Meli Payamak](https://www.melipayamak.com)
 * [Mediana](https://mediana.ir)
 * [Ghasedak Sms](https://ghasedak.me)
 * [Faraz Sms](https://farazsms.com/)
 * [Nik Sms](https://niksms.com/)
 * [Sms1](https://sms1.ir/)
+* [Sapak](https://sapak.me/)
 
 <br>
 
 # How to use?
 First lets install the package
 ```shell
 pip install prsmsp
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: prsmsp Version: 1.5.0 Summary: Package to work with
+Metadata-Version: 2.1 Name: prsmsp Version: 1.6.0 Summary: Package to work with
 sms panels Home-page: https://github.com/parsariyahi/prsmsp Author: Parsa
 Riyahi Author-email: pany.parsariyahi@gmail.com License: MIT License Project-
 URL: Homepage, https://github.com/parsariyahi/prsmsp Project-URL:
 Documentation, https://prsmsp.readthedocs.io/en/latest/ Project-URL: Source,
 https://github.com/parsariyahi/prsmsp Project-URL: Tracker, https://github.com/
 parsariyahi/prsmsp/issues Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python Classifier: Programming Language ::
@@ -23,15 +23,15 @@
   You have all the famous and well designed SMS panels ready to go. - You can
  have several SMS panels at the same time. - Don't need to build the wheel of
    your bicycle each time âº. - Fast and Small - Easy to implement and use
    # Supported panels * [Kavenegar](http://kavenegar.com) * [Sms.ir](http://
       sms.ir) * [Web one](http://webone-sms.ir) * [Meli Payamak](https://
 www.melipayamak.com) * [Mediana](https://mediana.ir) * [Ghasedak Sms](https://
     ghasedak.me) * [Faraz Sms](https://farazsms.com/) * [Nik Sms](https://
-                   niksms.com/) * [Sms1](https://sms1.ir/)
+     niksms.com/) * [Sms1](https://sms1.ir/) * [Sapak](https://sapak.me/)
  # How to use? First lets install the package ```shell pip install prsmsp ```
  This block of code is for **kavenegar** sms panel. Each of sms panels has its
   own parameters. Please read their docs first. ```python from prsmsp.panels
   import Kavenegar api_key = "your api key" panel = Kavenegar(api_key) # auth
  receptor = "your receptor" msg = "your message" panel.send_sms(receptor, msg)
  ``` #### [Docs](https://prsmsp.readthedocs.io/en/latest/panels/panels.html)
  # How to support this project? for this project to be better and bigger than
```

### Comparing `prsmsp-1.5.0/prsmsp.egg-info/SOURCES.txt` & `prsmsp-1.6.0/prsmsp.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -22,11 +22,12 @@
 prsmsp/panels/__init__.py
 prsmsp/panels/farazsms.py
 prsmsp/panels/ghasedaksms.py
 prsmsp/panels/kavenegar.py
 prsmsp/panels/mediana.py
 prsmsp/panels/melipayamak.py
 prsmsp/panels/niksms.py
+prsmsp/panels/sapak.py
 prsmsp/panels/smsdotir.py
 prsmsp/panels/smsone.py
 prsmsp/panels/webonesms.py
 tests/test_app.py
```

### Comparing `prsmsp-1.5.0/setup.cfg` & `prsmsp-1.6.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = prsmsp
-version = 1.5.0
+version = 1.6.0
 author = Parsa Riyahi
 author_email = pany.parsariyahi@gmail.com
 description = Package to work with sms panels
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT License
 license_files = file: LICENSE
```

