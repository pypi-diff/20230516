# Comparing `tmp/ovos-PHAL-plugin-dashboard-0.0.1.tar.gz` & `tmp/ovos-PHAL-plugin-dashboard-0.0.2a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-PHAL-plugin-dashboard-0.0.1.tar", last modified: Tue Mar 15 09:25:39 2022, max compression
+gzip compressed data, was "ovos-PHAL-plugin-dashboard-0.0.2a3.tar", last modified: Tue Dec  6 01:47:43 2022, max compression
```

## Comparing `ovos-PHAL-plugin-dashboard-0.0.1.tar` & `ovos-PHAL-plugin-dashboard-0.0.2a3.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 aix       (1000) aix       (1000)        0 2022-03-15 09:25:39.799588 ovos-PHAL-plugin-dashboard-0.0.1/
--rw-r--r--   0 aix       (1000) aix       (1000)    11357 2022-03-15 09:10:58.000000 ovos-PHAL-plugin-dashboard-0.0.1/LICENSE
--rw-r--r--   0 aix       (1000) aix       (1000)      617 2022-03-15 09:25:39.799588 ovos-PHAL-plugin-dashboard-0.0.1/PKG-INFO
-drwxr-xr-x   0 aix       (1000) aix       (1000)        0 2022-03-15 09:25:39.799588 ovos-PHAL-plugin-dashboard-0.0.1/ovos_PHAL_plugin_dashboard/
--rw-r--r--   0 aix       (1000) aix       (1000)     3472 2022-03-15 09:05:58.000000 ovos-PHAL-plugin-dashboard-0.0.1/ovos_PHAL_plugin_dashboard/__init__.py
-drwxr-xr-x   0 aix       (1000) aix       (1000)        0 2022-03-15 09:25:39.799588 ovos-PHAL-plugin-dashboard-0.0.1/ovos_PHAL_plugin_dashboard.egg-info/
--rw-r--r--   0 aix       (1000) aix       (1000)      617 2022-03-15 09:25:39.000000 ovos-PHAL-plugin-dashboard-0.0.1/ovos_PHAL_plugin_dashboard.egg-info/PKG-INFO
--rw-r--r--   0 aix       (1000) aix       (1000)      402 2022-03-15 09:25:39.000000 ovos-PHAL-plugin-dashboard-0.0.1/ovos_PHAL_plugin_dashboard.egg-info/SOURCES.txt
--rw-r--r--   0 aix       (1000) aix       (1000)        1 2022-03-15 09:25:39.000000 ovos-PHAL-plugin-dashboard-0.0.1/ovos_PHAL_plugin_dashboard.egg-info/dependency_links.txt
--rw-r--r--   0 aix       (1000) aix       (1000)       94 2022-03-15 09:25:39.000000 ovos-PHAL-plugin-dashboard-0.0.1/ovos_PHAL_plugin_dashboard.egg-info/entry_points.txt
--rw-r--r--   0 aix       (1000) aix       (1000)       27 2022-03-15 09:25:39.000000 ovos-PHAL-plugin-dashboard-0.0.1/ovos_PHAL_plugin_dashboard.egg-info/requires.txt
--rw-r--r--   0 aix       (1000) aix       (1000)       27 2022-03-15 09:25:39.000000 ovos-PHAL-plugin-dashboard-0.0.1/ovos_PHAL_plugin_dashboard.egg-info/top_level.txt
--rw-r--r--   0 aix       (1000) aix       (1000)        1 2022-03-15 09:25:39.000000 ovos-PHAL-plugin-dashboard-0.0.1/ovos_PHAL_plugin_dashboard.egg-info/zip-safe
--rw-r--r--   0 aix       (1000) aix       (1000)       38 2022-03-15 09:25:39.799588 ovos-PHAL-plugin-dashboard-0.0.1/setup.cfg
--rw-r--r--   0 aix       (1000) aix       (1000)      939 2022-03-15 09:06:03.000000 ovos-PHAL-plugin-dashboard-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 01:47:43.149944 ovos-PHAL-plugin-dashboard-0.0.2a3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2022-12-06 01:47:34.000000 ovos-PHAL-plugin-dashboard-0.0.2a3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2022-12-06 01:47:43.149944 ovos-PHAL-plugin-dashboard-0.0.2a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2022-12-06 01:47:34.000000 ovos-PHAL-plugin-dashboard-0.0.2a3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 01:47:43.145944 ovos-PHAL-plugin-dashboard-0.0.2a3/ovos_PHAL_plugin_dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2022-12-06 01:47:34.000000 ovos-PHAL-plugin-dashboard-0.0.2a3/ovos_PHAL_plugin_dashboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2022-12-06 01:47:37.000000 ovos-PHAL-plugin-dashboard-0.0.2a3/ovos_PHAL_plugin_dashboard/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 01:47:43.149944 ovos-PHAL-plugin-dashboard-0.0.2a3/ovos_PHAL_plugin_dashboard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2022-12-06 01:47:43.000000 ovos-PHAL-plugin-dashboard-0.0.2a3/ovos_PHAL_plugin_dashboard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2022-12-06 01:47:43.000000 ovos-PHAL-plugin-dashboard-0.0.2a3/ovos_PHAL_plugin_dashboard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-06 01:47:43.000000 ovos-PHAL-plugin-dashboard-0.0.2a3/ovos_PHAL_plugin_dashboard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2022-12-06 01:47:43.000000 ovos-PHAL-plugin-dashboard-0.0.2a3/ovos_PHAL_plugin_dashboard.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2022-12-06 01:47:43.000000 ovos-PHAL-plugin-dashboard-0.0.2a3/ovos_PHAL_plugin_dashboard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2022-12-06 01:47:43.000000 ovos-PHAL-plugin-dashboard-0.0.2a3/ovos_PHAL_plugin_dashboard.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-06 01:47:43.000000 ovos-PHAL-plugin-dashboard-0.0.2a3/ovos_PHAL_plugin_dashboard.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-06 01:47:43.149944 ovos-PHAL-plugin-dashboard-0.0.2a3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2022-12-06 01:47:34.000000 ovos-PHAL-plugin-dashboard-0.0.2a3/setup.py
```

### Comparing `ovos-PHAL-plugin-dashboard-0.0.1/LICENSE` & `ovos-PHAL-plugin-dashboard-0.0.2a3/LICENSE`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-dashboard-0.0.1/PKG-INFO` & `ovos-PHAL-plugin-dashboard-0.0.2a3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,16 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: ovos-PHAL-plugin-dashboard
-Version: 0.0.1
+Version: 0.0.2a3
 Summary: A plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-dashboard
 Author: AIIX
 Author-email: aix.m@outlook.com
 License: Apache-2.0
+Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
-License-File: LICENSE
-
-UNKNOWN
-
```

