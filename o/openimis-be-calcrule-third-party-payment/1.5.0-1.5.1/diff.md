# Comparing `tmp/openimis-be-calcrule-third_party_payment-1.5.0.tar.gz` & `tmp/openimis-be-calcrule-third_party_payment-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis-be-calcrule-third_party_payment-1.5.0.tar", last modified: Fri Nov 11 08:12:24 2022, max compression
+gzip compressed data, was "openimis-be-calcrule-third_party_payment-1.5.1.tar", last modified: Tue May 16 21:38:53 2023, max compression
```

## Comparing `openimis-be-calcrule-third_party_payment-1.5.0.tar` & `openimis-be-calcrule-third_party_payment-1.5.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:24.211090 openimis-be-calcrule-third_party_payment-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1853 2022-11-11 08:12:12.000000 openimis-be-calcrule-third_party_payment-1.5.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)     1479 2022-11-11 08:12:24.211090 openimis-be-calcrule-third_party_payment-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      697 2022-11-11 08:12:12.000000 openimis-be-calcrule-third_party_payment-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:24.207090 openimis-be-calcrule-third_party_payment-1.5.0/calcrule_third_party_payment/
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-11-11 08:12:12.000000 openimis-be-calcrule-third_party_payment-1.5.0/calcrule_third_party_payment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-11-11 08:12:12.000000 openimis-be-calcrule-third_party_payment-1.5.0/calcrule_third_party_payment/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)      859 2022-11-11 08:12:12.000000 openimis-be-calcrule-third_party_payment-1.5.0/calcrule_third_party_payment/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)    11166 2022-11-11 08:12:12.000000 openimis-be-calcrule-third_party_payment-1.5.0/calcrule_third_party_payment/calculation_rule.py
--rw-r--r--   0 runner    (1001) docker     (121)    11175 2022-11-11 08:12:12.000000 openimis-be-calcrule-third_party_payment-1.5.0/calcrule_third_party_payment/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:24.211090 openimis-be-calcrule-third_party_payment-1.5.0/calcrule_third_party_payment/converters/
--rw-r--r--   0 runner    (1001) docker     (121)      185 2022-11-11 08:12:12.000000 openimis-be-calcrule-third_party_payment-1.5.0/calcrule_third_party_payment/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3460 2022-11-11 08:12:12.000000 openimis-be-calcrule-third_party_payment-1.5.0/calcrule_third_party_payment/converters/claim_to_bill_item.py
--rw-r--r--   0 runner    (1001) docker     (121)     2903 2022-11-11 08:12:12.000000 openimis-be-calcrule-third_party_payment-1.5.0/calcrule_third_party_payment/converters/claims_to_bill.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:24.211090 openimis-be-calcrule-third_party_payment-1.5.0/calcrule_third_party_payment/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:12.000000 openimis-be-calcrule-third_party_payment-1.5.0/calcrule_third_party_payment/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-11-11 08:12:12.000000 openimis-be-calcrule-third_party_payment-1.5.0/calcrule_third_party_payment/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     9511 2022-11-11 08:12:12.000000 openimis-be-calcrule-third_party_payment-1.5.0/calcrule_third_party_payment/tests.py
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-11-11 08:12:12.000000 openimis-be-calcrule-third_party_payment-1.5.0/calcrule_third_party_payment/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     5269 2022-11-11 08:12:12.000000 openimis-be-calcrule-third_party_payment-1.5.0/calcrule_third_party_payment/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-11-11 08:12:12.000000 openimis-be-calcrule-third_party_payment-1.5.0/calcrule_third_party_payment/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:24.211090 openimis-be-calcrule-third_party_payment-1.5.0/openimis_be_calcrule_third_party_payment.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1479 2022-11-11 08:12:24.000000 openimis-be-calcrule-third_party_payment-1.5.0/openimis_be_calcrule_third_party_payment.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      966 2022-11-11 08:12:24.000000 openimis-be-calcrule-third_party_payment-1.5.0/openimis_be_calcrule_third_party_payment.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-11 08:12:24.000000 openimis-be-calcrule-third_party_payment-1.5.0/openimis_be_calcrule_third_party_payment.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-11-11 08:12:24.000000 openimis-be-calcrule-third_party_payment-1.5.0/openimis_be_calcrule_third_party_payment.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-11-11 08:12:24.000000 openimis-be-calcrule-third_party_payment-1.5.0/openimis_be_calcrule_third_party_payment.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-11 08:12:24.211090 openimis-be-calcrule-third_party_payment-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1350 2022-11-11 08:12:23.000000 openimis-be-calcrule-third_party_payment-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:53.040685 openimis-be-calcrule-third_party_payment-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-16 21:38:42.000000 openimis-be-calcrule-third_party_payment-1.5.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-16 21:38:53.040685 openimis-be-calcrule-third_party_payment-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-16 21:38:42.000000 openimis-be-calcrule-third_party_payment-1.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:53.036685 openimis-be-calcrule-third_party_payment-1.5.1/calcrule_third_party_payment/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-16 21:38:42.000000 openimis-be-calcrule-third_party_payment-1.5.1/calcrule_third_party_payment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-16 21:38:42.000000 openimis-be-calcrule-third_party_payment-1.5.1/calcrule_third_party_payment/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-16 21:38:42.000000 openimis-be-calcrule-third_party_payment-1.5.1/calcrule_third_party_payment/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11166 2023-05-16 21:38:42.000000 openimis-be-calcrule-third_party_payment-1.5.1/calcrule_third_party_payment/calculation_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11463 2023-05-16 21:38:42.000000 openimis-be-calcrule-third_party_payment-1.5.1/calcrule_third_party_payment/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:53.036685 openimis-be-calcrule-third_party_payment-1.5.1/calcrule_third_party_payment/converters/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-16 21:38:42.000000 openimis-be-calcrule-third_party_payment-1.5.1/calcrule_third_party_payment/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-05-16 21:38:42.000000 openimis-be-calcrule-third_party_payment-1.5.1/calcrule_third_party_payment/converters/claim_to_bill_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-05-16 21:38:42.000000 openimis-be-calcrule-third_party_payment-1.5.1/calcrule_third_party_payment/converters/claims_to_bill.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:53.036685 openimis-be-calcrule-third_party_payment-1.5.1/calcrule_third_party_payment/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:42.000000 openimis-be-calcrule-third_party_payment-1.5.1/calcrule_third_party_payment/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-16 21:38:42.000000 openimis-be-calcrule-third_party_payment-1.5.1/calcrule_third_party_payment/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9511 2023-05-16 21:38:42.000000 openimis-be-calcrule-third_party_payment-1.5.1/calcrule_third_party_payment/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 21:38:42.000000 openimis-be-calcrule-third_party_payment-1.5.1/calcrule_third_party_payment/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-05-16 21:38:42.000000 openimis-be-calcrule-third_party_payment-1.5.1/calcrule_third_party_payment/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-16 21:38:42.000000 openimis-be-calcrule-third_party_payment-1.5.1/calcrule_third_party_payment/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:53.040685 openimis-be-calcrule-third_party_payment-1.5.1/openimis_be_calcrule_third_party_payment.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-16 21:38:52.000000 openimis-be-calcrule-third_party_payment-1.5.1/openimis_be_calcrule_third_party_payment.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-16 21:38:53.000000 openimis-be-calcrule-third_party_payment-1.5.1/openimis_be_calcrule_third_party_payment.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 21:38:52.000000 openimis-be-calcrule-third_party_payment-1.5.1/openimis_be_calcrule_third_party_payment.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-16 21:38:52.000000 openimis-be-calcrule-third_party_payment-1.5.1/openimis_be_calcrule_third_party_payment.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-16 21:38:52.000000 openimis-be-calcrule-third_party_payment-1.5.1/openimis_be_calcrule_third_party_payment.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 21:38:53.040685 openimis-be-calcrule-third_party_payment-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-16 21:38:52.000000 openimis-be-calcrule-third_party_payment-1.5.1/setup.py
```

### Comparing `openimis-be-calcrule-third_party_payment-1.5.0/LICENSE.md` & `openimis-be-calcrule-third_party_payment-1.5.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule-third_party_payment-1.5.0/PKG-INFO` & `openimis-be-calcrule-third_party_payment-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-calcrule-third_party_payment
-Version: 1.5.0
+Version: 1.5.1
 Summary: The openIMIS Backend calculation rule thirdparty payment reference module.
 Home-page: https://openimis.org/
 Author: Seweryn Niedzielski
 Author-email: sniedzielski@soldevelo.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-calcrule-third_party_payment-1.5.0/README.md` & `openimis-be-calcrule-third_party_payment-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule-third_party_payment-1.5.0/calcrule_third_party_payment/apps.py` & `openimis-be-calcrule-third_party_payment-1.5.1/calcrule_third_party_payment/apps.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule-third_party_payment-1.5.0/calcrule_third_party_payment/calculation_rule.py` & `openimis-be-calcrule-third_party_payment-1.5.1/calcrule_third_party_payment/calculation_rule.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule-third_party_payment-1.5.0/calcrule_third_party_payment/config.py` & `openimis-be-calcrule-third_party_payment-1.5.1/calcrule_third_party_payment/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -390,15 +390,16 @@
 				},
 				"rights": {
 					"read": "121001",
 					"write": "121002",
 					"update": "121003",
 					"replace": "121006"
 				},
