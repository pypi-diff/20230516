# Comparing `tmp/django-utilitas-1.3.5.tar.gz` & `tmp/django-utilitas-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-utilitas-1.3.5.tar", last modified: Sun May 14 07:57:19 2023, max compression
+gzip compressed data, was "django-utilitas-1.3.6.tar", last modified: Tue May 16 13:12:52 2023, max compression
```

## Comparing `django-utilitas-1.3.5.tar` & `django-utilitas-1.3.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 jamesthiha   (501) staff       (20)        0 2023-05-14 07:57:19.183944 django-utilitas-1.3.5/
--rw-r--r--   0 jamesthiha   (501) staff       (20)    35149 2022-12-05 07:45:37.000000 django-utilitas-1.3.5/LICENSE
--rw-r--r--   0 jamesthiha   (501) staff       (20)     4808 2023-05-14 07:57:19.184193 django-utilitas-1.3.5/PKG-INFO
--rw-r--r--   0 jamesthiha   (501) staff       (20)     4563 2023-05-14 07:57:02.000000 django-utilitas-1.3.5/README.md
-drwxr-xr-x   0 jamesthiha   (501) staff       (20)        0 2023-05-14 07:57:19.170422 django-utilitas-1.3.5/django_utilitas.egg-info/
--rw-r--r--   0 jamesthiha   (501) staff       (20)     4808 2023-05-14 07:57:19.000000 django-utilitas-1.3.5/django_utilitas.egg-info/PKG-INFO
--rw-r--r--   0 jamesthiha   (501) staff       (20)      642 2023-05-14 07:57:19.000000 django-utilitas-1.3.5/django_utilitas.egg-info/SOURCES.txt
--rw-r--r--   0 jamesthiha   (501) staff       (20)        1 2023-05-14 07:57:19.000000 django-utilitas-1.3.5/django_utilitas.egg-info/dependency_links.txt
--rw-r--r--   0 jamesthiha   (501) staff       (20)       80 2023-05-14 07:57:19.000000 django-utilitas-1.3.5/django_utilitas.egg-info/requires.txt
--rw-r--r--   0 jamesthiha   (501) staff       (20)        9 2023-05-14 07:57:19.000000 django-utilitas-1.3.5/django_utilitas.egg-info/top_level.txt
--rw-r--r--   0 jamesthiha   (501) staff       (20)      428 2023-05-14 07:57:19.185054 django-utilitas-1.3.5/setup.cfg
--rw-r--r--   0 jamesthiha   (501) staff       (20)      263 2022-12-05 08:04:03.000000 django-utilitas-1.3.5/setup.py
-drwxr-xr-x   0 jamesthiha   (501) staff       (20)        0 2023-05-14 07:57:19.183199 django-utilitas-1.3.5/utilitas/
--rw-r--r--   0 jamesthiha   (501) staff       (20)        0 2022-11-28 18:11:49.000000 django-utilitas-1.3.5/utilitas/__init__.py
--rw-r--r--   0 jamesthiha   (501) staff       (20)       63 2022-11-28 18:11:49.000000 django-utilitas-1.3.5/utilitas/admin.py
--rw-r--r--   0 jamesthiha   (501) staff       (20)      148 2022-11-28 18:11:50.000000 django-utilitas-1.3.5/utilitas/apps.py
--rw-r--r--   0 jamesthiha   (501) staff       (20)      349 2022-12-05 07:27:09.000000 django-utilitas-1.3.5/utilitas/exception_handler.py
--rw-r--r--   0 jamesthiha   (501) staff       (20)        0 2022-11-28 19:38:13.000000 django-utilitas-1.3.5/utilitas/exceptions.py
--rw-r--r--   0 jamesthiha   (501) staff       (20)       76 2022-12-05 07:26:41.000000 django-utilitas-1.3.5/utilitas/managers.py
--rw-r--r--   0 jamesthiha   (501) staff       (20)      778 2022-12-05 03:43:29.000000 django-utilitas-1.3.5/utilitas/metadata.py
--rw-r--r--   0 jamesthiha   (501) staff       (20)      591 2023-01-25 15:05:12.000000 django-utilitas-1.3.5/utilitas/middlewares.py
-drwxr-xr-x   0 jamesthiha   (501) staff       (20)        0 2023-05-14 07:57:19.183644 django-utilitas-1.3.5/utilitas/migrations/
--rw-r--r--   0 jamesthiha   (501) staff       (20)        0 2022-11-28 18:11:49.000000 django-utilitas-1.3.5/utilitas/migrations/__init__.py
--rw-r--r--   0 jamesthiha   (501) staff       (20)     1454 2022-12-05 07:25:03.000000 django-utilitas-1.3.5/utilitas/models.py
--rw-r--r--   0 jamesthiha   (501) staff       (20)     1031 2023-02-22 06:50:16.000000 django-utilitas-1.3.5/utilitas/pagination.py
--rw-r--r--   0 jamesthiha   (501) staff       (20)      366 2022-11-28 19:43:27.000000 django-utilitas-1.3.5/utilitas/renderer.py
--rw-r--r--   0 jamesthiha   (501) staff       (20)     1450 2023-02-19 23:16:44.000000 django-utilitas-1.3.5/utilitas/serializers.py
--rw-r--r--   0 jamesthiha   (501) staff       (20)      945 2022-12-05 08:14:19.000000 django-utilitas-1.3.5/utilitas/swagger_query_params.py
--rw-r--r--   0 jamesthiha   (501) staff       (20)      347 2022-11-28 19:35:23.000000 django-utilitas-1.3.5/utilitas/swagger_serializers.py
--rw-r--r--   0 jamesthiha   (501) staff       (20)       60 2022-11-28 18:11:49.000000 django-utilitas-1.3.5/utilitas/tests.py
--rw-r--r--   0 jamesthiha   (501) staff       (20)       18 2022-11-28 18:28:32.000000 django-utilitas-1.3.5/utilitas/urls.py
--rw-r--r--   0 jamesthiha   (501) staff       (20)    17468 2023-05-14 07:55:49.000000 django-utilitas-1.3.5/utilitas/views.py
+drwxr-xr-x   0 jamesthiha   (501) staff       (20)        0 2023-05-16 13:12:52.995642 django-utilitas-1.3.6/
+-rw-r--r--   0 jamesthiha   (501) staff       (20)    35149 2022-12-05 07:45:37.000000 django-utilitas-1.3.6/LICENSE
+-rw-r--r--   0 jamesthiha   (501) staff       (20)     4894 2023-05-16 13:12:52.995790 django-utilitas-1.3.6/PKG-INFO
+-rw-r--r--   0 jamesthiha   (501) staff       (20)     4649 2023-05-16 13:12:11.000000 django-utilitas-1.3.6/README.md
+drwxr-xr-x   0 jamesthiha   (501) staff       (20)        0 2023-05-16 13:12:52.984243 django-utilitas-1.3.6/django_utilitas.egg-info/
+-rw-r--r--   0 jamesthiha   (501) staff       (20)     4894 2023-05-16 13:12:52.000000 django-utilitas-1.3.6/django_utilitas.egg-info/PKG-INFO
+-rw-r--r--   0 jamesthiha   (501) staff       (20)      642 2023-05-16 13:12:52.000000 django-utilitas-1.3.6/django_utilitas.egg-info/SOURCES.txt
+-rw-r--r--   0 jamesthiha   (501) staff       (20)        1 2023-05-16 13:12:52.000000 django-utilitas-1.3.6/django_utilitas.egg-info/dependency_links.txt
+-rw-r--r--   0 jamesthiha   (501) staff       (20)       80 2023-05-16 13:12:52.000000 django-utilitas-1.3.6/django_utilitas.egg-info/requires.txt
+-rw-r--r--   0 jamesthiha   (501) staff       (20)        9 2023-05-16 13:12:52.000000 django-utilitas-1.3.6/django_utilitas.egg-info/top_level.txt
+-rw-r--r--   0 jamesthiha   (501) staff       (20)      428 2023-05-16 13:12:52.996386 django-utilitas-1.3.6/setup.cfg
+-rw-r--r--   0 jamesthiha   (501) staff       (20)      263 2022-12-05 08:04:03.000000 django-utilitas-1.3.6/setup.py
+drwxr-xr-x   0 jamesthiha   (501) staff       (20)        0 2023-05-16 13:12:52.994940 django-utilitas-1.3.6/utilitas/
+-rw-r--r--   0 jamesthiha   (501) staff       (20)        0 2022-11-28 18:11:49.000000 django-utilitas-1.3.6/utilitas/__init__.py
+-rw-r--r--   0 jamesthiha   (501) staff       (20)       63 2022-11-28 18:11:49.000000 django-utilitas-1.3.6/utilitas/admin.py
+-rw-r--r--   0 jamesthiha   (501) staff       (20)      148 2022-11-28 18:11:50.000000 django-utilitas-1.3.6/utilitas/apps.py
+-rw-r--r--   0 jamesthiha   (501) staff       (20)      349 2022-12-05 07:27:09.000000 django-utilitas-1.3.6/utilitas/exception_handler.py
+-rw-r--r--   0 jamesthiha   (501) staff       (20)        0 2022-11-28 19:38:13.000000 django-utilitas-1.3.6/utilitas/exceptions.py
+-rw-r--r--   0 jamesthiha   (501) staff       (20)       76 2022-12-05 07:26:41.000000 django-utilitas-1.3.6/utilitas/managers.py
+-rw-r--r--   0 jamesthiha   (501) staff       (20)      778 2022-12-05 03:43:29.000000 django-utilitas-1.3.6/utilitas/metadata.py
+-rw-r--r--   0 jamesthiha   (501) staff       (20)      591 2023-01-25 15:05:12.000000 django-utilitas-1.3.6/utilitas/middlewares.py
+drwxr-xr-x   0 jamesthiha   (501) staff       (20)        0 2023-05-16 13:12:52.995386 django-utilitas-1.3.6/utilitas/migrations/
+-rw-r--r--   0 jamesthiha   (501) staff       (20)        0 2022-11-28 18:11:49.000000 django-utilitas-1.3.6/utilitas/migrations/__init__.py
+-rw-r--r--   0 jamesthiha   (501) staff       (20)     2452 2023-05-16 13:09:58.000000 django-utilitas-1.3.6/utilitas/models.py
+-rw-r--r--   0 jamesthiha   (501) staff       (20)     1031 2023-02-22 06:50:16.000000 django-utilitas-1.3.6/utilitas/pagination.py
+-rw-r--r--   0 jamesthiha   (501) staff       (20)      366 2022-11-28 19:43:27.000000 django-utilitas-1.3.6/utilitas/renderer.py
+-rw-r--r--   0 jamesthiha   (501) staff       (20)     1450 2023-02-19 23:16:44.000000 django-utilitas-1.3.6/utilitas/serializers.py
+-rw-r--r--   0 jamesthiha   (501) staff       (20)      945 2022-12-05 08:14:19.000000 django-utilitas-1.3.6/utilitas/swagger_query_params.py
+-rw-r--r--   0 jamesthiha   (501) staff       (20)      347 2022-11-28 19:35:23.000000 django-utilitas-1.3.6/utilitas/swagger_serializers.py
+-rw-r--r--   0 jamesthiha   (501) staff       (20)       60 2022-11-28 18:11:49.000000 django-utilitas-1.3.6/utilitas/tests.py
+-rw-r--r--   0 jamesthiha   (501) staff       (20)       18 2022-11-28 18:28:32.000000 django-utilitas-1.3.6/utilitas/urls.py
+-rw-r--r--   0 jamesthiha   (501) staff       (20)    17268 2023-05-16 13:11:12.000000 django-utilitas-1.3.6/utilitas/views.py
```

### Comparing `django-utilitas-1.3.5/LICENSE` & `django-utilitas-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `django-utilitas-1.3.5/PKG-INFO` & `django-utilitas-1.3.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-utilitas
-Version: 1.3.5
+Version: 1.3.6
 Summary: Django package with useful utility classes
 Home-page: https://github.com/ninnroot/utilitas
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Django Utilitas
@@ -117,14 +117,16 @@
 requests.get("api/books?csv=true")
 ```
 
 
 ## Changelog
 
 
