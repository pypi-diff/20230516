# Comparing `tmp/openimis-be-location-1.5.0.tar.gz` & `tmp/openimis-be-location-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis-be-location-1.5.0.tar", last modified: Thu Nov 10 18:09:17 2022, max compression
+gzip compressed data, was "openimis-be-location-1.5.1.tar", last modified: Tue May 16 21:37:57 2023, max compression
```

## Comparing `openimis-be-location-1.5.0.tar` & `openimis-be-location-1.5.1.tar`

### file list

```diff
@@ -1,38 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 18:09:17.535987 openimis-be-location-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1852 2022-11-10 18:09:04.000000 openimis-be-location-1.5.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-11-10 18:09:04.000000 openimis-be-location-1.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      690 2022-11-10 18:09:17.535987 openimis-be-location-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1579 2022-11-10 18:09:04.000000 openimis-be-location-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 18:09:17.531987 openimis-be-location-1.5.0/location/
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-11-10 18:09:04.000000 openimis-be-location-1.5.0/location/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-11-10 18:09:04.000000 openimis-be-location-1.5.0/location/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)     3239 2022-11-10 18:09:04.000000 openimis-be-location-1.5.0/location/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)      692 2022-11-10 18:09:04.000000 openimis-be-location-1.5.0/location/dataloaders.py
--rw-r--r--   0 runner    (1001) docker     (121)    11861 2022-11-10 18:09:04.000000 openimis-be-location-1.5.0/location/gql_mutations.py
--rw-r--r--   0 runner    (1001) docker     (121)     4806 2022-11-10 18:09:04.000000 openimis-be-location-1.5.0/location/gql_queries.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 18:09:17.531987 openimis-be-location-1.5.0/location/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     1918 2022-11-10 18:09:04.000000 openimis-be-location-1.5.0/location/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)     1815 2022-11-10 18:09:04.000000 openimis-be-location-1.5.0/location/migrations/0002_location.py
--rw-r--r--   0 runner    (1001) docker     (121)      954 2022-11-10 18:09:04.000000 openimis-be-location-1.5.0/location/migrations/0003_userdistrict.py
--rw-r--r--   0 runner    (1001) docker     (121)      985 2022-11-10 18:09:04.000000 openimis-be-location-1.5.0/location/migrations/0004_locationmutation.py
--rw-r--r--   0 runner    (1001) docker     (121)     3231 2022-11-10 18:09:04.000000 openimis-be-location-1.5.0/location/migrations/0005_healthfacilitycatchment_healthfacilitylegalform_healthfacilitymutation_healthfacilitysublevel.py
--rw-r--r--   0 runner    (1001) docker     (121)     1044 2022-11-10 18:09:04.000000 openimis-be-location-1.5.0/location/migrations/0006_users_api.py
--rw-r--r--   0 runner    (1001) docker     (121)      756 2022-11-10 18:09:04.000000 openimis-be-location-1.5.0/location/migrations/0007_auto_20211103_1046.py
--rw-r--r--   0 runner    (1001) docker     (121)     1042 2022-11-10 18:09:04.000000 openimis-be-location-1.5.0/location/migrations/0008_add_enrollment_officer_gql_query_location_right.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-10 18:09:04.000000 openimis-be-location-1.5.0/location/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13927 2022-11-10 18:09:04.000000 openimis-be-location-1.5.0/location/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     5624 2022-11-10 18:09:04.000000 openimis-be-location-1.5.0/location/schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     5837 2022-11-10 18:09:04.000000 openimis-be-location-1.5.0/location/services.py
--rw-r--r--   0 runner    (1001) docker     (121)    10172 2022-11-10 18:09:04.000000 openimis-be-location-1.5.0/location/test_graphql.py
--rw-r--r--   0 runner    (1001) docker     (121)     1503 2022-11-10 18:09:04.000000 openimis-be-location-1.5.0/location/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-11-10 18:09:04.000000 openimis-be-location-1.5.0/location/tests.py
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-11-10 18:09:04.000000 openimis-be-location-1.5.0/location/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-11-10 18:09:04.000000 openimis-be-location-1.5.0/location/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 18:09:17.535987 openimis-be-location-1.5.0/openimis_be_location.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      690 2022-11-10 18:09:17.000000 openimis-be-location-1.5.0/openimis_be_location.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1026 2022-11-10 18:09:17.000000 openimis-be-location-1.5.0/openimis_be_location.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-10 18:09:17.000000 openimis-be-location-1.5.0/openimis_be_location.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-11-10 18:09:17.000000 openimis-be-location-1.5.0/openimis_be_location.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-11-10 18:09:17.000000 openimis-be-location-1.5.0/openimis_be_location.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-10 18:09:17.535987 openimis-be-location-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1215 2022-11-10 18:09:15.000000 openimis-be-location-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:37:57.514262 openimis-be-location-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-16 21:37:57.514262 openimis-be-location-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:37:57.510262 openimis-be-location-1.5.1/location/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/location/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/location/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/location/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/location/dataloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12667 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/location/gql_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/location/gql_queries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:37:57.510262 openimis-be-location-1.5.1/location/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/location/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/location/migrations/0002_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/location/migrations/0003_userdistrict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/location/migrations/0004_locationmutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/location/migrations/0005_healthfacilitycatchment_healthfacilitylegalform_healthfacilitymutation_healthfacilitysublevel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/location/migrations/0006_users_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/location/migrations/0007_auto_20211103_1046.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/location/migrations/0008_add_enrollment_officer_gql_query_location_right.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/location/migrations/0009_add_location_read_right.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/location/migrations/0010_insert_create_region_location_perms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/location/migrations/0011_auto_20230317_0924.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/location/migrations/0012_auto_20230317_0927.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/location/migrations/0013_auto_20230317_1534.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/location/migrations/0014_add_missing_fields_to_django_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/location/migrations/0015_set_managed_to_true.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/location/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15924 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/location/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/location/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7747 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/location/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15748 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/location/test_graphql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/location/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/location/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/location/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-16 21:37:42.000000 openimis-be-location-1.5.1/location/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:37:57.514262 openimis-be-location-1.5.1/openimis_be_location.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-16 21:37:57.000000 openimis-be-location-1.5.1/openimis_be_location.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-16 21:37:57.000000 openimis-be-location-1.5.1/openimis_be_location.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 21:37:57.000000 openimis-be-location-1.5.1/openimis_be_location.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-16 21:37:57.000000 openimis-be-location-1.5.1/openimis_be_location.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-16 21:37:57.000000 openimis-be-location-1.5.1/openimis_be_location.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 21:37:57.514262 openimis-be-location-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-16 21:37:55.000000 openimis-be-location-1.5.1/setup.py
```

### Comparing `openimis-be-location-1.5.0/LICENSE.md` & `openimis-be-location-1.5.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openimis-be-location-1.5.0/PKG-INFO` & `openimis-be-location-1.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-location
-Version: 1.5.0
+Version: 1.5.1
 Summary: The openIMIS Backend Location reference module.
 Home-page: https://openimis.org/
 Author: Xavier Gillmann
 Author-email: xgillmann@bluesquarehub.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-location-1.5.0/README.md` & `openimis-be-location-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `openimis-be-location-1.5.0/location/apps.py` & `openimis-be-location-1.5.1/location/apps.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     "location_types": ['R', 'D', 'W', 'V'],
     "gql_query_locations_perms": ["121901"],
     "gql_query_health_facilities_perms": ["121101"],
     "gql_mutation_create_locations_perms": ["121902"],
     "gql_mutation_edit_locations_perms": ["121903"],
     "gql_mutation_delete_locations_perms": ["121904"],
     "gql_mutation_move_location_perms": ["121905"],
+    "gql_mutation_create_region_locations_perms": ["121906"],
     "gql_mutation_create_health_facilities_perms": ["121102"],
     "gql_mutation_edit_health_facilities_perms": ["121103"],
     "gql_mutation_delete_health_facilities_perms": ["121104"],
     "health_facility_level": [
         {
             "code": "D",
             "display": "Dispensary",
@@ -33,14 +34,15 @@
 class LocationConfig(AppConfig):
     name = MODULE_NAME
 
     location_types = []
     gql_query_locations_perms = []
     gql_query_health_facilities_perms = []
     gql_mutation_create_locations_perms = []
+    gql_mutation_create_region_locations_perms = []
     gql_mutation_edit_locations_perms = []
     gql_mutation_delete_locations_perms = []
     gql_mutation_move_location_perms = []
     gql_mutation_create_health_facilities_perms = []
     gql_mutation_edit_health_facilities_perms = []
     gql_mutation_delete_health_facilities_perms = []
 
@@ -52,14 +54,17 @@
         LocationConfig.gql_query_locations_perms = cfg[
             "gql_query_locations_perms"]
         LocationConfig.gql_query_health_facilities_perms = cfg[
             "gql_query_health_facilities_perms"]
         LocationConfig.gql_mutation_create_locations_perms = cfg[
             "gql_mutation_create_locations_perms"
         ]
+        LocationConfig.gql_mutation_create_region_locations_perms = cfg[
+            "gql_mutation_create_region_locations_perms"
+        ]
         LocationConfig.gql_mutation_edit_locations_perms = cfg[
             "gql_mutation_edit_locations_perms"
         ]
         LocationConfig.gql_mutation_delete_locations_perms = cfg[
             "gql_mutation_delete_locations_perms"
         ]
         LocationConfig.gql_mutation_move_location_perms = cfg[
```

