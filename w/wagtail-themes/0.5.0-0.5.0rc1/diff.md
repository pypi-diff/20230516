# Comparing `tmp/wagtail-themes-0.5.0.tar.gz` & `tmp/wagtail-themes-0.5.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-themes-0.5.0.tar", last modified: Tue May 16 08:44:07 2023, max compression
+gzip compressed data, was "wagtail-themes-0.5.0rc1.tar", last modified: Tue Aug 30 07:51:02 2022, max compression
```

## Comparing `wagtail-themes-0.5.0.tar` & `wagtail-themes-0.5.0rc1.tar`

### file list

```diff
@@ -1,96 +1,113 @@
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-05-16 08:44:07.007266 wagtail-themes-0.5.0/
--rw-r--r--   0 robmoorman   (501) staff       (20)     1073 2022-08-29 12:29:50.000000 wagtail-themes-0.5.0/LICENSE
--rw-r--r--   0 robmoorman   (501) staff       (20)       24 2022-08-29 12:29:50.000000 wagtail-themes-0.5.0/MANIFEST.in
--rw-r--r--   0 robmoorman   (501) staff       (20)      779 2023-05-16 08:44:07.007509 wagtail-themes-0.5.0/PKG-INFO
--rw-r--r--   0 robmoorman   (501) staff       (20)     4716 2023-05-16 08:38:35.000000 wagtail-themes-0.5.0/README.md
--rw-r--r--   0 robmoorman   (501) staff       (20)      339 2023-05-16 08:44:07.008662 wagtail-themes-0.5.0/setup.cfg
--rw-r--r--   0 robmoorman   (501) staff       (20)     1190 2023-05-16 08:39:26.000000 wagtail-themes-0.5.0/setup.py
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-05-16 08:44:06.952761 wagtail-themes-0.5.0/src/
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-05-16 08:44:06.959973 wagtail-themes-0.5.0/src/wagtail_themes.egg-info/
--rw-r--r--   0 robmoorman   (501) staff       (20)      779 2023-05-16 08:44:06.000000 wagtail-themes-0.5.0/src/wagtail_themes.egg-info/PKG-INFO
--rw-r--r--   0 robmoorman   (501) staff       (20)     3665 2023-05-16 08:44:06.000000 wagtail-themes-0.5.0/src/wagtail_themes.egg-info/SOURCES.txt
--rw-r--r--   0 robmoorman   (501) staff       (20)        1 2023-05-16 08:44:06.000000 wagtail-themes-0.5.0/src/wagtail_themes.egg-info/dependency_links.txt
--rw-r--r--   0 robmoorman   (501) staff       (20)       86 2023-05-16 08:44:06.000000 wagtail-themes-0.5.0/src/wagtail_themes.egg-info/requires.txt
--rw-r--r--   0 robmoorman   (501) staff       (20)       14 2023-05-16 08:44:06.000000 wagtail-themes-0.5.0/src/wagtail_themes.egg-info/top_level.txt
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-05-16 08:44:06.961511 wagtail-themes-0.5.0/src/wagtailthemes/
--rw-r--r--   0 robmoorman   (501) staff       (20)        0 2022-08-29 13:39:05.000000 wagtail-themes-0.5.0/src/wagtailthemes/__init__.py
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-05-16 08:44:06.967138 wagtail-themes-0.5.0/src/wagtailthemes/__pycache__/
--rw-r--r--   0 robmoorman   (501) staff       (20)      178 2022-08-29 13:39:19.000000 wagtail-themes-0.5.0/src/wagtailthemes/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 robmoorman   (501) staff       (20)     1447 2022-08-29 13:25:46.000000 wagtail-themes-0.5.0/src/wagtailthemes/__pycache__/cache.cpython-39.pyc
--rw-r--r--   0 robmoorman   (501) staff       (20)      858 2022-08-29 13:25:47.000000 wagtail-themes-0.5.0/src/wagtailthemes/__pycache__/forms.cpython-39.pyc
--rw-r--r--   0 robmoorman   (501) staff       (20)     1243 2022-12-02 10:28:42.000000 wagtail-themes-0.5.0/src/wagtailthemes/__pycache__/loaders.cpython-39.pyc
--rw-r--r--   0 robmoorman   (501) staff       (20)     1046 2022-12-02 10:28:43.000000 wagtail-themes-0.5.0/src/wagtailthemes/__pycache__/middleware.cpython-39.pyc
--rw-r--r--   0 robmoorman   (501) staff       (20)     1326 2022-12-02 10:28:40.000000 wagtail-themes-0.5.0/src/wagtailthemes/__pycache__/models.cpython-39.pyc
--rw-r--r--   0 robmoorman   (501) staff       (20)      861 2022-08-29 13:49:58.000000 wagtail-themes-0.5.0/src/wagtailthemes/__pycache__/settings.cpython-39.pyc
--rw-r--r--   0 robmoorman   (501) staff       (20)     2619 2022-08-29 14:30:25.000000 wagtail-themes-0.5.0/src/wagtailthemes/__pycache__/storage.cpython-39.pyc
--rw-r--r--   0 robmoorman   (501) staff       (20)      516 2022-12-02 10:28:42.000000 wagtail-themes-0.5.0/src/wagtailthemes/__pycache__/thread.cpython-39.pyc
--rw-r--r--   0 robmoorman   (501) staff       (20)     4008 2022-08-29 13:25:46.000000 wagtail-themes-0.5.0/src/wagtailthemes/__pycache__/utils.cpython-39.pyc
--rw-r--r--   0 robmoorman   (501) staff       (20)     2063 2022-08-29 13:25:47.000000 wagtail-themes-0.5.0/src/wagtailthemes/__pycache__/views.cpython-39.pyc
--rw-r--r--   0 robmoorman   (501) staff       (20)     3128 2022-08-29 13:25:47.000000 wagtail-themes-0.5.0/src/wagtailthemes/__pycache__/wagtail_hooks.cpython-39.pyc
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-05-16 08:44:06.953335 wagtail-themes-0.5.0/src/wagtailthemes/contrib/
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-05-16 08:44:06.967596 wagtail-themes-0.5.0/src/wagtailthemes/contrib/__pycache__/
--rw-r--r--   0 robmoorman   (501) staff       (20)      186 2022-08-25 13:23:06.000000 wagtail-themes-0.5.0/src/wagtailthemes/contrib/__pycache__/__init__.cpython-39.pyc
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-05-16 08:44:06.953436 wagtail-themes-0.5.0/src/wagtailthemes/contrib/aws/
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-05-16 08:44:06.968833 wagtail-themes-0.5.0/src/wagtailthemes/contrib/aws/__pycache__/
--rw-r--r--   0 robmoorman   (501) staff       (20)      190 2022-08-25 13:23:06.000000 wagtail-themes-0.5.0/src/wagtailthemes/contrib/aws/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 robmoorman   (501) staff       (20)      876 2022-08-29 13:43:10.000000 wagtail-themes-0.5.0/src/wagtailthemes/contrib/aws/__pycache__/storage.cpython-39.pyc
--rw-r--r--   0 robmoorman   (501) staff       (20)      927 2022-12-02 10:24:09.000000 wagtail-themes-0.5.0/src/wagtailthemes/loaders.py
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-05-16 08:44:06.953769 wagtail-themes-0.5.0/src/wagtailthemes/management/
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-05-16 08:44:06.954070 wagtail-themes-0.5.0/src/wagtailthemes/management/commands/
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-05-16 08:44:06.969521 wagtail-themes-0.5.0/src/wagtailthemes/management/commands/__pycache__/
--rw-r--r--   0 robmoorman   (501) staff       (20)      971 2022-08-29 09:40:56.000000 wagtail-themes-0.5.0/src/wagtailthemes/management/commands/__pycache__/import_theme.cpython-39.pyc
--rw-r--r--   0 robmoorman   (501) staff       (20)      670 2023-05-16 08:37:24.000000 wagtail-themes-0.5.0/src/wagtailthemes/middleware.py
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-05-16 08:44:06.971871 wagtail-themes-0.5.0/src/wagtailthemes/migrations/
--rw-r--r--   0 robmoorman   (501) staff       (20)      873 2022-12-02 10:24:09.000000 wagtail-themes-0.5.0/src/wagtailthemes/migrations/0001_initial.py
--rw-r--r--   0 robmoorman   (501) staff       (20)      449 2022-12-02 10:24:09.000000 wagtail-themes-0.5.0/src/wagtailthemes/migrations/0002_auto_20161124_1107.py
--rw-r--r--   0 robmoorman   (501) staff       (20)        0 2022-08-29 12:29:50.000000 wagtail-themes-0.5.0/src/wagtailthemes/migrations/__init__.py
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-05-16 08:44:06.977326 wagtail-themes-0.5.0/src/wagtailthemes/migrations/__pycache__/
--rw-r--r--   0 robmoorman   (501) staff       (20)     1001 2022-12-02 10:28:43.000000 wagtail-themes-0.5.0/src/wagtailthemes/migrations/__pycache__/0001_initial.cpython-39.pyc
--rw-r--r--   0 robmoorman   (501) staff       (20)      657 2022-12-02 10:28:43.000000 wagtail-themes-0.5.0/src/wagtailthemes/migrations/__pycache__/0002_auto_20161124_1107.cpython-39.pyc
--rw-r--r--   0 robmoorman   (501) staff       (20)     2559 2022-08-29 13:30:57.000000 wagtail-themes-0.5.0/src/wagtailthemes/migrations/__pycache__/0003_auto_20220829_1325.cpython-39.pyc
--rw-r--r--   0 robmoorman   (501) staff       (20)     2315 2022-08-29 13:39:34.000000 wagtail-themes-0.5.0/src/wagtailthemes/migrations/__pycache__/0003_auto_20220829_1339.cpython-39.pyc
--rw-r--r--   0 robmoorman   (501) staff       (20)     2491 2022-08-29 14:30:27.000000 wagtail-themes-0.5.0/src/wagtailthemes/migrations/__pycache__/0003_auto_20220829_1350.cpython-39.pyc
--rw-r--r--   0 robmoorman   (501) staff       (20)     2456 2022-08-29 14:32:12.000000 wagtail-themes-0.5.0/src/wagtailthemes/migrations/__pycache__/0003_auto_20220829_1431.cpython-39.pyc
--rw-r--r--   0 robmoorman   (501) staff       (20)      895 2022-08-30 14:03:57.000000 wagtail-themes-0.5.0/src/wagtailthemes/migrations/__pycache__/0004_auto_20220830_1603.cpython-39.pyc
--rw-r--r--   0 robmoorman   (501) staff       (20)      823 2022-09-01 10:02:58.000000 wagtail-themes-0.5.0/src/wagtailthemes/migrations/__pycache__/0005_alter_staticfile_id_alter_template_id_alter_theme_id.cpython-39.pyc
--rw-r--r--   0 robmoorman   (501) staff       (20)      189 2022-08-29 13:25:58.000000 wagtail-themes-0.5.0/src/wagtailthemes/migrations/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 robmoorman   (501) staff       (20)      951 2023-05-16 08:37:24.000000 wagtail-themes-0.5.0/src/wagtailthemes/models.py
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-05-16 08:44:06.954934 wagtail-themes-0.5.0/src/wagtailthemes/templatetags/
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-05-16 08:44:06.979379 wagtail-themes-0.5.0/src/wagtailthemes/templatetags/__pycache__/
--rw-r--r--   0 robmoorman   (501) staff       (20)      191 2022-08-23 06:41:04.000000 wagtail-themes-0.5.0/src/wagtailthemes/templatetags/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 robmoorman   (501) staff       (20)     1272 2022-08-25 08:36:42.000000 wagtail-themes-0.5.0/src/wagtailthemes/templatetags/__pycache__/theme.cpython-39.pyc
--rw-r--r--   0 robmoorman   (501) staff       (20)     2317 2022-08-29 10:44:51.000000 wagtail-themes-0.5.0/src/wagtailthemes/templatetags/__pycache__/themes.cpython-39.pyc
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-05-16 08:44:06.981458 wagtail-themes-0.5.0/src/wagtailthemes/tests/
--rw-r--r--   0 robmoorman   (501) staff       (20)        0 2022-08-17 07:25:56.000000 wagtail-themes-0.5.0/src/wagtailthemes/tests/__init__.py
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-05-16 08:44:06.984897 wagtail-themes-0.5.0/src/wagtailthemes/tests/__pycache__/
--rw-r--r--   0 robmoorman   (501) staff       (20)      184 2022-08-29 07:28:35.000000 wagtail-themes-0.5.0/src/wagtailthemes/tests/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 robmoorman   (501) staff       (20)     1058 2022-08-29 07:28:36.000000 wagtail-themes-0.5.0/src/wagtailthemes/tests/__pycache__/conftest.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 robmoorman   (501) staff       (20)     2561 2022-08-29 14:35:20.000000 wagtail-themes-0.5.0/src/wagtailthemes/tests/__pycache__/settings.cpython-39.pyc
--rw-r--r--   0 robmoorman   (501) staff       (20)      402 2022-08-29 07:28:42.000000 wagtail-themes-0.5.0/src/wagtailthemes/tests/__pycache__/urls.cpython-39.pyc
--rw-r--r--   0 robmoorman   (501) staff       (20)      488 2023-05-16 08:37:24.000000 wagtail-themes-0.5.0/src/wagtailthemes/tests/conftest.py
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-05-16 08:44:06.986228 wagtail-themes-0.5.0/src/wagtailthemes/tests/integration/
--rw-r--r--   0 robmoorman   (501) staff       (20)        0 2022-08-17 07:25:56.000000 wagtail-themes-0.5.0/src/wagtailthemes/tests/integration/__init__.py
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-05-16 08:44:06.995241 wagtail-themes-0.5.0/src/wagtailthemes/tests/integration/__pycache__/
--rw-r--r--   0 robmoorman   (501) staff       (20)      196 2022-08-29 07:28:36.000000 wagtail-themes-0.5.0/src/wagtailthemes/tests/integration/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 robmoorman   (501) staff       (20)     1757 2022-08-29 07:28:36.000000 wagtail-themes-0.5.0/src/wagtailthemes/tests/integration/__pycache__/test_middleware.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 robmoorman   (501) staff       (20)      814 2023-05-16 08:37:24.000000 wagtail-themes-0.5.0/src/wagtailthemes/tests/integration/test_middleware.py
--rw-r--r--   0 robmoorman   (501) staff       (20)     2980 2023-05-16 08:37:24.000000 wagtail-themes-0.5.0/src/wagtailthemes/tests/settings.py
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-05-16 08:44:06.997793 wagtail-themes-0.5.0/src/wagtailthemes/tests/templates/
--rw-r--r--   0 robmoorman   (501) staff       (20)       69 2022-08-17 07:25:56.000000 wagtail-themes-0.5.0/src/wagtailthemes/tests/templates/base.html
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-05-16 08:44:06.998942 wagtail-themes-0.5.0/src/wagtailthemes/tests/templates/brand/
--rw-r--r--   0 robmoorman   (501) staff       (20)      101 2022-08-17 07:25:56.000000 wagtail-themes-0.5.0/src/wagtailthemes/tests/templates/brand/base.html
--rw-r--r--   0 robmoorman   (501) staff       (20)       64 2022-08-17 07:25:56.000000 wagtail-themes-0.5.0/src/wagtailthemes/tests/templates/page.html
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-05-16 08:44:06.956116 wagtail-themes-0.5.0/src/wagtailthemes/tests/templates/themes/
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-05-16 08:44:06.999965 wagtail-themes-0.5.0/src/wagtailthemes/tests/templates/themes/brand/
--rw-r--r--   0 robmoorman   (501) staff       (20)      108 2022-08-17 07:25:56.000000 wagtail-themes-0.5.0/src/wagtailthemes/tests/templates/themes/brand/base.html
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-05-16 08:44:07.002235 wagtail-themes-0.5.0/src/wagtailthemes/tests/unit/
--rw-r--r--   0 robmoorman   (501) staff       (20)        0 2022-08-17 07:25:56.000000 wagtail-themes-0.5.0/src/wagtailthemes/tests/unit/__init__.py
-drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2023-05-16 08:44:07.006233 wagtail-themes-0.5.0/src/wagtailthemes/tests/unit/__pycache__/
--rw-r--r--   0 robmoorman   (501) staff       (20)      189 2022-08-29 07:28:36.000000 wagtail-themes-0.5.0/src/wagtailthemes/tests/unit/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 robmoorman   (501) staff       (20)     2044 2022-08-29 07:28:36.000000 wagtail-themes-0.5.0/src/wagtailthemes/tests/unit/__pycache__/test_cache.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 robmoorman   (501) staff       (20)     2254 2022-08-29 07:28:36.000000 wagtail-themes-0.5.0/src/wagtailthemes/tests/unit/__pycache__/test_loader.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 robmoorman   (501) staff       (20)     1249 2022-08-29 07:28:36.000000 wagtail-themes-0.5.0/src/wagtailthemes/tests/unit/__pycache__/test_thread.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 robmoorman   (501) staff       (20)      858 2022-12-02 10:24:09.000000 wagtail-themes-0.5.0/src/wagtailthemes/tests/unit/test_loader.py
--rw-r--r--   0 robmoorman   (501) staff       (20)      347 2022-12-02 10:24:09.000000 wagtail-themes-0.5.0/src/wagtailthemes/tests/unit/test_thread.py
--rw-r--r--   0 robmoorman   (501) staff       (20)      247 2023-05-16 08:37:24.000000 wagtail-themes-0.5.0/src/wagtailthemes/tests/urls.py
--rw-r--r--   0 robmoorman   (501) staff       (20)      225 2022-12-02 10:24:09.000000 wagtail-themes-0.5.0/src/wagtailthemes/thread.py
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2022-08-30 07:51:02.691072 wagtail-themes-0.5.0rc1/
+-rw-r--r--   0 robmoorman   (501) staff       (20)     1073 2022-08-29 12:29:50.000000 wagtail-themes-0.5.0rc1/LICENSE
+-rw-r--r--   0 robmoorman   (501) staff       (20)       24 2022-08-29 12:29:50.000000 wagtail-themes-0.5.0rc1/MANIFEST.in
+-rw-r--r--   0 robmoorman   (501) staff       (20)      689 2022-08-30 07:51:02.691263 wagtail-themes-0.5.0rc1/PKG-INFO
+-rw-r--r--   0 robmoorman   (501) staff       (20)     4722 2022-08-29 12:29:50.000000 wagtail-themes-0.5.0rc1/README.md
+-rw-r--r--   0 robmoorman   (501) staff       (20)      507 2022-08-30 07:51:02.692157 wagtail-themes-0.5.0rc1/setup.cfg
+-rw-r--r--   0 robmoorman   (501) staff       (20)     1150 2022-08-30 07:47:44.000000 wagtail-themes-0.5.0rc1/setup.py
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2022-08-30 07:51:02.639664 wagtail-themes-0.5.0rc1/src/
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2022-08-30 07:51:02.648906 wagtail-themes-0.5.0rc1/src/wagtail_themes.egg-info/
+-rw-r--r--   0 robmoorman   (501) staff       (20)      689 2022-08-30 07:51:02.000000 wagtail-themes-0.5.0rc1/src/wagtail_themes.egg-info/PKG-INFO
+-rw-r--r--   0 robmoorman   (501) staff       (20)     4151 2022-08-30 07:51:02.000000 wagtail-themes-0.5.0rc1/src/wagtail_themes.egg-info/SOURCES.txt
+-rw-r--r--   0 robmoorman   (501) staff       (20)        1 2022-08-30 07:51:02.000000 wagtail-themes-0.5.0rc1/src/wagtail_themes.egg-info/dependency_links.txt
+-rw-r--r--   0 robmoorman   (501) staff       (20)      122 2022-08-30 07:51:02.000000 wagtail-themes-0.5.0rc1/src/wagtail_themes.egg-info/requires.txt
+-rw-r--r--   0 robmoorman   (501) staff       (20)       14 2022-08-30 07:51:02.000000 wagtail-themes-0.5.0rc1/src/wagtail_themes.egg-info/top_level.txt
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2022-08-30 07:51:02.652587 wagtail-themes-0.5.0rc1/src/wagtailthemes/
+-rw-r--r--   0 robmoorman   (501) staff       (20)        0 2022-08-29 13:39:05.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/__init__.py
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2022-08-30 07:51:02.659614 wagtail-themes-0.5.0rc1/src/wagtailthemes/__pycache__/
+-rw-r--r--   0 robmoorman   (501) staff       (20)      178 2022-08-29 13:39:19.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 robmoorman   (501) staff       (20)     1447 2022-08-29 13:25:46.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/__pycache__/cache.cpython-39.pyc
+-rw-r--r--   0 robmoorman   (501) staff       (20)      858 2022-08-29 13:25:47.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/__pycache__/forms.cpython-39.pyc
+-rw-r--r--   0 robmoorman   (501) staff       (20)     2598 2022-08-29 13:25:47.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/__pycache__/loaders.cpython-39.pyc
+-rw-r--r--   0 robmoorman   (501) staff       (20)     1125 2022-08-29 13:31:38.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/__pycache__/middleware.cpython-39.pyc
+-rw-r--r--   0 robmoorman   (501) staff       (20)     6022 2022-08-29 13:39:19.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/__pycache__/models.cpython-39.pyc
+-rw-r--r--   0 robmoorman   (501) staff       (20)      861 2022-08-29 13:49:58.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/__pycache__/settings.cpython-39.pyc
+-rw-r--r--   0 robmoorman   (501) staff       (20)     2619 2022-08-29 14:30:25.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/__pycache__/storage.cpython-39.pyc
+-rw-r--r--   0 robmoorman   (501) staff       (20)      516 2022-08-29 13:25:47.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/__pycache__/thread.cpython-39.pyc
+-rw-r--r--   0 robmoorman   (501) staff       (20)     4008 2022-08-29 13:25:46.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/__pycache__/utils.cpython-39.pyc
+-rw-r--r--   0 robmoorman   (501) staff       (20)     2063 2022-08-29 13:25:47.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/__pycache__/views.cpython-39.pyc
+-rw-r--r--   0 robmoorman   (501) staff       (20)     3128 2022-08-29 13:25:47.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/__pycache__/wagtail_hooks.cpython-39.pyc
+-rw-r--r--   0 robmoorman   (501) staff       (20)      954 2022-08-29 07:43:05.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/cache.py
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2022-08-30 07:51:02.660183 wagtail-themes-0.5.0rc1/src/wagtailthemes/contrib/
+-rw-r--r--   0 robmoorman   (501) staff       (20)        0 2022-08-22 13:55:39.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/contrib/__init__.py
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2022-08-30 07:51:02.660408 wagtail-themes-0.5.0rc1/src/wagtailthemes/contrib/__pycache__/
+-rw-r--r--   0 robmoorman   (501) staff       (20)      186 2022-08-25 13:23:06.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/contrib/__pycache__/__init__.cpython-39.pyc
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2022-08-30 07:51:02.661169 wagtail-themes-0.5.0rc1/src/wagtailthemes/contrib/aws/
+-rw-r--r--   0 robmoorman   (501) staff       (20)        0 2022-08-22 13:55:47.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/contrib/aws/__init__.py
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2022-08-30 07:51:02.661981 wagtail-themes-0.5.0rc1/src/wagtailthemes/contrib/aws/__pycache__/
+-rw-r--r--   0 robmoorman   (501) staff       (20)      190 2022-08-25 13:23:06.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/contrib/aws/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 robmoorman   (501) staff       (20)      876 2022-08-29 13:43:10.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/contrib/aws/__pycache__/storage.cpython-39.pyc
+-rw-r--r--   0 robmoorman   (501) staff       (20)      541 2022-08-29 13:42:31.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/contrib/aws/storage.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)      454 2022-08-17 07:26:18.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/forms.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)     2884 2022-08-29 08:34:31.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/loaders.py
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2022-08-30 07:51:02.641506 wagtail-themes-0.5.0rc1/src/wagtailthemes/management/
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2022-08-30 07:51:02.662604 wagtail-themes-0.5.0rc1/src/wagtailthemes/management/commands/
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2022-08-30 07:51:02.663107 wagtail-themes-0.5.0rc1/src/wagtailthemes/management/commands/__pycache__/
+-rw-r--r--   0 robmoorman   (501) staff       (20)      971 2022-08-29 09:40:56.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/management/commands/__pycache__/import_theme.cpython-39.pyc
+-rw-r--r--   0 robmoorman   (501) staff       (20)      516 2022-08-29 09:41:19.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/management/commands/import_theme.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)      770 2022-08-29 08:48:05.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/middleware.py
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2022-08-30 07:51:02.665368 wagtail-themes-0.5.0rc1/src/wagtailthemes/migrations/
+-rw-r--r--   0 robmoorman   (501) staff       (20)     1205 2022-08-29 13:25:29.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/migrations/0001_initial.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)      449 2022-08-29 13:25:29.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/migrations/0002_auto_20161124_1107.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)     6171 2022-08-29 14:32:11.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/migrations/0003_auto_20220829_1431.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)        0 2022-08-29 12:29:50.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/migrations/__init__.py
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2022-08-30 07:51:02.670167 wagtail-themes-0.5.0rc1/src/wagtailthemes/migrations/__pycache__/
+-rw-r--r--   0 robmoorman   (501) staff       (20)     1027 2022-08-29 13:25:58.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/migrations/__pycache__/0001_initial.cpython-39.pyc
+-rw-r--r--   0 robmoorman   (501) staff       (20)      657 2022-08-29 13:25:58.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/migrations/__pycache__/0002_auto_20161124_1107.cpython-39.pyc
+-rw-r--r--   0 robmoorman   (501) staff       (20)     2559 2022-08-29 13:30:57.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/migrations/__pycache__/0003_auto_20220829_1325.cpython-39.pyc
+-rw-r--r--   0 robmoorman   (501) staff       (20)     2315 2022-08-29 13:39:34.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/migrations/__pycache__/0003_auto_20220829_1339.cpython-39.pyc
+-rw-r--r--   0 robmoorman   (501) staff       (20)     2491 2022-08-29 14:30:27.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/migrations/__pycache__/0003_auto_20220829_1350.cpython-39.pyc
+-rw-r--r--   0 robmoorman   (501) staff       (20)     2456 2022-08-29 14:32:12.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/migrations/__pycache__/0003_auto_20220829_1431.cpython-39.pyc
+-rw-r--r--   0 robmoorman   (501) staff       (20)      189 2022-08-29 13:25:58.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/migrations/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 robmoorman   (501) staff       (20)     6072 2022-08-29 13:36:47.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/models.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)      846 2022-08-29 13:44:10.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/settings.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)     2282 2022-08-29 14:29:41.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/storage.py
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2022-08-30 07:51:02.642632 wagtail-themes-0.5.0rc1/src/wagtailthemes/templates/
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2022-08-30 07:51:02.671778 wagtail-themes-0.5.0rc1/src/wagtailthemes/templates/wagtailthemes/
+-rw-r--r--   0 robmoorman   (501) staff       (20)     1441 2022-08-17 07:26:18.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/templates/wagtailthemes/export_theme.html
+-rw-r--r--   0 robmoorman   (501) staff       (20)     1433 2022-08-17 07:26:18.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/templates/wagtailthemes/import_theme.html
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2022-08-30 07:51:02.673762 wagtail-themes-0.5.0rc1/src/wagtailthemes/templatetags/
+-rw-r--r--   0 robmoorman   (501) staff       (20)        0 2022-08-22 15:20:31.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/templatetags/__init__.py
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2022-08-30 07:51:02.676854 wagtail-themes-0.5.0rc1/src/wagtailthemes/templatetags/__pycache__/
+-rw-r--r--   0 robmoorman   (501) staff       (20)      191 2022-08-23 06:41:04.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/templatetags/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 robmoorman   (501) staff       (20)     1272 2022-08-25 08:36:42.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/templatetags/__pycache__/theme.cpython-39.pyc
+-rw-r--r--   0 robmoorman   (501) staff       (20)     2317 2022-08-29 10:44:51.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/templatetags/__pycache__/themes.cpython-39.pyc
+-rw-r--r--   0 robmoorman   (501) staff       (20)     2900 2022-08-29 10:44:34.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/templatetags/themes.py
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2022-08-30 07:51:02.679012 wagtail-themes-0.5.0rc1/src/wagtailthemes/tests/
+-rw-r--r--   0 robmoorman   (501) staff       (20)        0 2022-08-17 07:25:56.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/tests/__init__.py
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2022-08-30 07:51:02.681878 wagtail-themes-0.5.0rc1/src/wagtailthemes/tests/__pycache__/
+-rw-r--r--   0 robmoorman   (501) staff       (20)      184 2022-08-29 07:28:35.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/tests/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 robmoorman   (501) staff       (20)     1058 2022-08-29 07:28:36.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/tests/__pycache__/conftest.cpython-39-pytest-7.1.2.pyc
+-rw-r--r--   0 robmoorman   (501) staff       (20)     2561 2022-08-29 14:35:20.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/tests/__pycache__/settings.cpython-39.pyc
+-rw-r--r--   0 robmoorman   (501) staff       (20)      402 2022-08-29 07:28:42.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/tests/__pycache__/urls.cpython-39.pyc
+-rw-r--r--   0 robmoorman   (501) staff       (20)      493 2022-08-17 07:26:18.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/tests/conftest.py
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2022-08-30 07:51:02.682805 wagtail-themes-0.5.0rc1/src/wagtailthemes/tests/integration/
+-rw-r--r--   0 robmoorman   (501) staff       (20)        0 2022-08-17 07:25:56.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/tests/integration/__init__.py
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2022-08-30 07:51:02.683795 wagtail-themes-0.5.0rc1/src/wagtailthemes/tests/integration/__pycache__/
+-rw-r--r--   0 robmoorman   (501) staff       (20)      196 2022-08-29 07:28:36.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/tests/integration/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 robmoorman   (501) staff       (20)     1757 2022-08-29 07:28:36.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/tests/integration/__pycache__/test_middleware.cpython-39-pytest-7.1.2.pyc
+-rw-r--r--   0 robmoorman   (501) staff       (20)      841 2022-08-17 07:26:18.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/tests/integration/test_middleware.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)     2836 2022-08-29 07:38:09.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/tests/settings.py
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2022-08-30 07:51:02.685054 wagtail-themes-0.5.0rc1/src/wagtailthemes/tests/templates/
+-rw-r--r--   0 robmoorman   (501) staff       (20)       69 2022-08-17 07:25:56.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/tests/templates/base.html
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2022-08-30 07:51:02.685587 wagtail-themes-0.5.0rc1/src/wagtailthemes/tests/templates/brand/
+-rw-r--r--   0 robmoorman   (501) staff       (20)      101 2022-08-17 07:25:56.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/tests/templates/brand/base.html
+-rw-r--r--   0 robmoorman   (501) staff       (20)       64 2022-08-17 07:25:56.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/tests/templates/page.html
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2022-08-30 07:51:02.644736 wagtail-themes-0.5.0rc1/src/wagtailthemes/tests/templates/themes/
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2022-08-30 07:51:02.686087 wagtail-themes-0.5.0rc1/src/wagtailthemes/tests/templates/themes/brand/
+-rw-r--r--   0 robmoorman   (501) staff       (20)      108 2022-08-17 07:25:56.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/tests/templates/themes/brand/base.html
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2022-08-30 07:51:02.687649 wagtail-themes-0.5.0rc1/src/wagtailthemes/tests/unit/
+-rw-r--r--   0 robmoorman   (501) staff       (20)        0 2022-08-17 07:25:56.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/tests/unit/__init__.py
+drwxr-xr-x   0 robmoorman   (501) staff       (20)        0 2022-08-30 07:51:02.690519 wagtail-themes-0.5.0rc1/src/wagtailthemes/tests/unit/__pycache__/
+-rw-r--r--   0 robmoorman   (501) staff       (20)      189 2022-08-29 07:28:36.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/tests/unit/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 robmoorman   (501) staff       (20)     2044 2022-08-29 07:28:36.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/tests/unit/__pycache__/test_cache.cpython-39-pytest-7.1.2.pyc
+-rw-r--r--   0 robmoorman   (501) staff       (20)     2254 2022-08-29 07:28:36.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/tests/unit/__pycache__/test_loader.cpython-39-pytest-7.1.2.pyc
+-rw-r--r--   0 robmoorman   (501) staff       (20)     1249 2022-08-29 07:28:36.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/tests/unit/__pycache__/test_thread.cpython-39-pytest-7.1.2.pyc
+-rw-r--r--   0 robmoorman   (501) staff       (20)      560 2022-08-17 07:26:18.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/tests/unit/test_cache.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)      858 2022-08-17 07:26:18.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/tests/unit/test_loader.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)      347 2022-08-17 07:26:18.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/tests/unit/test_thread.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)      252 2022-08-17 07:26:18.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/tests/urls.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)      225 2022-08-29 13:25:29.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/thread.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)     4481 2022-08-29 12:27:28.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/utils.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)     2306 2022-08-29 12:28:48.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/views.py
+-rw-r--r--   0 robmoorman   (501) staff       (20)     2459 2022-08-29 07:26:16.000000 wagtail-themes-0.5.0rc1/src/wagtailthemes/wagtail_hooks.py
```

### Comparing `wagtail-themes-0.5.0/LICENSE` & `wagtail-themes-0.5.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail-themes-0.5.0/PKG-INFO` & `wagtail-themes-0.5.0rc1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: wagtail-themes
-Version: 0.5.0
+Version: 0.5.0rc1
 Summary: Site specific theme loader for Django Wagtail.
