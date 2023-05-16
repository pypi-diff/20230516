# Comparing `tmp/lamineml-0.0.54.tar.gz` & `tmp/lamineml-0.0.55.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamineml-0.0.54.tar", last modified: Sat May 13 13:37:00 2023, max compression
+gzip compressed data, was "lamineml-0.0.55.tar", last modified: Tue May 16 19:21:26 2023, max compression
```

## Comparing `lamineml-0.0.54.tar` & `lamineml-0.0.55.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-13 13:37:00.195161 lamineml-0.0.54/
--rw-rw-r--   0 hello     (1000) hello     (1000)        0 2021-07-31 02:25:56.000000 lamineml-0.0.54/LICENSE
--rw-rw-r--   0 hello     (1000) hello     (1000)     2806 2023-05-13 13:37:00.195161 lamineml-0.0.54/PKG-INFO
--rw-rw-r--   0 hello     (1000) hello     (1000)     2304 2021-07-31 02:25:56.000000 lamineml-0.0.54/README.md
--rw-rw-r--   0 hello     (1000) hello     (1000)      126 2023-04-29 18:32:31.000000 lamineml-0.0.54/pyproject.toml
--rw-rw-r--   0 hello     (1000) hello     (1000)      626 2023-05-13 13:37:00.195161 lamineml-0.0.54/setup.cfg
-drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-13 13:37:00.191161 lamineml-0.0.54/src/
-drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-13 13:37:00.195161 lamineml-0.0.54/src/lamine/
--rw-rw-r--   0 hello     (1000) hello     (1000)        0 2023-04-29 17:24:39.000000 lamineml-0.0.54/src/lamine/__init__.py
--rw-rw-r--   0 hello     (1000) hello     (1000)     2942 2023-05-13 13:35:50.000000 lamineml-0.0.54/src/lamine/tools.py
-drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-13 13:37:00.195161 lamineml-0.0.54/src/lamineml.egg-info/
--rw-rw-r--   0 hello     (1000) hello     (1000)     2806 2023-05-13 13:37:00.000000 lamineml-0.0.54/src/lamineml.egg-info/PKG-INFO
--rw-rw-r--   0 hello     (1000) hello     (1000)      229 2023-05-13 13:37:00.000000 lamineml-0.0.54/src/lamineml.egg-info/SOURCES.txt
--rw-rw-r--   0 hello     (1000) hello     (1000)        1 2023-05-13 13:37:00.000000 lamineml-0.0.54/src/lamineml.egg-info/dependency_links.txt
--rw-rw-r--   0 hello     (1000) hello     (1000)        7 2023-05-13 13:37:00.000000 lamineml-0.0.54/src/lamineml.egg-info/top_level.txt
+drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-16 19:21:26.181210 lamineml-0.0.55/
+-rw-rw-r--   0 hello     (1000) hello     (1000)        0 2021-07-31 02:25:56.000000 lamineml-0.0.55/LICENSE
+-rw-rw-r--   0 hello     (1000) hello     (1000)     2806 2023-05-16 19:21:26.181210 lamineml-0.0.55/PKG-INFO
+-rw-rw-r--   0 hello     (1000) hello     (1000)     2304 2021-07-31 02:25:56.000000 lamineml-0.0.55/README.md
+-rw-rw-r--   0 hello     (1000) hello     (1000)      126 2023-04-29 18:32:31.000000 lamineml-0.0.55/pyproject.toml
+-rw-rw-r--   0 hello     (1000) hello     (1000)      626 2023-05-16 19:21:26.181210 lamineml-0.0.55/setup.cfg
+drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-16 19:21:26.181210 lamineml-0.0.55/src/
+drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-16 19:21:26.181210 lamineml-0.0.55/src/lamine/
+-rw-rw-r--   0 hello     (1000) hello     (1000)        0 2023-04-29 17:24:39.000000 lamineml-0.0.55/src/lamine/__init__.py
+-rw-rw-r--   0 hello     (1000) hello     (1000)     3275 2023-05-16 19:19:50.000000 lamineml-0.0.55/src/lamine/tools.py
+drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-16 19:21:26.181210 lamineml-0.0.55/src/lamineml.egg-info/
+-rw-rw-r--   0 hello     (1000) hello     (1000)     2806 2023-05-16 19:21:26.000000 lamineml-0.0.55/src/lamineml.egg-info/PKG-INFO
+-rw-rw-r--   0 hello     (1000) hello     (1000)      229 2023-05-16 19:21:26.000000 lamineml-0.0.55/src/lamineml.egg-info/SOURCES.txt
+-rw-rw-r--   0 hello     (1000) hello     (1000)        1 2023-05-16 19:21:26.000000 lamineml-0.0.55/src/lamineml.egg-info/dependency_links.txt
+-rw-rw-r--   0 hello     (1000) hello     (1000)        7 2023-05-16 19:21:26.000000 lamineml-0.0.55/src/lamineml.egg-info/top_level.txt
```

### Comparing `lamineml-0.0.54/PKG-INFO` & `lamineml-0.0.55/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamineml
-Version: 0.0.54
+Version: 0.0.55
 Summary: use this library in kivy android
 Home-page: https://github.com/pypa/sampleproject
 Author: Lamine ML
 Author-email: lamineml128@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lamineml-0.0.54/README.md` & `lamineml-0.0.55/README.md`

 * *Files identical despite different names*

### Comparing `lamineml-0.0.54/setup.cfg` & `lamineml-0.0.55/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lamineml
-version = 0.0.54
+version = 0.0.55
 author = Lamine ML
 author_email = lamineml128@gmail.com
 description = use this library in kivy android
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pypa/sampleproject
 project_urls =