### Comparing `openimis-be-location-1.5.0/location/dataloaders.py` & `openimis-be-location-1.5.1/location/dataloaders.py`

 * *Files identical despite different names*

### Comparing `openimis-be-location-1.5.0/location/gql_mutations.py` & `openimis-be-location-1.5.1/location/gql_mutations.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from core import assert_string_length, filter_validity
 from core.schema import OpenIMISMutation
 from .models import Location, HealthFacility, UserDistrict
 from django.contrib.auth.models import AnonymousUser
 from django.core.exceptions import ValidationError, PermissionDenied
 from django.utils.translation import gettext as _
 from graphene import InputObjectType
+import copy
 
 from .services import LocationService, HealthFacilityService
 
 
 class LocationCodeInputType(graphene.String):
     @staticmethod
     def coerce_string(value):
@@ -69,14 +70,17 @@
     _mutation_class = "CreateLocationMutation"
 
     class Input(LocationInputType):
         pass
 
     @classmethod
     def async_mutate(cls, user, **data):
+
+        if Location.objects.filter(code=data['code'], type=data['type'], validity_to=None).exists():
+            raise ValidationError("Location with this code already exists.")
         try:
             return cls.do_mutate(LocationConfig.gql_mutation_create_locations_perms, user, **data)
         except Exception as exc:
             return [{
                 'message': _("location.mutation.failed_to_create_location") % {'code': data['code']},
                 'detail': str(exc)}]
 
@@ -87,28 +91,33 @@
 
     class Input(LocationInputType):
         pass
 
     @classmethod
     def async_mutate(cls, user, **data):
         try:
-            return cls.do_mutate(LocationConfig.gql_mutation_edit_locations_perms, user, **data)
+            return cls.do_mutate(
+                LocationConfig.gql_mutation_edit_locations_perms,
+                user,
+                **data
+            )
         except Exception as exc:
             return [{
                 'message': _("location.mutation.failed_to_update_location") % {'code': data['code']},
                 'detail': str(exc)}]
 
 
 def tree_delete(parents, now):
     if parents:
         children = Location.objects \
             .filter(parent__in=parents) \
-            .filter(*filter_validity())
+            # .filter(*filter_validity())
+        org_children = copy.copy(children)
         children.update(validity_to=now)
