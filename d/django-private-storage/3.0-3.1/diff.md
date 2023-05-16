# Comparing `tmp/django-private-storage-3.0.tar.gz` & `tmp/django-private-storage-3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-private-storage-3.0.tar", last modified: Tue Nov 16 22:33:45 2021, max compression
+gzip compressed data, was "django-private-storage-3.1.tar", last modified: Tue May 16 10:08:18 2023, max compression
```

## Comparing `django-private-storage-3.0.tar` & `django-private-storage-3.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 diederik   (501) staff       (20)        0 2021-11-16 22:33:45.141180 django-private-storage-3.0/
--rw-r--r--   0 diederik   (501) staff       (20)      313 2019-11-04 15:54:14.000000 django-private-storage-3.0/AUTHORS
--rw-r--r--   0 diederik   (501) staff       (20)    11357 2016-10-06 14:00:25.000000 django-private-storage-3.0/LICENSE
--rw-r--r--   0 diederik   (501) staff       (20)      239 2016-10-10 10:16:47.000000 django-private-storage-3.0/MANIFEST.in
--rw-r--r--   0 diederik   (501) staff       (20)    16130 2021-11-16 22:33:45.140853 django-private-storage-3.0/PKG-INFO
--rw-r--r--   0 diederik   (501) staff       (20)    11875 2021-11-16 22:25:51.000000 django-private-storage-3.0/README.rst
-drwxr-xr-x   0 diederik   (501) staff       (20)        0 2021-11-16 22:33:45.127733 django-private-storage-3.0/django_private_storage.egg-info/
--rw-r--r--   0 diederik   (501) staff       (20)    16130 2021-11-16 22:33:44.000000 django-private-storage-3.0/django_private_storage.egg-info/PKG-INFO
--rw-r--r--   0 diederik   (501) staff       (20)     1221 2021-11-16 22:33:44.000000 django-private-storage-3.0/django_private_storage.egg-info/SOURCES.txt
--rw-r--r--   0 diederik   (501) staff       (20)        1 2021-11-16 22:33:44.000000 django-private-storage-3.0/django_private_storage.egg-info/dependency_links.txt
--rw-r--r--   0 diederik   (501) staff       (20)        1 2018-02-06 11:40:26.000000 django-private-storage-3.0/django_private_storage.egg-info/not-zip-safe
--rw-r--r--   0 diederik   (501) staff       (20)       16 2021-11-16 22:33:44.000000 django-private-storage-3.0/django_private_storage.egg-info/top_level.txt
-drwxr-xr-x   0 diederik   (501) staff       (20)        0 2021-11-16 22:33:45.131454 django-private-storage-3.0/private_storage/
--rw-r--r--   0 diederik   (501) staff       (20)       40 2021-11-16 22:33:03.000000 django-private-storage-3.0/private_storage/__init__.py
--rw-r--r--   0 diederik   (501) staff       (20)      866 2021-11-16 22:24:25.000000 django-private-storage-3.0/private_storage/appconfig.py
--rw-r--r--   0 diederik   (501) staff       (20)     8733 2021-11-16 22:32:06.000000 django-private-storage-3.0/private_storage/fields.py
-drwxr-xr-x   0 diederik   (501) staff       (20)        0 2021-11-16 22:33:45.123390 django-private-storage-3.0/private_storage/locale/
-drwxr-xr-x   0 diederik   (501) staff       (20)        0 2021-11-16 22:33:45.122724 django-private-storage-3.0/private_storage/locale/ca/
-drwxr-xr-x   0 diederik   (501) staff       (20)        0 2021-11-16 22:33:45.132336 django-private-storage-3.0/private_storage/locale/ca/LC_MESSAGES/
--rw-r--r--   0 diederik   (501) staff       (20)      529 2021-05-17 10:03:39.000000 django-private-storage-3.0/private_storage/locale/ca/LC_MESSAGES/django.mo
--rw-r--r--   0 diederik   (501) staff       (20)      822 2019-04-08 12:31:54.000000 django-private-storage-3.0/private_storage/locale/ca/LC_MESSAGES/django.po
-drwxr-xr-x   0 diederik   (501) staff       (20)        0 2021-11-16 22:33:45.122977 django-private-storage-3.0/private_storage/locale/en/
-drwxr-xr-x   0 diederik   (501) staff       (20)        0 2021-11-16 22:33:45.133439 django-private-storage-3.0/private_storage/locale/en/LC_MESSAGES/
--rw-r--r--   0 diederik   (501) staff       (20)      337 2021-05-17 10:03:39.000000 django-private-storage-3.0/private_storage/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 diederik   (501) staff       (20)      742 2018-09-10 08:51:49.000000 django-private-storage-3.0/private_storage/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 diederik   (501) staff       (20)        0 2021-11-16 22:33:45.123242 django-private-storage-3.0/private_storage/locale/fr/
-drwxr-xr-x   0 diederik   (501) staff       (20)        0 2021-11-16 22:33:45.134550 django-private-storage-3.0/private_storage/locale/fr/LC_MESSAGES/
--rw-r--r--   0 diederik   (501) staff       (20)      538 2021-05-17 10:03:39.000000 django-private-storage-3.0/private_storage/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 diederik   (501) staff       (20)      832 2021-05-17 08:59:05.000000 django-private-storage-3.0/private_storage/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 diederik   (501) staff       (20)        0 2021-11-16 22:33:45.123481 django-private-storage-3.0/private_storage/locale/nl/
-drwxr-xr-x   0 diederik   (501) staff       (20)        0 2021-11-16 22:33:45.135693 django-private-storage-3.0/private_storage/locale/nl/LC_MESSAGES/
--rw-r--r--   0 diederik   (501) staff       (20)      581 2021-05-17 10:03:39.000000 django-private-storage-3.0/private_storage/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0 diederik   (501) staff       (20)      906 2018-09-10 08:52:06.000000 django-private-storage-3.0/private_storage/locale/nl/LC_MESSAGES/django.po
--rw-r--r--   0 diederik   (501) staff       (20)     1749 2021-11-16 22:32:06.000000 django-private-storage-3.0/private_storage/models.py
--rw-r--r--   0 diederik   (501) staff       (20)      937 2021-05-17 09:16:01.000000 django-private-storage-3.0/private_storage/permissions.py
--rw-r--r--   0 diederik   (501) staff       (20)     6762 2021-11-16 22:32:06.000000 django-private-storage-3.0/private_storage/servers.py
-drwxr-xr-x   0 diederik   (501) staff       (20)        0 2021-11-16 22:33:45.137659 django-private-storage-3.0/private_storage/storage/
--rw-r--r--   0 diederik   (501) staff       (20)      335 2021-05-17 09:16:01.000000 django-private-storage-3.0/private_storage/storage/__init__.py
--rw-r--r--   0 diederik   (501) staff       (20)     1226 2021-11-16 22:32:06.000000 django-private-storage-3.0/private_storage/storage/files.py
--rw-r--r--   0 diederik   (501) staff       (20)     3841 2021-11-16 22:24:25.000000 django-private-storage-3.0/private_storage/storage/minio.py
--rw-r--r--   0 diederik   (501) staff       (20)     4245 2021-11-16 22:32:06.000000 django-private-storage-3.0/private_storage/storage/s3boto3.py
-drwxr-xr-x   0 diederik   (501) staff       (20)        0 2021-11-16 22:33:45.140071 django-private-storage-3.0/private_storage/tests/
--rw-r--r--   0 diederik   (501) staff       (20)        0 2018-02-06 11:14:38.000000 django-private-storage-3.0/private_storage/tests/__init__.py
--rw-r--r--   0 diederik   (501) staff       (20)     1125 2021-05-17 09:16:01.000000 django-private-storage-3.0/private_storage/tests/models.py
--rw-r--r--   0 diederik   (501) staff       (20)      380 2018-02-06 11:14:38.000000 django-private-storage-3.0/private_storage/tests/test_imports.py
--rw-r--r--   0 diederik   (501) staff       (20)     1720 2021-05-17 09:19:27.000000 django-private-storage-3.0/private_storage/tests/test_models.py
--rw-r--r--   0 diederik   (501) staff       (20)     5333 2021-11-16 22:32:06.000000 django-private-storage-3.0/private_storage/tests/test_views.py
--rw-r--r--   0 diederik   (501) staff       (20)      960 2021-11-16 22:32:06.000000 django-private-storage-3.0/private_storage/tests/utils.py
--rw-r--r--   0 diederik   (501) staff       (20)      179 2021-05-17 10:01:17.000000 django-private-storage-3.0/private_storage/urls.py
--rw-r--r--   0 diederik   (501) staff       (20)     6614 2021-11-16 22:32:06.000000 django-private-storage-3.0/private_storage/views.py
--rw-r--r--   0 diederik   (501) staff       (20)       38 2021-11-16 22:33:45.141269 django-private-storage-3.0/setup.cfg
--rwxr-xr-x   0 diederik   (501) staff       (20)     2586 2021-05-17 09:18:43.000000 django-private-storage-3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 10:08:18.040629 django-private-storage-3.1/
+-rw-r--r--   0 runner    (1001) docker     (122)      313 2023-05-16 10:08:05.000000 django-private-storage-3.1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-05-16 10:08:05.000000 django-private-storage-3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      239 2023-05-16 10:08:05.000000 django-private-storage-3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    16348 2023-05-16 10:08:18.040629 django-private-storage-3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    11875 2023-05-16 10:08:05.000000 django-private-storage-3.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 10:08:18.032628 django-private-storage-3.1/django_private_storage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    16348 2023-05-16 10:08:17.000000 django-private-storage-3.1/django_private_storage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1221 2023-05-16 10:08:17.000000 django-private-storage-3.1/django_private_storage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-16 10:08:17.000000 django-private-storage-3.1/django_private_storage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-16 10:08:17.000000 django-private-storage-3.1/django_private_storage.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-05-16 10:08:17.000000 django-private-storage-3.1/django_private_storage.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 10:08:18.032628 django-private-storage-3.1/private_storage/
+-rw-r--r--   0 runner    (1001) docker     (122)       40 2023-05-16 10:08:05.000000 django-private-storage-3.1/private_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      866 2023-05-16 10:08:05.000000 django-private-storage-3.1/private_storage/appconfig.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8733 2023-05-16 10:08:05.000000 django-private-storage-3.1/private_storage/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 10:08:18.028628 django-private-storage-3.1/private_storage/locale/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 10:08:18.028628 django-private-storage-3.1/private_storage/locale/ca/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 10:08:18.036629 django-private-storage-3.1/private_storage/locale/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      529 2023-05-16 10:08:17.000000 django-private-storage-3.1/private_storage/locale/ca/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)      822 2023-05-16 10:08:05.000000 django-private-storage-3.1/private_storage/locale/ca/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 10:08:18.028628 django-private-storage-3.1/private_storage/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 10:08:18.036629 django-private-storage-3.1/private_storage/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      337 2023-05-16 10:08:17.000000 django-private-storage-3.1/private_storage/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)      742 2023-05-16 10:08:05.000000 django-private-storage-3.1/private_storage/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 10:08:18.028628 django-private-storage-3.1/private_storage/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 10:08:18.036629 django-private-storage-3.1/private_storage/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      538 2023-05-16 10:08:17.000000 django-private-storage-3.1/private_storage/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)      832 2023-05-16 10:08:05.000000 django-private-storage-3.1/private_storage/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 10:08:18.028628 django-private-storage-3.1/private_storage/locale/nl/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 10:08:18.036629 django-private-storage-3.1/private_storage/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      581 2023-05-16 10:08:17.000000 django-private-storage-3.1/private_storage/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)      906 2023-05-16 10:08:05.000000 django-private-storage-3.1/private_storage/locale/nl/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     1750 2023-05-16 10:08:05.000000 django-private-storage-3.1/private_storage/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)      937 2023-05-16 10:08:05.000000 django-private-storage-3.1/private_storage/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7009 2023-05-16 10:08:05.000000 django-private-storage-3.1/private_storage/servers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 10:08:18.036629 django-private-storage-3.1/private_storage/storage/
+-rw-r--r--   0 runner    (1001) docker     (122)      335 2023-05-16 10:08:05.000000 django-private-storage-3.1/private_storage/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1226 2023-05-16 10:08:05.000000 django-private-storage-3.1/private_storage/storage/files.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3841 2023-05-16 10:08:05.000000 django-private-storage-3.1/private_storage/storage/minio.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4245 2023-05-16 10:08:05.000000 django-private-storage-3.1/private_storage/storage/s3boto3.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 10:08:18.040629 django-private-storage-3.1/private_storage/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-16 10:08:05.000000 django-private-storage-3.1/private_storage/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1125 2023-05-16 10:08:05.000000 django-private-storage-3.1/private_storage/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)      380 2023-05-16 10:08:05.000000 django-private-storage-3.1/private_storage/tests/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1720 2023-05-16 10:08:05.000000 django-private-storage-3.1/private_storage/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5333 2023-05-16 10:08:05.000000 django-private-storage-3.1/private_storage/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (122)      960 2023-05-16 10:08:05.000000 django-private-storage-3.1/private_storage/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      179 2023-05-16 10:08:05.000000 django-private-storage-3.1/private_storage/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6614 2023-05-16 10:08:05.000000 django-private-storage-3.1/private_storage/views.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-16 10:08:18.040629 django-private-storage-3.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2799 2023-05-16 10:08:05.000000 django-private-storage-3.1/setup.py
```

### Comparing `django-private-storage-3.0/LICENSE` & `django-private-storage-3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-private-storage-3.0/PKG-INFO` & `django-private-storage-3.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-private-storage
-Version: 3.0
+Version: 3.1
 Summary: Private media file storage for Django projects
 Home-page: https://github.com/edoburu/django-private-storage
 Author: Diederik van der Boor
 Author-email: opensource@edoburu.nl
 License: Apache 2.0
 Download-URL: https://github.com/edoburu/django-private-storage/zipball/master
 Description: django-private-storage
