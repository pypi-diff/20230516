# Comparing `tmp/nautobot-bgp-models-0.7.0b0.tar.gz` & `tmp/nautobot-bgp-models-0.7.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nautobot-bgp-models-0.7.0b0.tar", max compression
+gzip compressed data, was "nautobot-bgp-models-0.7.0b1.tar", max compression
```

## Comparing `nautobot-bgp-models-0.7.0b0.tar` & `nautobot-bgp-models-0.7.0b1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0      591 2022-09-14 16:16:10.300613 nautobot-bgp-models-0.7.0b0/LICENSE
--rw-r--r--   0        0        0     3705 2022-09-14 16:16:10.300613 nautobot-bgp-models-0.7.0b0/README.md
--rw-r--r--   0        0        0     1587 2022-09-14 16:16:10.320613 nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/__init__.py
--rw-r--r--   0        0        0       54 2022-09-14 16:16:10.320613 nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/api/__init__.py
--rw-r--r--   0        0        0     1554 2022-09-14 16:16:10.320613 nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/api/filter_backends.py
--rw-r--r--   0        0        0     3194 2022-09-14 16:16:10.320613 nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/api/nested_serializers.py
--rw-r--r--   0        0        0     9181 2022-09-14 16:16:10.320613 nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/api/serializers.py
--rw-r--r--   0        0        0      793 2022-09-14 16:16:10.320613 nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/api/urls.py
--rw-r--r--   0        0        0     4182 2022-09-14 16:16:10.320613 nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/api/views.py
--rw-r--r--   0        0        0     1238 2022-09-14 16:16:10.320613 nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/choices.py
--rw-r--r--   0        0        0     1006 2022-09-14 16:16:10.320613 nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/dolt_compat.py
--rw-r--r--   0        0        0     1332 2022-09-14 16:16:10.320613 nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/filter_extensions.py
--rw-r--r--   0        0        0     8094 2022-09-14 16:16:10.320613 nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/filters.py
--rw-r--r--   0        0        0    18497 2022-09-14 16:16:10.320613 nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/forms.py
--rw-r--r--   0        0        0    20854 2022-09-14 16:16:10.320613 nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2022-09-14 16:16:10.320613 nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/migrations/__init__.py
--rw-r--r--   0        0        0    22471 2022-09-14 16:16:10.320613 nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/models.py
--rw-r--r--   0        0        0     4736 2022-09-14 16:16:10.320613 nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/navigation.py
--rw-r--r--   0        0        0     1056 2022-09-14 16:16:10.320613 nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/signals.py
--rw-r--r--   0        0        0     7670 2022-09-14 16:16:10.320613 nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/tables.py
--rw-r--r--   0        0        0     2025 2022-09-14 16:16:10.320613 nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/template_content.py
--rw-r--r--   0        0        0     3134 2022-09-14 16:16:10.320613 nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/templates/nautobot_bgp_models/addressfamily.html
--rw-r--r--   0        0        0     1309 2022-09-14 16:16:10.320613 nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/templates/nautobot_bgp_models/autonomoussystem.html
--rw-r--r--   0        0        0     1875 2022-09-14 16:16:10.320613 nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/templates/nautobot_bgp_models/bgproutinginstance.html
--rw-r--r--   0        0        0     1507 2022-09-14 16:16:10.320613 nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/templates/nautobot_bgp_models/extra_attributes.html
--rw-r--r--   0        0        0      761 2022-09-14 16:16:10.320613 nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/templates/nautobot_bgp_models/inc/device_address_families.html
--rw-r--r--   0        0        0      839 2022-09-14 16:16:10.320613 nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/templates/nautobot_bgp_models/inc/device_bgp_routing_instances.html
--rw-r--r--   0        0        0      918 2022-09-14 16:16:10.320613 nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/templates/nautobot_bgp_models/inc/device_peer_endpoints.html
--rw-r--r--   0        0        0      793 2022-09-14 16:16:10.320613 nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/templates/nautobot_bgp_models/inc/inheritable_property.html
--rw-r--r--   0        0        0      853 2022-09-14 16:16:10.320613 nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/templates/nautobot_bgp_models/inc/native_property.html
--rw-r--r--   0        0        0     3146 2022-09-14 16:16:10.320613 nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/templates/nautobot_bgp_models/inc/peerendpoint.html
--rw-r--r--   0        0        0     6203 2022-09-14 16:16:10.324613 nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/templates/nautobot_bgp_models/peerendpoint.html
--rw-r--r--   0        0        0     5349 2022-09-14 16:16:10.324613 nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/templates/nautobot_bgp_models/peergroup.html
--rw-r--r--   0        0        0     3419 2022-09-14 16:16:10.324613 nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/templates/nautobot_bgp_models/peergrouptemplate.html
--rw-r--r--   0        0        0     1085 2022-09-14 16:16:10.324613 nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/templates/nautobot_bgp_models/peering.html
--rw-r--r--   0        0        0     2504 2022-09-14 16:16:10.324613 nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/templates/nautobot_bgp_models/peering_create.html
--rw-r--r--   0        0        0     1112 2022-09-14 16:16:10.324613 nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/templates/nautobot_bgp_models/peeringrole.html
--rw-r--r--   0        0        0       49 2022-09-14 16:16:10.324613 nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/tests/__init__.py
--rw-r--r--   0        0        0    25709 2022-09-14 16:16:10.324613 nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/tests/test_api.py
--rw-r--r--   0        0        0    22414 2022-09-14 16:16:10.324613 nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/tests/test_filters.py
--rw-r--r--   0        0        0    12400 2022-09-14 16:16:10.324613 nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/tests/test_forms.py
--rw-r--r--   0        0        0    17933 2022-09-14 16:16:10.324613 nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/tests/test_models.py
--rw-r--r--   0        0        0    13861 2022-09-14 16:16:10.324613 nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/tests/test_views.py
--rw-r--r--   0        0        0     8872 2022-09-14 16:16:10.324613 nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/urls.py
--rw-r--r--   0        0        0    16272 2022-09-14 16:16:10.324613 nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/views.py
--rw-r--r--   0        0        0     2529 2022-09-14 16:16:21.796762 nautobot-bgp-models-0.7.0b0/pyproject.toml
--rw-r--r--   0        0        0     4710 1970-01-01 00:00:00.000000 nautobot-bgp-models-0.7.0b0/setup.py
--rw-r--r--   0        0        0     4492 1970-01-01 00:00:00.000000 nautobot-bgp-models-0.7.0b0/PKG-INFO
+-rw-r--r--   0        0        0      591 2022-09-20 13:58:04.408465 nautobot-bgp-models-0.7.0b1/LICENSE
+-rw-r--r--   0        0        0     3705 2022-09-20 13:58:04.408465 nautobot-bgp-models-0.7.0b1/README.md
+-rw-r--r--   0        0        0     1587 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/__init__.py
+-rw-r--r--   0        0        0       54 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/api/__init__.py
+-rw-r--r--   0        0        0     1554 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/api/filter_backends.py
+-rw-r--r--   0        0        0     3194 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/api/nested_serializers.py
+-rw-r--r--   0        0        0     9181 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/api/serializers.py
+-rw-r--r--   0        0        0      793 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/api/urls.py
+-rw-r--r--   0        0        0     4182 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/api/views.py
+-rw-r--r--   0        0        0     1238 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/choices.py
+-rw-r--r--   0        0        0     1006 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/dolt_compat.py
+-rw-r--r--   0        0        0     1332 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/filter_extensions.py
+-rw-r--r--   0        0        0     8094 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/filters.py
+-rw-r--r--   0        0        0    18497 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/forms.py
+-rw-r--r--   0        0        0    20854 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/migrations/__init__.py
+-rw-r--r--   0        0        0    22471 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/models.py
+-rw-r--r--   0        0        0     4736 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/navigation.py
+-rw-r--r--   0        0        0     1148 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/signals.py
+-rw-r--r--   0        0        0     7670 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/tables.py
+-rw-r--r--   0        0        0     2025 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/template_content.py
+-rw-r--r--   0        0        0     3134 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/templates/nautobot_bgp_models/addressfamily.html
+-rw-r--r--   0        0        0     1309 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/templates/nautobot_bgp_models/autonomoussystem.html
+-rw-r--r--   0        0        0     1875 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/templates/nautobot_bgp_models/bgproutinginstance.html
+-rw-r--r--   0        0        0     1507 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/templates/nautobot_bgp_models/extra_attributes.html
+-rw-r--r--   0        0        0      761 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/templates/nautobot_bgp_models/inc/device_address_families.html
+-rw-r--r--   0        0        0      839 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/templates/nautobot_bgp_models/inc/device_bgp_routing_instances.html
+-rw-r--r--   0        0        0      918 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/templates/nautobot_bgp_models/inc/device_peer_endpoints.html
+-rw-r--r--   0        0        0      793 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/templates/nautobot_bgp_models/inc/inheritable_property.html
+-rw-r--r--   0        0        0      853 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/templates/nautobot_bgp_models/inc/native_property.html
+-rw-r--r--   0        0        0     3146 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/templates/nautobot_bgp_models/inc/peerendpoint.html
+-rw-r--r--   0        0        0     6203 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/templates/nautobot_bgp_models/peerendpoint.html
+-rw-r--r--   0        0        0     5349 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/templates/nautobot_bgp_models/peergroup.html
+-rw-r--r--   0        0        0     3419 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/templates/nautobot_bgp_models/peergrouptemplate.html
+-rw-r--r--   0        0        0     1085 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/templates/nautobot_bgp_models/peering.html
+-rw-r--r--   0        0        0     2504 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/templates/nautobot_bgp_models/peering_create.html
+-rw-r--r--   0        0        0     1112 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/templates/nautobot_bgp_models/peeringrole.html
+-rw-r--r--   0        0        0       49 2022-09-20 13:58:04.428466 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/tests/__init__.py
+-rw-r--r--   0        0        0    25709 2022-09-20 13:58:04.432467 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/tests/test_api.py
+-rw-r--r--   0        0        0    22414 2022-09-20 13:58:04.432467 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/tests/test_filters.py
+-rw-r--r--   0        0        0    12400 2022-09-20 13:58:04.432467 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/tests/test_forms.py
+-rw-r--r--   0        0        0    17933 2022-09-20 13:58:04.432467 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/tests/test_models.py
+-rw-r--r--   0        0        0    13861 2022-09-20 13:58:04.432467 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/tests/test_views.py
+-rw-r--r--   0        0        0     8872 2022-09-20 13:58:04.432467 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/urls.py
+-rw-r--r--   0        0        0    16272 2022-09-20 13:58:04.432467 nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/views.py
+-rw-r--r--   0        0        0     2529 2022-09-20 13:58:15.228920 nautobot-bgp-models-0.7.0b1/pyproject.toml
+-rw-r--r--   0        0        0     4710 1970-01-01 00:00:00.000000 nautobot-bgp-models-0.7.0b1/setup.py
+-rw-r--r--   0        0        0     4492 1970-01-01 00:00:00.000000 nautobot-bgp-models-0.7.0b1/PKG-INFO
```

### Comparing `nautobot-bgp-models-0.7.0b0/LICENSE` & `nautobot-bgp-models-0.7.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b0/README.md` & `nautobot-bgp-models-0.7.0b1/README.md`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/__init__.py` & `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/__init__.py`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/api/filter_backends.py` & `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/api/filter_backends.py`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/api/nested_serializers.py` & `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/api/nested_serializers.py`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/api/serializers.py` & `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/api/serializers.py`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/api/urls.py` & `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/api/urls.py`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/api/views.py` & `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/api/views.py`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/choices.py` & `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/choices.py`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/dolt_compat.py` & `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/dolt_compat.py`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/filter_extensions.py` & `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/filter_extensions.py`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/filters.py` & `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/filters.py`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/forms.py` & `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/forms.py`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/migrations/0001_initial.py` & `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/models.py` & `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/models.py`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/navigation.py` & `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/navigation.py`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/signals.py` & `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/signals.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 """Nautobot signal handler functions for nautobot_bgp_models."""
 