+- 1.3.6
+    - added an alias option for model fields. (user_friendly_field attribute)
 - 1.3.5
     - bug fixes
 - 1.3.4
     - bug fixes
 - 1.3.3
     - forgot to add csv library. hehe.
 - 1.3.2
```

### Comparing `django-utilitas-1.3.5/README.md` & `django-utilitas-1.3.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -108,14 +108,16 @@
 requests.get("api/books?csv=true")
 ```
 
 
 ## Changelog
 
 
+- 1.3.6
+    - added an alias option for model fields. (user_friendly_field attribute)
 - 1.3.5
     - bug fixes
 - 1.3.4
     - bug fixes
 - 1.3.3
     - forgot to add csv library. hehe.
 - 1.3.2
```

### Comparing `django-utilitas-1.3.5/django_utilitas.egg-info/PKG-INFO` & `django-utilitas-1.3.6/django_utilitas.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-utilitas
-Version: 1.3.5
+Version: 1.3.6
 Summary: Django package with useful utility classes
 Home-page: https://github.com/ninnroot/utilitas
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Django Utilitas
@@ -117,14 +117,16 @@
 requests.get("api/books?csv=true")
 ```
 
 
 ## Changelog
 
 
+- 1.3.6
+    - added an alias option for model fields. (user_friendly_field attribute)
 - 1.3.5
     - bug fixes
 - 1.3.4
     - bug fixes
 - 1.3.3
     - forgot to add csv library. hehe.
 - 1.3.2
```

