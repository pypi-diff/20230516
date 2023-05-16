# Comparing `tmp/dismake-0.0.8.tar.gz` & `tmp/dismake-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dismake-0.0.8.tar", last modified: Tue May 16 09:33:15 2023, max compression
+gzip compressed data, was "dist/dismake-0.0.9.tar", last modified: Tue May 16 09:45:52 2023, max compression
```

## Comparing `dismake-0.0.8.tar` & `dismake-0.0.9.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-05-16 09:33:15.028046 dismake-0.0.8/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       27 2023-05-16 01:23:36.000000 dismake-0.0.8/MANIFEST.in
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     6571 2023-05-16 09:33:15.028046 dismake-0.0.8/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     5078 2023-05-16 01:23:36.000000 dismake-0.0.8/README.md
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-05-16 09:33:15.024047 dismake-0.0.8/dismake/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      205 2023-05-16 01:23:36.000000 dismake-0.0.8/dismake/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1647 2023-05-16 01:23:36.000000 dismake-0.0.8/dismake/asset.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2525 2023-05-16 01:23:36.000000 dismake-0.0.8/dismake/cli.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)    14381 2023-05-16 01:23:36.000000 dismake-0.0.8/dismake/client.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)    20683 2023-05-16 01:23:36.000000 dismake-0.0.8/dismake/commands.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     3670 2023-05-16 01:23:36.000000 dismake-0.0.8/dismake/enums.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1638 2023-05-16 02:15:30.000000 dismake-0.0.8/dismake/errors.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      756 2023-05-16 01:23:36.000000 dismake-0.0.8/dismake/flags.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     9038 2023-05-16 04:36:10.000000 dismake-0.0.8/dismake/handler.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2366 2023-05-16 01:23:36.000000 dismake-0.0.8/dismake/http.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-05-16 09:33:15.028046 dismake-0.0.8/dismake/models/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      275 2023-05-16 01:23:36.000000 dismake-0.0.8/dismake/models/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1309 2023-05-16 01:23:36.000000 dismake-0.0.8/dismake/models/application_command.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2414 2023-05-16 01:23:36.000000 dismake-0.0.8/dismake/models/channels.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1574 2023-05-16 01:23:36.000000 dismake-0.0.8/dismake/models/components.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2694 2023-05-16 01:23:36.000000 dismake-0.0.8/dismake/models/embed.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1015 2023-05-16 01:23:36.000000 dismake-0.0.8/dismake/models/emoji.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     3145 2023-05-16 01:23:36.000000 dismake-0.0.8/dismake/models/guild.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)    13659 2023-05-16 03:24:23.000000 dismake-0.0.8/dismake/models/interaction.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1424 2023-05-16 01:23:36.000000 dismake-0.0.8/dismake/models/message.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      326 2023-05-16 01:23:36.000000 dismake-0.0.8/dismake/models/permission_overwrites.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      804 2023-05-16 01:23:36.000000 dismake-0.0.8/dismake/models/role.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1668 2023-05-16 01:23:36.000000 dismake-0.0.8/dismake/models/user.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1950 2023-05-16 01:23:36.000000 dismake-0.0.8/dismake/params.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2925 2023-05-16 01:23:36.000000 dismake-0.0.8/dismake/permissions.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     8446 2023-05-16 01:23:36.000000 dismake-0.0.8/dismake/plugin.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-05-16 09:33:15.028046 dismake-0.0.8/dismake/templates/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-05-16 01:23:36.000000 dismake-0.0.8/dismake/templates/__init__.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-05-16 09:33:15.028046 dismake-0.0.8/dismake/types/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      156 2023-05-16 01:23:36.000000 dismake-0.0.8/dismake/types/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      163 2023-05-16 01:23:36.000000 dismake-0.0.8/dismake/types/snowflake.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-05-16 09:33:15.028046 dismake-0.0.8/dismake/ui/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      132 2023-05-16 09:31:35.000000 dismake-0.0.8/dismake/ui/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2430 2023-05-16 01:23:36.000000 dismake-0.0.8/dismake/ui/button.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1730 2023-05-16 01:23:36.000000 dismake-0.0.8/dismake/ui/component.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2693 2023-05-16 09:30:40.000000 dismake-0.0.8/dismake/ui/modal.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     5729 2023-05-16 01:23:36.000000 dismake-0.0.8/dismake/ui/select.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     4583 2023-05-16 04:15:06.000000 dismake-0.0.8/dismake/ui/view.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1024 2023-05-16 01:23:36.000000 dismake-0.0.8/dismake/utils.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-05-16 09:33:15.024047 dismake-0.0.8/dismake.egg-info/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     6571 2023-05-16 09:33:15.000000 dismake-0.0.8/dismake.egg-info/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1041 2023-05-16 09:33:15.000000 dismake-0.0.8/dismake.egg-info/SOURCES.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2023-05-16 09:33:15.000000 dismake-0.0.8/dismake.egg-info/dependency_links.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       46 2023-05-16 09:33:15.000000 dismake-0.0.8/dismake.egg-info/entry_points.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      115 2023-05-16 09:33:15.000000 dismake-0.0.8/dismake.egg-info/requires.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        8 2023-05-16 09:33:15.000000 dismake-0.0.8/dismake.egg-info/top_level.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      112 2023-05-16 09:33:15.028046 dismake-0.0.8/setup.cfg
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1113 2023-05-16 09:31:51.000000 dismake-0.0.8/setup.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-05-16 09:33:15.028046 dismake-0.0.8/test/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     6651 2023-05-16 04:46:14.000000 dismake-0.0.8/test/tests.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-05-16 09:45:52.674792 dismake-0.0.9/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       27 2023-05-16 01:23:36.000000 dismake-0.0.9/MANIFEST.in
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     6571 2023-05-16 09:45:52.674792 dismake-0.0.9/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     5078 2023-05-16 01:23:36.000000 dismake-0.0.9/README.md
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-05-16 09:45:52.670792 dismake-0.0.9/dismake/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      205 2023-05-16 09:45:33.000000 dismake-0.0.9/dismake/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1647 2023-05-16 01:23:36.000000 dismake-0.0.9/dismake/asset.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2525 2023-05-16 01:23:36.000000 dismake-0.0.9/dismake/cli.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)    14381 2023-05-16 01:23:36.000000 dismake-0.0.9/dismake/client.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)    20683 2023-05-16 01:23:36.000000 dismake-0.0.9/dismake/commands.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     3670 2023-05-16 01:23:36.000000 dismake-0.0.9/dismake/enums.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1638 2023-05-16 02:15:30.000000 dismake-0.0.9/dismake/errors.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      756 2023-05-16 01:23:36.000000 dismake-0.0.9/dismake/flags.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     9038 2023-05-16 04:36:10.000000 dismake-0.0.9/dismake/handler.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2366 2023-05-16 01:23:36.000000 dismake-0.0.9/dismake/http.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-05-16 09:45:52.674792 dismake-0.0.9/dismake/models/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      275 2023-05-16 01:23:36.000000 dismake-0.0.9/dismake/models/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1309 2023-05-16 01:23:36.000000 dismake-0.0.9/dismake/models/application_command.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2414 2023-05-16 01:23:36.000000 dismake-0.0.9/dismake/models/channels.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1574 2023-05-16 01:23:36.000000 dismake-0.0.9/dismake/models/components.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2694 2023-05-16 01:23:36.000000 dismake-0.0.9/dismake/models/embed.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1015 2023-05-16 01:23:36.000000 dismake-0.0.9/dismake/models/emoji.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     3145 2023-05-16 01:23:36.000000 dismake-0.0.9/dismake/models/guild.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)    13659 2023-05-16 03:24:23.000000 dismake-0.0.9/dismake/models/interaction.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1424 2023-05-16 01:23:36.000000 dismake-0.0.9/dismake/models/message.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      326 2023-05-16 01:23:36.000000 dismake-0.0.9/dismake/models/permission_overwrites.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      804 2023-05-16 01:23:36.000000 dismake-0.0.9/dismake/models/role.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1668 2023-05-16 01:23:36.000000 dismake-0.0.9/dismake/models/user.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1950 2023-05-16 01:23:36.000000 dismake-0.0.9/dismake/params.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2925 2023-05-16 01:23:36.000000 dismake-0.0.9/dismake/permissions.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     8446 2023-05-16 01:23:36.000000 dismake-0.0.9/dismake/plugin.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-05-16 09:45:52.674792 dismake-0.0.9/dismake/templates/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-05-16 01:23:36.000000 dismake-0.0.9/dismake/templates/__init__.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-05-16 09:45:52.674792 dismake-0.0.9/dismake/types/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      156 2023-05-16 01:23:36.000000 dismake-0.0.9/dismake/types/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      163 2023-05-16 01:23:36.000000 dismake-0.0.9/dismake/types/snowflake.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-05-16 09:45:52.674792 dismake-0.0.9/dismake/ui/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      132 2023-05-16 09:31:35.000000 dismake-0.0.9/dismake/ui/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2430 2023-05-16 01:23:36.000000 dismake-0.0.9/dismake/ui/button.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1730 2023-05-16 01:23:36.000000 dismake-0.0.9/dismake/ui/component.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2693 2023-05-16 09:30:40.000000 dismake-0.0.9/dismake/ui/modal.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     5729 2023-05-16 01:23:36.000000 dismake-0.0.9/dismake/ui/select.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     4583 2023-05-16 04:15:06.000000 dismake-0.0.9/dismake/ui/view.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1024 2023-05-16 01:23:36.000000 dismake-0.0.9/dismake/utils.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-05-16 09:45:52.674792 dismake-0.0.9/dismake.egg-info/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     6571 2023-05-16 09:45:52.000000 dismake-0.0.9/dismake.egg-info/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1041 2023-05-16 09:45:52.000000 dismake-0.0.9/dismake.egg-info/SOURCES.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2023-05-16 09:45:52.000000 dismake-0.0.9/dismake.egg-info/dependency_links.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       46 2023-05-16 09:45:52.000000 dismake-0.0.9/dismake.egg-info/entry_points.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      115 2023-05-16 09:45:52.000000 dismake-0.0.9/dismake.egg-info/requires.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        8 2023-05-16 09:45:52.000000 dismake-0.0.9/dismake.egg-info/top_level.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      112 2023-05-16 09:45:52.678792 dismake-0.0.9/setup.cfg
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1123 2023-05-16 09:45:12.000000 dismake-0.0.9/setup.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-05-16 09:45:52.674792 dismake-0.0.9/test/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     6651 2023-05-16 04:46:14.000000 dismake-0.0.9/test/tests.py
```

### Comparing `dismake-0.0.8/PKG-INFO` & `dismake-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dismake
-Version: 0.0.8
+Version: 0.0.9
 Summary: None
 Home-page: https://github.com/Apptic-Development/dismake
 Author: Pranoy Majumdar
 Author-email: officialpranoy2@gmail.com
 License: MIT
 Project-URL: Homepage, https://github.com/Apptic-Development/dismake
 Description: # Introduction to Dismake