-Home-page: https://github.com/moorinl/wagtail-themes
+Home-page: https://github.com/moorinteractive/wagtail-themes
 Author: Rob Moorman
 Author-email: rob@moori.nl
 License: MIT
+Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Operating System :: Unix
-Classifier: Framework :: Wagtail
-Classifier: Framework :: Wagtail :: 3
-Classifier: Framework :: Wagtail :: 4
-Classifier: Framework :: Wagtail :: 5
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: aws
 Provides-Extra: test
 License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `wagtail-themes-0.5.0/README.md` & `wagtail-themes-0.5.0rc1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 
 * Issues: [https://github.com/moorinteractive/wagtail-themes/issues](https://github.com/moorinteractive/wagtail-themes/issues)
 * Testing: [https://travis-ci.org/moorinteractive/wagtail-themes](https://travis-ci.org/moorinteractive/wagtail-themes)
 * Coverage: [https://coveralls.io/github/moorinteractive/wagtail-themes](https://coveralls.io/github/moorinteractive/wagtail-themes)
 
 ## Compatibility
 
-* Django >= 4.2
-* Wagtail >= 5.0
+* Django >= 3.1
+* Wagtail > =2.12
 
-For older version of Django & Wagtail please use `wagtail-themes==0.4.1`.
+For older version of Django & Wagtail please use `wagtail-themes==0.3.0`.
 
 ## Example app
 
 See the [example](https://github.com/moorinteractive/wagtail-themes/tree/master/example) app for a working multisite with two different themes.
 
 Run `make` and the app will install all the necessary files and fixtures for you. You can login with `admin:admin` and check how `example.com` and `blog.example.com` serve different themes.
 
@@ -40,15 +40,15 @@
     'wagtail.sites',
     'wagtail.users',
     'wagtail.snippets',
     'wagtail.documents',
     'wagtail.images',
     'wagtail.search',
     'wagtail.admin',
-    'wagtail',
+    'wagtail.core',
 
     'modelcluster',
     'taggit',
 
     'django.contrib.admin',
     'django.contrib.auth',
     'django.contrib.contenttypes',
```

