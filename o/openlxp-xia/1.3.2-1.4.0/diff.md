# Comparing `tmp/openlxp-xia-1.3.2.tar.gz` & `tmp/openlxp-xia-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openlxp-xia-1.3.2.tar", last modified: Fri Jan 27 20:52:57 2023, max compression
+gzip compressed data, was "openlxp-xia-1.4.0.tar", last modified: Tue May 16 21:32:16 2023, max compression
```

## Comparing `openlxp-xia-1.3.2.tar` & `openlxp-xia-1.4.0.tar`

### file list

```diff
@@ -1,54 +1,51 @@
-drwxr-xr-x   0 kjijo      (502) staff       (20)        0 2023-01-27 20:52:57.114635 openlxp-xia-1.3.2/
--rw-r--r--   0 kjijo      (502) staff       (20)      853 2023-01-27 20:52:57.114844 openlxp-xia-1.3.2/PKG-INFO
-drwxr-xr-x   0 kjijo      (502) staff       (20)        0 2023-01-27 20:52:57.072497 openlxp-xia-1.3.2/openlxp_xia/
--rw-r--r--   0 kjijo      (502) staff       (20)        0 2023-01-27 19:40:44.000000 openlxp-xia-1.3.2/openlxp_xia/__init__.py
--rw-r--r--   0 kjijo      (502) staff       (20)     1930 2023-01-27 19:40:44.000000 openlxp-xia-1.3.2/openlxp_xia/admin.py
--rw-r--r--   0 kjijo      (502) staff       (20)      212 2023-01-27 19:40:44.000000 openlxp-xia-1.3.2/openlxp_xia/apps.py
-drwxr-xr-x   0 kjijo      (502) staff       (20)        0 2023-01-27 20:52:57.084148 openlxp-xia-1.3.2/openlxp_xia/management/
--rw-r--r--   0 kjijo      (502) staff       (20)        0 2023-01-27 19:40:44.000000 openlxp-xia-1.3.2/openlxp_xia/management/__init__.py
-drwxr-xr-x   0 kjijo      (502) staff       (20)        0 2023-01-27 20:52:57.088471 openlxp-xia-1.3.2/openlxp_xia/management/commands/
--rw-r--r--   0 kjijo      (502) staff       (20)        0 2023-01-27 19:40:44.000000 openlxp-xia-1.3.2/openlxp_xia/management/commands/__init__.py
--rw-r--r--   0 kjijo      (502) staff       (20)     4718 2023-01-27 19:40:44.000000 openlxp-xia-1.3.2/openlxp_xia/management/commands/load_supplemental_metadata.py
--rw-r--r--   0 kjijo      (502) staff       (20)     4403 2023-01-27 19:40:44.000000 openlxp-xia-1.3.2/openlxp_xia/management/commands/load_target_metadata.py
--rw-r--r--   0 kjijo      (502) staff       (20)    10217 2023-01-27 19:40:44.000000 openlxp-xia-1.3.2/openlxp_xia/management/commands/transform_source_metadata.py
--rw-r--r--   0 kjijo      (502) staff       (20)     5116 2023-01-27 19:40:44.000000 openlxp-xia-1.3.2/openlxp_xia/management/commands/validate_source_metadata.py
--rw-r--r--   0 kjijo      (502) staff       (20)     7852 2023-01-27 19:40:44.000000 openlxp-xia-1.3.2/openlxp_xia/management/commands/validate_target_metadata.py
-drwxr-xr-x   0 kjijo      (502) staff       (20)        0 2023-01-27 20:52:57.092734 openlxp-xia-1.3.2/openlxp_xia/management/utils/
--rw-r--r--   0 kjijo      (502) staff       (20)        0 2023-01-27 19:40:44.000000 openlxp-xia-1.3.2/openlxp_xia/management/utils/__init__.py
--rw-r--r--   0 kjijo      (502) staff       (20)    12792 2023-01-27 19:40:44.000000 openlxp-xia-1.3.2/openlxp_xia/management/utils/xia_internal.py
--rw-r--r--   0 kjijo      (502) staff       (20)     1658 2023-01-27 19:40:44.000000 openlxp-xia-1.3.2/openlxp_xia/management/utils/xis_client.py
--rw-r--r--   0 kjijo      (502) staff       (20)     5116 2023-01-27 19:44:06.000000 openlxp-xia-1.3.2/openlxp_xia/management/utils/xss_client.py
-drwxr-xr-x   0 kjijo      (502) staff       (20)        0 2023-01-27 20:52:57.100771 openlxp-xia-1.3.2/openlxp_xia/migrations/
--rw-r--r--   0 kjijo      (502) staff       (20)     7683 2023-01-27 19:40:44.000000 openlxp-xia-1.3.2/openlxp_xia/migrations/0001_initial.py
--rw-r--r--   0 kjijo      (502) staff       (20)     1726 2023-01-27 19:40:44.000000 openlxp-xia-1.3.2/openlxp_xia/migrations/0002_use_xss.py
--rw-r--r--   0 kjijo      (502) staff       (20)      884 2023-01-27 19:40:44.000000 openlxp-xia-1.3.2/openlxp_xia/migrations/0003_auto_20220708_1111.py
--rw-r--r--   0 kjijo      (502) staff       (20)      904 2023-01-27 20:11:56.000000 openlxp-xia-1.3.2/openlxp_xia/migrations/0004_auto_20230127_2011.py
--rw-r--r--   0 kjijo      (502) staff       (20)        0 2023-01-27 19:40:44.000000 openlxp-xia-1.3.2/openlxp_xia/migrations/__init__.py
--rw-r--r--   0 kjijo      (502) staff       (20)     7532 2023-01-27 19:40:44.000000 openlxp-xia-1.3.2/openlxp_xia/models.py
--rw-r--r--   0 kjijo      (502) staff       (20)     1677 2023-01-27 19:40:44.000000 openlxp-xia-1.3.2/openlxp_xia/signals.py
-drwxr-xr-x   0 kjijo      (502) staff       (20)        0 2023-01-27 20:52:57.108622 openlxp-xia-1.3.2/openlxp_xia/tests/
--rw-r--r--   0 kjijo      (502) staff       (20)        0 2023-01-27 19:40:44.000000 openlxp-xia-1.3.2/openlxp_xia/tests/__init__.py
--rw-r--r--   0 kjijo      (502) staff       (20)    17495 2023-01-27 19:40:44.000000 openlxp-xia-1.3.2/openlxp_xia/tests/test_setup.py
--rw-r--r--   0 kjijo      (502) staff       (20)     1002 2023-01-27 19:40:44.000000 openlxp-xia-1.3.2/openlxp_xia/tests/test_signals.py
--rw-r--r--   0 kjijo      (502) staff       (20)    27538 2023-01-27 19:40:44.000000 openlxp-xia-1.3.2/openlxp_xia/tests/test_xia_command_intergration.py
--rw-r--r--   0 kjijo      (502) staff       (20)    32523 2023-01-27 19:40:44.000000 openlxp-xia-1.3.2/openlxp_xia/tests/test_xia_command_unit.py
--rw-r--r--   0 kjijo      (502) staff       (20)     1120 2023-01-27 19:40:44.000000 openlxp-xia-1.3.2/openlxp_xia/tests/test_xia_models_integration.py
--rw-r--r--   0 kjijo      (502) staff       (20)    12116 2023-01-27 19:40:44.000000 openlxp-xia-1.3.2/openlxp_xia/tests/test_xia_models_unit.py
--rw-r--r--   0 kjijo      (502) staff       (20)      710 2023-01-27 19:40:44.000000 openlxp-xia-1.3.2/openlxp_xia/tests/test_xia_utils_integration.py
--rw-r--r--   0 kjijo      (502) staff       (20)    24691 2023-01-27 19:40:44.000000 openlxp-xia-1.3.2/openlxp_xia/tests/test_xia_utils_unit.py
--rw-r--r--   0 kjijo      (502) staff       (20)      761 2023-01-27 19:40:44.000000 openlxp-xia-1.3.2/openlxp_xia/urls.py
--rw-r--r--   0 kjijo      (502) staff       (20)        0 2023-01-27 19:40:44.000000 openlxp-xia-1.3.2/openlxp_xia/views.py
-drwxr-xr-x   0 kjijo      (502) staff       (20)        0 2023-01-27 20:52:57.083196 openlxp-xia-1.3.2/openlxp_xia.egg-info/
--rw-r--r--   0 kjijo      (502) staff       (20)      853 2023-01-27 20:52:56.000000 openlxp-xia-1.3.2/openlxp_xia.egg-info/PKG-INFO
--rw-r--r--   0 kjijo      (502) staff       (20)     1624 2023-01-27 20:52:57.000000 openlxp-xia-1.3.2/openlxp_xia.egg-info/SOURCES.txt
--rw-r--r--   0 kjijo      (502) staff       (20)        1 2023-01-27 20:52:56.000000 openlxp-xia-1.3.2/openlxp_xia.egg-info/dependency_links.txt
--rw-r--r--   0 kjijo      (502) staff       (20)       14 2023-01-27 20:52:56.000000 openlxp-xia-1.3.2/openlxp_xia.egg-info/requires.txt
--rw-r--r--   0 kjijo      (502) staff       (20)       32 2023-01-27 20:52:56.000000 openlxp-xia-1.3.2/openlxp_xia.egg-info/top_level.txt
-drwxr-xr-x   0 kjijo      (502) staff       (20)        0 2023-01-27 20:52:57.113334 openlxp-xia-1.3.2/openlxp_xia_project/
--rw-r--r--   0 kjijo      (502) staff       (20)        0 2023-01-27 19:40:44.000000 openlxp-xia-1.3.2/openlxp_xia_project/__init__.py
--rw-r--r--   0 kjijo      (502) staff       (20)      415 2023-01-27 19:40:44.000000 openlxp-xia-1.3.2/openlxp_xia_project/asgi.py
--rw-r--r--   0 kjijo      (502) staff       (20)     4618 2023-01-27 20:11:14.000000 openlxp-xia-1.3.2/openlxp_xia_project/settings.py
--rw-r--r--   0 kjijo      (502) staff       (20)      761 2023-01-27 19:40:44.000000 openlxp-xia-1.3.2/openlxp_xia_project/urls.py
--rw-r--r--   0 kjijo      (502) staff       (20)      415 2023-01-27 19:40:44.000000 openlxp-xia-1.3.2/openlxp_xia_project/wsgi.py
--rw-r--r--   0 kjijo      (502) staff       (20)      928 2023-01-27 20:52:57.117088 openlxp-xia-1.3.2/setup.cfg
--rw-r--r--   0 kjijo      (502) staff       (20)       95 2023-01-27 19:40:44.000000 openlxp-xia-1.3.2/setup.py
+drwxr-xr-x   0 jametobin   (502) staff       (20)        0 2023-05-16 21:32:16.095369 openlxp-xia-1.4.0/
+-rw-r--r--   0 jametobin   (502) staff       (20)     4930 2023-05-16 21:32:16.095522 openlxp-xia-1.4.0/PKG-INFO
+-rw-r--r--   0 jametobin   (502) staff       (20)     4064 2023-05-16 21:32:06.000000 openlxp-xia-1.4.0/README.md
+drwxr-xr-x   0 jametobin   (502) staff       (20)        0 2023-05-16 21:32:16.064772 openlxp-xia-1.4.0/openlxp_xia/
+-rw-r--r--   0 jametobin   (502) staff       (20)        0 2022-06-24 18:54:06.000000 openlxp-xia-1.4.0/openlxp_xia/__init__.py
+-rw-r--r--   0 jametobin   (502) staff       (20)     1930 2023-05-16 20:05:42.000000 openlxp-xia-1.4.0/openlxp_xia/admin.py
+-rw-r--r--   0 jametobin   (502) staff       (20)      147 2022-06-24 18:54:06.000000 openlxp-xia-1.4.0/openlxp_xia/apps.py
+drwxr-xr-x   0 jametobin   (502) staff       (20)        0 2023-05-16 21:32:16.070627 openlxp-xia-1.4.0/openlxp_xia/management/
+-rw-r--r--   0 jametobin   (502) staff       (20)        0 2022-06-24 18:54:06.000000 openlxp-xia-1.4.0/openlxp_xia/management/__init__.py
+drwxr-xr-x   0 jametobin   (502) staff       (20)        0 2023-05-16 21:32:16.078479 openlxp-xia-1.4.0/openlxp_xia/management/commands/
+-rw-r--r--   0 jametobin   (502) staff       (20)        0 2022-06-24 18:54:06.000000 openlxp-xia-1.4.0/openlxp_xia/management/commands/__init__.py
+-rw-r--r--   0 jametobin   (502) staff       (20)     4718 2022-06-24 18:54:06.000000 openlxp-xia-1.4.0/openlxp_xia/management/commands/load_supplemental_metadata.py
+-rw-r--r--   0 jametobin   (502) staff       (20)     4403 2022-06-24 18:54:06.000000 openlxp-xia-1.4.0/openlxp_xia/management/commands/load_target_metadata.py
+-rw-r--r--   0 jametobin   (502) staff       (20)    12029 2022-06-24 18:54:06.000000 openlxp-xia-1.4.0/openlxp_xia/management/commands/transform_source_metadata.py
+-rw-r--r--   0 jametobin   (502) staff       (20)     5116 2022-06-24 18:54:06.000000 openlxp-xia-1.4.0/openlxp_xia/management/commands/validate_source_metadata.py
+-rw-r--r--   0 jametobin   (502) staff       (20)     7956 2022-06-24 18:54:06.000000 openlxp-xia-1.4.0/openlxp_xia/management/commands/validate_target_metadata.py
+drwxr-xr-x   0 jametobin   (502) staff       (20)        0 2023-05-16 21:32:16.082221 openlxp-xia-1.4.0/openlxp_xia/management/utils/
+-rw-r--r--   0 jametobin   (502) staff       (20)        0 2022-06-24 18:54:06.000000 openlxp-xia-1.4.0/openlxp_xia/management/utils/__init__.py
+-rw-r--r--   0 jametobin   (502) staff       (20)     9840 2022-06-24 18:54:06.000000 openlxp-xia-1.4.0/openlxp_xia/management/utils/xia_internal.py
+-rw-r--r--   0 jametobin   (502) staff       (20)     2057 2023-05-16 20:12:32.000000 openlxp-xia-1.4.0/openlxp_xia/management/utils/xis_client.py
+-rw-r--r--   0 jametobin   (502) staff       (20)     5117 2023-05-16 20:05:42.000000 openlxp-xia-1.4.0/openlxp_xia/management/utils/xss_client.py
+drwxr-xr-x   0 jametobin   (502) staff       (20)        0 2023-05-16 21:32:16.084510 openlxp-xia-1.4.0/openlxp_xia/migrations/
+-rw-r--r--   0 jametobin   (502) staff       (20)     7683 2022-06-24 18:54:06.000000 openlxp-xia-1.4.0/openlxp_xia/migrations/0001_initial.py
+-rw-r--r--   0 jametobin   (502) staff       (20)     1726 2023-05-16 20:05:42.000000 openlxp-xia-1.4.0/openlxp_xia/migrations/0002_use_xss.py
+-rw-r--r--   0 jametobin   (502) staff       (20)        0 2022-06-24 18:54:06.000000 openlxp-xia-1.4.0/openlxp_xia/migrations/__init__.py
+-rw-r--r--   0 jametobin   (502) staff       (20)    10652 2023-05-16 20:32:25.000000 openlxp-xia-1.4.0/openlxp_xia/models.py
+drwxr-xr-x   0 jametobin   (502) staff       (20)        0 2023-05-16 21:32:16.092136 openlxp-xia-1.4.0/openlxp_xia/tests/
+-rw-r--r--   0 jametobin   (502) staff       (20)        0 2022-06-24 18:54:06.000000 openlxp-xia-1.4.0/openlxp_xia/tests/__init__.py
+-rw-r--r--   0 jametobin   (502) staff       (20)    17232 2022-06-24 18:54:06.000000 openlxp-xia-1.4.0/openlxp_xia/tests/test_setup.py
+-rw-r--r--   0 jametobin   (502) staff       (20)    27386 2022-06-24 18:54:06.000000 openlxp-xia-1.4.0/openlxp_xia/tests/test_xia_command_intergration.py
+-rw-r--r--   0 jametobin   (502) staff       (20)    33612 2022-06-24 18:54:06.000000 openlxp-xia-1.4.0/openlxp_xia/tests/test_xia_command_unit.py
+-rw-r--r--   0 jametobin   (502) staff       (20)     1120 2023-05-16 20:05:42.000000 openlxp-xia-1.4.0/openlxp_xia/tests/test_xia_models_integration.py
+-rw-r--r--   0 jametobin   (502) staff       (20)    12993 2023-05-16 20:05:42.000000 openlxp-xia-1.4.0/openlxp_xia/tests/test_xia_models_unit.py
+-rw-r--r--   0 jametobin   (502) staff       (20)      710 2022-06-24 18:54:06.000000 openlxp-xia-1.4.0/openlxp_xia/tests/test_xia_utils_integration.py
+-rw-r--r--   0 jametobin   (502) staff       (20)    22425 2023-05-16 20:05:42.000000 openlxp-xia-1.4.0/openlxp_xia/tests/test_xia_utils_unit.py
+-rw-r--r--   0 jametobin   (502) staff       (20)      761 2022-06-24 18:54:06.000000 openlxp-xia-1.4.0/openlxp_xia/urls.py
+-rw-r--r--   0 jametobin   (502) staff       (20)        0 2022-06-24 18:54:06.000000 openlxp-xia-1.4.0/openlxp_xia/views.py
+drwxr-xr-x   0 jametobin   (502) staff       (20)        0 2023-05-16 21:32:16.069893 openlxp-xia-1.4.0/openlxp_xia.egg-info/
+-rw-r--r--   0 jametobin   (502) staff       (20)     4930 2023-05-16 21:32:16.000000 openlxp-xia-1.4.0/openlxp_xia.egg-info/PKG-INFO
+-rw-r--r--   0 jametobin   (502) staff       (20)     1477 2023-05-16 21:32:16.000000 openlxp-xia-1.4.0/openlxp_xia.egg-info/SOURCES.txt
+-rw-r--r--   0 jametobin   (502) staff       (20)        1 2023-05-16 21:32:16.000000 openlxp-xia-1.4.0/openlxp_xia.egg-info/dependency_links.txt
+-rw-r--r--   0 jametobin   (502) staff       (20)       14 2023-05-16 21:32:16.000000 openlxp-xia-1.4.0/openlxp_xia.egg-info/requires.txt
+-rw-r--r--   0 jametobin   (502) staff       (20)       45 2023-05-16 21:32:16.000000 openlxp-xia-1.4.0/openlxp_xia.egg-info/top_level.txt
+drwxr-xr-x   0 jametobin   (502) staff       (20)        0 2023-05-16 21:32:16.095076 openlxp-xia-1.4.0/openlxp_xia_project/
+-rw-r--r--   0 jametobin   (502) staff       (20)        0 2022-06-24 18:54:06.000000 openlxp-xia-1.4.0/openlxp_xia_project/__init__.py
+-rw-r--r--   0 jametobin   (502) staff       (20)      415 2022-06-24 18:54:06.000000 openlxp-xia-1.4.0/openlxp_xia_project/asgi.py
+-rw-r--r--   0 jametobin   (502) staff       (20)     4540 2022-06-24 18:54:06.000000 openlxp-xia-1.4.0/openlxp_xia_project/settings.py
+-rw-r--r--   0 jametobin   (502) staff       (20)      761 2022-06-24 18:54:06.000000 openlxp-xia-1.4.0/openlxp_xia_project/urls.py
+-rw-r--r--   0 jametobin   (502) staff       (20)      415 2022-06-24 18:54:06.000000 openlxp-xia-1.4.0/openlxp_xia_project/wsgi.py
+-rw-r--r--   0 jametobin   (502) staff       (20)      974 2023-05-16 21:32:16.095987 openlxp-xia-1.4.0/setup.cfg
+-rw-r--r--   0 jametobin   (502) staff       (20)       95 2022-06-24 18:54:06.000000 openlxp-xia-1.4.0/setup.py
```

### Comparing `openlxp-xia-1.3.2/openlxp_xia/admin.py` & `openlxp-xia-1.4.0/openlxp_xia/admin.py`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.3.2/openlxp_xia/management/commands/load_supplemental_metadata.py` & `openlxp-xia-1.4.0/openlxp_xia/management/commands/load_supplemental_metadata.py`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.3.2/openlxp_xia/management/commands/load_target_metadata.py` & `openlxp-xia-1.4.0/openlxp_xia/management/commands/load_target_metadata.py`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.3.2/openlxp_xia/management/commands/transform_source_metadata.py` & `openlxp-xia-1.4.0/openlxp_xia/management/commands/transform_source_metadata.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,18 @@
-import copy
 import hashlib
 import logging
 
 import pandas as pd
 from django.core.management.base import BaseCommand
 from django.utils import timezone
 
 from openlxp_xia.management.utils.xia_internal import (
-    dict_flatten, get_target_metadata_key_value,
-    replace_field_on_target_schema, transform_to_target, traverse_dict,
-    traverse_dict_with_key_list, type_cast_overwritten_values,
-    type_check_change)
+    dict_flatten, get_target_metadata_key_value, is_date,
+    replace_field_on_target_schema, required_recommended_logs,
+    type_cast_overwritten_values)
 from openlxp_xia.management.utils.xss_client import (
     get_data_types_for_validation, get_required_fields_for_validation,
     get_source_validation_schema, get_target_metadata_for_transformation,
     get_target_validation_schema)
 from openlxp_xia.models import (MetadataFieldOverwrite, MetadataLedger,
                                 SupplementalLedger)
 
@@ -40,116 +38,143 @@
 
     for metadata_column_list in metadata_columns:
         for column in metadata_column_list:
             supplemental_metadata.pop(column, None)
     return supplemental_metadata
 
 
-def overwrite_append_metadata(metadata, column, value, overwrite_flag):
-    """Overwrite & append metadata fields based on overwrite flag """
+def get_metadata_fields_to_overwrite(metadata_df):
+    """looping through fields to be overwrite or appended"""
+    for each in MetadataFieldOverwrite.objects.all():
+        column = each.field_name
+        overwrite_flag = each.overwrite
+        # checking and converting type of overwritten values
+        value = type_cast_overwritten_values(each.field_type, each.field_value)
 
-    key_list = column.split(".")
-    # loop till last key_value in list
-    for key_value in key_list[:-1]:
-        metadata = traverse_dict(metadata, key_value)
+        metadata_df = overwrite_append_metadata(metadata_df, column, value,
+                                                overwrite_flag)
+    return metadata_df
+
+
+def overwrite_append_metadata(metadata_df, column, value, overwrite_flag):
+    """Overwrite & append metadata fields based on overwrite flag """
 
-    column = key_list[-1]
     # field should be overwritten and append
     if overwrite_flag:
-        metadata[column] = value
+        metadata_df[column] = value
     # skip field to be overwritten and append
     else:
-        if column not in metadata:
-            metadata[column] = value
+        if column not in metadata_df.columns:
+            metadata_df[column] = value
         else:
-            if metadata[column] is None or metadata[column] == "":
-                metadata[column] = value
+            metadata_df.loc[metadata_df[column].isnull(), column] = value
+            metadata_df.loc[metadata_df[column] == "", column] = value
+    return metadata_df
 
 
-def overwrite_metadata_field(metadata):
+def overwrite_metadata_field(metadata_df):
     """Overwrite & append metadata fields with admin entered values """
     # get metadata fields to be overwritten and appended and replace values
-    for each in MetadataFieldOverwrite.objects.all():
-        column = each.field_name
-        overwrite_flag = each.overwrite
-        # checking and converting type of overwritten values
-        value = type_cast_overwritten_values(each.field_type, each.field_value)
+    metadata_df = get_metadata_fields_to_overwrite(metadata_df)
+    # return source metadata as dictionary
 
-        overwrite_append_metadata(metadata, column, value,
-                                  overwrite_flag)
-    return metadata
+    source_data_dict = metadata_df.to_dict(orient='index')
+    return source_data_dict[0]
 
 
-def type_checking_target_metadata(ind, target_data_dict, expected_data_types,
-                                  element):
+def type_checking_target_metadata(ind, target_data_dict, expected_data_types):
     """Function for type checking and explicit type conversion of metadata"""
-    # for element in expected_data_types:
-    key_list = element.split(".")
-    # check_key_dict = copy.deepcopy(target_data_dict)
-    check_key_dict = target_data_dict
-    check_key_dict = traverse_dict_with_key_list(check_key_dict, key_list)
-    if check_key_dict:
-        if key_list[-1] in check_key_dict:
-            if isinstance(check_key_dict[key_list[-1]], list):
-                for index in range(len(check_key_dict)):
-                    type_check_change(ind, element, expected_data_types,
-                                      check_key_dict[key_list[-1]],
-                                      index)
-            else:
-                type_check_change(ind, element, expected_data_types,
-                                  check_key_dict, key_list[-1])
+    for index in target_data_dict:
+        for section in target_data_dict[index]:
+            for key in target_data_dict[index][section]:
+                item = section + '.' + key
+                # check if item has a expected datatype from schema
+                if item in expected_data_types:
+                    # check for datetime datatype for field in metadata
+                    if expected_data_types[item] == "datetime":
+                        if not is_date(target_data_dict[index][section][key]):
+                            # explicitly convert to string if incorrect
+                            target_data_dict[index][section][key] = str(
+                                target_data_dict[index][section][key])
+                            required_recommended_logs(ind, "datatype",
+                                                      item)
+                    # check for datatype for field in metadata(except datetime)
+                    elif (not isinstance(target_data_dict[index][section][key],
+                                         expected_data_types[item])):
+                        # explicitly convert to string if incorrect
+                        target_data_dict[index][section][key] = str(
+                            target_data_dict[index][section][key])
+                        required_recommended_logs(ind, "datatype",
+                                                  item)
+                # explicitly convert to string if datatype not present
+                else:
+                    target_data_dict[index][section][key] = str(
+                        target_data_dict[index][section][key])
+    return target_data_dict
 
 
-def create_target_metadata_dict(ind, target_mapping_replace, source_metadata,
+def create_target_metadata_dict(ind, target_mapping_dict, source_metadata,
                                 required_column_list, expected_data_types):
     """Function to replace and transform source data to target data for
     using target mapping schema"""
 
     # Create dataframe using target metadata schema
     target_schema = pd.DataFrame.from_dict(
-        target_mapping_replace,
+        target_mapping_dict,
         orient='index')
 
     # Flatten source data dictionary for replacing and transformation
     source_metadata = dict_flatten(source_metadata, required_column_list)
 
     # Updating null values with empty strings for replacing metadata
     source_metadata = {
         k: '' if not v else v for k, v in
         source_metadata.items()}
-    target_data_dict = transform_to_target(source_metadata,
-                                           target_mapping_replace)
 
     # replacing fields to be overwritten or appended
-    overwrite_metadata_field(target_data_dict)
+    metadata_df = pd.DataFrame(source_metadata, index=[0])
+    metadata = overwrite_metadata_field(metadata_df)
+
+    # Replacing metadata schema with mapped values from source metadata
+
+    target_schema_replaced = target_schema.replace(metadata)
+
+    # Dropping index value and creating json object
+    target_data = target_schema_replaced.apply(lambda x: [x.dropna()],
+                                               axis=1).to_json()
+    # Creating dataframe from json object
+    target_data_df = pd.read_json(target_data)
+
+    # transforming target dataframe to dictionary object for replacing
+    # values in target with new value
+    target_data_dict = target_data_df.to_dict(orient='index')
 
     # type checking and explicit type conversion of metadata
-    for element in expected_data_types:
-        data = copy.copy(target_data_dict)
-        type_checking_target_metadata(ind, data,
-                                      expected_data_types, element)
+    target_data_dict = type_checking_target_metadata(ind, target_data_dict,
+                                                     expected_data_types)
 
     # send values to be skipped while creating supplemental data
+
     supplemental_metadata = \
-        create_supplemental_metadata(target_schema.values.tolist(),
-                                     source_metadata)
+        create_supplemental_metadata(target_schema.values.tolist(), metadata)
 
     return target_data_dict, supplemental_metadata
 
 
 def store_transformed_source_metadata(key_value, key_value_hash,
                                       target_data_dict,
                                       hash_value, supplemental_metadata):
     """Storing target metadata in MetadataLedger"""
 
     source_extraction_date = MetadataLedger.objects.values_list(
-        "source_metadata_extraction_date", flat=True).filter(
+        "source_metadata_extraction_date", flat=True).get(
         source_metadata_key_hash=key_value_hash,
-        record_lifecycle_status='Active'
-    ).first()
+        record_lifecycle_status='Active',
+        source_metadata_transformation_date=None
+    )
 
     data_for_transformation = MetadataLedger.objects.filter(
         source_metadata_key_hash=key_value_hash,
         record_lifecycle_status='Active',
         source_metadata_transformation_date=None
     )
 
@@ -181,49 +206,52 @@
             supplemental_metadata_key=key_value,
             supplemental_metadata_key_hash=key_value_hash,
             record_lifecycle_status='Active').update(
             supplemental_metadata_extraction_date=source_extraction_date,
             supplemental_metadata_transformation_date=timezone.now())
 
 
-def transform_source_using_key(source_data_dict, target_mapping,
+def transform_source_using_key(source_data_dict, target_mapping_dict,
                                required_column_list, expected_data_types):
     """Transforming source data using target metadata schema"""
     logger.info(
         "Transforming source data using target renaming and mapping "
         "schemas and storing in json format ")
     logger.info("Identifying supplemental data and storing them ")
     len_source_metadata = len(source_data_dict)
     logger.info(
         "Overwrite & append metadata fields with admin entered values")
     for ind in range(len_source_metadata):
-        target_mapping_metadata = copy.deepcopy(target_mapping)
-        target_metadata, supplemental_metadata = \
-            create_target_metadata_dict(ind, target_mapping_metadata,
-                                        source_data_dict
-                                        [ind]
-                                        ['source_metadata'],
-                                        required_column_list,
-                                        expected_data_types
-                                        )
-        # Replacing values in field referring target schema
-        replace_field_on_target_schema(ind,
-                                       target_metadata)
-        # Key creation for target metadata
-        key = get_target_metadata_key_value(target_metadata)
-
-        hash_value = hashlib.sha512(
-            str(target_metadata).encode(
-                'utf-8')).hexdigest()
-        store_transformed_source_metadata(key['key_value'],
-                                          key[
-                                              'key_value_hash'],
-                                          target_metadata,
-                                          hash_value,
-                                          supplemental_metadata)
+        for table_column_name in source_data_dict[ind]:
+            target_data_dict, supplemental_metadata = \
+                create_target_metadata_dict(ind, target_mapping_dict,
+                                            source_data_dict
+                                            [ind]
+                                            [table_column_name],
+                                            required_column_list,
+                                            expected_data_types
+                                            )
+            # Looping through target values in dictionary
+            for ind1 in target_data_dict:
+                # Replacing values in field referring target schema
+                replace_field_on_target_schema(ind1,
+                                               target_data_dict)
+                # Key creation for target metadata
+                key = get_target_metadata_key_value(target_data_dict[ind1])
+
+                hash_value = hashlib.sha512(
+                    str(target_data_dict[ind1]).encode(
+                        'utf-8')).hexdigest()
+                store_transformed_source_metadata(key['key_value'],
+                                                  key[
+                                                      'key_value_hash'],
+                                                  target_data_dict[
+                                                      ind1],
+                                                  hash_value,
+                                                  supplemental_metadata)
 
 
 class Command(BaseCommand):
     """Django command to extract data in the Experience index Agent (XIA)"""
 
     def handle(self, *args, **options):
         """
```

