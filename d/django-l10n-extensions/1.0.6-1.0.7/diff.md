# Comparing `tmp/django-l10n-extensions-1.0.6.tar.gz` & `tmp/django-l10n-extensions-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-l10n-extensions-1.0.6.tar", last modified: Fri May 12 13:38:53 2023, max compression
+gzip compressed data, was "django-l10n-extensions-1.0.7.tar", last modified: Tue May 16 13:19:41 2023, max compression
```

## Comparing `django-l10n-extensions-1.0.6.tar` & `django-l10n-extensions-1.0.7.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxrwxr-x   0 cees      (1000) cees      (1000)        0 2023-05-12 13:38:53.296999 django-l10n-extensions-1.0.6/
--rw-rw-r--   0 cees      (1000) cees      (1000)      249 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/DESCRIPTION
--rw-rw-r--   0 cees      (1000) cees      (1000)      135 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/MANIFEST.in
--rw-rw-r--   0 cees      (1000) cees      (1000)     1635 2023-05-12 13:38:53.296999 django-l10n-extensions-1.0.6/PKG-INFO
--rw-rw-r--   0 cees      (1000) cees      (1000)     1405 2022-02-14 13:37:25.000000 django-l10n-extensions-1.0.6/README.md
--rw-rw-r--   0 cees      (1000) cees      (1000)       38 2023-05-12 13:38:53.296999 django-l10n-extensions-1.0.6/setup.cfg
--rw-rw-r--   0 cees      (1000) cees      (1000)      577 2023-05-12 13:38:18.000000 django-l10n-extensions-1.0.6/setup.py
-drwxrwxr-x   0 cees      (1000) cees      (1000)        0 2023-05-12 13:38:53.288999 django-l10n-extensions-1.0.6/src/
-drwxrwxr-x   0 cees      (1000) cees      (1000)        0 2023-05-12 13:38:53.292999 django-l10n-extensions-1.0.6/src/django_l10n_extensions/
--rw-rw-r--   0 cees      (1000) cees      (1000)     2438 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/django_l10n_extensions/__init__.py
--rw-rw-r--   0 cees      (1000) cees      (1000)      113 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/django_l10n_extensions/exceptions.py
-drwxrwxr-x   0 cees      (1000) cees      (1000)        0 2023-05-12 13:38:53.292999 django-l10n-extensions-1.0.6/src/django_l10n_extensions/forms/
--rw-rw-r--   0 cees      (1000) cees      (1000)        0 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/django_l10n_extensions/forms/__init__.py
--rw-rw-r--   0 cees      (1000) cees      (1000)     1150 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/django_l10n_extensions/forms/fields.py
--rw-rw-r--   0 cees      (1000) cees      (1000)      596 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/django_l10n_extensions/l10n_threading.py
-drwxrwxr-x   0 cees      (1000) cees      (1000)        0 2023-05-12 13:38:53.292999 django-l10n-extensions-1.0.6/src/django_l10n_extensions/management/
--rw-rw-r--   0 cees      (1000) cees      (1000)        0 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/django_l10n_extensions/management/__init__.py
-drwxrwxr-x   0 cees      (1000) cees      (1000)        0 2023-05-12 13:38:53.292999 django-l10n-extensions-1.0.6/src/django_l10n_extensions/management/commands/
--rw-rw-r--   0 cees      (1000) cees      (1000)        0 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/django_l10n_extensions/management/commands/__init__.py
--rw-rw-r--   0 cees      (1000) cees      (1000)     2898 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/django_l10n_extensions/management/commands/makemessages.py
--rw-rw-r--   0 cees      (1000) cees      (1000)    10899 2023-05-12 13:28:40.000000 django-l10n-extensions-1.0.6/src/django_l10n_extensions/measures.py
--rw-rw-r--   0 cees      (1000) cees      (1000)     1449 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/django_l10n_extensions/mixins.py
-drwxrwxr-x   0 cees      (1000) cees      (1000)        0 2023-05-12 13:38:53.292999 django-l10n-extensions-1.0.6/src/django_l10n_extensions/models/
--rw-rw-r--   0 cees      (1000) cees      (1000)       24 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/django_l10n_extensions/models/__init__.py
--rw-rw-r--   0 cees      (1000) cees      (1000)     7649 2023-05-12 13:36:56.000000 django-l10n-extensions-1.0.6/src/django_l10n_extensions/models/fields.py
--rw-rw-r--   0 cees      (1000) cees      (1000)     3899 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/django_l10n_extensions/models/models.py
--rw-rw-r--   0 cees      (1000) cees      (1000)     4785 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/django_l10n_extensions/po_utils.py
--rw-rw-r--   0 cees      (1000) cees      (1000)     2147 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/django_l10n_extensions/settings.py
-drwxrwxr-x   0 cees      (1000) cees      (1000)        0 2023-05-12 13:38:53.292999 django-l10n-extensions-1.0.6/src/django_l10n_extensions/templatetags/
--rw-rw-r--   0 cees      (1000) cees      (1000)        0 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/django_l10n_extensions/templatetags/__init__.py
--rw-rw-r--   0 cees      (1000) cees      (1000)     2290 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/django_l10n_extensions/templatetags/inlinetrans.py
--rw-rw-r--   0 cees      (1000) cees      (1000)     1102 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/django_l10n_extensions/urls.py
--rw-rw-r--   0 cees      (1000) cees      (1000)     1033 2023-05-12 13:35:39.000000 django-l10n-extensions-1.0.6/src/django_l10n_extensions/utils.py
--rw-rw-r--   0 cees      (1000) cees      (1000)     4424 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/django_l10n_extensions/views.py
-drwxrwxr-x   0 cees      (1000) cees      (1000)        0 2023-05-12 13:38:53.292999 django-l10n-extensions-1.0.6/src/django_l10n_extensions.egg-info/
--rw-rw-r--   0 cees      (1000) cees      (1000)     1635 2023-05-12 13:38:53.000000 django-l10n-extensions-1.0.6/src/django_l10n_extensions.egg-info/PKG-INFO
--rw-rw-r--   0 cees      (1000) cees      (1000)     1902 2023-05-12 13:38:53.000000 django-l10n-extensions-1.0.6/src/django_l10n_extensions.egg-info/SOURCES.txt
--rw-rw-r--   0 cees      (1000) cees      (1000)        1 2023-05-12 13:38:53.000000 django-l10n-extensions-1.0.6/src/django_l10n_extensions.egg-info/dependency_links.txt
--rw-rw-r--   0 cees      (1000) cees      (1000)        1 2023-05-12 13:38:53.000000 django-l10n-extensions-1.0.6/src/django_l10n_extensions.egg-info/not-zip-safe
--rw-rw-r--   0 cees      (1000) cees      (1000)       38 2023-05-12 13:38:53.000000 django-l10n-extensions-1.0.6/src/django_l10n_extensions.egg-info/requires.txt
--rw-rw-r--   0 cees      (1000) cees      (1000)       29 2023-05-12 13:38:53.000000 django-l10n-extensions-1.0.6/src/django_l10n_extensions.egg-info/top_level.txt
-drwxrwxr-x   0 cees      (1000) cees      (1000)        0 2023-05-12 13:38:53.292999 django-l10n-extensions-1.0.6/src/tests/
--rw-rw-r--   0 cees      (1000) cees      (1000)        0 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/tests/__init__.py
--rw-rw-r--   0 cees      (1000) cees      (1000)     2172 2023-05-12 13:27:15.000000 django-l10n-extensions-1.0.6/src/tests/conftest.py
-drwxrwxr-x   0 cees      (1000) cees      (1000)        0 2023-05-12 13:38:53.296999 django-l10n-extensions-1.0.6/src/tests/management/
--rw-rw-r--   0 cees      (1000) cees      (1000)        0 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/tests/management/__init__.py
-drwxrwxr-x   0 cees      (1000) cees      (1000)        0 2023-05-12 13:38:53.296999 django-l10n-extensions-1.0.6/src/tests/management/commands/
--rw-rw-r--   0 cees      (1000) cees      (1000)        0 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/tests/management/commands/__init__.py
--rw-rw-r--   0 cees      (1000) cees      (1000)     1813 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/tests/management/commands/test_make_messages.py
-drwxrwxr-x   0 cees      (1000) cees      (1000)        0 2023-05-12 13:38:53.296999 django-l10n-extensions-1.0.6/src/tests/models/
--rw-rw-r--   0 cees      (1000) cees      (1000)        0 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/tests/models/__init__.py
--rw-rw-r--   0 cees      (1000) cees      (1000)      734 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/tests/models/test_l10n_units.py
--rw-rw-r--   0 cees      (1000) cees      (1000)     4197 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/tests/models/test_measure_fields.py
--rw-rw-r--   0 cees      (1000) cees      (1000)     4273 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/tests/models/test_trans_fields.py
--rw-rw-r--   0 cees      (1000) cees      (1000)     2594 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/tests/test_measures.py
-drwxrwxr-x   0 cees      (1000) cees      (1000)        0 2023-05-12 13:38:53.296999 django-l10n-extensions-1.0.6/src/tests/testapp/
--rw-rw-r--   0 cees      (1000) cees      (1000)       80 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/tests/testapp/__init__.py
--rw-rw-r--   0 cees      (1000) cees      (1000)      119 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/tests/testapp/apps.py
-drwxrwxr-x   0 cees      (1000) cees      (1000)        0 2023-05-12 13:38:53.296999 django-l10n-extensions-1.0.6/src/tests/testapp/migrations/
--rw-rw-r--   0 cees      (1000) cees      (1000)     1558 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/tests/testapp/migrations/0001_initial.py
--rw-rw-r--   0 cees      (1000) cees      (1000)        0 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/tests/testapp/migrations/__init__.py
--rw-rw-r--   0 cees      (1000) cees      (1000)      726 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/tests/testapp/models.py
-drwxrwxr-x   0 cees      (1000) cees      (1000)        0 2023-05-12 13:38:53.296999 django-l10n-extensions-1.0.6/src/tests/testapp/scripts/
--rw-rw-r--   0 cees      (1000) cees      (1000)        0 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/tests/testapp/scripts/__init__.py
--rw-rw-r--   0 cees      (1000) cees      (1000)       44 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/tests/testapp/scripts/sample_script.py
--rw-rw-r--   0 cees      (1000) cees      (1000)     1595 2023-05-12 13:32:29.000000 django-l10n-extensions-1.0.6/src/tests/testapp/settings.py
--rw-rw-r--   0 cees      (1000) cees      (1000)     1378 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/tests/testapp/urls.py
--rw-rw-r--   0 cees      (1000) cees      (1000)      362 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/tests/testapp/views.py
+drwxrwxr-x   0 cees      (1000) cees      (1000)        0 2023-05-16 13:19:41.377299 django-l10n-extensions-1.0.7/
+-rw-rw-r--   0 cees      (1000) cees      (1000)      249 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.7/DESCRIPTION
+-rw-rw-r--   0 cees      (1000) cees      (1000)      135 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.7/MANIFEST.in
+-rw-rw-r--   0 cees      (1000) cees      (1000)     1635 2023-05-16 13:19:41.377299 django-l10n-extensions-1.0.7/PKG-INFO
+-rw-rw-r--   0 cees      (1000) cees      (1000)     1405 2022-02-14 13:37:25.000000 django-l10n-extensions-1.0.7/README.md
+-rw-rw-r--   0 cees      (1000) cees      (1000)       38 2023-05-16 13:19:41.377299 django-l10n-extensions-1.0.7/setup.cfg
+-rw-rw-r--   0 cees      (1000) cees      (1000)      577 2023-05-16 12:52:21.000000 django-l10n-extensions-1.0.7/setup.py
+drwxrwxr-x   0 cees      (1000) cees      (1000)        0 2023-05-16 13:19:41.369299 django-l10n-extensions-1.0.7/src/
+drwxrwxr-x   0 cees      (1000) cees      (1000)        0 2023-05-16 13:19:41.373299 django-l10n-extensions-1.0.7/src/django_l10n_extensions/
+-rw-rw-r--   0 cees      (1000) cees      (1000)     2438 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.7/src/django_l10n_extensions/__init__.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)      113 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.7/src/django_l10n_extensions/exceptions.py
+drwxrwxr-x   0 cees      (1000) cees      (1000)        0 2023-05-16 13:19:41.373299 django-l10n-extensions-1.0.7/src/django_l10n_extensions/forms/
+-rw-rw-r--   0 cees      (1000) cees      (1000)        0 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.7/src/django_l10n_extensions/forms/__init__.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)     1150 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.7/src/django_l10n_extensions/forms/fields.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)      596 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.7/src/django_l10n_extensions/l10n_threading.py
+drwxrwxr-x   0 cees      (1000) cees      (1000)        0 2023-05-16 13:19:41.373299 django-l10n-extensions-1.0.7/src/django_l10n_extensions/management/
+-rw-rw-r--   0 cees      (1000) cees      (1000)        0 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.7/src/django_l10n_extensions/management/__init__.py
+drwxrwxr-x   0 cees      (1000) cees      (1000)        0 2023-05-16 13:19:41.373299 django-l10n-extensions-1.0.7/src/django_l10n_extensions/management/commands/
+-rw-rw-r--   0 cees      (1000) cees      (1000)        0 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.7/src/django_l10n_extensions/management/commands/__init__.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)     2898 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.7/src/django_l10n_extensions/management/commands/makemessages.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)    10899 2023-05-12 15:01:09.000000 django-l10n-extensions-1.0.7/src/django_l10n_extensions/measures.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)     1449 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.7/src/django_l10n_extensions/mixins.py
+drwxrwxr-x   0 cees      (1000) cees      (1000)        0 2023-05-16 13:19:41.373299 django-l10n-extensions-1.0.7/src/django_l10n_extensions/models/
+-rw-rw-r--   0 cees      (1000) cees      (1000)       24 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.7/src/django_l10n_extensions/models/__init__.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)     7649 2023-05-12 13:36:56.000000 django-l10n-extensions-1.0.7/src/django_l10n_extensions/models/fields.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)     3900 2023-05-16 12:50:05.000000 django-l10n-extensions-1.0.7/src/django_l10n_extensions/models/models.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)     4785 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.7/src/django_l10n_extensions/po_utils.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)     2147 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.7/src/django_l10n_extensions/settings.py
+drwxrwxr-x   0 cees      (1000) cees      (1000)        0 2023-05-16 13:19:41.373299 django-l10n-extensions-1.0.7/src/django_l10n_extensions/templatetags/
+-rw-rw-r--   0 cees      (1000) cees      (1000)        0 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.7/src/django_l10n_extensions/templatetags/__init__.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)     2290 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.7/src/django_l10n_extensions/templatetags/inlinetrans.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)     1102 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.7/src/django_l10n_extensions/urls.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)     1033 2023-05-12 13:35:39.000000 django-l10n-extensions-1.0.7/src/django_l10n_extensions/utils.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)     4424 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.7/src/django_l10n_extensions/views.py
+drwxrwxr-x   0 cees      (1000) cees      (1000)        0 2023-05-16 13:19:41.373299 django-l10n-extensions-1.0.7/src/django_l10n_extensions.egg-info/
+-rw-rw-r--   0 cees      (1000) cees      (1000)     1635 2023-05-16 13:19:41.000000 django-l10n-extensions-1.0.7/src/django_l10n_extensions.egg-info/PKG-INFO
+-rw-rw-r--   0 cees      (1000) cees      (1000)     1902 2023-05-16 13:19:41.000000 django-l10n-extensions-1.0.7/src/django_l10n_extensions.egg-info/SOURCES.txt
+-rw-rw-r--   0 cees      (1000) cees      (1000)        1 2023-05-16 13:19:41.000000 django-l10n-extensions-1.0.7/src/django_l10n_extensions.egg-info/dependency_links.txt
+-rw-rw-r--   0 cees      (1000) cees      (1000)        1 2023-05-12 13:38:53.000000 django-l10n-extensions-1.0.7/src/django_l10n_extensions.egg-info/not-zip-safe
+-rw-rw-r--   0 cees      (1000) cees      (1000)       38 2023-05-16 13:19:41.000000 django-l10n-extensions-1.0.7/src/django_l10n_extensions.egg-info/requires.txt
+-rw-rw-r--   0 cees      (1000) cees      (1000)       29 2023-05-16 13:19:41.000000 django-l10n-extensions-1.0.7/src/django_l10n_extensions.egg-info/top_level.txt
+drwxrwxr-x   0 cees      (1000) cees      (1000)        0 2023-05-16 13:19:41.373299 django-l10n-extensions-1.0.7/src/tests/
+-rw-rw-r--   0 cees      (1000) cees      (1000)        0 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.7/src/tests/__init__.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)     2172 2023-05-12 13:27:15.000000 django-l10n-extensions-1.0.7/src/tests/conftest.py
+drwxrwxr-x   0 cees      (1000) cees      (1000)        0 2023-05-16 13:19:41.373299 django-l10n-extensions-1.0.7/src/tests/management/
+-rw-rw-r--   0 cees      (1000) cees      (1000)        0 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.7/src/tests/management/__init__.py
+drwxrwxr-x   0 cees      (1000) cees      (1000)        0 2023-05-16 13:19:41.377299 django-l10n-extensions-1.0.7/src/tests/management/commands/
+-rw-rw-r--   0 cees      (1000) cees      (1000)        0 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.7/src/tests/management/commands/__init__.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)     1813 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.7/src/tests/management/commands/test_make_messages.py
+drwxrwxr-x   0 cees      (1000) cees      (1000)        0 2023-05-16 13:19:41.377299 django-l10n-extensions-1.0.7/src/tests/models/
+-rw-rw-r--   0 cees      (1000) cees      (1000)        0 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.7/src/tests/models/__init__.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)      734 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.7/src/tests/models/test_l10n_units.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)     4197 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.7/src/tests/models/test_measure_fields.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)     4273 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.7/src/tests/models/test_trans_fields.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)     2594 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.7/src/tests/test_measures.py
+drwxrwxr-x   0 cees      (1000) cees      (1000)        0 2023-05-16 13:19:41.377299 django-l10n-extensions-1.0.7/src/tests/testapp/
+-rw-rw-r--   0 cees      (1000) cees      (1000)       80 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.7/src/tests/testapp/__init__.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)      119 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.7/src/tests/testapp/apps.py
+drwxrwxr-x   0 cees      (1000) cees      (1000)        0 2023-05-16 13:19:41.377299 django-l10n-extensions-1.0.7/src/tests/testapp/migrations/
+-rw-rw-r--   0 cees      (1000) cees      (1000)     1558 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.7/src/tests/testapp/migrations/0001_initial.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)        0 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.7/src/tests/testapp/migrations/__init__.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)      726 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.7/src/tests/testapp/models.py
+drwxrwxr-x   0 cees      (1000) cees      (1000)        0 2023-05-16 13:19:41.377299 django-l10n-extensions-1.0.7/src/tests/testapp/scripts/
+-rw-rw-r--   0 cees      (1000) cees      (1000)        0 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.7/src/tests/testapp/scripts/__init__.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)       44 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.7/src/tests/testapp/scripts/sample_script.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)     1595 2023-05-12 13:32:29.000000 django-l10n-extensions-1.0.7/src/tests/testapp/settings.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)     1378 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.7/src/tests/testapp/urls.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)      362 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.7/src/tests/testapp/views.py
```

### Comparing `django-l10n-extensions-1.0.6/PKG-INFO` & `django-l10n-extensions-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-l10n-extensions
-Version: 1.0.6
+Version: 1.0.7
 Summary: Extend Django with L10N features.
 Home-page: https://github.com/ceasaro/django-l10n-extensions
 Author: Cees van Wieringen
 Author-email: ceesvw@gmail.com
 
 # Django L10N extensions
 Django L10N extensions adds some useful L10N extensions to the Django framework