### Comparing `wagtail-themes-0.5.0/src/wagtail_themes.egg-info/PKG-INFO` & `wagtail-themes-0.5.0rc1/src/wagtail_themes.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: wagtail-themes
-Version: 0.5.0
+Version: 0.5.0rc1
 Summary: Site specific theme loader for Django Wagtail.
-Home-page: https://github.com/moorinl/wagtail-themes
+Home-page: https://github.com/moorinteractive/wagtail-themes
 Author: Rob Moorman
 Author-email: rob@moori.nl
 License: MIT
+Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Operating System :: Unix
-Classifier: Framework :: Wagtail
-Classifier: Framework :: Wagtail :: 3
-Classifier: Framework :: Wagtail :: 4
-Classifier: Framework :: Wagtail :: 5
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: aws
 Provides-Extra: test
 License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `wagtail-themes-0.5.0/src/wagtail_themes.egg-info/SOURCES.txt` & `wagtail-themes-0.5.0rc1/src/wagtail_themes.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -5,46 +5,60 @@
 setup.py
 src/wagtail_themes.egg-info/PKG-INFO
 src/wagtail_themes.egg-info/SOURCES.txt
 src/wagtail_themes.egg-info/dependency_links.txt
 src/wagtail_themes.egg-info/requires.txt
 src/wagtail_themes.egg-info/top_level.txt
 src/wagtailthemes/__init__.py
+src/wagtailthemes/cache.py
+src/wagtailthemes/forms.py
 src/wagtailthemes/loaders.py
 src/wagtailthemes/middleware.py
 src/wagtailthemes/models.py
+src/wagtailthemes/settings.py
+src/wagtailthemes/storage.py
 src/wagtailthemes/thread.py
+src/wagtailthemes/utils.py
+src/wagtailthemes/views.py
+src/wagtailthemes/wagtail_hooks.py
 src/wagtailthemes/__pycache__/__init__.cpython-39.pyc
 src/wagtailthemes/__pycache__/cache.cpython-39.pyc
 src/wagtailthemes/__pycache__/forms.cpython-39.pyc
 src/wagtailthemes/__pycache__/loaders.cpython-39.pyc
 src/wagtailthemes/__pycache__/middleware.cpython-39.pyc
 src/wagtailthemes/__pycache__/models.cpython-39.pyc
 src/wagtailthemes/__pycache__/settings.cpython-39.pyc
 src/wagtailthemes/__pycache__/storage.cpython-39.pyc
 src/wagtailthemes/__pycache__/thread.cpython-39.pyc
 src/wagtailthemes/__pycache__/utils.cpython-39.pyc
 src/wagtailthemes/__pycache__/views.cpython-39.pyc
 src/wagtailthemes/__pycache__/wagtail_hooks.cpython-39.pyc
+src/wagtailthemes/contrib/__init__.py
 src/wagtailthemes/contrib/__pycache__/__init__.cpython-39.pyc
+src/wagtailthemes/contrib/aws/__init__.py
+src/wagtailthemes/contrib/aws/storage.py
 src/wagtailthemes/contrib/aws/__pycache__/__init__.cpython-39.pyc
 src/wagtailthemes/contrib/aws/__pycache__/storage.cpython-39.pyc
+src/wagtailthemes/management/commands/import_theme.py
 src/wagtailthemes/management/commands/__pycache__/import_theme.cpython-39.pyc
 src/wagtailthemes/migrations/0001_initial.py
 src/wagtailthemes/migrations/0002_auto_20161124_1107.py
+src/wagtailthemes/migrations/0003_auto_20220829_1431.py
 src/wagtailthemes/migrations/__init__.py
 src/wagtailthemes/migrations/__pycache__/0001_initial.cpython-39.pyc
 src/wagtailthemes/migrations/__pycache__/0002_auto_20161124_1107.cpython-39.pyc
 src/wagtailthemes/migrations/__pycache__/0003_auto_20220829_1325.cpython-39.pyc
 src/wagtailthemes/migrations/__pycache__/0003_auto_20220829_1339.cpython-39.pyc
 src/wagtailthemes/migrations/__pycache__/0003_auto_20220829_1350.cpython-39.pyc
 src/wagtailthemes/migrations/__pycache__/0003_auto_20220829_1431.cpython-39.pyc
-src/wagtailthemes/migrations/__pycache__/0004_auto_20220830_1603.cpython-39.pyc
-src/wagtailthemes/migrations/__pycache__/0005_alter_staticfile_id_alter_template_id_alter_theme_id.cpython-39.pyc
 src/wagtailthemes/migrations/__pycache__/__init__.cpython-39.pyc
+src/wagtailthemes/templates/wagtailthemes/export_theme.html
+src/wagtailthemes/templates/wagtailthemes/import_theme.html
+src/wagtailthemes/templatetags/__init__.py
+src/wagtailthemes/templatetags/themes.py
 src/wagtailthemes/templatetags/__pycache__/__init__.cpython-39.pyc
 src/wagtailthemes/templatetags/__pycache__/theme.cpython-39.pyc
 src/wagtailthemes/templatetags/__pycache__/themes.cpython-39.pyc
 src/wagtailthemes/tests/__init__.py
 src/wagtailthemes/tests/conftest.py
 src/wagtailthemes/tests/settings.py
 src/wagtailthemes/tests/urls.py
@@ -57,13 +71,14 @@
 src/wagtailthemes/tests/integration/__pycache__/__init__.cpython-39.pyc
 src/wagtailthemes/tests/integration/__pycache__/test_middleware.cpython-39-pytest-7.1.2.pyc
 src/wagtailthemes/tests/templates/base.html
 src/wagtailthemes/tests/templates/page.html
 src/wagtailthemes/tests/templates/brand/base.html
 src/wagtailthemes/tests/templates/themes/brand/base.html
 src/wagtailthemes/tests/unit/__init__.py
+src/wagtailthemes/tests/unit/test_cache.py
 src/wagtailthemes/tests/unit/test_loader.py
 src/wagtailthemes/tests/unit/test_thread.py
 src/wagtailthemes/tests/unit/__pycache__/__init__.cpython-39.pyc
 src/wagtailthemes/tests/unit/__pycache__/test_cache.cpython-39-pytest-7.1.2.pyc
 src/wagtailthemes/tests/unit/__pycache__/test_loader.cpython-39-pytest-7.1.2.pyc
 src/wagtailthemes/tests/unit/__pycache__/test_thread.cpython-39-pytest-7.1.2.pyc
```