### Comparing `openlxp-xia-1.3.2/openlxp_xia/management/commands/validate_source_metadata.py` & `openlxp-xia-1.4.0/openlxp_xia/management/commands/validate_source_metadata.py`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.3.2/openlxp_xia/management/commands/validate_target_metadata.py` & `openlxp-xia-1.4.0/openlxp_xia/management/commands/validate_target_metadata.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 
 from django.core.management.base import BaseCommand
 from django.utils import timezone
 
 from openlxp_xia.management.utils.xia_internal import (
-    dict_flatten, required_recommended_logs, type_check_change)
+    dict_flatten, is_date, required_recommended_logs)
 from openlxp_xia.management.utils.xss_client import (
     get_data_types_for_validation, get_required_fields_for_validation,
     get_target_validation_schema)
 from openlxp_xia.models import MetadataLedger, SupplementalLedger
 
 logger = logging.getLogger('dict_config_logger')
 
@@ -124,23 +124,24 @@
                     required_recommended_logs(ind, "Recommended", item_name)
             else:
                 required_recommended_logs(ind, "Recommended", item_name)
         # Type checking for values in metadata
         for item in flattened_source_data:
             # check if datatype has been assigned to field
             if item in expected_data_types:
-                #
-                if isinstance(flattened_source_data[item], list):
-                    for index in range(len(flattened_source_data[item])):
-                        type_check_change(ind, item, expected_data_types,
-                                          flattened_source_data[item],
-                                          index)
-                else:
-                    type_check_change(ind, item, expected_data_types,
-                                      flattened_source_data, item)
+                # type checking for datetime datatype fields
+                if expected_data_types[item] == "datetime":
+                    if not is_date(flattened_source_data[item]):
+                        required_recommended_logs(ind, "datatype",
+                                                  item)
+                # type checking for datatype fields(except datetime)
+                elif (not isinstance(flattened_source_data[item],
+                                     expected_data_types[item])):
+                    required_recommended_logs(ind, "datatype",
+                                              item)
 
         # assigning key hash value for source metadata
         key_value_hash = target_data_dict[ind]['target_metadata_key_hash']
         # Calling function to update validation status
         store_target_metadata_validation_status(target_data_dict,
                                                 key_value_hash,
                                                 validation_result,
```

### Comparing `openlxp-xia-1.3.2/openlxp_xia/management/utils/xis_client.py` & `openlxp-xia-1.4.0/openlxp_xia/management/utils/xis_client.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 
 import requests
+from requests.auth import AuthBase
 
 from openlxp_xia.models import XISConfiguration
 
 logger = logging.getLogger('dict_config_logger')
 
 
 def get_xis_metadata_api_endpoint():
@@ -28,20 +29,31 @@
 
 def posting_metadata_ledger_to_xis(renamed_data):
     """This function post data to XIS and returns the XIS response to
             XIA load_target_metadata() """
     headers = {'Content-Type': 'application/json'}
 
     xis_response = requests.post(url=get_xis_metadata_api_endpoint(),
-                                 data=renamed_data, headers=headers)
+                                 data=renamed_data, headers=headers,
+                                 auth=TokenAuth())
     return xis_response
 
 
 def posting_supplemental_metadata_to_xis(renamed_data):
     """This function post data to XIS and returns the XIS response to
             XIA load_target_metadata() """
     headers = {'Content-Type': 'application/json'}
 
     xis_response = requests.post(
         url=get_xis_supplemental_metadata_api_endpoint(), data=renamed_data,
-        headers=headers)
+        headers=headers, auth=TokenAuth())
     return xis_response