-        tree_delete(children.all(), now)
+        tree_delete(org_children, now)
 
 
 class DeleteLocationMutation(OpenIMISMutation):
     _mutation_module = "location"
     _mutation_class = "DeleteLocationMutation"
 
     class Input(OpenIMISMutation.Input):
@@ -222,23 +231,23 @@
 
 class HealthFacilityInputType(OpenIMISMutation.Input):
     id = graphene.Int(required=False, read_only=True)
     uuid = graphene.String(required=False)
     code = HealthFacilityCodeInputType(required=True)
     name = graphene.String(required=True)
     acc_code = graphene.String(required=False)
-    legal_form_id = graphene.String(required=False)
-    level = graphene.String(required=False)
+    legal_form_id = graphene.String(required=True)
+    level = graphene.String(required=True)
     sub_level_id = graphene.String(required=False)
-    location_id = graphene.Int(required=False)
+    location_id = graphene.Int(required=True)
     address = graphene.String(required=False)
     phone = graphene.String(required=False)
     fax = graphene.String(required=False)
     email = graphene.String(required=False)
-    care_type = graphene.String(required=False)
+    care_type = graphene.String(required=True)
     services_pricelist_id = graphene.Int(required=False)
     items_pricelist_id = graphene.Int(required=False)
     offline = graphene.Boolean(required=False)
     catchments = graphene.List(HealthFacilityCatchmentInputType, required=False)
 
 
 def update_or_create_health_facility(data, user):
@@ -255,14 +264,17 @@
 
     class Input(HealthFacilityInputType):
         pass
 
     @classmethod
     def async_mutate(cls, user, **data):
         try:
+            if HealthFacilityService.check_unique_code(data.get('code')):
+                raise ValidationError(
+                    _("mutation.hf_code_duplicated"))
             if type(user) is AnonymousUser or not user.id:
                 raise ValidationError(
                     _("mutation.authentication_required"))
             if not user.has_perms(LocationConfig.gql_mutation_create_health_facilities_perms):
                 raise PermissionDenied(_("unauthorized"))
 
             data['audit_user_id'] = user.id_for_audit
@@ -288,14 +300,21 @@
         try:
             if type(user) is AnonymousUser or not user.id:
                 raise ValidationError(
                     _("mutation.authentication_required"))
             if not user.has_perms(LocationConfig.gql_mutation_edit_health_facilities_perms):
                 raise PermissionDenied(_("unauthorized"))
 