```

### Comparing `dismake-0.0.8/README.md` & `dismake-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `dismake-0.0.8/dismake/asset.py` & `dismake-0.0.9/dismake/asset.py`

 * *Files identical despite different names*

### Comparing `dismake-0.0.8/dismake/cli.py` & `dismake-0.0.9/dismake/cli.py`

 * *Files identical despite different names*

### Comparing `dismake-0.0.8/dismake/client.py` & `dismake-0.0.9/dismake/client.py`

 * *Files identical despite different names*

### Comparing `dismake-0.0.8/dismake/commands.py` & `dismake-0.0.9/dismake/commands.py`

 * *Files identical despite different names*

### Comparing `dismake-0.0.8/dismake/enums.py` & `dismake-0.0.9/dismake/enums.py`

 * *Files identical despite different names*

### Comparing `dismake-0.0.8/dismake/errors.py` & `dismake-0.0.9/dismake/errors.py`

 * *Files identical despite different names*

### Comparing `dismake-0.0.8/dismake/flags.py` & `dismake-0.0.9/dismake/flags.py`

 * *Files identical despite different names*

### Comparing `dismake-0.0.8/dismake/handler.py` & `dismake-0.0.9/dismake/handler.py`

 * *Files identical despite different names*

### Comparing `dismake-0.0.8/dismake/http.py` & `dismake-0.0.9/dismake/http.py`

 * *Files identical despite different names*