+from django.apps import apps as global_apps
 from django.conf import settings
 
 PLUGIN_SETTINGS = settings.PLUGINS_CONFIG["nautobot_bgp_models"]
 
 
-def post_migrate_create_statuses(sender, apps, **kwargs):
+def post_migrate_create_statuses(sender, *, apps=global_apps, **kwargs):
     """Callback function for post_migrate() -- create default Statuses."""
     # pylint: disable=invalid-name
+    if not apps:
+        return
+
     Status = apps.get_model("extras", "Status")
 
     for model_name, default_statuses in PLUGIN_SETTINGS.get("default_statuses", {}).items():
         model = sender.get_model(model_name)
 
         ContentType = apps.get_model("contenttypes", "ContentType")
         ct_model = ContentType.objects.get_for_model(model)
```

### Comparing `nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/tables.py` & `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/tables.py`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/template_content.py` & `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/template_content.py`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/templates/nautobot_bgp_models/addressfamily.html` & `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/templates/nautobot_bgp_models/addressfamily.html`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/templates/nautobot_bgp_models/autonomoussystem.html` & `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/templates/nautobot_bgp_models/autonomoussystem.html`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/templates/nautobot_bgp_models/bgproutinginstance.html` & `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/templates/nautobot_bgp_models/bgproutinginstance.html`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/templates/nautobot_bgp_models/extra_attributes.html` & `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/templates/nautobot_bgp_models/extra_attributes.html`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/templates/nautobot_bgp_models/inc/device_address_families.html` & `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/templates/nautobot_bgp_models/inc/device_address_families.html`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/templates/nautobot_bgp_models/inc/device_bgp_routing_instances.html` & `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/templates/nautobot_bgp_models/inc/device_bgp_routing_instances.html`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/templates/nautobot_bgp_models/inc/device_peer_endpoints.html` & `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/templates/nautobot_bgp_models/inc/device_peer_endpoints.html`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/templates/nautobot_bgp_models/inc/inheritable_property.html` & `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/templates/nautobot_bgp_models/inc/inheritable_property.html`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/templates/nautobot_bgp_models/inc/native_property.html` & `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/templates/nautobot_bgp_models/inc/native_property.html`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/templates/nautobot_bgp_models/inc/peerendpoint.html` & `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/templates/nautobot_bgp_models/inc/peerendpoint.html`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/templates/nautobot_bgp_models/peerendpoint.html` & `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/templates/nautobot_bgp_models/peerendpoint.html`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/templates/nautobot_bgp_models/peergroup.html` & `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/templates/nautobot_bgp_models/peergroup.html`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/templates/nautobot_bgp_models/peergrouptemplate.html` & `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/templates/nautobot_bgp_models/peergrouptemplate.html`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/templates/nautobot_bgp_models/peering.html` & `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/templates/nautobot_bgp_models/peering.html`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/templates/nautobot_bgp_models/peering_create.html` & `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/templates/nautobot_bgp_models/peering_create.html`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/templates/nautobot_bgp_models/peeringrole.html` & `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/templates/nautobot_bgp_models/peeringrole.html`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/tests/test_api.py` & `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/tests/test_filters.py` & `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/tests/test_forms.py` & `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/tests/test_models.py` & `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/tests/test_views.py` & `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/urls.py` & `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/urls.py`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b0/nautobot_bgp_models/views.py` & `nautobot-bgp-models-0.7.0b1/nautobot_bgp_models/views.py`

 * *Files identical despite different names*

