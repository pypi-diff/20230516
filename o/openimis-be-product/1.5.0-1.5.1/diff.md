# Comparing `tmp/openimis-be-product-1.5.0.tar.gz` & `tmp/openimis-be-product-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis-be-product-1.5.0.tar", last modified: Thu Nov 10 18:09:28 2022, max compression
+gzip compressed data, was "openimis-be-product-1.5.1.tar", last modified: Tue May 16 21:38:14 2023, max compression
```

## Comparing `openimis-be-product-1.5.0.tar` & `openimis-be-product-1.5.1.tar`

### file list

```diff
@@ -1,31 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 18:09:28.061656 openimis-be-product-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1852 2022-11-10 18:09:19.000000 openimis-be-product-1.5.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-11-10 18:09:19.000000 openimis-be-product-1.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      688 2022-11-10 18:09:28.061656 openimis-be-product-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1408 2022-11-10 18:09:19.000000 openimis-be-product-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 18:09:28.061656 openimis-be-product-1.5.0/openimis_be_product.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      688 2022-11-10 18:09:28.000000 openimis-be-product-1.5.0/openimis_be_product.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      670 2022-11-10 18:09:28.000000 openimis-be-product-1.5.0/openimis_be_product.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-10 18:09:28.000000 openimis-be-product-1.5.0/openimis_be_product.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-11-10 18:09:28.000000 openimis-be-product-1.5.0/openimis_be_product.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-11-10 18:09:28.000000 openimis-be-product-1.5.0/openimis_be_product.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 18:09:28.061656 openimis-be-product-1.5.0/product/
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-11-10 18:09:19.000000 openimis-be-product-1.5.0/product/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-11-10 18:09:19.000000 openimis-be-product-1.5.0/product/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)     1557 2022-11-10 18:09:19.000000 openimis-be-product-1.5.0/product/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)      365 2022-11-10 18:09:19.000000 openimis-be-product-1.5.0/product/dataloaders.py
--rw-r--r--   0 runner    (1001) docker     (121)      592 2022-11-10 18:09:19.000000 openimis-be-product-1.5.0/product/enums.py
--rw-r--r--   0 runner    (1001) docker     (121)    12686 2022-11-10 18:09:19.000000 openimis-be-product-1.5.0/product/gql_mutations.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 18:09:28.061656 openimis-be-product-1.5.0/product/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)    17039 2022-11-10 18:09:19.000000 openimis-be-product-1.5.0/product/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)     1015 2022-11-10 18:09:19.000000 openimis-be-product-1.5.0/product/migrations/0002_productmutation.py
--rw-r--r--   0 runner    (1001) docker     (121)     1038 2022-11-10 18:09:19.000000 openimis-be-product-1.5.0/product/migrations/0003_add_enrollment_officer_gql_query_products_perms.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-10 18:09:19.000000 openimis-be-product-1.5.0/product/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    21452 2022-11-10 18:09:19.000000 openimis-be-product-1.5.0/product/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     9621 2022-11-10 18:09:19.000000 openimis-be-product-1.5.0/product/schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     4645 2022-11-10 18:09:19.000000 openimis-be-product-1.5.0/product/services.py
--rw-r--r--   0 runner    (1001) docker     (121)     2158 2022-11-10 18:09:19.000000 openimis-be-product-1.5.0/product/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-11-10 18:09:19.000000 openimis-be-product-1.5.0/product/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-11-10 18:09:19.000000 openimis-be-product-1.5.0/product/views.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-10 18:09:28.061656 openimis-be-product-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1188 2022-11-10 18:09:27.000000 openimis-be-product-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 21:38:14.934757 openimis-be-product-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1852 2023-05-16 21:37:55.000000 openimis-be-product-1.5.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (122)       36 2023-05-16 21:37:55.000000 openimis-be-product-1.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      688 2023-05-16 21:38:14.934757 openimis-be-product-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1408 2023-05-16 21:37:55.000000 openimis-be-product-1.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 21:38:14.930756 openimis-be-product-1.5.1/openimis_be_product.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      688 2023-05-16 21:38:14.000000 openimis-be-product-1.5.1/openimis_be_product.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      909 2023-05-16 21:38:14.000000 openimis-be-product-1.5.1/openimis_be_product.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-16 21:38:14.000000 openimis-be-product-1.5.1/openimis_be_product.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       45 2023-05-16 21:38:14.000000 openimis-be-product-1.5.1/openimis_be_product.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-05-16 21:38:14.000000 openimis-be-product-1.5.1/openimis_be_product.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 21:38:14.934757 openimis-be-product-1.5.1/product/
+-rw-r--r--   0 runner    (1001) docker     (122)       50 2023-05-16 21:37:55.000000 openimis-be-product-1.5.1/product/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-05-16 21:37:55.000000 openimis-be-product-1.5.1/product/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2613 2023-05-16 21:37:55.000000 openimis-be-product-1.5.1/product/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)      365 2023-05-16 21:37:55.000000 openimis-be-product-1.5.1/product/dataloaders.py
+-rw-r--r--   0 runner    (1001) docker     (122)      592 2023-05-16 21:37:55.000000 openimis-be-product-1.5.1/product/enums.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17841 2023-05-16 21:37:55.000000 openimis-be-product-1.5.1/product/gql_mutations.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 21:38:14.934757 openimis-be-product-1.5.1/product/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)    18332 2023-05-16 21:37:55.000000 openimis-be-product-1.5.1/product/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1015 2023-05-16 21:37:55.000000 openimis-be-product-1.5.1/product/migrations/0002_productmutation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1038 2023-05-16 21:37:55.000000 openimis-be-product-1.5.1/product/migrations/0003_add_enrollment_officer_gql_query_products_perms.py
+-rw-r--r--   0 runner    (1001) docker     (122)      371 2023-05-16 21:37:55.000000 openimis-be-product-1.5.1/product/migrations/0004_alter_product_options.py
+-rw-r--r--   0 runner    (1001) docker     (122)      540 2023-05-16 21:37:55.000000 openimis-be-product-1.5.1/product/migrations/0005_add_ceiling_type_column.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1912 2023-05-16 21:37:55.000000 openimis-be-product-1.5.1/product/migrations/0006_insert_ceiling_type.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3670 2023-05-16 21:37:55.000000 openimis-be-product-1.5.1/product/migrations/0007_auto_20230510_1347.py
+-rw-r--r--   0 runner    (1001) docker     (122)      507 2023-05-16 21:37:55.000000 openimis-be-product-1.5.1/product/migrations/0008_auto_20230510_1347.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-16 21:37:55.000000 openimis-be-product-1.5.1/product/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21166 2023-05-16 21:37:55.000000 openimis-be-product-1.5.1/product/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12211 2023-05-16 21:37:55.000000 openimis-be-product-1.5.1/product/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4804 2023-05-16 21:37:55.000000 openimis-be-product-1.5.1/product/services.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2158 2023-05-16 21:37:55.000000 openimis-be-product-1.5.1/product/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-05-16 21:37:55.000000 openimis-be-product-1.5.1/product/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-05-16 21:37:55.000000 openimis-be-product-1.5.1/product/views.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-16 21:38:14.934757 openimis-be-product-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1189 2023-05-16 21:38:12.000000 openimis-be-product-1.5.1/setup.py
```

### Comparing `openimis-be-product-1.5.0/LICENSE.md` & `openimis-be-product-1.5.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openimis-be-product-1.5.0/PKG-INFO` & `openimis-be-product-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-product
-Version: 1.5.0
+Version: 1.5.1
 Summary: The openIMIS Backend Product reference module.
 Home-page: https://openimis.org/
 Author: Xavier Gillmann
 Author-email: xgillmann@bluesquarehub.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-product-1.5.0/README.md` & `openimis-be-product-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `openimis-be-product-1.5.0/openimis_be_product.egg-info/PKG-INFO` & `openimis-be-product-1.5.1/openimis_be_product.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-product
-Version: 1.5.0
+Version: 1.5.1
 Summary: The openIMIS Backend Product reference module.
 Home-page: https://openimis.org/
 Author: Xavier Gillmann
 Author-email: xgillmann@bluesquarehub.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-product-1.5.0/openimis_be_product.egg-info/SOURCES.txt` & `openimis-be-product-1.5.1/openimis_be_product.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -18,8 +18,13 @@
 product/services.py
 product/test_helpers.py
 product/urls.py
 product/views.py
 product/migrations/0001_initial.py
 product/migrations/0002_productmutation.py
 product/migrations/0003_add_enrollment_officer_gql_query_products_perms.py
+product/migrations/0004_alter_product_options.py
+product/migrations/0005_add_ceiling_type_column.py
+product/migrations/0006_insert_ceiling_type.py
+product/migrations/0007_auto_20230510_1347.py
+product/migrations/0008_auto_20230510_1347.py
 product/migrations/__init__.py
```

