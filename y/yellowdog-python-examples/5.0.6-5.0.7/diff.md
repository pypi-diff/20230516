# Comparing `tmp/yellowdog-python-examples-5.0.6.tar.gz` & `tmp/yellowdog-python-examples-5.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yellowdog-python-examples-5.0.6.tar", last modified: Wed May  3 10:28:18 2023, max compression
+gzip compressed data, was "yellowdog-python-examples-5.0.7.tar", last modified: Tue May 16 09:43:16 2023, max compression
```

## Comparing `yellowdog-python-examples-5.0.6.tar` & `yellowdog-python-examples-5.0.7.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-05-03 10:28:18.927729 yellowdog-python-examples-5.0.6/
--rw-r--r--   0 pwt        (501) staff       (20)    11357 2022-11-18 20:55:26.000000 yellowdog-python-examples-5.0.6/LICENSE
--rw-r--r--   0 pwt        (501) staff       (20)     1418 2023-05-03 10:28:18.927791 yellowdog-python-examples-5.0.6/PKG-INFO
--rw-r--r--   0 pwt        (501) staff       (20)      676 2022-11-22 08:58:59.000000 yellowdog-python-examples-5.0.6/PYPI_README.md
--rw-r--r--   0 pwt        (501) staff       (20)   109989 2023-05-03 10:27:28.000000 yellowdog-python-examples-5.0.6/README.md
--rw-r--r--   0 pwt        (501) staff       (20)     1806 2023-02-20 09:23:16.000000 yellowdog-python-examples-5.0.6/pyproject.toml
--rw-r--r--   0 pwt        (501) staff       (20)       46 2023-03-31 14:34:07.000000 yellowdog-python-examples-5.0.6/requirements.txt
--rw-r--r--   0 pwt        (501) staff       (20)     1366 2023-05-03 10:28:18.928081 yellowdog-python-examples-5.0.6/setup.cfg
--rw-r--r--   0 pwt        (501) staff       (20)      125 2023-02-14 10:40:48.000000 yellowdog-python-examples-5.0.6/setup.py
-drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-05-03 10:28:18.926862 yellowdog-python-examples-5.0.6/yd_commands/
--rw-r--r--   0 pwt        (501) staff       (20)       22 2023-05-03 10:27:28.000000 yellowdog-python-examples-5.0.6/yd_commands/__init__.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     3378 2023-04-19 15:22:46.000000 yellowdog-python-examples-5.0.6/yd_commands/abort.py
--rwxr-xr-x   0 pwt        (501) staff       (20)      982 2023-01-31 15:59:12.000000 yellowdog-python-examples-5.0.6/yd_commands/admin.py
--rwxr-xr-x   0 pwt        (501) staff       (20)    17864 2023-04-19 15:22:46.000000 yellowdog-python-examples-5.0.6/yd_commands/args.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     5077 2023-04-19 15:22:46.000000 yellowdog-python-examples-5.0.6/yd_commands/cancel.py
--rw-r--r--   0 pwt        (501) staff       (20)      579 2022-12-12 15:56:41.000000 yellowdog-python-examples-5.0.6/yd_commands/check_imports.py
--rw-r--r--   0 pwt        (501) staff       (20)     3757 2022-11-27 20:53:08.000000 yellowdog-python-examples-5.0.6/yd_commands/compact_json.py
--rw-r--r--   0 pwt        (501) staff       (20)    18351 2023-05-03 10:27:28.000000 yellowdog-python-examples-5.0.6/yd_commands/config.py
--rw-r--r--   0 pwt        (501) staff       (20)     5544 2023-05-03 10:27:28.000000 yellowdog-python-examples-5.0.6/yd_commands/config_keys.py
--rw-r--r--   0 pwt        (501) staff       (20)    12183 2023-04-19 15:22:46.000000 yellowdog-python-examples-5.0.6/yd_commands/csv_data.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     1647 2023-02-14 10:40:48.000000 yellowdog-python-examples-5.0.6/yd_commands/delete.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     3616 2023-02-14 10:40:48.000000 yellowdog-python-examples-5.0.6/yd_commands/download.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     9203 2023-04-19 15:22:46.000000 yellowdog-python-examples-5.0.6/yd_commands/instantiate.py
--rw-r--r--   0 pwt        (501) staff       (20)     3749 2023-04-19 15:22:46.000000 yellowdog-python-examples-5.0.6/yd_commands/interactive.py
--rwxr-xr-x   0 pwt        (501) staff       (20)      749 2023-03-28 14:27:45.000000 yellowdog-python-examples-5.0.6/yd_commands/jsonnet2json.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     7539 2023-04-19 15:22:46.000000 yellowdog-python-examples-5.0.6/yd_commands/list.py
--rw-r--r--   0 pwt        (501) staff       (20)     3012 2023-02-14 10:40:48.000000 yellowdog-python-examples-5.0.6/yd_commands/object_utilities.py
--rw-r--r--   0 pwt        (501) staff       (20)     9590 2023-04-19 15:22:46.000000 yellowdog-python-examples-5.0.6/yd_commands/printing.py
--rwxr-xr-x   0 pwt        (501) staff       (20)    16885 2023-04-19 15:22:46.000000 yellowdog-python-examples-5.0.6/yd_commands/provision.py
--rw-r--r--   0 pwt        (501) staff       (20)     1248 2023-05-03 10:27:28.000000 yellowdog-python-examples-5.0.6/yd_commands/provision_utils.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     1479 2023-02-14 10:40:48.000000 yellowdog-python-examples-5.0.6/yd_commands/reformat_json.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     3231 2023-04-19 15:22:46.000000 yellowdog-python-examples-5.0.6/yd_commands/shutdown.py
--rwxr-xr-x   0 pwt        (501) staff       (20)    40102 2023-04-19 15:22:46.000000 yellowdog-python-examples-5.0.6/yd_commands/submit.py
--rw-r--r--   0 pwt        (501) staff       (20)     6052 2023-05-03 10:27:28.000000 yellowdog-python-examples-5.0.6/yd_commands/submit_utils.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     2756 2023-04-19 15:22:46.000000 yellowdog-python-examples-5.0.6/yd_commands/terminate.py
--rw-r--r--   0 pwt        (501) staff       (20)     1678 2022-12-07 08:38:57.000000 yellowdog-python-examples-5.0.6/yd_commands/type_check.py
--rw-r--r--   0 pwt        (501) staff       (20)     2252 2023-04-19 15:22:46.000000 yellowdog-python-examples-5.0.6/yd_commands/upload.py
--rw-r--r--   0 pwt        (501) staff       (20)     3389 2023-04-19 15:22:46.000000 yellowdog-python-examples-5.0.6/yd_commands/upload_utils.py
--rw-r--r--   0 pwt        (501) staff       (20)     1630 2023-04-19 15:22:46.000000 yellowdog-python-examples-5.0.6/yd_commands/validate_properties.py
--rw-r--r--   0 pwt        (501) staff       (20)    11055 2023-04-19 15:22:46.000000 yellowdog-python-examples-5.0.6/yd_commands/variables.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     1247 2023-03-24 08:40:30.000000 yellowdog-python-examples-5.0.6/yd_commands/version.py
--rw-r--r--   0 pwt        (501) staff       (20)     2200 2023-04-19 15:22:46.000000 yellowdog-python-examples-5.0.6/yd_commands/wrapper.py
-drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-05-03 10:28:18.927618 yellowdog-python-examples-5.0.6/yellowdog_python_examples.egg-info/
--rw-r--r--   0 pwt        (501) staff       (20)     1418 2023-05-03 10:28:18.000000 yellowdog-python-examples-5.0.6/yellowdog_python_examples.egg-info/PKG-INFO
--rw-r--r--   0 pwt        (501) staff       (20)     1187 2023-05-03 10:28:18.000000 yellowdog-python-examples-5.0.6/yellowdog_python_examples.egg-info/SOURCES.txt
--rw-r--r--   0 pwt        (501) staff       (20)        1 2023-05-03 10:28:18.000000 yellowdog-python-examples-5.0.6/yellowdog_python_examples.egg-info/dependency_links.txt
--rw-r--r--   0 pwt        (501) staff       (20)      574 2023-05-03 10:28:18.000000 yellowdog-python-examples-5.0.6/yellowdog_python_examples.egg-info/entry_points.txt
--rw-r--r--   0 pwt        (501) staff       (20)       61 2023-05-03 10:28:18.000000 yellowdog-python-examples-5.0.6/yellowdog_python_examples.egg-info/requires.txt
--rw-r--r--   0 pwt        (501) staff       (20)       12 2023-05-03 10:28:18.000000 yellowdog-python-examples-5.0.6/yellowdog_python_examples.egg-info/top_level.txt
+drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-05-16 09:43:16.418703 yellowdog-python-examples-5.0.7/
+-rw-r--r--   0 pwt        (501) staff       (20)    11357 2022-11-18 20:55:26.000000 yellowdog-python-examples-5.0.7/LICENSE
+-rw-r--r--   0 pwt        (501) staff       (20)     1418 2023-05-16 09:43:16.418795 yellowdog-python-examples-5.0.7/PKG-INFO
+-rw-r--r--   0 pwt        (501) staff       (20)      676 2022-11-22 08:58:59.000000 yellowdog-python-examples-5.0.7/PYPI_README.md
+-rw-r--r--   0 pwt        (501) staff       (20)   109989 2023-05-03 10:27:28.000000 yellowdog-python-examples-5.0.7/README.md
+-rw-r--r--   0 pwt        (501) staff       (20)     1806 2023-02-20 09:23:16.000000 yellowdog-python-examples-5.0.7/pyproject.toml
+-rw-r--r--   0 pwt        (501) staff       (20)       46 2023-05-16 09:40:32.000000 yellowdog-python-examples-5.0.7/requirements.txt
+-rw-r--r--   0 pwt        (501) staff       (20)     1366 2023-05-16 09:43:16.419062 yellowdog-python-examples-5.0.7/setup.cfg
+-rw-r--r--   0 pwt        (501) staff       (20)      125 2023-02-14 10:40:48.000000 yellowdog-python-examples-5.0.7/setup.py
+drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-05-16 09:43:16.417930 yellowdog-python-examples-5.0.7/yd_commands/
+-rw-r--r--   0 pwt        (501) staff       (20)       22 2023-05-16 09:40:32.000000 yellowdog-python-examples-5.0.7/yd_commands/__init__.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     3415 2023-05-16 09:40:32.000000 yellowdog-python-examples-5.0.7/yd_commands/abort.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)      982 2023-01-31 15:59:12.000000 yellowdog-python-examples-5.0.7/yd_commands/admin.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)    18007 2023-05-16 09:40:32.000000 yellowdog-python-examples-5.0.7/yd_commands/args.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     5114 2023-05-16 09:40:32.000000 yellowdog-python-examples-5.0.7/yd_commands/cancel.py
+-rw-r--r--   0 pwt        (501) staff       (20)      579 2022-12-12 15:56:41.000000 yellowdog-python-examples-5.0.7/yd_commands/check_imports.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3757 2022-11-27 20:53:08.000000 yellowdog-python-examples-5.0.7/yd_commands/compact_json.py
+-rw-r--r--   0 pwt        (501) staff       (20)    18352 2023-05-16 09:40:32.000000 yellowdog-python-examples-5.0.7/yd_commands/config.py
+-rw-r--r--   0 pwt        (501) staff       (20)     5544 2023-05-03 10:27:28.000000 yellowdog-python-examples-5.0.7/yd_commands/config_keys.py
+-rw-r--r--   0 pwt        (501) staff       (20)    12181 2023-05-16 09:40:32.000000 yellowdog-python-examples-5.0.7/yd_commands/csv_data.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     1657 2023-05-16 09:40:32.000000 yellowdog-python-examples-5.0.7/yd_commands/delete.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     3626 2023-05-16 09:40:32.000000 yellowdog-python-examples-5.0.7/yd_commands/download.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     9251 2023-05-16 09:40:32.000000 yellowdog-python-examples-5.0.7/yd_commands/instantiate.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3729 2023-05-16 09:40:32.000000 yellowdog-python-examples-5.0.7/yd_commands/interactive.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)      749 2023-03-28 14:27:45.000000 yellowdog-python-examples-5.0.7/yd_commands/jsonnet2json.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     7798 2023-05-16 09:40:32.000000 yellowdog-python-examples-5.0.7/yd_commands/list.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3000 2023-05-16 09:40:32.000000 yellowdog-python-examples-5.0.7/yd_commands/object_utilities.py
+-rw-r--r--   0 pwt        (501) staff       (20)     9525 2023-05-16 09:40:32.000000 yellowdog-python-examples-5.0.7/yd_commands/printing.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)    16922 2023-05-16 09:40:32.000000 yellowdog-python-examples-5.0.7/yd_commands/provision.py
+-rw-r--r--   0 pwt        (501) staff       (20)     1248 2023-05-03 10:27:28.000000 yellowdog-python-examples-5.0.7/yd_commands/provision_utils.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     1479 2023-02-14 10:40:48.000000 yellowdog-python-examples-5.0.7/yd_commands/reformat_json.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     3232 2023-05-16 09:40:32.000000 yellowdog-python-examples-5.0.7/yd_commands/shutdown.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)    40228 2023-05-16 09:40:32.000000 yellowdog-python-examples-5.0.7/yd_commands/submit.py
+-rw-r--r--   0 pwt        (501) staff       (20)     6052 2023-05-03 10:27:28.000000 yellowdog-python-examples-5.0.7/yd_commands/submit_utils.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     2916 2023-05-16 09:40:32.000000 yellowdog-python-examples-5.0.7/yd_commands/terminate.py
+-rw-r--r--   0 pwt        (501) staff       (20)     1678 2022-12-07 08:38:57.000000 yellowdog-python-examples-5.0.7/yd_commands/type_check.py
+-rw-r--r--   0 pwt        (501) staff       (20)     2237 2023-05-16 09:40:32.000000 yellowdog-python-examples-5.0.7/yd_commands/upload.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3389 2023-04-19 15:22:46.000000 yellowdog-python-examples-5.0.7/yd_commands/upload_utils.py
+-rw-r--r--   0 pwt        (501) staff       (20)     1630 2023-04-19 15:22:46.000000 yellowdog-python-examples-5.0.7/yd_commands/validate_properties.py
+-rw-r--r--   0 pwt        (501) staff       (20)    11037 2023-05-16 09:40:32.000000 yellowdog-python-examples-5.0.7/yd_commands/variables.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     1247 2023-03-24 08:40:30.000000 yellowdog-python-examples-5.0.7/yd_commands/version.py
+-rw-r--r--   0 pwt        (501) staff       (20)     2200 2023-04-19 15:22:46.000000 yellowdog-python-examples-5.0.7/yd_commands/wrapper.py
+drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-05-16 09:43:16.418610 yellowdog-python-examples-5.0.7/yellowdog_python_examples.egg-info/
+-rw-r--r--   0 pwt        (501) staff       (20)     1418 2023-05-16 09:43:16.000000 yellowdog-python-examples-5.0.7/yellowdog_python_examples.egg-info/PKG-INFO
+-rw-r--r--   0 pwt        (501) staff       (20)     1187 2023-05-16 09:43:16.000000 yellowdog-python-examples-5.0.7/yellowdog_python_examples.egg-info/SOURCES.txt
+-rw-r--r--   0 pwt        (501) staff       (20)        1 2023-05-16 09:43:16.000000 yellowdog-python-examples-5.0.7/yellowdog_python_examples.egg-info/dependency_links.txt
+-rw-r--r--   0 pwt        (501) staff       (20)      574 2023-05-16 09:43:16.000000 yellowdog-python-examples-5.0.7/yellowdog_python_examples.egg-info/entry_points.txt
+-rw-r--r--   0 pwt        (501) staff       (20)       61 2023-05-16 09:43:16.000000 yellowdog-python-examples-5.0.7/yellowdog_python_examples.egg-info/requires.txt
+-rw-r--r--   0 pwt        (501) staff       (20)       12 2023-05-16 09:43:16.000000 yellowdog-python-examples-5.0.7/yellowdog_python_examples.egg-info/top_level.txt
```

### Comparing `yellowdog-python-examples-5.0.6/LICENSE` & `yellowdog-python-examples-5.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.6/PKG-INFO` & `yellowdog-python-examples-5.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yellowdog-python-examples
-Version: 5.0.6
+Version: 5.0.7
 Summary: Example Python commands using the YellowDog Python SDK
 Home-page: https://github.com/yellowdog/python-examples
 Author: YellowDog Limited
 Author-email: YellowDog Limited <support@yellowdog.co>
 Project-URL: Homepage, https://github.com/yellowdog/python-examples
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `yellowdog-python-examples-5.0.6/PYPI_README.md` & `yellowdog-python-examples-5.0.7/PYPI_README.md`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.6/README.md` & `yellowdog-python-examples-5.0.7/README.md`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.6/pyproject.toml` & `yellowdog-python-examples-5.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.6/setup.cfg` & `yellowdog-python-examples-5.0.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.6/yd_commands/abort.py` & `yellowdog-python-examples-5.0.7/yd_commands/abort.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,33 +23,33 @@
 from yd_commands.printing import print_error, print_log, sorted_objects
 from yd_commands.wrapper import CLIENT, CONFIG_COMMON, main_wrapper
 
 
 @main_wrapper
 def main():
     print_log(
-        f"Finding Work Requirements in "
+        "Finding Work Requirements in "
         f"namespace '{CONFIG_COMMON.namespace}' and "
         f"tag starting with '{CONFIG_COMMON.name_tag}'"
     )
 
     # Abort Tasks is always interactive
     ARGS_PARSER.interactive = True
 
-    selected_work_requirement_summaries: List[
-        WorkRequirementSummary
-    ] = get_filtered_work_requirements(
-        CLIENT,
-        namespace=CONFIG_COMMON.namespace,
-        tag=CONFIG_COMMON.name_tag,
-        exclude_filter=[
-            WorkRequirementStatus.COMPLETED,
-            WorkRequirementStatus.CANCELLED,
-            WorkRequirementStatus.FAILED,
-        ],
+    selected_work_requirement_summaries: List[WorkRequirementSummary] = (
+        get_filtered_work_requirements(
+            CLIENT,
+            namespace=CONFIG_COMMON.namespace,
+            tag=CONFIG_COMMON.name_tag,
+            exclude_filter=[
+                WorkRequirementStatus.COMPLETED,
+                WorkRequirementStatus.CANCELLED,
+                WorkRequirementStatus.FAILED,
+            ],
+        )
     )
 
     if len(selected_work_requirement_summaries) != 0:
         selected_work_requirement_summaries = select(
             CLIENT, selected_work_requirement_summaries, override_quiet=True
         )
     else:
@@ -86,17 +86,17 @@
                 override_quiet=True,
             )
         if len(tasks) != 0 and confirmed(f"Abort {len(tasks)} Tasks?"):
             for task in tasks:
                 try:
                     CLIENT.work_client.cancel_task(task, abort=True)
                     print_log(
-                        f"Aborting Task '{task.name}' "
-                        f"in Task Group '{get_task_group_name(CLIENT, wr_summary, task)}' "
-                        f"in Work Requirement '{wr_summary.name}'"
+                        f"Aborting Task '{task.name}' in Task Group"
+                        f" '{get_task_group_name(CLIENT, wr_summary, task)}' in Work"
+                        f" Requirement '{wr_summary.name}'"
                     )
                     aborted_tasks += 1
                 except Exception as e:
                     print_error(e)
                     continue
         if aborted_tasks == 0:
             print_log("No Tasks Aborted")
```