```

### Comparing `django-l10n-extensions-1.0.6/README.md` & `django-l10n-extensions-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.0.6/setup.py` & `django-l10n-extensions-1.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='django-l10n-extensions',
-    version='1.0.6',
+    version='1.0.7',
     author=u'Cees van Wieringen',
     author_email='ceesvw@gmail.com',
     package_dir={'': 'src'},
     packages=find_packages(where='./src'),
     include_package_data=True,
     install_requires=['GitPython==1.0.1', 'Django>=2', 'polib>=1.0'],
     url='https://github.com/ceasaro/django-l10n-extensions',
```

### Comparing `django-l10n-extensions-1.0.6/src/django_l10n_extensions/__init__.py` & `django-l10n-extensions-1.0.7/src/django_l10n_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.0.6/src/django_l10n_extensions/forms/fields.py` & `django-l10n-extensions-1.0.7/src/django_l10n_extensions/forms/fields.py`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.0.6/src/django_l10n_extensions/l10n_threading.py` & `django-l10n-extensions-1.0.7/src/django_l10n_extensions/l10n_threading.py`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.0.6/src/django_l10n_extensions/management/commands/makemessages.py` & `django-l10n-extensions-1.0.7/src/django_l10n_extensions/management/commands/makemessages.py`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.0.6/src/django_l10n_extensions/measures.py` & `django-l10n-extensions-1.0.7/src/django_l10n_extensions/measures.py`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.0.6/src/django_l10n_extensions/mixins.py` & `django-l10n-extensions-1.0.7/src/django_l10n_extensions/mixins.py`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.0.6/src/django_l10n_extensions/models/fields.py` & `django-l10n-extensions-1.0.7/src/django_l10n_extensions/models/fields.py`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.0.6/src/django_l10n_extensions/models/models.py` & `django-l10n-extensions-1.0.7/src/django_l10n_extensions/models/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,21 +22,21 @@
     VELOCITY_CHOICES = [(velocity_unit, measures.Velocity.UNITS_REPR.get(velocity_unit, velocity_unit))
                         for velocity_unit in measures.Velocity.UNITS.keys()]
 
     PRECIPITATION_CHOICES = [
         (precipitation_unit, measures.Precipitation.UNITS_REPR.get(precipitation_unit, precipitation_unit))
         for precipitation_unit in measures.Precipitation.UNITS.keys()]
 
