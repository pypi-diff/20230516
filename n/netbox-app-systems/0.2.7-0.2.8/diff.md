# Comparing `tmp/netbox-app-systems-0.2.7.tar.gz` & `tmp/netbox-app-systems-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-app-systems-0.2.7.tar", last modified: Thu Sep 29 11:20:34 2022, max compression
+gzip compressed data, was "netbox-app-systems-0.2.8.tar", last modified: Fri Mar 17 08:35:59 2023, max compression
```

## Comparing `netbox-app-systems-0.2.7.tar` & `netbox-app-systems-0.2.8.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-09-29 11:20:34.033236 netbox-app-systems-0.2.7/
--rw-rw-r--   0 user      (1000) user      (1000)     1071 2022-05-25 13:32:13.000000 netbox-app-systems-0.2.7/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)       43 2022-06-03 08:22:08.000000 netbox-app-systems-0.2.7/MANIFEST.in
--rw-rw-r--   0 user      (1000) user      (1000)     1574 2022-09-29 11:20:34.033236 netbox-app-systems-0.2.7/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      970 2022-05-26 07:37:31.000000 netbox-app-systems-0.2.7/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-09-29 11:20:34.025236 netbox-app-systems-0.2.7/netbox_app_systems/
--rw-rw-r--   0 user      (1000) user      (1000)      407 2022-09-26 10:15:53.000000 netbox-app-systems-0.2.7/netbox_app_systems/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-09-29 11:20:34.029236 netbox-app-systems-0.2.7/netbox_app_systems/api/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2022-05-25 14:08:19.000000 netbox-app-systems-0.2.7/netbox_app_systems/api/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2395 2022-09-22 13:29:14.000000 netbox-app-systems-0.2.7/netbox_app_systems/api/serializers.py
--rw-rw-r--   0 user      (1000) user      (1000)      280 2022-07-18 15:22:07.000000 netbox-app-systems-0.2.7/netbox_app_systems/api/urls.py
--rw-rw-r--   0 user      (1000) user      (1000)      636 2022-07-17 22:18:47.000000 netbox-app-systems-0.2.7/netbox_app_systems/api/views.py
--rw-rw-r--   0 user      (1000) user      (1000)     1028 2022-05-25 20:38:29.000000 netbox-app-systems-0.2.7/netbox_app_systems/filtersets.py
--rw-rw-r--   0 user      (1000) user      (1000)      673 2022-05-25 19:54:20.000000 netbox-app-systems-0.2.7/netbox_app_systems/forms.py
--rw-rw-r--   0 user      (1000) user      (1000)      802 2022-05-26 11:21:51.000000 netbox-app-systems-0.2.7/netbox_app_systems/graphql.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-09-29 11:20:34.029236 netbox-app-systems-0.2.7/netbox_app_systems/migrations/
--rw-rw-r--   0 user      (1000) user      (1000)     2285 2022-05-26 08:16:00.000000 netbox-app-systems-0.2.7/netbox_app_systems/migrations/0001_initial.py
--rw-rw-r--   0 user      (1000) user      (1000)        0 2022-05-26 08:16:00.000000 netbox-app-systems-0.2.7/netbox_app_systems/migrations/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2218 2022-09-29 10:04:43.000000 netbox-app-systems-0.2.7/netbox_app_systems/models.py
--rw-rw-r--   0 user      (1000) user      (1000)      492 2022-07-17 22:18:47.000000 netbox-app-systems-0.2.7/netbox_app_systems/navigation.py
--rw-rw-r--   0 user      (1000) user      (1000)      951 2022-05-25 16:39:19.000000 netbox-app-systems-0.2.7/netbox_app_systems/tables.py
--rw-rw-r--   0 user      (1000) user      (1000)     1697 2022-09-26 10:21:30.000000 netbox-app-systems-0.2.7/netbox_app_systems/template_content.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-09-29 11:20:34.021236 netbox-app-systems-0.2.7/netbox_app_systems/templates/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-09-29 11:20:34.033236 netbox-app-systems-0.2.7/netbox_app_systems/templates/netbox_app_systems/
--rw-rw-r--   0 user      (1000) user      (1000)      571 2022-07-04 17:19:57.000000 netbox-app-systems-0.2.7/netbox_app_systems/templates/netbox_app_systems/app_system_assignment_edit.html
--rw-rw-r--   0 user      (1000) user      (1000)     1416 2022-05-25 18:41:06.000000 netbox-app-systems-0.2.7/netbox_app_systems/templates/netbox_app_systems/app_system_panel.html
--rw-rw-r--   0 user      (1000) user      (1000)     1256 2022-07-04 17:20:03.000000 netbox-app-systems-0.2.7/netbox_app_systems/templates/netbox_app_systems/appsystem.html
--rw-rw-r--   0 user      (1000) user      (1000)     1265 2022-05-25 18:39:20.000000 netbox-app-systems-0.2.7/netbox_app_systems/urls.py
--rw-rw-r--   0 user      (1000) user      (1000)     2711 2022-09-26 08:29:49.000000 netbox-app-systems-0.2.7/netbox_app_systems/views.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-09-29 11:20:34.029236 netbox-app-systems-0.2.7/netbox_app_systems.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     1574 2022-09-29 11:20:34.000000 netbox-app-systems-0.2.7/netbox_app_systems.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      991 2022-09-29 11:20:34.000000 netbox-app-systems-0.2.7/netbox_app_systems.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2022-09-29 11:20:34.000000 netbox-app-systems-0.2.7/netbox_app_systems.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2022-05-25 14:30:38.000000 netbox-app-systems-0.2.7/netbox_app_systems.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)       19 2022-09-29 11:20:34.000000 netbox-app-systems-0.2.7/netbox_app_systems.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2022-09-29 11:20:34.033236 netbox-app-systems-0.2.7/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)      953 2022-09-29 10:05:16.000000 netbox-app-systems-0.2.7/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-03-17 08:35:59.592091 netbox-app-systems-0.2.8/
+-rw-rw-r--   0 user      (1000) user      (1000)     1071 2022-05-25 13:32:13.000000 netbox-app-systems-0.2.8/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)       43 2022-06-03 08:22:08.000000 netbox-app-systems-0.2.8/MANIFEST.in
+-rw-rw-r--   0 user      (1000) user      (1000)     1574 2023-03-17 08:35:59.592091 netbox-app-systems-0.2.8/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      970 2022-05-26 07:37:31.000000 netbox-app-systems-0.2.8/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-03-17 08:35:59.588091 netbox-app-systems-0.2.8/netbox_app_systems/
+-rw-rw-r--   0 user      (1000) user      (1000)      407 2022-09-26 10:15:53.000000 netbox-app-systems-0.2.8/netbox_app_systems/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-03-17 08:35:59.592091 netbox-app-systems-0.2.8/netbox_app_systems/api/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2022-05-25 14:08:19.000000 netbox-app-systems-0.2.8/netbox_app_systems/api/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2431 2023-03-17 08:26:02.000000 netbox-app-systems-0.2.8/netbox_app_systems/api/serializers.py
+-rw-rw-r--   0 user      (1000) user      (1000)      280 2022-07-18 15:22:07.000000 netbox-app-systems-0.2.8/netbox_app_systems/api/urls.py
+-rw-rw-r--   0 user      (1000) user      (1000)      636 2022-07-17 22:18:47.000000 netbox-app-systems-0.2.8/netbox_app_systems/api/views.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1028 2022-05-25 20:38:29.000000 netbox-app-systems-0.2.8/netbox_app_systems/filtersets.py
+-rw-rw-r--   0 user      (1000) user      (1000)      673 2023-03-17 08:05:45.000000 netbox-app-systems-0.2.8/netbox_app_systems/forms.py
+-rw-rw-r--   0 user      (1000) user      (1000)      802 2022-05-26 11:21:51.000000 netbox-app-systems-0.2.8/netbox_app_systems/graphql.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-03-17 08:35:59.592091 netbox-app-systems-0.2.8/netbox_app_systems/migrations/
+-rw-rw-r--   0 user      (1000) user      (1000)     2285 2022-05-26 08:16:00.000000 netbox-app-systems-0.2.8/netbox_app_systems/migrations/0001_initial.py
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2022-05-26 08:16:00.000000 netbox-app-systems-0.2.8/netbox_app_systems/migrations/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2218 2023-03-17 08:05:45.000000 netbox-app-systems-0.2.8/netbox_app_systems/models.py
+-rw-rw-r--   0 user      (1000) user      (1000)      492 2022-07-17 22:18:47.000000 netbox-app-systems-0.2.8/netbox_app_systems/navigation.py
+-rw-rw-r--   0 user      (1000) user      (1000)      951 2023-03-17 08:05:45.000000 netbox-app-systems-0.2.8/netbox_app_systems/tables.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1697 2022-09-26 10:21:30.000000 netbox-app-systems-0.2.8/netbox_app_systems/template_content.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-03-17 08:35:59.584092 netbox-app-systems-0.2.8/netbox_app_systems/templates/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-03-17 08:35:59.592091 netbox-app-systems-0.2.8/netbox_app_systems/templates/netbox_app_systems/
+-rw-rw-r--   0 user      (1000) user      (1000)      571 2022-07-04 17:19:57.000000 netbox-app-systems-0.2.8/netbox_app_systems/templates/netbox_app_systems/app_system_assignment_edit.html
+-rw-rw-r--   0 user      (1000) user      (1000)     1416 2022-05-25 18:41:06.000000 netbox-app-systems-0.2.8/netbox_app_systems/templates/netbox_app_systems/app_system_panel.html
+-rw-rw-r--   0 user      (1000) user      (1000)     1256 2023-03-17 08:05:45.000000 netbox-app-systems-0.2.8/netbox_app_systems/templates/netbox_app_systems/appsystem.html
+-rw-rw-r--   0 user      (1000) user      (1000)     1265 2022-05-25 18:39:20.000000 netbox-app-systems-0.2.8/netbox_app_systems/urls.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2711 2022-09-26 08:29:49.000000 netbox-app-systems-0.2.8/netbox_app_systems/views.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-03-17 08:35:59.592091 netbox-app-systems-0.2.8/netbox_app_systems.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)     1574 2023-03-17 08:35:59.000000 netbox-app-systems-0.2.8/netbox_app_systems.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      991 2023-03-17 08:35:59.000000 netbox-app-systems-0.2.8/netbox_app_systems.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-03-17 08:35:59.000000 netbox-app-systems-0.2.8/netbox_app_systems.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2022-05-25 14:30:38.000000 netbox-app-systems-0.2.8/netbox_app_systems.egg-info/not-zip-safe
+-rw-rw-r--   0 user      (1000) user      (1000)       19 2023-03-17 08:35:59.000000 netbox-app-systems-0.2.8/netbox_app_systems.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-03-17 08:35:59.592091 netbox-app-systems-0.2.8/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)      953 2023-03-17 08:12:08.000000 netbox-app-systems-0.2.8/setup.py
```

### Comparing `netbox-app-systems-0.2.7/LICENSE` & `netbox-app-systems-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-app-systems-0.2.7/PKG-INFO` & `netbox-app-systems-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-app-systems
-Version: 0.2.7
+Version: 0.2.8
 Summary: Netbox plugin. Assign devices and virtual machines to application systems
 Download-URL: https://pypi.org/project/netbox-app-systems/
 Author: Oleg Senchenko
 Author-email: senchenkoob@mail.ru
 Maintainer: Oleg Senchenko
 Maintainer-email: senchenkoob@mail.ru
 License: MIT