### Comparing `yellowdog-python-examples-5.0.6/yd_commands/admin.py` & `yellowdog-python-examples-5.0.7/yd_commands/admin.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.6/yd_commands/args.py` & `yellowdog-python-examples-5.0.7/yd_commands/args.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,16 +36,18 @@
             help="provide a link to the documentation for this version",
         )
         parser.add_argument(
             "--config",
             "-c",
             required=False,
             type=str,
-            help="configuration file in TOML format; "
-            "default is 'config.toml' in the current directory",
+            help=(
+                "configuration file in TOML format; "
+                "default is 'config.toml' in the current directory"
+            ),
             metavar="<config_file.toml>",
         )
         parser.add_argument(
             "--key",
             "-k",
             type=str,
             required=False,
@@ -175,15 +177,18 @@
                 metavar="<data.csv>",
             )
             parser.add_argument(
                 "--process-csv-only",
                 "-p",
                 action="store_true",
                 required=False,
-                help="process CSV variable substitutions only and output intermediate JSON",
+                help=(
+                    "process CSV variable substitutions only and output intermediate"
+                    " JSON"
+                ),
             )
 
         if any(module in sys.argv[0] for module in ["provision", "instantiate"]):
             parser.add_argument(
                 "--worker-pool",
                 "-p",
                 type=str,
@@ -398,16 +403,18 @@
             any(module in sys.argv[0] for module in ["submit"])
             and self.args.follow
             and sys.version_info >= (3, 10)
         ):
             print(
                 datetime.now().strftime("%Y-%m-%d %H:%M:%S"),
                 ":",
-                "Note: the '--follow' ('-f') option is partially supported "
-                "for Python versions 3.10 and above",
+                (
+                    "Note: the '--follow' ('-f') option is partially supported "
+                    "for Python versions 3.10 and above"
+                ),
             )
 
     @property
     def config_file(self) -> Optional[str]:
         return self.args.config
 
     @property