```

### Comparing `lamineml-0.0.54/src/lamine/tools.py` & `lamineml-0.0.55/src/lamine/tools.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,23 @@
 context=autoclass("android.content.Context")
 Context = autoclass('android.content.Context')
 window=autoclass ('android.view.WindowManager$LayoutParams')
 getL=autoclass("java.util.Locale")
 Intent = autoclass('android.content.Intent')
 uri = autoclass('android.net.Uri')
 ClipData =autoclass("android.content.ClipData")
+##################################################"
+g =autoclass("android.view.Gravity")
+t= autoclass("android.widget.Toast")
+window=autoclass ("android.view.WindowManager$LayoutParams")
+@run_on_ui_thread
+from android.runnable import run_on_ui_thread
+
+def KEEP_SCREEN_ON():
+    activity.getWindow(). addFlags (window.FLAG_KEEP_SCREEN_ON)
 def open_browser(url):
     intent = Intent()
     intent.setAction(Intent.ACTION_VIEW)
     intent.setData(uri.parse(url))
     activity.startActivity(intent)
 
 def copy_text(text):
@@ -30,19 +39,14 @@
     a = activity.getPackageManager().queryIntentActivities(sendIntent, 0)
     for i in a:
 
         if i.activityInfo.labelRes != 0:
             res = activity.getPackageManager().getResourcesForApplication(i.activityInfo.applicationInfo)
             dd = res.getString(i.activityInfo.labelRes)
             al.append(dd)
-
-
-
-
-
         else:
             i.activityInfo.applicationInfo.loadLabel(activity.getPackageManager())
     return al
 
 def get_permissions(package_name):
     f=""
     a = activity.getPackageManager().getPackageInfo(package_name, packagemanager.GET_PERMISSIONS)
```

### Comparing `lamineml-0.0.54/src/lamineml.egg-info/PKG-INFO` & `lamineml-0.0.55/src/lamineml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamineml
-Version: 0.0.54
+Version: 0.0.55
 Summary: use this library in kivy android
 Home-page: https://github.com/pypa/sampleproject
 Author: Lamine ML
 Author-email: lamineml128@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