-				"relevance": "MOD(1, OBJECT.periodicity) = 0"
+				"relevance": "MOD(1, OBJECT.periodicity) = 0",
+				"required": "True"
 			},
 			{
 				"type": "number",
 				"default": "0",
 				"name": "distr_2",
 				"label": {
 					"en": "distribution 2",
@@ -406,15 +407,16 @@
 				},
 				"rights": {
 					"read": "121001",
 					"write": "121002",
 					"update": "121003",
 					"replace": "121006"
 				},
-				"relevance": "MOD(2, OBJECT.periodicity) = 0"
+				"relevance": "MOD(2, OBJECT.periodicity) = 0",
+				"required": "True"
 			},
 			{
 				"type": "number",
 				"default": "0",
 				"name": "distr_3",
 				"label": {
 					"en": "distribution 3",
@@ -422,15 +424,16 @@
 				},
 				"rights": {
 					"read": "121001",
 					"write": "121002",
 					"update": "121003",
 					"replace": "121006"
 				},
-				"relevance": "MOD(3, OBJECT.periodicity) = 0"
+				"relevance": "MOD(3, OBJECT.periodicity) = 0",
+				"required": "True"
 			},
 			{
 				"type": "number",
 				"default": "0",
 				"name": "distr_4",
 				"label": {
 					"en": "distribution 4",
@@ -438,15 +441,16 @@
 				},
 				"rights": {
 					"read": "121001",
 					"write": "121002",
 					"update": "121003",
 					"replace": "121006"
 				},
-				"relevance": " MOD(4, OBJECT.periodicity) = 0"
+				"relevance": " MOD(4, OBJECT.periodicity) = 0",
+				"required": "True"
 			},
 			{
 				"type": "number",
 				"default": "0",
 				"name": "distr_5",
 				"label": {
 					"en": "distribution 5",
@@ -454,15 +458,16 @@
 				},
 				"rights": {
 					"read": "121001",
 					"write": "121002",
 					"update": "121003",
 					"replace": "121006"
 				},
-				"relevance": "MOD(5, OBJECT.periodicity) = 0"
+				"relevance": "MOD(5, OBJECT.periodicity) = 0",
+				"required": "True"
 			},
 			{
 				"type": "number",
 				"default": "0",
 				"name": "distr_6",
 				"label": {
 					"en": "distribution 6",
@@ -470,15 +475,16 @@
 				},
 				"rights": {
 					"read": "121001",
 					"write": "121002",
 					"update": "121003",
 					"replace": "121006"
 				},
-				"relevance": "MOD(6, OBJECT.periodicity) = 0"
+				"relevance": "MOD(6, OBJECT.periodicity) = 0",
+				"required": "True"
 			},
 			{
 				"type": "number",
 				"default": "0",
 				"name": "distr_7",
 				"label": {
 					"en": "distribution 7",
@@ -486,15 +492,16 @@
 				},
 				"rights": {
 					"read": "121001",
 					"write": "121002",
 					"update": "121003",
 					"replace": "121006"
 				},
-				"relevance": "MOD(7, OBJECT.periodicity) = 0"
+				"relevance": "MOD(7, OBJECT.periodicity) = 0",
+				"required": "True"
 			},
 			{
 				"type": "number",
 				"default": "0",
 				"name": "distr_8",
 				"label": {
 					"en": "distribution 8",
@@ -502,15 +509,16 @@
 				},
 				"rights": {
 					"read": "121001",
 					"write": "121002",
 					"update": "121003",
 					"replace": "121006"
 				},
-				"relevance": "MOD(8, OBJECT.periodicity) = 0"
+				"relevance": "MOD(8, OBJECT.periodicity) = 0",
+				"required": "True"
 			},
 			{
 				"type": "number",
 				"default": "0",
 				"name": "distr_9",
 				"label": {
 					"en": "distribution 9",
@@ -518,15 +526,16 @@
 				},
 				"rights": {
 					"read": "121001",
 					"write": "121002",
 					"update": "121003",
 					"replace": "121006"
 				},
-				"relevance": "MOD(9, OBJECT.periodicity) = 0"
+				"relevance": "MOD(9, OBJECT.periodicity) = 0",
+				"required": "True"
 			},
 			{
 				"type": "number",
 				"default": "0",
 				"name": "distr_10",
 				"label": {
 					"en": "distribution 10",
@@ -534,15 +543,16 @@
 				},
 				"rights": {
 					"read": "121001",
 					"write": "121002",
 					"update": "121003",
 					"replace": "121006"
 				},
-				"relevance": "MOD(10, OBJECT.periodicity) = 0"
+				"relevance": "MOD(10, OBJECT.periodicity) = 0",
+				"required": "True"
 			},
 			{
 				"type": "number",
 				"default": "0",
 				"name": "distr_11",
 				"label": {
 					"en": "distribution 11",
@@ -550,15 +560,16 @@
 				},
 				"rights": {
 					"read": "121001",
 					"write": "121002",
 					"update": "121003",
 					"replace": "121006"
 				},
-				"relevance": "MOD(11, OBJECT.periodicity) = 0"
+				"relevance": "MOD(11, OBJECT.periodicity) = 0",
+				"required": "True"
 			},
 			{
 				"type": "number",
 				"default": "0",
 				"name": "distr_12",
 				"label": {
 					"en": "distribution 12",
@@ -566,15 +577,16 @@
 				},
 				"rights": {
 					"read": "121001",
 					"write": "121002",
 					"update": "121003",
 					"replace": "121006"
 				},
-				"relevance": "MOD(12, OBJECT.periodicity) = 0"
+				"relevance": "MOD(12, OBJECT.periodicity) = 0",
+				"required": "True"
 			}
 		]
 	}
 ]
 
 
 FROM_TO = [
```

### Comparing `openimis-be-calcrule-third_party_payment-1.5.0/calcrule_third_party_payment/converters/claim_to_bill_item.py` & `openimis-be-calcrule-third_party_payment-1.5.1/calcrule_third_party_payment/converters/claim_to_bill_item.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule-third_party_payment-1.5.0/calcrule_third_party_payment/converters/claims_to_bill.py` & `openimis-be-calcrule-third_party_payment-1.5.1/calcrule_third_party_payment/converters/claims_to_bill.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule-third_party_payment-1.5.0/calcrule_third_party_payment/tests.py` & `openimis-be-calcrule-third_party_payment-1.5.1/calcrule_third_party_payment/tests.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule-third_party_payment-1.5.0/calcrule_third_party_payment/utils.py` & `openimis-be-calcrule-third_party_payment-1.5.1/calcrule_third_party_payment/utils.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule-third_party_payment-1.5.0/openimis_be_calcrule_third_party_payment.egg-info/PKG-INFO` & `openimis-be-calcrule-third_party_payment-1.5.1/openimis_be_calcrule_third_party_payment.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-calcrule-third-party-payment
-Version: 1.5.0
+Version: 1.5.1
 Summary: The openIMIS Backend calculation rule thirdparty payment reference module.
 Home-page: https://openimis.org/
 Author: Seweryn Niedzielski
 Author-email: sniedzielski@soldevelo.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-calcrule-third_party_payment-1.5.0/openimis_be_calcrule_third_party_payment.egg-info/SOURCES.txt` & `openimis-be-calcrule-third_party_payment-1.5.1/openimis_be_calcrule_third_party_payment.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule-third_party_payment-1.5.0/setup.py` & `openimis-be-calcrule-third_party_payment-1.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='openimis-be-calcrule-third_party_payment',
-    version='1.5.0',
+    version='v1.5.1',
     packages=find_packages(),
     include_package_data=True,
     license='GNU AGPL v3',
     description='The openIMIS Backend calculation rule thirdparty payment reference module.',
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://openimis.org/',
```