+
+
+class TokenAuth(AuthBase):
+    """Attaches HTTP Authentication Header to the given Request object."""
+
+    def __call__(self, r):
+        # modify and return the request
+        r.headers['Authenticate'] = "Token " + \
+            XISConfiguration.objects.first().xis_api_key
+        return r
```

### Comparing `openlxp-xia-1.3.2/openlxp_xia/management/utils/xss_client.py` & `openlxp-xia-1.4.0/openlxp_xia/management/utils/xss_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,33 +14,32 @@
     return conf.xss_api
 
 
 def read_json_data(source_schema_ref, target_schema_ref=None):
     """get schema from xss and ingest as dictionary values"""
     xss_host = xss_get()
     request_path = xss_host
-    if target_schema_ref is not None:
-        if target_schema_ref.startswith('xss:'):
+    if(target_schema_ref is not None):
+        if(target_schema_ref.startswith('xss:')):
             request_path += 'mappings/?targetIRI=' + target_schema_ref
         else:
             request_path += 'mappings/?targetName=' + target_schema_ref
-        if source_schema_ref.startswith('xss:'):
+        if(source_schema_ref.startswith('xss:')):
             request_path += '&sourceIRI=' + source_schema_ref
         else:
             request_path += '&sourceName=' + source_schema_ref
