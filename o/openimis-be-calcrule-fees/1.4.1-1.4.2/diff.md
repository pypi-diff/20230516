# Comparing `tmp/openimis-be-calcrule_fees-1.4.1.tar.gz` & `tmp/openimis-be-calcrule_fees-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis-be-calcrule_fees-1.4.1.tar", last modified: Fri Nov 11 08:12:37 2022, max compression
+gzip compressed data, was "openimis-be-calcrule_fees-1.4.2.tar", last modified: Tue May 16 21:51:17 2023, max compression
```

## Comparing `openimis-be-calcrule_fees-1.4.1.tar` & `openimis-be-calcrule_fees-1.4.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:37.096203 openimis-be-calcrule_fees-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1390 2022-11-11 08:12:37.096203 openimis-be-calcrule_fees-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      663 2022-11-11 08:12:27.000000 openimis-be-calcrule_fees-1.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:37.092203 openimis-be-calcrule_fees-1.4.1/calcrule_fees/
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-11-11 08:12:27.000000 openimis-be-calcrule_fees-1.4.1/calcrule_fees/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-11-11 08:12:27.000000 openimis-be-calcrule_fees-1.4.1/calcrule_fees/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)      816 2022-11-11 08:12:27.000000 openimis-be-calcrule_fees-1.4.1/calcrule_fees/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)    10579 2022-11-11 08:12:27.000000 openimis-be-calcrule_fees-1.4.1/calcrule_fees/calculation_rule.py
--rw-r--r--   0 runner    (1001) docker     (121)     1595 2022-11-11 08:12:27.000000 openimis-be-calcrule_fees-1.4.1/calcrule_fees/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:37.092203 openimis-be-calcrule_fees-1.4.1/calcrule_fees/converters/
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-11-11 08:12:27.000000 openimis-be-calcrule_fees-1.4.1/calcrule_fees/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2938 2022-11-11 08:12:27.000000 openimis-be-calcrule_fees-1.4.1/calcrule_fees/converters/batch_run_to_bill.py
--rw-r--r--   0 runner    (1001) docker     (121)     2813 2022-11-11 08:12:27.000000 openimis-be-calcrule_fees-1.4.1/calcrule_fees/converters/invoice_payment_to_bill_item.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:37.092203 openimis-be-calcrule_fees-1.4.1/calcrule_fees/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:27.000000 openimis-be-calcrule_fees-1.4.1/calcrule_fees/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-11-11 08:12:27.000000 openimis-be-calcrule_fees-1.4.1/calcrule_fees/models.py
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-11-11 08:12:27.000000 openimis-be-calcrule_fees-1.4.1/calcrule_fees/tests.py
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-11-11 08:12:27.000000 openimis-be-calcrule_fees-1.4.1/calcrule_fees/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-11-11 08:12:27.000000 openimis-be-calcrule_fees-1.4.1/calcrule_fees/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:37.092203 openimis-be-calcrule_fees-1.4.1/openimis_be_calcrule_fees.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1390 2022-11-11 08:12:37.000000 openimis-be-calcrule_fees-1.4.1/openimis_be_calcrule_fees.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      660 2022-11-11 08:12:37.000000 openimis-be-calcrule_fees-1.4.1/openimis_be_calcrule_fees.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-11 08:12:37.000000 openimis-be-calcrule_fees-1.4.1/openimis_be_calcrule_fees.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-11-11 08:12:37.000000 openimis-be-calcrule_fees-1.4.1/openimis_be_calcrule_fees.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-11-11 08:12:37.000000 openimis-be-calcrule_fees-1.4.1/openimis_be_calcrule_fees.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-11 08:12:37.096203 openimis-be-calcrule_fees-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1320 2022-11-11 08:12:36.000000 openimis-be-calcrule_fees-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:51:17.404241 openimis-be-calcrule_fees-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-16 21:51:17.404241 openimis-be-calcrule_fees-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-16 21:51:03.000000 openimis-be-calcrule_fees-1.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:51:17.400241 openimis-be-calcrule_fees-1.4.2/calcrule_fees/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-16 21:51:03.000000 openimis-be-calcrule_fees-1.4.2/calcrule_fees/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-16 21:51:03.000000 openimis-be-calcrule_fees-1.4.2/calcrule_fees/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-16 21:51:03.000000 openimis-be-calcrule_fees-1.4.2/calcrule_fees/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10579 2023-05-16 21:51:03.000000 openimis-be-calcrule_fees-1.4.2/calcrule_fees/calculation_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-16 21:51:03.000000 openimis-be-calcrule_fees-1.4.2/calcrule_fees/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:51:17.400241 openimis-be-calcrule_fees-1.4.2/calcrule_fees/converters/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-16 21:51:03.000000 openimis-be-calcrule_fees-1.4.2/calcrule_fees/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-05-16 21:51:03.000000 openimis-be-calcrule_fees-1.4.2/calcrule_fees/converters/batch_run_to_bill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-16 21:51:03.000000 openimis-be-calcrule_fees-1.4.2/calcrule_fees/converters/invoice_payment_to_bill_item.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:51:17.400241 openimis-be-calcrule_fees-1.4.2/calcrule_fees/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:51:03.000000 openimis-be-calcrule_fees-1.4.2/calcrule_fees/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-16 21:51:03.000000 openimis-be-calcrule_fees-1.4.2/calcrule_fees/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-16 21:51:03.000000 openimis-be-calcrule_fees-1.4.2/calcrule_fees/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 21:51:03.000000 openimis-be-calcrule_fees-1.4.2/calcrule_fees/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-16 21:51:03.000000 openimis-be-calcrule_fees-1.4.2/calcrule_fees/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:51:17.404241 openimis-be-calcrule_fees-1.4.2/openimis_be_calcrule_fees.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-16 21:51:17.000000 openimis-be-calcrule_fees-1.4.2/openimis_be_calcrule_fees.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-16 21:51:17.000000 openimis-be-calcrule_fees-1.4.2/openimis_be_calcrule_fees.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 21:51:17.000000 openimis-be-calcrule_fees-1.4.2/openimis_be_calcrule_fees.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-16 21:51:17.000000 openimis-be-calcrule_fees-1.4.2/openimis_be_calcrule_fees.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-16 21:51:17.000000 openimis-be-calcrule_fees-1.4.2/openimis_be_calcrule_fees.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 21:51:17.404241 openimis-be-calcrule_fees-1.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-16 21:51:15.000000 openimis-be-calcrule_fees-1.4.2/setup.py
```

### Comparing `openimis-be-calcrule_fees-1.4.1/calcrule_fees/apps.py` & `openimis-be-calcrule_fees-1.4.2/calcrule_fees/apps.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule_fees-1.4.1/calcrule_fees/calculation_rule.py` & `openimis-be-calcrule_fees-1.4.2/calcrule_fees/calculation_rule.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule_fees-1.4.1/calcrule_fees/config.py` & `openimis-be-calcrule_fees-1.4.2/calcrule_fees/config.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule_fees-1.4.1/calcrule_fees/converters/batch_run_to_bill.py` & `openimis-be-calcrule_fees-1.4.2/calcrule_fees/converters/batch_run_to_bill.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule_fees-1.4.1/calcrule_fees/converters/invoice_payment_to_bill_item.py` & `openimis-be-calcrule_fees-1.4.2/calcrule_fees/converters/invoice_payment_to_bill_item.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule_fees-1.4.1/openimis_be_calcrule_fees.egg-info/PKG-INFO` & `openimis-be-calcrule_fees-1.4.2/openimis_be_calcrule_fees.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-calcrule-fees
-Version: 1.4.1
+Version: 1.4.2
 Summary: The openIMIS Backend calculation rule fees reference module.
 Home-page: https://openimis.org/
 Author: Seweryn Niedzielski
 Author-email: sniedzielski@soldevelo.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -13,16 +13,15 @@
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 
-# openimis-be-calcrule-fees_py
-This repository holds the files of the openIMIS backend calculation rule fees reference module.
-It is dedicated to be deployed as a module of [openimis-be_py](https://github.com/openimis/openimis-be_py). It is an 
-extended part of calculation module [openimis-be-calculation_py](https://github.com/openimis/openimis-be-calculation_py) 
-and therefore that module is dependent on this core calculation module. This module contains additional calculation rules. 
+# Calcrule to calculate Paymen fees for payment source
 
-## Models
-  - None (using no database approach for CalculationRule) - Calculation Rule is saved by defining class 
-    extending the ABSCalculationClass from core module.
+
+ This calculation will, for the selected level and product, calculate how much the insurance need to pay the payment platform for the fee for payment service
+ 
+ it create bill for the payment platform based on the contribution made through that platform attached to invoice item
+ 
+ https://openimis.atlassian.net/wiki/spaces/OP/pages/3045818376/Payment+plan+calculation+rule+fees
```

### Comparing `openimis-be-calcrule_fees-1.4.1/openimis_be_calcrule_fees.egg-info/SOURCES.txt` & `openimis-be-calcrule_fees-1.4.2/openimis_be_calcrule_fees.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule_fees-1.4.1/setup.py` & `openimis-be-calcrule_fees-1.4.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='openimis-be-calcrule_fees',
-    version='1.4.1',
+    version='v1.4.2',
     packages=find_packages(),
     include_package_data=True,
     license='GNU AGPL v3',
     description='The openIMIS Backend calculation rule fees reference module.',
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://openimis.org/',
```

