# Comparing `tmp/openimis-be-calcrule_commission-1.4.2.tar.gz` & `tmp/openimis-be-calcrule_commission-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis-be-calcrule_commission-1.4.2.tar", last modified: Fri Nov 11 08:12:35 2022, max compression
+gzip compressed data, was "openimis-be-calcrule_commission-1.4.3.tar", last modified: Tue May 16 21:38:59 2023, max compression
```

## Comparing `openimis-be-calcrule_commission-1.4.2.tar` & `openimis-be-calcrule_commission-1.4.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:35.983671 openimis-be-calcrule_commission-1.4.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1854 2022-11-11 08:12:22.000000 openimis-be-calcrule_commission-1.4.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)     1437 2022-11-11 08:12:35.983671 openimis-be-calcrule_commission-1.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      674 2022-11-11 08:12:22.000000 openimis-be-calcrule_commission-1.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:35.983671 openimis-be-calcrule_commission-1.4.2/calcrule_commission/
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-11-11 08:12:22.000000 openimis-be-calcrule_commission-1.4.2/calcrule_commission/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-11-11 08:12:22.000000 openimis-be-calcrule_commission-1.4.2/calcrule_commission/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)      834 2022-11-11 08:12:22.000000 openimis-be-calcrule_commission-1.4.2/calcrule_commission/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)    10043 2022-11-11 08:12:22.000000 openimis-be-calcrule_commission-1.4.2/calcrule_commission/calculation_rule.py
--rw-r--r--   0 runner    (1001) docker     (121)     1056 2022-11-11 08:12:22.000000 openimis-be-calcrule_commission-1.4.2/calcrule_commission/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:35.983671 openimis-be-calcrule_commission-1.4.2/calcrule_commission/converters/
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-11-11 08:12:22.000000 openimis-be-calcrule_commission-1.4.2/calcrule_commission/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2967 2022-11-11 08:12:22.000000 openimis-be-calcrule_commission-1.4.2/calcrule_commission/converters/batch_run_to_bill.py
--rw-r--r--   0 runner    (1001) docker     (121)     2916 2022-11-11 08:12:22.000000 openimis-be-calcrule_commission-1.4.2/calcrule_commission/converters/premium_to_bill_item.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:35.983671 openimis-be-calcrule_commission-1.4.2/calcrule_commission/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:22.000000 openimis-be-calcrule_commission-1.4.2/calcrule_commission/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-11-11 08:12:22.000000 openimis-be-calcrule_commission-1.4.2/calcrule_commission/models.py
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-11-11 08:12:22.000000 openimis-be-calcrule_commission-1.4.2/calcrule_commission/tests.py
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-11-11 08:12:22.000000 openimis-be-calcrule_commission-1.4.2/calcrule_commission/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-11-11 08:12:22.000000 openimis-be-calcrule_commission-1.4.2/calcrule_commission/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:12:35.983671 openimis-be-calcrule_commission-1.4.2/openimis_be_calcrule_commission.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1437 2022-11-11 08:12:35.000000 openimis-be-calcrule_commission-1.4.2/openimis_be_calcrule_commission.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      771 2022-11-11 08:12:35.000000 openimis-be-calcrule_commission-1.4.2/openimis_be_calcrule_commission.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-11 08:12:35.000000 openimis-be-calcrule_commission-1.4.2/openimis_be_calcrule_commission.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-11-11 08:12:35.000000 openimis-be-calcrule_commission-1.4.2/openimis_be_calcrule_commission.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-11-11 08:12:35.000000 openimis-be-calcrule_commission-1.4.2/openimis_be_calcrule_commission.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-11 08:12:35.983671 openimis-be-calcrule_commission-1.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1331 2022-11-11 08:12:34.000000 openimis-be-calcrule_commission-1.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:59.669758 openimis-be-calcrule_commission-1.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-16 21:38:47.000000 openimis-be-calcrule_commission-1.4.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-16 21:38:59.669758 openimis-be-calcrule_commission-1.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-16 21:38:47.000000 openimis-be-calcrule_commission-1.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:59.669758 openimis-be-calcrule_commission-1.4.3/calcrule_commission/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-16 21:38:47.000000 openimis-be-calcrule_commission-1.4.3/calcrule_commission/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-16 21:38:47.000000 openimis-be-calcrule_commission-1.4.3/calcrule_commission/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-16 21:38:47.000000 openimis-be-calcrule_commission-1.4.3/calcrule_commission/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10043 2023-05-16 21:38:47.000000 openimis-be-calcrule_commission-1.4.3/calcrule_commission/calculation_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-16 21:38:47.000000 openimis-be-calcrule_commission-1.4.3/calcrule_commission/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:59.669758 openimis-be-calcrule_commission-1.4.3/calcrule_commission/converters/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-16 21:38:47.000000 openimis-be-calcrule_commission-1.4.3/calcrule_commission/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-05-16 21:38:47.000000 openimis-be-calcrule_commission-1.4.3/calcrule_commission/converters/batch_run_to_bill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-05-16 21:38:47.000000 openimis-be-calcrule_commission-1.4.3/calcrule_commission/converters/premium_to_bill_item.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:59.669758 openimis-be-calcrule_commission-1.4.3/calcrule_commission/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:47.000000 openimis-be-calcrule_commission-1.4.3/calcrule_commission/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-16 21:38:47.000000 openimis-be-calcrule_commission-1.4.3/calcrule_commission/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-16 21:38:47.000000 openimis-be-calcrule_commission-1.4.3/calcrule_commission/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 21:38:47.000000 openimis-be-calcrule_commission-1.4.3/calcrule_commission/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-16 21:38:47.000000 openimis-be-calcrule_commission-1.4.3/calcrule_commission/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:59.669758 openimis-be-calcrule_commission-1.4.3/openimis_be_calcrule_commission.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-16 21:38:59.000000 openimis-be-calcrule_commission-1.4.3/openimis_be_calcrule_commission.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-16 21:38:59.000000 openimis-be-calcrule_commission-1.4.3/openimis_be_calcrule_commission.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 21:38:59.000000 openimis-be-calcrule_commission-1.4.3/openimis_be_calcrule_commission.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-16 21:38:59.000000 openimis-be-calcrule_commission-1.4.3/openimis_be_calcrule_commission.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-16 21:38:59.000000 openimis-be-calcrule_commission-1.4.3/openimis_be_calcrule_commission.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 21:38:59.669758 openimis-be-calcrule_commission-1.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-16 21:38:57.000000 openimis-be-calcrule_commission-1.4.3/setup.py
```

### Comparing `openimis-be-calcrule_commission-1.4.2/LICENSE.md` & `openimis-be-calcrule_commission-1.4.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule_commission-1.4.2/calcrule_commission/apps.py` & `openimis-be-calcrule_commission-1.4.3/calcrule_commission/apps.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule_commission-1.4.2/calcrule_commission/calculation_rule.py` & `openimis-be-calcrule_commission-1.4.3/calcrule_commission/calculation_rule.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule_commission-1.4.2/calcrule_commission/config.py` & `openimis-be-calcrule_commission-1.4.3/calcrule_commission/config.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule_commission-1.4.2/calcrule_commission/converters/batch_run_to_bill.py` & `openimis-be-calcrule_commission-1.4.3/calcrule_commission/converters/batch_run_to_bill.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule_commission-1.4.2/calcrule_commission/converters/premium_to_bill_item.py` & `openimis-be-calcrule_commission-1.4.3/calcrule_commission/converters/premium_to_bill_item.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule_commission-1.4.2/openimis_be_calcrule_commission.egg-info/SOURCES.txt` & `openimis-be-calcrule_commission-1.4.3/openimis_be_calcrule_commission.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openimis-be-calcrule_commission-1.4.2/setup.py` & `openimis-be-calcrule_commission-1.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='openimis-be-calcrule_commission',
-    version='1.4.2',
+    version='v1.4.3',
     packages=find_packages(),
     include_package_data=True,
     license='GNU AGPL v3',
     description='The openIMIS Backend calculation rule commision reference module.',
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://openimis.org/',
```

