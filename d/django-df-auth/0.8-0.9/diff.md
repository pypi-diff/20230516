# Comparing `tmp/django-df-auth-0.8.tar.gz` & `tmp/django-df-auth-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-df-auth-0.8.tar", last modified: Tue Aug  9 06:59:19 2022, max compression
+gzip compressed data, was "django-df-auth-0.9.tar", last modified: Tue Aug  9 07:38:24 2022, max compression
```

## Comparing `django-df-auth-0.8.tar` & `django-df-auth-0.9.tar`

### file list

```diff
@@ -1,34 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 06:59:19.550340 django-df-auth-0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-08-09 06:59:08.000000 django-df-auth-0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      210 2022-08-09 06:59:08.000000 django-df-auth-0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      896 2022-08-09 06:59:19.550340 django-df-auth-0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2890 2022-08-09 06:59:08.000000 django-df-auth-0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 06:59:19.550340 django-df-auth-0.8/df_auth/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-09 06:59:08.000000 django-df-auth-0.8/df_auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-08-09 06:59:08.000000 django-df-auth-0.8/df_auth/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)      393 2022-08-09 06:59:08.000000 django-df-auth-0.8/df_auth/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)     2642 2022-08-09 06:59:08.000000 django-df-auth-0.8/df_auth/backends.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 06:59:19.550340 django-df-auth-0.8/df_auth/djangoflow/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-09 06:59:08.000000 django-df-auth-0.8/df_auth/djangoflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      231 2022-08-09 06:59:08.000000 django-df-auth-0.8/df_auth/djangoflow/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 06:59:19.550340 django-df-auth-0.8/df_auth/drf/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-09 06:59:08.000000 django-df-auth-0.8/df_auth/drf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4234 2022-08-09 06:59:08.000000 django-df-auth-0.8/df_auth/drf/serializers.py
--rw-r--r--   0 runner    (1001) docker     (121)      540 2022-08-09 06:59:08.000000 django-df-auth-0.8/df_auth/drf/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     2135 2022-08-09 06:59:08.000000 django-df-auth-0.8/df_auth/drf/viewsets.py
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-08-09 06:59:08.000000 django-df-auth-0.8/df_auth/models.py
--rw-r--r--   0 runner    (1001) docker     (121)      431 2022-08-09 06:59:08.000000 django-df-auth-0.8/df_auth/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)      265 2022-08-09 06:59:08.000000 django-df-auth-0.8/df_auth/strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 06:59:19.550340 django-df-auth-0.8/django_df_auth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      896 2022-08-09 06:59:19.000000 django-df-auth-0.8/django_df_auth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      589 2022-08-09 06:59:19.000000 django-df-auth-0.8/django_df_auth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-09 06:59:19.000000 django-df-auth-0.8/django_df_auth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      118 2022-08-09 06:59:19.000000 django-df-auth-0.8/django_df_auth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-08-09 06:59:19.000000 django-df-auth-0.8/django_df_auth.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 06:59:19.550340 django-df-auth-0.8/docs/
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-08-09 06:59:08.000000 django-df-auth-0.8/docs/TODO.md
--rw-r--r--   0 runner    (1001) docker     (121)      204 2022-08-09 06:59:08.000000 django-df-auth-0.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1228 2022-08-09 06:59:08.000000 django-df-auth-0.8/docs/requirements.md
--rw-r--r--   0 runner    (1001) docker     (121)      109 2022-08-09 06:59:08.000000 django-df-auth-0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1418 2022-08-09 06:59:19.550340 django-df-auth-0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-08-09 06:59:08.000000 django-df-auth-0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 07:38:24.312603 django-df-auth-0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-08-09 07:38:15.000000 django-df-auth-0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      210 2022-08-09 07:38:15.000000 django-df-auth-0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)      896 2022-08-09 07:38:24.312603 django-df-auth-0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2890 2022-08-09 07:38:15.000000 django-df-auth-0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 07:38:24.312603 django-df-auth-0.9/df_auth/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-09 07:38:15.000000 django-df-auth-0.9/df_auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       35 2022-08-09 07:38:15.000000 django-df-auth-0.9/df_auth/admin.py
+-rw-r--r--   0 runner    (1001) docker     (121)      393 2022-08-09 07:38:15.000000 django-df-auth-0.9/df_auth/apps.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2577 2022-08-09 07:38:15.000000 django-df-auth-0.9/df_auth/backends.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 07:38:24.312603 django-df-auth-0.9/df_auth/djangoflow/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-09 07:38:15.000000 django-df-auth-0.9/df_auth/djangoflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      231 2022-08-09 07:38:15.000000 django-df-auth-0.9/df_auth/djangoflow/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 07:38:24.312603 django-df-auth-0.9/df_auth/drf/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-09 07:38:15.000000 django-df-auth-0.9/df_auth/drf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4234 2022-08-09 07:38:15.000000 django-df-auth-0.9/df_auth/drf/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (121)      540 2022-08-09 07:38:15.000000 django-df-auth-0.9/df_auth/drf/urls.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2135 2022-08-09 07:38:15.000000 django-df-auth-0.9/df_auth/drf/viewsets.py
+-rw-r--r--   0 runner    (1001) docker     (121)       31 2022-08-09 07:38:15.000000 django-df-auth-0.9/df_auth/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)      431 2022-08-09 07:38:15.000000 django-df-auth-0.9/df_auth/settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)      265 2022-08-09 07:38:15.000000 django-df-auth-0.9/df_auth/strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 07:38:24.312603 django-df-auth-0.9/df_auth/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-09 07:38:15.000000 django-df-auth-0.9/df_auth/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      418 2022-08-09 07:38:15.000000 django-df-auth-0.9/df_auth/templatetags/auth_magic_link.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 07:38:24.312603 django-df-auth-0.9/django_df_auth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      896 2022-08-09 07:38:24.000000 django-df-auth-0.9/django_df_auth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      662 2022-08-09 07:38:24.000000 django-df-auth-0.9/django_df_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-09 07:38:24.000000 django-df-auth-0.9/django_df_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      118 2022-08-09 07:38:24.000000 django-df-auth-0.9/django_df_auth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-08-09 07:38:24.000000 django-df-auth-0.9/django_df_auth.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 07:38:24.312603 django-df-auth-0.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)       82 2022-08-09 07:38:15.000000 django-df-auth-0.9/docs/TODO.md
+-rw-r--r--   0 runner    (1001) docker     (121)      204 2022-08-09 07:38:15.000000 django-df-auth-0.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1228 2022-08-09 07:38:15.000000 django-df-auth-0.9/docs/requirements.md
+-rw-r--r--   0 runner    (1001) docker     (121)      109 2022-08-09 07:38:15.000000 django-df-auth-0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     1418 2022-08-09 07:38:24.312603 django-df-auth-0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)       39 2022-08-09 07:38:15.000000 django-df-auth-0.9/setup.py
```

### Comparing `django-df-auth-0.8/LICENSE` & `django-df-auth-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-df-auth-0.8/PKG-INFO` & `django-df-auth-0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-df-auth
-Version: 0.8
+Version: 0.9
 Summary: Opinionated Django REST auth endpoints for JWT authentication and social accounts.
 Home-page: https://apexive.com/
 Author: Apexive OSS
 Author-email: open-source@apexive.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `django-df-auth-0.8/README.md` & `django-df-auth-0.9/README.md`

 * *Files identical despite different names*

