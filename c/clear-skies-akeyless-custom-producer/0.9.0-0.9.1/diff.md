# Comparing `tmp/clear-skies-akeyless-custom-producer-0.9.0.tar.gz` & `tmp/clear-skies-akeyless-custom-producer-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clear-skies-akeyless-custom-producer-0.9.0.tar", last modified: Fri May 12 15:21:25 2023, max compression
+gzip compressed data, was "clear-skies-akeyless-custom-producer-0.9.1.tar", last modified: Mon May 15 23:28:57 2023, max compression
```

## Comparing `clear-skies-akeyless-custom-producer-0.9.0.tar` & `clear-skies-akeyless-custom-producer-0.9.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-12 15:21:25.350508 clear-skies-akeyless-custom-producer-0.9.0/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1053 2023-05-10 15:19:24.000000 clear-skies-akeyless-custom-producer-0.9.0/LICENSE
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       25 2023-05-10 10:53:24.000000 clear-skies-akeyless-custom-producer-0.9.0/MANIFEST.in
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     6920 2023-05-12 15:21:25.350508 clear-skies-akeyless-custom-producer-0.9.0/PKG-INFO
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     6259 2023-05-12 15:20:11.000000 clear-skies-akeyless-custom-producer-0.9.0/README.md
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       79 2023-05-12 15:21:25.350508 clear-skies-akeyless-custom-producer-0.9.0/setup.cfg
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1415 2023-05-10 10:57:34.000000 clear-skies-akeyless-custom-producer-0.9.0/setup.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-12 15:21:25.346508 clear-skies-akeyless-custom-producer-0.9.0/src/
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-12 15:21:25.350508 clear-skies-akeyless-custom-producer-0.9.0/src/clear_skies_akeyless_custom_producer.egg-info/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     6920 2023-05-12 15:21:25.000000 clear-skies-akeyless-custom-producer-0.9.0/src/clear_skies_akeyless_custom_producer.egg-info/PKG-INFO
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      604 2023-05-12 15:21:25.000000 clear-skies-akeyless-custom-producer-0.9.0/src/clear_skies_akeyless_custom_producer.egg-info/SOURCES.txt
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        1 2023-05-12 15:21:25.000000 clear-skies-akeyless-custom-producer-0.9.0/src/clear_skies_akeyless_custom_producer.egg-info/dependency_links.txt
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       12 2023-05-12 15:21:25.000000 clear-skies-akeyless-custom-producer-0.9.0/src/clear_skies_akeyless_custom_producer.egg-info/requires.txt
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       36 2023-05-12 15:21:25.000000 clear-skies-akeyless-custom-producer-0.9.0/src/clear_skies_akeyless_custom_producer.egg-info/top_level.txt
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-12 15:21:25.350508 clear-skies-akeyless-custom-producer-0.9.0/src/clearskies_akeyless_custom_producer/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       23 2023-05-10 10:54:42.000000 clear-skies-akeyless-custom-producer-0.9.0/src/clearskies_akeyless_custom_producer/__init__.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-12 15:21:25.350508 clear-skies-akeyless-custom-producer-0.9.0/src/clearskies_akeyless_custom_producer/handlers/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       30 2023-05-11 19:55:49.000000 clear-skies-akeyless-custom-producer-0.9.0/src/clearskies_akeyless_custom_producer/handlers/__init__.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)    10465 2023-05-12 15:09:33.000000 clear-skies-akeyless-custom-producer-0.9.0/src/clearskies_akeyless_custom_producer/handlers/no_input.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     5948 2023-05-12 14:49:21.000000 clear-skies-akeyless-custom-producer-0.9.0/src/clearskies_akeyless_custom_producer/handlers/with_input.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-15 23:28:57.184132 clear-skies-akeyless-custom-producer-0.9.1/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1053 2023-05-10 15:19:24.000000 clear-skies-akeyless-custom-producer-0.9.1/LICENSE
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       25 2023-05-10 10:53:24.000000 clear-skies-akeyless-custom-producer-0.9.1/MANIFEST.in
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     6920 2023-05-15 23:28:57.184132 clear-skies-akeyless-custom-producer-0.9.1/PKG-INFO
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     6259 2023-05-12 15:20:11.000000 clear-skies-akeyless-custom-producer-0.9.1/README.md
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       79 2023-05-15 23:28:57.184132 clear-skies-akeyless-custom-producer-0.9.1/setup.cfg
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1415 2023-05-15 23:26:56.000000 clear-skies-akeyless-custom-producer-0.9.1/setup.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-15 23:28:57.180132 clear-skies-akeyless-custom-producer-0.9.1/src/
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-15 23:28:57.184132 clear-skies-akeyless-custom-producer-0.9.1/src/clear_skies_akeyless_custom_producer.egg-info/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     6920 2023-05-15 23:28:57.000000 clear-skies-akeyless-custom-producer-0.9.1/src/clear_skies_akeyless_custom_producer.egg-info/PKG-INFO
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      604 2023-05-15 23:28:57.000000 clear-skies-akeyless-custom-producer-0.9.1/src/clear_skies_akeyless_custom_producer.egg-info/SOURCES.txt
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        1 2023-05-15 23:28:57.000000 clear-skies-akeyless-custom-producer-0.9.1/src/clear_skies_akeyless_custom_producer.egg-info/dependency_links.txt
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       12 2023-05-15 23:28:57.000000 clear-skies-akeyless-custom-producer-0.9.1/src/clear_skies_akeyless_custom_producer.egg-info/requires.txt
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       36 2023-05-15 23:28:57.000000 clear-skies-akeyless-custom-producer-0.9.1/src/clear_skies_akeyless_custom_producer.egg-info/top_level.txt
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-15 23:28:57.184132 clear-skies-akeyless-custom-producer-0.9.1/src/clearskies_akeyless_custom_producer/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       23 2023-05-10 10:54:42.000000 clear-skies-akeyless-custom-producer-0.9.1/src/clearskies_akeyless_custom_producer/__init__.py
+drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-15 23:28:57.184132 clear-skies-akeyless-custom-producer-0.9.1/src/clearskies_akeyless_custom_producer/handlers/
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       30 2023-05-11 19:55:49.000000 clear-skies-akeyless-custom-producer-0.9.1/src/clearskies_akeyless_custom_producer/handlers/__init__.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)    10449 2023-05-15 23:26:29.000000 clear-skies-akeyless-custom-producer-0.9.1/src/clearskies_akeyless_custom_producer/handlers/no_input.py
+-rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     5948 2023-05-12 14:49:21.000000 clear-skies-akeyless-custom-producer-0.9.1/src/clearskies_akeyless_custom_producer/handlers/with_input.py
```

### Comparing `clear-skies-akeyless-custom-producer-0.9.0/LICENSE` & `clear-skies-akeyless-custom-producer-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `clear-skies-akeyless-custom-producer-0.9.0/PKG-INFO` & `clear-skies-akeyless-custom-producer-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clear-skies-akeyless-custom-producer
-Version: 0.9.0
+Version: 0.9.1
 Summary: clearskies handlers for hosting Akeyless custom producer endpoints
 Home-page: https://github.com/cmancone/clearskies-akeyless-custom-producer
 Author: Conor Mancone
 Author-email: cmancone@gmail.com
 License: MIT
 Keywords: setuptools development
 Classifier: Development Status :: 4 - Beta
```