```

### Comparing `netbox-app-systems-0.2.7/README.md` & `netbox-app-systems-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `netbox-app-systems-0.2.7/netbox_app_systems/api/serializers.py` & `netbox-app-systems-0.2.8/netbox_app_systems/api/serializers.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,16 @@
 class NestedAppSystemAssignmentSerializer(WritableNestedSerializer):
     url = serializers.HyperlinkedIdentityField(
         view_name='plugins-api:netbox_app_systems-api:appsystemassignment-detail')
     app_system = NestedAppSystemSerializer()
 
     class Meta:
         model = AppSystemAssignment
-        fields = ['id', 'url', 'display', 'AppSystem', 'relation']
+        fields = ['id', 'url', 'display', 'app_system',
+                  'content_type', 'object_id']
 
 
 class AppSystemAssignmentSerializer(NetBoxModelSerializer):
     url = serializers.HyperlinkedIdentityField(
         view_name='plugins-api:netbox_app_systems-api:appsystemassignment-detail')
     content_type = ContentTypeField(
         queryset=ContentType.objects.all()
```

### Comparing `netbox-app-systems-0.2.7/netbox_app_systems/api/views.py` & `netbox-app-systems-0.2.8/netbox_app_systems/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox-app-systems-0.2.7/netbox_app_systems/filtersets.py` & `netbox-app-systems-0.2.8/netbox_app_systems/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox-app-systems-0.2.7/netbox_app_systems/forms.py` & `netbox-app-systems-0.2.8/netbox_app_systems/forms.py`

 * *Files identical despite different names*

