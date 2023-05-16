# Comparing `tmp/fwadmin-0.0.3.tar.gz` & `tmp/fwadmin-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fwadmin-0.0.3.tar", last modified: Wed May 10 15:56:09 2023, max compression
+gzip compressed data, was "fwadmin-0.0.5.tar", last modified: Tue May 16 09:04:54 2023, max compression
```

## Comparing `fwadmin-0.0.3.tar` & `fwadmin-0.0.5.tar`

### file list

```diff
@@ -1,59 +1,63 @@
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-10 15:56:09.291735 fwadmin-0.0.3/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    35149 2023-05-05 06:03:20.000000 fwadmin-0.0.3/LICENSE
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      248 2023-05-05 06:18:18.000000 fwadmin-0.0.3/MANIFEST.in
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      477 2023-05-10 15:56:09.291735 fwadmin-0.0.3/PKG-INFO
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      614 2023-05-05 19:11:38.000000 fwadmin-0.0.3/README.md
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-10 15:56:09.275735 fwadmin-0.0.3/fwadmin/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1414 2023-05-10 15:56:08.000000 fwadmin-0.0.3/fwadmin/__init__.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-10 15:56:09.279735 fwadmin-0.0.3/fwadmin/api/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-05-10 15:56:08.000000 fwadmin-0.0.3/fwadmin/api/__init__.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1911 2023-05-10 15:56:08.000000 fwadmin-0.0.3/fwadmin/api/serializers.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      604 2023-05-10 15:56:08.000000 fwadmin-0.0.3/fwadmin/api/urls.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1215 2023-05-10 15:56:08.000000 fwadmin-0.0.3/fwadmin/api/views.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2604 2023-05-10 15:56:08.000000 fwadmin-0.0.3/fwadmin/filtersets.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     4206 2023-05-10 15:56:08.000000 fwadmin-0.0.3/fwadmin/forms.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-10 15:56:09.283735 fwadmin-0.0.3/fwadmin/migrations/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     7938 2023-05-10 15:56:08.000000 fwadmin-0.0.3/fwadmin/migrations/0001_initial.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      499 2023-05-10 15:56:08.000000 fwadmin-0.0.3/fwadmin/migrations/0002_remove_sessionrequest_user_and_more.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1115 2023-05-10 15:56:08.000000 fwadmin-0.0.3/fwadmin/migrations/0003_sessionrequest_authorized_by_and_more.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      985 2023-05-10 15:56:08.000000 fwadmin-0.0.3/fwadmin/migrations/0004_remove_sessionrequest_action_reason_and_more.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      612 2023-05-10 15:56:08.000000 fwadmin-0.0.3/fwadmin/migrations/0005_rename_approved_by_sessionrequest_managed_by_and_more.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-05-10 15:56:08.000000 fwadmin-0.0.3/fwadmin/migrations/__init__.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     7231 2023-05-10 15:56:08.000000 fwadmin-0.0.3/fwadmin/models.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2162 2023-05-10 15:56:08.000000 fwadmin-0.0.3/fwadmin/navigation.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3008 2023-05-10 15:56:08.000000 fwadmin-0.0.3/fwadmin/tables.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3386 2023-05-10 15:56:08.000000 fwadmin-0.0.3/fwadmin/tasks.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-10 15:56:09.267734 fwadmin-0.0.3/fwadmin/templates/
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-10 15:56:09.287735 fwadmin-0.0.3/fwadmin/templates/fwadmin/
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-10 15:56:09.287735 fwadmin-0.0.3/fwadmin/templates/fwadmin/buttons/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      402 2023-05-08 19:10:26.000000 fwadmin-0.0.3/fwadmin/templates/fwadmin/buttons/approve.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      399 2023-05-08 19:10:38.000000 fwadmin-0.0.3/fwadmin/templates/fwadmin/buttons/reject.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      412 2023-05-08 19:11:15.000000 fwadmin-0.0.3/fwadmin/templates/fwadmin/buttons/self_approve.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1495 2023-05-06 13:26:26.000000 fwadmin-0.0.3/fwadmin/templates/fwadmin/devicegroup.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2557 2023-05-10 10:35:53.000000 fwadmin-0.0.3/fwadmin/templates/fwadmin/dynamiclist.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1852 2023-05-06 13:21:06.000000 fwadmin-0.0.3/fwadmin/templates/fwadmin/firewall.html
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-10 15:56:09.287735 fwadmin-0.0.3/fwadmin/templates/fwadmin/htmx/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1250 2023-05-09 18:44:21.000000 fwadmin-0.0.3/fwadmin/templates/fwadmin/htmx/manage_form.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3169 2023-05-08 18:21:36.000000 fwadmin-0.0.3/fwadmin/templates/fwadmin/sessionrequest.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1381 2023-05-10 09:38:16.000000 fwadmin-0.0.3/fwadmin/templates/fwadmin/sessionrequest_bulk_manage.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1973 2023-05-10 10:43:02.000000 fwadmin-0.0.3/fwadmin/templates/fwadmin/sessionrequest_list.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      637 2023-05-08 18:50:35.000000 fwadmin-0.0.3/fwadmin/templates/fwadmin/sessionrequest_manage.html
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-10 15:56:09.291735 fwadmin-0.0.3/fwadmin/templatetags/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-05-10 15:56:08.000000 fwadmin-0.0.3/fwadmin/templatetags/__init__.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-10 15:56:09.291735 fwadmin-0.0.3/fwadmin/templatetags/__pycache__/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      150 2023-05-05 15:02:55.000000 fwadmin-0.0.3/fwadmin/templatetags/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1284 2023-05-10 09:28:33.000000 fwadmin-0.0.3/fwadmin/templatetags/__pycache__/fwadmin_buttons.cpython-310.pyc
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1048 2023-05-05 06:16:08.000000 fwadmin-0.0.3/fwadmin/templatetags/__pycache__/netdoc_buttons.cpython-310.pyc
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1203 2023-05-10 15:56:08.000000 fwadmin-0.0.3/fwadmin/templatetags/fwadmin_buttons.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3980 2023-05-10 15:56:08.000000 fwadmin-0.0.3/fwadmin/urls.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    16276 2023-05-10 15:56:08.000000 fwadmin-0.0.3/fwadmin/views.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1006 2023-05-10 15:56:08.000000 fwadmin-0.0.3/fwadmin/workflows.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-10 15:56:09.279735 fwadmin-0.0.3/fwadmin.egg-info/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      477 2023-05-10 15:56:09.000000 fwadmin-0.0.3/fwadmin.egg-info/PKG-INFO
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1646 2023-05-10 15:56:09.000000 fwadmin-0.0.3/fwadmin.egg-info/SOURCES.txt
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        1 2023-05-10 15:56:09.000000 fwadmin-0.0.3/fwadmin.egg-info/dependency_links.txt
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        1 2023-05-05 14:55:33.000000 fwadmin-0.0.3/fwadmin.egg-info/not-zip-safe
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        9 2023-05-10 15:56:09.000000 fwadmin-0.0.3/fwadmin.egg-info/requires.txt
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        8 2023-05-10 15:56:09.000000 fwadmin-0.0.3/fwadmin.egg-info/top_level.txt
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      103 2023-05-10 15:56:09.291735 fwadmin-0.0.3/setup.cfg
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1058 2023-05-10 15:56:08.000000 fwadmin-0.0.3/setup.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-16 09:04:54.670095 fwadmin-0.0.5/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    35149 2023-05-05 06:03:20.000000 fwadmin-0.0.5/LICENSE
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      248 2023-05-05 06:18:18.000000 fwadmin-0.0.5/MANIFEST.in
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      477 2023-05-16 09:04:54.670095 fwadmin-0.0.5/PKG-INFO
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      614 2023-05-05 19:11:38.000000 fwadmin-0.0.5/README.md
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-16 09:04:54.634094 fwadmin-0.0.5/fwadmin/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      718 2023-05-16 09:04:53.000000 fwadmin-0.0.5/fwadmin/__init__.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-16 09:04:54.646095 fwadmin-0.0.5/fwadmin/api/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-05-10 15:56:08.000000 fwadmin-0.0.5/fwadmin/api/__init__.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1911 2023-05-10 15:56:08.000000 fwadmin-0.0.5/fwadmin/api/serializers.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      604 2023-05-10 15:56:08.000000 fwadmin-0.0.5/fwadmin/api/urls.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1215 2023-05-10 15:56:08.000000 fwadmin-0.0.5/fwadmin/api/views.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2604 2023-05-10 15:56:08.000000 fwadmin-0.0.5/fwadmin/filtersets.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     4206 2023-05-10 15:56:08.000000 fwadmin-0.0.5/fwadmin/forms.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-16 09:04:54.654095 fwadmin-0.0.5/fwadmin/migrations/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     7938 2023-05-10 15:56:08.000000 fwadmin-0.0.5/fwadmin/migrations/0001_initial.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      499 2023-05-10 15:56:08.000000 fwadmin-0.0.5/fwadmin/migrations/0002_remove_sessionrequest_user_and_more.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1115 2023-05-10 15:56:08.000000 fwadmin-0.0.5/fwadmin/migrations/0003_sessionrequest_authorized_by_and_more.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      985 2023-05-10 15:56:08.000000 fwadmin-0.0.5/fwadmin/migrations/0004_remove_sessionrequest_action_reason_and_more.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      612 2023-05-10 15:56:08.000000 fwadmin-0.0.5/fwadmin/migrations/0005_rename_approved_by_sessionrequest_managed_by_and_more.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      696 2023-05-13 16:01:48.000000 fwadmin-0.0.5/fwadmin/migrations/0006_remove_firewall_access_key_firewall_verify_cert_and_more.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-05-10 15:56:08.000000 fwadmin-0.0.5/fwadmin/migrations/__init__.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     7232 2023-05-16 07:19:51.000000 fwadmin-0.0.5/fwadmin/models.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2162 2023-05-10 15:56:08.000000 fwadmin-0.0.5/fwadmin/navigation.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3050 2023-05-15 11:22:35.000000 fwadmin-0.0.5/fwadmin/tables.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     4035 2023-05-15 11:20:38.000000 fwadmin-0.0.5/fwadmin/tasks.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-16 09:04:54.622094 fwadmin-0.0.5/fwadmin/templates/
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-16 09:04:54.662095 fwadmin-0.0.5/fwadmin/templates/fwadmin/
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-16 09:04:54.666095 fwadmin-0.0.5/fwadmin/templates/fwadmin/buttons/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      402 2023-05-08 19:10:26.000000 fwadmin-0.0.5/fwadmin/templates/fwadmin/buttons/approve.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      399 2023-05-08 19:10:38.000000 fwadmin-0.0.5/fwadmin/templates/fwadmin/buttons/reject.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      412 2023-05-08 19:11:15.000000 fwadmin-0.0.5/fwadmin/templates/fwadmin/buttons/self_approve.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1495 2023-05-06 13:26:26.000000 fwadmin-0.0.5/fwadmin/templates/fwadmin/devicegroup.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2557 2023-05-10 10:35:53.000000 fwadmin-0.0.5/fwadmin/templates/fwadmin/dynamiclist.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1851 2023-05-15 11:15:29.000000 fwadmin-0.0.5/fwadmin/templates/fwadmin/firewall.html
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-16 09:04:54.666095 fwadmin-0.0.5/fwadmin/templates/fwadmin/htmx/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1250 2023-05-09 18:44:21.000000 fwadmin-0.0.5/fwadmin/templates/fwadmin/htmx/manage_form.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3169 2023-05-08 18:21:36.000000 fwadmin-0.0.5/fwadmin/templates/fwadmin/sessionrequest.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1381 2023-05-10 09:38:16.000000 fwadmin-0.0.5/fwadmin/templates/fwadmin/sessionrequest_bulk_manage.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1973 2023-05-10 10:43:02.000000 fwadmin-0.0.5/fwadmin/templates/fwadmin/sessionrequest_list.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      637 2023-05-08 18:50:35.000000 fwadmin-0.0.5/fwadmin/templates/fwadmin/sessionrequest_manage.html
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-16 09:04:54.666095 fwadmin-0.0.5/fwadmin/templatetags/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-05-10 15:56:08.000000 fwadmin-0.0.5/fwadmin/templatetags/__init__.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-16 09:04:54.666095 fwadmin-0.0.5/fwadmin/templatetags/__pycache__/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      150 2023-05-13 15:47:23.000000 fwadmin-0.0.5/fwadmin/templatetags/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1284 2023-05-13 15:47:23.000000 fwadmin-0.0.5/fwadmin/templatetags/__pycache__/fwadmin_buttons.cpython-310.pyc
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1048 2023-05-05 06:16:08.000000 fwadmin-0.0.5/fwadmin/templatetags/__pycache__/netdoc_buttons.cpython-310.pyc
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1203 2023-05-10 15:56:08.000000 fwadmin-0.0.5/fwadmin/templatetags/fwadmin_buttons.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-16 09:04:54.666095 fwadmin-0.0.5/fwadmin/tests/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-05-13 12:37:53.000000 fwadmin-0.0.5/fwadmin/tests/__init__.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    19973 2023-05-15 12:57:10.000000 fwadmin-0.0.5/fwadmin/tests/test.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3980 2023-05-10 15:56:08.000000 fwadmin-0.0.5/fwadmin/urls.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    16783 2023-05-15 11:18:48.000000 fwadmin-0.0.5/fwadmin/views.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1006 2023-05-10 15:56:08.000000 fwadmin-0.0.5/fwadmin/workflows.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-05-16 09:04:54.634094 fwadmin-0.0.5/fwadmin.egg-info/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      477 2023-05-16 09:04:54.000000 fwadmin-0.0.5/fwadmin.egg-info/PKG-INFO
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1778 2023-05-16 09:04:54.000000 fwadmin-0.0.5/fwadmin.egg-info/SOURCES.txt
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        1 2023-05-16 09:04:54.000000 fwadmin-0.0.5/fwadmin.egg-info/dependency_links.txt
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        1 2023-05-05 14:55:33.000000 fwadmin-0.0.5/fwadmin.egg-info/not-zip-safe
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        9 2023-05-16 09:04:54.000000 fwadmin-0.0.5/fwadmin.egg-info/requires.txt
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        8 2023-05-16 09:04:54.000000 fwadmin-0.0.5/fwadmin.egg-info/top_level.txt
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      103 2023-05-16 09:04:54.670095 fwadmin-0.0.5/setup.cfg
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1059 2023-05-16 09:04:53.000000 fwadmin-0.0.5/setup.py
```

### Comparing `fwadmin-0.0.3/LICENSE` & `fwadmin-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fwadmin-0.0.3/README.md` & `fwadmin-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `fwadmin-0.0.3/fwadmin/api/serializers.py` & `fwadmin-0.0.5/fwadmin/api/serializers.py`

 * *Files identical despite different names*