-    unit_distance = models.CharField(choices=DISTANCE_CHOICES, max_length=24, null=True, blank=True)
-    unit_area = models.CharField(choices=AREA_CHOICES, max_length=24, null=True, blank=True)
-    unit_weight= models.CharField(choices=WEIGHT_CHOICES, max_length=24, null=True, blank=True)
-    unit_volume = models.CharField(choices=VOLUME_CHOICES, max_length=24, null=True, blank=True)
-    unit_temp = models.CharField(choices=TEMP_CHOICES, max_length=24, null=True, blank=True)
-    unit_velocity = models.CharField(choices=VELOCITY_CHOICES, max_length=24, null=True, blank=True)
-    unit_precipitation = models.CharField(choices=PRECIPITATION_CHOICES, max_length=24, null=True,
+    unit_distance = models.CharField(choices=DISTANCE_CHOICES, max_length=64, null=True, blank=True)
+    unit_area = models.CharField(choices=AREA_CHOICES, max_length=64, null=True, blank=True)
+    unit_weight = models.CharField(choices=WEIGHT_CHOICES, max_length=64, null=True, blank=True)
+    unit_volume = models.CharField(choices=VOLUME_CHOICES, max_length=64, null=True, blank=True)
+    unit_temp = models.CharField(choices=TEMP_CHOICES, max_length=64, null=True, blank=True)
+    unit_velocity = models.CharField(choices=VELOCITY_CHOICES, max_length=64, null=True, blank=True)
+    unit_precipitation = models.CharField(choices=PRECIPITATION_CHOICES, max_length=64, null=True,
                                           blank=True)
 
     def __unicode__(self):
         return u"L10n (Area= {area}) (Distance= {distance}) " \
                u"(Weight= {weight}) (Temperature= {temperature}) (Volume= {volume}) " \
                u"(Velocity = {velocity}) (Precipitation= {precipitation})".format(
             distance=self.get_unit_distance_display(),
```

### Comparing `django-l10n-extensions-1.0.6/src/django_l10n_extensions/po_utils.py` & `django-l10n-extensions-1.0.7/src/django_l10n_extensions/po_utils.py`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.0.6/src/django_l10n_extensions/settings.py` & `django-l10n-extensions-1.0.7/src/django_l10n_extensions/settings.py`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.0.6/src/django_l10n_extensions/templatetags/inlinetrans.py` & `django-l10n-extensions-1.0.7/src/django_l10n_extensions/templatetags/inlinetrans.py`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.0.6/src/django_l10n_extensions/urls.py` & `django-l10n-extensions-1.0.7/src/django_l10n_extensions/urls.py`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.0.6/src/django_l10n_extensions/utils.py` & `django-l10n-extensions-1.0.7/src/django_l10n_extensions/utils.py`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.0.6/src/django_l10n_extensions/views.py` & `django-l10n-extensions-1.0.7/src/django_l10n_extensions/views.py`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.0.6/src/django_l10n_extensions.egg-info/PKG-INFO` & `django-l10n-extensions-1.0.7/src/django_l10n_extensions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-l10n-extensions
-Version: 1.0.6
+Version: 1.0.7
 Summary: Extend Django with L10N features.
 Home-page: https://github.com/ceasaro/django-l10n-extensions
 Author: Cees van Wieringen
 Author-email: ceesvw@gmail.com
 
 # Django L10N extensions
 Django L10N extensions adds some useful L10N extensions to the Django framework
```

### Comparing `django-l10n-extensions-1.0.6/src/django_l10n_extensions.egg-info/SOURCES.txt` & `django-l10n-extensions-1.0.7/src/django_l10n_extensions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.0.6/src/tests/conftest.py` & `django-l10n-extensions-1.0.7/src/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.0.6/src/tests/management/commands/test_make_messages.py` & `django-l10n-extensions-1.0.7/src/tests/management/commands/test_make_messages.py`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.0.6/src/tests/models/test_l10n_units.py` & `django-l10n-extensions-1.0.7/src/tests/models/test_l10n_units.py`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.0.6/src/tests/models/test_measure_fields.py` & `django-l10n-extensions-1.0.7/src/tests/models/test_measure_fields.py`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.0.6/src/tests/models/test_trans_fields.py` & `django-l10n-extensions-1.0.7/src/tests/models/test_trans_fields.py`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.0.6/src/tests/test_measures.py` & `django-l10n-extensions-1.0.7/src/tests/test_measures.py`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.0.6/src/tests/testapp/migrations/0001_initial.py` & `django-l10n-extensions-1.0.7/src/tests/testapp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.0.6/src/tests/testapp/models.py` & `django-l10n-extensions-1.0.7/src/tests/testapp/models.py`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.0.6/src/tests/testapp/settings.py` & `django-l10n-extensions-1.0.7/src/tests/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.0.6/src/tests/testapp/urls.py` & `django-l10n-extensions-1.0.7/src/tests/testapp/urls.py`

 * *Files identical despite different names*

