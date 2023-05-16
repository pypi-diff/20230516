# Comparing `tmp/openimis-be-calculation-1.5.0.tar.gz` & `tmp/openimis-be-calculation-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis-be-calculation-1.5.0.tar", last modified: Fri Nov 11 08:11:49 2022, max compression
+gzip compressed data, was "openimis-be-calculation-1.5.1.tar", last modified: Tue May 16 21:38:34 2023, max compression
```

## Comparing `openimis-be-calculation-1.5.0.tar` & `openimis-be-calculation-1.5.1.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:11:49.718345 openimis-be-calculation-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1854 2022-11-11 08:11:39.000000 openimis-be-calculation-1.5.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)     2666 2022-11-11 08:11:49.718345 openimis-be-calculation-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1929 2022-11-11 08:11:39.000000 openimis-be-calculation-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:11:49.718345 openimis-be-calculation-1.5.0/calculation/
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-11-11 08:11:39.000000 openimis-be-calculation-1.5.0/calculation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-11-11 08:11:39.000000 openimis-be-calculation-1.5.0/calculation/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)     1321 2022-11-11 08:11:39.000000 openimis-be-calculation-1.5.0/calculation/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)    13231 2022-11-11 08:11:39.000000 openimis-be-calculation-1.5.0/calculation/calculation_rule.py
--rw-r--r--   0 runner    (1001) docker     (121)     5923 2022-11-11 08:11:39.000000 openimis-be-calculation-1.5.0/calculation/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:11:49.718345 openimis-be-calculation-1.5.0/calculation/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     9423 2022-11-11 08:11:39.000000 openimis-be-calculation-1.5.0/calculation/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)     2805 2022-11-11 08:11:39.000000 openimis-be-calculation-1.5.0/calculation/migrations/0002_auto_20210118_1426.py
--rw-r--r--   0 runner    (1001) docker     (121)      493 2022-11-11 08:11:39.000000 openimis-be-calculation-1.5.0/calculation/migrations/0003_add_calculation_roles_for_admin.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-11 08:11:39.000000 openimis-be-calculation-1.5.0/calculation/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-11 08:11:39.000000 openimis-be-calculation-1.5.0/calculation/models.py
--rw-r--r--   0 runner    (1001) docker     (121)    10464 2022-11-11 08:11:39.000000 openimis-be-calculation-1.5.0/calculation/schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     2720 2022-11-11 08:11:39.000000 openimis-be-calculation-1.5.0/calculation/services.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:11:49.718345 openimis-be-calculation-1.5.0/calculation/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-11-11 08:11:39.000000 openimis-be-calculation-1.5.0/calculation/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-11 08:11:39.000000 openimis-be-calculation-1.5.0/calculation/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-11 08:11:39.000000 openimis-be-calculation-1.5.0/calculation/tests/helpers_tests.py
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-11-11 08:11:39.000000 openimis-be-calculation-1.5.0/calculation/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-11-11 08:11:39.000000 openimis-be-calculation-1.5.0/calculation/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 08:11:49.718345 openimis-be-calculation-1.5.0/openimis_be_calculation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2666 2022-11-11 08:11:49.000000 openimis-be-calculation-1.5.0/openimis_be_calculation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      772 2022-11-11 08:11:49.000000 openimis-be-calculation-1.5.0/openimis_be_calculation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-11 08:11:49.000000 openimis-be-calculation-1.5.0/openimis_be_calculation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-11-11 08:11:49.000000 openimis-be-calculation-1.5.0/openimis_be_calculation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-11-11 08:11:49.000000 openimis-be-calculation-1.5.0/openimis_be_calculation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-11 08:11:49.718345 openimis-be-calculation-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1242 2022-11-11 08:11:47.000000 openimis-be-calculation-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:34.146304 openimis-be-calculation-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-16 21:38:24.000000 openimis-be-calculation-1.5.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-05-16 21:38:34.146304 openimis-be-calculation-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-16 21:38:24.000000 openimis-be-calculation-1.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:34.142304 openimis-be-calculation-1.5.1/calculation/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-16 21:38:24.000000 openimis-be-calculation-1.5.1/calculation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-16 21:38:24.000000 openimis-be-calculation-1.5.1/calculation/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-16 21:38:24.000000 openimis-be-calculation-1.5.1/calculation/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6812 2023-05-16 21:38:24.000000 openimis-be-calculation-1.5.1/calculation/calculation_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-05-16 21:38:24.000000 openimis-be-calculation-1.5.1/calculation/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:34.146304 openimis-be-calculation-1.5.1/calculation/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     9423 2023-05-16 21:38:24.000000 openimis-be-calculation-1.5.1/calculation/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-05-16 21:38:24.000000 openimis-be-calculation-1.5.1/calculation/migrations/0002_auto_20210118_1426.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-16 21:38:24.000000 openimis-be-calculation-1.5.1/calculation/migrations/0003_add_calculation_roles_for_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-05-16 21:38:24.000000 openimis-be-calculation-1.5.1/calculation/migrations/0004_auto_20230126_0903.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:24.000000 openimis-be-calculation-1.5.1/calculation/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:24.000000 openimis-be-calculation-1.5.1/calculation/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10497 2023-05-16 21:38:24.000000 openimis-be-calculation-1.5.1/calculation/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-05-16 21:38:24.000000 openimis-be-calculation-1.5.1/calculation/services.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:34.146304 openimis-be-calculation-1.5.1/calculation/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-16 21:38:24.000000 openimis-be-calculation-1.5.1/calculation/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:24.000000 openimis-be-calculation-1.5.1/calculation/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:24.000000 openimis-be-calculation-1.5.1/calculation/tests/helpers_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-16 21:38:24.000000 openimis-be-calculation-1.5.1/calculation/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-16 21:38:24.000000 openimis-be-calculation-1.5.1/calculation/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:38:34.146304 openimis-be-calculation-1.5.1/openimis_be_calculation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-05-16 21:38:34.000000 openimis-be-calculation-1.5.1/openimis_be_calculation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-16 21:38:34.000000 openimis-be-calculation-1.5.1/openimis_be_calculation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 21:38:34.000000 openimis-be-calculation-1.5.1/openimis_be_calculation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-16 21:38:34.000000 openimis-be-calculation-1.5.1/openimis_be_calculation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-16 21:38:34.000000 openimis-be-calculation-1.5.1/openimis_be_calculation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 21:38:34.146304 openimis-be-calculation-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-16 21:38:33.000000 openimis-be-calculation-1.5.1/setup.py
```

### Comparing `openimis-be-calculation-1.5.0/LICENSE.md` & `openimis-be-calculation-1.5.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openimis-be-calculation-1.5.0/PKG-INFO` & `openimis-be-calculation-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-calculation
-Version: 1.5.0
+Version: 1.5.1
 Summary: The openIMIS Backend Calculation reference module.
 Home-page: https://openimis.org/
 Author: Damian Borowiecki
 Author-email: dborowiecki@soldevelo.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-calculation-1.5.0/README.md` & `openimis-be-calculation-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `openimis-be-calculation-1.5.0/calculation/apps.py` & `openimis-be-calculation-1.5.1/calculation/apps.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calculation-1.5.0/calculation/calculation_rule.py` & `openimis-be-calculation-1.5.1/calculation/calculation_rule.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 
 from .apps import AbsCalculationRule
-from .config import CLASS_RULE_PARAM_VALIDATION, CLASS_RULE_PARAM_VALIDATION2, \
+from .config import CLASS_RULE_PARAM_VALIDATION, \
     DESCRIPTION_CONTRIBUTION_VALUATION, FROM_TO
 from contribution_plan.models import ContributionPlanBundleDetails
 from core.signals import Signal
 from core import datetime
 from django.contrib.contenttypes.models import ContentType
 from policyholder.models import PolicyHolderInsuree
 
@@ -97,15 +97,15 @@
             # check if json external calculation rule in instance exists
             if cp_params:
                 cp_params = cp_params["calculation_rule"] if "calculation_rule" in cp_params else None
             if cd_params:
                 cd_params = cd_params["calculation_rule"] if "calculation_rule" in cd_params else None
             if phi_params:
                 phi_params = phi_params["calculation_rule"] if "calculation_rule" in phi_params else None
-            if "rate" in cp_params:
+            if cp_params is not None and "rate" in cp_params:
                 rate = int(cp_params["rate"])
                 if cd_params:
                     if "income" in cd_params:
                         income = float(cd_params["income"])
                     elif "income" in phi_params:
                         income = float(phi_params["income"])
                     else:
@@ -128,148 +128,14 @@
             model_class = ContentType.objects.filter(model=class_name).first()
             if model_class:
                 model_class = model_class.model_class()
                 list_class = list_class + \
                              [f.remote_field.model.__name__ for f in model_class._meta.fields
                               if f.get_internal_type() == 'ForeignKey' and f.remote_field.model.__name__ != "User"]
         else:
-            list_class.append("Calculation")
-        # because we have calculation in ContributionPlan
-        #  as uuid - we have to consider this case
-        if class_name == "ContributionPlan":
-            list_class.append("Calculation")
-        # because we have no direct relation in ContributionPlanBundle
-        #  to ContributionPlan we have to consider this case
-        if class_name == "ContributionPlanBundle":
-            list_class.append("ContributionPlan")
-        return list_class
-
-
-class ContributionValuationRule_2(AbsCalculationRule):
-    version = 1
-    uuid = "0e556dd4-04a0-4aa4-ac47-2a99cfa5e9a8"
-    calculation_rule_name = "CV: percent of income, no dependants"
-    description = DESCRIPTION_CONTRIBUTION_VALUATION
-    impacted_class_parameter = CLASS_RULE_PARAM_VALIDATION2
-    date_valid_from = datetime.datetime(2000, 1, 1)
-    date_valid_to = None
-    status = "active"
-    from_to = FROM_TO
-    type = "account_receivable"
-    sub_type = "contribution"
-
-    signal_get_rule_name = Signal(providing_args=[])
-    signal_get_rule_details = Signal(providing_args=[])
-    signal_get_param = Signal(providing_args=[])
-    signal_get_linked_class = Signal(providing_args=[])
-    signal_calculate_event = Signal(providing_args=[])
-    signal_convert_from_to = Signal(providing_args=[])
-
-    @classmethod
-    def ready(cls):
-        now = datetime.datetime.now()
-        condition_is_valid = (cls.date_valid_from <= now <= cls.date_valid_to) \
-            if cls.date_valid_to else (now >= cls.date_valid_from and cls.date_valid_to is None)
-        if condition_is_valid:
-            if cls.status == "active":
-                # register signals getParameter to getParameter signal and getLinkedClass ot getLinkedClass signal
-                cls.signal_get_rule_name.connect(cls.get_rule_name, dispatch_uid="on_get_rule_name_signal")
-                cls.signal_get_rule_details.connect(cls.get_rule_details, dispatch_uid="on_get_rule_details_signal")
-                cls.signal_get_param.connect(cls.get_parameters, dispatch_uid="on_get_param_signal")
-                cls.signal_get_linked_class.connect(cls.get_linked_class, dispatch_uid="on_get_linked_class_signal")
-                cls.signal_calculate_event.connect(cls.run_calculation_rules, dispatch_uid="on_calculate_event_signal")
-
-    @classmethod
-    def active_for_object(cls, instance, context, type='account_receivable', sub_type='contribution'):
-        return instance.__class__.__name__ == "ContractContributionPlanDetails" \
-               and context in ["create", "update"] \
-               and cls.check_calculation(instance)
-
-    @classmethod
-    def check_calculation(cls, instance):
-        match = False
-        class_name = instance.__class__.__name__
-        list_class_name = [
-            "PolicyHolder", "ContributionPlan",
-            "PolicyHolderInsuree", "ContractDetails",
-            "ContractContributionPlanDetails", "ContributionPlanBundle"
-        ]
-        if class_name == "ABCMeta":
-            match = str(cls.uuid) == str(instance.uuid)
-        elif class_name == "ContributionPlan":
-            match = str(cls.uuid) == str(instance.calculation)
-        elif class_name == "ContributionPlanBundle":
-            list_cpbd = list(ContributionPlanBundleDetails.objects.filter(
-                contribution_plan_bundle=instance
-            ))
-            for cpbd in list_cpbd:
-                if match is False:
-                    if cls.check_calculation(cpbd.contribution_plan):
-                        match = True
-        else:
-            related_fields = [
-                f.name for f in instance.__class__._meta.fields
-                if f.get_internal_type() == 'ForeignKey' and f.remote_field.model.__name__ in list_class_name
-            ]
-            for rf in related_fields:
-                match = cls.check_calculation(getattr(instance, rf))
-        return match
-
-    @classmethod
-    def calculate(cls, instance, **kwargs):
-        if instance.__class__.__name__ == "ContractContributionPlanDetails":
-            # check type of json_ext - in case of string - json.loads
-            cp_params, cd_params = instance.contribution_plan.json_ext, instance.contract_details.json_ext
-            ph_insuree = PolicyHolderInsuree.objects.filter(
-                insuree=instance.contract_details.insuree).first()
-            phi_params = ph_insuree.json_ext
-            if isinstance(cp_params, str):
-                cp_params = json.loads(cp_params)
-            if isinstance(cd_params, str):
-                cd_params = json.loads(cd_params)
-            if isinstance(phi_params, str):
-                phi_params = json.loads(phi_params)
-            # check if json external calculation rule in instance exists
-            if cp_params:
-                cp_params = cp_params["calculation_rule"] if "calculation_rule" in cp_params else None
-            if cd_params:
-                cd_params = cd_params["calculation_rule"] if "calculation_rule" in cd_params else None
-            if phi_params:
-                phi_params = phi_params["calculation_rule"] if "calculation_rule" in phi_params else None
-            if "rate" in cp_params:
-                rate = int(cp_params["rate"])
-                if cd_params:
-                    if "income" in cd_params:
-                        income = float(cd_params["income"])
-                    elif "income" in phi_params:
-                        income = float(phi_params["income"])
-                    else:
-                        return False
-                elif "income" in phi_params:
-                    income = float(phi_params["income"])
-                else:
-                    return False
-                value = float(income) * (rate / 100)
-                return value
-            else:
-                return False
-        else:
-            return False
-
-    @classmethod
-    def get_linked_class(cls, sender, class_name, **kwargs):
-        list_class = []
-        if class_name != None:
-            model_class = ContentType.objects.filter(model=class_name).first()
-            if model_class:
-                model_class = model_class.model_class()
-                list_class = list_class + \
-                             [f.remote_field.model.__name__ for f in model_class._meta.fields
-                              if f.get_internal_type() == 'ForeignKey' and f.remote_field.model.__name__ != "User"]
-        else:
             list_class.append("Calculation")
         # because we have calculation in ContributionPlan
         #  as uuid - we have to consider this case
         if class_name == "ContributionPlan":
             list_class.append("Calculation")
         # because we have no direct relation in ContributionPlanBundle
         #  to ContributionPlan we have to consider this case
```

