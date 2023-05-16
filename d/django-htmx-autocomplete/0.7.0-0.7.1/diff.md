# Comparing `tmp/django-htmx-autocomplete-0.7.0.tar.gz` & `tmp/django-htmx-autocomplete-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-htmx-autocomplete-0.7.0.tar", last modified: Thu Apr 27 16:43:18 2023, max compression
+gzip compressed data, was "django-htmx-autocomplete-0.7.1.tar", last modified: Tue May 16 17:53:31 2023, max compression
```

## Comparing `django-htmx-autocomplete-0.7.0.tar` & `django-htmx-autocomplete-0.7.1.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:43:18.288826 django-htmx-autocomplete-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-04-27 16:43:18.288826 django-htmx-autocomplete-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5476 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:43:18.280826 django-htmx-autocomplete-0.7.0/autocomplete/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/autocomplete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/autocomplete/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)    25303 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/autocomplete/autocomplete.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:43:18.276826 django-htmx-autocomplete-0.7.0/autocomplete/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:43:18.276826 django-htmx-autocomplete-0.7.0/autocomplete/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:43:18.280826 django-htmx-autocomplete-0.7.0/autocomplete/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-27 16:43:18.000000 django-htmx-autocomplete-0.7.0/autocomplete/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/autocomplete/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:43:18.276826 django-htmx-autocomplete-0.7.0/autocomplete/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:43:18.280826 django-htmx-autocomplete-0.7.0/autocomplete/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-27 16:43:18.000000 django-htmx-autocomplete-0.7.0/autocomplete/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/autocomplete/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:43:18.276826 django-htmx-autocomplete-0.7.0/autocomplete/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:43:18.276826 django-htmx-autocomplete-0.7.0/autocomplete/static/autocomplete/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:43:18.280826 django-htmx-autocomplete-0.7.0/autocomplete/static/autocomplete/css/
--rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/autocomplete/static/autocomplete/css/autocomplete.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:43:18.280826 django-htmx-autocomplete-0.7.0/autocomplete/static/autocomplete/js/
--rw-r--r--   0 runner    (1001) docker     (123)    13659 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/autocomplete/static/autocomplete/js/autocomplete.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:43:18.276826 django-htmx-autocomplete-0.7.0/autocomplete/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:43:18.284826 django-htmx-autocomplete-0.7.0/autocomplete/templates/autocomplete/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/autocomplete/templates/autocomplete/ac_container.html
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/autocomplete/templates/autocomplete/chip.html
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/autocomplete/templates/autocomplete/chip_list.html
--rw-r--r--   0 runner    (1001) docker     (123)     6694 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/autocomplete/templates/autocomplete/component.html
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/autocomplete/templates/autocomplete/head.html
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/autocomplete/templates/autocomplete/indicator-icon.html
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/autocomplete/templates/autocomplete/item.html
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/autocomplete/templates/autocomplete/item_list.html
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/autocomplete/templates/autocomplete/scripts.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:43:18.284826 django-htmx-autocomplete-0.7.0/autocomplete/templates/autocomplete/strings/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/autocomplete/templates/autocomplete/strings/available_results.html
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/autocomplete/templates/autocomplete/strings/backspace_instruction.html
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/autocomplete/templates/autocomplete/strings/item_selected.html
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/autocomplete/templates/autocomplete/strings/more_results.html
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/autocomplete/templates/autocomplete/strings/multiselect.html
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/autocomplete/templates/autocomplete/strings/no_results.html
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/autocomplete/templates/autocomplete/strings/nothing_selected.html
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/autocomplete/templates/autocomplete/strings/selected.html
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/autocomplete/templates/autocomplete/textinput.html
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/autocomplete/templates/autocomplete/values.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:43:18.288826 django-htmx-autocomplete-0.7.0/autocomplete/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/autocomplete/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/autocomplete/templatetags/autocomplete.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/autocomplete/test_autocomplete.py
--rw-r--r--   0 runner    (1001) docker     (123)     5245 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/autocomplete/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:43:18.288826 django-htmx-autocomplete-0.7.0/django_htmx_autocomplete.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-04-27 16:43:18.000000 django-htmx-autocomplete-0.7.0/django_htmx_autocomplete.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-27 16:43:18.000000 django-htmx-autocomplete-0.7.0/django_htmx_autocomplete.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 16:43:18.000000 django-htmx-autocomplete-0.7.0/django_htmx_autocomplete.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-27 16:43:18.000000 django-htmx-autocomplete-0.7.0/django_htmx_autocomplete.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-27 16:43:18.000000 django-htmx-autocomplete-0.7.0/django_htmx_autocomplete.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-27 16:43:18.288826 django-htmx-autocomplete-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-27 16:42:41.000000 django-htmx-autocomplete-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:53:31.805837 django-htmx-autocomplete-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-16 17:53:05.000000 django-htmx-autocomplete-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-16 17:53:05.000000 django-htmx-autocomplete-0.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-05-16 17:53:31.805837 django-htmx-autocomplete-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5476 2023-05-16 17:53:05.000000 django-htmx-autocomplete-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:53:31.801837 django-htmx-autocomplete-0.7.1/autocomplete/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-16 17:53:05.000000 django-htmx-autocomplete-0.7.1/autocomplete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-16 17:53:05.000000 django-htmx-autocomplete-0.7.1/autocomplete/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25303 2023-05-16 17:53:05.000000 django-htmx-autocomplete-0.7.1/autocomplete/autocomplete.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:53:31.801837 django-htmx-autocomplete-0.7.1/autocomplete/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:53:31.801837 django-htmx-autocomplete-0.7.1/autocomplete/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:53:31.801837 django-htmx-autocomplete-0.7.1/autocomplete/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-16 17:53:31.000000 django-htmx-autocomplete-0.7.1/autocomplete/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-16 17:53:05.000000 django-htmx-autocomplete-0.7.1/autocomplete/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:53:31.801837 django-htmx-autocomplete-0.7.1/autocomplete/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:53:31.805837 django-htmx-autocomplete-0.7.1/autocomplete/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-16 17:53:31.000000 django-htmx-autocomplete-0.7.1/autocomplete/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-16 17:53:05.000000 django-htmx-autocomplete-0.7.1/autocomplete/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:53:31.801837 django-htmx-autocomplete-0.7.1/autocomplete/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:53:31.801837 django-htmx-autocomplete-0.7.1/autocomplete/static/autocomplete/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:53:31.805837 django-htmx-autocomplete-0.7.1/autocomplete/static/autocomplete/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-05-16 17:53:05.000000 django-htmx-autocomplete-0.7.1/autocomplete/static/autocomplete/css/autocomplete.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:53:31.805837 django-htmx-autocomplete-0.7.1/autocomplete/static/autocomplete/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    13946 2023-05-16 17:53:05.000000 django-htmx-autocomplete-0.7.1/autocomplete/static/autocomplete/js/autocomplete.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:53:31.801837 django-htmx-autocomplete-0.7.1/autocomplete/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:53:31.805837 django-htmx-autocomplete-0.7.1/autocomplete/templates/autocomplete/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-16 17:53:05.000000 django-htmx-autocomplete-0.7.1/autocomplete/templates/autocomplete/ac_container.html
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-16 17:53:05.000000 django-htmx-autocomplete-0.7.1/autocomplete/templates/autocomplete/chip.html
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-16 17:53:05.000000 django-htmx-autocomplete-0.7.1/autocomplete/templates/autocomplete/chip_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-05-16 17:53:05.000000 django-htmx-autocomplete-0.7.1/autocomplete/templates/autocomplete/component.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-16 17:53:05.000000 django-htmx-autocomplete-0.7.1/autocomplete/templates/autocomplete/head.html
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-16 17:53:05.000000 django-htmx-autocomplete-0.7.1/autocomplete/templates/autocomplete/indicator-icon.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-05-16 17:53:05.000000 django-htmx-autocomplete-0.7.1/autocomplete/templates/autocomplete/item.html
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-16 17:53:05.000000 django-htmx-autocomplete-0.7.1/autocomplete/templates/autocomplete/item_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-16 17:53:05.000000 django-htmx-autocomplete-0.7.1/autocomplete/templates/autocomplete/scripts.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:53:31.805837 django-htmx-autocomplete-0.7.1/autocomplete/templates/autocomplete/strings/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-16 17:53:05.000000 django-htmx-autocomplete-0.7.1/autocomplete/templates/autocomplete/strings/available_results.html
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-16 17:53:05.000000 django-htmx-autocomplete-0.7.1/autocomplete/templates/autocomplete/strings/backspace_instruction.html
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-16 17:53:05.000000 django-htmx-autocomplete-0.7.1/autocomplete/templates/autocomplete/strings/item_selected.html
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-16 17:53:05.000000 django-htmx-autocomplete-0.7.1/autocomplete/templates/autocomplete/strings/more_results.html
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-16 17:53:05.000000 django-htmx-autocomplete-0.7.1/autocomplete/templates/autocomplete/strings/multiselect.html
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-16 17:53:05.000000 django-htmx-autocomplete-0.7.1/autocomplete/templates/autocomplete/strings/no_results.html
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-16 17:53:05.000000 django-htmx-autocomplete-0.7.1/autocomplete/templates/autocomplete/strings/nothing_selected.html
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-16 17:53:05.000000 django-htmx-autocomplete-0.7.1/autocomplete/templates/autocomplete/strings/selected.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-05-16 17:53:05.000000 django-htmx-autocomplete-0.7.1/autocomplete/templates/autocomplete/textinput.html
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-16 17:53:05.000000 django-htmx-autocomplete-0.7.1/autocomplete/templates/autocomplete/values.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:53:31.805837 django-htmx-autocomplete-0.7.1/autocomplete/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 17:53:05.000000 django-htmx-autocomplete-0.7.1/autocomplete/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-05-16 17:53:05.000000 django-htmx-autocomplete-0.7.1/autocomplete/templatetags/autocomplete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-16 17:53:05.000000 django-htmx-autocomplete-0.7.1/autocomplete/test_autocomplete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5245 2023-05-16 17:53:05.000000 django-htmx-autocomplete-0.7.1/autocomplete/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:53:31.805837 django-htmx-autocomplete-0.7.1/django_htmx_autocomplete.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-05-16 17:53:31.000000 django-htmx-autocomplete-0.7.1/django_htmx_autocomplete.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-16 17:53:31.000000 django-htmx-autocomplete-0.7.1/django_htmx_autocomplete.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 17:53:31.000000 django-htmx-autocomplete-0.7.1/django_htmx_autocomplete.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-16 17:53:31.000000 django-htmx-autocomplete-0.7.1/django_htmx_autocomplete.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-16 17:53:31.000000 django-htmx-autocomplete-0.7.1/django_htmx_autocomplete.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:53:05.000000 django-htmx-autocomplete-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-16 17:53:31.809837 django-htmx-autocomplete-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-16 17:53:05.000000 django-htmx-autocomplete-0.7.1/setup.py
```

### Comparing `django-htmx-autocomplete-0.7.0/LICENSE` & `django-htmx-autocomplete-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-htmx-autocomplete-0.7.0/PKG-INFO` & `django-htmx-autocomplete-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-htmx-autocomplete
-Version: 0.7.0
+Version: 0.7.1
 Summary: A Django autocomplete component powered by htmx
 Home-page: https://github.com/PHACDataHub/django-htmx-autocomplete
 Author: Luc Belliveau
 Author-email: luc.belliveau@canada.ca
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-htmx-autocomplete Version: 0.7.0 Summary: A
+Metadata-Version: 2.1 Name: django-htmx-autocomplete Version: 0.7.1 Summary: A
 Django autocomplete component powered by htmx Home-page: https://github.com/
 PHACDataHub/django-htmx-autocomplete Author: Luc Belliveau Author-email:
 luc.belliveau@canada.ca License: MIT Classifier: Environment :: Web Environment
 Classifier: Framework :: Django Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