### Comparing `ovos-PHAL-plugin-dashboard-0.0.1/ovos_PHAL_plugin_dashboard/__init__.py` & `ovos-PHAL-plugin-dashboard-0.0.2a3/ovos_PHAL_plugin_dashboard/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,77 +7,65 @@
 from ovos_utils.network_utils import get_ip
 from mycroft_bus_client.message import Message
 from ovos_plugin_manager.phal import PHALPlugin
 
 
 class OVOSDashboardPlugin(PHALPlugin):
     def __init__(self, bus=None, config=None):
-        super().__init__(bus=bus, name="ovos-PHAL-dashboard-plugin", config=config)
+        super().__init__(bus=bus, name="ovos-PHAL-plugin-dashboard",
+                         config=config)
         self.bus = bus
         self.bus.on("ovos.PHAL.dashboard.enable",
                     self.handle_device_developer_enable_dash)
         self.bus.on("ovos.PHAL.dashboard.disable",
                     self.handle_device_developer_disable_dash)
         self.bus.on("ovos.PHAL.dashboard.get.status",
                     self.handle_device_dashboard_status_check)
 
         # Dashboard Specific
-        self.dash_running = None
         alphabet = string.ascii_letters + string.digits
         self.dash_secret = ''.join(secrets.choice(alphabet) for i in range(5))
+        self.username = self.config.get('username') or "OVOS"
+        LOG.info("Dashboard Plugin Initialized")
 
