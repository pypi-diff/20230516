# Comparing `tmp/sloth-framework-0.1.4.tar.gz` & `tmp/sloth-framework-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sloth-framework-0.1.4.tar", last modified: Fri May 12 09:17:15 2023, max compression
+gzip compressed data, was "sloth-framework-0.1.5.tar", last modified: Mon May 15 21:57:26 2023, max compression
```

## Comparing `sloth-framework-0.1.4.tar` & `sloth-framework-0.1.5.tar`

### file list

```diff
@@ -1,299 +1,299 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.282873 sloth-framework-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-12 09:17:15.282873 sloth-framework-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 09:17:15.282873 sloth-framework-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.262873 sloth-framework-0.1.4/sloth/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.262873 sloth-framework-0.1.4/sloth/actions/
--rw-r--r--   0 runner    (1001) docker     (123)    38675 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/actions/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/actions/inputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.262873 sloth-framework-0.1.4/sloth/api/
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18627 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/actions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.262873 sloth-framework-0.1.4/sloth/api/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16195 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/dashboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.262873 sloth-framework-0.1.4/sloth/api/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.262873 sloth-framework-0.1.4/sloth/api/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.262873 sloth-framework-0.1.4/sloth/api/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/management/commands/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/management/commands/query.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/management/commands/reset_passwords.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/management/commands/selenium.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/management/commands/send_web_push_notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/management/commands/startserver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/management/commands/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/management/commands/sync_roles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.262873 sloth-framework-0.1.4/sloth/api/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/migrations/0002_role_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/migrations/0003_alter_application_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/migrations/0004_task.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/migrations/0005_task_stopped_alter_task_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/migrations/0006_role_active_alter_role_name_alter_role_scope_key_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/migrations/0007_alter_scope_description_alter_task_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/migrations/0008_alter_application_available_scopes_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/migrations/0009_pushnotification.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/migrations/0010_alter_pushnotification_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/migrations/0011_alter_application_client_secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/migrations/0012_authcode.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/migrations/0013_task_partial_task_total.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/migrations/0014_email.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11023 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.258872 sloth-framework-0.1.4/sloth/api/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.262873 sloth-framework-0.1.4/sloth/api/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)    58578 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/css/all.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    67289 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/css/bootstrap-icons.css
--rw-r--r--   0 runner    (1001) docker     (123)   155845 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/css/colorpick.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.266873 sloth-framework-0.1.4/sloth/api/static/css/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)   107280 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/css/fonts/Eina02-Bold.f8011405.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   116316 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/css/fonts/Eina02-Regular.2e682693.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   112880 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/css/fonts/Eina02-SemiBold.c5f9b8e3.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   111976 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/css/fonts/bootstrap-icons.woff
--rw-r--r--   0 runner    (1001) docker     (123)    83304 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/css/fonts/bootstrap-icons.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    30702 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/css/icons.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.266873 sloth-framework-0.1.4/sloth/api/static/css/images/
--rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/css/images/ui-icons_444444_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/css/images/ui-icons_555555_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)    35973 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/css/jquery-ui.css
--rw-r--r--   0 runner    (1001) docker     (123)    14670 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/css/leaflet.css
--rw-r--r--   0 runner    (1001) docker     (123)    16264 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/css/select2.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     9009 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/css/sloth.css
--rw-r--r--   0 runner    (1001) docker     (123)    17867 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/css/trumbowyg.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.258872 sloth-framework-0.1.4/sloth/api/static/icons/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.266873 sloth-framework-0.1.4/sloth/api/static/icons/fontawesome/
--rw-r--r--   0 runner    (1001) docker     (123)   100170 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/icons/fontawesome/fontawesome.min.css
--rw-r--r--   0 runner    (1001) docker     (123)  1726692 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/icons/fontawesome/fontawesome.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.266873 sloth-framework-0.1.4/sloth/api/static/icons/fontawesome/webfonts/
--rw-r--r--   0 runner    (1001) docker     (123)   181852 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   105536 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    60520 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    23940 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    10556 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.270872 sloth-framework-0.1.4/sloth/api/static/icons/materialicons/
--rw-r--r--   0 runner    (1001) docker     (123)   174176 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/icons/materialicons/LDItaoyNOAY6Uewc665JcIzCKsKc_M9flwmPq_HTTw.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   127220 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/icons/materialicons/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   155604 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/icons/materialicons/gok-H7zzDkdnRel8-DQ6KAXJ69wP1tGnf4ZGhUcel5euIg.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/icons/materialicons/materialicons.css
--rw-r--r--   0 runner    (1001) docker     (123)   135988 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/icons/materialicons/oPWQ_lt5nv4pWNJpghLP75WiFR4kLh3kvmvRImcycg.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.270872 sloth-framework-0.1.4/sloth/api/static/images/
--rw-r--r--   0 runner    (1001) docker     (123)    57420 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/images/click.png
--rw-r--r--   0 runner    (1001) docker     (123)    55448 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/images/hand.png
--rw-r--r--   0 runner    (1001) docker     (123)    10276 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/images/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/images/icon.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.270872 sloth-framework-0.1.4/sloth/api/static/images/images/
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/images/images/badge.png
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/images/images/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)    45136 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/images/login.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)    22817 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/images/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    21495 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/images/no-image.png
--rw-r--r--   0 runner    (1001) docker     (123)    23102 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/images/sloth.png
--rw-r--r--   0 runner    (1001) docker     (123)    13670 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/images/user.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.270872 sloth-framework-0.1.4/sloth/api/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/js/api.js
--rw-r--r--   0 runner    (1001) docker     (123)    78743 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/js/bootstrap.bundle.min.js
--rwxr-xr-x   0 runner    (1001) docker     (123)     4098 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/js/colorpick.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.270872 sloth-framework-0.1.4/sloth/api/static/js/i18n/
--rwxr-xr-x   0 runner    (1001) docker     (123)      853 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/js/i18n/pt-BR.js
--rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/js/jquery-3.6.0.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   520714 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/js/jquery-ui.js
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/js/jquery.binarytransport.js
--rw-r--r--   0 runner    (1001) docker     (123)     8327 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/js/jquery.mask.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    80794 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/js/jquery.timepicker.js
--rw-r--r--   0 runner    (1001) docker     (123)   147555 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/js/leaflet.js
--rw-r--r--   0 runner    (1001) docker     (123)    24103 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/js/masonry.pkgd.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    18453 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/js/popper.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    43994 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/js/qr-scanner-worker.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    15538 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/js/qr-scanner.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    19927 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/js/qrcode.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    73163 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/js/select2.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    16580 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/js/sloth.js
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/js/sw.js
--rw-r--r--   0 runner    (1001) docker     (123)    10702 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/js/tests.js
--rw-r--r--   0 runner    (1001) docker     (123)    28280 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/js/trumbowyg.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/js/wpn.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.270872 sloth-framework-0.1.4/sloth/api/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/tasks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.258872 sloth-framework-0.1.4/sloth/api/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.274872 sloth-framework-0.1.4/sloth/api/templates/actions/
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/actions/execute_query.html
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/actions/execute_script.html
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/actions/show_icons.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.274872 sloth-framework-0.1.4/sloth/api/templates/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/api/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.274872 sloth-framework-0.1.4/sloth/api/templates/charts/
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/charts/bar.html
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/charts/column.html
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/charts/donut.html
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/charts/legend.html
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/charts/pie.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.274872 sloth-framework-0.1.4/sloth/api/templates/dashboard/
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/dashboard/actions.html
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/dashboard/apps.html
--rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/dashboard/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/dashboard/bottom.html
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/dashboard/cards.html
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/dashboard/dashboards.html
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/dashboard/default.html
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/dashboard/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/dashboard/form.html
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/dashboard/grids.html
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/dashboard/header.html
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/dashboard/links.html
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/dashboard/menu.html
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/dashboard/messages.html
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/dashboard/modal.html
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/dashboard/plus.html
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/dashboard/report.html
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/dashboard/search.html
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/dashboard/settings.html
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/dashboard/shortcuts.html
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/dashboard/tasks.html
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/dashboard/tools.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.274872 sloth-framework-0.1.4/sloth/api/templates/inputs/
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/inputs/picker.html
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/inputs/qrcode.html
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/inputs/select.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.274872 sloth-framework-0.1.4/sloth/api/templates/queryset/
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/queryset/accordion.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.274872 sloth-framework-0.1.4/sloth/api/templates/queryset/actions/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/queryset/actions/actions.html
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/queryset/actions/batch.html
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/queryset/actions/global.html
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/queryset/calendar.html
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/queryset/cards.html
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/queryset/checkbox.html
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/queryset/datatable.html
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/queryset/filter.html
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/queryset/filters.html
--rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/queryset/queryset.html
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/queryset/rows.html
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/queryset/scroll.html
--rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/queryset/statistics.html
--rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/queryset/timeline.html
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/queryset/tree.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.258872 sloth-framework-0.1.4/sloth/api/templates/renderers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.274872 sloth-framework-0.1.4/sloth/api/templates/renderers/badges/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/badges/badge.html
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/badges/boolean.html
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/badges/danger.html
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/badges/primary.html
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/badges/status.html
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/badges/warning.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.274872 sloth-framework-0.1.4/sloth/api/templates/renderers/boolean/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/boolean/thumb.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.278873 sloth-framework-0.1.4/sloth/api/templates/renderers/calendar/
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/calendar/calendar.html
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/calendar/events.html
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/calendar/legend.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.278873 sloth-framework-0.1.4/sloth/api/templates/renderers/documents/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/documents/document.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.278873 sloth-framework-0.1.4/sloth/api/templates/renderers/images/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/images/banner.html
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/images/group.html
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/images/image.html
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/images/round.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.278873 sloth-framework-0.1.4/sloth/api/templates/renderers/links/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/links/file.html
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/links/url.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.278873 sloth-framework-0.1.4/sloth/api/templates/renderers/maps/
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/maps/geolocation.html
--rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/maps/map.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.278873 sloth-framework-0.1.4/sloth/api/templates/renderers/messages/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/messages/custom.html
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/messages/danger.html
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/messages/message.html
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/messages/primary.html
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/messages/success.html
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/messages/warning.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.278873 sloth-framework-0.1.4/sloth/api/templates/renderers/photos/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/photos/photo.html
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/photos/round.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.278873 sloth-framework-0.1.4/sloth/api/templates/renderers/programing/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/programing/strtable.html
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/programing/terminal.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.278873 sloth-framework-0.1.4/sloth/api/templates/renderers/progress/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/progress/primary.html
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/progress/success.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.278873 sloth-framework-0.1.4/sloth/api/templates/renderers/tags/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/tags/primary.html
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/tags/tags.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.278873 sloth-framework-0.1.4/sloth/api/templates/renderers/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/utils/formatted.html
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/utils/progress.html
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/utils/qrcode.html
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/utils/steps.html
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/utils/table.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.278873 sloth-framework-0.1.4/sloth/api/templates/themes/
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/themes/dark.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.278873 sloth-framework-0.1.4/sloth/api/templates/valueset/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/valueset/2-column.html
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/valueset/field.html
--rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/valueset/fieldset-group.html
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/valueset/fieldset-list.html
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/valueset/fieldset-tab.html
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/valueset/fieldset.html
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/valueset/primitive.html
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/valueset/value.html
--rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/valueset/valueset.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.278873 sloth-framework-0.1.4/sloth/api/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9090 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templatetags/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    11431 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.278873 sloth-framework-0.1.4/sloth/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/cloud/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      688 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/cloud/printer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6116 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/cloud/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.278873 sloth-framework-0.1.4/sloth/conf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/conf/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.278873 sloth-framework-0.1.4/sloth/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21661 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    41705 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/core/queryset.py
--rw-r--r--   0 runner    (1001) docker     (123)    11540 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/core/statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/core/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    20156 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/core/valueset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.278873 sloth-framework-0.1.4/sloth/db/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.282873 sloth-framework-0.1.4/sloth/db/models/
--rw-r--r--   0 runner    (1001) docker     (123)    10004 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/db/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.282873 sloth-framework-0.1.4/sloth/test/
--rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.282873 sloth-framework-0.1.4/sloth/test/selenium/
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/test/selenium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10057 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/test/selenium/browser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.282873 sloth-framework-0.1.4/sloth/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.282873 sloth-framework-0.1.4/sloth/utils/formatter/
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/utils/formatter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.282873 sloth-framework-0.1.4/sloth/utils/http/
--rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/utils/http/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.282873 sloth-framework-0.1.4/sloth/utils/icons/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/utils/icons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28753 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/utils/icons/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)    53105 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/utils/icons/fontawesome.py
--rw-r--r--   0 runner    (1001) docker     (123)    20959 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/utils/icons/materialicons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.282873 sloth-framework-0.1.4/sloth/utils/log/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/utils/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/utils/log/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.282873 sloth-framework-0.1.4/sloth_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-12 09:17:15.000000 sloth-framework-0.1.4/sloth_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9734 2023-05-12 09:17:15.000000 sloth-framework-0.1.4/sloth_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 09:17:15.000000 sloth-framework-0.1.4/sloth_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-12 09:17:15.000000 sloth-framework-0.1.4/sloth_framework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-12 09:17:15.000000 sloth-framework-0.1.4/sloth_framework.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.364170 sloth-framework-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-15 21:57:26.364170 sloth-framework-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 21:57:26.364170 sloth-framework-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.336169 sloth-framework-0.1.5/sloth/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.336169 sloth-framework-0.1.5/sloth/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)    39352 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/actions/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/actions/inputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.340170 sloth-framework-0.1.5/sloth/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18627 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/actions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.340170 sloth-framework-0.1.5/sloth/api/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16195 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/dashboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.340170 sloth-framework-0.1.5/sloth/api/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.340170 sloth-framework-0.1.5/sloth/api/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.340170 sloth-framework-0.1.5/sloth/api/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/management/commands/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/management/commands/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/management/commands/reset_passwords.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/management/commands/selenium.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/management/commands/send_web_push_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/management/commands/startserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/management/commands/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/management/commands/sync_roles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.340170 sloth-framework-0.1.5/sloth/api/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/migrations/0002_role_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/migrations/0003_alter_application_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/migrations/0004_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/migrations/0005_task_stopped_alter_task_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/migrations/0006_role_active_alter_role_name_alter_role_scope_key_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/migrations/0007_alter_scope_description_alter_task_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/migrations/0008_alter_application_available_scopes_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/migrations/0009_pushnotification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/migrations/0010_alter_pushnotification_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/migrations/0011_alter_application_client_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/migrations/0012_authcode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/migrations/0013_task_partial_task_total.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/migrations/0014_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11023 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.336169 sloth-framework-0.1.5/sloth/api/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.344169 sloth-framework-0.1.5/sloth/api/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    58578 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/css/all.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    67289 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/css/bootstrap-icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)   155845 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/css/colorpick.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.344169 sloth-framework-0.1.5/sloth/api/static/css/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   107280 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/css/fonts/Eina02-Bold.f8011405.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   116316 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/css/fonts/Eina02-Regular.2e682693.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   112880 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/css/fonts/Eina02-SemiBold.c5f9b8e3.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   111976 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/css/fonts/bootstrap-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    83304 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/css/fonts/bootstrap-icons.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    30702 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/css/icons.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.344169 sloth-framework-0.1.5/sloth/api/static/css/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/css/images/ui-icons_444444_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/css/images/ui-icons_555555_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)    35973 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/css/jquery-ui.css
+-rw-r--r--   0 runner    (1001) docker     (123)    14670 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/css/leaflet.css
+-rw-r--r--   0 runner    (1001) docker     (123)    16264 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/css/select2.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     9009 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/css/sloth.css
+-rw-r--r--   0 runner    (1001) docker     (123)    17867 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/css/trumbowyg.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.336169 sloth-framework-0.1.5/sloth/api/static/icons/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.344169 sloth-framework-0.1.5/sloth/api/static/icons/fontawesome/
+-rw-r--r--   0 runner    (1001) docker     (123)   100170 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/icons/fontawesome/fontawesome.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)  1726692 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/icons/fontawesome/fontawesome.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.348169 sloth-framework-0.1.5/sloth/api/static/icons/fontawesome/webfonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   181852 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   105536 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    60520 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    23940 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    10556 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.348169 sloth-framework-0.1.5/sloth/api/static/icons/materialicons/
+-rw-r--r--   0 runner    (1001) docker     (123)   174176 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/icons/materialicons/LDItaoyNOAY6Uewc665JcIzCKsKc_M9flwmPq_HTTw.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   127220 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/icons/materialicons/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   155604 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/icons/materialicons/gok-H7zzDkdnRel8-DQ6KAXJ69wP1tGnf4ZGhUcel5euIg.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/icons/materialicons/materialicons.css
+-rw-r--r--   0 runner    (1001) docker     (123)   135988 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/icons/materialicons/oPWQ_lt5nv4pWNJpghLP75WiFR4kLh3kvmvRImcycg.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.348169 sloth-framework-0.1.5/sloth/api/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    57420 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/images/click.png
+-rw-r--r--   0 runner    (1001) docker     (123)    55448 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/images/hand.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10276 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/images/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/images/icon.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.348169 sloth-framework-0.1.5/sloth/api/static/images/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/images/images/badge.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/images/images/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    45136 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/images/login.jpeg
+-rw-r--r--   0 runner    (1001) docker     (123)    22817 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/images/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    21495 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/images/no-image.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23102 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/images/sloth.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13670 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/images/user.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.352170 sloth-framework-0.1.5/sloth/api/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/js/api.js
+-rw-r--r--   0 runner    (1001) docker     (123)    78743 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/js/bootstrap.bundle.min.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4098 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/js/colorpick.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.352170 sloth-framework-0.1.5/sloth/api/static/js/i18n/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      853 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/js/i18n/pt-BR.js
+-rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/js/jquery-3.6.0.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   520714 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/js/jquery-ui.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/js/jquery.binarytransport.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8327 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/js/jquery.mask.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    80794 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/js/jquery.timepicker.js
+-rw-r--r--   0 runner    (1001) docker     (123)   147555 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/js/leaflet.js
+-rw-r--r--   0 runner    (1001) docker     (123)    24103 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/js/masonry.pkgd.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18453 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/js/popper.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    43994 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/js/qr-scanner-worker.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15538 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/js/qr-scanner.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    19927 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/js/qrcode.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    73163 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/js/select2.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16580 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/js/sloth.js
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/js/sw.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10852 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/js/tests.js
+-rw-r--r--   0 runner    (1001) docker     (123)    28280 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/js/trumbowyg.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/static/js/wpn.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.352170 sloth-framework-0.1.5/sloth/api/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/tasks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.336169 sloth-framework-0.1.5/sloth/api/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.352170 sloth-framework-0.1.5/sloth/api/templates/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/actions/execute_query.html
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/actions/execute_script.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/actions/show_icons.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.352170 sloth-framework-0.1.5/sloth/api/templates/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/api/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.352170 sloth-framework-0.1.5/sloth/api/templates/charts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/charts/bar.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/charts/column.html
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/charts/donut.html
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/charts/legend.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/charts/pie.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.356170 sloth-framework-0.1.5/sloth/api/templates/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/dashboard/actions.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/dashboard/apps.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/dashboard/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/dashboard/bottom.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/dashboard/cards.html
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/dashboard/dashboards.html
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/dashboard/default.html
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/dashboard/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/dashboard/form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/dashboard/grids.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/dashboard/header.html
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/dashboard/links.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/dashboard/menu.html
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/dashboard/messages.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/dashboard/modal.html
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/dashboard/plus.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/dashboard/report.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/dashboard/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/dashboard/settings.html
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/dashboard/shortcuts.html
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/dashboard/tasks.html
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/dashboard/tools.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.356170 sloth-framework-0.1.5/sloth/api/templates/inputs/
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/inputs/picker.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/inputs/qrcode.html
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/inputs/select.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.356170 sloth-framework-0.1.5/sloth/api/templates/queryset/
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/queryset/accordion.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.356170 sloth-framework-0.1.5/sloth/api/templates/queryset/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/queryset/actions/actions.html
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/queryset/actions/batch.html
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/queryset/actions/global.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/queryset/calendar.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/queryset/cards.html
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/queryset/checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/queryset/datatable.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/queryset/filter.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/queryset/filters.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/queryset/queryset.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/queryset/rows.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/queryset/scroll.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/queryset/statistics.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/queryset/timeline.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/queryset/tree.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.336169 sloth-framework-0.1.5/sloth/api/templates/renderers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.356170 sloth-framework-0.1.5/sloth/api/templates/renderers/badges/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/badges/badge.html
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/badges/boolean.html
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/badges/danger.html
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/badges/primary.html
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/badges/status.html
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/badges/warning.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.356170 sloth-framework-0.1.5/sloth/api/templates/renderers/boolean/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/boolean/thumb.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.356170 sloth-framework-0.1.5/sloth/api/templates/renderers/calendar/
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/calendar/calendar.html
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/calendar/events.html
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/calendar/legend.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.356170 sloth-framework-0.1.5/sloth/api/templates/renderers/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/documents/document.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.356170 sloth-framework-0.1.5/sloth/api/templates/renderers/images/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/images/banner.html
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/images/group.html
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/images/image.html
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/images/round.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.356170 sloth-framework-0.1.5/sloth/api/templates/renderers/links/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/links/file.html
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/links/url.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.356170 sloth-framework-0.1.5/sloth/api/templates/renderers/maps/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/maps/geolocation.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/maps/map.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.360170 sloth-framework-0.1.5/sloth/api/templates/renderers/messages/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/messages/custom.html
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/messages/danger.html
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/messages/message.html
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/messages/primary.html
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/messages/success.html
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/messages/warning.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.360170 sloth-framework-0.1.5/sloth/api/templates/renderers/photos/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/photos/photo.html
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/photos/round.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.360170 sloth-framework-0.1.5/sloth/api/templates/renderers/programing/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/programing/strtable.html
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/programing/terminal.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.360170 sloth-framework-0.1.5/sloth/api/templates/renderers/progress/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/progress/primary.html
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/progress/success.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.360170 sloth-framework-0.1.5/sloth/api/templates/renderers/tags/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/tags/primary.html
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/tags/tags.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.360170 sloth-framework-0.1.5/sloth/api/templates/renderers/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/utils/formatted.html
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/utils/progress.html
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/utils/qrcode.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/utils/steps.html
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/renderers/utils/table.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.360170 sloth-framework-0.1.5/sloth/api/templates/themes/
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/themes/dark.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.360170 sloth-framework-0.1.5/sloth/api/templates/valueset/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/valueset/2-column.html
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/valueset/field.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/valueset/fieldset-group.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/valueset/fieldset-list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/valueset/fieldset-tab.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/valueset/fieldset.html
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/valueset/primitive.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/valueset/value.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6265 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templates/valueset/valueset.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.360170 sloth-framework-0.1.5/sloth/api/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9090 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/templatetags/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11965 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/api/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.360170 sloth-framework-0.1.5/sloth/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/cloud/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      688 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/cloud/printer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6116 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/cloud/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.360170 sloth-framework-0.1.5/sloth/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/conf/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.360170 sloth-framework-0.1.5/sloth/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21661 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42845 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/core/queryset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11540 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/core/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/core/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20797 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/core/valueset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.360170 sloth-framework-0.1.5/sloth/db/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.360170 sloth-framework-0.1.5/sloth/db/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    12155 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/db/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.360170 sloth-framework-0.1.5/sloth/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.360170 sloth-framework-0.1.5/sloth/test/selenium/
+-rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/test/selenium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10656 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/test/selenium/browser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.360170 sloth-framework-0.1.5/sloth/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.360170 sloth-framework-0.1.5/sloth/utils/formatter/
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/utils/formatter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.360170 sloth-framework-0.1.5/sloth/utils/http/
+-rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/utils/http/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.364170 sloth-framework-0.1.5/sloth/utils/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/utils/icons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28753 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/utils/icons/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53105 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/utils/icons/fontawesome.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20959 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/utils/icons/materialicons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.364170 sloth-framework-0.1.5/sloth/utils/log/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/utils/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-15 21:57:20.000000 sloth-framework-0.1.5/sloth/utils/log/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:57:26.364170 sloth-framework-0.1.5/sloth_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-15 21:57:26.000000 sloth-framework-0.1.5/sloth_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9734 2023-05-15 21:57:26.000000 sloth-framework-0.1.5/sloth_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 21:57:26.000000 sloth-framework-0.1.5/sloth_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-15 21:57:26.000000 sloth-framework-0.1.5/sloth_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-15 21:57:26.000000 sloth-framework-0.1.5/sloth_framework.egg-info/top_level.txt
```

### Comparing `sloth-framework-0.1.4/PKG-INFO` & `sloth-framework-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sloth-framework
-Version: 0.1.4
+Version: 0.1.5
 Summary: Metadata-based web framework for the development of management information systems
 Home-page: http://sloth.aplicativo.click/
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `sloth-framework-0.1.4/setup.py` & `sloth-framework-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 with open(os.path.join(root_dir, 'sloth/requirements.txt')) as file:
     requirements = file.read().strip().splitlines()
 
 os.chdir(root_dir)
 
 setup(
     name='sloth-framework',
-    version='0.1.4',
+    version='0.1.5',
     packages=find_packages(),
     install_requires=requirements,
     extras_require={
         'dev': [],
         'production': [],
     },
     include_package_data=True,
```

