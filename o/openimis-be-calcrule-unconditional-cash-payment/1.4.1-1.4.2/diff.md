# Comparing `tmp/openimis-be-calcrule_unconditional_cash_payment-1.4.1.tar.gz` & `tmp/openimis-be-calcrule_unconditional_cash_payment-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis-be-calcrule_unconditional_cash_payment-1.4.1.tar", last modified: Fri Nov 11 08:12:50 2022, max compression
+gzip compressed data, was "openimis-be-calcrule_unconditional_cash_payment-1.4.2.tar", last modified: Tue May 16 21:53:00 2023, max compression
```

## Comparing `openimis-be-calcrule_unconditional_cash_payment-1.4.1.tar` & `openimis-be-calcrule_unconditional_cash_payment-1.4.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:50.895860 openimis-be-calcrule_unconditional_cash_payment-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1854 2022-11-11 08:12:34.000000 openimis-be-calcrule_unconditional_cash_payment-1.4.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)      809 2022-11-11 08:12:50.895860 openimis-be-calcrule_unconditional_cash_payment-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-11-11 08:12:34.000000 openimis-be-calcrule_unconditional_cash_payment-1.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:50.895860 openimis-be-calcrule_unconditional_cash_payment-1.4.1/calcrule_unconditional_cash_payment/
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-11-11 08:12:34.000000 openimis-be-calcrule_unconditional_cash_payment-1.4.1/calcrule_unconditional_cash_payment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-11-11 08:12:34.000000 openimis-be-calcrule_unconditional_cash_payment-1.4.1/calcrule_unconditional_cash_payment/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)      879 2022-11-11 08:12:34.000000 openimis-be-calcrule_unconditional_cash_payment-1.4.1/calcrule_unconditional_cash_payment/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)     7311 2022-11-11 08:12:34.000000 openimis-be-calcrule_unconditional_cash_payment-1.4.1/calcrule_unconditional_cash_payment/calculation_rule.py
--rw-r--r--   0 runner    (1001) docker     (121)     1664 2022-11-11 08:12:34.000000 openimis-be-calcrule_unconditional_cash_payment-1.4.1/calcrule_unconditional_cash_payment/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:50.895860 openimis-be-calcrule_unconditional_cash_payment-1.4.1/calcrule_unconditional_cash_payment/converters/
--rw-r--r--   0 runner    (1001) docker     (121)      201 2022-11-11 08:12:34.000000 openimis-be-calcrule_unconditional_cash_payment-1.4.1/calcrule_unconditional_cash_payment/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2078 2022-11-11 08:12:34.000000 openimis-be-calcrule_unconditional_cash_payment-1.4.1/calcrule_unconditional_cash_payment/converters/policy_to_bill.py
--rw-r--r--   0 runner    (1001) docker     (121)     1313 2022-11-11 08:12:34.000000 openimis-be-calcrule_unconditional_cash_payment-1.4.1/calcrule_unconditional_cash_payment/converters/policy_to_bill_item.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:50.895860 openimis-be-calcrule_unconditional_cash_payment-1.4.1/calcrule_unconditional_cash_payment/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:34.000000 openimis-be-calcrule_unconditional_cash_payment-1.4.1/calcrule_unconditional_cash_payment/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-11-11 08:12:34.000000 openimis-be-calcrule_unconditional_cash_payment-1.4.1/calcrule_unconditional_cash_payment/models.py
--rw-r--r--   0 runner    (1001) docker     (121)      936 2022-11-11 08:12:34.000000 openimis-be-calcrule_unconditional_cash_payment-1.4.1/calcrule_unconditional_cash_payment/signals.py
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-11-11 08:12:34.000000 openimis-be-calcrule_unconditional_cash_payment-1.4.1/calcrule_unconditional_cash_payment/tests.py
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-11-11 08:12:34.000000 openimis-be-calcrule_unconditional_cash_payment-1.4.1/calcrule_unconditional_cash_payment/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-11-11 08:12:34.000000 openimis-be-calcrule_unconditional_cash_payment-1.4.1/calcrule_unconditional_cash_payment/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:50.895860 openimis-be-calcrule_unconditional_cash_payment-1.4.1/openimis_be_calcrule_unconditional_cash_payment.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      809 2022-11-11 08:12:50.000000 openimis-be-calcrule_unconditional_cash_payment-1.4.1/openimis_be_calcrule_unconditional_cash_payment.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-11-11 08:12:50.000000 openimis-be-calcrule_unconditional_cash_payment-1.4.1/openimis_be_calcrule_unconditional_cash_payment.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-11 08:12:50.000000 openimis-be-calcrule_unconditional_cash_payment-1.4.1/openimis_be_calcrule_unconditional_cash_payment.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-11-11 08:12:50.000000 openimis-be-calcrule_unconditional_cash_payment-1.4.1/openimis_be_calcrule_unconditional_cash_payment.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-11-11 08:12:50.000000 openimis-be-calcrule_unconditional_cash_payment-1.4.1/openimis_be_calcrule_unconditional_cash_payment.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-11 08:12:50.895860 openimis-be-calcrule_unconditional_cash_payment-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1270 2022-11-11 08:12:49.000000 openimis-be-calcrule_unconditional_cash_payment-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:53:00.355969 openimis-be-calcrule_unconditional_cash_payment-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-16 21:52:43.000000 openimis-be-calcrule_unconditional_cash_payment-1.4.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-16 21:53:00.355969 openimis-be-calcrule_unconditional_cash_payment-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-16 21:52:43.000000 openimis-be-calcrule_unconditional_cash_payment-1.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:53:00.355969 openimis-be-calcrule_unconditional_cash_payment-1.4.2/calcrule_unconditional_cash_payment/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-16 21:52:43.000000 openimis-be-calcrule_unconditional_cash_payment-1.4.2/calcrule_unconditional_cash_payment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-16 21:52:43.000000 openimis-be-calcrule_unconditional_cash_payment-1.4.2/calcrule_unconditional_cash_payment/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-16 21:52:43.000000 openimis-be-calcrule_unconditional_cash_payment-1.4.2/calcrule_unconditional_cash_payment/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-05-16 21:52:43.000000 openimis-be-calcrule_unconditional_cash_payment-1.4.2/calcrule_unconditional_cash_payment/calculation_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-16 21:52:43.000000 openimis-be-calcrule_unconditional_cash_payment-1.4.2/calcrule_unconditional_cash_payment/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:53:00.355969 openimis-be-calcrule_unconditional_cash_payment-1.4.2/calcrule_unconditional_cash_payment/converters/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-16 21:52:43.000000 openimis-be-calcrule_unconditional_cash_payment-1.4.2/calcrule_unconditional_cash_payment/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-05-16 21:52:43.000000 openimis-be-calcrule_unconditional_cash_payment-1.4.2/calcrule_unconditional_cash_payment/converters/policy_to_bill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-16 21:52:43.000000 openimis-be-calcrule_unconditional_cash_payment-1.4.2/calcrule_unconditional_cash_payment/converters/policy_to_bill_item.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:53:00.355969 openimis-be-calcrule_unconditional_cash_payment-1.4.2/calcrule_unconditional_cash_payment/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:52:43.000000 openimis-be-calcrule_unconditional_cash_payment-1.4.2/calcrule_unconditional_cash_payment/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-16 21:52:43.000000 openimis-be-calcrule_unconditional_cash_payment-1.4.2/calcrule_unconditional_cash_payment/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-16 21:52:43.000000 openimis-be-calcrule_unconditional_cash_payment-1.4.2/calcrule_unconditional_cash_payment/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-16 21:52:43.000000 openimis-be-calcrule_unconditional_cash_payment-1.4.2/calcrule_unconditional_cash_payment/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 21:52:43.000000 openimis-be-calcrule_unconditional_cash_payment-1.4.2/calcrule_unconditional_cash_payment/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-16 21:52:43.000000 openimis-be-calcrule_unconditional_cash_payment-1.4.2/calcrule_unconditional_cash_payment/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:53:00.355969 openimis-be-calcrule_unconditional_cash_payment-1.4.2/openimis_be_calcrule_unconditional_cash_payment.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-16 21:53:00.000000 openimis-be-calcrule_unconditional_cash_payment-1.4.2/openimis_be_calcrule_unconditional_cash_payment.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-16 21:53:00.000000 openimis-be-calcrule_unconditional_cash_payment-1.4.2/openimis_be_calcrule_unconditional_cash_payment.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 21:53:00.000000 openimis-be-calcrule_unconditional_cash_payment-1.4.2/openimis_be_calcrule_unconditional_cash_payment.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-16 21:53:00.000000 openimis-be-calcrule_unconditional_cash_payment-1.4.2/openimis_be_calcrule_unconditional_cash_payment.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-16 21:53:00.000000 openimis-be-calcrule_unconditional_cash_payment-1.4.2/openimis_be_calcrule_unconditional_cash_payment.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 21:53:00.355969 openimis-be-calcrule_unconditional_cash_payment-1.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-16 21:52:58.000000 openimis-be-calcrule_unconditional_cash_payment-1.4.2/setup.py
```

### Comparing `openimis-be-calcrule_unconditional_cash_payment-1.4.1/LICENSE.md` & `openimis-be-calcrule_unconditional_cash_payment-1.4.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule_unconditional_cash_payment-1.4.1/PKG-INFO` & `openimis-be-calcrule_unconditional_cash_payment-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-calcrule_unconditional_cash_payment
-Version: 1.4.1
+Version: 1.4.2
 Summary: The openIMIS Backend calcrule_unconditional_cash_payment reference module.
 Home-page: https://openimis.org/
 Author: Wojciech Zgliniecki
 Author-email: wzgliniecki@soldevelo.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-calcrule_unconditional_cash_payment-1.4.1/calcrule_unconditional_cash_payment/apps.py` & `openimis-be-calcrule_unconditional_cash_payment-1.4.2/calcrule_unconditional_cash_payment/apps.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule_unconditional_cash_payment-1.4.1/calcrule_unconditional_cash_payment/calculation_rule.py` & `openimis-be-calcrule_unconditional_cash_payment-1.4.2/calcrule_unconditional_cash_payment/calculation_rule.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule_unconditional_cash_payment-1.4.1/calcrule_unconditional_cash_payment/config.py` & `openimis-be-calcrule_unconditional_cash_payment-1.4.2/calcrule_unconditional_cash_payment/config.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule_unconditional_cash_payment-1.4.1/calcrule_unconditional_cash_payment/converters/policy_to_bill.py` & `openimis-be-calcrule_unconditional_cash_payment-1.4.2/calcrule_unconditional_cash_payment/converters/policy_to_bill.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule_unconditional_cash_payment-1.4.1/calcrule_unconditional_cash_payment/converters/policy_to_bill_item.py` & `openimis-be-calcrule_unconditional_cash_payment-1.4.2/calcrule_unconditional_cash_payment/converters/policy_to_bill_item.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule_unconditional_cash_payment-1.4.1/calcrule_unconditional_cash_payment/signals.py` & `openimis-be-calcrule_unconditional_cash_payment-1.4.2/calcrule_unconditional_cash_payment/signals.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule_unconditional_cash_payment-1.4.1/openimis_be_calcrule_unconditional_cash_payment.egg-info/PKG-INFO` & `openimis-be-calcrule_unconditional_cash_payment-1.4.2/openimis_be_calcrule_unconditional_cash_payment.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-calcrule-unconditional-cash-payment
-Version: 1.4.1
+Version: 1.4.2
 Summary: The openIMIS Backend calcrule_unconditional_cash_payment reference module.
 Home-page: https://openimis.org/
 Author: Wojciech Zgliniecki
 Author-email: wzgliniecki@soldevelo.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-calcrule_unconditional_cash_payment-1.4.1/openimis_be_calcrule_unconditional_cash_payment.egg-info/SOURCES.txt` & `openimis-be-calcrule_unconditional_cash_payment-1.4.2/openimis_be_calcrule_unconditional_cash_payment.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule_unconditional_cash_payment-1.4.1/setup.py` & `openimis-be-calcrule_unconditional_cash_payment-1.4.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='openimis-be-calcrule_unconditional_cash_payment',
-    version='1.4.1',
+    version='v1.4.2',
     packages=find_packages(),
     include_package_data=True,
     license='GNU AGPL v3',
     description='The openIMIS Backend calcrule_unconditional_cash_payment reference module.',
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://openimis.org/',
```

