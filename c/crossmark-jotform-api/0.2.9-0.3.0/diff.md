# Comparing `tmp/crossmark-jotform-api-0.2.9.tar.gz` & `tmp/crossmark-jotform-api-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crossmark-jotform-api-0.2.9.tar", last modified: Wed May 10 23:11:44 2023, max compression
+gzip compressed data, was "crossmark-jotform-api-0.3.0.tar", last modified: Tue May 16 17:58:31 2023, max compression
```

## Comparing `crossmark-jotform-api-0.2.9.tar` & `crossmark-jotform-api-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 23:11:44.297837 crossmark-jotform-api-0.2.9/
--rw-rw-rw-   0        0        0     1091 2023-02-01 01:57:52.000000 crossmark-jotform-api-0.2.9/LICENSE
--rw-rw-rw-   0        0        0     2526 2023-05-10 23:11:44.296840 crossmark-jotform-api-0.2.9/PKG-INFO
--rw-rw-rw-   0        0        0      626 2023-05-10 23:11:03.000000 crossmark-jotform-api-0.2.9/README.md
--rw-rw-rw-   0        0        0      789 2023-05-10 23:10:24.000000 crossmark-jotform-api-0.2.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-10 23:11:44.298834 crossmark-jotform-api-0.2.9/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-10 23:11:44.267796 crossmark-jotform-api-0.2.9/src/
-drwxrwxrwx   0        0        0        0 2023-05-10 23:11:44.279797 crossmark-jotform-api-0.2.9/src/crossmark_jotform_api/
--rw-rw-rw-   0        0        0    12789 2023-05-10 23:10:11.000000 crossmark-jotform-api-0.2.9/src/crossmark_jotform_api/jotForm.py
-drwxrwxrwx   0        0        0        0 2023-05-10 23:11:44.291798 crossmark-jotform-api-0.2.9/src/crossmark_jotform_api.egg-info/
--rw-rw-rw-   0        0        0     2526 2023-05-10 23:11:44.000000 crossmark-jotform-api-0.2.9/src/crossmark_jotform_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-05-10 23:11:44.000000 crossmark-jotform-api-0.2.9/src/crossmark_jotform_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 23:11:44.000000 crossmark-jotform-api-0.2.9/src/crossmark_jotform_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-05-10 23:11:44.000000 crossmark-jotform-api-0.2.9/src/crossmark_jotform_api.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-10 23:11:44.294850 crossmark-jotform-api-0.2.9/test/
--rw-rw-rw-   0        0        0      270 2023-05-10 23:06:10.000000 crossmark-jotform-api-0.2.9/test/test_jotform_class.py
+drwxrwxrwx   0        0        0        0 2023-05-16 17:58:31.350073 crossmark-jotform-api-0.3.0/
+-rw-rw-rw-   0        0        0     1091 2023-02-01 01:57:52.000000 crossmark-jotform-api-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0     2630 2023-05-16 17:58:31.349076 crossmark-jotform-api-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      730 2023-05-16 17:57:54.000000 crossmark-jotform-api-0.3.0/README.md
+-rw-rw-rw-   0        0        0      789 2023-05-16 17:57:19.000000 crossmark-jotform-api-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-16 17:58:31.350073 crossmark-jotform-api-0.3.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-16 17:58:31.310074 crossmark-jotform-api-0.3.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-16 17:58:31.323075 crossmark-jotform-api-0.3.0/src/crossmark_jotform_api/
+-rw-rw-rw-   0        0        0    12830 2023-05-16 17:56:23.000000 crossmark-jotform-api-0.3.0/src/crossmark_jotform_api/jotForm.py
+drwxrwxrwx   0        0        0        0 2023-05-16 17:58:31.342080 crossmark-jotform-api-0.3.0/src/crossmark_jotform_api.egg-info/
+-rw-rw-rw-   0        0        0     2630 2023-05-16 17:58:31.000000 crossmark-jotform-api-0.3.0/src/crossmark_jotform_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-05-16 17:58:31.000000 crossmark-jotform-api-0.3.0/src/crossmark_jotform_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 17:58:31.000000 crossmark-jotform-api-0.3.0/src/crossmark_jotform_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-05-16 17:58:31.000000 crossmark-jotform-api-0.3.0/src/crossmark_jotform_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 17:58:31.348073 crossmark-jotform-api-0.3.0/test/
+-rw-rw-rw-   0        0        0      270 2023-05-10 23:06:10.000000 crossmark-jotform-api-0.3.0/test/test_jotform_class.py
```

### Comparing `crossmark-jotform-api-0.2.9/LICENSE` & `crossmark-jotform-api-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `crossmark-jotform-api-0.2.9/PKG-INFO` & `crossmark-jotform-api-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crossmark-jotform-api
-Version: 0.2.9
+Version: 0.3.0
 Summary: Jotform api integration dedicated for server usage which limits calls and calling form only if there is a new submission
 Author-email: Renas Mirkan Kilic <mirkanbaba1@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -40,7 +40,8 @@
 specilized library for jotform api and crossmark needs
 
 ## updates
 - 2023-04-26: added `set_new_submission` function, time to time it cannot find the submission, in that cases pulls the data directly from the api and sets as it is.
 - 2023-05-01: added a logic for get_emails function. and added a TODO there.
 - 2023-05-01: setted set_answer function.
 - 2023-05-10: deleted submissions array and enhanced the logic according to it
+- 2023-05-16: created emails on class initilaization so that one dont need to call get_emails function
```