### Comparing `django-df-auth-0.8/df_auth/backends.py` & `django-df-auth-0.9/df_auth/backends.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,14 +47,12 @@
 
                                 return user
                             raise ValidationError(
                                 _("Wrong or expired one-time password")
                             )
 
     def generate_challenge(self, request=None, user=None, email=None, extra_context=None, **kwargs):
-        if extra_context is None:
-            extra_context = {}
         users = [user] if user else self.get_users(email)
         if email:
             for user in users:
                 device = EmailDevice.objects.get_or_create(user=user, email=email)[0]
                 device.generate_challenge(extra_context=extra_context)
```

### Comparing `django-df-auth-0.8/df_auth/drf/serializers.py` & `django-df-auth-0.9/df_auth/drf/serializers.py`

 * *Files identical despite different names*

### Comparing `django-df-auth-0.8/df_auth/drf/urls.py` & `django-df-auth-0.9/df_auth/drf/urls.py`

 * *Files identical despite different names*

### Comparing `django-df-auth-0.8/df_auth/drf/viewsets.py` & `django-df-auth-0.9/df_auth/drf/viewsets.py`

 * *Files identical despite different names*

### Comparing `django-df-auth-0.8/django_df_auth.egg-info/PKG-INFO` & `django-df-auth-0.9/django_df_auth.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-df-auth
-Version: 0.8
+Version: 0.9
 Summary: Opinionated Django REST auth endpoints for JWT authentication and social accounts.
 Home-page: https://apexive.com/
 Author: Apexive OSS
 Author-email: open-source@apexive.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `django-df-auth-0.8/django_df_auth.egg-info/SOURCES.txt` & `django-df-auth-0.9/django_df_auth.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 df_auth/strategy.py
 df_auth/djangoflow/__init__.py
 df_auth/djangoflow/settings.py
 df_auth/drf/__init__.py
 df_auth/drf/serializers.py
 df_auth/drf/urls.py
 df_auth/drf/viewsets.py
+df_auth/templatetags/__init__.py
+df_auth/templatetags/auth_magic_link.py
 django_df_auth.egg-info/PKG-INFO
 django_df_auth.egg-info/SOURCES.txt
 django_df_auth.egg-info/dependency_links.txt
 django_df_auth.egg-info/requires.txt
 django_df_auth.egg-info/top_level.txt
 docs/TODO.md
 docs/index.rst
```

### Comparing `django-df-auth-0.8/docs/requirements.md` & `django-df-auth-0.9/docs/requirements.md`

 * *Files identical despite different names*

### Comparing `django-df-auth-0.8/setup.cfg` & `django-df-auth-0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 force_alphabetical_sort = True
 force_single_line = True
 lines_after_imports = 2
 line_length = 160
 
 [metadata]
 name = django-df-auth
-version = 0.8
+version = 0.9
 description = Opinionated Django REST auth endpoints for JWT authentication and social accounts.
 long_description = file: README.rst
 url = https://apexive.com/
 author = Apexive OSS
 author_email = open-source@apexive.com
 license = MIT
 classifiers =
```

