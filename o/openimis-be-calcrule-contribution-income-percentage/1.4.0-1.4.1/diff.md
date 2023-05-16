# Comparing `tmp/openimis-be-calcrule_contribution_income_percentage-1.4.0.tar.gz` & `tmp/openimis-be-calcrule_contribution_income_percentage-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis-be-calcrule_contribution_income_percentage-1.4.0.tar", last modified: Mon May  9 15:44:30 2022, max compression
+gzip compressed data, was "openimis-be-calcrule_contribution_income_percentage-1.4.1.tar", last modified: Tue May 16 21:46:58 2023, max compression
```

## Comparing `openimis-be-calcrule_contribution_income_percentage-1.4.0.tar` & `openimis-be-calcrule_contribution_income_percentage-1.4.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 15:44:30.730153 openimis-be-calcrule_contribution_income_percentage-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (121)    34523 2022-05-09 15:44:20.000000 openimis-be-calcrule_contribution_income_percentage-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1885 2022-05-09 15:44:30.730153 openimis-be-calcrule_contribution_income_percentage-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1074 2022-05-09 15:44:20.000000 openimis-be-calcrule_contribution_income_percentage-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 15:44:30.730153 openimis-be-calcrule_contribution_income_percentage-1.4.0/calcrule_contribution_income_percentage/
--rw-r--r--   0 runner    (1001) docker     (121)      107 2022-05-09 15:44:20.000000 openimis-be-calcrule_contribution_income_percentage-1.4.0/calcrule_contribution_income_percentage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-05-09 15:44:20.000000 openimis-be-calcrule_contribution_income_percentage-1.4.0/calcrule_contribution_income_percentage/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)      885 2022-05-09 15:44:20.000000 openimis-be-calcrule_contribution_income_percentage-1.4.0/calcrule_contribution_income_percentage/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)     6816 2022-05-09 15:44:20.000000 openimis-be-calcrule_contribution_income_percentage-1.4.0/calcrule_contribution_income_percentage/calculation_rule.py
--rw-r--r--   0 runner    (1001) docker     (121)     3529 2022-05-09 15:44:20.000000 openimis-be-calcrule_contribution_income_percentage-1.4.0/calcrule_contribution_income_percentage/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 15:44:30.730153 openimis-be-calcrule_contribution_income_percentage-1.4.0/calcrule_contribution_income_percentage/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-09 15:44:20.000000 openimis-be-calcrule_contribution_income_percentage-1.4.0/calcrule_contribution_income_percentage/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-09 15:44:20.000000 openimis-be-calcrule_contribution_income_percentage-1.4.0/calcrule_contribution_income_percentage/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 15:44:30.730153 openimis-be-calcrule_contribution_income_percentage-1.4.0/calcrule_contribution_income_percentage/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-05-09 15:44:20.000000 openimis-be-calcrule_contribution_income_percentage-1.4.0/calcrule_contribution_income_percentage/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-09 15:44:20.000000 openimis-be-calcrule_contribution_income_percentage-1.4.0/calcrule_contribution_income_percentage/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-09 15:44:20.000000 openimis-be-calcrule_contribution_income_percentage-1.4.0/calcrule_contribution_income_percentage/tests/helpers_tests.py
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-05-09 15:44:20.000000 openimis-be-calcrule_contribution_income_percentage-1.4.0/calcrule_contribution_income_percentage/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-05-09 15:44:20.000000 openimis-be-calcrule_contribution_income_percentage-1.4.0/calcrule_contribution_income_percentage/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 15:44:30.730153 openimis-be-calcrule_contribution_income_percentage-1.4.0/openimis_be_calcrule_contribution_income_percentage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1885 2022-05-09 15:44:30.000000 openimis-be-calcrule_contribution_income_percentage-1.4.0/openimis_be_calcrule_contribution_income_percentage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1047 2022-05-09 15:44:30.000000 openimis-be-calcrule_contribution_income_percentage-1.4.0/openimis_be_calcrule_contribution_income_percentage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-09 15:44:30.000000 openimis-be-calcrule_contribution_income_percentage-1.4.0/openimis_be_calcrule_contribution_income_percentage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      141 2022-05-09 15:44:30.000000 openimis-be-calcrule_contribution_income_percentage-1.4.0/openimis_be_calcrule_contribution_income_percentage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-05-09 15:44:30.000000 openimis-be-calcrule_contribution_income_percentage-1.4.0/openimis_be_calcrule_contribution_income_percentage.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-09 15:44:30.730153 openimis-be-calcrule_contribution_income_percentage-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1441 2022-05-09 15:44:29.000000 openimis-be-calcrule_contribution_income_percentage-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:46:58.483996 openimis-be-calcrule_contribution_income_percentage-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-16 21:46:41.000000 openimis-be-calcrule_contribution_income_percentage-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-16 21:46:58.479995 openimis-be-calcrule_contribution_income_percentage-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-16 21:46:41.000000 openimis-be-calcrule_contribution_income_percentage-1.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:46:58.479995 openimis-be-calcrule_contribution_income_percentage-1.4.1/calcrule_contribution_income_percentage/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-16 21:46:41.000000 openimis-be-calcrule_contribution_income_percentage-1.4.1/calcrule_contribution_income_percentage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-16 21:46:41.000000 openimis-be-calcrule_contribution_income_percentage-1.4.1/calcrule_contribution_income_percentage/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-16 21:46:41.000000 openimis-be-calcrule_contribution_income_percentage-1.4.1/calcrule_contribution_income_percentage/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6816 2023-05-16 21:46:41.000000 openimis-be-calcrule_contribution_income_percentage-1.4.1/calcrule_contribution_income_percentage/calculation_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-05-16 21:46:41.000000 openimis-be-calcrule_contribution_income_percentage-1.4.1/calcrule_contribution_income_percentage/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:46:58.479995 openimis-be-calcrule_contribution_income_percentage-1.4.1/calcrule_contribution_income_percentage/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:46:41.000000 openimis-be-calcrule_contribution_income_percentage-1.4.1/calcrule_contribution_income_percentage/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:46:41.000000 openimis-be-calcrule_contribution_income_percentage-1.4.1/calcrule_contribution_income_percentage/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:46:58.479995 openimis-be-calcrule_contribution_income_percentage-1.4.1/calcrule_contribution_income_percentage/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-16 21:46:41.000000 openimis-be-calcrule_contribution_income_percentage-1.4.1/calcrule_contribution_income_percentage/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:46:41.000000 openimis-be-calcrule_contribution_income_percentage-1.4.1/calcrule_contribution_income_percentage/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:46:41.000000 openimis-be-calcrule_contribution_income_percentage-1.4.1/calcrule_contribution_income_percentage/tests/helpers_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-16 21:46:41.000000 openimis-be-calcrule_contribution_income_percentage-1.4.1/calcrule_contribution_income_percentage/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-16 21:46:41.000000 openimis-be-calcrule_contribution_income_percentage-1.4.1/calcrule_contribution_income_percentage/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:46:58.479995 openimis-be-calcrule_contribution_income_percentage-1.4.1/openimis_be_calcrule_contribution_income_percentage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-16 21:46:58.000000 openimis-be-calcrule_contribution_income_percentage-1.4.1/openimis_be_calcrule_contribution_income_percentage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-16 21:46:58.000000 openimis-be-calcrule_contribution_income_percentage-1.4.1/openimis_be_calcrule_contribution_income_percentage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 21:46:58.000000 openimis-be-calcrule_contribution_income_percentage-1.4.1/openimis_be_calcrule_contribution_income_percentage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-16 21:46:58.000000 openimis-be-calcrule_contribution_income_percentage-1.4.1/openimis_be_calcrule_contribution_income_percentage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-16 21:46:58.000000 openimis-be-calcrule_contribution_income_percentage-1.4.1/openimis_be_calcrule_contribution_income_percentage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 21:46:58.483996 openimis-be-calcrule_contribution_income_percentage-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-16 21:46:56.000000 openimis-be-calcrule_contribution_income_percentage-1.4.1/setup.py
```

### Comparing `openimis-be-calcrule_contribution_income_percentage-1.4.0/LICENSE` & `openimis-be-calcrule_contribution_income_percentage-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule_contribution_income_percentage-1.4.0/PKG-INFO` & `openimis-be-calcrule_contribution_income_percentage-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: openimis-be-calcrule_contribution_income_percentage
-Version: 1.4.0
+Version: 1.4.1
 Summary: The openIMIS Backend calculation rule fs income percentage reference module.
 Home-page: https://openimis.org/
 Author: Seweryn Niedzielski
 Author-email: sniedzielski@soldevelo.com
 License: GNU AGPL v3
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.1
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -40,9 +39,7 @@
   None
 
 ## Services
   None
 
 ## Configuration options (can be changed via core.ModuleConfiguration)
   loading implemented rules from "calculation_rule.py" into global variable "CALCULATION_RULE"
