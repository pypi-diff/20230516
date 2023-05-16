# Comparing `tmp/openimis-be-policy-1.5.0.tar.gz` & `tmp/openimis-be-policy-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis-be-policy-1.5.0.tar", last modified: Thu Nov 10 18:09:45 2022, max compression
+gzip compressed data, was "openimis-be-policy-1.5.1.tar", last modified: Tue May 16 21:38:20 2023, max compression
```

## Comparing `openimis-be-policy-1.5.0.tar` & `openimis-be-policy-1.5.1.tar`

### file list

```diff
@@ -1,38 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 18:09:45.430547 openimis-be-policy-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1852 2022-11-10 18:09:30.000000 openimis-be-policy-1.5.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-11-10 18:09:30.000000 openimis-be-policy-1.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      686 2022-11-10 18:09:45.430547 openimis-be-policy-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3838 2022-11-10 18:09:30.000000 openimis-be-policy-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 18:09:45.426547 openimis-be-policy-1.5.0/openimis_be_policy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      686 2022-11-10 18:09:45.000000 openimis-be-policy-1.5.0/openimis_be_policy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      755 2022-11-10 18:09:45.000000 openimis-be-policy-1.5.0/openimis_be_policy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-10 18:09:45.000000 openimis-be-policy-1.5.0/openimis_be_policy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-11-10 18:09:45.000000 openimis-be-policy-1.5.0/openimis_be_policy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-11-10 18:09:45.000000 openimis-be-policy-1.5.0/openimis_be_policy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 18:09:45.430547 openimis-be-policy-1.5.0/policy/
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-11-10 18:09:30.000000 openimis-be-policy-1.5.0/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-11-10 18:09:30.000000 openimis-be-policy-1.5.0/policy/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)     3401 2022-11-10 18:09:30.000000 openimis-be-policy-1.5.0/policy/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)     6015 2022-11-10 18:09:30.000000 openimis-be-policy-1.5.0/policy/gql_mutations.py
--rw-r--r--   0 runner    (1001) docker     (121)     3554 2022-11-10 18:09:30.000000 openimis-be-policy-1.5.0/policy/gql_queries.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 18:09:45.430547 openimis-be-policy-1.5.0/policy/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     1809 2022-11-10 18:09:30.000000 openimis-be-policy-1.5.0/policy/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)     2673 2022-11-10 18:09:30.000000 openimis-be-policy-1.5.0/policy/migrations/0002_policy_renewals.py
--rw-r--r--   0 runner    (1001) docker     (121)     1057 2022-11-10 18:09:30.000000 openimis-be-policy-1.5.0/policy/migrations/0003_auto_20201021_0811.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-10 18:09:30.000000 openimis-be-policy-1.5.0/policy/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5159 2022-11-10 18:09:30.000000 openimis-be-policy-1.5.0/policy/models.py
--rw-r--r--   0 runner    (1001) docker     (121)    12632 2022-11-10 18:09:30.000000 openimis-be-policy-1.5.0/policy/schema.py
--rw-r--r--   0 runner    (1001) docker     (121)    47238 2022-11-10 18:09:30.000000 openimis-be-policy-1.5.0/policy/services.py
--rw-r--r--   0 runner    (1001) docker     (121)      212 2022-11-10 18:09:30.000000 openimis-be-policy-1.5.0/policy/signals.py
--rw-r--r--   0 runner    (1001) docker     (121)     2164 2022-11-10 18:09:30.000000 openimis-be-policy-1.5.0/policy/tasks.py
--rw-r--r--   0 runner    (1001) docker     (121)     1958 2022-11-10 18:09:30.000000 openimis-be-policy-1.5.0/policy/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)    21452 2022-11-10 18:09:30.000000 openimis-be-policy-1.5.0/policy/test_services.py
--rw-r--r--   0 runner    (1001) docker     (121)     6950 2022-11-10 18:09:30.000000 openimis-be-policy-1.5.0/policy/test_values.py
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-11-10 18:09:30.000000 openimis-be-policy-1.5.0/policy/tests.py
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-11-10 18:09:30.000000 openimis-be-policy-1.5.0/policy/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)      806 2022-11-10 18:09:30.000000 openimis-be-policy-1.5.0/policy/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      851 2022-11-10 18:09:30.000000 openimis-be-policy-1.5.0/policy/validations.py
--rw-r--r--   0 runner    (1001) docker     (121)     6631 2022-11-10 18:09:30.000000 openimis-be-policy-1.5.0/policy/values.py
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-11-10 18:09:30.000000 openimis-be-policy-1.5.0/policy/views.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-10 18:09:45.430547 openimis-be-policy-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1274 2022-11-10 18:09:43.000000 openimis-be-policy-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:20.591902 openimis-be-policy-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-16 21:38:01.000000 openimis-be-policy-1.5.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-16 21:38:01.000000 openimis-be-policy-1.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-16 21:38:20.591902 openimis-be-policy-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-05-16 21:38:01.000000 openimis-be-policy-1.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:20.587902 openimis-be-policy-1.5.1/openimis_be_policy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-16 21:38:20.000000 openimis-be-policy-1.5.1/openimis_be_policy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-16 21:38:20.000000 openimis-be-policy-1.5.1/openimis_be_policy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 21:38:20.000000 openimis-be-policy-1.5.1/openimis_be_policy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-16 21:38:20.000000 openimis-be-policy-1.5.1/openimis_be_policy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-16 21:38:20.000000 openimis-be-policy-1.5.1/openimis_be_policy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:20.591902 openimis-be-policy-1.5.1/policy/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-16 21:38:01.000000 openimis-be-policy-1.5.1/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-16 21:38:01.000000 openimis-be-policy-1.5.1/policy/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-05-16 21:38:01.000000 openimis-be-policy-1.5.1/policy/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-05-16 21:38:01.000000 openimis-be-policy-1.5.1/policy/gql_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-05-16 21:38:01.000000 openimis-be-policy-1.5.1/policy/gql_queries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:20.591902 openimis-be-policy-1.5.1/policy/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-16 21:38:01.000000 openimis-be-policy-1.5.1/policy/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-05-16 21:38:01.000000 openimis-be-policy-1.5.1/policy/migrations/0002_policy_renewals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-16 21:38:01.000000 openimis-be-policy-1.5.1/policy/migrations/0003_auto_20201021_0811.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-16 21:38:01.000000 openimis-be-policy-1.5.1/policy/migrations/0004_add_medical_oficer_reading_rights.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-05-16 21:38:01.000000 openimis-be-policy-1.5.1/policy/migrations/0005_add_foreign_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-16 21:38:01.000000 openimis-be-policy-1.5.1/policy/migrations/0006_set_model_managed_to_true.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:01.000000 openimis-be-policy-1.5.1/policy/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-05-16 21:38:01.000000 openimis-be-policy-1.5.1/policy/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14453 2023-05-16 21:38:01.000000 openimis-be-policy-1.5.1/policy/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46589 2023-05-16 21:38:01.000000 openimis-be-policy-1.5.1/policy/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-16 21:38:01.000000 openimis-be-policy-1.5.1/policy/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-05-16 21:38:01.000000 openimis-be-policy-1.5.1/policy/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4771 2023-05-16 21:38:01.000000 openimis-be-policy-1.5.1/policy/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23317 2023-05-16 21:38:01.000000 openimis-be-policy-1.5.1/policy/test_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6950 2023-05-16 21:38:01.000000 openimis-be-policy-1.5.1/policy/test_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-16 21:38:01.000000 openimis-be-policy-1.5.1/policy/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-16 21:38:01.000000 openimis-be-policy-1.5.1/policy/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-16 21:38:01.000000 openimis-be-policy-1.5.1/policy/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-16 21:38:01.000000 openimis-be-policy-1.5.1/policy/validations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-05-16 21:38:01.000000 openimis-be-policy-1.5.1/policy/values.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-16 21:38:01.000000 openimis-be-policy-1.5.1/policy/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 21:38:20.591902 openimis-be-policy-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-16 21:38:18.000000 openimis-be-policy-1.5.1/setup.py
```

### Comparing `openimis-be-policy-1.5.0/LICENSE.md` & `openimis-be-policy-1.5.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openimis-be-policy-1.5.0/PKG-INFO` & `openimis-be-policy-1.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-policy
-Version: 1.5.0
+Version: 1.5.1
 Summary: The openIMIS Backend Policy reference module.
 Home-page: https://openimis.org/
 Author: Xavier Gillmann
 Author-email: xgillmann@bluesquarehub.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-policy-1.5.0/README.md` & `openimis-be-policy-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `openimis-be-policy-1.5.0/openimis_be_policy.egg-info/PKG-INFO` & `openimis-be-policy-1.5.1/openimis_be_policy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-policy
-Version: 1.5.0
+Version: 1.5.1
 Summary: The openIMIS Backend Policy reference module.
 Home-page: https://openimis.org/
 Author: Xavier Gillmann
 Author-email: xgillmann@bluesquarehub.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-policy-1.5.0/openimis_be_policy.egg-info/SOURCES.txt` & `openimis-be-policy-1.5.1/openimis_be_policy.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -25,8 +25,11 @@
 policy/utils.py
 policy/validations.py
 policy/values.py
 policy/views.py
 policy/migrations/0001_initial.py
 policy/migrations/0002_policy_renewals.py
 policy/migrations/0003_auto_20201021_0811.py
+policy/migrations/0004_add_medical_oficer_reading_rights.py
+policy/migrations/0005_add_foreign_keys.py
+policy/migrations/0006_set_model_managed_to_true.py
 policy/migrations/__init__.py
```