```

### Comparing `yellowdog-python-examples-5.0.6/yd_commands/cancel.py` & `yellowdog-python-examples-5.0.7/yd_commands/cancel.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,30 +28,30 @@
 
 ABORT_RETRY_INTERVAL = 20  # Seconds
 
 
 @main_wrapper
 def main():
     print_log(
-        f"Cancelling Work Requirements in "
+        "Cancelling Work Requirements in "
         f"namespace '{CONFIG_COMMON.namespace}' and "
         f"tag starting with '{CONFIG_COMMON.name_tag}'"
     )
 
-    selected_work_requirement_summaries: List[
-        WorkRequirementSummary
-    ] = get_filtered_work_requirements(
-        client=CLIENT,
-        namespace=CONFIG_COMMON.namespace,
-        tag=CONFIG_COMMON.name_tag,
-        exclude_filter=[
-            WorkRequirementStatus.COMPLETED,
-            WorkRequirementStatus.CANCELLED,
-            WorkRequirementStatus.FAILED,
-        ],
+    selected_work_requirement_summaries: List[WorkRequirementSummary] = (
+        get_filtered_work_requirements(
+            client=CLIENT,
+            namespace=CONFIG_COMMON.namespace,
+            tag=CONFIG_COMMON.name_tag,
+            exclude_filter=[
+                WorkRequirementStatus.COMPLETED,
+                WorkRequirementStatus.CANCELLED,
+                WorkRequirementStatus.FAILED,
+            ],
+        )
     )
 
     cancelled_count = 0
     cancelling_count = 0
 
     if len(selected_work_requirement_summaries) > 0:
         selected_work_requirement_summaries = select(
@@ -122,17 +122,17 @@
                 statuses=[TaskStatus.EXECUTING],
             )
             tasks: List[Task] = CLIENT.work_client.find_tasks(task_search)
             for task in tasks:
                 try:
                     CLIENT.work_client.cancel_task(task, abort=True)
                     print_log(
-                        f"Aborting Task '{task.name}' "
-                        f"in Task Group '{get_task_group_name(CLIENT, wr_summary, task)}' "
-                        f"in Work Requirement '{wr_summary.name}'"
+                        f"Aborting Task '{task.name}' in Task Group"
+                        f" '{get_task_group_name(CLIENT, wr_summary, task)}' in Work"
+                        f" Requirement '{wr_summary.name}'"
                     )
                     aborted_tasks += 1
                 except Exception as e:
                     print_log(f"Error: {e}")
                     continue
     if aborted_tasks == 0:
         print_log("No Tasks to abort")
```

### Comparing `yellowdog-python-examples-5.0.6/yd_commands/check_imports.py` & `yellowdog-python-examples-5.0.7/yd_commands/check_imports.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.6/yd_commands/compact_json.py` & `yellowdog-python-examples-5.0.7/yd_commands/compact_json.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.6/yd_commands/config.py` & `yellowdog-python-examples-5.0.7/yd_commands/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
     verify_at_start: List[str] = field(default_factory=list)
     verify_wait: List[str] = field(default_factory=list)
     worker_tags: Optional[List[str]] = None
     wr_data_file: Optional[str] = None
     wr_name: Optional[str] = None
 
 
-CR_BATCH_SIZE_DEFAULT = 2000
+CR_BATCH_SIZE_DEFAULT = 10000
 
 
 @dataclass
 class ConfigWorkerPool:
     asc_all_nodes_inactive: Optional[float] = None
     asc_all_workers_released: Optional[float] = None
     asc_node_action_failed: Optional[float] = None
```

### Comparing `yellowdog-python-examples-5.0.6/yd_commands/config_keys.py` & `yellowdog-python-examples-5.0.7/yd_commands/config_keys.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.6/yd_commands/csv_data.py` & `yellowdog-python-examples-5.0.7/yd_commands/csv_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,15 +164,15 @@
 def perform_csv_task_expansion(wr_data: Dict, csv_files: List[str]) -> Dict:
     """
     Expand a Work Requirement using CSV data.
     """
     if len(wr_data[TASK_GROUPS]) > len(csv_files):
         print_log(
             f"Note: Number of Task Groups ({len(wr_data[TASK_GROUPS])}) "
-            f"in Work Requirement is greater than number of CSV files "
+            "in Work Requirement is greater than number of CSV files "
             f"({len(csv_files)})"
         )
 
     if len(csv_files) > len(wr_data[TASK_GROUPS]):
         raise Exception("Number of CSV files exceeds number of Task Groups")
 
     for counter, csv_file in enumerate(csv_files):
@@ -191,15 +191,15 @@
             )
 
         csv_data = CSV_DATA_CACHE.get_csv_task_data(csv_file)
         task_prototype = task_group[TASKS][0]
 
         if not substitions_present(csv_data.var_names, str(task_prototype)):
             print_log(
-                f"Warning: No CSV substitutions to apply to Task Group "
+                "Warning: No CSV substitutions to apply to Task Group "
                 f"{index + 1}; not expanding Task list"
             )
             continue
 
         generated_task_list = []
         for task_data in csv_data:
             generated_task_list.append(
```

### Comparing `yellowdog-python-examples-5.0.6/yd_commands/delete.py` & `yellowdog-python-examples-5.0.7/yd_commands/delete.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 
 @main_wrapper
 def main():
     print_log(
         f"Deleting Object Paths in namespace '{CONFIG_COMMON.namespace}' and "
         f"names starting with '{CONFIG_COMMON.name_tag}'"
     )
-    object_paths: List[
-        ObjectPath
-    ] = CLIENT.object_store_client.get_namespace_object_paths(
-        ObjectPathsRequest(CONFIG_COMMON.namespace)
+    object_paths: List[ObjectPath] = (
+        CLIENT.object_store_client.get_namespace_object_paths(
+            ObjectPathsRequest(CONFIG_COMMON.namespace)
+        )
     )
     object_paths_to_delete: List[ObjectPath] = []
     for object_path in object_paths:
         if object_path.name.startswith(CONFIG_COMMON.name_tag):
             object_paths_to_delete.append(object_path)
 
     if len(object_paths_to_delete) > 0:
```

### Comparing `yellowdog-python-examples-5.0.6/yd_commands/download.py` & `yellowdog-python-examples-5.0.7/yd_commands/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,18 +24,18 @@
 def main():
     tag = CONFIG_COMMON.name_tag
     print_log(
         f"Downloading all Objects in namespace '{CONFIG_COMMON.namespace}' and "
         f"names starting with '{tag}'"
     )
 
-    object_paths: List[
-        ObjectPath
-    ] = CLIENT.object_store_client.get_namespace_object_paths(
-        ObjectPathsRequest(CONFIG_COMMON.namespace)
+    object_paths: List[ObjectPath] = (
+        CLIENT.object_store_client.get_namespace_object_paths(
+            ObjectPathsRequest(CONFIG_COMMON.namespace)
+        )
     )
     object_paths_to_download: List[ObjectPath] = []
     for object_path in object_paths:
         if object_path.name.startswith(tag):
             object_paths_to_download.append(object_path)
 
     if len(object_paths_to_download) > 0:
```

### Comparing `yellowdog-python-examples-5.0.6/yd_commands/instantiate.py` & `yellowdog-python-examples-5.0.7/yd_commands/instantiate.py`

 * *Files 1% similar despite different names*

```diff
@@ -223,17 +223,19 @@
     # Some values are configurable via the TOML configuration file;
     # values in the JSON file override values in the TOML file
     try:
         for key, value in [
             # Generate a default name
             (
                 "requirementName",
-                CONFIG_WP.name
-                if CONFIG_WP.name is not None
-                else generate_id("cr" + "_" + CONFIG_COMMON.name_tag),
+                (
+                    CONFIG_WP.name
+                    if CONFIG_WP.name is not None
+                    else generate_id("cr" + "_" + CONFIG_COMMON.name_tag)
+                ),
             ),
             ("requirementNamespace", CONFIG_COMMON.namespace),
             ("requirementTag", CONFIG_COMMON.name_tag),
             ("templateId", CONFIG_WP.template_id),
             ("userData", get_user_data_property(CONFIG_WP)),
             ("imagesId", CONFIG_WP.images_id),
             ("instanceTags", CONFIG_WP.instance_tags),
```

### Comparing `yellowdog-python-examples-5.0.6/yd_commands/interactive.py` & `yellowdog-python-examples-5.0.7/yd_commands/interactive.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,16 +91,15 @@
         else:
             break
 
     selected_list = sorted(list(selector_set))
     if len(selected_list) > 0:
         print(
             print_string(
-                f"Selected item number(s): "
-                f"{', '.join([str(x) for x in selected_list])}"
+                f"Selected item number(s): {', '.join([str(x) for x in selected_list])}"
             )
         )
     else:
         print_log("No items selected")
 
     return [objects[x - 1] for x in selected_list]
```

### Comparing `yellowdog-python-examples-5.0.6/yd_commands/jsonnet2json.py` & `yellowdog-python-examples-5.0.7/yd_commands/jsonnet2json.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.6/yd_commands/list.py` & `yellowdog-python-examples-5.0.7/yd_commands/list.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 """
 Command to list YellowDog entities.
 """
 
 from typing import List
 
 from requests import HTTPError
+from yellowdog_client.common import SearchClient
 from yellowdog_client.model import (
     ComputeRequirement,
+    ComputeRequirementSearch,
     ComputeRequirementStatus,
-    ComputeRequirementSummary,
     ObjectPath,
     ObjectPathsRequest,
     Task,
     TaskGroup,
     TaskSearch,
     WorkerPool,
     WorkerPoolStatus,
@@ -76,34 +77,36 @@
     List Work Requirements whenever --work-requirements, --task-groups or
     --tasks are selected.
 
     This function falls through from WRs to TGs to Tasks, depending on the
     options chosen.
     """
     print_log(
-        f"Listing Work Requirements in 'namespace={CONFIG_COMMON.namespace}' "
-        f"and names starting with 'tag={CONFIG_COMMON.name_tag}'",
+        (
+            f"Listing Work Requirements in 'namespace={CONFIG_COMMON.namespace}' "
+            f"and names starting with 'tag={CONFIG_COMMON.name_tag}'"
+        ),
         override_quiet=True,
     )
     exclude_filter = (
         [
             WorkRequirementStatus.COMPLETED,
             WorkRequirementStatus.CANCELLED,
             WorkRequirementStatus.FAILED,
         ]
         if ARGS_PARSER.live_only
         else []
     )
-    work_requirement_summaries: List[
-        WorkRequirementSummary
-    ] = get_filtered_work_requirements(
-        CLIENT,
-        namespace=CONFIG_COMMON.namespace,
-        tag=CONFIG_COMMON.name_tag,
-        exclude_filter=exclude_filter,
+    work_requirement_summaries: List[WorkRequirementSummary] = (
+        get_filtered_work_requirements(
+            CLIENT,
+            namespace=CONFIG_COMMON.namespace,
+            tag=CONFIG_COMMON.name_tag,
+            exclude_filter=exclude_filter,
+        )
     )
     work_requirement_summaries = sorted_objects(work_requirement_summaries)
     if not (ARGS_PARSER.task_groups or ARGS_PARSER.tasks):
         print_numbered_object_list(
             CLIENT, work_requirement_summaries, override_quiet=True
         )
     else:
@@ -137,31 +140,31 @@
 
 
 def list_object_paths():
     print_log(
         f"Listing Object Paths in namespace '{CONFIG_COMMON.namespace}' and "
         f"names starting with '{CONFIG_COMMON.name_tag}'"
     )
-    object_paths: List[
-        ObjectPath
-    ] = CLIENT.object_store_client.get_namespace_object_paths(
-        ObjectPathsRequest(CONFIG_COMMON.namespace)
+    object_paths: List[ObjectPath] = (
+        CLIENT.object_store_client.get_namespace_object_paths(
+            ObjectPathsRequest(CONFIG_COMMON.namespace)
+        )
     )
     print_numbered_object_list(CLIENT, object_paths)
 
 
 def list_worker_pools():
     print_log(
-        f"Listing Provisioned Worker Pools with Compute Requirements in "
+        "Listing Provisioned Worker Pools with Compute Requirements in "
         f"namespace '{CONFIG_COMMON.namespace}' and "
         f"names starting with '{CONFIG_COMMON.name_tag}'"
     )
-    worker_pool_summaries: List[
-        WorkerPoolSummary
-    ] = CLIENT.worker_pool_client.find_all_worker_pools()
+    worker_pool_summaries: List[WorkerPoolSummary] = (
+        CLIENT.worker_pool_client.find_all_worker_pools()
+    )
 
     selected_worker_pool_summaries: List[WorkerPoolSummary] = []
     excluded_states = (
         [WorkerPoolStatus.TERMINATED, WorkerPoolStatus.SHUTDOWN]
         if ARGS_PARSER.live_only
         else []
     )
@@ -194,41 +197,47 @@
     print_numbered_object_list(
         CLIENT, selected_worker_pool_summaries, override_quiet=True
     )
 
 
 def list_compute_requirements():
     print_log(
-        f"Listing Compute Requirements in "
+        "Listing Compute Requirements in "
         f"namespace '{CONFIG_COMMON.namespace}' and "
         f" names starting with '{CONFIG_COMMON.name_tag}'"
     )
 
-    compute_requirement_summaries: List[
-        ComputeRequirementSummary
-    ] = CLIENT.compute_client.find_all_compute_requirements()
+    cr_search = ComputeRequirementSearch(
+        namespace=CONFIG_COMMON.namespace,
+    )
+    search_client: SearchClient = CLIENT.compute_client.get_compute_requirements(
+        cr_search
+    )
+    compute_requirements: List[ComputeRequirement] = search_client.list_all()
 
-    filtered_compute_requirement_summaries: List[ComputeRequirementSummary] = []
+    filtered_compute_requirements: List[ComputeRequirement] = []
     excluded_states = (
         [ComputeRequirementStatus.TERMINATED, ComputeRequirementStatus.TERMINATING]
         if ARGS_PARSER.live_only
         else []
     )
-    for compute_summary in compute_requirement_summaries:
-        compute_summary.tag = "" if compute_summary.tag is None else compute_summary.tag
+    for compute_requirement in compute_requirements:
+        compute_requirement.tag = (
+            "" if compute_requirement.tag is None else compute_requirement.tag
+        )
         if (
-            compute_summary.tag.startswith(CONFIG_COMMON.name_tag)
-            and compute_summary.namespace == CONFIG_COMMON.namespace
-            and compute_summary.status not in excluded_states
+            compute_requirement.tag.startswith(CONFIG_COMMON.name_tag)
+            and compute_requirement.namespace == CONFIG_COMMON.namespace
+            and compute_requirement.status not in excluded_states
         ):
-            filtered_compute_requirement_summaries.append(compute_summary)
+            filtered_compute_requirements.append(compute_requirement)
 
     print_numbered_object_list(
         CLIENT,
-        sorted_objects(filtered_compute_requirement_summaries),
+        sorted_objects(filtered_compute_requirements),
         override_quiet=True,
     )
 
 
 # Entry point
 if __name__ == "__main__":
     main()
```

### Comparing `yellowdog-python-examples-5.0.6/yd_commands/object_utilities.py` & `yellowdog-python-examples-5.0.7/yd_commands/object_utilities.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 from functools import lru_cache
 from typing import List, Optional, TypeVar
 
 from yellowdog_client import PlatformClient
 from yellowdog_client.model import (
-    ComputeRequirementSummary,
+    ComputeRequirement,
     ConfiguredWorkerPool,
     ObjectPath,
     ProvisionedWorkerPool,
     Task,
     TaskGroup,
     WorkerPool,
     WorkerPoolSummary,
@@ -61,17 +61,17 @@
 
     # Avoid mutable keyword argument defaults
     include_filter = [] if include_filter is None else include_filter
     exclude_filter = [] if exclude_filter is None else exclude_filter
 
     filtered_work_summaries: List[WorkRequirementSummary] = []
 
-    work_requirement_summaries: List[
-        WorkRequirementSummary
-    ] = client.work_client.find_all_work_requirements()
+    work_requirement_summaries: List[WorkRequirementSummary] = (
+        client.work_client.find_all_work_requirements()
+    )
 
     for work_summary in work_requirement_summaries:
         work_summary.tag = "" if work_summary.tag is None else work_summary.tag
         if (
             work_summary.status in include_filter
             or not work_summary.status in exclude_filter
             and work_summary.namespace == namespace
@@ -81,15 +81,15 @@
 
     return filtered_work_summaries
 
 
 Item = TypeVar(
     "Item",
     ConfiguredWorkerPool,
-    ComputeRequirementSummary,
+    ComputeRequirement,
     ObjectPath,
     ProvisionedWorkerPool,
     Task,
     TaskGroup,
     WorkerPoolSummary,
     WorkRequirementSummary,
 )
```

### Comparing `yellowdog-python-examples-5.0.6/yd_commands/printing.py` & `yellowdog-python-examples-5.0.7/yd_commands/printing.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 
 from tabulate import tabulate
 from yellowdog_client import PlatformClient
 from yellowdog_client.common.json import Json
 from yellowdog_client.model import (
     BestComputeSourceReport,
     BestComputeSourceReportSource,
+    ComputeRequirement,
     ComputeRequirementDynamicTemplateTestResult,
-    ComputeRequirementSummary,
     ComputeRequirementTemplateTestResult,
     ComputeRequirementTemplateUsage,
     ConfiguredWorkerPool,
     ObjectPath,
     ProvisionedWorkerPool,
     ProvisionedWorkerPoolProperties,
     Task,
@@ -76,15 +76,15 @@
     print(print_string(f"Error: {error_obj}"), file=sys.stderr, flush=True)
 
 
 TYPE_MAP = {
     ConfiguredWorkerPool: "Configured Worker Pool",
     ProvisionedWorkerPool: "Provisioned Worker Pool",
     WorkerPoolSummary: "Worker Pool",
-    ComputeRequirementSummary: "Compute Requirement",
+    ComputeRequirement: "Compute Requirement",
     Task: "Task",
     TaskGroup: "Task Group",
     WorkRequirementSummary: "Work Requirement",
     ObjectPath: "Object Path",
 }
 
 
@@ -92,24 +92,24 @@
     """
     Get the display name of an object's type.
     """
     return TYPE_MAP.get(type(obj), "")
 
 
 def compute_requirement_table(
-    cr_summary_list: List[ComputeRequirementSummary],
+    cr_list: List[ComputeRequirement],
 ) -> List[List]:
     table = []
-    for index, cr_summary in enumerate(cr_summary_list):
+    for index, cr in enumerate(cr_list):
         table.append(
             [
                 index + 1,
                 ":",
-                cr_summary.name,
-                f"[{cr_summary.status}]",
+                cr.name,
+                f"[{cr.status}]",
             ]
         )
     return table
 
 
 def work_requirement_table(
     wr_summary_list: List[WorkRequirementSummary],
@@ -187,15 +187,15 @@
 
     print_log(
         f"Displaying matching {get_type_name(objects[0])}(s):",
         override_quiet=override_quiet,
     )
     print()
 
-    if isinstance(objects[0], ComputeRequirementSummary):
+    if isinstance(objects[0], ComputeRequirement):
         table = compute_requirement_table(objects)
     elif isinstance(objects[0], WorkRequirementSummary):
         table = work_requirement_table(objects)
     elif isinstance(objects[0], TaskGroup):
         table = task_group_table(objects)
     elif isinstance(objects[0], Task):
         table = task_table(objects)
@@ -353,9 +353,9 @@
                 source.type,
                 source.region,
                 source.instanceType,
                 source.name,
             ]
         )
     print()
-    print(tabulate(source_table, headers="firstrow", tablefmt="simple_grid"))
+    print(tabulate(source_table, headers="firstrow", tablefmt="simple_outline"))
     print()
```

### Comparing `yellowdog-python-examples-5.0.6/yd_commands/provision.py` & `yellowdog-python-examples-5.0.7/yd_commands/provision.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,17 +92,19 @@
     try:
         # requirementTemplateUsage insertions
         reqt_template_usage: Dict = wp_data["requirementTemplateUsage"]
         for key, value in [
             # Generate a default name
             (
                 "requirementName",
-                CONFIG_WP.name
-                if CONFIG_WP.name is not None
-                else generate_id("wp" + "_" + CONFIG_COMMON.name_tag),
+                (
+                    CONFIG_WP.name
+                    if CONFIG_WP.name is not None
+                    else generate_id("wp" + "_" + CONFIG_COMMON.name_tag)
+                ),
             ),
             ("requirementNamespace", CONFIG_COMMON.namespace),
             ("requirementTag", CONFIG_COMMON.name_tag),
             ("templateId", CONFIG_WP.template_id),
             ("userData", get_user_data_property(CONFIG_WP)),
             ("imagesId", CONFIG_WP.images_id),
             ("instanceTags", CONFIG_WP.instance_tags),
@@ -148,27 +150,27 @@
             )
         )
 
         type_prefix = "co.yellowdog.platform.model"
         auto_shutdown_conditions = [
             {
                 "delay": asc_all_nodes_inactive,
-                "type": (f"{type_prefix}.AllNodesInactiveShutdownCondition"),
+                "type": f"{type_prefix}.AllNodesInactiveShutdownCondition",
             },
             {
                 "delay": asc_all_workers_released,
-                "type": (f"{type_prefix}.AllWorkersReleasedShutdownCondition"),
+                "type": f"{type_prefix}.AllWorkersReleasedShutdownCondition",
             },
             {
                 "delay": asc_node_action_failed,
-                "type": (f"{type_prefix}.NodeActionFailedShutdownCondition"),
+                "type": f"{type_prefix}.NodeActionFailedShutdownCondition",
             },
             {
                 "delay": asc_unclaimed_after_startup,
-                "type": (f"{type_prefix}.UnclaimedAfterStartupShutdownCondition"),
+                "type": f"{type_prefix}.UnclaimedAfterStartupShutdownCondition",
             },
         ]
         if CONFIG_WP.asc_no_registered_workers is True:
             auto_shutdown_conditions.append(
                 {"type": f"{type_prefix}.NoRegisteredWorkersShutdownCondition"}
             )
 
@@ -370,19 +372,19 @@
                 )
 
         except Exception as e:
             print_error(f"Unable to provision worker pool")
             raise Exception(e)
 
     print_log(
-        f"Node boot time limit is "
+        "Node boot time limit is "
         f"{CONFIG_WP.node_boot_time_limit} minute(s) | "
-        f"Node idle grace period is "
+        "Node idle grace period is "
         f"{CONFIG_WP.node_idle_grace_period} minute(s) | "
-        f"Node idle time limit is "
+        "Node idle time limit is "
         f"{CONFIG_WP.node_idle_time_limit} minute(s)"
     )
 
     auto_shutdown = "enabled" if CONFIG_WP.auto_shutdown is True else "disabled"
     auto_shutdown_msg = f"Auto-Shutdown is {auto_shutdown}"
     auto_shutdown_msg = (
         auto_shutdown_msg
```

### Comparing `yellowdog-python-examples-5.0.6/yd_commands/provision_utils.py` & `yellowdog-python-examples-5.0.7/yd_commands/provision_utils.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.6/yd_commands/reformat_json.py` & `yellowdog-python-examples-5.0.7/yd_commands/reformat_json.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.6/yd_commands/shutdown.py` & `yellowdog-python-examples-5.0.7/yd_commands/shutdown.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,21 +20,21 @@
 from yd_commands.printing import print_error, print_log
 from yd_commands.wrapper import CLIENT, CONFIG_COMMON, main_wrapper
 
 
 @main_wrapper
 def main():
     print_log(
-        f"Shutting down Worker Pools with Compute Requirements in "
+        "Shutting down Worker Pools with Compute Requirements in "
         f"namespace '{CONFIG_COMMON.namespace}' and "
         f"tag starting with '{CONFIG_COMMON.name_tag}'"
     )
-    worker_pool_summaries: List[
-        WorkerPoolSummary
-    ] = CLIENT.worker_pool_client.find_all_worker_pools()
+    worker_pool_summaries: List[WorkerPoolSummary] = (
+        CLIENT.worker_pool_client.find_all_worker_pools()
+    )
     shutdown_count = 0
 
     selected_worker_pool_summaries: List[WorkerPoolSummary] = []
     for worker_pool_summary in worker_pool_summaries:
         if not (
             "ProvisionedWorkerPool" not in worker_pool_summary.type
             or worker_pool_summary.status
```

### Comparing `yellowdog-python-examples-5.0.6/yd_commands/submit.py` & `yellowdog-python-examples-5.0.7/yd_commands/submit.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,15 +250,15 @@
         tag=CONFIG_COMMON.name_tag,
         priority=priority,
         fulfilOnSubmit=fulfilOnSubmit,
     )
     if not ARGS_PARSER.dry_run:
         work_requirement = CLIENT.work_client.add_work_requirement(work_requirement)
         print_log(
-            f"Created "
+            "Created "
             f"{link_entity(CONFIG_COMMON.url, work_requirement)} "
             f"({work_requirement.name})"
         )
     else:
         global WR_SNAPSHOT
         WR_SNAPSHOT.set_work_requirement(work_requirement)
 
@@ -713,26 +713,27 @@
         else:
             global WR_SNAPSHOT
             WR_SNAPSHOT.add_tasks(task_group.name, tasks_list)
 
         if not ARGS_PARSER.dry_run:
             if num_task_batches > 1:
                 print_log(
-                    f"Batch {str(batch_number + 1).zfill(len(str(num_task_batches)))} : "
-                    f"Added {len(tasks_list):,d} "
-                    f"Task(s) to Work Requirement Task Group '{task_group.name}'"
+                    f"Batch {str(batch_number + 1).zfill(len(str(num_task_batches)))} :"
+                    f" Added {len(tasks_list):,d} Task(s) to Work Requirement Task"
+                    f" Group '{task_group.name}'"
                 )
 
         # Empty the task list for the next batch
         tasks_list.clear()
 
     if not ARGS_PARSER.dry_run:
         if num_tasks > 0:
             print_log(
-                f"Added a total of {num_tasks} Task(s) to Task Group '{task_group.name}'"
+                f"Added a total of {num_tasks} Task(s) to Task Group"
+                f" '{task_group.name}'"
             )
         else:
             print_log(f"No Tasks added to Task Group '{task_group.name}'")
 
 
 def get_task_data_property(
     wr_data: Dict, task_group_data: Dict, task: Dict, task_name: str
@@ -786,15 +787,15 @@
     completed = 0
     total = 0
     for task_group in work_req.taskGroups:
         completed += task_group.taskSummary.statusCounts[TaskStatus.COMPLETED]
         total += task_group.taskSummary.taskCount
     print_log(
         f"WORK REQUIREMENT is {work_req.status} with {completed}/{total} "
-        f"COMPLETED TASKS"
+        "COMPLETED TASKS"
     )
 
 
 def cleanup_on_failure(work_requirement: WorkRequirement) -> None:
     """
     Clean up the Work Requirement and any uploaded Objects on failure
     """
@@ -972,22 +973,24 @@
             ),
             verification=TaskInputVerification.VERIFY_AT_START,
         )
         # Avoid duplicate TaskInputs
         if task_input.objectNamePattern not in [x.objectNamePattern for x in inputs]:
             inputs.append(task_input)
         args = [
-            unique_upload_pathname(
-                filename=executable,
-                id=ID,
-                inputs_folder_name=INPUTS_FOLDER_NAME,
-                flatten_upload_paths=flatten_upload_paths,
+            (
+                unique_upload_pathname(
+                    filename=executable,
+                    id=ID,
+                    inputs_folder_name=INPUTS_FOLDER_NAME,
+                    flatten_upload_paths=flatten_upload_paths,
+                )
+                if flatten_input_paths is None
+                else basename(executable)
             )
-            if flatten_input_paths is None
-            else basename(executable)
         ] + args
         return _make_task(flatten_input_paths)
 
     # Special processing for Docker tasks if the 'executable property is set.
     # Sets up the '-e' environment strings and the DockerHub username and
     # password if specified.
     elif task_type == "docker":
@@ -1147,15 +1150,17 @@
             response = requests.post(
                 url=(
                     f"{CONFIG_COMMON.url}/work/namespaces/"
                     f"{CONFIG_COMMON.namespace}/requirements/{wr_name}/"
                     f"taskGroups/{task_group_name}/tasks"
                 ),
                 headers={
-                    "Authorization": f"yd-key {CONFIG_COMMON.key}:{CONFIG_COMMON.secret}"
+                    "Authorization": (
+                        f"yd-key {CONFIG_COMMON.key}:{CONFIG_COMMON.secret}"
+                    )
                 },
                 json=task_batch,
             )
 
             if response.status_code == 200:
                 print_log(
                     f"Added {len(task_batch)} Task(s) to Task Group "
```

### Comparing `yellowdog-python-examples-5.0.6/yd_commands/submit_utils.py` & `yellowdog-python-examples-5.0.7/yd_commands/submit_utils.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.6/yd_commands/terminate.py` & `yellowdog-python-examples-5.0.7/yd_commands/terminate.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,79 +2,83 @@
 
 """
 A script to terminate Compute Requirements.
 """
 
 from typing import List
 
+from yellowdog_client.common import SearchClient
 from yellowdog_client.model import (
     ComputeRequirement,
+    ComputeRequirementSearch,
     ComputeRequirementStatus,
-    ComputeRequirementSummary,
 )
 
 from yd_commands.config import link_entity
 from yd_commands.interactive import confirmed, select
 from yd_commands.printing import print_error, print_log
 from yd_commands.wrapper import CLIENT, CONFIG_COMMON, main_wrapper
 
 
 @main_wrapper
 def main():
     print_log(
-        f"Terminating Compute Requirements in "
+        "Terminating Compute Requirements in "
         f"namespace '{CONFIG_COMMON.namespace}' and tag "
         f"starting with '{CONFIG_COMMON.name_tag}'"
     )
 
-    compute_requirement_summaries: List[
-        ComputeRequirementSummary
-    ] = CLIENT.compute_client.find_all_compute_requirements()
+    cr_search = ComputeRequirementSearch(
+        namespace=CONFIG_COMMON.namespace,
+        statuses=[
+            ComputeRequirementStatus.NEW,
+            ComputeRequirementStatus.PROVISIONING,
+            ComputeRequirementStatus.STARTING,
+            ComputeRequirementStatus.RUNNING,
+            ComputeRequirementStatus.STOPPING,
+        ],
+        # Excludes TERMINATED, TERMINATING
+    )
+    search_client: SearchClient = CLIENT.compute_client.get_compute_requirements(
+        cr_search
+    )
+    compute_requirements: List[ComputeRequirement] = search_client.list_all()
 
     terminated_count = 0
-    selected_compute_requirement_summaries: List[ComputeRequirementSummary] = []
+    selected_compute_requirements: List[ComputeRequirement] = []
 
-    for compute_summary in compute_requirement_summaries:
-        compute_summary.tag = "" if compute_summary.tag is None else compute_summary.tag
-        if (
-            compute_summary.tag.startswith(CONFIG_COMMON.name_tag)
-            and compute_summary.namespace == CONFIG_COMMON.namespace
-            and compute_summary.status
-            not in [
-                ComputeRequirementStatus.TERMINATED,
-                ComputeRequirementStatus.TERMINATING,
-            ]
-        ):
-            selected_compute_requirement_summaries.append(compute_summary)
-
-    if len(selected_compute_requirement_summaries) > 0:
-        selected_compute_requirement_summaries = select(
-            CLIENT, selected_compute_requirement_summaries
+    for compute_requirement in compute_requirements:
+        compute_requirement.tag = (
+            "" if compute_requirement.tag is None else compute_requirement.tag
         )
+        if compute_requirement.tag.startswith(CONFIG_COMMON.name_tag):
+            selected_compute_requirements.append(compute_requirement)
+
+    if len(selected_compute_requirements) > 0:
+        selected_compute_requirements = select(CLIENT, selected_compute_requirements)
 
-    if len(selected_compute_requirement_summaries) > 0 and confirmed(
-        f"Terminate {len(selected_compute_requirement_summaries)} "
-        "Compute Requirement(s)?"
+    if len(selected_compute_requirements) > 0 and confirmed(
+        f"Terminate {len(selected_compute_requirements)} Compute Requirement(s)?"
     ):
-        for compute_summary in selected_compute_requirement_summaries:
+        for compute_requirement in selected_compute_requirements:
             try:
                 CLIENT.compute_client.terminate_compute_requirement_by_id(
-                    compute_summary.id
+                    compute_requirement.id
                 )
                 compute_requirement: ComputeRequirement = (
                     CLIENT.compute_client.get_compute_requirement_by_id(
-                        compute_summary.id
+                        compute_requirement.id
                     )
                 )
                 terminated_count += 1
                 print_log(
                     f"Terminated {link_entity(CONFIG_COMMON.url, compute_requirement)}"
                 )
             except:
-                print_error(f"Unable to terminate '{compute_summary.name}'")
+                print_error(f"Unable to terminate '{compute_requirement.name}'")
 
     if terminated_count > 0:
         print_log(f"Terminated {terminated_count} Compute Requirement(s)")
     else:
         print_log("No Compute Requirements terminated")
```

### Comparing `yellowdog-python-examples-5.0.6/yd_commands/type_check.py` & `yellowdog-python-examples-5.0.7/yd_commands/type_check.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.6/yd_commands/upload.py` & `yellowdog-python-examples-5.0.7/yd_commands/upload.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,15 @@
 
 
 @main_wrapper
 def main():
     if ARGS_PARSER.content_path is not None and ARGS_PARSER.content_path != "":
         chdir(ARGS_PARSER.content_path)
         print_log(
-            "Uploading files relative to local directory: "
-            f"'{ARGS_PARSER.content_path}'"
+            f"Uploading files relative to local directory: '{ARGS_PARSER.content_path}'"
         )
 
     print_log(
         f"Using Object Store namespace '{CONFIG_COMMON.namespace}' "
         f"and directory '{ARGS_PARSER.directory}'"
     )
```

### Comparing `yellowdog-python-examples-5.0.6/yd_commands/upload_utils.py` & `yellowdog-python-examples-5.0.7/yd_commands/upload_utils.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.6/yd_commands/validate_properties.py` & `yellowdog-python-examples-5.0.7/yd_commands/validate_properties.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.6/yd_commands/variables.py` & `yellowdog-python-examples-5.0.7/yd_commands/variables.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 # Directives from the command line (take precedence over environment variables)
 if ARGS_PARSER.variables is not None:
     for variable in ARGS_PARSER.variables:
         key_value: List = variable.split("=")
         if len(key_value) == 2:
             VARIABLE_SUBSTITUTIONS[key_value[0]] = key_value[1]
             print_log(
-                f"Adding command-line-defined variable substitution: "
+                "Adding command-line-defined variable substitution: "
                 f"'{key_value[0]}' = '{key_value[1]}'"
             )
         else:
             print_error(
                 f"Error in variable substitution '{key_value[0]}'",
             )
             print_log("Done")
@@ -177,15 +177,15 @@
         try:
             replaced_number = int(replaced)
         except ValueError:
             try:
                 replaced_number = float(replaced)
             except ValueError:
                 raise Exception(
-                    f"Non-number used in variable number "
+                    "Non-number used in variable number "
                     f"substitution: '{input}':'{replaced}'"
                 )
         return replaced_number
 
     if input.startswith(f"{{{{{BOOL_SUB}"):
         input_variable = input.replace(BOOL_SUB, "")
         if _remove_variable_brackets(input_variable) not in VARIABLE_SUBSTITUTIONS:
@@ -194,16 +194,15 @@
             return input
         replaced = simple_variable_substitution(input_variable)
         if replaced.lower() == "true":
             return True
         if replaced.lower() == "false":
             return False
         raise Exception(
-            f"Non-boolean used in variable boolean "
-            f"substitution: '{input}':'{replaced}'"
+            f"Non-boolean used in variable boolean substitution: '{input}':'{replaced}'"
         )
 
     # Note: this will break if variable substitutions intended for this
     # preprocessor are mixed with those intended to be passed through
     return simple_variable_substitution(input)
```

### Comparing `yellowdog-python-examples-5.0.6/yd_commands/version.py` & `yellowdog-python-examples-5.0.7/yd_commands/version.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.6/yd_commands/wrapper.py` & `yellowdog-python-examples-5.0.7/yd_commands/wrapper.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.6/yellowdog_python_examples.egg-info/PKG-INFO` & `yellowdog-python-examples-5.0.7/yellowdog_python_examples.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yellowdog-python-examples
-Version: 5.0.6
+Version: 5.0.7
 Summary: Example Python commands using the YellowDog Python SDK
 Home-page: https://github.com/yellowdog/python-examples
 Author: YellowDog Limited
 Author-email: YellowDog Limited <support@yellowdog.co>
 Project-URL: Homepage, https://github.com/yellowdog/python-examples
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `yellowdog-python-examples-5.0.6/yellowdog_python_examples.egg-info/SOURCES.txt` & `yellowdog-python-examples-5.0.7/yellowdog_python_examples.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.6/yellowdog_python_examples.egg-info/entry_points.txt` & `yellowdog-python-examples-5.0.7/yellowdog_python_examples.egg-info/entry_points.txt`

 * *Files identical despite different names*