### Comparing `openimis-be-product-1.5.0/product/enums.py` & `openimis-be-product-1.5.1/product/enums.py`

 * *Files identical despite different names*

### Comparing `openimis-be-product-1.5.0/product/gql_mutations.py` & `openimis-be-product-1.5.1/product/gql_mutations.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import datetime
 from gettext import gettext as _
 from operator import or_
 from dataclasses import dataclass
 
 import graphene
 from core.schema import OpenIMISMutation
 from django.contrib.auth.models import AnonymousUser
@@ -10,17 +11,18 @@
 from location.models import Location
 from .services import (
     set_product_items,
     set_product_relative_distribution,
     set_product_deductible_and_ceiling,
     save_product_history,
     set_product_services,
+    check_unique_code_product
 )
 from .apps import ProductConfig
-from .models import Product, ProductMutation
+from .models import Product, ProductItem, ProductService, ProductMutation, LIMIT_CHOICES
 from .enums import (
     CareTypeEnum,
     CeilingExclusionEnum,
     CeilingInterpretationEnum,
     CeilingTypeEnum,
     LimitTypeEnum,
     PriceOriginEnum,
@@ -40,31 +42,40 @@
         data.pop("deductible_ip", 0),
         data.pop("deductible_op", 0),
     )
 
 
 def extract_ceilings(data):
     return DeductibleOrCeilingValue(
-        data.pop("ceiling", 0), data.pop("ceiling_ip", 0), data.pop("ceiling_op", 0)
+        data.pop("ceiling", 0), data.pop(
+            "ceiling_ip", 0), data.pop("ceiling_op", 0)
     )
 
 