### Comparing `openimis-be-policy-1.5.0/policy/apps.py` & `openimis-be-policy-1.5.1/policy/apps.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policy-1.5.0/policy/gql_mutations.py` & `openimis-be-policy-1.5.1/policy/gql_mutations.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,24 @@
+import logging
+
 import graphene
-from policy.services import update_insuree_policies, PolicyService
+from django.db import transaction
+
+from policy.services import PolicyService
 
 from .apps import PolicyConfig
 from core.schema import OpenIMISMutation
 from .models import Policy
 from django.contrib.auth.models import AnonymousUser
 from django.core.exceptions import ValidationError, PermissionDenied
 from django.utils.translation import gettext as _
 from .validations import validate_idle_policy
 
+logger = logging.getLogger(__name__)
+
 
 class PolicyInputType(OpenIMISMutation.Input):
     # several fields (such as status, stage,...) are managed "internally"
     # and only initialized/updated via dedicated mutations (renew , cancel,...)
     id = graphene.Int(required=False, read_only=True)
     uuid = graphene.String(required=False)
     enroll_date = graphene.Date(required=True)
@@ -48,117 +54,132 @@
 
     class Input(PolicyInputType):
         pass
 
     @classmethod
     def async_mutate(cls, user, **data):
         try:
-            data["status"] = Policy.STATUS_IDLE
-            data["stage"] = Policy.STAGE_NEW
-            return cls.do_mutate(PolicyConfig.gql_mutation_create_policies_perms, user, **data)
+            with transaction.atomic():
+                data["status"] = Policy.STATUS_IDLE
+                data["stage"] = Policy.STAGE_NEW
+                return cls.do_mutate(PolicyConfig.gql_mutation_create_policies_perms, user, **data)
         except Exception as exc:
             return [{
                 'message': _("policy.mutation.failed_to_create_policy"),
-                'detail': str(exc)}]
+                'detail': str(exc),
+                'exc': exc}]
 
 
 class UpdatePolicyMutation(CreateRenewOrUpdatePolicyMutation):
     _mutation_module = "policy"
     _mutation_class = "UpdatePolicyMutation"
 
     class Input(PolicyInputType):
         pass
 
     @classmethod
     def async_mutate(cls, user, **data):
         try:
-            return cls.do_mutate(PolicyConfig.gql_mutation_edit_policies_perms, user, **data)
+            with transaction.atomic():
+                return cls.do_mutate(PolicyConfig.gql_mutation_edit_policies_perms, user, **data)
         except Exception as exc:
             return [{
                 'message': _("policy.mutation.failed_to_update_policy"),
-                'detail': str(exc)}]
+                'detail': str(exc),
+                'exc': exc}]
 
 
 class RenewPolicyMutation(CreateRenewOrUpdatePolicyMutation):
     _mutation_module = "policy"
     _mutation_class = "RenewPolicyMutation"
 
     class Input(PolicyInputType):
         pass
 
     @classmethod
     def async_mutate(cls, user, **data):
         try:
-            # ensure we don't update the existing one, but recreate a new one!
-            if 'policy_uuid' in data:
-                data.pop('policy_uuid')
-            data["status"] = Policy.STATUS_IDLE
-            data["stage"] = Policy.STAGE_RENEWED
-            return cls.do_mutate(PolicyConfig.gql_mutation_renew_policies_perms, user, **data)
+            with transaction.atomic():
+                # ensure we don't update the existing one, but recreate a new one!
+                if 'policy_uuid' in data:
+                    data.pop('policy_uuid')
+                data["status"] = Policy.STATUS_IDLE
+                data["stage"] = Policy.STAGE_RENEWED
+                return cls.do_mutate(PolicyConfig.gql_mutation_renew_policies_perms, user, **data)
         except Exception as exc:
             return [{
                 'message': _("policy.mutation.failed_to_renew_policy"),
-                'detail': str(exc)}]
+                'detail': str(exc),
+                'exc': exc}]
 
 
 class SuspendPoliciesMutation(OpenIMISMutation):
     _mutation_module = "policy"
     _mutation_class = "SuspendPolicyMutation"
 
     class Input(OpenIMISMutation.Input):
         uuids = graphene.List(graphene.String)
 
     @classmethod
     def async_mutate(cls, user, **data):
         try:
-            if type(user) is AnonymousUser or not user.id:
-                raise ValidationError(
-                    _("mutation.authentication_required"))
-            if not user.has_perms(PolicyConfig.gql_mutation_suspend_policies_perms):
-                raise PermissionDenied(_("unauthorized"))
-            errors = []
-            for policy_uuid in data["uuids"]:
-                policy = Policy.objects.filter(uuid=policy_uuid).first()
-                if policy is None:
-                    errors += {
-                        'title': policy_uuid,
-                        'list': [{'message': _(
-                            "policy.mutation.id_does_not_exist") % {'id': policy_uuid}}]
-                    }
-                    continue
-                errors += PolicyService(user).set_suspended(user, policy)
-            if len(errors) == 1:
-                errors = errors[0]['list']
-            return errors
+            with transaction.atomic():
+                if type(user) is AnonymousUser or not user.id:
+                    raise ValidationError(
+                        _("mutation.authentication_required"))
+                if not user.has_perms(PolicyConfig.gql_mutation_suspend_policies_perms):
+                    raise PermissionDenied(_("unauthorized"))
+                errors = []
+                for policy_uuid in data["uuids"]:
+                    policy = Policy.objects.filter(uuid=policy_uuid).first()
+                    if policy is None:
+                        errors += {
+                            'title': policy_uuid,
+                            'list': [{'message': _(
+                                "policy.mutation.id_does_not_exist") % {'id': policy_uuid}}]
+                        }
+                        continue
+                    errors += PolicyService(user).set_suspended(user, policy)
+                if len(errors) == 1:
+                    errors = errors[0]['list']
+                return errors
         except Exception as exc:
             return [{
                 'message': _("policy.mutation.failed_to_suspend_policy"),
-                'detail': str(exc)}]
+                'detail': str(exc),
+                'exc': exc}]
 
 
 class DeletePoliciesMutation(OpenIMISMutation):
     _mutation_module = "policy"
     _mutation_class = "DeletePoliciesMutation"
 
     class Input(OpenIMISMutation.Input):
         uuids = graphene.List(graphene.String)
 
     @classmethod
     def async_mutate(cls, user, **data):
-        if not user.has_perms(PolicyConfig.gql_mutation_delete_policies_perms):
-            raise PermissionDenied(_("unauthorized"))
-        errors = []
-        for policy_uuid in data["uuids"]:
-            policy = Policy.objects \
-                .filter(uuid=policy_uuid) \
-                .first()
-            if policy is None:
-                errors += {
-                    'title': policy_uuid,
-                    'list': [{'message': _(
-                        "policy.validation.id_does_not_exist") % {'id': policy_uuid}}]
-                }
-                continue
-            errors += PolicyService(user).set_deleted(policy)
-        if len(errors) == 1:
-            errors = errors[0]['list']
-        return errors
+        try:
+            with transaction.atomic():
+                if not user.has_perms(PolicyConfig.gql_mutation_delete_policies_perms):
+                    raise PermissionDenied(_("unauthorized"))
+                errors = []
+                for policy_uuid in data["uuids"]:
+                    policy = Policy.objects \
+                        .filter(uuid=policy_uuid) \
+                        .first()
+                    if policy is None:
+                        errors += {
+                            'title': policy_uuid,
+                            'list': [{'message': _(
+                                "policy.validation.id_does_not_exist") % {'id': policy_uuid}}]
+                        }
+                        continue
+                    errors += PolicyService(user).set_deleted(policy)
+                if len(errors) == 1:
+                    errors = errors[0]['list']
+                return errors
+        except Exception as exc:
+            return [{
+                'message': _("policy.mutation.failed_to_delete_policies"),
+                'detail': str(exc),
+                'exc': exc}]
```

### Comparing `openimis-be-policy-1.5.0/policy/gql_queries.py` & `openimis-be-policy-1.5.1/policy/gql_queries.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 import graphene
 from graphene_django import DjangoObjectType
+from django.utils.translation import gettext as _
+from .apps import PolicyConfig
 from .models import Policy
 from core import prefix_filterset, filter_validity, ExtendedConnection, ExtendedRelayConnection
 from core.schema import OfficerGQLType
 from product.schema import ProductGQLType
+from django.core.exceptions import PermissionDenied
 
 
 class PolicyGQLType(DjangoObjectType):
     sum_premiums = graphene.Float(source="sum_premiums")
 
     def resolve_family(self, info):
+        if not info.context.user.has_perms(PolicyConfig.gql_query_policies_perms):
+            raise PermissionDenied(_("unauthorized"))
         if "family_loader" in info.context.dataloaders and self.family_id:
             return info.context.dataloaders["family_loader"].load(self.family_id)
         return self.family
 
     def resolve_product(self, info):
+        if not info.context.user.has_perms(PolicyConfig.gql_query_policies_perms):
+            raise PermissionDenied(_("unauthorized"))
         if "product_loader" in info.context.dataloaders and self.product_id:
             return info.context.dataloaders["product_loader"].load(self.product_id)
         return self.product
 
     class Meta:
         model = Policy
         interfaces = (graphene.relay.Node,)
@@ -64,14 +71,15 @@
     ded_out_patient = graphene.Float()
     ceiling = graphene.Float()
     ceiling_in_patient = graphene.Float()
     ceiling_out_patient = graphene.Float()
     balance = graphene.Float()
     validity_from = graphene.Date()
     validity_to = graphene.Date()
+    max_installments = graphene.Int()
 
 
 class PolicyByFamilyOrInsureeConnection(ExtendedRelayConnection):
     class Meta:
         node = PolicyByFamilyOrInsureeGQLType
```

### Comparing `openimis-be-policy-1.5.0/policy/migrations/0001_initial.py` & `openimis-be-policy-1.5.1/policy/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policy-1.5.0/policy/migrations/0002_policy_renewals.py` & `openimis-be-policy-1.5.1/policy/migrations/0002_policy_renewals.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policy-1.5.0/policy/migrations/0003_auto_20201021_0811.py` & `openimis-be-policy-1.5.1/policy/migrations/0003_auto_20201021_0811.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policy-1.5.0/policy/models.py` & `openimis-be-policy-1.5.1/policy/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,27 +29,34 @@
                                 related_name="policies")
 
     offline = models.BooleanField(db_column='isOffline', blank=True, null=True)
     audit_user_id = models.IntegerField(db_column='AuditUserID')
     # row_id = models.BinaryField(db_column='RowID', blank=True, null=True)
 
     def sum_premiums(self, photo=False):
-        return sum([p.amount for p in self.premiums.filter(is_photo_fee=photo).all()])
+        return sum(
+            [
+                p.amount
+                for p in self.premiums.filter(
+                    is_photo_fee=photo, validity_to__isnull=True
+                ).all()
+            ]
+        )
 
     def claim_ded_rems(self):
         return self.claim_ded_rems
 
     def is_new(self):
         return not self.stage or self.stage == Policy.STAGE_NEW
 
     def can_add_insuree(self):
         return self.family.members.filter(validity_to__isnull=True).count() < self.product.max_members
 
     class Meta:
-        managed = False
+        managed = True
         db_table = 'tblPolicy'
 
     STATUS_IDLE = 1
     STATUS_ACTIVE = 2
     STATUS_SUSPENDED = 4
     STATUS_EXPIRED = 8
     STATUS_READY = 16
@@ -95,15 +102,15 @@
     renewal_warnings = models.SmallIntegerField(db_column='RenewalWarnings', null=True, blank=True, default=0)  # TODO choices
     response_status = models.IntegerField(db_column='ResponseStatus', null=True, blank=True, default=0)  # TODO Choices
     response_date = fields.DateTimeField(db_column='ResponseDate', null=True, blank=True)
 
     audit_user_id = models.IntegerField(db_column='AuditCreateUser', null=True, blank=True)
 
     class Meta:
-        managed = False
+        managed = True
         db_table = 'tblPolicyRenewals'
 
 
 class PolicyMutation(core_models.UUIDModel):
     policy = models.ForeignKey(Policy, models.DO_NOTHING,
                                  related_name='mutations')
     mutation = models.ForeignKey(
```

### Comparing `openimis-be-policy-1.5.0/policy/schema.py` & `openimis-be-policy-1.5.1/policy/schema.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from claim.apps import ClaimConfig
 from core.schema import (
     OrderedDjangoFilterConnectionField,
     signal_mutation_module_validate,
 )
 import graphene
 from django.core.exceptions import PermissionDenied
 from django.db.models import Prefetch
@@ -23,14 +24,15 @@
 
 # We do need all queries and mutations in the namespace here.
 from .gql_queries import *  # lgtm [py/polluting-import]
 from .gql_mutations import *  # lgtm [py/polluting-import]
 
 from .values import policy_values
 
+
 class Query(graphene.ObjectType):
     policy_values = graphene.Field(
         PolicyAndWarningsGQLType,
         prev_uuid=graphene.String(required=False),
         stage=graphene.String(required=True),
         enrollDate=graphene.DateTime(required=True),
         product_id=graphene.Int(required=True),
@@ -79,28 +81,43 @@
     )
     policy_service_eligibility_by_insuree = graphene.Field(
         EligibilityGQLType,
         chfId=graphene.String(required=True),
         serviceCode=graphene.String(required=True),
     )
     policy_officers = DjangoFilterConnectionField(
-        OfficerGQLType, search=graphene.String()
+        OfficerGQLType,
+        search=graphene.String(),
+        district=graphene.String(),
+        region=graphene.String(),
     )
 
     def resolve_policy_values(self, info, **kwargs):
-        product = Product.objects.get(id=kwargs.get('product_id'))
+        if not info.context.user.has_perms(PolicyConfig.gql_query_policies_perms):
+            raise PermissionDenied(_("unauthorized"))
+
+        product = Product.objects.filter(
+            Q(validity_to__isnull=True),
+            Q(id=kwargs.get('product_id')) | Q(legacy_id=kwargs.get('product_id')),
+            Q(validity_from__date__lte=kwargs.get('enrollDate')),
+        ).order_by('-validity_from').first()
+
+        if not product:
+            raise ValidationError('Provided product not available')
+
         policy = PolicyGQLType(
             stage=kwargs.get('stage'),
             enroll_date=kwargs.get('enrollDate'),
             start_date=kwargs.get('enrollDate'),
             product=product,
         )
         prefetch = Prefetch(
             'members',
-            queryset=Insuree.objects.filter(validity_to__isnull=True).order_by('validity_from')
+            queryset=Insuree.objects.filter(
+                validity_to__isnull=True).order_by('validity_from')
         )
         family = Family.objects \
             .prefetch_related(prefetch) \
             .get(id=kwargs.get('family_id'))
         prev_policy = None
         if 'prev_uuid' in kwargs:
             prev_policy = Policy.objects.get(uuid=kwargs.get('prev_uuid'))
@@ -117,26 +134,31 @@
             family_count = Insuree.objects.values('family_id')\
                 .filter(validity_to__isnull=True).annotate(m_count=Count('id'))
             family_sq = family_count.filter(family_id=OuterRef('family_id'))
             covered_count = InsureePolicy.objects.values('policy_id')\
                 .filter(validity_to__isnull=True).annotate(i_count=Count('id'))
             covered_sq = covered_count.filter(policy_id=OuterRef('id'))
             query = query.annotate(
-                inactive_count=Subquery(family_sq.values('m_count')) - Subquery(covered_sq.values('i_count'))
+                inactive_count=Subquery(family_sq.values(
+                    'm_count')) - Subquery(covered_sq.values('i_count'))
             )
             query = query.filter(inactive_count__gt=0)
         if kwargs.get('balance_lte') or kwargs.get('balance_gte'):
-            sum_premiums = Premium.objects.filter(is_photo_fee=False).values('policy_id').annotate(sum=Sum('amount'))
-            sum_premiums_subquery = sum_premiums.filter(policy_id=OuterRef('id'))
-            query = query.annotate(balance=F('value') - Subquery(sum_premiums_subquery.values('sum')))
+            sum_premiums = Premium.objects.filter(is_photo_fee=False).values(
+                'policy_id').annotate(sum=Sum('amount'))
+            sum_premiums_subquery = sum_premiums.filter(
+                policy_id=OuterRef('id'))
+            query = query.annotate(
+                balance=F('value') - Subquery(sum_premiums_subquery.values('sum')))
         if kwargs.get('balance_lte'):
             query = query.filter(balance__lte=kwargs.get('balance_lte'))
         if kwargs.get('balance_gte'):
             query = query.filter(balance__gte=kwargs.get('balance_gte'))
-        location_id = kwargs.get('district_id') if kwargs.get('district_id') else kwargs.get('region_id')
+        location_id = kwargs.get('district_id') if kwargs.get(
+            'district_id') else kwargs.get('region_id')
         if location_id:
             location_level = 2 if kwargs.get('district_id') else 1
             f = '_id'
             for i in range(len(LocationConfig.location_types) - location_level):
                 f = "__parent" + f
             f = PolicyConfig.policy_location_via + '__location' + f
             query = query.filter(Q(**{f: location_id}))
@@ -161,35 +183,39 @@
             ded_in_patient=item.ded_in_patient,
             ded_out_patient=item.ded_out_patient,
             ceiling=item.ceiling,
             ceiling_in_patient=item.ceiling_in_patient,
             ceiling_out_patient=item.ceiling_out_patient,
             balance=item.balance,
             validity_from=item.validity_from,
-            validity_to=item.validity_to
+            validity_to=item.validity_to,
+            max_installments=item.max_installments,
         )
 
     def resolve_policies_by_insuree(self, info, **kwargs):
