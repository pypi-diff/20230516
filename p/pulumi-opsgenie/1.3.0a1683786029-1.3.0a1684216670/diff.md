# Comparing `tmp/pulumi_opsgenie-1.3.0a1683786029.tar.gz` & `tmp/pulumi_opsgenie-1.3.0a1684216670.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_opsgenie-1.3.0a1683786029.tar", last modified: Thu May 11 06:33:37 2023, max compression
+gzip compressed data, was "pulumi_opsgenie-1.3.0a1684216670.tar", last modified: Tue May 16 06:03:33 2023, max compression
```

## Comparing `pulumi_opsgenie-1.3.0a1683786029.tar` & `pulumi_opsgenie-1.3.0a1684216670.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:33:37.298655 pulumi_opsgenie-1.3.0a1683786029/
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-11 06:33:37.294655 pulumi_opsgenie-1.3.0a1683786029/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-11 06:33:36.000000 pulumi_opsgenie-1.3.0a1683786029/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:33:37.294655 pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-05-11 06:33:36.000000 pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   179290 2023-05-11 06:33:36.000000 pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-05-11 06:33:36.000000 pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    57892 2023-05-11 06:33:36.000000 pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/alert_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    32958 2023-05-11 06:33:36.000000 pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/api_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:33:37.294655 pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-11 06:33:36.000000 pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-11 06:33:36.000000 pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    15459 2023-05-11 06:33:36.000000 pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/custom_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    23084 2023-05-11 06:33:36.000000 pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/email_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    17617 2023-05-11 06:33:36.000000 pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/escalation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6282 2023-05-11 06:33:36.000000 pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/get_escalation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9977 2023-05-11 06:33:36.000000 pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/get_heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     6178 2023-05-11 06:33:36.000000 pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/get_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-05-11 06:33:36.000000 pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/get_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4387 2023-05-11 06:33:36.000000 pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/get_team.py
--rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-05-11 06:33:36.000000 pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/get_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    23842 2023-05-11 06:33:36.000000 pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)    23703 2023-05-11 06:33:36.000000 pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/incident_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    26894 2023-05-11 06:33:36.000000 pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/integration_action.py
--rw-r--r--   0 runner    (1001) docker     (123)    13192 2023-05-11 06:33:36.000000 pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/maintenance.py
--rw-r--r--   0 runner    (1001) docker     (123)    34667 2023-05-11 06:33:36.000000 pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/notification_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    30482 2023-05-11 06:33:36.000000 pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/notification_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)   159991 2023-05-11 06:33:36.000000 pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-05-11 06:33:36.000000 pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-11 06:33:36.000000 pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 06:33:36.000000 pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    14376 2023-05-11 06:33:36.000000 pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)    25289 2023-05-11 06:33:36.000000 pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/schedule_rotation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10881 2023-05-11 06:33:36.000000 pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/service.py
--rw-r--r--   0 runner    (1001) docker     (123)    12998 2023-05-11 06:33:36.000000 pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/service_incident_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    19469 2023-05-11 06:33:36.000000 pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/team.py
--rw-r--r--   0 runner    (1001) docker     (123)    26743 2023-05-11 06:33:36.000000 pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/team_routing_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    26257 2023-05-11 06:33:36.000000 pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    13198 2023-05-11 06:33:36.000000 pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/user_contact.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 06:33:37.294655 pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-11 06:33:37.000000 pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-11 06:33:37.000000 pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 06:33:37.000000 pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 06:33:37.000000 pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-11 06:33:37.000000 pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-11 06:33:37.000000 pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 06:33:37.298655 pulumi_opsgenie-1.3.0a1683786029/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-11 06:33:36.000000 pulumi_opsgenie-1.3.0a1683786029/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:03:33.441231 pulumi_opsgenie-1.3.0a1684216670/
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-16 06:03:33.441231 pulumi_opsgenie-1.3.0a1684216670/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:03:33.441231 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   179290 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57892 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/alert_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32958 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/api_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:03:33.441231 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15459 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/custom_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23084 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/email_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17617 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/escalation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6282 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/get_escalation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9977 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/get_heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6178 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/get_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/get_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4387 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/get_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23842 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23703 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/incident_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26894 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/integration_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13192 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/maintenance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34667 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/notification_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30482 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/notification_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)   159991 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    14376 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25289 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/schedule_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10881 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12998 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/service_incident_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19469 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/team.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26743 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/team_routing_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26257 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13198 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/user_contact.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:03:33.441231 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 06:03:33.441231 pulumi_opsgenie-1.3.0a1684216670/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-16 06:03:33.000000 pulumi_opsgenie-1.3.0a1684216670/setup.py
```

### Comparing `pulumi_opsgenie-1.3.0a1683786029/PKG-INFO` & `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pulumi_opsgenie
-Version: 1.3.0a1683786029
+Name: pulumi-opsgenie
+Version: 1.3.0a1684216670
 Summary: A Pulumi package for creating and managing opsgenie cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-opsgenie
 Keywords: pulumi opsgenie
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_opsgenie-1.3.0a1683786029/README.md` & `pulumi_opsgenie-1.3.0a1684216670/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/__init__.py` & `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/_inputs.py` & `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/_utilities.py` & `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/alert_policy.py` & `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/alert_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/api_integration.py` & `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/api_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/config/vars.py` & `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/custom_role.py` & `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/custom_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/email_integration.py` & `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/email_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/escalation.py` & `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/escalation.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/get_escalation.py` & `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/get_escalation.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/get_heartbeat.py` & `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/get_heartbeat.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/get_schedule.py` & `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/get_schedule.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/get_service.py` & `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/get_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/get_team.py` & `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/get_team.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/get_user.py` & `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/heartbeat.py` & `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/heartbeat.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/incident_template.py` & `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/incident_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/integration_action.py` & `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/integration_action.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/maintenance.py` & `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/maintenance.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/notification_policy.py` & `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/notification_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/notification_rule.py` & `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/notification_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/outputs.py` & `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/provider.py` & `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/schedule.py` & `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/schedule.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/schedule_rotation.py` & `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/schedule_rotation.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/service.py` & `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/service.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/service_incident_rule.py` & `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/service_incident_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/team.py` & `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/team.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/team_routing_rule.py` & `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/team_routing_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/user.py` & `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie/user_contact.py` & `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie/user_contact.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie.egg-info/PKG-INFO` & `pulumi_opsgenie-1.3.0a1684216670/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pulumi-opsgenie
-Version: 1.3.0a1683786029
+Name: pulumi_opsgenie
+Version: 1.3.0a1684216670
 Summary: A Pulumi package for creating and managing opsgenie cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-opsgenie
 Keywords: pulumi opsgenie
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_opsgenie-1.3.0a1683786029/pulumi_opsgenie.egg-info/SOURCES.txt` & `pulumi_opsgenie-1.3.0a1684216670/pulumi_opsgenie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.3.0a1683786029/setup.py` & `pulumi_opsgenie-1.3.0a1684216670/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "1.3.0a1683786029"
-PLUGIN_VERSION = "1.3.0-alpha.1683786029+59e64485"
+VERSION = "1.3.0a1684216670"
+PLUGIN_VERSION = "1.3.0-alpha.1684216670+113c1638"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'opsgenie', PLUGIN_VERSION])
         except OSError as error:
```