### Comparing `django-utilitas-1.3.5/django_utilitas.egg-info/SOURCES.txt` & `django-utilitas-1.3.6/django_utilitas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-utilitas-1.3.5/utilitas/metadata.py` & `django-utilitas-1.3.6/utilitas/metadata.py`

 * *Files identical despite different names*

### Comparing `django-utilitas-1.3.5/utilitas/middlewares.py` & `django-utilitas-1.3.6/utilitas/middlewares.py`

 * *Files identical despite different names*

### Comparing `django-utilitas-1.3.5/utilitas/models.py` & `django-utilitas-1.3.6/utilitas/models.py`

 * *Files 21% similar despite different names*

```diff
@@ -18,14 +18,38 @@
     # model fields
     created_at = models.DateTimeField(auto_now_add=True)
     updated_at = models.DateTimeField(auto_now=True)
 
     # only one row can be True throughout the entire table.
     chosen_one_fields = []
 
+    # alias for the field names
+    user_friendly_fields = {
+
+    }
+
+    # provided a list of untransformed field, this function will return a list (in the same order)
+    # of fields translated with user-friendly names.
+    def get_user_friendly_fields(self, fields: Collection[str]):
+        # the 'fields' parameter can contain fields that are not in the 'self.user_firendly_fields' list.
+        # if that's the case, just return the field name as is.
+        lst = []
+        for i in fields:
+            lst.append(self.user_friendly_fields.get(i, i))
+        return lst
+
+
+    # get the field of the model
+    def get_fields(self, include_foreign_fields=False):
+        if not include_foreign_fields:
+            # TODO: clean this up
+            return [i.name for i in self._meta.get_fields() if isinstance(i, (models.CharField, models.TextField, models.BigAutoField, models.DateField, models.DateTimeField, models.BooleanField))]
+        return [i.name for i in self._meta.get_fields()]
+
+
     def save(self, *args, **kwargs):
         for i in self.chosen_one_fields:
             if getattr(self, i):
                 try:
                     obj = self.__class__.objects.get(**{i: True})
                     if obj != self:
                         setattr(obj, i, False)
```