-def create_or_update_product(user, data):
+def create_or_update_product(user, data, is_duplicate=False):
     client_mutation_id = data.pop("client_mutation_id", None)
     data.pop("client_mutation_label", None)
     product_uuid = data.pop("uuid", None)
     location_uuid = data.pop("location_uuid", None)
     conversion_product_uuid = data.pop("conversion_product_uuid", None)
     relative_prices = data.pop("relative_prices", None)
     items = data.pop("items", None)
     services = data.pop("services", None)
-    ceiling_type = data.pop("ceiling_type", None)
+    ceiling_type = data.get("ceiling_type", None)
     deductibles = extract_deductibles(data)
     ceilings = extract_ceilings(data)
 
+    incoming_code = data.get('code')
+    current_product = Product.objects.filter(uuid=product_uuid).first()
+    current_code = current_product.code if current_product else None
+
+    if current_code != incoming_code:
+        if check_unique_code_product(incoming_code):
+            raise ValidationError(_("mutation.product_code_duplicated"))
+
     # Validate start cycles
     for start_cycle_key in [
         "start_cycle_1",
         "start_cycle_2",
         "start_cycle_3",
         "start_cycle_4",
     ]:
@@ -73,54 +84,91 @@
         try:
             [d, m] = data[start_cycle_key].split("-")
         except ValueError:
             raise ValueError(
                 f"'{data[start_cycle_key]}' is not a correct value for product.start_cycle"
             )
 
+    if items:
+        for item in items:
+            values = [(item['limitation_type'], item['limit_adult']),
+                      (item['limitation_type_e'], item['limit_adult_e']),
+                      (item['limitation_type_r'], item['limit_adult_r']),
+                      (item['limitation_type'], item['limit_child']),
+                      (item['limitation_type_e'], item['limit_child_e']),
+                      (item['limitation_type_r'], item['limit_child_r'])]
+            # checking if value can be interpreted as percentage
+            if not all([True if i[1] >= 0 else False for i in values]):
+                raise ValueError("Item O,R,E limits must be positive.")
+            if not all([True if i[1] <= 100 else False for i in values if i[0] != LIMIT_CHOICES[0][0]]):
+                raise ValueError(
+                    "Item O,R,E co-insurance limits must be smaller or equal to 100.")
+
+    if services:
+        for service in services:
+            values = [(service['limitation_type'], service['limit_adult']),
+                      (service['limitation_type_e'], service['limit_adult_e']),
+                      (service['limitation_type_r'], service['limit_adult_r']),
+                      (service['limitation_type'], service['limit_child']),
+                      (service['limitation_type_e'], service['limit_child_e']),
+                      (service['limitation_type_r'], service['limit_child_r'])]
+            # checking if value can be interpreted as percentage
+            if not all([True if i[1] >= 0 else False for i in values]):
+                raise ValueError("Service O,R,E limits must be positive.")
+            if not all([True if i[1] <= 100 else False for i in values if i[0] != LIMIT_CHOICES[0][0]]):
+                raise ValueError(
+                    "Service O,R,E co-insurance limits must be smaller or equal to 100.")
+
     if data["date_from"] > data["date_to"]:
         raise ValueError("date_from must be before date_to")
-
     if product_uuid:
         product = Product.objects.get(uuid=product_uuid)
+        if product.validity_to:
+            raise ValidationError("Cannot update historical data.")
         save_product_history(product)
         for (key, value) in data.items():
             setattr(product, key, value)
     else:
         product = Product.objects.create(**data)
 
     if location_uuid is not None:
         product.location = Location.objects.get(uuid=location_uuid)
 
     if conversion_product_uuid is not None:
-        product.conversion_product = Product.objects.get(uuid=conversion_product_uuid)
+        product.conversion_product = Product.objects.get(
+            uuid=conversion_product_uuid)
 
     set_product_relative_distribution(user, product, relative_prices)
 
     set_product_deductible_and_ceiling(
         product, ceiling_type, deductibles, ceilings, user
     )
 
     if items is not None:
         set_product_items(product, items, user)
 
     if services is not None:
         set_product_services(product, services, user)
 
+    product.validity_from = datetime.datetime.now()
     product.save()
 
     if client_mutation_id:
         ProductMutation.object_mutated(
             user, client_mutation_id=client_mutation_id, product=product
         )
 
+    if is_duplicate:
+        return product
+
 
 class RelativePricesInput(graphene.InputObjectType):
     care_type = graphene.Field(CareTypeEnum)
