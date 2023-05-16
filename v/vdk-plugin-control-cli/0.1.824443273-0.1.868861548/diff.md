# Comparing `tmp/vdk-plugin-control-cli-0.1.824443273.tar.gz` & `tmp/vdk-plugin-control-cli-0.1.868861548.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vdk-plugin-control-cli-0.1.824443273.tar", last modified: Fri Mar 31 14:26:00 2023, max compression
+gzip compressed data, was "vdk-plugin-control-cli-0.1.868861548.tar", last modified: Tue May 16 12:39:55 2023, max compression
```

## Comparing `vdk-plugin-control-cli-0.1.824443273.tar` & `vdk-plugin-control-cli-0.1.868861548.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:26:00.734694 vdk-plugin-control-cli-0.1.824443273/
--rw-r--r--   0 root         (0) root         (0)     2168 2023-03-31 14:26:00.730694 vdk-plugin-control-cli-0.1.824443273/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1535 2023-03-31 14:25:49.000000 vdk-plugin-control-cli-0.1.824443273/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-31 14:26:00.734694 vdk-plugin-control-cli-0.1.824443273/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1480 2023-03-31 14:25:52.000000 vdk-plugin-control-cli-0.1.824443273/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:26:00.730694 vdk-plugin-control-cli-0.1.824443273/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:26:00.730694 vdk-plugin-control-cli-0.1.824443273/src/vdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:26:00.730694 vdk-plugin-control-cli-0.1.824443273/src/vdk/plugin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:26:00.730694 vdk-plugin-control-cli-0.1.824443273/src/vdk/plugin/control_cli_plugin/
--rw-rw-rw-   0 root         (0) root         (0)     4665 2023-03-31 14:25:49.000000 vdk-plugin-control-cli-0.1.824443273/src/vdk/plugin/control_cli_plugin/control_service_api_error_decorator.py
--rw-rw-rw-   0 root         (0) root         (0)     4460 2023-03-31 14:25:49.000000 vdk-plugin-control-cli-0.1.824443273/src/vdk/plugin/control_cli_plugin/control_service_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     1493 2023-03-31 14:25:49.000000 vdk-plugin-control-cli-0.1.824443273/src/vdk/plugin/control_cli_plugin/control_service_properties_client.py
--rw-rw-rw-   0 root         (0) root         (0)     7407 2023-03-31 14:25:49.000000 vdk-plugin-control-cli-0.1.824443273/src/vdk/plugin/control_cli_plugin/execution_skip.py
--rw-rw-rw-   0 root         (0) root         (0)     1237 2023-03-31 14:25:49.000000 vdk-plugin-control-cli-0.1.824443273/src/vdk/plugin/control_cli_plugin/properties_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     3750 2023-03-31 14:25:49.000000 vdk-plugin-control-cli-0.1.824443273/src/vdk/plugin/control_cli_plugin/vdk_plugin_control_cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:26:00.730694 vdk-plugin-control-cli-0.1.824443273/src/vdk_plugin_control_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2168 2023-03-31 14:26:00.000000 vdk-plugin-control-cli-0.1.824443273/src/vdk_plugin_control_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      837 2023-03-31 14:26:00.000000 vdk-plugin-control-cli-0.1.824443273/src/vdk_plugin_control_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-31 14:26:00.000000 vdk-plugin-control-cli-0.1.824443273/src/vdk_plugin_control_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      242 2023-03-31 14:26:00.000000 vdk-plugin-control-cli-0.1.824443273/src/vdk_plugin_control_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       34 2023-03-31 14:26:00.000000 vdk-plugin-control-cli-0.1.824443273/src/vdk_plugin_control_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-03-31 14:26:00.000000 vdk-plugin-control-cli-0.1.824443273/src/vdk_plugin_control_cli.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:26:00.730694 vdk-plugin-control-cli-0.1.824443273/tests/
--rw-rw-rw-   0 root         (0) root         (0)     3283 2023-03-31 14:25:49.000000 vdk-plugin-control-cli-0.1.824443273/tests/test_control_service_properties.py
--rw-rw-rw-   0 root         (0) root         (0)     7794 2023-03-31 14:25:49.000000 vdk-plugin-control-cli-0.1.824443273/tests/test_execution_skip.py
--rw-rw-rw-   0 root         (0) root         (0)     2562 2023-03-31 14:25:49.000000 vdk-plugin-control-cli-0.1.824443273/tests/test_properties_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     2669 2023-03-31 14:25:49.000000 vdk-plugin-control-cli-0.1.824443273/tests/test_vdk_plugin_control_cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 12:39:55.916908 vdk-plugin-control-cli-0.1.868861548/
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-05-16 12:39:55.916908 vdk-plugin-control-cli-0.1.868861548/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1535 2023-05-16 12:39:41.000000 vdk-plugin-control-cli-0.1.868861548/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-16 12:39:55.916908 vdk-plugin-control-cli-0.1.868861548/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1480 2023-05-16 12:39:45.000000 vdk-plugin-control-cli-0.1.868861548/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 12:39:55.916908 vdk-plugin-control-cli-0.1.868861548/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 12:39:55.916908 vdk-plugin-control-cli-0.1.868861548/src/vdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 12:39:55.916908 vdk-plugin-control-cli-0.1.868861548/src/vdk/plugin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 12:39:55.916908 vdk-plugin-control-cli-0.1.868861548/src/vdk/plugin/control_cli_plugin/
+-rw-rw-rw-   0 root         (0) root         (0)     4665 2023-05-16 12:39:41.000000 vdk-plugin-control-cli-0.1.868861548/src/vdk/plugin/control_cli_plugin/control_service_api_error_decorator.py
+-rw-rw-rw-   0 root         (0) root         (0)     4460 2023-05-16 12:39:41.000000 vdk-plugin-control-cli-0.1.868861548/src/vdk/plugin/control_cli_plugin/control_service_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     1493 2023-05-16 12:39:41.000000 vdk-plugin-control-cli-0.1.868861548/src/vdk/plugin/control_cli_plugin/control_service_properties_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     7407 2023-05-16 12:39:41.000000 vdk-plugin-control-cli-0.1.868861548/src/vdk/plugin/control_cli_plugin/execution_skip.py
+-rw-rw-rw-   0 root         (0) root         (0)     1237 2023-05-16 12:39:41.000000 vdk-plugin-control-cli-0.1.868861548/src/vdk/plugin/control_cli_plugin/properties_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     3854 2023-05-16 12:39:41.000000 vdk-plugin-control-cli-0.1.868861548/src/vdk/plugin/control_cli_plugin/vdk_plugin_control_cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 12:39:55.916908 vdk-plugin-control-cli-0.1.868861548/src/vdk_plugin_control_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-05-16 12:39:55.000000 vdk-plugin-control-cli-0.1.868861548/src/vdk_plugin_control_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      837 2023-05-16 12:39:55.000000 vdk-plugin-control-cli-0.1.868861548/src/vdk_plugin_control_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 12:39:55.000000 vdk-plugin-control-cli-0.1.868861548/src/vdk_plugin_control_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      242 2023-05-16 12:39:55.000000 vdk-plugin-control-cli-0.1.868861548/src/vdk_plugin_control_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       34 2023-05-16 12:39:55.000000 vdk-plugin-control-cli-0.1.868861548/src/vdk_plugin_control_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-05-16 12:39:55.000000 vdk-plugin-control-cli-0.1.868861548/src/vdk_plugin_control_cli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 12:39:55.916908 vdk-plugin-control-cli-0.1.868861548/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     3283 2023-05-16 12:39:41.000000 vdk-plugin-control-cli-0.1.868861548/tests/test_control_service_properties.py
+-rw-rw-rw-   0 root         (0) root         (0)     7812 2023-05-16 12:39:41.000000 vdk-plugin-control-cli-0.1.868861548/tests/test_execution_skip.py
+-rw-rw-rw-   0 root         (0) root         (0)     2562 2023-05-16 12:39:41.000000 vdk-plugin-control-cli-0.1.868861548/tests/test_properties_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2669 2023-05-16 12:39:41.000000 vdk-plugin-control-cli-0.1.868861548/tests/test_vdk_plugin_control_cli.py
```

### Comparing `vdk-plugin-control-cli-0.1.824443273/PKG-INFO` & `vdk-plugin-control-cli-0.1.868861548/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-plugin-control-cli
-Version: 0.1.824443273
+Version: 0.1.868861548
 Summary: Versatile Data Kit SDK plugin exposing CLI commands for managing the lifecycle of a Data Jobs.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vdk-plugin-control-cli-0.1.824443273/README.md` & `vdk-plugin-control-cli-0.1.868861548/README.md`

 * *Files identical despite different names*

### Comparing `vdk-plugin-control-cli-0.1.824443273/setup.py` & `vdk-plugin-control-cli-0.1.868861548/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import setuptools
 
 """
 Builds a package with the help of setuptools in order for this package to be imported in other projects
 """
 