### Comparing `django-utilitas-1.3.5/utilitas/pagination.py` & `django-utilitas-1.3.6/utilitas/pagination.py`

 * *Files identical despite different names*

### Comparing `django-utilitas-1.3.5/utilitas/serializers.py` & `django-utilitas-1.3.6/utilitas/serializers.py`

 * *Files identical despite different names*

### Comparing `django-utilitas-1.3.5/utilitas/swagger_query_params.py` & `django-utilitas-1.3.6/utilitas/swagger_query_params.py`

 * *Files identical despite different names*

### Comparing `django-utilitas-1.3.5/utilitas/views.py` & `django-utilitas-1.3.6/utilitas/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,25 +126,20 @@
         # sending a csv file as response
 
     def send_csv(self, request: Request, data: QuerySet, fields):
         response = HttpResponse(
             content_type="text/csv",
             headers={"Content-Disposition": "attachment; filename='data.csv'"},
         )
+
         if len(fields) == 0:
-            # TODO: clean this later
-            fields = [
-                i.name
-                for i in data.model._meta.get_fields()
-                if isinstance(
-                    i, (CharField, TextField, BigAutoField, DateField, DateTimeField)
-                )
-            ]
+            fields = data.model.get_fields(data.model)
+
         writer = csv.writer(response)
-        writer.writerow(fields)
+        writer.writerow(data.model.get_user_friendly_fields(data.model, fields))
         for i in data:
             lst = []
             for j in fields:
                 lst.append(getattr(i, j))
             writer.writerow(lst)
         return response
 
@@ -317,15 +312,15 @@
         if request.GET.get("meta"):
             return self.send_metadata(request)
 
         if request.query_params.get("csv"):
             return self.send_csv(
                 request,
                 self.get_queryset(
-                    request, filter_params, exclude_params, True, **query_params
+                    request, None, None, True, **query_params
                 ),
                 fields=query_params["fields"],
             )
 
         try:
             query_params = self.get_query_params(request)
         except BadRequest as e:
```