@@ -49,15 +49,15 @@
         Add to ``urls.py``:
         
         .. code-block:: python
         
             import private_storage.urls
         
             urlpatterns += [
-                url('^private-media/', include(private_storage.urls)),
+                path('private-media/', include(private_storage.urls)),
             ]
         
         Usage
         -----
         
         In a Django model, add the ``PrivateFileField``:
         
@@ -376,17 +376,22 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires: Django (>=1.11)
```

### Comparing `django-private-storage-3.0/README.rst` & `django-private-storage-3.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 Add to ``urls.py``:
 
 .. code-block:: python
 
     import private_storage.urls
 
     urlpatterns += [
-        url('^private-media/', include(private_storage.urls)),
+        path('private-media/', include(private_storage.urls)),
     ]
 
 Usage
 -----
 
 In a Django model, add the ``PrivateFileField``:
```

### Comparing `django-private-storage-3.0/django_private_storage.egg-info/PKG-INFO` & `django-private-storage-3.1/django_private_storage.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-private-storage
-Version: 3.0
+Version: 3.1
 Summary: Private media file storage for Django projects
 Home-page: https://github.com/edoburu/django-private-storage
 Author: Diederik van der Boor
 Author-email: opensource@edoburu.nl
 License: Apache 2.0
 Download-URL: https://github.com/edoburu/django-private-storage/zipball/master
 Description: django-private-storage