-        schema = requests.get(request_path, verify=False)
+        schema = requests.get(request_path, verify=True)
         json_content = schema.json()['schema_mapping']
     else:
-        if source_schema_ref.startswith('xss:'):
+        if(source_schema_ref.startswith('xss:')):
             request_path += 'schemas/?iri=' + source_schema_ref
         else:
             request_path += 'schemas/?name=' + source_schema_ref
-        schema = requests.get(request_path, verify=False)
+        schema = requests.get(request_path, verify=True)
         json_content = schema.json()['schema']
-
     return json_content
 
 
 def get_source_validation_schema():
     """Retrieve source validation schema from XIA configuration """
     logger.info("Configuration of schemas and files for source")
     xia_data = XIAConfiguration.objects.first()
```

### Comparing `openlxp-xia-1.3.2/openlxp_xia/migrations/0001_initial.py` & `openlxp-xia-1.4.0/openlxp_xia/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.3.2/openlxp_xia/migrations/0002_use_xss.py` & `openlxp-xia-1.4.0/openlxp_xia/migrations/0002_use_xss.py`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.3.2/openlxp_xia/tests/test_setup.py` & `openlxp-xia-1.4.0/openlxp_xia/tests/test_setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-import hashlib
 from uuid import UUID
 
+import pandas as pd
 from django.test import TestCase
 
 
 class TestSetUp(TestCase):
     """Class with setup and teardown for tests in XIS"""
 
     def setUp(self):
@@ -20,18 +20,16 @@
             "Start_date": "2017-03-28T00:00:00-04:00",
             "KEY": "TestData 123",
             "SOURCESYSTEM": "AGENT",
             "test_description": "test description",
             "supplemental_data": "sample1"
         }
         self.key_value = "TestData 123_AGENT"
-        self.key_value_hash = hashlib.sha512(self.key_value.encode('utf-8'))\
-            .hexdigest()
-        self.hash_value = hashlib.sha512(str(self.source_metadata).
-                                         encode('utf-8')).hexdigest()
+        self.key_value_hash = "d2a7f8cc5d5484a4dde099c6a21a903a"
+        self.hash_value = "f454114ba41034e14df2a8f3c14a047d"
 
         self.target_metadata = {
             "Course": {
                 "CourseCode": "TestData 123",
                 "CourseTitle": "Acquisition Law",
                 "CourseAudience": "test_data",
                 "DepartmentName": "",
@@ -66,20 +64,16 @@
             "Start_date": "2017-03-28T00:00:00-04:00",
             "KEY": "TestData 234",
             "SOURCESYSTEM": "AGENT",
             "test_description": "test description",
             "supplemental_data": "sample1"
         }
         self.key_value_overwrite = "TestData 234_AGENT"
-        self.key_value_hash_overwrite = \
-            hashlib.sha512(self.key_value_overwrite.encode('utf-8'))\
-            .hexdigest()
-        self.hash_value_overwrite = \
-            hashlib.sha512(str(self.source_metadata_overwrite).
-                           encode('utf-8')).hexdigest()
+        self.key_value_hash_overwrite = "5a9a682afe965fb2aa1f9f50e5148ebd"
+        self.hash_value_overwrite = "81b86d6ac3b4d8561bd26f11d8feea9a"
 
         self.target_metadata_overwrite = {
             "Course": {
                 "CourseCode": "TestData 234",
                 "CourseTitle": "Acquisition Law",
                 "CourseAudience": "test_data",
                 "DepartmentName": "",
@@ -434,18 +428,18 @@
         self.datatype_list_as_object = {
             'key1': 'datetime',
             'key2': str,
             'key3': int,
             'key4': bool
         }
 
-        self.test_target_required_column_names = [
-            'Course.CourseProviderName',
+        self.test_target_required_column_names = {
             'Course.CourseCode',
-            'Course.CourseShortDescription']
+            'Course.CourseProviderName',
+            'Course.CourseShortDescription'}
         self.recommended_column_name = {'Technical_Information.Thumbnail',
                                         'CourseInstance.Thumbnail'}
 
         self.xis_api_endpoint_url = 'http://openlxp-xis:8020/api/metadata/'
 
         self.supplemental_api_endpoint = 'http://openlxp-xis:8020' \
                                          '/api/supplemental-data/'
@@ -465,14 +459,14 @@
         }
 
         self.supplemental_data = {
             "supplemental_data1": "sample1",
             "supplemental_data2": "sample2"
         }
 
-        # self.metadata_df = pd.DataFrame.from_dict(
-        #     {0: {1: self.source_metadata}}, orient='index')
+        self.metadata_df = pd.DataFrame.from_dict(
+            {0: {1: self.source_metadata}}, orient='index')
 
         return super().setUp()
 
     def tearDown(self):
         return super().tearDown()
```