```

### Comparing `django-htmx-autocomplete-0.7.0/README.md` & `django-htmx-autocomplete-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `django-htmx-autocomplete-0.7.0/autocomplete/autocomplete.py` & `django-htmx-autocomplete-0.7.1/autocomplete/autocomplete.py`

 * *Files identical despite different names*

### Comparing `django-htmx-autocomplete-0.7.0/autocomplete/locale/en/LC_MESSAGES/django.po` & `django-htmx-autocomplete-0.7.1/autocomplete/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-htmx-autocomplete-0.7.0/autocomplete/locale/fr/LC_MESSAGES/django.mo` & `django-htmx-autocomplete-0.7.1/autocomplete/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-htmx-autocomplete-0.7.0/autocomplete/locale/fr/LC_MESSAGES/django.po` & `django-htmx-autocomplete-0.7.1/autocomplete/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-htmx-autocomplete-0.7.0/autocomplete/static/autocomplete/css/autocomplete.css` & `django-htmx-autocomplete-0.7.1/autocomplete/static/autocomplete/css/autocomplete.css`

 * *Files identical despite different names*

### Comparing `django-htmx-autocomplete-0.7.0/autocomplete/static/autocomplete/js/autocomplete.js` & `django-htmx-autocomplete-0.7.1/autocomplete/static/autocomplete/js/autocomplete.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,7 +1,17 @@
+function phac_aspc_autocomplete_trigger_change(container_id) {
+    setTimeout(() => {
+        const container = document.getElementById(container_id);
+        const el = container.querySelector('.textinput');
+        el.dispatchEvent(new Event('change', {
+            bubbles: true
+        }));
+    }, 0)
+}
+
 function phac_aspc_autocomplete_clear_focus(container, activate_ring) {
     const hasFocus = container.querySelectorAll('.hasFocus');
     for (const el of hasFocus) {
         el.classList.remove('hasFocus');
     }
 
     const el = container.querySelector('.textinput');
```

### Comparing `django-htmx-autocomplete-0.7.0/autocomplete/templates/autocomplete/ac_container.html` & `django-htmx-autocomplete-0.7.1/autocomplete/templates/autocomplete/ac_container.html`

 * *Files identical despite different names*

### Comparing `django-htmx-autocomplete-0.7.0/autocomplete/templates/autocomplete/chip.html` & `django-htmx-autocomplete-0.7.1/autocomplete/templates/autocomplete/chip.html`

 * *Files identical despite different names*

### Comparing `django-htmx-autocomplete-0.7.0/autocomplete/templates/autocomplete/component.html` & `django-htmx-autocomplete-0.7.1/autocomplete/templates/autocomplete/component.html`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 {% comment %} 
 This is the main component template that creates the basic HTML structure.
 {% endcomment %}
 <div class="phac_aspc_form_autocomplete_focus_ring {{ disabled|yesno:'disabled,' }}">
   <div
     id="{{ component_id }}__container"
     class="phac_aspc_form_autocomplete"
-    hx-preserve
   >
     {% comment %} Hidden input elements used to maintain the component's state {% endcomment %}
     {% comment %} and used when submitting forms {% endcomment %}
     <div id="{{ component_id }}">
       {% include "./values.html" %}
     </div>
 
@@ -63,83 +62,93 @@
             {% use_string "backspace_instruction" custom_strings %}
         {% endif %}
     </div>
     {% endif %}
   </div>
 </div>
 {% comment %} This code snippet loads the required CSS and JS if not already loaded. {% endcomment %}
-<script>
+<script
+    data-componentid="{{ component_id }}"
+    data-css="{% static 'autocomplete/css/autocomplete.css' %}"
+    data-js="{% static "autocomplete/js/autocomplete.js" %}"
+    data-toggleurl="{% url route_name method='toggle' %}"
+>
     (function () {
+        const { componentid, css, js, toggleurl } = document.currentScript.dataset;
         // Add CSS if not already added
         const ln = document.createElement('link');
-        ln.href = '{% static 'autocomplete/css/autocomplete.css' %}';
+        ln.href = css;
         ln.rel = 'stylesheet';
         if (!Array.from(document.querySelectorAll('link')).map(s => s.href).includes(ln.href)) {
             document.getElementsByTagName('head')[0].appendChild(ln);
         }
         {% if not disabled %}
         {% comment %} If component is disabled no JS is required {% endcomment %}
         // Add JS if not already added
         const sc = document.createElement('script');
-        sc.src = '{% static "autocomplete/js/autocomplete.js" %}';
+        sc.src = js;
         if (!Array.from(document.querySelectorAll('script')).map(s => s.src).includes(sc.src)) {
             document.body.appendChild(sc);
         }
         // Add click handler on container to set focus on <input> box
-        document.querySelector('#{{ component_id }}__container').addEventListener(
+        document.querySelector(`#${componentid}__container`).addEventListener(
             'mousedown',
             function(event) {
                 const container = event.target.closest('.phac_aspc_form_autocomplete');
                 const id = container.getAttribute('id');
                 phac_aspc_autocomplete_blur_skip[id] = true;
             }
         );