-        if not info.context.user.has_perms(PolicyConfig.gql_query_policies_by_insuree_perms):
+        if not info.context.user.has_perms(PolicyConfig.gql_query_policies_by_insuree_perms) \
+                and not info.context.user.has_perms(ClaimConfig.gql_query_claims_perms):
             raise PermissionDenied(_("unauthorized"))
         req = ByInsureeRequest(
             chf_id=kwargs.get('chf_id'),
-            active_or_last_expired_only=kwargs.get('active_or_last_expired_only', False),
+            active_or_last_expired_only=kwargs.get(
+                'active_or_last_expired_only', False),
             show_history=kwargs.get('show_history', False),
             order_by=kwargs.get('order_by', None)
         )
         res = ByInsureeService(user=info.context.user).request(req)
         return [Query._to_policy_by_family_or_insuree_item(x) for x in res.items]
 
     def resolve_policies_by_family(self, info, **kwargs):
         if not info.context.user.has_perms(PolicyConfig.gql_query_policies_by_family_perms):
             raise PermissionDenied(_("unauthorized"))
         req = ByFamilyRequest(
             family_uuid=kwargs.get('family_uuid'),
-            active_or_last_expired_only=kwargs.get('active_or_last_expired_only', False),
+            active_or_last_expired_only=kwargs.get(
+                'active_or_last_expired_only', False),
             show_history=kwargs.get('show_history', False),
             order_by=kwargs.get('order_by', None)
         )
         res = ByFamilyService(user=info.context.user).request(req)
         return [Query._to_policy_by_family_or_insuree_item(x) for x in res.items]
 
     @staticmethod
@@ -247,29 +273,50 @@
             service_code=kwargs.get('serviceCode')
         )
         return Query._resolve_policy_eligibility_by_insuree(
             user=info.context.user,
             req=req
         )
 
-    def resolve_policy_officers(self, info, search=None, **kwargs):
+    def resolve_policy_officers(
+            self,
+            info,
+            search=None,
+            district=None,
+            region=None,
+            **kwargs
+    ):
         if not info.context.user.has_perms(
             PolicyConfig.gql_query_policy_officers_perms
         ):
             raise PermissionDenied(_("unauthorized"))
+        queryset = Officer.objects
+        location_id = district if district else region
+
+        if location_id is not None:
+            location = int(location_id)
+            queryset = queryset.filter(
+                Q(officer_villages__location__isnull=False,
+                  officer_villages__location__id=location)  # villages
+                | Q(officer_villages__location__parent_id__isnull=False,
+                    officer_villages__location__parent_id=location)  # municipalities
+                | Q(officer_villages__location__parent__parent_id__isnull=False,
+                    officer_villages__location__parent__parent_id=location)  # districts
+                | Q(officer_villages__location__parent__parent__parent_id__isnull=False,
+                    officer_villages__location__parent__parent__parent_id=location)  # regions
+            ).distinct()
 
-        qs = Officer.objects
         if search is not None:
-            qs = qs.filter(
+            queryset = queryset.filter(
                 Q(code__icontains=search)
                 | Q(last_name__icontains=search)
                 | Q(other_names__icontains=search)
             )
 
-        return qs
+        return queryset
 
 
 class Mutation(graphene.ObjectType):
     create_policy = CreatePolicyMutation.Field()
     update_policy = UpdatePolicyMutation.Field()
     delete_policies = DeletePoliciesMutation.Field()
     renew_policy = RenewPolicyMutation.Field()
@@ -281,13 +328,14 @@
     if not uuids:
         uuid = kwargs['data'].get('policy_uuid', None)
         uuids = [uuid] if uuid else []
     if not uuids:
         return []
     impacted_policies = Policy.objects.filter(uuid__in=uuids).all()
     for policy in impacted_policies:
-        PolicyMutation.objects.create(policy=policy, mutation_id=kwargs['mutation_log_id'])
+        PolicyMutation.objects.create(
+            policy=policy, mutation_id=kwargs['mutation_log_id'])
     return []
 
 
 def bind_signals():
     signal_mutation_module_validate["policy"].connect(on_policy_mutation)
```

### Comparing `openimis-be-policy-1.5.0/policy/services.py` & `openimis-be-policy-1.5.1/policy/services.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import core
 from claim.models import ClaimService, Claim, ClaimItem
 from django import dispatch
 from django.core.exceptions import PermissionDenied
 from django.db import connection
 from django.db.models import Q, Count, Min, Max, Value
-from django.db.models import Sum, F
+from django.db.models import Sum, F, Case, When
 from django.db.models.functions import Coalesce
 from django.template import Template, Context
 from django.utils.translation import gettext as _
 from graphene.utils.str_converters import to_snake_case
 from core.signals import register_service_signal
 from insuree.models import Insuree, Family, InsureePolicy
 from insuree.services import create_insuree_renewal_detail
@@ -87,14 +87,17 @@
                 'list': [{
                     'message': _("policy.mutation.failed_to_suspend_policy") % {'uuid': policy.uuid},
                     'detail': policy.uuid}]
             }
 
     def set_deleted(self, policy):
         try:
+            insuree_policies = InsureePolicy.objects.filter(policy=policy)
+            for insuree_policy in insuree_policies:
+                insuree_policy.delete_history()
             policy.delete_history()
             return []
         except Exception as exc:
             return {
                 'title': policy.uuid,
                 'list': [{
                     'message': _("policy.mutation.failed_to_change_status_of_policy") % {'policy': str(policy)},
@@ -135,15 +138,16 @@
                  ded_in_patient,
                  ded_out_patient,
                  ceiling,
                  ceiling_in_patient,
                  ceiling_out_patient,
                  balance,
                  validity_from,
-                 validity_to
+                 validity_to,
+                 max_installments
                  ):
         self.policy_id = policy_id
         self.policy_uuid = policy_uuid
         self.policy_value = policy_value
         self.product_code = product_code
         self.product_name = product_name
         self.start_date = start_date
@@ -158,14 +162,15 @@
         self.ded_out_patient = ded_out_patient
         self.ceiling = ceiling
         self.ceiling_in_patient = ceiling_in_patient
         self.ceiling_out_patient = ceiling_out_patient
         self.balance = balance
         self.validity_from = validity_from
         self.validity_to = validity_to
+        self.max_installments = max_installments
 
     def __eq__(self, other):
         return isinstance(other, self.__class__) and self.__dict__ == other.__dict__
 
 
 @core.comparable
 class ByInsureeResponse(object):
@@ -196,21 +201,41 @@
         if row.product.max_insuree:
             ceiling = row.product.max_insuree - (row.total_rem_g if row.total_rem_g else 0)
         else:
             if row.product.max_ip_insuree:
                 ceiling_ip = row.product.max_ip_insuree - (row.total_rem_ip if row.total_rem_ip else 0)
             if row.product.max_op_insuree:
                 ceiling_op = row.product.max_op_insuree - (row.total_rem_op if row.total_rem_op else 0)
+
+        members_count = row.family.members.count()
+        threshold = row.product.threshold
+        total_rem_g = row.total_rem_g if row.total_rem_g else 0
+        total_rem_ip = row.total_rem_ip if row.total_rem_ip else 0
+        total_rem_op = row.total_rem_op if row.total_rem_op else 0
+
         if row.product.max_policy:
-            ceiling = row.product.max_policy - (row.total_rem_g if row.total_rem_g else 0)
+            max_policy = row.product.max_policy
+            if members_count > threshold:
+                max_policy += (members_count - threshold) * row.product.max_policy_extra_member
+            ceiling = max_policy - total_rem_g
         else:
+            ceiling_ip = 0
             if row.product.max_ip_policy:
-                ceiling_ip = row.product.max_ip_policy - (row.total_rem_ip if row.total_rem_ip else 0)
+                max_ip_policy = row.product.max_ip_policy
+                if members_count > threshold:
+                    max_ip_policy += (members_count - threshold) * row.product.max_policy_extra_member_ip
+                ceiling_ip = max_ip_policy - total_rem_ip
+
+            ceiling_op = 0
             if row.product.max_op_policy:
-                ceiling_op = row.product.max_op_policy - (row.total_rem_op if row.total_rem_op else 0)
+                max_op_policy = row.product.max_op_policy
+                if members_count > threshold:
+                    max_op_policy += (members_count - threshold) * row.product.max_policy_extra_member_op
+                ceiling_op = max_op_policy - total_rem_op
+
         balance = row.value
         if row.total_ded_g:
             balance -= row.total_ded_g
 
         return ByFamilyOrInsureeResponseItem(
             policy_id=row.id,
             policy_uuid=row.uuid,
@@ -228,15 +253,16 @@
             ded_in_patient=row.total_ded_ip,
             ded_out_patient=row.total_ded_op,
             ceiling=ceiling,
             ceiling_in_patient=ceiling_ip,
             ceiling_out_patient=ceiling_op,
             balance=balance,
             validity_from=row.validity_from,
-            validity_to=row.validity_to
+            validity_to=row.validity_to,
+            max_installments=row.product.max_installments,
         )
 
     def build_query(self, req):
         # TODO: prevent direct dependency on claim_ded structure?
         res = Policy.objects \
             .select_related('product') \
             .select_related('officer') \
@@ -530,123 +556,93 @@
             )
 
 
 class NativeEligibilityService(object):
     def __init__(self, user):
         self.user = user
 
+
+    def get_eligibility(self, insuree, item_or_service, model, req, now):
+        if insuree.is_adult():
+            waiting_period_field = f"policy__product__{item_or_service}s__waiting_period_adult"
+            limit_field = f"policy__product__{item_or_service}s__limit_no_adult"
+        else:
+            waiting_period_field = f"policy__product__{item_or_service}s__waiting_period_child"
+            limit_field = f"policy__product__{item_or_service}s__limit_no_child"
+
+        item_or_service_code = req.service_code
+        if item_or_service == "item":
+            item_or_service_code = req.item_code
+
+        # TODO validity is checked but should be optional in get_queryset
+        item_or_service_obj = model.get_queryset(None, self.user).get(code__iexact=item_or_service_code)
+
+        # Beware that MonthAdd() is in Gregorian calendar, not Nepalese or anything else
+        queryset_item_or_service = InsureePolicy.objects\
+            .filter(validity_to__isnull=True)\
+            .filter(policy__validity_to__isnull=True)\
+            .filter(**{f"policy__product__{item_or_service}s__validity_to__isnull": True},
+                    **{f"policy__product__{item_or_service}s__{item_or_service}_id": item_or_service_obj.id}) \
+            .filter(policy__status=Policy.STATUS_ACTIVE) \
+            .filter(insuree=insuree) \
+            .filter(Q(insuree__claim__validity_to__isnull=True,
+                      **{f"insuree__claim__{item_or_service}s__{item_or_service}_id": item_or_service_obj.id})
+                    & Q(**{f"insuree__claim__{item_or_service}s__validity_to__isnull": True})
+                    & (Q(**{f"insuree__claim__{item_or_service}s__status": ClaimItem.STATUS_PASSED})
+                       | Q(**{f"insuree__claim__{item_or_service}s__status__isnull": True}))
+                    & (Q(insuree__claim__status__gt=Claim.STATUS_ENTERED)
+                       | Q(insuree__claim__status__isnull=True))) \
+            .values("effective_date",
+                    "policy__product_id",
+                    waiting_period=F(waiting_period_field),
+                    limit_no=F(limit_field)) \
+            .annotate(min_date=MonthsAdd(Coalesce(F(waiting_period_field), 0), "effective_date")) \
+            .annotate(count=Sum(Coalesce(
+                                f"insuree__claim__{item_or_service}s__qty_approved",
+                                f'insuree__claim__{item_or_service}s__qty_provided'
+                            ))) \
+            .annotate(left=F("limit_no") - F("count"))
+
+        min_date_qs = queryset_item_or_service.aggregate(
+            min_date_lte=Min("min_date", filter=Q(min_date__lte=now)),
+            min_date_all=Min("min_date"),
+        )
+        from core import datetime
+        min_date_item = datetime.date.from_ad_date(min_date_qs["min_date_lte"]
+                                                   if min_date_qs["min_date_lte"]
+                                                   else min_date_qs["min_date_all"])
+
+        if queryset_item_or_service.filter(min_date__lte=now).filter(left__isnull=True).first():
+            items_or_services_left = None
+        else:
+            items_or_services_left = queryset_item_or_service\
+                .filter(Q(min_date__isnull=True) | Q(min_date__lte=now))\
+                .aggregate(Max("left"))["left__max"]
+
+        return item_or_service_obj, min_date_item, items_or_services_left
+
+
     def request(self, req, response):
         insuree = Insuree.get_queryset(None, self.user)\
             .filter(validity_to__isnull=True)\
             .get(chf_id=req.chf_id)  # Will throw an exception if not found
         now = core.datetime.datetime.now()
         eligibility = response
 
         if req.service_code:
-            if insuree.is_adult():
-                waiting_period_field = "policy__product__services__waiting_period_adult"
-                limit_field = "policy__product__services__limit_no_adult"
-            else:
-                waiting_period_field = "policy__product__services__waiting_period_child"
-                limit_field = "policy__product__services__limit_no_child"
-
-            # TODO validity is checked but should be optional in get_queryset
-            service = Service.get_queryset(None, self.user).get(code__iexact=req.service_code)
-
-            # Beware that MonthAdd() is in Gregorian calendar, not Nepalese or anything else
-            queryset_svc = InsureePolicy.objects\
-                .filter(validity_to__isnull=True)\
-                .filter(policy__validity_to__isnull=True) \
-                .filter(policy__product__services__validity_to__isnull=True,
-                        policy__product__services__service_id=service.id) \
-                .filter(policy__status=Policy.STATUS_ACTIVE) \
-                .filter(insuree=insuree) \
-                .filter(Q(insuree__claim__validity_to__isnull=True)
-                        & Q(insuree__claim__services__validity_to__isnull=True)
-                        & (Q(insuree__claim__services__status=ClaimService.STATUS_PASSED)
-                            | Q(insuree__claim__services__status__isnull=True))
-                        & (Q(insuree__claim__status__gt=Claim.STATUS_ENTERED)
-                           | Q(insuree__claim__status__isnull=True))) \
-                .values("effective_date",
-                        "policy__product_id",
-                        waiting_period=F(waiting_period_field),
-                        limit_no=F(limit_field))\
-                .annotate(min_date=MonthsAdd(Coalesce(F(waiting_period_field), 0), "effective_date"))\
-                .annotate(services_count=Count("policy__product__services__service_id"))\
-                .annotate(services_left=F("limit_no") - F("services_count"))
-
-            min_date_qs = queryset_svc.aggregate(
-                min_date_lte=Min("min_date", filter=Q(min_date__lte=now)),
-                min_date_all=Min("min_date"),
-            )
-            from core import datetime
-            min_date_service = datetime.date.from_ad_date(
-                min_date_qs["min_date_lte"] if min_date_qs["min_date_lte"]
-                else min_date_qs["min_date_all"])
-
-            if queryset_svc.filter(min_date__lte=now).filter(services_left__isnull=True).first():
-                services_left = None
-            else:
-                services_left = queryset_svc\
-                    .filter(Q(min_date__isnull=True) | Q(min_date__lte=now))\
-                    .aggregate(Max("services_left"))["services_left__max"]
+            service, min_date_service, services_left = self.get_eligibility(insuree, "service", Service, req, now)
         else:
             service = None
             services_left = None
             min_date_service = None
         eligibility.min_date_service = min_date_service
         eligibility.service_left = services_left
 
-        # TODO remove code duplication between service and item
         if req.item_code:
-            if insuree.is_adult():
-                waiting_period_field = "policy__product__items__waiting_period_adult"
-                limit_field = "policy__product__items__limit_no_adult"
-            else:
-                waiting_period_field = "policy__product__items__waiting_period_child"
-                limit_field = "policy__product__items__limit_no_child"
-
-            item = Item.get_queryset(None, self.user).get(code__iexact=req.item_code)
-
-            queryset_item = InsureePolicy.objects\
-                .filter(validity_to__isnull=True)\
-                .filter(policy__validity_to__isnull=True)\
-                .filter(policy__product__items__validity_to__isnull=True,
-                        policy__product__items__item_id=item.id) \
-                .filter(policy__status=Policy.STATUS_ACTIVE) \
-                .filter(insuree=insuree) \
-                .filter(Q(insuree__claim__validity_to__isnull=True)
-                        & Q(insuree__claim__items__validity_to__isnull=True)
-                        & (Q(insuree__claim__items__status=ClaimItem.STATUS_PASSED)
-                            | Q(insuree__claim__items__status__isnull=True))
-                        & (Q(insuree__claim__status__gt=Claim.STATUS_ENTERED)
-                           | Q(insuree__claim__status__isnull=True))) \
-                .values("effective_date",
-                        "policy__product_id",
-                        waiting_period=F(waiting_period_field),
-                        limit_no=F(limit_field))\
-                .annotate(min_date=MonthsAdd(Coalesce(F(waiting_period_field), 0), "effective_date"))\
-                .annotate(items_count=Count("policy__product__items__item_id")) \
-                .annotate(items_left=F("limit_no") - F("items_count"))
-
-            min_date_qs = queryset_item.aggregate(
-                min_date_lte=Min("min_date", filter=Q(min_date__lte=now)),
-                min_date_all=Min("min_date"),
-            )
-            from core import datetime
-            min_date_item = datetime.date.from_ad_date(min_date_qs["min_date_lte"]
-                                                       if min_date_qs["min_date_lte"]
-                                                       else min_date_qs["min_date_all"])
-
-            if queryset_item.filter(min_date__lte=now).filter(items_left__isnull=True).first():
-                items_left = None
-            else:
-                items_left = queryset_item\
-                    .filter(Q(min_date__isnull=True) | Q(min_date__lte=now))\
-                    .aggregate(Max("items_left"))["items_left__max"]
+            item, min_date_item, items_left = self.get_eligibility(insuree, "item", Item, req, now)
         else:
             item = None
             items_left = None
             min_date_item = None
         eligibility.min_date_item = min_date_item
         eligibility.item_left = items_left
```

### Comparing `openimis-be-policy-1.5.0/policy/tasks.py` & `openimis-be-policy-1.5.1/policy/tasks.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policy-1.5.0/policy/test_services.py` & `openimis-be-policy-1.5.1/policy/test_services.py`

 * *Files 8% similar despite different names*

```diff
@@ -74,14 +74,15 @@
                 service_left=20,
                 item_left=21,
                 is_item_ok=True,
                 is_service_ok=True,
             )
             self.assertEquals(expected, res)
 