+            incoming_HF_code = data['code']
+            current_HF = HealthFacility.objects.get(uuid=data['uuid'])
+            if current_HF.code != incoming_HF_code:
+                if HealthFacilityService.check_unique_code(incoming_HF_code):
+                    raise ValidationError(
+                        _("mutation.hf_code_duplicated"))
+
             data['audit_user_id'] = user.id_for_audit
             from core.utils import TimeUtils
             data['validity_from'] = TimeUtils.now()
             update_or_create_health_facility(data, user)
             return None
         except Exception as exc:
             return [{
```

### Comparing `openimis-be-location-1.5.0/location/gql_queries.py` & `openimis-be-location-1.5.1/location/gql_queries.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,46 @@
 import graphene
 import base64
 from graphene_django import DjangoObjectType
+from django.core.exceptions import PermissionDenied
+from django.utils.translation import gettext as _
 from core import prefix_filterset, filter_validity, ExtendedConnection
+from location.apps import LocationConfig
 from location.models import HealthFacilityLegalForm, Location, HealthFacilitySubLevel, HealthFacilityCatchment, \
     HealthFacility, UserDistrict, OfficerVillage
 
 
 class LocationGQLType(DjangoObjectType):
     client_mutation_id = graphene.String()
 
     def resolve_parent(self, info):
+        if not info.context.user.is_authenticated:
+            raise PermissionDenied(_("unauthorized"))
         if "location_loader" in info.context.dataloaders and self.parent_id:
             return info.context.dataloaders["location_loader"].load(self.parent_id)
         return self.parent
 
     class Meta:
         model = Location
         interfaces = (graphene.relay.Node,)
         filter_fields = {
             "id": ["exact"],
             "uuid": ["exact"],
             "code": ["exact", "istartswith", "icontains", "iexact"],
             "name": ["exact", "istartswith", "icontains", "iexact"],
             "type": ["exact"],
-            "parent__uuid": ["exact"],  # can't import itself!
-            "parent__id": ["exact"],  # can't import itself!
+            "parent__uuid": ["exact", "in"],  # can't import itself!
+            "parent__parent__uuid": ["exact", "in"],  # can't import itself!
+            "parent__parent__parent__uuid": ["exact", "in"],  # can't import itself!
+            "parent__id": ["exact", "in"],  # can't import itself!
         }
 
     def resolve_client_mutation_id(self, info):
+        if not info.context.user.is_authenticated:
+            raise PermissionDenied(_("unauthorized"))
         location_mutation = self.mutations.select_related(
             'mutation').filter(mutation__status=0).first()
         return location_mutation.mutation.client_mutation_id if location_mutation else None
 
     @classmethod
     def get_queryset(cls, queryset, info):
         return Location.get_queryset(queryset, info.context.user)
@@ -70,21 +79,27 @@
             "care_type": ["exact"],
             "legal_form__code": ["exact"],
             **prefix_filterset("location__", LocationGQLType._meta.filter_fields)
         }
         connection_class = ExtendedConnection
 
     def resolve_location(self, info):
+        if not info.context.user.is_authenticated:
+            raise PermissionDenied(_("unauthorized"))
         if "location_loader" in info.context.dataloaders:
             return info.context.dataloaders["location_loader"].load(self.location_id)
 
     def resolve_catchments(self, info):
+        if not info.context.user.has_perms(LocationConfig.gql_query_health_facilities_perms):
+            raise PermissionDenied(_("unauthorized"))
         return self.catchments.filter(validity_to__isnull=True)
 
     def resolve_client_mutation_id(self, info):
+        if not info.context.user.has_perms(LocationConfig.gql_query_health_facilities_perms):
+            raise PermissionDenied(_("unauthorized"))
         health_facility_mutation = self.mutations.select_related(
             'mutation').filter(mutation__status=0).first()
         return health_facility_mutation.mutation.client_mutation_id if health_facility_mutation else None
 
 
 class UserRegionGQLType(graphene.ObjectType):
     id = graphene.String()
```

### Comparing `openimis-be-location-1.5.0/location/migrations/0001_initial.py` & `openimis-be-location-1.5.1/location/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openimis-be-location-1.5.0/location/migrations/0002_location.py` & `openimis-be-location-1.5.1/location/migrations/0002_location.py`

 * *Files identical despite different names*

### Comparing `openimis-be-location-1.5.0/location/migrations/0003_userdistrict.py` & `openimis-be-location-1.5.1/location/migrations/0003_userdistrict.py`

 * *Files identical despite different names*

### Comparing `openimis-be-location-1.5.0/location/migrations/0004_locationmutation.py` & `openimis-be-location-1.5.1/location/migrations/0004_locationmutation.py`

 * *Files identical despite different names*

### Comparing `openimis-be-location-1.5.0/location/migrations/0005_healthfacilitycatchment_healthfacilitylegalform_healthfacilitymutation_healthfacilitysublevel.py` & `openimis-be-location-1.5.1/location/migrations/0005_healthfacilitycatchment_healthfacilitylegalform_healthfacilitymutation_healthfacilitysublevel.py`

 * *Files identical despite different names*

### Comparing `openimis-be-location-1.5.0/location/migrations/0006_users_api.py` & `openimis-be-location-1.5.1/location/migrations/0006_users_api.py`

 * *Files identical despite different names*

### Comparing `openimis-be-location-1.5.0/location/migrations/0007_auto_20211103_1046.py` & `openimis-be-location-1.5.1/location/migrations/0007_auto_20211103_1046.py`

 * *Files identical despite different names*

### Comparing `openimis-be-location-1.5.0/location/migrations/0008_add_enrollment_officer_gql_query_location_right.py` & `openimis-be-location-1.5.1/location/migrations/0008_add_enrollment_officer_gql_query_location_right.py`

 * *Files identical despite different names*

### Comparing `openimis-be-location-1.5.0/location/models.py` & `openimis-be-location-1.5.1/location/models.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,82 +1,83 @@
 from functools import reduce
 import uuid
 
-from core import fields, filter_validity
+from core import filter_validity
 from django.conf import settings
 from django.db import models
 from core import models as core_models
 from graphql import ResolveInfo
 from .apps import LocationConfig
 import logging
+from django.db.models import Q
 
 logger = logging.getLogger(__file__)
 
 
 class LocationManager(models.Manager):
     def parents(self, location_id):
         parents = Location.objects.raw(
-            """
-            WITH CTE_PARENTS AS (
+            f"""
+            WITH {"" if settings.MSSQL else "RECURSIVE"} CTE_PARENTS AS (
             SELECT
-                LocationId,
-                LocationType,
-                ParentLocationId
+                "LocationId",
+                "LocationType",
+                "ParentLocationId"
             FROM
-                tblLocations
-            WHERE LocationId = %s
+                "tblLocations"
+            WHERE "LocationId" = %s
             UNION ALL
 
             SELECT
-                parent.LocationId,
-                parent.LocationType,
-                parent.ParentLocationId
+                parent."LocationId",
+                parent."LocationType",
+                parent."ParentLocationId"
             FROM
-                tblLocations parent
+                "tblLocations" parent
                 INNER JOIN CTE_PARENTS leaf
-                    ON parent.LocationId = leaf.ParentLocationId
+                    ON parent."LocationId" = leaf."ParentLocationId"
             )
             SELECT * FROM CTE_PARENTS;
         """,
             (location_id,),
         )
         return self.filter(id__in=[x.id for x in parents])
 
     def children(self, location_id):
         children = Location.objects.raw(
-            """
-            WITH CTE_CHILDREN AS (
-            SELECT
-                LocationId,
-                LocationType,
-                ParentLocationId,
-                0 as Level
-            FROM
-                tblLocations
-            WHERE ParentLocationId = %s
-            UNION ALL
-
-            SELECT
-                child.LocationId,
-                child.LocationType,
-                child.ParentLocationId,
-                parent.Level + 1
-            FROM
-                tblLocations child
-                INNER JOIN CTE_CHILDREN parent
-                    ON child.ParentLocationId = parent.LocationId
-            )
-            SELECT * FROM CTE_CHILDREN;
-        """,
+            f"""
+                WITH {"" if settings.MSSQL else "RECURSIVE"} CTE_CHILDREN AS (
+                SELECT
+                    "LocationId",
+                    "LocationType",
+                    "ParentLocationId",
+                    0 as "Level"
+                FROM
+                    "tblLocations"
+                WHERE "ParentLocationId" = %s
+                UNION ALL
+
+                SELECT
+                    child."LocationId",
+                    child."LocationType",
+                    child."ParentLocationId",
+                    parent."Level" + 1
+                FROM
+                    "tblLocations" child
+                    INNER JOIN CTE_CHILDREN parent
+                        ON child."ParentLocationId" = parent."LocationId"
+                )
+                SELECT * FROM CTE_CHILDREN;
+            """,
             (location_id,),
         )
         return self.filter(id__in=[x.id for x in children])
 
 
-class Location(core_models.VersionedModel):
+class Location(core_models.VersionedModel, core_models.ExtendableModel):
     objects = LocationManager()
 
     id = models.AutoField(db_column='LocationId', primary_key=True)
     uuid = models.CharField(db_column='LocationUUID',
                             max_length=36, default=uuid.uuid4, unique=True)
     code = models.CharField(db_column='LocationCode',
                             max_length=8, blank=True, null=True)
@@ -108,55 +109,77 @@
         if isinstance(user, ResolveInfo):
             user = user.context.user
         if settings.ROW_SECURITY and user.is_anonymous:
             return queryset.filter(id=-1)
 
         # OMT-280: if you create a new region and your user has district limitations, you won't find what you
         # just created. So we'll consider that if you were allowed to create it, you are also allowed to retrieve it.
-        if settings.ROW_SECURITY and not user.has_perms(LocationConfig.gql_mutation_create_locations_perms):
-            dists = UserDistrict.get_user_districts(user._u)
-            regs = set([d.location.parent.id for d in dists])
-            dists = set([d.location.id for d in dists])
-            filters = []
-            prev = "id"
-            for i, tpe in enumerate(LocationConfig.location_types):
-                loc_ids = dists if i else regs
-                filters += [models.Q(type__exact=tpe) & models.Q(**{"%s__in" % prev: loc_ids})]
-                prev = "parent__" + prev if i > 1 else "parent_" + prev if i else prev
-            return queryset.filter(reduce((lambda x, y: x | y), filters))
+        if settings.ROW_SECURITY \
+                and not user.has_perms(LocationConfig.gql_mutation_create_region_locations_perms) \
+                and not user.is_superuser:
+            if user.is_officer:
+                from core.models import Officer
+                return Officer.objects \
+                    .filter(code=user.username, has_login=True, validity_to__isnull=True) \
+                    .get().officer_allowed_locations
+            elif user.is_claim_admin:
+                from claim.models import ClaimAdmin
+                return ClaimAdmin.objects \
+                    .filter(code=user.username, has_login=True, validity_to__isnull=True) \
+                    .get().officer_allowed_locations
+            else:
+                dists = UserDistrict.get_user_districts(user._u)
+                regs = set([d.location.parent.id for d in dists])
+                dists = set([d.location.id for d in dists])
+                filters = []
+                prev = "id"
+                for i, tpe in enumerate(LocationConfig.location_types):
+                    loc_ids = dists if i else regs
+                    filters += [models.Q(type__exact=tpe) & models.Q(**{"%s__in" % prev: loc_ids})]
+                    prev = "parent__" + prev if i > 1 else "parent_" + prev if i else prev
+                return queryset.filter(reduce((lambda x, y: x | y), filters))
         return queryset
 
+    @staticmethod
+    def build_user_location_filter_query(user: core_models.InteractiveUser) -> Q:
+        user_districts = UserDistrict.get_user_districts(user)
+
+        return Q(location__in=Location.objects.filter(uuid__in=user_districts.values_list('location__uuid', flat=True))) | Q(
+            location__in=Location.objects.filter(uuid__in=user_districts.values_list('location__parent__uuid', flat=True))) | Q(
+            location__isnull=True
+        )
+
     class Meta:
-        managed = False
+        managed = True
         db_table = 'tblLocations'
 
 
 class HealthFacilityLegalForm(models.Model):
     code = models.CharField(db_column='LegalFormCode', primary_key=True, max_length=1)
     legal_form = models.CharField(db_column='LegalForms', max_length=50)
     sort_order = models.IntegerField(db_column='SortOrder', blank=True, null=True)
     alt_language = models.CharField(db_column='AltLanguage', max_length=50, blank=True, null=True)
 
     class Meta:
-        managed = False
+        managed = True
         db_table = 'tblLegalForms'
 
 
 class HealthFacilitySubLevel(models.Model):
     code = models.CharField(db_column='HFSublevel', primary_key=True, max_length=1)
     health_facility_sub_level = models.CharField(db_column='HFSublevelDesc', max_length=50, blank=True, null=True)
     sort_order = models.IntegerField(db_column='SortOrder', blank=True, null=True)
     alt_language = models.CharField(db_column='AltLanguage', max_length=50, blank=True, null=True)
 
     class Meta:
-        managed = False
+        managed = True
         db_table = 'tblHFSublevel'
 
 
-class HealthFacility(core_models.VersionedModel):
+class HealthFacility(core_models.VersionedModel, core_models.ExtendableModel):
     id = models.AutoField(db_column='HfID', primary_key=True)
     uuid = models.CharField(
         db_column='HfUUID', max_length=36, default=uuid.uuid4, unique=True)
 
     code = models.CharField(db_column='HFCode', max_length=8)
     name = models.CharField(db_column='HFName', max_length=100)
     acc_code = models.CharField(
@@ -184,15 +207,15 @@
     care_type = models.CharField(db_column='HFCareType', max_length=1)
 
     services_pricelist = models.ForeignKey('medical_pricelist.ServicesPricelist', models.DO_NOTHING,
                                            db_column='PLServiceID', blank=True, null=True,
                                            related_name="health_facilities")
     items_pricelist = models.ForeignKey('medical_pricelist.ItemsPricelist', models.DO_NOTHING, db_column='PLItemID',
                                         blank=True, null=True, related_name="health_facilities")
-    offline = models.BooleanField(db_column='OffLine')
+    offline = models.BooleanField(db_column='OffLine', default=False)
     # row_id = models.BinaryField(db_column='RowID', blank=True, null=True)
     audit_user_id = models.IntegerField(db_column='AuditUserID')
 
     def __str__(self):
         return self.code + " " + self.name
 
     @classmethod
@@ -204,21 +227,22 @@
             queryset = HealthFacility.objects
         else:
             queryset = cls.filter_queryset(queryset)
         if settings.ROW_SECURITY and user.is_anonymous:
             return queryset.filter(id=-1)
         if settings.ROW_SECURITY:
             dist = UserDistrict.get_user_districts(user._u)
-            return queryset.filter(
-                location_id__in=[l.location_id for l in dist]
-            )
+            if dist:
+                return queryset.filter(
+                    location_id__in=[l.location_id for l in dist]
+                )
         return queryset
 
     class Meta:
-        managed = False
+        managed = True
         db_table = 'tblHF'
 
     LEVEL_HEALTH_CENTER = 'C'
     LEVEL_DISPENSARY = 'D'
     LEVEL_HOSPITAL = 'H'
 
     CARE_TYPE_IN_PATIENT = 'I'
@@ -244,49 +268,65 @@
     catchment = models.IntegerField(db_column='Catchment', blank=True, null=True)
     validity_from = models.DateTimeField(db_column='ValidityFrom', blank=True, null=True)
     validity_to = models.DateTimeField(db_column='ValidityTo', blank=True, null=True)
 
     audit_user_id = models.IntegerField(db_column='AuditUserId', blank=True, null=True)
 
     class Meta:
-        managed = False
+        managed = True
         db_table = 'tblHFCatchment'
 
 
 class UserDistrict(core_models.VersionedModel):
     id = models.AutoField(db_column="UserDistrictID", primary_key=True)
     user = models.ForeignKey(
         core_models.InteractiveUser, models.DO_NOTHING, db_column="UserID"
     )
     location = models.ForeignKey(Location, models.DO_NOTHING, db_column="LocationId")
     audit_user_id = models.IntegerField(db_column="AuditUserID")
 
     class Meta:
-        managed = False
+        managed = True
         db_table = 'tblUsersDistricts'
 
     @classmethod
     def get_user_districts(cls, user):
         """
         Retrieve the list of UserDistricts for a user, the locations are prefetched on two levels.
         :param user: InteractiveUser to filter on
         :return: UserDistrict *objects*
         """
+        if user.is_superuser is True:
+            return (
+                UserDistrict.objects
+                .filter(*filter_validity())
+                .filter(location__type='D')
+            )
         if not isinstance(user, core_models.InteractiveUser):
             if isinstance(user, core_models.TechnicalUser):
                 logger.warning(f"get_user_districts called with a technical user `{user.username}`. "
                                "We'll return an empty list, but it should be handled before reaching here.")
             return UserDistrict.objects.none()
         return (
-            UserDistrict.objects.select_related("location")
-            .only("location__id", "location__parent__id")
-            .select_related("location__parent")
+            UserDistrict.objects.filter(location__type='D')
+            .filter(location__validity_to__isnull=True)
+            .select_related("location")
+            .only(
+                "location__id",
+                "location__uuid",
+                "location__code",
+                "location__name",
+                "location__type",
+                "location__parent_id",
+                "location__parent__code",
+            )
+            .prefetch_related("location__parent")
             .filter(user=user)
             .filter(*filter_validity())
-            .order_by("location__parent_code")
+            .order_by("location__parent__code")
             .order_by("location__code")
             .exclude(location__parent__isnull=True)
         )
 
     @classmethod
     def get_user_locations(cls, user):
         """
@@ -325,15 +365,15 @@
         models.CASCADE,
         db_column="LocationId",
         related_name="officer_villages",
     )
     audit_user_id = models.IntegerField(db_column="AuditUserID")
 
     class Meta:
-        managed = False
+        managed = True
         db_table = 'tblOfficerVillages'
 
     @classmethod
     def get_queryset(cls, queryset, user):
         if isinstance(user, ResolveInfo):
             user = user.context.user
         if settings.ROW_SECURITY and user.is_anonymous:
```

### Comparing `openimis-be-location-1.5.0/location/schema.py` & `openimis-be-location-1.5.1/location/schema.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,107 +1,146 @@
 import graphene_django_optimizer as gql_optimizer
 
-from core.models import Officer
+from core.models import Officer, InteractiveUser
 from core.schema import OrderedDjangoFilterConnectionField
 from core.schema import signal_mutation_module_validate
 from django.db.models import Q
 from django.utils.translation import gettext as _
 from graphene_django.filter import DjangoFilterConnectionField
 
 from .gql_mutations import *
 from .gql_queries import *
 from .models import *
+from .services import LocationService
 
 
 class Query(graphene.ObjectType):
     health_facilities = OrderedDjangoFilterConnectionField(
         HealthFacilityGQLType,
         showHistory=graphene.Boolean(),
         orderBy=graphene.List(of_type=graphene.String)
     )
-    locations = DjangoFilterConnectionField(LocationGQLType)
+    locations = OrderedDjangoFilterConnectionField(
+        LocationGQLType,
+        orderBy=graphene.List(of_type=graphene.String),
+    )
     locations_str = DjangoFilterConnectionField(
         LocationGQLType,
         str=graphene.String(),
     )
     user_districts = graphene.List(
         UserDistrictGQLType
     )
+    officer_locations = graphene.List(LocationGQLType,
+                                      officer_code=graphene.String(required=True),
+                                      location_type=graphene.String(required=False),
+                                      description="Returns list of locations assigned to a given enrolment officer.")
     health_facilities_str = DjangoFilterConnectionField(
         HealthFacilityGQLType,
         str=graphene.String(),
         region_uuid=graphene.String(),
         district_uuid=graphene.String(),
         districts_uuids=graphene.List(of_type=graphene.String),
     )
+    validate_location_code = graphene.Field(
+        graphene.Boolean,
+        location_code=graphene.String(required=True),
+        description="Checks that the specified location code is unique."
+    )
+    validate_health_facility_code = graphene.Field(
+        graphene.Boolean,
+        health_facility_code=graphene.String(required=True),
+        description="Checks that the specified health facility code is unique."
+    )
 
     def resolve_health_facilities(self, info, **kwargs):
         show_history = kwargs.get('showHistory', False) and info.context.user.has_perms(
             LocationConfig.gql_query_health_facilities_perms)
         # OMT-281 allow anyone to query, limited by the get_queryset
         # if not info.context.user.has_perms(LocationConfig.gql_query_health_facilities_perms):
         if info.context.user.is_anonymous:
             raise PermissionDenied(_("unauthorized"))
         query = HealthFacility.get_queryset(None, info.context.user, **kwargs)
         if not show_history:
             query = HealthFacility.filter_queryset(query)
+
+        query = query.filter(Location.build_user_location_filter_query(info.context.user._u))
+
         return gql_optimizer.query(query.all(), info)
 
+    def resolve_validate_location_code(self, info, **kwargs):
+        if not info.context.user.has_perms(LocationConfig.gql_query_locations_perms):
+            raise PermissionDenied(_("unauthorized"))
+        errors = LocationService.check_unique_code(code=kwargs['location_code'])
+        return False if errors else True
+
+    def resolve_validate_health_facility_code(self, info, **kwargs):
+        if not info.context.user.has_perms(LocationConfig.gql_query_health_facilities_perms):
+            raise PermissionDenied(_("unauthorized"))
+        errors = HealthFacilityService.check_unique_code(code=kwargs['health_facility_code'])
+        return False if errors else True
+
     def resolve_locations(self, info, **kwargs):
         # OMT-281 allow querying to anyone, with limitations in the get_queryset
         # if not info.context.user.has_perms(LocationConfig.gql_query_locations_perms):
         if info.context.user.is_anonymous:
             raise PermissionDenied(_("unauthorized"))
 
     def resolve_locations_str(self, info, **kwargs):
-        if not info.context.user.has_perms(LocationConfig.gql_query_locations_perms):
+        if info.context.user.is_anonymous:
             raise PermissionDenied(_("unauthorized"))
+
+        queryset = Location.get_queryset(None, info.context.user)
         filters = [*filter_validity(**kwargs)]
+
         str = kwargs.get('str')
         if str is not None:
             filters += [Q(code__icontains=str) | Q(name__icontains=str)]
 
-        locations = Location.objects.filter(*filters)
-        #return locations
-        if info.context.user.is_officer:
-            officer = Officer.objects\
-                .filter(code=info.context.user.username, has_login=True, validity_to__isnull=True).get()
-            locations = locations.filter(uuid__in=officer.officer_allowed_locations)
-        return locations
+        return queryset.filter(*filters)
 
     def resolve_health_facilities_str(self, info, **kwargs):
-        if not info.context.user.has_perms(LocationConfig.gql_query_locations_perms):
+        if not info.context.user.is_authenticated:
             raise PermissionDenied(_("unauthorized"))
         filters = [*filter_validity(**kwargs)]
-        str = kwargs.get('str')
-        if str is not None:
-            filters += [Q(code__icontains=str) | Q(name__icontains=str)]
+        search = kwargs.get('str')
         district_uuid = kwargs.get('district_uuid')
         district_uuids = kwargs.get('districts_uuids')
+        region_uuid = kwargs.get('region_uuid')
+        if search is not None:
+            filters += [Q(code__icontains=search) | Q(name__icontains=search)]
         if district_uuid is not None:
             filters += [Q(location__uuid=district_uuid)]
         if district_uuids is not None:
-            filters += [Q(location__uuid__in=district_uuids)]
-
-        region_uuid = kwargs.get('region_uuid')
+            if None not in district_uuids:
+                filters += [Q(location__uuid__in=district_uuids)]
         if region_uuid is not None:
             filters += [Q(location__parent__uuid=region_uuid)]
-        dist = UserDistrict.get_user_districts(info.context.user._u)
-        filters += [Q(location__id__in=[l.location_id for l in dist])]
+        if settings.ROW_SECURITY:
+            dist = UserDistrict.get_user_districts(info.context.user._u)
+            filters += [Q(location__id__in=[l.location_id for l in dist])]
         return HealthFacility.objects.filter(*filters)
 
     def resolve_user_districts(self, info, **kwargs):
         if info.context.user.is_anonymous:
             raise NotImplementedError(
                 'Anonymous Users are not registered for districts')
         if not isinstance(info.context.user._u, core_models.InteractiveUser):
             raise NotImplementedError(
                 'Only Interactive Users are registered for districts')
         return [UserDistrictGQLType(d) for d in UserDistrict.get_user_districts(info.context.user._u)]
 
+    def resolve_officer_locations(self, info, **kwargs):
+        if not info.context.user.has_perms(LocationConfig.gql_query_locations_perms):
+            raise PermissionDenied(_("unauthorized"))
+        current_officer = Officer.objects.get(code=kwargs['officer_code'], validity_to__isnull=True)
+        if 'location_type' in kwargs:
+            return current_officer.officer_allowed_locations.filter(type=kwargs['location_type'])
+        return current_officer.officer_allowed_locations
+
 
 class Mutation(graphene.ObjectType):
     create_location = CreateLocationMutation.Field()
     update_location = UpdateLocationMutation.Field()
     delete_location = DeleteLocationMutation.Field()
     move_location = MoveLocationMutation.Field()
     create_health_facility = CreateHealthFacilityMutation.Field()
```

### Comparing `openimis-be-location-1.5.0/location/services.py` & `openimis-be-location-1.5.1/location/services.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import datetime
 import json
 
 from django.contrib.auth.models import AnonymousUser
+from django.core.exceptions import PermissionDenied, ValidationError
 from django.core.serializers.json import DjangoJSONEncoder
+from django.utils.translation import gettext as _
 
 from core.signals import register_service_signal
 from location.apps import LocationConfig
 from location.models import Location, HealthFacility, HealthFacilityCatchment, UserDistrict
 
 
 def check_authentication(function):
@@ -42,31 +44,72 @@
     }
 
 
 class LocationService:
     def __init__(self, user):
         self.user = user
 