### Comparing `crossmark-jotform-api-0.2.9/README.md` & `crossmark-jotform-api-0.3.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -6,8 +6,9 @@
 ## description
 specilized library for jotform api and crossmark needs
 
 ## updates
 - 2023-04-26: added `set_new_submission` function, time to time it cannot find the submission, in that cases pulls the data directly from the api and sets as it is.
 - 2023-05-01: added a logic for get_emails function. and added a TODO there.
 - 2023-05-01: setted set_answer function.
-- 2023-05-10: deleted submissions array and enhanced the logic according to it
+- 2023-05-10: deleted submissions array and enhanced the logic according to it
+- 2023-05-16: created emails on class initilaization so that one dont need to call get_emails function
```

### Comparing `crossmark-jotform-api-0.2.9/pyproject.toml` & `crossmark-jotform-api-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0","requests>=2.22.0","wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "crossmark-jotform-api"
-version = "0.2.9"
+version = "0.3.0"
 authors = [
   { name="Renas Mirkan Kilic", email="mirkanbaba1@gmail.com" },
 ]
 description = "Jotform api integration dedicated for server usage which limits calls and calling form only if there is a new submission"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.6"
```

### Comparing `crossmark-jotform-api-0.2.9/src/crossmark_jotform_api/jotForm.py` & `crossmark-jotform-api-0.3.0/src/crossmark_jotform_api/jotForm.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,14 +225,15 @@
         self.answers_arr = self.set_answers(self.answers)
         self.case_id = self.get_answer_by_text('CASE')['answer']
         self.editor = self.get_answer_by_text('EDITOR')['answer']
         self.status = self.get_answer_by_text('STATUS')['answer']
         self.store = self.get_answer_by_text('STORE')['answer']
         self.GUID = self.get_answer_by_text('GUID')['answer']
         self.client = self.get_answer_by_text('CLIENT')['answer']
+        self.emails = self.get_emails()
 
     def set_answers(self, answers):
         answers_arr = []
         for key, value in answers.items():
             if 'name' in value:
                 name = value['name']
             else:
```

### Comparing `crossmark-jotform-api-0.2.9/src/crossmark_jotform_api.egg-info/PKG-INFO` & `crossmark-jotform-api-0.3.0/src/crossmark_jotform_api.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crossmark-jotform-api
-Version: 0.2.9
+Version: 0.3.0
 Summary: Jotform api integration dedicated for server usage which limits calls and calling form only if there is a new submission
 Author-email: Renas Mirkan Kilic <mirkanbaba1@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -40,7 +40,8 @@
 specilized library for jotform api and crossmark needs
 
 ## updates
 - 2023-04-26: added `set_new_submission` function, time to time it cannot find the submission, in that cases pulls the data directly from the api and sets as it is.
 - 2023-05-01: added a logic for get_emails function. and added a TODO there.
 - 2023-05-01: setted set_answer function.
 - 2023-05-10: deleted submissions array and enhanced the logic according to it
+- 2023-05-16: created emails on class initilaization so that one dont need to call get_emails function
```