+    @skip("skip test that uses sp")
     def test_eligibility_sp_call(self):
         mock_user = mock.Mock(is_anonymous=False)
         mock_user.has_perm = mock.MagicMock(return_value=True)
         req = EligibilityRequest(chf_id="070707070")
         service = StoredProcEligibilityService(mock_user)
         res = service.request(req, EligibilityResponse(req))
         expected = EligibilityResponse(
@@ -112,76 +113,113 @@
             Service.CATEGORY_SURGERY,
             Service.CATEGORY_CONSULTATION,
             Service.CATEGORY_HOSPITALIZATION,
             Service.CATEGORY_OTHER,
             Service.CATEGORY_ANTENATAL,
         ]:
             with self.subTest(category=category):
-                self.eligibility_stored_proc_serv(category)
+                self.eligibility_serv(category)
 
-    def eligibility_stored_proc_serv(self, category):
+    def eligibility_serv(self, category):
         insuree = create_test_insuree(custom_props={"chf_id": "elgsp" + category})
         product = create_test_product("ELI1")
         (policy, insuree_policy) = create_test_policy2(product, insuree)
         service = create_test_service(category)
         svc_pl_detail = add_service_to_hf_pricelist(service)
         product_service = create_test_product_service(product, service, custom_props={"limit_no_adult": 20})
         claim = create_test_claim(custom_props={"insuree_id": insuree.id})
         claim_service = create_test_claimservice(claim, custom_props={"service_id": service.id})
         errors = validate_claim(claim, True)
         errors += validate_assign_prod_to_claimitems_and_services(claim)
         errors += process_dedrem(claim, -1, True)
         self.assertEqual(len(errors), 0)
 
-        sp_el_svc = StoredProcEligibilityService(self.user)
         native_el_svc = NativeEligibilityService(self.user)
         req = EligibilityRequest(chf_id=insuree.chf_id, service_code=service.code)
+        expected_resposnse = EligibilityResponse(
+            antenatal_amount_left=None,
+            consultation_amount_left=None,
+            delivery_amount_left=None,
+            eligibility_request=req,
+            final=False,
+            hospitalization_amount_left=None,
+            is_item_ok=True,
+            is_service_ok=True,
+            item_left=None,
+            min_date_item=core.datetime.date(2019, 3, 1),
+            min_date_service=None,
+            prod_id=product.id,
+            service_left=13.00,
+            surgery_amount_left=None,
+            total_visits_left=None,
+            total_antenatal_left=None,
+            total_surgeries_left=None,
+            total_admissions_left=None,
+            total_deliveries_left=None,
+            total_consultations_left=None,
+        )
         settings.ROW_SECURITY = False
         native_response = native_el_svc.request(req, EligibilityResponse(req))