### Comparing `wagtail-themes-0.5.0/src/wagtailthemes/__pycache__/cache.cpython-39.pyc` & `wagtail-themes-0.5.0rc1/src/wagtailthemes/__pycache__/cache.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `wagtail-themes-0.5.0/src/wagtailthemes/__pycache__/forms.cpython-39.pyc` & `wagtail-themes-0.5.0rc1/src/wagtailthemes/__pycache__/forms.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `wagtail-themes-0.5.0/src/wagtailthemes/__pycache__/loaders.cpython-39.pyc` & `wagtail-themes-0.5.0rc1/src/wagtailthemes/__pycache__/middleware.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri Dec  2 10:24:09 2022 UTC, .py size: 927 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 27% similar despite different names*

```diff
@@ -1,78 +1,71 @@
-00000000: 610d 0d0a 0000 0000 49d2 8963 9f03 0000  a.......I..c....
+00000000: 610d 0d0a 0000 0000 457d 0c63 0203 0000  a.......E}.c....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 4000 0000 6400  .....@...s@...d.
+00000020: 0003 0000 0040 0000 0073 5400 0000 6400  .....@...sT...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
-00000040: 0100 6400 6403 6c03 6d04 5a05 0100 6400  ..d.d.l.m.Z...d.
-00000050: 6404 6c06 6d07 5a07 0100 4700 6405 6406  d.l.m.Z...G.d.d.
-00000060: 8400 6406 6505 8303 5a08 6401 5300 2907  ..d.e...Z.d.S.).
-00000070: e900 0000 004e 2901 da08 7365 7474 696e  .....N)...settin
-00000080: 6773 2901 da06 4c6f 6164 6572 2901 da09  gs)...Loader)...
-00000090: 6765 745f 7468 656d 6563 0000 0000 0000  get_themec......
-000000a0: 0000 0000 0000 0000 0000 0300 0000 0000  ................
-000000b0: 0000 7320 0000 0065 005a 0164 005a 0264  ..s ...e.Z.d.Z.d
-000000c0: 015a 0387 0066 0164 0264 0384 085a 0487  .Z...f.d.d...Z..
-000000d0: 0004 005a 0553 0029 04da 0b54 6865 6d65  ...Z.S.)...Theme
-000000e0: 4c6f 6164 6572 7a53 0a20 2020 2054 6865  LoaderzS.    The
-000000f0: 6d65 2074 656d 706c 6174 6520 4c6f 6164  me template Load
-00000100: 6572 2063 6c61 7373 2066 6f72 2073 6572  er class for ser
-00000110: 7669 6e67 206f 7074 696f 6e61 6c20 7468  ving optional th
-00000120: 656d 6573 2070 6572 2057 6167 7461 696c  emes per Wagtail
-00000130: 2073 6974 652e 0a20 2020 2063 0100 0000   site..    c....
-00000140: 0000 0000 0000 0000 0300 0000 0400 0000  ................
-00000150: 0300 0000 7358 0000 0074 0074 017c 0083  ....sX...t.t.|..
-00000160: 02a0 02a1 007d 0174 0383 0089 0074 0474  .....}.t.....t.t
-00000170: 0564 0164 0083 0389 0188 0072 5488 0172  .d.d.......rT..r
-00000180: 3e87 0087 0166 0264 0264 0384 087c 0144  >....f.d.d...|.D
-00000190: 0083 017d 026e 1287 0066 0164 0464 0384  ...}.n...f.d.d..
-000001a0: 087c 0144 0083 017d 027c 0253 007c 0153  .|.D...}.|.S.|.S
-000001b0: 0029 054e da12 5741 4754 4149 4c5f 5448  .).N..WAGTAIL_TH
-000001c0: 454d 455f 5041 5448 6301 0000 0000 0000  EME_PATHc.......
-000001d0: 0000 0000 0002 0000 0007 0000 0013 0000  ................
-000001e0: 0073 1c00 0000 6700 7c00 5d14 7d01 7400  .s....g.|.].}.t.
-000001f0: 6a01 a002 7c01 8801 8800 a103 9102 7104  j...|.........q.
-00000200: 5300 a900 a903 da02 6f73 da04 7061 7468  S.......os..path
-00000210: da04 6a6f 696e a902 da02 2e30 da03 6469  ..join.....0..di
-00000220: 72a9 02da 0574 6865 6d65 5a0a 7468 656d  r....themeZ.them
-00000230: 655f 7061 7468 7207 0000 00fa 562f 5573  e_pathr.....V/Us
-00000240: 6572 732f 726f 626d 6f6f 726d 616e 2f44  ers/robmoorman/D
-00000250: 6576 656c 6f70 6572 2f67 6974 6875 622f  eveloper/github/
-00000260: 6d6f 6f72 696e 6c2f 7761 6774 6169 6c2d  moorinl/wagtail-
-00000270: 7468 656d 6573 2f73 7263 2f77 6167 7461  themes/src/wagta
-00000280: 696c 7468 656d 6573 2f6c 6f61 6465 7273  ilthemes/loaders
-00000290: 2e70 79da 0a3c 6c69 7374 636f 6d70 3e15  .py..<listcomp>.
-000002a0: 0000 0073 0200 0000 0601 7a28 5468 656d  ...s......z(Them
-000002b0: 654c 6f61 6465 722e 6765 745f 6469 7273  eLoader.get_dirs
-000002c0: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
-000002d0: 6f6d 703e 6301 0000 0000 0000 0000 0000  omp>c...........
-000002e0: 0002 0000 0006 0000 0013 0000 0073 1a00  .............s..
-000002f0: 0000 6700 7c00 5d12 7d01 7400 6a01 a002  ..g.|.].}.t.j...
-00000300: 7c01 8800 a102 9102 7104 5300 7207 0000  |.......q.S.r...
-00000310: 0072 0800 0000 720c 0000 0029 0172 1000  .r....r....).r..
-00000320: 0000 7207 0000 0072 1100 0000 7212 0000  ..r....r....r...
-00000330: 001a 0000 00f3 0000 0000 2906 da05 7375  ..........)...su
-00000340: 7065 7272 0500 0000 da08 6765 745f 6469  perr......get_di
-00000350: 7273 7204 0000 00da 0767 6574 6174 7472  rsr......getattr
-00000360: 7202 0000 0029 03da 0473 656c 66da 0464  r....)...self..d
-00000370: 6972 735a 0a74 6865 6d65 5f64 6972 73a9  irsZ.theme_dirs.
-00000380: 01da 095f 5f63 6c61 7373 5f5f 720f 0000  ...__class__r...
-00000390: 0072 1100 0000 7215 0000 000d 0000 0073  .r....r........s
-000003a0: 1600 0000 0001 0e01 0601 0c02 0401 0402  ................
-000003b0: 0c01 02ff 0805 1201 0402 7a14 5468 656d  ..........z.Them
-000003c0: 654c 6f61 6465 722e 6765 745f 6469 7273  eLoader.get_dirs
-000003d0: 2906 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
-000003e0: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
-000003f0: 6e61 6d65 5f5f da07 5f5f 646f 635f 5f72  name__..__doc__r
-00000400: 1500 0000 da0d 5f5f 636c 6173 7363 656c  ......__classcel
-00000410: 6c5f 5f72 0700 0000 7207 0000 0072 1900  l__r....r....r..
-00000420: 0000 7211 0000 0072 0500 0000 0900 0000  ..r....r........
-00000430: 7304 0000 0008 0104 0372 0500 0000 2909  s........r....).
-00000440: 7209 0000 00da 0b64 6a61 6e67 6f2e 636f  r......django.co
-00000450: 6e66 7202 0000 005a 2264 6a61 6e67 6f2e  nfr....Z"django.
-00000460: 7465 6d70 6c61 7465 2e6c 6f61 6465 7273  template.loaders
-00000470: 2e66 696c 6573 7973 7465 6d72 0300 0000  .filesystemr....
-00000480: da0a 4261 7365 4c6f 6164 6572 5a14 7761  ..BaseLoaderZ.wa
-00000490: 6774 6169 6c74 6865 6d65 732e 7468 7265  gtailthemes.thre
-000004a0: 6164 7204 0000 0072 0500 0000 7207 0000  adr....r....r...
-000004b0: 0072 0700 0000 7207 0000 0072 1100 0000  .r....r....r....
-000004c0: da08 3c6d 6f64 756c 653e 0100 0000 7308  ..<module>....s.
-000004d0: 0000 0008 020c 010c 020c 03              ...........
+00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
+00000050: 6404 6c05 6d06 5a06 0100 6400 6405 6c07  d.l.m.Z...d.d.l.
+00000060: 6d08 5a08 0100 6500 a009 650a a101 5a0b  m.Z...e...e...Z.
+00000070: 4700 6406 6407 8400 6407 8302 5a0c 6401  G.d.d...d...Z.d.
+00000080: 5300 2908 e900 0000 004e 2901 da14 496d  S.)......N)...Im
+00000090: 7072 6f70 6572 6c79 436f 6e66 6967 7572  properlyConfigur
+000000a0: 6564 2901 da04 5369 7465 2901 da0d 5468  ed)...Site)...Th
+000000b0: 656d 6553 6574 7469 6e67 7329 01da 0973  emeSettings)...s
+000000c0: 6574 5f74 6865 6d65 6300 0000 0000 0000  et_themec.......
+000000d0: 0000 0000 0000 0000 0002 0000 0040 0000  .............@..
+000000e0: 0073 1c00 0000 6500 5a01 6400 5a02 6401  .s....e.Z.d.Z.d.
+000000f0: 6402 8400 5a03 6403 6404 8400 5a04 6405  d...Z.d.d...Z.d.
+00000100: 5300 2906 da0f 5468 656d 654d 6964 646c  S.)...ThemeMiddl
+00000110: 6577 6172 6563 0200 0000 0000 0000 0000  ewarec..........
+00000120: 0000 0200 0000 0200 0000 4300 0000 730a  ..........C...s.
+00000130: 0000 007c 017c 005f 0064 0053 0029 014e  ...|.|._.d.S.).N
+00000140: 2901 da0c 6765 745f 7265 7370 6f6e 7365  )...get_response
+00000150: 2902 da04 7365 6c66 7207 0000 00a9 0072  )...selfr......r
+00000160: 0900 0000 fa59 2f55 7365 7273 2f72 6f62  .....Y/Users/rob
+00000170: 6d6f 6f72 6d61 6e2f 4465 7665 6c6f 7065  moorman/Develope
+00000180: 722f 6769 7468 7562 2f6d 6f6f 7269 6e6c  r/github/moorinl
+00000190: 2f77 6167 7461 696c 2d74 6865 6d65 732f  /wagtail-themes/
+000001a0: 7372 632f 7761 6774 6169 6c74 6865 6d65  src/wagtailtheme
+000001b0: 732f 6d69 6464 6c65 7761 7265 2e70 79da  s/middleware.py.
+000001c0: 085f 5f69 6e69 745f 5f0d 0000 0073 0200  .__init__....s..
+000001d0: 0000 0001 7a18 5468 656d 654d 6964 646c  ....z.ThemeMiddl
+000001e0: 6577 6172 652e 5f5f 696e 6974 5f5f 6302  eware.__init__c.
+000001f0: 0000 0000 0000 0000 0000 0006 0000 0003  ................
+00000200: 0000 0043 0000 0073 5400 0000 7400 a001  ...C...sT...t...
+00000210: 7c01 a101 7d02 7c02 6400 7500 721a 7402  |...}.|.d.u.r.t.
+00000220: 6401 8301 8201 7403 a004 7c02 a101 7d03  d.....t...|...}.
+00000230: 7c03 6a05 7232 7c03 6a05 6a06 6e02 6402  |.j.r2|.j.j.n.d.
+00000240: 7d04 7c04 6400 7501 7246 7407 7c04 8301  }.|.d.u.rFt.|...
+00000250: 0100 7c00 a008 7c01 a101 7d05 7c05 5300  ..|...|...}.|.S.
+00000260: 2903 4e7a 0f53 6974 6520 6e6f 7420 666f  ).Nz.Site not fo
+00000270: 756e 6421 da00 2909 7203 0000 00da 1066  und!..).r......f
+00000280: 696e 645f 666f 725f 7265 7175 6573 7472  ind_for_requestr
+00000290: 0200 0000 7204 0000 00da 0866 6f72 5f73  ....r......for_s
+000002a0: 6974 65da 0574 6865 6d65 da08 7061 7468  ite..theme..path
+000002b0: 6e61 6d65 7205 0000 0072 0700 0000 2906  namer....r....).
+000002c0: 7208 0000 00da 0772 6571 7565 7374 da04  r......request..
+000002d0: 7369 7465 5a0e 7468 656d 655f 7365 7474  siteZ.theme_sett
+000002e0: 696e 6773 720f 0000 00da 0872 6573 706f  ingsr......respo
+000002f0: 6e73 6572 0900 0000 7209 0000 0072 0a00  nser....r....r..
+00000300: 0000 da08 5f5f 6361 6c6c 5f5f 1000 0000  ....__call__....
+00000310: 7312 0000 0000 010a 0208 0108 020a 0112  s...............
+00000320: 0208 0108 020a 017a 1854 6865 6d65 4d69  .......z.ThemeMi
+00000330: 6464 6c65 7761 7265 2e5f 5f63 616c 6c5f  ddleware.__call_
+00000340: 5f4e 2905 da08 5f5f 6e61 6d65 5f5f da0a  _N)...__name__..
+00000350: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
+00000360: 616c 6e61 6d65 5f5f 720b 0000 0072 1400  alname__r....r..
+00000370: 0000 7209 0000 0072 0900 0000 7209 0000  ..r....r....r...
+00000380: 0072 0a00 0000 7206 0000 000c 0000 0073  .r....r........s
+00000390: 0400 0000 0801 0803 7206 0000 0029 0dda  ........r....)..
+000003a0: 076c 6f67 6769 6e67 da16 646a 616e 676f  .logging..django
+000003b0: 2e63 6f72 652e 6578 6365 7074 696f 6e73  .core.exceptions
+000003c0: 7202 0000 00da 1377 6167 7461 696c 2e63  r......wagtail.c
+000003d0: 6f72 652e 6d6f 6465 6c73 7203 0000 00da  ore.modelsr.....
+000003e0: 1477 6167 7461 696c 7468 656d 6573 2e6d  .wagtailthemes.m
+000003f0: 6f64 656c 7372 0400 0000 da14 7761 6774  odelsr......wagt
+00000400: 6169 6c74 6865 6d65 732e 7468 7265 6164  ailthemes.thread
+00000410: 7205 0000 00da 0967 6574 4c6f 6767 6572  r......getLogger
+00000420: 7215 0000 00da 066c 6f67 6765 7272 0600  r......loggerr..
+00000430: 0000 7209 0000 0072 0900 0000 7209 0000  ..r....r....r...
+00000440: 0072 0a00 0000 da08 3c6d 6f64 756c 653e  .r......<module>
+00000450: 0100 0000 730c 0000 0008 020c 010c 020c  ....s...........
+00000460: 010c 020a 03                             .....
```