-    periods = graphene.NonNull(graphene.List(graphene.NonNull(graphene.Decimal)))
+    periods = graphene.NonNull(graphene.List(
+        graphene.NonNull(graphene.Decimal)))
 
 
 class CreateOrUpdateProductMutation(OpenIMISMutation):
     @classmethod
     def do_mutate(cls, perms, user, **data):
         if type(user) is AnonymousUser or not user.id:
             raise ValidationError(_("mutation.authentication_required"))
@@ -202,15 +250,16 @@
     grace_period_renewal = graphene.Int(default_value=0)
     grace_period_payment = graphene.Int(default_value=0)
     grace_period_enrolment = graphene.Int(default_value=0)
 
     registration_lump_sum = graphene.Decimal(
         max_digits=18, decimal_places=2, required=False
     )
-    registration_fee = graphene.Decimal(max_digits=18, decimal_places=2, required=False)
+    registration_fee = graphene.Decimal(
+        max_digits=18, decimal_places=2, required=False)
     general_assembly_lump_sum = graphene.Decimal(
         max_digits=18, decimal_places=2, required=False
     )
     general_assembly_fee = graphene.Decimal(
         max_digits=18, decimal_places=2, required=False
     )
 
@@ -274,15 +323,16 @@
     max_no_hospitalization = graphene.Int()
     max_no_visits = graphene.Int()
     max_no_antenatal = graphene.Int()
 
     max_amount_consultation = graphene.Decimal(max_digits=18, decimal_places=2)
     max_amount_surgery = graphene.Decimal(max_digits=18, decimal_places=2)
     max_amount_delivery = graphene.Decimal(max_digits=18, decimal_places=2)
-    max_amount_hospitalization = graphene.Decimal(max_digits=18, decimal_places=2)
+    max_amount_hospitalization = graphene.Decimal(
+        max_digits=18, decimal_places=2)
     max_amount_antenatal = graphene.Decimal(max_digits=18, decimal_places=2)
 
     relative_prices = graphene.List(RelativePricesInput)
     items = graphene.List(graphene.NonNull(ProductItemInput))
     services = graphene.List(graphene.NonNull(ProductServiceInput))
 
 
@@ -297,29 +347,102 @@
     def async_mutate(cls, user, **data):
         try:
             cls.do_mutate(
                 ProductConfig.gql_mutation_products_add_perms,
                 user,
                 **data,
             )
+        except ValueError as exc:
+            return [
+                {
+                    "message": str(exc)
+                }
+            ]
         except Exception as exc:
             return [
                 {
                     "message": _("product.mutation.failed_to_create_product"),
                     "detail": str(exc),
                 }
             ]
 
 
+class DuplicateProductMutation(OpenIMISMutation):
+    _mutation_module = "product"
+    _mutation_class = "DuplicateProductMutation"
+
+    class Input(ProductInputType):
+        code = graphene.String(required=True)
+        uuid = graphene.UUID(required=False)
+
+    @classmethod
+    def async_mutate(cls, user, **data):
+        try:
+            cls.do_mutate(
+                ProductConfig.gql_mutation_products_add_perms,
+                user,
+                **data,
+            )
+        except ValueError as exc:
+            return [
+                {
+                    "message": str(exc)
+                }
+            ]
+        except Exception as exc:
+            return [
+                {
+                    "message": _("product.mutation.failed_to_duplicate_product"),
+                    "detail": str(exc),
+                }
+            ]
+
+    @classmethod
+    def do_mutate(cls, perms, user, **data):
+        if type(user) is AnonymousUser or not user.id:
+            raise ValidationError(_("mutation.authentication_required"))
+        if not user.has_perms(perms):
+            raise PermissionDenied(_("unauthorized"))
+        current_uuid = data.pop("uuid") if "uuid" in data else None
+
+        data["audit_user_id"] = user.id_for_audit
+
+        duplicate_items = True if 'items' not in data else False
+        duplicate_services = True if 'services' not in data else False
+
+        new_product = create_or_update_product(user, data, is_duplicate=True)
+
+        if duplicate_items:
+            new_product_items = ProductItem.objects.filter(product=Product.objects.get(uuid=current_uuid,
+                                                           validity_to__isnull=True))
+            for item in new_product_items:
+                # create a new instance by setting pk = None
+                item.pk = None
+                item.product = new_product
+                item.save()
+
+        if duplicate_services:
+            new_product_services = ProductService.objects.filter(product=Product.objects.get(uuid=current_uuid,
+                                                                 validity_to__isnull=True))
+            for service in new_product_services:
+                # create a new instance by setting pk = None
+                service.pk = None
+                service.product = new_product
+                service.save()
+
+        return new_product
+
+
 class UpdateProductMutation(CreateOrUpdateProductMutation):
     _mutation_module = "product"
     _mutation_class = "UpdateProductMutation"
 
     class Input(ProductInputType):
         uuid = graphene.UUID(required=True)