+    @staticmethod
+    def check_unique_code(code):
+        if Location.objects.filter(code=code, validity_to__isnull=True).exists():
+            return [{"message": "Location code %s already exists" % code}]
+        return []
+
+    def validate_data(self, **data):
+        error = None
+        error = self.check_unique_code(data["code"])
+
+        return error
+
     @register_service_signal('location_service.update_or_create')
     def update_or_create(self, data):
         location_uuid = data.pop('uuid') if 'uuid' in data else None
         parent_uuid = data.pop('parent_uuid') if 'parent_uuid' in data else None
+        incoming_code = data.get('code')
+        current_location = Location.objects.filter(uuid=location_uuid).first()
+        current_code = current_location.code if current_location else None
+        if current_code != incoming_code:
+            if self.check_unique_code(incoming_code):
+                raise ValidationError(_("mutation.location_code_duplicated"))
         # update_or_create(uuid=location_uuid, ...)
         # doesn't work because of explicit attempt to set null to uuid!
+        self._check_users_locations_rights(data['type'])
         if location_uuid:
             location = Location.objects.get(uuid=location_uuid)
             self._reset_location_before_update(location)
             [setattr(location, key, data[key]) for key in data]
         else:
-            location = Location.objects.create(**data)
+            error = self.validate_data(**data)
+            if error:
+                raise ValueError(error)
+            else:
+                location = Location.objects.create(**data)
+
         if parent_uuid:
             location.parent = Location.objects.get(uuid=parent_uuid)
         location.save()
         self._ensure_user_belongs_to_district(location)
 
