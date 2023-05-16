# Comparing `tmp/openimis-be-payer-1.4.1.tar.gz` & `tmp/openimis-be-payer-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis-be-payer-1.4.1.tar", last modified: Thu Nov 10 18:09:46 2022, max compression
+gzip compressed data, was "openimis-be-payer-1.4.2.tar", last modified: Tue May 16 21:38:20 2023, max compression
```

## Comparing `openimis-be-payer-1.4.1.tar` & `openimis-be-payer-1.4.2.tar`

### file list

```diff
@@ -1,28 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 18:09:46.767188 openimis-be-payer-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1852 2022-11-10 18:09:38.000000 openimis-be-payer-1.4.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-11-10 18:09:38.000000 openimis-be-payer-1.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      684 2022-11-10 18:09:46.767188 openimis-be-payer-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1200 2022-11-10 18:09:38.000000 openimis-be-payer-1.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 18:09:46.767188 openimis-be-payer-1.4.1/openimis_be_payer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      684 2022-11-10 18:09:46.000000 openimis-be-payer-1.4.1/openimis_be_payer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      496 2022-11-10 18:09:46.000000 openimis-be-payer-1.4.1/openimis_be_payer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-10 18:09:46.000000 openimis-be-payer-1.4.1/openimis_be_payer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-11-10 18:09:46.000000 openimis-be-payer-1.4.1/openimis_be_payer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-11-10 18:09:46.000000 openimis-be-payer-1.4.1/openimis_be_payer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 18:09:46.767188 openimis-be-payer-1.4.1/payer/
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-11-10 18:09:38.000000 openimis-be-payer-1.4.1/payer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-11-10 18:09:38.000000 openimis-be-payer-1.4.1/payer/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)     1103 2022-11-10 18:09:38.000000 openimis-be-payer-1.4.1/payer/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)     6676 2022-11-10 18:09:38.000000 openimis-be-payer-1.4.1/payer/gql_mutations.py
--rw-r--r--   0 runner    (1001) docker     (121)     2326 2022-11-10 18:09:38.000000 openimis-be-payer-1.4.1/payer/gql_queries.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 18:09:46.767188 openimis-be-payer-1.4.1/payer/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     3210 2022-11-10 18:09:38.000000 openimis-be-payer-1.4.1/payer/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-10 18:09:38.000000 openimis-be-payer-1.4.1/payer/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3081 2022-11-10 18:09:38.000000 openimis-be-payer-1.4.1/payer/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     2045 2022-11-10 18:09:38.000000 openimis-be-payer-1.4.1/payer/schema.py
--rw-r--r--   0 runner    (1001) docker     (121)      529 2022-11-10 18:09:38.000000 openimis-be-payer-1.4.1/payer/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-11-10 18:09:38.000000 openimis-be-payer-1.4.1/payer/tests.py
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-11-10 18:09:38.000000 openimis-be-payer-1.4.1/payer/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-11-10 18:09:38.000000 openimis-be-payer-1.4.1/payer/views.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-10 18:09:46.767188 openimis-be-payer-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-11-10 18:09:46.000000 openimis-be-payer-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:20.094083 openimis-be-payer-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-16 21:38:03.000000 openimis-be-payer-1.4.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-16 21:38:03.000000 openimis-be-payer-1.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-16 21:38:20.094083 openimis-be-payer-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-16 21:38:03.000000 openimis-be-payer-1.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:20.094083 openimis-be-payer-1.4.2/openimis_be_payer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-16 21:38:20.000000 openimis-be-payer-1.4.2/openimis_be_payer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-16 21:38:20.000000 openimis-be-payer-1.4.2/openimis_be_payer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 21:38:20.000000 openimis-be-payer-1.4.2/openimis_be_payer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-16 21:38:20.000000 openimis-be-payer-1.4.2/openimis_be_payer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-16 21:38:20.000000 openimis-be-payer-1.4.2/openimis_be_payer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:20.094083 openimis-be-payer-1.4.2/payer/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-16 21:38:03.000000 openimis-be-payer-1.4.2/payer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-16 21:38:03.000000 openimis-be-payer-1.4.2/payer/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-16 21:38:03.000000 openimis-be-payer-1.4.2/payer/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-05-16 21:38:03.000000 openimis-be-payer-1.4.2/payer/gql_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-05-16 21:38:03.000000 openimis-be-payer-1.4.2/payer/gql_queries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:20.094083 openimis-be-payer-1.4.2/payer/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-05-16 21:38:03.000000 openimis-be-payer-1.4.2/payer/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-16 21:38:03.000000 openimis-be-payer-1.4.2/payer/migrations/0002_add_missing_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-16 21:38:03.000000 openimis-be-payer-1.4.2/payer/migrations/0003_set_managed_to_true.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:03.000000 openimis-be-payer-1.4.2/payer/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-05-16 21:38:03.000000 openimis-be-payer-1.4.2/payer/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-16 21:38:03.000000 openimis-be-payer-1.4.2/payer/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-16 21:38:03.000000 openimis-be-payer-1.4.2/payer/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-16 21:38:03.000000 openimis-be-payer-1.4.2/payer/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-16 21:38:03.000000 openimis-be-payer-1.4.2/payer/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-16 21:38:03.000000 openimis-be-payer-1.4.2/payer/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 21:38:20.094083 openimis-be-payer-1.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-16 21:38:18.000000 openimis-be-payer-1.4.2/setup.py
```

### Comparing `openimis-be-payer-1.4.1/LICENSE.md` & `openimis-be-payer-1.4.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openimis-be-payer-1.4.1/PKG-INFO` & `openimis-be-payer-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-payer
-Version: 1.4.1
+Version: 1.4.2
 Summary: The openIMIS Backend Payer reference module.
 Home-page: https://openimis.org/
 Author: Xavier Gillmann
 Author-email: xgillmann@bluesquarehub.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-payer-1.4.1/README.md` & `openimis-be-payer-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `openimis-be-payer-1.4.1/openimis_be_payer.egg-info/PKG-INFO` & `openimis-be-payer-1.4.2/openimis_be_payer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-payer
-Version: 1.4.1
+Version: 1.4.2
 Summary: The openIMIS Backend Payer reference module.
 Home-page: https://openimis.org/
 Author: Xavier Gillmann
 Author-email: xgillmann@bluesquarehub.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-payer-1.4.1/payer/apps.py` & `openimis-be-payer-1.4.2/payer/apps.py`

 * *Files identical despite different names*