+        code = graphene.String(required=True)
 
     @classmethod
     def async_mutate(cls, user, **data):
         try:
             cls.do_mutate(
                 ProductConfig.gql_mutation_products_edit_perms,
                 user,
```

### Comparing `openimis-be-product-1.5.0/product/migrations/0001_initial.py` & `openimis-be-product-1.5.1/product/migrations/0001_initial.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Generated by Django 3.0.14 on 2021-09-16 14:49
 
 import core.fields
 import datetime
 from django.db import migrations, models
+import django.db.models.deletion
 import product.models
 import uuid
 
 
 class Migration(migrations.Migration):
 
     initial = True
@@ -89,25 +90,31 @@
                 ('max_policy_extra_member_ip', models.DecimalField(blank=True, db_column='MaxPolicyExtraMemberIP', decimal_places=2, max_digits=18, null=True)),
                 ('max_policy_extra_member_op', models.DecimalField(blank=True, db_column='MaxPolicyExtraMemberOP', decimal_places=2, max_digits=18, null=True)),
                 ('max_ceiling_policy', models.DecimalField(blank=True, db_column='MaxCeilingPolicy', decimal_places=2, max_digits=18, null=True)),
                 ('max_ceiling_policy_ip', models.DecimalField(blank=True, db_column='MaxCeilingPolicyIP', decimal_places=2, max_digits=18, null=True)),
                 ('max_ceiling_policy_op', models.DecimalField(blank=True, db_column='MaxCeilingPolicyOP', decimal_places=2, max_digits=18, null=True)),
                 ('max_amount_antenatal', models.DecimalField(blank=True, db_column='MaxAmountAntenatal', decimal_places=2, max_digits=18, null=True)),
                 ('max_no_antenatal', models.IntegerField(blank=True, db_column='MaxNoAntenatal', null=True)),
-                ('ceiling_interpretation', models.CharField(blank=True, db_column='CeilingInterpretation', max_length=1, null=True)),
                 ('capitation_level_1', models.CharField(blank=True, db_column='Level1', max_length=1, null=True)),
                 ('capitation_level_2', models.CharField(blank=True, db_column='Level2', max_length=1, null=True)),
                 ('capitation_level_3', models.CharField(blank=True, db_column='Level3', max_length=1, null=True)),
                 ('capitation_level_4', models.CharField(blank=True, db_column='Level4', max_length=1, null=True)),
                 ('weight_population', models.DecimalField(blank=True, db_column='WeightPopulation', decimal_places=2, max_digits=5, null=True)),
                 ('weight_nb_families', models.DecimalField(blank=True, db_column='WeightNumberFamilies', decimal_places=2, max_digits=5, null=True)),
                 ('weight_insured_population', models.DecimalField(blank=True, db_column='WeightInsuredPopulation', decimal_places=2, max_digits=5, null=True)),
                 ('weight_nb_insured_families', models.DecimalField(blank=True, db_column='WeightNumberInsuredFamilies', decimal_places=2, max_digits=5, null=True)),
                 ('weight_nb_visits', models.DecimalField(blank=True, db_column='WeightNumberVisits', decimal_places=2, max_digits=5, null=True)),
                 ('weight_adjusted_amount', models.DecimalField(blank=True, db_column='WeightAdjustedAmount', decimal_places=2, max_digits=5, null=True)),
+                ('capitation_sublevel_1', models.ForeignKey(blank=True, db_column='Sublevel1', null=True, on_delete=django.db.models.deletion.DO_NOTHING, related_name='+', to='location.healthfacilitysublevel')),
+                ('capitation_sublevel_2', models.ForeignKey(blank=True, db_column='Sublevel2', null=True, on_delete=django.db.models.deletion.DO_NOTHING, related_name='+', to='location.healthfacilitysublevel')),
+                ('capitation_sublevel_3', models.ForeignKey(blank=True, db_column='Sublevel3', null=True, on_delete=django.db.models.deletion.DO_NOTHING, related_name='+', to='location.healthfacilitysublevel')),
+                ('capitation_sublevel_4', models.ForeignKey(blank=True, db_column='Sublevel4', null=True, on_delete=django.db.models.deletion.DO_NOTHING, related_name='+', to='location.healthfacilitysublevel')),
+                ('conversion_product', models.ForeignKey(blank=True, db_column='ConversionProdID', null=True, on_delete=django.db.models.deletion.DO_NOTHING, to='product.product')),
+                ('location', models.ForeignKey(blank=True, db_column='LocationId', null=True, on_delete=django.db.models.deletion.DO_NOTHING, to='location.location')),
+                ('ceiling_interpretation', models.CharField(blank=True, choices=[('I', 'Claim Type'), ('H', 'Health Facility Type')], db_column='CeilingInterpretation', max_length=1, null=True)),
             ],
             options={
                 'db_table': 'tblProduct',
                 'managed': False,
             },
         ),
         migrations.CreateModel(
```

### Comparing `openimis-be-product-1.5.0/product/migrations/0002_productmutation.py` & `openimis-be-product-1.5.1/product/migrations/0002_productmutation.py`

 * *Files identical despite different names*

### Comparing `openimis-be-product-1.5.0/product/migrations/0003_add_enrollment_officer_gql_query_products_perms.py` & `openimis-be-product-1.5.1/product/migrations/0003_add_enrollment_officer_gql_query_products_perms.py`

 * *Files identical despite different names*

### Comparing `openimis-be-product-1.5.0/product/models.py` & `openimis-be-product-1.5.1/product/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -286,14 +286,27 @@
     max_amount_antenatal = models.DecimalField(
         db_column="MaxAmountAntenatal",
         max_digits=18,
         decimal_places=2,
         blank=True,
         null=True,
     )
+
+    ceiling_type = models.CharField(
+        max_length=1,
+        db_column="CeilingType",
+        blank=True,
+        null=True,
+        choices=(
+            ("I", gettext_lazy("INSUREE")),
+            ("T", gettext_lazy("TREATMENT")),
+            ("P", gettext_lazy("POLICY")),
+        ),
+    )
+
     max_no_antenatal = models.IntegerField(
         db_column="MaxNoAntenatal", blank=True, null=True
     )
     ceiling_interpretation = models.CharField(
         max_length=1,
         db_column="CeilingInterpretation",
         blank=True,
@@ -386,37 +399,14 @@
         db_column="WeightAdjustedAmount",
         max_digits=5,
         decimal_places=2,
         blank=True,
         null=True,
     )
 
-    @property
-    def ceiling_type(self):
-        if (
-            self.ded_treatment
-            or self.ded_op_treatment
-            or self.ded_ip_treatment
-            or self.max_treatment
-            or self.max_ip_treatment
-            or self.max_op_treatment
-        ):
-            return "T"
-        elif (
-            self.ded_policy
-            or self.ded_op_policy
-            or self.ded_ip_policy
-            or self.max_policy
-            or self.max_ip_policy
-            or self.max_op_policy
-        ):
-            return "P"
-        else:
-            return "I"
-
     def has_cycle(self):
         return (
             bool(self.start_cycle_1)
             or bool(self.start_cycle_2)
             or bool(self.start_cycle_3)
             or bool(self.start_cycle_4)
         )
@@ -434,15 +424,15 @@
             "'member_count' has been deprecated in favor of 'max_members'",
             DeprecationWarning,
             stacklevel=2
         )
         return self.max_members
 
     class Meta:
-        managed = False
+        managed = True
         db_table = "tblProduct"
 
     CEILING_INTERPRETATION_HOSPITAL = "H"
     CEILING_INTERPRETATION_IN_PATIENT = "I"
 
     RELATIVE_PRICE_PERIOD_MONTH = "M"
     RELATIVE_PRICE_PERIOD_QUARTER = "Q"
@@ -562,15 +552,15 @@
     )
     audit_user_id = models.IntegerField(db_column="AuditUserID")
     # rowid = models.TextField(db_column='RowID', blank=True, null=True) This field type is a guess.
     model_prefix = "item"
     objects = ProductItemOrServiceManager()
 
     class Meta:
-        managed = False
+        managed = True
         db_table = "tblProductItems"
 
 
 class ProductService(VersionedModel, ProductItemOrService):
     id = models.AutoField(db_column="ProdServiceID", primary_key=True)
     product = models.ForeignKey(
         Product,
@@ -649,15 +639,15 @@
     audit_user_id = models.IntegerField(db_column="AuditUserID")
     # rowid = models.TextField(db_column='RowID', blank=True, null=True) This field type is a guess.
 
     model_prefix = "service"
     objects = ProductItemOrServiceManager()
 
     class Meta:
-        managed = False
+        managed = True
         db_table = "tblProductServices"
 
 
 class ProductMutation(UUIDModel, ObjectMutation):
     product = models.ForeignKey(Product, models.DO_NOTHING, related_name="+")
     mutation = models.ForeignKey(
         MutationLog, models.DO_NOTHING, related_name="products"
```

### Comparing `openimis-be-product-1.5.0/product/schema.py` & `openimis-be-product-1.5.1/product/schema.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,26 @@
+import json
+
 from django.core.exceptions import PermissionDenied
 from core import ExtendedConnection, prefix_filterset
 from django.db.models import Q
 import graphene
 from graphene.relay import Node
 from django.utils.translation import gettext_lazy
 from graphene_django import DjangoObjectType
 from graphene_django.filter import DjangoFilterConnectionField
 import graphene_django_optimizer as gql_optimizer
 
 from .models import Product, ProductItem, ProductService
+from .services import check_unique_code_product
 from .gql_mutations import (
     CreateProductMutation,
     UpdateProductMutation,
     DeleteProductMutation,
+    DuplicateProductMutation
 )
 from .apps import ProductConfig
 from django.utils.translation import gettext as _
 from core import filter_validity
 from .enums import (
     CareTypeEnum,
     CeilingExclusionEnum,
@@ -25,15 +29,16 @@
     LimitTypeEnum,
     PriceOriginEnum,
 )
 
 
 class ProductRelativePricesGQLType(graphene.ObjectType):
     care_type = graphene.Field(CareTypeEnum)
-    periods = graphene.NonNull(graphene.List(graphene.NonNull(graphene.Decimal)))
+    periods = graphene.NonNull(graphene.List(
+        graphene.NonNull(graphene.Decimal)))
 
 
 def period_type_to_number(period_type):
     if period_type == "M":
         return 12
     elif period_type == "Y":
         return 1
@@ -41,15 +46,16 @@
         return 4
     else:
         return None
 
 
 class ProductGQLType(DjangoObjectType):
     ceiling_interpretation = graphene.Field(CeilingInterpretationEnum)
-    relative_prices = graphene.NonNull(graphene.List(ProductRelativePricesGQLType))
+    relative_prices = graphene.NonNull(
+        graphene.List(ProductRelativePricesGQLType))
 
     ceiling_type = graphene.Field(CeilingTypeEnum)
 
     deductible = graphene.Decimal()
     deductible_ip = graphene.Decimal()
     deductible_op = graphene.Decimal()
 
@@ -134,17 +140,17 @@
                     care_type=care_type, periods=[x.percent for x in periods]
                 )
             )
 
         return relative_prices
 
     def resolve_location(self, info):