### Comparing `netbox-app-systems-0.2.7/netbox_app_systems/graphql.py` & `netbox-app-systems-0.2.8/netbox_app_systems/graphql.py`

 * *Files identical despite different names*

### Comparing `netbox-app-systems-0.2.7/netbox_app_systems/migrations/0001_initial.py` & `netbox-app-systems-0.2.8/netbox_app_systems/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox-app-systems-0.2.7/netbox_app_systems/models.py` & `netbox-app-systems-0.2.8/netbox_app_systems/models.py`

 * *Files identical despite different names*

### Comparing `netbox-app-systems-0.2.7/netbox_app_systems/tables.py` & `netbox-app-systems-0.2.8/netbox_app_systems/tables.py`

 * *Files identical despite different names*

### Comparing `netbox-app-systems-0.2.7/netbox_app_systems/template_content.py` & `netbox-app-systems-0.2.8/netbox_app_systems/template_content.py`

 * *Files identical despite different names*

### Comparing `netbox-app-systems-0.2.7/netbox_app_systems/templates/netbox_app_systems/app_system_assignment_edit.html` & `netbox-app-systems-0.2.8/netbox_app_systems/templates/netbox_app_systems/app_system_assignment_edit.html`

 * *Files identical despite different names*

### Comparing `netbox-app-systems-0.2.7/netbox_app_systems/templates/netbox_app_systems/app_system_panel.html` & `netbox-app-systems-0.2.8/netbox_app_systems/templates/netbox_app_systems/app_system_panel.html`

 * *Files identical despite different names*