### Comparing `fwadmin-0.0.3/fwadmin/api/urls.py` & `fwadmin-0.0.5/fwadmin/api/urls.py`

 * *Files identical despite different names*

### Comparing `fwadmin-0.0.3/fwadmin/api/views.py` & `fwadmin-0.0.5/fwadmin/api/views.py`

 * *Files identical despite different names*

### Comparing `fwadmin-0.0.3/fwadmin/filtersets.py` & `fwadmin-0.0.5/fwadmin/filtersets.py`

 * *Files identical despite different names*

### Comparing `fwadmin-0.0.3/fwadmin/forms.py` & `fwadmin-0.0.5/fwadmin/forms.py`

 * *Files identical despite different names*

### Comparing `fwadmin-0.0.3/fwadmin/migrations/0001_initial.py` & `fwadmin-0.0.5/fwadmin/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `fwadmin-0.0.3/fwadmin/migrations/0003_sessionrequest_authorized_by_and_more.py` & `fwadmin-0.0.5/fwadmin/migrations/0003_sessionrequest_authorized_by_and_more.py`

 * *Files identical despite different names*

### Comparing `fwadmin-0.0.3/fwadmin/migrations/0004_remove_sessionrequest_action_reason_and_more.py` & `fwadmin-0.0.5/fwadmin/migrations/0004_remove_sessionrequest_action_reason_and_more.py`

 * *Files identical despite different names*