@@ -49,15 +49,15 @@
         Add to ``urls.py``:
         
         .. code-block:: python
         
             import private_storage.urls
         
             urlpatterns += [
-                url('^private-media/', include(private_storage.urls)),
+                path('private-media/', include(private_storage.urls)),
             ]
         
         Usage
         -----
         
         In a Django model, add the ``PrivateFileField``:
         
@@ -376,17 +376,22 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires: Django (>=1.11)
```

### Comparing `django-private-storage-3.0/django_private_storage.egg-info/SOURCES.txt` & `django-private-storage-3.1/django_private_storage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-private-storage-3.0/private_storage/appconfig.py` & `django-private-storage-3.1/private_storage/appconfig.py`

 * *Files identical despite different names*

### Comparing `django-private-storage-3.0/private_storage/fields.py` & `django-private-storage-3.1/private_storage/fields.py`

 * *Files identical despite different names*

### Comparing `django-private-storage-3.0/private_storage/locale/ca/LC_MESSAGES/django.mo` & `django-private-storage-3.1/private_storage/locale/ca/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-private-storage-3.0/private_storage/locale/ca/LC_MESSAGES/django.po` & `django-private-storage-3.1/private_storage/locale/ca/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-private-storage-3.0/private_storage/locale/en/LC_MESSAGES/django.po` & `django-private-storage-3.1/private_storage/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-private-storage-3.0/private_storage/locale/fr/LC_MESSAGES/django.mo` & `django-private-storage-3.1/private_storage/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-private-storage-3.0/private_storage/locale/fr/LC_MESSAGES/django.po` & `django-private-storage-3.1/private_storage/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-private-storage-3.0/private_storage/locale/nl/LC_MESSAGES/django.mo` & `django-private-storage-3.1/private_storage/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-private-storage-3.0/private_storage/locale/nl/LC_MESSAGES/django.po` & `django-private-storage-3.1/private_storage/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-private-storage-3.0/private_storage/models.py` & `django-private-storage-3.1/private_storage/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import mimetypes
 