-__version__ = "0.1.824443273"
+__version__ = "0.1.868861548"
 
 setuptools.setup(
     name="vdk-plugin-control-cli",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="Versatile Data Kit SDK plugin exposing CLI commands for managing the lifecycle of a Data Jobs.",
     long_description=pathlib.Path("README.md").read_text(),
```

### Comparing `vdk-plugin-control-cli-0.1.824443273/src/vdk/plugin/control_cli_plugin/control_service_api_error_decorator.py` & `vdk-plugin-control-cli-0.1.868861548/src/vdk/plugin/control_cli_plugin/control_service_api_error_decorator.py`

 * *Files identical despite different names*

### Comparing `vdk-plugin-control-cli-0.1.824443273/src/vdk/plugin/control_cli_plugin/control_service_configuration.py` & `vdk-plugin-control-cli-0.1.868861548/src/vdk/plugin/control_cli_plugin/control_service_configuration.py`

 * *Files identical despite different names*

### Comparing `vdk-plugin-control-cli-0.1.824443273/src/vdk/plugin/control_cli_plugin/control_service_properties_client.py` & `vdk-plugin-control-cli-0.1.868861548/src/vdk/plugin/control_cli_plugin/control_service_properties_client.py`

 * *Files identical despite different names*

### Comparing `vdk-plugin-control-cli-0.1.824443273/src/vdk/plugin/control_cli_plugin/execution_skip.py` & `vdk-plugin-control-cli-0.1.868861548/src/vdk/plugin/control_cli_plugin/execution_skip.py`

 * *Files identical despite different names*

### Comparing `vdk-plugin-control-cli-0.1.824443273/src/vdk/plugin/control_cli_plugin/properties_plugin.py` & `vdk-plugin-control-cli-0.1.868861548/src/vdk/plugin/control_cli_plugin/properties_plugin.py`

 * *Files identical despite different names*

### Comparing `vdk-plugin-control-cli-0.1.824443273/src/vdk/plugin/control_cli_plugin/vdk_plugin_control_cli.py` & `vdk-plugin-control-cli-0.1.868861548/src/vdk/plugin/control_cli_plugin/vdk_plugin_control_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import click
 from vdk.api.plugin.hook_markers import hookimpl
 from vdk.internal.control.command_groups.common_group.default import (
     reset_default_command,
 )
 from vdk.internal.control.command_groups.common_group.default import set_default_command
+from vdk.internal.control.command_groups.info_group.info import info
 from vdk.internal.control.command_groups.job.create import create
 from vdk.internal.control.command_groups.job.delete import delete
 from vdk.internal.control.command_groups.job.deploy_cli import deploy
 from vdk.internal.control.command_groups.job.download_job import download_job
 from vdk.internal.control.command_groups.job.download_key import download_key
 from vdk.internal.control.command_groups.job.execute import execute
 from vdk.internal.control.command_groups.job.list import list_command
@@ -39,14 +40,15 @@
     root_command.add_command(deploy)
     root_command.add_command(execute)
     root_command.add_command(download_job)
     root_command.add_command(set_default_command)
     root_command.add_command(reset_default_command)
     root_command.add_command(show_command)
     root_command.add_command(properties_command)
+    root_command.add_command(info)
 
     plugins = control_plugin_manager.Plugins()
     default_options = DefaultOptions(plugins)
     if default_options.get_default_map():
         root_command.context_settings["default_map"] = default_options.get_default_map()
```

### Comparing `vdk-plugin-control-cli-0.1.824443273/src/vdk_plugin_control_cli.egg-info/PKG-INFO` & `vdk-plugin-control-cli-0.1.868861548/src/vdk_plugin_control_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-plugin-control-cli
-Version: 0.1.824443273
+Version: 0.1.868861548
 Summary: Versatile Data Kit SDK plugin exposing CLI commands for managing the lifecycle of a Data Jobs.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vdk-plugin-control-cli-0.1.824443273/src/vdk_plugin_control_cli.egg-info/SOURCES.txt` & `vdk-plugin-control-cli-0.1.868861548/src/vdk_plugin_control_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vdk-plugin-control-cli-0.1.824443273/tests/test_control_service_properties.py` & `vdk-plugin-control-cli-0.1.868861548/tests/test_control_service_properties.py`

 * *Files identical despite different names*

### Comparing `vdk-plugin-control-cli-0.1.824443273/tests/test_execution_skip.py` & `vdk-plugin-control-cli-0.1.868861548/tests/test_execution_skip.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,40 +131,40 @@
         assert result is True
 
     def test_real_call(self):
         # This test re creates a real DataJobExecution object received from the API as is.
         # Intention is to get as close as possible to the real API call.
         deployment = {
             "deployed_by": "mzhivkov",
-            "deployed_date": "datetime.datetime(2021, 7, 29, 18, 8, 55, 435596, tzinfo=tzutc())",
+            "deployed_date": "2021-09-23T14:14:03.922Z",
             "enabled": True,
             "id": "release",
             "job_version": "b4d24a249709874ad8c8e43d93ed2824c6ed0292",
             "mode": "release",
             "resources": {
                 "cpu_limit": 0.5,
                 "cpu_request": 0.5,
                 "memory_limit": 1000,
                 "memory_request": 1000,
             },
             "schedule": {"schedule_cron": "*/5 * * * *"},
             "vdk_version": "",
         }
         data_job_execution = DataJobExecution(
-            "mzhivkov-test-job3-latest-1627583589244-9681d",
-            "mzhivkov-test-job3",
-            "running",
-            "manual",
-            "datetime(2021, 7, 29, 18, 33, 9, tzinfo=tzutc())",
-            None,
-            "manual/vdk-control-cli",
-            None,
-            "e61d395859dc4c45",
-            deployment,
-            None,
+            id="mzhivkov-test-job3-latest-1627583589244-9681d",
+            job_name="mzhivkov-test-job3",
+            status="running",
+            type="manual",
+            start_time="2021-09-24T14:14:03.922Z",
+            end_time=None,
+            started_by="manual/vdk-control-cli",
+            logs_url=None,
+            op_id="e61d395859dc4c45",
+            deployment=deployment,
+            # None,
         )
         self.mock_api.data_job_execution_list.return_value = [data_job_execution]
         result = self.checker.is_job_execution_running(
             "mzhivkov-test-job3",
             "supercollider",
             "mzhivkov-test-job3-latest-1627583589244-9681d-tkr4l",
         )
```

### Comparing `vdk-plugin-control-cli-0.1.824443273/tests/test_properties_plugin.py` & `vdk-plugin-control-cli-0.1.868861548/tests/test_properties_plugin.py`

 * *Files identical despite different names*

### Comparing `vdk-plugin-control-cli-0.1.824443273/tests/test_vdk_plugin_control_cli.py` & `vdk-plugin-control-cli-0.1.868861548/tests/test_vdk_plugin_control_cli.py`

 * *Files identical despite different names*