### Comparing `fwadmin-0.0.3/fwadmin/migrations/0005_rename_approved_by_sessionrequest_managed_by_and_more.py` & `fwadmin-0.0.5/fwadmin/migrations/0005_rename_approved_by_sessionrequest_managed_by_and_more.py`

 * *Files identical despite different names*

### Comparing `fwadmin-0.0.3/fwadmin/models.py` & `fwadmin-0.0.5/fwadmin/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Models (ORM).
 
-Define ORM models for NetDoc objects:
+Define ORM models for FWAdmin objects:
 * A Discoverable is a device willed to be discovered using a specific mode.
 * Credential is associated to one or more Discoverables.
 * A DiscoveryLog is the output for a specific discovery command executed in a Discoverable.
 """
 __author__ = "Andrea Dainese"
 __contact__ = "andrea@adainese.it"
 __copyright__ = "Copyright 2022, Andrea Dainese"
```

### Comparing `fwadmin-0.0.3/fwadmin/navigation.py` & `fwadmin-0.0.5/fwadmin/navigation.py`

 * *Files identical despite different names*

### Comparing `fwadmin-0.0.3/fwadmin/tables.py` & `fwadmin-0.0.5/fwadmin/tables.py`

 * *Files 4% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 
 class SessionRequestTable(NetBoxTable):
     """SessionRequest list table used in SessionRequestlView."""
 
     name = tables.Column(linkify=True)
     model = ChoiceFieldColumn()
     dynamiclist_count = tables.Column()
-    # TODO: boolean to see if session is alive
+    is_active = tables.BooleanColumn()
     actions = []
 
     class Meta(NetBoxTable.Meta):
         """Table metadata."""
 
         model = models.SessionRequest
         fields = [
@@ -114,18 +114,20 @@
             "managed_by",
             "status",
             "start_at",
             "end_at",
             "cleared",
             "last_updated",
             "created",
+            "is_active",
             "request_reason",
         ]
         default_columns = [
             "id",
             "requested_by",
             "managed_by",
             "status",
             "start_at",
             "end_at",
+            "is_active",
             "request_reason",
         ]
```

### Comparing `fwadmin-0.0.3/fwadmin/templates/fwadmin/devicegroup.html` & `fwadmin-0.0.5/fwadmin/templates/fwadmin/devicegroup.html`

 * *Files identical despite different names*

### Comparing `fwadmin-0.0.3/fwadmin/templates/fwadmin/dynamiclist.html` & `fwadmin-0.0.5/fwadmin/templates/fwadmin/dynamiclist.html`

 * *Files identical despite different names*

### Comparing `fwadmin-0.0.3/fwadmin/templates/fwadmin/firewall.html` & `fwadmin-0.0.5/fwadmin/templates/fwadmin/firewall.html`

 * *Files 2% similar despite different names*

```diff
@@ -39,12 +39,12 @@
             {% include "inc/panels/comments.html" %}
         </div>
     </div>
     <div class="row">
         <div class="col col-md-12">
             <div class="card">
                 <h5 class="card-header">Dynamic lists</h5>
-                <div class="card-body table-responsive">render_table discoverables_table TODO</div>
+                <div class="card-body table-responsive">{% render_table dynamiclist_table %}</div>
             </div>
         </div>
     </div>
 {% endblock content %}
```

#### html2text {}

```diff
@@ -6,9 +6,9 @@
 Name                  {{ object.name }}
 Address               {{ object.address }}
 Model                 {{ object.model }}
 Dynamic lists (count) {{ object.dynamiclist_count }}
 {% include "inc/panels/custom_fields.html" %}
 {% include "inc/panels/tags.html" %} {% include "inc/panels/comments.html" %}
 ** Dynamic lists **
-render_table discoverables_table TODO
+{% render_table dynamiclist_table %}
 {% endblock content %}
```

### Comparing `fwadmin-0.0.3/fwadmin/templates/fwadmin/htmx/manage_form.html` & `fwadmin-0.0.5/fwadmin/templates/fwadmin/htmx/manage_form.html`

 * *Files identical despite different names*

### Comparing `fwadmin-0.0.3/fwadmin/templates/fwadmin/sessionrequest.html` & `fwadmin-0.0.5/fwadmin/templates/fwadmin/sessionrequest.html`

 * *Files identical despite different names*

### Comparing `fwadmin-0.0.3/fwadmin/templates/fwadmin/sessionrequest_bulk_manage.html` & `fwadmin-0.0.5/fwadmin/templates/fwadmin/sessionrequest_bulk_manage.html`

 * *Files identical despite different names*

### Comparing `fwadmin-0.0.3/fwadmin/templates/fwadmin/sessionrequest_list.html` & `fwadmin-0.0.5/fwadmin/templates/fwadmin/sessionrequest_list.html`

 * *Files identical despite different names*

### Comparing `fwadmin-0.0.3/fwadmin/templates/fwadmin/sessionrequest_manage.html` & `fwadmin-0.0.5/fwadmin/templates/fwadmin/sessionrequest_manage.html`

 * *Files identical despite different names*

### Comparing `fwadmin-0.0.3/fwadmin/templatetags/__pycache__/fwadmin_buttons.cpython-310.pyc` & `fwadmin-0.0.5/fwadmin/templatetags/__pycache__/fwadmin_buttons.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed May 10 09:28:30 2023 UTC, .py size: 1203 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 be63 5b64 b304 0000  o........c[d....
+00000000: 6f0d 0d0a 0000 0000 98be 5b64 b304 0000  o.........[d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 7a00 0000 6400  .....@...sz...d.
 00000030: 5a00 6401 5a01 6402 5a02 6403 5a03 6404  Z.d.Z.d.Z.d.Z.d.
 00000040: 5a04 6405 6406 6c05 6d06 5a06 0100 6405  Z.d.d.l.m.Z...d.
 00000050: 6407 6c07 6d08 5a08 0100 6405 6408 6c09  d.l.m.Z...d.d.l.
 00000060: 6d0a 5a0a 0100 6506 a00b a100 5a0c 650c  m.Z...e.....Z.e.
 00000070: a00d 6409 a101 640a 640b 8400 8301 5a0e  ..d...d.d.....Z.
```

### Comparing `fwadmin-0.0.3/fwadmin/templatetags/__pycache__/netdoc_buttons.cpython-310.pyc` & `fwadmin-0.0.5/fwadmin/templatetags/__pycache__/netdoc_buttons.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fwadmin-0.0.3/fwadmin/templatetags/fwadmin_buttons.py` & `fwadmin-0.0.5/fwadmin/templatetags/fwadmin_buttons.py`

 * *Files identical despite different names*

### Comparing `fwadmin-0.0.3/fwadmin/urls.py` & `fwadmin-0.0.5/fwadmin/urls.py`

 * *Files identical despite different names*

### Comparing `fwadmin-0.0.3/fwadmin/views.py` & `fwadmin-0.0.5/fwadmin/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 __author__ = "Andrea Dainese"
 __contact__ = "andrea@adainese.it"
 __copyright__ = "Copyright 2022, Andrea Dainese"
 __license__ = "GPLv3"
 
 import logging
 
-from django.db.models import Count
+from django.db.models import Count, Q, BooleanField, ExpressionWrapper
 from django.contrib import messages
 from django.shortcuts import redirect, render
 from django.urls import reverse
 from django.utils import timezone
 from django.views import View
 from django.http import HttpResponse, HttpResponseNotFound
 
@@ -42,15 +42,15 @@
 
 class DeviceGroupView(generic.ObjectView):
     """Detailed DeviceGroup view."""
 
     queryset = models.DeviceGroup.objects.annotate(device_count=Count("devices"))
 
     def get_extra_context(self, request, instance):
-        """Get associated Device obhects."""
+        """Get associated Device objects."""
         table = DeviceTable(instance.devices.all().order_by("name"))
         table.configure(request)
 
         return {
             "device_table": table,
         }
 
@@ -97,15 +97,15 @@
     """Detailed DynamicList view."""
 
     queryset = models.DynamicList.objects.annotate(
         device_count=Count("device_groups__devices")
     )
 
     def get_extra_context(self, request, instance):
-        """Get associated DynamicList obhects."""
+        """Get associated Firewall objects."""
         firewall_table = tables.FirewallTable(instance.firewalls.all().order_by("name"))
         firewall_table.configure(request)
         devicegroup_table = tables.DeviceGroupTable(
             instance.device_groups.all().order_by("name")
         )
         devicegroup_table.configure(request)
 
@@ -139,14 +139,15 @@
 
 
 class DynamicListText(View):
     """Print the content of the EDL in text format."""
 
     def get(self, request, slug=None):  # pylint: disable=unused-argument
         """Get the content of the list in text/plain format."""
+        ip_list = []
         now = timezone.now()
 
         # Load the list
         try:
             dynamiclist_o = models.DynamicList.objects.get(slug=slug)
         except models.DynamicList.DoesNotExist:  # pylint: disable=no-member
             # List not found
@@ -169,18 +170,20 @@
             )
             ip_list = [
                 f"{ipaddress_o.ip}/32"
                 for ipaddress_o in IPAddress.objects.filter(
                     interface__in=interface_ids
                 ).values_list("address", flat=True)
             ]
-        else:
-            # No session request
+
+        if not ip_list:
+            # Empty IP list
             ip_list = ["0.0.0.0/32"]
 
+        ip_list.sort()
         return HttpResponse("\n".join(ip_list), content_type="text/plain")
 
 
 #
 # Firewall views
 #
 
@@ -198,14 +201,23 @@
 class FirewallView(generic.ObjectView):
     """Detailed Firewall view."""
 
     queryset = models.Firewall.objects.annotate(
         dynamiclist_count=Count("dynamic_lists")
     )
 
+    def get_extra_context(self, request, instance):
+        """Get associated DynamicList objects."""
+        table = tables.DynamicListTable(instance.dynamic_lists.all().order_by("name"))
+        table.configure(request)
+
+        return {
+            "dynamiclist_table": table,
+        }
+
 
 class FirewallEditView(generic.ObjectEditView):
     """Edit Firewall view."""
 
     queryset = models.Firewall.objects.all()
     form = forms.FirewallForm
 
@@ -230,15 +242,19 @@
 # SessionRequest views
 #
 
 
 class SessionRequestListView(generic.ObjectListView):
     """Summary view listing all SessionRequest objects."""
 
-    queryset = models.SessionRequest.objects.order_by("-id")
+    queryset = models.SessionRequest.objects.annotate(
+        is_active=ExpressionWrapper(
+            Q(end_at__gt=timezone.now()), output_field=BooleanField()
+        )
+    ).order_by("-id")
     table = tables.SessionRequestTable
     filterset = filtersets.SessionRequestFilterSet
     template_name = "fwadmin/sessionrequest_list.html"
     actions = [
         "add",
         "export",
         "bulk_approve",
```

### Comparing `fwadmin-0.0.3/fwadmin/workflows.py` & `fwadmin-0.0.5/fwadmin/workflows.py`

 * *Files identical despite different names*

### Comparing `fwadmin-0.0.3/fwadmin.egg-info/SOURCES.txt` & `fwadmin-0.0.5/fwadmin.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 fwadmin/api/urls.py
 fwadmin/api/views.py
 fwadmin/migrations/0001_initial.py
 fwadmin/migrations/0002_remove_sessionrequest_user_and_more.py
 fwadmin/migrations/0003_sessionrequest_authorized_by_and_more.py
 fwadmin/migrations/0004_remove_sessionrequest_action_reason_and_more.py
 fwadmin/migrations/0005_rename_approved_by_sessionrequest_managed_by_and_more.py
+fwadmin/migrations/0006_remove_firewall_access_key_firewall_verify_cert_and_more.py
 fwadmin/migrations/__init__.py
 fwadmin/templates/fwadmin/devicegroup.html
 fwadmin/templates/fwadmin/dynamiclist.html
 fwadmin/templates/fwadmin/firewall.html
 fwadmin/templates/fwadmin/sessionrequest.html
 fwadmin/templates/fwadmin/sessionrequest_bulk_manage.html
 fwadmin/templates/fwadmin/sessionrequest_list.html
@@ -40,8 +41,10 @@
 fwadmin/templates/fwadmin/buttons/reject.html
 fwadmin/templates/fwadmin/buttons/self_approve.html
 fwadmin/templates/fwadmin/htmx/manage_form.html
 fwadmin/templatetags/__init__.py
 fwadmin/templatetags/fwadmin_buttons.py
 fwadmin/templatetags/__pycache__/__init__.cpython-310.pyc
 fwadmin/templatetags/__pycache__/fwadmin_buttons.cpython-310.pyc
-fwadmin/templatetags/__pycache__/netdoc_buttons.cpython-310.pyc
+fwadmin/templatetags/__pycache__/netdoc_buttons.cpython-310.pyc
+fwadmin/tests/__init__.py
+fwadmin/tests/test.py
```

### Comparing `fwadmin-0.0.3/setup.py` & `fwadmin-0.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """
-NetDoc PYPI setup file.
+FWAdmin PYPI setup file.
 
 Install with: python3 setup.py install
 Develop with: python3 setup.py develop
 Make it available on PIP with:
     python3 setup.py sdist
     pip3 install twine
     twine upload dist/*
 """
 
 __author__ = "Andrea Dainese"
 __contact__ = "andrea@adainese.it"
 __copyright__ = "Copyright 2022, Andrea Dainese"
 __license__ = "GPLv3"
-__version__ = "0.0.3"
+__version__ = "0.0.5"
 
 from setuptools import find_packages, setup
 
 setup(
     name="fwadmin",
     version=__version__,
     description="Firewall manager and viewer plugin for Netbox",
```