-from django.core.files.storage import File, Storage
+#from django.core.files.storage import File, Storage
 from django.utils.functional import cached_property
 
 
 class PrivateFile:
     """
     A wrapper object that describes the file that is being accessed.
     """
```

### Comparing `django-private-storage-3.0/private_storage/permissions.py` & `django-private-storage-3.1/private_storage/permissions.py`

 * *Files identical despite different names*

### Comparing `django-private-storage-3.0/private_storage/servers.py` & `django-private-storage-3.1/private_storage/servers.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import time
 from functools import lru_cache, wraps
 from urllib.parse import quote
 
 from django.conf import settings
 from django.core.exceptions import ImproperlyConfigured
 from django.http import FileResponse, HttpResponse, HttpResponseNotModified
+from django.utils import version
 from django.utils.http import http_date
 from django.utils.module_loading import import_string
 from django.views.static import serve, was_modified_since
 
 
 @lru_cache()
 def get_server_class(path):
@@ -58,27 +59,31 @@
 
     @staticmethod
     @add_no_cache_headers
     def serve(private_file):
         # Support If-Last-Modified
         mtime = private_file.modified_time.timestamp()
         size = private_file.size
-        if not was_modified_since(private_file.request.META.get('HTTP_IF_MODIFIED_SINCE'), mtime, size):
-            return HttpResponseNotModified()
+        if version.get_main_version() >= '4.1':
+            was_modified = was_modified_since(private_file.request.META.get('HTTP_IF_MODIFIED_SINCE'), mtime)
+        else:
+            was_modified = was_modified_since(private_file.request.META.get('HTTP_IF_MODIFIED_SINCE'), mtime, size)
+
+        if not was_modified: return HttpResponseNotModified()
 
         # As of Django 1.8, FileResponse triggers 'wsgi.file_wrapper' in Django's WSGIHandler.
         # This uses efficient file streaming, such as sendfile() in uWSGI.
         # When the WSGI container doesn't provide 'wsgi.file_wrapper', it submits the file in 4KB chunks.
         if private_file.request.method == 'HEAD':
             # Avoid reading the file at all
             response = HttpResponse()
         else:
             response = FileResponse(private_file.open())
         response['Content-Type'] = private_file.content_type