### Comparing `clear-skies-akeyless-custom-producer-0.9.0/README.md` & `clear-skies-akeyless-custom-producer-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `clear-skies-akeyless-custom-producer-0.9.0/setup.py` & `clear-skies-akeyless-custom-producer-0.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='clear-skies-akeyless-custom-producer',
-    version='0.9.0',
+    version='0.9.1',
     description='clearskies handlers for hosting Akeyless custom producer endpoints',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/cmancone/clearskies-akeyless-custom-producer',
     author='Conor Mancone',
     author_email='cmancone@gmail.com',
     license='MIT',
```

### Comparing `clear-skies-akeyless-custom-producer-0.9.0/src/clear_skies_akeyless_custom_producer.egg-info/PKG-INFO` & `clear-skies-akeyless-custom-producer-0.9.1/src/clear_skies_akeyless_custom_producer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clear-skies-akeyless-custom-producer
-Version: 0.9.0
+Version: 0.9.1
 Summary: clearskies handlers for hosting Akeyless custom producer endpoints
 Home-page: https://github.com/cmancone/clearskies-akeyless-custom-producer
 Author: Conor Mancone
 Author-email: cmancone@gmail.com
 License: MIT
 Keywords: setuptools development
 Classifier: Development Status :: 4 - Beta
```

### Comparing `clear-skies-akeyless-custom-producer-0.9.0/src/clear_skies_akeyless_custom_producer.egg-info/SOURCES.txt` & `clear-skies-akeyless-custom-producer-0.9.1/src/clear_skies_akeyless_custom_producer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clear-skies-akeyless-custom-producer-0.9.0/src/clearskies_akeyless_custom_producer/handlers/no_input.py` & `clear-skies-akeyless-custom-producer-0.9.1/src/clearskies_akeyless_custom_producer/handlers/no_input.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,19 +111,19 @@
             raise InputError("Missing 'ids' in JSON POST body")
         return request_json['ids']
 
     def create(self, input_output):
         try:
             payload = self._get_payload(input_output)
         except InputError as e:
-            return self.error(input_output, str(e), 400)
+            return self.error(input_output, e.errors, 400)
 
         errors = self._check_payload(payload)
         if errors:
-            return self.input_errors(input_output, input_errors)
+            return self.input_errors(input_output, errors)
 
         credentials = self._di.call_function(
             self.configuration('create_callable'),
             **payload,
             payload=payload,
             for_rotate=False,
         )
@@ -152,35 +152,35 @@
         This is here because Akeyless always requires a revoke endpoint, but revokation is not always
         possible. So, if revoke is disabled, we still need to respond to the revoke endpoint.
         """
         try:
             payload = self._get_payload(input_output)
             ids = self._get_ids(input_output)
         except InputError as e:
-            return self.error(input_output, str(e), 400)
+            return self.error(input_output, e.errors, 400)
 
         errors = self._check_payload(payload)
         if errors:
-            return self.input_errors(input_output, input_errors)
+            return self.input_errors(input_output, errors)
 
         return input_output.respond({
             'revoked': ids,
             'message': '',
         }, 200)
 
     def revoke(self, input_output):
         try:
             payload = self._get_payload(input_output)
             ids = self._get_ids(input_output)
         except InputError as e:
-            return self.error(input_output, str(e), 400)
+            return self.error(input_output, e.errors, 400)
 
         errors = self._check_payload(payload)
         if errors:
-            return self.input_errors(input_output, input_errors)
+            return self.input_errors(input_output, errors)
 
         for raw_id in ids:
             # Akeyless prepends some stuff to the id to make it unique, which we have to remove.
             # They will stick some parts and separate things with an underscore.  We therefore want
             # to split on an underscore and grab the part at the end.  This can cause trouble if the
             # id itself contains an underscore.  To avoid this, the create function replaces underscores
             # with a string that is very unlikely to exist in the actual id, so we have to reverse that.
@@ -197,19 +197,19 @@
             'message': '',
         }, 200)
 
     def rotate(self, input_output):
         try:
             payload = self._get_payload(input_output)
         except InputError as e:
-            return self.error(input_output, str(e), 400)
+            return self.error(input_output, e.errors, 400)
 
         errors = self._check_payload(payload)
         if errors:
-            return self.input_errors(input_output, input_errors)
+            return self.input_errors(input_output, errors)
 
         # The user may have provided a rotate callable, in which case just use that.
         if self.configuration('rotate_callable'):
             new_payload = self._di.call_function(
                 self.configuration('rotate_callable'),
                 **payload,
                 payload=payload,
```

### Comparing `clear-skies-akeyless-custom-producer-0.9.0/src/clearskies_akeyless_custom_producer/handlers/with_input.py` & `clear-skies-akeyless-custom-producer-0.9.1/src/clearskies_akeyless_custom_producer/handlers/with_input.py`

 * *Files identical despite different names*