+    def _check_users_locations_rights(self, loc_type):
+        if self.user.is_superuser \
+            or self.user.has_perms(
+                    LocationConfig.gql_mutation_create_region_locations_perms
+                ):
+            pass
+        elif loc_type in ['R', 'D']:
+            raise PermissionDenied(_(
+                "unauthorized to create or update region and district"
+            ))
+        elif not self.user.has_perms(
+                LocationConfig.gql_mutation_create_locations_perms
+        ):
+            raise PermissionDenied(_(
+                "unauthorized to create or update municipalities and villages"
+            ))
+
     @staticmethod
     def _reset_location_before_update(location):
         location.male_population = None
         location.female_population = None
         location.other_population = None
         location.families = None
 
@@ -79,32 +122,38 @@
             )
 
 
 class HealthFacilityService:
     def __init__(self, user):
         self.user = user
 
+    @staticmethod
+    def check_unique_code(code):
+        if HealthFacility.objects.filter(code=code, validity_to__isnull=True).exists():
+            return [{"message": "Health facility code %s already exists" % code}]
+        return []
+
     @register_service_signal('health_facility_service.update_or_create')
     def update_or_create(self, data):
         hf_uuid = data.pop('uuid') if 'uuid' in data else None
         catchments = data.pop('catchments') if 'catchments' in data else []
         # address may be multiline > sent as JSON
         # update_or_create(uuid=location_uuid, ...)
         # doesn't work because of explicit attempt to set null to uuid!
         prev_hf_id = None
         if hf_uuid:
             hf = HealthFacility.objects.get(uuid=hf_uuid)