### Comparing `openlxp-xia-1.3.2/openlxp_xia/tests/test_xia_command_intergration.py` & `openlxp-xia-1.4.0/openlxp_xia/tests/test_xia_command_intergration.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,16 +163,15 @@
         test_data_dict = MetadataLedger.objects.values(
             'source_metadata').filter(
             source_metadata_validation_status='Y',
             record_lifecycle_status='Active').exclude(
             source_metadata_validation_date=None)
 
         test_metadata_overwrite = \
-            MetadataFieldOverwrite(field_name='Course.test_name',
-                                   field_type='char',
+            MetadataFieldOverwrite(field_name='test_name', field_type='char',
                                    field_value='new_value', overwrite=True)
         test_metadata_overwrite.save()
         transform_source_using_key(test_data_dict, self.source_target_mapping,
                                    self.test_required_column_names,
                                    self.expected_datatype)
 
         result_data = MetadataLedger.objects.filter(
@@ -219,15 +218,14 @@
             record_lifecycle_status='Active',
             source_metadata=self.source_metadata,
             source_metadata_key_hash=self.key_value_hash,
             source_metadata_validation_status='Y',
             source_metadata_key=self.key_value,
             source_metadata_validation_date=timezone.now(),
             source_metadata_extraction_date=timezone.now())
-
         metadata_ledger.save()
 
         test_data_dict = MetadataLedger.objects.values(
             'source_metadata').filter(
             source_metadata_validation_status='Y',
             record_lifecycle_status='Active').exclude(
             source_metadata_validation_date=None)
@@ -322,20 +320,19 @@
 
     # Test cases for validate_target_metadata
 
     def test_get_target_validation_schema(self):
         """Test to retrieve source validation schema from XIA configuration """
         with patch('openlxp_xia.models.XIAConfiguration.field_overwrite'):
             xiaConfig = XIAConfiguration(
-                xss_api="https://xss.deloitteopenlxp.com/api/",
-                target_metadata_schema='p2881')
+                target_metadata_schema='p2881_target_validation_schema.json')
             xiaConfig.save()
             result_dict = get_target_validation_schema()
             expected_dict = \