### Comparing `openimis-be-calculation-1.5.0/calculation/config.py` & `openimis-be-calculation-1.5.1/calculation/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -102,100 +102,14 @@
                 "condition": "INPUT>100",
                 "default": ""
             }
         ],
     },
 ]
 
-CLASS_RULE_PARAM_VALIDATION2 = [
-    {
-        "class": "ContributionPlan",
-        "parameters": [
-            {
-                "type": "select",
-                "name": "rate",
-                "label": {
-                    "en": "Percentage of income",
-                    "fr": "Pourcentage du salaire"
-                },
-                "rights": {
-                    "read": "151201",
-                    "write": "151202",
-                    "update": "151203",
-                    "replace": "151206",
-                },
-                'optionSet': [
-                    {
-                        "value": "5",
-                        "label": {
-                            "en": "5%",
-                            "fr": "5%"
-                        }
-                    },
-                    {
-                        "value": "10",
-                        "label": {
-                            "en": "10%",
-                            "fr": "10%"
-                        }
-                    },
-                    {
-                        "value": "15",
-                        "label": {
-                            "en": "15%",
-                            "fr": "15%"
-                        }
-                    },
-                ],
-                "default": "5"
-            },
-        ],
-    },
-    {
-        "class": "ContractDetails",
-        "parameters": [
-            {
-                "type": "number",
-                "name": "income",
-                "label": {
-                    "en": "Income",
-                    "fr": "Salaire"
-                },
-                "rights": {
-                    "read": "152101",
-                    "write": "152102",
-                    "update": "152103",
-                    "replace": "152103",
-                },
-                "default": ""
-            }
-        ],
-    },
-    {
-        "class": "PolicyHolderInsuree",
-        "parameters": [
-            {
-                "type": "number",
-                "name": "income",
-                "label": {
-                    "en": "Income",
-                    "fr": "Salaire"
-                },
-                "rights": {
-                    "read": "150201",
-                    "write": "150202",
-                    "update": "150203",
-                    "replace": "150206",
-                },
-                "default": ""
-            }
-        ],
-    },
-]
-
 DESCRIPTION_CONTRIBUTION_VALUATION = F"" \
     F"This calcutation will add the income in the contract details " \
     F"and PHinsuree and the percentage in the Contribution plan" \
     F" so when a contract valuation is requested then the calculation will" \
     F" determine the value based on the contract details income and CP percentage"
 
 FROM_TO = []