+            if hf.validity_to:
+                raise ValidationError(_("Cannot update historical hf."))
             prev_hf_id = hf.save_history()
             # reset the non required fields
             # (each update is 'complete', necessary to be able to set 'null')
             self._reset_health_facility_before_update(hf)
             [setattr(hf, key, data[key]) for key in data]
         else:
-            # UI don't foresee a field for offline > set via API (and mobile 'world' ?
-            data['offline'] = False
             hf = HealthFacility.objects.create(**data)
         self._process_catchments(catchments, prev_hf_id, hf.id, hf.catchments)
         hf.save()
         return hf
 
     def _process_catchments(self, data_catchments, prev_hf_id, hf_id, catchments):
         prev_catchments = [c.id for c in catchments.all()]
```

### Comparing `openimis-be-location-1.5.0/location/test_helpers.py` & `openimis-be-location-1.5.1/location/test_helpers.py`

 * *Files identical despite different names*

### Comparing `openimis-be-location-1.5.0/openimis_be_location.egg-info/PKG-INFO` & `openimis-be-location-1.5.1/openimis_be_location.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-location
-Version: 1.5.0
+Version: 1.5.1
 Summary: The openIMIS Backend Location reference module.
 Home-page: https://openimis.org/
 Author: Xavier Gillmann
 Author-email: xgillmann@bluesquarehub.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-location-1.5.0/openimis_be_location.egg-info/SOURCES.txt` & `openimis-be-location-1.5.1/openimis_be_location.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -20,13 +20,20 @@
 location/migrations/0002_location.py
 location/migrations/0003_userdistrict.py
 location/migrations/0004_locationmutation.py
 location/migrations/0005_healthfacilitycatchment_healthfacilitylegalform_healthfacilitymutation_healthfacilitysublevel.py
 location/migrations/0006_users_api.py
 location/migrations/0007_auto_20211103_1046.py
 location/migrations/0008_add_enrollment_officer_gql_query_location_right.py
+location/migrations/0009_add_location_read_right.py
+location/migrations/0010_insert_create_region_location_perms.py
+location/migrations/0011_auto_20230317_0924.py
+location/migrations/0012_auto_20230317_0927.py
+location/migrations/0013_auto_20230317_1534.py
+location/migrations/0014_add_missing_fields_to_django_scheme.py
+location/migrations/0015_set_managed_to_true.py
 location/migrations/__init__.py
 openimis_be_location.egg-info/PKG-INFO
 openimis_be_location.egg-info/SOURCES.txt
 openimis_be_location.egg-info/dependency_links.txt
 openimis_be_location.egg-info/requires.txt
 openimis_be_location.egg-info/top_level.txt
```

### Comparing `openimis-be-location-1.5.0/setup.py` & `openimis-be-location-1.5.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='openimis-be-location',
-    version='1.5.0',
+    version='v1.5.1',
     packages=find_packages(),
     include_package_data=True,
     license='GNU AGPL v3',
     description='The openIMIS Backend Location reference module.',
     # long_description=README,
     url='https://openimis.org/',
     author='Xavier Gillmann',
```