### Comparing `netbox-app-systems-0.2.7/netbox_app_systems/templates/netbox_app_systems/appsystem.html` & `netbox-app-systems-0.2.8/netbox_app_systems/templates/netbox_app_systems/appsystem.html`

 * *Files identical despite different names*

### Comparing `netbox-app-systems-0.2.7/netbox_app_systems/urls.py` & `netbox-app-systems-0.2.8/netbox_app_systems/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-app-systems-0.2.7/netbox_app_systems/views.py` & `netbox-app-systems-0.2.8/netbox_app_systems/views.py`

 * *Files identical despite different names*

### Comparing `netbox-app-systems-0.2.7/netbox_app_systems.egg-info/PKG-INFO` & `netbox-app-systems-0.2.8/netbox_app_systems.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-app-systems
-Version: 0.2.7
+Version: 0.2.8
 Summary: Netbox plugin. Assign devices and virtual machines to application systems
 Download-URL: https://pypi.org/project/netbox-app-systems/
 Author: Oleg Senchenko
 Author-email: senchenkoob@mail.ru
 Maintainer: Oleg Senchenko
 Maintainer-email: senchenkoob@mail.ru
 License: MIT
```

### Comparing `netbox-app-systems-0.2.7/netbox_app_systems.egg-info/SOURCES.txt` & `netbox-app-systems-0.2.8/netbox_app_systems.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netbox-app-systems-0.2.7/setup.py` & `netbox-app-systems-0.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='netbox-app-systems',
-    version='0.2.7',
+    version='0.2.8',
     description='Netbox plugin. Assign devices and virtual machines to application systems',
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[],
     download_url='https://pypi.org/project/netbox-app-systems/',
     packages=find_packages(),
     include_package_data=True,
```