-
-
```

### Comparing `openimis-be-calcrule_contribution_income_percentage-1.4.0/README.md` & `openimis-be-calcrule_contribution_income_percentage-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule_contribution_income_percentage-1.4.0/calcrule_contribution_income_percentage/apps.py` & `openimis-be-calcrule_contribution_income_percentage-1.4.1/calcrule_contribution_income_percentage/apps.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule_contribution_income_percentage-1.4.0/calcrule_contribution_income_percentage/calculation_rule.py` & `openimis-be-calcrule_contribution_income_percentage-1.4.1/calcrule_contribution_income_percentage/calculation_rule.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule_contribution_income_percentage-1.4.0/calcrule_contribution_income_percentage/config.py` & `openimis-be-calcrule_contribution_income_percentage-1.4.1/calcrule_contribution_income_percentage/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,16 +11,14 @@
                 },
                 "rights": {
                     "read": "151201",
                     "write": "151202",
                     "update": "151203",
                     "replace": "151206",
                 },
-                'relevance': "True",
-                'condition': "INPUT>1",
                 'optionSet': [
                     {
                         "value": "5",
                         "label": {
                             "en": "5%",
                             "fr": "5%"
                         }
@@ -36,32 +34,18 @@
                         "value": "15",
                         "label": {
                             "en": "15%",
                             "fr": "15%"
                         }
                     },
                 ],