### Comparing `wagtail-themes-0.5.0/src/wagtailthemes/__pycache__/models.cpython-39.pyc` & `wagtail-themes-0.5.0rc1/src/wagtailthemes/migrations/__pycache__/0001_initial.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri Dec  2 10:27:49 2022 UTC, .py size: 958 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,83 +1,65 @@
-00000000: 610d 0d0a 0000 0000 25d3 8963 be03 0000  a.......%..c....
+00000000: 610d 0d0a 0000 0000 49be 0c63 b504 0000  a.......I..c....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0005 0000 0040 0000 0073 9400 0000 6400  .....@...s....d.
+00000020: 0004 0000 0040 0000 0073 3a00 0000 6400  .....@...s:...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
-00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
-00000050: 0100 6400 6404 6c06 6d07 5a08 0100 6400  ..d.d.l.m.Z...d.
-00000060: 6405 6c09 6d0a 5a0b 0100 6400 6406 6c0c  d.l.m.Z...d.d.l.
-00000070: 6d0d 5a0d 0100 6400 6407 6c0e 6d0f 5a0f  m.Z...d.d.l.m.Z.
-00000080: 0100 650b 6408 6b00 726a 6400 6409 6c0e  ..e.d.k.rjd.d.l.
-00000090: 6d10 5a10 0100 6e0c 6400 640a 6c0e 6d11  m.Z...n.d.d.l.m.
-000000a0: 5a10 0100 640b 6701 5a12 650f 4700 640c  Z...d.g.Z.e.G.d.
-000000b0: 640b 8400 640b 6510 8303 8301 5a13 640d  d...d.e.....Z.d.
-000000c0: 5300 290e e900 0000 0029 01da 0566 6f72  S.)......)...for
-000000d0: 6d73 2901 da08 7365 7474 696e 6773 2901  ms)...settings).
-000000e0: da06 6d6f 6465 6c73 2901 da07 6765 7474  ..models)...gett
-000000f0: 6578 7429 01da 0756 4552 5349 4f4e 2901  ext)...VERSION).
-00000100: da0a 4669 656c 6450 616e 656c 2901 da10  ..FieldPanel)...
-00000110: 7265 6769 7374 6572 5f73 6574 7469 6e67  register_setting
-00000120: 2902 e904 0000 0072 0100 0000 2901 da0b  )......r....)...
-00000130: 4261 7365 5365 7474 696e 6729 01da 0f42  BaseSetting)...B
-00000140: 6173 6553 6974 6553 6574 7469 6e67 da0d  aseSiteSetting..
-00000150: 5468 656d 6553 6574 7469 6e67 7363 0000  ThemeSettingsc..
-00000160: 0000 0000 0000 0000 0000 0000 0000 0600  ................
-00000170: 0000 4000 0000 735e 0000 0065 005a 0164  ..@...s^...e.Z.d
-00000180: 005a 0265 0365 0464 0164 0283 035a 0565  .Z.e.e.d.d...Z.e
-00000190: 066a 0764 0364 0364 0464 0564 068d 045a  .j.d.d.d.d.d...Z
-000001a0: 0865 066a 0964 0364 0764 0364 088d 035a  .e.j.d.d.d.d...Z
-000001b0: 0a65 0b64 0965 0c6a 0d65 0564 0a8d 0164  .e.d.e.j.e.d...d
-000001c0: 0b8d 0267 015a 0e47 0064 0c64 0d84 0064  ...g.Z.G.d.d...d
-000001d0: 0d83 025a 0f64 0253 0029 0e72 0c00 0000  ...Z.d.S.).r....
-000001e0: da0e 5741 4754 4149 4c5f 5448 454d 4553  ..WAGTAIL_THEMES
-000001f0: 4e54 46da 0249 4429 04da 0c61 7574 6f5f  NTF..ID)...auto_
-00000200: 6372 6561 7465 64da 0b70 7269 6d61 7279  created..primary
-00000210: 5f6b 6579 da09 7365 7269 616c 697a 65da  _key..serialize.
-00000220: 0c76 6572 626f 7365 5f6e 616d 65e9 ff00  .verbose_name...
-00000230: 0000 2903 da05 626c 616e 6bda 0a6d 6178  ..)...blank..max
-00000240: 5f6c 656e 6774 68da 046e 756c 6cda 0574  _length..null..t
-00000250: 6865 6d65 2901 da07 6368 6f69 6365 7329  heme)...choices)
-00000260: 01da 0677 6964 6765 7463 0000 0000 0000  ...widgetc......
-00000270: 0000 0000 0000 0000 0000 0200 0000 4000  ..............@.
-00000280: 0000 731c 0000 0065 005a 0164 005a 0265  ..s....e.Z.d.Z.e
-00000290: 0364 0183 015a 0465 0364 0183 015a 0564  .d...Z.e.d...Z.d
-000002a0: 0253 0029 037a 1254 6865 6d65 5365 7474  .S.).z.ThemeSett
-000002b0: 696e 6773 2e4d 6574 61da 0674 6865 6d65  ings.Meta..theme
-000002c0: 734e 2906 da08 5f5f 6e61 6d65 5f5f da0a  sN)...__name__..
-000002d0: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
-000002e0: 616c 6e61 6d65 5f5f da01 5f72 1200 0000  alname__.._r....
-000002f0: da13 7665 7262 6f73 655f 6e61 6d65 5f70  ..verbose_name_p
-00000300: 6c75 7261 6ca9 0072 2000 0000 7220 0000  lural..r ...r ..
-00000310: 00fa 552f 5573 6572 732f 726f 626d 6f6f  ..U/Users/robmoo
-00000320: 726d 616e 2f44 6576 656c 6f70 6572 2f67  rman/Developer/g
-00000330: 6974 6875 622f 6d6f 6f72 696e 6c2f 7761  ithub/moorinl/wa
-00000340: 6774 6169 6c2d 7468 656d 6573 2f73 7263  gtail-themes/src
-00000350: 2f77 6167 7461 696c 7468 656d 6573 2f6d  /wagtailthemes/m
-00000360: 6f64 656c 732e 7079 da04 4d65 7461 1c00  odels.py..Meta..
-00000370: 0000 7304 0000 0008 0108 0172 2200 0000  ..s........r"...
-00000380: 2910 721b 0000 0072 1c00 0000 721d 0000  ).r....r....r...
-00000390: 00da 0767 6574 6174 7472 7203 0000 005a  ...getattrr....Z
-000003a0: 0654 4845 4d45 5372 0400 0000 da09 4175  .THEMESr......Au
-000003b0: 746f 4669 656c 64da 0269 64da 0943 6861  toField..id..Cha
-000003c0: 7246 6965 6c64 7217 0000 0072 0700 0000  rFieldr....r....
-000003d0: 7202 0000 00da 0653 656c 6563 74da 0670  r......Select..p
-000003e0: 616e 656c 7372 2200 0000 7220 0000 0072  anelsr"...r ...r
-000003f0: 2000 0000 7220 0000 0072 2100 0000 720c   ...r ...r!...r.
-00000400: 0000 0011 0000 0073 0e00 0000 0802 0c02  .......s........
-00000410: 0401 08ff 0603 1002 1602 4e29 14da 0664  ..........N)...d
-00000420: 6a61 6e67 6f72 0200 0000 da0b 646a 616e  jangor......djan
-00000430: 676f 2e63 6f6e 6672 0300 0000 da09 646a  go.confr......dj
-00000440: 616e 676f 2e64 6272 0400 0000 da18 646a  ango.dbr......dj
-00000450: 616e 676f 2e75 7469 6c73 2e74 7261 6e73  ango.utils.trans
-00000460: 6c61 7469 6f6e 7205 0000 0072 1e00 0000  lationr....r....
-00000470: da07 7761 6774 6169 6c72 0600 0000 5a0f  ..wagtailr....Z.
-00000480: 5741 4754 4149 4c5f 5645 5253 494f 4eda  WAGTAIL_VERSION.
-00000490: 1b77 6167 7461 696c 2e61 646d 696e 2e65  .wagtail.admin.e
-000004a0: 6469 745f 6861 6e64 6c65 7273 7207 0000  dit_handlersr...
-000004b0: 005a 1f77 6167 7461 696c 2e63 6f6e 7472  .Z.wagtail.contr
-000004c0: 6962 2e73 6574 7469 6e67 732e 6d6f 6465  ib.settings.mode
-000004d0: 6c73 7208 0000 0072 0a00 0000 720b 0000  lsr....r....r...
-000004e0: 00da 075f 5f41 4c4c 5f5f 720c 0000 0072  ...__ALL__r....r
-000004f0: 2000 0000 7220 0000 0072 2000 0000 7221   ...r ...r ...r!
-00000500: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-00000510: 0073 1800 0000 0c01 0c01 0c01 0c01 0c01  .s..............
-00000520: 0c01 0c02 0801 0e02 0c02 0603 0201       ..............
+00000040: 5a03 6400 6403 6c04 6d05 5a05 6d06 5a06  Z.d.d.l.m.Z.m.Z.
+00000050: 0100 4700 6404 6405 8400 6405 6505 6a07  ..G.d.d...d.e.j.
+00000060: 8303 5a07 6402 5300 2906 e900 0000 0029  ..Z.d.S.)......)
+00000070: 01da 1075 6e69 636f 6465 5f6c 6974 6572  ...unicode_liter
+00000080: 616c 734e 2902 da0a 6d69 6772 6174 696f  alsN)...migratio
+00000090: 6e73 da06 6d6f 6465 6c73 6300 0000 0000  ns..modelsc.....
+000000a0: 0000 0000 0000 0000 0000 000a 0000 0040  ...............@
+000000b0: 0000 0073 6c00 0000 6500 5a01 6400 5a02  ...sl...e.Z.d.Z.
+000000c0: 6401 5a03 6402 6701 5a04 6505 6a06 6403  d.Z.d.g.Z.e.j.d.
+000000d0: 6404 6507 6a08 6401 6401 6405 6406 6407  d.e.j.d.d.d.d.d.
+000000e0: 8d04 6602 6408 6507 6a09 6401 6409 6401  ..f.d.e.j.d.d.d.
+000000f0: 640a 8d03 6602 640b 6507 6a0a 6405 650b  d...f.d.e.j.d.e.
+00000100: 6a0c 6a07 6a0d 6a0e 640c 640d 8d03 6602  j.j.j.j.d.d...f.
+00000110: 6703 640e 6405 6901 640f 8d03 6701 5a0f  g.d.d.i.d...g.Z.
+00000120: 6410 5300 2911 da09 4d69 6772 6174 696f  d.S.)...Migratio
+00000130: 6e54 2902 da0b 7761 6774 6169 6c63 6f72  nT)...wagtailcor
+00000140: 65da 1b30 3032 395f 756e 6963 6f64 655f  e..0029_unicode_
+00000150: 736c 7567 6669 656c 645f 646a 3139 da0d  slugfield_dj19..
+00000160: 5468 656d 6553 6574 7469 6e67 73da 0269  ThemeSettings..i
+00000170: 6446 da02 4944 2904 da0c 6175 746f 5f63  dF..ID)...auto_c
+00000180: 7265 6174 6564 da0b 7072 696d 6172 795f  reated..primary_
+00000190: 6b65 79da 0973 6572 6961 6c69 7a65 da0c  key..serialize..
+000001a0: 7665 7262 6f73 655f 6e61 6d65 da05 7468  verbose_name..th
+000001b0: 656d 65e9 ff00 0000 2903 da05 626c 616e  eme.....)...blan
+000001c0: 6bda 0a6d 6178 5f6c 656e 6774 68da 046e  k..max_length..n
+000001d0: 756c 6cda 0473 6974 657a 1077 6167 7461  ull..sitez.wagta
+000001e0: 696c 636f 7265 2e53 6974 6529 03da 0865  ilcore.Site)...e
+000001f0: 6469 7461 626c 65da 096f 6e5f 6465 6c65  ditable..on_dele
+00000200: 7465 da02 746f da08 6162 7374 7261 6374  te..to..abstract
+00000210: 2903 da04 6e61 6d65 da06 6669 656c 6473  )...name..fields
+00000220: da07 6f70 7469 6f6e 734e 2910 da08 5f5f  ..optionsN)...__
+00000230: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
+00000240: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
+00000250: da07 696e 6974 6961 6cda 0c64 6570 656e  ..initial..depen
+00000260: 6465 6e63 6965 7372 0300 0000 da0b 4372  denciesr......Cr
+00000270: 6561 7465 4d6f 6465 6c72 0400 0000 da09  eateModelr......
+00000280: 4175 746f 4669 656c 64da 0943 6861 7246  AutoField..CharF
+00000290: 6965 6c64 da0d 4f6e 6554 6f4f 6e65 4669  ield..OneToOneFi
+000002a0: 656c 64da 0664 6a61 6e67 6fda 0264 62da  eld..django..db.
+000002b0: 0864 656c 6574 696f 6eda 0743 4153 4341  .deletion..CASCA
+000002c0: 4445 da0a 6f70 6572 6174 696f 6e73 a900  DE..operations..
+000002d0: 722a 0000 0072 2a00 0000 fa66 2f55 7365  r*...r*....f/Use
+000002e0: 7273 2f72 6f62 6d6f 6f72 6d61 6e2f 4465  rs/robmoorman/De
+000002f0: 7665 6c6f 7065 722f 6769 7468 7562 2f6d  veloper/github/m
+00000300: 6f6f 7269 6e6c 2f77 6167 7461 696c 2d74  oorinl/wagtail-t
+00000310: 6865 6d65 732f 7372 632f 7761 6774 6169  hemes/src/wagtai
+00000320: 6c74 6865 6d65 732f 6d69 6772 6174 696f  lthemes/migratio
+00000330: 6e73 2f30 3030 315f 696e 6974 6961 6c2e  ns/0001_initial.
+00000340: 7079 7205 0000 0009 0000 0073 3400 0000  pyr........s4...
+00000350: 0802 0403 02ff 0405 0401 0203 0201 0401  ................
+00000360: 0201 0201 0201 02fc 04fe 0209 1202 0201  ................
+00000370: 0401 0201 0a01 02fd 04fe 02f5 0215 04ff  ................
+00000380: 02ea 04ff 7205 0000 0029 08da 0a5f 5f66  ....r....)...__f
+00000390: 7574 7572 655f 5f72 0200 0000 da19 646a  uture__r......dj
+000003a0: 616e 676f 2e64 622e 6d6f 6465 6c73 2e64  ango.db.models.d
+000003b0: 656c 6574 696f 6e72 2500 0000 da09 646a  eletionr%.....dj
+000003c0: 616e 676f 2e64 6272 0300 0000 7204 0000  ango.dbr....r...
+000003d0: 0072 0500 0000 722a 0000 0072 2a00 0000  .r....r*...r*...
+000003e0: 722a 0000 0072 2b00 0000 da08 3c6d 6f64  r*...r+.....<mod
+000003f0: 756c 653e 0300 0000 7306 0000 000c 0208  ule>....s.......
+00000400: 0110 03                                  ...
```

### Comparing `wagtail-themes-0.5.0/src/wagtailthemes/__pycache__/settings.cpython-39.pyc` & `wagtail-themes-0.5.0rc1/src/wagtailthemes/__pycache__/settings.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `wagtail-themes-0.5.0/src/wagtailthemes/__pycache__/storage.cpython-39.pyc` & `wagtail-themes-0.5.0rc1/src/wagtailthemes/__pycache__/storage.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `wagtail-themes-0.5.0/src/wagtailthemes/__pycache__/thread.cpython-39.pyc` & `wagtail-themes-0.5.0rc1/src/wagtailthemes/__pycache__/thread.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri Dec  2 10:24:09 2022 UTC, .py size: 225 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 49d2 8963 e100 0000  a.......I..c....
+00000000: 610d 0d0a 0000 0000 49be 0c63 e100 0000  a.......I..c....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
 00000030: 6401 6c00 6d01 5a01 0100 6501 8300 5a02  d.l.m.Z...e...Z.
 00000040: 6402 6403 8400 5a03 6404 6405 8400 5a04  d.d...Z.d.d...Z.
 00000050: 6406 5300 2907 e900 0000 0029 01da 056c  d.S.)......)...l
 00000060: 6f63 616c 6301 0000 0000 0000 0000 0000  ocalc...........
 00000070: 0001 0000 0004 0000 0043 0000 0073 1000  .........C...s..