-        response['Content-Length'] = size
+        response['Content-Length'] = private_file.size
         response["Last-Modified"] = http_date(mtime)
         return response
 
 
 class DjangoServer(DjangoStreamingServer):
     """
     Serve static files from the local filesystem through Django or ``wsgi_file_wrapper``.
```

### Comparing `django-private-storage-3.0/private_storage/storage/files.py` & `django-private-storage-3.1/private_storage/storage/files.py`

 * *Files identical despite different names*

### Comparing `django-private-storage-3.0/private_storage/storage/minio.py` & `django-private-storage-3.1/private_storage/storage/minio.py`

 * *Files identical despite different names*

### Comparing `django-private-storage-3.0/private_storage/storage/s3boto3.py` & `django-private-storage-3.1/private_storage/storage/s3boto3.py`

 * *Files identical despite different names*

### Comparing `django-private-storage-3.0/private_storage/tests/models.py` & `django-private-storage-3.1/private_storage/tests/models.py`

 * *Files identical despite different names*

### Comparing `django-private-storage-3.0/private_storage/tests/test_models.py` & `django-private-storage-3.1/private_storage/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django-private-storage-3.0/private_storage/tests/test_views.py` & `django-private-storage-3.1/private_storage/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-private-storage-3.0/private_storage/tests/utils.py` & `django-private-storage-3.1/private_storage/tests/utils.py`

 * *Files identical despite different names*

### Comparing `django-private-storage-3.0/private_storage/views.py` & `django-private-storage-3.1/private_storage/views.py`

 * *Files identical despite different names*

### Comparing `django-private-storage-3.0/setup.py` & `django-private-storage-3.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -65,18 +65,23 @@
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
         'Framework :: Django',
         'Framework :: Django :: 2.2',
         'Framework :: Django :: 3.0',
         'Framework :: Django :: 3.1',
         'Framework :: Django :: 3.2',
+        'Framework :: Django :: 4.0',
+        'Framework :: Django :: 4.1',
+        'Framework :: Django :: 4.2',
         'Topic :: Internet :: WWW/HTTP',
         'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
         'Topic :: Software Development :: Libraries :: Application Frameworks',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ]
 )
```