### Comparing `dismake-0.0.8/dismake/models/application_command.py` & `dismake-0.0.9/dismake/models/application_command.py`

 * *Files identical despite different names*

### Comparing `dismake-0.0.8/dismake/models/channels.py` & `dismake-0.0.9/dismake/models/channels.py`

 * *Files identical despite different names*

### Comparing `dismake-0.0.8/dismake/models/components.py` & `dismake-0.0.9/dismake/models/components.py`

 * *Files identical despite different names*

### Comparing `dismake-0.0.8/dismake/models/embed.py` & `dismake-0.0.9/dismake/models/embed.py`

 * *Files identical despite different names*

### Comparing `dismake-0.0.8/dismake/models/emoji.py` & `dismake-0.0.9/dismake/models/emoji.py`

 * *Files identical despite different names*

### Comparing `dismake-0.0.8/dismake/models/guild.py` & `dismake-0.0.9/dismake/models/guild.py`

 * *Files identical despite different names*

### Comparing `dismake-0.0.8/dismake/models/interaction.py` & `dismake-0.0.9/dismake/models/interaction.py`

 * *Files identical despite different names*

### Comparing `dismake-0.0.8/dismake/models/message.py` & `dismake-0.0.9/dismake/models/message.py`

 * *Files identical despite different names*