```

### Comparing `wagtail-themes-0.5.0/src/wagtailthemes/__pycache__/utils.cpython-39.pyc` & `wagtail-themes-0.5.0rc1/src/wagtailthemes/__pycache__/utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `wagtail-themes-0.5.0/src/wagtailthemes/__pycache__/views.cpython-39.pyc` & `wagtail-themes-0.5.0rc1/src/wagtailthemes/__pycache__/views.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `wagtail-themes-0.5.0/src/wagtailthemes/__pycache__/wagtail_hooks.cpython-39.pyc` & `wagtail-themes-0.5.0rc1/src/wagtailthemes/__pycache__/wagtail_hooks.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `wagtail-themes-0.5.0/src/wagtailthemes/contrib/aws/__pycache__/storage.cpython-39.pyc` & `wagtail-themes-0.5.0rc1/src/wagtailthemes/contrib/aws/__pycache__/storage.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `wagtail-themes-0.5.0/src/wagtailthemes/management/commands/__pycache__/import_theme.cpython-39.pyc` & `wagtail-themes-0.5.0rc1/src/wagtailthemes/management/commands/__pycache__/import_theme.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `wagtail-themes-0.5.0/src/wagtailthemes/middleware.py` & `wagtail-themes-0.5.0rc1/src/wagtailthemes/middleware.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,29 @@
+import logging
+
 from django.core.exceptions import ImproperlyConfigured
-from wagtail.models import Site
+from wagtail.core.models import Site
 
 from wagtailthemes.models import ThemeSettings
 from wagtailthemes.thread import set_theme
 
+logger = logging.getLogger(__name__)
+
 
 class ThemeMiddleware:
     def __init__(self, get_response):
         self.get_response = get_response
 
     def __call__(self, request):
         site = Site.find_for_request(request)
 
         if site is None:
             raise ImproperlyConfigured("Site not found!")
 
         theme_settings = ThemeSettings.for_site(site)
-        theme = theme_settings.theme
+        theme = theme_settings.theme.pathname if theme_settings.theme else ""
 
         if theme is not None:
             set_theme(theme)
 
         response = self.get_response(request)
         return response
```