```

### Comparing `openimis-be-calculation-1.5.0/calculation/migrations/0001_initial.py` & `openimis-be-calculation-1.5.1/calculation/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calculation-1.5.0/calculation/migrations/0002_auto_20210118_1426.py` & `openimis-be-calculation-1.5.1/calculation/migrations/0002_auto_20210118_1426.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calculation-1.5.0/calculation/schema.py` & `openimis-be-calculation-1.5.1/calculation/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 class CalculationParamsGQLType(graphene.ObjectType):
     type = graphene.String()
     name = graphene.String()
     label = graphene.Field(LabelParamGQLType)
     rights = graphene.Field(RightParamGQLType)
     option_set = graphene.List(OptionParamGQLType)
     relevance = graphene.String()
+    required = graphene.String()
     condition = graphene.String()
     default_value = graphene.String()
 
 
 class CalculationParamsListGQLType(graphene.ObjectType):
     calculation_params = graphene.List(CalculationParamsGQLType)
```

### Comparing `openimis-be-calculation-1.5.0/calculation/services.py` & `openimis-be-calculation-1.5.1/calculation/services.py`

 * *Files identical despite different names*

### Comparing `openimis-be-calculation-1.5.0/openimis_be_calculation.egg-info/PKG-INFO` & `openimis-be-calculation-1.5.1/openimis_be_calculation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-calculation
-Version: 1.5.0
+Version: 1.5.1
 Summary: The openIMIS Backend Calculation reference module.
 Home-page: https://openimis.org/
 Author: Damian Borowiecki
 Author-email: dborowiecki@soldevelo.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `openimis-be-calculation-1.5.0/openimis_be_calculation.egg-info/SOURCES.txt` & `openimis-be-calculation-1.5.1/openimis_be_calculation.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 calculation/schema.py
 calculation/services.py
 calculation/urls.py
 calculation/views.py
 calculation/migrations/0001_initial.py
 calculation/migrations/0002_auto_20210118_1426.py
 calculation/migrations/0003_add_calculation_roles_for_admin.py
+calculation/migrations/0004_auto_20230126_0903.py
 calculation/migrations/__init__.py
 calculation/tests/__init__.py
 calculation/tests/helpers.py
 calculation/tests/helpers_tests.py
 openimis_be_calculation.egg-info/PKG-INFO
 openimis_be_calculation.egg-info/SOURCES.txt
 openimis_be_calculation.egg-info/dependency_links.txt
```

### Comparing `openimis-be-calculation-1.5.0/setup.py` & `openimis-be-calculation-1.5.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='openimis-be-calculation',
-    version='1.5.0',
+    version='v1.5.1',
     packages=find_packages(),
     include_package_data=True,
     license='GNU AGPL v3',
     description='The openIMIS Backend Calculation reference module.',
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://openimis.org/',
```