-                read_json_data('p2881')
+                read_json_data('p2881_target_validation_schema.json')
             self.assertEqual(expected_dict, result_dict)
 
     def test_validate_target_using_key(self):
         """Test for Validating target data for required columns """
         metadata_ledger = MetadataLedger(
             record_lifecycle_status='Active',
             source_metadata=self.source_metadata,
@@ -388,20 +385,17 @@
         metadata_ledger = MetadataLedger(
             source_metadata=self.source_metadata,
             target_metadata=self.target_metadata,
             target_metadata_key_hash=self.key_value_hash)
         metadata_ledger.save()
 
         supplemental_ledger = SupplementalLedger(
-            supplemental_metadata={"key1": "value1"},
-            supplemental_metadata_key_hash=self.key_value_hash,
-            record_lifecycle_status="Active"
-        )
+            supplemental_metadata={"key": "value"},
+            supplemental_metadata_key_hash=self.key_value_hash)
         supplemental_ledger.save()
-
         store_target_metadata_validation_status(MetadataLedger.objects.
                                                 values('target_metadata'),
                                                 self.key_value_hash,
                                                 'Y', 'Active', MetadataLedger.
                                                 objects.
                                                 values('target_metadata')
                                                 )
@@ -429,18 +423,16 @@
         metadata_ledger = MetadataLedger(
             source_metadata=self.source_metadata,
             target_metadata=self.target_metadata,
             target_metadata_key_hash=self.key_value_hash)
         metadata_ledger.save()
         supplemental_ledger = SupplementalLedger(
             supplemental_metadata={"key": "value"},
-            supplemental_metadata_key_hash=self.key_value_hash,
-            record_lifecycle_status="Active")
+            supplemental_metadata_key_hash=self.key_value_hash)
         supplemental_ledger.save()
-
         store_target_metadata_validation_status(MetadataLedger.objects.
                                                 values('target_metadata'),
                                                 self.key_value_hash,
                                                 'N', 'Inactive',
                                                 MetadataLedger.objects.
                                                 values('target_metadata')
                                                 )
```

### Comparing `openlxp-xia-1.3.2/openlxp_xia/tests/test_xia_command_unit.py` & `openlxp-xia-1.4.0/openlxp_xia/tests/test_xia_command_unit.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import copy
 import logging
 from unittest.mock import patch
 
 from ddt import ddt
 from django.test import tag
 from django.utils import timezone
 
@@ -10,25 +9,26 @@
     load_supplemental_metadata_to_xis, post_supplemental_metadata_to_xis,
     rename_supplemental_metadata_fields)
 from openlxp_xia.management.commands.load_target_metadata import (
     get_records_to_load_into_xis, post_data_to_xis,
     rename_metadata_ledger_fields)
 from openlxp_xia.management.commands.transform_source_metadata import (
     create_supplemental_metadata, create_target_metadata_dict,
-    get_source_metadata_for_transformation, overwrite_append_metadata,
-    overwrite_metadata_field, transform_source_using_key,
-    type_checking_target_metadata)
+    get_metadata_fields_to_overwrite, get_source_metadata_for_transformation,
+    overwrite_append_metadata, overwrite_metadata_field,
+    transform_source_using_key, type_checking_target_metadata)
 from openlxp_xia.management.commands.validate_source_metadata import (
-    get_source_metadata_for_validation,
-    store_source_metadata_validation_status, validate_source_using_key)
+    get_source_metadata_for_validation, validate_source_using_key,
+    store_source_metadata_validation_status)
 from openlxp_xia.management.commands.validate_target_metadata import (
     get_target_metadata_for_validation, update_previous_instance_in_metadata,
     validate_target_using_key)
-from openlxp_xia.models import (MetadataLedger, SupplementalLedger,
-                                XIAConfiguration, XISConfiguration)
+from openlxp_xia.models import (MetadataFieldOverwrite, MetadataLedger,
+                                SupplementalLedger, XIAConfiguration,
+                                XISConfiguration)
 
 from .test_setup import TestSetUp
 
 logger = logging.getLogger('dict_config_logger')
 
 
 @tag('unit')
@@ -154,20 +154,19 @@
         self.assertTrue(result_metadata['metadata_record_inactivation_date'])
 
     # Test cases for transform_source_metadata
 
     def test_type_checking_target_metadata(self):
         """"Test function for type checking and explicit type conversion of
         metadata """