-        sp_response = sp_el_svc.request(req, EligibilityResponse(req))
         self.assertIsNotNone(native_response)
-        self.assertIsNotNone(sp_response)
-        self.assertEquals(native_response, sp_response)
+        self.assertEquals(native_response, expected_resposnse)
 
         claim.dedrems.all().delete()
         claim_service.delete()
         claim.delete()
         product_service.delete()
         svc_pl_detail.delete()
         service.delete()
         policy.insuree_policies.all().delete()
         policy.delete()
         product.delete()
         insuree.delete()
 
-    def test_eligibility_stored_proc_item(self):
+    def test_eligibility_item(self):
         insuree = create_test_insuree()
         product = create_test_product("ELI1")
         (policy, insuree_policy) = create_test_policy2(product, insuree)
         item = create_test_item("A")
         item_pl_detail = add_item_to_hf_pricelist(item)
         product_item = create_test_product_item(product, item, custom_props={"limit_no_adult": 12})
         claim = create_test_claim(custom_props={"insuree_id": insuree.id})
         claim_item = create_test_claimitem(claim, "A", custom_props={"item_id": item.id})
         errors = validate_claim(claim, True)
         errors += validate_assign_prod_to_claimitems_and_services(claim)
         errors += process_dedrem(claim, -1, True)
         self.assertEqual(len(errors), 0)
 
-        sp_el_svc = StoredProcEligibilityService(self.user)
         native_el_svc = NativeEligibilityService(self.user)
         req = EligibilityRequest(chf_id=insuree.chf_id, item_code=item.code)
+        expected_resposnse = EligibilityResponse(
+            antenatal_amount_left=None,
+            consultation_amount_left=None,
+            delivery_amount_left=None,
+            eligibility_request=req,
+            final=False,
+            hospitalization_amount_left=None,
+            is_item_ok=True,
+            is_service_ok=True,
+            item_left=5.00,
+            min_date_item=core.datetime.date(2019, 3, 1),
+            min_date_service=None,
+            prod_id=product.id,
+            service_left=None,
+            surgery_amount_left=None,
+            total_visits_left=None,
+            total_antenatal_left=None,
+            total_surgeries_left=None,
+            total_admissions_left=None,
+            total_deliveries_left=None,
+            total_consultations_left=None,
+        )
         settings.ROW_SECURITY = False
         native_response = EligibilityResponse(req)
         native_response = native_el_svc.request(req, native_response)
-        sp_response = EligibilityResponse(req)
-        sp_response = sp_el_svc.request(req, sp_response)
         self.assertIsNotNone(native_response)
-        self.assertIsNotNone(sp_response)
-        self.assertEquals(native_response, sp_response)
+        self.assertEquals(native_response, expected_resposnse)
 
         claim.dedrems.all().delete()
         claim_item.delete()
         claim.delete()
         product_item.delete()
         item_pl_detail.delete()
         item.delete()
@@ -200,25 +238,43 @@
         claim = create_test_claim(custom_props={"insuree_id": insuree.id})
         claim_item = create_test_claimitem(claim, "A", custom_props={"item_id": item.id})
         errors = validate_claim(claim, True)
         errors += validate_assign_prod_to_claimitems_and_services(claim)
         errors += process_dedrem(claim, -1, True)
         self.assertEqual(len(errors), 0)
 
-        sp_el_svc = StoredProcEligibilityService(self.user)
         native_el_svc = NativeEligibilityService(self.user)
         req = EligibilityRequest(chf_id=insuree.chf_id, item_code=item.code)
+        expected_resposnse = EligibilityResponse(
+            antenatal_amount_left=None,
+            consultation_amount_left=None,
+            delivery_amount_left=None,
+            eligibility_request=req,
+            final=False,
+            hospitalization_amount_left=None,
+            is_item_ok=True,
+            is_service_ok=True,
+            item_left=5.00,
+            min_date_item=core.datetime.date(2019, 3, 1),
+            min_date_service=None,
+            prod_id=product.id,
+            service_left=None,
+            surgery_amount_left=None,
+            total_visits_left=None,
+            total_antenatal_left=None,
+            total_surgeries_left=None,
+            total_admissions_left=None,
+            total_deliveries_left=None,
+            total_consultations_left=None,
+        )
         settings.ROW_SECURITY = False
         native_response = EligibilityResponse(req)
         native_response = native_el_svc.request(req, native_response)
-        sp_response = EligibilityResponse(req)
-        sp_response = sp_el_svc.request(req, sp_response)
         self.assertIsNotNone(native_response)
-        self.assertIsNotNone(sp_response)
-        self.assertEquals(native_response, sp_response)
+        self.assertEquals(native_response, expected_resposnse)
 
         claim.dedrems.all().delete()
         claim_item.delete()
         claim.delete()
         product_item.delete()
         item_pl_detail.delete()
         item.delete()
```

### Comparing `openimis-be-policy-1.5.0/policy/test_values.py` & `openimis-be-policy-1.5.1/policy/test_values.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policy-1.5.0/policy/utils.py` & `openimis-be-policy-1.5.1/policy/utils.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policy-1.5.0/policy/validations.py` & `openimis-be-policy-1.5.1/policy/validations.py`

 * *Files identical despite different names*

### Comparing `openimis-be-policy-1.5.0/policy/values.py` & `openimis-be-policy-1.5.1/policy/values.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from django.utils.translation import gettext as _
 import datetime as py_datetime
+from decimal import *
 from core.apps import CoreConfig
 from .models import Policy
 
 
 def cycle_start(product, cycle, ref_date):
     c = getattr(product, "start_cycle_%s" % (cycle + 1), None)
     if not c:
@@ -164,15 +165,15 @@
 
 def set_value(policy, family, prev_policy):
     product = policy.product
     f_counts = family_counts(policy.product, family)
     contributions = sum_contributions(product, f_counts)
     general_assembly = sum_general_assemblies(product, f_counts)
     registration = sum_registrations(policy, product, f_counts)
-    policy.value = contributions + general_assembly + registration
+    policy.value = Decimal(contributions + general_assembly + registration)
     discount(policy, prev_policy)
 
 
 def policy_values(policy, family, prev_policy):
     members = family.members.filter(validity_to__isnull=True).count()
     max_members = policy.product.max_members
     above_max = max(0, members - max_members)
```

### Comparing `openimis-be-policy-1.5.0/setup.py` & `openimis-be-policy-1.5.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='openimis-be-policy',
-    version='1.5.0',
+    version='v1.5.1',
     packages=find_packages(),
     include_package_data=True,
     license='GNU AGPL v3',
     description='The openIMIS Backend Policy reference module.',
     # long_description=README,
     url='https://openimis.org/',
     author='Xavier Gillmann',
```