### Comparing `nautobot-bgp-models-0.7.0b0/pyproject.toml` & `nautobot-bgp-models-0.7.0b1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nautobot-bgp-models"
-version = "v0.7.0-beta.0"
+version = "v0.7.0-beta.1"
 description = "Nautobot BGP Models Plugin"
 authors = ["Network to Code, LLC <info@networktocode.com>"]
 
 license = "Apache-2.0"
 
 readme = "README.md"
 homepage = "https://github.com/nautobot/nautobot-plugin-bgp-models"
```

### Comparing `nautobot-bgp-models-0.7.0b0/setup.py` & `nautobot-bgp-models-0.7.0b1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
                          'templates/nautobot_bgp_models/inc/*']}
 
 install_requires = \
 ['nautobot>=1.3,<2.0']
 
 setup_kwargs = {
     'name': 'nautobot-bgp-models',
-    'version': '0.7.0b0',
+    'version': '0.7.0b1',
     'description': 'Nautobot BGP Models Plugin',
     'long_description': '# Nautobot BGP Models Plugin\n\nA plugin for [Nautobot](https://github.com/nautobot/nautobot) extending the core models with BGP-specific models.\n\nNew models enable modeling and management of BGP peerings, whether or not the peer device is present in Nautobot.\n\n> The initial development of this plugin was sponsored by Riot Games, Inc.\n\n## Data Models\n\nNavigate to [Data Models](docs/cisco_use_case.md) for detailed descriptions on additional data models provided in the plugin.\n\n## Use Cases\n\nTo make the start with the plugin easier, we provide two example use cases for common OS platforms: Cisco and Juniper.\n\n### Cisco Configuration Modeling and Rendering\n\nNavigate to [Cisco Example Use Case](docs/cisco_use_case.md) for detailed instructions how to consume BGP Models plugin on Cisco devices.\n\n### Juniper Configuration Modeling and Rendering\n\nNavigate to [Juniper Example Use Case](docs/juniper_use_case.md) for detailed instructions how to consume BGP Models plugin on Juniper devices.\n\n## Installation\n\nThe plugin is available as a Python package in PyPI and can be installed with `pip`:\n\n```shell\npip install nautobot-bgp-models\n```\n\n> The plugin is compatible with Nautobot 1.3 and higher\n\nTo ensure Nautobot BGP Models Plugin is automatically re-installed during future upgrades, create a file named `local_requirements.txt` (if not already existing) in the Nautobot root directory (alongside `requirements.txt`) and list the `nautobot-bgp-models` package:\n\n```no-highlight\n# echo nautobot-bgp-models >> local_requirements.txt\n```\n\nOnce installed, the plugin needs to be enabled in your `nautobot_config.py`\n\n```python\n# In your configuration.py\nPLUGINS = ["nautobot_bgp_models"]\n```\n\n```python\nPLUGINS_CONFIG = {\n    "nautobot_bgp_models": {\n        "default_statuses": {\n            "AutonomousSystem": ["active", "available", "planned"],\n            "Peering": ["active", "decommissioned", "deprovisioning", "offline", "planned", "provisioning"],\n        }\n    }\n}\n```\n\nIn the `default_statuses` section, you can define a list of default statuses to make available to `AutonomousSystem` and/or `Peering`. The lists must be composed of valid slugs of existing Status objects.\n\n## Screenshots\n\n![Menu](https://github.com/nautobot/nautobot-plugin-bgp-models/blob/main/docs/images/main-page-menu.png)\n\n![Autonomous System](https://github.com/nautobot/nautobot-plugin-bgp-models/blob/main/docs/images/autonomous_system_01.png)\n\n![Peering List](https://github.com/nautobot/nautobot-plugin-bgp-models/blob/main/docs/images/peering_list.png)\n\n![Peering](https://github.com/nautobot/nautobot-plugin-bgp-models/blob/main/docs/images/peering_01.png)\n\n![Peer Endpoint](https://github.com/nautobot/nautobot-plugin-bgp-models/blob/main/docs/images/peer_endpoint_01.png)\n\n![Peer Group](https://github.com/nautobot/nautobot-plugin-bgp-models/blob/main/docs/images/peer_group_01.png)\n\n## Contributing\n\nPull requests are welcomed and automatically built and tested against multiple version of Python and multiple version of Nautobot through TravisCI.\n\nThe project is packaged with a light development environment based on `docker-compose` to help with the local development of the project and to run the tests within TravisCI.\n\nThe project is following Network to Code software development guideline and is leveraging:\n\n- Black, Pylint, Bandit and pydocstyle for Python linting and formatting.\n- Django unit test to ensure the plugin is working properly.\n\n## Questions\n\nFor any questions or comments, please check the [FAQ](FAQ.md) first and feel free to swing by the [Network to Code slack channel](https://networktocode.slack.com/) (channel #networktocode).\nSign up [here](http://slack.networktocode.com/)\n',
     'author': 'Network to Code, LLC',
     'author_email': 'info@networktocode.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/nautobot/nautobot-plugin-bgp-models',
```

### Comparing `nautobot-bgp-models-0.7.0b0/PKG-INFO` & `nautobot-bgp-models-0.7.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nautobot-bgp-models
-Version: 0.7.0b0
+Version: 0.7.0b1
 Summary: Nautobot BGP Models Plugin
 Home-page: https://github.com/nautobot/nautobot-plugin-bgp-models
 License: Apache-2.0
 Keywords: nautobot,nautobot-plugin
 Author: Network to Code, LLC
 Author-email: info@networktocode.com
 Requires-Python: >=3.7,<4.0
```