### Comparing `sloth-framework-0.1.4/sloth/Dockerfile` & `sloth-framework-0.1.5/sloth/Dockerfile`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/__init__.py` & `sloth-framework-0.1.5/sloth/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-
+from threading import local
 from django.apps import apps
 from django.conf import settings
 from django.db import models
 from django.db.models import options
 from django.db.models import manager
 from django.db.models.base import ModelBase
 
@@ -15,14 +15,16 @@
 # file_name = os.path.join(os.path.dirname(__file__), 'app', 'static', 'icons', 'fontawesome', 'fontawesome.min.js')
 # if not os.path.exists(file_name):
 #     with zipfile.ZipFile('{}.zip'.format(file_name), 'r') as file:
 #         file.extractall(os.path.dirname(file_name))
 
 PROXIED_MODELS = []
 
+threadlocals = local()
+
 
 class RoleLookup:
     def __init__(self, instance):
         self.instance = instance
         self.lookups = []
 
     def role_lookups(self, *names, **scopes):
@@ -122,9 +124,9 @@
 
 
 ModelBase.__new__ = __new__
 models.QuerySet = QuerySet
 models.Manager = Manager
 
 setattr(options, 'DEFAULT_NAMES', options.DEFAULT_NAMES + (
-    'icon', 'fieldsets', 'edit_fieldsets', 'select_template', 'select_fields', 'search_fields', 'autouser'
+    'icon', 'fieldsets', 'edit_fieldsets', 'select_template', 'select_fields', 'search_fields', 'autouser', 'logging'
 ))