-        LOG.info("Dashboard Plugin Initalized")
+    def handle_device_dashboard_status_check(self, _):
+        if self._check_dash_running():
+            self.bus.emit(Message("ovos.PHAL.dashboard.status.response",
+                                  {"status": True,
+                                   "url": "https://{0}:5000".format(get_ip()),
+                                   "user": self.username,
+                                   "password": self.dash_secret}))
+        else:
+            self.bus.emit(Message("ovos.PHAL.dashboard.status.response",
+                                  {"status": False, "url": None,
+                                   "user": None, "password": None}))
 
-    def handle_device_dashboard_status_check(self):
+    def _check_dash_running(self) -> bool:
         build_status_check_call = "systemctl --user is-active --quiet ovos-dashboard@'{0}'.service".format(
             self.dash_secret)
-        status = os.system(build_status_check_call)
-
-        if status == 0:
-            self.dash_running = True
-        else:
-            self.dash_running = False
-
-        if self.dash_running:
-            self.bus.emit(Message("ovos.PHAL.dashboard.status.response", {
-                          "running": True, "url": "https://{0}:5000".format(get_ip()), "user": "OVOS", "password": self.dash_secret}))
-        else:
-            self.bus.emit(Message("ovos.PHAL.dashboard.status.response", {
-                          "running": False, "url": None, "user": None, "password": None}))
+        dash_status = subprocess.run(build_status_check_call, shell=True,
+                                     env=dict(os.environ))
+        LOG.debug(f"Dash status check got return: {dash_status.returncode}")
+        return dash_status.returncode == 0
 
     def handle_device_developer_enable_dash(self, message):
-        os.environ["SIMPLELOGIN_USERNAME"] = "OVOS"
+        os.environ["SIMPLELOGIN_USERNAME"] = self.username
         os.environ["SIMPLELOGIN_PASSWORD"] = self.dash_secret
         build_call = "systemctl --user start ovos-dashboard@'{0}'.service".format(
             self.dash_secret)
-        call_dash = subprocess.Popen([build_call], shell=True)
-        time.sleep(3)
-        build_status_check_call = "systemctl --user is-active --quiet ovos-dashboard@'{0}'.service".format(
-            self.dash_secret)
-        status = os.system(build_status_check_call)
-
-        if status == 0:
-            self.dash_running = True
-        else:
-            self.dash_running = False
-
-        if self.dash_running:
-            self.bus.emit(Message("ovos.PHAL.dashboard.status.response", {
-                          "running": True, "url": "https://{0}:5000".format(get_ip()), "user": "OVOS", "password": self.dash_secret}))
+        LOG.debug(f'Starting dash with: `{build_call}`')
+        dash_create = subprocess.run(build_call, shell=True,
+                                     env=dict(os.environ))
+        LOG.debug(f'Dash returned: {dash_create.returncode}')
+        # time.sleep(3)
+        self.handle_device_dashboard_status_check(message)
 
     def handle_device_developer_disable_dash(self, message):
         build_call = "systemctl --user stop ovos-dashboard@'{0}'.service".format(
             self.dash_secret)
         subprocess.Popen([build_call], shell=True)
         time.sleep(3)
-        build_status_check_call = "systemctl --user is-active --quiet ovos-dashboard@'{0}'.service".format(
-            self.dash_secret)
-        status = os.system(build_status_check_call)
-
-        if status == 0:
-            self.dash_running = True
-        else:
-            self.dash_running = False
 
-        if not self.dash_running:
-            self.bus.emit(Message("ovos.PHAL.dashboard.status.response", {
-                          "running": False, "url": None, "user": None, "password": None}))
+        if not self._check_dash_running():
+            self.bus.emit(Message("ovos.PHAL.dashboard.status.response",
+                                  {"status": False, "url": None, "user": None,
+                                   "password": None}))
```

### Comparing `ovos-PHAL-plugin-dashboard-0.0.1/ovos_PHAL_plugin_dashboard.egg-info/PKG-INFO` & `ovos-PHAL-plugin-dashboard-0.0.2a3/ovos_PHAL_plugin_dashboard.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,16 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: ovos-PHAL-plugin-dashboard
-Version: 0.0.1
+Version: 0.0.2a3
 Summary: A plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-dashboard
 Author: AIIX
 Author-email: aix.m@outlook.com
 License: Apache-2.0
+Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
-License-File: LICENSE
-
-UNKNOWN
-
```