### Comparing `wagtail-themes-0.5.0/src/wagtailthemes/migrations/__pycache__/0002_auto_20161124_1107.cpython-39.pyc` & `wagtail-themes-0.5.0rc1/src/wagtailthemes/migrations/__pycache__/0002_auto_20161124_1107.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri Dec  2 10:24:09 2022 UTC, .py size: 449 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 49d2 8963 c101 0000  a.......I..c....
+00000000: 610d 0d0a 0000 0000 49be 0c63 c101 0000  a.......I..c....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 4700 6403 6404 8400 6404  m.Z...G.d.d...d.
 00000050: 6503 6a04 8303 5a04 6405 5300 2906 e900  e.j...Z.d.S.)...
 00000060: 0000 0029 01da 1075 6e69 636f 6465 5f6c  ...)...unicode_l
 00000070: 6974 6572 616c 7329 01da 0a6d 6967 7261  iterals)...migra
```

### Comparing `wagtail-themes-0.5.0/src/wagtailthemes/migrations/__pycache__/0003_auto_20220829_1325.cpython-39.pyc` & `wagtail-themes-0.5.0rc1/src/wagtailthemes/migrations/__pycache__/0003_auto_20220829_1325.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `wagtail-themes-0.5.0/src/wagtailthemes/migrations/__pycache__/0003_auto_20220829_1339.cpython-39.pyc` & `wagtail-themes-0.5.0rc1/src/wagtailthemes/migrations/__pycache__/0003_auto_20220829_1339.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `wagtail-themes-0.5.0/src/wagtailthemes/migrations/__pycache__/0003_auto_20220829_1350.cpython-39.pyc` & `wagtail-themes-0.5.0rc1/src/wagtailthemes/migrations/__pycache__/0003_auto_20220829_1350.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `wagtail-themes-0.5.0/src/wagtailthemes/migrations/__pycache__/0003_auto_20220829_1431.cpython-39.pyc` & `wagtail-themes-0.5.0rc1/src/wagtailthemes/migrations/__pycache__/0003_auto_20220829_1431.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `wagtail-themes-0.5.0/src/wagtailthemes/templatetags/__pycache__/theme.cpython-39.pyc` & `wagtail-themes-0.5.0rc1/src/wagtailthemes/templatetags/__pycache__/theme.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `wagtail-themes-0.5.0/src/wagtailthemes/templatetags/__pycache__/themes.cpython-39.pyc` & `wagtail-themes-0.5.0rc1/src/wagtailthemes/templatetags/__pycache__/themes.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `wagtail-themes-0.5.0/src/wagtailthemes/tests/__pycache__/conftest.cpython-39-pytest-7.1.2.pyc` & `wagtail-themes-0.5.0rc1/src/wagtailthemes/tests/__pycache__/conftest.cpython-39-pytest-7.1.2.pyc`

 * *Files identical despite different names*

### Comparing `wagtail-themes-0.5.0/src/wagtailthemes/tests/__pycache__/settings.cpython-39.pyc` & `wagtail-themes-0.5.0rc1/src/wagtailthemes/tests/__pycache__/settings.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `wagtail-themes-0.5.0/src/wagtailthemes/tests/integration/__pycache__/test_middleware.cpython-39-pytest-7.1.2.pyc` & `wagtail-themes-0.5.0rc1/src/wagtailthemes/tests/integration/__pycache__/test_middleware.cpython-39-pytest-7.1.2.pyc`

 * *Files identical despite different names*