-
-        key_check = copy.deepcopy(self.target_metadata)
-        type_checking_target_metadata(1, key_check,
-                                      self.expected_datatype,
-                                      "General_Information.EndDate")
-        self.assertIsInstance(key_check['General_Information'][
+        target_metadata = {
+            0: self.target_metadata}
+        target_metadata = type_checking_target_metadata(1, target_metadata,
+                                                        self.expected_datatype)
+        self.assertIsInstance(target_metadata[0]['General_Information'][
                                   "EndDate"], str)
 
     def test_get_source_metadata_for_transformation(self):
         """Test to Retrieving Source metadata from MetadataLedger that needs
         to be transformed"""
         with patch('openlxp_xia.management.commands.'
                    'transform_source_metadata'
@@ -199,19 +198,18 @@
                    'dict_flatten', return_value=self.source_metadata), \
                 patch('openlxp_xia.management.commands.'
                       'transform_source_metadata.create_supplemental_metadata',
                       return_value=None):
             result_data_dict, supplemental_data = create_target_metadata_dict(
                 1, self.source_target_mapping, self.source_metadata,
                 self.test_required_column_names, self.expected_datatype)
-
-            self.assertEqual(result_data_dict['Course'].get('CourseCode'),
+            self.assertEqual(result_data_dict[0]['Course'].get('CourseCode'),
                              expected_data_dict[0]['Course'].get('CourseCode'))
             self.assertEqual(
-                result_data_dict['Course'].get('CourseProviderName'),
+                result_data_dict[0]['Course'].get('CourseProviderName'),
                 expected_data_dict[0]['Course'].get('CourseProviderName'))
 
     def test_transform_source_using_key_more_zero(self):
         """Test for transforming source data using target metadata schema
         with no data"""
         data = []
         with patch('openlxp_xia.management.utils.xia_internal'
@@ -234,16 +232,16 @@
 
             self.assertEqual(
                 mock_store_transformed_source.call_count, 0)
 
     def test_transform_source_using_key_more_than_one(self):
         """Test for transforming source data using target metadata schema for
         more than one row"""
-        data = [{"source_metadata": self.source_metadata},
-                {"source_metadata": self.source_metadata}]
+        data = [{0: self.source_metadata},
+                {1: self.source_metadata}]
         with patch('openlxp_xia.management.utils.xia_internal'
                    '.get_target_metadata_key_value',
                    return_value=None), \
                 patch('openlxp_xia.management.commands.'
                       'transform_source_metadata'
                       '.store_transformed_source_metadata',
                       return_value=None) as mock_store_transformed_source:
@@ -262,26 +260,46 @@
                 mock_store_transformed_source.call_count, 2)
 
     def test_overwrite_metadata_field(self):
         """Test to overwrite metadata with admin entered values and
         return metadata in dictionary format """
 
         with patch('openlxp_xia.management.commands.transform_source_metadata'
-                   '.overwrite_append_metadata') as mock_get_overwrite:
-            mock_get_overwrite.return_value = self.target_metadata
+                   '.get_metadata_fields_to_overwrite') as mock_get_overwrite:
+            mock_get_overwrite.return_value = self.metadata_df
 
-            return_val = overwrite_metadata_field(self.target_metadata)
+            return_val = overwrite_metadata_field(self.metadata_df)
             self.assertIsInstance(return_val, dict)
 
+    def test_get_metadata_fields_to_overwrite(self):
+        """Test for looping through fields to be overwrite or appended"""
+        with patch('openlxp_xia.management.commands.'
+                   'transform_source_metadata.MetadataFieldOverwrite.'
+                   'objects') as mock_field, \
+                patch('openlxp_xia.management.commands.'
+                      'transform_source_metadata.'
+                      'overwrite_append_metadata') as mock_overwrite_fun:
+            config = \
+                [MetadataFieldOverwrite(field_name='column1', overwrite=True,
+                                        field_value='value1'),
+                 MetadataFieldOverwrite(field_name='column2', overwrite=False,
+                                        field_value='value2')]
+            mock_field.all.return_value = config
+            mock_overwrite_fun.return_value = self.metadata_df
+
+            get_metadata_fields_to_overwrite(self.metadata_df)
+            self.assertEqual(mock_overwrite_fun.call_count, 2)
+
     def test_overwrite_append_metadata(self):
         """test Overwrite & append metadata fields based on overwrite flag """
-        overwrite_append_metadata(self.target_metadata, 'column_1',
-                                  'value_1', True)
+        return_val = \
+            overwrite_append_metadata(self.metadata_df, 'column_1', 'value_1',
+                                      True)
 
-        self.assertEqual(self.target_metadata['column_1'], 'value_1')
+        self.assertEqual(return_val['column_1'][0], 'value_1')
 
     # Test cases for validate_target_metadata
 
     def test_get_target_metadata_for_validation(self):
         """Test to Retrieving target metadata from MetadataLedger that needs
         to be validated"""
         with patch('openlxp_xia.management.commands.'
@@ -356,15 +374,15 @@
                                   target_metadata_validation_date=timezone.
                                   now())
         metadata.save()
         update_previous_instance_in_metadata(self.key_value_hash)
 
         updated_value = MetadataLedger.objects. \
             get(target_metadata_key_hash=self.target_key_value_hash)
-        self.assertEqual(updated_value.record_lifecycle_status, 'Active')
+        self.assertEqual(updated_value.record_lifecycle_status, 'Inactive')
 
     # Test cases for load_target_metadata
 
     def test_rename_metadata_ledger_fields(self):
         """Test for Renaming XIA column names to match with XIS column names"""
         with patch('openlxp_xia.management.utils.xia_internal'
                    '.get_publisher_detail'), \
```

### Comparing `openlxp-xia-1.3.2/openlxp_xia/tests/test_xia_models_integration.py` & `openlxp-xia-1.4.0/openlxp_xia/tests/test_xia_models_integration.py`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.3.2/openlxp_xia/tests/test_xia_models_unit.py` & `openlxp-xia-1.4.0/openlxp_xia/tests/test_xia_models_unit.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,27 +29,44 @@
         self.assertEqual(xiaConfig.xss_api, xss_api)
         self.assertEqual(xiaConfig.target_metadata_schema,
                          target_metadata_schema)
 
     def test_create_two_xia_configuration(self):
         """Test that trying to create more than one XIS Configuration throws
         ValidationError """
-        with patch('openlxp_xia.signals.read_json_data'):
+        with patch("openlxp_xia.models.XIAConfiguration.field_overwrite"):
             with self.assertRaises(ValidationError):
                 xiaConfig = \
                     XIAConfiguration(source_metadata_schema="example1.json",
                                      xss_api="https://localhost",
                                      target_metadata_schema="example1.json")
                 xiaConfig2 = \
                     XIAConfiguration(source_metadata_schema="example2.json",
                                      xss_api="https://localhost",
                                      target_metadata_schema="example2.json")
                 xiaConfig.save()
                 xiaConfig2.save()
 
+    def test_xia_field_overwrite(self):
+        """Test that field_overwrite in an XIA Configuration generates
+        MetadataFieldOverwrite objects """
+        with patch("openlxp_xia.models.requests") as mock:
+            target_schema = {"schema": {
+                "start": {"test": {"use": "Required"}}}}
+            transform_schema = {"schema_mapping": {
+                "start": {"test": "start.test"}}}
+            mock.get.return_value = mock
+            mock.json.side_effect = [target_schema, transform_schema]
+            xiaConfig = \
+                XIAConfiguration(source_metadata_schema="example1.json",
+                                 xss_api="https://localhost",
+                                 target_metadata_schema="example1.json")
+            xiaConfig.save()
+            self.assertEqual(MetadataFieldOverwrite.objects.count(), 1)
+
     def test_create_xis_configuration(self):
         """Test that creating a new XIS Configuration entry is successful
         with defaults """
         xis_metadata_api_endpoint = 'http://localhost:8000/api/metadata/'
         xis_supplemental_api_endpoint = 'http://localhost:8000/api/supplement/'
 
         xisConfig = XISConfiguration(
```

### Comparing `openlxp-xia-1.3.2/openlxp_xia/tests/test_xia_utils_integration.py` & `openlxp-xia-1.4.0/openlxp_xia/tests/test_xia_utils_integration.py`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.3.2/openlxp_xia/tests/test_xia_utils_unit.py` & `openlxp-xia-1.4.0/openlxp_xia/tests/test_xia_utils_unit.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,19 +2,18 @@
 import logging
 from unittest.mock import patch
 
 from ddt import data, ddt, unpack
 from django.test import tag
 
 from openlxp_xia.management.utils.xia_internal import (
-    assign_target_value_str_list, dict_flatten, flatten_dict_object,
-    flatten_list_object, get_key_dict, get_publisher_detail,
-    get_target_metadata_key_value, is_date, replace_field_on_target_schema,
-    transform_to_target, traverse_dict, traverse_dict_with_key_list,
-    type_cast_overwritten_values, type_check_change, update_flattened_object)
+    dict_flatten, flatten_dict_object, flatten_list_object, get_key_dict,
+    get_publisher_detail, get_target_metadata_key_value, is_date,
+    replace_field_on_target_schema, type_cast_overwritten_values,
+    update_flattened_object)
 from openlxp_xia.management.utils.xis_client import (
     get_xis_metadata_api_endpoint, get_xis_supplemental_metadata_api_endpoint)
 from openlxp_xia.management.utils.xss_client import (
     get_data_types_for_validation, get_required_fields_for_validation,
     get_source_validation_schema, get_target_metadata_for_transformation,
     get_target_validation_schema, read_json_data, xss_get)
 from openlxp_xia.models import XIAConfiguration, XISConfiguration
@@ -49,32 +48,34 @@
             'key_value_hash': second_value
         }
         result = get_key_dict(first_value, second_value)
         self.assertEquals(result, expected_result)
 
     def test_replace_field_on_target_schema(self):
         """test to check if values under educational context are replaced"""