### Comparing `dismake-0.0.8/dismake/models/role.py` & `dismake-0.0.9/dismake/models/role.py`

 * *Files identical despite different names*

### Comparing `dismake-0.0.8/dismake/models/user.py` & `dismake-0.0.9/dismake/models/user.py`

 * *Files identical despite different names*

### Comparing `dismake-0.0.8/dismake/params.py` & `dismake-0.0.9/dismake/params.py`

 * *Files identical despite different names*

### Comparing `dismake-0.0.8/dismake/permissions.py` & `dismake-0.0.9/dismake/permissions.py`

 * *Files identical despite different names*

### Comparing `dismake-0.0.8/dismake/plugin.py` & `dismake-0.0.9/dismake/plugin.py`

 * *Files identical despite different names*

### Comparing `dismake-0.0.8/dismake/ui/button.py` & `dismake-0.0.9/dismake/ui/button.py`

 * *Files identical despite different names*

### Comparing `dismake-0.0.8/dismake/ui/component.py` & `dismake-0.0.9/dismake/ui/component.py`

 * *Files identical despite different names*

### Comparing `dismake-0.0.8/dismake/ui/modal.py` & `dismake-0.0.9/dismake/ui/modal.py`

 * *Files identical despite different names*

### Comparing `dismake-0.0.8/dismake/ui/select.py` & `dismake-0.0.9/dismake/ui/select.py`

 * *Files identical despite different names*

### Comparing `dismake-0.0.8/dismake/ui/view.py` & `dismake-0.0.9/dismake/ui/view.py`

 * *Files identical despite different names*

### Comparing `dismake-0.0.8/dismake/utils.py` & `dismake-0.0.9/dismake/utils.py`

 * *Files identical despite different names*

### Comparing `dismake-0.0.8/dismake.egg-info/PKG-INFO` & `dismake-0.0.9/dismake.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dismake
-Version: 0.0.8
+Version: 0.0.9
 Summary: None
 Home-page: https://github.com/Apptic-Development/dismake
 Author: Pranoy Majumdar
 Author-email: officialpranoy2@gmail.com
 License: MIT
 Project-URL: Homepage, https://github.com/Apptic-Development/dismake
 Description: # Introduction to Dismake
```

### Comparing `dismake-0.0.8/dismake.egg-info/SOURCES.txt` & `dismake-0.0.9/dismake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dismake-0.0.8/setup.py` & `dismake-0.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as file:
     long_description = file.read()
 
-with open("requirements/requirements.txt", "r") as file:
-    requirements = list(
-        filter(lambda x: not x.startswith("#") and not x == "", file.read().split("\n"))
-    )
 
 setup(
     name="dismake",
-    version="0.0.8",
+    version="0.0.9",
     author="Pranoy Majumdar",
     author_email="officialpranoy2@gmail.com",
     description="None",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Apptic-Development/dismake",
     project_urls={"Homepage": "https://github.com/Apptic-Development/dismake"},
@@ -22,14 +18,22 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(),
     python_requires=">=3.9",
     license="MIT",
-    install_requires=requirements,
     entry_points={"console_scripts": ["dismake=dismake.cli:main"]},
     package_data={"templates": ["templates/*"]},
+    install_requires=[
+        "fastapi==0.95.1",
+        "httpx==0.24.0",
+        "pydantic==1.10.7",
+        "PyNaCl==1.5.0",
+        "rich==13.3.5",
+        "typing_extensions==4.5.0",
+        "uvicorn==0.22.0",
+    ],
 )
 
 
 print("Successfully installed dismake")
```

### Comparing `dismake-0.0.8/test/tests.py` & `dismake-0.0.9/test/tests.py`

 * *Files identical despite different names*