-        document.querySelector('#{{ component_id }}__container').addEventListener(
+        document.querySelector(`#${componentid}__container`).addEventListener(
             'mouseup',
             function(event) {
                 const container = event.target.closest('.phac_aspc_form_autocomplete');
                 const id = container.getAttribute('id');
                 phac_aspc_autocomplete_blur_skip[id] = false;
             }
         );
-        document.querySelector('#{{ component_id }}__container').addEventListener(
+        document.querySelector(`#${componentid}__container`).addEventListener(
             'click',
             function(event) {
                 if (
                     event.target === this ||
                     event.target.classList.contains('ac_container') ||
                     event.target.classList.contains('textinput')
                 ) {
                     return phac_aspc_autocomplete_click_handler(event);
                 }
             }
         );
         document.body.addEventListener(
             'htmx:afterSettle', (event) => {
-                if (event.detail.elt.getAttribute('id') === '{{ component_id }}__items') {
+                if (event.detail.elt.getAttribute('id') === `${componentid}__items`) {
                     const shown = event.detail.elt.classList.contains('show');
-                    const el = document.querySelector('#{{ component_id }}__textinput');
+                    const el = document.querySelector(`#${componentid}__textinput`);
                     el.setAttribute('aria-expanded', shown);	
+                } else if (
+                    event.detail.elt.getAttribute('id') === `${componentid}__textinput` &&
+                    event.detail.pathInfo.requestPath === toggleurl
+                ) {
+                    phac_aspc_autocomplete_trigger_change(`${componentid}__container`);
                 }
             }
         );
         document.body.addEventListener(
-        //document.querySelector('#{{ component_id }}__textinput').addEventListener(
             'htmx:oobAfterSwap', (event) => {
-                if (event.detail.target.getAttribute('id') == '{{ component_id }}__textinput') {
+                if (event.detail.target.getAttribute('id') == `${componentid}__textinput`) {
                     setTimeout(() => {
-                        const el = document.querySelector('#{{ component_id }}__textinput');
-                        phac_aspc_autocomplete_set_initial_value(document.querySelector('#{{ component_id }}__container'), true);
+                        const el = document.querySelector(`#${componentid}__textinput`);
+                        phac_aspc_autocomplete_set_initial_value(document.querySelector(`#${componentid}__container`), true);
                         el.selectionStart = el.selectionEnd = el.value.length;
                     }, 0)
                 }
             }
         );
         document.body.addEventListener('htmx:configRequest', function(event) {
-            const container = document.querySelector('#{{ component_id }}__container');
+            const container = document.querySelector(`#${componentid}__container`);
             if (
                 container.contains(event.detail.elt) &&
                 event.detail.path.endsWith('/toggle')
             ) {
                 // HTMX will include the entire form for non get requests, so we update
                 // it here.  If the name is being used in multiple locations in the
                 // form, without this intervention it will not work as expected.
```

### Comparing `django-htmx-autocomplete-0.7.0/autocomplete/templates/autocomplete/head.html` & `django-htmx-autocomplete-0.7.1/autocomplete/templates/autocomplete/head.html`

 * *Files identical despite different names*

### Comparing `django-htmx-autocomplete-0.7.0/autocomplete/templates/autocomplete/indicator-icon.html` & `django-htmx-autocomplete-0.7.1/autocomplete/templates/autocomplete/indicator-icon.html`

 * *Files identical despite different names*

### Comparing `django-htmx-autocomplete-0.7.0/autocomplete/templates/autocomplete/item.html` & `django-htmx-autocomplete-0.7.1/autocomplete/templates/autocomplete/item.html`

 * *Files 4% similar despite different names*

```diff
@@ -169,8 +169,19 @@
 00000a80: 6f63 6f6d 706c 6574 652f 6974 656d 2e68  ocomplete/item.h
 00000a90: 746d 6c22 2077 6974 6820 746f 6767 6c65  tml" with toggle
 00000aa0: 3d4e 6f6e 6520 7377 6170 5f6f 6f62 3d54  =None swap_oob=T
 00000ab0: 7275 6520 257d 0a20 2020 2020 2020 2020  rue %}.         
 00000ac0: 2020 207b 2520 656e 6469 6620 257d 0a20     {% endif %}. 
 00000ad0: 2020 2020 2020 207b 2520 656e 6466 6f72         {% endfor
 00000ae0: 2025 7d0a 2020 2020 7b25 2065 6e64 6966   %}.    {% endif
-00000af0: 2025 7d0a 7b25 2065 6e64 6966 2025 7d     %}.{% endif %}
+00000af0: 2025 7d0a 2020 2020 3c73 6372 6970 7420   %}.    <script 
+00000b00: 6461 7461 2d63 6f6d 706f 6e65 6e74 6964  data-componentid
+00000b10: 3d22 7b7b 2063 6f6d 706f 6e65 6e74 5f69  ="{{ component_i
+00000b20: 6420 7d7d 223e 0a20 2020 2020 2020 2070  d }}">.        p
+00000b30: 6861 635f 6173 7063 5f61 7574 6f63 6f6d  hac_aspc_autocom
+00000b40: 706c 6574 655f 7472 6967 6765 725f 6368  plete_trigger_ch
+00000b50: 616e 6765 2864 6f63 756d 656e 742e 6375  ange(document.cu
+00000b60: 7272 656e 7453 6372 6970 742e 6461 7461  rrentScript.data
+00000b70: 7365 742e 636f 6d70 6f6e 656e 7469 6420  set.componentid 
+00000b80: 2b20 275f 5f63 6f6e 7461 696e 6572 2729  + '__container')
+00000b90: 3b0a 2020 2020 3c2f 7363 7269 7074 3e0a  ;.    </script>.
+00000ba0: 0a7b 2520 656e 6469 6620 257d            .{% endif %}
```

### Comparing `django-htmx-autocomplete-0.7.0/autocomplete/templates/autocomplete/item_list.html` & `django-htmx-autocomplete-0.7.1/autocomplete/templates/autocomplete/item_list.html`

 * *Files identical despite different names*

### Comparing `django-htmx-autocomplete-0.7.0/autocomplete/templates/autocomplete/scripts.html` & `django-htmx-autocomplete-0.7.1/autocomplete/templates/autocomplete/scripts.html`

 * *Files identical despite different names*

### Comparing `django-htmx-autocomplete-0.7.0/autocomplete/templates/autocomplete/textinput.html` & `django-htmx-autocomplete-0.7.1/autocomplete/templates/autocomplete/textinput.html`

 * *Files identical despite different names*

### Comparing `django-htmx-autocomplete-0.7.0/autocomplete/templatetags/autocomplete.py` & `django-htmx-autocomplete-0.7.1/autocomplete/templatetags/autocomplete.py`

 * *Files identical despite different names*

### Comparing `django-htmx-autocomplete-0.7.0/autocomplete/test_autocomplete.py` & `django-htmx-autocomplete-0.7.1/autocomplete/test_autocomplete.py`

 * *Files identical despite different names*

### Comparing `django-htmx-autocomplete-0.7.0/autocomplete/widgets.py` & `django-htmx-autocomplete-0.7.1/autocomplete/widgets.py`

 * *Files identical despite different names*

### Comparing `django-htmx-autocomplete-0.7.0/django_htmx_autocomplete.egg-info/PKG-INFO` & `django-htmx-autocomplete-0.7.1/django_htmx_autocomplete.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-htmx-autocomplete
-Version: 0.7.0
+Version: 0.7.1
 Summary: A Django autocomplete component powered by htmx
 Home-page: https://github.com/PHACDataHub/django-htmx-autocomplete
 Author: Luc Belliveau
 Author-email: luc.belliveau@canada.ca
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-htmx-autocomplete Version: 0.7.0 Summary: A
+Metadata-Version: 2.1 Name: django-htmx-autocomplete Version: 0.7.1 Summary: A
 Django autocomplete component powered by htmx Home-page: https://github.com/
 PHACDataHub/django-htmx-autocomplete Author: Luc Belliveau Author-email:
 luc.belliveau@canada.ca License: MIT Classifier: Environment :: Web Environment
 Classifier: Framework :: Django Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
```

### Comparing `django-htmx-autocomplete-0.7.0/django_htmx_autocomplete.egg-info/SOURCES.txt` & `django-htmx-autocomplete-0.7.1/django_htmx_autocomplete.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-htmx-autocomplete-0.7.0/setup.cfg` & `django-htmx-autocomplete-0.7.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-htmx-autocomplete
-version = 0.7.0
+version = 0.7.1
 description = A Django autocomplete component powered by htmx
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/PHACDataHub/django-htmx-autocomplete
 author = Luc Belliveau
 author_email = luc.belliveau@canada.ca
 license = MIT
```

### Comparing `django-htmx-autocomplete-0.7.0/setup.py` & `django-htmx-autocomplete-0.7.1/setup.py`

 * *Files identical despite different names*