### Comparing `openimis-be-payer-1.4.1/payer/gql_mutations.py` & `openimis-be-payer-1.4.2/payer/gql_mutations.py`

 * *Files identical despite different names*

### Comparing `openimis-be-payer-1.4.1/payer/migrations/0001_initial.py` & `openimis-be-payer-1.4.2/payer/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openimis-be-payer-1.4.1/payer/models.py` & `openimis-be-payer-1.4.2/payer/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     payer_type = models.CharField(db_column="PayerType", max_length=50)
     alt_language = models.CharField(
         db_column="AltLanguage", max_length=50, blank=True, null=True
     )
     sort_order = models.IntegerField(db_column="SortOrder", blank=True, null=True)
 
     class Meta:
-        managed = False
+        managed = True
         db_table = "tblPayerType"
 
 
 class Payer(core_models.VersionedModel):
     PAYER_TYPE_COOP = "C"
     PAYER_TYPE_DONOR = "D"
     PAYER_TYPE_GOV = "G"
@@ -72,15 +72,15 @@
             )
             flat_locations = itertools.chain(*districts)
             queryset = Payer.objects.filter(location__id__in=flat_locations)
 
         return queryset
 
     class Meta:
-        managed = False
+        managed = True
         db_table = "tblPayer"
 
 
 class PayerMutation(core_models.UUIDModel, core_models.ObjectMutation):
     payer = models.ForeignKey(Payer, models.DO_NOTHING, related_name="+")
     mutation = models.ForeignKey(
         core_models.MutationLog, models.DO_NOTHING, related_name="payers"
```

### Comparing `openimis-be-payer-1.4.1/payer/schema.py` & `openimis-be-payer-1.4.2/payer/schema.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from django.core.exceptions import PermissionDenied
 import graphene_django_optimizer as gql_optimizer
 from core import filter_validity
 from django.utils.translation import gettext as _, gettext_lazy
 from payer.apps import PayerConfig
 from core.schema import OrderedDjangoFilterConnectionField
 from .models import Payer
+from location.models import Location
 
 from .gql_queries import PayerGQLType
 
 from .gql_mutations import (
     CreatePayerMutation,
     UpdatePayerMutation,
     DeletePayerMutation,
@@ -34,28 +35,32 @@
             raise PermissionDenied(_("unauthorized"))
 
         return Payer.objects.get(uuid=uuid)
 
     def resolve_payers(self, info, **kwargs):
         if not info.context.user.has_perms(PayerConfig.gql_query_payers_perms):
             raise PermissionDenied(_("unauthorized"))
-        filters = []
+
+        filters = Payer.objects
         show_history = kwargs.get("show_history", False)
         if not show_history:
-            filters += filter_validity(**kwargs)
+            filters = filters.filter(*filter_validity(**kwargs))
 
         search = kwargs.get("search", None)
         if search is not None:
-            filters.append(
+            filters = filters.filter(
                 Q(name__icontains=search)
                 | Q(phone__icontains=search)
                 | Q(email__icontains=search)
             )
 
-        return gql_optimizer.query(Payer.objects.filter(*filters), info)
+        filters = filters.filter(
+            Location.build_user_location_filter_query(info.context.user._u))
+
+        return gql_optimizer.query(filters, info)
 
 
 class Mutation(graphene.ObjectType):
     create_payer = CreatePayerMutation.Field()
     update_payer = UpdatePayerMutation.Field()
     delete_payer = DeletePayerMutation.Field()
     add_funding = AddFundingMutation.Field()
```

### Comparing `openimis-be-payer-1.4.1/payer/test_helpers.py` & `openimis-be-payer-1.4.2/payer/test_helpers.py`

 * *Files identical despite different names*

### Comparing `openimis-be-payer-1.4.1/setup.py` & `openimis-be-payer-1.4.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='openimis-be-payer',
-    version='1.4.1',
+    version='v1.4.2',
     packages=find_packages(),
     include_package_data=True,
     license='GNU AGPL v3',
     description='The openIMIS Backend Payer reference module.',
     # long_description=README,
     url='https://openimis.org/',
     author='Xavier Gillmann',
```