-      if "location_loader" in info.context.dataloaders and self.location_id:
-          return info.context.dataloaders["location_loader"].load(self.location_id)
-      return self.location
+        if "location_loader" in info.context.dataloaders and self.location_id:
+            return info.context.dataloaders["location_loader"].load(self.location_id)
+        return self.location
 
     class Meta:
         model = Product
         interfaces = (Node,)
         filter_fields = {
             "id": ["exact"],
             "uuid": ["exact"],
@@ -194,14 +200,42 @@
             "max_policy",
             "max_ip_policy",
             "max_op_policy",
         )
         connection_class = ExtendedConnection
 
 
+class PageDisplayRulesGQLType(graphene.ObjectType):
+    min_limit_value = graphene.Decimal()
+    max_limit_value = graphene.Decimal()
+
+    def resolve_min_limit_value(self, info):
+        return ProductConfig.min_limit_value
+
+    def resolve_max_limit_value(self, info):
+        return ProductConfig.max_limit_value
+
+
+class ProductItemOrServiceDefaultValuesGQLType(graphene.ObjectType):
+    default_price_origin = graphene.String()
+    default_limit = graphene.String()
+    default_limit_co_insurance_value = graphene.Int()
+    default_limit_fixed_value = graphene.Int()
+
+    def resolve_default_price_origin(self, info):
+        return ProductConfig.default_price_origin
+    def resolve_default_limit(self, info):
+        return ProductConfig.default_limit
+    def resolve_default_limit_co_insurance_value(self, info):
+        return ProductConfig.default_limit_co_insurance_value
+
+    def resolve_default_limit_fixed_value(self, info):
+        return ProductConfig.default_limit_fixed_value
+
+
 class ProductItemGQLType(DjangoObjectType):
     ceiling_exclusion_adult = graphene.Field(CeilingExclusionEnum)
     ceiling_exclusion_child = graphene.Field(CeilingExclusionEnum)
     limitation_type = graphene.Field(LimitTypeEnum)
     limitation_type_r = graphene.Field(LimitTypeEnum)
     limitation_type_e = graphene.Field(LimitTypeEnum)
     price_origin = graphene.Field(PriceOriginEnum)
@@ -241,17 +275,36 @@
 
 
 class Query(graphene.ObjectType):
     products = DjangoFilterConnectionField(
         ProductGQLType,
         location=graphene.Int(),
         show_history=graphene.Boolean(),
-        search=graphene.String(description=gettext_lazy("Search in `name` & `code`")),
+        search=graphene.String(description=gettext_lazy(
+            "Search in `name` & `code`")),
     )
-    product = graphene.Field(ProductGQLType, id=graphene.ID(), uuid=graphene.String())
+    product = graphene.Field(
+        ProductGQLType, id=graphene.ID(), uuid=graphene.String())
+    page_display_rules = graphene.Field(PageDisplayRulesGQLType)
+    limit_defaults = graphene.Field(ProductItemOrServiceDefaultValuesGQLType)
+    validate_product_code = graphene.Field(
+        graphene.Boolean,
+        product_code=graphene.String(required=True),
+        description="Checks that the specified product code is unique."
+    )
+
+    def resolve_limit_defaults(self, info):
+        if not info.context.user.has_perms(ProductConfig.gql_query_products_perms):
+            raise PermissionDenied("unauthorized")
+        return ProductItemOrServiceDefaultValuesGQLType()
+
+    def resolve_page_display_rules(self, info):
+        if not info.context.user.has_perms(ProductConfig.gql_query_products_perms):
+            raise PermissionDenied(_("unauthorized"))
+        return PageDisplayRulesGQLType()
 
     def resolve_product(self, info, **kwargs):
         if not info.context.user.has_perms(ProductConfig.gql_query_products_perms):
             raise PermissionDenied(_("unauthorized"))
         if kwargs.get("id", None) is not None:
             return Node.get_node_from_global_id(info, kwargs["id"])
         elif kwargs.get("uuid", None) is not None:
@@ -266,24 +319,39 @@
             raise PermissionDenied(_("unauthorized"))
 
         qs = Product.objects
         if not show_history:
             qs = qs.filter(*filter_validity(**kwargs))
 
         if search is not None:
-            qs = qs.filter(Q(name__icontains=search) | Q(code__icontains=search))
+            qs = qs.filter(Q(name__icontains=search) |
+                           Q(code__icontains=search))
 
         if location is not None:
             from location.models import Location
 
             qs = qs.filter(
                 Q(location__in=Location.objects.parents(location))
                 | Q(location__id=location)
+                | Q(location__isnull=True)
+
             )
 
+        # Consider only the locations user is configured for
+        from location.models import Location
+        qs = qs.filter(Location.build_user_location_filter_query(
+            info.context.user._u))
+
         return gql_optimizer.query(qs, info)
 
+    def resolve_validate_product_code(self, info, **kwargs):
+        if not info.context.user.has_perms(ProductConfig.gql_query_products_perms):
+            raise PermissionDenied(_("unauthorized"))
+        errors = check_unique_code_product(code=kwargs['product_code'])
+        return False if errors else True
+
 
 class Mutation(graphene.ObjectType):
     create_product = CreateProductMutation.Field()
+    duplicate_product = DuplicateProductMutation.Field()
     update_product = UpdateProductMutation.Field()
     delete_product = DeleteProductMutation.Field()
```

### Comparing `openimis-be-product-1.5.0/product/services.py` & `openimis-be-product-1.5.1/product/services.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from core import datetime
 from django.apps import apps
 from core.utils import TimeUtils
 import logging
+from .models import Product
 
 from django.core.exceptions import ValidationError
 
 logger = logging.getLogger(__name__)
 
 
 def save_product_history(product):
@@ -19,15 +20,16 @@
     "B": "period_rel_prices",
 }
 
 periods_to_period_rel_prices = {1: "Y", 4: "Q", 12: "M"}
 
 
 def set_product_relative_distribution(user, product, relative_distributions):
-    RelativeDistribution = apps.get_model("claim_batch", "RelativeDistribution")
+    RelativeDistribution = apps.get_model(
+        "claim_batch", "RelativeDistribution")
     if RelativeDistribution is None:
         logger.warning("RelativeDistribution does not exist.")
         return
 
     product.relative_distributions.update(validity_to=TimeUtils.now())
     product.period_rel_prices = None
     product.period_rel_prices_ip = None
@@ -36,17 +38,14 @@
     if relative_distributions is None:
         return
 
     for distr in relative_distributions:
         if len(distr.periods) not in (1, 4, 12):
             raise ValueError("Number of periods can only be 1, 4 or 12")
 
-        if sum([x for x in distr.periods]) != 100:
-            raise ValueError("Sum of periods must be 100%")
-
         setattr(
             product,
             care_type_to_field[distr.care_type],
             periods_to_period_rel_prices[len(distr.periods)],
         )
         for idx, percent in enumerate(distr.periods):
             RelativeDistribution.objects.create(
@@ -115,15 +114,16 @@
     # Ensure there no duplicates
     seen_uuids = []
 
     product.items.update(validity_to=TimeUtils.now())
     for item in items:
         uuid = item.pop("item_uuid")
         if uuid in seen_uuids:
-            raise ValidationError(f"'{uuid}' is already linked to the product.")
+            raise ValidationError(
+                f"'{uuid}' is already linked to the product.")
         seen_uuids.append(uuid)
 
         product.items.create(
             item=Item.objects.get(uuid=uuid),
             audit_user_id=user.id_for_audit,
             **item,
         )
@@ -138,15 +138,22 @@
     # Ensure there no duplicates
     seen_uuids = []
 
     product.services.update(validity_to=TimeUtils.now())
     for service in services:
         uuid = service.pop("service_uuid")
         if uuid in seen_uuids:
-            raise ValidationError(f"'{uuid}' is already linked to the product.")
+            raise ValidationError(
+                f"'{uuid}' is already linked to the product.")
         seen_uuids.append(uuid)
 
         product.services.create(
             service=Service.objects.get(uuid=uuid),
             audit_user_id=user.id_for_audit,
             **service,
         )
+
+
+def check_unique_code_product(code):
+    if Product.objects.filter(code=code, validity_to__isnull=True).exists():
+        return [{"message": "Product code %s already exists" % code}]
+    return []
```

### Comparing `openimis-be-product-1.5.0/product/test_helpers.py` & `openimis-be-product-1.5.1/product/test_helpers.py`

 * *Files identical despite different names*

### Comparing `openimis-be-product-1.5.0/setup.py` & `openimis-be-product-1.5.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='openimis-be-product',
-    version='1.5.0',
+    version='v1.5.1',
     packages=find_packages(),
     include_package_data=True,
     license='GNU AGPL v3',
     description='The openIMIS Backend Product reference module.',
     # long_description=README,
     url='https://openimis.org/',
     author='Xavier Gillmann',
```