### Comparing `wagtail-themes-0.5.0/src/wagtailthemes/tests/integration/test_middleware.py` & `wagtail-themes-0.5.0rc1/src/wagtailthemes/tests/integration/test_middleware.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 import pytest
 from django.core.exceptions import ImproperlyConfigured
 from django.test.utils import override_settings
-from wagtail.models import Site
+from wagtail.core.models import Site
 
 from wagtailthemes.thread import get_theme, set_theme
 
 
 @pytest.mark.django_db
 def test_middleware_no_site(client):
-    with override_settings(MIDDLEWARE=[
-        'wagtailthemes.middleware.ThemeMiddleware',
-    ]):
+    with override_settings(
+        MIDDLEWARE=[
+            "wagtailthemes.middleware.ThemeMiddleware",
+        ]
+    ):
         # Remove all sites to simulate not being able to find the site.
         Site.objects.all().delete()
         with pytest.raises(ImproperlyConfigured):
-            client.get('/')
+            client.get("/")
 
 
 @pytest.mark.django_db
 def test_middleware_set_theme_for_site(client, site, settings):
-    settings.theme = 'personal'
+    settings.theme = "personal"
     settings.save()
 
-    set_theme('wagtail')
-    assert get_theme() == 'wagtail'
+    set_theme("wagtail")
+    assert get_theme() == "wagtail"
 
-    client.get('/')
-    assert get_theme() == 'personal'
+    client.get("/")
+    assert get_theme() == "personal"
```

### Comparing `wagtail-themes-0.5.0/src/wagtailthemes/tests/unit/__pycache__/test_cache.cpython-39-pytest-7.1.2.pyc` & `wagtail-themes-0.5.0rc1/src/wagtailthemes/tests/unit/__pycache__/test_cache.cpython-39-pytest-7.1.2.pyc`

 * *Files identical despite different names*

### Comparing `wagtail-themes-0.5.0/src/wagtailthemes/tests/unit/__pycache__/test_loader.cpython-39-pytest-7.1.2.pyc` & `wagtail-themes-0.5.0rc1/src/wagtailthemes/tests/unit/__pycache__/test_loader.cpython-39-pytest-7.1.2.pyc`

 * *Files identical despite different names*

### Comparing `wagtail-themes-0.5.0/src/wagtailthemes/tests/unit/__pycache__/test_thread.cpython-39-pytest-7.1.2.pyc` & `wagtail-themes-0.5.0rc1/src/wagtailthemes/tests/unit/__pycache__/test_thread.cpython-39-pytest-7.1.2.pyc`

 * *Files identical despite different names*

### Comparing `wagtail-themes-0.5.0/src/wagtailthemes/tests/unit/test_loader.py` & `wagtail-themes-0.5.0rc1/src/wagtailthemes/tests/unit/test_loader.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 from django.test.utils import override_settings
 
 from wagtailthemes.thread import set_theme
 
 
 def test_get_dirs_no_theme_set():
     set_theme(None)
-    template = get_template('base.html')
-    assert template.render() == 'Base'
+    template = get_template("base.html")
+    assert template.render() == "Base"
 
 
 @override_settings(WAGTAIL_THEME_PATH=None)
 def test_get_dirs_no_theme_dir():
-    set_theme('brand')
-    template = get_template('base.html')
-    assert template.render() == 'Brand Base'
+    set_theme("brand")
+    template = get_template("base.html")
+    assert template.render() == "Brand Base"
 
 
-@override_settings(WAGTAIL_THEME_PATH='themes')
+@override_settings(WAGTAIL_THEME_PATH="themes")
 def test_get_dirs():
-    set_theme('brand')
-    template = get_template('base.html')
-    assert template.render() == 'Themes Brand Base'
+    set_theme("brand")
+    template = get_template("base.html")
+    assert template.render() == "Themes Brand Base"
 
 
-@override_settings(WAGTAIL_THEME_PATH='themes')
+@override_settings(WAGTAIL_THEME_PATH="themes")
 def test_get_dirs_with_extend():
-    set_theme('brand')
-    template = get_template('page.html')
-    assert template.render() == 'Page - Themes Brand Base'
+    set_theme("brand")
+    template = get_template("page.html")
+    assert template.render() == "Page - Themes Brand Base"
```

