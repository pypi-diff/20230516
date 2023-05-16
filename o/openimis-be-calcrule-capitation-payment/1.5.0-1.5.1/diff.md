# Comparing `tmp/openimis-be-calcrule-capitation_payment-1.5.0.tar.gz` & `tmp/openimis-be-calcrule-capitation_payment-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis-be-calcrule-capitation_payment-1.5.0.tar", last modified: Fri Nov 11 08:12:28 2022, max compression
+gzip compressed data, was "openimis-be-calcrule-capitation_payment-1.5.1.tar", last modified: Tue May 16 21:38:52 2023, max compression
```

## Comparing `openimis-be-calcrule-capitation_payment-1.5.0.tar` & `openimis-be-calcrule-capitation_payment-1.5.1.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:28.491779 openimis-be-calcrule-capitation_payment-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (121)    34523 2022-11-11 08:12:17.000000 openimis-be-calcrule-capitation_payment-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1473 2022-11-11 08:12:28.491779 openimis-be-calcrule-capitation_payment-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      695 2022-11-11 08:12:17.000000 openimis-be-calcrule-capitation_payment-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:28.483779 openimis-be-calcrule-capitation_payment-1.5.0/calcrule_capitation_payment/
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-11-11 08:12:17.000000 openimis-be-calcrule-capitation_payment-1.5.0/calcrule_capitation_payment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-11-11 08:12:17.000000 openimis-be-calcrule-capitation_payment-1.5.0/calcrule_capitation_payment/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)      857 2022-11-11 08:12:17.000000 openimis-be-calcrule-capitation_payment-1.5.0/calcrule_capitation_payment/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)    12392 2022-11-11 08:12:17.000000 openimis-be-calcrule-capitation_payment-1.5.0/calcrule_capitation_payment/calculation_rule.py
--rw-r--r--   0 runner    (1001) docker     (121)    38359 2022-11-11 08:12:17.000000 openimis-be-calcrule-capitation_payment-1.5.0/calcrule_capitation_payment/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:28.487779 openimis-be-calcrule-capitation_payment-1.5.0/calcrule_capitation_payment/converters/
--rw-r--r--   0 runner    (1001) docker     (121)      213 2022-11-11 08:12:17.000000 openimis-be-calcrule-capitation_payment-1.5.0/calcrule_capitation_payment/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2494 2022-11-11 08:12:17.000000 openimis-be-calcrule-capitation_payment-1.5.0/calcrule_capitation_payment/converters/batch_run_to_bill.py
--rw-r--r--   0 runner    (1001) docker     (121)     4020 2022-11-11 08:12:17.000000 openimis-be-calcrule-capitation_payment-1.5.0/calcrule_capitation_payment/converters/capitation_payment_to_bill_item.py
--rw-r--r--   0 runner    (1001) docker     (121)      699 2022-11-11 08:12:17.000000 openimis-be-calcrule-capitation_payment-1.5.0/calcrule_capitation_payment/legacy.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:28.487779 openimis-be-calcrule-capitation_payment-1.5.0/calcrule_capitation_payment/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     5643 2022-11-11 08:12:17.000000 openimis-be-calcrule-capitation_payment-1.5.0/calcrule_capitation_payment/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)      230 2022-11-11 08:12:17.000000 openimis-be-calcrule-capitation_payment-1.5.0/calcrule_capitation_payment/migrations/0002_delete_capitationpayment.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:17.000000 openimis-be-calcrule-capitation_payment-1.5.0/calcrule_capitation_payment/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:17.000000 openimis-be-calcrule-capitation_payment-1.5.0/calcrule_capitation_payment/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     9218 2022-11-11 08:12:17.000000 openimis-be-calcrule-capitation_payment-1.5.0/calcrule_capitation_payment/tests.py
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-11-11 08:12:17.000000 openimis-be-calcrule-capitation_payment-1.5.0/calcrule_capitation_payment/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)    21665 2022-11-11 08:12:17.000000 openimis-be-calcrule-capitation_payment-1.5.0/calcrule_capitation_payment/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-11-11 08:12:17.000000 openimis-be-calcrule-capitation_payment-1.5.0/calcrule_capitation_payment/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:28.491779 openimis-be-calcrule-capitation_payment-1.5.0/openimis_be_calcrule_capitation_payment.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1473 2022-11-11 08:12:28.000000 openimis-be-calcrule-capitation_payment-1.5.0/openimis_be_calcrule_capitation_payment.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1125 2022-11-11 08:12:28.000000 openimis-be-calcrule-capitation_payment-1.5.0/openimis_be_calcrule_capitation_payment.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-11 08:12:28.000000 openimis-be-calcrule-capitation_payment-1.5.0/openimis_be_calcrule_capitation_payment.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-11-11 08:12:28.000000 openimis-be-calcrule-capitation_payment-1.5.0/openimis_be_calcrule_capitation_payment.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-11-11 08:12:28.000000 openimis-be-calcrule-capitation_payment-1.5.0/openimis_be_calcrule_capitation_payment.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-11 08:12:28.491779 openimis-be-calcrule-capitation_payment-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1348 2022-11-11 08:12:26.000000 openimis-be-calcrule-capitation_payment-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:52.018333 openimis-be-calcrule-capitation_payment-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-16 21:38:41.000000 openimis-be-calcrule-capitation_payment-1.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-16 21:38:52.018333 openimis-be-calcrule-capitation_payment-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-16 21:38:41.000000 openimis-be-calcrule-capitation_payment-1.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:52.018333 openimis-be-calcrule-capitation_payment-1.5.1/calcrule_capitation_payment/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-16 21:38:41.000000 openimis-be-calcrule-capitation_payment-1.5.1/calcrule_capitation_payment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-16 21:38:41.000000 openimis-be-calcrule-capitation_payment-1.5.1/calcrule_capitation_payment/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-16 21:38:41.000000 openimis-be-calcrule-capitation_payment-1.5.1/calcrule_capitation_payment/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12392 2023-05-16 21:38:41.000000 openimis-be-calcrule-capitation_payment-1.5.1/calcrule_capitation_payment/calculation_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38368 2023-05-16 21:38:41.000000 openimis-be-calcrule-capitation_payment-1.5.1/calcrule_capitation_payment/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:52.018333 openimis-be-calcrule-capitation_payment-1.5.1/calcrule_capitation_payment/converters/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-16 21:38:41.000000 openimis-be-calcrule-capitation_payment-1.5.1/calcrule_capitation_payment/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-05-16 21:38:41.000000 openimis-be-calcrule-capitation_payment-1.5.1/calcrule_capitation_payment/converters/batch_run_to_bill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-05-16 21:38:41.000000 openimis-be-calcrule-capitation_payment-1.5.1/calcrule_capitation_payment/converters/capitation_payment_to_bill_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-16 21:38:41.000000 openimis-be-calcrule-capitation_payment-1.5.1/calcrule_capitation_payment/legacy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:52.018333 openimis-be-calcrule-capitation_payment-1.5.1/calcrule_capitation_payment/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-05-16 21:38:41.000000 openimis-be-calcrule-capitation_payment-1.5.1/calcrule_capitation_payment/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-16 21:38:41.000000 openimis-be-calcrule-capitation_payment-1.5.1/calcrule_capitation_payment/migrations/0002_delete_capitationpayment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-16 21:38:41.000000 openimis-be-calcrule-capitation_payment-1.5.1/calcrule_capitation_payment/migrations/0003_delete_capitationpayment.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:41.000000 openimis-be-calcrule-capitation_payment-1.5.1/calcrule_capitation_payment/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:41.000000 openimis-be-calcrule-capitation_payment-1.5.1/calcrule_capitation_payment/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9218 2023-05-16 21:38:41.000000 openimis-be-calcrule-capitation_payment-1.5.1/calcrule_capitation_payment/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 21:38:41.000000 openimis-be-calcrule-capitation_payment-1.5.1/calcrule_capitation_payment/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21665 2023-05-16 21:38:41.000000 openimis-be-calcrule-capitation_payment-1.5.1/calcrule_capitation_payment/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-16 21:38:41.000000 openimis-be-calcrule-capitation_payment-1.5.1/calcrule_capitation_payment/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:52.018333 openimis-be-calcrule-capitation_payment-1.5.1/openimis_be_calcrule_capitation_payment.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-16 21:38:51.000000 openimis-be-calcrule-capitation_payment-1.5.1/openimis_be_calcrule_capitation_payment.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-16 21:38:51.000000 openimis-be-calcrule-capitation_payment-1.5.1/openimis_be_calcrule_capitation_payment.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 21:38:51.000000 openimis-be-calcrule-capitation_payment-1.5.1/openimis_be_calcrule_capitation_payment.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-16 21:38:51.000000 openimis-be-calcrule-capitation_payment-1.5.1/openimis_be_calcrule_capitation_payment.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-16 21:38:51.000000 openimis-be-calcrule-capitation_payment-1.5.1/openimis_be_calcrule_capitation_payment.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 21:38:52.018333 openimis-be-calcrule-capitation_payment-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-05-16 21:38:50.000000 openimis-be-calcrule-capitation_payment-1.5.1/setup.py
```

### Comparing `openimis-be-calcrule-capitation_payment-1.5.0/LICENSE` & `openimis-be-calcrule-capitation_payment-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule-capitation_payment-1.5.0/PKG-INFO` & `openimis-be-calcrule-capitation_payment-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-calcrule-capitation_payment
-Version: 1.5.0
+Version: 1.5.1
 Summary: The openIMIS Backend calculation rule capitation payment reference module.
 Home-page: https://openimis.org/
 Author: Seweryn Niedzielski
 Author-email: sniedzielski@soldevelo.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-calcrule-capitation_payment-1.5.0/README.md` & `openimis-be-calcrule-capitation_payment-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule-capitation_payment-1.5.0/calcrule_capitation_payment/apps.py` & `openimis-be-calcrule-capitation_payment-1.5.1/calcrule_capitation_payment/apps.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule-capitation_payment-1.5.0/calcrule_capitation_payment/calculation_rule.py` & `openimis-be-calcrule-capitation_payment-1.5.1/calcrule_capitation_payment/calculation_rule.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule-capitation_payment-1.5.0/calcrule_capitation_payment/config.py` & `openimis-be-calcrule-capitation_payment-1.5.1/calcrule_capitation_payment/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -431,16 +431,16 @@
             "condition": "INPUT<100",
             "default": ""
          },
          {
             "type": "number",
             "name": "weight_insured_population",
             "label": {
-               "en": "Weight Number Population",
-               "fr": "Weight Number Population"
+               "en": "Weight of Insured Population",
+               "fr": "Weight of Insured Population"
             },
             "rights": {
                "read": "121001",
                "write": "121002",
                "update": "121003",
                "replace": "121006"
             },
@@ -492,15 +492,15 @@
             "rights": {
                "read": "121001",
                "write": "121002",
                "update": "121003",
                "replace": "121006"
             },
             "relevance": "True",
-            "condition": "INPUT<100",
+            "condition": "INPUT<=100",
             "default": ""
          },
          {
             "type": "number",
             "default": "0",
             "name": "distr_1",
             "label": {
```

### Comparing `openimis-be-calcrule-capitation_payment-1.5.0/calcrule_capitation_payment/converters/batch_run_to_bill.py` & `openimis-be-calcrule-capitation_payment-1.5.1/calcrule_capitation_payment/converters/batch_run_to_bill.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule-capitation_payment-1.5.0/calcrule_capitation_payment/converters/capitation_payment_to_bill_item.py` & `openimis-be-calcrule-capitation_payment-1.5.1/calcrule_capitation_payment/converters/capitation_payment_to_bill_item.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule-capitation_payment-1.5.0/calcrule_capitation_payment/legacy.py` & `openimis-be-calcrule-capitation_payment-1.5.1/calcrule_capitation_payment/legacy.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule-capitation_payment-1.5.0/calcrule_capitation_payment/migrations/0001_initial.py` & `openimis-be-calcrule-capitation_payment-1.5.1/calcrule_capitation_payment/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule-capitation_payment-1.5.0/calcrule_capitation_payment/tests.py` & `openimis-be-calcrule-capitation_payment-1.5.1/calcrule_capitation_payment/tests.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule-capitation_payment-1.5.0/calcrule_capitation_payment/utils.py` & `openimis-be-calcrule-capitation_payment-1.5.1/calcrule_capitation_payment/utils.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule-capitation_payment-1.5.0/openimis_be_calcrule_capitation_payment.egg-info/PKG-INFO` & `openimis-be-calcrule-capitation_payment-1.5.1/openimis_be_calcrule_capitation_payment.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-calcrule-capitation-payment
-Version: 1.5.0
+Version: 1.5.1
 Summary: The openIMIS Backend calculation rule capitation payment reference module.
 Home-page: https://openimis.org/
 Author: Seweryn Niedzielski
 Author-email: sniedzielski@soldevelo.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-calcrule-capitation_payment-1.5.0/openimis_be_calcrule_capitation_payment.egg-info/SOURCES.txt` & `openimis-be-calcrule-capitation_payment-1.5.1/openimis_be_calcrule_capitation_payment.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,13 +13,14 @@
 calcrule_capitation_payment/utils.py
 calcrule_capitation_payment/views.py
 calcrule_capitation_payment/converters/__init__.py
 calcrule_capitation_payment/converters/batch_run_to_bill.py
 calcrule_capitation_payment/converters/capitation_payment_to_bill_item.py
 calcrule_capitation_payment/migrations/0001_initial.py
 calcrule_capitation_payment/migrations/0002_delete_capitationpayment.py
+calcrule_capitation_payment/migrations/0003_delete_capitationpayment.py
 calcrule_capitation_payment/migrations/__init__.py
 openimis_be_calcrule_capitation_payment.egg-info/PKG-INFO
 openimis_be_calcrule_capitation_payment.egg-info/SOURCES.txt
 openimis_be_calcrule_capitation_payment.egg-info/dependency_links.txt
 openimis_be_calcrule_capitation_payment.egg-info/requires.txt
 openimis_be_calcrule_capitation_payment.egg-info/top_level.txt
```

### Comparing `openimis-be-calcrule-capitation_payment-1.5.0/setup.py` & `openimis-be-calcrule-capitation_payment-1.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='openimis-be-calcrule-capitation_payment',
-    version='1.5.0',
+    version='v1.5.1',
     packages=find_packages(),
     include_package_data=True,
     license='GNU AGPL v3',
     description='The openIMIS Backend calculation rule capitation payment reference module.',
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://openimis.org/',
```