+                'relevance': "True",
+                'condition': "INPUT>1",
                 "default": "5"
             },
-            {
-                "type": "checkbox",
-                "name": "includeFamilly",
-                "label": {
-                    "en": "include family members",
-                    "fr": "Inclure les membres de la familles"
-                },
-                "rights": {
-                    "read": "151201",
-                    "write": "151202",
-                    "update": "151203",
-                    "replace": "151206",
-                },
-                "relevance": "True",
-                "default": "False"
-            },
         ],
     },
     {
         "class": "ContractDetails",
         "parameters": [
             {
                 "type": "number",
@@ -103,13 +87,13 @@
                 "default": ""
             }
         ],
     },
 ]
 
 DESCRIPTION_CONTRIBUTION_VALUATION = F"" \
-    F"This calcutation will add the income in the contract details " \
-    F"and PHinsuree and the percentage in the Contribution plan" \
-    F" so when a contract valuation is requested then the calculation will" \
-    F" determine the value based on the contract details income and CP percentage"
+                                     F"This calcutation will add the income in the contract details " \
+                                     F"and PHinsuree and the percentage in the Contribution plan" \
+                                     F" so when a contract valuation is requested then the calculation will" \
+                                     F" determine the value based on the contract details income and CP percentage"
 
 FROM_TO = []
```

### Comparing `openimis-be-calcrule_contribution_income_percentage-1.4.0/openimis_be_calcrule_contribution_income_percentage.egg-info/PKG-INFO` & `openimis-be-calcrule_contribution_income_percentage-1.4.1/openimis_be_calcrule_contribution_income_percentage.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: openimis-be-calcrule-contribution-income-percentage
-Version: 1.4.0
+Version: 1.4.1
 Summary: The openIMIS Backend calculation rule fs income percentage reference module.
 Home-page: https://openimis.org/
 Author: Seweryn Niedzielski
 Author-email: sniedzielski@soldevelo.com
 License: GNU AGPL v3
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.1
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -40,9 +39,7 @@
   None
 
 ## Services
   None
 
 ## Configuration options (can be changed via core.ModuleConfiguration)
   loading implemented rules from "calculation_rule.py" into global variable "CALCULATION_RULE"
-
-
```

### Comparing `openimis-be-calcrule_contribution_income_percentage-1.4.0/openimis_be_calcrule_contribution_income_percentage.egg-info/SOURCES.txt` & `openimis-be-calcrule_contribution_income_percentage-1.4.1/openimis_be_calcrule_contribution_income_percentage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule_contribution_income_percentage-1.4.0/setup.py` & `openimis-be-calcrule_contribution_income_percentage-1.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='openimis-be-calcrule_contribution_income_percentage',
-    version='v1.4.0',
+    version='v1.4.1',
     packages=find_packages(),
     include_package_data=True,
     license='GNU AGPL v3',
     description='The openIMIS Backend calculation rule fs income percentage reference module.',
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://openimis.org/',
```