-        test_dict0 = {
+        test_dict0 = {'0': {
             "Course": {
                 "EducationalContext": "Y"
             }
         }
+        }
 
-        test_dict1 = {
+        test_dict1 = {'1': {
             "Course": {
                 "EducationalContext": "n"
             }
         }
+        }
 
         replace_field_on_target_schema('0', test_dict0)
-        self.assertEqual(test_dict0['Course']['EducationalContext'],
+        self.assertEqual(test_dict0['0']['Course']['EducationalContext'],
                          'Mandatory')
 
         replace_field_on_target_schema('1', test_dict1)
-        self.assertEqual(test_dict1['Course']['EducationalContext'],
+        self.assertEqual(test_dict1['1']['Course']['EducationalContext'],
                          'Non - Mandatory')
 
     @data((1, False), ("1990-12-1", True), ("Monday at 12:01am", True))
     @unpack
     def test_is_date(self, value_to_be_tested, result):
         """tests whether the string can be interpreted as a date."""
         check = is_date(value_to_be_tested)
@@ -378,59 +379,14 @@
         """Test the function to check type of overwritten value and convert it
         into required format"""
         field_type = first_value
         field_value = second_value
         values = type_cast_overwritten_values(field_type, field_value)
         self.assertNotIsInstance(values, int)
 
-    @data("Course", "test")
-    def test_traverse_dict(self, value):
-        """Test Function to traverse through dict"""
-        return_val = traverse_dict(self.target_metadata, value)
-
-        self.assertIsInstance(return_val, dict)
-
-    def test_assign_target_value_str_list(self):
-        """Test Function to replace source key with
-        source value in target metadata"""
-        assign_target_value_str_list(self.source_metadata,
-                                     self.source_target_mapping["Course"],
-                                     "CourseProviderName")
-        self.assertEqual(
-            self.source_target_mapping["Course"]["CourseProviderName"],
-            self.source_metadata["SOURCESYSTEM"])
-
-    def test_transform_to_target(self):
-        """Test Function to transform source to target"""
-        with patch('openlxp_xia.management.'
-                   'utils.xia_internal.'
-                   'assign_target_value_str_list') as mock_assign_target_value:
-            transform_to_target(self.source_metadata,
-                                self.source_target_mapping)
-
-            self.assertEqual(mock_assign_target_value.call_count,
-                             sum(len(v) for v in
-                                 self.source_target_mapping.values()))
-
-    def test_type_check_change(self):
-        """Test to function for type checking explicitly converting datatype"""
-        item = 'General_Information.EndDate'
-        target_metadata = self.target_metadata["General_Information"]
-        type_check_change(1, item, self.expected_datatype,
-                          target_metadata, 'EndDate')
-        self.assertIsInstance(target_metadata[
-                                  "EndDate"], str)
-
-    def test_traverse_dict_with_key_list(self):
-        """Test Function to traverse through dict with a key list"""
-        key_list = self.test_target_required_column_names[0].split('.')
-        return_val = \
-            traverse_dict_with_key_list(self.target_metadata, key_list)
-        self.assertEqual(return_val, self.target_metadata[key_list[0]])
-
     # Test cases for XIS_CLIENT
 
     def test_get_xis_metadata_api_endpoint(self):
         """Test to retrieve xis_metadata_api_endpoint from XIS configuration"""
         with patch('openlxp_xia.management.utils.xis_client'
                    '.XISConfiguration.objects') as xisCfg:
             xisConfig = XISConfiguration(
@@ -504,17 +460,17 @@
         """Test to retrieve target metadata schema from XIA configuration """
         with patch('openlxp_xia.management.utils.xss_client'
                    '.XIAConfiguration.objects') as xia_config_obj, \
                 patch('openlxp_xia.management.utils.xss_client'
                       '.read_json_data') as read_obj:
             xiaConfig = XIAConfiguration(
                 target_metadata_schema='AGENT_p2881_target_metadata_schema' +
-                                       '.json',
+                '.json',
                 source_metadata_schema='AGENT_p2881_target_metadata_schema' +
-                                       '.json'
+                '.json'
             )
             xia_config_obj.return_value = xiaConfig
             read_obj.return_value = read_obj
             read_obj.return_value = self.target_data_dict
             return_from_function = get_target_metadata_for_transformation()
             self.assertEqual(read_obj.return_value,
                              return_from_function)
@@ -522,28 +478,28 @@
     def test_xss_get(self):
         """Test for retrieving XSS api root """
         with patch('openlxp_xia.management.utils.xss_client'
                    '.XIAConfiguration.objects') as xia_config_obj:
             xss_api = "http://test_xss_api"
             xiaConfig = XIAConfiguration(
                 target_metadata_schema='AGENT_p2881_target_metadata_schema' +
-                                       '.json',
+                '.json',
                 source_metadata_schema='AGENT_p2881_target_metadata_schema' +
-                                       '.json',
+                '.json',
                 xss_api=xss_api
             )
             xia_config_obj.first.return_value = xiaConfig
 
             self.assertEqual(xss_get(), xss_api)
 
     def test_read_json_data(self):
         """Test for retrieving XSS json schemas """
         with patch('openlxp_xia.management.utils.xss_client.xss_get') as \
-                xss_host, patch('openlxp_xia.management.utils.xss_client.'
-                                'requests') as req:
+            xss_host, patch('openlxp_xia.management.utils.xss_client.'
+                            'requests') as req:
             xss_api = "http://test_xss_api"
             schema = {"schema": {"test": "val"}}
             xss_host.return_value = xss_api
             req.get.return_value = req
             req.json.return_value = schema
 
             self.assertEqual(read_json_data(""), schema['schema'])
```

### Comparing `openlxp-xia-1.3.2/openlxp_xia/urls.py` & `openlxp-xia-1.4.0/openlxp_xia/urls.py`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.3.2/openlxp_xia.egg-info/SOURCES.txt` & `openlxp-xia-1.4.0/openlxp_xia.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
+README.md
 setup.cfg
 setup.py
 openlxp_xia/__init__.py
 openlxp_xia/admin.py
 openlxp_xia/apps.py
 openlxp_xia/models.py
-openlxp_xia/signals.py
 openlxp_xia/urls.py
 openlxp_xia/views.py
 openlxp_xia.egg-info/PKG-INFO
 openlxp_xia.egg-info/SOURCES.txt
 openlxp_xia.egg-info/dependency_links.txt
 openlxp_xia.egg-info/requires.txt
 openlxp_xia.egg-info/top_level.txt
@@ -21,20 +21,17 @@
 openlxp_xia/management/commands/validate_target_metadata.py
 openlxp_xia/management/utils/__init__.py
 openlxp_xia/management/utils/xia_internal.py
 openlxp_xia/management/utils/xis_client.py
 openlxp_xia/management/utils/xss_client.py
 openlxp_xia/migrations/0001_initial.py
 openlxp_xia/migrations/0002_use_xss.py
-openlxp_xia/migrations/0003_auto_20220708_1111.py
-openlxp_xia/migrations/0004_auto_20230127_2011.py
 openlxp_xia/migrations/__init__.py
 openlxp_xia/tests/__init__.py
 openlxp_xia/tests/test_setup.py
-openlxp_xia/tests/test_signals.py
 openlxp_xia/tests/test_xia_command_intergration.py
 openlxp_xia/tests/test_xia_command_unit.py
 openlxp_xia/tests/test_xia_models_integration.py
 openlxp_xia/tests/test_xia_models_unit.py
 openlxp_xia/tests/test_xia_utils_integration.py
 openlxp_xia/tests/test_xia_utils_unit.py
 openlxp_xia_project/__init__.py
```

### Comparing `openlxp-xia-1.3.2/openlxp_xia_project/settings.py` & `openlxp-xia-1.4.0/openlxp_xia_project/settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 INSTALLED_APPS = [
     'django.contrib.admin',
     'django.contrib.auth',
     'django.contrib.contenttypes',
     'django.contrib.sessions',
     'django.contrib.messages',
     'django.contrib.staticfiles',
-    'openlxp_xia.apps.CoreConfig',
+    'openlxp_xia',
 ]
 
 MIDDLEWARE = [
     'django.middleware.security.SecurityMiddleware',
     'django.contrib.sessions.middleware.SessionMiddleware',
     'django.middleware.common.CommonMiddleware',
     'django.middleware.csrf.CsrfViewMiddleware',
@@ -80,15 +80,15 @@
 
 
 # Database
 # https://docs.djangoproject.com/en/3.2/ref/settings/#databases
 #
 DATABASES = {
     'default': {
-        'ENGINE': 'mysql.connector.django',
+        'ENGINE': 'django.db.backends.mysql',
         'NAME': os.environ.get('DB_NAME'),
         'USER': os.environ.get('DB_USER'),
         'PASSWORD': os.environ.get('DB_PASSWORD'),
         'HOST': os.environ.get('DB_HOST'),
         'PORT': 3306,
     }
 }
@@ -136,46 +136,46 @@
 # Static files (CSS, JavaScript, Images)
 # https://docs.djangoproject.com/en/3.2/howto/static-files/
 
 STATIC_URL = '/static/'
 STATIC_ROOT = os.path.join(BASE_DIR, 'static')
 
 LOG_PATH = os.environ.get('LOG_PATH')
-# LOGGING = {
-#     'version': 1,
-#     'disable_existing_loggers': False,
-#
-#     'loggers': {
-#         'dict_config_logger': {
-#             'handlers': ['console', 'file_logs'],
-#             'level': 'INFO',
-#             'propagate': True,
-#         },
-#     },
-#
-#     'handlers': {
-#         'console': {
-#             'class': 'logging.StreamHandler',
-#             'stream': sys.stdout,
-#             'formatter': 'simpleRe',
-#         },
-#         'file_logs': {
-#             'level': 'WARNING',
-#             'class': 'logging.FileHandler',
-#             'filename': LOG_PATH,
-#             'formatter': 'simpleRe',
-#         },
-#
-#     },
-#
-#     'formatters': {
-#         'simpleRe': {
-#             'format': '{levelname} {asctime} {module} {message}',
-#             'style': '{',
-#         }
-#     }
-# }
+LOGGING = {
+    'version': 1,
+    'disable_existing_loggers': False,
+
+    'loggers': {
+        'dict_config_logger': {
+            'handlers': ['console', 'file_logs'],
+            'level': 'INFO',
+            'propagate': True,
+        },
+    },
+
+    'handlers': {
+        'console': {
+            'class': 'logging.StreamHandler',
+            'stream': sys.stdout,
+            'formatter': 'simpleRe',
+        },
+        'file_logs': {
+            'level': 'WARNING',
+            'class': 'logging.FileHandler',
+            'filename': LOG_PATH,
+            'formatter': 'simpleRe',
+        },
+
+    },
+
+    'formatters': {
+        'simpleRe': {
+            'format': '{levelname} {asctime} {module} {message}',
+            'style': '{',
+        }
+    }
+}
 
 CORS_ORIGIN_ALLOW_ALL = True
 
 MEDIA_URL = '/media/'
 MEDIA_ROOT = os.path.join(BASE_DIR, 'media')
```

### Comparing `openlxp-xia-1.3.2/openlxp_xia_project/urls.py` & `openlxp-xia-1.4.0/openlxp_xia_project/urls.py`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.3.2/setup.cfg` & `openlxp-xia-1.4.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 [metadata]
 name = openlxp-xia
-version = 1.3.2
+version = 1.4.0
 description = Sample installable XIA
 long_description = file:README.md
+long_description_content_type = text/markdown
 url = https://github.com/OpenLXP/openlxp-xia/
 author = OpenLXP
 author_email = openlxphost@gmail.com
 license = MIT
 classifiers = 
 	Development Status :: 4 - Beta
 	Environment :: Web Environment
```