```

### Comparing `sloth-framework-0.1.4/sloth/__main__.py` & `sloth-framework-0.1.5/sloth/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -125,27 +125,35 @@
 docker-compose.yml
 Dockerfile
 static
 media
 *.pyc
 *.sqlite3
 *.md
+local_settings.py
+'''
+
+REQUIREMENTS = '''
+sloth-framework
 '''
 
 def startproject():
     name = os.path.basename(os.path.abspath('.'))
     ManagementUtility(['django-admin.py', 'startproject', name, '.']).execute()
     settings_path = os.path.join(name, 'settings.py')
     settings_content = open(settings_path).read().replace(
         "'django.contrib.admin'",
         "'{}', 'oauth2_provider', 'sloth.api'".format(name)
     ).replace('from pathlib', 'import os\nfrom pathlib')
     settings_append = open(settings.__file__).read().replace('import os', '').replace('# ', '')
     with open(settings_path, 'w') as file:
         file.write('{}{}'.format(settings_content, settings_append))
+    local_settings_path = os.path.join(name, 'local_settings.py')
+    with open(local_settings_path, 'w') as file:
+        file.write('')
     urls_path = os.path.join(name, 'urls.py')
     with open(urls_path, 'w') as file:
         file.write(URLS_FILE_CONTENT)
     models_path = os.path.join(name, 'models.py')
     with open(models_path, 'w') as file:
         file.write(MODELS_FILE_CONTENT)
     actions_path = os.path.join(name, 'actions.py')
@@ -158,27 +166,29 @@
     with open(dashboard_path, 'w') as file:
         file.write(DASHBOARD_FILE_CONTENT)
     workflows_path = os.path.join('.github', 'workflows')
     os.makedirs(workflows_path, exist_ok=True)
     deploy_workflow_path = os.path.join(workflows_path, 'deploy.yml')
     with open(deploy_workflow_path, 'w') as file:
         file.write(DEPLOY_WORKFLOW_CONTENT)
-    ignore = ['bin/server.log', '.idea/', 'db.sqlite3', '*.pyc', '.DS_Store', 'geckodriver.log', '.docker', 'media']
+    ignore = ['bin/server.log', '.idea/', 'db.sqlite3', '*.pyc', '.DS_Store', 'geckodriver.log', '.docker', 'media', 'local_settings.py']
     if os.path.exists('.gitignore'):
         with open('.gitignore', 'a') as file:
             file.write('\n'.join(ignore))
     else:
         with open('.gitignore', 'w') as file:
             file.write('\n'.join(ignore))
     with open('Dockerfile', 'w') as file:
         file.write(DOCKER_FILE_CONTENT.format(name))
     with open('docker-compose.yml', 'w') as file:
         file.write(DOCKER_COMPOSE_FILE_CONTENT)
     with open('.dockerignore', 'w') as file:
         file.write(DOCKER_IGNORE_FILE_CONTENT)
+    with open('requirements.txt', 'w') as file:
+        file.write(REQUIREMENTS)
 
 
 if __name__ == "__main__":
     if len(sys.argv) == 1:
         startproject()
         os.system('python3 manage.py sync')
     if len(sys.argv) == 2:
```

### Comparing `sloth-framework-0.1.4/sloth/actions/__init__.py` & `sloth-framework-0.1.5/sloth/actions/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -541,20 +541,20 @@
         )
         return metadata
 
     def get_method(self):
         return getattr(self.metaclass, 'method', 'post') if hasattr(self, 'Meta') else 'post'
 
     def get_instances(self):
-        if self.instance:
-            return type(self.instance).objects.filter(pk=self.instance.pk)
-        elif self.instances is not None:
+        if self.instances is not None:
             return self.instances
         elif self.queryset is not None:
             return self.queryset
+        elif self.instance:
+            return type(self.instance).objects.filter(pk=self.instance.pk)
         return []
 
     def is_modal(self):
         return getattr(self.metaclass, 'modal', True) if hasattr(self, 'Meta') else True
 
     def has_permission(self, user):
         return user.is_superuser
@@ -771,24 +771,34 @@
                 value = None
             getattr(self, 'on_{}_change'.format(field_name))(value)
             raise JsonReadyResponseException(self.on_change_data)
         return super().is_valid()
 
     def choices(self, field_name, q=None):
         field = self.fields[field_name]
-        attr = getattr(self, 'get_{}_queryset'.format(field_name), None)
-        self.data.update(self.request.GET)
+        if self.__class__.__name__ in ('Add', 'Edit'):
+            attr = getattr(self.instance, 'get_{}_queryset'.format(field_name), None)
+            if attr:
+                for name in self.fields:
+                    if isinstance(self.fields[name], MultipleChoiceField):
+                        value = self.request.GET.getlist(name)
+                    if isinstance(self.fields[name], ModelMultipleChoiceField):
+                        value = self.request.GET.getlist(name)
+                    else:
+                        value = self.request.GET.get(name)
+                        if value:
+                            setattr(self.instance, name, self.fields[name].clean(value))
+        else:
+            attr = getattr(self, 'get_{}_queryset'.format(field_name), None)
         qs = field.queryset if attr is None else attr(field.queryset)
+        self.data.update(self.request.GET)
         total = qs.count()
         qs = qs.search(q=q) if q else qs
         items = [dict(id=value.id, text=str(value), html=value.get_select_display()) for value in qs[0:25]]
-        return dict(
-            total=total, page=1, pages=math.ceil((1.0 * total) / 25),
-            q=q, items=items
-        )
+        return dict(total=total, page=1, pages=math.ceil((1.0 * total) / 25), q=q, items=items )
 
     def dispose(self, milleseconds=2000):
         self.response.update(dispose=milleseconds)
 
     def reload(self):
         return self.redirect('.')
```

### Comparing `sloth-framework-0.1.4/sloth/actions/fields.py` & `sloth-framework-0.1.5/sloth/actions/fields.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/actions/inputs.py` & `sloth-framework-0.1.5/sloth/actions/inputs.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/__init__.py` & `sloth-framework-0.1.5/sloth/api/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/actions.py` & `sloth-framework-0.1.5/sloth/api/actions.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/backends/__init__.py` & `sloth-framework-0.1.5/sloth/api/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/dashboard.py` & `sloth-framework-0.1.5/sloth/api/dashboard.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,14 +90,15 @@
     def footer(self, title=None, text=None, version=None):
         self.data['footer'].update(title=title, text=text, version=version)
 
     def to_item(self, model, count=True):
         return
 
     def _load(self, key, items, modal=False, count=False, app=None):
+        new_item = None
         allways = 'floating', 'navigation', 'settings', 'actions', 'menu', 'links', 'tools', 'search', 'plus'
         for cls in items:
             if '.' in cls:
                 modal = False if key in ('tools', 'settings') else modal
                 tokens = cls.split('.')
                 cls = apps.get_model(*tokens[0:2])
                 subset = 'all' if len(tokens) == 2 else tokens[-1]
@@ -137,15 +138,15 @@
                                 new_item = dict(
                                     url=url, label=label, modal=modal or key == 'plus',
                                     count=cls.objects.all().apply_role_lookups(self.request.user).count() if count else None,
                                     icon=getattr(cls.metaclass(), 'icon', None),
                                     app=app
                                 )
                                 self.data[key].append(new_item)
-                                return new_item
+        return new_item
 
     def _item(self, key, url, label, icon, count=None, app=None):
         self.data[key].append(
             dict(url=url, label=label, count=count, icon=icon, app=app)
         )
 
     def info(self, *items, app=None):
```

### Comparing `sloth-framework-0.1.4/sloth/api/management/commands/cloud.py` & `sloth-framework-0.1.5/sloth/api/management/commands/cloud.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/management/commands/query.py` & `sloth-framework-0.1.5/sloth/api/management/commands/query.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/management/commands/send_web_push_notification.py` & `sloth-framework-0.1.5/sloth/api/management/commands/send_web_push_notification.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/management/commands/startserver.py` & `sloth-framework-0.1.5/sloth/api/management/commands/startserver.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/management/commands/sync.py` & `sloth-framework-0.1.5/sloth/api/management/commands/sync.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/migrations/0001_initial.py` & `sloth-framework-0.1.5/sloth/api/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/migrations/0002_role_user.py` & `sloth-framework-0.1.5/sloth/api/migrations/0002_role_user.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/migrations/0003_alter_application_user.py` & `sloth-framework-0.1.5/sloth/api/migrations/0003_alter_application_user.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/migrations/0004_task.py` & `sloth-framework-0.1.5/sloth/api/migrations/0004_task.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/migrations/0005_task_stopped_alter_task_message.py` & `sloth-framework-0.1.5/sloth/api/migrations/0005_task_stopped_alter_task_message.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/migrations/0006_role_active_alter_role_name_alter_role_scope_key_and_more.py` & `sloth-framework-0.1.5/sloth/api/migrations/0006_role_active_alter_role_name_alter_role_scope_key_and_more.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/migrations/0007_alter_scope_description_alter_task_error.py` & `sloth-framework-0.1.5/sloth/api/migrations/0007_alter_scope_description_alter_task_error.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/migrations/0008_alter_application_available_scopes_and_more.py` & `sloth-framework-0.1.5/sloth/api/migrations/0008_alter_application_available_scopes_and_more.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/migrations/0009_pushnotification.py` & `sloth-framework-0.1.5/sloth/api/migrations/0009_pushnotification.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/migrations/0010_alter_pushnotification_user.py` & `sloth-framework-0.1.5/sloth/api/migrations/0010_alter_pushnotification_user.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/migrations/0011_alter_application_client_secret.py` & `sloth-framework-0.1.5/sloth/api/migrations/0011_alter_application_client_secret.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/migrations/0012_authcode.py` & `sloth-framework-0.1.5/sloth/api/migrations/0012_authcode.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/migrations/0013_task_partial_task_total.py` & `sloth-framework-0.1.5/sloth/api/migrations/0013_task_partial_task_total.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/migrations/0014_email.py` & `sloth-framework-0.1.5/sloth/api/migrations/0014_email.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/models.py` & `sloth-framework-0.1.5/sloth/api/models.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/static/css/all.min.css` & `sloth-framework-0.1.5/sloth/api/static/css/all.min.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/static/css/bootstrap-icons.css` & `sloth-framework-0.1.5/sloth/api/static/css/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/static/css/bootstrap.min.css` & `sloth-framework-0.1.5/sloth/api/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/static/css/colorpick.min.css` & `sloth-framework-0.1.5/sloth/api/static/css/colorpick.min.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/static/css/fonts/Eina02-Bold.f8011405.ttf` & `sloth-framework-0.1.5/sloth/api/static/css/fonts/Eina02-Bold.f8011405.ttf`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/static/css/fonts/Eina02-Regular.2e682693.ttf` & `sloth-framework-0.1.5/sloth/api/static/css/fonts/Eina02-Regular.2e682693.ttf`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/static/css/fonts/Eina02-SemiBold.c5f9b8e3.ttf` & `sloth-framework-0.1.5/sloth/api/static/css/fonts/Eina02-SemiBold.c5f9b8e3.ttf`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/static/css/fonts/bootstrap-icons.woff` & `sloth-framework-0.1.5/sloth/api/static/css/fonts/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/static/css/fonts/bootstrap-icons.woff2` & `sloth-framework-0.1.5/sloth/api/static/css/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/static/css/icons.svg` & `sloth-framework-0.1.5/sloth/api/static/css/icons.svg`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/static/css/images/ui-icons_444444_256x240.png` & `sloth-framework-0.1.5/sloth/api/static/css/images/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/static/css/images/ui-icons_555555_256x240.png` & `sloth-framework-0.1.5/sloth/api/static/css/images/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/static/css/jquery-ui.css` & `sloth-framework-0.1.5/sloth/api/static/css/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/static/css/leaflet.css` & `sloth-framework-0.1.5/sloth/api/static/css/leaflet.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/static/css/select2.min.css` & `sloth-framework-0.1.5/sloth/api/static/css/select2.min.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/static/css/sloth.css` & `sloth-framework-0.1.5/sloth/api/static/css/sloth.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/static/css/trumbowyg.min.css` & `sloth-framework-0.1.5/sloth/api/static/css/trumbowyg.min.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/static/icons/fontawesome/fontawesome.min.css` & `sloth-framework-0.1.5/sloth/api/static/icons/fontawesome/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/static/icons/fontawesome/fontawesome.min.js` & `sloth-framework-0.1.5/sloth/api/static/icons/fontawesome/fontawesome.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.ttf` & `sloth-framework-0.1.5/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.woff2` & `sloth-framework-0.1.5/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.ttf` & `sloth-framework-0.1.5/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.woff2` & `sloth-framework-0.1.5/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.ttf` & `sloth-framework-0.1.5/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.woff2` & `sloth-framework-0.1.5/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/static/icons/materialicons/LDItaoyNOAY6Uewc665JcIzCKsKc_M9flwmPq_HTTw.woff2` & `sloth-framework-0.1.5/sloth/api/static/icons/materialicons/LDItaoyNOAY6Uewc665JcIzCKsKc_M9flwmPq_HTTw.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/static/icons/materialicons/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2` & `sloth-framework-0.1.5/sloth/api/static/icons/materialicons/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/static/icons/materialicons/gok-H7zzDkdnRel8-DQ6KAXJ69wP1tGnf4ZGhUcel5euIg.woff2` & `sloth-framework-0.1.5/sloth/api/static/icons/materialicons/gok-H7zzDkdnRel8-DQ6KAXJ69wP1tGnf4ZGhUcel5euIg.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/static/icons/materialicons/materialicons.css` & `sloth-framework-0.1.5/sloth/api/static/icons/materialicons/materialicons.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/static/icons/materialicons/oPWQ_lt5nv4pWNJpghLP75WiFR4kLh3kvmvRImcycg.woff2` & `sloth-framework-0.1.5/sloth/api/static/icons/materialicons/oPWQ_lt5nv4pWNJpghLP75WiFR4kLh3kvmvRImcycg.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/static/images/click.png` & `sloth-framework-0.1.5/sloth/api/static/images/click.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/static/images/hand.png` & `sloth-framework-0.1.5/sloth/api/static/images/hand.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/static/images/icon.png` & `sloth-framework-0.1.5/sloth/api/static/images/icon.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/static/images/icon.svg` & `sloth-framework-0.1.5/sloth/api/static/images/icon.svg`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/static/images/images/badge.png` & `sloth-framework-0.1.5/sloth/api/static/images/images/badge.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/static/images/images/icon.png` & `sloth-framework-0.1.5/sloth/api/static/images/images/icon.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/static/images/login.jpeg` & `sloth-framework-0.1.5/sloth/api/static/images/login.jpeg`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/static/images/logo.png` & `sloth-framework-0.1.5/sloth/api/static/images/logo.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/static/images/logo.svg` & `sloth-framework-0.1.5/sloth/api/static/images/logo.svg`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/static/images/no-image.png` & `sloth-framework-0.1.5/sloth/api/static/images/no-image.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/static/images/sloth.png` & `sloth-framework-0.1.5/sloth/api/static/images/sloth.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/static/images/user.png` & `sloth-framework-0.1.5/sloth/api/static/images/user.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/static/js/api.js` & `sloth-framework-0.1.5/sloth/api/static/js/api.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/static/js/bootstrap.bundle.min.js` & `sloth-framework-0.1.5/sloth/api/static/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/static/js/colorpick.min.js` & `sloth-framework-0.1.5/sloth/api/static/js/colorpick.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/static/js/i18n/pt-BR.js` & `sloth-framework-0.1.5/sloth/api/static/js/i18n/pt-BR.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/static/js/jquery-3.6.0.min.js` & `sloth-framework-0.1.5/sloth/api/static/js/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/static/js/jquery-ui.js` & `sloth-framework-0.1.5/sloth/api/static/js/jquery-ui.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/static/js/jquery.binarytransport.js` & `sloth-framework-0.1.5/sloth/api/static/js/jquery.binarytransport.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/static/js/jquery.mask.min.js` & `sloth-framework-0.1.5/sloth/api/static/js/jquery.mask.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/static/js/jquery.timepicker.js` & `sloth-framework-0.1.5/sloth/api/static/js/jquery.timepicker.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/static/js/leaflet.js` & `sloth-framework-0.1.5/sloth/api/static/js/leaflet.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/static/js/masonry.pkgd.min.js` & `sloth-framework-0.1.5/sloth/api/static/js/masonry.pkgd.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/static/js/popper.min.js` & `sloth-framework-0.1.5/sloth/api/static/js/popper.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/static/js/qr-scanner-worker.min.js` & `sloth-framework-0.1.5/sloth/api/static/js/qr-scanner-worker.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/static/js/qr-scanner.min.js` & `sloth-framework-0.1.5/sloth/api/static/js/qr-scanner.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/static/js/qrcode.min.js` & `sloth-framework-0.1.5/sloth/api/static/js/qrcode.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/static/js/select2.min.js` & `sloth-framework-0.1.5/sloth/api/static/js/select2.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/static/js/sloth.js` & `sloth-framework-0.1.5/sloth/api/static/js/sloth.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/static/js/sw.js` & `sloth-framework-0.1.5/sloth/api/static/js/sw.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/static/js/tests.js` & `sloth-framework-0.1.5/sloth/api/static/js/tests.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -146,15 +146,15 @@
             }
             return scroolToElement(element, afterScrool);
         }
     }
     throw Error('Not found.')
 }
 
-function clickMenu(name) {
+function searchMenu(name) {
     enter('search', name)
     return clickLink(name);
 }
 
 function clickLink(name) {
     return click(name, 'link');
 }
@@ -221,14 +221,16 @@
 
 function lookAtPanel(text) {
     return lookAt(text, true);
 }
 
 function enter(name, value, submit) {
     if (String(value) != 'null' && String(value)) {
+        var tokens = value.split('/');
+        if (tokens.length == 3 && value[2] == '/' && value[5] == '/') value = tokens[2] + '-' + tokens[1] + '-' + tokens[0];
         var element = $(cursor || document).find("input[name='" + name + "'], textarea[name='" + name + "']").not("input[type='checkbox']").not("input[type='hidden']").first();
         if (!element[0]) element = $(cursor || document).find("label").filter(function() {
             return $(this).text().trim().replace('*', '') === name;
         }).parent().find('input, textarea').not("input[type='checkbox']").first();
         $('input[name=hidden-upload-value]').remove();
         if (element.prop("type") == 'file') {
             $('<input type="hidden" name="hidden-upload-value" value="' + element[0].id + ':' + value + '">').appendTo(document.body);
```

### Comparing `sloth-framework-0.1.4/sloth/api/static/js/trumbowyg.min.js` & `sloth-framework-0.1.5/sloth/api/static/js/trumbowyg.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/static/js/wpn.js` & `sloth-framework-0.1.5/sloth/api/static/js/wpn.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/tasks/__init__.py` & `sloth-framework-0.1.5/sloth/api/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/templates/actions/execute_query.html` & `sloth-framework-0.1.5/sloth/api/templates/actions/execute_query.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/templates/actions/show_icons.html` & `sloth-framework-0.1.5/sloth/api/templates/actions/show_icons.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/templates/api/index.html` & `sloth-framework-0.1.5/sloth/api/templates/api/index.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/templates/charts/bar.html` & `sloth-framework-0.1.5/sloth/api/templates/charts/bar.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/templates/charts/column.html` & `sloth-framework-0.1.5/sloth/api/templates/charts/column.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/templates/charts/pie.html` & `sloth-framework-0.1.5/sloth/api/templates/charts/pie.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/templates/dashboard/actions.html` & `sloth-framework-0.1.5/sloth/api/templates/dashboard/actions.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {% load tags %}
 {% if actions %}
-<div class="action-container {{ target }}" id="{{ target }}-{{ uuid }}-{{id}}">
+<div class="action-container {{ target }}" id="{{ target }}-{{ uuid }}-{{id}}-{{ forloop.counter }}">
     {% if compact or request|mobile or request|tablet or request.GET.compact %}
     {% with grouped_actions=actions|group_by_icon %}
         {% for action in grouped_actions.with_icon %}
             {% if  target != 'instance' or  target == 'instance' and action.key in enabled %}
             <a href="{{ action.path }}"
                data-url="{{ action.path }}"
                data-id="{{ id }}"
@@ -64,15 +64,15 @@
         var extra = '{{ request|post_querystring }}';
         if(extra){
             console.log(extra);
             if(url.indexOf('?')>0) return url + '&' + extra;
             else return url + '?' + extra;
         } else { return url;}
     }
-    $('#{{ target }}-{{ uuid }}-{{id}}').find('.action-button').on('mouseenter', function(){
+    $('#{{ target }}-{{ uuid }}-{{id}}-{{ forloop.counter }}').find('.action-button').on('mouseenter', function(){
         if($(this).hasClass('instance')){
             this.href = actionURL($(this).data('url').replace('{id}', $(this).data('id')));
         }
         if($(this).hasClass('queryset')){
             var ids = $('#queryset-{{ uuid }}').find('.action-checkbox:checked').map(function(){
               return $(this).val();
             }).get().filter(function (id) { return id!='' }).join('-');
```

### Comparing `sloth-framework-0.1.4/sloth/api/templates/dashboard/apps.html` & `sloth-framework-0.1.5/sloth/api/templates/dashboard/apps.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/templates/dashboard/base.html` & `sloth-framework-0.1.5/sloth/api/templates/dashboard/base.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/templates/dashboard/bottom.html` & `sloth-framework-0.1.5/sloth/api/templates/dashboard/bottom.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/templates/dashboard/cards.html` & `sloth-framework-0.1.5/sloth/api/templates/dashboard/cards.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/templates/dashboard/footer.html` & `sloth-framework-0.1.5/sloth/api/templates/dashboard/footer.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/templates/dashboard/form.html` & `sloth-framework-0.1.5/sloth/api/templates/dashboard/form.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/templates/dashboard/grids.html` & `sloth-framework-0.1.5/sloth/api/templates/dashboard/grids.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/templates/dashboard/header.html` & `sloth-framework-0.1.5/sloth/api/templates/dashboard/header.html`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
       <style>
         .navbar {box-shadow: 0 .125rem .25rem rgba(0,0,0,.075);}
       </style>
     {% endif %}
     <nav class="navbar navbar-expand">
       <div class="container-fluid">
         {% if dashboard.data.menu %}
-          <i class="bi bi-list"></i>
+          <span id="menu-toogler"><i class="bi bi-list"></i></span>
         {% endif %}
         <a class="navbar-brand" href="/app/dashboard/">
           {% if dashboard.data.header.logo %}
             <img height="30" src="{{ dashboard.data.header.logo }}" style="border-radius:3px;">
           {% endif %}
           {% if dashboard.data.header.title %}
             <span>{{ dashboard.data.header.title }}</span>
```

### Comparing `sloth-framework-0.1.4/sloth/api/templates/dashboard/links.html` & `sloth-framework-0.1.5/sloth/api/templates/dashboard/links.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/templates/dashboard/menu.html` & `sloth-framework-0.1.5/sloth/api/templates/dashboard/menu.html`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     <i class="bi bi-x"></i>
     <ul class="open">
         {{ menu }}
     </ul>
 </div>
 <script>
 $( document ).ready(function() {
-    $('nav .bi-list').click(function(){$('.side-menu').animate({'margin-left': '0px'},'slow');});
+    $('#menu-toogler').click(function(){$('.side-menu').animate({'margin-left': '0px'},'slow');});
     $('.side-menu .bi-x').click(function() {$('.side-menu').animate({'margin-left': '-250px'},'slow');});
     $('.side-menu').mouseleave(function(){$(this).find('.bi-x').click()});
     $('.side-menu a').click(function(){
         var opened = $(this).parent().parent().find('ul.open');
         opened.slideUp();
         $(opened).parent().find('> a > i.bi-chevron-left').removeClass('bi-chevron-left').addClass('bi-chevron-down');
         if($(this).parent().find('> ul').hasClass('open')){
```

### Comparing `sloth-framework-0.1.4/sloth/api/templates/dashboard/messages.html` & `sloth-framework-0.1.5/sloth/api/templates/dashboard/messages.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/templates/dashboard/modal.html` & `sloth-framework-0.1.5/sloth/api/templates/dashboard/modal.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/templates/dashboard/plus.html` & `sloth-framework-0.1.5/sloth/api/templates/dashboard/plus.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/templates/dashboard/report.html` & `sloth-framework-0.1.5/sloth/api/templates/dashboard/report.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/templates/dashboard/search.html` & `sloth-framework-0.1.5/sloth/api/templates/dashboard/search.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/templates/dashboard/settings.html` & `sloth-framework-0.1.5/sloth/api/templates/dashboard/settings.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/templates/dashboard/shortcuts.html` & `sloth-framework-0.1.5/sloth/api/templates/dashboard/shortcuts.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/templates/dashboard/tasks.html` & `sloth-framework-0.1.5/sloth/api/templates/dashboard/tasks.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/templates/dashboard/tools.html` & `sloth-framework-0.1.5/sloth/api/templates/dashboard/tools.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/templates/inputs/picker.html` & `sloth-framework-0.1.5/sloth/api/templates/inputs/picker.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/templates/inputs/qrcode.html` & `sloth-framework-0.1.5/sloth/api/templates/inputs/qrcode.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/templates/inputs/select.html` & `sloth-framework-0.1.5/sloth/api/templates/inputs/select.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/templates/queryset/accordion.html` & `sloth-framework-0.1.5/sloth/api/templates/queryset/accordion.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/templates/queryset/calendar.html` & `sloth-framework-0.1.5/sloth/api/templates/queryset/calendar.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/templates/queryset/cards.html` & `sloth-framework-0.1.5/sloth/api/templates/queryset/cards.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/templates/queryset/datatable.html` & `sloth-framework-0.1.5/sloth/api/templates/queryset/datatable.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/templates/queryset/filter.html` & `sloth-framework-0.1.5/sloth/api/templates/queryset/filter.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/templates/queryset/filters.html` & `sloth-framework-0.1.5/sloth/api/templates/queryset/filters.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/templates/queryset/queryset.html` & `sloth-framework-0.1.5/sloth/api/templates/queryset/queryset.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/templates/queryset/rows.html` & `sloth-framework-0.1.5/sloth/api/templates/queryset/rows.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/templates/queryset/scroll.html` & `sloth-framework-0.1.5/sloth/api/templates/queryset/scroll.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/templates/queryset/statistics.html` & `sloth-framework-0.1.5/sloth/api/templates/queryset/statistics.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/templates/queryset/timeline.html` & `sloth-framework-0.1.5/sloth/api/templates/queryset/timeline.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/templates/queryset/tree.html` & `sloth-framework-0.1.5/sloth/api/templates/queryset/tree.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/templates/renderers/calendar/calendar.html` & `sloth-framework-0.1.5/sloth/api/templates/renderers/calendar/calendar.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/templates/renderers/maps/map.html` & `sloth-framework-0.1.5/sloth/api/templates/renderers/maps/map.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/templates/renderers/programing/strtable.html` & `sloth-framework-0.1.5/sloth/api/templates/renderers/programing/strtable.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/templates/renderers/utils/steps.html` & `sloth-framework-0.1.5/sloth/api/templates/renderers/utils/steps.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/templates/renderers/utils/table.html` & `sloth-framework-0.1.5/sloth/api/templates/renderers/utils/table.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/templates/themes/dark.html` & `sloth-framework-0.1.5/sloth/api/templates/themes/dark.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/templates/valueset/fieldset-group.html` & `sloth-framework-0.1.5/sloth/api/templates/valueset/fieldset-group.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/templates/valueset/fieldset-list.html` & `sloth-framework-0.1.5/sloth/api/templates/valueset/fieldset-list.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/templates/valueset/fieldset.html` & `sloth-framework-0.1.5/sloth/api/templates/valueset/fieldset.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/templates/valueset/value.html` & `sloth-framework-0.1.5/sloth/api/templates/valueset/value.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/templates/valueset/valueset.html` & `sloth-framework-0.1.5/sloth/api/templates/valueset/valueset.html`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 {% load tags %}
 <div class="valueset row clearfix">
-    <div class="{% if append %}col-lg-9 col-md-8 col-sm-12{% else %}col{% endif %}">
+    {% for item in data.append.top.values %}
+        <div class="col col-sm-12">{% include 'valueset/value.html' with v=item %}</div>
+    {% endfor %}
+    <div class="{% if data.append.right %}col-lg-9 col-md-8 col-sm-12{% else %}col{% endif %}">
 
         {% include "dashboard/shortcuts.html" with shortcuts=data.instance.data.shortcuts %}
         {% include "dashboard/cards.html" with cards=data.instance.data.cards %}
 
         <div class="valueset-header">
             <div class="valueset-title">
                 {% if data.title %}
@@ -105,23 +108,28 @@
                         {% endif %}
                     {% endfor %}
                 {% endif %}
             </div>
             {% endif %}
         {% endif %}
     </div>
-    {% if data.append %}
-    <div class="col-lg-3 col-md-4 col-sm-12 fieldset-side-panel">
-        {% for name, item in data.append.items %}
-            <div class="reloadable-fieldset" id="{{ item.key }}" data-path="{{ item.path }}?compact=1">
-                {% include 'valueset/fieldset.html' with data=item compact=True %}
-            </div>
-        {% endfor %}
-    </div>
+    {% for item in data.append.center.values %}
+        <div class="col col-sm-12">{% include 'valueset/value.html' with v=item %}</div>
+    {% endfor %}
+    {% if data.append.right %}
+        <div class="col-lg-3 col-md-4 col-sm-12 fieldset-side-panel">
+            {% for name, item in data.append.right.items %}
+                <div class="reloadable-fieldset" id="{{ item.key }}" data-path="{{ item.path }}?compact=1">
+                    {% include 'valueset/fieldset.html' with data=item compact=True %}
+                </div>
+            {% endfor %}
+        </div>
     {% endif %}
-
+    {% for item in data.append.bottom.values %}
+        <div class="col col-sm-12">{% include 'valueset/value.html' with v=item %}</div>
+    {% endfor %}
 </div>
```

### Comparing `sloth-framework-0.1.4/sloth/api/templatetags/tags.py` & `sloth-framework-0.1.5/sloth/api/templatetags/tags.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/api/urls.py` & `sloth-framework-0.1.5/sloth/api/urls.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,9 +29,9 @@
 urlpatterns.extend([
     path('', views.index),
     path('app/', views.index),
     path('app/manifest/', views.manifest),
     path('icon', views.icon),
     path('favicon.ico', views.favicon),
     re_path(r'^apple-touch.*', views.icon),
-    re_path(r'^app/(?P<path>.*)/$', views.dashboard),
+    re_path(r'^app/(?P<path>.*)/$', views.app),
 ])
```

### Comparing `sloth-framework-0.1.4/sloth/api/views.py` & `sloth-framework-0.1.5/sloth/api/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
-
+import json
 import base64
 import traceback
-
+from datetime import datetime
+from sloth import threadlocals
 from django.core.cache import cache
 from django.http import QueryDict
 from django.apps import apps
 from oauth2_provider.oauth2_backends import get_oauthlib_core
 from ..core.valueset import ValueSet
 from ..utils.http import ApiResponse
 from django.contrib.auth import authenticate
@@ -25,15 +26,28 @@
 from .dashboard import Dashboards, Dashboard
 from .. import initialize
 
 
 initialize()
 
 
-def dashboard(request, path):
+def logger(func):
+    def decorate(request, *args, **kwargs):
+        threadlocals.transaction = dict(
+            user=request.user.username, operation=None, time=datetime.now().strftime('%d/%m/%Y %H:%M'), path=request.path, diff=[]
+        )
+        response = func(request, *args, **kwargs)
+        if threadlocals.transaction['diff']:
+            print(json.dumps(threadlocals.transaction, ensure_ascii=False))
+        return response
+    return decorate
+
+
+@logger
+def app(request, path):
     if request.user.is_authenticated and settings.FORCE_PASSWORD_DEFINITION:
         default_password = settings.DEFAULT_PASSWORD(request.user)
         if request.user.check_password(default_password):
             messages.warning(request, 'Altere sua senha padrão')
             return HttpResponseRedirect('/app/dashboard/change_password/')
     try:
         ctx = dict(dashboard=Dashboards(request))
```

### Comparing `sloth-framework-0.1.4/sloth/cloud/printer.py` & `sloth-framework-0.1.5/sloth/cloud/printer.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/cloud/server.py` & `sloth-framework-0.1.5/sloth/cloud/server.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/conf/settings.py` & `sloth-framework-0.1.5/sloth/conf/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,7 +77,10 @@
 if os.environ.get('POSTGRES_HOST'):
     DATABASES['default']['ENGINE'] = 'django.db.backends.postgresql_psycopg2'
     DATABASES['default']['NAME'] = os.environ.get('DATABASE_NAME', 'database')
     DATABASES['default']['USER'] = os.environ.get('DATABASE_USER', 'postgres')
     DATABASES['default']['PASSWORD'] = os.environ.get('DATABASE_PASSWORD', 'password')
     DATABASES['default']['HOST'] = os.environ.get('DATABASE_HOST', 'postgres')
     DATABASES['default']['PORT'] = os.environ.get('DATABASE_PORT', '5432')
+
+
+from .local_settings import *
```

### Comparing `sloth-framework-0.1.4/sloth/core/base.py` & `sloth-framework-0.1.5/sloth/core/base.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/core/queryset.py` & `sloth-framework-0.1.5/sloth/core/queryset.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from django.conf import settings
 from django.contrib import messages
 from django.db import models
 from django.db.models import Q
 from django.db.models.aggregates import Sum, Count
 from django.template.loader import render_to_string
 from django.apps import apps
+
 from sloth.utils.http import XlsResponse, CsvResponse
 from sloth.core.statistics import QuerySetStatistics
 from sloth.api.exceptions import JsonReadyResponseException, HtmlReadyResponseException, ReadyResponseException
 from sloth.utils import getattrr, serialize, pretty, to_snake_case
 
 
 class QuerySet(models.QuerySet):
@@ -163,18 +164,17 @@
             list_filter = self.metadata['filters']
         else:
             list_filter = self.model.default_filter_fields()
         return [name for name in list_filter if name not in self.metadata['ignore']]
 
     def get_search(self):
         search = {}
-        if self.metadata['search'] is None:
-            for lookup in self.metadata['search'] or self.model.default_search_fields():
-                verbose_name = self.model.get_attr_metadata(lookup)[0]
-                search[lookup] = dict(key=lookup, name=verbose_name)
+        for lookup in self.metadata['search'] or self.model.default_search_fields():
+            verbose_name = self.model.get_attr_metadata(lookup)[0]
+            search[lookup] = dict(key=lookup, name=verbose_name)
         return search
 
     def get_display(self):
         display = {}
         for lookup in self.get_list_display():
             verbose_name, sort, _, _ = self.model.get_attr_metadata(lookup)
             display[lookup] = dict(
@@ -304,27 +304,26 @@
     # choices function
 
     def choices(self, request):
         items = []
         filter_lookup = request.GET['choices']
         q = request.GET.get('term')
         field = self.model.get_field(filter_lookup)
-        values = self.apply_role_lookups(request.user).values_list(
+        ids = self.apply_role_lookups(request.user).values_list(
             filter_lookup, flat=True
-        ).order_by(filter_lookup).order_by(filter_lookup).distinct()
+        ).order_by(filter_lookup).distinct()
         if field.null:
             items.append(dict(id='null', text='Indefinido'))
         if field.related_model:
-            qs = field.related_model.objects.filter(id__in=values)
+            qs = field.related_model.objects.filter(pk__in=ids)
             qs = qs.search(q=q) if q else qs
-            qs = qs.distinct()
-            total = values.count()
+            total = 25
             items.extend([dict(id=value.id, text=str(value)) for value in qs[0:25]])
         else:
-            total = values.count()
+            total = ids.count()
             items.extend([dict(id=value, text=str(value)) for value in values])
         return dict(
             total=total, page=1, pages=math.ceil((1.0 * total) / 25),
             q=q, items=items
         )
 
     # calendar
@@ -517,21 +516,24 @@
                 for view in self.metadata['view']:
                     if view['name'] == 'self':
                         view_suffix = ''
                         view_name = 'Visualizar'
                     else:
                         view_suffix = '{}/'.format(view['name'])
                         view_name = pretty(self.model.get_attr_metadata(view['name'])[0])
-                    data['actions']['instance'].insert(0,
-                        dict(
-                            type='view', key=view['name'], name=view_name, submit=view_name, target='instance',
-                            method='get', icon=view['icon'], style='primary', ajax=False,
-                            modal=view['modal'], path='{}{{id}}/{}'.format((path or '').split('?')[0], view_suffix)
-                        )
+                    item = dict(
+                        type='view', key=view['name'], name=view_name, submit=view_name, target='instance',
+                        method='get', icon=view['icon'], style='primary', ajax=False,
+                        modal=view['modal'], path='{}{{id}}/{}'.format((path or '').split('?')[0], view_suffix)
                     )
+                    if view_suffix:
+                        data['actions']['instance'].append(item)
+                    else:
+                        data['actions']['instance'].insert(0, item)
+
                 for action_type in ('global_actions', 'actions', 'batch_actions', 'inline_actions'):
                     target = dict(global_actions='model', actions='instance', batch_actions='queryset', inline_actions='inline')[action_type]
                     for form_name in self.metadata[action_type]:
                         if form_name == 'view':
                             continue
                         form_cls = self.model.action_form_cls(form_name)
                         has_permission = self.request is None or form_cls.check_fake_permission(
@@ -703,25 +705,28 @@
 
     def page(self, n):
         self.metadata['page'] = n
         return self
 
     # action functions
 
-    def actions(self, *names, clear=False):
+    def actions(self, *names, clear=False, priority=False):
         qs = self._clone()
         qs.metadata['actions'] = qs.metadata['actions'].copy()
         if clear:
             qs.metadata['actions'].clear()
         for name in names:
             if name == 'view':
                 qs.metadata['view'] = self.metadata['view'].copy()
                 qs.metadata['view'].append(dict(name='self', modal=False, icon='search'))
             elif to_snake_case(name) not in qs.metadata['actions']:
-                qs.metadata['actions'].append(to_snake_case(name))
+                if priority:
+                    qs.metadata['actions'].insert(0, to_snake_case(name))
+                else:
+                    qs.metadata['actions'].append(to_snake_case(name))
         return qs
 
     def global_actions(self, *names, clear=False):
         qs = self._clone()
         qs.metadata['global_actions'] = qs.metadata['global_actions'].copy()
         if clear:
             qs.metadata['global_actions'].clear()
@@ -748,15 +753,15 @@
         q.metadata['inline_actions'].extend(
             [to_snake_case(name) for name in names if to_snake_case(name) not in qs.metadata['inline_actions']]
         )
         return qs
 
     def default_actions(self):
         if self.metadata['attr'] is None:
-            return self.actions('view', 'edit', 'delete').global_actions('add')
+            return self.actions('delete', 'edit', 'view', priority=True).global_actions('add')
         return self
 
     # search and pagination functions
 
     def get_ordering(self):
         ordering = self.request.GET.get('ordering') if self.request else None
         if ordering:
@@ -976,7 +981,30 @@
         return queryset
 
     def action_form_cls(self, action):
         return self.model.action_form_cls(action)
 
     def get_full_path(self):
         pass
+
+    # logging
+
+    def __log__(self, operation, **kwargs):
+        from sloth import threadlocals
+        if hasattr(threadlocals, 'transaction'):
+            threadlocals.transaction['operation'] = operation
+            model_name = '{}.{}'.format(self.model.metaclass().app_label, self.model.metaclass().model_name)
+            for values in self.values(*(set(kwargs.keys()) | {'pk'})):
+                item = dict(pk=values['pk'], model=model_name, fields={
+                    k: (serialize(values[k], identifier=True), serialize(kwargs[k], identifier=True))
+                    for k in kwargs if values[k] != kwargs[k] and k != 'id'
+                })
+                threadlocals.transaction['diff'].append(item) if item['fields'] else None
+
+    def update(self, **kwargs):
+        self.__log__('edit', **kwargs)
+        super().update(**kwargs)
+
+    def delete(self):
+        kwargs = {f.name: None for f in self.model._meta.fields}
+        self.__log__('delete', **kwargs)
+        super().delete()
```

### Comparing `sloth-framework-0.1.4/sloth/core/statistics.py` & `sloth-framework-0.1.5/sloth/core/statistics.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/core/validation.py` & `sloth-framework-0.1.5/sloth/core/validation.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/core/valueset.py` & `sloth-framework-0.1.5/sloth/core/valueset.py`

 * *Files 8% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 class ValueSet(dict):
     def __init__(self, instance, names):
         self.path = None
         self.request = None
         self.instance = instance
         self.metadata = dict(
             model=type(instance), names={}, metadata=[], actions=[], type=None, attr=None, source=None,
-            attach=[], append=[], image=None, template=None, primitive=False, verbose_name=None,
+            attach=[], append={}, image=None, template=None, primitive=False, verbose_name=None,
             title=None, subtitle=None, status=None, icon=None, only={}, refresh={}, inline_actions=[],
             cards=[], shortcuts=[], collapsed=False, printing=False
         )
         for attr_name in names:
             if isinstance(attr_name, tuple):
                 for name in attr_name:
                     self.metadata['names'][name] = 100 // len(attr_name)
@@ -81,18 +81,30 @@
         self.metadata['actions'] = [to_snake_case(name) for name in names]
         return self
 
     def inline_actions(self, *names):
         self.metadata['inline_actions'] = [to_snake_case(name) for name in names]
         return self
 
-    def append(self, *names):
-        self.metadata['append'] = [to_snake_case(name) for name in names]
+    def append(self, *names, position='right'):
+        self.metadata['append'][position] = [to_snake_case(name) for name in names]
         return self
 
+    def top(self, *names):
+        return self.append(*names, position='top')
+
+    def left(self, *names):
+        return self.append(*names, position='left')
+
+    def right(self, *names):
+        return self.append(*names, position='right')
+
+    def bottom(self, *names):
+        return self.append(*names, position='bottom')
+
     def attach(self, *names):
         self.metadata['attach'] = [to_snake_case(name) for name in names]
         return self
 
     def image(self, image):
         image_attr = getattr(self.instance, image)
         self.metadata['image'] = image_attr() if callable(image_attr) else image_attr
@@ -127,16 +139,18 @@
         if source:
             return self.source(name)
         else:
             return self
 
     def get_allowed_attrs(self, recursive=True):
         allowed = []
-        for key in ('actions', 'inline_actions', 'append', 'attach'):
+        for key in ('actions', 'inline_actions', 'attach'):
             allowed.extend(self.metadata[key])
+        for items in self.metadata['append']:
+            allowed.extend(items)
         allowed.extend([name for name in self.metadata['names'].keys() if name.startswith('get_')])
         return allowed
 
     def source(self, name):
         self.metadata['source'] = name
         return self
 
@@ -359,20 +373,23 @@
                             request=self.request, instance=self.instance, instantiator=self.instance,
                     ):
                         output[action_type].append(form_cls.get_metadata(self.path))
             for attr_name in self.metadata['attach']:
                 name = getattr(self.instance, attr_name)().metadata['verbose_name'] or pretty(attr_name)
                 if self.request is None or self.instance.has_attr_permission(self.request.user, attr_name):
                     output['attach'].append(dict(name=name, path='{}{}/'.format(self.path, attr_name)))
-            for attr_name in self.metadata['append']:
-                if self.request is None or self.instance.has_attr_permission(self.request.user, attr_name):
-                    template = getattr(getattr(self.instance, attr_name), '__template__', None)
-                    output['append'].update(
-                        self.instance.value_set(attr_name).renderer(template).contextualize(self.request).load(wrap=wrap)
-                    )
+            for position, attr_names in self.metadata['append'].items():
+                for attr_name in attr_names:
+                    if self.request is None or self.instance.has_attr_permission(self.request.user, attr_name):
+                        template = getattr(getattr(self.instance, attr_name), '__template__', None)
+                        if position not in output['append']:
+                            output['append'][position] = {}
+                        output['append'][position].update(
+                            self.instance.value_set(attr_name).renderer(template).contextualize(self.request).load(wrap=wrap)
+                        )
             return output
         else:
             if len(self.metadata['names']) == 1:
                 return self[list(self.metadata['names'].keys())[0]]
             return self
 
     def html(self, path=None, print=False):
```

### Comparing `sloth-framework-0.1.4/sloth/db/models/__init__.py` & `sloth-framework-0.1.5/sloth/db/models/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # -*- coding: utf-8 -*-
 import datetime
 import json
+from sloth import threadlocals
 from decimal import Decimal
 from django.apps import apps
 from django.db import models
 from django.db.models import *
 from django.db.models import base
 from django.db.models.query_utils import DeferredAttribute
-
+from django.forms.models import model_to_dict
 from sloth.core.queryset import QuerySet
 from sloth.core.base import ModelMixin
+from sloth.utils import serialize
 
 
 class GenericModelWrapper(object):
     def __init__(self, obj):
         self._wrapped_obj = obj
 
     def __getattr__(self, attr):
@@ -271,14 +273,32 @@
 
 
 class Model(models.Model, ModelMixin, metaclass=ModelBase):
 
     class Meta:
         abstract = True
 
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.__dict__['__diff__'] = {}
+        if not hasattr(type(self), '__fieldnames__'):
+            type(self).__fieldnames__ = [f.name for f in type(self)._meta.get_fields()]
+
+    def __setattr__(self, key, value):
+        if getattr(self.metaclass(), 'logging', False) and self.__dict__.get('__diff__') is not None and key != 'id':
+            if value != self.__dict__.get(key) and key in type(self).__fieldnames__:
+                field_names = getattr(self.metaclass(), 'logging')
+                if field_names is True or key in field_names:
+                    if self.__dict__.get('{}_id'.format(key), 0) is None:
+                        previous = None
+                    else:
+                        previous = serialize(getattr(self, key), identifier=True)
+                    self.__dict__['__diff__'][key] = previous, serialize(value, identifier=True)
+        super().__setattr__(key, value)
+
     def pre_save(self, *args, **kwargs):
         setattr(self, '_pre_saved', True)
         if hasattr(self, '__roles__'):
             setattr(self, '_role_tuples', self.get_role_tuples(True))
 
     def save(self, *args, **kwargs):
         pre_saved = getattr(self, '_pre_saved', False)
@@ -287,27 +307,45 @@
 
         super().save(*args, **kwargs)
 
         if pre_saved is False:
             self.post_save()
 
     def post_save(self, *args, **kwargs):
+        self.__log__()
         if hasattr(self, '__roles__') and hasattr(self, '_role_tuples'):
             self.sync_roles(getattr(self, '_role_tuples'))
 
-    def persist(self):
-        self.pre_save()
-        self.save()
-        self.post_save()
-
     def delete(self, *args, **kwargs):
+        if getattr(self.metaclass(), 'logging', False):
+            field_names = getattr(self.metaclass(), 'logging')
+            for key in type(self).__fieldnames__:
+                if field_names is True or key in field_names:
+                    self.__dict__['__diff__'][key]= serialize(self.__dict__.get(key), identifier=True), None
+            self.__log__(delete=True)
         if hasattr(self, '__roles__'):
             setattr(self, '_role_tuples', self.get_role_tuples(True))
         super().delete(*args, **kwargs)
         if hasattr(self, '__roles__') and hasattr(self, '_role_tuples'):
             self.sync_roles(getattr(self, '_role_tuples'))
 
+    def __log__(self, delete=False):
+        if getattr(self.metaclass(), 'logging', False) and hasattr(threadlocals, 'transaction'):
+            if self.__dict__['__diff__']:
+                if delete:
+                    operation = 'delete'
+                elif 'id' in self.__dict__['__diff__']:
+                    operation = 'add'
+                else:
+                    operation = 'edit'
+                threadlocals.transaction['operation'] = operation
+                threadlocals.transaction['diff'].append(
+                    dict(pk=self.pk, model='{}.{}'.format(
+                        self.metaclass().app_label, self.metaclass().model_name
+                    ), fields=self.__dict__['__diff__'])
+                )
+
     def __str__(self):
         for field in self.metaclass().fields:
             if isinstance(field, models.CharField):
                 return getattr(self, field.name)
         return '{} #{}'.format(self.metaclass().verbose_name, self.pk)
```

### Comparing `sloth-framework-0.1.4/sloth/test/__init__.py` & `sloth-framework-0.1.5/sloth/test/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/test/selenium/__init__.py` & `sloth-framework-0.1.5/sloth/test/selenium/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,14 +84,17 @@
 
     def look_at_panel(self, text, count=2):
         self.browser.look_at_panel(text, count)
 
     def click_menu(self, *texts):
         self.browser.click_menu(*texts)
 
+    def search_menu(self, *texts):
+        self.browser.search_menu(*texts)
+
     def click_link(self, text):
         self.browser.click_link(text)
 
     def click_button(self, text):
         self.browser.click_button(text)
 
     def click_tab(self, text):
```

### Comparing `sloth-framework-0.1.4/sloth/test/selenium/browser.py` & `sloth-framework-0.1.5/sloth/test/selenium/browser.py`

 * *Files 1% similar despite different names*

```diff
@@ -232,19 +232,37 @@
             if count:
                 self.wait()
                 self.check_radio(text=text, count=count - 1)
             else:
                 self.watch(e)
         self.wait()
 
-    def click_menu(self, *texts, count=4):
-        self.print('Clicking menu "{}"'.format('->'.join(texts)))
+    def search_menu(self, *texts, count=4):
+        self.print('Searching "{}"'.format('->'.join(texts)))
         for text in texts:
             try:
-                self.execute_script("clickMenu('{}')".format(text.strip()))
+                self.execute_script("searchMenu('{}')".format(text.strip()))
+            except WebDriverException as e:
+                if count:
+                    self.wait()
+                    self.search_menu(*texts, count=count - 1)
+                else:
+                    self.watch(e)
+        self.wait()
+
+    def click_menu(self, *texts, count=1):
+        self.print('Clicking menu "{}"'.format('->'.join(texts)))
+        for i, text in enumerate(texts):
+            if i==0:
+                self.click_icon('list')
+                time.sleep(1)
+            if i==len(texts)-1:
+                time.sleep(0.5)
+            try:
+                self.click_link(text)
             except WebDriverException as e:
                 if count:
                     self.wait()
                     self.click_menu(*texts, count=count - 1)
                 else:
                     self.watch(e)
         self.wait()
```

### Comparing `sloth-framework-0.1.4/sloth/utils/__init__.py` & `sloth-framework-0.1.5/sloth/utils/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 def igetattr(obj, attr):
     for a in dir(obj):
         if a.lower() == attr.lower():
             return getattr(obj, a)
 
 
-def serialize(obj):
+def serialize(obj, identifier=False):
     if obj is not None:
         if isinstance(obj, str):
             return obj
         elif isinstance(obj, bool):
             return 'Sim' if obj else 'Não'
         elif isinstance(obj, datetime.datetime):
             return obj.strftime('%d/%m/%Y %H:%M')
@@ -60,16 +60,18 @@
             return float(obj)
         elif isinstance(obj, bool):
             return obj
         elif isinstance(obj, list):
             return [serialize(o) for o in obj]
         elif isinstance(obj, tuple):
             return [serialize(o) for o in obj]
+        elif hasattr(obj, 'pk'):
+            return obj.pk if identifier else str(obj)
         elif hasattr(obj, 'all'):
-            return [str(o) for o in obj.filter()]
+            return [o.pk if identifier else str(o) for o in obj.filter()]
         elif isinstance(obj, FieldFile):
             return obj and obj.url or '/static/images/no-image.png'
         return str(obj)
     return None
 
 
 def pretty(name):
```

### Comparing `sloth-framework-0.1.4/sloth/utils/formatter/__init__.py` & `sloth-framework-0.1.5/sloth/utils/formatter/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/utils/http/__init__.py` & `sloth-framework-0.1.5/sloth/utils/http/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/utils/icons/bootstrap.py` & `sloth-framework-0.1.5/sloth/utils/icons/bootstrap.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/utils/icons/fontawesome.py` & `sloth-framework-0.1.5/sloth/utils/icons/fontawesome.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/utils/icons/materialicons.py` & `sloth-framework-0.1.5/sloth/utils/icons/materialicons.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth/utils/log/sql.py` & `sloth-framework-0.1.5/sloth/utils/log/sql.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.4/sloth_framework.egg-info/PKG-INFO` & `sloth-framework-0.1.5/sloth_framework.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sloth-framework
-Version: 0.1.4
+Version: 0.1.5
 Summary: Metadata-based web framework for the development of management information systems
 Home-page: http://sloth.aplicativo.click/
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `sloth-framework-0.1.4/sloth_framework.egg-info/SOURCES.txt` & `sloth-framework-0.1.5/sloth_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

